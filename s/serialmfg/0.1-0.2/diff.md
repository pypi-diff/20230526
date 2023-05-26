# Comparing `tmp/serialmfg-0.1.tar.gz` & `tmp/serialmfg-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serialmfg-0.1.tar", last modified: Fri May 26 06:13:53 2023, max compression
+gzip compressed data, was "serialmfg-0.2.tar", last modified: Fri May 26 06:39:56 2023, max compression
```

## Comparing `serialmfg-0.1.tar` & `serialmfg-0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 devon      (501) staff       (20)        0 2023-05-26 06:13:53.191756 serialmfg-0.1/
--rw-rw-r--   0 devon      (501) staff       (20)     1081 2023-05-26 06:01:43.000000 serialmfg-0.1/LICENSE
--rw-r--r--   0 devon      (501) staff       (20)     6173 2023-05-26 06:13:53.191604 serialmfg-0.1/PKG-INFO
--rw-rw-r--   0 devon      (501) staff       (20)     5515 2023-05-26 06:01:43.000000 serialmfg-0.1/README.md
-drwxr-xr-x   0 devon      (501) staff       (20)        0 2023-05-26 06:13:53.190691 serialmfg-0.1/serialmfg/
--rw-rw-r--   0 devon      (501) staff       (20)       90 2023-05-26 06:01:43.000000 serialmfg-0.1/serialmfg/__init__.py
--rw-rw-r--   0 devon      (501) staff       (20)      490 2023-05-26 06:01:43.000000 serialmfg-0.1/serialmfg/identifier.py
--rw-rw-r--   0 devon      (501) staff       (20)     5170 2023-05-26 06:01:43.000000 serialmfg-0.1/serialmfg/process.py
--rw-rw-r--   0 devon      (501) staff       (20)     2471 2023-05-26 06:01:43.000000 serialmfg-0.1/serialmfg/serial.py
-drwxr-xr-x   0 devon      (501) staff       (20)        0 2023-05-26 06:13:53.191411 serialmfg-0.1/serialmfg.egg-info/
--rw-r--r--   0 devon      (501) staff       (20)     6173 2023-05-26 06:13:53.000000 serialmfg-0.1/serialmfg.egg-info/PKG-INFO
--rw-r--r--   0 devon      (501) staff       (20)      277 2023-05-26 06:13:53.000000 serialmfg-0.1/serialmfg.egg-info/SOURCES.txt
--rw-r--r--   0 devon      (501) staff       (20)        1 2023-05-26 06:13:53.000000 serialmfg-0.1/serialmfg.egg-info/dependency_links.txt
--rw-r--r--   0 devon      (501) staff       (20)        9 2023-05-26 06:13:53.000000 serialmfg-0.1/serialmfg.egg-info/requires.txt
--rw-r--r--   0 devon      (501) staff       (20)       10 2023-05-26 06:13:53.000000 serialmfg-0.1/serialmfg.egg-info/top_level.txt
--rw-r--r--   0 devon      (501) staff       (20)       38 2023-05-26 06:13:53.191805 serialmfg-0.1/setup.cfg
--rw-rw-r--   0 devon      (501) staff       (20)      881 2023-05-26 06:01:43.000000 serialmfg-0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:39:56.543963 serialmfg-0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-26 06:39:40.000000 serialmfg-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-05-26 06:39:56.543963 serialmfg-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-05-26 06:39:40.000000 serialmfg-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:39:56.539963 serialmfg-0.2/serialmfg/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-26 06:39:40.000000 serialmfg-0.2/serialmfg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-26 06:39:40.000000 serialmfg-0.2/serialmfg/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-05-26 06:39:40.000000 serialmfg-0.2/serialmfg/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-05-26 06:39:40.000000 serialmfg-0.2/serialmfg/serial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:39:56.543963 serialmfg-0.2/serialmfg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-05-26 06:39:56.000000 serialmfg-0.2/serialmfg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-26 06:39:56.000000 serialmfg-0.2/serialmfg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 06:39:56.000000 serialmfg-0.2/serialmfg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-26 06:39:56.000000 serialmfg-0.2/serialmfg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-26 06:39:56.000000 serialmfg-0.2/serialmfg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 06:39:56.543963 serialmfg-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-26 06:39:40.000000 serialmfg-0.2/setup.py
```

### Comparing `serialmfg-0.1/LICENSE` & `serialmfg-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `serialmfg-0.1/PKG-INFO` & `serialmfg-0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serialmfg
-Version: 0.1
+Version: 0.2
 Summary: This module provides a simple Python interface to interact with the Serial API. It allows you to easily perform common operations such as uploading process data, initializing identifiers, and checking the server connection.
 Home-page: https://github.com/serialmfg/serial-py
 Author: Devon Copeland
 Author-email: founders@serial.io
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -15,33 +15,25 @@
 
 # Overview
 
 This module provides a simple Python interface to interact with the Serial API. It allows you to easily perform common operations such as uploading process data, initializing identifiers, and checking the server connection. The latest version of the library can be downloaded [here](https://github.com/serialmfg/serial-py)
 
 # Installation
 
-1. Clone the repository from GitHub:
-   ```
-   git clone https://https://github.com/serialmfg/serial-py.git
-   ```
-   or 
-   ```
-   pip install serialmfg
-   ```
-
-2. Navigate to the project directory:
-   ```
-   cd serial-py
-   ```
-3. Install the required dependencies using pip:
-   ```
-   pip install -r requirements.txt
-   ```
+Clone the repository from GitHub or install via pip:
+```
+git clone https://https://github.com/serialmfg/serial-py.git
+```
+or 
+```
+pip install serialmfg
+```
 
 # Dependencies
+
 This project requires the following dependencies:
 - requests
 - json
 - os
 
 # Usage
```

