# Comparing `tmp/gecco-tool-0.9.6.tar.gz` & `tmp/gecco-tool-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gecco-tool-0.9.6.tar", last modified: Wed Jan 11 19:34:47 2023, max compression
+gzip compressed data, was "gecco-tool-0.9.7.tar", last modified: Fri May 26 12:00:09 2023, max compression
```

## Comparing `gecco-tool-0.9.6.tar` & `gecco-tool-0.9.7.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 19:34:47.817230 gecco-tool-0.9.6/
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-01-11 19:33:55.000000 gecco-tool-0.9.6/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)    31905 2023-01-11 19:33:55.000000 gecco-tool-0.9.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-01-11 19:33:55.000000 gecco-tool-0.9.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8708 2023-01-11 19:34:47.817230 gecco-tool-0.9.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7201 2023-01-11 19:33:55.000000 gecco-tool-0.9.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 19:34:47.789231 gecco-tool-0.9.6/gecco/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-01-11 19:33:55.000000 gecco-tool-0.9.6/gecco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-01-11 19:33:55.000000 gecco-tool-0.9.6/gecco/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-01-11 19:33:55.000000 gecco-tool-0.9.6/gecco/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-01-11 19:33:55.000000 gecco-tool-0.9.6/gecco/_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 19:34:47.789231 gecco-tool-0.9.6/gecco/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-01-11 19:33:55.000000 gecco-tool-0.9.6/gecco/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-01-11 19:33:55.000000 gecco-tool-0.9.6/gecco/cli/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 19:34:47.793231 gecco-tool-0.9.6/gecco/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 19:33:55.000000 gecco-tool-0.9.6/gecco/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-01-11 19:33:55.000000 gecco-tool-0.9.6/gecco/cli/commands/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-01-11 19:33:55.000000 gecco-tool-0.9.6/gecco/cli/commands/_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    21835 2023-01-11 19:33:55.000000 gecco-tool-0.9.6/gecco/cli/commands/_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-01-11 19:33:55.000000 gecco-tool-0.9.6/gecco/cli/commands/annotate.py
--rw-r--r--   0 runner    (1001) docker     (123)     9895 2023-01-11 19:33:55.000000 gecco-tool-0.9.6/gecco/cli/commands/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     9675 2023-01-11 19:33:55.000000 gecco-tool-0.9.6/gecco/cli/commands/cv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-01-11 19:33:55.000000 gecco-tool-0.9.6/gecco/cli/commands/help.py
--rw-r--r--   0 runner    (1001) docker     (123)    14172 2023-01-11 19:33:55.000000 gecco-tool-0.9.6/gecco/cli/commands/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)    14838 2023-01-11 19:33:55.000000 gecco-tool-0.9.6/gecco/cli/commands/run.py
--rw-r--r--   0 runner    (1001) docker     (123)    11983 2023-01-11 19:33:55.000000 gecco-tool-0.9.6/gecco/cli/commands/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 19:34:47.793231 gecco-tool-0.9.6/gecco/crf/
--rw-r--r--   0 runner    (1001) docker     (123)    16301 2023-01-11 19:33:55.000000 gecco-tool-0.9.6/gecco/crf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-01-11 19:33:55.000000 gecco-tool-0.9.6/gecco/crf/cv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-01-11 19:33:55.000000 gecco-tool-0.9.6/gecco/crf/features.py
--rw-r--r--   0 runner    (1001) docker     (123)   517283 2023-01-11 19:33:55.000000 gecco-tool-0.9.6/gecco/crf/model.pkl
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-01-11 19:33:55.000000 gecco-tool-0.9.6/gecco/crf/model.pkl.md5
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-01-11 19:33:55.000000 gecco-tool-0.9.6/gecco/crf/select.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 19:34:47.797231 gecco-tool-0.9.6/gecco/hmmer/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-01-11 19:33:55.000000 gecco-tool-0.9.6/gecco/hmmer/Pfam.ini
--rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-01-11 19:33:55.000000 gecco-tool-0.9.6/gecco/hmmer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 19:34:47.797231 gecco-tool-0.9.6/gecco/interpro/
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-01-11 19:33:55.000000 gecco-tool-0.9.6/gecco/interpro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123) 20566339 2023-01-11 19:33:55.000000 gecco-tool-0.9.6/gecco/interpro/interpro.json
--rw-r--r--   0 runner    (1001) docker     (123)    35524 2023-01-11 19:33:55.000000 gecco-tool-0.9.6/gecco/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-01-11 19:33:55.000000 gecco-tool-0.9.6/gecco/orf.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 19:33:55.000000 gecco-tool-0.9.6/gecco/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8408 2023-01-11 19:33:55.000000 gecco-tool-0.9.6/gecco/refine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 19:34:47.813230 gecco-tool-0.9.6/gecco/types/
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-01-11 19:33:55.000000 gecco-tool-0.9.6/gecco/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   143388 2023-01-11 19:33:55.000000 gecco-tool-0.9.6/gecco/types/compositions.npz
--rw-r--r--   0 runner    (1001) docker     (123)    22128 2023-01-11 19:33:55.000000 gecco-tool-0.9.6/gecco/types/domains.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    38175 2023-01-11 19:33:55.000000 gecco-tool-0.9.6/gecco/types/types.tsv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 19:34:47.817230 gecco-tool-0.9.6/gecco_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8708 2023-01-11 19:34:47.000000 gecco-tool-0.9.6/gecco_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-01-11 19:34:47.000000 gecco-tool-0.9.6/gecco_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 19:34:47.000000 gecco-tool-0.9.6/gecco_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-01-11 19:34:47.000000 gecco-tool-0.9.6/gecco_tool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 19:34:47.000000 gecco-tool-0.9.6/gecco_tool.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-01-11 19:34:47.000000 gecco-tool-0.9.6/gecco_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-11 19:34:47.000000 gecco-tool-0.9.6/gecco_tool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-01-11 19:34:47.000000 gecco-tool-0.9.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-01-11 19:34:47.817230 gecco-tool-0.9.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    16470 2023-01-11 19:33:55.000000 gecco-tool-0.9.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 19:34:47.817230 gecco-tool-0.9.6/static/
--rw-r--r--   0 runner    (1001) docker     (123)    23632 2023-01-11 19:33:55.000000 gecco-tool-0.9.6/static/gecco.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:00:09.432466 gecco-tool-0.9.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)    31905 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8709 2023-05-26 12:00:09.432466 gecco-tool-0.9.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7201 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:00:09.400465 gecco-tool-0.9.7/gecco/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:00:09.400465 gecco-tool-0.9.7/gecco/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/cli/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:00:09.404465 gecco-tool-0.9.7/gecco/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/cli/commands/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/cli/commands/_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22720 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/cli/commands/_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9045 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/cli/commands/annotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13208 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/cli/commands/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9675 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/cli/commands/cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/cli/commands/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14172 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/cli/commands/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15490 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/cli/commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11983 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/cli/commands/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:00:09.408465 gecco-tool-0.9.7/gecco/crf/
+-rw-r--r--   0 runner    (1001) docker     (123)    16301 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/crf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/crf/cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/crf/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)   517283 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/crf/model.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/crf/model.pkl.md5
+-rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/crf/select.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:00:09.408465 gecco-tool-0.9.7/gecco/hmmer/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/hmmer/Pfam.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     8247 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/hmmer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:00:09.408465 gecco-tool-0.9.7/gecco/interpro/
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/interpro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123) 20566339 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/interpro/interpro.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31338 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/orf.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8408 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/refine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:00:09.428465 gecco-tool-0.9.7/gecco/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   143388 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/types/compositions.npz
+-rw-r--r--   0 runner    (1001) docker     (123)    22128 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/types/domains.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    38175 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/types/types.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:00:09.432466 gecco-tool-0.9.7/gecco_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8709 2023-05-26 12:00:09.000000 gecco-tool-0.9.7/gecco_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-26 12:00:09.000000 gecco-tool-0.9.7/gecco_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 12:00:09.000000 gecco-tool-0.9.7/gecco_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-26 12:00:09.000000 gecco-tool-0.9.7/gecco_tool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 12:00:09.000000 gecco-tool-0.9.7/gecco_tool.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-26 12:00:09.000000 gecco-tool-0.9.7/gecco_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-26 12:00:09.000000 gecco-tool-0.9.7/gecco_tool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-26 12:00:09.000000 gecco-tool-0.9.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-05-26 12:00:09.432466 gecco-tool-0.9.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    16470 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:00:09.432466 gecco-tool-0.9.7/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    23632 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/static/gecco.png
```

### Comparing `gecco-tool-0.9.6/CITATION.cff` & `gecco-tool-0.9.7/CITATION.cff`

 * *Files identical despite different names*

### Comparing `gecco-tool-0.9.6/LICENSE` & `gecco-tool-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gecco-tool-0.9.6/PKG-INFO` & `gecco-tool-0.9.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gecco-tool
-Version: 0.9.6
+Version: 0.9.7
 Summary: Gene cluster prediction with Conditional random fields.
 Home-page: https://gecco.embl.de
 Author: Martin Larralde
 Author-email: martin.larralde@embl.de
 License: GPLv3
 Project-URL: Repository, https://github.com/zellerlab/GECCO
 Project-URL: Bug Tracker, https://github.com/zellerlab/GECCO/issues
@@ -17,23 +17,23 @@
 Platform: powerpc
 Platform: ppc64
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Typing :: Typed
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: train
 License-File: LICENSE
 
 <img align="right" width="180" height="180" src="https://raw.githubusercontent.com/zellerlab/GECCO/v0.6.2/static/gecco-square.png">
 
 # Hi, I'm GECCO!
