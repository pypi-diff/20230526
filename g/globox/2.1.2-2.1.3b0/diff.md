# Comparing `tmp/globox-2.1.2.tar.gz` & `tmp/globox-2.1.3b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globox-2.1.2.tar", last modified: Mon May  8 17:04:46 2023, max compression
+gzip compressed data, was "globox-2.1.3b0.tar", max compression
```

## Comparing `globox-2.1.2.tar` & `globox-2.1.3b0.tar`

### file list

```diff
@@ -1,38 +1,16 @@
-drwxr-xr-x   0 louislac   (501) staff       (20)        0 2023-05-08 17:04:46.766928 globox-2.1.2/
--rw-r--r--   0 louislac   (501) staff       (20)     1048 2022-09-12 14:17:20.000000 globox-2.1.2/LICENCE
--rw-r--r--   0 louislac   (501) staff       (20)    10259 2023-05-08 17:04:46.766661 globox-2.1.2/PKG-INFO
--rw-r--r--   0 louislac   (501) staff       (20)     9461 2023-05-04 12:47:54.000000 globox-2.1.2/README.md
--rw-r--r--   0 louislac   (501) staff       (20)       80 2022-10-03 20:55:21.000000 globox-2.1.2/pyproject.toml
--rw-r--r--   0 louislac   (501) staff       (20)       38 2023-05-08 17:04:46.767027 globox-2.1.2/setup.cfg
--rw-r--r--   0 louislac   (501) staff       (20)     1745 2023-04-27 15:10:15.000000 globox-2.1.2/setup.py
-drwxr-xr-x   0 louislac   (501) staff       (20)        0 2023-05-08 17:04:46.759871 globox-2.1.2/src/
-drwxr-xr-x   0 louislac   (501) staff       (20)        0 2023-05-08 17:04:46.764236 globox-2.1.2/src/globox/
--rw-r--r--   0 louislac   (501) staff       (20)      273 2023-04-27 15:10:15.000000 globox-2.1.2/src/globox/__init__.py
--rw-r--r--   0 louislac   (501) staff       (20)       30 2022-10-26 18:29:42.000000 globox-2.1.2/src/globox/__main__.py
--rw-r--r--   0 louislac   (501) staff       (20)       63 2023-05-08 17:03:33.000000 globox-2.1.2/src/globox/__version__.py
--rw-r--r--   0 louislac   (501) staff       (20)    18551 2023-04-27 15:10:15.000000 globox-2.1.2/src/globox/annotation.py
--rw-r--r--   0 louislac   (501) staff       (20)    33312 2023-05-08 17:02:15.000000 globox-2.1.2/src/globox/annotationset.py
--rw-r--r--   0 louislac   (501) staff       (20)     1015 2023-04-27 15:10:15.000000 globox-2.1.2/src/globox/atomic.py
--rw-r--r--   0 louislac   (501) staff       (20)    17250 2023-04-27 15:10:15.000000 globox-2.1.2/src/globox/boundingbox.py
--rw-r--r--   0 louislac   (501) staff       (20)    14247 2023-04-27 15:10:15.000000 globox-2.1.2/src/globox/cli.py
--rw-r--r--   0 louislac   (501) staff       (20)      539 2023-04-27 15:10:15.000000 globox-2.1.2/src/globox/errors.py
--rw-r--r--   0 louislac   (501) staff       (20)    21347 2023-04-27 15:10:15.000000 globox-2.1.2/src/globox/evaluation.py
--rw-r--r--   0 louislac   (501) staff       (20)      699 2023-04-27 15:10:15.000000 globox-2.1.2/src/globox/file_utils.py
--rw-r--r--   0 louislac   (501) staff       (20)     6983 2023-04-27 15:10:15.000000 globox-2.1.2/src/globox/image_utils.py
--rw-r--r--   0 louislac   (501) staff       (20)      880 2023-04-27 15:10:15.000000 globox-2.1.2/src/globox/thread_utils.py
--rw-r--r--   0 louislac   (501) staff       (20)      747 2023-04-27 15:10:15.000000 globox-2.1.2/src/globox/utils.py
-drwxr-xr-x   0 louislac   (501) staff       (20)        0 2023-05-08 17:04:46.765227 globox-2.1.2/src/globox.egg-info/
--rw-r--r--   0 louislac   (501) staff       (20)    10259 2023-05-08 17:04:46.000000 globox-2.1.2/src/globox.egg-info/PKG-INFO
--rw-r--r--   0 louislac   (501) staff       (20)      755 2023-05-08 17:04:46.000000 globox-2.1.2/src/globox.egg-info/SOURCES.txt
--rw-r--r--   0 louislac   (501) staff       (20)        1 2023-05-08 17:04:46.000000 globox-2.1.2/src/globox.egg-info/dependency_links.txt
--rw-r--r--   0 louislac   (501) staff       (20)       43 2023-05-08 17:04:46.000000 globox-2.1.2/src/globox.egg-info/entry_points.txt
--rw-r--r--   0 louislac   (501) staff       (20)       65 2023-05-08 17:04:46.000000 globox-2.1.2/src/globox.egg-info/requires.txt
--rw-r--r--   0 louislac   (501) staff       (20)        7 2023-05-08 17:04:46.000000 globox-2.1.2/src/globox.egg-info/top_level.txt
-drwxr-xr-x   0 louislac   (501) staff       (20)        0 2023-05-08 17:04:46.766427 globox-2.1.2/tests/
--rw-r--r--   0 louislac   (501) staff       (20)     7607 2023-04-27 15:10:15.000000 globox-2.1.2/tests/test_annotation.py
--rw-r--r--   0 louislac   (501) staff       (20)     8505 2023-04-27 15:10:15.000000 globox-2.1.2/tests/test_annotationset.py
--rw-r--r--   0 louislac   (501) staff       (20)     7846 2023-04-27 15:10:15.000000 globox-2.1.2/tests/test_bbox.py
--rw-r--r--   0 louislac   (501) staff       (20)     5168 2023-04-27 15:10:15.000000 globox-2.1.2/tests/test_coco_evaluation.py
--rw-r--r--   0 louislac   (501) staff       (20)     2151 2023-04-27 15:10:15.000000 globox-2.1.2/tests/test_conversion.py
--rw-r--r--   0 louislac   (501) staff       (20)      226 2023-04-27 15:10:15.000000 globox-2.1.2/tests/test_evaluation.py
--rw-r--r--   0 louislac   (501) staff       (20)     2867 2023-04-27 15:10:15.000000 globox-2.1.2/tests/test_parsing.py
+-rw-r--r--   0        0        0     9236 2023-05-26 20:44:52.964782 globox-2.1.3b0/README.md
+-rw-r--r--   0        0        0     1042 2023-05-26 20:44:52.964782 globox-2.1.3b0/pyproject.toml
+-rw-r--r--   0        0        0      273 2023-05-26 20:44:52.968782 globox-2.1.3b0/src/globox/__init__.py
+-rw-r--r--   0        0        0       30 2023-05-26 20:44:52.968782 globox-2.1.3b0/src/globox/__main__.py
+-rw-r--r--   0        0        0    18551 2023-05-26 20:44:52.968782 globox-2.1.3b0/src/globox/annotation.py
+-rw-r--r--   0        0        0    33312 2023-05-26 20:44:52.968782 globox-2.1.3b0/src/globox/annotationset.py
+-rw-r--r--   0        0        0     1015 2023-05-26 20:44:52.968782 globox-2.1.3b0/src/globox/atomic.py
+-rw-r--r--   0        0        0    17250 2023-05-26 20:44:52.968782 globox-2.1.3b0/src/globox/boundingbox.py
+-rw-r--r--   0        0        0    14247 2023-05-26 20:44:52.968782 globox-2.1.3b0/src/globox/cli.py
+-rw-r--r--   0        0        0      539 2023-05-26 20:44:52.968782 globox-2.1.3b0/src/globox/errors.py
+-rw-r--r--   0        0        0    21347 2023-05-26 20:44:52.968782 globox-2.1.3b0/src/globox/evaluation.py
+-rw-r--r--   0        0        0      699 2023-05-26 20:44:52.968782 globox-2.1.3b0/src/globox/file_utils.py
+-rw-r--r--   0        0        0     6983 2023-05-26 20:44:52.968782 globox-2.1.3b0/src/globox/image_utils.py
+-rw-r--r--   0        0        0      880 2023-05-26 20:44:52.968782 globox-2.1.3b0/src/globox/thread_utils.py
+-rw-r--r--   0        0        0      747 2023-05-26 20:44:52.968782 globox-2.1.3b0/src/globox/utils.py
+-rw-r--r--   0        0        0    10289 1970-01-01 00:00:00.000000 globox-2.1.3b0/PKG-INFO
```

### Comparing `globox-2.1.2/PKG-INFO` & `globox-2.1.3b0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 Metadata-Version: 2.1
 Name: globox
