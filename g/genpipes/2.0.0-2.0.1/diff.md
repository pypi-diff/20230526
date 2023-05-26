# Comparing `tmp/genpipes-2.0.0.tar.gz` & `tmp/genpipes-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genpipes-2.0.0.tar", max compression
+gzip compressed data, was "genpipes-2.0.1.tar", max compression
```

## Comparing `genpipes-2.0.0.tar` & `genpipes-2.0.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35149 2023-03-20 13:31:00.120503 genpipes-2.0.0/LICENSE
--rw-r--r--   0        0        0     7765 2023-03-20 13:31:00.120503 genpipes-2.0.0/README.md
--rw-r--r--   0        0        0        1 2023-03-20 15:32:47.530503 genpipes-2.0.0/genpipes/__init__.py
--rw-r--r--   0        0        0     1876 2023-03-20 15:32:47.530503 genpipes-2.0.0/genpipes/compose.py
--rw-r--r--   0        0        0     1258 2023-03-20 15:32:47.530503 genpipes-2.0.0/genpipes/declare.py
--rw-r--r--   0        0        0      505 2023-03-20 15:32:47.530503 genpipes-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     8612 1970-01-01 00:00:00.000000 genpipes-2.0.0/setup.py
--rw-r--r--   0        0        0     8293 1970-01-01 00:00:00.000000 genpipes-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-03-20 13:31:00.120503 genpipes-2.0.1/LICENSE
+-rw-r--r--   0        0        0     7765 2023-03-20 13:31:00.120503 genpipes-2.0.1/README.md
+-rw-r--r--   0        0        0        1 2023-03-20 15:32:47.530503 genpipes-2.0.1/genpipes/__init__.py
+-rw-r--r--   0        0        0     1876 2023-03-20 15:32:47.530503 genpipes-2.0.1/genpipes/compose.py
+-rw-r--r--   0        0        0     1258 2023-03-20 15:32:47.530503 genpipes-2.0.1/genpipes/declare.py
+-rw-r--r--   0        0        0      504 2023-05-26 12:38:48.257881 genpipes-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     8612 1970-01-01 00:00:00.000000 genpipes-2.0.1/setup.py
+-rw-r--r--   0        0        0     8343 1970-01-01 00:00:00.000000 genpipes-2.0.1/PKG-INFO
```

### Comparing `genpipes-2.0.0/LICENSE` & `genpipes-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `genpipes-2.0.0/README.md` & `genpipes-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `genpipes-2.0.0/genpipes/compose.py` & `genpipes-2.0.1/genpipes/compose.py`

 * *Files identical despite different names*

### Comparing `genpipes-2.0.0/genpipes/declare.py` & `genpipes-2.0.1/genpipes/declare.py`

 * *Files identical despite different names*

### Comparing `genpipes-2.0.0/setup.py` & `genpipes-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 ['genpipes']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'genpipes',
-    'version': '2.0.0',
+    'version': '2.0.1',
     'description': 'Simple library to compose pipeline in the sklearn way thanks to generators',
     'long_description': '![alt](https://img.shields.io/github/workflow/status/Mg30/genpipes/genpipes-tests)\n[![Downloads](https://pepy.tech/badge/genpipes)](https://pepy.tech/project/genpipes)\n# Genpipes\nLibrary to write readable and reproductible pipelines using decorators and generators.\nTested for Python > 3.6.9.\n\n## Installation\n`pip install genpipes`\n\n## Usage\n\nBelow some use case on how to use the library.\n### Quick Start\n\nThis quick start assume that you have pandas installed as dependency in you project.\n\n```python\n\nimport pandas as pd\nfrom genpipes import declare, compose\nfrom collections.abc import Iterable\n\n@declare.generator()\ndef data_to_be_processed(path:str) -> pd.DataFrame:\n    df = pd.read_csv(path)\n    return df\n\n\n@declare.processor(inputs=["col1"])\ndef filter_by(stream: Iterable[pd.DataFrame], col_to_filter:str, value:str):\n    for df in stream:\n        dff = df[df[col_to_filter] == value]\n        yield dff\n\npipe = compose.Pipeline(steps=[\n    ("fetching datasource from some csv file", data_to_be_processed, {}),\n    ("performing some filtering based on col1", filter_by, {"value": "some_value"} )\n])\n\noutput = pipe.run()\n```\n\n### Declaring a data source\nThe first task in data processing is usally to write code to acquire data. The library provide a decorator to declare your data source so they can be easily shared and readable.\n\nThe decorators take in a list of inputs to be passed as positional arguments to the decorated function. This way you are binding arguments to the function but you are not hardcoding arguments inside the function.\n\n```python\n# my_datasource.py\nimport pandas as pd\nfrom genpipes import declare\n\n@declare.generator(inputs=["some_file.csv"])\ndef data_to_be_processed(path:str) -> pd.DataFrame:\n    df = pd.read_csv(path)\n    return df\n\n# other_file.py\nfrom my_datasource import data_to_be_processed\n\ndf = data_to_be_processed()\n```\n\nHowever if you want to let some arguments be defined later you could use keywords arguments like so :\n\n```python\n# my_datasource.py\nimport pandas as pd\nfrom genpipes import declare\n\n@declare.generator(inputs=["some_file.csv"])\ndef data_to_be_processed(path:str, read_options:dict) -> pd.DataFrame:\n    df = pd.read_csv(path, **read_options)\n    return df\n\n# other_file.py\nfrom my_datasource import data_to_be_processed\n\ndf = data_to_be_processed(read_options={"encoding":"latin1"})\n\n```\n\n### Declaring generator\n\n`generator` decorator is use to initialize a stream.  **Function decorated are transformed to a Python generator object**. You can decorate any function like a `@generator`.\n\n```python\n\nimport pandas as pd\nfrom genpipes import declare, compose\n\n@declare.generator(inputs=["some_file.csv"])\ndef data_to_be_processed(path:str) -> pd.DataFrame:\n    df = pd.read_csv(path)\n    return df\n```\n\nOr a more complexe function\n\n```python\nimport pandas as pd\nfrom genpipes import declare, compose\n\n@declare.generator(inputs=["some_file.csv"])\ndef data_one(path:str) -> pd.DataFrame:\n    df = pd.read_csv(path)\n    return df\n\n@declare.generator(inputs=["some_file_bis.csv"])\ndef data_two(path:str) -> pd.DataFrame:\n    df = pd.read_csv(path)\n    return df\n\n\n@declare.generator(inputs=[data_one, data_two])\ndef merging_data(input_one:Callable, input_two:Callable) -> pd.DataFrame:\n    df_one = input_one()\n    df_two = input_two()\n    df_merged = df_one.merge(df_two, on="key")\n    return df_merged\n\n```\nDecorated function will not received the value from the stream. But the wrapper does receive the value from stream and push it downstream unchanged. \n\nThat\'s why when calling  your function once decorated you have to pass it as first argument a generator object, so if you want to test you function you can do like that:\n```python\n\nempty_stream = () # use to feed the generator decorated function\n\ngen = merging_data(empty_stream)\n\ndf_merge = next(gen)# consumming merging_data\n\n```\nBecause the decorator returns a function that create a generator object you can create many generator object and feed several consumers.\n\n```python\nempty_stream = () # use to feed the generator decorated function\n\ngen_one = merging_data(empty_stream)\ngen_two = merging_data(empty_stream)\n\n# multiple consuming\nconsumer_one = next(gen_one)\nconsumer_two = next(gen_two)\n\nassert consumer_one.equals(consumer_two) # True\n```\n\n\n### Declaring processing functions\n\nNow that we have seen how to declare data sources and how to generate a stream thanks to generator decorator. Let\'s see how to declare processing functions.\n\n```python\nimport pandas as pd\nfrom genpipes import declare, compose\n\n@declare.generator(inputs=["some_file.csv"])\ndef data_one(path:str) -> pd.DataFrame:\n    df = pd.read_csv(path)\n    return df\n\n@declare.generator(inputs=["some_file_bis.csv"])\ndef data_two(path:str) -> pd.DataFrame:\n    df = pd.read_csv(path)\n    return df\n\n\n@declare.generator(inputs=[data_one, data_two])\ndef merging_data(input_one:Callable, input_two:Callable) -> pd.DataFrame:\n    df_one = input_one()\n    df_two = input_two()\n    df_merged = df_one.merge(df_two, on="key")\n    return df_merged\n\n@declare.processor(inputs=[["col1, col2"]])\ndef deduplicate(stream:Iterable[pd.DataFrame], subset:List):\n    for df in stream:\n        df_nodup = df[~df.duplicated(subset=[subset])]\n        yield df_nodup\n\n```\n As you can see, `processor` decorated function **MUST BE** a generator function that take as first argument a generator that represent the stream of values.\n\n ### Composing pipelines\n\n Even if we can use the decorator helper function alone, the library provide a `Pipeline` class that help to assemble functions decorated with both `generator` and `processor`.\n\n A pipeline object is compose of steps that are `tuple` with 3 components:  \n 1- The description of the step  \n 2- The decorated function  \n 3- The keywords arguments to forward as dict, if none then empty dict\n\n ```python\nimport pandas as pd\nfrom genpipes import compose, declare\n\n@declare.generator(inputs=["some_file.csv"])\ndef data_one(path:str) -> pd.DataFrame:\n    df = pd.read_csv(path)\n    return df\n\n@declare.generator(inputs=["some_file_bis.csv"])\ndef data_two(path:str) -> pd.DataFrame:\n    df = pd.read_csv(path)\n    return df\n\n@declare.generator(inputs=[data_one, data_two])\ndef merging_data(input_one:Callable, input_two:Callable) -> pd.DataFrame:\n    df_one = input_one()\n    df_two = input_two()\n    df_merged = df_one.merge(df_two, on="key")\n    return df_merged\n\n@declare.processor()\ndef deduplicate(stream:Iterable[pd.DataFrame], subset:List):\n    for df in stream:\n        df_nodup = df[~df.duplicated(subset=[subset])]\n        yield df_nodup\n\n\npipe = compose.Pipeline(\n    steps=[\n        ("data source is the merging of data one and data two",merging_data,{}) # empty dict use here as there is no kwargs,\n        ("droping dups",deduplicate, {"subset": ["col1"]} ) # forwarding subset as kwarg\n    ]\n)\n```\nWhen declaring pipeline objects we are not evaluating them. For that we need to call the `run` method. The `run` method return the last object pulled out from the stream. In our case it will be the dedup dataframe from the last step.\n\n``` python\ndedup_df = pipe.run()\n```\nWe can run the pipeline multiple time, it will re do all the steps:\n\n``` python\ndedup_df = pipe.run()\ndedup_df_bis = pipe.run()\nassert dedup_df.equals(dedup_df_bis) # True\n```\n\npipeline objects can be used in other pipeline instance as a step:\n\n``` python\n@declare.processor()\ndef filtering_df(stream:Iterable[pd.DataFrame]):\n    for df in stream:\n        dff = df.filter("some expr")\n        yield dff\n\nother_pipe = compose.Pipeline(steps=[\n    ("take input other pipeline instance",pipe, {} ),\n    ("filtering the output of the first pipe", filtering_df, {})\n])\n\noutput_from_second_pipe = other_pipe.run() # will run the first pipe instance\n\n```\n',
     'author': 'Matt G.',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Mg30/genpipes',
     'packages': packages,
     'package_data': package_data,
-    'python_requires': '>=3.8.1,<4.0.0',
+    'python_requires': '>=3.8.0,<4.0.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `genpipes-2.0.0/PKG-INFO` & `genpipes-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: genpipes
-Version: 2.0.0
+Version: 2.0.1
 Summary: Simple library to compose pipeline in the sklearn way thanks to generators
 Home-page: https://github.com/Mg30/genpipes
 Author: Matt G.
-Requires-Python: >=3.8.1,<4.0.0
+Requires-Python: >=3.8.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Project-URL: Repository, https://github.com/Mg30/genpipes
 Description-Content-Type: text/markdown
 
 ![alt](https://img.shields.io/github/workflow/status/Mg30/genpipes/genpipes-tests)
```

