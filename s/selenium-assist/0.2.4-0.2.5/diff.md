# Comparing `tmp/selenium_assist-0.2.4.tar.gz` & `tmp/selenium_assist-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium_assist-0.2.4.tar", last modified: Thu May 25 21:22:29 2023, max compression
+gzip compressed data, was "selenium_assist-0.2.5.tar", last modified: Thu May 25 22:49:10 2023, max compression
```

## Comparing `selenium_assist-0.2.4.tar` & `selenium_assist-0.2.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 mich      (1000) mich      (1000)        0 2023-05-25 21:22:29.374039 selenium_assist-0.2.4/
--rw-rw-r--   0 mich      (1000) mich      (1000)     1071 2023-04-05 22:02:25.000000 selenium_assist-0.2.4/LICENSE
--rw-rw-r--   0 mich      (1000) mich      (1000)      831 2023-05-25 21:22:29.374039 selenium_assist-0.2.4/PKG-INFO
--rw-rw-r--   0 mich      (1000) mich      (1000)       71 2023-05-12 23:13:38.000000 selenium_assist-0.2.4/README.md
-drwxrwxr-x   0 mich      (1000) mich      (1000)        0 2023-05-25 21:22:29.374039 selenium_assist-0.2.4/selenium_assist/
--rw-rw-r--   0 mich      (1000) mich      (1000)      458 2023-05-12 23:13:37.000000 selenium_assist-0.2.4/selenium_assist/__init__.py
--rw-rw-r--   0 mich      (1000) mich      (1000)     1308 2023-05-25 21:15:18.000000 selenium_assist-0.2.4/selenium_assist/helpers.py
--rw-rw-r--   0 mich      (1000) mich      (1000)     1125 2023-05-17 20:55:52.000000 selenium_assist-0.2.4/selenium_assist/managers.py
--rw-rw-r--   0 mich      (1000) mich      (1000)     3847 2023-05-12 23:13:37.000000 selenium_assist-0.2.4/selenium_assist/wrappers.py
-drwxrwxr-x   0 mich      (1000) mich      (1000)        0 2023-05-25 21:22:29.374039 selenium_assist-0.2.4/selenium_assist.egg-info/
--rw-rw-r--   0 mich      (1000) mich      (1000)      831 2023-05-25 21:22:29.000000 selenium_assist-0.2.4/selenium_assist.egg-info/PKG-INFO
--rw-rw-r--   0 mich      (1000) mich      (1000)      341 2023-05-25 21:22:29.000000 selenium_assist-0.2.4/selenium_assist.egg-info/SOURCES.txt
--rw-rw-r--   0 mich      (1000) mich      (1000)        1 2023-05-25 21:22:29.000000 selenium_assist-0.2.4/selenium_assist.egg-info/dependency_links.txt
--rw-rw-r--   0 mich      (1000) mich      (1000)       39 2023-05-25 21:22:29.000000 selenium_assist-0.2.4/selenium_assist.egg-info/requires.txt
--rw-rw-r--   0 mich      (1000) mich      (1000)       16 2023-05-25 21:22:29.000000 selenium_assist-0.2.4/selenium_assist.egg-info/top_level.txt
--rw-rw-r--   0 mich      (1000) mich      (1000)       79 2023-05-25 21:22:29.374039 selenium_assist-0.2.4/setup.cfg
--rw-rw-r--   0 mich      (1000) mich      (1000)     1097 2023-05-25 21:18:06.000000 selenium_assist-0.2.4/setup.py
+drwxrwxr-x   0 mich      (1000) mich      (1000)        0 2023-05-25 22:49:10.847734 selenium_assist-0.2.5/
+-rw-rw-r--   0 mich      (1000) mich      (1000)     1071 2023-04-05 22:02:25.000000 selenium_assist-0.2.5/LICENSE
+-rw-rw-r--   0 mich      (1000) mich      (1000)      831 2023-05-25 22:49:10.847734 selenium_assist-0.2.5/PKG-INFO
+-rw-rw-r--   0 mich      (1000) mich      (1000)       71 2023-05-12 23:13:38.000000 selenium_assist-0.2.5/README.md
+drwxrwxr-x   0 mich      (1000) mich      (1000)        0 2023-05-25 22:49:10.847734 selenium_assist-0.2.5/selenium_assist/
+-rw-rw-r--   0 mich      (1000) mich      (1000)      458 2023-05-12 23:13:37.000000 selenium_assist-0.2.5/selenium_assist/__init__.py
+-rw-rw-r--   0 mich      (1000) mich      (1000)     1308 2023-05-25 21:15:18.000000 selenium_assist-0.2.5/selenium_assist/helpers.py
+-rw-rw-r--   0 mich      (1000) mich      (1000)     1125 2023-05-17 20:55:52.000000 selenium_assist-0.2.5/selenium_assist/managers.py
+-rw-rw-r--   0 mich      (1000) mich      (1000)     3904 2023-05-25 22:43:54.000000 selenium_assist-0.2.5/selenium_assist/wrappers.py
+drwxrwxr-x   0 mich      (1000) mich      (1000)        0 2023-05-25 22:49:10.847734 selenium_assist-0.2.5/selenium_assist.egg-info/
+-rw-rw-r--   0 mich      (1000) mich      (1000)      831 2023-05-25 22:49:10.000000 selenium_assist-0.2.5/selenium_assist.egg-info/PKG-INFO
+-rw-rw-r--   0 mich      (1000) mich      (1000)      341 2023-05-25 22:49:10.000000 selenium_assist-0.2.5/selenium_assist.egg-info/SOURCES.txt
+-rw-rw-r--   0 mich      (1000) mich      (1000)        1 2023-05-25 22:49:10.000000 selenium_assist-0.2.5/selenium_assist.egg-info/dependency_links.txt
+-rw-rw-r--   0 mich      (1000) mich      (1000)       39 2023-05-25 22:49:10.000000 selenium_assist-0.2.5/selenium_assist.egg-info/requires.txt
+-rw-rw-r--   0 mich      (1000) mich      (1000)       16 2023-05-25 22:49:10.000000 selenium_assist-0.2.5/selenium_assist.egg-info/top_level.txt
+-rw-rw-r--   0 mich      (1000) mich      (1000)       79 2023-05-25 22:49:10.847734 selenium_assist-0.2.5/setup.cfg
+-rw-rw-r--   0 mich      (1000) mich      (1000)     1097 2023-05-25 22:48:36.000000 selenium_assist-0.2.5/setup.py
```

### Comparing `selenium_assist-0.2.4/LICENSE` & `selenium_assist-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `selenium_assist-0.2.4/PKG-INFO` & `selenium_assist-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: selenium_assist
-Version: 0.2.4
+Version: 0.2.5
 Summary: Helper functions for selenium
 Home-page: https://github.com/ivanmicetic/selenium-assist
-Download-URL: https://github.com/ivanmicetic/selenium-assist/archive/refs/tags/v0.2.4.tar.gz
+Download-URL: https://github.com/ivanmicetic/selenium-assist/archive/refs/tags/v0.2.5.tar.gz
 Author: Ivan Mičetić
 Author-email: ivan.micetic@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/ivanmicetic/selenium-assist/issues
 Keywords: pypi,selenium_assist
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `selenium_assist-0.2.4/selenium_assist/helpers.py` & `selenium_assist-0.2.5/selenium_assist/helpers.py`

 * *Files identical despite different names*

### Comparing `selenium_assist-0.2.4/selenium_assist/managers.py` & `selenium_assist-0.2.5/selenium_assist/managers.py`

 * *Files identical despite different names*

### Comparing `selenium_assist-0.2.4/selenium_assist/wrappers.py` & `selenium_assist-0.2.5/selenium_assist/wrappers.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,25 +52,26 @@
     try:
         driver.find_element_by_xpath(xpath).click()
     except (ElementClickInterceptedException, StaleElementReferenceException):
         dump_and_exit("Cannot click on element, dumping source and exiting!", driver)
     return
 
 
