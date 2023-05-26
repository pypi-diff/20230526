# Comparing `tmp/salesea-1.0.25.tar.gz` & `tmp/salesea-1.0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salesea-1.0.25.tar", last modified: Fri May 26 07:36:25 2023, max compression
+gzip compressed data, was "salesea-1.0.26.tar", last modified: Fri May 26 08:11:18 2023, max compression
```

## Comparing `salesea-1.0.25.tar` & `salesea-1.0.26.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 07:36:25.806797 salesea-1.0.25/
--rw-rw-rw-   0        0        0     2588 2023-05-26 07:36:25.807798 salesea-1.0.25/PKG-INFO
--rw-rw-rw-   0        0        0     1613 2023-05-22 09:08:17.000000 salesea-1.0.25/README.md
--rw-rw-rw-   0        0        0      111 2023-05-26 07:36:25.807798 salesea-1.0.25/setup.cfg
--rw-rw-rw-   0        0        0     2312 2023-05-26 07:36:21.000000 salesea-1.0.25/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-26 07:36:25.787797 salesea-1.0.25/src/
-drwxrwxrwx   0        0        0        0 2023-05-26 07:36:25.799802 salesea-1.0.25/src/salesea/
--rw-rw-rw-   0        0        0       25 2023-05-18 07:08:55.000000 salesea-1.0.25/src/salesea/__init__.py
--rw-rw-rw-   0        0        0     4545 2023-05-25 03:12:20.000000 salesea-1.0.25/src/salesea/__main__.py
--rw-rw-rw-   0        0        0     7629 2023-05-26 05:18:58.000000 salesea-1.0.25/src/salesea/app.py
--rw-rw-rw-   0        0        0     3746 2023-05-24 08:02:59.000000 salesea-1.0.25/src/salesea/config.py
--rw-rw-rw-   0        0        0     1214 2023-05-22 05:27:18.000000 salesea-1.0.25/src/salesea/log.py
--rw-rw-rw-   0        0        0    22869 2023-05-26 07:36:04.000000 salesea-1.0.25/src/salesea/nginx.py
--rw-rw-rw-   0        0        0      970 2023-05-24 10:13:19.000000 salesea-1.0.25/src/salesea/solution.py
--rw-rw-rw-   0        0        0      134 2023-05-18 07:39:33.000000 salesea-1.0.25/src/salesea/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-26 07:36:25.805799 salesea-1.0.25/src/salesea.egg-info/
--rw-rw-rw-   0        0        0     2588 2023-05-26 07:36:25.000000 salesea-1.0.25/src/salesea.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      414 2023-05-26 07:36:25.000000 salesea-1.0.25/src/salesea.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 07:36:25.000000 salesea-1.0.25/src/salesea.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-26 07:36:25.000000 salesea-1.0.25/src/salesea.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-05-26 07:36:25.000000 salesea-1.0.25/src/salesea.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-26 07:36:25.000000 salesea-1.0.25/src/salesea.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-26 08:11:18.455524 salesea-1.0.26/
+-rw-rw-rw-   0        0        0     2588 2023-05-26 08:11:18.456524 salesea-1.0.26/PKG-INFO
+-rw-rw-rw-   0        0        0     1613 2023-05-22 09:08:17.000000 salesea-1.0.26/README.md
+-rw-rw-rw-   0        0        0      111 2023-05-26 08:11:18.456524 salesea-1.0.26/setup.cfg
+-rw-rw-rw-   0        0        0     2312 2023-05-26 08:11:05.000000 salesea-1.0.26/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 08:11:18.436524 salesea-1.0.26/src/
+drwxrwxrwx   0        0        0        0 2023-05-26 08:11:18.448524 salesea-1.0.26/src/salesea/
+-rw-rw-rw-   0        0        0       25 2023-05-18 07:08:55.000000 salesea-1.0.26/src/salesea/__init__.py
+-rw-rw-rw-   0        0        0     4545 2023-05-25 03:12:20.000000 salesea-1.0.26/src/salesea/__main__.py
+-rw-rw-rw-   0        0        0     7629 2023-05-26 05:18:58.000000 salesea-1.0.26/src/salesea/app.py
+-rw-rw-rw-   0        0        0     3746 2023-05-24 08:02:59.000000 salesea-1.0.26/src/salesea/config.py
+-rw-rw-rw-   0        0        0     1214 2023-05-22 05:27:18.000000 salesea-1.0.26/src/salesea/log.py
+-rw-rw-rw-   0        0        0    23008 2023-05-26 08:09:29.000000 salesea-1.0.26/src/salesea/nginx.py
+-rw-rw-rw-   0        0        0      970 2023-05-24 10:13:19.000000 salesea-1.0.26/src/salesea/solution.py
+-rw-rw-rw-   0        0        0      134 2023-05-18 07:39:33.000000 salesea-1.0.26/src/salesea/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-26 08:11:18.454554 salesea-1.0.26/src/salesea.egg-info/
+-rw-rw-rw-   0        0        0     2588 2023-05-26 08:11:18.000000 salesea-1.0.26/src/salesea.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      414 2023-05-26 08:11:18.000000 salesea-1.0.26/src/salesea.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 08:11:18.000000 salesea-1.0.26/src/salesea.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-26 08:11:18.000000 salesea-1.0.26/src/salesea.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-05-26 08:11:18.000000 salesea-1.0.26/src/salesea.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-26 08:11:18.000000 salesea-1.0.26/src/salesea.egg-info/top_level.txt
```

### Comparing `salesea-1.0.25/PKG-INFO` & `salesea-1.0.26/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salesea
-Version: 1.0.25
+Version: 1.0.26
 Summary: This is an Nginx log collection tool.
 Author: howard
 Author-email: 18071131140telephone@gmail.com
 Keywords: nginx,logs,collection
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.0
```

### Comparing `salesea-1.0.25/README.md` & `salesea-1.0.26/README.md`

 * *Files identical despite different names*

### Comparing `salesea-1.0.25/setup.py` & `salesea-1.0.26/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #     print(requires.splitlines())
 # ------------------------------------------------------------------------------- #
 
 setup(
     name='salesea',
     author='howard',
     author_email='18071131140telephone@gmail.com',
-    version='1.0.25',
+    version='1.0.26',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     description='This is an Nginx log collection tool.',
     long_description=readme,
     long_description_content_type='text/markdown',
     keywords=[
         'nginx',
```

### Comparing `salesea-1.0.25/src/salesea/__main__.py` & `salesea-1.0.26/src/salesea/__main__.py`

 * *Files identical despite different names*

### Comparing `salesea-1.0.25/src/salesea/app.py` & `salesea-1.0.26/src/salesea/app.py`

 * *Files identical despite different names*

### Comparing `salesea-1.0.25/src/salesea/config.py` & `salesea-1.0.26/src/salesea/config.py`

 * *Files identical despite different names*

### Comparing `salesea-1.0.25/src/salesea/log.py` & `salesea-1.0.26/src/salesea/log.py`

 * *Files identical despite different names*

### Comparing `salesea-1.0.25/src/salesea/nginx.py` & `salesea-1.0.26/src/salesea/nginx.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,18 @@
     def include_salesea(self, api_key):
         logger.debug(f"检查[{self.names[0]}]服务是否包含[salesea.conf]")
         global_flag = 0
 
         self.salesea_conf_dir.mkdir(parents=True, exist_ok=True)
         salesea_conf = f'access_log {self.log_path} salesea;\n\n'
         salesea_conf += 'if ($uri = /salesea) {\n'
-        # salesea_conf += '    add_header Content-Type text/plain;\n'
+        salesea_conf += '    rewrite ^(.*)$ $1 last;\n'
+        salesea_conf += '}\n\n'
+        salesea_conf += 'location = /salesea {\n'
+        salesea_conf += '    add_header Content-Type text/plain;\n'
         salesea_conf += f'    return 200 "{api_key}";\n'
         salesea_conf += '}'
 
         if self.read_config() != salesea_conf:
             global_flag = 1
             self.write_config(salesea_conf)
```

### Comparing `salesea-1.0.25/src/salesea/solution.py` & `salesea-1.0.26/src/salesea/solution.py`

 * *Files identical despite different names*

### Comparing `salesea-1.0.25/src/salesea.egg-info/PKG-INFO` & `salesea-1.0.26/src/salesea.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salesea
-Version: 1.0.25
+Version: 1.0.26
 Summary: This is an Nginx log collection tool.
 Author: howard
 Author-email: 18071131140telephone@gmail.com
 Keywords: nginx,logs,collection
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.0
```

