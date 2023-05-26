# Comparing `tmp/plogger-1.0.7.tar.gz` & `tmp/plogger-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plogger-1.0.7.tar", last modified: Mon Oct 10 15:24:59 2022, max compression
+gzip compressed data, was "plogger-1.0.8.tar", last modified: Fri May 26 16:01:54 2023, max compression
```

## Comparing `plogger-1.0.7.tar` & `plogger-1.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2022-10-10 15:24:59.691157 plogger-1.0.7/
--rw-rw-rw-   0        0        0     1095 2022-10-10 12:53:46.000000 plogger-1.0.7/LICENSE
--rw-rw-rw-   0        0        0     3108 2022-10-10 15:24:59.690246 plogger-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2269 2022-10-10 15:22:43.000000 plogger-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2022-10-10 15:24:59.677157 plogger-1.0.7/plogger/
--rw-rw-rw-   0        0        0     7889 2022-10-10 15:22:43.000000 plogger-1.0.7/plogger/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-10 15:24:59.689160 plogger-1.0.7/plogger.egg-info/
--rw-rw-rw-   0        0        0     3108 2022-10-10 15:24:59.000000 plogger-1.0.7/plogger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      170 2022-10-10 15:24:59.000000 plogger-1.0.7/plogger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-10 15:24:59.000000 plogger-1.0.7/plogger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2022-10-10 15:24:59.000000 plogger-1.0.7/plogger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-10-10 15:24:59.691157 plogger-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1161 2022-10-10 15:20:24.000000 plogger-1.0.7/setup.py
+drwxr-xr-x   0 c-pher     (502) staff       (20)        0 2023-05-26 16:01:54.774302 plogger-1.0.8/
+-rw-r--r--   0 c-pher     (502) staff       (20)     1074 2023-05-26 15:15:27.000000 plogger-1.0.8/LICENSE
+-rw-r--r--   0 c-pher     (502) staff       (20)     3100 2023-05-26 16:01:54.774184 plogger-1.0.8/PKG-INFO
+-rw-r--r--   0 c-pher     (502) staff       (20)     2283 2023-05-26 16:01:50.000000 plogger-1.0.8/README.md
+drwxr-xr-x   0 c-pher     (502) staff       (20)        0 2023-05-26 16:01:54.773298 plogger-1.0.8/plogger/
+-rw-r--r--   0 c-pher     (502) staff       (20)     5452 2023-05-26 16:00:11.000000 plogger-1.0.8/plogger/__init__.py
+drwxr-xr-x   0 c-pher     (502) staff       (20)        0 2023-05-26 16:01:54.774015 plogger-1.0.8/plogger.egg-info/
+-rw-r--r--   0 c-pher     (502) staff       (20)     3100 2023-05-26 16:01:54.000000 plogger-1.0.8/plogger.egg-info/PKG-INFO
+-rw-r--r--   0 c-pher     (502) staff       (20)      170 2023-05-26 16:01:54.000000 plogger-1.0.8/plogger.egg-info/SOURCES.txt
+-rw-r--r--   0 c-pher     (502) staff       (20)        1 2023-05-26 16:01:54.000000 plogger-1.0.8/plogger.egg-info/dependency_links.txt
+-rw-r--r--   0 c-pher     (502) staff       (20)        8 2023-05-26 16:01:54.000000 plogger-1.0.8/plogger.egg-info/top_level.txt
+-rw-r--r--   0 c-pher     (502) staff       (20)       38 2023-05-26 16:01:54.774344 plogger-1.0.8/setup.cfg
+-rw-r--r--   0 c-pher     (502) staff       (20)     1129 2023-05-26 15:18:17.000000 plogger-1.0.8/setup.py
```

### Comparing `plogger-1.0.7/PKG-INFO` & `plogger-1.0.8/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,120 +1,104 @@
-Metadata-Version: 2.1
-Name: plogger
-Version: 1.0.7
-Summary: A simple high level logger wrapper to log into console/file with different level.
-Home-page: https://github.com/c-pher/plogger.git
-Author: Andrey Komissarov
-Author-email: a.komisssarov@gmail.com
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: System Administrators
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Topic :: System :: Systems Administration
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![PyPI version](https://badge.fury.io/py/plogger.svg)](https://badge.fury.io/py/plogger)
-[![Build Status](https://travis-ci.org/c-pher/plogger.svg?branch=master)](https://travis-ci.org/c-pher/plogger)
-[![Coverage Status](https://coveralls.io/repos/github/c-pher/plogger/badge.svg?branch=master)](https://coveralls.io/github/c-pher/plogger?branch=master)
-
-
-## Plogger
-
-Plogger - a simple high level logger wrapper to log into console/file with different level. Used built-in logger module.
-
-## Installation
-For most users, the recommended method to install is via pip:
-```cmd
-pip install plogger
-```
-
-## Import and usage
-
-```python
-from plogger import logger
-
-log = logger('NAME')
-log.info('Test message')
-```
-
-```python
-import plogger
-
-log = plogger.logger('NAME')
-log.info('Log it as INFO')
-```
-
-## Result
-
-```cmd
-2022-10-10 18:17:46 | INFO      | NAME                 26 | <module> | Log it as INFO
-```
-
-## Usage
-
-- As standalone logger function:
-
-```python
-import plogger
-
-logger = plogger.logger('NAME', level=10)
-
-logger.info('Test message')
-logger.error('Test message')
-logger.warning('Test message')
-logger.debug('Test message')
-```
-
-```
-2022-10-10 18:18:44 | INFO      | NAME                 27 | <module> | Test message
-2022-10-10 18:18:44 | ERROR     | NAME                 28 | <module> | Test message
-2022-10-10 18:18:44 | WARNING   | NAME                 29 | <module> | Test message
-2022-10-10 18:18:44 | DEBUG     | NAME                 30 | <module> | Test message
-```
-
-## Changelog
-
-##### 1.0.7 (10.10.2022)
-
-- Method/function name added into log
-
-##### 1.0.6 (16.04.2022)
-
-- Enable/disable logging fixed
-
-##### 1.0.5.post0 (4.04.2022)
-
-- minor changes in log entry format
-
-##### 1.0.5 (4.04.2022)
-
-- Console log will be colorized.
-- use_color=True param added
-- Line number added to the log
-
-##### 1.0.4 (28.03.2022)
-
-- added log level selection with the "level" param
-- log level entry aligned
-
-##### 1.0.3 (29.01.2022)
-
-Fixed entries duplicating. Added handlers cleaning
-
-##### 1.0.2 (25.01.2022)
-
-console_output=sys.stderr by default
-
-##### 1.0.1 (10.01.2022)
-
-Added console_output=sys.stdout param
-
-##### 1.0.0 (26.01.2020)
-
-Added logger() function
+[![PyPI version](https://badge.fury.io/py/plogger.svg)](https://badge.fury.io/py/plogger)
+[![Build Status](https://travis-ci.org/c-pher/plogger.svg?branch=master)](https://travis-ci.org/c-pher/plogger)
+[![Coverage Status](https://coveralls.io/repos/github/c-pher/plogger/badge.svg?branch=master)](https://coveralls.io/github/c-pher/plogger?branch=master)
+
+
+## Plogger
+
+Plogger - a simple high level logger wrapper to log into console/file with different level. Used built-in logger module.
+
+## Installation
+For most users, the recommended method to install is via pip:
+```cmd
+pip install plogger
+```
+
+## Import and usage
+
+```python
+from plogger import logger
+
+log = logger('NAME')
+log.info('Test message')
+```
+
+```python
+import plogger
+
+log = plogger.logger('NAME')
+log.info('Log it as INFO')
+```
+
+## Result
+
+```cmd
+2022-10-10 18:17:46 | INFO      | NAME                 26 | <module> | Log it as INFO
+```
+
+## Usage
+
+- As standalone logger function:
+
+```python
+import plogger
+
+logger = plogger.logger('NAME', level=10)
+
+logger.info('Test message')
+logger.error('Test message')
+logger.warning('Test message')
+logger.debug('Test message')
+```
+
+```
+2022-10-10 18:18:44 | INFO      | NAME                 27 | <module> | Test message
+2022-10-10 18:18:44 | ERROR     | NAME                 28 | <module> | Test message
+2022-10-10 18:18:44 | WARNING   | NAME                 29 | <module> | Test message
+2022-10-10 18:18:44 | DEBUG     | NAME                 30 | <module> | Test message
+```
+
+## Changelog
+
+##### 1.0.8 (26.05.2022)
+
+- time format changed. microseconds added (2023-05-26 18:24:28.389)
+- class obsolete
+
+##### 1.0.7 (10.10.2022)
+
+- Method/function name added into log
+
+##### 1.0.6 (16.04.2022)
+
+- Enable/disable logging fixed
+
+##### 1.0.5.post0 (4.04.2022)
+
+- minor changes in log entry format
+
+##### 1.0.5 (4.04.2022)
+
+- Console log will be colorized.
+- use_color=True param added
+- Line number added to the log
+
+##### 1.0.4 (28.03.2022)
+
+- added log level selection with the "level" param
+- log level entry aligned
+
+##### 1.0.3 (29.01.2022)
+
+Fixed entries duplicating. Added handlers cleaning
+
+##### 1.0.2 (25.01.2022)
+
+console_output=sys.stderr by default
+
+##### 1.0.1 (10.01.2022)
+
+Added console_output=sys.stdout param
+
+##### 1.0.0 (26.01.2020)
+
+Added logger() function
```

### Comparing `plogger-1.0.7/setup.py` & `plogger-1.0.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-from os import path
-
-from setuptools import setup
-
-this_directory = path.abspath(path.dirname(__file__))
-with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
-    long_description = f.read()
-
-setup(
-    name='plogger',
-    version='1.0.7',
-    packages=['plogger'],
-    url='https://github.com/c-pher/plogger.git',
-    license='MIT',
-    author='Andrey Komissarov',
-    author_email='a.komisssarov@gmail.com',
-    description='A simple high level logger wrapper to log into console/file with different level.',
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    classifiers=[
-        'Programming Language :: Python :: 3',
-        'License :: OSI Approved :: MIT License',
-        'Operating System :: OS Independent',
-        'Intended Audience :: System Administrators',
-        'Intended Audience :: Developers',
-        'Natural Language :: English',
-        'Programming Language :: Python :: 3.6',
-        'Topic :: System :: Systems Administration',
-        'Topic :: Software Development :: Libraries :: Python Modules'
-    ],
-    python_requires='>=3.6',
-)
+from os import path
+
+from setuptools import setup
+
+this_directory = path.abspath(path.dirname(__file__))
+with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
+    long_description = f.read()
+
+setup(
+    name='plogger',
+    version='1.0.8',
+    packages=['plogger'],
+    url='https://github.com/c-pher/plogger.git',
+    license='MIT',
+    author='Andrey Komissarov',
+    author_email='a.komisssarov@gmail.com',
+    description='A simple high level logger wrapper to log into console/file with different level.',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    classifiers=[
+        'Programming Language :: Python :: 3',
+        'License :: OSI Approved :: MIT License',
+        'Operating System :: OS Independent',
+        'Intended Audience :: System Administrators',
+        'Intended Audience :: Developers',
+        'Natural Language :: English',
+        'Programming Language :: Python :: 3.6',
+        'Topic :: System :: Systems Administration',
+        'Topic :: Software Development :: Libraries :: Python Modules'
+    ],
+    python_requires='>=3.6',
+)
```