-Version: 2.1.2
+Version: 2.1.3b0
 Summary: Globox is a package and command line interface to read and convert object detection databases (COCO, YOLO, PascalVOC, LabelMe, CVAT, OpenImage, ...) and evaluate them with COCO and PascalVOC.
 Home-page: https://github.com/laclouis5/globox
-Author: Louis Lac
-Author-email: lac.louis5@gmail.com
 License: MIT
 Keywords: annotation,metrics,object detection,bounding boxes,yolo,openimages,cvat,coco,pascal voc,average precision,mean average precision
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
+Author: Louis Lac
+Author-email: lac.louis5@gmail.com
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: numpy (>=1.24.3,<2.0.0)
+Requires-Dist: rich (>=13.3.5,<14.0.0)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0)
+Project-URL: Repository, https://github.com/laclouis5/globox
 Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENCE
 
 # Globox — Object Detection Toolbox
 
 This framework can:
 
 * parse all kinds of object detection datasets (ImageNet, COCO, YOLO, PascalVOC, OpenImage, CVAT, LabelMe, etc.) and show statistics,
 * convert them to other formats (ImageNet, COCO, YOLO, PascalVOC, OpenImage, CVAT, LabelMe, etc.),
-* and evaluate predictions using standard object detection metrics such as AP@[.5:.05:.95], AP@50, mAP, AR<sub>1</sub>, AR<sub>10</sub>, AR<sub>100</sub>.
+* and evaluate predictions using standard object detection metrics such as $AP_{[.5:.05:.95]}$, $AP_{50}$, $mAP$, $AR_{1}$, $AR_{10}$, $AR_{100}$.
 
 This framework can be used both as a library in your own code and as a command line tool. This tool is designed to be simple to use, fast and correct.
 
 ## Install
 
 You can install the package using pip:
 
