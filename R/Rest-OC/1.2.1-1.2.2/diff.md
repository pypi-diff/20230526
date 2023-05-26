# Comparing `tmp/Rest-OC-1.2.1.tar.gz` & `tmp/Rest-OC-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Rest-OC-1.2.1.tar", last modified: Mon Mar 20 18:19:01 2023, max compression
+gzip compressed data, was "Rest-OC-1.2.2.tar", last modified: Fri May 26 11:06:59 2023, max compression
```

## Comparing `Rest-OC-1.2.1.tar` & `Rest-OC-1.2.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 bast      (1002) bast      (1002)        0 2023-03-20 18:19:01.480399 Rest-OC-1.2.1/
--rw-rw-r--   0 bast      (1002) bast      (1002)     1073 2023-03-03 20:50:56.000000 Rest-OC-1.2.1/LICENSE
--rw-rw-r--   0 bast      (1002) bast      (1002)      856 2023-03-20 18:19:01.480399 Rest-OC-1.2.1/PKG-INFO
--rw-rw-r--   0 bast      (1002) bast      (1002)      217 2023-03-20 17:38:57.000000 Rest-OC-1.2.1/README.md
-drwxrwxr-x   0 bast      (1002) bast      (1002)        0 2023-03-20 18:19:01.480399 Rest-OC-1.2.1/RestOC/
--rw-rw-r--   0 bast      (1002) bast      (1002)     2524 2023-01-10 16:46:53.000000 Rest-OC-1.2.1/RestOC/CLI.py
--rw-rw-r--   0 bast      (1002) bast      (1002)     3857 2023-01-10 16:46:53.000000 Rest-OC-1.2.1/RestOC/Conf.py
--rw-rw-r--   0 bast      (1002) bast      (1002)     5041 2023-01-10 16:46:53.000000 Rest-OC-1.2.1/RestOC/DateTimeHelper.py
--rw-rw-r--   0 bast      (1002) bast      (1002)     5631 2023-01-27 13:06:17.000000 Rest-OC-1.2.1/RestOC/DictHelper.py
--rw-rw-r--   0 bast      (1002) bast      (1002)     3326 2023-03-03 20:50:56.000000 Rest-OC-1.2.1/RestOC/EMail.py
--rw-rw-r--   0 bast      (1002) bast      (1002)     1037 2023-01-10 16:46:53.000000 Rest-OC-1.2.1/RestOC/Environment.py
--rw-rw-r--   0 bast      (1002) bast      (1002)      381 2023-03-20 18:18:38.000000 Rest-OC-1.2.1/RestOC/Errors.py
--rw-rw-r--   0 bast      (1002) bast      (1002)     5526 2023-03-20 17:38:57.000000 Rest-OC-1.2.1/RestOC/Image.py
--rw-rw-r--   0 bast      (1002) bast      (1002)     2946 2023-01-10 16:46:53.000000 Rest-OC-1.2.1/RestOC/JSON.py
--rw-rw-r--   0 bast      (1002) bast      (1002)    14972 2023-03-20 18:18:38.000000 Rest-OC-1.2.1/RestOC/REST.py
--rw-rw-r--   0 bast      (1002) bast      (1002)    23650 2023-02-13 23:13:11.000000 Rest-OC-1.2.1/RestOC/Record_Base.py
--rw-rw-r--   0 bast      (1002) bast      (1002)    66432 2023-03-11 14:44:28.000000 Rest-OC-1.2.1/RestOC/Record_MySQL.py
--rw-rw-r--   0 bast      (1002) bast      (1002)    47196 2023-01-27 13:06:17.000000 Rest-OC-1.2.1/RestOC/Record_ReDB.py
--rw-rw-r--   0 bast      (1002) bast      (1002)     2738 2023-01-10 16:46:53.000000 Rest-OC-1.2.1/RestOC/Resize.py
--rw-rw-r--   0 bast      (1002) bast      (1002)     7092 2023-01-10 16:46:53.000000 Rest-OC-1.2.1/RestOC/SMTP.py
--rw-rw-r--   0 bast      (1002) bast      (1002)    19557 2023-03-03 20:50:56.000000 Rest-OC-1.2.1/RestOC/Services.py
--rw-rw-r--   0 bast      (1002) bast      (1002)     4502 2023-01-10 16:46:53.000000 Rest-OC-1.2.1/RestOC/Session.py
--rw-rw-r--   0 bast      (1002) bast      (1002)    18147 2023-01-10 16:46:53.000000 Rest-OC-1.2.1/RestOC/StrHelper.py
--rw-rw-r--   0 bast      (1002) bast      (1002)     1653 2023-01-10 16:46:53.000000 Rest-OC-1.2.1/RestOC/Templates.py
--rw-r--r--   0 bast      (1002) bast      (1002)        0 2021-06-08 11:58:01.000000 Rest-OC-1.2.1/RestOC/__init__.py
-drwxrwxr-x   0 bast      (1002) bast      (1002)        0 2023-03-20 18:19:01.480399 Rest-OC-1.2.1/Rest_OC.egg-info/
--rw-rw-r--   0 bast      (1002) bast      (1002)      856 2023-03-20 18:19:01.000000 Rest-OC-1.2.1/Rest_OC.egg-info/PKG-INFO
--rw-rw-r--   0 bast      (1002) bast      (1002)      587 2023-03-20 18:19:01.000000 Rest-OC-1.2.1/Rest_OC.egg-info/SOURCES.txt
--rw-rw-r--   0 bast      (1002) bast      (1002)        1 2023-03-20 18:19:01.000000 Rest-OC-1.2.1/Rest_OC.egg-info/dependency_links.txt
--rw-rw-r--   0 bast      (1002) bast      (1002)      199 2023-03-20 18:19:01.000000 Rest-OC-1.2.1/Rest_OC.egg-info/requires.txt
--rw-rw-r--   0 bast      (1002) bast      (1002)        7 2023-03-20 18:19:01.000000 Rest-OC-1.2.1/Rest_OC.egg-info/top_level.txt
--rw-rw-r--   0 bast      (1002) bast      (1002)        1 2022-06-23 11:30:41.000000 Rest-OC-1.2.1/Rest_OC.egg-info/zip-safe
--rw-r--r--   0 bast      (1002) bast      (1002)       79 2023-03-20 18:19:01.480399 Rest-OC-1.2.1/setup.cfg
--rw-rw-r--   0 bast      (1002) bast      (1002)     1074 2023-03-20 18:18:38.000000 Rest-OC-1.2.1/setup.py
+drwxrwxr-x   0 bast      (1002) bast      (1002)        0 2023-05-26 11:06:59.804096 Rest-OC-1.2.2/
+-rw-rw-r--   0 bast      (1002) bast      (1002)     1073 2023-03-03 20:50:56.000000 Rest-OC-1.2.2/LICENSE
+-rw-rw-r--   0 bast      (1002) bast      (1002)      856 2023-05-26 11:06:59.804096 Rest-OC-1.2.2/PKG-INFO
+-rw-rw-r--   0 bast      (1002) bast      (1002)      217 2023-03-20 17:38:57.000000 Rest-OC-1.2.2/README.md
+drwxrwxr-x   0 bast      (1002) bast      (1002)        0 2023-05-26 11:06:59.804096 Rest-OC-1.2.2/RestOC/
+-rw-rw-r--   0 bast      (1002) bast      (1002)     2524 2023-01-10 16:46:53.000000 Rest-OC-1.2.2/RestOC/CLI.py
+-rw-rw-r--   0 bast      (1002) bast      (1002)     3857 2023-01-10 16:46:53.000000 Rest-OC-1.2.2/RestOC/Conf.py
+-rw-rw-r--   0 bast      (1002) bast      (1002)     5041 2023-01-10 16:46:53.000000 Rest-OC-1.2.2/RestOC/DateTimeHelper.py
+-rw-rw-r--   0 bast      (1002) bast      (1002)     5631 2023-01-27 13:06:17.000000 Rest-OC-1.2.2/RestOC/DictHelper.py
+-rw-rw-r--   0 bast      (1002) bast      (1002)     3326 2023-03-03 20:50:56.000000 Rest-OC-1.2.2/RestOC/EMail.py
+-rw-rw-r--   0 bast      (1002) bast      (1002)     1037 2023-01-10 16:46:53.000000 Rest-OC-1.2.2/RestOC/Environment.py
+-rw-rw-r--   0 bast      (1002) bast      (1002)      381 2023-03-20 18:18:38.000000 Rest-OC-1.2.2/RestOC/Errors.py
+-rw-rw-r--   0 bast      (1002) bast      (1002)     5526 2023-03-20 17:38:57.000000 Rest-OC-1.2.2/RestOC/Image.py
+-rw-rw-r--   0 bast      (1002) bast      (1002)     2946 2023-01-10 16:46:53.000000 Rest-OC-1.2.2/RestOC/JSON.py
+-rw-rw-r--   0 bast      (1002) bast      (1002)    15049 2023-05-26 11:06:24.000000 Rest-OC-1.2.2/RestOC/REST.py
+-rw-rw-r--   0 bast      (1002) bast      (1002)    23650 2023-02-13 23:13:11.000000 Rest-OC-1.2.2/RestOC/Record_Base.py
+-rw-rw-r--   0 bast      (1002) bast      (1002)    66432 2023-03-11 14:44:28.000000 Rest-OC-1.2.2/RestOC/Record_MySQL.py
+-rw-rw-r--   0 bast      (1002) bast      (1002)    47196 2023-01-27 13:06:17.000000 Rest-OC-1.2.2/RestOC/Record_ReDB.py
+-rw-rw-r--   0 bast      (1002) bast      (1002)     2738 2023-01-10 16:46:53.000000 Rest-OC-1.2.2/RestOC/Resize.py
+-rw-rw-r--   0 bast      (1002) bast      (1002)     7092 2023-01-10 16:46:53.000000 Rest-OC-1.2.2/RestOC/SMTP.py
+-rw-rw-r--   0 bast      (1002) bast      (1002)    19557 2023-03-26 13:12:06.000000 Rest-OC-1.2.2/RestOC/Services.py
+-rw-rw-r--   0 bast      (1002) bast      (1002)     4502 2023-01-10 16:46:53.000000 Rest-OC-1.2.2/RestOC/Session.py
+-rw-rw-r--   0 bast      (1002) bast      (1002)    18147 2023-01-10 16:46:53.000000 Rest-OC-1.2.2/RestOC/StrHelper.py
+-rw-rw-r--   0 bast      (1002) bast      (1002)     1653 2023-01-10 16:46:53.000000 Rest-OC-1.2.2/RestOC/Templates.py
+-rw-r--r--   0 bast      (1002) bast      (1002)        0 2021-06-08 11:58:01.000000 Rest-OC-1.2.2/RestOC/__init__.py
+drwxrwxr-x   0 bast      (1002) bast      (1002)        0 2023-05-26 11:06:59.804096 Rest-OC-1.2.2/Rest_OC.egg-info/
+-rw-rw-r--   0 bast      (1002) bast      (1002)      856 2023-05-26 11:06:59.000000 Rest-OC-1.2.2/Rest_OC.egg-info/PKG-INFO
+-rw-rw-r--   0 bast      (1002) bast      (1002)      587 2023-05-26 11:06:59.000000 Rest-OC-1.2.2/Rest_OC.egg-info/SOURCES.txt
+-rw-rw-r--   0 bast      (1002) bast      (1002)        1 2023-05-26 11:06:59.000000 Rest-OC-1.2.2/Rest_OC.egg-info/dependency_links.txt
+-rw-rw-r--   0 bast      (1002) bast      (1002)      199 2023-05-26 11:06:59.000000 Rest-OC-1.2.2/Rest_OC.egg-info/requires.txt
+-rw-rw-r--   0 bast      (1002) bast      (1002)        7 2023-05-26 11:06:59.000000 Rest-OC-1.2.2/Rest_OC.egg-info/top_level.txt
+-rw-rw-r--   0 bast      (1002) bast      (1002)        1 2022-06-23 11:30:41.000000 Rest-OC-1.2.2/Rest_OC.egg-info/zip-safe
+-rw-r--r--   0 bast      (1002) bast      (1002)       79 2023-05-26 11:06:59.808096 Rest-OC-1.2.2/setup.cfg
+-rw-rw-r--   0 bast      (1002) bast      (1002)     1074 2023-05-26 11:06:24.000000 Rest-OC-1.2.2/setup.py
```

### Comparing `Rest-OC-1.2.1/LICENSE` & `Rest-OC-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Rest-OC-1.2.1/PKG-INFO` & `Rest-OC-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Rest-OC
-Version: 1.2.1
+Version: 1.2.2
 Summary: Rest-OC is a library of python 3 modules for rapidly setting up REST microservices.
 Home-page: https://ouroboroscoding.com/rest-oc/
 Author: Chris Nasr - Ouroboros Coding Inc.
 Author-email: chris@ouroboroscoding.com
 License: MIT
 Project-URL: Documentation, https://ouroboroscoding.com/rest-oc/
 Project-URL: Source, https://github.com/ouroboroscoding/rest-oc-python
