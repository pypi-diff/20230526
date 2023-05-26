# Comparing `tmp/torchmanager-1.1.2.tar.gz` & `tmp/torchmanager-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchmanager-1.1.2.tar", last modified: Fri Apr 21 18:44:52 2023, max compression
+gzip compressed data, was "torchmanager-1.1.3.tar", max compression
```

## Comparing `torchmanager-1.1.2.tar` & `torchmanager-1.1.3.tar`

### file list

```diff
@@ -1,67 +1,44 @@
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-21 18:44:52.733735 torchmanager-1.1.2/
--rw-r--r--   0 kisonho    (501) staff       (20)     1318 2023-04-07 18:23:00.000000 torchmanager-1.1.2/LICENSE
--rw-r--r--   0 kisonho    (501) staff       (20)     2102 2023-04-21 18:44:52.733328 torchmanager-1.1.2/PKG-INFO
--rw-r--r--   0 kisonho    (501) staff       (20)     1806 2023-04-07 18:23:00.000000 torchmanager-1.1.2/README.md
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-21 18:44:52.709401 torchmanager-1.1.2/core/
--rw-r--r--   0 kisonho    (501) staff       (20)      443 2023-04-21 18:38:20.000000 torchmanager-1.1.2/core/__init__.py
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-21 18:44:52.711064 torchmanager-1.1.2/core/devices/
--rw-r--r--   0 kisonho    (501) staff       (20)      114 2023-04-21 18:38:20.000000 torchmanager-1.1.2/core/devices/__init__.py
--rw-r--r--   0 kisonho    (501) staff       (20)     5587 2023-04-21 18:38:20.000000 torchmanager-1.1.2/core/devices/device.py
--rw-r--r--   0 kisonho    (501) staff       (20)      264 2023-03-16 14:38:14.000000 torchmanager-1.1.2/core/devices/protocols.py
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-21 18:44:52.712803 torchmanager-1.1.2/core/errors/
--rw-r--r--   0 kisonho    (501) staff       (20)      153 2023-04-07 18:23:00.000000 torchmanager-1.1.2/core/errors/__init__.py
--rw-r--r--   0 kisonho    (501) staff       (20)      350 2023-04-07 18:23:00.000000 torchmanager-1.1.2/core/errors/runtime.py
--rw-r--r--   0 kisonho    (501) staff       (20)      669 2023-04-07 18:23:00.000000 torchmanager-1.1.2/core/errors/train.py
--rw-r--r--   0 kisonho    (501) staff       (20)     2728 2023-04-21 18:38:20.000000 torchmanager-1.1.2/core/protocols.py
--rw-r--r--   0 kisonho    (501) staff       (20)      204 2023-04-07 18:23:00.000000 torchmanager-1.1.2/core/typing.py
--rw-r--r--   0 kisonho    (501) staff       (20)     5288 2023-04-21 18:38:20.000000 torchmanager-1.1.2/core/version.py
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-21 18:44:52.713919 torchmanager-1.1.2/core/view/
--rw-r--r--   0 kisonho    (501) staff       (20)      126 2023-04-21 18:38:20.000000 torchmanager-1.1.2/core/view/__init__.py
--rw-r--r--   0 kisonho    (501) staff       (20)      313 2023-03-16 14:38:14.000000 torchmanager-1.1.2/core/view/protocols.py
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-21 18:44:52.716500 torchmanager-1.1.2/lib/
--rw-r--r--   0 kisonho    (501) staff       (20)      281 2023-04-21 18:38:20.000000 torchmanager-1.1.2/lib/__init__.py
--rw-r--r--   0 kisonho    (501) staff       (20)    11052 2023-04-21 18:38:20.000000 torchmanager-1.1.2/lib/basic.py
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-21 18:44:52.720931 torchmanager-1.1.2/lib/callbacks/
--rw-r--r--   0 kisonho    (501) staff       (20)      658 2023-04-21 18:31:47.000000 torchmanager-1.1.2/lib/callbacks/__init__.py
--rw-r--r--   0 kisonho    (501) staff       (20)     4255 2023-04-07 18:23:00.000000 torchmanager-1.1.2/lib/callbacks/callback.py
--rw-r--r--   0 kisonho    (501) staff       (20)     4542 2023-04-07 18:23:00.000000 torchmanager-1.1.2/lib/callbacks/ckpt.py
--rw-r--r--   0 kisonho    (501) staff       (20)     3523 2023-04-07 18:23:00.000000 torchmanager-1.1.2/lib/callbacks/dynamic.py
--rw-r--r--   0 kisonho    (501) staff       (20)     1608 2023-04-07 18:23:00.000000 torchmanager-1.1.2/lib/callbacks/early_stop.py
--rw-r--r--   0 kisonho    (501) staff       (20)     4846 2023-04-21 18:38:20.000000 torchmanager-1.1.2/lib/callbacks/experiment.py
--rw-r--r--   0 kisonho    (501) staff       (20)     2224 2023-04-07 18:23:00.000000 torchmanager-1.1.2/lib/callbacks/lr.py
--rw-r--r--   0 kisonho    (501) staff       (20)     2440 2023-04-07 18:23:00.000000 torchmanager-1.1.2/lib/callbacks/tensorboard.py
--rw-r--r--   0 kisonho    (501) staff       (20)      963 2023-04-21 18:34:55.000000 torchmanager-1.1.2/lib/compatibility.py
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-21 18:44:52.722427 torchmanager-1.1.2/lib/data/
--rw-r--r--   0 kisonho    (501) staff       (20)       85 2023-04-21 18:31:47.000000 torchmanager-1.1.2/lib/data/__init__.py
--rw-r--r--   0 kisonho    (501) staff       (20)     6866 2023-04-21 18:38:20.000000 torchmanager-1.1.2/lib/data/dataset.py
--rw-r--r--   0 kisonho    (501) staff       (20)     2236 2023-04-21 18:38:20.000000 torchmanager-1.1.2/lib/data/sliding.py
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-21 18:44:52.724764 torchmanager-1.1.2/lib/losses/
--rw-r--r--   0 kisonho    (501) staff       (20)      171 2023-04-21 18:38:20.000000 torchmanager-1.1.2/lib/losses/__init__.py
--rw-r--r--   0 kisonho    (501) staff       (20)     5386 2023-04-07 18:23:00.000000 torchmanager-1.1.2/lib/losses/cross_entropy.py
--rw-r--r--   0 kisonho    (501) staff       (20)     1044 2023-04-21 18:38:20.000000 torchmanager-1.1.2/lib/losses/dice.py
--rw-r--r--   0 kisonho    (501) staff       (20)     7061 2023-04-21 18:38:20.000000 torchmanager-1.1.2/lib/losses/loss.py
--rw-r--r--   0 kisonho    (501) staff       (20)     2381 2023-04-21 18:38:20.000000 torchmanager-1.1.2/lib/losses/mse.py
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-21 18:44:52.727102 torchmanager-1.1.2/lib/metrics/
--rw-r--r--   0 kisonho    (501) staff       (20)      234 2023-04-21 18:38:20.000000 torchmanager-1.1.2/lib/metrics/__init__.py
--rw-r--r--   0 kisonho    (501) staff       (20)     3272 2023-04-21 18:38:20.000000 torchmanager-1.1.2/lib/metrics/accuracy.py
--rw-r--r--   0 kisonho    (501) staff       (20)     2546 2023-04-21 18:38:20.000000 torchmanager-1.1.2/lib/metrics/conf_met.py
--rw-r--r--   0 kisonho    (501) staff       (20)     2440 2023-04-21 18:38:20.000000 torchmanager-1.1.2/lib/metrics/iou.py
--rw-r--r--   0 kisonho    (501) staff       (20)     4000 2023-04-21 18:38:20.000000 torchmanager-1.1.2/lib/metrics/metric.py
--rw-r--r--   0 kisonho    (501) staff       (20)     9401 2023-04-21 18:38:20.000000 torchmanager-1.1.2/lib/testing.py
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-21 18:44:52.728550 torchmanager-1.1.2/lib/train/
--rw-r--r--   0 kisonho    (501) staff       (20)      191 2023-04-21 18:38:20.000000 torchmanager-1.1.2/lib/train/__init__.py
--rw-r--r--   0 kisonho    (501) staff       (20)     4964 2023-04-07 18:23:00.000000 torchmanager-1.1.2/lib/train/checkpoint.py
--rw-r--r--   0 kisonho    (501) staff       (20)     2037 2023-04-21 18:38:20.000000 torchmanager-1.1.2/lib/train/learning_rate.py
--rw-r--r--   0 kisonho    (501) staff       (20)    14893 2023-04-21 18:38:20.000000 torchmanager-1.1.2/lib/training.py
--rw-r--r--   0 kisonho    (501) staff       (20)       38 2023-04-21 18:44:52.733904 torchmanager-1.1.2/setup.cfg
--rw-r--r--   0 kisonho    (501) staff       (20)     1377 2023-04-21 18:38:20.000000 torchmanager-1.1.2/setup.py
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-21 18:44:52.730162 torchmanager-1.1.2/tests/
--rw-r--r--   0 kisonho    (501) staff       (20)     1203 2023-04-17 18:56:25.000000 torchmanager-1.1.2/tests/test_0101.py
--rw-r--r--   0 kisonho    (501) staff       (20)      934 2023-04-17 15:45:19.000000 torchmanager-1.1.2/tests/test_0102.py
--rw-r--r--   0 kisonho    (501) staff       (20)      263 2023-04-17 15:33:18.000000 torchmanager-1.1.2/tests/test_base.py
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-21 18:44:52.732740 torchmanager-1.1.2/torchmanager.egg-info/
--rw-r--r--   0 kisonho    (501) staff       (20)     2102 2023-04-21 18:44:52.000000 torchmanager-1.1.2/torchmanager.egg-info/PKG-INFO
--rw-r--r--   0 kisonho    (501) staff       (20)     1154 2023-04-21 18:44:52.000000 torchmanager-1.1.2/torchmanager.egg-info/SOURCES.txt
--rw-r--r--   0 kisonho    (501) staff       (20)        1 2023-04-21 18:44:52.000000 torchmanager-1.1.2/torchmanager.egg-info/dependency_links.txt
--rw-r--r--   0 kisonho    (501) staff       (20)       11 2023-04-21 18:44:52.000000 torchmanager-1.1.2/torchmanager.egg-info/requires.txt
--rw-r--r--   0 kisonho    (501) staff       (20)       31 2023-04-21 18:44:52.000000 torchmanager-1.1.2/torchmanager.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1318 2023-04-21 19:45:23.217167 torchmanager-1.1.3/LICENSE
+-rw-r--r--   0        0        0      616 2023-05-26 14:45:47.094692 torchmanager-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0      281 2023-05-26 13:57:53.914350 torchmanager-1.1.3/torchmanager/__init__.py
+-rw-r--r--   0        0        0    11052 2023-05-26 13:57:53.914710 torchmanager-1.1.3/torchmanager/basic.py
+-rw-r--r--   0        0        0      658 2023-05-26 13:57:53.915031 torchmanager-1.1.3/torchmanager/callbacks/__init__.py
+-rw-r--r--   0        0        0     4255 2023-05-26 13:57:53.915310 torchmanager-1.1.3/torchmanager/callbacks/callback.py
+-rw-r--r--   0        0        0     4628 2023-05-26 13:57:23.129146 torchmanager-1.1.3/torchmanager/callbacks/ckpt.py
+-rw-r--r--   0        0        0     3523 2023-05-26 13:57:23.129390 torchmanager-1.1.3/torchmanager/callbacks/dynamic.py
+-rw-r--r--   0        0        0     1608 2023-05-26 13:57:23.129552 torchmanager-1.1.3/torchmanager/callbacks/early_stop.py
+-rw-r--r--   0        0        0     4846 2023-05-26 13:57:53.915619 torchmanager-1.1.3/torchmanager/callbacks/experiment.py
+-rw-r--r--   0        0        0     2224 2023-05-26 13:57:23.129973 torchmanager-1.1.3/torchmanager/callbacks/lr.py
+-rw-r--r--   0        0        0     2440 2023-05-26 13:57:53.915840 torchmanager-1.1.3/torchmanager/callbacks/tensorboard.py
+-rw-r--r--   0        0        0      963 2023-05-26 13:57:53.916340 torchmanager-1.1.3/torchmanager/compatibility.py
+-rw-r--r--   0        0        0       85 2023-05-26 13:57:23.131070 torchmanager-1.1.3/torchmanager/data/__init__.py
+-rw-r--r--   0        0        0     6962 2023-05-26 13:57:53.916733 torchmanager-1.1.3/torchmanager/data/dataset.py
+-rw-r--r--   0        0        0     2236 2023-05-26 13:57:53.917130 torchmanager-1.1.3/torchmanager/data/sliding.py
+-rw-r--r--   0        0        0      171 2023-05-26 13:57:53.917364 torchmanager-1.1.3/torchmanager/losses/__init__.py
+-rw-r--r--   0        0        0     5386 2023-05-26 13:57:23.132661 torchmanager-1.1.3/torchmanager/losses/cross_entropy.py
+-rw-r--r--   0        0        0     1044 2023-05-26 13:57:53.917665 torchmanager-1.1.3/torchmanager/losses/dice.py
+-rw-r--r--   0        0        0     7061 2023-05-26 13:57:53.917950 torchmanager-1.1.3/torchmanager/losses/loss.py
+-rw-r--r--   0        0        0     2381 2023-05-26 13:57:53.918243 torchmanager-1.1.3/torchmanager/losses/mse.py
+-rw-r--r--   0        0        0      234 2023-05-26 13:57:53.918541 torchmanager-1.1.3/torchmanager/metrics/__init__.py
+-rw-r--r--   0        0        0     3272 2023-05-26 13:57:53.918835 torchmanager-1.1.3/torchmanager/metrics/accuracy.py
+-rw-r--r--   0        0        0     2546 2023-05-26 13:57:53.919126 torchmanager-1.1.3/torchmanager/metrics/conf_met.py
+-rw-r--r--   0        0        0     2440 2023-05-26 13:57:53.919427 torchmanager-1.1.3/torchmanager/metrics/iou.py
+-rw-r--r--   0        0        0     4000 2023-05-26 13:57:53.919829 torchmanager-1.1.3/torchmanager/metrics/metric.py
+-rw-r--r--   0        0        0     9401 2023-05-26 13:57:53.920555 torchmanager-1.1.3/torchmanager/testing.py
+-rw-r--r--   0        0        0      191 2023-05-26 13:57:53.920853 torchmanager-1.1.3/torchmanager/train/__init__.py
+-rw-r--r--   0        0        0     4964 2023-05-26 13:57:23.135892 torchmanager-1.1.3/torchmanager/train/checkpoint.py
+-rw-r--r--   0        0        0     2037 2023-05-26 13:57:53.922149 torchmanager-1.1.3/torchmanager/train/learning_rate.py
+-rw-r--r--   0        0        0    14893 2023-05-26 13:57:53.922553 torchmanager-1.1.3/torchmanager/training.py
+-rw-r--r--   0        0        0      443 2023-05-26 13:57:53.922922 torchmanager-1.1.3/torchmanager_core/__init__.py
+-rw-r--r--   0        0        0      114 2023-05-26 13:57:53.923187 torchmanager-1.1.3/torchmanager_core/devices/__init__.py
+-rw-r--r--   0        0        0     5587 2023-05-26 13:57:53.923476 torchmanager-1.1.3/torchmanager_core/devices/device.py
+-rw-r--r--   0        0        0      264 2023-05-26 13:57:23.137865 torchmanager-1.1.3/torchmanager_core/devices/protocols.py
+-rw-r--r--   0        0        0      153 2023-05-26 13:57:23.138096 torchmanager-1.1.3/torchmanager_core/errors/__init__.py
+-rw-r--r--   0        0        0      350 2023-05-26 13:57:23.138227 torchmanager-1.1.3/torchmanager_core/errors/runtime.py
+-rw-r--r--   0        0        0      669 2023-05-26 13:57:23.138467 torchmanager-1.1.3/torchmanager_core/errors/train.py
+-rw-r--r--   0        0        0     2728 2023-05-26 13:57:53.923701 torchmanager-1.1.3/torchmanager_core/protocols.py
+-rw-r--r--   0        0        0      204 2023-05-26 13:57:23.138928 torchmanager-1.1.3/torchmanager_core/typing.py
+-rw-r--r--   0        0        0     5253 2023-05-26 13:57:53.924003 torchmanager-1.1.3/torchmanager_core/version.py
+-rw-r--r--   0        0        0      126 2023-05-26 13:57:53.924253 torchmanager-1.1.3/torchmanager_core/view/__init__.py
+-rw-r--r--   0        0        0      313 2023-05-26 13:57:23.140532 torchmanager-1.1.3/torchmanager_core/view/protocols.py
+-rw-r--r--   0        0        0      664 1970-01-01 00:00:00.000000 torchmanager-1.1.3/PKG-INFO
```

### Comparing `torchmanager-1.1.2/LICENSE` & `torchmanager-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.2/core/devices/device.py` & `torchmanager-1.1.3/torchmanager_core/devices/device.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.2/core/errors/train.py` & `torchmanager-1.1.3/torchmanager_core/errors/train.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.2/core/protocols.py` & `torchmanager-1.1.3/torchmanager_core/protocols.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.2/core/version.py` & `torchmanager-1.1.3/torchmanager_core/version.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,36 +14,32 @@
         # convert to string
         version_str = str(v)
 
         # format version
         if version_str.startswith('v'):
             version_str = version_str[1:]
 
