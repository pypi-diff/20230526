# Comparing `tmp/mono-dense-keras-0.0.6rc0.tar.gz` & `tmp/mono-dense-keras-0.0.6rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mono-dense-keras-0.0.6rc0.tar", last modified: Fri May 26 14:23:55 2023, max compression
+gzip compressed data, was "mono-dense-keras-0.0.6rc1.tar", last modified: Fri May 26 14:28:10 2023, max compression
```

## Comparing `mono-dense-keras-0.0.6rc0.tar` & `mono-dense-keras-0.0.6rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-05-26 14:23:55.472180 mono-dense-keras-0.0.6rc0/
--rw-r--r--   0 davor     (1000) davor     (1000)    20848 2022-09-02 19:27:53.000000 mono-dense-keras-0.0.6rc0/LICENSE
--rw-rw-r--   0 davor     (1000) davor     (1000)      111 2022-08-18 19:39:58.000000 mono-dense-keras-0.0.6rc0/MANIFEST.in
--rw-rw-r--   0 davor     (1000) davor     (1000)     7453 2023-05-26 14:23:55.472180 mono-dense-keras-0.0.6rc0/PKG-INFO
--rw-rw-r--   0 davor     (1000) davor     (1000)     6546 2023-05-26 14:19:35.000000 mono-dense-keras-0.0.6rc0/README.md
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-05-26 14:23:55.472180 mono-dense-keras-0.0.6rc0/airt/
--rw-r--r--   0 davor     (1000) davor     (1000)       22 2022-09-03 17:11:42.000000 mono-dense-keras-0.0.6rc0/airt/__init__.py
--rw-r--r--   0 davor     (1000) davor     (1000)     1275 2022-09-03 17:11:04.000000 mono-dense-keras-0.0.6rc0/airt/_modidx.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-05-26 14:23:55.472180 mono-dense-keras-0.0.6rc0/airt/keras/
--rw-r--r--   0 davor     (1000) davor     (1000)        0 2022-09-03 17:11:01.000000 mono-dense-keras-0.0.6rc0/airt/keras/__init__.py
--rw-r--r--   0 davor     (1000) davor     (1000)     3906 2022-09-03 17:11:01.000000 mono-dense-keras-0.0.6rc0/airt/keras/layers.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-05-26 14:23:55.472180 mono-dense-keras-0.0.6rc0/mono_dense_keras/
--rw-rw-r--   0 davor     (1000) davor     (1000)      472 2023-05-26 14:19:35.000000 mono-dense-keras-0.0.6rc0/mono_dense_keras/__init__.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-05-26 14:23:55.472180 mono-dense-keras-0.0.6rc0/mono_dense_keras/_components/
--rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-05-26 14:19:35.000000 mono-dense-keras-0.0.6rc0/mono_dense_keras/_components/__init__.py
--rw-rw-r--   0 davor     (1000) davor     (1000)    10318 2023-05-26 14:19:35.000000 mono-dense-keras-0.0.6rc0/mono_dense_keras/_components/mono_dense_layer.py
--rw-rw-r--   0 davor     (1000) davor     (1000)     4050 2023-05-26 14:19:35.000000 mono-dense-keras-0.0.6rc0/mono_dense_keras/_modidx.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-05-26 14:23:55.472180 mono-dense-keras-0.0.6rc0/mono_dense_keras.egg-info/
--rw-r--r--   0 davor     (1000) davor     (1000)     7453 2023-05-26 14:23:55.000000 mono-dense-keras-0.0.6rc0/mono_dense_keras.egg-info/PKG-INFO
--rw-r--r--   0 davor     (1000) davor     (1000)      556 2023-05-26 14:23:55.000000 mono-dense-keras-0.0.6rc0/mono_dense_keras.egg-info/SOURCES.txt
--rw-r--r--   0 davor     (1000) davor     (1000)        1 2023-05-26 14:23:55.000000 mono-dense-keras-0.0.6rc0/mono_dense_keras.egg-info/dependency_links.txt
--rw-r--r--   0 davor     (1000) davor     (1000)       54 2023-05-26 14:23:55.000000 mono-dense-keras-0.0.6rc0/mono_dense_keras.egg-info/entry_points.txt
--rw-r--r--   0 davor     (1000) davor     (1000)        1 2022-12-06 04:51:35.000000 mono-dense-keras-0.0.6rc0/mono_dense_keras.egg-info/not-zip-safe
--rw-r--r--   0 davor     (1000) davor     (1000)      219 2023-05-26 14:23:55.000000 mono-dense-keras-0.0.6rc0/mono_dense_keras.egg-info/requires.txt
--rw-r--r--   0 davor     (1000) davor     (1000)       22 2023-05-26 14:23:55.000000 mono-dense-keras-0.0.6rc0/mono_dense_keras.egg-info/top_level.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)      969 2023-05-26 14:19:35.000000 mono-dense-keras-0.0.6rc0/settings.ini
--rw-rw-r--   0 davor     (1000) davor     (1000)       38 2023-05-26 14:23:55.472180 mono-dense-keras-0.0.6rc0/setup.cfg
--rw-rw-r--   0 davor     (1000) davor     (1000)     2761 2023-05-26 14:19:35.000000 mono-dense-keras-0.0.6rc0/setup.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-05-26 14:28:10.871570 mono-dense-keras-0.0.6rc1/
+-rw-r--r--   0 davor     (1000) davor     (1000)    20848 2022-09-02 19:27:53.000000 mono-dense-keras-0.0.6rc1/LICENSE
+-rw-rw-r--   0 davor     (1000) davor     (1000)      111 2022-08-18 19:39:58.000000 mono-dense-keras-0.0.6rc1/MANIFEST.in
+-rw-rw-r--   0 davor     (1000) davor     (1000)     7659 2023-05-26 14:28:10.871570 mono-dense-keras-0.0.6rc1/PKG-INFO
+-rw-rw-r--   0 davor     (1000) davor     (1000)     6546 2023-05-26 14:19:35.000000 mono-dense-keras-0.0.6rc1/README.md
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-05-26 14:28:10.871570 mono-dense-keras-0.0.6rc1/airt/
+-rw-r--r--   0 davor     (1000) davor     (1000)       22 2022-09-03 17:11:42.000000 mono-dense-keras-0.0.6rc1/airt/__init__.py
+-rw-r--r--   0 davor     (1000) davor     (1000)     1275 2022-09-03 17:11:04.000000 mono-dense-keras-0.0.6rc1/airt/_modidx.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-05-26 14:28:10.871570 mono-dense-keras-0.0.6rc1/airt/keras/
+-rw-r--r--   0 davor     (1000) davor     (1000)        0 2022-09-03 17:11:01.000000 mono-dense-keras-0.0.6rc1/airt/keras/__init__.py
+-rw-r--r--   0 davor     (1000) davor     (1000)     3906 2022-09-03 17:11:01.000000 mono-dense-keras-0.0.6rc1/airt/keras/layers.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-05-26 14:28:10.871570 mono-dense-keras-0.0.6rc1/mono_dense_keras/
+-rw-rw-r--   0 davor     (1000) davor     (1000)      472 2023-05-26 14:27:26.000000 mono-dense-keras-0.0.6rc1/mono_dense_keras/__init__.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-05-26 14:28:10.871570 mono-dense-keras-0.0.6rc1/mono_dense_keras/_components/
+-rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-05-26 14:27:26.000000 mono-dense-keras-0.0.6rc1/mono_dense_keras/_components/__init__.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)    10318 2023-05-26 14:27:26.000000 mono-dense-keras-0.0.6rc1/mono_dense_keras/_components/mono_dense_layer.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)     4050 2023-05-26 14:27:26.000000 mono-dense-keras-0.0.6rc1/mono_dense_keras/_modidx.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-05-26 14:28:10.871570 mono-dense-keras-0.0.6rc1/mono_dense_keras.egg-info/
+-rw-r--r--   0 davor     (1000) davor     (1000)     7659 2023-05-26 14:28:10.000000 mono-dense-keras-0.0.6rc1/mono_dense_keras.egg-info/PKG-INFO
+-rw-r--r--   0 davor     (1000) davor     (1000)      556 2023-05-26 14:28:10.000000 mono-dense-keras-0.0.6rc1/mono_dense_keras.egg-info/SOURCES.txt
+-rw-r--r--   0 davor     (1000) davor     (1000)        1 2023-05-26 14:28:10.000000 mono-dense-keras-0.0.6rc1/mono_dense_keras.egg-info/dependency_links.txt
+-rw-r--r--   0 davor     (1000) davor     (1000)       54 2023-05-26 14:28:10.000000 mono-dense-keras-0.0.6rc1/mono_dense_keras.egg-info/entry_points.txt
+-rw-r--r--   0 davor     (1000) davor     (1000)        1 2022-12-06 04:51:35.000000 mono-dense-keras-0.0.6rc1/mono_dense_keras.egg-info/not-zip-safe
+-rw-r--r--   0 davor     (1000) davor     (1000)      219 2023-05-26 14:28:10.000000 mono-dense-keras-0.0.6rc1/mono_dense_keras.egg-info/requires.txt
+-rw-r--r--   0 davor     (1000) davor     (1000)       22 2023-05-26 14:28:10.000000 mono-dense-keras-0.0.6rc1/mono_dense_keras.egg-info/top_level.txt
+-rw-rw-r--   0 davor     (1000) davor     (1000)      969 2023-05-26 14:27:16.000000 mono-dense-keras-0.0.6rc1/settings.ini
+-rw-rw-r--   0 davor     (1000) davor     (1000)       38 2023-05-26 14:28:10.871570 mono-dense-keras-0.0.6rc1/setup.cfg
+-rw-rw-r--   0 davor     (1000) davor     (1000)     3081 2023-05-26 14:25:56.000000 mono-dense-keras-0.0.6rc1/setup.py
```

### Comparing `mono-dense-keras-0.0.6rc0/LICENSE` & `mono-dense-keras-0.0.6rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `mono-dense-keras-0.0.6rc0/PKG-INFO` & `mono-dense-keras-0.0.6rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: mono-dense-keras
-Version: 0.0.6rc0
+Version: 0.0.6rc1
 Summary: Monotonic Dense Layer implemented in Keras
 Home-page: https://github.com/airtai/mono-dense-keras
 Author: AIRT Technologies d.o.o.
 Author-email: info@airt.ai
 License: Creative Commons License
+Project-URL: Bug Tracker, https://github.com/airtai/mono-dense-keras/issues
+Project-URL: CI, https://github.com/airtai/mono-dense-keras/actions
+Project-URL: Documentation, https://mono-dense-keras.airt.ai/
 Keywords: tensorflow monotone monotonic dense layer nbdev nbdev-mkdocs jupyter notebook python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mono-dense-keras-0.0.6rc0/README.md` & `mono-dense-keras-0.0.6rc1/README.md`

 * *Files identical despite different names*

