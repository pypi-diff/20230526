# Comparing `tmp/chatgptonic-1.1.0.tar.gz` & `tmp/chatgptonic-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgptonic-1.1.0.tar", last modified: Tue Mar 14 17:52:17 2023, max compression
+gzip compressed data, was "chatgptonic-1.1.1.tar", last modified: Fri May 26 15:28:18 2023, max compression
```

## Comparing `chatgptonic-1.1.0.tar` & `chatgptonic-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 howardmederiros   (501) staff       (20)        0 2023-03-14 17:52:17.164074 chatgptonic-1.1.0/
--rw-r--r--   0 howardmederiros   (501) staff       (20)      537 2023-03-14 17:52:17.163941 chatgptonic-1.1.0/PKG-INFO
--rw-r--r--   0 howardmederiros   (501) staff       (20)      301 2023-03-13 16:03:22.000000 chatgptonic-1.1.0/README.md
-drwxr-xr-x   0 howardmederiros   (501) staff       (20)        0 2023-03-14 17:52:17.162625 chatgptonic-1.1.0/chatgptonic/
--rw-r--r--   0 howardmederiros   (501) staff       (20)       73 2023-03-13 16:04:44.000000 chatgptonic-1.1.0/chatgptonic/__init__.py
--rw-r--r--   0 howardmederiros   (501) staff       (20)     2350 2023-03-14 17:44:16.000000 chatgptonic-1.1.0/chatgptonic/integration.py
-drwxr-xr-x   0 howardmederiros   (501) staff       (20)        0 2023-03-14 17:52:17.163756 chatgptonic-1.1.0/chatgptonic.egg-info/
--rw-r--r--   0 howardmederiros   (501) staff       (20)      537 2023-03-14 17:52:17.000000 chatgptonic-1.1.0/chatgptonic.egg-info/PKG-INFO
--rw-r--r--   0 howardmederiros   (501) staff       (20)      277 2023-03-14 17:52:17.000000 chatgptonic-1.1.0/chatgptonic.egg-info/SOURCES.txt
--rw-r--r--   0 howardmederiros   (501) staff       (20)        1 2023-03-14 17:52:17.000000 chatgptonic-1.1.0/chatgptonic.egg-info/dependency_links.txt
--rw-r--r--   0 howardmederiros   (501) staff       (20)        1 2023-03-13 16:03:25.000000 chatgptonic-1.1.0/chatgptonic.egg-info/not-zip-safe
--rw-r--r--   0 howardmederiros   (501) staff       (20)       89 2023-03-14 17:52:17.000000 chatgptonic-1.1.0/chatgptonic.egg-info/requires.txt
--rw-r--r--   0 howardmederiros   (501) staff       (20)       12 2023-03-14 17:52:17.000000 chatgptonic-1.1.0/chatgptonic.egg-info/top_level.txt
--rw-r--r--   0 howardmederiros   (501) staff       (20)       38 2023-03-14 17:52:17.164120 chatgptonic-1.1.0/setup.cfg
--rw-r--r--   0 howardmederiros   (501) staff       (20)      986 2023-03-14 17:52:15.000000 chatgptonic-1.1.0/setup.py
+drwxr-xr-x   0 howardmederiros   (501) staff       (20)        0 2023-05-26 15:28:18.179377 chatgptonic-1.1.1/
+-rw-r--r--   0 howardmederiros   (501) staff       (20)      537 2023-05-26 15:28:18.179260 chatgptonic-1.1.1/PKG-INFO
+-rw-r--r--   0 howardmederiros   (501) staff       (20)      301 2023-03-13 16:03:22.000000 chatgptonic-1.1.1/README.md
+drwxr-xr-x   0 howardmederiros   (501) staff       (20)        0 2023-05-26 15:28:18.178160 chatgptonic-1.1.1/chatgptonic/
+-rw-r--r--   0 howardmederiros   (501) staff       (20)       73 2023-03-14 20:08:55.000000 chatgptonic-1.1.1/chatgptonic/__init__.py
+-rw-r--r--   0 howardmederiros   (501) staff       (20)     2350 2023-03-14 20:08:55.000000 chatgptonic-1.1.1/chatgptonic/integration.py
+drwxr-xr-x   0 howardmederiros   (501) staff       (20)        0 2023-05-26 15:28:18.179089 chatgptonic-1.1.1/chatgptonic.egg-info/
+-rw-r--r--   0 howardmederiros   (501) staff       (20)      537 2023-05-26 15:28:18.000000 chatgptonic-1.1.1/chatgptonic.egg-info/PKG-INFO
+-rw-r--r--   0 howardmederiros   (501) staff       (20)      277 2023-05-26 15:28:18.000000 chatgptonic-1.1.1/chatgptonic.egg-info/SOURCES.txt
+-rw-r--r--   0 howardmederiros   (501) staff       (20)        1 2023-05-26 15:28:18.000000 chatgptonic-1.1.1/chatgptonic.egg-info/dependency_links.txt
+-rw-r--r--   0 howardmederiros   (501) staff       (20)        1 2023-03-13 16:03:25.000000 chatgptonic-1.1.1/chatgptonic.egg-info/not-zip-safe
+-rw-r--r--   0 howardmederiros   (501) staff       (20)       89 2023-05-26 15:28:18.000000 chatgptonic-1.1.1/chatgptonic.egg-info/requires.txt
+-rw-r--r--   0 howardmederiros   (501) staff       (20)       12 2023-05-26 15:28:18.000000 chatgptonic-1.1.1/chatgptonic.egg-info/top_level.txt
+-rw-r--r--   0 howardmederiros   (501) staff       (20)       38 2023-05-26 15:28:18.179420 chatgptonic-1.1.1/setup.cfg
+-rw-r--r--   0 howardmederiros   (501) staff       (20)      986 2023-05-26 15:28:00.000000 chatgptonic-1.1.1/setup.py
```

### Comparing `chatgptonic-1.1.0/PKG-INFO` & `chatgptonic-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgptonic
-Version: 1.1.0
+Version: 1.1.1
 Summary: A package to facilitate integration with chatgpt
 Home-page: https://github.com/how-dev/chatgpython
 Author: Howard Medeiros (howard.medeiros@gmail.com)
 License: UNKNOWN
 Keywords: chatgptonic
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `chatgptonic-1.1.0/chatgptonic/integration.py` & `chatgptonic-1.1.1/chatgptonic/integration.py`

 * *Files identical despite different names*

### Comparing `chatgptonic-1.1.0/chatgptonic.egg-info/PKG-INFO` & `chatgptonic-1.1.1/chatgptonic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgptonic
-Version: 1.1.0
+Version: 1.1.1
 Summary: A package to facilitate integration with chatgpt
 Home-page: https://github.com/how-dev/chatgpython
 Author: Howard Medeiros (howard.medeiros@gmail.com)
 License: UNKNOWN
 Keywords: chatgptonic
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `chatgptonic-1.1.0/setup.py` & `chatgptonic-1.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,20 +14,20 @@
         'Programming Language :: Python :: 3.8',
     ],
     description="A package to facilitate integration with chatgpt",
     install_requires=[
         "certifi==2022.12.7",
         "charset-normalizer==3.1.0",
         "idna==3.4",
-        "requests==2.28.2",
+        "requests==2.31.0",
         "urllib3==1.26.15",
     ],
     include_package_data=True,
     keywords='chatgptonic',
     name='chatgptonic',
     packages=find_packages(include=['chatgptonic',
                                     'chatgptonic.*']),
     test_suite='tests',
     url='https://github.com/how-dev/chatgpython',
-    version='1.1.0',
+    version='1.1.1',
     zip_safe=False,
 )
```