```

### Comparing `Rest-OC-1.2.1/RestOC/CLI.py` & `Rest-OC-1.2.2/RestOC/CLI.py`

 * *Files identical despite different names*

### Comparing `Rest-OC-1.2.1/RestOC/Conf.py` & `Rest-OC-1.2.2/RestOC/Conf.py`

 * *Files identical despite different names*

### Comparing `Rest-OC-1.2.1/RestOC/DateTimeHelper.py` & `Rest-OC-1.2.2/RestOC/DateTimeHelper.py`

 * *Files identical despite different names*

### Comparing `Rest-OC-1.2.1/RestOC/DictHelper.py` & `Rest-OC-1.2.2/RestOC/DictHelper.py`

 * *Files identical despite different names*

### Comparing `Rest-OC-1.2.1/RestOC/EMail.py` & `Rest-OC-1.2.2/RestOC/EMail.py`

 * *Files identical despite different names*

### Comparing `Rest-OC-1.2.1/RestOC/Environment.py` & `Rest-OC-1.2.2/RestOC/Environment.py`

 * *Files identical despite different names*

### Comparing `Rest-OC-1.2.1/RestOC/Image.py` & `Rest-OC-1.2.2/RestOC/Image.py`

 * *Files identical despite different names*

### Comparing `Rest-OC-1.2.1/RestOC/JSON.py` & `Rest-OC-1.2.2/RestOC/JSON.py`

 * *Files identical despite different names*

### Comparing `Rest-OC-1.2.1/RestOC/REST.py` & `Rest-OC-1.2.2/RestOC/REST.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,15 +205,19 @@
 
 							# If we got a string
 							if isinstance(m, str):
 								m = [m]
 
 							# Generate unique request details for the element
 							dRequest = DictHelper.clone(dReq)
