# Comparing `tmp/code-snapshot-0.2.3.tar.gz` & `tmp/code-snapshot-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "code-snapshot-0.2.3.tar", last modified: Mon May 22 10:07:45 2023, max compression
+gzip compressed data, was "code-snapshot-0.2.4.tar", last modified: Fri May 26 06:10:35 2023, max compression
```

## Comparing `code-snapshot-0.2.3.tar` & `code-snapshot-0.2.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:45.061855 code-snapshot-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-22 10:07:30.000000 code-snapshot-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-22 10:07:30.000000 code-snapshot-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-22 10:07:45.061855 code-snapshot-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-22 10:07:30.000000 code-snapshot-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   165206 2023-05-22 10:07:30.000000 code-snapshot-0.2.3/Showcode_API_token.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:45.061855 code-snapshot-0.2.3/code_snapshot/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-22 10:07:30.000000 code-snapshot-0.2.3/code_snapshot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-22 10:07:30.000000 code-snapshot-0.2.3/code_snapshot/code_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-22 10:07:30.000000 code-snapshot-0.2.3/code_snapshot/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:45.061855 code-snapshot-0.2.3/code_snapshot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-22 10:07:45.000000 code-snapshot-0.2.3/code_snapshot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-22 10:07:45.000000 code-snapshot-0.2.3/code_snapshot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 10:07:45.000000 code-snapshot-0.2.3/code_snapshot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-22 10:07:45.000000 code-snapshot-0.2.3/code_snapshot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-22 10:07:45.000000 code-snapshot-0.2.3/code_snapshot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    26215 2023-05-22 10:07:30.000000 code-snapshot-0.2.3/code_snapshot.png
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 10:07:45.061855 code-snapshot-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-22 10:07:30.000000 code-snapshot-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:10:35.579592 code-snapshot-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-26 06:10:20.000000 code-snapshot-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-26 06:10:20.000000 code-snapshot-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-26 06:10:35.579592 code-snapshot-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-26 06:10:20.000000 code-snapshot-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   165206 2023-05-26 06:10:20.000000 code-snapshot-0.2.4/Showcode_API_token.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:10:35.579592 code-snapshot-0.2.4/code_snapshot/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-26 06:10:20.000000 code-snapshot-0.2.4/code_snapshot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-26 06:10:20.000000 code-snapshot-0.2.4/code_snapshot/code_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-26 06:10:20.000000 code-snapshot-0.2.4/code_snapshot/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:10:35.579592 code-snapshot-0.2.4/code_snapshot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-26 06:10:35.000000 code-snapshot-0.2.4/code_snapshot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-26 06:10:35.000000 code-snapshot-0.2.4/code_snapshot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 06:10:35.000000 code-snapshot-0.2.4/code_snapshot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-26 06:10:35.000000 code-snapshot-0.2.4/code_snapshot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-26 06:10:35.000000 code-snapshot-0.2.4/code_snapshot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    26215 2023-05-26 06:10:20.000000 code-snapshot-0.2.4/code_snapshot.png
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 06:10:35.579592 code-snapshot-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-26 06:10:20.000000 code-snapshot-0.2.4/setup.py
```

### Comparing `code-snapshot-0.2.3/LICENSE` & `code-snapshot-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `code-snapshot-0.2.3/PKG-INFO` & `code-snapshot-0.2.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: code-snapshot
-Version: 0.2.3
+Version: 0.2.4
 Summary: code_snapshot - A Python library for interacting with the Showcode api.
 Home-page: https://github.com/ainomic/code-snapshot
 Author: Ainomic Technology
 Author-email: contact@ainomic.in
 License: GNU General Public License (GPL)
 Keywords: snapshot,screenshot,code-snapshot,code-screenshot
 Platform: ALL
@@ -23,23 +23,23 @@
 
 1. Create an account on [Showcode App](https://api.showcode.app/register) to fetch the API key.
 1. Sign in to the account and create an API token:
    1. Token name: _Provide a name to the token which you can remember where it is being used_
    1. Check "read" permissions
    1. Copy the token displayed and store somewhere in safe. __Note: This token won't be shown again, so you need to paste it before you close the window__
 
-   ![Create API token snapshot](https://github.com/ainomic/code-snapshot/blob/0.1.3/Showcode_API_token.png)
+   ![Create API token snapshot](Showcode_API_token.png)
 1. Export an environment variable to store the token in the terminal: `export SHOWCODE_API_KEY={API Token}`
 1. Now, you're ready to use the package in your applications.
 
 ## Installation
 
 1. Create a virtual environment: `conda create -n code-snapshot-test-env -y python=3.8`
 1. Activate the environment: `conda activate code-snapshot-test-env`
-1. Install the package `pip install -i https://test.pypi.org/simple/ code-snapshot`
+1. Install the package `pip install code-snapshot`
 
 ## Usage
 
 1. Set the Showcode API token as an environment variable following [Getting started](#getting-started) section
 1. Write a python script as following:
 
    ```python
@@ -61,9 +61,9 @@
       cs = CodeSnapshot()
       cs.save_snapshot(settings, editor, filepath="./code_snapshot.png")
 
    ```
 
 1. Run the python script `python main.py`. This should generate a file `code_snapshot.png` in the same directory as `main.py`.
 1. It should look like this:
-   ![code_snapshot](https://github.com/ainomic/code-snapshot/blob/0.1.5/code_snapshot.png)
+   ![code_snapshot](code_snapshot.png)
 1. You can use `cs.generate_snapshot(settings, editor)` to consume `bytes` if required.
```

### Comparing `code-snapshot-0.2.3/README.md` & `code-snapshot-0.2.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 
 1. Create an account on [Showcode App](https://api.showcode.app/register) to fetch the API key.
 1. Sign in to the account and create an API token:
    1. Token name: _Provide a name to the token which you can remember where it is being used_
    1. Check "read" permissions
    1. Copy the token displayed and store somewhere in safe. __Note: This token won't be shown again, so you need to paste it before you close the window__
 
-   ![Create API token snapshot](https://github.com/ainomic/code-snapshot/blob/0.1.3/Showcode_API_token.png)
+   ![Create API token snapshot](Showcode_API_token.png)
 1. Export an environment variable to store the token in the terminal: `export SHOWCODE_API_KEY={API Token}`
 1. Now, you're ready to use the package in your applications.
 
 ## Installation
 
 1. Create a virtual environment: `conda create -n code-snapshot-test-env -y python=3.8`
 1. Activate the environment: `conda activate code-snapshot-test-env`
-1. Install the package `pip install -i https://test.pypi.org/simple/ code-snapshot`
+1. Install the package `pip install code-snapshot`
 
 ## Usage
 
 1. Set the Showcode API token as an environment variable following [Getting started](#getting-started) section
 1. Write a python script as following:
 
    ```python
@@ -44,9 +44,9 @@
       cs = CodeSnapshot()
       cs.save_snapshot(settings, editor, filepath="./code_snapshot.png")
 
    ```
 
 1. Run the python script `python main.py`. This should generate a file `code_snapshot.png` in the same directory as `main.py`.
 1. It should look like this:
-   ![code_snapshot](https://github.com/ainomic/code-snapshot/blob/0.1.5/code_snapshot.png)
+   ![code_snapshot](code_snapshot.png)
 1. You can use `cs.generate_snapshot(settings, editor)` to consume `bytes` if required.
```

### Comparing `code-snapshot-0.2.3/Showcode_API_token.png` & `code-snapshot-0.2.4/Showcode_API_token.png`

 * *Files identical despite different names*

### Comparing `code-snapshot-0.2.3/code_snapshot/code_snapshot.py` & `code-snapshot-0.2.4/code_snapshot/code_snapshot.py`

 * *Files identical despite different names*

### Comparing `code-snapshot-0.2.3/code_snapshot.egg-info/PKG-INFO` & `code-snapshot-0.2.4/code_snapshot.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: code-snapshot
-Version: 0.2.3
+Version: 0.2.4
 Summary: code_snapshot - A Python library for interacting with the Showcode api.
 Home-page: https://github.com/ainomic/code-snapshot
 Author: Ainomic Technology
 Author-email: contact@ainomic.in
 License: GNU General Public License (GPL)
 Keywords: snapshot,screenshot,code-snapshot,code-screenshot
 Platform: ALL
@@ -23,23 +23,23 @@
 
 1. Create an account on [Showcode App](https://api.showcode.app/register) to fetch the API key.
 1. Sign in to the account and create an API token:
    1. Token name: _Provide a name to the token which you can remember where it is being used_
    1. Check "read" permissions
    1. Copy the token displayed and store somewhere in safe. __Note: This token won't be shown again, so you need to paste it before you close the window__
 
-   ![Create API token snapshot](https://github.com/ainomic/code-snapshot/blob/0.1.3/Showcode_API_token.png)
+   ![Create API token snapshot](Showcode_API_token.png)
 1. Export an environment variable to store the token in the terminal: `export SHOWCODE_API_KEY={API Token}`
 1. Now, you're ready to use the package in your applications.
 
 ## Installation
 
 1. Create a virtual environment: `conda create -n code-snapshot-test-env -y python=3.8`
 1. Activate the environment: `conda activate code-snapshot-test-env`
-1. Install the package `pip install -i https://test.pypi.org/simple/ code-snapshot`
+1. Install the package `pip install code-snapshot`
 
 ## Usage
 
 1. Set the Showcode API token as an environment variable following [Getting started](#getting-started) section
 1. Write a python script as following:
 
    ```python
@@ -61,9 +61,9 @@
       cs = CodeSnapshot()
       cs.save_snapshot(settings, editor, filepath="./code_snapshot.png")
 
    ```
 
 1. Run the python script `python main.py`. This should generate a file `code_snapshot.png` in the same directory as `main.py`.
 1. It should look like this:
-   ![code_snapshot](https://github.com/ainomic/code-snapshot/blob/0.1.5/code_snapshot.png)
+   ![code_snapshot](code_snapshot.png)
 1. You can use `cs.generate_snapshot(settings, editor)` to consume `bytes` if required.
```

### Comparing `code-snapshot-0.2.3/code_snapshot.png` & `code-snapshot-0.2.4/code_snapshot.png`

 * *Files identical despite different names*

### Comparing `code-snapshot-0.2.3/setup.py` & `code-snapshot-0.2.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         ][0],
         keywords=["snapshot", "screenshot",
                   "code-snapshot", "code-screenshot"],
         packages=find_packages(),
         include_package_data=True,
         platforms="ALL",
         install_requires=[
-            "requests >= 2.20.0, < 2.21",
+            "requests >= 2.31.0, < 2.32",
             "certifi",
         ],
         extras_require={},
     )
 
 
 if __name__ == '__main__':
```