-def send_keys(task, xpath, keys, driver, extra_timeout=5):
+def send_keys(task, xpath, keys, driver, extra_timeout=5, skip_check=False):
     logging.debug(task)
     try:
         element_present = EC.element_to_be_clickable((By.XPATH, xpath))
         WebDriverWait(driver, extra_timeout).until(element_present)
         element = driver.find_element_by_xpath(xpath)
         element.clear()
         element.send_keys(keys)
-        WebDriverWait(driver, extra_timeout).until(
-            lambda browser: element.get_attribute("value") == keys
-        )
+        if not skip_check:
+            WebDriverWait(driver, extra_timeout).until(
+                lambda browser: element.get_attribute("value") == keys
+            )
     except Exception as e:
         dump_and_exit(
             "Cannot send keys on element, dumping source and exiting!", driver, exc=e
         )
     return
```

### Comparing `selenium_assist-0.2.4/selenium_assist.egg-info/PKG-INFO` & `selenium_assist-0.2.5/selenium_assist.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: selenium-assist
-Version: 0.2.4
+Version: 0.2.5
 Summary: Helper functions for selenium
 Home-page: https://github.com/ivanmicetic/selenium-assist
-Download-URL: https://github.com/ivanmicetic/selenium-assist/archive/refs/tags/v0.2.4.tar.gz
+Download-URL: https://github.com/ivanmicetic/selenium-assist/archive/refs/tags/v0.2.5.tar.gz
 Author: Ivan Mičetić
 Author-email: ivan.micetic@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/ivanmicetic/selenium-assist/issues
 Keywords: pypi,selenium_assist
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `selenium_assist-0.2.4/setup.py` & `selenium_assist-0.2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="selenium_assist",
-    version="0.2.4",
+    version="0.2.5",
     author="Ivan Mičetić",
     author_email="ivan.micetic@gmail.com",
     description="Helper functions for selenium",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ivanmicetic/selenium-assist",
     project_urls={
@@ -22,9 +22,9 @@
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
     ],
-    download_url="https://github.com/ivanmicetic/selenium-assist/archive/refs/tags/v0.2.4.tar.gz"
+    download_url="https://github.com/ivanmicetic/selenium-assist/archive/refs/tags/v0.2.5.tar.gz"
 )
```

