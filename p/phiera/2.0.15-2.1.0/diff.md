# Comparing `tmp/phiera-2.0.15.tar.gz` & `tmp/phiera-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phiera-2.0.15.tar", max compression
+gzip compressed data, was "phiera-2.1.0.tar", max compression
```

## Comparing `phiera-2.0.15.tar` & `phiera-2.1.0.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0    10346 2023-01-30 16:08:09.023664 phiera-2.0.15/LICENSE.md
--rw-r--r--   0        0        0     2494 2023-01-30 16:08:09.023664 phiera-2.0.15/README.md
--rw-r--r--   0        0        0       22 2023-01-30 16:08:09.023664 phiera-2.0.15/phiera/__init__.py
--rw-r--r--   0        0        0     1581 2023-01-30 16:08:09.023664 phiera-2.0.15/phiera/backends.py
--rw-r--r--   0        0        0       45 2023-01-30 16:08:09.023664 phiera-2.0.15/phiera/exceptions.py
--rw-r--r--   0        0        0    14273 2023-01-30 16:08:09.023664 phiera-2.0.15/phiera/phiera.py
--rw-r--r--   0        0        0      527 2023-01-30 16:08:09.023664 phiera-2.0.15/phiera/util.py
--rw-r--r--   0        0        0      677 2023-01-30 16:08:09.023664 phiera-2.0.15/pyproject.toml
--rw-r--r--   0        0        0     3256 2023-01-30 16:08:17.485653 phiera-2.0.15/setup.py
--rw-r--r--   0        0        0     3221 2023-01-30 16:08:17.486054 phiera-2.0.15/PKG-INFO
+-rw-r--r--   0        0        0    10346 2023-05-26 16:53:32.514493 phiera-2.1.0/LICENSE.md
+-rw-r--r--   0        0        0     2485 2023-05-26 16:53:32.514493 phiera-2.1.0/README.md
+-rw-r--r--   0        0        0       22 2023-05-26 16:53:32.514493 phiera-2.1.0/phiera/__init__.py
+-rw-r--r--   0        0        0     1581 2023-05-26 16:53:32.514493 phiera-2.1.0/phiera/backends.py
+-rw-r--r--   0        0        0       45 2023-05-26 16:53:32.514493 phiera-2.1.0/phiera/exceptions.py
+-rw-r--r--   0        0        0    14275 2023-05-26 16:53:32.514493 phiera-2.1.0/phiera/phiera.py
+-rw-r--r--   0        0        0      527 2023-05-26 16:53:32.514493 phiera-2.1.0/phiera/util.py
+-rw-r--r--   0        0        0      668 2023-05-26 16:53:32.514493 phiera-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3067 1970-01-01 00:00:00.000000 phiera-2.1.0/PKG-INFO
```

### Comparing `phiera-2.0.15/LICENSE.md` & `phiera-2.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `phiera-2.0.15/README.md` & `phiera-2.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 
 ### Manually
 
 ```bash
 git clone git@github.com/Nike-Inc/phiera.git
 cd phiera
-python setup.py install
+poetry install
 ```
 
 # <a name="usage"></a> Usage:
 
 ```python
 import phiera
```

### Comparing `phiera-2.0.15/phiera/backends.py` & `phiera-2.1.0/phiera/backends.py`

 * *Files identical despite different names*

### Comparing `phiera-2.0.15/phiera/phiera.py` & `phiera-2.1.0/phiera/phiera.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,19 +150,19 @@
         if hierarchy is None:
             raise Exception("Invalid Base Hiera Config: missing hierarchy key")
 
         self.hierarchy = []
 
         # Load our heirarchy
         for path in hierarchy:
-            self.hierarchy.append(rformat.sub("{\g<1>}", path, count=0))
+            self.hierarchy.append(rformat.sub(r"{\g<1>}", path, count=0))
 
         # Load our backends
         for backend in list(self.backends.values()):
