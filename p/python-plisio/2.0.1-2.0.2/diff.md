# Comparing `tmp/python_plisio-2.0.1.tar.gz` & `tmp/python_plisio-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_plisio-2.0.1.tar", max compression
+gzip compressed data, was "python_plisio-2.0.2.tar", max compression
```

## Comparing `python_plisio-2.0.1.tar` & `python_plisio-2.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1061 2023-05-26 00:26:35.552919 python_plisio-2.0.1/LICENSE
--rw-r--r--   0        0        0     2255 2023-05-26 00:26:35.552919 python_plisio-2.0.1/README.md
--rw-r--r--   0        0        0     1733 2023-05-26 00:26:35.552919 python_plisio-2.0.1/pyproject.toml
--rw-r--r--   0        0        0      125 2023-05-26 00:26:35.552919 python_plisio-2.0.1/src/plisio/__init__.py
--rw-r--r--   0        0        0      298 2023-05-26 00:26:35.552919 python_plisio-2.0.1/src/plisio/_meta.py
--rw-r--r--   0        0        0     4575 2023-05-26 00:26:35.552919 python_plisio-2.0.1/src/plisio/_types.py
--rw-r--r--   0        0        0      323 2023-05-26 00:26:35.552919 python_plisio-2.0.1/src/plisio/clients/__init__.py
--rw-r--r--   0        0        0     6142 2023-05-26 00:26:35.552919 python_plisio-2.0.1/src/plisio/clients/_base.py
--rw-r--r--   0        0        0    12961 2023-05-26 00:26:35.552919 python_plisio-2.0.1/src/plisio/clients/async_client.py
--rw-r--r--   0        0        0    12648 2023-05-26 00:26:35.552919 python_plisio-2.0.1/src/plisio/clients/client.py
--rw-r--r--   0        0        0     7512 2023-05-26 00:26:35.552919 python_plisio-2.0.1/src/plisio/enums.py
--rw-r--r--   0        0        0     1777 2023-05-26 00:26:35.552919 python_plisio-2.0.1/src/plisio/exceptions.py
--rw-r--r--   0        0        0      238 2023-05-26 00:26:35.552919 python_plisio-2.0.1/src/plisio/utils.py
--rw-r--r--   0        0        0     3328 1970-01-01 00:00:00.000000 python_plisio-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-05-26 21:07:46.450648 python_plisio-2.0.2/LICENSE
+-rw-r--r--   0        0        0     2820 2023-05-26 21:07:46.450648 python_plisio-2.0.2/README.md
+-rw-r--r--   0        0        0     1975 2023-05-26 21:07:46.450648 python_plisio-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0      167 2023-05-26 21:07:46.450648 python_plisio-2.0.2/src/plisio/__init__.py
+-rw-r--r--   0        0        0      298 2023-05-26 21:07:46.450648 python_plisio-2.0.2/src/plisio/_meta.py
+-rw-r--r--   0        0        0     4575 2023-05-26 21:07:46.450648 python_plisio-2.0.2/src/plisio/_types.py
+-rw-r--r--   0        0        0      318 2023-05-26 21:07:46.450648 python_plisio-2.0.2/src/plisio/clients/__init__.py
+-rw-r--r--   0        0        0     6159 2023-05-26 21:07:46.450648 python_plisio-2.0.2/src/plisio/clients/_base.py
+-rw-r--r--   0        0        0    12961 2023-05-26 21:07:46.450648 python_plisio-2.0.2/src/plisio/clients/async_client.py
+-rw-r--r--   0        0        0    12696 2023-05-26 21:07:46.450648 python_plisio-2.0.2/src/plisio/clients/client.py
+-rw-r--r--   0        0        0     7512 2023-05-26 21:07:46.454648 python_plisio-2.0.2/src/plisio/enums.py
+-rw-r--r--   0        0        0     1777 2023-05-26 21:07:46.454648 python_plisio-2.0.2/src/plisio/exceptions.py
+-rw-r--r--   0        0        0      238 2023-05-26 21:07:46.454648 python_plisio-2.0.2/src/plisio/utils.py
+-rw-r--r--   0        0        0     3947 1970-01-01 00:00:00.000000 python_plisio-2.0.2/PKG-INFO
```

### Comparing `python_plisio-2.0.1/LICENSE` & `python_plisio-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python_plisio-2.0.1/README.md` & `python_plisio-2.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 # Python-Plisio-SDK
 