+        # split pre-release version
+        pre_release_parts = version_str.split('a')
+        if len(pre_release_parts) > 1:
+            self.pre_release = 'a' + pre_release_parts[1]
+            version_str = pre_release_parts[0]
+        else:
+            pre_release_parts = version_str.split('b')
+            if len(pre_release_parts) > 1:
+                self.pre_release = 'b' + pre_release_parts[1]
+                version_str = pre_release_parts[0]
+            else:
+                self.pre_release = "0"
+
         # split version
         version_parts = version_str.split('.')
         self.main_version = int(version_parts[0])
         self.minor_version = int(version_parts[1])
-        self.pre_release = None
-
-        # set sub  version
-        if len(version_parts) > 2:
-            # split alpha subversion parts
-            sub_version_parts = version_parts[2].split('a')
-            if len(sub_version_parts) > 1:
-                self.sub_version = int(sub_version_parts[0])
-                self.pre_release = 'a' + sub_version_parts[1]
-            else:
-                sub_version_parts = version_parts[2].split('b')
-                if len(sub_version_parts) > 1:
-                    self.sub_version = int(sub_version_parts[0])
-                    self.pre_release = 'b' + sub_version_parts[1]
-                else:
-                    self.sub_version = int(version_parts[2])
-        else:
-            self.sub_version = 0
+        self.sub_version = int(version_parts[2]) if len(version_parts) > 2 else 0
 
     def __repr__(self) -> str:
         version_str = f"v{self.main_version}"
         if self.minor_version > 0 or self.sub_version > 0:
             version_str += f".{self.minor_version}"
         if self.sub_version > 0:
             version_str += f".{self.sub_version}"
