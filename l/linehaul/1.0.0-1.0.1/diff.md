# Comparing `tmp/linehaul-1.0.0.tar.gz` & `tmp/linehaul-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linehaul-1.0.0.tar", last modified: Fri May 26 10:23:14 2023, max compression
+gzip compressed data, was "linehaul-1.0.1.tar", last modified: Fri May 26 12:19:06 2023, max compression
```

## Comparing `linehaul-1.0.0.tar` & `linehaul-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:23:14.855489 linehaul-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     9695 2023-05-26 10:23:01.000000 linehaul-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-26 10:23:14.855489 linehaul-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-26 10:23:01.000000 linehaul-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:23:14.855489 linehaul-1.0.0/linehaul/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-26 10:23:01.000000 linehaul-1.0.0/linehaul/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:23:14.855489 linehaul-1.0.0/linehaul/events/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-26 10:23:01.000000 linehaul-1.0.0/linehaul/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-05-26 10:23:01.000000 linehaul-1.0.0/linehaul/events/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-26 10:23:01.000000 linehaul-1.0.0/linehaul/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:23:14.855489 linehaul-1.0.0/linehaul/ua/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-26 10:23:01.000000 linehaul-1.0.0/linehaul/ua/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-26 10:23:01.000000 linehaul-1.0.0/linehaul/ua/datastructures.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-05-26 10:23:01.000000 linehaul-1.0.0/linehaul/ua/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-05-26 10:23:01.000000 linehaul-1.0.0/linehaul/ua/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:23:14.855489 linehaul-1.0.0/linehaul.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-26 10:23:14.000000 linehaul-1.0.0/linehaul.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-26 10:23:14.000000 linehaul-1.0.0/linehaul.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 10:23:14.000000 linehaul-1.0.0/linehaul.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-26 10:23:14.000000 linehaul-1.0.0/linehaul.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-26 10:23:14.000000 linehaul-1.0.0/linehaul.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-26 10:23:01.000000 linehaul-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-26 10:23:14.855489 linehaul-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:19:06.236803 linehaul-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     9695 2023-05-26 12:18:57.000000 linehaul-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-26 12:19:06.236803 linehaul-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-26 12:18:57.000000 linehaul-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:19:06.236803 linehaul-1.0.1/linehaul/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-26 12:18:57.000000 linehaul-1.0.1/linehaul/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:19:06.236803 linehaul-1.0.1/linehaul/events/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-26 12:18:57.000000 linehaul-1.0.1/linehaul/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-05-26 12:18:57.000000 linehaul-1.0.1/linehaul/events/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-26 12:18:57.000000 linehaul-1.0.1/linehaul/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:19:06.236803 linehaul-1.0.1/linehaul/ua/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-26 12:18:57.000000 linehaul-1.0.1/linehaul/ua/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-26 12:18:57.000000 linehaul-1.0.1/linehaul/ua/datastructures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-05-26 12:18:57.000000 linehaul-1.0.1/linehaul/ua/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11135 2023-05-26 12:18:57.000000 linehaul-1.0.1/linehaul/ua/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:19:06.236803 linehaul-1.0.1/linehaul.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-26 12:19:06.000000 linehaul-1.0.1/linehaul.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-26 12:19:06.000000 linehaul-1.0.1/linehaul.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 12:19:06.000000 linehaul-1.0.1/linehaul.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-26 12:19:06.000000 linehaul-1.0.1/linehaul.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-26 12:19:06.000000 linehaul-1.0.1/linehaul.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-26 12:18:57.000000 linehaul-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-26 12:19:06.240803 linehaul-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:19:06.236803 linehaul-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-26 12:18:57.000000 linehaul-1.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-26 12:18:57.000000 linehaul-1.0.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-05-26 12:18:57.000000 linehaul-1.0.1/tests/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-05-26 12:18:57.000000 linehaul-1.0.1/tests/test_strategies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:19:06.236803 linehaul-1.0.1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-26 12:18:57.000000 linehaul-1.0.1/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:19:06.236803 linehaul-1.0.1/tests/unit/events/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-26 12:18:57.000000 linehaul-1.0.1/tests/unit/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-26 12:18:57.000000 linehaul-1.0.1/tests/unit/events/test_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:19:06.236803 linehaul-1.0.1/tests/unit/ua/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-26 12:18:57.000000 linehaul-1.0.1/tests/unit/ua/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-05-26 12:18:57.000000 linehaul-1.0.1/tests/unit/ua/test_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-05-26 12:18:57.000000 linehaul-1.0.1/tests/unit/ua/test_parser.py
```

### Comparing `linehaul-1.0.0/LICENSE` & `linehaul-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `linehaul-1.0.0/PKG-INFO` & `linehaul-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: linehaul
-Version: 1.0.0
+Version: 1.0.1
 Summary: User-Agent parsing for PyPI analytics
 Author-email: PyPI Admins <admin@pypi.org>
 Project-URL: Homepage, https://github.com/pypi/linehaul-cloud-function
 Project-URL: Source, https://github.com/pypi/linehaul-cloud-function
 Keywords: pypi,user-agent,parsing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: <4,>=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `linehaul-1.0.0/linehaul/__init__.py` & `linehaul-1.0.1/linehaul/__init__.py`

 * *Files identical despite different names*

### Comparing `linehaul-1.0.0/linehaul/events/__init__.py` & `linehaul-1.0.1/linehaul/events/__init__.py`

 * *Files identical despite different names*

### Comparing `linehaul-1.0.0/linehaul/events/parser.py` & `linehaul-1.0.1/linehaul/events/parser.py`

 * *Files identical despite different names*

### Comparing `linehaul-1.0.0/linehaul/logging.py` & `linehaul-1.0.1/linehaul/logging.py`

 * *Files identical despite different names*

### Comparing `linehaul-1.0.0/linehaul/ua/__init__.py` & `linehaul-1.0.1/linehaul/ua/__init__.py`

 * *Files identical despite different names*

### Comparing `linehaul-1.0.0/linehaul/ua/datastructures.py` & `linehaul-1.0.1/linehaul/ua/datastructures.py`

 * *Files identical despite different names*

### Comparing `linehaul-1.0.0/linehaul/ua/impl.py` & `linehaul-1.0.1/linehaul/ua/impl.py`

 * *Files identical despite different names*

### Comparing `linehaul-1.0.0/linehaul/ua/parser.py` & `linehaul-1.0.1/linehaul/ua/parser.py`

 * *Files 23% similar despite different names*

```diff
@@ -154,14 +154,53 @@
 
 @_parser.register
 @regex_ua_parser(r"^pep381client(?:-proxy)?/(?P<version>\S+)$")
 def PEP381ClientUserAgent(*, version):
     return {"installer": {"name": "pep381client", "version": version}}
 
 
