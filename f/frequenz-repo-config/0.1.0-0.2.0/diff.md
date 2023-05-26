# Comparing `tmp/frequenz-repo-config-0.1.0.tar.gz` & `tmp/frequenz-repo-config-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frequenz-repo-config-0.1.0.tar", last modified: Tue May  9 14:14:18 2023, max compression
+gzip compressed data, was "frequenz-repo-config-0.2.0.tar", last modified: Fri May 26 09:41:45 2023, max compression
```

## Comparing `frequenz-repo-config-0.1.0.tar` & `frequenz-repo-config-0.2.0.tar`

### file list

```diff
@@ -1,32 +1,68 @@
-drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-09 14:14:18.196657 frequenz-repo-config-0.1.0/
--rw-r--r--   0 luca      (1000) luca      (1000)       34 2023-04-03 13:31:43.000000 frequenz-repo-config-0.1.0/.darglint
--rw-r--r--   0 luca      (1000) luca      (1000)     2134 2023-03-10 15:07:55.000000 frequenz-repo-config-0.1.0/.gitignore
--rw-r--r--   0 luca      (1000) luca      (1000)     1090 2023-03-31 14:27:27.000000 frequenz-repo-config-0.1.0/LICENSE
--rw-r--r--   0 luca      (1000) luca      (1000)     1738 2023-05-09 14:14:18.196657 frequenz-repo-config-0.1.0/PKG-INFO
--rw-r--r--   0 luca      (1000) luca      (1000)      341 2023-04-12 09:48:19.000000 frequenz-repo-config-0.1.0/README.md
--rw-r--r--   0 luca      (1000) luca      (1000)      343 2023-05-08 13:51:55.000000 frequenz-repo-config-0.1.0/noxfile.py
--rw-r--r--   0 luca      (1000) luca      (1000)     2846 2023-05-08 13:51:55.000000 frequenz-repo-config-0.1.0/pyproject.toml
--rw-r--r--   0 luca      (1000) luca      (1000)       38 2023-05-09 14:14:18.196657 frequenz-repo-config-0.1.0/setup.cfg
-drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-09 14:14:18.196657 frequenz-repo-config-0.1.0/src/
-drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-09 14:14:18.196657 frequenz-repo-config-0.1.0/src/frequenz/
--rw-r--r--   0 luca      (1000) luca      (1000)        0 2023-04-13 14:08:23.000000 frequenz-repo-config-0.1.0/src/frequenz/py.typed
-drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-09 14:14:18.196657 frequenz-repo-config-0.1.0/src/frequenz/repo/
-drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-09 14:14:18.196657 frequenz-repo-config-0.1.0/src/frequenz/repo/config/
--rw-r--r--   0 luca      (1000) luca      (1000)     6951 2023-05-08 13:51:55.000000 frequenz-repo-config-0.1.0/src/frequenz/repo/config/__init__.py
-drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-09 14:14:18.196657 frequenz-repo-config-0.1.0/src/frequenz/repo/config/nox/
--rw-r--r--   0 luca      (1000) luca      (1000)     1478 2023-03-31 14:27:27.000000 frequenz-repo-config-0.1.0/src/frequenz/repo/config/nox/__init__.py
--rw-r--r--   0 luca      (1000) luca      (1000)     6103 2023-05-08 13:51:55.000000 frequenz-repo-config-0.1.0/src/frequenz/repo/config/nox/config.py
--rw-r--r--   0 luca      (1000) luca      (1000)     3413 2023-05-08 13:51:55.000000 frequenz-repo-config-0.1.0/src/frequenz/repo/config/nox/default.py
--rw-r--r--   0 luca      (1000) luca      (1000)     4956 2023-05-08 13:51:55.000000 frequenz-repo-config-0.1.0/src/frequenz/repo/config/nox/session.py
--rw-r--r--   0 luca      (1000) luca      (1000)     6413 2023-05-08 13:51:55.000000 frequenz-repo-config-0.1.0/src/frequenz/repo/config/nox/util.py
--rw-r--r--   0 luca      (1000) luca      (1000)        0 2023-05-08 13:51:55.000000 frequenz-repo-config-0.1.0/src/frequenz/repo/config/py.typed
-drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-09 14:14:18.196657 frequenz-repo-config-0.1.0/src/frequenz/repo/config/setuptools/
--rw-r--r--   0 luca      (1000) luca      (1000)      157 2023-03-30 12:38:00.000000 frequenz-repo-config-0.1.0/src/frequenz/repo/config/setuptools/__init__.py
--rw-r--r--   0 luca      (1000) luca      (1000)     3279 2023-05-08 13:51:55.000000 frequenz-repo-config-0.1.0/src/frequenz/repo/config/setuptools/grpc_tools.py
-drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-09 14:14:18.196657 frequenz-repo-config-0.1.0/src/frequenz_repo_config.egg-info/
--rw-r--r--   0 luca      (1000) luca      (1000)     1738 2023-05-09 14:14:18.000000 frequenz-repo-config-0.1.0/src/frequenz_repo_config.egg-info/PKG-INFO
--rw-r--r--   0 luca      (1000) luca      (1000)      742 2023-05-09 14:14:18.000000 frequenz-repo-config-0.1.0/src/frequenz_repo_config.egg-info/SOURCES.txt
--rw-r--r--   0 luca      (1000) luca      (1000)        1 2023-05-09 14:14:18.000000 frequenz-repo-config-0.1.0/src/frequenz_repo_config.egg-info/dependency_links.txt
--rw-r--r--   0 luca      (1000) luca      (1000)       93 2023-05-09 14:14:18.000000 frequenz-repo-config-0.1.0/src/frequenz_repo_config.egg-info/entry_points.txt
--rw-r--r--   0 luca      (1000) luca      (1000)      714 2023-05-09 14:14:18.000000 frequenz-repo-config-0.1.0/src/frequenz_repo_config.egg-info/requires.txt
--rw-r--r--   0 luca      (1000) luca      (1000)        9 2023-05-09 14:14:18.000000 frequenz-repo-config-0.1.0/src/frequenz_repo_config.egg-info/top_level.txt
+drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-26 09:41:45.131061 frequenz-repo-config-0.2.0/
+-rw-r--r--   0 luca      (1000) luca      (1000)       34 2023-04-03 13:31:43.000000 frequenz-repo-config-0.2.0/.darglint
+-rw-r--r--   0 luca      (1000) luca      (1000)     2134 2023-03-10 15:07:55.000000 frequenz-repo-config-0.2.0/.gitignore
+-rw-r--r--   0 luca      (1000) luca      (1000)     1090 2023-03-31 14:27:27.000000 frequenz-repo-config-0.2.0/LICENSE
+-rw-r--r--   0 luca      (1000) luca      (1000)     2907 2023-05-26 09:41:45.131061 frequenz-repo-config-0.2.0/PKG-INFO
+-rw-r--r--   0 luca      (1000) luca      (1000)     1488 2023-05-24 13:01:23.000000 frequenz-repo-config-0.2.0/README.md
+drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-26 09:41:45.123061 frequenz-repo-config-0.2.0/cookiecutter/
+-rw-r--r--   0 luca      (1000) luca      (1000)      740 2023-05-24 13:01:23.000000 frequenz-repo-config-0.2.0/cookiecutter/cookiecutter.json
+drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-26 09:41:45.123061 frequenz-repo-config-0.2.0/cookiecutter/hooks/
+-rw-r--r--   0 luca      (1000) luca      (1000)    13771 2023-05-26 09:40:07.000000 frequenz-repo-config-0.2.0/cookiecutter/hooks/post_gen_project.py
+-rw-r--r--   0 luca      (1000) luca      (1000)     3001 2023-05-24 13:01:23.000000 frequenz-repo-config-0.2.0/cookiecutter/local_extensions.py
+drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-26 09:41:45.127061 frequenz-repo-config-0.2.0/cookiecutter/{{cookiecutter.github_repo_name}}/
+-rw-r--r--   0 luca      (1000) luca      (1000)     2134 2023-05-24 13:01:23.000000 frequenz-repo-config-0.2.0/cookiecutter/{{cookiecutter.github_repo_name}}/.gitignore
+-rw-r--r--   0 luca      (1000) luca      (1000)      316 2023-05-26 09:40:07.000000 frequenz-repo-config-0.2.0/cookiecutter/{{cookiecutter.github_repo_name}}/.gitmodules
+-rw-r--r--   0 luca      (1000) luca      (1000)     1090 2023-05-24 13:01:23.000000 frequenz-repo-config-0.2.0/cookiecutter/{{cookiecutter.github_repo_name}}/LICENSE
+-rw-r--r--   0 luca      (1000) luca      (1000)      130 2023-05-24 13:01:23.000000 frequenz-repo-config-0.2.0/cookiecutter/{{cookiecutter.github_repo_name}}/README.md
+-rw-r--r--   0 luca      (1000) luca      (1000)      216 2023-05-24 13:01:23.000000 frequenz-repo-config-0.2.0/cookiecutter/{{cookiecutter.github_repo_name}}/noxfile.py
+drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-26 09:41:45.123061 frequenz-repo-config-0.2.0/cookiecutter/{{cookiecutter.github_repo_name}}/proto/
+drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-26 09:41:45.123061 frequenz-repo-config-0.2.0/cookiecutter/{{cookiecutter.github_repo_name}}/proto/frequenz/
+drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-26 09:41:45.123061 frequenz-repo-config-0.2.0/cookiecutter/{{cookiecutter.github_repo_name}}/proto/frequenz/api/
+drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-26 09:41:45.127061 frequenz-repo-config-0.2.0/cookiecutter/{{cookiecutter.github_repo_name}}/proto/frequenz/api/{{cookiecutter.name}}/
+-rw-r--r--   0 luca      (1000) luca      (1000)      433 2023-05-24 13:01:23.000000 frequenz-repo-config-0.2.0/cookiecutter/{{cookiecutter.github_repo_name}}/proto/frequenz/api/{{cookiecutter.name}}/{{cookiecutter.name}}.proto
+-rw-r--r--   0 luca      (1000) luca      (1000)     4317 2023-05-26 09:40:07.000000 frequenz-repo-config-0.2.0/cookiecutter/{{cookiecutter.github_repo_name}}/pyproject.toml
+drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-26 09:41:45.123061 frequenz-repo-config-0.2.0/cookiecutter/{{cookiecutter.github_repo_name}}/src/
+drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-26 09:41:45.123061 frequenz-repo-config-0.2.0/cookiecutter/{{cookiecutter.github_repo_name}}/src/frequenz/
+drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-26 09:41:45.123061 frequenz-repo-config-0.2.0/cookiecutter/{{cookiecutter.github_repo_name}}/src/frequenz/{{cookiecutter.type}}/
+drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-26 09:41:45.127061 frequenz-repo-config-0.2.0/cookiecutter/{{cookiecutter.github_repo_name}}/src/frequenz/{{cookiecutter.type}}/{{cookiecutter.name}}/
+-rw-r--r--   0 luca      (1000) luca      (1000)      646 2023-05-24 13:01:23.000000 frequenz-repo-config-0.2.0/cookiecutter/{{cookiecutter.github_repo_name}}/src/frequenz/{{cookiecutter.type}}/{{cookiecutter.name}}/__init__.py
+-rw-r--r--   0 luca      (1000) luca      (1000)        0 2023-05-24 13:01:23.000000 frequenz-repo-config-0.2.0/cookiecutter/{{cookiecutter.github_repo_name}}/src/frequenz/{{cookiecutter.type}}/{{cookiecutter.name}}/py.typed
+drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-26 09:41:45.127061 frequenz-repo-config-0.2.0/cookiecutter/{{cookiecutter.github_repo_name}}/tests/
+-rw-r--r--   0 luca      (1000) luca      (1000)     1361 2023-05-24 13:01:23.000000 frequenz-repo-config-0.2.0/cookiecutter/{{cookiecutter.github_repo_name}}/tests/test_{{cookiecutter.name}}.py
+-rw-r--r--   0 luca      (1000) luca      (1000)      335 2023-05-24 13:01:23.000000 frequenz-repo-config-0.2.0/noxfile.py
+-rw-r--r--   0 luca      (1000) luca      (1000)     3184 2023-05-24 13:58:13.000000 frequenz-repo-config-0.2.0/pyproject.toml
+-rw-r--r--   0 luca      (1000) luca      (1000)       38 2023-05-26 09:41:45.131061 frequenz-repo-config-0.2.0/setup.cfg
+drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-26 09:41:45.123061 frequenz-repo-config-0.2.0/src/
+drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-26 09:41:45.127061 frequenz-repo-config-0.2.0/src/frequenz/
+-rw-r--r--   0 luca      (1000) luca      (1000)        0 2023-04-13 14:08:23.000000 frequenz-repo-config-0.2.0/src/frequenz/py.typed
+drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-26 09:41:45.123061 frequenz-repo-config-0.2.0/src/frequenz/repo/
+drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-26 09:41:45.127061 frequenz-repo-config-0.2.0/src/frequenz/repo/config/
+-rw-r--r--   0 luca      (1000) luca      (1000)     8427 2023-05-26 09:40:07.000000 frequenz-repo-config-0.2.0/src/frequenz/repo/config/__init__.py
+-rw-r--r--   0 luca      (1000) luca      (1000)      501 2023-05-17 11:36:59.000000 frequenz-repo-config-0.2.0/src/frequenz/repo/config/_core.py
+drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-26 09:41:45.127061 frequenz-repo-config-0.2.0/src/frequenz/repo/config/nox/
+-rw-r--r--   0 luca      (1000) luca      (1000)     1478 2023-03-31 14:27:27.000000 frequenz-repo-config-0.2.0/src/frequenz/repo/config/nox/__init__.py
+-rw-r--r--   0 luca      (1000) luca      (1000)     6257 2023-05-25 10:46:13.000000 frequenz-repo-config-0.2.0/src/frequenz/repo/config/nox/config.py
+-rw-r--r--   0 luca      (1000) luca      (1000)     3708 2023-05-24 13:01:23.000000 frequenz-repo-config-0.2.0/src/frequenz/repo/config/nox/default.py
+-rw-r--r--   0 luca      (1000) luca      (1000)     4996 2023-05-17 11:36:59.000000 frequenz-repo-config-0.2.0/src/frequenz/repo/config/nox/session.py
+-rw-r--r--   0 luca      (1000) luca      (1000)     6943 2023-05-24 13:01:23.000000 frequenz-repo-config-0.2.0/src/frequenz/repo/config/nox/util.py
+-rw-r--r--   0 luca      (1000) luca      (1000)        0 2023-05-08 13:51:55.000000 frequenz-repo-config-0.2.0/src/frequenz/repo/config/py.typed
+drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-26 09:41:45.131061 frequenz-repo-config-0.2.0/src/frequenz/repo/config/setuptools/
+-rw-r--r--   0 luca      (1000) luca      (1000)      157 2023-03-30 12:38:00.000000 frequenz-repo-config-0.2.0/src/frequenz/repo/config/setuptools/__init__.py
+-rw-r--r--   0 luca      (1000) luca      (1000)     5305 2023-05-26 09:40:07.000000 frequenz-repo-config-0.2.0/src/frequenz/repo/config/setuptools/grpc_tools.py
+drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-26 09:41:45.131061 frequenz-repo-config-0.2.0/src/frequenz_repo_config.egg-info/
+-rw-r--r--   0 luca      (1000) luca      (1000)     2907 2023-05-26 09:41:45.000000 frequenz-repo-config-0.2.0/src/frequenz_repo_config.egg-info/PKG-INFO
+-rw-r--r--   0 luca      (1000) luca      (1000)     1830 2023-05-26 09:41:45.000000 frequenz-repo-config-0.2.0/src/frequenz_repo_config.egg-info/SOURCES.txt
+-rw-r--r--   0 luca      (1000) luca      (1000)        1 2023-05-26 09:41:45.000000 frequenz-repo-config-0.2.0/src/frequenz_repo_config.egg-info/dependency_links.txt
+-rw-r--r--   0 luca      (1000) luca      (1000)       93 2023-05-26 09:41:45.000000 frequenz-repo-config-0.2.0/src/frequenz_repo_config.egg-info/entry_points.txt
+-rw-r--r--   0 luca      (1000) luca      (1000)      759 2023-05-26 09:41:45.000000 frequenz-repo-config-0.2.0/src/frequenz_repo_config.egg-info/requires.txt
+-rw-r--r--   0 luca      (1000) luca      (1000)        9 2023-05-26 09:41:45.000000 frequenz-repo-config-0.2.0/src/frequenz_repo_config.egg-info/top_level.txt
+drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-26 09:41:45.131061 frequenz-repo-config-0.2.0/tests/
+-rw-r--r--   0 luca      (1000) luca      (1000)      102 2023-05-17 11:36:44.000000 frequenz-repo-config-0.2.0/tests/__init__.py
+drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-26 09:41:45.131061 frequenz-repo-config-0.2.0/tests/integration/
+-rw-r--r--   0 luca      (1000) luca      (1000)     1208 2023-05-26 09:40:07.000000 frequenz-repo-config-0.2.0/tests/integration/test_cookiecutter_generation.py
+drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-26 09:41:45.131061 frequenz-repo-config-0.2.0/tests/nox/
+-rw-r--r--   0 luca      (1000) luca      (1000)      103 2023-05-17 11:36:44.000000 frequenz-repo-config-0.2.0/tests/nox/__init__.py
+-rw-r--r--   0 luca      (1000) luca      (1000)      831 2023-05-17 11:36:44.000000 frequenz-repo-config-0.2.0/tests/nox/test_default.py
+-rw-r--r--   0 luca      (1000) luca      (1000)      508 2023-05-17 11:36:58.000000 frequenz-repo-config-0.2.0/tests/test_core.py
+-rw-r--r--   0 luca      (1000) luca      (1000)      710 2023-05-17 11:36:57.000000 frequenz-repo-config-0.2.0/tests/test_pyproject.py
+-rw-r--r--   0 luca      (1000) luca      (1000)      322 2023-05-17 11:36:44.000000 frequenz-repo-config-0.2.0/tests/utils.py
```

### Comparing `frequenz-repo-config-0.1.0/.gitignore` & `frequenz-repo-config-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.1.0/LICENSE` & `frequenz-repo-config-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.1.0/pyproject.toml` & `frequenz-repo-config-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -44,37 +44,41 @@
 api = [
   "grpcio-tools >= 1.47.0, < 2",
   "mypy-protobuf >= 3.0.0, < 4",
   "setuptools >= 67.6.0, < 68",
 ]
 app = []
 lib = []
