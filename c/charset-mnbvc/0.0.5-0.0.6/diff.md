# Comparing `tmp/charset_mnbvc-0.0.5.tar.gz` & `tmp/charset_mnbvc-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "charset_mnbvc-0.0.5.tar", last modified: Wed May 10 09:57:03 2023, max compression
+gzip compressed data, was "charset_mnbvc-0.0.6.tar", last modified: Fri May 26 06:35:44 2023, max compression
```

## Comparing `charset_mnbvc-0.0.5.tar` & `charset_mnbvc-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 alan       (501) staff       (20)        0 2023-05-10 09:57:03.764220 charset_mnbvc-0.0.5/
--rw-r--r--   0 alan       (501) staff       (20)     1064 2023-02-09 08:52:50.000000 charset_mnbvc-0.0.5/LICENSE
--rw-r--r--   0 alan       (501) staff       (20)     9711 2023-05-10 09:57:03.764020 charset_mnbvc-0.0.5/PKG-INFO
--rw-r--r--   0 alan       (501) staff       (20)     9108 2023-03-27 15:02:20.000000 charset_mnbvc-0.0.5/README.md
-drwxr-xr-x   0 alan       (501) staff       (20)        0 2023-05-10 09:57:03.763342 charset_mnbvc-0.0.5/charset_mnbvc/
--rw-r--r--   0 alan       (501) staff       (20)        0 2023-02-09 02:34:27.000000 charset_mnbvc-0.0.5/charset_mnbvc/__init__.py
--rw-r--r--   0 alan       (501) staff       (20)     3109 2023-04-06 08:14:07.000000 charset_mnbvc-0.0.5/charset_mnbvc/api.py
--rw-r--r--   0 alan       (501) staff       (20)     2902 2023-03-27 14:46:45.000000 charset_mnbvc-0.0.5/charset_mnbvc/constant.py
--rw-r--r--   0 alan       (501) staff       (20)       70 2023-05-10 09:56:21.000000 charset_mnbvc-0.0.5/charset_mnbvc/version.py
-drwxr-xr-x   0 alan       (501) staff       (20)        0 2023-05-10 09:57:03.763846 charset_mnbvc-0.0.5/charset_mnbvc.egg-info/
--rw-r--r--   0 alan       (501) staff       (20)     9711 2023-05-10 09:57:03.000000 charset_mnbvc-0.0.5/charset_mnbvc.egg-info/PKG-INFO
--rw-r--r--   0 alan       (501) staff       (20)      272 2023-05-10 09:57:03.000000 charset_mnbvc-0.0.5/charset_mnbvc.egg-info/SOURCES.txt
--rw-r--r--   0 alan       (501) staff       (20)        1 2023-05-10 09:57:03.000000 charset_mnbvc-0.0.5/charset_mnbvc.egg-info/dependency_links.txt
--rw-r--r--   0 alan       (501) staff       (20)       14 2023-05-10 09:57:03.000000 charset_mnbvc-0.0.5/charset_mnbvc.egg-info/top_level.txt
--rw-r--r--   0 alan       (501) staff       (20)       38 2023-05-10 09:57:03.764261 charset_mnbvc-0.0.5/setup.cfg
--rw-r--r--   0 alan       (501) staff       (20)      912 2023-05-10 09:56:11.000000 charset_mnbvc-0.0.5/setup.py
+drwxr-xr-x   0 alan       (501) staff       (20)        0 2023-05-26 06:35:44.724753 charset_mnbvc-0.0.6/
+-rw-r--r--   0 alan       (501) staff       (20)     1064 2023-02-09 08:52:50.000000 charset_mnbvc-0.0.6/LICENSE
+-rw-r--r--   0 alan       (501) staff       (20)     9748 2023-05-26 06:35:44.724596 charset_mnbvc-0.0.6/PKG-INFO
+-rw-r--r--   0 alan       (501) staff       (20)     9108 2023-03-27 15:02:20.000000 charset_mnbvc-0.0.6/README.md
+drwxr-xr-x   0 alan       (501) staff       (20)        0 2023-05-26 06:35:44.724008 charset_mnbvc-0.0.6/charset_mnbvc/
+-rw-r--r--   0 alan       (501) staff       (20)        0 2023-02-09 02:34:27.000000 charset_mnbvc-0.0.6/charset_mnbvc/__init__.py
+-rw-r--r--   0 alan       (501) staff       (20)     3109 2023-04-06 08:14:07.000000 charset_mnbvc-0.0.6/charset_mnbvc/api.py
+-rw-r--r--   0 alan       (501) staff       (20)      453 2023-05-26 03:45:39.000000 charset_mnbvc-0.0.6/charset_mnbvc/common_utils.py
+-rw-r--r--   0 alan       (501) staff       (20)     2902 2023-03-27 14:46:45.000000 charset_mnbvc-0.0.6/charset_mnbvc/constant.py
+-rw-r--r--   0 alan       (501) staff       (20)     1144 2023-05-26 06:34:46.000000 charset_mnbvc-0.0.6/charset_mnbvc/verify.py
+-rw-r--r--   0 alan       (501) staff       (20)       70 2023-05-26 03:30:47.000000 charset_mnbvc-0.0.6/charset_mnbvc/version.py
+drwxr-xr-x   0 alan       (501) staff       (20)        0 2023-05-26 06:35:44.724430 charset_mnbvc-0.0.6/charset_mnbvc.egg-info/
+-rw-r--r--   0 alan       (501) staff       (20)     9748 2023-05-26 06:35:44.000000 charset_mnbvc-0.0.6/charset_mnbvc.egg-info/PKG-INFO
+-rw-r--r--   0 alan       (501) staff       (20)      326 2023-05-26 06:35:44.000000 charset_mnbvc-0.0.6/charset_mnbvc.egg-info/SOURCES.txt
+-rw-r--r--   0 alan       (501) staff       (20)        1 2023-05-26 06:35:44.000000 charset_mnbvc-0.0.6/charset_mnbvc.egg-info/dependency_links.txt
+-rw-r--r--   0 alan       (501) staff       (20)       14 2023-05-26 06:35:44.000000 charset_mnbvc-0.0.6/charset_mnbvc.egg-info/top_level.txt
+-rw-r--r--   0 alan       (501) staff       (20)       38 2023-05-26 06:35:44.724795 charset_mnbvc-0.0.6/setup.cfg
+-rw-r--r--   0 alan       (501) staff       (20)      962 2023-05-26 03:31:25.000000 charset_mnbvc-0.0.6/setup.py
```

### Comparing `charset_mnbvc-0.0.5/LICENSE` & `charset_mnbvc-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `charset_mnbvc-0.0.5/PKG-INFO` & `charset_mnbvc-0.0.6/charset_mnbvc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
-Name: charset_mnbvc
-Version: 0.0.5
+Name: charset-mnbvc
+Version: 0.0.6
 Summary: 本项目旨在对大量文本文件进行快速编码检测以辅助mnbvc语料集项目的数据清洗工作
 Home-page: https://github.com/alanshi/charset_mnbvc
 Author: Alan Shi
 Author-email: alan.shi86@gmail.com
+License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/alanshi/charset_mnbvc/issues
 Project-URL: Source, https://github.com/alanshi/charset_mnbvc/
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ### 项目描述
@@ -184,7 +186,9 @@
 
 现在解决这个问题的最简单的思路是换一种语言实现编码转换或者在Python中引入Java的库对MS936编码进行正确处理。
 
 
 
 
 
+
+
```

