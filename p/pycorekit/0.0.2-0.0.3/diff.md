# Comparing `tmp/pycorekit-0.0.2.tar.gz` & `tmp/pycorekit-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycorekit-0.0.2.tar", last modified: Fri May 26 01:45:49 2023, max compression
+gzip compressed data, was "pycorekit-0.0.3.tar", last modified: Fri May 26 01:55:08 2023, max compression
```

## Comparing `pycorekit-0.0.2.tar` & `pycorekit-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 01:45:49.218555 pycorekit-0.0.2/
--rw-rw-rw-   0        0        0     1077 2023-05-25 07:40:26.000000 pycorekit-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0      592 2023-05-26 01:45:49.218555 pycorekit-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      121 2023-05-26 01:42:08.000000 pycorekit-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 01:45:49.217555 pycorekit-0.0.2/pycorekit.egg-info/
--rw-rw-rw-   0        0        0      592 2023-05-26 01:45:49.000000 pycorekit-0.0.2/pycorekit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      204 2023-05-26 01:45:49.000000 pycorekit-0.0.2/pycorekit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 01:45:49.000000 pycorekit-0.0.2/pycorekit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-26 01:45:49.000000 pycorekit-0.0.2/pycorekit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 01:45:49.000000 pycorekit-0.0.2/pycorekit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-26 01:45:49.219555 pycorekit-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1105 2023-05-26 01:45:38.000000 pycorekit-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 01:55:08.066553 pycorekit-0.0.3/
+-rw-rw-rw-   0        0        0     1077 2023-05-25 07:40:26.000000 pycorekit-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      592 2023-05-26 01:55:08.067549 pycorekit-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      121 2023-05-26 01:42:08.000000 pycorekit-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 01:55:08.065552 pycorekit-0.0.3/pycorekit.egg-info/
+-rw-rw-rw-   0        0        0      592 2023-05-26 01:55:07.000000 pycorekit-0.0.3/pycorekit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      204 2023-05-26 01:55:07.000000 pycorekit-0.0.3/pycorekit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 01:55:07.000000 pycorekit-0.0.3/pycorekit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-26 01:55:07.000000 pycorekit-0.0.3/pycorekit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 01:55:07.000000 pycorekit-0.0.3/pycorekit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-26 01:55:08.068548 pycorekit-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1105 2023-05-26 01:55:05.000000 pycorekit-0.0.3/setup.py
```

### Comparing `pycorekit-0.0.2/LICENSE.txt` & `pycorekit-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pycorekit-0.0.2/PKG-INFO` & `pycorekit-0.0.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycorekit
-Version: 0.0.2
+Version: 0.0.3
 Summary: An underlying tool library that can be used by any script
 Home-page: https://github.com/MeDeity/core-kit
 Author: MeDeity
 Author-email: langrenbule@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pycorekit-0.0.2/pycorekit.egg-info/PKG-INFO` & `pycorekit-0.0.3/pycorekit.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycorekit
-Version: 0.0.2
+Version: 0.0.3
 Summary: An underlying tool library that can be used by any script
 Home-page: https://github.com/MeDeity/core-kit
 Author: MeDeity
 Author-email: langrenbule@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pycorekit-0.0.2/setup.py` & `pycorekit-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools #导入setuptools打包工具
  
 with open("README.md", "r", encoding="utf-8") as readme:
     description = readme.read()
  
 setuptools.setup(
     name="pycorekit", # 用自己的名替换其中的YOUR_USERNAME_
-    version="0.0.2",    #包版本号，便于维护版本
+    version="0.0.3",    #包版本号，便于维护版本
     author="MeDeity",    #作者，可以写自己的姓名
     author_email="langrenbule@gmail.com",    #作者联系方式，可写自己的邮箱地址
     description="An underlying tool library that can be used by any script",#包的简述
     long_description=description,    #包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="https://github.com/MeDeity/core-kit",    #自己项目地址，比如github的项目地址
     packages=setuptools.find_packages(),
```

