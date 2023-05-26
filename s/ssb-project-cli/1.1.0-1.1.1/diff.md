# Comparing `tmp/ssb_project_cli-1.1.0.tar.gz` & `tmp/ssb_project_cli-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssb_project_cli-1.1.0.tar", max compression
+gzip compressed data, was "ssb_project_cli-1.1.1.tar", max compression
```

## Comparing `ssb_project_cli-1.1.0.tar` & `ssb_project_cli-1.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1073 2023-05-23 13:59:00.044906 ssb_project_cli-1.1.0/LICENSE
--rw-r--r--   0        0        0     2881 2023-05-23 13:59:00.048905 ssb_project_cli-1.1.0/README.md
--rw-r--r--   0        0        0     2635 2023-05-23 13:59:15.789056 ssb_project_cli-1.1.0/pyproject.toml
--rw-r--r--   0        0        0       23 2023-05-23 13:59:00.048905 ssb_project_cli-1.1.0/src/ssb_project_cli/__init__.py
--rw-r--r--   0        0        0      171 2023-05-23 13:59:00.048905 ssb_project_cli-1.1.0/src/ssb_project_cli/__main__.py
--rw-r--r--   0        0        0        0 2023-05-23 13:59:00.048905 ssb_project_cli-1.1.0/src/ssb_project_cli/py.typed
--rw-r--r--   0        0        0      257 2023-05-23 13:59:00.048905 ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/__init__.py
--rw-r--r--   0        0        0     4305 2023-05-23 13:59:15.789056 ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/app.py
--rw-r--r--   0        0        0       29 2023-05-23 13:59:00.048905 ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/build/__init__.py
--rw-r--r--   0        0        0     3021 2023-05-23 13:59:15.789056 ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/build/build.py
--rw-r--r--   0        0        0     3740 2023-05-23 13:59:15.789056 ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/build/environment.py
--rw-r--r--   0        0        0     4938 2023-05-23 13:59:00.048905 ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/build/poetry.py
--rw-r--r--   0        0        0     1886 2023-05-23 13:59:15.789056 ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/build/prompt.py
--rw-r--r--   0        0        0     1644 2023-05-23 13:59:15.789056 ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/build/temp_template_repo.py
--rw-r--r--   0        0        0       69 2023-05-23 13:59:00.048905 ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/build_cmds.md
--rw-r--r--   0        0        0       29 2023-05-23 13:59:00.048905 ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/clean/__init__.py
--rw-r--r--   0        0        0     3008 2023-05-23 13:59:15.789056 ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/clean/clean.py
--rw-r--r--   0        0        0       30 2023-05-23 13:59:00.048905 ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/create/__init__.py
--rw-r--r--   0        0        0     6285 2023-05-23 13:59:15.789056 ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/create/create.py
--rw-r--r--   0        0        0     9618 2023-05-23 13:59:00.048905 ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/create/github.py
--rw-r--r--   0        0        0     6057 2023-05-23 13:59:15.789056 ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/create/local_repo.py
--rw-r--r--   0        0        0     1631 2023-05-23 13:59:00.052906 ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/create/prompt.py
--rw-r--r--   0        0        0      224 2023-05-23 13:59:00.052906 ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/create/repo_privacy.py
--rw-r--r--   0        0        0     1303 2023-05-23 13:59:00.052906 ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/create/temp_git_repo.py
--rw-r--r--   0        0        0      368 2023-05-23 13:59:00.052906 ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/settings.py
--rw-r--r--   0        0        0     3209 2023-05-23 13:59:00.052906 ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/util.py
--rw-r--r--   0        0        0     4427 1970-01-01 00:00:00.000000 ssb_project_cli-1.1.0/setup.py
--rw-r--r--   0        0        0     4323 1970-01-01 00:00:00.000000 ssb_project_cli-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-26 14:07:02.708777 ssb_project_cli-1.1.1/LICENSE
+-rw-r--r--   0        0        0     2881 2023-05-26 14:07:02.708777 ssb_project_cli-1.1.1/README.md
+-rw-r--r--   0        0        0     2635 2023-05-26 14:07:15.249068 ssb_project_cli-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0       23 2023-05-26 14:07:02.712777 ssb_project_cli-1.1.1/src/ssb_project_cli/__init__.py
+-rw-r--r--   0        0        0      171 2023-05-26 14:07:02.712777 ssb_project_cli-1.1.1/src/ssb_project_cli/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-26 14:07:02.712777 ssb_project_cli-1.1.1/src/ssb_project_cli/py.typed
+-rw-r--r--   0        0        0      257 2023-05-26 14:07:02.712777 ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/__init__.py
+-rw-r--r--   0        0        0     4305 2023-05-26 14:07:02.712777 ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/app.py
+-rw-r--r--   0        0        0       29 2023-05-26 14:07:02.712777 ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/build/__init__.py
+-rw-r--r--   0        0        0     3021 2023-05-26 14:07:02.712777 ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/build/build.py
+-rw-r--r--   0        0        0     3740 2023-05-26 14:07:02.712777 ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/build/environment.py
+-rw-r--r--   0        0        0     4947 2023-05-26 14:07:15.249068 ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/build/poetry.py
+-rw-r--r--   0        0        0     1886 2023-05-26 14:07:02.712777 ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/build/prompt.py
+-rw-r--r--   0        0        0     1644 2023-05-26 14:07:02.712777 ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/build/temp_template_repo.py
+-rw-r--r--   0        0        0       69 2023-05-26 14:07:02.712777 ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/build_cmds.md
+-rw-r--r--   0        0        0       29 2023-05-26 14:07:02.712777 ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/clean/__init__.py
+-rw-r--r--   0        0        0     3008 2023-05-26 14:07:02.712777 ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/clean/clean.py
+-rw-r--r--   0        0        0       30 2023-05-26 14:07:02.712777 ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/create/__init__.py
+-rw-r--r--   0        0        0     6285 2023-05-26 14:07:02.712777 ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/create/create.py
+-rw-r--r--   0        0        0     9618 2023-05-26 14:07:02.712777 ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/create/github.py
+-rw-r--r--   0        0        0     6057 2023-05-26 14:07:02.712777 ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/create/local_repo.py
+-rw-r--r--   0        0        0     1631 2023-05-26 14:07:02.712777 ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/create/prompt.py
+-rw-r--r--   0        0        0      224 2023-05-26 14:07:02.712777 ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/create/repo_privacy.py
+-rw-r--r--   0        0        0     1303 2023-05-26 14:07:02.712777 ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/create/temp_git_repo.py
+-rw-r--r--   0        0        0      368 2023-05-26 14:07:02.712777 ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/settings.py
+-rw-r--r--   0        0        0     3209 2023-05-26 14:07:02.712777 ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/util.py
+-rw-r--r--   0        0        0     4427 1970-01-01 00:00:00.000000 ssb_project_cli-1.1.1/setup.py
+-rw-r--r--   0        0        0     4323 1970-01-01 00:00:00.000000 ssb_project_cli-1.1.1/PKG-INFO
```

### Comparing `ssb_project_cli-1.1.0/LICENSE` & `ssb_project_cli-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ssb_project_cli-1.1.0/README.md` & `ssb_project_cli-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ssb_project_cli-1.1.0/pyproject.toml` & `ssb_project_cli-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ssb-project-cli"
-version = "1.1.0"
+version = "1.1.1"
 description = "SSB Project CLI"
 authors = ["Statistics Norway <stat-dev@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/statisticsnorway/ssb-project-cli"
 repository = "https://github.com/statisticsnorway/ssb-project-cli"
 documentation = "https://ssb-project-cli.readthedocs.io"
```

### Comparing `ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/app.py` & `ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/app.py`

 * *Files identical despite different names*

### Comparing `ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/build/build.py` & `ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/build/build.py`

 * *Files identical despite different names*

### Comparing `ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/build/environment.py` & `ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/build/environment.py`

 * *Files identical despite different names*

### Comparing `ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/build/poetry.py` & `ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/build/poetry.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
     Args:
         source_url: URL of 'simple' package API of package server
         cwd: Path of project to add source to
         source_name: Name of source to add
     """
     print("Adding package installation source for poetry...")
     execute_command(
-        f"poetry source add --default {source_name} {source_url}".split(" "),
+        f"poetry source add --priority=primary {source_name} {source_url}".split(" "),
         "poetry-source-add",
         "Poetry source successfully added!",
         "Failed to add poetry source.",
         cwd=cwd,
     )
 
     # If the lock is created off-prem, we need to refresh the lock.
```

### Comparing `ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/build/prompt.py` & `ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/build/prompt.py`

 * *Files identical despite different names*

### Comparing `ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/build/temp_template_repo.py` & `ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/build/temp_template_repo.py`

 * *Files identical despite different names*

### Comparing `ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/clean/clean.py` & `ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/clean/clean.py`

 * *Files identical despite different names*

### Comparing `ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/create/create.py` & `ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/create/create.py`

 * *Files identical despite different names*

### Comparing `ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/create/github.py` & `ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/create/github.py`

 * *Files identical despite different names*

### Comparing `ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/create/local_repo.py` & `ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/create/local_repo.py`

 * *Files identical despite different names*

### Comparing `ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/create/prompt.py` & `ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/create/prompt.py`

 * *Files identical despite different names*

### Comparing `ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/create/temp_git_repo.py` & `ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/create/temp_git_repo.py`

 * *Files identical despite different names*

### Comparing `ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/util.py` & `ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/util.py`

 * *Files identical despite different names*

### Comparing `ssb_project_cli-1.1.0/setup.py` & `ssb_project_cli-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
  'urllib3>=1.26.12,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['ssb-project = ssb_project_cli.__main__:main']}
 
 setup_kwargs = {
     'name': 'ssb-project-cli',
-    'version': '1.1.0',
+    'version': '1.1.1',
     'description': 'SSB Project CLI',
     'long_description': '# SSB Project CLI\n\n[![PyPI](https://img.shields.io/pypi/v/ssb-project-cli.svg)][pypi status]\n[![Status](https://img.shields.io/pypi/status/ssb-project-cli.svg)][pypi status]\n[![Python Version](https://img.shields.io/pypi/pyversions/ssb-project-cli)][pypi status]\n[![License](https://img.shields.io/pypi/l/ssb-project-cli)][license]\n\n[![Read the documentation](https://img.shields.io/badge/docs-Github%20Pages-purple)](https://statisticsnorway.github.io/ssb-project-cli/)\n[![Tests](https://github.com/statisticsnorway/ssb-project-cli/workflows/Tests/badge.svg)][tests]\n[![Codecov](https://codecov.io/gh/statisticsnorway/ssb-project-cli/branch/main/graph/badge.svg)][codecov]\n\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]\n\n[pypi status]: https://pypi.org/project/ssb-project-cli/\n[read the docs]: https://ssb-project-cli.readthedocs.io/\n[tests]: https://github.com/statisticsnorway/ssb-project-cli/actions?workflow=Tests\n[codecov]: https://app.codecov.io/gh/statisticsnorway/ssb-project-cli\n[pre-commit]: https://github.com/pre-commit/pre-commit\n[black]: https://github.com/psf/black\n\n## Features\n\n![Help text](docs/assets/cli_help_screenshot.png)\n\n- Create a new project quickly and easily with `ssb-project create`.\n- Your colleagues can quickly get started when you share the project with them with `ssb-project build`.\n- Includes:\n  - Local directory structure\n  - Virtual Environment\n  - Kernel for use on Jupyter\n  - Github repo (if desired)\n- The project will follow the most recent SSB guidelines for security and quality.\n- It will always be possible to update existing projects as guidelines change.\n\n## Installation\n\nYou can install _SSB Project CLI_ via [pip] from [PyPI]:\n\n```console\npip install ssb-project-cli\n```\n\n## Releasing a new version\n\nTo release a new version of the CLI, run the following sequence.\n\n```console\ngit switch --create release main\n```\n\n```console\npoetry version <version>\n```\n\n```console\ngit commit --message="<project> <version>" pyproject.toml\n```\n\n```console\ngit push origin release\n```\n\n## Contributing\n\n### Setup\n\n1. [Install dependencies](https://cookiecutter-hypermodern-python.readthedocs.io/en/latest/guide.html#installation)\n1. [Install pre-commit hooks](https://cookiecutter-hypermodern-python.readthedocs.io/en/latest/guide.html#running-pre-commit-from-git)\n1. Run tests: `nox -r` ([More information here](https://cookiecutter-hypermodern-python.readthedocs.io/en/latest/guide.html#using-nox))\n1. Run the help command: `poetry run ssb-project --help`\n\n## License\n\nDistributed under the terms of the [MIT license][license],\n_SSB Project CLI_ is free and open source software.\n\n<!-- github-only -->\n\n[license]: https://github.com/statisticsnorway/ssb-project-cli/blob/main/LICENSE\n',
     'author': 'Statistics Norway',
     'author_email': 'stat-dev@ssb.no',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/statisticsnorway/ssb-project-cli',
```

### Comparing `ssb_project_cli-1.1.0/PKG-INFO` & `ssb_project_cli-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssb-project-cli
-Version: 1.1.0
+Version: 1.1.1
 Summary: SSB Project CLI
 Home-page: https://github.com/statisticsnorway/ssb-project-cli
 License: MIT
 Author: Statistics Norway
 Author-email: stat-dev@ssb.no
 Requires-Python: >=3.10,<3.11
 Classifier: Development Status :: 4 - Beta
```

