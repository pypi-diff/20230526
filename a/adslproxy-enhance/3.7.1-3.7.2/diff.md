# Comparing `tmp/adslproxy-enhance-3.7.1.tar.gz` & `tmp/adslproxy-enhance-3.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adslproxy-enhance-3.7.1.tar", last modified: Thu May 25 14:43:37 2023, max compression
+gzip compressed data, was "adslproxy-enhance-3.7.2.tar", last modified: Fri May 26 02:20:17 2023, max compression
```

## Comparing `adslproxy-enhance-3.7.1.tar` & `adslproxy-enhance-3.7.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 andylee    (501) staff       (20)        0 2023-05-25 14:43:37.795725 adslproxy-enhance-3.7.1/
--rw-r--r--   0 andylee    (501) staff       (20)     1076 2023-05-25 13:52:29.000000 adslproxy-enhance-3.7.1/LICENSE
--rw-r--r--   0 andylee    (501) staff       (20)     3142 2023-05-25 14:43:37.794508 adslproxy-enhance-3.7.1/PKG-INFO
--rw-r--r--   0 andylee    (501) staff       (20)     2501 2023-05-25 13:52:29.000000 adslproxy-enhance-3.7.1/README.md
-drwxr-xr-x   0 andylee    (501) staff       (20)        0 2023-05-25 14:43:37.789537 adslproxy-enhance-3.7.1/adslproxy/
--rw-r--r--   0 andylee    (501) staff       (20)      165 2023-05-25 13:52:29.000000 adslproxy-enhance-3.7.1/adslproxy/__init__.py
--rw-r--r--   0 andylee    (501) staff       (20)       94 2023-05-25 14:34:56.000000 adslproxy-enhance-3.7.1/adslproxy/__version__.py
-drwxr-xr-x   0 andylee    (501) staff       (20)        0 2023-05-25 14:43:37.790124 adslproxy-enhance-3.7.1/adslproxy/checker/
--rw-r--r--   0 andylee    (501) staff       (20)        0 2023-05-25 13:52:29.000000 adslproxy-enhance-3.7.1/adslproxy/checker/__init__.py
--rw-r--r--   0 andylee    (501) staff       (20)     2141 2023-05-25 13:52:29.000000 adslproxy-enhance-3.7.1/adslproxy/checker/checker.py
--rw-r--r--   0 andylee    (501) staff       (20)     3871 2023-05-25 13:52:29.000000 adslproxy-enhance-3.7.1/adslproxy/cmd.py
--rw-r--r--   0 andylee    (501) staff       (20)     2229 2023-05-25 13:52:29.000000 adslproxy-enhance-3.7.1/adslproxy/db.py
-drwxr-xr-x   0 andylee    (501) staff       (20)        0 2023-05-25 14:43:37.790689 adslproxy-enhance-3.7.1/adslproxy/sender/
--rw-r--r--   0 andylee    (501) staff       (20)        0 2023-05-25 13:52:29.000000 adslproxy-enhance-3.7.1/adslproxy/sender/__init__.py
--rw-r--r--   0 andylee    (501) staff       (20)     4990 2023-05-25 14:20:09.000000 adslproxy-enhance-3.7.1/adslproxy/sender/sender.py
-drwxr-xr-x   0 andylee    (501) staff       (20)        0 2023-05-25 14:43:37.791627 adslproxy-enhance-3.7.1/adslproxy/server/
--rw-r--r--   0 andylee    (501) staff       (20)        0 2023-05-25 13:52:29.000000 adslproxy-enhance-3.7.1/adslproxy/server/__init__.py
--rw-r--r--   0 andylee    (501) staff       (20)     1981 2023-05-25 13:52:29.000000 adslproxy-enhance-3.7.1/adslproxy/server/server.py
--rw-r--r--   0 andylee    (501) staff       (20)     1303 2023-05-25 13:56:44.000000 adslproxy-enhance-3.7.1/adslproxy/settings.py
-drwxr-xr-x   0 andylee    (501) staff       (20)        0 2023-05-25 14:43:37.793765 adslproxy-enhance-3.7.1/adslproxy_enhance.egg-info/
--rw-r--r--   0 andylee    (501) staff       (20)     3142 2023-05-25 14:43:37.000000 adslproxy-enhance-3.7.1/adslproxy_enhance.egg-info/PKG-INFO
--rw-r--r--   0 andylee    (501) staff       (20)      547 2023-05-25 14:43:37.000000 adslproxy-enhance-3.7.1/adslproxy_enhance.egg-info/SOURCES.txt
--rw-r--r--   0 andylee    (501) staff       (20)        1 2023-05-25 14:43:37.000000 adslproxy-enhance-3.7.1/adslproxy_enhance.egg-info/dependency_links.txt
--rw-r--r--   0 andylee    (501) staff       (20)       48 2023-05-25 14:43:37.000000 adslproxy-enhance-3.7.1/adslproxy_enhance.egg-info/entry_points.txt
--rw-r--r--   0 andylee    (501) staff       (20)       47 2023-05-25 14:43:37.000000 adslproxy-enhance-3.7.1/adslproxy_enhance.egg-info/requires.txt
--rw-r--r--   0 andylee    (501) staff       (20)       10 2023-05-25 14:43:37.000000 adslproxy-enhance-3.7.1/adslproxy_enhance.egg-info/top_level.txt
--rw-r--r--   0 andylee    (501) staff       (20)       38 2023-05-25 14:43:37.796218 adslproxy-enhance-3.7.1/setup.cfg
--rw-r--r--   0 andylee    (501) staff       (20)     3338 2023-05-25 14:43:35.000000 adslproxy-enhance-3.7.1/setup.py
+drwxr-xr-x   0 andylee    (501) staff       (20)        0 2023-05-26 02:20:17.484336 adslproxy-enhance-3.7.2/
+-rw-r--r--   0 andylee    (501) staff       (20)     1076 2023-05-25 13:52:29.000000 adslproxy-enhance-3.7.2/LICENSE
+-rw-r--r--   0 andylee    (501) staff       (20)     3142 2023-05-26 02:20:17.484015 adslproxy-enhance-3.7.2/PKG-INFO
+-rw-r--r--   0 andylee    (501) staff       (20)     2501 2023-05-25 13:52:29.000000 adslproxy-enhance-3.7.2/README.md
+drwxr-xr-x   0 andylee    (501) staff       (20)        0 2023-05-26 02:20:17.471512 adslproxy-enhance-3.7.2/adslproxy/
+-rw-r--r--   0 andylee    (501) staff       (20)      165 2023-05-25 13:52:29.000000 adslproxy-enhance-3.7.2/adslproxy/__init__.py
+-rw-r--r--   0 andylee    (501) staff       (20)       94 2023-05-26 02:20:16.000000 adslproxy-enhance-3.7.2/adslproxy/__version__.py
+drwxr-xr-x   0 andylee    (501) staff       (20)        0 2023-05-26 02:20:17.472846 adslproxy-enhance-3.7.2/adslproxy/checker/
+-rw-r--r--   0 andylee    (501) staff       (20)        0 2023-05-25 13:52:29.000000 adslproxy-enhance-3.7.2/adslproxy/checker/__init__.py
+-rw-r--r--   0 andylee    (501) staff       (20)     2141 2023-05-25 13:52:29.000000 adslproxy-enhance-3.7.2/adslproxy/checker/checker.py
+-rw-r--r--   0 andylee    (501) staff       (20)     3871 2023-05-25 13:52:29.000000 adslproxy-enhance-3.7.2/adslproxy/cmd.py
+-rw-r--r--   0 andylee    (501) staff       (20)     2229 2023-05-25 13:52:29.000000 adslproxy-enhance-3.7.2/adslproxy/db.py
+drwxr-xr-x   0 andylee    (501) staff       (20)        0 2023-05-26 02:20:17.474185 adslproxy-enhance-3.7.2/adslproxy/sender/
+-rw-r--r--   0 andylee    (501) staff       (20)        0 2023-05-25 13:52:29.000000 adslproxy-enhance-3.7.2/adslproxy/sender/__init__.py
+-rw-r--r--   0 andylee    (501) staff       (20)     5028 2023-05-26 02:19:53.000000 adslproxy-enhance-3.7.2/adslproxy/sender/sender.py
+drwxr-xr-x   0 andylee    (501) staff       (20)        0 2023-05-26 02:20:17.475201 adslproxy-enhance-3.7.2/adslproxy/server/
+-rw-r--r--   0 andylee    (501) staff       (20)        0 2023-05-25 13:52:29.000000 adslproxy-enhance-3.7.2/adslproxy/server/__init__.py
+-rw-r--r--   0 andylee    (501) staff       (20)     1981 2023-05-25 13:52:29.000000 adslproxy-enhance-3.7.2/adslproxy/server/server.py
+-rw-r--r--   0 andylee    (501) staff       (20)     1311 2023-05-26 02:19:42.000000 adslproxy-enhance-3.7.2/adslproxy/settings.py
+drwxr-xr-x   0 andylee    (501) staff       (20)        0 2023-05-26 02:20:17.483398 adslproxy-enhance-3.7.2/adslproxy_enhance.egg-info/
+-rw-r--r--   0 andylee    (501) staff       (20)     3142 2023-05-26 02:20:17.000000 adslproxy-enhance-3.7.2/adslproxy_enhance.egg-info/PKG-INFO
+-rw-r--r--   0 andylee    (501) staff       (20)      547 2023-05-26 02:20:17.000000 adslproxy-enhance-3.7.2/adslproxy_enhance.egg-info/SOURCES.txt
+-rw-r--r--   0 andylee    (501) staff       (20)        1 2023-05-26 02:20:17.000000 adslproxy-enhance-3.7.2/adslproxy_enhance.egg-info/dependency_links.txt
+-rw-r--r--   0 andylee    (501) staff       (20)       48 2023-05-26 02:20:17.000000 adslproxy-enhance-3.7.2/adslproxy_enhance.egg-info/entry_points.txt
+-rw-r--r--   0 andylee    (501) staff       (20)       47 2023-05-26 02:20:17.000000 adslproxy-enhance-3.7.2/adslproxy_enhance.egg-info/requires.txt
+-rw-r--r--   0 andylee    (501) staff       (20)       10 2023-05-26 02:20:17.000000 adslproxy-enhance-3.7.2/adslproxy_enhance.egg-info/top_level.txt
+-rw-r--r--   0 andylee    (501) staff       (20)       38 2023-05-26 02:20:17.484421 adslproxy-enhance-3.7.2/setup.cfg
+-rw-r--r--   0 andylee    (501) staff       (20)     3338 2023-05-25 14:43:35.000000 adslproxy-enhance-3.7.2/setup.py
```

### Comparing `adslproxy-enhance-3.7.1/LICENSE` & `adslproxy-enhance-3.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `adslproxy-enhance-3.7.1/PKG-INFO` & `adslproxy-enhance-3.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adslproxy-enhance
-Version: 3.7.1
+Version: 3.7.2
 Summary: ADSL Proxy Pool Tool 
 Home-page: https://github.com/thefantasystudio/AdslProxy
 Author: Germey
 Author-email: cqc@cuiqingcai.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `adslproxy-enhance-3.7.1/README.md` & `adslproxy-enhance-3.7.2/README.md`

 * *Files identical despite different names*

### Comparing `adslproxy-enhance-3.7.1/adslproxy/checker/checker.py` & `adslproxy-enhance-3.7.2/adslproxy/checker/checker.py`

 * *Files identical despite different names*

### Comparing `adslproxy-enhance-3.7.1/adslproxy/cmd.py` & `adslproxy-enhance-3.7.2/adslproxy/cmd.py`

 * *Files identical despite different names*

### Comparing `adslproxy-enhance-3.7.1/adslproxy/db.py` & `adslproxy-enhance-3.7.2/adslproxy/db.py`

 * *Files identical despite different names*

### Comparing `adslproxy-enhance-3.7.1/adslproxy/sender/sender.py` & `adslproxy-enhance-3.7.2/adslproxy/sender/sender.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         """
         logger.info(f'Removing {CLIENT_NAME}...')
         try:
             payload = {
                 'client_name': CLIENT_NAME
             }
 
-            qs = generate_url_signature(payload)
+            qs = generate_url_signature(payload, API_SIGNATURE_KEY)
 
             url = f"{API_URL}/remove?{qs}"
             res = requests.get(url)
             if res.ok:
                 logger.info(f'Result is {res.text} Removed {CLIENT_NAME} successfully')
                 logger.info(f'Removed {CLIENT_NAME} successfully')
                 return True
@@ -96,15 +96,15 @@
         :return: None
         """
         payload = {
             'client_name': CLIENT_NAME,
             'client_ip': proxy
         }
 