-            backend.datadir = rformat.sub("{\g<1>}", backend.datadir, count=0)
+            backend.datadir = rformat.sub(r"{\g<1>}", backend.datadir, count=0)
 
         # Now pre-load/cache a bunch of global stuff. If context vars where provided
         #  in the constructor, we'll also load those files into the cache.
         self.get(None)
 
     def load_directory(self, path, backend=None):
         """
```

### Comparing `phiera-2.0.15/phiera/util.py` & `phiera-2.1.0/phiera/util.py`

 * *Files identical despite different names*

### Comparing `phiera-2.0.15/pyproject.toml` & `phiera-2.1.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "phiera"
-version = "2.0.15"
+version = "2.1.0"
 description = "a python hiera parser"
 authors = ["Andrei Zbikowski, Rob King"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/Nike-Inc/phiera"
 packages = [
     { include = "phiera" },
@@ -14,18 +14,17 @@
   "Mohamed Abdul Huq Ismail <Abdul.Ismail@nike.com>",
   "Manasi Waghmare <Manasi.Waghmare@nike.com>",
   "Marcin Zalewski <Marcin.Zalewski@nike.com"
 ]
 
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.10.10"
 PyYAML = "^6.0.0"
 
-[tool.poetry.dev-dependencies]
-pytest = "^6.2.2"
-pytest-cov = ">=3.0.0"
-mock = ">=3.0.4"
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.3.1"
+pytest-cov = "^4.1.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `phiera-2.0.15/setup.py` & `phiera-2.1.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,94 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: phiera
+Version: 2.1.0
+Summary: a python hiera parser
+Home-page: https://github.com/Nike-Inc/phiera
+License: Apache 2.0
+Author: Andrei Zbikowski, Rob King
+Maintainer: Mohamed Abdul Huq Ismail
+Maintainer-email: Abdul.Ismail@nike.com
+Requires-Python: >=3.10.10,<4.0.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: PyYAML (>=6.0.0,<7.0.0)
+Project-URL: Repository, https://github.com/Nike-Inc/phiera
+Description-Content-Type: text/markdown
+
+Phiera
+---
+
+[![codecov](https://codecov.io/gh/Nike-Inc/phiera/branch/master/graph/badge.svg?token=J9slc2blRx)](https://codecov.io/gh/Nike-Inc/phiera)
+[![Test](https://github.com/Nike-Inc/phiera/actions/workflows/python-test.yaml/badge.svg)](https://github.com/Nike-Inc/phiera/actions/workflows/python-test.yaml)
+[![PyPi Release](https://github.com/Nike-Inc/phiera/actions/workflows/python-build.yaml/badge.svg)](https://github.com/Nike-Inc/phiera/actions/workflows/python-build.yaml)
+![License](https://img.shields.io/pypi/l/phiera)
+![Python Versions](https://img.shields.io/pypi/pyversions/phiera)
+![Python Wheel](https://img.shields.io/pypi/wheel/phiera)
+
+Phiera is a fork of [Piera](https://github.com/b1naryth1ef/pierahttps://github.com/b1naryth1ef/piera), a lightweight, pure-Python [Hiera](http://docs.puppetlabs.com/hiera/) parser. Piera was originally built to provide Python tooling access to Puppet/Hiera configurations. The original Piera is currently not feature complete; lacking some less-used interpolation and loading features.
+
+Table of content
+* [Why](#why)
+* [Installation](#installation)
+* [Usage](#usage)
+* [Unit Tests](#tests)
+
+# <a name="why"></a> Why?:
+
+Piera/Phiera generalizes Puppet Hiera's hierarchical storage system; making a simple, very flexible, abstracted, and DRY mechanism for managing complex configuration data available to a broad set of tooling and applicable to a broad set of problems.
+
+Phiera builds on the original Piera work, adding:
+  
+  - Python3 compatibility
+  - Support for deep merging
+  - Support for configuration as a dict
+
+# <a name="installation"></a> Installation:
+
+### From PyPi:
+```shell script
+pip install phiera
+```
+
+### From GitHub:
+```shell script
+pip install git+https://github.com/Nike-Inc/phiera#egg=phiera
+```
+
+
+### Manually
+
+```bash
+git clone git@github.com/Nike-Inc/phiera.git
+cd phiera
+poetry install
+```
+
+# <a name="usage"></a> Usage:
+
+```python
+import phiera
+
+h = phiera.Hiera("my_hiera.yaml")
+
+# You can use phiera to simply interact with your structured Hiera data
+
+# key: 'value'
+assert h.get("key") == "value"
+
+# key_alias: '%{alias('key')}'
+assert h.get("key_alias") == "value"
+
+# key_hiera: 'OHAI %{hiera('key_alias')}'
+assert h.get("key_hiera") == "OHAI value"
+
+# Give phiera context
+assert h.get("my_context_based_key", name='test01', environment='qa') == "context is great!"
+```
+
+# <a name="tests"></a> Unit Tests:
+
+```bash
+poetry run pytest --cov-report=html --cov=phiera --cov-fail-under=80 tests/
+```
 
-packages = \
-['phiera']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['PyYAML>=6.0.0,<7.0.0']
-
-setup_kwargs = {
-    'name': 'phiera',
-    'version': '2.0.15',
-    'description': 'a python hiera parser',
-    'long_description': 'Phiera\n---\n\n[![codecov](https://codecov.io/gh/Nike-Inc/phiera/branch/master/graph/badge.svg?token=J9slc2blRx)](https://codecov.io/gh/Nike-Inc/phiera)\n[![Test](https://github.com/Nike-Inc/phiera/actions/workflows/python-test.yaml/badge.svg)](https://github.com/Nike-Inc/phiera/actions/workflows/python-test.yaml)\n[![PyPi Release](https://github.com/Nike-Inc/phiera/actions/workflows/python-build.yaml/badge.svg)](https://github.com/Nike-Inc/phiera/actions/workflows/python-build.yaml)\n![License](https://img.shields.io/pypi/l/phiera)\n![Python Versions](https://img.shields.io/pypi/pyversions/phiera)\n![Python Wheel](https://img.shields.io/pypi/wheel/phiera)\n\nPhiera is a fork of [Piera](https://github.com/b1naryth1ef/pierahttps://github.com/b1naryth1ef/piera), a lightweight, pure-Python [Hiera](http://docs.puppetlabs.com/hiera/) parser. Piera was originally built to provide Python tooling access to Puppet/Hiera configurations. The original Piera is currently not feature complete; lacking some less-used interpolation and loading features.\n\nTable of content\n* [Why](#why)\n* [Installation](#installation)\n* [Usage](#usage)\n* [Unit Tests](#tests)\n\n# <a name="why"></a> Why?:\n\nPiera/Phiera generalizes Puppet Hiera\'s hierarchical storage system; making a simple, very flexible, abstracted, and DRY mechanism for managing complex configuration data available to a broad set of tooling and applicable to a broad set of problems.\n\nPhiera builds on the original Piera work, adding:\n  \n  - Python3 compatibility\n  - Support for deep merging\n  - Support for configuration as a dict\n\n# <a name="installation"></a> Installation:\n\n### From PyPi:\n```shell script\npip install phiera\n```\n\n### From GitHub:\n```shell script\npip install git+https://github.com/Nike-Inc/phiera#egg=phiera\n```\n\n\n### Manually\n\n```bash\ngit clone git@github.com/Nike-Inc/phiera.git\ncd phiera\npython setup.py install\n```\n\n# <a name="usage"></a> Usage:\n\n```python\nimport phiera\n\nh = phiera.Hiera("my_hiera.yaml")\n\n# You can use phiera to simply interact with your structured Hiera data\n\n# key: \'value\'\nassert h.get("key") == "value"\n\n# key_alias: \'%{alias(\'key\')}\'\nassert h.get("key_alias") == "value"\n\n# key_hiera: \'OHAI %{hiera(\'key_alias\')}\'\nassert h.get("key_hiera") == "OHAI value"\n\n# Give phiera context\nassert h.get("my_context_based_key", name=\'test01\', environment=\'qa\') == "context is great!"\n```\n\n# <a name="tests"></a> Unit Tests:\n\n```bash\npoetry run pytest --cov-report=html --cov=phiera --cov-fail-under=80 tests/\n```\n',
-    'author': 'Andrei Zbikowski, Rob King',
-    'author_email': None,
-    'maintainer': 'Mohamed Abdul Huq Ismail',
-    'maintainer_email': 'Abdul.Ismail@nike.com',
-    'url': 'https://github.com/Nike-Inc/phiera',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

