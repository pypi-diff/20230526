# Comparing `tmp/elgin-0.1.7.tar.gz` & `tmp/elgin-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elgin-0.1.7.tar", last modified: Fri May 26 12:39:13 2023, max compression
+gzip compressed data, was "elgin-0.1.8.tar", last modified: Fri May 26 12:52:04 2023, max compression
```

## Comparing `elgin-0.1.7.tar` & `elgin-0.1.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 joao-soares  (1000) joao-soares  (1000)        0 2023-05-26 12:39:13.485464 elgin-0.1.7/
--rw-r--r--   0 joao-soares  (1000) joao-soares  (1000)     2341 2023-05-26 12:39:13.485464 elgin-0.1.7/PKG-INFO
--rw-r--r--   0 joao-soares  (1000) joao-soares  (1000)     1625 2023-05-25 14:57:03.000000 elgin-0.1.7/README.md
-drwxr-xr-x   0 joao-soares  (1000) joao-soares  (1000)        0 2023-05-26 12:39:13.475464 elgin-0.1.7/elgin/
--rw-r--r--   0 joao-soares  (1000) joao-soares  (1000)        0 2023-05-24 18:41:57.000000 elgin-0.1.7/elgin/__init__.py
--rw-r--r--   0 joao-soares  (1000) joao-soares  (1000)    11967 2023-05-25 16:12:16.000000 elgin-0.1.7/elgin/monitoramento.py
-drwxr-xr-x   0 joao-soares  (1000) joao-soares  (1000)        0 2023-05-26 12:39:13.485464 elgin-0.1.7/elgin/templates/
--rw-r--r--   0 joao-soares  (1000) joao-soares  (1000)     3978 2023-05-24 18:09:12.000000 elgin-0.1.7/elgin/templates/template_email_log.html
--rw-r--r--   0 joao-soares  (1000) joao-soares  (1000)     4019 2023-05-24 20:41:00.000000 elgin-0.1.7/elgin/templates/template_teams.json
-drwxr-xr-x   0 joao-soares  (1000) joao-soares  (1000)        0 2023-05-26 12:39:13.475464 elgin-0.1.7/elgin.egg-info/
--rw-r--r--   0 joao-soares  (1000) joao-soares  (1000)     2341 2023-05-26 12:39:13.000000 elgin-0.1.7/elgin.egg-info/PKG-INFO
--rw-r--r--   0 joao-soares  (1000) joao-soares  (1000)      279 2023-05-26 12:39:13.000000 elgin-0.1.7/elgin.egg-info/SOURCES.txt
--rw-r--r--   0 joao-soares  (1000) joao-soares  (1000)        1 2023-05-26 12:39:13.000000 elgin-0.1.7/elgin.egg-info/dependency_links.txt
--rw-r--r--   0 joao-soares  (1000) joao-soares  (1000)       32 2023-05-26 12:39:13.000000 elgin-0.1.7/elgin.egg-info/requires.txt
--rw-r--r--   0 joao-soares  (1000) joao-soares  (1000)        6 2023-05-26 12:39:13.000000 elgin-0.1.7/elgin.egg-info/top_level.txt
--rw-r--r--   0 joao-soares  (1000) joao-soares  (1000)       38 2023-05-26 12:39:13.485464 elgin-0.1.7/setup.cfg
--rw-r--r--   0 joao-soares  (1000) joao-soares  (1000)     1045 2023-05-26 12:38:41.000000 elgin-0.1.7/setup.py
+drwxr-xr-x   0 joao-soares  (1000) joao-soares  (1000)        0 2023-05-26 12:52:04.415450 elgin-0.1.8/
+-rw-r--r--   0 joao-soares  (1000) joao-soares  (1000)     2341 2023-05-26 12:52:04.415450 elgin-0.1.8/PKG-INFO
+-rw-r--r--   0 joao-soares  (1000) joao-soares  (1000)     1625 2023-05-25 14:57:03.000000 elgin-0.1.8/README.md
+drwxr-xr-x   0 joao-soares  (1000) joao-soares  (1000)        0 2023-05-26 12:52:04.415450 elgin-0.1.8/elgin/
+-rw-r--r--   0 joao-soares  (1000) joao-soares  (1000)        0 2023-05-24 18:41:57.000000 elgin-0.1.8/elgin/__init__.py
+-rw-r--r--   0 joao-soares  (1000) joao-soares  (1000)    11967 2023-05-25 16:12:16.000000 elgin-0.1.8/elgin/monitoramento.py
+drwxr-xr-x   0 joao-soares  (1000) joao-soares  (1000)        0 2023-05-26 12:52:04.415450 elgin-0.1.8/elgin/templates/
+-rw-r--r--   0 joao-soares  (1000) joao-soares  (1000)     3978 2023-05-24 18:09:12.000000 elgin-0.1.8/elgin/templates/template_email_log.html
+-rw-r--r--   0 joao-soares  (1000) joao-soares  (1000)     4019 2023-05-24 20:41:00.000000 elgin-0.1.8/elgin/templates/template_teams.json
+drwxr-xr-x   0 joao-soares  (1000) joao-soares  (1000)        0 2023-05-26 12:52:04.415450 elgin-0.1.8/elgin.egg-info/
+-rw-r--r--   0 joao-soares  (1000) joao-soares  (1000)     2341 2023-05-26 12:52:04.000000 elgin-0.1.8/elgin.egg-info/PKG-INFO
+-rw-r--r--   0 joao-soares  (1000) joao-soares  (1000)      279 2023-05-26 12:52:04.000000 elgin-0.1.8/elgin.egg-info/SOURCES.txt
+-rw-r--r--   0 joao-soares  (1000) joao-soares  (1000)        1 2023-05-26 12:52:04.000000 elgin-0.1.8/elgin.egg-info/dependency_links.txt
+-rw-r--r--   0 joao-soares  (1000) joao-soares  (1000)        9 2023-05-26 12:52:04.000000 elgin-0.1.8/elgin.egg-info/requires.txt
+-rw-r--r--   0 joao-soares  (1000) joao-soares  (1000)        6 2023-05-26 12:52:04.000000 elgin-0.1.8/elgin.egg-info/top_level.txt
+-rw-r--r--   0 joao-soares  (1000) joao-soares  (1000)       38 2023-05-26 12:52:04.415450 elgin-0.1.8/setup.cfg
+-rw-r--r--   0 joao-soares  (1000) joao-soares  (1000)     1020 2023-05-26 12:51:55.000000 elgin-0.1.8/setup.py
```

### Comparing `elgin-0.1.7/PKG-INFO` & `elgin-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elgin
-Version: 0.1.7
+Version: 0.1.8
 Summary: Biblioteca responsavel por gerar o monitoramento dos processos da empresa elgin.
 Home-page: UNKNOWN
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `elgin-0.1.7/README.md` & `elgin-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `elgin-0.1.7/elgin/monitoramento.py` & `elgin-0.1.8/elgin/monitoramento.py`

 * *Files identical despite different names*

### Comparing `elgin-0.1.7/elgin/templates/template_email_log.html` & `elgin-0.1.8/elgin/templates/template_email_log.html`

 * *Files identical despite different names*

### Comparing `elgin-0.1.7/elgin/templates/template_teams.json` & `elgin-0.1.8/elgin/templates/template_teams.json`

 * *Files identical despite different names*

### Comparing `elgin-0.1.7/elgin.egg-info/PKG-INFO` & `elgin-0.1.8/elgin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elgin
-Version: 0.1.7
+Version: 0.1.8
 Summary: Biblioteca responsavel por gerar o monitoramento dos processos da empresa elgin.
 Home-page: UNKNOWN
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `elgin-0.1.7/setup.py` & `elgin-0.1.8/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('./README.md') as f:
     long_desc = f.read()
 
 setup(
      name='elgin'
-    ,version='0.1.7'
+    ,version='0.1.8'
     ,description='Biblioteca responsavel por gerar o monitoramento dos processos da empresa elgin.'
     ,long_description=long_desc
     ,long_description_content_type='text/markdown'
     ,license="MIT"
     ,classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
@@ -22,9 +22,9 @@
         "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent"
     ]
     ,packages=['elgin']
     ,package_dir={'elgin': 'elgin'}
     ,package_data={'elgin': ['templates/*']}
     ,include_package_data=True
-    ,install_requires=["mysql-connector-python","requests"]
+    ,install_requires=["requests"]
 )
```