+model = []
 dev-docs-gen = [
   "mike == 1.1.2",
   "mkdocs-gen-files == 0.4.0",
   "mkdocs-literate-nav == 0.4.0",
   "mkdocs-material == 9.1.4",
   "mkdocs-section-index == 0.3.5",
   "mkdocstrings[python] == 0.20.0",
 ]
 dev-docstrings = ["pydocstyle == 6.3.0", "darglint == 1.8.1"]
 dev-formatting = ["black == 23.3.0", "isort == 5.12.0"]
 dev-mypy = [
   "mypy == 1.1.1",
   "types-setuptools >= 67.6.0, < 68", # Should match the global dependency
   # For checking the docs/ script, and tests
-  "frequenz-repo-config[docs-gen,pytest]",
+  "frequenz-repo-config[dev-docs-gen,dev-pytest]",
 ]
 dev-pylint = [
   "pylint == 2.17.1",
   "pylint-google-style-guide-imports-enforcing == 1.3.0",
   # For checking the docs/ script, and tests
-  "frequenz-repo-config[docs-gen,pytest]",
+  "frequenz-repo-config[dev-docs-gen,dev-pytest]",
+]
+dev-pytest = [
+  "pytest == 7.2.2",
+  "cookiecutter == 2.1.1", # For checking the cookiecutter scripts
 ]
