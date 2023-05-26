# Comparing `tmp/caqui-1.0.3.tar.gz` & `tmp/caqui-1.0.4.tar.gz`

## Comparing `caqui-1.0.3.tar` & `caqui-1.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 caqui-1.0.3/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 caqui-1.0.3/sample.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 caqui-1.0.3/test-requirements.txt
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 caqui-1.0.3/.github/workflows/python-app.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 caqui-1.0.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 caqui-1.0.3/.vscode/settings.json
--rw-r--r--   0        0        0    43559 2020-02-02 00:00:00.000000 caqui-1.0.3/caqui/__init__.py
--rw-r--r--   0        0        0     4237 2020-02-02 00:00:00.000000 caqui-1.0.3/caqui/asynchronous.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 caqui-1.0.3/caqui/constants.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 caqui-1.0.3/caqui/exceptions.py
--rw-r--r--   0        0        0     4195 2020-02-02 00:00:00.000000 caqui-1.0.3/caqui/synchronous.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 caqui-1.0.3/tests/__init__.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 caqui-1.0.3/tests/constants.py
--rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 caqui-1.0.3/tests/fake_responses.py
--rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 caqui-1.0.3/tests/feature/test_functions.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 caqui-1.0.3/tests/html/playground.html
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 caqui-1.0.3/tests/integration/test_async_scenarios.py
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 caqui-1.0.3/tests/integration/test_sync_scenarios.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 caqui-1.0.3/tests/unit/__initi__.py
--rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 caqui-1.0.3/tests/unit/test_async_unit.py
--rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 caqui-1.0.3/tests/unit/test_sync_unit.py
--rwxr-xr-x   0        0        0       58 2020-02-02 00:00:00.000000 caqui-1.0.3/utils/publish.sh
--rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 caqui-1.0.3/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 caqui-1.0.3/LICENSE
--rw-r--r--   0        0        0     8833 2020-02-02 00:00:00.000000 caqui-1.0.3/README.md
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 caqui-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     9434 2020-02-02 00:00:00.000000 caqui-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 caqui-1.0.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 caqui-1.0.4/sample.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 caqui-1.0.4/test-requirements.txt
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 caqui-1.0.4/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 caqui-1.0.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 caqui-1.0.4/.vscode/settings.json
+-rw-r--r--   0        0        0    43559 2020-02-02 00:00:00.000000 caqui-1.0.4/caqui/__init__.py
+-rw-r--r--   0        0        0     4246 2020-02-02 00:00:00.000000 caqui-1.0.4/caqui/asynchronous.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 caqui-1.0.4/caqui/constants.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 caqui-1.0.4/caqui/exceptions.py
+-rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 caqui-1.0.4/caqui/synchronous.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 caqui-1.0.4/tests/__init__.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 caqui-1.0.4/tests/constants.py
+-rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 caqui-1.0.4/tests/fake_responses.py
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 caqui-1.0.4/tests/test_sniffer.py
+-rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 caqui-1.0.4/tests/feature/test_functions.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 caqui-1.0.4/tests/html/playground.html
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 caqui-1.0.4/tests/integration/test_async_scenarios.py
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 caqui-1.0.4/tests/integration/test_sync_scenarios.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 caqui-1.0.4/tests/unit/__initi__.py
+-rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 caqui-1.0.4/tests/unit/test_async_unit.py
+-rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 caqui-1.0.4/tests/unit/test_sync_unit.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 caqui-1.0.4/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 caqui-1.0.4/LICENSE
+-rw-r--r--   0        0        0     8833 2020-02-02 00:00:00.000000 caqui-1.0.4/README.md
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 caqui-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     9434 2020-02-02 00:00:00.000000 caqui-1.0.4/PKG-INFO
```

### Comparing `caqui-1.0.3/CODE_OF_CONDUCT.md` & `caqui-1.0.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `caqui-1.0.3/sample.py` & `caqui-1.0.4/sample.py`

 * *Files identical despite different names*

### Comparing `caqui-1.0.3/.github/workflows/python-app.yml` & `caqui-1.0.4/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `caqui-1.0.3/.github/workflows/python-publish.yml` & `caqui-1.0.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `caqui-1.0.3/caqui/__init__.py` & `caqui-1.0.4/caqui/__init__.py`

 * *Files identical despite different names*

### Comparing `caqui-1.0.3/caqui/asynchronous.py` & `caqui-1.0.4/caqui/asynchronous.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,17 +22,17 @@
         return [x.get("ELEMENT") for x in response.get("value")]
     except Exception as error:
         raise WebDriverError(
             f"Failed to find element by '{locator_type}'-'{locator_value}'."
         ) from error
 
 
-async def get_property_value(driver_url, session, element):
+async def get_property(driver_url, session, element, property):
     try:
-        url = f"{driver_url}/session/{session}/element/{element}/property/value"
+        url = f"{driver_url}/session/{session}/element/{element}/property/{property}"
         async with aiohttp.ClientSession() as session:
             async with session.get(url, headers=HEADERS) as resp:
                 response = await resp.json()
                 return response.get("value")
     except Exception as error:
         raise WebDriverError("Failed to get value from element.") from error
```

### Comparing `caqui-1.0.3/caqui/synchronous.py` & `caqui-1.0.4/caqui/synchronous.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,17 +43,17 @@
         return [x.get("ELEMENT") for x in response.get("value")]
     except Exception as error:
         raise WebDriverError(
             f"Failed to find elements by '{locator_type}'-'{locator_value}'."
         ) from error
 
 
-def get_property_value(driver_url, session, element):
+def get_property(driver_url, session, element, property):
     try:
