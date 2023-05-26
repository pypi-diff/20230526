# Comparing `tmp/dataset-librarian-0.0.0.dev0.tar.gz` & `tmp/dataset_librarian-0.0.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataset-librarian-0.0.0.dev0.tar", last modified: Fri May  5 17:40:47 2023, max compression
+gzip compressed data, was "dataset_librarian-0.0.0.dev1.tar", last modified: Fri May 26 08:30:31 2023, max compression
```

## Comparing `dataset-librarian-0.0.0.dev0.tar` & `dataset_librarian-0.0.0.dev1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-05-05 17:40:47.785416 dataset-librarian-0.0.0.dev0/
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     3890 2023-05-05 17:40:47.781416 dataset-librarian-0.0.0.dev0/PKG-INFO
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     3425 2023-05-05 17:39:12.000000 dataset-librarian-0.0.0.dev0/README.md
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)      673 2023-05-05 17:38:35.000000 dataset-librarian-0.0.0.dev0/pyproject.toml
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)       38 2023-05-05 17:40:47.785416 dataset-librarian-0.0.0.dev0/setup.cfg
-drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-05-05 17:40:47.781416 dataset-librarian-0.0.0.dev0/src/
-drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-05-05 17:40:47.781416 dataset-librarian-0.0.0.dev0/src/dataset_librarian.egg-info/
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     3890 2023-05-05 17:40:47.000000 dataset-librarian-0.0.0.dev0/src/dataset_librarian.egg-info/PKG-INFO
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)      338 2023-05-05 17:40:47.000000 dataset-librarian-0.0.0.dev0/src/dataset_librarian.egg-info/SOURCES.txt
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)        1 2023-05-05 17:40:47.000000 dataset-librarian-0.0.0.dev0/src/dataset_librarian.egg-info/dependency_links.txt
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)       19 2023-05-05 17:40:47.000000 dataset-librarian-0.0.0.dev0/src/dataset_librarian.egg-info/requires.txt
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)        8 2023-05-05 17:40:47.000000 dataset-librarian-0.0.0.dev0/src/dataset_librarian.egg-info/top_level.txt
-drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-05-05 17:40:47.781416 dataset-librarian-0.0.0.dev0/src/package/
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)        0 2023-05-05 17:36:44.000000 dataset-librarian-0.0.0.dev0/src/package/__init__.py
-drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-05-05 17:40:47.781416 dataset-librarian-0.0.0.dev0/src/package/subpackage/
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)        0 2023-05-05 17:36:44.000000 dataset-librarian-0.0.0.dev0/src/package/subpackage/__init__.py
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)       34 2023-05-05 17:36:44.000000 dataset-librarian-0.0.0.dev0/src/package/subpackage/test.py
+drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-05-26 08:30:31.112306 dataset_librarian-0.0.0.dev1/
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     4570 2023-05-26 08:30:31.112306 dataset_librarian-0.0.0.dev1/PKG-INFO
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     4105 2023-05-25 19:30:11.000000 dataset_librarian-0.0.0.dev1/README.md
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)      608 2023-05-26 08:30:22.000000 dataset_librarian-0.0.0.dev1/pyproject.toml
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)       38 2023-05-26 08:30:31.112306 dataset_librarian-0.0.0.dev1/setup.cfg
+drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-05-26 08:30:31.112306 dataset_librarian-0.0.0.dev1/src/
+drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-05-26 08:30:31.112306 dataset_librarian-0.0.0.dev1/src/dataset_librarian/
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)        0 2023-05-05 17:36:44.000000 dataset_librarian-0.0.0.dev1/src/dataset_librarian/__init__.py
+drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-05-26 08:30:31.112306 dataset_librarian-0.0.0.dev1/src/dataset_librarian/subpackage/
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)        0 2023-05-05 17:36:44.000000 dataset_librarian-0.0.0.dev1/src/dataset_librarian/subpackage/__init__.py
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)       34 2023-05-05 17:36:44.000000 dataset_librarian-0.0.0.dev1/src/dataset_librarian/subpackage/test.py
+drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-05-26 08:30:31.112306 dataset_librarian-0.0.0.dev1/src/dataset_librarian.egg-info/
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     4570 2023-05-26 08:30:31.000000 dataset_librarian-0.0.0.dev1/src/dataset_librarian.egg-info/PKG-INFO
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)      368 2023-05-26 08:30:31.000000 dataset_librarian-0.0.0.dev1/src/dataset_librarian.egg-info/SOURCES.txt
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)        1 2023-05-26 08:30:31.000000 dataset_librarian-0.0.0.dev1/src/dataset_librarian.egg-info/dependency_links.txt
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)       16 2023-05-26 08:30:31.000000 dataset_librarian-0.0.0.dev1/src/dataset_librarian.egg-info/requires.txt
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)       18 2023-05-26 08:30:31.000000 dataset_librarian-0.0.0.dev1/src/dataset_librarian.egg-info/top_level.txt
```

### Comparing `dataset-librarian-0.0.0.dev0/PKG-INFO` & `dataset_librarian-0.0.0.dev1/src/dataset_librarian.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,72 +1,88 @@
 Metadata-Version: 2.1
 Name: dataset-librarian
