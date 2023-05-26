# Comparing `tmp/cn2int-0.2.2.tar.gz` & `tmp/cn2int-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cn2int-0.2.2.tar", last modified: Fri Mar 24 06:17:29 2023, max compression
+gzip compressed data, was "cn2int-0.2.3.tar", last modified: Fri May 26 01:51:48 2023, max compression
```

## Comparing `cn2int-0.2.2.tar` & `cn2int-0.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 suhecheng  (1000) suhecheng  (1000)        0 2023-03-24 06:17:29.890809 cn2int-0.2.2/
--rwxrwxr-x   0 suhecheng  (1000) suhecheng  (1000)       38 2023-02-26 11:54:18.000000 cn2int-0.2.2/MANIFEST.in
--rw-rw-r--   0 suhecheng  (1000) suhecheng  (1000)     1473 2023-03-24 06:17:29.890809 cn2int-0.2.2/PKG-INFO
--rw-rw-r--   0 suhecheng  (1000) suhecheng  (1000)     1120 2023-02-26 11:54:18.000000 cn2int-0.2.2/README-PyPI.md
--rw-rw-r--   0 suhecheng  (1000) suhecheng  (1000)     4336 2023-02-26 11:54:18.000000 cn2int-0.2.2/README.md
-drwxrwxr-x   0 suhecheng  (1000) suhecheng  (1000)        0 2023-03-24 06:17:29.890809 cn2int-0.2.2/cn2int/
--rw-rw-r--   0 suhecheng  (1000) suhecheng  (1000)      191 2023-02-26 11:54:18.000000 cn2int-0.2.2/cn2int/__init__.py
--rw-rw-r--   0 suhecheng  (1000) suhecheng  (1000)    17247 2023-03-24 06:11:33.000000 cn2int-0.2.2/cn2int/cn2int.py
--rw-rw-r--   0 suhecheng  (1000) suhecheng  (1000)     1396 2023-02-26 11:54:18.000000 cn2int-0.2.2/cn2int/performance.py
-drwxrwxr-x   0 suhecheng  (1000) suhecheng  (1000)        0 2023-03-24 06:17:29.890809 cn2int-0.2.2/cn2int.egg-info/
--rw-rw-r--   0 suhecheng  (1000) suhecheng  (1000)     1473 2023-03-24 06:17:29.000000 cn2int-0.2.2/cn2int.egg-info/PKG-INFO
--rw-rw-r--   0 suhecheng  (1000) suhecheng  (1000)      231 2023-03-24 06:17:29.000000 cn2int-0.2.2/cn2int.egg-info/SOURCES.txt
--rw-rw-r--   0 suhecheng  (1000) suhecheng  (1000)        1 2023-03-24 06:17:29.000000 cn2int-0.2.2/cn2int.egg-info/dependency_links.txt
--rw-rw-r--   0 suhecheng  (1000) suhecheng  (1000)        7 2023-03-24 06:17:29.000000 cn2int-0.2.2/cn2int.egg-info/top_level.txt
--rw-rw-r--   0 suhecheng  (1000) suhecheng  (1000)       38 2023-03-24 06:17:29.890809 cn2int-0.2.2/setup.cfg
--rw-rw-r--   0 suhecheng  (1000) suhecheng  (1000)      868 2023-02-26 11:54:18.000000 cn2int-0.2.2/setup.py
--rw-rw-r--   0 suhecheng  (1000) suhecheng  (1000)    11638 2023-03-24 06:11:15.000000 cn2int-0.2.2/test.py
+drwxrwxr-x   0 suhecheng  (1000) suhecheng  (1000)        0 2023-05-26 01:51:48.704789 cn2int-0.2.3/
+-rwxrwxr-x   0 suhecheng  (1000) suhecheng  (1000)       38 2023-02-26 11:54:18.000000 cn2int-0.2.3/MANIFEST.in
+-rw-rw-r--   0 suhecheng  (1000) suhecheng  (1000)     1473 2023-05-26 01:51:48.704789 cn2int-0.2.3/PKG-INFO
+-rw-rw-r--   0 suhecheng  (1000) suhecheng  (1000)     1120 2023-02-26 11:54:18.000000 cn2int-0.2.3/README-PyPI.md
+-rw-rw-r--   0 suhecheng  (1000) suhecheng  (1000)     4336 2023-02-26 11:54:18.000000 cn2int-0.2.3/README.md
+drwxrwxr-x   0 suhecheng  (1000) suhecheng  (1000)        0 2023-05-26 01:51:48.704789 cn2int-0.2.3/cn2int/
+-rw-rw-r--   0 suhecheng  (1000) suhecheng  (1000)      191 2023-02-26 11:54:18.000000 cn2int-0.2.3/cn2int/__init__.py
+-rw-rw-r--   0 suhecheng  (1000) suhecheng  (1000)    17249 2023-05-26 01:50:29.000000 cn2int-0.2.3/cn2int/cn2int.py
+-rw-rw-r--   0 suhecheng  (1000) suhecheng  (1000)     1396 2023-04-27 09:02:40.000000 cn2int-0.2.3/cn2int/performance.py
+drwxrwxr-x   0 suhecheng  (1000) suhecheng  (1000)        0 2023-05-26 01:51:48.704789 cn2int-0.2.3/cn2int.egg-info/
+-rw-rw-r--   0 suhecheng  (1000) suhecheng  (1000)     1473 2023-05-26 01:51:48.000000 cn2int-0.2.3/cn2int.egg-info/PKG-INFO
+-rw-rw-r--   0 suhecheng  (1000) suhecheng  (1000)      231 2023-05-26 01:51:48.000000 cn2int-0.2.3/cn2int.egg-info/SOURCES.txt
+-rw-rw-r--   0 suhecheng  (1000) suhecheng  (1000)        1 2023-05-26 01:51:48.000000 cn2int-0.2.3/cn2int.egg-info/dependency_links.txt
+-rw-rw-r--   0 suhecheng  (1000) suhecheng  (1000)        7 2023-05-26 01:51:48.000000 cn2int-0.2.3/cn2int.egg-info/top_level.txt
+-rw-rw-r--   0 suhecheng  (1000) suhecheng  (1000)       38 2023-05-26 01:51:48.704789 cn2int-0.2.3/setup.cfg
+-rw-rw-r--   0 suhecheng  (1000) suhecheng  (1000)      868 2023-02-26 11:54:18.000000 cn2int-0.2.3/setup.py
+-rw-rw-r--   0 suhecheng  (1000) suhecheng  (1000)    11638 2023-03-24 06:11:15.000000 cn2int-0.2.3/test.py
```

### Comparing `cn2int-0.2.2/PKG-INFO` & `cn2int-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cn2int
-Version: 0.2.2
+Version: 0.2.3
 Summary: Conversion bettwen Chinese number and integer/float
 Home-page: https://github.com/citysu/cn2int
 Author: Hecheng Su
 Author-email: 2215523266@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cn2int-0.2.2/README-PyPI.md` & `cn2int-0.2.3/README-PyPI.md`

 * *Files identical despite different names*

### Comparing `cn2int-0.2.2/README.md` & `cn2int-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `cn2int-0.2.2/cn2int/cn2int.py` & `cn2int-0.2.3/cn2int/cn2int.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Author: suhecheng
 Home: https://github/citysu/cn2int
 """
 
 import re
 
 
-__version__ = "0.2.2"
+__version__ = "0.2.3"
 
 
 __all__ = [
     "int2roman", "roman2int",
     "int2chinese", "float2chinese", "chinese2int", "chinese2float"
     "convert2int"
 ]
@@ -416,66 +416,65 @@
         string: 中文数字. 如果返回None, 表示超出转换范围.
     """
     if number <= -1e12 or number >= 1e12:
         return None
 
     n, s = number, ""
     sign = ""
+    i = 0
 
     if enumeration:
         if lower:
             if use_upper_zero:
                 digits = Table.lower_traditional
             else:
                 digits = Table.lower_enumeration
         else:
             digits = Table.upper_enumeration
         if n < 0:
             sign = digits[-1]
             n = -n
         if n == 0:
             s = digits[0]
-        i = 0
         while n > 0:
             p = n % 10
             n //= 10
             s = digits[p] + s
             i += 1
-        if i < width:
-            s = digits[0] * (width - i) + s
+        if len(s) < width:
+            s = digits[0] * (width - len(s)) + s
     else:
         if lower:
             digits = Table.lower_traditional
             units = Table.lower_uint
             delimiters = Table.lower_delimiter
         else:
-            digits = Table.lower_traditional
+            digits = Table.upper_traditional
             units = Table.upper_unit
             delimiters = Table.upper_delimiter
         if n < 0:
             sign = digits[-1]
             n = -n
         if n == 0:
             s = digits[0]
-        i = 0
         while n > 0:
             p = n % 10000
             n //= 10000
             delimiter = delimiters[0] if p == 0 else delimiters[i]
             s_small = small2chinese(p, delimiter, digits, units, use_liang)
             s = s_small + delimiter + s
             if n != 0:
                 s = chinese_fill_zero(s, p)
             i += 1
         if use_simple_ten:
             s = chinese_simple_ten(s, p)
         if use_simple_zero_tail:
             s = chinese_simple_zero_tail(s, lower)
-        if i < width:
-            s = digits[0] * (width - i) + s
+        if len(s) < width:
+            s = digits[0] * (width - len(s)) + s
     s = sign + s
     return s
 
 
 def float2chinese(number, lower=True, precision=6,
                   use_liang=False,
                   use_simple_ten=False,
```

### Comparing `cn2int-0.2.2/cn2int/performance.py` & `cn2int-0.2.3/cn2int/performance.py`

 * *Files identical despite different names*

### Comparing `cn2int-0.2.2/cn2int.egg-info/PKG-INFO` & `cn2int-0.2.3/cn2int.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cn2int
-Version: 0.2.2
+Version: 0.2.3
 Summary: Conversion bettwen Chinese number and integer/float
 Home-page: https://github.com/citysu/cn2int
 Author: Hecheng Su
 Author-email: 2215523266@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cn2int-0.2.2/setup.py` & `cn2int-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `cn2int-0.2.2/test.py` & `cn2int-0.2.3/test.py`

 * *Files identical despite different names*

