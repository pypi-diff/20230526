# Comparing `tmp/flxtrd-0.0.3.tar.gz` & `tmp/flxtrd-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flxtrd-0.0.3.tar", max compression
+gzip compressed data, was "flxtrd-0.0.4.tar", max compression
```

## Comparing `flxtrd-0.0.3.tar` & `flxtrd-0.0.4.tar`

### file list

```diff
@@ -1,5 +1,32 @@
--rw-r--r--   0        0        0     9135 2023-05-05 08:04:47.294863 flxtrd-0.0.3/LICENSE
--rw-r--r--   0        0        0     2637 2023-05-07 17:59:58.410005 flxtrd-0.0.3/README.md
--rw-r--r--   0        0        0     1883 2023-05-07 18:00:34.383985 flxtrd-0.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-07 17:55:35.934823 flxtrd-0.0.3/src/__init__.py
--rw-r--r--   0        0        0     3357 1970-01-01 00:00:00.000000 flxtrd-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     9135 2023-05-17 07:19:03.818074 flxtrd-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1489 2023-05-26 12:52:03.065023 flxtrd-0.0.4/README.md
+-rw-r--r--   0        0        0     1936 2023-05-26 12:46:40.793011 flxtrd-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      417 2023-05-26 12:05:54.244915 flxtrd-0.0.4/src/flxtrd/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-26 11:38:00.772850 flxtrd-0.0.4/src/flxtrd/core/__init__.py
+-rw-r--r--   0        0        0      148 2023-05-26 11:56:09.804892 flxtrd-0.0.4/src/flxtrd/core/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1902 2023-05-26 12:52:17.085024 flxtrd-0.0.4/src/flxtrd/core/__pycache__/api_client.cpython-310.pyc
+-rw-r--r--   0        0        0     1756 2023-05-26 12:44:23.737005 flxtrd-0.0.4/src/flxtrd/core/api_client.py
+-rw-r--r--   0        0        0        0 2023-05-26 11:38:08.360850 flxtrd-0.0.4/src/flxtrd/core/plugins/__init__.py
+-rw-r--r--   0        0        0      156 2023-05-26 12:00:50.840903 flxtrd-0.0.4/src/flxtrd/core/plugins/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1793 2023-05-26 12:36:19.900987 flxtrd-0.0.4/src/flxtrd/core/plugins/__pycache__/auth.cpython-310.pyc
+-rw-r--r--   0        0        0     1017 2023-05-26 12:41:50.480999 flxtrd-0.0.4/src/flxtrd/core/plugins/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0      957 2023-05-26 12:36:19.916987 flxtrd-0.0.4/src/flxtrd/core/plugins/__pycache__/log.cpython-310.pyc
+-rw-r--r--   0        0        0     1041 2023-05-26 12:35:35.412985 flxtrd-0.0.4/src/flxtrd/core/plugins/auth.py
+-rw-r--r--   0        0        0      469 2023-05-26 12:41:28.000999 flxtrd-0.0.4/src/flxtrd/core/plugins/base.py
+-rw-r--r--   0        0        0      430 2023-05-26 12:36:16.552986 flxtrd-0.0.4/src/flxtrd/core/plugins/log.py
+-rw-r--r--   0        0        0        0 2023-05-26 11:37:40.696849 flxtrd-0.0.4/src/flxtrd/protocols/__init__.py
+-rw-r--r--   0        0        0      153 2023-05-26 11:56:09.816892 flxtrd-0.0.4/src/flxtrd/protocols/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      733 2023-05-26 12:08:38.328922 flxtrd-0.0.4/src/flxtrd/protocols/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0      798 2023-05-26 11:31:42.840835 flxtrd-0.0.4/src/flxtrd/protocols/__pycache__/base_api.cpython-310.pyc
+-rw-r--r--   0        0        0      260 2023-05-26 12:08:28.712921 flxtrd-0.0.4/src/flxtrd/protocols/base.py
+-rw-r--r--   0        0        0        0 2023-05-26 11:45:29.372867 flxtrd-0.0.4/src/flxtrd/protocols/grpc/__init__.py
+-rw-r--r--   0        0        0      158 2023-05-26 12:07:00.048918 flxtrd-0.0.4/src/flxtrd/protocols/grpc/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      570 2023-05-26 12:07:00.048918 flxtrd-0.0.4/src/flxtrd/protocols/grpc/__pycache__/grpc_api.cpython-310.pyc
+-rw-r--r--   0        0        0      527 2023-05-26 11:32:55.156838 flxtrd-0.0.4/src/flxtrd/protocols/grpc/__pycache__/grpc_client.cpython-310.pyc
+-rw-r--r--   0        0        0      777 2023-05-26 12:06:20.196916 flxtrd-0.0.4/src/flxtrd/protocols/grpc/grpc_api.py
+-rw-r--r--   0        0        0        0 2023-05-26 12:00:47.920903 flxtrd-0.0.4/src/flxtrd/protocols/rest/__init__.py
+-rw-r--r--   0        0        0      158 2023-05-26 12:00:50.596903 flxtrd-0.0.4/src/flxtrd/protocols/rest/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1348 2023-05-26 12:30:30.944973 flxtrd-0.0.4/src/flxtrd/protocols/rest/__pycache__/rest_api.cpython-310.pyc
+-rw-r--r--   0        0        0      841 2023-05-25 12:34:41.675840 flxtrd-0.0.4/src/flxtrd/protocols/rest/__pycache__/rest_client.cpython-310.pyc
+-rw-r--r--   0        0        0     1145 2023-05-26 12:20:23.344949 flxtrd-0.0.4/src/flxtrd/protocols/rest/rest_api.py
+-rw-r--r--   0        0        0     2230 1970-01-01 00:00:00.000000 flxtrd-0.0.4/PKG-INFO
```

### Comparing `flxtrd-0.0.3/LICENSE` & `flxtrd-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `flxtrd-0.0.3/README.md` & `flxtrd-0.0.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,56 +1,64 @@
+Metadata-Version: 2.1
+Name: flxtrd
+Version: 0.0.4
+Summary: Public client API for the flexible energy trading market GLocalFlex.
+Home-page: https://github.com/glocalflex/GLocalFlexTrade
+Author: glocalflex
+Requires-Python: >=3.8,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pika (>=1.3.1,<2.0.0)
+Requires-Dist: requests (>=2.28.0)
+Project-URL: Documentation, https://glocalflex.github.io/GLocalFlexTrade/
+Project-URL: Repository, https://github.com/glocalflex/GLocalFlexTrade
+Description-Content-Type: text/markdown
+
 # GLocalFlexTrade Public API 
 
+Public client API for the flexible energy trading market GLocalFlex.
 Trade energy or offer flexible loads to the European energy market.
 
 [![Release](https://img.shields.io/github/v/release/glocalflex/flxtrd)](https://img.shields.io/github/v/release/glocalflex/flxtrd)
 [![Build status](https://img.shields.io/github/actions/workflow/status/glocalflex/flxtrd/main.yml?branch=main)](https://github.com/glocalflex/flxtrd/actions/workflows/main.yml?query=branch%3Amain)
 [![codecov](https://codecov.io/gh/glocalflex/flxtrd/branch/main/graph/badge.svg)](https://codecov.io/gh/glocalflex/flxtrd)
 [![Commit activity](https://img.shields.io/github/commit-activity/m/glocalflex/flxtrd)](https://img.shields.io/github/commit-activity/m/glocalflex/flxtrd)
 [![License](https://img.shields.io/github/license/glocalflex/flxtrd)](https://img.shields.io/github/license/glocalflex/flxtrd)
 
-Public client API for the flexible energy trading market GLocalFlex.
 
-- **Github repository**: <https://github.com/glocalflex/flxtrd/>
-- **Documentation** <https://glocalflex.github.io/flxtrd/>
+- **Github repository**: <https://github.com/glocalflex/GLocalFlexTrade/>
 
-## Getting started with your project
+## Getting started with GLocalFlexTrade
 
-First, create a repository on GitHub with the same name as this project, and then run the following commands:
+- **Documentation** <https://glocalflex.github.io/GLocalFlexTrade/>
 
-``` bash
-git init -b main
-git add .
-git commit -m "init commit"
-git remote add origin git@github.com:glocalflex/flxtrd.git
-git push -u origin main
-```
+## Basic Example
 
-Finally, install the environment and the pre-commit hooks with 
+```py
+
+from flxtrd import FlexAPIClient
+from flxtrd import AuthPlugin
 
