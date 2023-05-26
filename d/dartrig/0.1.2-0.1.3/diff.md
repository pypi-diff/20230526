# Comparing `tmp/dartrig-0.1.2.tar.gz` & `tmp/dartrig-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dartrig-0.1.2.tar", last modified: Fri May 26 04:34:11 2023, max compression
+gzip compressed data, was "dist/dartrig-0.1.3.tar", last modified: Fri May 26 05:28:23 2023, max compression
```

## Comparing `dartrig-0.1.2.tar` & `dartrig-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-26 04:34:11.000000 dartrig-0.1.2/
--rw-r--r--   0 nezah      (501) staff       (20)     1485 2023-05-26 04:34:11.000000 dartrig-0.1.2/PKG-INFO
--rw-r--r--   0 nezah      (501) staff       (20)     1081 2023-03-17 05:39:07.000000 dartrig-0.1.2/LICENSE
--rw-r--r--   0 nezah      (501) staff       (20)     1061 2023-04-11 08:24:52.000000 dartrig-0.1.2/README.md
--rw-r--r--   0 nezah      (501) staff       (20)      693 2023-05-26 04:34:10.000000 dartrig-0.1.2/setup.py
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-26 04:34:11.000000 dartrig-0.1.2/dartrig/
--rw-r--r--   0 nezah      (501) staff       (20)    13097 2023-05-25 14:35:10.000000 dartrig-0.1.2/dartrig/__init__.py
--rw-r--r--   0 nezah      (501) staff       (20)      682 2023-03-18 12:39:55.000000 dartrig-0.1.2/dartrig/annotations.py
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-26 04:34:11.000000 dartrig-0.1.2/dartrig.egg-info/
--rw-r--r--   0 nezah      (501) staff       (20)     1485 2023-05-26 04:34:11.000000 dartrig-0.1.2/dartrig.egg-info/PKG-INFO
--rw-r--r--   0 nezah      (501) staff       (20)      223 2023-05-26 04:34:11.000000 dartrig-0.1.2/dartrig.egg-info/SOURCES.txt
--rw-r--r--   0 nezah      (501) staff       (20)       31 2023-05-26 04:34:11.000000 dartrig-0.1.2/dartrig.egg-info/requires.txt
--rw-r--r--   0 nezah      (501) staff       (20)        8 2023-05-26 04:34:11.000000 dartrig-0.1.2/dartrig.egg-info/top_level.txt
--rw-r--r--   0 nezah      (501) staff       (20)        1 2023-05-26 04:34:11.000000 dartrig-0.1.2/dartrig.egg-info/dependency_links.txt
--rw-r--r--   0 nezah      (501) staff       (20)       38 2023-05-26 04:34:11.000000 dartrig-0.1.2/setup.cfg
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-26 05:28:23.000000 dartrig-0.1.3/
+-rw-r--r--   0 nezah      (501) staff       (20)     1485 2023-05-26 05:28:23.000000 dartrig-0.1.3/PKG-INFO
+-rw-r--r--   0 nezah      (501) staff       (20)     1081 2023-03-17 05:39:07.000000 dartrig-0.1.3/LICENSE
+-rw-r--r--   0 nezah      (501) staff       (20)     1061 2023-04-11 08:24:52.000000 dartrig-0.1.3/README.md
+-rw-r--r--   0 nezah      (501) staff       (20)      693 2023-05-26 05:28:22.000000 dartrig-0.1.3/setup.py
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-26 05:28:23.000000 dartrig-0.1.3/dartrig/
+-rw-r--r--   0 nezah      (501) staff       (20)    13644 2023-05-26 05:25:15.000000 dartrig-0.1.3/dartrig/__init__.py
+-rw-r--r--   0 nezah      (501) staff       (20)      682 2023-03-18 12:39:55.000000 dartrig-0.1.3/dartrig/annotations.py
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-26 05:28:23.000000 dartrig-0.1.3/dartrig.egg-info/
+-rw-r--r--   0 nezah      (501) staff       (20)     1485 2023-05-26 05:28:23.000000 dartrig-0.1.3/dartrig.egg-info/PKG-INFO
+-rw-r--r--   0 nezah      (501) staff       (20)      223 2023-05-26 05:28:23.000000 dartrig-0.1.3/dartrig.egg-info/SOURCES.txt
+-rw-r--r--   0 nezah      (501) staff       (20)       31 2023-05-26 05:28:23.000000 dartrig-0.1.3/dartrig.egg-info/requires.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        8 2023-05-26 05:28:23.000000 dartrig-0.1.3/dartrig.egg-info/top_level.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        1 2023-05-26 05:28:23.000000 dartrig-0.1.3/dartrig.egg-info/dependency_links.txt
+-rw-r--r--   0 nezah      (501) staff       (20)       38 2023-05-26 05:28:23.000000 dartrig-0.1.3/setup.cfg
```

### Comparing `dartrig-0.1.2/PKG-INFO` & `dartrig-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dartrig
-Version: 0.1.2
+Version: 0.1.3
 Summary: dartrig api wrapper
 Home-page: https://github.com/cheddars/dart_rigger
 Author: cheddars
 Author-email: nezahrish@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dartrig-0.1.2/LICENSE` & `dartrig-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dartrig-0.1.2/README.md` & `dartrig-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `dartrig-0.1.2/setup.py` & `dartrig-0.1.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="dartrig",
-    version="0.1.2",
+    version="0.1.3",
     install_requires=[
         'requests',
         'bs4',
         'adt_cache==0.0.11'
     ],
     license='MIT',
     author="cheddars",
```

