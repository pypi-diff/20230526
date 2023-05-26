# Comparing `tmp/pycontent_type-1.0.0.tar.gz` & `tmp/pycontent_type-1.1.0.tar.gz`

## Comparing `pycontent_type-1.0.0.tar` & `pycontent_type-1.1.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 pycontent_type-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 pycontent_type-1.0.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 pycontent_type-1.0.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 pycontent_type-1.0.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 pycontent_type-1.0.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 pycontent_type-1.0.0/pycontent_type/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pycontent_type-1.0.0/pycontent_type/py.typed
--rw-r--r--   0        0        0     4051 2020-02-02 00:00:00.000000 pycontent_type-1.0.0/pycontent_type/query.py
--rw-r--r--   0        0        0   191766 2020-02-02 00:00:00.000000 pycontent_type-1.0.0/pycontent_type/data/application.json
--rw-r--r--   0        0        0    15044 2020-02-02 00:00:00.000000 pycontent_type-1.0.0/pycontent_type/data/audio.json
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 pycontent_type-1.0.0/pycontent_type/data/font.json
--rw-r--r--   0        0        0     7663 2020-02-02 00:00:00.000000 pycontent_type-1.0.0/pycontent_type/data/image.json
--rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 pycontent_type-1.0.0/pycontent_type/data/message.json
--rw-r--r--   0        0        0     4003 2020-02-02 00:00:00.000000 pycontent_type-1.0.0/pycontent_type/data/model.json
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 pycontent_type-1.0.0/pycontent_type/data/multipart.json
--rw-r--r--   0        0        0     9282 2020-02-02 00:00:00.000000 pycontent_type-1.0.0/pycontent_type/data/text.json
--rw-r--r--   0        0        0     8879 2020-02-02 00:00:00.000000 pycontent_type-1.0.0/pycontent_type/data/video.json
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 pycontent_type-1.0.0/scripts/clean.sh
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 pycontent_type-1.0.0/scripts/format.sh
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 pycontent_type-1.0.0/scripts/mypy.sh
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 pycontent_type-1.0.0/scripts/test.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pycontent_type-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 pycontent_type-1.0.0/tests/test_pycontent_type.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pycontent_type-1.0.0/tests/test_version.py
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 pycontent_type-1.0.0/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pycontent_type-1.0.0/LICENSE
--rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 pycontent_type-1.0.0/README.md
--rw-r--r--   0        0        0     3788 2020-02-02 00:00:00.000000 pycontent_type-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4079 2020-02-02 00:00:00.000000 pycontent_type-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 pycontent_type-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 pycontent_type-1.1.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 pycontent_type-1.1.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 pycontent_type-1.1.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 pycontent_type-1.1.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 pycontent_type-1.1.0/pycontent_type/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pycontent_type-1.1.0/pycontent_type/py.typed
+-rw-r--r--   0        0        0     4051 2020-02-02 00:00:00.000000 pycontent_type-1.1.0/pycontent_type/query.py
+-rw-r--r--   0        0        0   191766 2020-02-02 00:00:00.000000 pycontent_type-1.1.0/pycontent_type/data/application.json
+-rw-r--r--   0        0        0    15044 2020-02-02 00:00:00.000000 pycontent_type-1.1.0/pycontent_type/data/audio.json
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 pycontent_type-1.1.0/pycontent_type/data/font.json
+-rw-r--r--   0        0        0     7663 2020-02-02 00:00:00.000000 pycontent_type-1.1.0/pycontent_type/data/image.json
+-rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 pycontent_type-1.1.0/pycontent_type/data/message.json
+-rw-r--r--   0        0        0     4003 2020-02-02 00:00:00.000000 pycontent_type-1.1.0/pycontent_type/data/model.json
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 pycontent_type-1.1.0/pycontent_type/data/multipart.json
+-rw-r--r--   0        0        0     9282 2020-02-02 00:00:00.000000 pycontent_type-1.1.0/pycontent_type/data/text.json
+-rw-r--r--   0        0        0     8879 2020-02-02 00:00:00.000000 pycontent_type-1.1.0/pycontent_type/data/video.json
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 pycontent_type-1.1.0/scripts/clean.sh
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 pycontent_type-1.1.0/scripts/format.sh
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 pycontent_type-1.1.0/scripts/mypy.sh
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 pycontent_type-1.1.0/scripts/test.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pycontent_type-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 pycontent_type-1.1.0/tests/test_pycontent_type.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pycontent_type-1.1.0/tests/test_version.py
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 pycontent_type-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pycontent_type-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 pycontent_type-1.1.0/README.md
+-rw-r--r--   0        0        0     3774 2020-02-02 00:00:00.000000 pycontent_type-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 pycontent_type-1.1.0/PKG-INFO
```

### Comparing `pycontent_type-1.0.0/.pre-commit-config.yaml` & `pycontent_type-1.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pycontent_type-1.0.0/.github/workflows/ci.yml` & `pycontent_type-1.1.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pycontent_type-1.0.0/.github/workflows/release.yml` & `pycontent_type-1.1.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pycontent_type-1.0.0/pycontent_type/__init__.py` & `pycontent_type-1.1.0/pycontent_type/__init__.py`

 * *Files identical despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Python library to access all Supported Content-Types/Media-Types
 """
 
-__version__ = "1.0.0"
+__version__ = "1.1.0"
 
 import os.path
 import unicodedata
 
 import pycontent_type.query
 
 try:
```