-							dRequest['data'] = len(m) == 2 and m[1] or None
+							if len(m) == 2:
+								dRequest['data'] = m[1]
+							else:
+								try: del dRequest['data']
+								except KeyError: pass
 
 							# Call the request and append the data to the
 							#	response
 							lResponse.append([
 								m[0],
 								Services.read(
 									self.service, m[0], dRequest
```

### Comparing `Rest-OC-1.2.1/RestOC/Record_Base.py` & `Rest-OC-1.2.2/RestOC/Record_Base.py`

 * *Files identical despite different names*

### Comparing `Rest-OC-1.2.1/RestOC/Record_MySQL.py` & `Rest-OC-1.2.2/RestOC/Record_MySQL.py`

 * *Files identical despite different names*

### Comparing `Rest-OC-1.2.1/RestOC/Record_ReDB.py` & `Rest-OC-1.2.2/RestOC/Record_ReDB.py`

 * *Files identical despite different names*

### Comparing `Rest-OC-1.2.1/RestOC/Resize.py` & `Rest-OC-1.2.2/RestOC/Resize.py`

 * *Files identical despite different names*

### Comparing `Rest-OC-1.2.1/RestOC/SMTP.py` & `Rest-OC-1.2.2/RestOC/SMTP.py`

 * *Files identical despite different names*

### Comparing `Rest-OC-1.2.1/RestOC/Services.py` & `Rest-OC-1.2.2/RestOC/Services.py`

 * *Files identical despite different names*

### Comparing `Rest-OC-1.2.1/RestOC/Session.py` & `Rest-OC-1.2.2/RestOC/Session.py`

 * *Files identical despite different names*

### Comparing `Rest-OC-1.2.1/RestOC/StrHelper.py` & `Rest-OC-1.2.2/RestOC/StrHelper.py`

 * *Files identical despite different names*

### Comparing `Rest-OC-1.2.1/RestOC/Templates.py` & `Rest-OC-1.2.2/RestOC/Templates.py`

 * *Files identical despite different names*

### Comparing `Rest-OC-1.2.1/Rest_OC.egg-info/PKG-INFO` & `Rest-OC-1.2.2/Rest_OC.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Rest-OC
-Version: 1.2.1
+Version: 1.2.2
 Summary: Rest-OC is a library of python 3 modules for rapidly setting up REST microservices.
 Home-page: https://ouroboroscoding.com/rest-oc/
 Author: Chris Nasr - Ouroboros Coding Inc.
 Author-email: chris@ouroboroscoding.com
 License: MIT
 Project-URL: Documentation, https://ouroboroscoding.com/rest-oc/
 Project-URL: Source, https://github.com/ouroboroscoding/rest-oc-python
```

### Comparing `Rest-OC-1.2.1/Rest_OC.egg-info/SOURCES.txt` & `Rest-OC-1.2.2/Rest_OC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Rest-OC-1.2.1/setup.py` & `Rest-OC-1.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as oF:
 	long_description=oF.read()
 
 setup(
 	name='Rest-OC',
-	version='1.2.1',
+	version='1.2.2',
 	description='Rest-OC is a library of python 3 modules for rapidly setting up REST microservices.',
 	long_description=long_description,
 	long_description_content_type='text/markdown',
 	url='https://ouroboroscoding.com/rest-oc/',
 	project_urls={
 		'Documentation': 'https://ouroboroscoding.com/rest-oc/',
 		'Source': 'https://github.com/ouroboroscoding/rest-oc-python',
```