@@ -96,15 +100,15 @@
 
 Datasets stats can printed to the console:
 
 ```python
 coco_gts.show_stats()
 ```
 
-```shell
+```text
          Database Stats         
 ┏━━━━━━━━━━━━━┳━━━━━━━━┳━━━━━━━┓
 ┃ Label       ┃ Images ┃ Boxes ┃
 ┡━━━━━━━━━━━━━╇━━━━━━━━╇━━━━━━━┩
 │ aeroplane   │     10 │    15 │
 │ bicycle     │      7 │    14 │
 │ bird        │      4 │     6 │
@@ -175,15 +179,15 @@
 
 ```python
 evaluator.show_summary()
 ```
 
 which outputs:
 
-```shell
+```text
                               COCO Evaluation
 ┏━━━━━━━━━━━┳━━━━━━━━━━┳━━━━━━━━┳...┳━━━━━━━━┳━━━━━━━━┳━━━━━━━━┓
 ┃ Label     ┃ AP 50:95 ┃  AP 50 ┃   ┃   AR S ┃   AR M ┃   AR L ┃
 ┡━━━━━━━━━━━╇━━━━━━━━━━╇━━━━━━━━╇...╇━━━━━━━━╇━━━━━━━━╇━━━━━━━━┩
 │ airplane  │    22.7% │  25.2% │   │   nan% │  90.0% │   0.0% │
 │ apple     │    46.4% │  57.4% │   │  48.5% │   nan% │   nan% │
 │ backpack  │    54.8% │  85.1% │   │ 100.0% │  72.0% │   0.0% │
@@ -257,51 +261,47 @@
 
 ## Run Tests
 
 Clone the repo with its test data:
 
 ```shell
 git clone https://github.com/laclouis5/globox --recurse-submodules=tests/globox_test_data
+cd globox
 ```
 
-Install developement dependencies (virtual env recommended):
+Install with Poetry:
 
 ```shell
-pip install -e ".[dev]"
+poetry install
 ```
 
-Run tox:
+Run the tests:
 
 ```shell
-tox
+poetry run pytest
 ```
 
 ## Speed Banchmarks
 
-<details>
-<summary>Click to expand</summary>
-
 Speed benchmark can be executed with:
 
 ```shell
-python3 tests/benchmark.py
+poetry shell
+python tests/benchmark.py -n 5
 ```
 
