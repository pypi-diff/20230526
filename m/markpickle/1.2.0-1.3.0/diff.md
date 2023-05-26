# Comparing `tmp/markpickle-1.2.0.tar.gz` & `tmp/markpickle-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markpickle-1.2.0.tar", max compression
+gzip compressed data, was "markpickle-1.3.0.tar", max compression
```

## Comparing `markpickle-1.2.0.tar` & `markpickle-1.3.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0     1071 2023-03-13 16:01:29.095278 markpickle-1.2.0/LICENSE
--rw-r--r--   0        0        0      520 2023-03-25 02:59:54.639724 markpickle-1.2.0/markpickle/__init__.py
--rw-r--r--   0        0        0     1543 2023-05-13 21:17:46.471801 markpickle-1.2.0/markpickle/binary_streams.py
--rw-r--r--   0        0        0     2298 2023-05-13 21:17:46.474842 markpickle-1.2.0/markpickle/config_class.py
--rw-r--r--   0        0        0    11510 2023-05-13 21:06:47.467612 markpickle-1.2.0/markpickle/deserialize.py
--rw-r--r--   0        0        0      890 2023-05-13 21:06:43.777843 markpickle-1.2.0/markpickle/import_string.py
--rw-r--r--   0        0        0      359 2023-03-25 02:20:40.183215 markpickle-1.2.0/markpickle/meta.py
--rw-r--r--   0        0        0      568 2023-03-19 01:38:27.019163 markpickle-1.2.0/markpickle/mypy_types.py
--rw-r--r--   0        0        0       80 2023-01-30 03:12:57.741220 markpickle-1.2.0/markpickle/py.typed
--rw-r--r--   0        0        0     4817 2023-03-19 15:40:41.780446 markpickle-1.2.0/markpickle/python_to_tables.py
--rw-r--r--   0        0        0    14695 2023-05-13 21:17:51.391118 markpickle-1.2.0/markpickle/serialize.py
--rw-r--r--   0        0        0      737 2023-03-19 15:41:53.757488 markpickle-1.2.0/markpickle/simplify_types.py
--rw-r--r--   0        0        0     1032 2023-03-20 03:05:14.208164 markpickle-1.2.0/markpickle/split_file_code.py
--rw-r--r--   0        0        0     1252 2023-03-19 15:02:17.487053 markpickle-1.2.0/markpickle/third_party_tables.py
--rw-r--r--   0        0        0     1741 2023-05-13 21:06:36.820923 markpickle-1.2.0/markpickle/tool.py
--rw-r--r--   0        0        0     3624 2023-05-13 21:21:21.556492 markpickle-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     5015 2023-05-13 21:21:08.812592 markpickle-1.2.0/README.md
--rw-r--r--   0        0        0     5790 1970-01-01 00:00:00.000000 markpickle-1.2.0/setup.py
--rw-r--r--   0        0        0     6580 1970-01-01 00:00:00.000000 markpickle-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-26 20:14:01.644909 markpickle-1.3.0/LICENSE
+-rw-r--r--   0        0        0     5763 2023-05-26 20:16:03.084691 markpickle-1.3.0/README.md
+-rw-r--r--   0        0        0      574 2023-05-26 20:14:01.648909 markpickle-1.3.0/markpickle/__init__.py
+-rw-r--r--   0        0        0     1225 2023-05-26 20:14:01.648909 markpickle-1.3.0/markpickle/__main__.py
+-rw-r--r--   0        0        0     1543 2023-05-26 20:14:01.648909 markpickle-1.3.0/markpickle/binary_streams.py
+-rw-r--r--   0        0        0       57 2023-05-26 20:14:01.648909 markpickle-1.3.0/markpickle/cli.py
+-rw-r--r--   0        0        0     2298 2023-05-26 20:14:01.648909 markpickle-1.3.0/markpickle/config_class.py
+-rw-r--r--   0        0        0    11510 2023-05-26 20:14:01.648909 markpickle-1.3.0/markpickle/deserialize.py
+-rw-r--r--   0        0        0      359 2023-05-26 20:14:01.648909 markpickle-1.3.0/markpickle/meta.py
+-rw-r--r--   0        0        0      568 2023-05-26 20:14:01.648909 markpickle-1.3.0/markpickle/mypy_types.py
+-rw-r--r--   0        0        0       80 2023-05-26 20:14:01.648909 markpickle-1.3.0/markpickle/py.typed
+-rw-r--r--   0        0        0     4817 2023-05-26 20:14:01.648909 markpickle-1.3.0/markpickle/python_to_tables.py
+-rw-r--r--   0        0        0    14695 2023-05-26 20:14:01.648909 markpickle-1.3.0/markpickle/serialize.py
+-rw-r--r--   0        0        0      737 2023-05-26 20:14:01.648909 markpickle-1.3.0/markpickle/simplify_types.py
+-rw-r--r--   0        0        0     1032 2023-05-26 20:14:01.648909 markpickle-1.3.0/markpickle/split_file_code.py
+-rw-r--r--   0        0        0     1252 2023-05-26 20:14:01.648909 markpickle-1.3.0/markpickle/third_party_tables.py
+-rw-r--r--   0        0        0     1741 2023-05-26 20:14:01.648909 markpickle-1.3.0/markpickle/tool.py
+-rw-r--r--   0        0        0      762 2023-05-26 20:14:01.648909 markpickle-1.3.0/markpickle/unicode_formatting.py
+-rw-r--r--   0        0        0     3624 2023-05-26 20:14:01.648909 markpickle-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7278 1970-01-01 00:00:00.000000 markpickle-1.3.0/PKG-INFO
```

### Comparing `markpickle-1.2.0/LICENSE` & `markpickle-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `markpickle-1.2.0/markpickle/__init__.py` & `markpickle-1.3.0/markpickle/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,8 +4,19 @@
 Will not be able to meaningfully serialize all Markdown to a sensible python type.
 """
 from markpickle.config_class import Config
 from markpickle.deserialize import load, load_all, loads, loads_all
 from markpickle.serialize import dump, dump_all, dumps, dumps_all
 from markpickle.split_file_code import split_file
 
-__all__ = ["load", "load_all", "loads", "loads_all", "dump", "dump_all", "dumps", "dumps_all", "Config", "split_file"]
+__all__ = [
+    "load",
+    "load_all",
+    "loads",
+    "loads_all",
+    "dump",
+    "dump_all",
+    "dumps",
+    "dumps_all",
+    "Config",
+    "split_file",
+]
```

