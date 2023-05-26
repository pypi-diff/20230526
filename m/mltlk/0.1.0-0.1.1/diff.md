# Comparing `tmp/mltlk-0.1.0.tar.gz` & `tmp/mltlk-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mltlk-0.1.0.tar", last modified: Thu May 25 10:42:28 2023, max compression
+gzip compressed data, was "dist/mltlk-0.1.1.tar", last modified: Fri May 26 08:15:31 2023, max compression
```

## Comparing `mltlk-0.1.0.tar` & `mltlk-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,26 @@
-drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-25 10:42:28.630978 mltlk-0.1.0/
--rw-r--r--   0 johanhagelback   (503) staff       (20)     1073 2023-05-25 10:25:18.000000 mltlk-0.1.0/LICENSE
--rw-r--r--   0 johanhagelback   (503) staff       (20)      233 2023-05-25 10:42:28.629771 mltlk-0.1.0/PKG-INFO
--rw-r--r--   0 johanhagelback   (503) staff       (20)       51 2023-05-25 10:25:18.000000 mltlk-0.1.0/README.md
--rw-r--r--   0 johanhagelback   (503) staff       (20)    44001 2023-05-25 10:42:13.000000 mltlk-0.1.0/Wikipedia.ipynb
-drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-25 10:42:28.608207 mltlk-0.1.0/data/
--rw-r--r--   0 johanhagelback   (503) staff       (20)  6323835 2019-12-13 13:20:58.000000 mltlk-0.1.0/data/wikipedia_300.csv
-drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-25 10:42:28.623398 mltlk-0.1.0/mltlk/
--rwxr-xr-x   0 johanhagelback   (503) staff       (20)       73 2023-05-17 10:32:17.000000 mltlk-0.1.0/mltlk/__init__.py
--rw-r--r--   0 johanhagelback   (503) staff       (20)    23314 2023-05-25 10:28:26.000000 mltlk-0.1.0/mltlk/ml.py
--rw-r--r--   0 johanhagelback   (503) staff       (20)     3565 2023-05-17 10:35:48.000000 mltlk-0.1.0/mltlk/resampling.py
--rw-r--r--   0 johanhagelback   (503) staff       (20)     4544 2023-05-25 10:04:04.000000 mltlk-0.1.0/mltlk/word2vec.py
-drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-25 10:42:28.628654 mltlk-0.1.0/mltlk.egg-info/
--rw-r--r--   0 johanhagelback   (503) staff       (20)      233 2023-05-25 10:42:27.000000 mltlk-0.1.0/mltlk.egg-info/PKG-INFO
--rw-r--r--   0 johanhagelback   (503) staff       (20)      277 2023-05-25 10:42:28.000000 mltlk-0.1.0/mltlk.egg-info/SOURCES.txt
--rw-r--r--   0 johanhagelback   (503) staff       (20)        1 2023-05-25 10:42:28.000000 mltlk-0.1.0/mltlk.egg-info/dependency_links.txt
--rw-r--r--   0 johanhagelback   (503) staff       (20)       74 2023-05-25 10:42:28.000000 mltlk-0.1.0/mltlk.egg-info/requires.txt
--rw-r--r--   0 johanhagelback   (503) staff       (20)        6 2023-05-25 10:42:28.000000 mltlk-0.1.0/mltlk.egg-info/top_level.txt
--rw-r--r--   0 johanhagelback   (503) staff       (20)       38 2023-05-25 10:42:28.631168 mltlk-0.1.0/setup.cfg
--rw-r--r--   0 johanhagelback   (503) staff       (20)      361 2023-05-25 10:28:57.000000 mltlk-0.1.0/setup.py
+drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-26 08:15:31.486745 mltlk-0.1.1/
+-rw-r--r--   0 johanhagelback   (503) staff       (20)     1073 2023-05-25 10:25:18.000000 mltlk-0.1.1/LICENSE
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      233 2023-05-26 08:15:31.485739 mltlk-0.1.1/PKG-INFO
+-rw-r--r--   0 johanhagelback   (503) staff       (20)       51 2023-05-25 10:25:18.000000 mltlk-0.1.1/README.md
+-rw-r--r--   0 johanhagelback   (503) staff       (20)    31455 2023-05-26 08:12:45.000000 mltlk-0.1.1/Spiral.ipynb
+-rw-r--r--   0 johanhagelback   (503) staff       (20)    19563 2023-05-26 08:12:40.000000 mltlk-0.1.1/Weather.ipynb
+-rw-r--r--   0 johanhagelback   (503) staff       (20)    50437 2023-05-26 07:57:41.000000 mltlk-0.1.1/Wikipedia.ipynb
+-rw-r--r--   0 johanhagelback   (503) staff       (20)    49725 2023-05-26 08:00:41.000000 mltlk-0.1.1/Wikipedia_word2vec.ipynb
+drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-26 08:15:31.465655 mltlk-0.1.1/data/
+-rw-r--r--   0 johanhagelback   (503) staff       (20)     4505 2021-03-10 11:22:51.000000 mltlk-0.1.1/data/spiral.csv
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      414 2023-05-26 08:09:41.000000 mltlk-0.1.1/data/weather.csv
+-rw-r--r--   0 johanhagelback   (503) staff       (20)  2061699 2019-12-13 13:20:58.000000 mltlk-0.1.1/data/wikipedia_300.csv.gz
+drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-26 08:15:31.476845 mltlk-0.1.1/mltlk/
+-rwxr-xr-x   0 johanhagelback   (503) staff       (20)       73 2023-05-26 07:57:16.000000 mltlk-0.1.1/mltlk/__init__.py
+-rw-r--r--   0 johanhagelback   (503) staff       (20)    29402 2023-05-26 07:56:23.000000 mltlk-0.1.1/mltlk/ml.py
+-rw-r--r--   0 johanhagelback   (503) staff       (20)     3324 2023-05-25 12:08:40.000000 mltlk-0.1.1/mltlk/resampling.py
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      337 2023-05-25 12:06:32.000000 mltlk-0.1.1/mltlk/utils.py
+-rw-r--r--   0 johanhagelback   (503) staff       (20)     4978 2023-05-26 07:38:19.000000 mltlk-0.1.1/mltlk/word2vec.py
+drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-26 08:15:31.484136 mltlk-0.1.1/mltlk.egg-info/
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      233 2023-05-26 08:15:30.000000 mltlk-0.1.1/mltlk.egg-info/PKG-INFO
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      380 2023-05-26 08:15:31.000000 mltlk-0.1.1/mltlk.egg-info/SOURCES.txt
+-rw-r--r--   0 johanhagelback   (503) staff       (20)        1 2023-05-26 08:15:30.000000 mltlk-0.1.1/mltlk.egg-info/dependency_links.txt
+-rw-r--r--   0 johanhagelback   (503) staff       (20)       74 2023-05-26 08:15:31.000000 mltlk-0.1.1/mltlk.egg-info/requires.txt
+-rw-r--r--   0 johanhagelback   (503) staff       (20)        6 2023-05-26 08:15:31.000000 mltlk-0.1.1/mltlk.egg-info/top_level.txt
+-rw-r--r--   0 johanhagelback   (503) staff       (20)       38 2023-05-26 08:15:31.487138 mltlk-0.1.1/setup.cfg
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      361 2023-05-26 07:57:08.000000 mltlk-0.1.1/setup.py
```

### Comparing `mltlk-0.1.0/LICENSE` & `mltlk-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mltlk-0.1.0/Wikipedia.ipynb` & `mltlk-0.1.1/Wikipedia_word2vec.ipynb`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9548055872882262%*

 * *Differences: {"'cells'": "{1: {'outputs': [OrderedDict([('name', 'stdout'), ('output_type', 'stream'), ('text', "*

 * *            "['0.1.1\\n'])])], 'source': {insert: [(0, 'import mltlk\\n'), (1, "*

 * *            "'print(mltlk.__version__)\\n')]}}, 2: {'source': ['## Load data\\n', 'Load data, "*

 * *            "clean text and use Word2vec word vectors preprocessing.']}, 3: {'outputs': {0: "*

 * *            "{'text': {insert: [(1, '\\x1b[1m\\x1b[33mInfo: \\x1b[0mUsed stopwords "*

 * *            "\\x1b[36menglish\\x1b[0m\\n'), (2, '\\x1b[ […]*

```diff
@@ -7,63 +7,83 @@
                 "## Imports"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "0.1.1\n"