-dev-pytest = ["pytest == 7.2.2"]
 dev = [
   "frequenz-repo-config[dev-docs-gen,dev-docstrings,dev-formatting,dev-pytest,dev-mypy,dev-pylint]",
 ]
 
 [project.urls]
 Changelog = "https://github.com/frequenz-floss/frequenz-repo-config-python/releases"
 Repository = "https://github.com/frequenz-floss/frequenz-repo-config-python"
@@ -100,7 +104,17 @@
   "ungrouped-imports",
 ]
 
 [tool.isort]
 profile = "black"
 line_length = 88
 src_paths = ["src"]
+
+[[tool.mypy.overrides]]
+module = ["cookiecutter", "cookiecutter.*"]
+ignore_missing_imports = true
+
+[tool.pytest.ini_options]
+testpaths = ["tests"]
+markers = [
+  "integration: integration tests (deselect with '-m \"not integration\"')",
+]
```

### Comparing `frequenz-repo-config-0.1.0/src/frequenz/repo/config/__init__.py` & `frequenz-repo-config-0.2.0/src/frequenz/repo/config/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 # License: MIT
 # Copyright © 2023 Frequenz Energy-as-a-Service GmbH
 
-"""Frequenz project setup tools and common configuration.
+r"""Frequenz project setup tools and common configuration.
 
