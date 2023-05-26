# Comparing `tmp/langchain_wenxin-0.2.0.tar.gz` & `tmp/langchain_wenxin-0.3.0.tar.gz`

## Comparing `langchain_wenxin-0.2.0.tar` & `langchain_wenxin-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 langchain_wenxin-0.2.0/src/langchain_wenxin/__about__.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 langchain_wenxin-0.2.0/src/langchain_wenxin/__init__.py
--rw-r--r--   0        0        0    13474 2020-02-02 00:00:00.000000 langchain_wenxin-0.2.0/src/langchain_wenxin/llms.py
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 langchain_wenxin-0.2.0/src/langchain_wenxin/retrievers.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 langchain_wenxin-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 langchain_wenxin-0.2.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 langchain_wenxin-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 langchain_wenxin-0.2.0/README.md
--rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 langchain_wenxin-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 langchain_wenxin-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 langchain_wenxin-0.3.0/src/langchain_wenxin/__about__.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 langchain_wenxin-0.3.0/src/langchain_wenxin/__init__.py
+-rw-r--r--   0        0        0    13474 2020-02-02 00:00:00.000000 langchain_wenxin-0.3.0/src/langchain_wenxin/llms.py
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 langchain_wenxin-0.3.0/src/langchain_wenxin/retrievers.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 langchain_wenxin-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 langchain_wenxin-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 langchain_wenxin-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 langchain_wenxin-0.3.0/README.md
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 langchain_wenxin-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 langchain_wenxin-0.3.0/PKG-INFO
```

### Comparing `langchain_wenxin-0.2.0/src/langchain_wenxin/llms.py` & `langchain_wenxin-0.3.0/src/langchain_wenxin/llms.py`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.2.0/src/langchain_wenxin/retrievers.py` & `langchain_wenxin-0.3.0/src/langchain_wenxin/retrievers.py`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.2.0/.gitignore` & `langchain_wenxin-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.2.0/LICENSE.txt` & `langchain_wenxin-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.2.0/README.md` & `langchain_wenxin-0.3.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -27,19 +27,23 @@
 export BAIDU_SECRET_KEY="xxxxx"
 ```
 
 ```python3
 from langchain_wenxin.llms import Wenxin,ChatWenxin
 
 # Wenxin model
-llm = Wenxin()
+llm = Wenxin(model="eb-instant")
 print(llm("你好"))
 
 # Wenxin chat model
 from langchain.schema import HumanMessage
 llm = ChatWenxin()
 print(llm([HumanMessage(content="你好")]))
 ```
 
+Support models:
+- wenxin: 文心一言
+- eb-instant: 文心 EB-Lite
+
 ## License
 
 `langchain-wenxin` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

### Comparing `langchain_wenxin-0.2.0/pyproject.toml` & `langchain_wenxin-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "langchain>=0.0.175",
   "requests",
-  "sseclient",
+  "sseclient-py",
 ]
 
 [project.urls]
 Documentation = "https://github.com/unknown/langchain-wenxin#readme"
 Issues = "https://github.com/unknown/langchain-wenxin/issues"
 Source = "https://github.com/unknown/langchain-wenxin"
```

### Comparing `langchain_wenxin-0.2.0/PKG-INFO` & `langchain_wenxin-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-wenxin
-Version: 0.2.0
+Version: 0.3.0
 Project-URL: Documentation, https://github.com/unknown/langchain-wenxin#readme
 Project-URL: Issues, https://github.com/unknown/langchain-wenxin/issues
 Project-URL: Source, https://github.com/unknown/langchain-wenxin
 Author-email: Tao Yang <swulling@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Requires-Dist: langchain>=0.0.175
 Requires-Dist: requests
-Requires-Dist: sseclient
+Requires-Dist: sseclient-py
 Description-Content-Type: text/markdown
 
 # langchain-wenxin - Langchain Baidu WENXINWORKSHOP wrapper
 
 [![PyPI - Version](https://img.shields.io/pypi/v/langchain-wenxin.svg)](https://pypi.org/project/langchain-wenxin)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/langchain-wenxin.svg)](https://pypi.org/project/langchain-wenxin)
 
@@ -51,19 +51,23 @@
 export BAIDU_SECRET_KEY="xxxxx"
 ```
 
 ```python3
 from langchain_wenxin.llms import Wenxin,ChatWenxin
 
 # Wenxin model
-llm = Wenxin()
+llm = Wenxin(model="eb-instant")
 print(llm("你好"))
 
 # Wenxin chat model
 from langchain.schema import HumanMessage
 llm = ChatWenxin()
 print(llm([HumanMessage(content="你好")]))
 ```
 
+Support models:
+- wenxin: 文心一言
+- eb-instant: 文心 EB-Lite
+
 ## License
 
 `langchain-wenxin` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