### Comparing `mono-dense-keras-0.0.6rc0/airt/_modidx.py` & `mono-dense-keras-0.0.6rc1/airt/_modidx.py`

 * *Files identical despite different names*

### Comparing `mono-dense-keras-0.0.6rc0/airt/keras/layers.py` & `mono-dense-keras-0.0.6rc1/airt/keras/layers.py`

 * *Files identical despite different names*

### Comparing `mono-dense-keras-0.0.6rc0/mono_dense_keras/_components/mono_dense_layer.py` & `mono-dense-keras-0.0.6rc1/mono_dense_keras/_components/mono_dense_layer.py`

 * *Files identical despite different names*

### Comparing `mono-dense-keras-0.0.6rc0/mono_dense_keras/_modidx.py` & `mono-dense-keras-0.0.6rc1/mono_dense_keras/_modidx.py`

 * *Files identical despite different names*

### Comparing `mono-dense-keras-0.0.6rc0/mono_dense_keras.egg-info/PKG-INFO` & `mono-dense-keras-0.0.6rc1/mono_dense_keras.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: mono-dense-keras
-Version: 0.0.6rc0
+Version: 0.0.6rc1
 Summary: Monotonic Dense Layer implemented in Keras
 Home-page: https://github.com/airtai/mono-dense-keras
 Author: AIRT Technologies d.o.o.
 Author-email: info@airt.ai
 License: Creative Commons License
