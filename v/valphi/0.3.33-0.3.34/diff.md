# Comparing `tmp/valphi-0.3.33.tar.gz` & `tmp/valphi-0.3.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valphi-0.3.33.tar", max compression
+gzip compressed data, was "valphi-0.3.34.tar", max compression
```

## Comparing `valphi-0.3.33.tar` & `valphi-0.3.34.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1070 2022-09-22 13:08:25.021598 valphi-0.3.33/LICENSE
--rw-r--r--   0        0        0      445 2023-02-17 13:45:47.123135 valphi-0.3.33/pyproject.toml
--rw-r--r--   0        0        0        0 2022-09-22 13:13:37.919365 valphi-0.3.33/valphi/__init__.py
--rwxr-xr-x   0        0        0       97 2022-09-22 16:30:02.808202 valphi-0.3.33/valphi/__main__.py
--rw-r--r--   0        0        0     7742 2023-01-20 13:32:27.686186 valphi-0.3.33/valphi/cli.py
--rw-r--r--   0        0        0     2266 2023-01-17 17:02:20.445653 valphi-0.3.33/valphi/contexts.py
--rw-r--r--   0        0        0    17029 2023-01-19 09:06:20.915594 valphi-0.3.33/valphi/controllers.py
--rw-r--r--   0        0        0     1899 2023-01-17 17:07:21.715958 valphi-0.3.33/valphi/models.py
--rw-r--r--   0        0        0    14909 2023-01-17 17:02:20.461653 valphi-0.3.33/valphi/networks.py
--rw-r--r--   0        0        0     5570 2023-01-17 17:02:20.453652 valphi-0.3.33/valphi/propagators.py
--rw-r--r--   0        0        0      102 2023-01-13 07:23:53.009969 valphi-0.3.33/valphi/utils.py
--rw-r--r--   0        0        0      718 1970-01-01 00:00:00.000000 valphi-0.3.33/setup.py
--rw-r--r--   0        0        0      503 1970-01-01 00:00:00.000000 valphi-0.3.33/PKG-INFO
+-rw-r--r--   0        0        0     1070 2022-09-22 13:08:25.021598 valphi-0.3.34/LICENSE
+-rw-r--r--   0        0        0      427 2023-05-26 18:18:04.224918 valphi-0.3.34/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-09-22 13:13:37.919365 valphi-0.3.34/valphi/__init__.py
+-rwxr-xr-x   0        0        0       97 2022-09-22 16:30:02.808202 valphi-0.3.34/valphi/__main__.py
+-rw-r--r--   0        0        0    10620 2023-05-26 18:14:44.616560 valphi-0.3.34/valphi/cli.py
+-rw-r--r--   0        0        0     2266 2023-01-17 17:02:20.445653 valphi-0.3.34/valphi/contexts.py
+-rw-r--r--   0        0        0    17029 2023-01-19 09:06:20.915594 valphi-0.3.34/valphi/controllers.py
+-rw-r--r--   0        0        0     1899 2023-01-17 17:07:21.715958 valphi-0.3.34/valphi/models.py
+-rw-r--r--   0        0        0    14909 2023-01-17 17:02:20.461653 valphi-0.3.34/valphi/networks.py
+-rw-r--r--   0        0        0     5570 2023-01-17 17:02:20.453652 valphi-0.3.34/valphi/propagators.py
+-rw-r--r--   0        0        0      102 2023-01-13 07:23:53.009969 valphi-0.3.34/valphi/utils.py
+-rw-r--r--   0        0        0      691 1970-01-01 00:00:00.000000 valphi-0.3.34/setup.py
+-rw-r--r--   0        0        0      464 1970-01-01 00:00:00.000000 valphi-0.3.34/PKG-INFO
```

### Comparing `valphi-0.3.33/LICENSE` & `valphi-0.3.34/LICENSE`

 * *Files identical despite different names*

### Comparing `valphi-0.3.33/valphi/contexts.py` & `valphi-0.3.34/valphi/contexts.py`

 * *Files identical despite different names*

### Comparing `valphi-0.3.33/valphi/controllers.py` & `valphi-0.3.34/valphi/controllers.py`

 * *Files identical despite different names*

### Comparing `valphi-0.3.33/valphi/models.py` & `valphi-0.3.34/valphi/models.py`

 * *Files identical despite different names*

### Comparing `valphi-0.3.33/valphi/networks.py` & `valphi-0.3.34/valphi/networks.py`

 * *Files identical despite different names*

### Comparing `valphi-0.3.33/valphi/propagators.py` & `valphi-0.3.34/valphi/propagators.py`

 * *Files identical despite different names*

### Comparing `valphi-0.3.33/setup.py` & `valphi-0.3.34/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,22 +4,19 @@
 packages = \
 ['valphi']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['clingo>=5.6.2,<6.0.0',
- 'distlib>=0.3.6,<0.4.0',
- 'dumbo-asp>=0.0.19,<0.0.20',
- 'pydot>=1.4.2,<2.0.0']
+['distlib>=0.3.6,<0.4.0', 'dumbo-asp>=0.0.37,<0.0.38', 'pydot>=1.4.2,<2.0.0']
 
 setup_kwargs = {
     'name': 'valphi',
-    'version': '0.3.33',
+    'version': '0.3.34',
     'description': 'Logic programs ralying on ValPhi semantics',
     'long_description': 'None',
     'author': 'Mario Alviano',
     'author_email': 'mario.alviano@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