### Comparing `pycontent_type-1.0.0/pycontent_type/query.py` & `pycontent_type-1.1.0/pycontent_type/query.py`

 * *Files identical despite different names*

### Comparing `pycontent_type-1.0.0/pycontent_type/data/application.json` & `pycontent_type-1.1.0/pycontent_type/data/application.json`

 * *Files identical despite different names*

### Comparing `pycontent_type-1.0.0/pycontent_type/data/audio.json` & `pycontent_type-1.1.0/pycontent_type/data/audio.json`

 * *Files identical despite different names*

### Comparing `pycontent_type-1.0.0/pycontent_type/data/font.json` & `pycontent_type-1.1.0/pycontent_type/data/font.json`

 * *Files identical despite different names*

### Comparing `pycontent_type-1.0.0/pycontent_type/data/image.json` & `pycontent_type-1.1.0/pycontent_type/data/image.json`

 * *Files identical despite different names*

### Comparing `pycontent_type-1.0.0/pycontent_type/data/message.json` & `pycontent_type-1.1.0/pycontent_type/data/message.json`

 * *Files identical despite different names*

### Comparing `pycontent_type-1.0.0/pycontent_type/data/model.json` & `pycontent_type-1.1.0/pycontent_type/data/model.json`

 * *Files identical despite different names*

### Comparing `pycontent_type-1.0.0/pycontent_type/data/multipart.json` & `pycontent_type-1.1.0/pycontent_type/data/multipart.json`

 * *Files identical despite different names*

### Comparing `pycontent_type-1.0.0/pycontent_type/data/text.json` & `pycontent_type-1.1.0/pycontent_type/data/text.json`

 * *Files identical despite different names*

### Comparing `pycontent_type-1.0.0/pycontent_type/data/video.json` & `pycontent_type-1.1.0/pycontent_type/data/video.json`

 * *Files identical despite different names*

### Comparing `pycontent_type-1.0.0/scripts/clean.sh` & `pycontent_type-1.1.0/scripts/clean.sh`

 * *Files identical despite different names*

### Comparing `pycontent_type-1.0.0/tests/test_pycontent_type.py` & `pycontent_type-1.1.0/tests/test_pycontent_type.py`

 * *Files identical despite different names*

### Comparing `pycontent_type-1.0.0/.gitignore` & `pycontent_type-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pycontent_type-1.0.0/LICENSE` & `pycontent_type-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycontent_type-1.0.0/README.md` & `pycontent_type-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pycontent_type-1.0.0/pyproject.toml` & `pycontent_type-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -36,24 +36,24 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Internet",
     "Typing :: Typed",
 ]
 
 dependencies = [
     "typing-extensions >=3.7.4,<4.7.0",
+    "setuptools",
 ]
 
 dynamic = ["version"]
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [project.urls]
-Homepage = "https://github.com/yezz123/authx"
-Documentation = "https://authx.yezz.me/"
+Homepage = "https://github.com/yezz123/pycontent_type"
 Funding = 'https://github.com/sponsors/yezz123'
 
 [project.optional-dependencies]
 lint = [
     "pre-commit==3.3.2",
     "mypy==1.3.0",
 ]