-The tools are provided to configure 4 main types of repositories:
-
-- APIs (api)
-- Actors (actor)
-- Applications (app)
-- Libraries (lib)
+The tools are provided to configure the main types of repositories most commonly used at
+Frequenz, defined in
+[`freq.repo.config.RepositoryType`][freq.repo.config.RepositoryType].
+
+- actor: SDK actors
+- api: gRPC APIs
+- app: SDK applications
+- lib: General purpose Python libraries
+- model: SDK machine learning models
 
 # Common
 
 ## `nox`
 
 ### Writing the `noxfile.py`
 
@@ -28,16 +31,16 @@
 
 ```python
 from frequenz.repo.config import nox
 
 nox.configure(nox.default.lib_config)
 ```
 
-Again, make sure to pick the correct default configuration based on the type of
-your project (`api_config`, `actor_config`, `app_config`, `lib_config`).
+Again, make sure to pick the correct default configuration based on the type of your
+project (`actor_config`, `api_config`, `app_config`, `lib_config`, `model_config`).
 
 If you need to modify the configuration, you can copy one of the default
 configurations by using the
 [`copy()`][frequenz.repo.config.nox.config.Config.copy] method:
 
 ```python
 from frequenz.repo.config import nox
@@ -159,23 +162,29 @@
 - `proto/`: Directory containing the `.proto` files.
 - `py/`: Directory containing the Python code. It should only provide
   a `py.typed` file and a `__init__.py` file. API repositories should not
   contain any other Python code.
 - `pytests/`: Directory containing the tests for the Python code.
 - `submodules/api-common-protos`: Directory containing the submodule with the
   `google/api-common-protos` repository.
+- `submodules/frequenz-api-common`: Directory containing the submodule with the
+  `frequenz-floss/frequenz-api-common` repository.
 
 Normally Frequenz APIs use basic types from
-[`google/api-common-protos`](https://github.com/googleapis/api-common-protos),
-so you need to make sure the proper submodule is added to your project:
+[`google/api-common-protos`](https://github.com/googleapis/api-common-protos) and
+[`frequenz-floss/frequenz-api-common`](https://github.com/frequenz-floss/frequenz-api-common),
+so you need to make sure the proper submodules are added to your project:
 
 ```sh
 mkdir submodules