-        url = f"{driver_url}/session/{session}/element/{element}/property/value"
+        url = f"{driver_url}/session/{session}/element/{element}/property/{property}"
         response = __get(url, {})
         return response.get("value")
     except Exception as error:
         raise WebDriverError("Failed to get value from element.") from error
 
 
 def go_to_page(driver_url, session, page_url):
```

### Comparing `caqui-1.0.3/tests/fake_responses.py` & `caqui-1.0.4/tests/fake_responses.py`

 * *Files identical despite different names*

### Comparing `caqui-1.0.3/tests/feature/test_functions.py` & `caqui-1.0.4/tests/feature/test_functions.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,25 +37,28 @@
     )
 
     assert len(elements) > 0
     assert len(async_elements) > 0
 
 
 @mark.asyncio
-async def test_get_property_value(__setup):
+async def test_get_property(__setup):
     driver_url, session = __setup
     text = "any_value"
     locator_type = "xpath"
     locator_value = "//input"
+    property = "value"
 
     element = synchronous.find_element(driver_url, session, locator_type, locator_value)
     synchronous.send_keys(driver_url, session, element, text)
 
-    assert synchronous.get_property_value(driver_url, session, element) == text
-    assert await asynchronous.get_property_value(driver_url, session, element) == text
+    assert synchronous.get_property(driver_url, session, element, property) == text
+    assert (
+        await asynchronous.get_property(driver_url, session, element, property) == text
+    )
 
 
 @mark.asyncio
 async def test_get_text(__setup):
     driver_url, session = __setup
     expected = "end"
     locator_type = "xpath"
```

### Comparing `caqui-1.0.3/tests/html/playground.html` & `caqui-1.0.4/tests/html/playground.html`

 * *Files 27% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 
 <body>
     <h1>Basic page</h1>
     <p> This is a sample page to be used to sanity check </p>
     <input id="input">
     <button id="button" onclick="myFunction(this, 'red')">test</button>
     <p id="end">end</p>
-    <a src="http://any1.com" id="a1">any1.com</a>
-    <a src="http://any2.com" id="a2">any2.com</a>
-    <a src="http://any3.com" id="a3">any3.com</a>
-    <a src="http://any4.com" id="a4">any4.com</a>
+    <a href="http://any1.com" id="a1">any1.com</a>
+    <a href="http://any2.com" id="a2">any2.com</a>
+    <a href="http://any3.com" id="a3">any3.com</a>
+    <a href="http://any4.com" id="a4">any4.com</a>
 
     <script>
         function myFunction(element, color) {
             element.style.color = color;
         }
     </script>
 </body>
```

### Comparing `caqui-1.0.3/tests/integration/test_async_scenarios.py` & `caqui-1.0.4/tests/integration/test_async_scenarios.py`

 * *Files identical despite different names*

### Comparing `caqui-1.0.3/tests/unit/test_async_unit.py` & `caqui-1.0.4/tests/unit/test_async_unit.py`

 * *Files identical despite different names*

### Comparing `caqui-1.0.3/tests/unit/test_sync_unit.py` & `caqui-1.0.4/tests/unit/test_sync_unit.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     find_element,
     get_session,
     click,
     send_keys,
     get_text,
     close_session,
     go_to_page,
-    get_property_value,
+    get_property,
     find_elements,
 )
 from tests.fake_responses import (
     FIND_ELEMENT,
     GET_SESSION,
     CLICK,
     GET_TEXT,
@@ -40,20 +40,21 @@
     elements = find_elements(driver_url, session, locator_type, locator_value)
 
     assert element in elements
     assert len(elements) == 3
 
 
 @patch("requests.request", return_value=GET_PROPERTY_VALUE)
-def test_get_property_value(*args):
+def test_get_property(*args):
     driver_url, session, _ = __setup()
     element = "any"
+    property = "value"
     expected = "any_value"
 
-    assert get_property_value(driver_url, session, element) == expected
+    assert get_property(driver_url, session, element, property) == expected
 
 
 @patch("requests.request", return_value=GO_TO_PAGE)
 def test_go_to_page(*args):
     driver_url, session, _ = __setup()
     url = "http://any.com"
```

### Comparing `caqui-1.0.3/.gitignore` & `caqui-1.0.4/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-chromedriver*
-geckodriver*
-test_sniffer.py
-
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
```

### Comparing `caqui-1.0.3/LICENSE` & `caqui-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `caqui-1.0.3/README.md` & `caqui-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `caqui-1.0.3/pyproject.toml` & `caqui-1.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.setuptools.packages.find]
 include = ["caqui*"]
 exclude = ["tests*", "utils", ".vscode", ".git*", "dist"]
 
 [project]
 name = "caqui"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="Douglas Cardoso", email="noemail@noemail.com" },
 ]
 description = "Run asynchronous commands in WebDrivers"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `caqui-1.0.3/PKG-INFO` & `caqui-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caqui
-Version: 1.0.3
+Version: 1.0.4
 Summary: Run asynchronous commands in WebDrivers
 Project-URL: Homepage, https://github.com/douglasdcm/caqui
 Project-URL: Bug Tracker, https://github.com/douglasdcm/caqui/issues
 Author-email: Douglas Cardoso <noemail@noemail.com>
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: caqui Version: 1.0.3 Summary: Run asynchronous
+Metadata-Version: 2.1 Name: caqui Version: 1.0.4 Summary: Run asynchronous
 commands in WebDrivers Project-URL: Homepage, https://github.com/douglasdcm/
 caqui Project-URL: Bug Tracker, https://github.com/douglasdcm/caqui/issues
 Author-email: Douglas Cardoso
 noemail.com> License-File: LICENSE Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 3 Requires-
 Python: >=3.7 Requires-Dist: aiohttp Requires-Dist: requests Description-
```