@@ -59,15 +59,15 @@
 [![Versions](https://img.shields.io/pypi/pyversions/gecco-tool.svg?style=flat-square&maxAge=3600)](https://pypi.org/project/gecco-tool/#files)
 [![Wheel](https://img.shields.io/pypi/wheel/gecco-tool?style=flat-square&maxAge=3600)](https://pypi.org/project/gecco-tool/#files)
 
 
 ## 🔧 Installing GECCO
 
 GECCO is implemented in [Python](https://www.python.org/), and supports [all
-versions](https://endoflife.date/python) from Python 3.6. It requires
+versions](https://endoflife.date/python) from Python 3.7. It requires
 additional libraries that can be installed directly from
 [PyPI](https://pypi.org), the Python Package Index.
 
 Use [`pip`](https://pip.pypa.io/en/stable/) to install GECCO on your
 machine:
 ```console
 $ pip install gecco-tool
```

### Comparing `gecco-tool-0.9.6/README.md` & `gecco-tool-0.9.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [![Versions](https://img.shields.io/pypi/pyversions/gecco-tool.svg?style=flat-square&maxAge=3600)](https://pypi.org/project/gecco-tool/#files)
 [![Wheel](https://img.shields.io/pypi/wheel/gecco-tool?style=flat-square&maxAge=3600)](https://pypi.org/project/gecco-tool/#files)
 
 
 ## 🔧 Installing GECCO
 
 GECCO is implemented in [Python](https://www.python.org/), and supports [all
-versions](https://endoflife.date/python) from Python 3.6. It requires
+versions](https://endoflife.date/python) from Python 3.7. It requires
 additional libraries that can be installed directly from
 [PyPI](https://pypi.org), the Python Package Index.
 
 Use [`pip`](https://pip.pypa.io/en/stable/) to install GECCO on your
 machine:
 ```console
 $ pip install gecco-tool
```

### Comparing `gecco-tool-0.9.6/gecco/_meta.py` & `gecco-tool-0.9.7/gecco/_meta.py`

 * *Files identical despite different names*

### Comparing `gecco-tool-0.9.6/gecco/cli/_utils.py` & `gecco-tool-0.9.7/gecco/cli/_utils.py`

 * *Files identical despite different names*

### Comparing `gecco-tool-0.9.6/gecco/cli/commands/_base.py` & `gecco-tool-0.9.7/gecco/cli/commands/_base.py`

 * *Files identical despite different names*

### Comparing `gecco-tool-0.9.6/gecco/cli/commands/_main.py` & `gecco-tool-0.9.7/gecco/cli/commands/_main.py`

 * *Files identical despite different names*

### Comparing `gecco-tool-0.9.6/gecco/cli/commands/_mixins.py` & `gecco-tool-0.9.7/gecco/cli/commands/_mixins.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import collections
 import csv
 import gzip
 import io
 import itertools
+import math
+import multiprocessing.pool
 import os
 import operator
 import typing
 from typing import (
     BinaryIO,
     Container,
     Collection,
@@ -79,17 +81,15 @@
             # get filesize and unit
             input_size = os.stat(self.genes).st_size
             total, scale, unit = ProgressReader.scale_size(input_size)
             task = self.progress.add_task("Loading genetable", total=total, unit=unit, precision=".1f")
             # load gene table
             self.info("Loading", "genes table from file", repr(self.genes))
             with typing.cast(BinaryIO, ProgressReader(open(self.genes, "rb"), self.progress, task, scale)) as in_:
-                if self.genes.endswith(".gz"):
-                    in_ = typing.cast(BinaryIO, gzip.open(in_))
-                table = GeneTable.load(io.TextIOWrapper(in_))
+                table = GeneTable.load(in_)
             # count genes and yield gene objects
             n_genes = len(set(table.protein_id))
             unit = "gene" if n_genes == 1 else "genes"
             task = self.progress.add_task("Building genes", total=n_genes, unit=unit, precision="")
             yield from self.progress.track(table.to_genes(), task_id=task)
         except OSError as err:
             self.error("Fail to parse genes coordinates: {}", err)
@@ -104,17 +104,15 @@
                 # get filesize and unit
                 input_size = os.stat(filename).st_size
                 total, scale, unit = ProgressReader.scale_size(input_size)
                 task = self.progress.add_task("Loading features", total=total, unit=unit, precision=".1f")
                 # load features
                 self.info("Loading", "features table from file", repr(filename))
                 with typing.cast(BinaryIO, ProgressReader(open(filename, "rb"), self.progress, task, scale)) as in_:
-                    if filename.endswith(".gz"):
-                        in_ = typing.cast(BinaryIO, gzip.open(in_))
-                    features += FeatureTable.load(io.TextIOWrapper(in_))
+                    features += FeatureTable.load(in_)
             except FileNotFoundError as err:
                 self.error("Could not find feature file:", repr(filename))
                 raise CommandExit(err.errno) from err
 
         self.success("Loaded", "a total of", len(features), "features", level=1)
         return features
 
@@ -125,38 +123,37 @@
         gene_index = { gene.protein.id:gene for gene in genes }
         if len(gene_index) < len(genes):
             raise ValueError("Duplicate gene names in input genes")
 
         # add domains from the feature table
         unit = "row" if len(features) == 1 else "rows"
         task = self.progress.add_task("Annotating genes", total=len(features), unit=unit, precision="")
-        for row in typing.cast(Iterable["FeatureTable.Row"], self.progress.track(features, total=len(features), task_id=task)):
+        for i in self.progress.track(range(len(features)), task_id=task):
             # get gene by ID and check consistency
-            gene = gene_index[row.protein_id]
-            if gene.source.id != row.sequence_id:
-                raise ValueError(f"Mismatched source sequence for {row.protein_id!r}: {gene.source.id!r} != {row.sequence_id!r}")
-            elif gene.end - gene.start != row.end - row.start:
-                raise ValueError(f"Mismatched gene length for {row.protein_id!r}: {gene.end - gene.start!r} != {row.end - row.start!r}")
-            elif gene.start != row.start:
-                raise ValueError(f"Mismatched gene start for {row.protein_id!r}: {gene.start!r} != {row.start!r}")
-            elif gene.end != row.end:
-                raise ValueError(f"Mismatched gene end for {row.protein_id!r}: {gene.end!r} != {row.end!r}")
-            elif gene.strand.sign != row.strand:
-                raise ValueError(f"Mismatched gene strand for {row.protein_id!r}: {gene.strand.sign!r} != {row.strand!r}")
-            elif gene.source.id != row.sequence_id:
-                raise ValueError(f"Mismatched sequence ID {row.protein_id!r}: {gene.source.id!r} != {row.sequence_id!r}")
+            length = features.end[i] - features.start[i]
+            gene = gene_index[features.protein_id[i]]
+            if gene.source.id != features.sequence_id[i]:
+                raise ValueError(f"Mismatched source sequence for {features.protein_id[i]!r}: {gene.source.id!r} != {features.sequence_id[i]!r}")
+            elif gene.end - gene.start != length:
+                raise ValueError(f"Mismatched gene length for {row.protein_id!r}: {gene.end - gene.start!r} != {length!r}")
+            elif gene.start != features.start[i]:
+                raise ValueError(f"Mismatched gene start for {row.protein_id!r}: {gene.start!r} != {features.start[i]!r}")
+            elif gene.end != features.end[i]:
+                raise ValueError(f"Mismatched gene end for {row.protein_id!r}: {gene.end!r} != {features.end[i]!r}")
+            elif gene.strand.sign != features.strand[i]:
+                raise ValueError(f"Mismatched gene strand for {row.protein_id!r}: {gene.strand.sign!r} != {features.strand[i]!r}")
             # add the row domain to the gene
             domain = Domain(
-                name=row.domain,
-                start=row.domain_start,
-                end=row.domain_end,
-                hmm=row.hmm,
-                i_evalue=row.i_evalue,
-                pvalue=row.pvalue,
-                probability=row.cluster_probability,
+                name=features.domain[i],
+                start=features.domain_start[i],
+                end=features.domain_end[i],
+                hmm=features.hmm[i],
+                i_evalue=features.i_evalue[i],
+                pvalue=features.pvalue[i],
+                probability=features.cluster_probability[i],
             )
             gene.protein.domains.append(domain)
 
         # return
         return list(gene_index.values())
 
 
@@ -182,33 +179,33 @@
 
     def _write_feature_table(self, genes: List["Gene"]) -> None:
         from ...model import FeatureTable
 
         base, _ = os.path.splitext(os.path.basename(self.genome))
         pred_out = os.path.join(self.output_dir, f"{base}.features.tsv")
         self.info("Writing", "feature table to", repr(pred_out), level=1)
-        with open(pred_out, "w") as f:
+        with open(pred_out, "wb") as f:
             FeatureTable.from_genes(genes).dump(f)
 
     def _write_genes_table(self, genes: List["Gene"]) -> None:
         from ...model import GeneTable
 
         base, _ = os.path.splitext(os.path.basename(self.genome))
         pred_out = os.path.join(self.output_dir, f"{base}.genes.tsv")
         self.info("Writing", "gene table to", repr(pred_out), level=1)
-        with open(pred_out, "w") as f:
+        with open(pred_out, "wb") as f:
             GeneTable.from_genes(genes).dump(f)
 
     def _write_cluster_table(self, clusters: List["Cluster"]) -> None:
         from ...model import ClusterTable
 
         base, _ = os.path.splitext(os.path.basename(self.genome))
         cluster_out = os.path.join(self.output_dir, f"{base}.clusters.tsv")
         self.info("Writing", "cluster table to", repr(cluster_out), level=1)
-        with open(cluster_out, "w") as out:
+        with open(cluster_out, "wb") as out:
             ClusterTable.from_clusters(clusters).dump(out)
 
     def _write_clusters(self, clusters: List["Cluster"], merge: bool = False) -> None:
         from Bio import SeqIO
 
         if merge:
             base, _ = os.path.splitext(os.path.basename(self.genome))
@@ -222,14 +219,15 @@
                 SeqIO.write(cluster.to_seq_record(), gbk_out, "genbank")
 
 
 class DomainFilterMixin(Command):
 
     e_filter: Optional[float]
     p_filter: Optional[float]
+    disentangle: bool
 
     def _filter_domains(self, genes: List["Gene"]) -> List["Gene"]:
         # Filter i-evalue and p-value if required
         if self.e_filter is not None:
             self.info("Excluding", "domains with e-value over", self.e_filter, level=1)
             key = lambda d: d.i_evalue < self.e_filter
             genes = [
@@ -244,20 +242,45 @@
                 for gene in genes
             ]
         if self.p_filter is not None or self.e_filter is not None:
             count = sum(1 for gene in genes for domain in gene.protein.domains)
             self.info("Using", "remaining", count, "domains", level=1)
         return genes
 
+    def _disentangle(self, gene: "Gene") -> "Gene":
+        if len(gene.protein.domains) <= 1:
+            return gene
+
+        domains_to_keep = []
+        gene_domains = gene.protein.domains.copy()
+        while gene_domains:
+            # get a domain and collect other overlaping domains
+            domain = gene_domains.pop()
+            overlaps = [
+                other for other in gene_domains
+                if other.start <= domain.end and domain.start <= other.end
+            ]
+            # keep only overlapping domain with the best p-value
+            if not overlaps or domain.pvalue < min(d.pvalue for d in overlaps):
+                domains_to_keep.append(domain)
+                for other in overlaps:
+                    gene_domains.remove(other)
+
+        return gene.with_protein(gene.protein.with_domains(domains_to_keep))
+
+    def _disentangle_domains(self, genes: List["Gene"]) -> List["Gene"]:
+        self.info("Disentangling", "overlapping domains in each gene", level=1)
+        return list(map(self._disentangle, genes))
+
 
 class AnnotatorMixin(DomainFilterMixin):
 
     hmm: Optional[List[str]]
-    hmm_x: Optional[List[str]]
     jobs: int
+    bit_cutoffs: Optional[str]
 
     def _custom_hmms(self) -> Iterable["HMM"]:
         from ...hmmer import HMM
 
         for path in typing.cast(List[str], self.hmm):
             base = os.path.basename(path)
             file: BinaryIO = open(path, "rb")
@@ -267,55 +290,43 @@
             base, _ = os.path.splitext(base)
             yield HMM(
                 id=base,
                 version="?",
                 url="?",
                 path=path,
                 size=None,
-                exclusive=False,
-                relabel_with=r"s/([^\.]*)(\..*)?/\1/"
-            )
-        for path in typing.cast(List[str], self.hmm_x):
-            base = os.path.basename(path)
-            file = open(path, "rb")
-            if base.endswith(".gz"):
-                base, _ = os.path.splitext(base)
-                file = gzip.GzipFile(fileobj=file, mode="rb")   # type: ignore
-            base, _ = os.path.splitext(base)
-            yield HMM(
-                id=base,
-                version="?",
-                url="?",
-                path=path,
-                size=None,
-                exclusive=True,
                 relabel_with=r"s/([^\.]*)(\..*)?/\1/"
             )
 
     def _annotate_domains(self, genes: List["Gene"], whitelist: Optional[Collection[str]] = None) -> List["Gene"]:
         from ...hmmer import PyHMMER, embedded_hmms
 
         self.info("Running", "HMMER domain annotation", level=1)
 
         # Run all HMMs over ORFs to annotate with protein domains
         hmms = list(self._custom_hmms() if self.hmm else embedded_hmms())
-        task = self.progress.add_task(description=f"Annotating domains", unit="HMMs", total=len(hmms), precision="")
-        for hmm in self.progress.track(hmms, task_id=task, total=len(hmms)):
-            total = hmm.size if whitelist is None else len(whitelist)
-            task = self.progress.add_task(description=f"  {hmm.id} v{hmm.version}", total=total, unit="domains", precision="")
-            callback = lambda h, t: self.progress.update(task, advance=1)
+        total = None if whitelist is None else len(whitelist)
+        task_hmms = self.progress.add_task(description=f"Annotating domains", unit="HMMs", total=len(hmms), precision="")
+        task_domains = self.progress.add_task(description="", total=total, unit="domains", precision="")
+        for hmm in self.progress.track(hmms, task_id=task_hmms, total=len(hmms)):
+            self.progress.update(task_domains, description=f" {hmm.id} v{hmm.version}")
+            callback = lambda h, t: self.progress.update(task_domains, advance=1)
             self.info("Starting", f"annotation with [bold blue]{hmm.id} v{hmm.version}[/]", level=2)
-            genes = PyHMMER(hmm, self.jobs, whitelist).run(genes, progress=callback)
+            genes = PyHMMER(hmm, self.jobs, whitelist).run(genes, progress=callback, bit_cutoffs=self.bit_cutoffs)
             self.success("Finished", f"annotation with [bold blue]{hmm.id} v{hmm.version}[/]", level=2)
-            self.progress.update(task_id=task, visible=False)
+        self.progress.update(task_id=task_domains, visible=False)
 
         # Count number of annotated domains
         count = sum(1 for gene in genes for domain in gene.protein.domains)
         self.success("Found", count, "domains across all proteins", level=1)
 
+        # Disentangle if required
+        if self.disentangle:
+            genes = self._disentangle_domains(genes)
+
         # Filter i-evalue and p-value if required
         genes = self._filter_domains(genes)
 
         # Sort genes
         self.info("Sorting", "genes by coordinates", level=2)
         genes.sort(key=lambda g: (g.source.id, g.start, g.end))
         for gene in genes:
@@ -418,63 +429,76 @@
             # get filesize and unit
             input_size = os.stat(self.clusters).st_size
             total, scale, unit = ProgressReader.scale_size(input_size)
             task = self.progress.add_task("Loading clusters", total=total, unit=unit, precision=".1f")
             # load clusters
             self.info("Loading", "clusters table from file", repr(self.clusters))
             with ProgressReader(open(self.clusters, "rb"), self.progress, task, scale) as in_:
-                return ClusterTable.load(io.TextIOWrapper(in_))   # type: ignore
+                return ClusterTable.load(in_)   # type: ignore
         except FileNotFoundError as err:
             self.error("Could not find clusters file:", repr(self.clusters))
             raise CommandExit(err.errno) from err
 
     def _label_genes(self, genes: List["Gene"], clusters: "ClusterTable") -> List["Gene"]:
         cluster_by_seq = collections.defaultdict(list)
-        for cluster_row in clusters:
-            cluster_by_seq[cluster_row.sequence_id].append(cluster_row)
+        for i in range(len(clusters)):
+            cluster_by_seq[clusters.sequence_id[i]].append((clusters.start[i], clusters.end[i]))
 
         gene_count = len(genes)
         unit = "gene" if gene_count == 1 else "genes"
         task = self.progress.add_task("Labelling genes", total=gene_count, unit=unit, precision="")
 
         self.info("Labelling", "genes belonging to clusters")
         labelled_genes = []
         for seq_id, seq_genes in itertools.groupby(genes, key=operator.attrgetter("source.id")):
             for gene in seq_genes:
                 if any(
-                    cluster_row.start <= gene.start and gene.end <= cluster_row.end
-                    for cluster_row in cluster_by_seq[seq_id]
+                    cluster_start <= gene.start and gene.end <= cluster_end
+                    for (cluster_start, cluster_end) in cluster_by_seq[seq_id]
                 ):
                     gene = gene.with_probability(1)
                 else:
                     gene = gene.with_probability(0)
                 labelled_genes.append(gene)
                 self.progress.update(task_id=task, advance=1)
 
         return labelled_genes
 
     def _extract_clusters(self, genes: List["Gene"], clusters: "ClusterTable") -> List["Cluster"]:
-        from ...model import Cluster
+        from ...model import Cluster, ClusterType
 
+        cluster_types = {}
         cluster_by_seq = collections.defaultdict(list)
-        for cluster_row in clusters:
-            cluster_by_seq[cluster_row.sequence_id].append(cluster_row)
+        for i in range(len(clusters)):
+            seq_id = clusters.sequence_id[i]
+            cluster_id = clusters.cluster_id[i]
+            cluster_by_seq[seq_id].append((
+                clusters.start[i],
+                clusters.end[i],
+                clusters.cluster_id[i],
+            ))
+            if not "type" in clusters.data.columns:
+                cluster_types[cluster_id] = None
+            elif clusters.type[i] == "Unknown" or clusters.type[i] is None:
+                cluster_types[cluster_id] = ClusterType()
+            else:
+                cluster_types[cluster_id] = ClusterType(*clusters.type[i].split(";"))
 
         self.info("Extracting", "genes belonging to clusters")
         genes_by_cluster = collections.defaultdict(list)
         for seq_id, seq_genes in itertools.groupby(genes, key=operator.attrgetter("source.id")):
             for gene in seq_genes:
-                for cluster_row in cluster_by_seq[seq_id]:
-                    if cluster_row.start <= gene.start and gene.end <= cluster_row.end:
-                        genes_by_cluster[cluster_row.cluster_id].append(gene)
+                for cluster_start, cluster_end, cluster_id in cluster_by_seq[seq_id]:
+                    if cluster_start <= gene.start and gene.end <= cluster_end:
+                        genes_by_cluster[cluster_id].append(gene)
 
         return [
-            Cluster(cluster_row.cluster_id, genes_by_cluster[cluster_row.cluster_id], cluster_row.type)
-            for cluster_row in typing.cast(Iterable["ClusterTable.Row"], sorted(clusters, key=operator.attrgetter("cluster_id")))
-            if genes_by_cluster[cluster_row.cluster_id]
+            Cluster(cluster_id, genes_by_cluster[cluster_id], cluster_types[cluster_id])
+            for cluster_id in sorted(clusters.cluster_id)
+            if genes_by_cluster[cluster_id]
         ]
 
 
 class CompositionWriterMixin(Command):
 
     output_dir: str
```

### Comparing `gecco-tool-0.9.6/gecco/cli/commands/annotate.py` & `gecco-tool-0.9.7/gecco/cli/commands/annotate.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,29 +77,34 @@
                                           genes from scratch.
             --locus-tag <locus_tag>       The name of the feature qualifier
                                           to use for naming extracted genes
                                           when using the ``--cds-feature``
                                           flag. [default: locus_tag]
 
         Parameters - Domain Annotation:
+            --hmm <hmm>                   the path to one or more alternative
+                                          HMM file to use (in HMMER format).
             -e <e>, --e-filter <e>        the e-value cutoff for protein domains
                                           to be included. This is not stable
                                           across versions, so consider using
                                           a p-value filter instead.
             -p <p>, --p-filter <p>        the p-value cutoff for protein domains
                                           to be included. [default: 1e-9]
+            --bit-cutoffs <name>          use bitscore cutoffs (one of *noise*,
+                                          *gathering*, or *trusted*) to filter
+                                          domain annotations.
+            --disentangle                 disentangle overlapping domains in 
+                                          each gene by keeping only the domains
+                                          with the lowest E-value over a given
+                                          position.
 
-        Parameters - Debug:
-            --hmm <hmm>                   the path to one or more alternative
-                                          HMM file to use (in HMMER format).
-            --hmm-x <hmm>                 the path to one or more exclusive
-                                          HMM file to use (in HMMER format).
         """
 
     def _check(self) -> None:
+        _BITSCORE_CUTOFFS = {"gathering", "noise", "trusted"}
         super()._check()
         try:
             self.e_filter = self._check_flag(
                 "--e-filter",
                 float,
                 lambda x: x > 0,
                 hint="real number above 0",
@@ -112,20 +117,27 @@
                 hint="real number above 0",
                 optional=True,
             )
             self.jobs = self._check_flag("--jobs", int, lambda x: x >= 0, hint="positive or null integer")
             self.format: Optional[str] = self._check_flag("--format", optional=True)
             self.genome: str = self._check_flag("--genome")
             self.hmm: Optional[List[str]] = self._check_flag("--hmm", optional=True)
-            self.hmm_x: Optional[List[str]] = self._check_flag("--hmm-x", optional=True)
             self.output_dir: str = self._check_flag("--output-dir")
             self.mask = self._check_flag("--mask", bool)
             self.force_tsv = self._check_flag("--force-tsv", bool)
             self.cds_feature: Optional[str] = self._check_flag("--cds-feature", optional=True)
             self.locus_tag: str = self._check_flag("--locus-tag")
+            self.disentangle = self._check_flag("--disentangle", bool)
+            self.bit_cutoffs: str = self._check_flag(
+                "--bit-cutoffs",
+                str,
+                _BITSCORE_CUTOFFS.__contains__,
+                optional=True,
+                hint="one of {}".format(", ".join(sorted(_BITSCORE_CUTOFFS)))
+            )
         except InvalidArgument:
             raise CommandExit(1)
 
     # ---
 
     _OUTPUT_FILES = ["features.tsv", "genes.tsv"]
```

### Comparing `gecco-tool-0.9.6/gecco/cli/commands/convert.py` & `gecco-tool-0.9.7/gecco/cli/commands/convert.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """Implementation of the ``gecco convert`` subcommand.
 """
 
 import contextlib
 import copy
+import csv
 import errno
 import functools
 import itertools
 import glob
 import os
 import operator
 import multiprocessing
 import random
 import re
 import signal
 import typing
+import urllib.parse
 from typing import Any, Dict, Union, Optional, List, TextIO, Mapping, Set
 
 from ... import __version__
 from ._base import Command, CommandExit, InvalidArgument
 from .._utils import patch_showwarnings
 
 
@@ -28,14 +30,15 @@
     @classmethod
     def doc(cls, fast: bool = False) -> str:  # noqa: D102
         return f"""
         gecco convert  - {cls.summary}
 
         Usage:
             gecco convert gbk -i <input> -f <format> [options]
+            gecco convert clusters -i <input> -f <format> [options]
 
         Arguments:
             -i <input>, --input-dir <input> the path to the input directory
                                             containing files to convert.
             -f <format>, --format <format>  the name of the output format to
                                             write.
 
@@ -59,17 +62,22 @@
             sequence of the cluster. Output files are named ``*.fna``.
 
         ``gecco convert gbk --format=faa``
             Convert the GenBank files to FASTA files containing the amino-acid
             sequences of all the proteins in a cluster. Output files are
             named ``*.faa``.
 
+        ``gecco convert clusters --format=gff``
+            Convert the clusters tables to GFF3 containing the position
+            and metadata for all the predicted clusters. Output file is 
+            named ``*.clusters.gff``.
+
         """
 
-    _CLUSTERS_FORMATS: Set[str] = set()
+    _CLUSTERS_FORMATS: Set[str] = {"gff"}
     _GBK_FORMATS = {"bigslice", "faa", "fna"}
 
     def _check(self) -> None:
         try:
             super()._check()
             formats = self._GBK_FORMATS if self.args["gbk"] else self._CLUSTERS_FORMATS
             self.format = self._check_flag("--format", str, lambda x: x in formats, hint=", ".join(formats))
@@ -92,19 +100,18 @@
         cluster_files = glob.glob(os.path.join(self.input_dir, "*.clusters.tsv"))
         unit = "table" if len(cluster_files) == 1 else "tables"
         task = self.progress.add_task("Loading clusters", total=len(cluster_files), unit=unit, precision="")
         # load the original coordinates from the `*.clusters.tsv` files
         coordinates = {}
         types = {}
         for cluster_file in self.progress.track(cluster_files, task_id=task):
-            cluster_fh = ctx.enter_context(open(cluster_file))
-            for row in ClusterTable.load(cluster_fh):
-                ty = ";".join(sorted(row.type.names))
-                coordinates[row.cluster_id] = (row.start, row.end)
-                types[row.cluster_id] = ty or "Unknown"
+            table = ClusterTable.load(cluster_file)
+            for i, cluster_id in enumerate(table.cluster_id):
+                coordinates[cluster_id] = (table.start[i], table.end[i])
+                types[cluster_id] = table.type[i] or "Unknown"
 
         # collect `*_clusters_{N}.gbk` files
         gbk_files = glob.glob(os.path.join(self.input_dir, "*_cluster_*.gbk"))
         unit = "file" if len(gbk_files) == 1 else "files"
         task = self.progress.add_task("Converting", total=len(gbk_files), unit=unit, precision="")
         done = 0
         # rewrite GenBank files
@@ -190,28 +197,86 @@
             # write proteins to FASTA
             new_name = re.sub(r"\.gbk$", ".faa", gbk_file)
             self.info(f"Converting {gbk_file!r} proteins to FASTA file {new_name!r}")
             Bio.SeqIO.write(proteins, new_name, "fasta")
             done += 1
         self.success("Converted", f"{done} GenBank {unit} to protein FASTA format", level=0)
 
+    def _convert_clusters_gff(self, ctx: contextlib.ExitStack) -> None:
+        import Bio.SeqIO
+        from ...model import ClusterTable
+
+        # collect `*_clusters_{N}.gbk` files
+        tsv_files = glob.glob(os.path.join(self.input_dir, "*.clusters.tsv"))
+        unit = "file" if len(tsv_files) == 1 else "files"
+        task = self.progress.add_task("Converting", total=len(tsv_files), unit=unit, precision="")
+        done = 0
+        # rewrite GenBank files
+        for tsv_file in self.progress.track(tsv_files, task_id=task, total=len(tsv_files)):
+            table = ClusterTable.load(tsv_file)
+            gff_file = re.sub(r"\.tsv$", ".gff", tsv_file)
+            with open(gff_file, "w") as dst:
+                writer = csv.writer(dst, dialect="excel-tab")
+                writer.writerow(["##gff-version 3"])
+                for row in table.data.rows(named=True):
+                    # load the GenBank files of the cluster to extract the GECCO version
+                    gbk_file = os.path.join(self.input_dir, f"{row['cluster_id']}.gbk")
+                    cluster = Bio.SeqIO.read(gbk_file, "genbank")
+                    annotations = cluster.annotations['structured_comment']['GECCO-Data']
+                    # make sure to have a BGC type to write down
+                    bgc_types = ["Unknown"] if not row["type"] else row["type"].split(";")
+                    # extract type probabilities
+                    type_probas = []
+                    for key, value in row.items():
+                        if key.endswith("_probability"):
+                            ty = key.split("_")[0].capitalize()
+                            if ty == "Nrp":
+                                ty = "NRP"
+                            type_probas.append(f"Type{ty}={value}")
+                    # write the GFF row
+                    writer.writerow([
+                        row["sequence_id"],
+                        annotations["version"],
+                        "BGC",
+                        str(row["start"]),
+                        str(row["end"]),
+                        str(row["average_p"]),
+                        ".",
+                        ".",
+                        ";".join([
+                            f"ID={row['cluster_id']}",
+                            f"Name={ '/'.join(sorted(bgc_types)) } cluster",
+                            f"Type={ ','.join(sorted(bgc_types)) }",
+                            f"ProbabilityAverage={row['average_p']}",
+                            f"ProbabilityMax={row['max_p']}",
+                            *type_probas,
+                            f"Genes={row['proteins'].count(';') + 1}",
+                            f"Domains={row['domains'].count(';') + 1}",
+                        ])
+                    ])
+            done += 1
+        self.success("Converted", f"{done} TSV {unit} to GFF format", level=0)
+
     def execute(self, ctx: contextlib.ExitStack) -> int:  # noqa: D102
         try:
             # check the CLI arguments were fine and enter context
             self._check()
             ctx.enter_context(self.progress)
             ctx.enter_context(patch_showwarnings(self._showwarnings))  # type: ignore
             # run the appropriate method
             if self.args["gbk"]:
                 if self.args["--format"] == "bigslice":
                     self._convert_gbk_bigslice(ctx)
                 elif self.args["--format"] == "fna":
                     self._convert_gbk_fna(ctx)
                 elif self.args["--format"] == "faa":
                     self._convert_gbk_faa(ctx)
+            elif self.args["clusters"]:
+                if self.args["--format"] == "gff":
+                    self._convert_clusters_gff(ctx)
         except CommandExit as cexit:
             return cexit.code
         except KeyboardInterrupt:
             self.error("Interrupted")
             return -signal.SIGINT
         except Exception as err:
             self.progress.stop()
```

### Comparing `gecco-tool-0.9.6/gecco/cli/commands/cv.py` & `gecco-tool-0.9.7/gecco/cli/commands/cv.py`

 * *Files identical despite different names*

### Comparing `gecco-tool-0.9.6/gecco/cli/commands/help.py` & `gecco-tool-0.9.7/gecco/cli/commands/help.py`

 * *Files identical despite different names*

### Comparing `gecco-tool-0.9.6/gecco/cli/commands/predict.py` & `gecco-tool-0.9.7/gecco/cli/commands/predict.py`

 * *Files identical despite different names*

### Comparing `gecco-tool-0.9.6/gecco/cli/commands/run.py` & `gecco-tool-0.9.7/gecco/cli/commands/run.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,25 +83,36 @@
                                           genes from scratch.
             --locus-tag <locus_tag>       The name of the feature qualifier
                                           to use for naming extracted genes
                                           when using the ``--cds-feature``
                                           flag. [default: locus_tag]
 
         Parameters - Domain Annotation:
+            --hmm <hmm>                   the path to one or more alternative
+                                          HMM file to use (in HMMER format).
             -e <e>, --e-filter <e>        the e-value cutoff for protein domains
                                           to be included. This is not stable
                                           across versions, so consider using
                                           a p-value filter instead.
             -p <p>, --p-filter <p>        the p-value cutoff for protein domains
                                           to be included. [default: 1e-9]
+            --bit-cutoffs <name>          use bitscore cutoffs (one of *noise*,
+                                          *gathering*, or *trusted*) to filter
+                                          domain annotations.
+            --disentangle                 disentangle overlapping domains in 
+                                          each gene by keeping only the domains
+                                          with the lowest E-value over a given
+                                          position.
 
         Parameters - Cluster Detection:
+            --model <directory>           the path to an alternative CRF model
+                                          to use (obtained with `gecco train`).
             --no-pad                      disable padding of gene sequences
-                                          (used to predict gene clusters in 
-                                          contigs smaller than the CRF window 
+                                          (used to predict gene clusters in
+                                          contigs smaller than the CRF window
                                           length).
             -c <N>, --cds <N>             the minimum number of coding sequences a
                                           valid cluster must contain. [default: 3]
             -m <m>, --threshold <m>       the probability threshold for cluster
                                           detection. Default depends on the
                                           post-processing method (0.8 for gecco,
                                           0.6 for antismash).
@@ -111,24 +122,18 @@
                                           that must separate a cluster from the
                                           edge. Edge clusters will still be
                                           included if they are longer. A lower
                                           number will increase the number of
                                           false positives on small contigs.
                                           [default: 0]
 
-        Parameters - Debug:
-            --model <directory>           the path to an alternative CRF model
-                                          to use (obtained with `gecco train`).
-            --hmm <hmm>                   the path to one or more alternative
-                                          HMM file to use (in HMMER format).
-            --hmm-x <hmm>                 the path to one or more exclusive
-                                          HMM file to use (in HMMER format).
         """
 
     def _check(self) -> None:
+        _BITSCORE_CUTOFFS = {"gathering", "noise", "trusted"}
         Command._check(self)
         try:
             self.cds = self._check_flag("--cds", int, lambda x: x > 0, hint="positive integer")
             self.e_filter = self._check_flag(
                 "--e-filter",
                 float,
                 lambda x: x > 0,
@@ -149,23 +154,30 @@
             self.jobs = self._check_flag("--jobs", int, lambda x: x >= 0, hint="positive or null integer")
             self.postproc = self._check_flag("--postproc", str, lambda x: x in ("gecco", "antismash"), hint="'gecco' or 'antismash'")
             self.edge_distance = self._check_flag("--edge-distance", int, lambda x: x >= 0, hint="positive or null integer")
             self.format = self._check_flag("--format", optional=True)
             self.genome = self._check_flag("--genome")
             self.model: Optional[str] = self._check_flag("--model", optional=True)
             self.hmm = self._check_flag("--hmm")
-            self.hmm_x = self._check_flag("--hmm-x")
             self.output_dir = self._check_flag("--output-dir")
             self.antismash_sideload = self._check_flag("--antismash-sideload", bool)
             self.force_tsv = self._check_flag("--force-tsv", bool)
             self.mask = self._check_flag("--mask", bool)
             self.cds_feature = self._check_flag("--cds-feature", optional=True)
             self.locus_tag = self._check_flag("--locus-tag")
             self.no_pad = self._check_flag("--no-pad", bool)
             self.merge_gbk = self._check_flag("--merge-gbk", bool)
+            self.disentangle = self._check_flag("--disentangle", bool)
+            self.bit_cutoffs: str = self._check_flag(
+                "--bit-cutoffs",
+                str,
+                _BITSCORE_CUTOFFS.__contains__,
+                optional=True,
+                hint="one of {}".format(", ".join(sorted(_BITSCORE_CUTOFFS)))
+            )
         except InvalidArgument:
             raise CommandExit(1)
 
     # ---
 
     def _load_model_domains(self) -> typing.Set[str]:
         try:
@@ -193,27 +205,26 @@
                 "name": "GECCO",
                 "version": __version__,
                 "description": "Biosynthetic Gene Cluster prediction with Conditional Random Fields.",
                 "configuration": {
                     "cds": repr(self.cds),
                     "e-filter": repr(self.e_filter),
                     "p-filter": repr(self.p_filter),
+                    "bit-cutoffs": repr(self.bit_cutoffs),
                     "postproc": repr(self.postproc),
                     "threshold": repr(self.threshold),
                     "mask": repr(self.mask),
                     "edge-distance": repr(self.edge_distance),
                     "no-pad": repr(self.no_pad),
                 }
             }
         }
         # record if non-standard HMM or model was used
         if self.hmm:
             data["tool"]["configuration"]["hmm"] = list(self.hmm)
-        if self.hmm_x:
-            data["tool"]["configuration"]["hmm_x"] = list(self.hmm_x)
         if self.model:
             data["tool"]["configuration"]["model"] = self.model
         # create a record per sequence
         for seq_id, seq_clusters in itertools.groupby(clusters, key=operator.attrgetter("source.id")):
             data["records"].append({"name": seq_id, "subregions": []})
             for cluster in seq_clusters:
                 probabilities = {
```

### Comparing `gecco-tool-0.9.6/gecco/cli/commands/train.py` & `gecco-tool-0.9.7/gecco/cli/commands/train.py`

 * *Files identical despite different names*

### Comparing `gecco-tool-0.9.6/gecco/crf/__init__.py` & `gecco-tool-0.9.7/gecco/crf/__init__.py`

 * *Files identical despite different names*

### Comparing `gecco-tool-0.9.6/gecco/crf/cv.py` & `gecco-tool-0.9.7/gecco/crf/cv.py`

 * *Files identical despite different names*

### Comparing `gecco-tool-0.9.6/gecco/crf/features.py` & `gecco-tool-0.9.7/gecco/crf/features.py`

 * *Files identical despite different names*

### Comparing `gecco-tool-0.9.6/gecco/crf/model.pkl` & `gecco-tool-0.9.7/gecco/crf/model.pkl`

 * *Files identical despite different names*

### Comparing `gecco-tool-0.9.6/gecco/crf/select.py` & `gecco-tool-0.9.7/gecco/crf/select.py`

 * *Files identical despite different names*

### Comparing `gecco-tool-0.9.6/gecco/hmmer/__init__.py` & `gecco-tool-0.9.7/gecco/hmmer/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,15 +38,14 @@
     """
 
     id: str
     version: str
     url: str
     path: str
     size: Optional[int] = None
-    exclusive: bool = False
     relabel_with: Optional[str] = None
     md5: Optional[str] = None
 
     def relabel(self, domain: str) -> str:
         """Rename a domain obtained by this HMM to the right accession.
 
         This method can be used with HMM libraries that have separate HMMs
@@ -95,15 +94,16 @@
 class PyHMMER(DomainAnnotator):
     """A domain annotator that uses `pyhmmer`.
     """
 
     def run(
         self,
         genes: Iterable[Gene],
-        progress: Optional[Callable[[pyhmmer.plan7.HMM, int], None]] = None
+        progress: Optional[Callable[[pyhmmer.plan7.HMM, int], None]] = None,
+        bit_cutoffs: Optional[str] = None,
     ) -> List[Gene]:
         # collect genes and keep them in original order
         gene_index = list(genes)
 
         # convert proteins to Easel sequences, namind them after
         # their location in the original input to ignore any duplicate
         # protein identifiers
@@ -131,88 +131,72 @@
             )
             # Run search pipeline using the filtered HMMs
             cpus = 0 if self.cpus is None else self.cpus
             hmms_hits = hmmsearch(
                 profiles,
                 esl_sqs,
                 cpus=cpus,
-                callback=progress,
+                callback=progress, # type: ignore
                 Z=self.hmm.size,  # type: ignore
-                domZ=self.hmm.size  # type: ignore
+                domZ=self.hmm.size, # type: ignore
+                bit_cutoffs=bit_cutoffs,  # type: ignore
             )
 
             # Load InterPro metadata for the annotation
             interpro = InterPro.load()
 
             # Transcribe HMMER hits to GECCO model
-            for hit in itertools.chain.from_iterable(hmms_hits):
-                target_index = int(hit.name)
-                for domain in hit.domains:
-                    # extract name and get InterPro metadata about hit
-                    raw_acc = domain.alignment.hmm_accession or domain.alignment.hmm_name
-                    accession = self.hmm.relabel(raw_acc.decode('utf-8'))
-                    entry = interpro.by_accession.get(accession)
-
-                    # extract coordinates
-                    start = domain.alignment.target_from
-                    end = domain.alignment.target_to
-
-                    # extract qualifiers and GO terms
-                    qualifiers: Dict[str, List[str]] = {
-                        "inference": ["protein motif"],
-                        "db_xref": ["{}:{}".format(self.hmm.id.upper(), accession)],
-                        "note": [
-                            "e-value: {}".format(domain.i_evalue),
-                            "p-value: {}".format(domain.pvalue),
-                        ],
-                    }
-                    if entry is not None:
-                        qualifiers["function"] = [entry.name]
-                        qualifiers["db_xref"].append("InterPro:{}".format(entry.accession))
-                        go_terms = entry.go_terms
-                        go_functions = entry.go_functions
-                    else:
-                        go_terms = []
-                        go_functions = []
-
-                    # add the domain to the protein domains of the right gene
-                    assert domain.env_from < domain.env_to
-                    assert domain.i_evalue >= 0
-                    assert domain.pvalue >= 0
-                    gene_index[target_index].protein.domains.append(
-                        Domain(
-                            accession,
-                            start,
-                            end,
-                            self.hmm.id,
-                            domain.i_evalue,
-                            domain.pvalue,
-                            go_terms=go_terms,
-                            go_functions=go_functions,
-                            qualifiers=qualifiers,
+            for hits in hmms_hits:
+                for hit in hits.reported:
+                    target_index = int(hit.name)
+                    for domain in hit.domains.reported:
+                        # extract name and get InterPro metadata about hit
+                        raw_acc = domain.alignment.hmm_accession or domain.alignment.hmm_name
+                        accession = self.hmm.relabel(raw_acc.decode('utf-8'))
+                        entry = interpro.by_accession.get(accession)
+
+                        # extract coordinates
+                        start = domain.alignment.target_from
+                        end = domain.alignment.target_to
+
+                        # extract qualifiers and GO terms
+                        qualifiers: Dict[str, List[str]] = {
+                            "inference": ["protein motif"],
+                            "db_xref": ["{}:{}".format(self.hmm.id.upper(), accession)],
+                            "note": [
+                                "e-value: {}".format(domain.i_evalue),
+                                "p-value: {}".format(domain.pvalue),
+                            ],
+                        }
+                        if entry is not None:
+                            qualifiers["function"] = [entry.name]
+                            qualifiers["db_xref"].append("InterPro:{}".format(entry.accession))
+                            go_terms = entry.go_terms
+                            go_functions = entry.go_functions
+                        else:
+                            go_terms = []
+                            go_functions = []
+
+                        # add the domain to the protein domains of the right gene
+                        assert domain.env_from < domain.env_to
+                        assert domain.i_evalue >= 0
+                        assert domain.pvalue >= 0
+                        gene_index[target_index].protein.domains.append(
+                            Domain(
+                                accession,
+                                start,
+                                end,
+                                self.hmm.id,
+                                domain.i_evalue,
+                                domain.pvalue,
+                                go_terms=go_terms,
+                                go_functions=go_functions,
+                                qualifiers=qualifiers,
+                            )
                         )
-                    )
-
-        # deduplicate hits per gene for exclusive HMMs
-        if self.hmm.exclusive:
-            for i, gene in enumerate(gene_index):
-                # extract domains specific to this HMM
-                hmm_domains = [
-                    domain for domain in gene.protein.domains
-                    if domain.hmm == self.hmm.id
-                ]
-                # if more than one domain was found, keep the one with lowest p-value
-                # (but make sure to keep any domain found by other HMMs, if any)
-                if len(hmm_domains) > 1:
-                    best_domain = min(hmm_domains, key=lambda domain: domain.pvalue)
-                    gene_index[i] = gene.with_protein(gene.protein.with_domains([
-                        domain for domain in gene.protein.domains
-                        if domain.hmm != self.hmm.id
-                        or domain.name is best_domain.name
-                    ]))
 
         # return the updated list of genes that was given in argument
         return gene_index
 
 
 def embedded_hmms() -> Iterator[HMM]:
     """Iterate over the embedded HMMs that are shipped with GECCO.
```

### Comparing `gecco-tool-0.9.6/gecco/interpro/__init__.py` & `gecco-tool-0.9.7/gecco/interpro/__init__.py`

 * *Files identical despite different names*

### Comparing `gecco-tool-0.9.6/gecco/interpro/interpro.json` & `gecco-tool-0.9.7/gecco/interpro/interpro.json`

 * *Files identical despite different names*

### Comparing `gecco-tool-0.9.6/gecco/model.py` & `gecco-tool-0.9.7/gecco/model.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,32 +6,35 @@
 import csv
 import datetime
 import enum
 import functools
 import itertools
 import math
 import operator
+import os
 import re
 import statistics
 import typing
 from array import array
 from collections import OrderedDict
 from collections.abc import Sized
 from dataclasses import dataclass, field
-from typing import Dict, Iterable, List, Mapping, Optional, Sequence, TextIO, NamedTuple, Union, Iterator, Set
+from typing import Dict, Iterable, List, Mapping, Optional, Sequence, BinaryIO, NamedTuple, Union, Iterator, Set
+from typing import Dict, Iterable, List, Mapping, Optional, Sequence, BinaryIO, NamedTuple, Union, Iterator
 
 import Bio
 import numpy
+import polars
 from Bio.Seq import Seq
 from Bio.SeqFeature import SeqFeature, FeatureLocation, CompoundLocation, Reference
 from Bio.SeqRecord import SeqRecord
 
 from . import __version__
 from .interpro import GOTerm
-from ._base import Dumpable, Table, _SELF
+from ._base import Dumpable, Table
 from ._meta import patch_locale
 
 if typing.TYPE_CHECKING:
     from numpy.typing import NDArray
 
 
 __all__ = [
@@ -61,14 +64,17 @@
 
         """
         self.names = frozenset(names)
 
     def __repr__(self) -> str:  # noqa: D105
         return "ClusterType({})".format(", ".join(map(repr, sorted(self.names))))
 
+    def __str__(self) -> str: # noqa: D105
+        return "Unknown" if not self else ";".join(sorted(self.names))
+
     def __hash__(self) -> int:  # noqa: D105
         return hash(self.names)
 
     def __eq__(self, other: object) -> bool:  # noqa: D105
         if not isinstance(other, ClusterType):
             return NotImplemented
         return self.names == other.names
@@ -397,22 +403,22 @@
             each cluster type was identified (same dimension as the ``types``
             attribute).
 
     """
 
     id: str
     genes: List[Gene]
-    type: ClusterType
+    type: Optional[ClusterType]
     type_probabilities: Dict[str, float]
 
     def __init__(
         self,
         id: str,
         genes: Optional[List[Gene]] = None,
-        type: ClusterType = ClusterType(),
+        type: Optional[ClusterType] = None,
         type_probabilities: Optional[Dict[str, float]] = None,
     ):  # noqa: D107
         self.id = id
         self.genes = genes or list()
         self.type = type
         self.type_probabilities = type_probabilities or dict()
 
@@ -542,23 +548,30 @@
             "Alessio Milanese",
             "Elisa Cappio Barazzone",
             "Georg Zeller"
         ])
         cluster.annotations.setdefault("references", []).append(ref)
 
         # add GECCO-specific annotations as a structured comment
-        probabilities = {
-            f"{key.lower()}_probability":f"{value:.3f}"
-            for key, value in self.type_probabilities.items()
-        }
+        if self.type is not None:
+            cluster_type = {
+                "cluster_type": ";".join(sorted(self.type.names)) or "Unknown"
+            }
+            probabilities = {
+                f"{key.lower()}_probability":f"{value:.3f}"
+                for key, value in self.type_probabilities.items()
+            }
+        else:
+            cluster_type = probabilities = {}
+
         structured_comment = cluster.annotations.setdefault("structured_comment", OrderedDict())
         structured_comment['GECCO-Data'] = {
             "version": f"GECCO v{__version__}",
             "creation_date": now.isoformat(),
-            "cluster_type": ";".join(sorted(self.type.names)) or "Unknown",
+            **cluster_type,
             **probabilities,
         }
 
         # add proteins as CDS features
         for gene in self.genes:
             # write gene as a /cds GenBank record
             cds = gene.to_seq_feature()
@@ -602,342 +615,208 @@
 
     def __getitem__(self, index: Union[slice, int]) -> Union[str, Seq]:
         if isinstance(index, slice):
             return Seq("N" * ((index.stop - index.start) // (index.step or 1)) )
         return "N"
 
 
-@dataclass(frozen=True)
 class FeatureTable(Table):
     """A table storing condensed domain annotations from different genes.
     """
 
-    sequence_id: List[str] = field(default_factory = list)
-    protein_id: List[str] = field(default_factory = list)
-    start: List[int] = field(default_factory = lambda: array("l"))          # type: ignore
-    end: List[int] = field(default_factory = lambda: array("l"))            # type: ignore
-    strand: List[str] = field(default_factory = list)
-    domain: List[str] = field(default_factory = list)
-    hmm: List[str] = field(default_factory = list)
-    i_evalue: List[float] = field(default_factory = lambda: array("d"))     # type: ignore
-    pvalue: List[float] = field(default_factory = lambda: array("d"))       # type: ignore
-    domain_start: List[int] = field(default_factory = lambda: array("l"))   # type: ignore
-    domain_end: List[int] = field(default_factory = lambda: array("l"))     # type: ignore
-    cluster_probability: List[Optional[float]] = field(default_factory = list)
-
-    class Row(NamedTuple):
-        """A single row in a feature table.
-        """
-
-        sequence_id: str
-        protein_id: str
-        start: int
-        end: int
-        strand: str
-        domain: str
-        hmm: str
-        i_evalue: float
-        pvalue: float
-        domain_start: int
-        domain_end: int
-        cluster_probability: Optional[float]
-
-    if typing.TYPE_CHECKING:
-
-        @typing.overload  # type: ignore
-        def __getitem__(self, item: int) -> "FeatureTable.Row":  # noqa: D105
-            pass
-
-        @typing.overload
-        def __getitem__(self, item: slice) -> "FeatureTable.Row":  # noqa: D105
-            pass
-
-        def __getitem__(self, item: Union[slice, int]) -> Union["FeatureTable", "FeatureTable.Row"]:   # noqa: D105
-            return super().__getitem__(item)  # type: ignore
-
-        def __iter__(self) -> Iterator["FeatureTable.Row"]:  # type: ignore  # noqa: D105
-            return super().__iter__()  # type: ignore
+    @classmethod
+    def _get_columns(cls) -> List["Table.Column"]:
+        return [
+            Table.Column("sequence_id", polars.Utf8),
+            Table.Column("protein_id", polars.Utf8),
+            Table.Column("start", polars.Int64),
+            Table.Column("end", polars.Int64),
+            Table.Column("strand", polars.Utf8),
+            Table.Column("domain", polars.Utf8),
+            Table.Column("hmm", polars.Utf8),
+            Table.Column("i_evalue", polars.Float64),
+            Table.Column("pvalue", polars.Float64),
+            Table.Column("domain_start", polars.Int64),
+            Table.Column("domain_end", polars.Int64),
+            Table.Column("cluster_probability", polars.Float64, default=math.nan),
+        ]
 
     @classmethod
     def from_genes(cls, genes: Iterable[Gene]) -> "FeatureTable":
         """Create a new feature table from an iterable of genes.
         """
-        table = cls()
+        columns = cls._get_columns()
+        data = { column.name: [] for column in columns }
         for gene in genes:
             for domain in gene.protein.domains:
-                table.sequence_id.append(gene.source.id)
-                table.protein_id.append(gene.protein.id)
-                table.start.append(gene.start)
-                table.end.append(gene.end)
-                table.strand.append(gene.strand.sign)
-                table.domain.append(domain.name)
-                table.hmm.append(domain.hmm)
-                table.i_evalue.append(domain.i_evalue)
-                table.pvalue.append(domain.pvalue)
-                table.domain_start.append(domain.start)
-                table.domain_end.append(domain.end)
-                table.cluster_probability.append(domain.probability)
-        return table
+                data["sequence_id"].append(gene.source.id)
+                data["protein_id"].append(gene.protein.id)
+                data["start"].append(gene.start)
+                data["end"].append(gene.end)
+                data["strand"].append(gene.strand.sign)
+                data["domain"].append(domain.name)
+                data["hmm"].append(domain.hmm)
+                data["i_evalue"].append(domain.i_evalue)
+                data["pvalue"].append(domain.pvalue)
+                data["domain_start"].append(domain.start)
+                data["domain_end"].append(domain.end)
+                if domain.probability is not None:
+                    data["cluster_probability"].append(domain.probability)
+        for name in list(data):
+            if not data[name]:
+                del data[name]
+        return cls(polars.DataFrame(data))
 
     def to_genes(self) -> Iterable[Gene]:
         """Convert a feature table to actual genes.
 
         Since the source sequence cannot be known, a *dummy* sequence is
         built for each gene of size ``gene.end``, so that each gene can still
         be converted to a `~Bio.SeqRecord.SeqRecord` if needed.
+
         """
         # group rows by protein/gene ID
         protein_indices = collections.defaultdict(list)
         for i, protein_id in enumerate(self.protein_id):
             protein_indices[protein_id].append(i)
         # yield genes in order
         for protein_id in sorted(protein_indices):
-            rows = [self[i] for i in protein_indices[protein_id]]
-            assert all(x.sequence_id == rows[0].sequence_id for x in rows)
-            assert all(x.protein_id == rows[0].protein_id for x in rows)
-            assert all(x.start == rows[0].start for x in rows)
-            assert all(x.end == rows[0].end for x in rows)
-            source = SeqRecord(id=rows[0].sequence_id, seq=_UnknownSeq())
-            strand = Strand.Coding if rows[0].strand == "+" else Strand.Reverse
-            protein = Protein(rows[0].protein_id, seq=_UnknownSeq)
-            gene = Gene(source, rows[0].start, rows[0].end, strand, protein)
-            for row in rows:
-                domain = Domain(row.domain, row.domain_start, row.domain_end, row.hmm, row.i_evalue, row.pvalue, row.cluster_probability)
+            indices = protein_indices[protein_id]
+            assert all(self.sequence_id[i] == self.sequence_id[indices[0]] for i in indices)
+            assert all(self.protein_id[i] == self.protein_id[indices[0]] for i in indices)
+            assert all(self.start[i] == self.start[indices[0]] for i in indices)
+            assert all(self.end[i] == self.end[indices[0]] for i in indices)
+            source = SeqRecord(id=self.sequence_id[indices[0]], seq=_UnknownSeq())
+            strand = Strand.Coding if self.strand[indices[0]] == "+" else Strand.Reverse
+            protein = Protein(self.protein_id[indices[0]], seq=_UnknownSeq)
+            gene = Gene(source, self.start[indices[0]], self.end[indices[0]], strand, protein)
+            for i in indices:
+                domain = Domain(
+                    self.domain[i], 
+                    self.domain_start[i], 
+                    self.domain_end[i],
+                    self.hmm[i], 
+                    self.i_evalue[i], 
+                    self.pvalue[i], 
+                    self.cluster_probability[i]
+                )
                 gene.protein.domains.append(domain)
             yield gene
 
-    def __len__(self) -> int:  # noqa: D105
-        return len(self.sequence_id)
-
-
-def _format_product_type(value: "ClusterType") -> str:
-    return ";".join(sorted(value.names))
-
-
-def _parse_product_type(value: str) -> "ClusterType":
-    return ClusterType(*map(str.strip, value.split(";"))) if value.strip() else ClusterType()
 
-
-@dataclass(frozen=True)
 class ClusterTable(Table):
     """A table storing condensed information from several clusters.
     """
 
-    sequence_id: List[str] = field(default_factory = list)
-    cluster_id: List[str] = field(default_factory = list)
-    start: List[int] = field(default_factory = lambda: array("l"))   # type: ignore
-    end: List[int] = field(default_factory = lambda: array("l"))     # type: ignore
-    average_p: List[Optional[float]] = field(default_factory = list)
-    max_p: List[Optional[float]] = field(default_factory = list)
-
-    type: List[ClusterType] = field(default_factory = list)
-    type_p: List[Dict[str, float]] = field(default_factory = list)
-
-    proteins: List[Optional[List[str]]] = field(default_factory = list)
-    domains: List[Optional[List[str]]] = field(default_factory = list)
-
-    class Row(NamedTuple):
-        """A single row in a cluster table.
-        """
-
-        sequence_id: str
-        cluster_id: str
-        start: int
-        end: int
-        average_p: Optional[float]
-        max_p: Optional[float]
-
-        type: ClusterType
-        type_p: Dict[ClusterType, float]
-
-        proteins: Optional[List[str]]
-        domains: Optional[List[str]]
-
-    _FORMAT_FIELD = {ClusterType: _format_product_type, **Table._FORMAT_FIELD}
-    _PARSE_FIELD = {ClusterType: _parse_product_type, **Table._PARSE_FIELD}
+    @classmethod
+    def _get_columns(cls) -> List["Table.Column"]:
+        return [
+            Table.Column("sequence_id", polars.Utf8),
+            Table.Column("cluster_id", polars.Utf8),
+            Table.Column("start", polars.Int64),
+            Table.Column("end", polars.Int64),
+            Table.Column("average_p", polars.Float64, default=math.nan),
+            Table.Column("max_p", polars.Float64, default=math.nan),
+            Table.Column("type", polars.Utf8, default="Unknown"),
+            # + possible type columns that are handled in `from_clusters`
+            Table.Column("proteins", polars.Utf8, default=""),
+            Table.Column("domains", polars.Utf8, default=""),
+        ]
 
     @classmethod
     def from_clusters(cls, clusters: Iterable[Cluster]) -> "ClusterTable":
         """Create a new cluster table from an iterable of clusters.
         """
-        table = cls()
+        data = collections.defaultdict(list)
         for cluster in clusters:
-            table.sequence_id.append(cluster.source.id)
-            table.cluster_id.append(cluster.id)
-            table.start.append(cluster.start)
-            table.end.append(cluster.end)
-            table.average_p.append(cluster.average_probability)
-            table.max_p.append(cluster.maximum_probability)
-
-            table.type.append(cluster.type)
-            table.type_p.append(cluster.type_probabilities.copy())
-
-            table.proteins.append([ gene.protein.id for gene in cluster.genes ])
-            domains = {d.name for g in cluster.genes for d in g.protein.domains}
-            table.domains.append(sorted(domains))
-        return table
-
-    def __len__(self) -> int:  # noqa: D105
-        return len(self.sequence_id)
-
-    if typing.TYPE_CHECKING:
-
-        @typing.overload  # type: ignore
-        def __getitem__(self, item: int) -> "ClusterTable.Row":  # noqa: D105
-            pass
-
-        @typing.overload
-        def __getitem__(self, item: slice) -> "ClusterTable.Row":  # noqa: D105
-            pass
-
-        def __getitem__(self, item: Union[slice, int]) -> Union["ClusterTable", "ClusterTable.Row"]:   # noqa: D105
-            return super().__getitem__(item)  # type: ignore
-
-        def __iter__(self) -> Iterator["ClusterTable.Row"]:  # type: ignore  # noqa: D105
-            return super().__iter__()  # type: ignore
-
-    def dump(self, fh: TextIO, dialect: str = "excel-tab", header: bool = True) -> None:  # noqa: D102
-        writer = csv.writer(fh, dialect=dialect)
-        column_names = list(self.__annotations__)
-        type_p_col = column_names.index("type_p")
-        column_names.pop(type_p_col)
-        optional = self._optional_columns()
-
-        # do not write optional columns if they are completely empty
-        for name in optional:
-            if all(x is None for x in getattr(self, name)):
-                column_names.remove(name)
-
-        # build column formatters
-        columns = [getattr(self, name) for name in column_names]
-        formatters = [self._FORMAT_FIELD[self.Row.__annotations__[name]] for name in column_names]
-
-        # add probability columns if any row countains probabilities
-        if any(d for d in self.type_p):
-            classes = sorted({
-                name
-                for probabilities in self.type_p
-                for name in probabilities.keys()
-            })
-            for name in classes:
-                column_names.insert(type_p_col, f"{name.lower()}_probability")
-                columns.insert(type_p_col, [self.type_p[i][name] for i in range(len(self))])
-                formatters.insert(type_p_col, str)  # type: ignore
-                type_p_col += 1
-
-         # write header if desired
-        if header:
-            writer.writerow(column_names)
-        # write each row
-        for i in range(len(self)):
-            writer.writerow([format(col[i]) for col,format in zip(columns, formatters)])
+            data["sequence_id"].append(cluster.source.id)
+            data["bgc_id"].append(cluster.id)
+            data["start"].append(cluster.start)
+            data["end"].append(cluster.end)
+            if cluster.average_probability is not None:
+                data["average_p"].append(cluster.average_probability)
+            if cluster.maximum_probability is not None:
+                data["max_p"].append(cluster.maximum_probability)
+            if cluster.type is not None:
+                data["type"].append(str(cluster.type))
+                for type_name in sorted(cluster.type_probabilities, key=str.casefold):
+                    data[f"{type_name.lower()}_probability"].append(cluster.type_probabilities[type_name])
+            data["proteins"].append(";".join(
+                sorted(gene.protein.id for gene in cluster.genes)
+            ))
+            data["domains"].append(";".join(sorted( 
+                domain.name 
+                for gene in cluster.genes 
+                for domain in gene.protein.domains 
+            )))
+            # TODO: member proteins
+            # TODO: member domains
+        return cls(polars.DataFrame(data))
+
+    def dump(self, fh: Union[BinaryIO, str, os.PathLike]) -> None:
+        # patch `Table.dump` so that all columns are always written
+        data = self.data
+        for column_name in data.columns:
+            if data[column_name].dtype in (polars.Float64, polars.Float64):
+                data = data.with_columns(polars.col(column_name).fill_nan(None))
+        data.write_csv(fh, sep="\t")
 
-    @classmethod
-    def load(cls, fh: TextIO, dialect: str = "excel-tab") -> "ClusterTable":  # noqa: D102
-        table = cls()
-        reader = csv.reader(fh, dialect=dialect)
-        header = next(reader)
-
-        # check that if a column is missing, it is one of the optional values
-        optional = cls._optional_columns()
-        missing = set(cls.__annotations__).difference({"type_p"}).difference(header)
-        missing_required = missing.difference(optional)
-        if missing_required:
-            raise ValueError("table is missing columns: {}".format(", ".join(missing_required)))
-
-        # get the name of each column and check which columns are optional
-        columns = [getattr(table, col, None) for col in header]
-        parsers = [
-            cls._PARSE_FIELD[table.Row.__annotations__[col]]
-            if col in table.Row.__annotations__
-            else None
-            for col in header
-        ]
 
-        # extract elements from the CSV rows
-        for row in reader:
-            probabilities = {}
-            for name, col, value, parser in zip(header, columns, row, parsers):
-                if parser is not None and col is not None:
-                    col.append(parser(value))
-                elif name.endswith("_probability"):
-                    probabilities[name[:-12]] = float(value)
-            table.type_p.append(probabilities)
-
-        for col in missing:
-            getattr(table, col).extend(None for _ in range(len(table)))
-        return table
-
-
-@dataclass(frozen=True)
 class GeneTable(Table):
     """A table storing gene coordinates and optional cluster probabilities.
     """
 
-    sequence_id: List[str] = field(default_factory = list)
-    protein_id: List[str] = field(default_factory = list)
-    start: List[int] = field(default_factory = lambda: array("l"))    # type: ignore
-    end: List[int] = field(default_factory = lambda: array("l"))      # type: ignore
-    strand: List[str] = field(default_factory = list)
-    average_p: List[Optional[float]] = field(default_factory = list)
-    max_p: List[Optional[float]] = field(default_factory = list)
-
-    class Row(NamedTuple):
-        """A single row in a gene table.
-        """
-
-        sequence_id: str
-        protein_id: str
-        start: int
-        end: int
-        strand: str
-        average_p: Optional[float]
-        max_p: Optional[float]
-
-    if typing.TYPE_CHECKING:
-
-        @typing.overload  # type: ignore
-        def __getitem__(self, item: int) -> "GeneTable.Row":  # noqa: D105
-            pass
-
-        @typing.overload
-        def __getitem__(self, item: slice) -> "GeneTable.Row":  # noqa: D105
-            pass
-
-        def __getitem__(self, item: Union[slice, int]) -> Union["GeneTable", "GeneTable.Row"]:   # noqa: D105
-            return super().__getitem__(item)  # type: ignore
-
-        def __iter__(self) -> Iterator["GeneTable.Row"]:  # type: ignore  # noqa: D105
-            return super().__iter__()  # type: ignore
+    @classmethod
+    def _get_columns(cls) -> List["Table.Column"]:
+        return [
+            Table.Column("sequence_id", polars.Utf8),
+            Table.Column("protein_id", polars.Utf8),
+            Table.Column("start", polars.Int64),
+            Table.Column("end", polars.Int64),
+            Table.Column("strand", polars.Utf8),
+            Table.Column("average_p", polars.Float64, default=math.nan),
+            Table.Column("max_p", polars.Float64, default=math.nan),
+        ]
 
     @classmethod
     def from_genes(cls, genes: Iterable[Gene]) -> "GeneTable":
         """Create a new gene table from an iterable of genes.
         """
-        table = cls()
+        columns = cls._get_columns()
+        data = { column.name: [] for column in columns }
         for gene in genes:
-            table.sequence_id.append(gene.source.id)
-            table.protein_id.append(gene.protein.id)
-            table.start.append(gene.start)
-            table.end.append(gene.end)
-            table.strand.append(gene.strand.sign)
-            table.average_p.append(gene.average_probability)
-            table.max_p.append(gene.maximum_probability)
-        return table
+            data["sequence_id"].append(gene.source.id)
+            data["protein_id"].append(gene.protein.id)
+            data["start"].append(gene.start)
+            data["end"].append(gene.end)
+            data["strand"].append(gene.strand.sign)
+            if gene.average_probability is not None:
+                data["average_p"].append(gene.average_probability)
+            else:
+                data["average_p"].append(math.nan)
+            if gene.maximum_probability is not None:
+                data["max_p"].append(gene.maximum_probability)
+            else:
+                data["max_p"].append(math.nan)
+        return cls(polars.DataFrame(data))
 
     def to_genes(self) -> Iterable[Gene]:
         """Convert a gene table to actual genes.
 
         Since the source sequence cannot be known, a *dummy* sequence is
         built for each gene of size ``gene.end``, so that each gene can still
         be converted to a `~Bio.SeqRecord.SeqRecord` if needed.
 
         """
-        for row in typing.cast(Iterable["GeneTable.Row"], self):
-            source = SeqRecord(id=row.sequence_id, seq=_UnknownSeq())
-            strand = Strand.Coding if row.strand == "+" else Strand.Reverse
-            seq = Seq("X" * (row.end - row.start // 3))
-            protein = Protein(row.protein_id, seq=_UnknownSeq())
-            yield Gene(source, row.start, row.end, strand, protein, _probability=row.average_p)
-
-    def __len__(self) -> int:  # noqa: D105
-        return len(self.protein_id)
+        # check if a probability column is available 
+        has_probas = "average_p" in self.data.columns
+        # yield genes in order
+        for i, protein_id in enumerate(self.protein_id):
+            source = SeqRecord(id=self.sequence_id[i], seq=_UnknownSeq())
+            strand = Strand.Coding if self.strand[i] == "+" else Strand.Reverse
+            start = self.start[i]
+            end = self.end[i]
+            seq = Seq("X" * ((end - start) // 3))
+            protein = Protein(self.protein_id[i], seq=seq)
+            probability = self.average_p[i] if has_probas else None
+            gene = Gene(source, start, end, strand, protein, _probability=probability)
+            yield gene
```

### Comparing `gecco-tool-0.9.6/gecco/orf.py` & `gecco-tool-0.9.7/gecco/orf.py`

 * *Files identical despite different names*

### Comparing `gecco-tool-0.9.6/gecco/refine.py` & `gecco-tool-0.9.7/gecco/refine.py`

 * *Files identical despite different names*

### Comparing `gecco-tool-0.9.6/gecco/types/__init__.py` & `gecco-tool-0.9.7/gecco/types/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,16 @@
                 for ty in filter(None, line.split("\t")[1].strip().split(";")):
                     unpacked.add(ty)
                     unique_types.add(ty)
                 types.append(ClusterType(*unpacked))
 
         classifier = cls(classes=sorted(unique_types), random_state=0)
         types_bin = classifier.binarizer.transform(types)
-        classifier.model.fit(compositions, y=types_bin)
+        if len(classifier.classes_) > 1:
+            classifier.model.fit(compositions, y=types_bin)
         classifier.model.attributes_ = domains
         return classifier
 
     def __init__(self, classes: Iterable[str] = (), **kwargs: object) -> None:
         """Instantiate a new type classifier.
 
         Keyword Arguments:
```

### Comparing `gecco-tool-0.9.6/gecco/types/compositions.npz` & `gecco-tool-0.9.7/gecco/types/compositions.npz`

 * *Files identical despite different names*

### Comparing `gecco-tool-0.9.6/gecco/types/domains.tsv` & `gecco-tool-0.9.7/gecco/types/domains.tsv`

 * *Files identical despite different names*

### Comparing `gecco-tool-0.9.6/gecco/types/types.tsv` & `gecco-tool-0.9.7/gecco/types/types.tsv`

 * *Files identical despite different names*

### Comparing `gecco-tool-0.9.6/gecco_tool.egg-info/PKG-INFO` & `gecco-tool-0.9.7/gecco_tool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gecco-tool
-Version: 0.9.6
+Version: 0.9.7
 Summary: Gene cluster prediction with Conditional random fields.
 Home-page: https://gecco.embl.de
 Author: Martin Larralde
 Author-email: martin.larralde@embl.de
 License: GPLv3
 Project-URL: Repository, https://github.com/zellerlab/GECCO
 Project-URL: Bug Tracker, https://github.com/zellerlab/GECCO/issues
@@ -17,23 +17,23 @@
 Platform: powerpc
 Platform: ppc64
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Typing :: Typed
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: train
 License-File: LICENSE
 
 <img align="right" width="180" height="180" src="https://raw.githubusercontent.com/zellerlab/GECCO/v0.6.2/static/gecco-square.png">
 
 # Hi, I'm GECCO!
@@ -59,15 +59,15 @@
 [![Versions](https://img.shields.io/pypi/pyversions/gecco-tool.svg?style=flat-square&maxAge=3600)](https://pypi.org/project/gecco-tool/#files)
 [![Wheel](https://img.shields.io/pypi/wheel/gecco-tool?style=flat-square&maxAge=3600)](https://pypi.org/project/gecco-tool/#files)
 
 
 ## 🔧 Installing GECCO
 
 GECCO is implemented in [Python](https://www.python.org/), and supports [all
-versions](https://endoflife.date/python) from Python 3.6. It requires
+versions](https://endoflife.date/python) from Python 3.7. It requires
 additional libraries that can be installed directly from
 [PyPI](https://pypi.org), the Python Package Index.
 
 Use [`pip`](https://pip.pypa.io/en/stable/) to install GECCO on your
 machine:
 ```console
 $ pip install gecco-tool
```

### Comparing `gecco-tool-0.9.6/gecco_tool.egg-info/SOURCES.txt` & `gecco-tool-0.9.7/gecco_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gecco-tool-0.9.6/setup.cfg` & `gecco-tool-0.9.7/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 platform = x86, x86_64, powerpc, ppc64
 classifiers = 
 	Development Status :: 3 - Alpha
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 	Operating System :: POSIX
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Scientific/Engineering :: Bio-Informatics
 	Topic :: Scientific/Engineering :: Medical Science Apps.
 	Typing :: Typed
 project_urls = 
 	Repository = https://github.com/zellerlab/GECCO
 	Bug Tracker = https://github.com/zellerlab/GECCO/issues
 	Changelog = https://github.com/zellerlab/GECCO/blob/master/CHANGELOG.md
@@ -31,43 +31,39 @@
 	Builds = https://git.embl.de/grp-zeller/GECCO/-/pipelines
 	Preprint = https://www.biorxiv.org/content/10.1101/2021.05.03.442509v1
 
 [options]
 zip_safe = false
 packages = find:
 include_package_data = true
-python_requires = >=3.6
+python_requires = >=3.7
 setup_requires = 
 	setuptools >=39.2
 	rich >=12.4.0
-	pyhmmer ~=0.7.0
+	pyhmmer ~=0.8.0
 	wheel >=0.30
 	pronto ~=2.2
 install_requires = 
 	biopython ~=1.73
-	dataclasses ~=0.8             ; python_version < '3.7'
 	docopt ~=0.6.2
 	importlib-metadata >=4.0      ; python_version < '3.10'
-	importlib-resources >=1.0     ; python_version < '3.7'
 	numpy ~=1.16
+	polars ~=0.16.1
 	psutil ~=5.8
-	pyhmmer ~=0.7.0
-	pyrodigal ~=2.0
+	pyhmmer ~=0.8.0
+	pyrodigal ~=2.1
 	rich >=12.4.0
-	scikit-learn ~=0.24.0         ; python_version < '3.7'
-	scikit-learn ~=1.0            ; python_version >= '3.7'
+	scikit-learn ~=1.0
 	scipy ~=1.4
 	sklearn-crfsuite ~=0.3.6
 
 [options.extras_require]
 train = 
 	fisher ~=0.1.10
-	pandas ~=1.0
-	statsmodels ~=0.12.1          ; python_version < '3.7'
-	statsmodels ~=0.13.0          ; python_version >= '3.7'
+	statsmodels ~=0.13.0
 
 [options.packages.find]
 include = 
 	gecco
 	gecco.cli
 	gecco.cli.commands
 	gecco.crf
```

### Comparing `gecco-tool-0.9.6/setup.py` & `gecco-tool-0.9.7/setup.py`

 * *Files identical despite different names*

### Comparing `gecco-tool-0.9.6/static/gecco.png` & `gecco-tool-0.9.7/static/gecco.png`

 * *Files identical despite different names*