### Comparing `charset_mnbvc-0.0.5/README.md` & `charset_mnbvc-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `charset_mnbvc-0.0.5/charset_mnbvc/api.py` & `charset_mnbvc-0.0.6/charset_mnbvc/api.py`

 * *Files identical despite different names*

### Comparing `charset_mnbvc-0.0.5/charset_mnbvc/constant.py` & `charset_mnbvc-0.0.6/charset_mnbvc/constant.py`

 * *Files identical despite different names*

### Comparing `charset_mnbvc-0.0.5/charset_mnbvc.egg-info/PKG-INFO` & `charset_mnbvc-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
-Name: charset-mnbvc
-Version: 0.0.5
+Name: charset_mnbvc
+Version: 0.0.6
 Summary: 本项目旨在对大量文本文件进行快速编码检测以辅助mnbvc语料集项目的数据清洗工作
 Home-page: https://github.com/alanshi/charset_mnbvc
 Author: Alan Shi
 Author-email: alan.shi86@gmail.com
+License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/alanshi/charset_mnbvc/issues
 Project-URL: Source, https://github.com/alanshi/charset_mnbvc/
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ### 项目描述
@@ -184,7 +186,9 @@
 
 现在解决这个问题的最简单的思路是换一种语言实现编码转换或者在Python中引入Java的库对MS936编码进行正确处理。
 
 
 
 
 
+
+
```

### Comparing `charset_mnbvc-0.0.5/setup.py` & `charset_mnbvc-0.0.6/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from setuptools import setup
 import pathlib
 
+from charset_mnbvc.version import __version__
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 
 setup(
     name="charset_mnbvc",
-    version="0.0.5",
+    version=__version__,
     description="本项目旨在对大量文本文件进行快速编码检测以辅助mnbvc语料集项目的数据清洗工作",
     url="https://github.com/alanshi/charset_mnbvc",
     author="Alan Shi",
     author_email="alan.shi86@gmail.com",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
```

