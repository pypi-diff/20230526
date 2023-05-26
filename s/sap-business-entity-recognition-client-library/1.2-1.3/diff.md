# Comparing `tmp/sap-business-entity-recognition-client-library-1.2.tar.gz` & `tmp/sap-business-entity-recognition-client-library-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sap-business-entity-recognition-client-library-1.2.tar", last modified: Wed May  3 08:08:29 2023, max compression
+gzip compressed data, was "sap-business-entity-recognition-client-library-1.3.tar", last modified: Fri May 26 04:58:06 2023, max compression
```

## Comparing `sap-business-entity-recognition-client-library-1.2.tar` & `sap-business-entity-recognition-client-library-1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 vipulprabhu   (501) staff       (20)        0 2023-05-03 08:08:29.621726 sap-business-entity-recognition-client-library-1.2/
--rw-r--r--   0 vipulprabhu   (501) staff       (20)    11357 2023-05-03 03:32:13.000000 sap-business-entity-recognition-client-library-1.2/LICENSE
--rw-r--r--   0 vipulprabhu   (501) staff       (20)       39 2023-05-03 03:32:13.000000 sap-business-entity-recognition-client-library-1.2/MANIFEST.in
--rw-r--r--   0 vipulprabhu   (501) staff       (20)      870 2023-05-03 08:08:29.621888 sap-business-entity-recognition-client-library-1.2/PKG-INFO
--rw-r--r--   0 vipulprabhu   (501) staff       (20)     2314 2023-05-03 03:32:13.000000 sap-business-entity-recognition-client-library-1.2/README.md
--rw-r--r--   0 vipulprabhu   (501) staff       (20)       12 2023-05-03 03:32:13.000000 sap-business-entity-recognition-client-library-1.2/runtime.txt
-drwxr-xr-x   0 vipulprabhu   (501) staff       (20)        0 2023-05-03 08:08:29.615865 sap-business-entity-recognition-client-library-1.2/sap_ber_client/
--rw-r--r--   0 vipulprabhu   (501) staff       (20)       43 2023-05-03 03:32:13.000000 sap-business-entity-recognition-client-library-1.2/sap_ber_client/__init__.py
--rw-r--r--   0 vipulprabhu   (501) staff       (20)    18630 2023-05-03 03:32:13.000000 sap-business-entity-recognition-client-library-1.2/sap_ber_client/ber_api_client.py
--rw-r--r--   0 vipulprabhu   (501) staff       (20)     2045 2023-05-03 03:32:13.000000 sap-business-entity-recognition-client-library-1.2/sap_ber_client/constants.py
--rw-r--r--   0 vipulprabhu   (501) staff       (20)     4743 2023-05-03 03:32:13.000000 sap-business-entity-recognition-client-library-1.2/sap_ber_client/http_client_base.py
--rw-r--r--   0 vipulprabhu   (501) staff       (20)      838 2023-05-03 03:32:13.000000 sap-business-entity-recognition-client-library-1.2/sap_ber_client/http_request_retry.py
-drwxr-xr-x   0 vipulprabhu   (501) staff       (20)        0 2023-05-03 08:08:29.621129 sap-business-entity-recognition-client-library-1.2/sap_business_entity_recognition_client_library.egg-info/
--rw-r--r--   0 vipulprabhu   (501) staff       (20)      870 2023-05-03 08:08:29.000000 sap-business-entity-recognition-client-library-1.2/sap_business_entity_recognition_client_library.egg-info/PKG-INFO
--rw-r--r--   0 vipulprabhu   (501) staff       (20)      569 2023-05-03 08:08:29.000000 sap-business-entity-recognition-client-library-1.2/sap_business_entity_recognition_client_library.egg-info/SOURCES.txt
--rw-r--r--   0 vipulprabhu   (501) staff       (20)        1 2023-05-03 08:08:29.000000 sap-business-entity-recognition-client-library-1.2/sap_business_entity_recognition_client_library.egg-info/dependency_links.txt
--rw-r--r--   0 vipulprabhu   (501) staff       (20)       17 2023-05-03 08:08:29.000000 sap-business-entity-recognition-client-library-1.2/sap_business_entity_recognition_client_library.egg-info/requires.txt
--rw-r--r--   0 vipulprabhu   (501) staff       (20)       15 2023-05-03 08:08:29.000000 sap-business-entity-recognition-client-library-1.2/sap_business_entity_recognition_client_library.egg-info/top_level.txt
--rw-r--r--   0 vipulprabhu   (501) staff       (20)       79 2023-05-03 08:08:29.624483 sap-business-entity-recognition-client-library-1.2/setup.cfg
--rw-r--r--   0 vipulprabhu   (501) staff       (20)     1359 2023-05-03 08:05:52.000000 sap-business-entity-recognition-client-library-1.2/setup.py
+drwxr-xr-x   0 vipulprabhu   (501) staff       (20)        0 2023-05-26 04:58:06.163918 sap-business-entity-recognition-client-library-1.3/
+-rw-r--r--   0 vipulprabhu   (501) staff       (20)    11357 2023-05-03 03:32:13.000000 sap-business-entity-recognition-client-library-1.3/LICENSE
+-rw-r--r--   0 vipulprabhu   (501) staff       (20)       39 2023-05-03 03:32:13.000000 sap-business-entity-recognition-client-library-1.3/MANIFEST.in
+-rw-r--r--   0 vipulprabhu   (501) staff       (20)      898 2023-05-26 04:58:06.164104 sap-business-entity-recognition-client-library-1.3/PKG-INFO
+-rw-r--r--   0 vipulprabhu   (501) staff       (20)     2314 2023-05-03 03:32:13.000000 sap-business-entity-recognition-client-library-1.3/README.md
+-rw-r--r--   0 vipulprabhu   (501) staff       (20)       12 2023-05-03 03:32:13.000000 sap-business-entity-recognition-client-library-1.3/runtime.txt
+drwxr-xr-x   0 vipulprabhu   (501) staff       (20)        0 2023-05-26 04:58:06.158974 sap-business-entity-recognition-client-library-1.3/sap_ber_client/
+-rw-r--r--   0 vipulprabhu   (501) staff       (20)       43 2023-05-03 03:32:13.000000 sap-business-entity-recognition-client-library-1.3/sap_ber_client/__init__.py
+-rw-r--r--   0 vipulprabhu   (501) staff       (20)    18630 2023-05-03 03:32:13.000000 sap-business-entity-recognition-client-library-1.3/sap_ber_client/ber_api_client.py
+-rw-r--r--   0 vipulprabhu   (501) staff       (20)     2045 2023-05-03 03:32:13.000000 sap-business-entity-recognition-client-library-1.3/sap_ber_client/constants.py
+-rw-r--r--   0 vipulprabhu   (501) staff       (20)     4743 2023-05-03 03:32:13.000000 sap-business-entity-recognition-client-library-1.3/sap_ber_client/http_client_base.py
+-rw-r--r--   0 vipulprabhu   (501) staff       (20)      838 2023-05-03 03:32:13.000000 sap-business-entity-recognition-client-library-1.3/sap_ber_client/http_request_retry.py
+drwxr-xr-x   0 vipulprabhu   (501) staff       (20)        0 2023-05-26 04:58:06.163231 sap-business-entity-recognition-client-library-1.3/sap_business_entity_recognition_client_library.egg-info/
+-rw-r--r--   0 vipulprabhu   (501) staff       (20)      898 2023-05-26 04:58:05.000000 sap-business-entity-recognition-client-library-1.3/sap_business_entity_recognition_client_library.egg-info/PKG-INFO
+-rw-r--r--   0 vipulprabhu   (501) staff       (20)      569 2023-05-26 04:58:05.000000 sap-business-entity-recognition-client-library-1.3/sap_business_entity_recognition_client_library.egg-info/SOURCES.txt
+-rw-r--r--   0 vipulprabhu   (501) staff       (20)        1 2023-05-26 04:58:05.000000 sap-business-entity-recognition-client-library-1.3/sap_business_entity_recognition_client_library.egg-info/dependency_links.txt
+-rw-r--r--   0 vipulprabhu   (501) staff       (20)       15 2023-05-26 04:58:05.000000 sap-business-entity-recognition-client-library-1.3/sap_business_entity_recognition_client_library.egg-info/requires.txt
+-rw-r--r--   0 vipulprabhu   (501) staff       (20)       15 2023-05-26 04:58:05.000000 sap-business-entity-recognition-client-library-1.3/sap_business_entity_recognition_client_library.egg-info/top_level.txt
+-rw-r--r--   0 vipulprabhu   (501) staff       (20)       79 2023-05-26 04:58:06.166598 sap-business-entity-recognition-client-library-1.3/setup.cfg
+-rw-r--r--   0 vipulprabhu   (501) staff       (20)     1357 2023-05-26 04:56:42.000000 sap-business-entity-recognition-client-library-1.3/setup.py
```

### Comparing `sap-business-entity-recognition-client-library-1.2/LICENSE` & `sap-business-entity-recognition-client-library-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sap-business-entity-recognition-client-library-1.2/PKG-INFO` & `sap-business-entity-recognition-client-library-1.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 Metadata-Version: 2.1
 Name: sap-business-entity-recognition-client-library