+                    ]
+                }
+            ],
             "source": [
+                "import mltlk\n",
+                "print(mltlk.__version__)\n",
                 "from mltlk import *"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "tags": []
             },
             "source": [
-                "## Load bag-of-words data"
+                "## Load data\n",
+                "Load data, clean text and use Word2vec word vectors preprocessing."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "\u001b[1m\u001b[33mInfo: \u001b[0mClean texts keeping letters and digits\n",
-                        "\u001b[1m\u001b[33mInfo: \u001b[0mUsed bag-of-words with stopwords \u001b[36menglish\u001b[0m removed\n",
-                        "\u001b[1m\u001b[33mInfo: \u001b[0mUsed TF-IDF\n",
+                        "\u001b[1m\u001b[33mInfo: \u001b[0mUsed stopwords \u001b[36menglish\u001b[0m\n",
+                        "\u001b[1m\u001b[33mInfo: \u001b[0mWord2vec model generated in \u001b[34m4.61\u001b[0m sec\n",
+                        "\u001b[1m\u001b[33mInfo: \u001b[0mWord2vec model stored to \u001b[36mword2vec/wikipedia_300_75.w2v\u001b[0m\n",
+                        "\u001b[1m\u001b[33mInfo: \u001b[0mWord2vec embeddings generated in \u001b[34m14.45\u001b[0m sec\n",
+                        "\u001b[1m\u001b[33mInfo: \u001b[0mWord2vec embeddings stored to \u001b[36mword2vec/wikipedia_300_75.emb\u001b[0m\n",
                         "\u001b[1m\u001b[33mInfo: \u001b[0mLoaded \u001b[34m300\u001b[0m examples in \u001b[34m2\u001b[0m categories\n"
                     ]
                 }
             ],
             "source": [
-                "session = load_data(\"data/wikipedia_300.csv\", conf={\n",
-                "    \"bag-of-words\": True,\n",
-                "    \"encode_labels\": False,\n",
-                "    \"TF-IDF\": True,\n",
+                "session = load_data(\"data/wikipedia_300.csv.gz\", conf={\n",
+                "    \"preprocess\": \"word2vec\",\n",
+                "    \"w2v_vector_size\": 75,\n",
                 "    \"stopwords\": \"english\",\n",
-                "    \"clean_text\": 2,\n",
+                "    \"clean_text\": \"letters digits\",\n",
                 "})"
             ]
         },
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "#### Show data stats"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Acc</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>No</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>%</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>\u03a3%</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Acc</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>No</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>%</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>\u03a3%</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Acc</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>No</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>%</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>\u03a3%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#666;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Games</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>150</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>50.0%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:green;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>50.0%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#666;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Programming</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>150</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>50.0%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:green;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>100.0%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#666;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'></td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'></td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'></td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:green;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'></td></tr></table>"
+                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Category</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>No</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>%</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>\u03a3%</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Category</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>No</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>%</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>\u03a3%</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Category</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>No</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>%</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>\u03a3%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#666;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Games</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>150</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>50.0%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:green;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>50.0%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#666;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Programming</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>150</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>50.0%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:green;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>100.0%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#666;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'></td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'></td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'></td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:green;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'></td></tr><tr><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#666;row-toggle-background:0;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;'>Examples:</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;row-toggle-background:0;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;'>300</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;row-toggle-background:0;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;'></td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:green;row-toggle-background:0;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;'></td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#666;row-toggle-background:0;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;'>Features:</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;row-toggle-background:0;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;'>75</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;row-toggle-background:0;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;'></td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:green;row-toggle-background:0;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;'></td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#666;row-toggle-background:0;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;'>Categories:</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;row-toggle-background:0;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;'>2</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;row-toggle-background:0;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;'></td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:green;row-toggle-background:0;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;'></td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -73,62 +93,35 @@
                 "data_stats(session)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Split into train and test set"