+Project-URL: Bug Tracker, https://github.com/airtai/mono-dense-keras/issues
+Project-URL: CI, https://github.com/airtai/mono-dense-keras/actions
+Project-URL: Documentation, https://mono-dense-keras.airt.ai/
 Keywords: tensorflow monotone monotonic dense layer nbdev nbdev-mkdocs jupyter notebook python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mono-dense-keras-0.0.6rc0/mono_dense_keras.egg-info/SOURCES.txt` & `mono-dense-keras-0.0.6rc1/mono_dense_keras.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mono-dense-keras-0.0.6rc0/settings.ini` & `mono-dense-keras-0.0.6rc1/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = mono-dense-keras
 lib_name = %(repo)s
-version = 0.0.6rc0
+version = 0.0.6rc1
 min_python = 3.7
 license = cc
 
 ### nbdev ###
 doc_path = _docs
 lib_path = mono_dense_keras
 nbs_path = nbs
```

### Comparing `mono-dense-keras-0.0.6rc0/setup.py` & `mono-dense-keras-0.0.6rc1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -41,23 +41,31 @@
     "matplotlib==3.7.1",
     "seaborn==0.12.2",
     "mypy==1.3.0",
     "bandit==1.7.5",
     "semgrep==1.23.0",
 ]
 
+project_urls = {
+   'Bug Tracker': cfg['git_url'] + '/issues',
+   'CI': cfg['git_url'] + '/actions',
+   'Documentation': 'https://mono-dense-keras.airt.ai/',
+#    'Tutorial': 'https://colab.research.google.com/github/airtai/fastkafka/blob/main/nbs/guides/Guide_00_FastKafka_Demo.ipynb'
+}
+
 setuptools.setup(
     name = cfg['lib_name'],
     license = lic[0],
     classifiers = [
         'Development Status :: ' + statuses[int(cfg['status'])],
         'Intended Audience :: ' + cfg['audience'].title(),
         'Natural Language :: ' + cfg['language'].title(),
     ] + ['Programming Language :: Python :: '+o for o in py_versions[py_versions.index(min_python):]] + (['License :: ' + lic[1] ] if lic[1] else []),
     url = cfg['git_url'],
+    project_urls=project_urls,
     packages = setuptools.find_packages(),
     include_package_data = True,
     install_requires = requirements,
     extras_require={ 'dev': dev_requirements },
     dependency_links = cfg.get('dep_links','').split(),
     python_requires  = '>=' + cfg['min_python'],
     long_description = open('README.md').read(),
```