### Comparing `markpickle-1.2.0/markpickle/binary_streams.py` & `markpickle-1.3.0/markpickle/binary_streams.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.2.0/markpickle/config_class.py` & `markpickle-1.3.0/markpickle/config_class.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.2.0/markpickle/deserialize.py` & `markpickle-1.3.0/markpickle/deserialize.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.2.0/markpickle/mypy_types.py` & `markpickle-1.3.0/markpickle/mypy_types.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.2.0/markpickle/python_to_tables.py` & `markpickle-1.3.0/markpickle/python_to_tables.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.2.0/markpickle/serialize.py` & `markpickle-1.3.0/markpickle/serialize.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.2.0/markpickle/simplify_types.py` & `markpickle-1.3.0/markpickle/simplify_types.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.2.0/markpickle/split_file_code.py` & `markpickle-1.3.0/markpickle/split_file_code.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.2.0/markpickle/third_party_tables.py` & `markpickle-1.3.0/markpickle/third_party_tables.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.2.0/markpickle/tool.py` & `markpickle-1.3.0/markpickle/tool.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.2.0/pyproject.toml` & `markpickle-1.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "markpickle"
-version = "1.2.0"
+version = "1.3.0"
 description = "Lossy python to markdown serializer"
 authors = ["Matthew Martin <matthewdeanmartin@gmail.com>"]
 keywords = ["serializer", "deserializer", "markdown",]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
```

### Comparing `markpickle-1.2.0/README.md` & `markpickle-1.3.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -63,19 +63,27 @@
 
 ### Round Tripping
 
 Some but not all data structures will be round-trippable. The goal is that the sort of dicts you get from loading JSON will be round-trippable, provided everything is a string.
 
 ### Splitting Files
 
