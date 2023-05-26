# Comparing `tmp/rppt-1.1.1.tar.gz` & `tmp/rppt-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rppt-1.1.1.tar", last modified: Fri May 26 07:38:43 2023, max compression
+gzip compressed data, was "rppt-1.1.2.tar", last modified: Fri May 26 07:58:03 2023, max compression
```

## Comparing `rppt-1.1.1.tar` & `rppt-1.1.2.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 07:38:43.721799 rppt-1.1.1/
--rw-rw-rw-   0        0        0       14 2023-05-26 07:38:39.000000 rppt-1.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2137 2023-05-26 07:38:43.721799 rppt-1.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-26 07:38:43.487440 rppt-1.1.1/rppt/
--rw-rw-rw-   0        0        0      201 2023-05-26 07:08:22.000000 rppt-1.1.1/rppt/__init__.py
--rw-rw-rw-   0        0        0     1576 2023-05-26 07:08:21.000000 rppt-1.1.1/rppt/class_Rlist.py
-drwxrwxrwx   0        0        0        0 2023-05-26 07:38:43.721799 rppt-1.1.1/rppt.egg-info/
--rw-rw-rw-   0        0        0     2137 2023-05-26 07:38:42.000000 rppt-1.1.1/rppt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      179 2023-05-26 07:38:42.000000 rppt-1.1.1/rppt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 07:38:42.000000 rppt-1.1.1/rppt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-05-26 07:38:42.000000 rppt-1.1.1/rppt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-26 07:38:43.721799 rppt-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      690 2023-05-26 07:38:39.000000 rppt-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 07:58:03.674925 rppt-1.1.2/
+-rw-rw-rw-   0        0        0       14 2023-05-26 07:57:58.000000 rppt-1.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2137 2023-05-26 07:58:03.674925 rppt-1.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-26 07:58:03.169804 rppt-1.1.2/rppt/
+-rw-rw-rw-   0        0        0     1800 2023-05-26 07:55:10.000000 rppt-1.1.2/rppt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 07:58:03.673923 rppt-1.1.2/rppt.egg-info/
+-rw-rw-rw-   0        0        0     2137 2023-05-26 07:58:02.000000 rppt-1.1.2/rppt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      159 2023-05-26 07:58:02.000000 rppt-1.1.2/rppt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 07:58:02.000000 rppt-1.1.2/rppt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-05-26 07:58:02.000000 rppt-1.1.2/rppt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 07:58:03.678923 rppt-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      690 2023-05-26 07:57:58.000000 rppt-1.1.2/setup.py
```

### Comparing `rppt-1.1.1/PKG-INFO` & `rppt-1.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rppt
-Version: 1.1.1
+Version: 1.1.2
 Summary: a library that simplifies writing code using "random" library
 Home-page: https://github.com/Rand0mLit3ral/rppt-v1.1.0/tree/main
 Author: Rand0mLit3ral
 Author-email: randomliteral@mail.ru
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rppt-1.1.1/rppt/class_Rlist.py` & `rppt-1.1.2/rppt/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+'''RLIST CODE
+->'''
+
 import random
 
 class Rlist:
 	def __init__(self, list: list, blackList: list = []):
 		self.list = list
 		self.blackList = blackList
 		self.outputList = []
@@ -56,8 +59,18 @@
 
 	def GetList(self, settype: str = 'list'):
 		if settype == 'list':
 			return self.outputList
 		elif settype == 'str':
 			return ', '.join(map(str, self.outputList))
 		else:
-			return 'None'
+			return 'None'
+
+'''RLIST CODE
+<-'''
+
+class Main:
+	def __init__(self):
+		self.link_to_the_project = "https://pypi.org/project/randomPlusPlus-tools/"
+
+	def __str__(self):
+		return self.link_to_the_project
```

### Comparing `rppt-1.1.1/rppt.egg-info/PKG-INFO` & `rppt-1.1.2/rppt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rppt
-Version: 1.1.1
+Version: 1.1.2
 Summary: a library that simplifies writing code using "random" library
 Home-page: https://github.com/Rand0mLit3ral/rppt-v1.1.0/tree/main
 Author: Rand0mLit3ral
 Author-email: randomliteral@mail.ru
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rppt-1.1.1/setup.py` & `rppt-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 with open(r'C:\Users\Имя\Desktop\pyth_library\README.md', 'r', encoding='utf-8') as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name='rppt',
-	version='1.1.1',
+	version='1.1.2',
 	author='Rand0mLit3ral',
 	author_email='randomliteral@mail.ru',
 	description='a library that simplifies writing code using "random" library',
 	long_description=long_description,
 	long_description_content_type='text/markdown',
 	url='https://github.com/Rand0mLit3ral/rppt-v1.1.0/tree/main',
 	packages=['rppt'],
```

