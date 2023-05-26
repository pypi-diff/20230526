# Comparing `tmp/ttkDesigner-0.30.0a80.tar.gz` & `tmp/ttkDesigner-0.30.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ttkDesigner-0.30.0a80.tar", last modified: Fri May 26 18:38:50 2023, max compression
+gzip compressed data, was "ttkDesigner-0.30.0a9.tar", last modified: Mon Apr 17 18:29:34 2023, max compression
```

## Comparing `ttkDesigner-0.30.0a80.tar` & `ttkDesigner-0.30.0a9.tar`

### file list

```diff
@@ -1,44 +1,41 @@
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2023-05-26 18:38:50.179536 ttkDesigner-0.30.0a80/
--rw-rw-r--   0 one       (1000) one       (1000)     1118 2023-05-26 18:38:46.000000 ttkDesigner-0.30.0a80/LICENSE
--rw-rw-r--   0 one       (1000) one       (1000)     2880 2023-05-26 18:38:50.179536 ttkDesigner-0.30.0a80/PKG-INFO
--rw-rw-r--   0 one       (1000) one       (1000)     2094 2023-05-26 18:38:46.000000 ttkDesigner-0.30.0a80/README.md
--rw-rw-r--   0 one       (1000) one       (1000)       38 2023-05-26 18:38:50.179536 ttkDesigner-0.30.0a80/setup.cfg
--rw-rw-r--   0 one       (1000) one       (1000)     1410 2023-05-26 18:38:46.000000 ttkDesigner-0.30.0a80/setup.py
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2023-05-26 18:38:50.175536 ttkDesigner-0.30.0a80/ttkDesigner/
--rwxrwxr-x   0 one       (1000) one       (1000)     1215 2023-04-18 15:38:03.000000 ttkDesigner-0.30.0a80/ttkDesigner/__init__.py
--rw-rw-r--   0 one       (1000) one       (1000)     1218 2023-04-18 15:38:03.000000 ttkDesigner-0.30.0a80/ttkDesigner/__main__.py
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2023-05-26 18:38:50.175536 ttkDesigner-0.30.0a80/ttkDesigner/app/
--rw-rw-r--   0 one       (1000) one       (1000)     1569 2023-04-26 13:07:10.000000 ttkDesigner-0.30.0a80/ttkDesigner/app/__init__.py
--rw-rw-r--   0 one       (1000) one       (1000)     3305 2023-05-09 12:25:12.000000 ttkDesigner-0.30.0a80/ttkDesigner/app/about.py
--rw-rw-r--   0 one       (1000) one       (1000)     1352 2023-05-26 18:38:46.000000 ttkDesigner-0.30.0a80/ttkDesigner/app/cfg.py
--rw-rw-r--   0 one       (1000) one       (1000)    14784 2023-05-02 15:49:12.000000 ttkDesigner-0.30.0a80/ttkDesigner/app/designer.py
--rw-rw-r--   0 one       (1000) one       (1000)     1964 2023-05-05 13:40:13.000000 ttkDesigner-0.30.0a80/ttkDesigner/app/main.py
--rw-rw-r--   0 one       (1000) one       (1000)     8701 2023-05-20 09:49:51.000000 ttkDesigner-0.30.0a80/ttkDesigner/app/notepad.py
--rw-rw-r--   0 one       (1000) one       (1000)    12474 2023-04-18 15:38:03.000000 ttkDesigner-0.30.0a80/ttkDesigner/app/propertyeditor.py
--rw-rw-r--   0 one       (1000) one       (1000)     3715 2023-04-26 22:52:25.000000 ttkDesigner-0.30.0a80/ttkDesigner/app/quickexport.py
--rw-rw-r--   0 one       (1000) one       (1000)     9448 2023-04-18 15:38:03.000000 ttkDesigner-0.30.0a80/ttkDesigner/app/signalsloteditor.py
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2023-05-26 18:38:50.179536 ttkDesigner-0.30.0a80/ttkDesigner/app/superobj/
--rw-rw-r--   0 one       (1000) one       (1000)     1597 2023-05-05 18:53:40.000000 ttkDesigner-0.30.0a80/ttkDesigner/app/superobj/__init__.py
--rw-rw-r--   0 one       (1000) one       (1000)     4339 2023-05-09 12:25:12.000000 ttkDesigner-0.30.0a80/ttkDesigner/app/superobj/supercontrol.py
--rw-rw-r--   0 one       (1000) one       (1000)     8691 2023-05-09 12:35:26.000000 ttkDesigner-0.30.0a80/ttkDesigner/app/superobj/superlayout.py
--rw-rw-r--   0 one       (1000) one       (1000)    16421 2023-05-09 12:25:12.000000 ttkDesigner-0.30.0a80/ttkDesigner/app/superobj/superlayoutgrid.py
--rw-rw-r--   0 one       (1000) one       (1000)     1481 2023-04-18 15:38:03.000000 ttkDesigner-0.30.0a80/ttkDesigner/app/superobj/superlayouthbox.py
--rw-rw-r--   0 one       (1000) one       (1000)     1479 2023-04-18 15:38:03.000000 ttkDesigner-0.30.0a80/ttkDesigner/app/superobj/superlayoutvbox.py
--rw-rw-r--   0 one       (1000) one       (1000)     4004 2023-04-18 15:38:03.000000 ttkDesigner-0.30.0a80/ttkDesigner/app/superobj/superobj.py
--rw-rw-r--   0 one       (1000) one       (1000)    11061 2023-05-21 13:09:53.000000 ttkDesigner-0.30.0a80/ttkDesigner/app/superobj/superwidget.py
--rw-rw-r--   0 one       (1000) one       (1000)     1385 2023-05-05 18:57:59.000000 ttkDesigner-0.30.0a80/ttkDesigner/app/superobj/superwidgetframe.py
--rw-rw-r--   0 one       (1000) one       (1000)     1679 2023-04-18 15:38:03.000000 ttkDesigner-0.30.0a80/ttkDesigner/app/superobj/superwidgetradiobutton.py
--rw-rw-r--   0 one       (1000) one       (1000)     1793 2023-04-18 15:38:03.000000 ttkDesigner-0.30.0a80/ttkDesigner/app/superobj/superwidgettextedit.py
--rw-rw-r--   0 one       (1000) one       (1000)     6627 2023-05-02 15:49:30.000000 ttkDesigner-0.30.0a80/ttkDesigner/app/treeinspector.py
--rw-rw-r--   0 one       (1000) one       (1000)     7049 2023-05-09 12:25:12.000000 ttkDesigner-0.30.0a80/ttkDesigner/app/widgetbox.py
--rw-rw-r--   0 one       (1000) one       (1000)     4932 2023-05-09 12:25:12.000000 ttkDesigner-0.30.0a80/ttkDesigner/app/windoweditor.py
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2023-05-26 18:38:50.179536 ttkDesigner-0.30.0a80/ttkDesigner/tui/
--rw-rw-r--   0 one       (1000) one       (1000)     8721 2023-04-18 15:38:03.000000 ttkDesigner-0.30.0a80/ttkDesigner/tui/newWindow.tui.json
--rw-rw-r--   0 one       (1000) one       (1000)     3880 2023-04-26 22:26:45.000000 ttkDesigner-0.30.0a80/ttkDesigner/tui/quickExport.tui.json
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2023-05-26 18:38:50.175536 ttkDesigner-0.30.0a80/ttkDesigner.egg-info/
--rw-rw-r--   0 one       (1000) one       (1000)     2880 2023-05-26 18:38:50.000000 ttkDesigner-0.30.0a80/ttkDesigner.egg-info/PKG-INFO
--rw-rw-r--   0 one       (1000) one       (1000)     1179 2023-05-26 18:38:50.000000 ttkDesigner-0.30.0a80/ttkDesigner.egg-info/SOURCES.txt
--rw-rw-r--   0 one       (1000) one       (1000)        1 2023-05-26 18:38:50.000000 ttkDesigner-0.30.0a80/ttkDesigner.egg-info/dependency_links.txt
--rw-rw-r--   0 one       (1000) one       (1000)       49 2023-05-26 18:38:50.000000 ttkDesigner-0.30.0a80/ttkDesigner.egg-info/entry_points.txt
--rw-rw-r--   0 one       (1000) one       (1000)       37 2023-05-26 18:38:50.000000 ttkDesigner-0.30.0a80/ttkDesigner.egg-info/requires.txt
--rw-rw-r--   0 one       (1000) one       (1000)       12 2023-05-26 18:38:50.000000 ttkDesigner-0.30.0a80/ttkDesigner.egg-info/top_level.txt
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2023-04-17 18:29:34.652006 ttkDesigner-0.30.0a9/
+-rw-rw-r--   0 one       (1000) one       (1000)     1118 2023-04-17 18:29:31.000000 ttkDesigner-0.30.0a9/LICENSE
+-rw-rw-r--   0 one       (1000) one       (1000)     1832 2023-04-17 18:29:34.652006 ttkDesigner-0.30.0a9/PKG-INFO
+-rw-rw-r--   0 one       (1000) one       (1000)     1047 2023-04-17 18:29:31.000000 ttkDesigner-0.30.0a9/README.md
+-rw-rw-r--   0 one       (1000) one       (1000)       38 2023-04-17 18:29:34.652006 ttkDesigner-0.30.0a9/setup.cfg
+-rw-rw-r--   0 one       (1000) one       (1000)     1408 2023-04-17 18:29:31.000000 ttkDesigner-0.30.0a9/setup.py
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2023-04-17 18:29:34.652006 ttkDesigner-0.30.0a9/ttkDesigner/
+-rwxrwxr-x   0 one       (1000) one       (1000)     1215 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a9/ttkDesigner/__init__.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1218 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a9/ttkDesigner/__main__.py
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2023-04-17 18:29:34.652006 ttkDesigner-0.30.0a9/ttkDesigner/app/
+-rw-rw-r--   0 one       (1000) one       (1000)     1540 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a9/ttkDesigner/app/__init__.py
+-rw-rw-r--   0 one       (1000) one       (1000)     3313 2023-04-17 16:52:51.000000 ttkDesigner-0.30.0a9/ttkDesigner/app/about.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1351 2023-04-17 18:29:31.000000 ttkDesigner-0.30.0a9/ttkDesigner/app/cfg.py
+-rw-rw-r--   0 one       (1000) one       (1000)    14349 2023-04-17 13:42:54.000000 ttkDesigner-0.30.0a9/ttkDesigner/app/designer.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1538 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a9/ttkDesigner/app/main.py
+-rw-rw-r--   0 one       (1000) one       (1000)    12474 2023-04-15 00:27:24.000000 ttkDesigner-0.30.0a9/ttkDesigner/app/propertyeditor.py
+-rw-rw-r--   0 one       (1000) one       (1000)     2985 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a9/ttkDesigner/app/quickexport.py
+-rw-rw-r--   0 one       (1000) one       (1000)     9448 2023-04-15 00:31:37.000000 ttkDesigner-0.30.0a9/ttkDesigner/app/signalsloteditor.py
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2023-04-17 18:29:34.652006 ttkDesigner-0.30.0a9/ttkDesigner/app/superobj/
+-rw-rw-r--   0 one       (1000) one       (1000)     1544 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a9/ttkDesigner/app/superobj/__init__.py
+-rw-rw-r--   0 one       (1000) one       (1000)     4308 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a9/ttkDesigner/app/superobj/supercontrol.py
+-rw-rw-r--   0 one       (1000) one       (1000)     8555 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a9/ttkDesigner/app/superobj/superlayout.py
+-rw-rw-r--   0 one       (1000) one       (1000)    12712 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a9/ttkDesigner/app/superobj/superlayoutgrid.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1481 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a9/ttkDesigner/app/superobj/superlayouthbox.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1479 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a9/ttkDesigner/app/superobj/superlayoutvbox.py
+-rw-rw-r--   0 one       (1000) one       (1000)     4004 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a9/ttkDesigner/app/superobj/superobj.py
+-rw-rw-r--   0 one       (1000) one       (1000)    10603 2023-04-16 15:59:33.000000 ttkDesigner-0.30.0a9/ttkDesigner/app/superobj/superwidget.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1679 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a9/ttkDesigner/app/superobj/superwidgetradiobutton.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1793 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a9/ttkDesigner/app/superobj/superwidgettextedit.py
+-rw-rw-r--   0 one       (1000) one       (1000)     6623 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a9/ttkDesigner/app/treeinspector.py
+-rw-rw-r--   0 one       (1000) one       (1000)     7053 2023-04-17 14:07:48.000000 ttkDesigner-0.30.0a9/ttkDesigner/app/widgetbox.py
+-rw-rw-r--   0 one       (1000) one       (1000)     5205 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a9/ttkDesigner/app/windoweditor.py
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2023-04-17 18:29:34.652006 ttkDesigner-0.30.0a9/ttkDesigner/tui/
+-rw-rw-r--   0 one       (1000) one       (1000)     8721 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a9/ttkDesigner/tui/newWindow.tui.json
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2023-04-17 18:29:34.652006 ttkDesigner-0.30.0a9/ttkDesigner.egg-info/
+-rw-rw-r--   0 one       (1000) one       (1000)     1832 2023-04-17 18:29:34.000000 ttkDesigner-0.30.0a9/ttkDesigner.egg-info/PKG-INFO
+-rw-rw-r--   0 one       (1000) one       (1000)     1070 2023-04-17 18:29:34.000000 ttkDesigner-0.30.0a9/ttkDesigner.egg-info/SOURCES.txt
+-rw-rw-r--   0 one       (1000) one       (1000)        1 2023-04-17 18:29:34.000000 ttkDesigner-0.30.0a9/ttkDesigner.egg-info/dependency_links.txt
+-rw-rw-r--   0 one       (1000) one       (1000)       49 2023-04-17 18:29:34.000000 ttkDesigner-0.30.0a9/ttkDesigner.egg-info/entry_points.txt
+-rw-rw-r--   0 one       (1000) one       (1000)       36 2023-04-17 18:29:34.000000 ttkDesigner-0.30.0a9/ttkDesigner.egg-info/requires.txt
+-rw-rw-r--   0 one       (1000) one       (1000)       12 2023-04-17 18:29:34.000000 ttkDesigner-0.30.0a9/ttkDesigner.egg-info/top_level.txt
```

### Comparing `ttkDesigner-0.30.0a80/LICENSE` & `ttkDesigner-0.30.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.30.0a80/README.md` & `ttkDesigner-0.30.0a9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,32 @@
+Metadata-Version: 2.1
+Name: ttkDesigner
+Version: 0.30.0a9
+Summary: ttkDesigner is a terminal user interface designer for pyTermTk applications
+Home-page: https://github.com/ceccopierangiolieugenio/pyTermTk
+Author: Eugenio Parodi
+Author-email: ceccopierangiolieugenio@googlemail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: Topic :: Terminals
+Classifier: Topic :: Software Development :: User Interfaces
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ![Linux](https://img.shields.io/badge/-Linux-grey?logo=linux)
 ![Usage](https://img.shields.io/badge/Usage-Terminal%20User%20Interface-yellow)
 ![Python](https://img.shields.io/badge/Python-v3.8%5E-green?logo=python)
 ![pyTermTk_version](https://img.shields.io/github/v/tag/ceccopierangiolieugenio/pyTermTk?label=version)
 [![Test Status](https://img.shields.io/github/actions/workflow/status/ceccopierangiolieugenio/pyTermTk/testing.yml?branch=main&label=tests)](https://github.com/ceccopierangiolieugenio/pyTermTk/actions?query=workflow%3Atesting)
-[![pypi_version](https://img.shields.io/pypi/v/ttkDesigner?label=pypi)](https://pypi.org/project/ttkDesigner)
+[![pypi_version](https://img.shields.io/pypi/v/pyTermTk?label=pypi)](https://pypi.org/project/pyTermTk)
 [![pypi_version](https://img.shields.io/twitter/follow/Pier95886803?style=social&logo=twitter)](https://twitter.com/hashtag/pyTermTk?src=hashtag_click&f=live)
 
-[![screenshot](https://user-images.githubusercontent.com/8876552/236525667-dcdcec6e-1066-4294-bdb0-db98ef8850da.png)](https://pypi.org/project/ttkDesigner)
-
-## [ttkDesigner](https://github.com/ceccopierangiolieugenio/pyTermTk/tree/main/ttkDesigner)
-
-**ttkDesigner** is the [pyTermTk](https://github.com/ceccopierangiolieugenio/pyTermTk) tool for designing and building Text-based user interfaces ([TUI](https://en.wikipedia.org/wiki/Text-based_user_interface)s) with [pyTermTk](https://github.com/ceccopierangiolieugenio/pyTermTk) Widgets. You can compose and customize your windows or dialogs in a what-you-see-is-what-you-get (WYSIWYG) manner, and test them interactively.
-
-Widgets and forms created with **ttkDesigner** integrate seamlessly with programmed code, using [pyTermTk](https://github.com/ceccopierangiolieugenio/pyTermTk)'s signals and slots mechanism, so that you can easily assign behavior to graphical elements. All properties set in **ttkDesigner** can be changed dynamically within the code.
+[![screenshot](https://user-images.githubusercontent.com/8876552/232550100-89e80528-85b1-40d8-b752-6dc5feedf3ae.png)](https://pypi.org/project/pyTermTk)
 
-## Features
-tbd
+## [ttkDesigner](https://github.com/ceccopierangiolieugenio/pyTermTk/ttkDesigner)
 
-## Install/Upgrade
-[ttkDesigner](https://github.com/ceccopierangiolieugenio/pyTermTk/tree/main/ttkDesigner)
- is available on [PyPI](https://pypi.org/project/ttkDesigner/)
-```bash
-pip3 install --upgrade ttkDesigner
-```
-## Run
-```bash
-ttkDesigner
-```
```

### Comparing `ttkDesigner-0.30.0a80/setup.py` & `ttkDesigner-0.30.0a9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-version = "0.30.0-a80"
+version = "0.30.0-a9"
 name = "ttkDesigner"
 
 print(f"Version: {version}")
 print(f"Name: {name}")
 
 setup(
     name=name,
@@ -29,15 +29,15 @@
         "Topic :: Terminals",
         "Topic :: Software Development :: User Interfaces"],
     include_package_data=False,
     packages=['ttkDesigner','ttkDesigner.app', 'ttkDesigner.app.superobj'],
     package_data={'ttkDesigner': ['tui/*']},
     python_requires=">=3.8",
     install_requires=[
-        'pyTermTk>=0.30.0a69',
+        'pyTermTk>=0.30.0a5',
         'pyperclip',
         'Pillow'],
     entry_points={
         'console_scripts': [
             'ttkDesigner = ttkDesigner:main',
         ],
     },
```

### Comparing `ttkDesigner-0.30.0a80/ttkDesigner/__init__.py` & `ttkDesigner-0.30.0a9/ttkDesigner/__init__.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.30.0a80/ttkDesigner/__main__.py` & `ttkDesigner-0.30.0a9/ttkDesigner/__main__.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.30.0a80/ttkDesigner/app/__init__.py` & `ttkDesigner-0.30.0a9/ttkDesigner/app/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,9 +27,8 @@
 from .designer import TTkDesigner
 from .treeinspector import TreeInspector
 from .widgetbox import DragDesignItem, WidgetBox
 from .windoweditor import WindowEditor
 from .propertyeditor import PropertyEditor
 from .signalsloteditor import SignalSlotEditor
 from .quickexport import QuickExport
-from .notepad import NotePad
 from .superobj import *
```

### Comparing `ttkDesigner-0.30.0a80/ttkDesigner/app/about.py` & `ttkDesigner-0.30.0a9/ttkDesigner/app/about.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,18 +41,18 @@
         TTkString("╰─────────────────",TTkColor.fg("#9900FF"))+         TTkString(                  "|___|",            TTkColor.fg("#DFFF9F"))+TTkString("──────────┄ ",TTkColor.fg("#BB00FF"))]
 
     __slots__=('_image')
     def __init__(self, *args, **kwargs):
         TTkAbout.__init__(self, *args, **kwargs)
 
         self.setTitle('[PierCecco Cecco] Eugenio Parodi proudly presents...')
-        self.resize(56,15)
+        self.resize(56,16)
 
-    def paintEvent(self, canvas):
+    def paintEvent(self):
         c = [0xFF,0xFF,0xFF]
         for y, line in enumerate(About.designerTxt):
-            canvas.drawText(pos=(13,3+y),text=line)
-        canvas.drawText(pos=(20, 9),text=f"  Version: {TTkDesignerCfg.version}", color=TTkColor.fg('#AAAAFF'))
-        canvas.drawText(pos=(14,11),text=f"Powered By, pyTermTk")
-        canvas.drawText(pos=( 2,13),text=f"https://github.com/ceccopierangiolieugenio/pyTermTk", color=TTkColor.fg('#44FFFF'))
+            self._canvas.drawText(pos=(13,3+y),text=line)
+        self._canvas.drawText(pos=(26, 9),text=f"  Version: {TTkDesignerCfg.version}", color=TTkColor.fg('#AAAAFF'))
+        self._canvas.drawText(pos=(14,11),text=f"Powered By, pyTermTk")
+        self._canvas.drawText(pos=( 2,14),text=f"https://github.com/ceccopierangiolieugenio/pyTermTk", color=TTkColor.fg('#44FFFF'))
 
-        TTkWindow.paintEvent(self, canvas)
+        TTkWindow.paintEvent(self)
```

### Comparing `ttkDesigner-0.30.0a80/ttkDesigner/app/cfg.py` & `ttkDesigner-0.30.0a9/ttkDesigner/app/cfg.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,14 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import os
 # import yaml
 
 class TTkDesignerCfg:
-    version="0.30.0-a80"
+    version="0.30.0-a9"
     name="ttkDesigner"
     cfgVersion = '1.0'
     pathCfg="."
     options={}
     maxsearches=200
```

### Comparing `ttkDesigner-0.30.0a80/ttkDesigner/app/designer.py` & `ttkDesigner-0.30.0a9/ttkDesigner/app/designer.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,14 @@
 from .about import *
 from .widgetbox import DragDesignItem, WidgetBox, WidgetBoxScrollArea
 from .windoweditor import WindowEditor, SuperWidget
 from .treeinspector import TreeInspector
 from .propertyeditor import PropertyEditor
 from .signalsloteditor import SignalSlotEditor
 from .quickexport import QuickExport
-from .notepad import NotePad
 
 #
 #      Mimic the QT Designer layout
 #
 #      ┌─────────────────────╥───────────────────────────────╥───────────────────┐
 #      │                     ║┌─────────────────────────────┐║                   │
 #      │                     ║│       ToolBar               │║  Tree Inspector   │
@@ -73,19 +72,19 @@
 #      │                     ╟───────────────────────────────╢                   │
 #      │                     ║     LOG Viewer                ║   Editor          │
 #      │                     ║                               ║                   │
 #      └─────────────────────╨───────────────────────────────╨───────────────────┘
 #
 
 class TTkDesigner(TTkGridLayout):
-    __slots__ = ('_pippo', '_main', '_windowEditor', '_toolBar', '_fileNameLabel', '_sigslotEditor', '_treeInspector', '_fileName', '_currentPath', '_notepad',
+    __slots__ = ('_pippo', '_main', '_windowEditor', '_toolBar', '_fileNameLabel', '_sigslotEditor', '_treeInspector', '_fileName', '_currentPath',
                  # Signals
                  'weModified', 'thingSelected', 'widgetNameChanged'
                  )
-    def __init__(self, fileName=None, *args, **kwargs):
+    def __init__(self, *args, **kwargs):
         self._fileName = "untitled.tui.json"
         self._currentPath = self._currentPath =  os.path.abspath('.')
 
         self.weModified = pyTTkSignal()
         self.thingSelected = pyTTkSignal(TTkWidget, TTkWidget)
         self.widgetNameChanged = pyTTkSignal(str, str)
 
@@ -95,15 +94,14 @@
         mainSplit.addItem(widgetBoxLayout := TTkVBoxLayout())
         #mainSplit.addWidget(TTkButton(text='A',border=True))
 
         # mainSplit.addWidget(sa := TTkScrollArea())
         # sa.viewport().setLayout(TTkGridLayout())
         # sa.viewport().layout().addWidget(WindowEditor())
 
-        self._notepad = NotePad()
         self._main = TTkVBoxLayout()
         self._toolBar = TTkHBoxLayout()
         self._windowEditor = WindowEditor(self)
         self._sigslotEditor = SignalSlotEditor(self)
         self._treeInspector = TreeInspector(self, self._windowEditor.viewport())
         self._fileNameLabel = TTkLabel(text=f"( {self._fileName} )", alignment=TTkK.CENTER_ALIGN)
 
@@ -134,18 +132,16 @@
         fileMenu = topMenuFrame.menubarTop().addMenu("&File")
         fileMenu.addMenu("New").menuButtonClicked.connect(self.new)
         fileMenu.addMenu("Open").menuButtonClicked.connect(self.open)
         fileMenu.addMenu("Save").menuButtonClicked.connect(self.save)
         fileMenu.addMenu("Save As...").menuButtonClicked.connect(self.saveAs)
         fileMenu.addMenu("Exit").menuButtonClicked.connect(TTkHelper.quit)
 
-        extraMenu = topMenuFrame.menubarTop().addMenu("E&xtra")
-        extraMenu.addMenu("Scratchpad").menuButtonClicked.connect(self.scratchpad)
-        extraMenu.addSpacer()
-        extraMenu.addMenu("Preview...").menuButtonClicked.connect(self.preview)
+        fileMenu = topMenuFrame.menubarTop().addMenu("F&orm")
+        fileMenu.addMenu("Preview...").menuButtonClicked.connect(self.preview)
 
         def _showAbout(btn):
             TTkHelper.overlay(None, About(), 30,10)
         def _showAboutTTk(btn):
             TTkHelper.overlay(None, TTkAbout(), 30,10)
 
         helpMenu = topMenuFrame.menubarTop().addMenu("&Help", alignment=TTkK.RIGHT_ALIGN)
@@ -167,21 +163,19 @@
 
         btnPreview.clicked.connect(self.preview)
         btnExport.clicked.connect(self.quickExport)
         btnColors.toggled.connect(self.toggleColors)
 
         self._toolBar.addWidget(self._fileNameLabel)
 
-        if fileName:
-            self._openFile(fileName)
 
     def getWidgets(self):
         widgets = []
         def _getItems(layoutItem):
-            if layoutItem.layoutItemType() == TTkK.WidgetItem:
+            if layoutItem.layoutItemType == TTkK.WidgetItem:
                 superThing = layoutItem.widget()
                 if issubclass(type(superThing), SuperWidget):
                     widgets.append(superThing._wid)
                 for c in superThing.layout().children():
                     _getItems(c)
         _getItems(self._windowEditor.getTTk().widgetItem())
         return widgets
@@ -195,25 +189,19 @@
         tui = self._windowEditor.dumpDict()
         connections = self._sigslotEditor.dumpDict()
         data = {
             'version':'1.0.0',
             'tui':tui,
             'connections':connections}
 
-        win = QuickExport(data)
-        TTkHelper.overlay(None, win, 2, 2, modal=True)
-
-    @pyTTkSlot()
-    def scratchpad(self):
-        win = TTkWindow(
-                title="Mr Scratchpad",
-                size=(80,30),
-                layout=self._notepad,
+        win = QuickExport(
+                data=data,
+                title="Mr Export", size=(80,30),
                 flags=TTkK.WindowFlag.WindowMaximizeButtonHint|TTkK.WindowFlag.WindowCloseButtonHint)
-        TTkHelper.overlay(None, win, 2, 2, toolWindow=True)
+        TTkHelper.overlay(None, win, 2, 2, modal=True)
 
     @pyTTkSlot()
     def preview(self):
         tui = self._windowEditor.dumpDict()
         connections = self._sigslotEditor.dumpDict()
         # for line in jj.split('\n'):
         #     TTkLog.debug(f"{line}")
@@ -279,19 +267,20 @@
             fp.write(jj)
 
     @pyTTkSlot()
     def saveAs(self):
         def _approveFile(fileName):
             if os.path.exists(fileName):
                 messageBox = TTkMessageBox(
+                    title='Title',
                     text= (
                         TTkString( f'A file named "{os.path.basename(fileName)}" already exists.\nDo you want to replace it?', TTkColor.BOLD) +
                         TTkString( f'\n\nReplacing it will overwrite its contents.') ),
                     icon=TTkMessageBox.Icon.Warning,
                     standardButtons=TTkMessageBox.StandardButton.Discard|TTkMessageBox.StandardButton.Save|TTkMessageBox.StandardButton.Cancel)
                 messageBox.buttonSelected.connect(lambda btn : self._saveToFile(fileName) if btn == TTkMessageBox.StandardButton.Save else None)
                 TTkHelper.overlay(None, messageBox, 5, 5, True)
             else:
                 self._saveToFile(fileName)
-        filePicker = TTkFileDialogPicker(pos = (3,3), size=(80,30), acceptMode=TTkK.AcceptMode.AcceptSave, caption="Save As...", path=os.path.join(self._currentPath,self._fileName), fileMode=TTkK.FileMode.AnyFile ,filter="TTk Tui Files (*.tui.json);;Json Files (*.json);;All Files (*)")
+        filePicker = TTkFileDialogPicker(pos = (3,3), size=(80,30), caption="Save As...", path=os.path.join(self._currentPath,self._fileName), fileMode=TTkK.FileMode.AnyFile ,filter="TTk Tui Files (*.tui.json);;Json Files (*.json);;All Files (*)")
         filePicker.pathPicked.connect(_approveFile)
         TTkHelper.overlay(None, filePicker, 5, 5, True)
```

### Comparing `ttkDesigner-0.30.0a80/ttkDesigner/app/main.py` & `ttkDesigner-0.30.0a9/ttkDesigner/app/superobj/superlayouthbox.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,32 +16,16 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-import argparse
-
-from TermTk import TTk, TTkLog, TTkTheme, TTkTerm
-
-from .designer import TTkDesigner
-
-def main():
-    parser = argparse.ArgumentParser()
-    # parser.add_argument('-c', help=f'config folder (default: "{TTKodeCfg.pathCfg}")', default=TTKodeCfg.pathCfg)
-    parser.add_argument('filename', type=str, nargs='?', help='the file to open')
-    args = parser.parse_args()
-
-    # TTkLog.use_default_file_logging()
-    TTkTheme.loadTheme( TTkTheme.NERD )
-
-    root = TTk(
-            title="TTk Designer",
-            mouseTrack=True,
-            sigmask=(
-                TTkTerm.Sigmask.CTRL_C |
-                TTkTerm.Sigmask.CTRL_Q |
-                TTkTerm.Sigmask.CTRL_S |
-                TTkTerm.Sigmask.CTRL_Z ))
-    root.setLayout(TTkDesigner(fileName=args.filename))
-    root.mainloop()
+import TermTk as ttk
+import ttkDesigner.app.superobj as so
+from .superlayoutgrid import SuperLayoutGrid
+
+class SuperLayoutHBox(SuperLayoutGrid):
+    def __init__(self, *args, **kwargs):
+        kwargs['layout'] = ttk.TTkHBoxLayout()
+        super().__init__(*args, **kwargs)
+        self._orientation = ttk.TTkK.HORIZONTAL
```

### Comparing `ttkDesigner-0.30.0a80/ttkDesigner/app/propertyeditor.py` & `ttkDesigner-0.30.0a9/ttkDesigner/app/propertyeditor.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.30.0a80/ttkDesigner/app/signalsloteditor.py` & `ttkDesigner-0.30.0a9/ttkDesigner/app/signalsloteditor.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.30.0a80/ttkDesigner/app/superobj/__init__.py` & `ttkDesigner-0.30.0a9/ttkDesigner/app/superobj/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,13 +22,12 @@
 # SOFTWARE.
 
 from .supercontrol import SuperControlWidget
 
 from .superwidget            import SuperWidget
 from .superwidgettextedit    import SuperWidgetTextEdit
 from .superwidgetradiobutton import SuperWidgetRadioButton
-from .superwidgetframe       import SuperWidgetFrame
 
 from .superlayout     import SuperLayout
 from .superlayoutgrid import SuperLayoutGrid
 from .superlayoutvbox import SuperLayoutVBox
 from .superlayouthbox import SuperLayoutHBox
```

### Comparing `ttkDesigner-0.30.0a80/ttkDesigner/app/superobj/supercontrol.py` & `ttkDesigner-0.30.0a9/ttkDesigner/app/superobj/supercontrol.py`

 * *Files 12% similar despite different names*

```diff
@@ -75,16 +75,15 @@
             return True
         ret = super().mouseDragEvent(evt)
         self._alignWidToPos(bkPos)
         return ret
 
     def keyEvent(self, evt):
         if evt.type == ttk.TTkK.SpecialKey:
-            if ( evt.key in (ttk.TTkK.Key_Delete, ttk.TTkK.Key_Backspace) and
-                 not self._wid.isRootWidget() ):
+            if evt.key in (ttk.TTkK.Key_Delete, ttk.TTkK.Key_Backspace) :
                 self._wid.parentWidget().removeSuperWidget(self._wid)
                 self._wid.close()
                 self.close()
                 self._wid._designer.weModified.emit()
                 return True
             bkPos = self.pos()
             x,y = 0,0
@@ -93,21 +92,21 @@
             elif evt.key == ttk.TTkK.Key_Left:  x=-1
             elif evt.key == ttk.TTkK.Key_Right: x=1
             if any((x,y)):
                 self.move(bkPos[0]+x, bkPos[1]+y)
                 self._alignWidToPos(bkPos)
         return True
 
-    def paintEvent(self, canvas):
+    def paintEvent(self):
         w,h = self.size()
-        self._wid.paintEvent(canvas)
+        self._wid.paintEvent()
         self._wid.paintChildCanvas()
-        canvas.paintCanvas(
+        self._canvas.paintCanvas(
                 self._wid.getCanvas(),
                 (    1,     1, w, h), # geometry
                 (    0,     0, w, h), # slice
                 (    0,     0, w, h)) # bound
-        canvas.drawBox(pos=(0,0),size=self.size())
-        canvas.drawChar(pos=(  0,   0), char='▛')
-        canvas.drawChar(pos=(w-1,   0), char='▜')
-        canvas.drawChar(pos=(  0, h-1), char='▙')
-        canvas.drawChar(pos=(w-1, h-1), char='▟')
+        self._canvas.drawBox(pos=(0,0),size=self.size())
+        self._canvas.drawChar(pos=(  0,   0), char='▛')
+        self._canvas.drawChar(pos=(w-1,   0), char='▜')
+        self._canvas.drawChar(pos=(  0, h-1), char='▙')
+        self._canvas.drawChar(pos=(w-1, h-1), char='▟')
```

### Comparing `ttkDesigner-0.30.0a80/ttkDesigner/app/superobj/superlayout.py` & `ttkDesigner-0.30.0a9/ttkDesigner/app/superobj/superlayout.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,29 +106,23 @@
 
     def mouseDragEvent(self, evt) -> bool:
         if self._superRootWidget or not self._selectable: return False
         drag = ttk.TTkDrag()
         data = self
         canvas = self.getCanvas()
         canvas.clean()
-        self.paintEvent(canvas)
+        self.paintEvent()
         ttk.TTkWidget._paintChildCanvas(canvas, self.layout(), self.layout().geometry(), self.layout().offset())
         drag.setHotSpot(evt.x, evt.y)
         drag.setPixmap(canvas)
         drag.setData(data)
         drag.exec()
         self.parentWidget().removeSuperWidget(self)
         return True
 
-    def isRootWidget(self):
-        return self._superRootWidget
-
-    def makeRootWidget(self):
-        self._superRootWidget = True
-
     def superChild(self):
         return self._lay
 
     @staticmethod
     def slFromLayout(layout: ttk.TTkLayout, *args, **kwargs):
         if 'lay' not in kwargs:
             kwargs |= {'lay':layout}
@@ -215,15 +209,15 @@
         return super().move(x, y)
 
     def resizeEvent(self, w, h):
         x,y = self._lay.pos()
         self._lay.setGeometry(x,y,w,h)
         return super().resizeEvent(w, h)
 
-    def paintEvent(self, canvas):
+    def paintEvent(self):
         if self._selectable:
             if so.SuperWidget._showLayout:
                 w,h = self.size()
-                canvas.drawBox(pos=(0,0),size=(w,h), color=ttk.TTkColor.fg('#88DD88', modifier=ttk.TTkColorGradient(increment=+1)))
+                self._canvas.drawBox(pos=(0,0),size=(w,h), color=ttk.TTkColor.fg('#88DD88', modifier=ttk.TTkColorGradient(increment=+1)))
             else:
                 w,h = self.size()
-                canvas.drawBox(pos=(0,0),size=(w,h), color=ttk.TTkColor.fg('#223322', modifier=ttk.TTkColorGradient(increment=+1)))
+                self._canvas.drawBox(pos=(0,0),size=(w,h), color=ttk.TTkColor.fg('#223322', modifier=ttk.TTkColorGradient(increment=+1)))
```

### Comparing `ttkDesigner-0.30.0a80/ttkDesigner/app/superobj/superlayoutgrid.py` & `ttkDesigner-0.30.0a9/ttkDesigner/app/superobj/superlayoutgrid.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,111 +20,79 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import TermTk as ttk
 import ttkDesigner.app.superobj as so
 from .superlayout import SuperLayout
 
-class _SuperExpandButton(ttk.TTkButton):
-    NONE     = 0x00
-    PRESSED  = 0x01
-    RELEASED = 0x02
-    __slots__ = ('superExpandButtonDragged','superExpandButtonHidden','_mouseStatus')
+class _superExpandButton(ttk.TTkButton):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._direction = ttk.TTkK.TOP
-        # This signal is required by the superGridLayout to identify a dragging
-        # that may change the padding of the linked widget
-        self.superExpandButtonDragged = ttk.pyTTkSignal(int,int,bool)
-        self.superExpandButtonHidden = ttk.pyTTkSignal()
-        self._mouseStatus = self.NONE
 
     def setDirection(self, d):
         self._direction = d
 
     def _processInput(self, kevt, mevt):
         if not mevt:
             self.hide()
             return
         ax,ay = ttk.TTkHelper.absPos(self)
         w,h = self.size()
-        # x,y,w,h = self._boundaries
         mx,my = mevt.x, mevt.y
-        if ( self._mouseStatus == self.NONE and
-             ( not (0 <= (mx-ax) < w) or
-               not (0 <= (my-ay) < h) ) ) :
-            self.hide()
-
-    def mousePressEvent(self, evt):
-        self._mouseStatus = self.PRESSED
-        return super().mousePressEvent(evt)
-    def mouseReleaseEvent(self, evt):
-        self._mouseStatus = self.NONE
-        return super().mouseReleaseEvent(evt)
-
-    def mouseDragEvent(self, evt) -> bool:
-        # ttk.TTkLog.debug(f"Drag - {evt}")
-        x,y,w,h = self.geometry()
-        self.superExpandButtonDragged.emit(evt.x+x, evt.y+y, 0<=evt.x<w and 0<=evt.y<h)
-        return True
+        if ( not (0 <= (mx-ax) < w) or
+             not (0 <= (my-ay) < h) ) :
+             self.hide()
 
     def show(self):
         ttk.TTkHelper._rootWidget._input.inputEvent.connect(self._processInput)
         return super().show()
 
     def hide(self):
-        self.superExpandButtonHidden.emit()
         ttk.TTkHelper._rootWidget._input.inputEvent.disconnect(self._processInput)
         return super().hide()
 
-    def paintEvent(self, canvas):
+    def paintEvent(self):
+        canvas = self.getCanvas()
         # '▶','◀','▼','▲'
         w,h = self.size()
         if w==1:
-            canvas.drawText(text='╽', pos=(0,0),   color=ttk.TTkColor.fg("FFFF00"))
-            canvas.drawText(text='╿', pos=(0,h-1), color=ttk.TTkColor.fg("FFFF00"))
+            self.getCanvas().drawText(text='╽', pos=(0,0),     color=ttk.TTkColor.fg("FFFF00"))
+            self.getCanvas().drawText(text='╿', pos=(0,h-1), color=ttk.TTkColor.fg("FFFF00"))
             for yy in range(1,h-1):
-                canvas.drawText(text='┃', pos=(0, yy), color=ttk.TTkColor.fg("FFFF00"))
+                self.getCanvas().drawText(text='┃', pos=(0, yy), color=ttk.TTkColor.fg("FFFF00"))
         elif h==1:
             txt = '╼'+'━'*(w-2)+'╾'
-            canvas.drawText(text=txt, pos=(0,0), width=w, color=ttk.TTkColor.fg("FFFF00"))
+            self.getCanvas().drawText(text=txt, pos=(0,0), width=w, color=ttk.TTkColor.fg("FFFF00"))
 
         ch = {
             ttk.TTkK.TOP    : '▲',
             ttk.TTkK.BOTTOM : '▼',
             ttk.TTkK.LEFT   : '◀',
             ttk.TTkK.RIGHT  : '▶',
-            ttk.TTkK.HORIZONTAL : '↔',
-            ttk.TTkK.VERTICAL   : '↕',
         }.get(self._direction, 'X')
 
         x,y = 0,0
         if w==1 and h>4:
             y = h//2-2
             h = 4
         elif h==1 and w>4:
             x = w//2-2
             w = 4
         canvas.fill(pos=(x,y), size=(w,h), char=ch, color=ttk.TTkColor.fg("#FF0000")+ttk.TTkColor.bg("#FFFF44"))
 
 class SuperLayoutGrid(SuperLayout):
-    __slots__ = ('_expandButton','_dragOver','_spanOver','_expandStuff','_orientation','_snappId')
     def __init__(self, *args, **kwargs):
         kwargs['layout'] = ttk.TTkGridLayout()
         super().__init__(*args, **kwargs)
-        self._expandButton = _SuperExpandButton()
+        self._expandButton = _superExpandButton()
         self.rootLayout().addWidget(self._expandButton)
         self._expandButton.hide()
         self._expandButton.clicked.connect(self._clickExpand)
-        self._expandButton.superExpandButtonDragged.connect(self._expandButtonDragged)
-        self._expandButton.superExpandButtonHidden.connect(self._expandButtonHidden)
-        # self._expandButton.superExpandButtonDragged.connect()
         self._dragOver = None
-        self._spanOver = None
-        self._snappId  = None
         self._expandStuff = None
         self._orientation = ttk.TTkK.HORIZONTAL|ttk.TTkK.VERTICAL
 
     def dragEnterEvent(self, evt) -> bool:
         # ttk.TTkLog.debug(f"Enter")
         _, __, ___, self._dragOver = self._processDragOver(evt.x,evt.y)
         return True
@@ -138,73 +106,56 @@
         _, __, ___, self._dragOver = self._processDragOver(evt.x,evt.y)
         return True
     def dropEvent(self, evt) -> bool:
         self._dragOver = None
         self._pushRow, self._pushCol, self._direction, self._dragOver = self._processDragOver(evt.x,evt.y)
         return super().dropEvent(evt)
 
-    @ttk.pyTTkSlot()
-    def _expandButtonHidden(self):
-        self._spanOver = None
-        self.update()
+    # def mouseDragEvent(self, evt) -> bool:
+    #     if ret := super().mouseDragEvent(evt):
+    #         # removed unallocated rows/cols
+    #         self.parentWidget().layout().repack()
+    #     return ret
 
     def removeSuperWidget(self, sw):
         super().removeSuperWidget(sw)
         self.layout().repack()
 
     def mouseMoveEvent(self, evt) -> bool:
         # ttk.TTkLog.debug(f"Move {evt}")
-        dir, pos, wid, spanOver = self._processMouseOver(evt.x, evt.y)
-
+        dir, wid = self._processMouseOver(evt.x, evt.y)
         if not wid or not dir:
             self._expandButton.hide()
             return super().mouseMoveEvent(evt)
         x,y,w,h = wid.geometry()
         ebs = {
             ttk.TTkK.TOP    : (x,     y,     w, 1),
             ttk.TTkK.BOTTOM : (x,     y+h-1, w, 1),
             ttk.TTkK.LEFT   : (x,     y,     1, h),
             ttk.TTkK.RIGHT  : (x+w-1, y,     1, h),
-        }.get(pos, None)
+        }.get(dir, None)
 
         if not ebs:
             self._expandButton.hide()
         else:
             self._expandButton.setGeometry(*ebs)
             self._expandButton.setDirection(dir)
             self._expandButton.raiseWidget(raiseParent=False)
             self._expandButton.show()
         self._expandStuff = (dir,wid)
-        self._spanOver = spanOver
         return True
 
     def addSuperWidget(self, sw):
         self._dragOver = None
         if self._direction == ttk.TTkK.HORIZONTAL or self._orientation == ttk.TTkK.HORIZONTAL:
             self.layout().insertColumn(self._pushCol)
         elif self._direction == ttk.TTkK.VERTICAL or self._orientation == ttk.TTkK.VERTICAL:
             self.layout().insertRow(self._pushRow)
         self.layout().addWidget(sw, self._pushRow, self._pushCol,1,1)
 
-    @ttk.pyTTkSlot(int, int)
-    def _expandButtonDragged(self, dx, dy, expand):
-        # ttk.TTkLog.debug(f"Drag - {(dx,dy)}")
-        self._snappId = None
-        self.update()
-        if expand:
-            self._snappId = self._expandButton
-        elif self._spanOver:
-            for snapId in self._spanOver:
-                ((x,y,w,h),_) = snapId
-                ttk.TTkLog.debug(f"{snapId=} {(x,dx,w)=} {(y,dy,h)=}")
-                if x<=dx<x+w and y<=dy<y+h:
-                    # ttk.TTkLog.debug(f"XXXX -> {snapId=}")
-                    self._snappId = snapId
-                    return
-
     ttk.pyTTkSlot()
     def _clickExpand(self):
         if not self._expandButton.isVisible(): return
         self._expandButton.hide()
         dir, wid = self._expandStuff
         row = wid._row
         col = wid._col
@@ -213,106 +164,82 @@
         self.layout().removeItem(wid)
         if ttk.TTkK.TOP and row==0:
             self.layout().insertRow(0)
             row+=1
         elif ttk.TTkK.LEFT and col==0:
             self.layout().insertColumn(0)
             col+=1
-        rc = (row,col,rowspan,colspan)
-        if self._snappId == self._expandButton:
-            rc = {
-                ttk.TTkK.TOP    : (row-1,col,  rowspan+1,colspan),
-                ttk.TTkK.BOTTOM : (row,  col,  rowspan+1,colspan),
-                ttk.TTkK.LEFT   : (row,  col-1,rowspan,colspan+1),
-                ttk.TTkK.RIGHT  : (row,  col,  rowspan,colspan+1),
-            }.get(dir, (row,col,rowspan,colspan))
-        elif self._snappId:
-            (_,rc) = self._snappId
-        self._snappId = None
+        rc = {
+            ttk.TTkK.TOP    : (row-1,col,  rowspan+1,colspan),
+            ttk.TTkK.BOTTOM : (row,  col,  rowspan+1,colspan),
+            ttk.TTkK.LEFT   : (row,  col-1,rowspan,colspan+1),
+            ttk.TTkK.RIGHT  : (row,  col,  rowspan,colspan+1),
+        }.get(dir, (row,col,rowspan,colspan))
         self.layout().addItem(wid,*rc)
 
     def _processMouseOver(self, x, y):
         # cehck the closest edge
-        col, row, dir, pos, placesSpan = 0, 0, None, None, []
+        col, row, dir = 0,0,None
         wid = None
 
         if type(self.layout()) != ttk.TTkGridLayout:
-            return dir,pos,wid,placesSpan
+            return dir,wid
 
         # Retrieve a list of widths,heights
         rows,cols = self.layout().gridSize()
-        if not rows or not cols: return dir,pos,wid,placesSpan
+        if not rows or not cols: return dir,wid
 
         horSizes, verSizes = self.layout().getSizes()
 
         # Find the row/col where the pointer is in
         for col,(a,b) in enumerate(horSizes):
             if a <= x < a+b: break
         for row,(a,b) in enumerate(verSizes):
             if a <= y < a+b: break
 
-        # ix, iw = horSizes[col]
-        # iy, ih = verSizes[row]
+        ix, iw = horSizes[col]
+        iy, ih = verSizes[row]
 
         wid = self.layout().itemAtPosition(row,col)
         if wid == None:
-            return dir,pos,wid,placesSpan
+            return dir,wid
 
         col = wid._col
         row = wid._row
         rowspan = wid._rowspan
         colspan = wid._colspan
 
-        widX,widY,widW,widH = wid.geometry()
-        widMaxW,widMaxH = wid.maximumSize()
+        maxw,maxh = wid.maximumSize()
+
+        #
 
         #Top
-        if ( y==widY ):
-            placesSpan = [[[widX,iy,widW,1],[row+i,col,rowspan-i,colspan]] for i,(iy,ih) in enumerate(verSizes[row+1:row+rowspan],1)]
-            pos = ttk.TTkK.TOP if placesSpan else None
-            dir = ttk.TTkK.VERTICAL
-            if ( widMaxH>widH and
-                 not any([self.layout().itemAtPosition(row-1,col+cs) for cs in range(colspan)])):
-                dir = pos = ttk.TTkK.TOP
+        if (( y==iy ) and maxh>1 and
+              not any([self.layout().itemAtPosition(row-1,col+cs) for cs in range(colspan)])):
+            dir = ttk.TTkK.TOP
         #Bottom
-        elif (widY+widH==y+1):
-            placesSpan = [[[widX,iy+ih-1,widW,1],[row,col,i,colspan]] for i,(iy,ih) in enumerate(verSizes[row:row+rowspan-1],1)]
-            pos = ttk.TTkK.BOTTOM if placesSpan else None
-            dir = ttk.TTkK.VERTICAL
-            if ( widMaxH>widH and
-                 not any([self.layout().itemAtPosition(row+rowspan,col+cs) for cs in range(colspan)])):
-                dir = pos = ttk.TTkK.BOTTOM
+        elif ((iy+ih==y+1) and maxh>1 and
+              not any([self.layout().itemAtPosition(row+rowspan,col+cs) for cs in range(colspan)])):
+            dir = ttk.TTkK.BOTTOM
         #Left
-        elif (x==widX):
-            placesSpan = [[[ix,widY,1,widH],[row,col+i,rowspan,colspan-i]] for i,(ix,iw) in enumerate(horSizes[col+1:col+colspan],1)]
-            pos = ttk.TTkK.LEFT if placesSpan else None
-            dir = ttk.TTkK.HORIZONTAL
-            if ( widMaxW>widW and
-                 not any([self.layout().itemAtPosition(row+rs,col-1) for rs in range(rowspan)])):
-                dir = pos = ttk.TTkK.LEFT
+        elif ((x==ix) and maxw>1 and
+              not any([self.layout().itemAtPosition(row+rs,col-1) for rs in range(rowspan)])):
+            dir = ttk.TTkK.LEFT
         #Right
-        elif (widX+widW==x+1):
-            placesSpan = [[[ix+iw-1,widY,1,widH],[row,col,rowspan,i]] for i,(ix,iw) in enumerate(horSizes[col:col+colspan-1],1)]
-            pos = ttk.TTkK.RIGHT if placesSpan else None
-            dir = ttk.TTkK.HORIZONTAL
-            if ( widMaxW>widW and
-                 not any([self.layout().itemAtPosition(row+rs,col+colspan) for rs in range(rowspan)])):
-                dir = pos = ttk.TTkK.RIGHT
-        else:
-            wid=None
-
-        self._snappId=self._expandButton
+        elif ((ix+iw==x+1) and maxw>1 and
+              not any([self.layout().itemAtPosition(row+rs,col+colspan) for rs in range(rowspan)])):
+            dir = ttk.TTkK.RIGHT
 
         # ttk.TTkLog.debug(f"Move {dir} {wid}")
 
         # ttk.TTkLog.debug(f"{horSizes=}")
         # ttk.TTkLog.debug(f"{verSizes=}")
         # ttk.TTkLog.debug(f"{row=} {col=} {dir=} {self._dragOver=}")
         self.update()
-        return dir,pos,wid,placesSpan
+        return dir, wid
 
     def _processDragOver(self, x, y):
         # cehck the closest edge
         col, row, dir = 0,0,None
         ret = None
 
         # Retrieve a list of widths,heights
@@ -379,33 +306,21 @@
         # ttk.TTkLog.debug(f"{row=} {col=} {dir=} {self._dragOver=}")
         self.update()
         return row, col, dir, ret
 
     # Stupid hack to paint on top of the child widgets
     def paintChildCanvas(self):
         super().paintChildCanvas()
-
-        canvas = self.getCanvas()
-        def _lineDraw(x,y,w,h,color):
+        if self._dragOver is not None:
+            x,y,w,h = self._dragOver
             if h==1 and w==1:
-                canvas.drawText(text='◉', pos=(x,y), color=color)
+                self.getCanvas().drawText(text='◉', pos=(x,y), color=ttk.TTkColor.fg("FFFF00"))
             elif w==1:
-                canvas.drawText(text='╽', pos=(x,y),     color=color)
-                canvas.drawText(text='╿', pos=(x,y+h-1), color=color)
+                self.getCanvas().drawText(text='╽', pos=(x,y),     color=ttk.TTkColor.fg("FFFF00"))
+                self.getCanvas().drawText(text='╿', pos=(x,y+h-1), color=ttk.TTkColor.fg("FFFF00"))
                 for yy in range(y+1,y+h-1):
-                    canvas.drawText(text='┃', pos=(x, yy), color=color)
+                    self.getCanvas().drawText(text='┃', pos=(x, yy), color=ttk.TTkColor.fg("FFFF00"))
             elif h==1:
                 txt = '╼'+'━'*(w-2)+'╾'
-                canvas.drawText(text=txt, pos=(x,y), width=w, color=color)
+                self.getCanvas().drawText(text=txt, pos=(x,y), width=w, color=ttk.TTkColor.fg("FFFF00"))
             else:
-                canvas.drawBox(pos=(x,y), size=(w,h), color=color)
-
-        if self._dragOver is not None:
-            _lineDraw(*self._dragOver, ttk.TTkColor.fg("FFFF00"))
-        if self._spanOver:
-            for (geom,_) in self._spanOver:
-                _lineDraw(*geom, ttk.TTkColor.fg("FFFF00"))
-        if self._snappId and self._snappId != self._expandButton:
-            (geom,_) = self._snappId
-            _lineDraw(*geom, ttk.TTkColor.bg("88FF88")+ttk.TTkColor.fg("#000044"))
-
-
+                self.getCanvas().drawBox(pos=(x,y), size=(w,h), color=ttk.TTkColor.fg("FFFF00"))
```

### Comparing `ttkDesigner-0.30.0a80/ttkDesigner/app/superobj/superlayouthbox.py` & `ttkDesigner-0.30.0a9/ttkDesigner/app/superobj/superlayoutvbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,12 +20,12 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import TermTk as ttk
 import ttkDesigner.app.superobj as so
 from .superlayoutgrid import SuperLayoutGrid
 
-class SuperLayoutHBox(SuperLayoutGrid):
+class SuperLayoutVBox(SuperLayoutGrid):
     def __init__(self, *args, **kwargs):
         kwargs['layout'] = ttk.TTkHBoxLayout()
         super().__init__(*args, **kwargs)
-        self._orientation = ttk.TTkK.HORIZONTAL
+        self._orientation = ttk.TTkK.VERTICAL
```

### Comparing `ttkDesigner-0.30.0a80/ttkDesigner/app/superobj/superlayoutvbox.py` & `ttkDesigner-0.30.0a9/ttkDesigner/app/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,16 +16,27 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-import TermTk as ttk
-import ttkDesigner.app.superobj as so
-from .superlayoutgrid import SuperLayoutGrid
-
-class SuperLayoutVBox(SuperLayoutGrid):
-    def __init__(self, *args, **kwargs):
-        kwargs['layout'] = ttk.TTkHBoxLayout()
-        super().__init__(*args, **kwargs)
-        self._orientation = ttk.TTkK.VERTICAL
+import os
+import re
+import sys
+import argparse
+
+import appdirs
+
+from TermTk import TTk, TTkLog, TTkTheme
+
+from .cfg  import *
+from .about import *
+from .designer import TTkDesigner
+
+def main():
+    TTkLog.use_default_file_logging()
+    TTkTheme.loadTheme(TTkTheme.NERD )
+
+    root = TTk(title="TTk Designer", mouseTrack=True)
+    root.setLayout(TTkDesigner())
+    root.mainloop()
```

### Comparing `ttkDesigner-0.30.0a80/ttkDesigner/app/superobj/superobj.py` & `ttkDesigner-0.30.0a9/ttkDesigner/app/superobj/superobj.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.30.0a80/ttkDesigner/app/superobj/superwidget.py` & `ttkDesigner-0.30.0a9/ttkDesigner/app/superobj/superwidget.py`

 * *Files 3% similar despite different names*

```diff
@@ -112,20 +112,17 @@
         sw = so.SuperWidget(wid=wid, *args, **kwargs)
         sw.changeSuperLayout(type(wid.layout()))
         return sw
 
     @staticmethod
     def swFromWidget(wid, *args, **kwargs):
         swClass = {
-            ttk.TTkTextEdit:       so.SuperWidgetTextEdit,
-            ttk.TTkRadioButton:    so.SuperWidgetRadioButton,
-            ttk.TTkFrame:          so.SuperWidgetFrame,
-            ttk.TTkResizableFrame: so.SuperWidgetFrame,
-            ttk.TTkWindow:         so.SuperWidgetFrame,
-                }.get(type(wid), so.SuperWidget)
+            ttk.TTkTextEdit: so.SuperWidgetTextEdit,
+            ttk.TTkRadioButton: so.SuperWidgetRadioButton,
+                }.get(type(wid),so.SuperWidget)
         return swClass._swFromWidget(wid=wid, *args, **kwargs)
 
     @staticmethod
     def loadDict(designer, parent, widProp):
         ttkClass = getattr(ttk,widProp['class'])
         if issubclass(ttkClass,ttk.TTkLayout):
             demiProp = {
@@ -160,25 +157,18 @@
             wid = ttk.TTkUiLoader.loadDict(demiProp)
             sup = so.SuperWidget.swFromWidget(designer=designer, wid=wid, pos=wid.pos())
             sl = sup._superLayout
             children = widProp['layout']['children'] if setLayout else []
 
         for ch in children:
             sch = SuperWidget.loadDict(designer, parent, ch)
-            if issubclass(type(sch),so.SuperLayout):
-                schl = sch
-            else:
-                schl = sch._superLayout
-
             if issubclass(type(sl),so.SuperLayoutGrid):
                 sl.layout().addWidget(sch,ch['row'],ch['col'],ch['rowspan'],ch['colspan'])
-                schl.setDropBorder(1)
             else:
                 sl.layout().addWidget(sch)
-                schl.setDropBorder(0)
         return sup
 
     def changeSuperLayout(self, layout):
         sl = self._superLayout
         self.layout().removeWidget(sl)
         if layout == ttk.TTkVBoxLayout:
             sl = so.SuperLayoutVBox(designer=self._designer, lay=self._wid.layout(), selectable=False)
@@ -200,17 +190,14 @@
         self.setMaximumSize(*(self._wid.maximumSize()))
         self.setMinimumSize(*(self._wid.minimumSize()))
         self.update()
 
     def mousePressEvent(self, evt) -> bool:
         return True
 
-    def isRootWidget(self):
-        return self._superRootWidget
-
     def makeRootWidget(self):
         self._superRootWidget = True
 
     def pushSuperControlWidget(self):
         # if self._superRootWidget: return False
         scw = so.SuperControlWidget(self)
         ttk.TTkHelper.removeOverlay()
@@ -251,25 +238,25 @@
 
     def resizeEvent(self, w, h):
         self._wid.resize(w,h)
         self._wid._canvas.updateSize()
         self.superResized.emit(w,h)
         return super().resizeEvent(w, h)
 
-    def paintEvent(self, canvas):
+    def paintEvent(self):
         w,h = self.size()
         if SuperWidget._showLayout:
             t,b,l,r = self._wid.getPadding()
             for y in range(h):
-                canvas.drawText(pos=(0,y),text='',width=w,color=self._layoutColor)
+                self._canvas.drawText(pos=(0,y),text='',width=w,color=self._layoutColor)
             for y in range(t,h-b):
-                canvas.drawText(pos=(l,y),text='',width=w-r-l,color=self._layoutPadColor)
-            # canvas.fill(color=self._layoutColor)
-            # canvas.fill(pos=(l,t), size=(w-r-l,h-b-t), color=self._layoutPadColor)
+                self._canvas.drawText(pos=(l,y),text='',width=w-r-l,color=self._layoutPadColor)
+            # self._canvas.fill(color=self._layoutColor)
+            # self._canvas.fill(pos=(l,t), size=(w-r-l,h-b-t), color=self._layoutPadColor)
         else:
             self._wid.getCanvas().updateSize()
-            self._wid.paintEvent(self._wid.getCanvas())
-            canvas.paintCanvas(
+            self._wid.paintEvent()
+            self._canvas.paintCanvas(
                     self._wid.getCanvas(),
                     (    0,     0, w, h), # geometry
                     (    0,     0, w, h), # slice
                     (    0,     0, w, h)) # bound
```

### Comparing `ttkDesigner-0.30.0a80/ttkDesigner/app/superobj/superwidgetframe.py` & `ttkDesigner-0.30.0a9/ttkDesigner/app/superobj/superwidgetradiobutton.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,11 +19,16 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import TermTk as ttk
 import ttkDesigner.app.superobj as so
 
-class SuperWidgetFrame(so.SuperWidget):
+class SuperWidgetRadioButton(so.SuperWidget):
     def getSuperProperties(self):
         exceptions, exclude = super().getSuperProperties()
+        exceptions |= {
+            'RadioGroup' : {
+                'init': {'name':'radiogroup',            'type':str } ,
+                'get':  {'cb':ttk.TTkRadioButton.radioGroup, 'type':str } ,
+                'set':  {'cb':lambda w,l: setattr(w,'_radiogroup',l), 'type':str } } }
         return exceptions, exclude
```

### Comparing `ttkDesigner-0.30.0a80/ttkDesigner/app/superobj/superwidgettextedit.py` & `ttkDesigner-0.30.0a9/ttkDesigner/app/superobj/superwidgettextedit.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.30.0a80/ttkDesigner/app/treeinspector.py` & `ttkDesigner-0.30.0a9/ttkDesigner/app/treeinspector.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     @ttk.pyTTkSlot()
     def refresh(self, thing=None):
         self._tomTree.clear()
         self._tomTree.addTopLevelItem(TreeInspector._getTomTreeItem(self._windowEditor.getTTk().widgetItem()))
 
     @staticmethod
     def _getTomTreeItem(layoutItem, widSelected=None):
-        if layoutItem.layoutItemType() == ttk.TTkK.WidgetItem:
+        if layoutItem.layoutItemType == ttk.TTkK.WidgetItem:
             superThing = thing = layoutItem.widget()
             if issubclass(type(superThing), SuperWidget):
                 thing = thing._wid
             elif issubclass(type(superThing), SuperLayout):
                 thing = thing._lay
             expanded = True # ttk.TTkHelper.isParent(widSelected,thing) if widSelected else False
             if issubclass(type(superThing), SuperWidget):
@@ -129,14 +129,14 @@
             #     if c == thing.layout(): continue
             #     if c.layoutItemType == ttk.TTkK.LayoutItem:
             #         top.addChild(tc:=_TTkTomTreeWidgetItem(["layout (Other)", c.__class__.__name__, ""]))
             #         for cc in c.children():
             #             tc.addChild(TreeInspector._getTomTreeItem(cc,widSelected))
             return top
 
-        if layoutItem.layoutItemType() == ttk.TTkK.LayoutItem:
+        if layoutItem.layoutItemType == ttk.TTkK.LayoutItem:
             top = _TTkTomTreeWidgetItem(["layout", layoutItem.__class__.__name__,"",layoutItem.__class__.__name__])
             for c in layoutItem.children():
                 top.addChild(TreeInspector._getTomTreeItem(c,widSelected))
             return top
 
         return _TTkTomTreeWidgetItem(["ERROR!!!", "None"])
```

### Comparing `ttkDesigner-0.30.0a80/ttkDesigner/app/widgetbox.py` & `ttkDesigner-0.30.0a9/ttkDesigner/app/widgetbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,21 +107,21 @@
             pm = ttk.TTkCanvas(width=w, height=h)
             pm.drawBox(pos=(0,0),size=(w,h), color=ttk.TTkColor.fg('#888888'))
             drag.setPixmap(pm)
         drag.setData(data)
         drag.exec()
         return True
 
-    def paintEvent(self, canvas):
+    def paintEvent(self):
         if self.isEnabled():
             color=ttk.TTkColor.RST
         else:
             color=ttk.TTkColor.fg('#AAAAAA')
-        canvas.drawText(text=self._itemName, pos=(1,1), color=color)
-        canvas.drawBox(pos=(0,0),size=self.size(), color=color)
+        self._canvas.drawText(text=self._itemName, pos=(1,1), color=color)
+        self._canvas.drawBox(pos=(0,0),size=self.size(), color=color)
 
 class WidgetBox(ttk.TTkVBoxLayout):
     def __init__(self, designer, *args, **kwargs):
         super().__init__(*args, **kwargs)
         for tw in dWidgets:
             self.addWidget(ttk.TTkLabel(text=tw, color=ttk.TTkColor.fg('#FFFF88')+ttk.TTkColor.bg('#0000FF')))
             for ww in dWidgets[tw]:
```

### Comparing `ttkDesigner-0.30.0a80/ttkDesigner/app/windoweditor.py` & `ttkDesigner-0.30.0a9/ttkDesigner/app/windoweditor.py`

 * *Files 10% similar despite different names*

```diff
@@ -56,25 +56,29 @@
         self._ttk = SuperWidget(wid=ttk.TTkWidget(name = 'MainWidget'), designer=self._designer, pos=(4,2), superRootWidget=True)
         self._ttk.resize(self.width()-8,self.height()-4)
         self._snapRootWidget = True
         self.layout().addWidget(self._ttk)
         self._ttk.superResized.connect(self._superChanged)
         self._ttk.superMoved.connect(self._superChanged)
 
-    def importSuperWidget(self, sw):
+    def importWidget(self, wid):
         if self._ttk:
             self._ttk.superResized.disconnect(self._superChanged)
             self._ttk.superMoved.disconnect(self._superChanged)
-            self.layout().removeWidget(self._ttk)
         self._snapRootWidget = False
+        self._ttk = SuperWidget.swFromWidget(wid=wid, designer=self._designer, pos=(4,2), size=(self.width()-8,self.height()-4))
+        self._ttk.makeRootWidget()
+        self.layout().addWidget(self._ttk)
+
+    def importSuperWidget(self, sw):
+        if self._ttk:
+            self.layout().removeWidget(self._ttk)
         self._ttk = sw
         self._ttk.makeRootWidget()
         self.layout().addWidget(self._ttk)
-        self._ttk.superResized.connect(self._superChanged)
-        self._ttk.superMoved.connect(self._superChanged)
 
     def getTTk(self):
         return self._ttk
 
     def dumpDict(self):
         return self._ttk.dumpDict()
 
@@ -97,25 +101,27 @@
     def viewFullAreaSize(self):
         x,y,w,h = self.layout().fullWidgetAreaGeometry()
         return x+w, y+h
 
     def viewDisplayedSize(self):
         return self.size()
 
-    def paintEvent(self, canvas):
+    def paintEvent(self):
         w,h = self.size()
-        # canvas.fill(pos=(0,0),size=(w,h), char="╳", color=ttk.TTkColor.fg("#444400")+ttk.TTkColor.bg("#000044"))
-        canvas.fill(pos=(0,0),size=(w,h), char="#", color=ttk.TTkColor.fg("#220044")+ttk.TTkColor.bg("#000022"))
+        # self._canvas.fill(pos=(0,0),size=(w,h), char="╳", color=ttk.TTkColor.fg("#444400")+ttk.TTkColor.bg("#000044"))
+        self._canvas.fill(pos=(0,0),size=(w,h), char="#", color=ttk.TTkColor.fg("#220044")+ttk.TTkColor.bg("#000022"))
 
 class WindowEditor(ttk.TTkAbstractScrollArea):
-    __slots__ = ('getTTk', 'dumpDict', 'importSuperWidget',
+    __slots__ = ('getTTk', 'dumpDict', 'importWidget', 'importSuperWidget',
                  # Forwarded slots
                  'newWindow', 'newWidget')
     def __init__(self, designer, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.setViewport(wev := WindowEditorView(designer))
+        # wev.importWidget(ttk.TTkWidget(name = 'TTk'))
         # Forward Methods
         self.getTTk            = wev.getTTk
         self.dumpDict          = wev.dumpDict
+        self.importWidget      = wev.importWidget
         self.importSuperWidget = wev.importSuperWidget
         self.newWindow         = wev.newWindow
         self.newWidget         = wev.newWidget
```

### Comparing `ttkDesigner-0.30.0a80/ttkDesigner/tui/newWindow.tui.json` & `ttkDesigner-0.30.0a9/ttkDesigner/tui/newWindow.tui.json`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.30.0a80/ttkDesigner.egg-info/SOURCES.txt` & `ttkDesigner-0.30.0a9/ttkDesigner.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -10,27 +10,24 @@
 ttkDesigner.egg-info/requires.txt
 ttkDesigner.egg-info/top_level.txt
 ttkDesigner/app/__init__.py
 ttkDesigner/app/about.py
 ttkDesigner/app/cfg.py
 ttkDesigner/app/designer.py
 ttkDesigner/app/main.py
-ttkDesigner/app/notepad.py
 ttkDesigner/app/propertyeditor.py
 ttkDesigner/app/quickexport.py
 ttkDesigner/app/signalsloteditor.py
 ttkDesigner/app/treeinspector.py
 ttkDesigner/app/widgetbox.py
 ttkDesigner/app/windoweditor.py
 ttkDesigner/app/superobj/__init__.py
 ttkDesigner/app/superobj/supercontrol.py
 ttkDesigner/app/superobj/superlayout.py
 ttkDesigner/app/superobj/superlayoutgrid.py
 ttkDesigner/app/superobj/superlayouthbox.py
 ttkDesigner/app/superobj/superlayoutvbox.py
 ttkDesigner/app/superobj/superobj.py
 ttkDesigner/app/superobj/superwidget.py
-ttkDesigner/app/superobj/superwidgetframe.py
 ttkDesigner/app/superobj/superwidgetradiobutton.py
 ttkDesigner/app/superobj/superwidgettextedit.py
-ttkDesigner/tui/newWindow.tui.json
-ttkDesigner/tui/quickExport.tui.json
+ttkDesigner/tui/newWindow.tui.json
```

