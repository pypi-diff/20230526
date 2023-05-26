# Comparing `tmp/mltlk-0.1.1.tar.gz` & `tmp/mltlk-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mltlk-0.1.1.tar", last modified: Fri May 26 08:15:31 2023, max compression
+gzip compressed data, was "dist/mltlk-0.1.2.tar", last modified: Fri May 26 09:50:42 2023, max compression
```

## Comparing `mltlk-0.1.1.tar` & `mltlk-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-26 08:15:31.486745 mltlk-0.1.1/
--rw-r--r--   0 johanhagelback   (503) staff       (20)     1073 2023-05-25 10:25:18.000000 mltlk-0.1.1/LICENSE
--rw-r--r--   0 johanhagelback   (503) staff       (20)      233 2023-05-26 08:15:31.485739 mltlk-0.1.1/PKG-INFO
--rw-r--r--   0 johanhagelback   (503) staff       (20)       51 2023-05-25 10:25:18.000000 mltlk-0.1.1/README.md
--rw-r--r--   0 johanhagelback   (503) staff       (20)    31455 2023-05-26 08:12:45.000000 mltlk-0.1.1/Spiral.ipynb
--rw-r--r--   0 johanhagelback   (503) staff       (20)    19563 2023-05-26 08:12:40.000000 mltlk-0.1.1/Weather.ipynb
--rw-r--r--   0 johanhagelback   (503) staff       (20)    50437 2023-05-26 07:57:41.000000 mltlk-0.1.1/Wikipedia.ipynb
--rw-r--r--   0 johanhagelback   (503) staff       (20)    49725 2023-05-26 08:00:41.000000 mltlk-0.1.1/Wikipedia_word2vec.ipynb
-drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-26 08:15:31.465655 mltlk-0.1.1/data/
--rw-r--r--   0 johanhagelback   (503) staff       (20)     4505 2021-03-10 11:22:51.000000 mltlk-0.1.1/data/spiral.csv
--rw-r--r--   0 johanhagelback   (503) staff       (20)      414 2023-05-26 08:09:41.000000 mltlk-0.1.1/data/weather.csv
--rw-r--r--   0 johanhagelback   (503) staff       (20)  2061699 2019-12-13 13:20:58.000000 mltlk-0.1.1/data/wikipedia_300.csv.gz
-drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-26 08:15:31.476845 mltlk-0.1.1/mltlk/
--rwxr-xr-x   0 johanhagelback   (503) staff       (20)       73 2023-05-26 07:57:16.000000 mltlk-0.1.1/mltlk/__init__.py
--rw-r--r--   0 johanhagelback   (503) staff       (20)    29402 2023-05-26 07:56:23.000000 mltlk-0.1.1/mltlk/ml.py
--rw-r--r--   0 johanhagelback   (503) staff       (20)     3324 2023-05-25 12:08:40.000000 mltlk-0.1.1/mltlk/resampling.py
--rw-r--r--   0 johanhagelback   (503) staff       (20)      337 2023-05-25 12:06:32.000000 mltlk-0.1.1/mltlk/utils.py
--rw-r--r--   0 johanhagelback   (503) staff       (20)     4978 2023-05-26 07:38:19.000000 mltlk-0.1.1/mltlk/word2vec.py
-drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-26 08:15:31.484136 mltlk-0.1.1/mltlk.egg-info/
--rw-r--r--   0 johanhagelback   (503) staff       (20)      233 2023-05-26 08:15:30.000000 mltlk-0.1.1/mltlk.egg-info/PKG-INFO
--rw-r--r--   0 johanhagelback   (503) staff       (20)      380 2023-05-26 08:15:31.000000 mltlk-0.1.1/mltlk.egg-info/SOURCES.txt
--rw-r--r--   0 johanhagelback   (503) staff       (20)        1 2023-05-26 08:15:30.000000 mltlk-0.1.1/mltlk.egg-info/dependency_links.txt
--rw-r--r--   0 johanhagelback   (503) staff       (20)       74 2023-05-26 08:15:31.000000 mltlk-0.1.1/mltlk.egg-info/requires.txt
--rw-r--r--   0 johanhagelback   (503) staff       (20)        6 2023-05-26 08:15:31.000000 mltlk-0.1.1/mltlk.egg-info/top_level.txt
--rw-r--r--   0 johanhagelback   (503) staff       (20)       38 2023-05-26 08:15:31.487138 mltlk-0.1.1/setup.cfg
--rw-r--r--   0 johanhagelback   (503) staff       (20)      361 2023-05-26 07:57:08.000000 mltlk-0.1.1/setup.py
+drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-26 09:50:42.745453 mltlk-0.1.2/
+-rw-r--r--   0 johanhagelback   (503) staff       (20)       93 2023-05-26 08:29:02.000000 mltlk-0.1.2/.gitignore
+-rw-r--r--   0 johanhagelback   (503) staff       (20)     1073 2023-05-25 10:25:18.000000 mltlk-0.1.2/LICENSE
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      233 2023-05-26 09:50:42.744697 mltlk-0.1.2/PKG-INFO
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      311 2023-05-26 08:20:29.000000 mltlk-0.1.2/README.md
+-rw-r--r--   0 johanhagelback   (503) staff       (20)    31370 2023-05-26 09:49:14.000000 mltlk-0.1.2/Spiral.ipynb
+-rw-r--r--   0 johanhagelback   (503) staff       (20)    40302 2023-05-26 09:48:44.000000 mltlk-0.1.2/Weather.ipynb
+-rw-r--r--   0 johanhagelback   (503) staff       (20)    50437 2023-05-26 09:49:20.000000 mltlk-0.1.2/Wikipedia.ipynb
+-rw-r--r--   0 johanhagelback   (503) staff       (20)    49851 2023-05-26 09:44:45.000000 mltlk-0.1.2/Wikipedia_word2vec.ipynb
+drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-26 09:50:42.718924 mltlk-0.1.2/data/
+-rw-r--r--   0 johanhagelback   (503) staff       (20)     4505 2021-03-10 11:22:51.000000 mltlk-0.1.2/data/spiral.csv
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      414 2023-05-26 08:09:41.000000 mltlk-0.1.2/data/weather.csv
+-rw-r--r--   0 johanhagelback   (503) staff       (20)  2061699 2019-12-13 13:20:58.000000 mltlk-0.1.2/data/wikipedia_300.csv.gz
+drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-26 09:50:42.733923 mltlk-0.1.2/mltlk/
+-rwxr-xr-x   0 johanhagelback   (503) staff       (20)       73 2023-05-26 08:58:43.000000 mltlk-0.1.2/mltlk/__init__.py
+-rw-r--r--   0 johanhagelback   (503) staff       (20)    32015 2023-05-26 09:48:27.000000 mltlk-0.1.2/mltlk/ml.py
+-rw-r--r--   0 johanhagelback   (503) staff       (20)     3324 2023-05-25 12:08:40.000000 mltlk-0.1.2/mltlk/resampling.py
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      337 2023-05-25 12:06:32.000000 mltlk-0.1.2/mltlk/utils.py
+-rw-r--r--   0 johanhagelback   (503) staff       (20)     4978 2023-05-26 07:38:19.000000 mltlk-0.1.2/mltlk/word2vec.py
+drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-26 09:50:42.743215 mltlk-0.1.2/mltlk.egg-info/
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      233 2023-05-26 09:50:42.000000 mltlk-0.1.2/mltlk.egg-info/PKG-INFO
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      391 2023-05-26 09:50:42.000000 mltlk-0.1.2/mltlk.egg-info/SOURCES.txt
+-rw-r--r--   0 johanhagelback   (503) staff       (20)        1 2023-05-26 09:50:42.000000 mltlk-0.1.2/mltlk.egg-info/dependency_links.txt
+-rw-r--r--   0 johanhagelback   (503) staff       (20)       74 2023-05-26 09:50:42.000000 mltlk-0.1.2/mltlk.egg-info/requires.txt
+-rw-r--r--   0 johanhagelback   (503) staff       (20)        6 2023-05-26 09:50:42.000000 mltlk-0.1.2/mltlk.egg-info/top_level.txt
+-rw-r--r--   0 johanhagelback   (503) staff       (20)       38 2023-05-26 09:50:42.745715 mltlk-0.1.2/setup.cfg
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      361 2023-05-26 08:58:35.000000 mltlk-0.1.2/setup.py
```

### Comparing `mltlk-0.1.1/LICENSE` & `mltlk-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mltlk-0.1.1/Spiral.ipynb` & `mltlk-0.1.2/Spiral.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9988055555555555%*

 * *Differences: {"'cells'": "{1: {'outputs': {0: {'text': ['0.1.2\\n']}}}, 3: {'outputs': {0: {'text': {delete: "*

 * *            '[0]}}}, \'source\': [\'session = load_data("data/spiral.csv", conf={"preprocess": '*

 * *            '"scale"})\']}, 8: {\'outputs\': {0: {\'text\': {insert: [(0, \'Building and '*

 * *            "evaluating model using 10-fold cross validaton took \\x1b[34m14.39\\x1b[0m sec\\n')], "*

 * *            "delete: [0]}}}}, 10: {'outputs': {0: {'text': {insert: [(0, 'Building and evaluating "*

 * *            "model using  […]*

```diff
@@ -12,15 +12,15 @@
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "0.1.1\n"
+                        "0.1.2\n"
                     ]
                 }
             ],
             "source": [
                 "import mltlk\n",
                 "print(mltlk.__version__)\n",
                 "from mltlk import *"
@@ -41,22 +41,21 @@
             "execution_count": 2,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "\u001b[1m\u001b[33mInfo: \u001b[0mLabels encoded\n",
                         "\u001b[1m\u001b[33mInfo: \u001b[0mScaled input data using standard scaler\n",
                         "\u001b[1m\u001b[33mInfo: \u001b[0mLoaded \u001b[34m300\u001b[0m examples in \u001b[34m3\u001b[0m categories\n"
                     ]
                 }
             ],
             "source": [
-                "session = load_data(\"data/spiral.csv\", conf={\"preprocess\": \"scale\", \"encode_labels\": True})"
+                "session = load_data(\"data/spiral.csv\", conf={\"preprocess\": \"scale\"})"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Show data stats"
@@ -103,15 +102,15 @@
             "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Building and evaluating model using 10-fold cross validaton took \u001b[34m11.54\u001b[0m sec\n",
+                        "Building and evaluating model using 10-fold cross validaton took \u001b[34m14.39\u001b[0m sec\n",
                         "\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
                             "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Results</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Accuracy:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>97.33%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>F1-score:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>97.33%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Precision:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>97.36%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Recall:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>97.33%</td></tr></table>"
@@ -170,15 +169,15 @@
             "execution_count": 5,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Building and evaluating model using 10-fold cross validaton took \u001b[34m2.25\u001b[0m sec\n",
+                        "Building and evaluating model using 10-fold cross validaton took \u001b[34m1.88\u001b[0m sec\n",
                         "\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
                             "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Results</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Accuracy:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>97.67%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>F1-score:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>97.68%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Precision:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>97.76%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Recall:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>97.67%</td></tr></table>"
@@ -238,15 +237,15 @@
             "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "\u001b[1m\u001b[33mInfo: \u001b[0mBuilding final model on all data took \u001b[36m0.18\u001b[0m sec\n"
+                        "\u001b[1m\u001b[33mInfo: \u001b[0mBuilding final model on all data took \u001b[36m0.20\u001b[0m sec\n"
                     ]
                 }
             ],
             "source": [
                 "build_model(RandomForestClassifier(), session)"
             ]
         },
```

### Comparing `mltlk-0.1.1/Wikipedia.ipynb` & `mltlk-0.1.2/Wikipedia.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997960758377424%*

 * *Differences: {"'cells'": "{1: {'outputs': {0: {'text': ['0.1.2\\n']}}}, 7: {'outputs': {0: {'text': {insert: "*

 * *            "[(0, 'Building and evaluating model using 10-fold cross validaton took "*

 * *            "\\x1b[34m0.33\\x1b[0m sec\\n')], delete: [0]}}}}, 12: {'outputs': {0: {'text': "*

 * *            "{insert: [(0, '\\x1b[1m\\x1b[33mInfo: \\x1b[0mBuilding final model on all data took "*

 * *            "\\x1b[36m0.04\\x1b[0m sec\\n')], delete: [0]}}}}}"}*

```diff
@@ -12,15 +12,15 @@
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "0.1.1\n"
+                        "0.1.2\n"
                     ]
                 }
             ],
             "source": [
                 "import mltlk\n",
                 "print(mltlk.__version__)\n",
                 "from mltlk import *"
@@ -103,15 +103,15 @@
             "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Building and evaluating model using 10-fold cross validaton took \u001b[34m0.32\u001b[0m sec\n",
+                        "Building and evaluating model using 10-fold cross validaton took \u001b[34m0.33\u001b[0m sec\n",
                         "\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
                             "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Results</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Accuracy:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>95.33%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>F1-score:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>95.33%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Precision:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>95.37%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Recall:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>95.33%</td></tr></table>"
@@ -278,15 +278,15 @@
             "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "\u001b[1m\u001b[33mInfo: \u001b[0mBuilding final model on all data took \u001b[36m0.05\u001b[0m sec\n",
+                        "\u001b[1m\u001b[33mInfo: \u001b[0mBuilding final model on all data took \u001b[36m0.04\u001b[0m sec\n",
                         "\u001b[1m\u001b[33mInfo: \u001b[0mExample is predicted as \u001b[32mGames\u001b[0m\n"
                     ]
                 }
             ],
             "source": [
                 "build_model(LinearSVC(), session)\n",
                 "predict(\"This is an article about gamers - people who love playing games\", session)"
```

### Comparing `mltlk-0.1.1/Wikipedia_word2vec.ipynb` & `mltlk-0.1.2/Wikipedia_word2vec.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996550217309146%*

 * *Differences: {"'cells'": "{1: {'outputs': {0: {'text': ['0.1.2\\n']}}}, 3: {'outputs': {0: {'text': {insert: "*

 * *            "[(2, '\\x1b[1m\\x1b[33mInfo: \\x1b[0mWord2vec model generated in "*

 * *            "\\x1b[34m3.77\\x1b[0m sec\\n'), (4, '\\x1b[1m\\x1b[33mInfo: \\x1b[0mWord2vec "*

 * *            "embeddings generated in \\x1b[34m11.31\\x1b[0m sec\\n')], delete: [4, 2]}}}}, 7: "*

 * *            '{\'outputs\': {1: {\'data\': {\'text/html\': ["<table><tr><td '*

 * *            "style='color:black;background:#ddd;padding-top:3px;paddi […]*

```diff
@@ -12,15 +12,15 @@
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "0.1.1\n"
+                        "0.1.2\n"
                     ]
                 }
             ],
             "source": [
                 "import mltlk\n",
                 "print(mltlk.__version__)\n",
                 "from mltlk import *"
@@ -43,17 +43,17 @@
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "\u001b[1m\u001b[33mInfo: \u001b[0mClean texts keeping letters and digits\n",
                         "\u001b[1m\u001b[33mInfo: \u001b[0mUsed stopwords \u001b[36menglish\u001b[0m\n",
-                        "\u001b[1m\u001b[33mInfo: \u001b[0mWord2vec model generated in \u001b[34m4.61\u001b[0m sec\n",
+                        "\u001b[1m\u001b[33mInfo: \u001b[0mWord2vec model generated in \u001b[34m3.77\u001b[0m sec\n",
                         "\u001b[1m\u001b[33mInfo: \u001b[0mWord2vec model stored to \u001b[36mword2vec/wikipedia_300_75.w2v\u001b[0m\n",
-                        "\u001b[1m\u001b[33mInfo: \u001b[0mWord2vec embeddings generated in \u001b[34m14.45\u001b[0m sec\n",
+                        "\u001b[1m\u001b[33mInfo: \u001b[0mWord2vec embeddings generated in \u001b[34m11.31\u001b[0m sec\n",
                         "\u001b[1m\u001b[33mInfo: \u001b[0mWord2vec embeddings stored to \u001b[36mword2vec/wikipedia_300_75.emb\u001b[0m\n",
                         "\u001b[1m\u001b[33mInfo: \u001b[0mLoaded \u001b[34m300\u001b[0m examples in \u001b[34m2\u001b[0m categories\n"
                     ]
                 }
             ],
             "source": [
                 "session = load_data(\"data/wikipedia_300.csv.gz\", conf={\n",
@@ -113,15 +113,15 @@
                         "Building and evaluating model using 10-fold cross validaton took \u001b[34m0.16\u001b[0m sec\n",
                         "\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
-                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Results</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Accuracy:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>93.33%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>F1-score:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>93.33%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Precision:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>93.34%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Recall:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>93.33%</td></tr></table>"
+                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Results</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Accuracy:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>92.67%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>F1-score:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>92.67%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Precision:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>92.67%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Recall:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>92.67%</td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -132,15 +132,15 @@
                     "text": [
                         "\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
-                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;row-toggle-background:0;'>Category</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;row-toggle-background:0;'>Accuracy</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;row-toggle-background:0;'>n</td></tr><tr><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#048512;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>Programming</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>94.00%</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#3b08d3;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>150</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#fd8e8a;font-family:Verdana;font-size:12px;font:Verdana 12px;'>&nbsp;&nbsp;Games</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;num-format:pct-2;font-family:Verdana;font-size:12px;font:Verdana 12px;'>6.00%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;font-family:Verdana;font-size:12px;font:Verdana 12px;'>9</td></tr><tr><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#048512;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>Games</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>92.67%</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#3b08d3;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>150</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#fd8e8a;font-family:Verdana;font-size:12px;border-bottom:1px solid #aaa;font:Verdana 12px;'>&nbsp;&nbsp;Programming</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;num-format:pct-2;font-family:Verdana;font-size:12px;border-bottom:1px solid #aaa;font:Verdana 12px;'>7.33%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;font-family:Verdana;font-size:12px;border-bottom:1px solid #aaa;font:Verdana 12px;'>11</td></tr></table>"
+                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;row-toggle-background:0;'>Category</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;row-toggle-background:0;'>Accuracy</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;row-toggle-background:0;'>n</td></tr><tr><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#048512;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>Programming</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>92.67%</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#3b08d3;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>150</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#fd8e8a;font-family:Verdana;font-size:12px;font:Verdana 12px;'>&nbsp;&nbsp;Games</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;num-format:pct-2;font-family:Verdana;font-size:12px;font:Verdana 12px;'>7.33%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;font-family:Verdana;font-size:12px;font:Verdana 12px;'>11</td></tr><tr><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#048512;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>Games</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>92.67%</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#3b08d3;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>150</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#fd8e8a;font-family:Verdana;font-size:12px;border-bottom:1px solid #aaa;font:Verdana 12px;'>&nbsp;&nbsp;Programming</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;num-format:pct-2;font-family:Verdana;font-size:12px;border-bottom:1px solid #aaa;font:Verdana 12px;'>7.33%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;font-family:Verdana;font-size:12px;border-bottom:1px solid #aaa;font:Verdana 12px;'>11</td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -150,15 +150,15 @@
                     "output_type": "stream",
                     "text": [
                         "\n"
                     ]
                 },
                 {
                     "data": {
-                        "image/png": "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+0ySlJiYqNOnT+udd96RJE2cOFELFy7U7Nmz9dNPP2nw4MHq2rWrNm/eLOlqUOnUqZPatm2r3bt364UXXtCrr75a6PfEy8tL8+fP188//6x33nlHc+bM0dSpU236HDp0SEuXLtWqVav01VdfadeuXerTp491+eLFi/X6669r/Pjx2r9/vyZMmKCRI0dqwYIFha4HuCYLABRAZGSkpX379haLxWIxm82W9evXW1xcXCxRUVHW5YGBgZYrV65Y11m0aJElPDzcYjabrW1XrlyxuLm5WdauXWuxWCyWcuXKWd58803r8qysLEuFChWs+7JYLJaHHnrIMnDgQIvFYrEkJiZaJFnWr1+fb52bNm2ySLL88ccf1rbLly9b3N3dLd9++61N3549e1qeeeYZi8VisYwYMcJSo0YNm+XDhw/Ps62/k2T5/PPPr7n8rbfestSrV8/6etSoURZnZ2fLiRMnrG1ffvmlxcnJyXL69GmLxWKxVKlSxfLRRx/ZbGfs2LGWhg0bWiwWiyUpKckiybJr165r7hf4J8wBAFBgsbGx8vT0VFZWlsxms5599llFR0dbl0dERNhc99+zZ48OHTokLy8vm+1cvnxZhw8fVkpKik6fPq17773XuqxEiRK655578lwGyLV79245OzvroYceKnDdhw4dUkZGhh555BGb9szMTNWtW1eStH//fps6JKlhw4YF3keuTz75RNOnT9fhw4eVlpam7OxseXt72/SpWLGiypcvb7Mfs9msxMREeXl56fDhw+rZs6defPFFa5/s7Gz5+PgUuh7gWggAAAqsadOmmjVrlkqVKqWgoCCVKGH7J+Sv3/YmSWlpaapXr54WL16cZ1t33HHHDdXg5uZW6HXS0tIkSatXr7b54JVk8611N2vbtm3q0qWLRo8erZYtW8rHx0dLlizR5MmTC13rnDlz8gQSZ2dnu9UKEAAAFJiHh4fCwsIK3P/uu+/WJ598ooCAgDxnwbnKlSun77//Xo0bN5Z09Uw3ISFBd999d779IyIiZDabtXnzZjVv3jzP8twRiJycHGtbjRo15OLiouPHj19z5KB69erWCY25vvvuu38+yL/49ttvValSJf3nP/+xth07dixPv+PHj+vUqVMKCgqy7sfJyUnh4eEKDAxUUFCQjhw5oi5duhRq/0BhMAkQQJHp0qWLypQpo/bt22vLli1KSkrS119/rQEDBujEiROSpIEDB+qNN97QihUrdODAAfXp0+e69/CHhIQoMjJSzz//vFasWGHd5tKlSyVJlSpVkslkUmxsrM6fP6+0tDR5eXkpKipKgwcP1oIFC3T48GHt3LlTM2bMsE6s69Wrl3755Re98sorSkxM1EcffaT58+cX6njvvPNOHT9+XEuWLNHhw4c1ffr0fCc0urq6KjIyUnv27NGWLVs0YMAAde7cWWXLlpUkjR49WhMnTtT06dN18OBB7d27VzExMZoyZUqh6gGuhwAAoMi4u7vrm2++UcWKFdWpUydVr15dPXv21OXLl60jAkOHDlW3bt0UGRmphg0bysvLSx07drzudmfNmqUnnnhCffr0UbVq1fTiiy8qPT1dklS+fHmNHj1ar776qgIDA9WvXz9J0tixYzVy5EhNnDhR1atXV6tWrbR69WpVrlxZ0tXr8p999plWrFih2rVra/bs2ZowYUKhjrddu3YaPHiw+vXrpzp16ujbb7/VyJEj8/QLCwtTp06d1Lp1a7Vo0UK1atWyuc3vhRde0Ny5cxUTE6OIiAg99NBDmj9/vrVWwB5MlmvNtAEAALctRgAAADAgAgAAAAZEAAAAwIAIAAAAGBABAAAAAyIAAABgQAQAAAAMiAAAAIABEQAAADAgAgAAAAZEAAAAwID+DyaguQYU/MexAAAAAElFTkSuQmCC\n",
+                        "image/png": "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1arWBY05fvjhh9sf5P/4/vvvVb58ef33v/+1tv3+++83jDtx4oTOnDmjwMBA636cnJwUFhamgIAABQYG6ujRo+rWrVu+9g/kB4sAARSYbt26qUSJEurYsaO2bdumY8eO6bvvvtPgwYN16tQpSdKQIUP05ptvatWqVfr111/Vv3//W97DHxwcrPDwcL3wwgtatWqVdZvLly+XJJUvX14mk0lr1qzRxYsXlZKSIi8vL0VERGjYsGFatGiRjhw5ovj4eM2ePdu6sK5v37767bff9OqrryohIUEff/yxoqOj83W8lSpV0okTJ7Rs2TIdOXJEs2bNynVBo6urq8LDw7V3715t27ZNgwcP1lNPPaVSpUpJksaNG6fJkydr1qxZOnTokPbt26eoqChNmzYtX/UAt0IAAFBg3N3dtXXrVpUrV05dunRR1apV1bt3b127ds06IzB8+HD16NFD4eHhatCggby8vNS5c+dbbnfu3Lnq2rWr+vfvrypVqujFF19UamqqJKlMmTIaN26cXnvtNQUEBGjgwIGSpDfeeEOjR4/W5MmTVbVqVbVp00Zr165VhQoVJF2/Lv/5559r1apVql27tubNm6dJkybl63g7dOigYcOGaeDAgapTp46+//57jR49+oZxoaGh6tKli9q2batWrVqpVq1aNrf59enTRwsWLFBUVJRq1qypRx99VNHR0dZaAXswWW620gYAANyzmAEAAMCACAAAABgQAQAAAAMiAAAAYEAEAAAADIgAAACAAREAAAAwIAIAAAAGRAAAAMCACAAAABgQAQAAAAP6f5JS+2r8OYa9AAAAAElFTkSuQmCC\n",
                         "text/plain": [
                             "<Figure size 640x480 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
@@ -220,15 +220,15 @@
                         "Building and evaluating model using 10-fold cross validaton took \u001b[34m0.16\u001b[0m sec\n",
                         "\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
-                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Results</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Accuracy:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>93.33%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>F1-score:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>93.33%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Precision:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>93.34%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Recall:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>93.33%</td></tr></table>"
+                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Results</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Accuracy:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>92.67%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>F1-score:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>92.67%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Precision:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>92.67%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Recall:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>92.67%</td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -239,15 +239,15 @@
                     "text": [
                         "\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
-                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;row-toggle-background:0;'>Category</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;row-toggle-background:0;'>Accuracy</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;row-toggle-background:0;'>n</td></tr><tr><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#048512;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>Programming</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>94.00%</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#3b08d3;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>150</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#fd8e8a;font-family:Verdana;font-size:12px;font:Verdana 12px;'>&nbsp;&nbsp;Games</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;num-format:pct-2;font-family:Verdana;font-size:12px;font:Verdana 12px;'>6.00%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;font-family:Verdana;font-size:12px;font:Verdana 12px;'>9</td></tr><tr><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#048512;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>Games</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>92.67%</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#3b08d3;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>150</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#fd8e8a;font-family:Verdana;font-size:12px;border-bottom:1px solid #aaa;font:Verdana 12px;'>&nbsp;&nbsp;Programming</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;num-format:pct-2;font-family:Verdana;font-size:12px;border-bottom:1px solid #aaa;font:Verdana 12px;'>7.33%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;font-family:Verdana;font-size:12px;border-bottom:1px solid #aaa;font:Verdana 12px;'>11</td></tr></table>"
+                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;row-toggle-background:0;'>Category</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;row-toggle-background:0;'>Accuracy</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;row-toggle-background:0;'>n</td></tr><tr><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#048512;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>Programming</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>92.67%</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#3b08d3;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>150</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#fd8e8a;font-family:Verdana;font-size:12px;font:Verdana 12px;'>&nbsp;&nbsp;Games</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;num-format:pct-2;font-family:Verdana;font-size:12px;font:Verdana 12px;'>7.33%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;font-family:Verdana;font-size:12px;font:Verdana 12px;'>11</td></tr><tr><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#048512;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>Games</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>92.67%</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#3b08d3;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>150</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#fd8e8a;font-family:Verdana;font-size:12px;border-bottom:1px solid #aaa;font:Verdana 12px;'>&nbsp;&nbsp;Programming</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;num-format:pct-2;font-family:Verdana;font-size:12px;border-bottom:1px solid #aaa;font:Verdana 12px;'>7.33%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;font-family:Verdana;font-size:12px;border-bottom:1px solid #aaa;font:Verdana 12px;'>11</td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -281,15 +281,15 @@
             "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "\u001b[1m\u001b[33mInfo: \u001b[0mBuilding final model on all data took \u001b[36m0.02\u001b[0m sec\n",
+                        "\u001b[1m\u001b[33mInfo: \u001b[0mBuilding final model on all data took \u001b[36m0.01\u001b[0m sec\n",
                         "\u001b[1m\u001b[33mInfo: \u001b[0mExample is predicted as \u001b[32mGames\u001b[0m\n"
                     ]
                 }
             ],
             "source": [
                 "build_model(LinearSVC(), session)\n",
                 "predict(\"This is an article about gamers - people who love playing games\", session)"
```

### Comparing `mltlk-0.1.1/data/spiral.csv` & `mltlk-0.1.2/data/spiral.csv`

 * *Files identical despite different names*

### Comparing `mltlk-0.1.1/data/wikipedia_300.csv.gz` & `mltlk-0.1.2/data/wikipedia_300.csv.gz`

 * *Files identical despite different names*

### Comparing `mltlk-0.1.1/mltlk/ml.py` & `mltlk-0.1.2/mltlk/ml.py`

 * *Files 12% similar despite different names*

```diff
@@ -67,14 +67,24 @@
         for c,val in enumerate(r):
             if c in Xcols:
                 row.append(val)
         if len(row) == 1:
             row = row[0]
         X.append(row)
         y.append(r[ycol])
+        
+    # Check if all yi is integer
+    y_tmp = [yi for yi in y if type(yi) in [float, np.float64]]
+    if len(y_tmp) == len(y):
+        y_tmp = [yi for yi in y_tmp if float(yi).is_integer()]
+        if len(y_tmp) == len(y):
+            # Convert to int
+            y = [int(yi) for yi in y]
+            
+    # Update session
     session["X_original"] = X
     session["y_original"] = y
     session["X"] = X.copy()
     session["y"] = y.copy()
     
     # Skip minority categories
     if "min_samples" in conf:
@@ -213,14 +223,22 @@
 # Show data stats
 #
 def data_stats(session, max_rows=None, show_graph=False, descriptions=None):
     if session is None:
         error("Session is empty")
         return
     
+    # Set descriptions (if found)
+    if descriptions is not None:
+        if type(descriptions) == dict:
+            session["descriptions"] = descriptions
+        else:
+            warning("Invalid type for descriptions (expected " + colored("dict", "cyan") + ")")
+            descriptions = None
+    
     y = session["y"]
     cnt = Counter(y)
     tab = []
     for key,no in cnt.items():
         tab.append([key,no,f"{no/len(y)*100:.1f}%"])
     tab = sorted(tab, key=lambda x: x[1], reverse=True)
     rno = 0
@@ -270,15 +288,19 @@
         t.column_style([1,5,9], {"color": "value"})
         t.column_style([2,6,10], {"color": "percent"})
         t.column_style([3,7,11], {"color": "green"})
     for i in range(0,s):
         r = []
         for j in range(0,3):
             if i < len(tab2[j]):
-                r.append(tab2[j][i][0])
+                if "label_encoder" in session:
+                    l = session["label_encoder"].inverse_transform([tab2[j][i][0]])[0]
+                    r.append(f"{l} ({tab2[j][i][0]})")
+                else:
+                    r.append(tab2[j][i][0])
                 r.append(tab2[j][i][1])
                 r.append(tab2[j][i][2])
                 r.append(tab2[j][i][3])
                 if descriptions is not None:
                     desc = ""
                     if tab2[j][i][0] in descriptions:
                         desc = descriptions[tab2[j][i][0]]
@@ -543,45 +565,70 @@
             errs = []
             for j in range(0,len(r)):
                 if i != j and r[j] > 0:
                     errs.append([r[j], cats[j]])
             tmp.append([r[i]/sum(r),cat,sum(r),errs])
         tmp = sorted(tmp, reverse=True)
         # Show table
-        t = CustomizedTable(["Category", "Accuracy", "n"], style={"row-toggle-background": 0})
+        if "descriptions" not in session:
+            t = CustomizedTable(["Category", "Accuracy", "n"], style={"row-toggle-background": 0})
+        else:
+            t = CustomizedTable(["Category", "Accuracy", "n", "Description"], style={"row-toggle-background": 0})
+            t.column_style("Description", {"color": "#05760f"})
         t.column_style(0, {"color": "#048512"})
         t.column_style(1, {"color": "percent", "num-format": "pct-2"})
         t.column_style(2, {"color": "value"})
         sidx = 0
         maxcats = len(tmp)
         if "sidx" in conf:
             sidx = conf["sidx"]
         if "max_categories" in conf:
             maxcats = conf["max_categories"]
         for r in tmp[sidx:sidx+maxcats]:
-            t.add_row([r[1], float(r[0]), r[2]], style={"border": "top", "background": "#eee"})
+            cat = r[1]
+            if "label_encoder" in session:
+                l = session["label_encoder"].inverse_transform([cat])[0]
+                cat = f"{l} ({cat})"
+            row = [cat, float(r[0]), r[2]]
+            if "descriptions" in session:
+                row.append(session["descriptions"][r[1]])
+            t.add_row(row, style={"border": "top", "background": "#eee"})
             if len(r[3]) > 0:
                 errs = sorted(r[3], reverse=True)
                 if "max_errors" in conf:
                     errs = errs[:conf["max_errors"]]
                 for err in errs:
-                    t.add_row([f"&nbsp;&nbsp;{err[1]}", float(err[0]/r[2]), err[0]])
+                    ecat = err[1]
+                    if "label_encoder" in session:
+                        l = session["label_encoder"].inverse_transform([ecat])[0]
+                        ecat = f"{l} ({ecat})"
+                    erow = [f"&nbsp;&nbsp;{ecat}", float(err[0]/r[2]), err[0]]
+                    if "descriptions" in session:
+                        erow.append(session["descriptions"][err[1]])
+                    t.add_row(erow)
+                    if "descriptions" in session:
+                        t.cell_style(3,-1, {"color": "#fb6d6d"})
                     t.cell_style(0,-1, {"color": "#fd8e8a"})
                     t.cell_style([1,2],-1, {"color": "#aaa4fa"})
         print()
         t.display()
         
     # Confusion matrix
     if "confusion_matrix" in conf and conf["confusion_matrix"]:
         print()
-        from sklearn.metrics import ConfusionMatrixDisplay
         norm = None
         if type(conf["confusion_matrix"]) == str:
             norm = conf["confusion_matrix"]
-        ConfusionMatrixDisplay.from_predictions(session["y_actual"], session["y_pred"], normalize=norm, xticks_rotation="vertical", cmap="inferno", values_format=".2f", colorbar=False)
+        labels = None
+        if "label_encoder" in session:
+            labels = []
+            for cat in cats:
+                l = session["label_encoder"].inverse_transform([cat])[0]
+                labels.append(f"{l} ({cat})")
+        ConfusionMatrixDisplay.from_predictions(session["y_actual"], session["y_pred"], normalize=norm, xticks_rotation="vertical", cmap="inferno", values_format=".2f", colorbar=False, display_labels=labels)
         plt.show()
     
     print()
 
 
 #
 # Builds final model
@@ -754,28 +801,40 @@
     
     # Bag of words
     if type(xi) == str and session["preprocess"] in ["bag-of-words", "bow"]:
         X = session["bow"].transform([xi])
         if "tf-idf" in session:
             X = session["tf-idf"].transform(X)
         pred = session["model"].predict(X)
-        info("Example is predicted as " + colored(pred[0], "green"))
+        res = pred[0]
+        if "label_encoder" in session:
+            res = f"{session['label_encoder'].inverse_transform([res])[0]} ({res})"
+        info("Example is predicted as " + colored(res, "green"))
         return
     
     # Word2vec
     if type(xi) == str and session["preprocess"] in ["word2vec", "wordtovec"]:
         X = [word_vector(xi, session)]
         pred = session["model"].predict(X)
-        info("Example is predicted as " + colored(pred[0], "green"))
+        res = pred[0]
+        if "label_encoder" in session:
+            res = f"{session['label_encoder'].inverse_transform([res])[0]} ({res})"
+        info("Example is predicted as " + colored(res, "green"))
         return
     
     # Numerical/ordinal data
     if "scaler" in session:
         X = session["scaler"].transform([xi])
         pred = session["model"].predict(X)
-        info("Example is predicted as " + colored(pred[0], "green"))
+        res = pred[0]
+        if "label_encoder" in session:
+            res = f"{session['label_encoder'].inverse_transform([res])[0]} ({res})"
+        info("Example is predicted as " + colored(res, "green"))
         return
     
     # No pre-processing
     pred = session["model"].predict([xi])
-    info("Example is predicted as " + colored(pred[0], "green"))
+    res = pred[0]
+    if "label_encoder" in session:
+        res = f"{session['label_encoder'].inverse_transform([res])[0]} ({res})"
+    info("Example is predicted as " + colored(res, "green"))
```

### Comparing `mltlk-0.1.1/mltlk/resampling.py` & `mltlk-0.1.2/mltlk/resampling.py`

 * *Files identical despite different names*

### Comparing `mltlk-0.1.1/mltlk/word2vec.py` & `mltlk-0.1.2/mltlk/word2vec.py`

 * *Files identical despite different names*

