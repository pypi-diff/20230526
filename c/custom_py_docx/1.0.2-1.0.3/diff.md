# Comparing `tmp/custom_py_docx-1.0.2.tar.gz` & `tmp/custom_py_docx-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custom_py_docx-1.0.2.tar", last modified: Fri May 26 17:27:49 2023, max compression
+gzip compressed data, was "custom_py_docx-1.0.3.tar", last modified: Fri May 26 17:29:00 2023, max compression
```

## Comparing `custom_py_docx-1.0.2.tar` & `custom_py_docx-1.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rwxr-xr-x   0        0        0      443 2023-05-10 19:25:28.305834 custom_py_docx-1.0.2/.github/workflows/publish.yml
--rwxr-xr-x   0        0        0       10 2023-05-26 17:27:13.215692 custom_py_docx-1.0.2/.gitignore
--rwxr-xr-x   0        0        0     1477 2023-05-26 17:10:37.436031 custom_py_docx-1.0.2/LICENSE
--rwxr-xr-x   0        0        0     7318 2023-05-10 18:50:32.182036 custom_py_docx-1.0.2/README.srt
--rwxr-xr-x   0        0        0       90 2023-05-26 17:25:49.569926 custom_py_docx-1.0.2/custom_py_docx/__init__.py
--rwxr-xr-x   0        0        0     6055 2023-05-10 19:42:31.740864 custom_py_docx-1.0.2/custom_py_docx/document.py
--rwxr-xr-x   0        0        0      625 2023-05-26 17:24:14.154911 custom_py_docx-1.0.2/flit.ini
--rwxr-xr-x   0        0        0      408 2023-05-26 17:15:36.394324 custom_py_docx-1.0.2/pyproject.toml
--rwxr-xr-x   0        0        0      216 2023-05-10 19:12:17.567939 custom_py_docx-1.0.2/requirements.txt
--rwxr-xr-x   0        0        0       28 2023-05-26 17:13:05.942101 custom_py_docx-1.0.2/setup.cfg
--rwxr-xr-x   0        0        0      455 2023-05-10 20:07:26.314292 custom_py_docx-1.0.2/setup.py
--rw-r--r--   0        0        0      273 1970-01-01 00:00:00.000000 custom_py_docx-1.0.2/PKG-INFO
+-rwxr-xr-x   0        0        0      443 2023-05-10 19:25:28.305834 custom_py_docx-1.0.3/.github/workflows/publish.yml
+-rwxr-xr-x   0        0        0       10 2023-05-26 17:27:13.215692 custom_py_docx-1.0.3/.gitignore
+-rwxr-xr-x   0        0        0     1477 2023-05-26 17:10:37.436031 custom_py_docx-1.0.3/LICENSE
+-rwxr-xr-x   0        0        0     7318 2023-05-10 18:50:32.182036 custom_py_docx-1.0.3/README.srt
+-rwxr-xr-x   0        0        0       91 2023-05-26 17:28:48.471415 custom_py_docx-1.0.3/custom_py_docx/__init__.py
+-rwxr-xr-x   0        0        0     6055 2023-05-10 19:42:31.740864 custom_py_docx-1.0.3/custom_py_docx/document.py
+-rwxr-xr-x   0        0        0      625 2023-05-26 17:24:14.154911 custom_py_docx-1.0.3/flit.ini
+-rwxr-xr-x   0        0        0      408 2023-05-26 17:15:36.394324 custom_py_docx-1.0.3/pyproject.toml
+-rwxr-xr-x   0        0        0      216 2023-05-10 19:12:17.567939 custom_py_docx-1.0.3/requirements.txt
+-rwxr-xr-x   0        0        0       28 2023-05-26 17:13:05.942101 custom_py_docx-1.0.3/setup.cfg
+-rwxr-xr-x   0        0        0      455 2023-05-10 20:07:26.314292 custom_py_docx-1.0.3/setup.py
+-rw-r--r--   0        0        0      274 1970-01-01 00:00:00.000000 custom_py_docx-1.0.3/PKG-INFO
```

### Comparing `custom_py_docx-1.0.2/LICENSE` & `custom_py_docx-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `custom_py_docx-1.0.2/README.srt` & `custom_py_docx-1.0.3/README.srt`

 * *Files identical despite different names*

### Comparing `custom_py_docx-1.0.2/custom_py_docx/document.py` & `custom_py_docx-1.0.3/custom_py_docx/document.py`

 * *Files identical despite different names*

### Comparing `custom_py_docx-1.0.2/flit.ini` & `custom_py_docx-1.0.3/flit.ini`

 * *Files identical despite different names*

