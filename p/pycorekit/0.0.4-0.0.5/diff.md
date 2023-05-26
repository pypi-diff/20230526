# Comparing `tmp/pycorekit-0.0.4.tar.gz` & `tmp/pycorekit-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycorekit-0.0.4.tar", last modified: Fri May 26 01:58:24 2023, max compression
+gzip compressed data, was "pycorekit-0.0.5.tar", last modified: Fri May 26 02:13:17 2023, max compression
```

## Comparing `pycorekit-0.0.4.tar` & `pycorekit-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 01:58:24.760314 pycorekit-0.0.4/
--rw-rw-rw-   0        0        0     1077 2023-05-25 07:40:26.000000 pycorekit-0.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0      592 2023-05-26 01:58:24.760314 pycorekit-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      121 2023-05-26 01:42:08.000000 pycorekit-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 01:58:24.751316 pycorekit-0.0.4/pycorekit/
--rw-rw-rw-   0        0        0     8029 2023-05-26 01:25:40.000000 pycorekit-0.0.4/pycorekit/ShellKit.py
--rw-rw-rw-   0        0        0        0 2023-05-26 01:57:45.000000 pycorekit-0.0.4/pycorekit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 01:58:24.759313 pycorekit-0.0.4/pycorekit.egg-info/
--rw-rw-rw-   0        0        0      592 2023-05-26 01:58:24.000000 pycorekit-0.0.4/pycorekit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2023-05-26 01:58:24.000000 pycorekit-0.0.4/pycorekit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 01:58:24.000000 pycorekit-0.0.4/pycorekit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-26 01:58:24.000000 pycorekit-0.0.4/pycorekit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-26 01:58:24.000000 pycorekit-0.0.4/pycorekit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-26 01:58:24.761313 pycorekit-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1105 2023-05-26 01:57:54.000000 pycorekit-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 02:13:17.020165 pycorekit-0.0.5/
+-rw-rw-rw-   0        0        0     1077 2023-05-25 07:40:26.000000 pycorekit-0.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      592 2023-05-26 02:13:17.020165 pycorekit-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      121 2023-05-26 01:42:08.000000 pycorekit-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 02:13:17.006170 pycorekit-0.0.5/pycorekit/
+-rw-rw-rw-   0        0        0     8029 2023-05-26 01:25:40.000000 pycorekit-0.0.5/pycorekit/ShellKit.py
+-rw-rw-rw-   0        0        0        0 2023-05-26 01:57:45.000000 pycorekit-0.0.5/pycorekit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 02:13:17.019163 pycorekit-0.0.5/pycorekit.egg-info/
+-rw-rw-rw-   0        0        0      592 2023-05-26 02:13:16.000000 pycorekit-0.0.5/pycorekit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2023-05-26 02:13:16.000000 pycorekit-0.0.5/pycorekit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 02:13:16.000000 pycorekit-0.0.5/pycorekit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-26 02:13:16.000000 pycorekit-0.0.5/pycorekit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-26 02:13:16.000000 pycorekit-0.0.5/pycorekit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-26 02:13:17.021161 pycorekit-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1105 2023-05-26 02:13:01.000000 pycorekit-0.0.5/setup.py
```

### Comparing `pycorekit-0.0.4/LICENSE.txt` & `pycorekit-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pycorekit-0.0.4/PKG-INFO` & `pycorekit-0.0.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycorekit
-Version: 0.0.4
+Version: 0.0.5
 Summary: An underlying tool library that can be used by any script
 Home-page: https://github.com/MeDeity/core-kit
 Author: MeDeity
 Author-email: langrenbule@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pycorekit-0.0.4/pycorekit/ShellKit.py` & `pycorekit-0.0.5/pycorekit/ShellKit.py`

 * *Files identical despite different names*

### Comparing `pycorekit-0.0.4/pycorekit.egg-info/PKG-INFO` & `pycorekit-0.0.5/pycorekit.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycorekit
-Version: 0.0.4
+Version: 0.0.5
 Summary: An underlying tool library that can be used by any script
 Home-page: https://github.com/MeDeity/core-kit
 Author: MeDeity
 Author-email: langrenbule@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pycorekit-0.0.4/setup.py` & `pycorekit-0.0.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools #导入setuptools打包工具
  
 with open("README.md", "r", encoding="utf-8") as readme:
     description = readme.read()
  
 setuptools.setup(
     name="pycorekit", # 用自己的名替换其中的YOUR_USERNAME_
-    version="0.0.4",    #包版本号，便于维护版本
+    version="0.0.5",    #包版本号，便于维护版本
     author="MeDeity",    #作者，可以写自己的姓名
     author_email="langrenbule@gmail.com",    #作者联系方式，可写自己的邮箱地址
     description="An underlying tool library that can be used by any script",#包的简述
     long_description=description,    #包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="https://github.com/MeDeity/core-kit",    #自己项目地址，比如github的项目地址
     packages=setuptools.find_packages(),
```

