# Comparing `tmp/spl_widgets-1.5.0.tar.gz` & `tmp/spl_widgets-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spl_widgets-1.5.0.tar", last modified: Fri May 26 16:38:24 2023, max compression
+gzip compressed data, was "spl_widgets-1.5.1.tar", last modified: Fri May 26 16:46:21 2023, max compression
```

## Comparing `spl_widgets-1.5.0.tar` & `spl_widgets-1.5.1.tar`

### file list

```diff
@@ -1,27 +1,31 @@
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-05-26 16:38:24.517957 spl_widgets-1.5.0/
--rw-r--r--   0 colin      (501) staff       (20)     1073 2021-11-03 16:44:37.000000 spl_widgets-1.5.0/LICENSE
--rw-r--r--   0 colin      (501) staff       (20)      411 2023-05-26 16:38:24.517649 spl_widgets-1.5.0/PKG-INFO
--rw-r--r--   0 colin      (501) staff       (20)     2101 2022-06-26 15:02:40.000000 spl_widgets-1.5.0/README.md
--rw-r--r--   0 colin      (501) staff       (20)      103 2021-11-03 16:36:22.000000 spl_widgets-1.5.0/pyproject.toml
--rw-r--r--   0 colin      (501) staff       (20)       38 2023-05-26 16:38:24.518037 spl_widgets-1.5.0/setup.cfg
--rw-r--r--   0 colin      (501) staff       (20)     1178 2023-05-26 16:38:11.000000 spl_widgets-1.5.0/setup.py
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-05-26 16:38:24.475472 spl_widgets-1.5.0/src/
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-05-26 16:38:24.489323 spl_widgets-1.5.0/src/spl_widgets/
--rw-r--r--   0 colin      (501) staff       (20)      279 2022-06-26 16:32:08.000000 spl_widgets-1.5.0/src/spl_widgets/__init__.py
--rw-r--r--   0 colin      (501) staff       (20)        0 2022-06-26 14:59:05.000000 spl_widgets-1.5.0/src/spl_widgets/__main__.py
--rw-r--r--   0 colin      (501) staff       (20)     3722 2023-05-26 16:24:48.000000 spl_widgets-1.5.0/src/spl_widgets/batch_tune.py
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-05-26 16:38:24.494042 spl_widgets-1.5.0/src/spl_widgets/data/
--rw-r--r--   0 colin      (501) staff       (20)  9670656 2023-05-26 16:25:12.000000 spl_widgets-1.5.0/src/spl_widgets/data/cmudict.sqlite
--rwxr-xr-x   0 colin      (501) staff       (20)     5378 2022-10-21 13:14:40.000000 spl_widgets-1.5.0/src/spl_widgets/gorilla_clean.py
--rw-r--r--   0 colin      (501) staff       (20)     2483 2022-12-17 21:45:28.000000 spl_widgets-1.5.0/src/spl_widgets/jukemake.py
--rw-r--r--   0 colin      (501) staff       (20)     4166 2023-05-25 22:28:36.000000 spl_widgets-1.5.0/src/spl_widgets/misc_util.py
--rwxr-xr-x   0 colin      (501) staff       (20)     3598 2023-04-14 19:27:21.000000 spl_widgets-1.5.0/src/spl_widgets/stk_swx.py
--rw-r--r--   0 colin      (501) staff       (20)     3614 2023-04-23 14:58:27.000000 spl_widgets-1.5.0/src/spl_widgets/tune_freq.py
--rw-r--r--   0 colin      (501) staff       (20)    17694 2023-05-26 16:20:21.000000 spl_widgets-1.5.0/src/spl_widgets/tuner.py
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-05-26 16:38:24.493461 spl_widgets-1.5.0/src/spl_widgets.egg-info/
--rw-r--r--   0 colin      (501) staff       (20)      411 2023-05-26 16:38:24.000000 spl_widgets-1.5.0/src/spl_widgets.egg-info/PKG-INFO
--rw-r--r--   0 colin      (501) staff       (20)      570 2023-05-26 16:38:24.000000 spl_widgets-1.5.0/src/spl_widgets.egg-info/SOURCES.txt
--rw-r--r--   0 colin      (501) staff       (20)        1 2023-05-26 16:38:24.000000 spl_widgets-1.5.0/src/spl_widgets.egg-info/dependency_links.txt
--rw-r--r--   0 colin      (501) staff       (20)      265 2023-05-26 16:38:24.000000 spl_widgets-1.5.0/src/spl_widgets.egg-info/entry_points.txt
--rw-r--r--   0 colin      (501) staff       (20)        7 2023-05-26 16:38:24.000000 spl_widgets-1.5.0/src/spl_widgets.egg-info/requires.txt
--rw-r--r--   0 colin      (501) staff       (20)       12 2023-05-26 16:38:24.000000 spl_widgets-1.5.0/src/spl_widgets.egg-info/top_level.txt
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-05-26 16:46:21.202797 spl_widgets-1.5.1/
+-rw-r--r--   0 colin      (501) staff       (20)     1073 2021-11-03 16:44:37.000000 spl_widgets-1.5.1/LICENSE
+-rw-r--r--   0 colin      (501) staff       (20)      411 2023-05-26 16:46:21.202222 spl_widgets-1.5.1/PKG-INFO
+-rw-r--r--   0 colin      (501) staff       (20)     2101 2022-06-26 15:02:40.000000 spl_widgets-1.5.1/README.md
+-rw-r--r--   0 colin      (501) staff       (20)      103 2021-11-03 16:36:22.000000 spl_widgets-1.5.1/pyproject.toml
+-rw-r--r--   0 colin      (501) staff       (20)       38 2023-05-26 16:46:21.202912 spl_widgets-1.5.1/setup.cfg
+-rw-r--r--   0 colin      (501) staff       (20)     1197 2023-05-26 16:46:01.000000 spl_widgets-1.5.1/setup.py
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-05-26 16:46:21.142418 spl_widgets-1.5.1/src/
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-05-26 16:46:21.155588 spl_widgets-1.5.1/src/spl_widgets/
+-rw-r--r--   0 colin      (501) staff       (20)      279 2022-06-26 16:32:08.000000 spl_widgets-1.5.1/src/spl_widgets/__init__.py
+-rw-r--r--   0 colin      (501) staff       (20)        0 2022-06-26 14:59:05.000000 spl_widgets-1.5.1/src/spl_widgets/__main__.py
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-05-26 16:46:21.165541 spl_widgets-1.5.1/src/spl_widgets/autoscorer/
+-rw-r--r--   0 colin      (501) staff       (20)    13677 2023-05-26 16:37:32.000000 spl_widgets-1.5.1/src/spl_widgets/autoscorer/autoscore.py
+-rw-r--r--   0 colin      (501) staff       (20)    15285 2023-05-26 16:35:21.000000 spl_widgets-1.5.1/src/spl_widgets/autoscorer/autoscorer_gui.py
+-rw-r--r--   0 colin      (501) staff       (20)     5387 2023-05-26 16:37:26.000000 spl_widgets-1.5.1/src/spl_widgets/autoscorer/tokenize_to_ipa.py
+-rw-r--r--   0 colin      (501) staff       (20)     3722 2023-05-26 16:24:48.000000 spl_widgets-1.5.1/src/spl_widgets/batch_tune.py
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-05-26 16:46:21.166497 spl_widgets-1.5.1/src/spl_widgets/data/
+-rw-r--r--   0 colin      (501) staff       (20)  9670656 2023-05-26 16:25:12.000000 spl_widgets-1.5.1/src/spl_widgets/data/cmudict.sqlite
+-rwxr-xr-x   0 colin      (501) staff       (20)     5378 2022-10-21 13:14:40.000000 spl_widgets-1.5.1/src/spl_widgets/gorilla_clean.py
+-rw-r--r--   0 colin      (501) staff       (20)     2483 2022-12-17 21:45:28.000000 spl_widgets-1.5.1/src/spl_widgets/jukemake.py
+-rw-r--r--   0 colin      (501) staff       (20)     4166 2023-05-25 22:28:36.000000 spl_widgets-1.5.1/src/spl_widgets/misc_util.py
+-rwxr-xr-x   0 colin      (501) staff       (20)     3598 2023-04-14 19:27:21.000000 spl_widgets-1.5.1/src/spl_widgets/stk_swx.py
+-rw-r--r--   0 colin      (501) staff       (20)     3614 2023-04-23 14:58:27.000000 spl_widgets-1.5.1/src/spl_widgets/tune_freq.py
+-rw-r--r--   0 colin      (501) staff       (20)    17694 2023-05-26 16:20:21.000000 spl_widgets-1.5.1/src/spl_widgets/tuner.py
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-05-26 16:46:21.160054 spl_widgets-1.5.1/src/spl_widgets.egg-info/
+-rw-r--r--   0 colin      (501) staff       (20)      411 2023-05-26 16:46:21.000000 spl_widgets-1.5.1/src/spl_widgets.egg-info/PKG-INFO
+-rw-r--r--   0 colin      (501) staff       (20)      701 2023-05-26 16:46:21.000000 spl_widgets-1.5.1/src/spl_widgets.egg-info/SOURCES.txt
+-rw-r--r--   0 colin      (501) staff       (20)        1 2023-05-26 16:46:21.000000 spl_widgets-1.5.1/src/spl_widgets.egg-info/dependency_links.txt
+-rw-r--r--   0 colin      (501) staff       (20)      265 2023-05-26 16:46:21.000000 spl_widgets-1.5.1/src/spl_widgets.egg-info/entry_points.txt
+-rw-r--r--   0 colin      (501) staff       (20)       19 2023-05-26 16:46:21.000000 spl_widgets-1.5.1/src/spl_widgets.egg-info/requires.txt
+-rw-r--r--   0 colin      (501) staff       (20)       12 2023-05-26 16:46:21.000000 spl_widgets-1.5.1/src/spl_widgets.egg-info/top_level.txt
```

### Comparing `spl_widgets-1.5.0/LICENSE` & `spl_widgets-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.5.0/README.md` & `spl_widgets-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.5.0/setup.py` & `spl_widgets-1.5.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import setuptools
 
 # with open("README.md", "r", encoding="utf-8") as fh:
 #     long_description = fh.read()
 
 setuptools.setup(
     name="spl_widgets",
-    version="1.5.0",
+    version="1.5.1",
     author="Colin Simon-Fellowes",
     author_email="colin.tsf@gmail.com",
     description="Widgets for the Barnard Speech Perception Laboratory",
     # long_description=long_description,
     # long_description_content_type="text/markdown",
     url="https://github.com/clntsf/spl_widgets",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: MacOS",
     ],
     package_dir={"": "src"},
