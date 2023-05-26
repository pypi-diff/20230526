# Comparing `tmp/std_daq_client-1.0.2.tar.gz` & `tmp/std_daq_client-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "std_daq_client-1.0.2.tar", last modified: Wed May 24 09:57:08 2023, max compression
+gzip compressed data, was "std_daq_client-1.1.0.tar", last modified: Fri May 26 10:09:02 2023, max compression
```

## Comparing `std_daq_client-1.0.2.tar` & `std_daq_client-1.1.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 babic_a    (501) staff       (20)        0 2023-05-24 09:57:08.678678 std_daq_client-1.0.2/
--rw-r--r--   0 babic_a    (501) staff       (20)      359 2023-05-24 09:57:08.678150 std_daq_client-1.0.2/PKG-INFO
--rw-r--r--   0 babic_a    (501) staff       (20)    11059 2023-05-12 12:51:12.000000 std_daq_client-1.0.2/README.md
--rw-r--r--   0 babic_a    (501) staff       (20)       38 2023-05-24 09:57:08.678831 std_daq_client-1.0.2/setup.cfg
--rw-r--r--   0 babic_a    (501) staff       (20)     1317 2023-05-16 08:33:36.000000 std_daq_client-1.0.2/setup.py
--rw-r--r--   0 babic_a    (501) staff       (20)     1003 2023-05-24 09:56:42.000000 std_daq_client-1.0.2/setup_client.py
-drwxr-xr-x   0 babic_a    (501) staff       (20)        0 2023-05-24 09:57:08.671269 std_daq_client-1.0.2/std_daq_client/
--rw-r--r--   0 babic_a    (501) staff       (20)       68 2023-05-24 09:15:21.000000 std_daq_client-1.0.2/std_daq_client/__init__.py
-drwxr-xr-x   0 babic_a    (501) staff       (20)        0 2023-05-24 09:57:08.677454 std_daq_client-1.0.2/std_daq_client/cli/
--rw-r--r--   0 babic_a    (501) staff       (20)        0 2023-05-24 09:17:15.000000 std_daq_client-1.0.2/std_daq_client/cli/__init__.py
--rw-r--r--   0 babic_a    (501) staff       (20)      448 2023-05-24 09:55:36.000000 std_daq_client-1.0.2/std_daq_client/cli/get_config.py
--rw-r--r--   0 babic_a    (501) staff       (20)      470 2023-05-24 09:55:47.000000 std_daq_client-1.0.2/std_daq_client/cli/get_deploy_status.py
--rw-r--r--   0 babic_a    (501) staff       (20)      550 2023-05-24 09:55:59.000000 std_daq_client-1.0.2/std_daq_client/cli/get_logs.py
--rw-r--r--   0 babic_a    (501) staff       (20)      446 2023-05-24 09:56:12.000000 std_daq_client-1.0.2/std_daq_client/cli/get_stats.py
--rw-r--r--   0 babic_a    (501) staff       (20)      448 2023-05-24 09:56:17.000000 std_daq_client-1.0.2/std_daq_client/cli/get_status.py
--rw-r--r--   0 babic_a    (501) staff       (20)     2344 2023-05-24 09:15:21.000000 std_daq_client-1.0.2/std_daq_client/client.py
-drwxr-xr-x   0 babic_a    (501) staff       (20)        0 2023-05-24 09:57:08.674458 std_daq_client-1.0.2/std_daq_client.egg-info/
--rw-r--r--   0 babic_a    (501) staff       (20)      359 2023-05-24 09:57:08.000000 std_daq_client-1.0.2/std_daq_client.egg-info/PKG-INFO
--rw-r--r--   0 babic_a    (501) staff       (20)      516 2023-05-24 09:57:08.000000 std_daq_client-1.0.2/std_daq_client.egg-info/SOURCES.txt
--rw-r--r--   0 babic_a    (501) staff       (20)        1 2023-05-24 09:57:08.000000 std_daq_client-1.0.2/std_daq_client.egg-info/dependency_links.txt
--rw-r--r--   0 babic_a    (501) staff       (20)      306 2023-05-24 09:57:08.000000 std_daq_client-1.0.2/std_daq_client.egg-info/entry_points.txt
--rw-r--r--   0 babic_a    (501) staff       (20)        9 2023-05-24 09:57:08.000000 std_daq_client-1.0.2/std_daq_client.egg-info/requires.txt
--rw-r--r--   0 babic_a    (501) staff       (20)       15 2023-05-24 09:57:08.000000 std_daq_client-1.0.2/std_daq_client.egg-info/top_level.txt
+drwxr-xr-x   0 babic_a    (501) staff       (20)        0 2023-05-26 10:09:02.704617 std_daq_client-1.1.0/
+-rw-r--r--   0 babic_a    (501) staff       (20)      693 2023-05-26 10:09:02.703907 std_daq_client-1.1.0/PKG-INFO
+-rw-r--r--   0 babic_a    (501) staff       (20)    11059 2023-05-12 12:51:12.000000 std_daq_client-1.1.0/README.md
+-rw-r--r--   0 babic_a    (501) staff       (20)       38 2023-05-26 10:09:02.704766 std_daq_client-1.1.0/setup.cfg
+-rw-r--r--   0 babic_a    (501) staff       (20)     1317 2023-05-16 08:33:36.000000 std_daq_client-1.1.0/setup.py
+-rw-r--r--   0 babic_a    (501) staff       (20)     1129 2023-05-26 10:08:28.000000 std_daq_client-1.1.0/setup_client.py
+drwxr-xr-x   0 babic_a    (501) staff       (20)        0 2023-05-26 10:09:02.695878 std_daq_client-1.1.0/std_daq_client/
+-rw-r--r--   0 babic_a    (501) staff       (20)       68 2023-05-24 09:15:21.000000 std_daq_client-1.1.0/std_daq_client/__init__.py
+drwxr-xr-x   0 babic_a    (501) staff       (20)        0 2023-05-26 10:09:02.703246 std_daq_client-1.1.0/std_daq_client/cli/
+-rw-r--r--   0 babic_a    (501) staff       (20)        0 2023-05-24 09:17:15.000000 std_daq_client-1.1.0/std_daq_client/cli/__init__.py
+-rw-r--r--   0 babic_a    (501) staff       (20)      448 2023-05-24 09:55:36.000000 std_daq_client-1.1.0/std_daq_client/cli/get_config.py
+-rw-r--r--   0 babic_a    (501) staff       (20)      470 2023-05-24 09:55:47.000000 std_daq_client-1.1.0/std_daq_client/cli/get_deploy_status.py
+-rw-r--r--   0 babic_a    (501) staff       (20)      550 2023-05-24 09:55:59.000000 std_daq_client-1.1.0/std_daq_client/cli/get_logs.py
+-rw-r--r--   0 babic_a    (501) staff       (20)      446 2023-05-24 09:56:12.000000 std_daq_client-1.1.0/std_daq_client/cli/get_stats.py
+-rw-r--r--   0 babic_a    (501) staff       (20)      448 2023-05-24 09:56:17.000000 std_daq_client-1.1.0/std_daq_client/cli/get_status.py
+-rw-r--r--   0 babic_a    (501) staff       (20)     1149 2023-05-26 10:03:12.000000 std_daq_client-1.1.0/std_daq_client/cli/write.py
+-rw-r--r--   0 babic_a    (501) staff       (20)    12087 2023-05-26 09:52:04.000000 std_daq_client-1.1.0/std_daq_client/client.py
+drwxr-xr-x   0 babic_a    (501) staff       (20)        0 2023-05-26 10:09:02.699366 std_daq_client-1.1.0/std_daq_client.egg-info/
+-rw-r--r--   0 babic_a    (501) staff       (20)      693 2023-05-26 10:09:02.000000 std_daq_client-1.1.0/std_daq_client.egg-info/PKG-INFO
+-rw-r--r--   0 babic_a    (501) staff       (20)      544 2023-05-26 10:09:02.000000 std_daq_client-1.1.0/std_daq_client.egg-info/SOURCES.txt
+-rw-r--r--   0 babic_a    (501) staff       (20)        1 2023-05-26 10:09:02.000000 std_daq_client-1.1.0/std_daq_client.egg-info/dependency_links.txt
+-rw-r--r--   0 babic_a    (501) staff       (20)      420 2023-05-26 10:09:02.000000 std_daq_client-1.1.0/std_daq_client.egg-info/entry_points.txt
+-rw-r--r--   0 babic_a    (501) staff       (20)        9 2023-05-26 10:09:02.000000 std_daq_client-1.1.0/std_daq_client.egg-info/requires.txt
+-rw-r--r--   0 babic_a    (501) staff       (20)       15 2023-05-26 10:09:02.000000 std_daq_client-1.1.0/std_daq_client.egg-info/top_level.txt
```

### Comparing `std_daq_client-1.0.2/README.md` & `std_daq_client-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `std_daq_client-1.0.2/setup.py` & `std_daq_client-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `std_daq_client-1.0.2/setup_client.py` & `std_daq_client-1.1.0/setup_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 from setuptools import setup
 