-Speed test is done using `timeit` with 5 iterations on an early 2015 MacBook Air (8 GB RAM Dual-Core 1.6 GHz). The dataset is COCO 2017 Validation which comprises 5k images and 36 781 bounding boxes.
+The following speed test is performed using Python 3.11 and `timeit` with 5 iterations on a 2021 MacBook Pro 14" (M1 Pro 8 Cores and 16 GB of RAM). The dataset is COCO 2017 Validation which comprises 5k images and 36 781 bounding boxes.
 
 Task   |COCO |CVAT |OpenImage|LabelMe|PascalVOC|YOLO |TXT
 -------|-----|-----|---------|-------|---------|-----|-----
-Parsing|0.52s|0.59s|3.44s    |1.84s  |2.45s    |3.01s|2.54s
-Saving |1.12s|0.74s|0.42s    |4.39s  |4.46s    |3.75s|3.52s
+Parsing|0.25s|0.13s|0.47s    |0.72s  |1.04s    |1.68s|1.42s
+Saving |0.34s|0.20s|0.15s    |1.09s  |1.14s    |0.91s|0.88s
 
-OpenImage, YOLO and TXT are slower because they store bounding box coordinates in relative coordinates and do not provide the image size, so reading it from the image file is required.
-
-The fastest format is COCO and LabelMe.
-
-`AnnotationSet.show_stats()`: 0.12 s
+* `AnnotationSet.show_stats()`: 0.02 s
+* Evalaution: 0.06 s
 
 </details>
 
 ## Todo
 
 * [x] Basic data structures and utilities
 * [x] Parsers (ImageNet, COCO, YOLO, Pascal, OpenImage, CVAT, LabelMe)