@@ -92,31 +88,35 @@
         return self == other or self < other
 
     def __ge__(self, other: Any) -> bool:
         return self == other or self > other
 
 
 API = Version("v1.1")
-CURRENT = Version("v1.1.2")
-DESCRIPTION: str = "PyTorch Training Manager v1.1.2"
+CURRENT = Version("v1.1.3")
+DESCRIPTION: str = "PyTorch Training Manager v1.1.3"
 
 
 class VersionError(SystemError):
     def __init__(self, method_name: str, maximum_supported_version: str) -> None:
         super().__init__(f"`{method_name}` has been deprecated and removed from version {maximum_supported_version}. Current version: {CURRENT}.")
 
 
-def deprecated(target_version: str, removing_version: str):
+def deprecated(target_version: Any, removing_version: Any):
     '''
     Deprecated decorator function
 
     - Parameters:
-        - target_version: A `str` of version for the deprecation
-        - removing_version: A `str` of version for removing
+        - target_version: `Any` type of version for the deprecation
+        - removing_version: `Any` type of version for removing
     '''
+    # format versions
+    target_version = Version(target_version)
+    removing_version = Version(removing_version)
+
     # define wrapping function
     def wrapping_fn(fn):
         @functools.wraps(fn)
         def deprecated_fn(*args, **kwargs):
             if CURRENT >= removing_version:
                 raise VersionError(fn.__name__, removing_version)
             elif CURRENT >= target_version:
```

### Comparing `torchmanager-1.1.2/lib/basic.py` & `torchmanager-1.1.3/torchmanager/basic.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.2/lib/callbacks/__init__.py` & `torchmanager-1.1.3/torchmanager/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.2/lib/callbacks/callback.py` & `torchmanager-1.1.3/torchmanager/callbacks/callback.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.2/lib/callbacks/ckpt.py` & `torchmanager-1.1.3/torchmanager/callbacks/ckpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,39 +13,43 @@
 
     * extends: `.Callback
 
     - Properties:
         - ckpt_path: A `str` of checkpoint path
     """
     __ckpt_path: str
-    _checkpoint: Ckpt[T]
+    __checkpoint: Ckpt[T]
 
     @property
     def ckpt_path(self) -> str:
         return self.__ckpt_path
 
     @ckpt_path.setter
     def ckpt_path(self, p: str) -> None:
         self.__ckpt_path = os.path.normpath(p)
 
+    @property
+    def checkpoint(self) -> Ckpt[T]:
+        return self.__checkpoint
+
     def __init__(self, model: T, ckpt_path: str, **kwargs: Any) -> None:
         """
         Constructor
 
         - Parameters:
             - model: Any type of model to be saved
             - ckpt_path: A `str` of the checkpoint path
             - **kwargs: Other arguments in `Checkpoint` constructor
         """
         super().__init__()
-        self._checkpoint = Ckpt(model, **kwargs)
+        self.__checkpoint = Ckpt(model, **kwargs)
         self.ckpt_path = os.path.normpath(ckpt_path)
 
     def on_epoch_end(self, epoch: int, summary: Dict[str, float] = ..., val_summary: Optional[Dict[str, float]] = ...) -> None:
-        self._checkpoint.save(epoch, self.ckpt_path)
+        self.checkpoint.save(epoch, self.ckpt_path)
 
 class LastCheckpoint(_Checkpoint[T]):
     """
     Last checkpoint with frequency control support
 
     * extends: `_Checkpoint`
```

