# Comparing `tmp/seqslab-connector-0.0.0a1.tar.gz` & `tmp/seqslab-connector-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seqslab-connector-0.0.0a1.tar", last modified: Thu May 25 10:53:11 2023, max compression
+gzip compressed data, was "seqslab-connector-0.9.0.tar", last modified: Fri May 26 08:12:52 2023, max compression
```

## Comparing `seqslab-connector-0.0.0a1.tar` & `seqslab-connector-0.9.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-25 10:53:11.121442 seqslab-connector-0.0.0a1/
--rw-r--r--   0 chris      (501) staff       (20)    11357 2023-05-25 09:59:51.000000 seqslab-connector-0.0.0a1/LICENSE
--rw-r--r--   0 chris      (501) staff       (20)     2161 2023-05-25 10:53:11.122035 seqslab-connector-0.0.0a1/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)     1582 2023-05-25 09:59:51.000000 seqslab-connector-0.0.0a1/README.md
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-25 10:53:11.111556 seqslab-connector-0.0.0a1/seqslab/
--rw-r--r--   0 chris      (501) staff       (20)       25 2023-05-25 10:52:17.000000 seqslab-connector-0.0.0a1/seqslab/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)     2486 2023-05-25 09:59:51.000000 seqslab-connector-0.0.0a1/seqslab/hive.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-25 10:53:11.114332 seqslab-connector-0.0.0a1/seqslab/sqlalchemy/
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-05-25 09:59:51.000000 seqslab-connector-0.0.0a1/seqslab/sqlalchemy/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)     3231 2023-05-25 09:59:51.000000 seqslab-connector-0.0.0a1/seqslab/sqlalchemy/hive.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-25 10:53:11.115254 seqslab-connector-0.0.0a1/seqslab/superset/
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-05-25 09:59:51.000000 seqslab-connector-0.0.0a1/seqslab/superset/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)     1772 2023-05-25 09:59:51.000000 seqslab-connector-0.0.0a1/seqslab/superset/seqslab.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-25 10:53:11.120261 seqslab-connector-0.0.0a1/seqslab_connector.egg-info/
--rw-r--r--   0 chris      (501) staff       (20)     2161 2023-05-25 10:53:11.000000 seqslab-connector-0.0.0a1/seqslab_connector.egg-info/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)      435 2023-05-25 10:53:11.000000 seqslab-connector-0.0.0a1/seqslab_connector.egg-info/SOURCES.txt
--rw-r--r--   0 chris      (501) staff       (20)        1 2023-05-25 10:53:11.000000 seqslab-connector-0.0.0a1/seqslab_connector.egg-info/dependency_links.txt
--rw-r--r--   0 chris      (501) staff       (20)      165 2023-05-25 10:53:11.000000 seqslab-connector-0.0.0a1/seqslab_connector.egg-info/entry_points.txt
--rw-r--r--   0 chris      (501) staff       (20)       74 2023-05-25 10:53:11.000000 seqslab-connector-0.0.0a1/seqslab_connector.egg-info/requires.txt
--rw-r--r--   0 chris      (501) staff       (20)        8 2023-05-25 10:53:11.000000 seqslab-connector-0.0.0a1/seqslab_connector.egg-info/top_level.txt
--rw-r--r--   0 chris      (501) staff       (20)      208 2023-05-25 10:53:11.124092 seqslab-connector-0.0.0a1/setup.cfg
--rw-r--r--   0 chris      (501) staff       (20)     1964 2023-05-25 10:53:02.000000 seqslab-connector-0.0.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:12:52.838075 seqslab-connector-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-26 08:12:37.000000 seqslab-connector-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-26 08:12:52.838075 seqslab-connector-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-26 08:12:37.000000 seqslab-connector-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-26 08:12:37.000000 seqslab-connector-0.9.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:12:52.834075 seqslab-connector-0.9.0/seqslab/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-26 08:12:37.000000 seqslab-connector-0.9.0/seqslab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-05-26 08:12:37.000000 seqslab-connector-0.9.0/seqslab/hive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:12:52.838075 seqslab-connector-0.9.0/seqslab/sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:12:37.000000 seqslab-connector-0.9.0/seqslab/sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-05-26 08:12:37.000000 seqslab-connector-0.9.0/seqslab/sqlalchemy/hive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:12:52.838075 seqslab-connector-0.9.0/seqslab/superset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:12:37.000000 seqslab-connector-0.9.0/seqslab/superset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-05-26 08:12:37.000000 seqslab-connector-0.9.0/seqslab/superset/seqslab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:12:52.838075 seqslab-connector-0.9.0/seqslab_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-26 08:12:52.000000 seqslab-connector-0.9.0/seqslab_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-26 08:12:52.000000 seqslab-connector-0.9.0/seqslab_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 08:12:52.000000 seqslab-connector-0.9.0/seqslab_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-26 08:12:52.000000 seqslab-connector-0.9.0/seqslab_connector.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-26 08:12:52.000000 seqslab-connector-0.9.0/seqslab_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-26 08:12:52.000000 seqslab-connector-0.9.0/seqslab_connector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-26 08:12:52.838075 seqslab-connector-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-05-26 08:12:37.000000 seqslab-connector-0.9.0/setup.py
```

### Comparing `seqslab-connector-0.0.0a1/LICENSE` & `seqslab-connector-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `seqslab-connector-0.0.0a1/PKG-INFO` & `seqslab-connector-0.9.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: seqslab-connector
-Version: 0.0.0a1
-Summary: Atgenomix SeqsLab Connector for Python
-Home-page: https://github.com/atgenomix/seqslab-connector
-Author: Allen Chang
-Author-email: allen.chang@atgenomix.com
-License: Apache License, Version 2.0
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Database :: Front-Ends
-Description-Content-Type: text/markdown
-Provides-Extra: sqlalchemy
-Provides-Extra: superset
-License-File: LICENSE
-
 # seqslab-connector
 
 The SeqsLab Connector for Python based on [pyhive](https://github.com/dropbox/PyHive) allows you to create 
 a Python DB API connection to Atgenomix SeqsLab interactive jobs (clusters) and develop Python-based workflow applications. 
 It is a Hive-Thrift-based client with no dependencies on ODBC or JDBC. 
 It also provides a [SQLAlchemy](https://www.sqlalchemy.org/) dialect and an [Apache Superset](https://superset.apache.org/)
 database engine spec for use with tools to execute DQL.
```