@@ -322,7 +322,8 @@
 ## Acknowledgement
 
 This repo is based on the work of [Rafael Padilla](https://github.com/rafaelpadilla/review_object_detection_metrics). The goal of this repo is to improve the performance and flexibility and to provide additional tools.
 
 ## Contribution
 
 Feel free to contribute, any help you can offer with this project is most welcome.
+
```

### Comparing `globox-2.1.2/README.md` & `globox-2.1.3b0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Globox — Object Detection Toolbox
 
 This framework can:
 
 * parse all kinds of object detection datasets (ImageNet, COCO, YOLO, PascalVOC, OpenImage, CVAT, LabelMe, etc.) and show statistics,
 * convert them to other formats (ImageNet, COCO, YOLO, PascalVOC, OpenImage, CVAT, LabelMe, etc.),
-* and evaluate predictions using standard object detection metrics such as AP@[.5:.05:.95], AP@50, mAP, AR<sub>1</sub>, AR<sub>10</sub>, AR<sub>100</sub>.
+* and evaluate predictions using standard object detection metrics such as $AP_{[.5:.05:.95]}$, $AP_{50}$, $mAP$, $AR_{1}$, $AR_{10}$, $AR_{100}$.
 
 This framework can be used both as a library in your own code and as a command line tool. This tool is designed to be simple to use, fast and correct.
 
 ## Install
 
 You can install the package using pip:
 
@@ -78,15 +78,15 @@
 
 Datasets stats can printed to the console:
 
 ```python
 coco_gts.show_stats()
 ```
 
-```shell
+```text
          Database Stats         
 ┏━━━━━━━━━━━━━┳━━━━━━━━┳━━━━━━━┓
 ┃ Label       ┃ Images ┃ Boxes ┃
 ┡━━━━━━━━━━━━━╇━━━━━━━━╇━━━━━━━┩
 │ aeroplane   │     10 │    15 │
 │ bicycle     │      7 │    14 │
 │ bird        │      4 │     6 │
@@ -157,15 +157,15 @@
 
 ```python
 evaluator.show_summary()
 ```
 
 which outputs:
 
-```shell
+```text
                               COCO Evaluation
 ┏━━━━━━━━━━━┳━━━━━━━━━━┳━━━━━━━━┳...┳━━━━━━━━┳━━━━━━━━┳━━━━━━━━┓
 ┃ Label     ┃ AP 50:95 ┃  AP 50 ┃   ┃   AR S ┃   AR M ┃   AR L ┃
 ┡━━━━━━━━━━━╇━━━━━━━━━━╇━━━━━━━━╇...╇━━━━━━━━╇━━━━━━━━╇━━━━━━━━┩
 │ airplane  │    22.7% │  25.2% │   │   nan% │  90.0% │   0.0% │
 │ apple     │    46.4% │  57.4% │   │  48.5% │   nan% │   nan% │
 │ backpack  │    54.8% │  85.1% │   │ 100.0% │  72.0% │   0.0% │
@@ -239,51 +239,47 @@
 
 ## Run Tests
 
 Clone the repo with its test data:
 
 ```shell
 git clone https://github.com/laclouis5/globox --recurse-submodules=tests/globox_test_data
+cd globox
 ```
 
-Install developement dependencies (virtual env recommended):
+Install with Poetry:
 
 ```shell
-pip install -e ".[dev]"
+poetry install
 ```
 
-Run tox:
+Run the tests:
 
 ```shell
-tox
+poetry run pytest
 ```
 
 ## Speed Banchmarks
 
-<details>
-<summary>Click to expand</summary>
-
 Speed benchmark can be executed with:
 
 ```shell
-python3 tests/benchmark.py
+poetry shell
+python tests/benchmark.py -n 5
 ```
 
-Speed test is done using `timeit` with 5 iterations on an early 2015 MacBook Air (8 GB RAM Dual-Core 1.6 GHz). The dataset is COCO 2017 Validation which comprises 5k images and 36 781 bounding boxes.
+The following speed test is performed using Python 3.11 and `timeit` with 5 iterations on a 2021 MacBook Pro 14" (M1 Pro 8 Cores and 16 GB of RAM). The dataset is COCO 2017 Validation which comprises 5k images and 36 781 bounding boxes.
 
 Task   |COCO |CVAT |OpenImage|LabelMe|PascalVOC|YOLO |TXT
 -------|-----|-----|---------|-------|---------|-----|-----
-Parsing|0.52s|0.59s|3.44s    |1.84s  |2.45s    |3.01s|2.54s
-Saving |1.12s|0.74s|0.42s    |4.39s  |4.46s    |3.75s|3.52s
-
-OpenImage, YOLO and TXT are slower because they store bounding box coordinates in relative coordinates and do not provide the image size, so reading it from the image file is required.
-
-The fastest format is COCO and LabelMe.
+Parsing|0.25s|0.13s|0.47s    |0.72s  |1.04s    |1.68s|1.42s
+Saving |0.34s|0.20s|0.15s    |1.09s  |1.14s    |0.91s|0.88s
 
-`AnnotationSet.show_stats()`: 0.12 s
+* `AnnotationSet.show_stats()`: 0.02 s
+* Evalaution: 0.06 s
 
 </details>
 
 ## Todo
 
 * [x] Basic data structures and utilities
 * [x] Parsers (ImageNet, COCO, YOLO, Pascal, OpenImage, CVAT, LabelMe)
```

### Comparing `globox-2.1.2/src/globox/annotation.py` & `globox-2.1.3b0/src/globox/annotation.py`

 * *Files identical despite different names*

### Comparing `globox-2.1.2/src/globox/annotationset.py` & `globox-2.1.3b0/src/globox/annotationset.py`

 * *Files identical despite different names*

### Comparing `globox-2.1.2/src/globox/atomic.py` & `globox-2.1.3b0/src/globox/atomic.py`

 * *Files identical despite different names*

### Comparing `globox-2.1.2/src/globox/boundingbox.py` & `globox-2.1.3b0/src/globox/boundingbox.py`

 * *Files identical despite different names*

### Comparing `globox-2.1.2/src/globox/cli.py` & `globox-2.1.3b0/src/globox/cli.py`

 * *Files identical despite different names*

### Comparing `globox-2.1.2/src/globox/errors.py` & `globox-2.1.3b0/src/globox/errors.py`

 * *Files identical despite different names*

### Comparing `globox-2.1.2/src/globox/evaluation.py` & `globox-2.1.3b0/src/globox/evaluation.py`

 * *Files identical despite different names*

### Comparing `globox-2.1.2/src/globox/file_utils.py` & `globox-2.1.3b0/src/globox/file_utils.py`

 * *Files identical despite different names*

### Comparing `globox-2.1.2/src/globox/image_utils.py` & `globox-2.1.3b0/src/globox/image_utils.py`

 * *Files identical despite different names*

### Comparing `globox-2.1.2/src/globox/thread_utils.py` & `globox-2.1.3b0/src/globox/thread_utils.py`

 * *Files identical despite different names*

### Comparing `globox-2.1.2/src/globox/utils.py` & `globox-2.1.3b0/src/globox/utils.py`

 * *Files identical despite different names*

