# Comparing `tmp/gmsofttest-0.0.6.tar.gz` & `tmp/gmsofttest-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gmsofttest-0.0.6.tar", last modified: Wed May 24 02:48:52 2023, max compression
+gzip compressed data, was "dist\gmsofttest-0.0.7.tar", last modified: Fri May 26 06:02:06 2023, max compression
```

## Comparing `gmsofttest-0.0.6.tar` & `gmsofttest-0.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 02:48:52.000000 gmsofttest-0.0.6/
--rw-rw-rw-   0        0        0     1091 2023-02-11 08:11:24.000000 gmsofttest-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     1271 2023-05-24 02:48:52.000000 gmsofttest-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      777 2023-05-24 02:45:32.000000 gmsofttest-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-05-24 02:48:52.000000 gmsofttest-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      803 2023-05-24 02:48:48.000000 gmsofttest-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-24 02:48:52.000000 gmsofttest-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-05-24 02:48:52.000000 gmsofttest-0.0.6/src/gmsofttest/
--rw-rw-rw-   0        0        0      125 2023-02-11 07:45:36.000000 gmsofttest-0.0.6/src/gmsofttest/__init__.py
--rw-rw-rw-   0        0        0    89848 2023-04-22 07:37:37.000000 gmsofttest-0.0.6/src/gmsofttest/china_address.py
--rw-rw-rw-   0        0        0     2965 2023-05-23 08:08:28.000000 gmsofttest-0.0.6/src/gmsofttest/gm_assert_utils.py
--rw-rw-rw-   0        0        0     4867 2023-05-23 08:36:05.000000 gmsofttest-0.0.6/src/gmsofttest/gm_excel_utils.py
--rw-rw-rw-   0        0        0     2576 2023-05-20 08:22:39.000000 gmsofttest-0.0.6/src/gmsofttest/gm_parse_response_utils.py
--rw-rw-rw-   0        0        0     2197 2023-05-20 08:15:01.000000 gmsofttest-0.0.6/src/gmsofttest/gm_randomdata_utils.py
--rw-rw-rw-   0        0        0     1806 2023-05-24 02:44:27.000000 gmsofttest-0.0.6/src/gmsofttest/gm_request_utils.py
--rw-rw-rw-   0        0        0    11797 2023-05-23 08:03:00.000000 gmsofttest-0.0.6/src/gmsofttest/gm_sqlconn_utils.py
--rw-rw-rw-   0        0        0      877 2023-05-23 08:40:42.000000 gmsofttest-0.0.6/src/gmsofttest/gm_stock_enum.py
--rw-rw-rw-   0        0        0     3109 2023-05-20 08:15:01.000000 gmsofttest-0.0.6/src/gmsofttest/gm_timestamp_utils.py
--rw-rw-rw-   0        0        0     2196 2023-05-23 08:01:45.000000 gmsofttest-0.0.6/src/gmsofttest/gm_yaml_process_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-24 02:48:52.000000 gmsofttest-0.0.6/src/gmsofttest.egg-info/
--rw-rw-rw-   0        0        0     1271 2023-05-24 02:48:52.000000 gmsofttest-0.0.6/src/gmsofttest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      563 2023-05-24 02:48:52.000000 gmsofttest-0.0.6/src/gmsofttest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 02:48:52.000000 gmsofttest-0.0.6/src/gmsofttest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-24 02:48:52.000000 gmsofttest-0.0.6/src/gmsofttest.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-26 06:02:06.000000 gmsofttest-0.0.7/
+-rw-rw-rw-   0        0        0     1091 2023-02-11 08:11:24.000000 gmsofttest-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     1271 2023-05-26 06:02:06.000000 gmsofttest-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      777 2023-05-24 02:45:32.000000 gmsofttest-0.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-26 06:02:06.000000 gmsofttest-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      803 2023-05-26 06:01:45.000000 gmsofttest-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 06:02:06.000000 gmsofttest-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-05-26 06:02:06.000000 gmsofttest-0.0.7/src/gmsofttest/
+-rw-rw-rw-   0        0        0      125 2023-02-11 07:45:36.000000 gmsofttest-0.0.7/src/gmsofttest/__init__.py
+-rw-rw-rw-   0        0        0    89848 2023-04-22 07:37:37.000000 gmsofttest-0.0.7/src/gmsofttest/china_address.py
+-rw-rw-rw-   0        0        0     3327 2023-05-24 03:07:23.000000 gmsofttest-0.0.7/src/gmsofttest/gm_assert_utils.py
+-rw-rw-rw-   0        0        0     4867 2023-05-23 08:36:05.000000 gmsofttest-0.0.7/src/gmsofttest/gm_excel_utils.py
+-rw-rw-rw-   0        0        0     3369 2023-05-26 05:38:26.000000 gmsofttest-0.0.7/src/gmsofttest/gm_parse_response_utils.py
+-rw-rw-rw-   0        0        0     2197 2023-05-20 08:15:01.000000 gmsofttest-0.0.7/src/gmsofttest/gm_randomdata_utils.py
+-rw-rw-rw-   0        0        0     1806 2023-05-24 02:44:27.000000 gmsofttest-0.0.7/src/gmsofttest/gm_request_utils.py
+-rw-rw-rw-   0        0        0    11797 2023-05-23 08:03:00.000000 gmsofttest-0.0.7/src/gmsofttest/gm_sqlconn_utils.py
+-rw-rw-rw-   0        0        0      877 2023-05-23 08:40:42.000000 gmsofttest-0.0.7/src/gmsofttest/gm_stock_enum.py
+-rw-rw-rw-   0        0        0     3109 2023-05-20 08:15:01.000000 gmsofttest-0.0.7/src/gmsofttest/gm_timestamp_utils.py
+-rw-rw-rw-   0        0        0     2196 2023-05-23 08:01:45.000000 gmsofttest-0.0.7/src/gmsofttest/gm_yaml_process_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-26 06:02:06.000000 gmsofttest-0.0.7/src/gmsofttest.egg-info/
+-rw-rw-rw-   0        0        0     1271 2023-05-26 06:02:05.000000 gmsofttest-0.0.7/src/gmsofttest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      563 2023-05-26 06:02:06.000000 gmsofttest-0.0.7/src/gmsofttest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 06:02:05.000000 gmsofttest-0.0.7/src/gmsofttest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-26 06:02:05.000000 gmsofttest-0.0.7/src/gmsofttest.egg-info/top_level.txt
```

### Comparing `gmsofttest-0.0.6/LICENSE` & `gmsofttest-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gmsofttest-0.0.6/PKG-INFO` & `gmsofttest-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmsofttest
-Version: 0.0.6
+Version: 0.0.7
 Summary: 大家软件内部测试技术线支撑工具
 Home-page: https://www.gec123.com
 Author: ronaldsu
 Author-email: uph4rmt@dingtalk.com
 Project-URL: Bug Tracker, https://www.gpwbeta.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gmsofttest-0.0.6/README.md` & `gmsofttest-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `gmsofttest-0.0.6/setup.py` & `gmsofttest-0.0.7/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="gmsofttest",
