# Comparing `tmp/custom_py_docx-1.0.0.tar.gz` & `tmp/custom_py_docx-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custom_py_docx-1.0.0.tar", last modified: Fri May 26 17:16:43 2023, max compression
+gzip compressed data, was "custom_py_docx-1.0.1.tar", last modified: Fri May 26 17:24:58 2023, max compression
```

## Comparing `custom_py_docx-1.0.0.tar` & `custom_py_docx-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rwxr-xr-x   0        0        0      443 2023-05-10 19:25:28.305834 custom_py_docx-1.0.0/.github/workflows/publish.yml
--rwxr-xr-x   0        0        0        4 2023-05-10 19:06:35.692200 custom_py_docx-1.0.0/.gitignore
--rwxr-xr-x   0        0        0     1477 2023-05-26 17:10:37.436031 custom_py_docx-1.0.0/LICENSE
--rwxr-xr-x   0        0        0     7318 2023-05-10 18:50:32.182036 custom_py_docx-1.0.0/README.md
--rwxr-xr-x   0        0        0       90 2023-05-26 17:00:11.720571 custom_py_docx-1.0.0/custom_py_docx/__init__.py
--rwxr-xr-x   0        0        0     6055 2023-05-10 19:42:31.740864 custom_py_docx-1.0.0/custom_py_docx/document.py
--rwxr-xr-x   0        0        0      624 2023-05-26 17:09:03.749633 custom_py_docx-1.0.0/flit.ini
--rwxr-xr-x   0        0        0      408 2023-05-26 17:15:36.394324 custom_py_docx-1.0.0/pyproject.toml
--rwxr-xr-x   0        0        0      216 2023-05-10 19:12:17.567939 custom_py_docx-1.0.0/requirements.txt
--rwxr-xr-x   0        0        0       28 2023-05-26 17:13:05.942101 custom_py_docx-1.0.0/setup.cfg
--rwxr-xr-x   0        0        0      455 2023-05-10 20:07:26.314292 custom_py_docx-1.0.0/setup.py
--rw-r--r--   0        0        0      273 1970-01-01 00:00:00.000000 custom_py_docx-1.0.0/PKG-INFO
+-rwxr-xr-x   0        0        0      443 2023-05-10 19:25:28.305834 custom_py_docx-1.0.1/.github/workflows/publish.yml
+-rwxr-xr-x   0        0        0        4 2023-05-10 19:06:35.692200 custom_py_docx-1.0.1/.gitignore
+-rwxr-xr-x   0        0        0     1477 2023-05-26 17:10:37.436031 custom_py_docx-1.0.1/LICENSE
+-rwxr-xr-x   0        0        0     7318 2023-05-10 18:50:32.182036 custom_py_docx-1.0.1/README.md
+-rwxr-xr-x   0        0        0       90 2023-05-26 17:23:57.317446 custom_py_docx-1.0.1/custom_py_docx/__init__.py
+-rwxr-xr-x   0        0        0     6055 2023-05-10 19:42:31.740864 custom_py_docx-1.0.1/custom_py_docx/document.py
+-rwxr-xr-x   0        0        0      625 2023-05-26 17:24:14.154911 custom_py_docx-1.0.1/flit.ini
+-rwxr-xr-x   0        0        0      408 2023-05-26 17:15:36.394324 custom_py_docx-1.0.1/pyproject.toml
+-rwxr-xr-x   0        0        0      216 2023-05-10 19:12:17.567939 custom_py_docx-1.0.1/requirements.txt
+-rwxr-xr-x   0        0        0       28 2023-05-26 17:13:05.942101 custom_py_docx-1.0.1/setup.cfg
+-rwxr-xr-x   0        0        0      455 2023-05-10 20:07:26.314292 custom_py_docx-1.0.1/setup.py
+-rw-r--r--   0        0        0      273 1970-01-01 00:00:00.000000 custom_py_docx-1.0.1/PKG-INFO
```

### Comparing `custom_py_docx-1.0.0/LICENSE` & `custom_py_docx-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `custom_py_docx-1.0.0/README.md` & `custom_py_docx-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `custom_py_docx-1.0.0/custom_py_docx/document.py` & `custom_py_docx-1.0.1/custom_py_docx/document.py`

 * *Files identical despite different names*

### Comparing `custom_py_docx-1.0.0/flit.ini` & `custom_py_docx-1.0.1/flit.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 author=Renato Pinheiro
 author-email=renato.dev.pinheiro@gmail.com
 home-page=https://github.com/cristianovisk/custom-py-docx
 requires=["Babel==2.12.1","docxcompose==1.4.0","lxml==4.9.2","numpy==1.24.3","packaging==23.1","pandas==2.0.1","plotly==5.14.1","python-dateutil==2.8.2","python-docx==0.8.11","pytz==2023.3","six==1.16.0","tenacity==8.2.2","tzdata==2023.3"]
 requires-python= >=3
-description-file=README.md
+description-file=README.srt
 classifiers=Intended Audience :: Developers
     License :: OSI Approved :: BSD License
     Programming Language :: Python :: 3
     Topic :: Software Development :: Libraries :: Python Modules
```