+                "## Evaluate model using cross-validation\n",
+                "Build a LinearSVC model and evaluate results using 10-fold cross-validation."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "\u001b[1m\u001b[33mInfo: \u001b[0mSplit data using \u001b[34m85%\u001b[0m training data and \u001b[34m15%\u001b[0m test data with seed \u001b[34m4\u001b[0m and stratify\n"
-                    ]
-                }
-            ],
-            "source": [
-                "split_data(session, conf={\n",
-                "    \"test_size\": 0.15,\n",
-                "    \"seed\": 4,\n",
-                "    \"stratify\": True,\n",
-                "})"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "## Evaluate model using cross-validation"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 5,
-            "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "Building and evaluating model using 10-fold cross validaton took \u001b[34m0.3591\u001b[0m sec\n",
+                        "Building and evaluating model using 10-fold cross validaton took \u001b[34m0.16\u001b[0m sec\n",
                         "\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
-                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'></td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Accuracy:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>95.33%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>F1-score:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>95.33%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Precision:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>95.37%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Recall:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>95.33%</td></tr></table>"
+                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Results</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Accuracy:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>93.33%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>F1-score:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>93.33%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Precision:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>93.34%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Recall:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>93.33%</td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -139,15 +132,15 @@
                     "text": [
                         "\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
-                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;row-toggle-background:0;'>Category</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;row-toggle-background:0;'>Accuracy</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;row-toggle-background:0;'>n</td></tr><tr><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#048512;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>Programming</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>96.67%</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#3b08d3;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>150</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#fd8e8a;font-family:Verdana;font-size:12px;font:Verdana 12px;'>&nbsp;&nbsp;Games</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;num-format:pct-2;font-family:Verdana;font-size:12px;font:Verdana 12px;'>3.33%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;font-family:Verdana;font-size:12px;font:Verdana 12px;'>5</td></tr><tr><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#048512;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>Games</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>94.00%</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#3b08d3;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>150</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#fd8e8a;font-family:Verdana;font-size:12px;border-bottom:1px solid #aaa;font:Verdana 12px;'>&nbsp;&nbsp;Programming</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;num-format:pct-2;font-family:Verdana;font-size:12px;border-bottom:1px solid #aaa;font:Verdana 12px;'>6.00%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;font-family:Verdana;font-size:12px;border-bottom:1px solid #aaa;font:Verdana 12px;'>9</td></tr></table>"
+                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;row-toggle-background:0;'>Category</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;row-toggle-background:0;'>Accuracy</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;row-toggle-background:0;'>n</td></tr><tr><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#048512;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>Programming</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>94.00%</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#3b08d3;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>150</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#fd8e8a;font-family:Verdana;font-size:12px;font:Verdana 12px;'>&nbsp;&nbsp;Games</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;num-format:pct-2;font-family:Verdana;font-size:12px;font:Verdana 12px;'>6.00%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;font-family:Verdana;font-size:12px;font:Verdana 12px;'>9</td></tr><tr><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#048512;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>Games</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>92.67%</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#3b08d3;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>150</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#fd8e8a;font-family:Verdana;font-size:12px;border-bottom:1px solid #aaa;font:Verdana 12px;'>&nbsp;&nbsp;Programming</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;num-format:pct-2;font-family:Verdana;font-size:12px;border-bottom:1px solid #aaa;font:Verdana 12px;'>7.33%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;font-family:Verdana;font-size:12px;border-bottom:1px solid #aaa;font:Verdana 12px;'>11</td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -157,15 +150,15 @@
                     "output_type": "stream",
                     "text": [
                         "\n"
                     ]
                 },
                 {
                     "data": {
-                        "image/png": "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\n",
+                        "image/png": "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+0ySlJiYqNOnT+udd96RJE2cOFELFy7U7Nmz9dNPP2nw4MHq2rWrNm/eLOlqUOnUqZPatm2r3bt364UXXtCrr75a6PfEy8tL8+fP188//6x33nlHc+bM0dSpU236HDp0SEuXLtWqVav01VdfadeuXerTp491+eLFi/X6669r/Pjx2r9/vyZMmKCRI0dqwYIFha4HuCYLABRAZGSkpX379haLxWIxm82W9evXW1xcXCxRUVHW5YGBgZYrV65Y11m0aJElPDzcYjabrW1XrlyxuLm5WdauXWuxWCyWcuXKWd58803r8qysLEuFChWs+7JYLJaHHnrIMnDgQIvFYrEkJiZaJFnWr1+fb52bNm2ySLL88ccf1rbLly9b3N3dLd9++61N3549e1qeeeYZi8VisYwYMcJSo0YNm+XDhw/Ps62/k2T5/PPPr7n8rbfestSrV8/6etSoURZnZ2fLiRMnrG1ffvmlxcnJyXL69GmLxWKxVKlSxfLRRx/ZbGfs2LGWhg0bWiwWiyUpKckiybJr165r7hf4J8wBAFBgsbGx8vT0VFZWlsxms5599llFR0dbl0dERNhc99+zZ48OHTokLy8vm+1cvnxZhw8fVkpKik6fPq17773XuqxEiRK655578lwGyLV79245OzvroYceKnDdhw4dUkZGhh555BGb9szMTNWtW1eStH//fps6JKlhw4YF3keuTz75RNOnT9fhw4eVlpam7OxseXt72/SpWLGiypcvb7Mfs9msxMREeXl56fDhw+rZs6defPFFa5/s7Gz5+PgUuh7gWggAAAqsadOmmjVrlkqVKqWgoCCVKGH7J+Sv3/YmSWlpaapXr54WL16cZ1t33HHHDdXg5uZW6HXS0tIkSatXr7b54JVk8611N2vbtm3q0qWLRo8erZYtW8rHx0dLlizR5MmTC13rnDlz8gQSZ2dnu9UKEAAAFJiHh4fCwsIK3P/uu+/WJ598ooCAgDxnwbnKlSun77//Xo0bN5Z09Uw3ISFBd999d779IyIiZDabtXnzZjVv3jzP8twRiJycHGtbjRo15OLiouPHj19z5KB69erWCY25vvvuu38+yL/49ttvValSJf3nP/+xth07dixPv+PHj+vUqVMKCgqy7sfJyUnh4eEKDAxUUFCQjhw5oi5duhRq/0BhMAkQQJHp0qWLypQpo/bt22vLli1KSkrS119/rQEDBujEiROSpIEDB+qNN97QihUrdODAAfXp0+e69/CHhIQoMjJSzz//vFasWGHd5tKlSyVJlSpVkslkUmxsrM6fP6+0tDR5eXkpKipKgwcP1oIFC3T48GHt3LlTM2bMsE6s69Wrl3755Re98sorSkxM1EcffaT58+cX6njvvPNOHT9+XEuWLNHhw4c1ffr0fCc0urq6KjIyUnv27NGWLVs0YMAAde7cWWXLlpUkjR49WhMnTtT06dN18OBB7d27VzExMZoyZUqh6gGuhwAAoMi4u7vrm2++UcWKFdWpUydVr15dPXv21OXLl60jAkOHDlW3bt0UGRmphg0bysvLSx07drzudmfNmqUnnnhCffr0UbVq1fTiiy8qPT1dklS+fHmNHj1ar776qgIDA9WvXz9J0tixYzVy5EhNnDhR1atXV6tWrbR69WpVrlxZ0tXr8p999plWrFih2rVra/bs2ZowYUKhjrddu3YaPHiw+vXrpzp16ujbb7/VyJEj8/QLCwtTp06d1Lp1a7Vo0UK1atWyuc3vhRde0Ny5cxUTE6OIiAg99NBDmj9/vrVWwB5MlmvNtAEAALctRgAAADAgAgAAAAZEAAAAwIAIAAAAGBABAAAAAyIAAABgQAQAAAAMiAAAAIABEQAAADAgAgAAAAZEAAAAwID+DyaguQYU/MexAAAAAElFTkSuQmCC\n",
                         "text/plain": [
                             "<Figure size 640x480 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
@@ -174,116 +167,33 @@
                     "output_type": "stream",
                     "text": [
                         "\n"
                     ]
                 }
             ],
             "source": [
-                "evaluate_model(LinearSVC(C=1), session, reload=False, conf={\n",
+                "evaluate_model(LinearSVC(), session, reload=False, conf={\n",
                 "    \"mode\": \"CV-10\",\n",
                 "    \"categories\": True,\n",
                 "    \"confusion_matrix\": True,\n",
                 "    \"seed\": 42,\n",
                 "})"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Build final model"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 6,
-            "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "Building final model on all data took \u001b[36m0.0479\u001b[0m sec\n"
-                    ]
-                }
-            ],
-            "source": [
-                "build_model(LinearSVC(C=1), session, conf={\n",
-                "    \"mode\": \"all\",\n",
-                "})"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "## Save session"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 7,
-            "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "\u001b[1m\u001b[33mInfo: \u001b[0mSession saved to \u001b[34msessions/wikipedia.gz\u001b[0m\n"
-                    ]
-                }
-            ],
-            "source": [
-                "save_session(session, \"sessions/wikipedia\")    "
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "## Load word2vec data"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 8,
-            "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "\u001b[1m\u001b[33mInfo: \u001b[0mClean texts keeping letters and digits\n",
-                        "\u001b[1m\u001b[31mWarning: \u001b[0m\u001b[36mw2v_vector_size\u001b[0m not set (using \u001b[34m75\u001b[0m)\n",
-                        "\u001b[1m\u001b[33mInfo: \u001b[0mWord2vec model generated in \u001b[34m4.79\u001b[0m sec\n",
-                        "\u001b[1m\u001b[33mInfo: \u001b[0mWord2vec model stored to \u001b[36mword2vec/wikipedia_300_75.w2v\u001b[0m\n",
-                        "\u001b[1m\u001b[33mInfo: \u001b[0mWord2vec embeddings generated in \u001b[34m14.56\u001b[0m sec\n",
-                        "\u001b[1m\u001b[33mInfo: \u001b[0mWord2vec embeddings stored to \u001b[36mword2vec/wikipedia_300_75.emb\u001b[0m\n",
-                        "\u001b[1m\u001b[33mInfo: \u001b[0mLoaded \u001b[34m300\u001b[0m examples in \u001b[34m2\u001b[0m categories\n"
-                    ]
-                }
-            ],
-            "source": [
-                "session = load_data(\"data/wikipedia_300.csv\", conf={\n",
-                "    \"word2vec\": True,\n",
-                "    \"stopwords\": \"english\",\n",
-                "    \"clean_text\": 2,\n",
-                "})"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "## Evaluate model using train-test split"
+                "## Evaluate model using train-test split\n",
+                "Build a LinearSVC model and evaluate results using train-test split."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 5,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "\u001b[1m\u001b[33mInfo: \u001b[0mSplit data using \u001b[34m85%\u001b[0m training data and \u001b[34m15%\u001b[0m test data with seed \u001b[34m4\u001b[0m and stratify\n"
@@ -291,44 +201,53 @@
                 }
             ],
             "source": [
                 "split_data(session, conf={\n",
                 "    \"test_size\": 0.15,\n",
                 "    \"seed\": 4,\n",
                 "    \"stratify\": True,\n",
-                "    \"categories\": True,\n",
-                "    \"confusion_matrix\": True,\n",
                 "})"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Building and evaluating model using train-test split took \u001b[34m0.9034\u001b[0m sec\n",
+                        "Building and evaluating model using 10-fold cross validaton took \u001b[34m0.16\u001b[0m sec\n",
                         "\n"
                     ]
                 },
                 {
-                    "name": "stderr",
+                    "data": {
+                        "text/html": [
+                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Results</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Accuracy:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>93.33%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>F1-score:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>93.33%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Precision:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>93.34%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Recall:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>93.33%</td></tr></table>"
+                        ],
+                        "text/plain": [
+                            "<IPython.core.display.HTML object>"
+                        ]
+                    },
+                    "metadata": {},
+                    "output_type": "display_data"
+                },
+                {
+                    "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "/usr/local/lib/python3.11/site-packages/sklearn/neural_network/_multilayer_perceptron.py:686: ConvergenceWarning: Stochastic Optimizer: Maximum iterations (500) reached and the optimization hasn't converged yet.\n",
-                        "  warnings.warn(\n"
+                        "\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
-                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'></td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Accuracy:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>91.11%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>F1-score:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>91.11%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Precision:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>91.11%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Recall:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>91.11%</td></tr></table>"
+                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;row-toggle-background:0;'>Category</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;row-toggle-background:0;'>Accuracy</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;row-toggle-background:0;'>n</td></tr><tr><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#048512;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>Programming</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>94.00%</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#3b08d3;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>150</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#fd8e8a;font-family:Verdana;font-size:12px;font:Verdana 12px;'>&nbsp;&nbsp;Games</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;num-format:pct-2;font-family:Verdana;font-size:12px;font:Verdana 12px;'>6.00%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;font-family:Verdana;font-size:12px;font:Verdana 12px;'>9</td></tr><tr><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#048512;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>Games</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>92.67%</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#3b08d3;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>150</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#fd8e8a;font-family:Verdana;font-size:12px;border-bottom:1px solid #aaa;font:Verdana 12px;'>&nbsp;&nbsp;Programming</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;num-format:pct-2;font-family:Verdana;font-size:12px;border-bottom:1px solid #aaa;font:Verdana 12px;'>7.33%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;font-family:Verdana;font-size:12px;border-bottom:1px solid #aaa;font:Verdana 12px;'>11</td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -338,19 +257,54 @@
                     "output_type": "stream",
                     "text": [
                         "\n"
                     ]
                 }
             ],
             "source": [
-                "evaluate_model(MLPClassifier(max_iter=500), session, reload=False, conf={\n",
-                "    \"mode\": \"split\",\n",
+                "evaluate_model(LinearSVC(), session, reload=False, conf={\n",
+                "    \"mode\": \"CV-10\",\n",
+                "    \"categories\": True,\n",
                 "    \"seed\": 42,\n",
                 "})"
             ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## Build final model and predict example\n",
+                "Build final model using all data and predict an unknown example."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 7,
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "\u001b[1m\u001b[33mInfo: \u001b[0mBuilding final model on all data took \u001b[36m0.02\u001b[0m sec\n",
+                        "\u001b[1m\u001b[33mInfo: \u001b[0mExample is predicted as \u001b[32mGames\u001b[0m\n"
+                    ]
+                }
+            ],
+            "source": [
+                "build_model(LinearSVC(), session)\n",
+                "predict(\"This is an article about gamers - people who love playing games\", session)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
```

### Comparing `mltlk-0.1.0/mltlk/ml.py` & `mltlk-0.1.1/mltlk/ml.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,68 +3,66 @@
 import numpy as np
 import pandas as pd
 from collections import Counter
 from customized_table import *
 import time
 import matplotlib.pyplot as plt
 import re
+from .utils import *
 # Pre-processing
 from sklearn.preprocessing import LabelEncoder
 from sklearn.feature_extraction.text import CountVectorizer, TfidfTransformer
 from sklearn.model_selection import train_test_split
 from nltk.corpus import stopwords
+from sklearn.preprocessing import StandardScaler
+from sklearn.preprocessing import Normalizer
+from sklearn.preprocessing import OneHotEncoder
+from sklearn.preprocessing import OrdinalEncoder
 # Classifiers
 from sklearn.naive_bayes import MultinomialNB
 from sklearn.svm import LinearSVC
 from sklearn.neural_network import MLPClassifier
 from sklearn.ensemble import RandomForestClassifier
 # Evaluation
-from sklearn.model_selection import cross_val_predict
 from sklearn.metrics import accuracy_score, f1_score, recall_score, precision_score, confusion_matrix, ConfusionMatrixDisplay
 # File stuff
 from pickle import dump,load
 from os.path import exists
 from os import makedirs
 import gzip
 # Resampling
 from .resampling import resample
 from .word2vec import *
 
 
 #
-# Error message
-#
-def error(e):
-    print(colored("Error: ", "red", attrs=["bold"]) + e)
-
-    
-#
-# Warning message
-#
-def warning(e):
-    print(colored("Warning: ", "red", attrs=["bold"]) + e)
-    
-
-#
-# Info message
-#
-def info(e):
-    print(colored("Info: ", "yellow", attrs=["bold"]) + e)
-
-
-#
 # Load and pre-process data
 #
-def load_data(file, Xcols=[0], ycol=1, verbose=1, conf={}):
+def load_data(file, Xcols=None, ycol=None, verbose=1, conf={}):
     session = {}
     
+    # Check config
+    if "preprocess" not in conf:
+        conf["preprocess"] = ""
+    conf["preprocess"] = conf["preprocess"].lower()
+    
     # Load data
+    if not exists(file):
+        error("data file " + colored(file, "cyan") + " not found")
+        return None
     data = pd.read_csv(file).values
     session["file"] = file
     
+    # Set X features to be all but last column
+    if Xcols is None:
+        Xcols = range(0,len(data[0]) - 1)
+    # Set y to be last column
+    if ycol is None:
+        ycol = len(data[0]) - 1
+    
     # Convert to X and y
     X = []
     y = []
     for r in data:
         row = []
         for c,val in enumerate(r):
             if c in Xcols:
@@ -97,47 +95,66 @@
         if verbose >= 1:
             s = ""
             for li,ni in cnt.items():
                 if ni < conf["min_samples"]:
                     s += li + ", "
             if s != "":
                 info("Removed minority categories " + colored(s[:-2], "cyan"))
-                
-    # Clean inputs
-    if "clean_text" in conf:
-        if conf["clean_text"] == 2 or conf["clean_text"] == "digits":
-            info("Clean texts keeping letters and digits")
-        else:
-            info("Clean texts keeping letters only")    
-        for i,xi in enumerate(session["X"]):
-            # Remove new line and whitespaces
-            xi = xi.replace("<br>", " ")
-            xi = xi.replace("&nbsp;", " ")
-            # Remove special chars
-            if conf["clean_text"] == 2 or conf["clean_text"] == "digits":
-                xi = re.sub("[^a-zA-Z0-9åäöÅÄÖ ]", " ", xi)
-            else:
-                xi = re.sub("[^a-zA-ZåäöÅÄÖ ]", " ", xi)
-            # Remove multiple whitespaces
-            xi = " ".join(xi.split())
-            # Set to lower case
-            xi = xi.lower()
-            # Strip trailing/leading whitespaces
-            xi = xi.strip()
-            session["X"][i] = xi
-            
+    
     # Encode labels
     if "encode_labels" in conf and conf["encode_labels"]:
         session["label_encoder"] = LabelEncoder().fit(session["y"])
         session["y"] = session["label_encoder"].transform(session["y"])
         if verbose >= 1:
             info("Labels encoded")
+            
+    # Check text inputs without text preprocessing
+    if conf["preprocess"] not in ["bag-of-words", "bow", "wordtovec", "word2vec"]:
+        if type(X[0]) == str:
+            error("Input seems to be text but no text-preprocessing is set")
+            return None
+        
+    # Check ordinal features without encoding
+    if conf["preprocess"] not in ["one-hot", "onehot", "one hot", "ordinal"]:
+        if type(X[0]) != str:
+            for xi in X[0]:
+                if type(xi) == str:
+                    error("Input contains ordinal features but no encoding is set (use " + colored("one-hot", "blue") + " or " + colored("ordinal", "blue") + ")")
+                    return None
+    
+    # Clean text inputs
+    if "clean_text" in conf and conf["preprocess"] in ["word2vec", "bag-of-words", "bow"]:
+        clean = True
+        if conf["clean_text"] in [2, "letters digits", "digits letters"]:
+            info("Clean texts keeping letters and digits")
+        elif conf["clean_text"] in [1, "letters"]:
+            info("Clean texts keeping letters only")
+        else:
+            warning("Invalid clean text mode " + colored(conf["clean_text"], "cyan"))
+            clean = False
+        if clean:
+            for i,xi in enumerate(session["X"]):
+                # Remove new line and whitespaces
+                xi = xi.replace("<br>", " ")
+                xi = xi.replace("&nbsp;", " ")
+                # Remove special chars
+                if conf["clean_text"] in [2, "letters digits", "digits letters"]:
+                    xi = re.sub("[^a-zA-Z0-9åäöÅÄÖ ]", " ", xi)
+                else:
+                    xi = re.sub("[^a-zA-ZåäöÅÄÖ ]", " ", xi)
+                # Remove multiple whitespaces
+                xi = " ".join(xi.split())
+                # Set to lower case
+                xi = xi.lower()
+                # Strip trailing/leading whitespaces
+                xi = xi.strip()
+                session["X"][i] = xi
     
     # Bag-of-words representation for input texts
-    if "bag-of-words" in conf and conf["bag-of-words"]:
+    if conf["preprocess"] in ["bag-of-words", "bow"]:
         if "stopwords" in conf:
             sw = list(stopwords.words(conf["stopwords"]))
             if verbose >= 1:
                 info("Used bag-of-words with stopwords " + colored(conf["stopwords"], "cyan") + " removed")
         else:
             sw = None
             if verbose >= 1:
@@ -148,27 +165,62 @@
         # TF-IDF conversion for bag-of-words
         if "TF-IDF" in conf and conf["TF-IDF"] or "tf-idf" in conf and conf["tf-idf"]:
             session["TF-IDF"] = TfidfTransformer().fit(session["X"])
             session["X"] = session["TF-IDF"].transform(session["X"])
             if verbose >= 1:
                 info("Used TF-IDF")
     # Word2vec
-    if "word2vec" in conf and conf["word2vec"]:
+    if conf["preprocess"] in ["word2vec", "wordtovec"]:
         load_word2vec_data(session, conf, verbose=verbose)
         
+    # One-hot encoding
+    if conf["preprocess"] in ["one-hot", "onehot", "one hot"]:
+        session["scaler"] = OneHotEncoder(handle_unknown="ignore").fit(session["X"])
+        session["X"] = session["scaler"].transform(session["X"])
+        if verbose >= 1:
+            info("Transformed input data using one-hot encoding")
+            
+    # Ordinal encoding
+    if conf["preprocess"] in ["ordinal"]:
+        session["scaler"] = OrdinalEncoder().fit(session["X"])
+        session["X"] = session["scaler"].transform(session["X"])
+        if verbose >= 1:
+            info("Transformed input data using ordinal encoding")
+        
+    # Standard scaler
+    if conf["preprocess"] == "scale":
+        session["scaler"] = StandardScaler().fit(session["X"])
+        session["X"] = session["scaler"].transform(session["X"])
+        if verbose >= 1:
+            info("Scaled input data using standard scaler")
+            
+    # Normalize
+    if conf["preprocess"] == "normalize":
+        session["scaler"] = Normalizer().fit(session["X"])
+        session["X"] = session["scaler"].transform(session["X"])
+        if verbose >= 1:
+            info("Normalized input data")
+            
+    # Set mode in session
+    session["preprocess"] = conf["preprocess"]
+        
     if verbose >= 1:
         info("Loaded " + colored(f"{len(session['y'])}", "blue") + " examples in " + colored(f"{len(Counter(session['y']))}", "blue") + " categories")
     
     return session
 
 
 #
 # Show data stats
 #
 def data_stats(session, max_rows=None, show_graph=False, descriptions=None):
+    if session is None:
+        error("Session is empty")
+        return
+    
     y = session["y"]
     cnt = Counter(y)
     tab = []
     for key,no in cnt.items():
         tab.append([key,no,f"{no/len(y)*100:.1f}%"])
     tab = sorted(tab, key=lambda x: x[1], reverse=True)
     rno = 0
@@ -202,22 +254,22 @@
     for i,r in enumerate(tab):
         tab2[c].append(r)
         if (i+1) % s == 0:
             c += 1
     
     # Show table
     if descriptions is not None:
-        t = CustomizedTable(["Acc", "No", "%", "Σ%", "Description", "Acc", "No", "%", "Σ%", "Description", "Acc", "No", "%", "Σ%", "Description"])
+        t = CustomizedTable(["Category", "No", "%", "Σ%", "Description", "Category", "No", "%", "Σ%", "Description", "Category", "No", "%", "Σ%", "Description"])
         t.column_style([0,5,10], {"color": "id"})
         t.column_style([1,6,11], {"color": "value"})
         t.column_style([2,7,12], {"color": "percent"})
         t.column_style([3,8,13], {"color": "green"})
         t.column_style([4,9,14], {"color": "name"})
     else:
-        t = CustomizedTable(["Acc", "No", "%", "Σ%", "Acc", "No", "%", "Σ%", "Acc", "No", "%", "Σ%"])
+        t = CustomizedTable(["Category", "No", "%", "Σ%", "Category", "No", "%", "Σ%", "Category", "No", "%", "Σ%"])
         t.column_style([0,4,8], {"color": "id"})
         t.column_style([1,5,9], {"color": "value"})
         t.column_style([2,6,10], {"color": "percent"})
         t.column_style([3,7,11], {"color": "green"})
     for i in range(0,s):
         r = []
         for j in range(0,3):
@@ -232,59 +284,87 @@
                         desc = descriptions[tab2[j][i][0]]
                     r.append(desc)
         # Fill row, if not full
         rsize = 15
         if descriptions is None:
             rsize = 12
         if len(r) < rsize:
-            for i in range(rsize - len(r)):
-                r.append("")
+            i = rsize - len(r)
+            r += [""] * (i)
         t.add_row(r)
+    
+    # Overall stats
+    if type(session["X"]) == list:
+        fts = len(session["X"][0])
+    else:
+        fts = session["X"].shape[1]
+    if descriptions is not None:
+        t.add_row(["Examples:", len(session["y"]), "", "", "", "Features:", fts, "", "", "", "Categories:", len(cnt), "", "", ""], style={"row-toggle-background": 0, "background": "#eee", "border": "top"})
+        t.cell_style([0,5,10], -1, {"font": "bold"})
+    else:
+        t.add_row(["Examples:", len(session["y"]), "", "", "Features:", fts, "", "", "Categories:", len(cnt), "", ""], style={"row-toggle-background": 0, "background": "#eee", "border": "top"})
+        t.cell_style([0,4,8], -1, {"font": "bold"})
+    
     t.display()
 
 
 #
 # Split data into train and test sets
 #
 def split_data(session, verbose=1, conf={}):
-    # Test size
-    test_size = 0.15
+    if session is None:
+        error("Session is empty")
+        return
+    
+    # Check test size
     if "test_size" in conf:
         test_size = conf["test_size"]
-    s = "Split data using " + colored(f"{(1-test_size)*100:.0f}%", "blue") + " training data and " + colored(f"{(test_size)*100:.0f}%", "blue") + " test data"
+    else:
+        conf["test_size"] = 0.2
+        warning(colored("test_size", "cyan") + " not set (using " + colored("0.2", "blue") + ")")
+        
+    # Info string
+    s = "Split data using " + colored(f"{(1-conf['test_size'])*100:.0f}%", "blue") + " training data and " + colored(f"{(conf['test_size'])*100:.0f}%", "blue") + " test data"
     
     # Random seed
     seed = None
     if "seed" in conf:
         seed = conf["seed"]
         s += " with seed " + colored(seed, "blue") 
         
     # Stratify
     stratify = None
     if "stratify" in conf and conf["stratify"]:
         stratify = session["y"]
         s += " and stratify"
     
     # Split data
-    X_train, X_test, y_train, y_test = train_test_split(session["X"], session["y"], test_size=test_size, random_state=seed, stratify=stratify)
+    X_train, X_test, y_train, y_test = train_test_split(session["X"], session["y"], test_size=conf["test_size"], random_state=seed, stratify=stratify)
     
     # Update session
     session["X_train"] = X_train
     session["X_test"] = X_test
     session["y_train"] = y_train
     session["y_test"] = y_test
+    if "mode" in session:
+        # Trigger reload
+        session["mode"] = ""
     
     if verbose >= 1:
         info(s)
 
 
 #
 # Sets resampling method to use
 #
 def set_resample(session, conf={}):
+    if session is None:
+        error("Session is empty")
+        return
+    
     # Check mode parameter
     if "mode" not in conf:
         error("Missing parameter " + colored("mode", "cyan"))
         return
     if type(conf["mode"]) != str:
         error("Resample mode must be a string")
         return
@@ -347,23 +427,32 @@
         session["mode"] = ""
 
 
 #
 # Builds and evaluates model
 #
 def evaluate_model(model, session, reload=False, conf={}):
+    if session is None:
+        error("Session is empty")
+        return
+    
+    # Check mode param
+    if "mode" not in conf:
+        conf["mode"] = "all"
+        warning(colored("mode", "cyan") + " not set (using " + colored("all", "blue") + ")")
+        
     # Check if rebuild model
     if "mode" in conf and "mode" in session and conf["mode"] != session["mode"]:
         reload = True
     if "modelid" in session and session["modelid"] != str(model):
         reload = True
     
     # Build model and predict data (if not already built)
     if "y_pred" not in session or reload:
-        if "mode" in conf and (conf["mode"].startswith("CV") or conf["mode"].startswith("cv")):
+        if conf["mode"].lower().startswith("cv"):
             st = time.time()
             cv = 5
             if len(conf["mode"]) > 2:
                 if "-" in conf["mode"]: 
                     cv = int(conf["mode"].split("-")[1])
                 elif " " in conf["mode"]:
                     cv = int(conf["mode"].split(" ")[1])
@@ -399,43 +488,46 @@
                 model_obj.fit(X_train, y_train)
                 y_pred += list(model_obj.predict(X_test))
                 y_actual += list(y_test)
             session["y_pred"] = y_pred
             session["y_actual"] = y_actual
             
             en = time.time()
-            print(f"Building and evaluating model using {cv}-fold cross validaton took " + colored(f"{en-st:.4f}", "blue") + " sec")
-        elif "mode" in conf and (conf["mode"] == "train-test" or conf["mode"] == "split"):
+            print(f"Building and evaluating model using {cv}-fold cross validaton took " + colored(f"{en-st:.2f}", "blue") + " sec")
+        elif conf["mode"].lower() in ["train-test", "split"]:
             st = time.time()
             if "X_train" not in session or "y_train" not in session:
                 error("Data must be split using function " + colored("split_data()", "cyan") + " before evaluating model using train-test split")
                 return
             X_train = session["X_train"]
             y_train = session["y_train"]
             if "resample" in session:
                 X_train, y_train = resample(session, X_train, y_train)
             model.fit(X_train, y_train)
             session["y_pred"] = model.predict(session["X_test"])
             session["y_actual"] = session["y_test"]
             en = time.time()
-            print("Building and evaluating model using train-test split took " + colored(f"{en-st:.4f}", "blue") + " sec")
-        else:
+            print("Building and evaluating model using train-test split took " + colored(f"{en-st:.2f}", "blue") + " sec")
+        elif conf["mode"].lower() in ["all", ""]:
             st = time.time()
             model.fit(session["X"], session["y"])
             session["y_pred"] = model.predict(session["X"])
             session["y_actual"] = session["y"]
             en = time.time()
-            print("Building and evaluating model on all data took " + colored(f"{en-st:.4f}", "blue") + " sec")
+            print("Building and evaluating model on all data took " + colored(f"{en-st:.2f}", "blue") + " sec")
             conf["mode"] = "all"
+        else:
+            warning("Invalid mode " + colored(conf["mode"], "cyan"))
+            return
             
         session["mode"] = conf["mode"]
         session["modelid"] = str(model)
     
     # Results
-    t = CustomizedTable(["", ""])
+    t = CustomizedTable(["Results", ""])
     t.column_style(1, {"color": "percent", "num-format": "pct-2"})
     t.add_row(["Accuracy:", float(accuracy_score(session["y_actual"], session["y_pred"]))])
     t.add_row(["F1-score:", float(f1_score(session["y_actual"], session["y_pred"], average="weighted"))])
     t.add_row(["Precision:", float(precision_score(session["y_actual"], session["y_pred"], average="weighted", zero_division=False))])
     t.add_row(["Recall:", float(recall_score(session["y_actual"], session["y_pred"], average="weighted", zero_division=False))])
     print()
     t.display()
@@ -468,15 +560,15 @@
         for r in tmp[sidx:sidx+maxcats]:
             t.add_row([r[1], float(r[0]), r[2]], style={"border": "top", "background": "#eee"})
             if len(r[3]) > 0:
                 errs = sorted(r[3], reverse=True)
                 if "max_errors" in conf:
                     errs = errs[:conf["max_errors"]]
                 for err in errs:
-                    t.add_row(["&nbsp;&nbsp;" + err[1], float(err[0]/r[2]), err[0]])
+                    t.add_row([f"&nbsp;&nbsp;{err[1]}", float(err[0]/r[2]), err[0]])
                     t.cell_style(0,-1, {"color": "#fd8e8a"})
                     t.cell_style([1,2],-1, {"color": "#aaa4fa"})
         print()
         t.display()
         
     # Confusion matrix
     if "confusion_matrix" in conf and conf["confusion_matrix"]:
@@ -491,49 +583,61 @@
     print()
 
 
 #
 # Builds final model
 #
 def build_model(model, session, conf={}):
-    if "mode" in conf and (conf["mode"] == "train-test" or conf["mode"] == "split"):
+    if session is None:
+        error("Session is empty")
+        return
+    if "mode" not in conf:
+        conf["mode"] = "all"
+    
+    if conf["mode"] in ["train-test", "split"]:
         st = time.time()
         model.fit(session["X_train"], session["y_train"])
         session["model"] = model
         en = time.time()
-        print("Building final model on training data took " + colored(f"{en-st:.4f}", "cyan") + " sec")
-    else:
+        info("Building final model on training data took " + colored(f"{en-st:.2f}", "cyan") + " sec")
+    elif conf["mode"] in ["all", ""]:
         st = time.time()
         model.fit(session["X"], session["y"])
         session["model"] = model
         en = time.time()
-        print("Building final model on all data took " + colored(f"{en-st:.4f}", "cyan") + " sec")
+        info("Building final model on all data took " + colored(f"{en-st:.2f}", "cyan") + " sec")
+    else:
+        error("Invalid mode " + colored(conf["mode"], "cyan"))
 
 
 #
 # Save session to file
 #
-def save_session(session, file, verbose=1):
+def save_session(session, id, verbose=1):
+    if session is None:
+        error("Session is empty")
+        return
+    
     # Check if path exists
-    if "/" in file:
-        path = file[:file.rfind("/")]
-        if not exists(path):
-            makedirs(path)
-    if not file.endswith(".gz"):
-        file += ".gz"
+    fpath = "sessions"
+    if not exists(fpath):
+        mkdir(fpath)
+    
     # Dump to file
+    file = f"sessions/{id}.gz"
     dump(session, gzip.open(file, "wb"))
     if verbose >= 1:
         info("Session saved to " + colored(file, "blue"))
 
 
 #
 # Load session from file
 #
-def load_session(file, verbose=1):
+def load_session(id, verbose=1):
+    file = f"sessions/{id}.gz"
     if not exists(file) and not file.endswith(".gz"):
         file += ".gz"
     if not exists(file):
         error("File " + colored(file, "cyan") + " not found")
         return None
     # Load file
     s = load(gzip.open(file, "rb"))
@@ -542,17 +646,22 @@
     return s
 
 
 #
 # Dump n prediction errors
 #
 def prediction_errors_for_category(session, category, predicted_category=None, sidx=0, n=5):
+    if session is None:
+        error("Session is empty")
+        return
+    
     # Check if model has been built
     if "model" not in session:
         error("Final model has not been built. Use the function " + colored("build_model()", "cyan"))
+        return
     
     # Find n errors
     ht = f"Actual: <id>{category}</>"
     t = CustomizedTable(["Predicted", tag_text(ht)])
     t.column_style(1, {"color": "#e65205"})
     cidx = 0
     for xi_raw,xi,yi in zip(session["X_original"], session["X"], session["y"]):
@@ -570,17 +679,22 @@
     t.display()
     
 
 #
 # Check actual categories for prediction errors where predicted category is specified as param
 #
 def errors_for_predicted_category(session, category, n=None):
+    if session is None:
+        error("Session is empty")
+        return
+    
     # Check if model has been built
     if "model" not in session:
         error("Final model has not been built. Use the function " + colored("build_model()", "cyan"))
+        return
     
     # Get test data
     y_preds = session["model"].predict(session["X_test"])
     y = session["y_test"]
     
     # Find errors where predictions match specified account
     cnt = 0
@@ -614,7 +728,54 @@
     for e in linf:
         t.add_row([e[1], e[0], f"{e[0]/cnt*100:.1f}%", f"{e[0]/tot*100:.1f}%"])
     
     t.add_subheader(["Total:", cnt, "", tag_text(f"(<percent>{cnt/tot*100:.1f}%</> of all <value>{tot}</> errors are predicted as <id>{category}</>)")])
     t.cell_style(0, -1, {"font": "bold"})
     t.cell_style(1, -1, {"color": "value"})
     t.display()
+    
+    
+#
+# Predict example
+#
+def predict(xi, session):
+    if session is None:
+        error("Session is empty")
+        return
+    
+    # Check if model has been built
+    if "model" not in session:
+        error("Final model has not been built. Use the function " + colored("build_model()", "cyan"))
+        return
+    
+    # Error checks
+    if type(xi) == str and session["preprocess"] not in ["bag-of-words", "bow", "word2vec", "wordtovec"]:
+        error("Example is text but no text preprocessing is specified")
+        return
+    
+    # Bag of words
+    if type(xi) == str and session["preprocess"] in ["bag-of-words", "bow"]:
+        X = session["bow"].transform([xi])
+        if "tf-idf" in session:
+            X = session["tf-idf"].transform(X)
+        pred = session["model"].predict(X)
+        info("Example is predicted as " + colored(pred[0], "green"))
+        return
+    
+    # Word2vec
+    if type(xi) == str and session["preprocess"] in ["word2vec", "wordtovec"]:
+        X = [word_vector(xi, session)]
+        pred = session["model"].predict(X)
+        info("Example is predicted as " + colored(pred[0], "green"))
+        return
+    
+    # Numerical/ordinal data
+    if "scaler" in session:
+        X = session["scaler"].transform([xi])
+        pred = session["model"].predict(X)
+        info("Example is predicted as " + colored(pred[0], "green"))
+        return
+    
+    # No pre-processing
+    pred = session["model"].predict([xi])
+    info("Example is predicted as " + colored(pred[0], "green"))
+
```

### Comparing `mltlk-0.1.0/mltlk/resampling.py` & `mltlk-0.1.1/mltlk/resampling.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,16 @@
+# Basic stuff
 from termcolor import colored
+from .utils import *
 from collections import Counter
+# Imbalanced-learn
 from imblearn.over_sampling import RandomOverSampler
 from imblearn.under_sampling import RandomUnderSampler
 from imblearn.over_sampling import SMOTE
-
-
-#
-# Error message
-#
-def error(e):
-    print(colored("Error: ", "red", attrs=["bold"]) + e)
-
-    
-#
-# Warning message
-#
-def warning(e):
-    print(colored("Warning: ", "red", attrs=["bold"]) + e)
-    
-
-#
-# Info message
-#
-def info(e):
-    print(colored("Info: ", "yellow", attrs=["bold"]) + e)
-    
+  
     
 #
 # Random undersampling
 #
 def rnd_undersampling(session, X, y):
     # Set no per label
     lcnt = Counter(y)
```

### Comparing `mltlk-0.1.0/mltlk/word2vec.py` & `mltlk-0.1.1/mltlk/word2vec.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,23 @@
 # Basic stuff
 from termcolor import colored
+from .utils import *
 import time
 # Pre-processing
 from nltk.corpus import stopwords
 # Word2Vec
 from gensim.models import Word2Vec
 # File stuff
 from pickle import dump,load
 from os.path import exists
 from os import mkdir
 import gzip
 
 
 #
-# Error message
-#
-def error(e):
-    print(colored("Error: ", "red", attrs=["bold"]) + e)
-
-    
-#
-# Warning message
-#
-def warning(e):
-    print(colored("Warning: ", "red", attrs=["bold"]) + e)
-    
-
-#
-# Info message
-#
-def info(e):
-    print(colored("Info: ", "yellow", attrs=["bold"]) + e)
-
-
-#
 # Load or build Word2vec model
 #
 def load_word2vec_model(session, conf, verbose=1):
     # Check if path exists
     fpath = "word2vec"
     if not exists(fpath):
         mkdir(fpath)
@@ -60,14 +40,16 @@
         if verbose >= 1:
             info("Word2vec model loaded from " + colored(f"word2vec/{fname}", "cyan"))
         return wtovec
     
     # Stopwords
     if "stopwords" in conf:
         stpwrds = set(stopwords.words(conf["stopwords"]))
+        if verbose >= 1:
+            info("Used stopwords " + colored(conf["stopwords"], "cyan"))
     
     # Convert to list of list of words
     X = []
     for wds in session["X"]:
         xi = []
         for w in wds.split(" "):
             if w not in stpwrds and w.strip() != "":
@@ -161,7 +143,31 @@
     if verbose >= 1:
         info("Word2vec embeddings generated in " + colored(f"{end-start:.2f}", "blue") + " sec")
     
     # Store
     dump([X,y], gzip.open(f"word2vec/{fname}", "wb"))
     if verbose >= 1:
         info("Word2vec embeddings stored to " + colored(f"word2vec/{fname}", "cyan"))
+
+        
+#
+# Create word vector for example
+#
+def word_vector(xi, session):
+    # Get vector size
+    if type(session["X"][0]) == list:
+        size = len(session["X"][0])
+    else:
+        size = session["X"][0].shape[1]
+        
+    # Get Word2Vec model
+    wtovec = load_word2vec_model(session, {"w2v_vector_size": size}, verbose=0)
+        
+    # Generate new word vectors
+    vec = [0] * size
+    for w in xi.lower().split(" "):
+        # Add vectors for each word
+        if w.strip() != "":
+            if w in wtovec:
+                vec = [x1+x2 for x1,x2 in zip(vec,wtovec[w])]
+    return vec
+
```