-## If typical serialization scenarios, many json files might be written to a single file, or in the case of yaml, you can put multiple documents into one file separated by `---`. markpickle can treat the horizontal rule as a document spliter if you use `split_file`. It works like [splitstream](https://github.com/rickardp/splitstream), but less efficiently.
+If typical serialization scenarios, many json files might be written to a single file, or in the case of yaml, you can put multiple documents into one file separated by `---`. markpickle can treat the horizontal rule as a document spliter if you use `split_file`. It works like [splitstream](https://github.com/rickardp/splitstream), but less efficiently.
+
+## CLI
+
+This command will take a deserializable markdown file and output json.
+
+```bash
+python -m markpickle "docs/individual/list of scalars.md"
+```
 
 ## Prior Art
 
-## People normally want to convert json to markdown. Json looks like python dict, so if you can do that you can probably do both.
+People normally want to convert json to markdown. Json looks like python dict, so if you can do that you can probably do both.
 
 ### Serializing to Markdown
 
 [json2md](https://github.com/IonicaBizau/json2md), a node package, will turn json that looks like the HTML document object model into markdown, e.g.
 
 ```python
 {"h1": "Some Header",
@@ -84,23 +92,33 @@
 
 [tomark](https://pypi.org/project/tomark/) will turn dict into a markdown table. Unmaintained.
 
 [pytablewriter](https://pytablewriter.readthedocs.io/en/latest/pages/reference/writers/text/markup/md.html) also, dict to table, but supports many tabular formats.
 
 ### Deserializing to Python
 
-I don't know of any libraries that turn markdown into basic python types. At the moment, they all turn markdown into document object model.
+Most libraries turn markdown into document object model. Markdown-to-json is the most similar to markpickle's goal of turning a markdown document into a python data types, in this case nested dicts.
+
+[markdown-to-json](https://github.com/njvack/markdown-to-json)
 
 [mistune](https://pypi.org/project/mistune/) will turn markdown into an Abstract Syntax Tree. The AST is faithful representation of the Markdown, including concepts that have no semantic equivalent to python datatypes.
 
 ## [beautifulsoup](https://www.crummy.com/software/BeautifulSoup/bs4/doc/) will let you navigate the HTML DOM. So you can turn the markdown into HTML, then parse with Beautiful Soup.
 
+## Schema Validation for Markdown
+
+In the case of a serialization library, you'd want something that would indicate if your markdown file will successfully deserialize back into python.
+
+I haven't really found anything that says, for example, "This markdown document shall have one # Header and a 3 column table and nothing else."
+
+- [schema-markdown-js](https://craigahobbs.github.io/schema-markdown-js/language/) A json schema that happens to be using markdown as its syntax.
+
 ## Documentation
 
 - [Examples](https://github.com/matthewdeanmartin/markpickle/blob/main/docs/examples.md)
 - [TODO](https://github.com/matthewdeanmartin/markpickle/blob/main/docs/TODO.md)
 - [People solving similar problems on StackOverflow](https://github.com/matthewdeanmartin/markpickle/blob/main/docs/stackoverflow.md)
 
-
 ## Change Log
+
 - 1.1.0 - Basic functionality. See [examples](https://github.com/matthewdeanmartin/markpickle/blob/main/docs/examples.md) for what is supported.
-- 1.2.0 - Add support for binary data, which is serialized as images with data URLs.
+- 1.2.0 - Add support for binary data, which is serialized as images with data URLs.
```

### Comparing `markpickle-1.2.0/PKG-INFO` & `markpickle-1.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markpickle
-Version: 1.2.0
+Version: 1.3.0
 Summary: Lossy python to markdown serializer
 Home-page: https://github.com/matthewdeanmartin/markpickle
 License: MIT
 Keywords: serializer,deserializer,markdown
 Author: Matthew Martin
 Author-email: matthewdeanmartin@gmail.com
 Classifier: Development Status :: 3 - Alpha
@@ -19,15 +19,14 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.6
 Requires-Dist: mdformat
 Requires-Dist: mistune
 Requires-Dist: pillow
 Requires-Dist: tabulate
 Project-URL: Bug Tracker, https://github.com/matthewdeanmartin/markpickle/issues
 Project-URL: Change Log, https://github.com/matthewdeanmartin/markpickle/blob/main/CHANGES.md
 Project-URL: Documentation, https://github.com/matthewdeanmartin/markpickle
@@ -99,19 +98,27 @@
 
 ### Round Tripping
 
 Some but not all data structures will be round-trippable. The goal is that the sort of dicts you get from loading JSON will be round-trippable, provided everything is a string.
 
 ### Splitting Files
 
-## If typical serialization scenarios, many json files might be written to a single file, or in the case of yaml, you can put multiple documents into one file separated by `---`. markpickle can treat the horizontal rule as a document spliter if you use `split_file`. It works like [splitstream](https://github.com/rickardp/splitstream), but less efficiently.
+If typical serialization scenarios, many json files might be written to a single file, or in the case of yaml, you can put multiple documents into one file separated by `---`. markpickle can treat the horizontal rule as a document spliter if you use `split_file`. It works like [splitstream](https://github.com/rickardp/splitstream), but less efficiently.
+
+## CLI
+
+This command will take a deserializable markdown file and output json.
+
+```bash
+python -m markpickle "docs/individual/list of scalars.md"
+```
 
 ## Prior Art
 
-## People normally want to convert json to markdown. Json looks like python dict, so if you can do that you can probably do both.
+People normally want to convert json to markdown. Json looks like python dict, so if you can do that you can probably do both.
 
 ### Serializing to Markdown
 
 [json2md](https://github.com/IonicaBizau/json2md), a node package, will turn json that looks like the HTML document object model into markdown, e.g.
 
 ```python
 {"h1": "Some Header",
@@ -120,23 +127,34 @@
 
 [tomark](https://pypi.org/project/tomark/) will turn dict into a markdown table. Unmaintained.
 
 [pytablewriter](https://pytablewriter.readthedocs.io/en/latest/pages/reference/writers/text/markup/md.html) also, dict to table, but supports many tabular formats.
 
 ### Deserializing to Python
 
-I don't know of any libraries that turn markdown into basic python types. At the moment, they all turn markdown into document object model.
+Most libraries turn markdown into document object model. Markdown-to-json is the most similar to markpickle's goal of turning a markdown document into a python data types, in this case nested dicts.
+
+[markdown-to-json](https://github.com/njvack/markdown-to-json)
 
 [mistune](https://pypi.org/project/mistune/) will turn markdown into an Abstract Syntax Tree. The AST is faithful representation of the Markdown, including concepts that have no semantic equivalent to python datatypes.
 
 ## [beautifulsoup](https://www.crummy.com/software/BeautifulSoup/bs4/doc/) will let you navigate the HTML DOM. So you can turn the markdown into HTML, then parse with Beautiful Soup.
 
+## Schema Validation for Markdown
+
+In the case of a serialization library, you'd want something that would indicate if your markdown file will successfully deserialize back into python.
+
+I haven't really found anything that says, for example, "This markdown document shall have one # Header and a 3 column table and nothing else."
+
+- [schema-markdown-js](https://craigahobbs.github.io/schema-markdown-js/language/) A json schema that happens to be using markdown as its syntax.
+
 ## Documentation
 
 - [Examples](https://github.com/matthewdeanmartin/markpickle/blob/main/docs/examples.md)
 - [TODO](https://github.com/matthewdeanmartin/markpickle/blob/main/docs/TODO.md)
 - [People solving similar problems on StackOverflow](https://github.com/matthewdeanmartin/markpickle/blob/main/docs/stackoverflow.md)
 
-
 ## Change Log
+
 - 1.1.0 - Basic functionality. See [examples](https://github.com/matthewdeanmartin/markpickle/blob/main/docs/examples.md) for what is supported.
 - 1.2.0 - Add support for binary data, which is serialized as images with data URLs.
+
```