-Version: 1.2
+Version: 1.3
 Summary: Exposes easy consumable methods via a client library, to access and use the API offerings of the AI BUS Service - Business Entity Recognition.
 Home-page: https://github.com/SAP/business-entity-recognition-client-library
-Download-URL: https://github.com/SAP/business-entity-recognition-client-library/archive/refs/heads/main.zip
 Author: Gokul Mohanarangan
 Author-email: gokumohan@gmail.com
 Maintainer: Gokul Mohanarangan
 Maintainer-email: gokumohan@gmail.com
 License: apache-2.0
+Download-URL: https://github.com/SAP/business-entity-recognition-client-library/archive/refs/heads/main.zip
 Keywords: business,entity,recognition,machine learning,SAP,client,library
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `sap-business-entity-recognition-client-library-1.2/README.md` & `sap-business-entity-recognition-client-library-1.3/README.md`

 * *Files identical despite different names*

### Comparing `sap-business-entity-recognition-client-library-1.2/sap_ber_client/ber_api_client.py` & `sap-business-entity-recognition-client-library-1.3/sap_ber_client/ber_api_client.py`

 * *Files identical despite different names*

### Comparing `sap-business-entity-recognition-client-library-1.2/sap_ber_client/constants.py` & `sap-business-entity-recognition-client-library-1.3/sap_ber_client/constants.py`

 * *Files identical despite different names*