-```bash
-make install
-```
 
-You are now ready to start development on your project! The CI/CD
-pipeline will be triggered when you open a pull request, merge to main,
-or when you create a new release.
+def main():
 
-To finalize the set-up for publishing to PyPi or Artifactory, see
-[here](https://fpgmaas.github.io/cookiecutter-poetry/features/publishing/#set-up-for-pypi).
-For activating the automatic documentation with MkDocs, see
-[here](https://fpgmaas.github.io/cookiecutter-poetry/features/mkdocs/#enabling-the-documentation-on-github).
-To enable the code coverage reports, see [here](https://fpgmaas.github.io/cookiecutter-poetry/features/codecov/).
+    API_BASE_URL = "localhost"
 
-## Releasing a new version
+    client = FlexAPIClient(base_url=API_BASE_URL)
+    client.add_plugin(AuthPlugin(app_token="secret"))
+
+    response = client.make_request(method="POST", endpoint="/user/login")
+    print(response)
+
+
+if __name__ == "__main__":
+        main()
+
+```
 
-- Create an API Token on [Pypi](https://pypi.org/).
-- Add the API Token to your projects secrets with the name `PYPI_TOKEN` by visiting 
-[this page](https://github.com/glocalflex/flxtrd/settings/secrets/actions/new).
-- Create a [new release](https://github.com/glocalflex/flxtrd/releases/new) on Github. 
-Create a new tag in the form ``*.*.*``.
 
-For more details, see [here](https://fpgmaas.github.io/cookiecutter-poetry/features/cicd/#how-to-trigger-a-release).
+# Development
 
----
 
-Repository initiated with [fpgmaas/cookiecutter-poetry](https://github.com/fpgmaas/cookiecutter-poetry).
```

### Comparing `flxtrd-0.0.3/pyproject.toml` & `flxtrd-0.0.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [tool.poetry]
 name = "flxtrd"
-version = "0.0.3"
+version = "0.0.4"
 description = "Public client API for the flexible energy trading market GLocalFlex."
 authors = ["glocalflex"]
-repository = "https://github.com/glocalflex/flxtrade"
-documentation = "https://glocalflex.github.io/flxtrade/"
+repository = "https://github.com/glocalflex/GLocalFlexTrade"
+documentation = "https://glocalflex.github.io/GLocalFlexTrade/"
 readme = "README.md"
-packages = [
-  {include = "src"}
-]
+# packages = [
+#   {include = "src"},
+#   {include = "examples"},
+# ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 pika = "^1.3.1"
 requests = ">=2.28.0"
 
 [tool.poetry.group.dev.dependencies]
@@ -27,16 +28,16 @@
 mkdocs-material = "^8.5.10"
 mkdocstrings = {extras = ["python"], version = "^0.19.0"}
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
-[tool.poetry.scripts]
-gflex-trading-bot = "gflex.client:main"
+# [tool.poetry.scripts]
+# gflex-trading-bot = "gflex.client:main"
 
 [tool.black]
 line-length = 120
 target-version = ['py37']
 preview = true
 
 [tool.mypy]
```