### Comparing `seqslab-connector-0.0.0a1/README.md` & `seqslab-connector-0.9.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,55 +1,79 @@
-# seqslab-connector
-
-The SeqsLab Connector for Python based on [pyhive](https://github.com/dropbox/PyHive) allows you to create 
-a Python DB API connection to Atgenomix SeqsLab interactive jobs (clusters) and develop Python-based workflow applications. 
-It is a Hive-Thrift-based client with no dependencies on ODBC or JDBC. 
-It also provides a [SQLAlchemy](https://www.sqlalchemy.org/) dialect and an [Apache Superset](https://superset.apache.org/)
-database engine spec for use with tools to execute DQL.
-
-You are welcome to file an issue for general use cases. You can also contact Atgenomix Support [here](https://console.seqslab.net).
-
-
-### Requirements
-Python 3.7 or above is required.
-
-
-### Installation
-
-Install using pip.
-
-`pip install seqslab-connector` 
-
-For Apache Superset integration install with
-
-`pip install seqslab-connector[superset]`
-
-
-### Usage
-
-#### DB-API
-
-```python
-from seqslab import hive
-
-cursor = hive.connect(database='run_name', http_path='job_run_id', username='user', password='pass', host='job_cluster_host')
-cursor.execute('SHOW TABLES')
-print(cursor.fetchall())
-cursor.execute('SELECT * FROM my_workflow_table_name LIMIT 10')
-print(cursor.fetchall())
-cursor.close()
-```
-
-#### SQLAlchemy
-
-```python
-from sqlalchemy.engine import create_engine
-
-engine = create_engine('seqslab+hive://user:pass@job_cluster_host/run_name?http_path=job_run_id')
-```
-
-#### Apache Superset
-
-[Connecting to Databases](https://superset.apache.org/docs/databases/db-connection-ui)
-
-#### Documentation
-For the latest documentation, see [SeqsLab](https://docs.atgenomix.com).
+Metadata-Version: 2.1
+Name: seqslab-connector
+Version: 0.9.0
+Summary: Atgenomix SeqsLab Connector for Python
+Home-page: https://github.com/atgenomix/seqslab-connector
+Author: Allen Chang
+Author-email: allen.chang@atgenomix.com
+License: Apache License, Version 2.0
+Project-URL: Documentation, https://docs.atgenomix.com/
+Project-URL: Repository, https://github.com/atgenomix/seqslab-connector
+Description: # seqslab-connector
+        
+        The SeqsLab Connector for Python based on [pyhive](https://github.com/dropbox/PyHive) allows you to create 
+        a Python DB API connection to Atgenomix SeqsLab interactive jobs (clusters) and develop Python-based workflow applications. 
+        It is a Hive-Thrift-based client with no dependencies on ODBC or JDBC. 
+        It also provides a [SQLAlchemy](https://www.sqlalchemy.org/) dialect and an [Apache Superset](https://superset.apache.org/)
+        database engine spec for use with tools to execute DQL.
+        
+        You are welcome to file an issue for general use cases. You can also contact Atgenomix Support [here](https://console.seqslab.net).
+        
+        
+        ### Requirements
+        Python 3.7 or above is required.
+        
+        
+        ### Installation
+        
+        Install using pip.
+        
+        `pip install seqslab-connector` 
+        
+        For Apache Superset integration install with
+        
+        `pip install seqslab-connector[superset]`
+        
+        
+        ### Usage
+        
+        #### DB-API
+        
+        ```python
+        from seqslab import hive
+        
+        cursor = hive.connect(database='run_name', http_path='job_run_id', username='user', password='pass', host='job_cluster_host')
+        cursor.execute('SHOW TABLES')
+        print(cursor.fetchall())
+        cursor.execute('SELECT * FROM my_workflow_table_name LIMIT 10')
+        print(cursor.fetchall())
+        cursor.close()
+        ```
+        
+        #### SQLAlchemy
+        
+        ```python
+        from sqlalchemy.engine import create_engine
+        
+        engine = create_engine('seqslab+hive://user:pass@job_cluster_host/run_name?http_path=job_run_id')
+        ```
+        
+        #### Apache Superset
+        
+        [Connecting to Databases](https://superset.apache.org/docs/databases/db-connection-ui)
+        
+        #### Documentation
+        For the latest documentation, see [SeqsLab](https://docs.atgenomix.com).
+        
+Platform: UNKNOWN
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Database :: Front-Ends
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
+Provides-Extra: sqlalchemy
+Provides-Extra: superset
```

### Comparing `seqslab-connector-0.0.0a1/seqslab/hive.py` & `seqslab-connector-0.9.0/seqslab/hive.py`

 * *Files identical despite different names*

### Comparing `seqslab-connector-0.0.0a1/seqslab/sqlalchemy/hive.py` & `seqslab-connector-0.9.0/seqslab/sqlalchemy/hive.py`

 * *Files identical despite different names*

### Comparing `seqslab-connector-0.0.0a1/seqslab/superset/seqslab.py` & `seqslab-connector-0.9.0/seqslab/superset/seqslab.py`

 * *Files identical despite different names*

### Comparing `seqslab-connector-0.0.0a1/setup.py` & `seqslab-connector-0.9.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 #!/usr/bin/env python3
 
-from setuptools import setup
-import seqslab
 import os
-import re
 from typing import Union, Any
 
-from setuptools import setup, find_packages
+from setuptools import setup
+
+import seqslab
 
 setup_file_loc: Union[Union[str, bytes], Any] = os.path.abspath(
     os.path.dirname(__file__))
 # allow setup.py to be run from any path
 os.chdir(setup_file_loc)
 
-extras_require = {
-}
+extras_require = {}
 
 
 def get_requirement():
-    requirements = [    # dependency list
+    requirements = [  # dependency list
         'pip>=22.0.4'
     ]
     with open(os.path.join(setup_file_loc, 'requirements.txt'), 'r') as f:
         ori_req = f.read().splitlines()
     requirements.extend(ori_req)
     return requirements
 
@@ -45,19 +43,22 @@
     license="Apache License, Version 2.0",
     packages=["seqslab", "seqslab.sqlalchemy", "seqslab.superset"],
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Topic :: Database :: Front-Ends",
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10'
     ],
-    install_requires=[
-        "pyhive",
-        "thrift",
-    ],
+    data_files=[('requirements', ['requirements.txt'])],
+    install_requires=get_requirement(),
     extras_require={
         "sqlalchemy": ["sqlalchemy>=1.3.0"],
         "superset": ["superset>=2.0.1"],
     },
     tests_require=[],
     cmdclass={},
     package_data={
```

