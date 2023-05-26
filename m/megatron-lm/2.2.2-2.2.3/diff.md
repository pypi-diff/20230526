# Comparing `tmp/megatron-lm-2.2.2.tar.gz` & `tmp/megatron-lm-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/ashish/packj-recon/04-27-2023/pypi/megatron-lm/dist/tmp13cqb0ij/megatron-lm-2.2.2.tar", last modified: Fri Apr 28 15:01:53 2023, max compression
+gzip compressed data, was "megatron-lm-2.2.3.tar", last modified: Fri May 26 13:47:58 2023, max compression
```

## Comparing `megatron-lm-2.2.2.tar` & `megatron-lm-2.2.3.tar`

### file list

```diff
@@ -1,13 +1,11 @@
-drwxrwxr-x   0 ashish    (1000) ashish    (1000)        0 2023-04-28 15:01:53.000000 megatron-lm-2.2.2/
--rw-rw-r--   0 ashish    (1000) ashish    (1000)     1831 2023-04-28 15:01:44.000000 megatron-lm-2.2.2/setup.py
--rw-rw-r--   0 ashish    (1000) ashish    (1000)      568 2023-04-28 15:01:53.000000 megatron-lm-2.2.2/PKG-INFO
--rw-rw-r--   0 ashish    (1000) ashish    (1000)       38 2023-04-28 15:01:53.000000 megatron-lm-2.2.2/setup.cfg
-drwxrwxr-x   0 ashish    (1000) ashish    (1000)        0 2023-04-28 15:01:53.000000 megatron-lm-2.2.2/megatron/
--rw-rw-r--   0 ashish    (1000) ashish    (1000)       84 2023-04-28 14:51:16.000000 megatron-lm-2.2.2/megatron/__init__.py
-drwxrwxr-x   0 ashish    (1000) ashish    (1000)        0 2023-04-28 15:01:53.000000 megatron-lm-2.2.2/megatron_lm.egg-info/
--rw-rw-r--   0 ashish    (1000) ashish    (1000)      568 2023-04-28 15:01:53.000000 megatron-lm-2.2.2/megatron_lm.egg-info/PKG-INFO
--rw-rw-r--   0 ashish    (1000) ashish    (1000)        1 2023-04-28 15:01:53.000000 megatron-lm-2.2.2/megatron_lm.egg-info/dependency_links.txt
--rw-rw-r--   0 ashish    (1000) ashish    (1000)      187 2023-04-28 15:01:53.000000 megatron-lm-2.2.2/megatron_lm.egg-info/SOURCES.txt
--rw-rw-r--   0 ashish    (1000) ashish    (1000)        9 2023-04-28 15:01:53.000000 megatron-lm-2.2.2/megatron_lm.egg-info/top_level.txt
--rw-rw-r--   0 ashish    (1000) ashish    (1000)     1069 2023-04-27 21:19:14.000000 megatron-lm-2.2.2/LICENSE
--rw-rw-r--   0 ashish    (1000) ashish    (1000)       77 2023-04-27 21:40:11.000000 megatron-lm-2.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:47:58.224049 megatron-lm-2.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-26 13:47:45.000000 megatron-lm-2.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-26 13:47:58.224049 megatron-lm-2.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-26 13:47:45.000000 megatron-lm-2.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:47:58.224049 megatron-lm-2.2.3/megatron_lm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-26 13:47:58.000000 megatron-lm-2.2.3/megatron_lm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-26 13:47:58.000000 megatron-lm-2.2.3/megatron_lm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 13:47:58.000000 megatron-lm-2.2.3/megatron_lm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 13:47:58.000000 megatron-lm-2.2.3/megatron_lm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 13:47:58.224049 megatron-lm-2.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-26 13:47:45.000000 megatron-lm-2.2.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `megatron-lm-2.2.2/PKG-INFO` & `megatron-lm-2.2.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: megatron-lm
-Version: 2.2.2
-Summary: A placeholder package for megatron-lm
-Home-page: https://github.com/ashishbijlani/megatron-lm
+Version: 2.2.3
+Summary: A placeholder package
+Home-page: https://github.com/ashishbijlani/sample-pypi-package
 Author: Ashish Bijlani
-Author-email: ashish.bijlani@gmail.com
+Author-email: ab@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Placeholder package
 
-This is a placeholder for megatron-lm package v1.1.5 
+This is a placeholder package
```

### Comparing `megatron-lm-2.2.2/megatron_lm.egg-info/PKG-INFO` & `megatron-lm-2.2.3/megatron_lm.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: megatron-lm
-Version: 2.2.2
-Summary: A placeholder package for megatron-lm
-Home-page: https://github.com/ashishbijlani/megatron-lm
+Version: 2.2.3
+Summary: A placeholder package
+Home-page: https://github.com/ashishbijlani/sample-pypi-package
 Author: Ashish Bijlani
-Author-email: ashish.bijlani@gmail.com
+Author-email: ab@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Placeholder package
 
-This is a placeholder for megatron-lm package v1.1.5 
+This is a placeholder package
```

