# Comparing `tmp/tldrwl-1.0.0.tar.gz` & `tmp/tldrwl-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tldrwl-1.0.0.tar", last modified: Thu May 25 03:34:46 2023, max compression
+gzip compressed data, was "tldrwl-1.0.1.tar", last modified: Fri May 26 03:01:27 2023, max compression
```

## Comparing `tldrwl-1.0.0.tar` & `tldrwl-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:34:46.063610 tldrwl-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-25 03:34:30.000000 tldrwl-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16752 2023-05-25 03:34:46.063610 tldrwl-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16499 2023-05-25 03:34:30.000000 tldrwl-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-25 03:34:30.000000 tldrwl-1.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 03:34:46.063610 tldrwl-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-25 03:34:30.000000 tldrwl-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:34:46.059610 tldrwl-1.0.0/tldrwl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 03:34:30.000000 tldrwl-1.0.0/tldrwl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-25 03:34:30.000000 tldrwl-1.0.0/tldrwl/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-25 03:34:30.000000 tldrwl-1.0.0/tldrwl/ai_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-25 03:34:30.000000 tldrwl-1.0.0/tldrwl/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-25 03:34:30.000000 tldrwl-1.0.0/tldrwl/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-25 03:34:30.000000 tldrwl-1.0.0/tldrwl/register.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-25 03:34:30.000000 tldrwl-1.0.0/tldrwl/summarize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-05-25 03:34:30.000000 tldrwl-1.0.0/tldrwl/summarize_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-05-25 03:34:30.000000 tldrwl-1.0.0/tldrwl/summarize_webpage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-05-25 03:34:30.000000 tldrwl-1.0.0/tldrwl/summarize_youtube.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:34:46.059610 tldrwl-1.0.0/tldrwl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16752 2023-05-25 03:34:46.000000 tldrwl-1.0.0/tldrwl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-25 03:34:46.000000 tldrwl-1.0.0/tldrwl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 03:34:46.000000 tldrwl-1.0.0/tldrwl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-25 03:34:46.000000 tldrwl-1.0.0/tldrwl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-25 03:34:46.000000 tldrwl-1.0.0/tldrwl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:01:27.482098 tldrwl-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-26 03:01:14.000000 tldrwl-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16752 2023-05-26 03:01:27.482098 tldrwl-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16499 2023-05-26 03:01:14.000000 tldrwl-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-26 03:01:14.000000 tldrwl-1.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 03:01:27.482098 tldrwl-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-26 03:01:14.000000 tldrwl-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:01:27.482098 tldrwl-1.0.1/tldrwl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 03:01:14.000000 tldrwl-1.0.1/tldrwl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-26 03:01:14.000000 tldrwl-1.0.1/tldrwl/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-26 03:01:14.000000 tldrwl-1.0.1/tldrwl/ai_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-26 03:01:14.000000 tldrwl-1.0.1/tldrwl/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-26 03:01:14.000000 tldrwl-1.0.1/tldrwl/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-26 03:01:14.000000 tldrwl-1.0.1/tldrwl/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-26 03:01:14.000000 tldrwl-1.0.1/tldrwl/summarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-05-26 03:01:14.000000 tldrwl-1.0.1/tldrwl/summarize_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-05-26 03:01:14.000000 tldrwl-1.0.1/tldrwl/summarize_webpage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-05-26 03:01:14.000000 tldrwl-1.0.1/tldrwl/summarize_youtube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:01:27.482098 tldrwl-1.0.1/tldrwl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16752 2023-05-26 03:01:27.000000 tldrwl-1.0.1/tldrwl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-26 03:01:27.000000 tldrwl-1.0.1/tldrwl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 03:01:27.000000 tldrwl-1.0.1/tldrwl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-26 03:01:27.000000 tldrwl-1.0.1/tldrwl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-26 03:01:27.000000 tldrwl-1.0.1/tldrwl.egg-info/top_level.txt
```

### Comparing `tldrwl-1.0.0/PKG-INFO` & `tldrwl-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tldrwl
-Version: 1.0.0
+Version: 1.0.1
 Summary: Too long, didn't read/watch/listen
 Home-page: https://github.com/jrodal98/tldrwl
 Author: Jacob Rodal
 Author-email: dev@jrodal.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `tldrwl-1.0.0/README.md` & `tldrwl-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `tldrwl-1.0.0/setup.py` & `tldrwl-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 with open("requirements.txt") as f:
     install_requires = f.read().splitlines()
 
 setuptools.setup(
     name="tldrwl",
-    version="1.0.0",
+    version="1.0.1",
     author="Jacob Rodal",
     author_email="dev@jrodal.com",
     description="Too long, didn't read/watch/listen",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jrodal98/tldrwl",
     packages=setuptools.find_packages(),
```

### Comparing `tldrwl-1.0.0/tldrwl/__main__.py` & `tldrwl-1.0.1/tldrwl/__main__.py`

 * *Files identical despite different names*

### Comparing `tldrwl-1.0.0/tldrwl/ai_interface.py` & `tldrwl-1.0.1/tldrwl/ai_interface.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,34 +28,34 @@
 
     @property
     def estimated_cost_usd(self) -> float:
         return self.num_tokens * self.model.cost_per_1000_tokens * (1 / 1000)
 
 
 class AiInterface(ABC):
-    def __init_subclass__(cls) -> None:
-        if not Register.is_registered():
-            Register.register()
-
     @abstractmethod
     def _summarize_sync(self, text: str) -> Summary:
         pass
 
     @abstractmethod
     async def _summarize_async(self, text: str) -> Summary:
         pass
 
     def summarize_sync(self, text: str) -> Summary:
+        if not Register.is_registered():
+            Register.register()
         try:
             return self._summarize_sync(text)
         except TldrwlException:
             raise
         except Exception as e:
             raise TldrwlException(msg=str(e), cause="n/a", remediation="n/a") from e
 
     async def summarize_async(self, text: str) -> Summary:
+        if not Register.is_registered():
+            Register.register()
         try:
             return await self._summarize_async(text)
         except TldrwlException:
             raise
         except Exception as e:
             raise TldrwlException(msg=str(e), cause="n/a", remediation="n/a") from e
```

### Comparing `tldrwl-1.0.0/tldrwl/exception.py` & `tldrwl-1.0.1/tldrwl/exception.py`

 * *Files identical despite different names*

### Comparing `tldrwl-1.0.0/tldrwl/logger.py` & `tldrwl-1.0.1/tldrwl/logger.py`

 * *Files identical despite different names*

### Comparing `tldrwl-1.0.0/tldrwl/register.py` & `tldrwl-1.0.1/tldrwl/register.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     @classmethod
     def is_registered(cls) -> bool:
         return cls._registered
 
     @classmethod
     def register(
         cls,
-        *,
         openai_api_key_env_var: str = "OPENAI_API_KEY",
     ) -> None:
         openai_api_key = os.getenv(openai_api_key_env_var)
         if not openai_api_key:
             raise TldrwlRegisterException.make_error(
                 field="openai api key", env_var=openai_api_key_env_var
             )
```

### Comparing `tldrwl-1.0.0/tldrwl/summarize.py` & `tldrwl-1.0.1/tldrwl/summarize.py`

 * *Files identical despite different names*

### Comparing `tldrwl-1.0.0/tldrwl/summarize_text.py` & `tldrwl-1.0.1/tldrwl/summarize_text.py`

 * *Files identical despite different names*

### Comparing `tldrwl-1.0.0/tldrwl/summarize_webpage.py` & `tldrwl-1.0.1/tldrwl/summarize_webpage.py`

 * *Files identical despite different names*

### Comparing `tldrwl-1.0.0/tldrwl/summarize_youtube.py` & `tldrwl-1.0.1/tldrwl/summarize_youtube.py`

 * *Files identical despite different names*

### Comparing `tldrwl-1.0.0/tldrwl.egg-info/PKG-INFO` & `tldrwl-1.0.1/tldrwl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tldrwl
-Version: 1.0.0
+Version: 1.0.1
 Summary: Too long, didn't read/watch/listen
 Home-page: https://github.com/jrodal98/tldrwl
 Author: Jacob Rodal
 Author-email: dev@jrodal.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