-CLIENT_VERSION = "1.0.2"
+CLIENT_VERSION = "1.1.0"
 
 with open(os.path.join(os.path.dirname(__file__), 'std_daq_client/', 'README.md')) as readme:
     long_description = readme.read()
 
 setup(
     version=CLIENT_VERSION,
     name='std_daq_client',
@@ -18,14 +18,16 @@
     entry_points='''
         [console_scripts]
         std_cli_get_config=std_daq_client.cli.get_config:main
         std_cli_get_deploy_status=std_daq_client.cli.get_deploy_status:main
         std_cli_get_logs=std_daq_client.cli.get_logs:main
         std_cli_get_stats=std_daq_client.cli.get_stats:main
         std_cli_get_status=std_daq_client.cli.get_status:main
+        std_cli_write_async=std_daq_client.cli.write:main_sync
+        std_cli_write_sync=std_daq_client.cli.write:main_async
     ''',
 
     author="Paul Scherrer Institute",
     url='https://github.com/paulscherrerinstitute/std_daq_service',
     description='Python client for standard-daq',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

### Comparing `std_daq_client-1.0.2/std_daq_client/cli/get_logs.py` & `std_daq_client-1.1.0/std_daq_client/cli/get_logs.py`

 * *Files identical despite different names*

### Comparing `std_daq_client-1.0.2/std_daq_client.egg-info/SOURCES.txt` & `std_daq_client-1.1.0/std_daq_client.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -10,8 +10,9 @@
 std_daq_client.egg-info/requires.txt
 std_daq_client.egg-info/top_level.txt
 std_daq_client/cli/__init__.py
 std_daq_client/cli/get_config.py
 std_daq_client/cli/get_deploy_status.py
 std_daq_client/cli/get_logs.py
 std_daq_client/cli/get_stats.py
-std_daq_client/cli/get_status.py
+std_daq_client/cli/get_status.py
+std_daq_client/cli/write.py
```