### Comparing `dartrig-0.1.2/dartrig/__init__.py` & `dartrig-0.1.3/dartrig/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,34 +44,45 @@
         :param ele_id:
         :param offset:
         :return:
         """
         dcm_no = self._get_dcm_no_by_rcp_no(rcp_no)
         return self._request_detail_with_dcm(rcp_no, dtd, dcm_no, ele_id, offset)
 
-    def _try_file_cache_request(self, url, prefix, file_cache_key):
+    def _try_file_cache_request(self, url, prefix, file_cache_key, ext="html"):
         if self.file_cache is not None:
-            cached = self.file_cache.get_file(prefix=prefix, key=file_cache_key, ext="html")
+            cached = self.file_cache.get_file(prefix=prefix, key=file_cache_key, ext=ext)
             if cached is not None:
                 self.logger.debug(f"file cache hit for key {file_cache_key}")
                 return cached
 
-        text = self.session.get(url, headers=HEADERS).text
+        response = self.session.get(url, headers=HEADERS)
+        self.logger.info(response.headers)
+        content_type = response.headers["Content-Type"]
+        if content_type is not None and "MS949" in content_type.upper():
+            self.logger.debug(f"response encoding is MS949. change to utf-8")
+            response.encoding = "ms949"
+            text = response.text
+        else:
+            text = response.text
+
+        # self.logger.debug(f"_try_file_cache_request response text : {text}")
 
         if self.file_cache is not None:
-            self.file_cache.save_file(prefix=prefix, key=file_cache_key, ext="html", data=text)
+            self.file_cache.save_file(prefix=prefix, key=file_cache_key, ext=ext, data=text)
             self.logger.debug(f"file cache set for key {file_cache_key}")
         return text
 
     def _request_detail_with_dcm(self, rcp_no, dtd, dcm_no, ele_id=0, offset=0):
-        file_cache_key = f"{rcp_no}_{dcm_no}_{dtd}_{ele_id}_{offset}"
+        dtd_split = dtd.split(".")[0]
+        file_cache_key = f"{rcp_no}_{dcm_no}_{dtd_split}_{ele_id}_{offset}"
 
         url = f"{URLS['DART_VIEWER']}?rcpNo={rcp_no}&dcmNo={dcm_no}&eleId={ele_id}&offset={offset}&length=0&dtd={dtd}"
         self.logger.info(f"request_detail_with_dcm url : {url}")
-        return self._try_file_cache_request(url, "viewer", file_cache_key)
+        return self._try_file_cache_request(url, "viewer", file_cache_key, ext="html" if dtd.lower() == "html" else "xml")
 
     def _get_dcm_no_by_rcp_no(self, rcp_no):
         cache_key = f"dcm_no_{rcp_no}"
         try:
             if self.cache is not None:
                 cached = self.cache.get(cache_key)
                 if cached is not None:
```

### Comparing `dartrig-0.1.2/dartrig/annotations.py` & `dartrig-0.1.3/dartrig/annotations.py`

 * *Files identical despite different names*

### Comparing `dartrig-0.1.2/dartrig.egg-info/PKG-INFO` & `dartrig-0.1.3/dartrig.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dartrig
-Version: 0.1.2
+Version: 0.1.3
 Summary: dartrig api wrapper
 Home-page: https://github.com/cheddars/dart_rigger
 Author: cheddars
 Author-email: nezahrish@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