-    packages=setuptools.find_packages(where="src"),
-    install_requires=['pandas'],
+    packages=["spl_widgets", "spl_widgets.autoscorer"],
+    install_requires=['pandas', 'tkinterdnd2'],
     python_requires=">=3.8",
     entry_points='''
         [console_scripts]
         gorilla_clean=spl_widgets.gorilla_clean:main
         tuner=spl_widgets.tuner:main
         stk_swx=spl_widgets.stk_swx:main
         batch_tune=spl_widgets.batch_tune:main
```

### Comparing `spl_widgets-1.5.0/src/spl_widgets/batch_tune.py` & `spl_widgets-1.5.1/src/spl_widgets/batch_tune.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.5.0/src/spl_widgets/data/cmudict.sqlite` & `spl_widgets-1.5.1/src/spl_widgets/data/cmudict.sqlite`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.5.0/src/spl_widgets/gorilla_clean.py` & `spl_widgets-1.5.1/src/spl_widgets/gorilla_clean.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.5.0/src/spl_widgets/jukemake.py` & `spl_widgets-1.5.1/src/spl_widgets/jukemake.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.5.0/src/spl_widgets/misc_util.py` & `spl_widgets-1.5.1/src/spl_widgets/misc_util.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.5.0/src/spl_widgets/stk_swx.py` & `spl_widgets-1.5.1/src/spl_widgets/stk_swx.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.5.0/src/spl_widgets/tune_freq.py` & `spl_widgets-1.5.1/src/spl_widgets/tune_freq.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.5.0/src/spl_widgets/tuner.py` & `spl_widgets-1.5.1/src/spl_widgets/tuner.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.5.0/src/spl_widgets.egg-info/SOURCES.txt` & `spl_widgets-1.5.1/src/spl_widgets.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -13,8 +13,11 @@
 src/spl_widgets/tuner.py
 src/spl_widgets.egg-info/PKG-INFO
 src/spl_widgets.egg-info/SOURCES.txt
 src/spl_widgets.egg-info/dependency_links.txt
 src/spl_widgets.egg-info/entry_points.txt
 src/spl_widgets.egg-info/requires.txt
 src/spl_widgets.egg-info/top_level.txt
+src/spl_widgets/autoscorer/autoscore.py
+src/spl_widgets/autoscorer/autoscorer_gui.py
+src/spl_widgets/autoscorer/tokenize_to_ipa.py
 src/spl_widgets/data/cmudict.sqlite
```