### Comparing `torchmanager-1.1.2/lib/callbacks/dynamic.py` & `torchmanager-1.1.3/torchmanager/callbacks/dynamic.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.2/lib/callbacks/early_stop.py` & `torchmanager-1.1.3/torchmanager/callbacks/early_stop.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.2/lib/callbacks/experiment.py` & `torchmanager-1.1.3/torchmanager/callbacks/experiment.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.2/lib/callbacks/lr.py` & `torchmanager-1.1.3/torchmanager/callbacks/lr.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.2/lib/callbacks/tensorboard.py` & `torchmanager-1.1.3/torchmanager/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.2/lib/compatibility.py` & `torchmanager-1.1.3/torchmanager/compatibility.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.2/lib/data/dataset.py` & `torchmanager-1.1.3/torchmanager/data/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,14 @@
     * Used as a combination of `torch.utils.data.Dataset` and `torch.utils.data.DataLoader`
 
     >>> from torchmanager import Manager
     >>> class SomeDataset(Dataset):
     ...    @property
     ...    def unbatched_size(self) -> int: ...
     ...
-    ...    def __init__(self, ...,  batch_size: int, device: torch.device = devices.CPU) -> None: ...
     ...    def __getitem__(self, index: Any) -> Any: ...
     >>> dataset = SomeDataset(..., batch_size)
     >>> manager = Manager(...)
     >>> manager.fit(dataset, ...)
 
     - Properties:
         - batch_size: An `int` of batch size for the current dataset
