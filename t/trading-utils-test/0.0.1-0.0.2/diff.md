# Comparing `tmp/trading_utils_test-0.0.1.tar.gz` & `tmp/trading_utils_test-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trading_utils_test-0.0.1.tar", max compression
+gzip compressed data, was "trading_utils_test-0.0.2.tar", max compression
```

## Comparing `trading_utils_test-0.0.1.tar` & `trading_utils_test-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0      340 2023-05-26 11:12:46.417035 trading_utils_test-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-26 10:26:21.308636 trading_utils_test-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-05-26 10:26:21.308636 trading_utils_test-0.0.1/trading_utils/__init__.py
--rw-r--r--   0        0        0     1419 2023-05-26 10:51:19.210821 trading_utils_test-0.0.1/trading_utils/logger/__init__.py
--rw-r--r--   0        0        0        0 2023-05-26 10:26:21.308636 trading_utils_test-0.0.1/trading_utils/thread_manager/__init__.py
--rw-r--r--   0        0        0     1365 2023-05-26 10:42:18.062471 trading_utils_test-0.0.1/trading_utils/thread_manager/smiley.py
--rw-r--r--   0        0        0     1546 2023-05-26 10:42:38.312139 trading_utils_test-0.0.1/trading_utils/thread_manager/thread_manager.py
--rw-r--r--   0        0        0      412 1970-01-01 00:00:00.000000 trading_utils_test-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      340 2023-05-26 11:45:42.087515 trading_utils_test-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-26 10:26:21.308636 trading_utils_test-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-26 10:26:21.308636 trading_utils_test-0.0.2/trading_utils/__init__.py
+-rw-r--r--   0        0        0     1419 2023-05-26 10:51:19.210821 trading_utils_test-0.0.2/trading_utils/logger/__init__.py
+-rw-r--r--   0        0        0     1546 2023-05-26 11:44:51.472515 trading_utils_test-0.0.2/trading_utils/thread_manager/__init__.py
+-rw-r--r--   0        0        0     1365 2023-05-26 10:42:18.062471 trading_utils_test-0.0.2/trading_utils/thread_manager/smiley.py
+-rw-r--r--   0        0        0      412 1970-01-01 00:00:00.000000 trading_utils_test-0.0.2/PKG-INFO
```

### Comparing `trading_utils_test-0.0.1/trading_utils/logger/__init__.py` & `trading_utils_test-0.0.2/trading_utils/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `trading_utils_test-0.0.1/trading_utils/thread_manager/smiley.py` & `trading_utils_test-0.0.2/trading_utils/thread_manager/smiley.py`

 * *Files identical despite different names*

### Comparing `trading_utils_test-0.0.1/trading_utils/thread_manager/thread_manager.py` & `trading_utils_test-0.0.2/trading_utils/thread_manager/__init__.py`

 * *Files identical despite different names*