-        qs = generate_url_signature(payload)
+        qs = generate_url_signature(payload, API_SIGNATURE_KEY)
         url = f"{API_URL}/update?{qs}"
         res = requests.get(url)
         if res.ok:
             logger.info(f'Result is {res.text} Set {CLIENT_NAME} successfully')
             return True
         else:
             logger.info(f'Result is {res.text} Removed {CLIENT_NAME} failed')
```

### Comparing `adslproxy-enhance-3.7.1/adslproxy/server/server.py` & `adslproxy-enhance-3.7.2/adslproxy/server/server.py`

 * *Files identical despite different names*

### Comparing `adslproxy-enhance-3.7.1/adslproxy/settings.py` & `adslproxy-enhance-3.7.2/adslproxy/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,8 +38,8 @@
 SERVER_HOST = env.str('SERVER_HOST', '0.0.0.0')
 
 # 代理端口
 PROXY_PORT = env.int('PROXY_PORT', 3128)
 PROXY_USERNAME = env.str('PROXY_USERNAME', '')
 PROXY_PASSWORD = env.str('PROXY_PASSWORD', '')
 API_URL = env.str('API_URL', '')
-API_SIGNATURE = env.str('API_SIGNATURE', '')
+API_SIGNATURE_KEY = env.str('API_SIGNATURE_KEY', '')
```

### Comparing `adslproxy-enhance-3.7.1/adslproxy_enhance.egg-info/PKG-INFO` & `adslproxy-enhance-3.7.2/adslproxy_enhance.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adslproxy-enhance
-Version: 3.7.1
+Version: 3.7.2
 Summary: ADSL Proxy Pool Tool 
 Home-page: https://github.com/thefantasystudio/AdslProxy
 Author: Germey
 Author-email: cqc@cuiqingcai.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `adslproxy-enhance-3.7.1/adslproxy_enhance.egg-info/SOURCES.txt` & `adslproxy-enhance-3.7.2/adslproxy_enhance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adslproxy-enhance-3.7.1/setup.py` & `adslproxy-enhance-3.7.2/setup.py`

 * *Files identical despite different names*