@@ -97,18 +96,17 @@
         return NotImplemented
 
     def __iter__(self) -> Iterator[T]:
         # initialize devices
         cpu_count = os.cpu_count()
         if cpu_count is None:
             cpu_count = 0
-        device = self.device
 
         # initialize loader
-        if device != devices.CPU:
+        if self.device != devices.CPU:
             data_loader = DataLoader(self, batch_size=self.batch_size, drop_last=self.drop_last, shuffle=self.shuffle, num_workers=cpu_count, pin_memory=True, pin_memory_device=str(self.device))
         else:
             data_loader = DataLoader(self, batch_size=self.batch_size, drop_last=self.drop_last, shuffle=self.shuffle, num_workers=cpu_count)
 
         # yield data
         for data in data_loader:
             yield self.unpack_data(data)
@@ -122,18 +120,20 @@
         """
         Unpacks a single data into inputs and targets
 
         - Parameters:
             - data: `Any` kind of single data
         - Returns: `Any` kind of inputs with type `T`
         """
-        if isinstance(data, Sequence):
-            return data[0], data[1] if len(data) >= 2 else NotImplemented # type: ignore
+        if isinstance(data, torch.Tensor) or isinstance(data, dict):
+            return data, data  # type: ignore # suppose for unsupervised reconstruction or a dictionary of packed data
+        if isinstance(data, Sequence) and len(data) == 2:
+            return data[0], data[1]  # type: ignore # suppose for supervised
         else:
-            return NotImplemented
+            return NotImplemented  # unknown type of dataset
 
 
 def batched(fn: Callable[..., _Dataset]):
     """
     Wrap a loading PyTorch dataset function into a loading dataset function
 
     Use as decorator with a function:
```

### Comparing `torchmanager-1.1.2/lib/data/sliding.py` & `torchmanager-1.1.3/torchmanager/data/sliding.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.2/lib/losses/cross_entropy.py` & `torchmanager-1.1.3/torchmanager/losses/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.2/lib/losses/dice.py` & `torchmanager-1.1.3/torchmanager/losses/dice.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.2/lib/losses/loss.py` & `torchmanager-1.1.3/torchmanager/losses/loss.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.2/lib/losses/mse.py` & `torchmanager-1.1.3/torchmanager/losses/mse.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.2/lib/metrics/accuracy.py` & `torchmanager-1.1.3/torchmanager/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.2/lib/metrics/conf_met.py` & `torchmanager-1.1.3/torchmanager/metrics/conf_met.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.2/lib/metrics/iou.py` & `torchmanager-1.1.3/torchmanager/metrics/iou.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.2/lib/metrics/metric.py` & `torchmanager-1.1.3/torchmanager/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.2/lib/testing.py` & `torchmanager-1.1.3/torchmanager/testing.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.2/lib/train/checkpoint.py` & `torchmanager-1.1.3/torchmanager/train/checkpoint.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.2/lib/train/learning_rate.py` & `torchmanager-1.1.3/torchmanager/train/learning_rate.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.2/lib/training.py` & `torchmanager-1.1.3/torchmanager/training.py`

 * *Files identical despite different names*