+@_parser.register
+@regex_ua_parser(r"^maturin/(?P<version>\S+)$")
+def MaturinUserAgent(*, version):
+    return {"installer": {"name": "maturin", "version": version}}
+
+
+@_parser.register
+@regex_ua_parser(r"^pdm/(?P<version>\S+) (?P<impl_name>\S+)/(?P<impl_version>\S+)$")
+def PDMUserAgent(*, version, impl_name, impl_version):
+    return {
+        "installer": {"name": "pdm", "version": version},
+        "implementation": {"name": impl_name, "version": impl_version},
+    }
+
+
+@_parser.register
+@regex_ua_parser(
+    r"^poetry/(?P<version>\S+) (?P<impl_name>\S+)/(?P<impl_version>\S+) "
+    r"(?P<system_name>\S+)/(?P<system_release>\S+)?$"
+)
+def PoetryUserAgent(*, version, impl_name, impl_version, system_name, system_release):
+    return {
+        "installer": {"name": "poetry", "version": version},
+        "implementation": {"name": impl_name, "version": impl_version},
+        "system": {"name": system_name, "release": system_release},
+    }
+
+
+@_parser.register
+@regex_ua_parser(
+    r"^twine/(?P<version>\S+)(?: .+)? (?P<impl_name>\S+)/(?P<impl_version>\S+)$"
+)
+def TwineUserAgent(*, version, impl_name, impl_version):
+    return {
+        "installer": {"name": "twine", "version": version},
+        "implementation": {"name": impl_name, "version": impl_version},
+    }
+
+
 # TODO: We should probably consider not parsing this specially, and moving it to
 #       just the same as we treat browsers, since we don't really know anything
 #       about it-- including whether or not the version of Python mentioned is
 #       the one they're going to install it into or not. The one real sticking
 #       point is that before pip 1.4, pip just used the default urllib2 UA, so
 #       right now we're counting pip 1.4 in here... but pip 1.4 usage is probably
 #       low enough not to worry about that any more.
```

### Comparing `linehaul-1.0.0/linehaul.egg-info/PKG-INFO` & `linehaul-1.0.1/linehaul.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: linehaul
-Version: 1.0.0
+Version: 1.0.1
 Summary: User-Agent parsing for PyPI analytics
 Author-email: PyPI Admins <admin@pypi.org>
 Project-URL: Homepage, https://github.com/pypi/linehaul-cloud-function
 Project-URL: Source, https://github.com/pypi/linehaul-cloud-function
 Keywords: pypi,user-agent,parsing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: <4,>=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `linehaul-1.0.0/pyproject.toml` & `linehaul-1.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 [project]
 name = "linehaul"
-version = "1.0.0"
+version = "1.0.1"
 description = "User-Agent parsing for PyPI analytics"
 
 readme = "README.md"
 requires-python = ">=3.11, <4"
 license = {file = "LICENSE.txt"}
 
 keywords = ["pypi", "user-agent", "parsing"]
 authors = [
   {name = "PyPI Admins", email = "admin@pypi.org" }
 ]
 
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Intended Audience :: Developers",
-  "Topic :: Software Development :: Build Tools",
   "License :: OSI Approved :: Apache Software License",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3 :: Only",
 ]
 
 dependencies = [
```