-Version: 0.0.0.dev0
+Version: 0.0.0.dev1
 Summary: Package Placeholder
 Author-email: IntelAI <IntelAI@intel.com>
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: <3.10,>=3.8
 Description-Content-Type: text/markdown
 
 # Dataset API
 
 ## Dataset API structure
 ```
-models/datasets/dataset_api/
-|── dataset.py
-├── dataset_urls.json
+dataset_api
+├── conda
+│   └── recipes
+│       ├── py38_recipe
+│       └── py39_recipe
+├── src
+│   └── dataset_librarian
+│       ├── dataset_api
+│       ├── scripts
+│       ├── __init__.py
+│       ├── dataset.py
+│       ├── datasets_urls.json
+├── MANIFEST.in
 ├── README.md
-├── scripts
-├── setup.sh
-└── dataset_api/
-    ├── __init__.py
-    ├── download.py
-    └── preprocess.py
+├── pyproject.toml
+└── requirements.txt
 ```
 
 ## Environment setup
 Clone the [Model Zoo for Intel® Architecture](https://github.com/IntelAI/models) repository and navigate to the `dataset_api` directory.
-```
-# Optional: create and activate a virtual environment
+
+```bash
+# Step 1 (recommended): Create and activate a virtual environment
+## Option 1: Using virtualenv
 virtualenv -p python3 venv
 . venv/bin/activate
+## Option 2: Using conda
+conda create -n venv python=<3.8 or 3.9> -c conda-forge
+conda activate venv
 
+# Step 2: Installing package
+## Option 1: Installing from source code
 cd models/datasets/dataset_api
-# Install dependencies, some dependencies might require root privilages.
-./setup.sh
+python -m pip install --upgrade pip build setuptools wheel
+python -m pip install .
+## Option 2: Installing from PyPI
+python -m pip install dataset-librarian
 ```
+PyPI package can be found [here](https://pypi.org/project/dataset-librarian/).
 
 ## Datasets
 | Dataset name | Description | Download | Preprocessing | command |
 | ------------ | ----------- | -------- | --------------| ------- |
-| `brca` | [Breast Cancer dataset](https://wiki.cancerimagingarchive.net/pages/viewpage.action?pageId=109379611#10937961150f24f71b869471e8366180549549d75) that contains categorized contrast enhanced mammography data and radiologists’ notes. | supported | **A prerequisite:** Use a browser, download [the Low Energy and Subtracted images](https://faspex.cancerimagingarchive.net/aspera/faspex/external_deliveries/260?passcode=5335d2514638afdaf03237780dcdfec29edf4238#), then provide the path to the directory that contains the downloaded images using `--directory` argument. | `python dataset.py -n brca --download --preprocess -d <path to the dataset directory>` |
-| `tabformer` | [Credit card data](https://ibm.ent.box.com/v/tabformer-data/folder/130748337023) for TabFormer | supported | not supported | `python dataset.py -n tabformer --download` |
-| `dureader-vis` | [DuReader-vis](https://github.com/baidu/DuReader/tree/master/DuReader-vis) for document automation. Chinese Open-domain Document Visual Question Answering (Open-Domain DocVQA) dataset, containing about 15K question-answering pairs and 158K document images from the Baidu search engine. | supported | not supported  | `python dataset.py -n dureader-vis --download` |
-| `msmarco` | [MS MARCO](https://microsoft.github.io/msmarco/)  is a collection of datasets focused on deep learning in search | supported | not supported | `python dataset.py -n msmarco --download` |
-| `mvtec-ad` | [MVTEC Anomaly Detection DATASET](https://www.mvtec.com/company/research/datasets/mvtec-ad) for industrial inspection. It contains over 5000 high-resolution images divided into fifteen different object and texture categories. | supported | supported  | `python dataset.py -n mvtec-ad --download --preprocess -d <path to the dataset directory>` |
+| `brca` | [Breast Cancer dataset](https://wiki.cancerimagingarchive.net/pages/viewpage.action?pageId=109379611#10937961150f24f71b869471e8366180549549d75) that contains categorized contrast enhanced mammography data and radiologists’ notes. | supported | **A prerequisite:** Use a browser, download [the Low Energy and Subtracted images](https://faspex.cancerimagingarchive.net/aspera/faspex/external_deliveries/260?passcode=5335d2514638afdaf03237780dcdfec29edf4238#), then provide the path to the directory that contains the downloaded images using `--directory` argument. | `python -m dataset_librarian.dataset -n brca --download --preprocess -d <path to the dataset directory>` |
+| `tabformer` | [Credit card data](https://ibm.ent.box.com/v/tabformer-data/folder/130748337023) for TabFormer | supported | not supported | `python -m dataset_librarian.dataset -n tabformer --download` |
+| `dureader-vis` | [DuReader-vis](https://github.com/baidu/DuReader/tree/master/DuReader-vis) for document automation. Chinese Open-domain Document Visual Question Answering (Open-Domain DocVQA) dataset, containing about 15K question-answering pairs and 158K document images from the Baidu search engine. | supported | not supported  | `python -m dataset_librarian.dataset -n dureader-vis --download` |
+| `msmarco` | [MS MARCO](https://microsoft.github.io/msmarco/)  is a collection of datasets focused on deep learning in search | supported | not supported | `python -m dataset_librarian.dataset -n msmarco --download` |
+| `mvtec-ad` | [MVTEC Anomaly Detection DATASET](https://www.mvtec.com/company/research/datasets/mvtec-ad) for industrial inspection. It contains over 5000 high-resolution images divided into fifteen different object and texture categories. | supported | supported  | `python -m dataset_librarian.dataset -n mvtec-ad --download --preprocess -d <path to the dataset directory>` |
 
 ## Command-line Interface
 
 | Input Arguments | Description |
 | --------------- | ----------- |
 | --list (-l) | list the supported datasets. |
 | --name (-n) | dataset name |
 | --directory (-d) | directory location where the raw dataset will be saved on your system. It's also where the preprocessed dataset files will be written. If not set, a directory with the dataset name will be created. |
 | --download | download the dataset specified. |
 | --preprocess | preprocess the dataset if supported. |
 
 
 ## Python API
 ```
-from dataset_api.download import download_dataset
-from dataset_api.preprocess import preprocess_dataset
+from dataset_librarian.dataset_api.download import download_dataset
+from dataset_librarian.dataset_api.preprocess import preprocess_dataset
 
 # Download the datasets
 download_dataset('brca', <path to the raw dataset directory>)
 
 # Preprocess the datasets
 preprocess_dataset('brca', <path to the raw dataset directory>)
 ```
```

### Comparing `dataset-librarian-0.0.0.dev0/README.md` & `dataset_librarian-0.0.0.dev1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,88 @@
+Metadata-Version: 2.1
+Name: dataset_librarian
+Version: 0.0.0.dev1
+Summary: Package Placeholder
+Author-email: IntelAI <IntelAI@intel.com>
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Operating System :: OS Independent
+Requires-Python: <3.10,>=3.8
+Description-Content-Type: text/markdown
+
 # Dataset API
 
 ## Dataset API structure
 ```
-models/datasets/dataset_api/
-|── dataset.py
-├── dataset_urls.json
+dataset_api
+├── conda
+│   └── recipes
+│       ├── py38_recipe
+│       └── py39_recipe
+├── src
+│   └── dataset_librarian
+│       ├── dataset_api
+│       ├── scripts
+│       ├── __init__.py
+│       ├── dataset.py
+│       ├── datasets_urls.json
+├── MANIFEST.in
 ├── README.md
-├── scripts
-├── setup.sh
-└── dataset_api/
-    ├── __init__.py
-    ├── download.py
-    └── preprocess.py
+├── pyproject.toml
+└── requirements.txt
 ```
 
 ## Environment setup
 Clone the [Model Zoo for Intel® Architecture](https://github.com/IntelAI/models) repository and navigate to the `dataset_api` directory.
-```
-# Optional: create and activate a virtual environment
+
+```bash
+# Step 1 (recommended): Create and activate a virtual environment
+## Option 1: Using virtualenv
 virtualenv -p python3 venv
 . venv/bin/activate
+## Option 2: Using conda
+conda create -n venv python=<3.8 or 3.9> -c conda-forge
+conda activate venv
 
+# Step 2: Installing package
+## Option 1: Installing from source code
 cd models/datasets/dataset_api
-# Install dependencies, some dependencies might require root privilages.
-./setup.sh
+python -m pip install --upgrade pip build setuptools wheel
+python -m pip install .
+## Option 2: Installing from PyPI
+python -m pip install dataset-librarian
 ```
+PyPI package can be found [here](https://pypi.org/project/dataset-librarian/).
 
 ## Datasets
 | Dataset name | Description | Download | Preprocessing | command |
 | ------------ | ----------- | -------- | --------------| ------- |
-| `brca` | [Breast Cancer dataset](https://wiki.cancerimagingarchive.net/pages/viewpage.action?pageId=109379611#10937961150f24f71b869471e8366180549549d75) that contains categorized contrast enhanced mammography data and radiologists’ notes. | supported | **A prerequisite:** Use a browser, download [the Low Energy and Subtracted images](https://faspex.cancerimagingarchive.net/aspera/faspex/external_deliveries/260?passcode=5335d2514638afdaf03237780dcdfec29edf4238#), then provide the path to the directory that contains the downloaded images using `--directory` argument. | `python dataset.py -n brca --download --preprocess -d <path to the dataset directory>` |
-| `tabformer` | [Credit card data](https://ibm.ent.box.com/v/tabformer-data/folder/130748337023) for TabFormer | supported | not supported | `python dataset.py -n tabformer --download` |
-| `dureader-vis` | [DuReader-vis](https://github.com/baidu/DuReader/tree/master/DuReader-vis) for document automation. Chinese Open-domain Document Visual Question Answering (Open-Domain DocVQA) dataset, containing about 15K question-answering pairs and 158K document images from the Baidu search engine. | supported | not supported  | `python dataset.py -n dureader-vis --download` |
-| `msmarco` | [MS MARCO](https://microsoft.github.io/msmarco/)  is a collection of datasets focused on deep learning in search | supported | not supported | `python dataset.py -n msmarco --download` |
-| `mvtec-ad` | [MVTEC Anomaly Detection DATASET](https://www.mvtec.com/company/research/datasets/mvtec-ad) for industrial inspection. It contains over 5000 high-resolution images divided into fifteen different object and texture categories. | supported | supported  | `python dataset.py -n mvtec-ad --download --preprocess -d <path to the dataset directory>` |
+| `brca` | [Breast Cancer dataset](https://wiki.cancerimagingarchive.net/pages/viewpage.action?pageId=109379611#10937961150f24f71b869471e8366180549549d75) that contains categorized contrast enhanced mammography data and radiologists’ notes. | supported | **A prerequisite:** Use a browser, download [the Low Energy and Subtracted images](https://faspex.cancerimagingarchive.net/aspera/faspex/external_deliveries/260?passcode=5335d2514638afdaf03237780dcdfec29edf4238#), then provide the path to the directory that contains the downloaded images using `--directory` argument. | `python -m dataset_librarian.dataset -n brca --download --preprocess -d <path to the dataset directory>` |
+| `tabformer` | [Credit card data](https://ibm.ent.box.com/v/tabformer-data/folder/130748337023) for TabFormer | supported | not supported | `python -m dataset_librarian.dataset -n tabformer --download` |
+| `dureader-vis` | [DuReader-vis](https://github.com/baidu/DuReader/tree/master/DuReader-vis) for document automation. Chinese Open-domain Document Visual Question Answering (Open-Domain DocVQA) dataset, containing about 15K question-answering pairs and 158K document images from the Baidu search engine. | supported | not supported  | `python -m dataset_librarian.dataset -n dureader-vis --download` |
+| `msmarco` | [MS MARCO](https://microsoft.github.io/msmarco/)  is a collection of datasets focused on deep learning in search | supported | not supported | `python -m dataset_librarian.dataset -n msmarco --download` |
+| `mvtec-ad` | [MVTEC Anomaly Detection DATASET](https://www.mvtec.com/company/research/datasets/mvtec-ad) for industrial inspection. It contains over 5000 high-resolution images divided into fifteen different object and texture categories. | supported | supported  | `python -m dataset_librarian.dataset -n mvtec-ad --download --preprocess -d <path to the dataset directory>` |
 
 ## Command-line Interface
 
 | Input Arguments | Description |
 | --------------- | ----------- |
 | --list (-l) | list the supported datasets. |
 | --name (-n) | dataset name |
 | --directory (-d) | directory location where the raw dataset will be saved on your system. It's also where the preprocessed dataset files will be written. If not set, a directory with the dataset name will be created. |
 | --download | download the dataset specified. |
 | --preprocess | preprocess the dataset if supported. |
 
 
 ## Python API
 ```
-from dataset_api.download import download_dataset
-from dataset_api.preprocess import preprocess_dataset
+from dataset_librarian.dataset_api.download import download_dataset
+from dataset_librarian.dataset_api.preprocess import preprocess_dataset
 
 # Download the datasets
 download_dataset('brca', <path to the raw dataset directory>)
 
 # Preprocess the datasets
 preprocess_dataset('brca', <path to the raw dataset directory>)
 ```
```

### Comparing `dataset-librarian-0.0.0.dev0/pyproject.toml` & `dataset_librarian-0.0.0.dev1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,23 @@
-# Check "name" and "requires-python"
-
 [build-system]
 requires = ["setuptools>=61.0", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
-name = "dataset-librarian"
-version = "0.0.0dev0"
+name = "dataset_librarian"
+version = "0.0.0dev1"
 requires-python = ">=3.8,<3.10"
 authors = [
     { name="IntelAI", email="IntelAI@intel.com"}
 ]
 description = "Package Placeholder"
 readme = "README.md"
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Operating System :: OS Independent"
 ]
 dependencies = [
-    # "azureml>=0.2.7",
-    "azure-ai-ml>=1.4.0"
-]
+    "packaging >=23.0"
+]
```

### Comparing `dataset-librarian-0.0.0.dev0/src/dataset_librarian.egg-info/PKG-INFO` & `dataset_librarian-0.0.0.dev1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,72 +1,75 @@
-Metadata-Version: 2.1
-Name: dataset-librarian
-Version: 0.0.0.dev0
-Summary: Package Placeholder
-Author-email: IntelAI <IntelAI@intel.com>
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Operating System :: OS Independent
-Requires-Python: <3.10,>=3.8
-Description-Content-Type: text/markdown
-
 # Dataset API
 
 ## Dataset API structure
 ```
-models/datasets/dataset_api/
-|── dataset.py
-├── dataset_urls.json
+dataset_api
+├── conda
+│   └── recipes
+│       ├── py38_recipe
+│       └── py39_recipe
+├── src
+│   └── dataset_librarian
+│       ├── dataset_api
+│       ├── scripts
+│       ├── __init__.py
+│       ├── dataset.py
+│       ├── datasets_urls.json
+├── MANIFEST.in
 ├── README.md
-├── scripts
-├── setup.sh
-└── dataset_api/
-    ├── __init__.py
-    ├── download.py
-    └── preprocess.py
+├── pyproject.toml
+└── requirements.txt
 ```
 
 ## Environment setup
 Clone the [Model Zoo for Intel® Architecture](https://github.com/IntelAI/models) repository and navigate to the `dataset_api` directory.
-```
-# Optional: create and activate a virtual environment
+
+```bash
+# Step 1 (recommended): Create and activate a virtual environment
+## Option 1: Using virtualenv
 virtualenv -p python3 venv
 . venv/bin/activate
+## Option 2: Using conda
+conda create -n venv python=<3.8 or 3.9> -c conda-forge
+conda activate venv
 
+# Step 2: Installing package
+## Option 1: Installing from source code
 cd models/datasets/dataset_api
-# Install dependencies, some dependencies might require root privilages.
-./setup.sh
+python -m pip install --upgrade pip build setuptools wheel
+python -m pip install .
+## Option 2: Installing from PyPI
+python -m pip install dataset-librarian
 ```
+PyPI package can be found [here](https://pypi.org/project/dataset-librarian/).
 
 ## Datasets
 | Dataset name | Description | Download | Preprocessing | command |
 | ------------ | ----------- | -------- | --------------| ------- |
-| `brca` | [Breast Cancer dataset](https://wiki.cancerimagingarchive.net/pages/viewpage.action?pageId=109379611#10937961150f24f71b869471e8366180549549d75) that contains categorized contrast enhanced mammography data and radiologists’ notes. | supported | **A prerequisite:** Use a browser, download [the Low Energy and Subtracted images](https://faspex.cancerimagingarchive.net/aspera/faspex/external_deliveries/260?passcode=5335d2514638afdaf03237780dcdfec29edf4238#), then provide the path to the directory that contains the downloaded images using `--directory` argument. | `python dataset.py -n brca --download --preprocess -d <path to the dataset directory>` |
-| `tabformer` | [Credit card data](https://ibm.ent.box.com/v/tabformer-data/folder/130748337023) for TabFormer | supported | not supported | `python dataset.py -n tabformer --download` |
-| `dureader-vis` | [DuReader-vis](https://github.com/baidu/DuReader/tree/master/DuReader-vis) for document automation. Chinese Open-domain Document Visual Question Answering (Open-Domain DocVQA) dataset, containing about 15K question-answering pairs and 158K document images from the Baidu search engine. | supported | not supported  | `python dataset.py -n dureader-vis --download` |
-| `msmarco` | [MS MARCO](https://microsoft.github.io/msmarco/)  is a collection of datasets focused on deep learning in search | supported | not supported | `python dataset.py -n msmarco --download` |
-| `mvtec-ad` | [MVTEC Anomaly Detection DATASET](https://www.mvtec.com/company/research/datasets/mvtec-ad) for industrial inspection. It contains over 5000 high-resolution images divided into fifteen different object and texture categories. | supported | supported  | `python dataset.py -n mvtec-ad --download --preprocess -d <path to the dataset directory>` |
+| `brca` | [Breast Cancer dataset](https://wiki.cancerimagingarchive.net/pages/viewpage.action?pageId=109379611#10937961150f24f71b869471e8366180549549d75) that contains categorized contrast enhanced mammography data and radiologists’ notes. | supported | **A prerequisite:** Use a browser, download [the Low Energy and Subtracted images](https://faspex.cancerimagingarchive.net/aspera/faspex/external_deliveries/260?passcode=5335d2514638afdaf03237780dcdfec29edf4238#), then provide the path to the directory that contains the downloaded images using `--directory` argument. | `python -m dataset_librarian.dataset -n brca --download --preprocess -d <path to the dataset directory>` |
+| `tabformer` | [Credit card data](https://ibm.ent.box.com/v/tabformer-data/folder/130748337023) for TabFormer | supported | not supported | `python -m dataset_librarian.dataset -n tabformer --download` |
+| `dureader-vis` | [DuReader-vis](https://github.com/baidu/DuReader/tree/master/DuReader-vis) for document automation. Chinese Open-domain Document Visual Question Answering (Open-Domain DocVQA) dataset, containing about 15K question-answering pairs and 158K document images from the Baidu search engine. | supported | not supported  | `python -m dataset_librarian.dataset -n dureader-vis --download` |
+| `msmarco` | [MS MARCO](https://microsoft.github.io/msmarco/)  is a collection of datasets focused on deep learning in search | supported | not supported | `python -m dataset_librarian.dataset -n msmarco --download` |
+| `mvtec-ad` | [MVTEC Anomaly Detection DATASET](https://www.mvtec.com/company/research/datasets/mvtec-ad) for industrial inspection. It contains over 5000 high-resolution images divided into fifteen different object and texture categories. | supported | supported  | `python -m dataset_librarian.dataset -n mvtec-ad --download --preprocess -d <path to the dataset directory>` |
 
 ## Command-line Interface
 
 | Input Arguments | Description |
 | --------------- | ----------- |
 | --list (-l) | list the supported datasets. |
 | --name (-n) | dataset name |
 | --directory (-d) | directory location where the raw dataset will be saved on your system. It's also where the preprocessed dataset files will be written. If not set, a directory with the dataset name will be created. |
 | --download | download the dataset specified. |
 | --preprocess | preprocess the dataset if supported. |
 
 
 ## Python API
 ```
-from dataset_api.download import download_dataset
-from dataset_api.preprocess import preprocess_dataset
+from dataset_librarian.dataset_api.download import download_dataset
+from dataset_librarian.dataset_api.preprocess import preprocess_dataset
 
 # Download the datasets
 download_dataset('brca', <path to the raw dataset directory>)
 
 # Preprocess the datasets
 preprocess_dataset('brca', <path to the raw dataset directory>)
 ```
```