-git submodule add https://github.com:googleapis/api-common-protos.git submodules/api-common-protos
-git commit -m "Add Google api-common-protos submodule" submodules/api-common-protos
+git submodule add https://github.com/googleapis/api-common-protos.git \
+        submodules/api-common-protos
+git submodule add https://github.com/frequenz-floss/frequenz-api-common.git \
+        submodules/frequenz-api-common
+git commit -m "Add api-common-protos and frequenz-api-common submodules" submodules
 ```
 
 Then you need to add this package as a build dependency and a few extra
 dependencies to your project, for example:
 
 ```toml
 requires = [
@@ -183,16 +192,17 @@
   "setuptools_scm[toml] >= 7.1.0, < 8",
   "frequenz-repo-config[api] >= 0.1.0, < 0.2.0",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 dependencies = [
-  "googleapis-common-protos == 1.56.2",
-  "grpcio == 1.51.0",
+  "frequenz-api-common >= 0.2.0, < 0.3.0",
+  "googleapis-common-protos >= 1.56.2, < 2",
+  "grpcio >= 1.51.1, < 2",
 ]
 ```
 
 Note the `api` extra in `frequenz-repo-config[api]`, this will ensure all
 dependencies to build the protocol files will be installed when building the
 package. Of course you need to replace the version numbers with the correct
 ones too.
@@ -215,20 +225,40 @@
 source distribution, as well as the Google api-common-protos files, as it
 is not handled automatically yet
 ([#13](https://github.com/frequenz-floss/frequenz-repo-config-python/issues/13)).
 Make sure to include these lines in the `MANIFEST.in` file:
 
 ```
 recursive-include submodules/api-common-protos/google *.proto
+recursive-include submodules/frequenz-api-common/proto *.proto
+```
+
+If the defaults are not suitable for you (for example you need to use more or less
+submodules or your proto files are located somewhere else, you can customize how
+the protocol files are generated by adding the following section to your
+`pyproject.toml` file:
+
+```toml
+[tool.frequenz_repo_config.setuptools.grpc_tools]
+# Location of the proto files relative to the root of the repository (default: "proto")
+proto_path = "proto_files"
+# Glob pattern to use to find the proto files in the proto_path (default: "*.proto")
+proto_glob = "*.prt"  # Default: "*.proto"
+# List of paths to pass to the protoc compiler as include paths (default:
+# ["submodules/api-common-protos", "submodules/frequenz-api-common/proto"])
+include_paths = ["submodules/api-common-protos"]
+# Path where to generate the Python files (default: "py")
+py_path = "generated"
 ```
 
-For now there is no way to customize where the protocol files are located,
-where the generated files should be placed, or which extra directories must be
-included when compiling the protocol files.
+Please adapt the instructions above to your project structure if you need to change the
+defaults.
 """
 
 from . import nox, setuptools
+from ._core import RepositoryType
 
 __all__ = [
+    "RepositoryType",
     "nox",
     "setuptools",
 ]
```

### Comparing `frequenz-repo-config-0.1.0/src/frequenz/repo/config/nox/__init__.py` & `frequenz-repo-config-0.2.0/src/frequenz/repo/config/nox/__init__.py`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.1.0/src/frequenz/repo/config/nox/config.py` & `frequenz-repo-config-0.2.0/src/frequenz/repo/config/nox/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,104 +8,105 @@
 
 The `get()` function can be used to retrieve the current configuration object
 so it can be used when implementing custom nox sessions.
 
 The `configure()` function must be called before `get()` is used.
 """
 
-import dataclasses
+import dataclasses as _dataclasses
+import itertools as _itertools
 from typing import Self
 
-import nox
+import nox as _nox
 
-from . import util
+from . import util as _util
 
 
-@dataclasses.dataclass(kw_only=True, slots=True)
+@_dataclasses.dataclass(kw_only=True, slots=True)
 class CommandsOptions:
     """Command-line options for each command."""
 
-    black: list[str] = dataclasses.field(default_factory=lambda: [])
+    black: list[str] = _dataclasses.field(default_factory=lambda: [])
     """Command-line options for the `black` command."""
 
-    darglint: list[str] = dataclasses.field(default_factory=lambda: [])
+    darglint: list[str] = _dataclasses.field(default_factory=lambda: [])
     """Command-line options for the `darglint` command."""
 
-    isort: list[str] = dataclasses.field(default_factory=lambda: [])
+    isort: list[str] = _dataclasses.field(default_factory=lambda: [])
     """Command-line options for the `isort` command."""
 
-    mypy: list[str] = dataclasses.field(default_factory=lambda: [])
+    mypy: list[str] = _dataclasses.field(default_factory=lambda: [])
     """Command-line options for the `mypy` command."""
 
-    pydocstyle: list[str] = dataclasses.field(default_factory=lambda: [])
+    pydocstyle: list[str] = _dataclasses.field(default_factory=lambda: [])
     """Command-line options for the `pydocstyle` command."""
 
-    pylint: list[str] = dataclasses.field(default_factory=lambda: [])
+    pylint: list[str] = _dataclasses.field(default_factory=lambda: [])
     """Command-line options for the `pylint` command."""
 
-    pytest: list[str] = dataclasses.field(default_factory=lambda: [])
+    pytest: list[str] = _dataclasses.field(default_factory=lambda: [])
     """Command-line options for the `pytest` command."""
 
     def copy(self) -> Self:
         """Create a new object as a copy of self.
 
         Returns:
             The copy of self.
         """
-        return dataclasses.replace(self)
+        return _dataclasses.replace(self)
 
 
-@dataclasses.dataclass(kw_only=True, slots=True)
+@_dataclasses.dataclass(kw_only=True, slots=True)
 class Config:
     """Configuration for nox sessions."""
 
-    opts: CommandsOptions = dataclasses.field(default_factory=CommandsOptions)
+    opts: CommandsOptions = _dataclasses.field(default_factory=CommandsOptions)
     """Command-line options for each command used by sessions."""
 
-    sessions: list[str] = dataclasses.field(default_factory=lambda: [])
+    sessions: list[str] = _dataclasses.field(default_factory=lambda: [])
     """List of sessions to run."""
 
-    source_paths: list[str] = dataclasses.field(default_factory=lambda: [])
+    source_paths: list[str] = _dataclasses.field(default_factory=lambda: [])
     """List of paths containing source files that should be analyzed by the sessions.
 
     Source paths are inspected for `__init__.py` files to look for packages.
     The path should be the top-level directory containing packages that will be
     actually part of the distribution, not development paths, like tests,
     benchmarks, etc.
 
     This path will be removed when calculating the package name for the found
     packages. `mypy` needs the package name to be able to do full import
     checking.
     """
 
-    extra_paths: list[str] = dataclasses.field(default_factory=lambda: [])
+    extra_paths: list[str] = _dataclasses.field(default_factory=lambda: [])
     """List of extra paths to be analyzed by the sessions.
 
     These are not inspected for packages, as they are passed verbatim to the
     tools invoked by the sessions.
     """
 
     def __post_init__(self) -> None:
         """Initialize the configuration object.
 
         This will add extra paths discovered in config files and other sources.
         """
-        for path in util.discover_paths():
+        for path in _util.discover_paths():
             if path not in self.extra_paths:
                 self.extra_paths.append(path)
 
     def copy(self, /) -> Self:
         """Create a new object as a copy of self.
 
         Returns:
             The copy of self.
         """
-        return dataclasses.replace(self)
+        return _dataclasses.replace(self)
 
-    def path_args(self, session: nox.Session, /) -> list[str]:
+    def path_args(self, session: _nox.Session, /) -> list[str]:
         """Return the file paths to run the checks on.
 
         If positional arguments are present in the nox session, those are used
         as the file paths verbatim, and if not, all **existing** `source_paths`
         and `extra_paths` are used.
 
         Args:
@@ -113,19 +114,19 @@
 
         Returns:
             The file paths to run the checks on.
         """
         if session.posargs:
             return session.posargs
 
-        return [
-            str(p) for p in util.existing_paths(self.source_paths + self.extra_paths)
-        ]
+        return list(
+            str(p) for p in _util.existing_paths(self.source_paths + self.extra_paths)
+        )
 
-    def package_args(self, session: nox.Session, /) -> list[str]:
+    def package_args(self, session: _nox.Session, /) -> list[str]:
         """Return the package names to run the checks on.
 
         If positional arguments are present in the nox session, those are used
         as the file paths verbatim, and if not, all **existing** `source_paths`
         are searched for python packges by looking for `__init__.py` files.
         `extra_paths` are used as is, only converting the paths to python
         package names (replacing `/` with `.` and removing the suffix `.pyi?`
@@ -137,29 +138,31 @@
         Returns:
             The package names found in the `source_paths`.
         """
         if session.posargs:
             return session.posargs
 
         sources_package_dirs_with_roots = (
-            (p, util.find_toplevel_package_dirs(p))
-            for p in util.existing_paths(self.source_paths)
+            (p, _util.find_toplevel_package_dirs(p))
+            for p in _util.existing_paths(self.source_paths)
         )
 
         source_packages = (
-            util.path_to_package(pkg_path, root=root)
+            _util.path_to_package(pkg_path, root=root)
             for root, pkg_paths in sources_package_dirs_with_roots
             for pkg_path in pkg_paths
         )
 
         extra_packages = (
-            util.path_to_package(p) for p in util.existing_paths(self.extra_paths)
+            _util.path_to_package(p) for p in _util.existing_paths(self.extra_paths)
         )
 
-        return [*source_packages, *extra_packages]
+        return list(
+            _util.deduplicate(_itertools.chain(source_packages, extra_packages))
+        )
 
 
 _config: Config | None = None
 """The global configuration object."""
 
 
 def get() -> Config:
@@ -178,8 +181,8 @@
     """Configure nox using the provided configuration.
 
     Args:
         conf: The configuration to use to configure nox.
     """
     global _config  # pylint: disable=global-statement
     _config = conf
-    nox.options.sessions = _config.sessions
+    _nox.options.sessions = _config.sessions
```

### Comparing `frequenz-repo-config-0.1.0/src/frequenz/repo/config/nox/default.py` & `frequenz-repo-config-0.2.0/src/frequenz/repo/config/nox/default.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,37 @@
 # License: MIT
 # Copyright © 2023 Frequenz Energy-as-a-Service GmbH
 
 """Default nox configuration for different types of repositories.
 
-This module provides the default configuration for different types of
-repositories:
-
-- Libraries (lib)
-- APIs (api)
-- Actors (actor)
-- Applications (app)
-
-The `lib_config`, `api_config`, `actor_config` and `app_config`
-variables are the default configurations for libraries, APIs, actors and
-applications, respectively. The `common_config` variable is the default
-configuration for all types of repositories.
-
-The `lib_command_options`, `api_command_options`, `actor_command_options` and
-`app_command_options` variables are the default command-line options for the same
-types of repositories, and the `common_command_options` variable is the default
-command-line options for all types of repositories.
+This module provides the default configuration for the different types of
+repositories defined by
+[`frequenz.repo.config.RepositoryType`][frequenz.repo.config.RepositoryType].
+
+The `actor_config`, `api_config`, `app_config`, `lib_config`, and `model_config`
+variables are the default configurations for libraries, APIs, actors and applications,
+respectively. The `common_config` variable is the default configuration for all types of
+repositories.
+
+The `actor_command_options`, `api_command_options`, `app_command_options`,
+`lib_command_options`, and `model_command_options` variables are the default
+command-line options for the same types of repositories, and the
+`common_command_options` variable is the default command-line options for all types of
+repositories.
 
 They can be modified before being passed to
 [`nox.configure()`][frequenz.repo.config.nox.configure] by using the
 [`CommandsOptions.copy()`][frequenz.repo.config.nox.config.CommandsOptions.copy]
 method.
 """
 
 import dataclasses
 
 from . import config as _config
-from . import util
+from . import util as _util
 
 common_command_options: _config.CommandsOptions = _config.CommandsOptions(
     black=[
         "--check",
     ],
     darglint=[
         "-v2",  # for verbose error messages.
@@ -76,41 +73,47 @@
         "examples",
         "noxfile.py",
         "tests",
     ],
 )
 """Default configuration for all types of repositories."""
 
-lib_command_options: _config.CommandsOptions = common_command_options.copy()
-"""Default command-line options for libraries."""
+actor_command_options: _config.CommandsOptions = common_command_options.copy()
+"""Default command-line options for actors."""
 
-lib_config: _config.Config = common_config.copy()
-"""Default configuration for libraries."""
+actor_config: _config.Config = common_config.copy()
+"""Default configuration for actors."""
 
 api_command_options: _config.CommandsOptions = common_command_options.copy()
 """Default command-line options for APIs."""
 
 api_config: _config.Config = dataclasses.replace(
     common_config,
     opts=api_command_options,
     # We don't check the sources at all because they are automatically generated.
     source_paths=[],
     # We adapt the path to the tests.
-    extra_paths=list(util.replace(common_config.extra_paths, {"tests": "pytests"})),
+    extra_paths=list(_util.replace(common_config.extra_paths, {"tests": "pytests"})),
 )
 """Default configuration for APIs.
 
 Same as `common_config`, but with `source_paths` replacing `"src"` with `"py"`
 and `extra_paths` replacing `"tests"` with `"pytests"`.
 """
 
-actor_command_options: _config.CommandsOptions = common_command_options.copy()
-"""Default command-line options for actors."""
-
-actor_config: _config.Config = common_config.copy()
-"""Default configuration for actors."""
-
 app_command_options: _config.CommandsOptions = common_command_options.copy()
 """Default command-line options for applications."""
 
 app_config: _config.Config = common_config.copy()
 """Default configuration for applications."""
+
+lib_command_options: _config.CommandsOptions = common_command_options.copy()
+"""Default command-line options for libraries."""
+
+lib_config: _config.Config = common_config.copy()
+"""Default configuration for libraries."""
+
+model_command_options: _config.CommandsOptions = common_command_options.copy()
+"""Default command-line options for models."""
+
+model_config: _config.Config = common_config.copy()
+"""Default configuration for models."""
```

### Comparing `frequenz-repo-config-0.1.0/src/frequenz/repo/config/nox/session.py` & `frequenz-repo-config-0.2.0/src/frequenz/repo/config/nox/session.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 """Predefined nox sessions.
 
 This module defines the predefined nox sessions that are used by the default.
 """
 
 import nox
 
-from . import config, util
+from . import config as _config
+from . import util as _util
 
 
 @nox.session
 def ci_checks_max(session: nox.Session) -> None:
     """Run all checks with max dependencies in a single session.
 
     This is faster than running the checks separately, so it is suitable for CI.
@@ -38,15 +39,15 @@
     Args:
         session: the nox session.
         install_deps: True if dependencies should be installed.
     """
     if install_deps:
         session.install("-e", ".[dev-formatting]")
 
-    conf = config.get()
+    conf = _config.get()
     session.run("black", *conf.opts.black, *conf.path_args(session))
     session.run("isort", *conf.opts.isort, *conf.path_args(session))
 
 
 @nox.session
 def mypy(session: nox.Session, install_deps: bool = True) -> None:
     """Check type hints with mypy.
@@ -56,16 +57,16 @@
         install_deps: True if dependencies should be installed.
     """
     if install_deps:
         # install the package itself as editable, so that it is possible to do
         # fast local tests with `nox -R -e mypy`.
         session.install("-e", ".[dev-mypy]")
 
-    conf = config.get()
-    pkg_args = util.flatten(("-p", p) for p in conf.package_args(session))
+    conf = _config.get()
+    pkg_args = _util.flatten(("-p", p) for p in conf.package_args(session))
     session.run("mypy", *conf.opts.mypy, *pkg_args)
 
 
 @nox.session
 def pylint(session: nox.Session, install_deps: bool = True) -> None:
     """Check for code smells with pylint.
 
@@ -74,30 +75,30 @@
         install_deps: True if dependencies should be installed.
     """
     if install_deps:
         # install the package itself as editable, so that it is possible to do
         # fast local tests with `nox -R -e pylint`.
         session.install("-e", ".[dev-pylint]")
 
-    conf = config.get()
+    conf = _config.get()
     session.run("pylint", *conf.opts.pylint, *conf.path_args(session))
 
 
 @nox.session
 def docstrings(session: nox.Session, install_deps: bool = True) -> None:
     """Check docstring tone with pydocstyle and param descriptions with darglint.
 
     Args:
         session: the nox session.
         install_deps: True if dependencies should be installed.
     """
     if install_deps:
         session.install("-e", ".[dev-docstrings]")
 
-    conf = config.get()
+    conf = _config.get()
     session.run("pydocstyle", *conf.opts.pydocstyle, *conf.path_args(session))
 
     # Darglint checks that function argument and return values are documented.
     # This is needed only for the `src` dir, so we exclude the other top level
     # dirs that contain code, unless some paths were specified by argument, in
     # which case we use those untouched.
     darglint_paths = session.posargs or filter(
@@ -132,23 +133,23 @@
     Args:
         session: the nox session.
         install_deps: True if dependencies should be installed.
     """
     if install_deps:
         # install the package itself as editable, so that it is possible to do
         # fast local tests with `nox -R -e pytest_min`.
-        session.install("-e", ".[dev-pytest]", *util.min_dependencies())
+        session.install("-e", ".[dev-pytest]", *_util.min_dependencies())
 
     _pytest_impl(session, "min")
 
 
 def _pytest_impl(
     session: nox.Session, max_or_min_deps: str  # pylint: disable=unused-argument
 ) -> None:
-    conf = config.get()
+    conf = _config.get()
     session.run("pytest", *conf.opts.pytest, *session.posargs)
 
     # pylint: disable=fixme
     # TODO: Implement coverage reporting, we need to research this a bit and it
     # makes sense to do so when we actually collect the coverage somewhere
     # "--cov=frequenz.sdk",
     # "--cov-report=term",
```

### Comparing `frequenz-repo-config-0.1.0/src/frequenz/repo/config/nox/util.py` & `frequenz-repo-config-0.2.0/src/frequenz/repo/config/nox/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 """General purpose utilities.
 
 This module contains general purpose utilities that are used by the other
 modules in this package.
 """
 
 
-import pathlib
-import tomllib
+import pathlib as _pathlib
+import tomllib as _tomllib
 from collections.abc import Iterable, Mapping
 from typing import TypeVar
 
 _T = TypeVar("_T")
 
 
 def flatten(iterables: Iterable[Iterable[_T]], /) -> Iterable[_T]:
@@ -47,42 +47,56 @@
     for item in iterable:
         if item in replacements:
             yield replacements[item]
         else:
             yield item
 
 
-def existing_paths(paths: Iterable[str], /) -> Iterable[pathlib.Path]:
-    """Filter paths to only leave valid paths that exist.
+def deduplicate(iterable: Iterable[_T], /) -> Iterable[_T]:
+    """Filter out duplicates from an iterable preserving the original iterable order.
+
+    Args:
+        iterable: The iterable to remove duplicates from.
+
+    Returns:
+        The elements of `iterable`, without duplicates but preserving order.
+    """
+    # We can't use a set() here because sets don't preserve order.  We use this hack
+    # with dict.fromkeys() because dicts do preserve order in Python 3.7+.
+    return dict.fromkeys(iterable).keys()
+
+
+def existing_paths(paths: Iterable[str], /) -> Iterable[_pathlib.Path]:
+    """Filter paths to only leave valid paths that exist and are unique.
 
     Args:
         paths: The paths to check and filter.
 
     Returns:
         An iterable with the valid paths as `pathlib.Path` objects.
 
     Example:
         >>> assert list(existing_paths([".", "/fake"])) == [pathlib.Path(".")]
     """
-    return (p for p in map(pathlib.Path, paths) if p.exists())
+    return deduplicate(p for p in map(_pathlib.Path, paths) if p.exists())
 
 
-def is_python_file(path: pathlib.Path, /) -> bool:
+def is_python_file(path: _pathlib.Path, /) -> bool:
     """Check if a path is a Python file.
 
     Args:
         path: The path to check.
 
     Returns:
         `True` if the path is a Python file, `False` otherwise.
     """
     return path.suffix in (".py", ".pyi")
 
 
-def path_to_package(path: pathlib.Path, root: pathlib.Path | None = None) -> str:
+def path_to_package(path: _pathlib.Path, root: _pathlib.Path | None = None) -> str:
     """Convert paths to Python package names.
 
     Paths should exist and be either a directory or a file ending with `.pyi?`
     (otherwise this function will assert). The `root` and `path` are
     concatenated when performing the check.
 
     Directory separators in `path` are replaced with `.` and the `.pyi?` suffix
@@ -107,16 +121,16 @@
 
     if is_python_file(real_path):
         path = path.with_suffix("")
     return path.as_posix().replace("/", ".")
 
 
 def find_toplevel_package_dirs(
-    path: pathlib.Path, /, *, root: pathlib.Path | None = None
-) -> Iterable[pathlib.Path]:
+    path: _pathlib.Path, /, *, root: _pathlib.Path | None = None
+) -> Iterable[_pathlib.Path]:
     """Find top-level packages directories in a `path`.
 
     Searches recursively for the top-level packages in `path`, relative to
     `root`.
 
     Args:
         path: The path to look for python packages.
@@ -163,30 +177,29 @@
         )
     return ()
 
 
 def min_dependencies() -> list[str]:
     """Extract the minimum dependencies from pyproject.toml.
 
-    Raises:
-        RuntimeError: If minimun dependencies are not properly
-            set in pyproject.toml.
-
     Returns:
-        the minimun dependencies defined in pyproject.toml.
+        The minimun dependencies defined in pyproject.toml.
 
+    Raises:
+        RuntimeError: If minimun dependencies are not properly set in pyproject.toml.
     """
     with open("pyproject.toml", "rb") as toml_file:
-        data = tomllib.load(toml_file)
+        data = _tomllib.load(toml_file)
+
+    min_deps: list[str] = []
 
     dependencies = data.get("project", {}).get("dependencies", {})
     if not dependencies:
-        raise RuntimeError(f"No dependencies found in file: {toml_file.name}")
+        return min_deps
 
-    min_deps: list[str] = []
     for dep in dependencies:
         min_dep = dep.split(",")[0]
         if any(op in min_dep for op in (">=", "==")):
             min_deps.append(min_dep.replace(">=", "=="))
         else:
             raise RuntimeError(f"Minimum requirement is not set: {dep}")
     return min_deps
@@ -203,17 +216,17 @@
     - The `testpaths` option in the `tools.pytest.ini_options` section of
       `pyproject.toml`.
 
     Returns:
         The discovered paths to check.
     """
     with open("pyproject.toml", "rb") as toml_file:
-        data = tomllib.load(toml_file)
+        data = _tomllib.load(toml_file)
 
     testpaths: list[str] = (
         data.get("tool", {})
         .get("pytest", {})
         .get("ini_options", {})
         .get("testpaths", [])
     )
 
-    return testpaths
+    return list(deduplicate(testpaths))
```

### Comparing `frequenz-repo-config-0.1.0/src/frequenz_repo_config.egg-info/requires.txt` & `frequenz-repo-config-0.2.0/src/frequenz_repo_config.egg-info/requires.txt`

 * *Files 21% similar despite different names*

```diff
@@ -27,18 +27,21 @@
 [dev-formatting]
 black==23.3.0
 isort==5.12.0
 
 [dev-mypy]
 mypy==1.1.1
 types-setuptools<68,>=67.6.0
-frequenz-repo-config[docs-gen,pytest]
+frequenz-repo-config[dev-docs-gen,dev-pytest]
 
 [dev-pylint]
 pylint==2.17.1
 pylint-google-style-guide-imports-enforcing==1.3.0
-frequenz-repo-config[docs-gen,pytest]
+frequenz-repo-config[dev-docs-gen,dev-pytest]
 
 [dev-pytest]
 pytest==7.2.2
+cookiecutter==2.1.1
 
 [lib]
+
+[model]
```

