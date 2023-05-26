# Comparing `tmp/dav_tools-0.0.7.tar.gz` & `tmp/dav_tools-0.0.8.tar.gz`

## Comparing `dav_tools-0.0.7.tar` & `dav_tools-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 dav_tools-0.0.7/Makefile
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 dav_tools-0.0.7/requirements.txt
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 dav_tools-0.0.7/src/dav_tools/__init__.py
--rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 dav_tools-0.0.7/src/dav_tools/_arg_parser.py
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 dav_tools-0.0.7/src/dav_tools/_text_format.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 dav_tools-0.0.7/src/dav_tools/commands.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 dav_tools-0.0.7/src/dav_tools/devtools.py
--rw-r--r--   0        0        0     5195 2020-02-02 00:00:00.000000 dav_tools-0.0.7/src/dav_tools/messages.py
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 dav_tools-0.0.7/src/dav_tools/requirements.py
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 dav_tools-0.0.7/src/dav_tools/text_color.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 dav_tools-0.0.7/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 dav_tools-0.0.7/LICENSE
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 dav_tools-0.0.7/README.md
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 dav_tools-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 dav_tools-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 dav_tools-0.0.8/Makefile
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 dav_tools-0.0.8/src/dav_tools/__init__.py
+-rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 dav_tools-0.0.8/src/dav_tools/_arg_parser.py
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 dav_tools-0.0.8/src/dav_tools/_text_format.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 dav_tools-0.0.8/src/dav_tools/commands.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 dav_tools-0.0.8/src/dav_tools/devtools.py
+-rw-r--r--   0        0        0     5195 2020-02-02 00:00:00.000000 dav_tools-0.0.8/src/dav_tools/messages.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 dav_tools-0.0.8/src/dav_tools/requirements.py
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 dav_tools-0.0.8/src/dav_tools/text_color.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 dav_tools-0.0.8/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 dav_tools-0.0.8/LICENSE
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 dav_tools-0.0.8/README.md
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 dav_tools-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 dav_tools-0.0.8/PKG-INFO
```

### Comparing `dav_tools-0.0.7/Makefile` & `dav_tools-0.0.8/Makefile`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 NAME=dav-tools
 
+
+install: uninstall build
+	sudo python3 -m pip install ./dist/*.whl
+
 build:
+	python3 -m pip install pipreqs
+	pipreqs --force
 	sudo python3 -m pip install --upgrade -r requirements.txt
 	sudo rm -rf dist/
 	python3 -m pip install build
 	python3 -m build
 
+uninstall:
+	sudo python3 -m pip uninstall -y $(NAME)
+
+
+### PyPi ###
 upload: build
 	python3 -m pip install --upgrade twine
 	python3 -m twine upload --verbose dist/*
 
-install-local: uninstall build
-	sudo python3 -m pip install ./dist/*.whl
-
-uninstall:
-	sudo python3 -m pip uninstall -y $(NAME)
-	
 download: uninstall
 	sudo python3 -m pip install $(NAME)
 
+
+### TestPyPi ###
 download-test: uninstall
 	python3 -m pip install --index-url https://test.pypi.org/simple/ --no-deps $(NAME)
 
 upload-test: build
 	python3 -m pip install --upgrade twine
 	python3 -m twine upload --repository testpypi dist/*
```

### Comparing `dav_tools-0.0.7/src/dav_tools/_arg_parser.py` & `dav_tools-0.0.8/src/dav_tools/_arg_parser.py`

 * *Files identical despite different names*

### Comparing `dav_tools-0.0.7/src/dav_tools/_text_format.py` & `dav_tools-0.0.8/src/dav_tools/_text_format.py`

 * *Files identical despite different names*

### Comparing `dav_tools-0.0.7/src/dav_tools/commands.py` & `dav_tools-0.0.8/src/dav_tools/commands.py`

 * *Files identical despite different names*

### Comparing `dav_tools-0.0.7/src/dav_tools/messages.py` & `dav_tools-0.0.8/src/dav_tools/messages.py`

 * *Files identical despite different names*

### Comparing `dav_tools-0.0.7/src/dav_tools/text_color.py` & `dav_tools-0.0.8/src/dav_tools/text_color.py`

 * *Files identical despite different names*

### Comparing `dav_tools-0.0.7/LICENSE` & `dav_tools-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dav_tools-0.0.7/pyproject.toml` & `dav_tools-0.0.8/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "dav_tools"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Davide Ponzini", email="davide.ponzini95@gmail.com" },
 ]
 description = "Various utilies to aid in program development"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+  "elevate",
+  "argparse"
+]
 
 [project.urls]
 "Homepage" = "https://github.com/DavidePonzini/dav-utils"
 "Bug Tracker" = "https://github.com/DavidePonzini/dav-utils/issues"
```