```

### Comparing `pycontent_type-1.0.0/PKG-INFO` & `pycontent_type-1.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Metadata-Version: 2.1
 Name: pycontent_type
-Version: 1.0.0
+Version: 1.1.0
 Summary: Python library to access all Supported Content-Types/Media-Types
-Project-URL: Homepage, https://github.com/yezz123/authx
-Project-URL: Documentation, https://authx.yezz.me/
+Project-URL: Homepage, https://github.com/yezz123/pycontent_type
 Project-URL: Funding, https://github.com/sponsors/yezz123
 Author-email: Yasser Tahiri <hello@yezz.me>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: Content-Type,MIME,MIME-Type,Media-Type
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -23,14 +22,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
+Requires-Dist: setuptools
 Requires-Dist: typing-extensions<4.7.0,>=3.7.4
 Provides-Extra: lint
 Requires-Dist: mypy==1.3.0; extra == 'lint'
 Requires-Dist: pre-commit==3.3.2; extra == 'lint'
 Provides-Extra: test
 Requires-Dist: httpx==0.24.1; extra == 'test'
 Requires-Dist: pytest-asyncio==0.21.0; extra == 'test'
```

#### html2text {}

```diff
@@ -1,32 +1,31 @@
-Metadata-Version: 2.1 Name: pycontent_type Version: 1.0.0 Summary: Python
+Metadata-Version: 2.1 Name: pycontent_type Version: 1.1.0 Summary: Python
 library to access all Supported Content-Types/Media-Types Project-URL:
-Homepage, https://github.com/yezz123/authx Project-URL: Documentation, https://
-authx.yezz.me/ Project-URL: Funding, https://github.com/sponsors/yezz123
-Author-email: Yasser Tahiri
+Homepage, https://github.com/yezz123/pycontent_type Project-URL: Funding,
+https://github.com/sponsors/yezz123 Author-email: Yasser Tahiri
 yezz.me> License-Expression: MIT License-File: LICENSE Keywords: Content-
 Type,MIME,MIME-Type,Media-Type Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Information Technology Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet Classifier: Topic :: Internet :: WWW/HTTP ::
 Session Classifier: Topic :: Software Development :: Libraries :: Python
 Modules Classifier: Typing :: Typed Requires-Python: >=3.7 Requires-Dist:
-typing-extensions<4.7.0,>=3.7.4 Provides-Extra: lint Requires-Dist:
-mypy==1.3.0; extra == 'lint' Requires-Dist: pre-commit==3.3.2; extra == 'lint'
-Provides-Extra: test Requires-Dist: httpx==0.24.1; extra == 'test' Requires-
-Dist: pytest-asyncio==0.21.0; extra == 'test' Requires-Dist: pytest-cov==4.1.0;
-extra == 'test' Requires-Dist: pytest==7.3.1; extra == 'test' Requires-Dist:
-requests==2.31.0; extra == 'test' Description-Content-Type: text/markdown #
-pycontent-type
+setuptools Requires-Dist: typing-extensions<4.7.0,>=3.7.4 Provides-Extra: lint
+Requires-Dist: mypy==1.3.0; extra == 'lint' Requires-Dist: pre-commit==3.3.2;
+extra == 'lint' Provides-Extra: test Requires-Dist: httpx==0.24.1; extra ==
+'test' Requires-Dist: pytest-asyncio==0.21.0; extra == 'test' Requires-Dist:
+pytest-cov==4.1.0; extra == 'test' Requires-Dist: pytest==7.3.1; extra ==
+'test' Requires-Dist: requests==2.31.0; extra == 'test' Description-Content-
+Type: text/markdown # pycontent-type
     A Python library to access all Supported Content-Types/Media-Types â¡
 [lint] [Package_version] [https://codecov.io/gh/yezz123/pycontent-type/branch/
                              main/graph/badge.svg]
 ## Installation You can add pycontent-type in a few easy steps. First of all,
 install the dependency: ```shell $ pip install pycontent-type ---> 100%
 Successfully installed pycontent-type ``` ## Usage We have a simple API to
 access all the supported content-types: As known the categories of content-
```