### Comparing `serialmfg-0.1/README.md` & `serialmfg-0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,24 @@
 # Overview
 
 This module provides a simple Python interface to interact with the Serial API. It allows you to easily perform common operations such as uploading process data, initializing identifiers, and checking the server connection. The latest version of the library can be downloaded [here](https://github.com/serialmfg/serial-py)
 
 # Installation
 
-1. Clone the repository from GitHub:
-   ```
-   git clone https://https://github.com/serialmfg/serial-py.git
-   ```
-   or 
-   ```
-   pip install serialmfg
-   ```
-
-2. Navigate to the project directory:
-   ```
-   cd serial-py
-   ```
-3. Install the required dependencies using pip:
-   ```
-   pip install -r requirements.txt
-   ```
+Clone the repository from GitHub or install via pip:
+```
+git clone https://https://github.com/serialmfg/serial-py.git
+```
+or 
+```
+pip install serialmfg
+```
 
 # Dependencies
+
 This project requires the following dependencies:
 - requests
 - json
 - os
 
 # Usage
```

### Comparing `serialmfg-0.1/serialmfg/process.py` & `serialmfg-0.2/serialmfg/process.py`

 * *Files identical despite different names*

### Comparing `serialmfg-0.1/serialmfg/serial.py` & `serialmfg-0.2/serialmfg/serial.py`

 * *Files identical despite different names*

### Comparing `serialmfg-0.1/serialmfg.egg-info/PKG-INFO` & `serialmfg-0.2/serialmfg.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serialmfg
-Version: 0.1
+Version: 0.2
 Summary: This module provides a simple Python interface to interact with the Serial API. It allows you to easily perform common operations such as uploading process data, initializing identifiers, and checking the server connection.
 Home-page: https://github.com/serialmfg/serial-py
 Author: Devon Copeland
 Author-email: founders@serial.io
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -15,33 +15,25 @@
 
 # Overview
 
 This module provides a simple Python interface to interact with the Serial API. It allows you to easily perform common operations such as uploading process data, initializing identifiers, and checking the server connection. The latest version of the library can be downloaded [here](https://github.com/serialmfg/serial-py)
 
 # Installation
 
-1. Clone the repository from GitHub:
-   ```
-   git clone https://https://github.com/serialmfg/serial-py.git
-   ```
-   or 
-   ```
-   pip install serialmfg
-   ```
-
-2. Navigate to the project directory:
-   ```
-   cd serial-py
-   ```
-3. Install the required dependencies using pip:
-   ```
-   pip install -r requirements.txt
-   ```
+Clone the repository from GitHub or install via pip:
+```
+git clone https://https://github.com/serialmfg/serial-py.git
+```
+or 
+```
+pip install serialmfg
+```
 
 # Dependencies
+
 This project requires the following dependencies:
 - requests
 - json
 - os
 
 # Usage
```

### Comparing `serialmfg-0.1/setup.py` & `serialmfg-0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="serialmfg",
-    version="0.1",
+    version="0.2",
     packages=find_packages(),
     description="This module provides a simple Python interface to interact with the Serial API. It allows you to easily perform common operations such as uploading process data, initializing identifiers, and checking the server connection.",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/serialmfg/serial-py",
     author="Devon Copeland",
     author_email="founders@serial.io",
```