+[![Poetry](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/johnthagen/poetry/poetry-badge/assets/badge/v0.json)](https://python-poetry.org/)
 [![python](https://img.shields.io/badge/Python-%5E3.8.1-3776AB.svg?style=flat&logo=python&logoColor=tellow)](https://www.python.org)
+![PyPI](https://img.shields.io/pypi/v/python-plisio?color=blue)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/152926ced23a45c6abb55af6884f890f)](https://app.codacy.com/gh/amiwrpremium/python-plisio/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 ![GitHub](https://img.shields.io/github/license/amiwrpremium/python-plisio)
 [![Documentation Status](https://readthedocs.org/projects/python-plisio/badge/?version=latest)](https://python-plisio.readthedocs.io/en/latest/?badge=latest)
 [![Documentation Status](https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat)](https://squidfunk.github.io/mkdocs-material/)
 [![pydocstyle](https://img.shields.io/badge/pydocstyle-enabled-AD4CD3)](http://www.pydocstyle.org/en/stable/)
+[![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
+[![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/pylint-dev/pylint)
+[![Flake8 Status](./reports/flake8/flake8-badge.svg?dummy=8484744)](./reports/flake8/index.html)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/amiwrpremium/python-plisio/master.svg)](https://results.pre-commit.ci/latest/github/amiwrpremium/python-plisio/master)
-![PyPI](https://img.shields.io/pypi/v/python-plisio?color=blue)
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/amiwrpremium/python-plisio/publish.yml?label=publish)
 
 ## About
 
 [Plisio](https://plisio.net/) is a payment gateway for accepting
 payments in cryptocurrencies. Plisio enables your customers to pay with
 15+ cryptocurrencies, including Bitcoin, Ethereum, Litecoin, Dash, etc.
 
 **I'm in no way affiliated with Plisio and this is not an official SDK.**
 
 ## Installation
 
-Install using `pip`
-> $ pip install python-plisio
+Install using `pip` from [PyPI](https://pypi.org/project/python-plisio/):
+> pip install python-plisio
 
 Install from `git`
 > pip install git+https://github.com/amiwrpremium/python-plisio.git
 
 ## Usage
 
-See [examples](docs/examples) for more usage examples.
+See [examples](https://python-plisio.readthedocs.io/en/latest/examples/) for more usage examples.
 
 ## Documentation
 
 See [documentation](https://python-plisio.readthedocs.io/en/latest/).
 
 ## License
```

### Comparing `python_plisio-2.0.1/pyproject.toml` & `python_plisio-2.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,32 @@
 [tool.poetry]
 name = "python-plisio"
-version = "2.0.1"
+version = "2.0.2"
 description = "Python SDK for Plisio API."
 authors = ["amiwrpremium <amiwrpremium@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://amiwrpremium.github.io/python-plisio/"
 repository = "https://github.com/amiwrpremium/python-plisio"
-documentation = "https://amiwrpremium.github.io/python-plisio/"
-keywords = ["plisio", "api", "sdk", "python", "payments", "crypto", "gateway"]
+documentation = "https://python-plisio.readthedocs.io/en/latest/"
+keywords = [
+    "plisio",
+    "api",
+    "sdk",
+    "python",
+    "payments",
+    "crypto",
+    "gateway",
+    "crypto payment",
+    "bitcoin",
+    "etherium",
+    "blockchain",
+    "tron",
+    "BSC"
+]
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Utilities",
@@ -29,25 +43,30 @@
 
 [tool.poetry.group.dev.dependencies]
 curlify = "^2.2.1"
 flake8 = "^6.0.0"
 pylint = "^2.17.4"
 mypy = "^1.3.0"
 types-requests = "^2.31.0.0"
+mkdocs-autorefs = "^0.4.1"
+pydocstyle = "^6.3.0"
+black = "^23.3.0"
+flake8-html = "^0.4.3"
+genbadge = {extras = ["flake8"], version = "^1.1.0"}
+
+
+[tool.poetry.group.docs.dependencies]
 mkdocs = "^1.4.3"
 mkdocs-material = "^9.1.14"
 mkdocstrings = "^0.21.2"
 mkdocs-git-revision-date-localized-plugin = "^1.2.0"
 mkdocs-git-committers-plugin-2 = "^1.1.2"
 mkdocs-gen-files = "^0.5.0"
 mkdocs-literate-nav = "^0.6.0"
 mkdocs-section-index = "^0.3.5"
-mkdocs-autorefs = "^0.4.1"
-pydocstyle = "^6.3.0"
-black = "^23.3.0"
 mkdocstrings-python = "^1.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
```

### Comparing `python_plisio-2.0.1/src/plisio/_types.py` & `python_plisio-2.0.2/src/plisio/_types.py`

 * *Files identical despite different names*

### Comparing `python_plisio-2.0.1/src/plisio/clients/_base.py` & `python_plisio-2.0.2/src/plisio/clients/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
             path (str): Path.
             version (str): API version.
 
         Returns:
             str: URI.
         """
 
-        return f"{self.BASE_URL}/{version}/{path}"
+        return f"{self.BASE_URL}/{version}/{path.lstrip('/').rstrip('/')}"
 
     @staticmethod
     def _get_params(locals_: _t.DictStrAny, exclude_unset: bool = True) -> _t.DictStrAny:
         """
         Get params.
 
         Args:
@@ -103,24 +103,23 @@
 
         kwargs["timeout"] = self.REQUEST_TIMEOUT
 
         if self._requests_params:
             kwargs.update(self._requests_params)
 
         data = kwargs.pop("data", None)
+        data.update({"api_key": self.api_key})
 
         if data and isinstance(data, dict):
             kwargs["data"] = data
 
             if "requests_params" in kwargs["data"]:
                 kwargs.update(kwargs["data"]["requests_params"])
                 del kwargs["data"]["requests_params"]
 
-            kwargs["data"]["api_key"] = self.api_key
-
         if data and (str(method).upper() == _Methods.GET or force_params):
             _ = ""
             for data in kwargs["data"].items():
                 key = data[0]
                 if isinstance(data[1], list):
                     value = ",".join(data[1])
                 else:
```

### Comparing `python_plisio-2.0.1/src/plisio/clients/async_client.py` & `python_plisio-2.0.2/src/plisio/clients/async_client.py`

 * *Files identical despite different names*

### Comparing `python_plisio-2.0.1/src/plisio/clients/client.py` & `python_plisio-2.0.2/src/plisio/clients/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,15 +221,15 @@
             PlisioRequestException: If request failed.
             PlisioAPIException: If API returned error.
         """
 
         params = self._get_params(locals())
         return self._get("invoices/new", data=params, force_params=True)
 
-    def transactions(  # pylint: disable=too-many-arguments, too-many-locals
+    def transactions(  # pylint: disable=too-many-arguments
         self,
         page: _t.OptionalNumberLike = None,
         limit: _t.OptionalNumberLike = None,
         shop_id: _t.OptionalNumberLike = None,
         type: _t.OptionalTransactionStatus = None,  # pylint: disable=redefined-builtin
         status: _t.OptionalTransactionStatus = None,
         currency: _t.OptionalCurrencies = None,
@@ -307,15 +307,15 @@
             dict: Response data.
 
         Raises:
             PlisioRequestException: If request failed.
             PlisioAPIException: If API returned error.
         """
 
-        return self._get(f"operations/{id}")
+        return self._get("operations", data={"id": id}, force_params=True)
 
     def balance(self, psys_cid: _t.OptionalCurrencies = None) -> _t.Result:
         """
         Get balance.
 
         See Also:
             https://plisio.net/documentation/endpoints/balance
@@ -327,15 +327,15 @@
             dict: Response data.
 
         Raises:
             PlisioRequestException: If request failed.
             PlisioAPIException: If API returned error.
         """
 
-        return self._get("balance/", data={"psys_cid": psys_cid}, force_params=True)
+        return self._get("balance", data={"psys_cid": psys_cid}, force_params=True)
 
     def fee_plans(self, psys_cid: _t.Currencies) -> _t.Result:
         """
         Get fee plans.
 
         See Also:
             https://plisio.net/documentation/endpoints/fee-plans
@@ -347,15 +347,15 @@
             dict: Response data.
 
         Raises:
             PlisioRequestException: If request failed.
             PlisioAPIException: If API returned error.
         """
 
-        return self._get(f"operations/fee-plan/{psys_cid}")
+        return self._get("operations/fee-plan", data={"psys_cid": psys_cid}, force_params=True)
 
     async def fee_estimation(
         self,
         currency: _t.OptionalCurrencies = None,
         addresses: _t.OptionalListStr = None,
         amounts: _t.OptionalListNumberLike = None,
         fee_plan: _t.OptionalFeePlans = None,
```

### Comparing `python_plisio-2.0.1/src/plisio/enums.py` & `python_plisio-2.0.2/src/plisio/enums.py`

 * *Files identical despite different names*

### Comparing `python_plisio-2.0.1/src/plisio/exceptions.py` & `python_plisio-2.0.2/src/plisio/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_plisio-2.0.1/PKG-INFO` & `python_plisio-2.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: python-plisio
-Version: 2.0.1
+Version: 2.0.2
 Summary: Python SDK for Plisio API.
 Home-page: https://amiwrpremium.github.io/python-plisio/
 License: MIT
-Keywords: plisio,api,sdk,python,payments,crypto,gateway
+Keywords: plisio,api,sdk,python,payments,crypto,gateway,crypto payment,bitcoin,etherium,blockchain,tron,BSC
 Author: amiwrpremium
 Author-email: amiwrpremium@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
@@ -16,51 +16,55 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: pydantic[email] (>=1.10.8,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
-Project-URL: Documentation, https://amiwrpremium.github.io/python-plisio/
+Project-URL: Documentation, https://python-plisio.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/amiwrpremium/python-plisio
 Description-Content-Type: text/markdown
 
 # Python-Plisio-SDK
 
+[![Poetry](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/johnthagen/poetry/poetry-badge/assets/badge/v0.json)](https://python-poetry.org/)
 [![python](https://img.shields.io/badge/Python-%5E3.8.1-3776AB.svg?style=flat&logo=python&logoColor=tellow)](https://www.python.org)
+![PyPI](https://img.shields.io/pypi/v/python-plisio?color=blue)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/152926ced23a45c6abb55af6884f890f)](https://app.codacy.com/gh/amiwrpremium/python-plisio/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 ![GitHub](https://img.shields.io/github/license/amiwrpremium/python-plisio)
 [![Documentation Status](https://readthedocs.org/projects/python-plisio/badge/?version=latest)](https://python-plisio.readthedocs.io/en/latest/?badge=latest)
 [![Documentation Status](https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat)](https://squidfunk.github.io/mkdocs-material/)
 [![pydocstyle](https://img.shields.io/badge/pydocstyle-enabled-AD4CD3)](http://www.pydocstyle.org/en/stable/)
+[![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
+[![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/pylint-dev/pylint)
+[![Flake8 Status](./reports/flake8/flake8-badge.svg?dummy=8484744)](./reports/flake8/index.html)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/amiwrpremium/python-plisio/master.svg)](https://results.pre-commit.ci/latest/github/amiwrpremium/python-plisio/master)
-![PyPI](https://img.shields.io/pypi/v/python-plisio?color=blue)
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/amiwrpremium/python-plisio/publish.yml?label=publish)
 
 ## About
 
 [Plisio](https://plisio.net/) is a payment gateway for accepting
 payments in cryptocurrencies. Plisio enables your customers to pay with
 15+ cryptocurrencies, including Bitcoin, Ethereum, Litecoin, Dash, etc.
 
 **I'm in no way affiliated with Plisio and this is not an official SDK.**
 
 ## Installation
 
-Install using `pip`
-> $ pip install python-plisio
+Install using `pip` from [PyPI](https://pypi.org/project/python-plisio/):
+> pip install python-plisio
 
 Install from `git`
 > pip install git+https://github.com/amiwrpremium/python-plisio.git
 
 ## Usage
 
-See [examples](docs/examples) for more usage examples.
+See [examples](https://python-plisio.readthedocs.io/en/latest/examples/) for more usage examples.
 
 ## Documentation
 
 See [documentation](https://python-plisio.readthedocs.io/en/latest/).
 
 ## License
```