### Comparing `sap-business-entity-recognition-client-library-1.2/sap_ber_client/http_client_base.py` & `sap-business-entity-recognition-client-library-1.3/sap_ber_client/http_client_base.py`

 * *Files identical despite different names*

### Comparing `sap-business-entity-recognition-client-library-1.2/sap_ber_client/http_request_retry.py` & `sap-business-entity-recognition-client-library-1.3/sap_ber_client/http_request_retry.py`

 * *Files identical despite different names*

### Comparing `sap-business-entity-recognition-client-library-1.2/sap_business_entity_recognition_client_library.egg-info/PKG-INFO` & `sap-business-entity-recognition-client-library-1.3/sap_business_entity_recognition_client_library.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 Metadata-Version: 2.1
 Name: sap-business-entity-recognition-client-library
-Version: 1.2
+Version: 1.3
 Summary: Exposes easy consumable methods via a client library, to access and use the API offerings of the AI BUS Service - Business Entity Recognition.
 Home-page: https://github.com/SAP/business-entity-recognition-client-library
-Download-URL: https://github.com/SAP/business-entity-recognition-client-library/archive/refs/heads/main.zip
 Author: Gokul Mohanarangan
 Author-email: gokumohan@gmail.com
 Maintainer: Gokul Mohanarangan
 Maintainer-email: gokumohan@gmail.com
 License: apache-2.0
+Download-URL: https://github.com/SAP/business-entity-recognition-client-library/archive/refs/heads/main.zip
 Keywords: business,entity,recognition,machine learning,SAP,client,library
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `sap-business-entity-recognition-client-library-1.2/sap_business_entity_recognition_client_library.egg-info/SOURCES.txt` & `sap-business-entity-recognition-client-library-1.3/sap_business_entity_recognition_client_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sap-business-entity-recognition-client-library-1.2/setup.py` & `sap-business-entity-recognition-client-library-1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 https://github.com/pypa/sampleproject
 """
 
 # Always prefer setuptools over distutils
 from setuptools import setup, find_packages
 
 setup(name='sap-business-entity-recognition-client-library',
-      version=1.2,
+      version=1.3,
       license='apache-2.0',
       install_requires=[
-          'requests==2.26.0'
+          'requests~=2.31'
       ],
       packages=find_packages(
           exclude=['examples*']),
       description='Exposes easy consumable methods via a client library, to access and use the API offerings of the AI '
                   'BUS Service - Business Entity Recognition.',
       author='Gokul Mohanarangan',
       author_email='gokumohan@gmail.com',
```