-    version="0.0.6",
+    version="0.0.7",
     author="ronaldsu",
     author_email="uph4rmt@dingtalk.com",
     description="大家软件内部测试技术线支撑工具",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.gec123.com",
     project_urls={
```

### Comparing `gmsofttest-0.0.6/src/gmsofttest/china_address.py` & `gmsofttest-0.0.7/src/gmsofttest/china_address.py`

 * *Files identical despite different names*

### Comparing `gmsofttest-0.0.6/src/gmsofttest/gm_assert_utils.py` & `gmsofttest-0.0.7/src/gmsofttest/gm_assert_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -71,8 +71,16 @@
     except (ValueError, TypeError):
         return default
 
 
 if __name__ == '__main__':
     gm_assert_equal(2, '2', int)  # 将第1和第2个参数转换成int型比较
     gm_assert_multiple_values_equal([3, 3, '3'], int)
-    gm_assert_not_in("hello", "hello world", str)
+    first_value = 'ok'
+    # second_value = '{"code":20000,"message":"ok","description":"","data":{"todoRationalNum":18,"todoAuditNum":1,"todoEleGuaranteeNum":1,"todoAbolishEleGuaranteeNum":0}}'
+    types = 'str'
+    second_value = 'okok'
+    # gm_assert_in(first_value,second_value, types)
+    # print(second_value)
+    # print(type(second_value))
+    gm_assert_equal('str', 'str1', str)
+    # print(s)
```

### Comparing `gmsofttest-0.0.6/src/gmsofttest/gm_excel_utils.py` & `gmsofttest-0.0.7/src/gmsofttest/gm_excel_utils.py`

 * *Files identical despite different names*

### Comparing `gmsofttest-0.0.6/src/gmsofttest/gm_parse_response_utils.py` & `gmsofttest-0.0.7/src/gmsofttest/gm_parse_response_utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,17 +7,28 @@
 """
 
 import json
 from jsonpath import jsonpath
 
 def extract_json_data(text, jsonpath_expression):
     """使用jsonpath工具类解析请求返回值"""
-    json_text = json.loads(text)  # 转换requests请求返回string为python对象
-    data = jsonpath(json_text, jsonpath_expression)  # 使用jsonpath进行解析
-    return data
+    try:
+        # 判断是否
+        if isinstance(text, dict):
+            data = jsonpath(text, jsonpath_expression)  # 使用jsonpath进行解析
+        elif isinstance(text, str):
+            data = jsonpath(text, jsonpath_expression)  # 使用jsonpath进行解析
+        elif isinstance(text, list):
+            data = jsonpath(text, jsonpath_expression)  # 使用jsonpath进行解析
+        else:
+            json_text = json.loads(text)  # 转换requests请求返回string为python对象
+            data = jsonpath(json_text, jsonpath_expression)  # 使用jsonpath进行解析
+        return data
+    except TypeError as e:
+        print("入参{}的类型错误，请检查,{}".format(text, e))
 
 
 if __name__ == '__main__':
     json_data = """
     { "store": {
         "book": [
           { "category": "reference",
@@ -67,7 +78,13 @@
     print(price_book)
     print(category)
     print(price)
     print(three_price)
     print(last_book)
     print(type(last_book))
     print(jsonpath.jsonpath(json_data, '$..book[-2:]'))  # 最后两本书)
+
+    s = """{"code":20000,"message":"ok","description":"",
+    "data":{"todoRationalNum":18,"todoAuditNum":1,"todoEleGuaranteeNum":1,"todoAbolishEleGuaranteeNum":0}}"""
+    s = json.loads(s)
+    s1 = jsonpath.jsonpath(s, '$.code')
+    print(s1[0])
```

### Comparing `gmsofttest-0.0.6/src/gmsofttest/gm_randomdata_utils.py` & `gmsofttest-0.0.7/src/gmsofttest/gm_randomdata_utils.py`

 * *Files identical despite different names*

### Comparing `gmsofttest-0.0.6/src/gmsofttest/gm_request_utils.py` & `gmsofttest-0.0.7/src/gmsofttest/gm_request_utils.py`

 * *Files identical despite different names*

### Comparing `gmsofttest-0.0.6/src/gmsofttest/gm_sqlconn_utils.py` & `gmsofttest-0.0.7/src/gmsofttest/gm_sqlconn_utils.py`

 * *Files identical despite different names*

### Comparing `gmsofttest-0.0.6/src/gmsofttest/gm_stock_enum.py` & `gmsofttest-0.0.7/src/gmsofttest/gm_stock_enum.py`

 * *Files identical despite different names*

### Comparing `gmsofttest-0.0.6/src/gmsofttest/gm_timestamp_utils.py` & `gmsofttest-0.0.7/src/gmsofttest/gm_timestamp_utils.py`

 * *Files identical despite different names*

### Comparing `gmsofttest-0.0.6/src/gmsofttest/gm_yaml_process_utils.py` & `gmsofttest-0.0.7/src/gmsofttest/gm_yaml_process_utils.py`

 * *Files identical despite different names*

### Comparing `gmsofttest-0.0.6/src/gmsofttest.egg-info/PKG-INFO` & `gmsofttest-0.0.7/src/gmsofttest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmsofttest
-Version: 0.0.6
+Version: 0.0.7
 Summary: 大家软件内部测试技术线支撑工具
 Home-page: https://www.gec123.com
 Author: ronaldsu
 Author-email: uph4rmt@dingtalk.com
 Project-URL: Bug Tracker, https://www.gpwbeta.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gmsofttest-0.0.6/src/gmsofttest.egg-info/SOURCES.txt` & `gmsofttest-0.0.7/src/gmsofttest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

