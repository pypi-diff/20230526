# Comparing `tmp/pymemuc-0.2.6.tar.gz` & `tmp/pymemuc-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymemuc-0.2.6.tar", max compression
+gzip compressed data, was "pymemuc-0.2.7.tar", max compression
```

## Comparing `pymemuc-0.2.6.tar` & `pymemuc-0.2.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1057 2023-04-19 18:00:35.150590 pymemuc-0.2.6/LICENSE
--rw-r--r--   0        0        0     1580 2023-04-19 18:00:35.150590 pymemuc-0.2.6/README.md
--rw-r--r--   0        0        0      386 2023-04-19 18:00:35.154590 pymemuc-0.2.6/pymemuc/__init__.py
--rw-r--r--   0        0        0    22754 2023-04-19 18:00:35.154590 pymemuc-0.2.6/pymemuc/_command.py
--rw-r--r--   0        0        0      465 2023-04-19 18:00:35.154590 pymemuc-0.2.6/pymemuc/_constants.py
--rw-r--r--   0        0        0     4984 2023-04-19 18:00:35.154590 pymemuc-0.2.6/pymemuc/_control.py
--rw-r--r--   0        0        0     1150 2023-04-19 18:00:35.154590 pymemuc-0.2.6/pymemuc/_decorators.py
--rw-r--r--   0        0        0    13670 2023-04-19 18:00:35.158590 pymemuc-0.2.6/pymemuc/_manage.py
--rw-r--r--   0        0        0     3938 2023-04-19 18:00:35.158590 pymemuc-0.2.6/pymemuc/_memuc.py
--rw-r--r--   0        0        0      891 2023-04-19 18:00:35.158590 pymemuc-0.2.6/pymemuc/exceptions.py
--rw-r--r--   0        0        0     2216 2023-04-19 18:00:35.158590 pymemuc-0.2.6/pymemuc/pymemuc.py
--rw-r--r--   0        0        0      379 2023-04-19 18:00:35.158590 pymemuc-0.2.6/pymemuc/vminfo.py
--rw-r--r--   0        0        0     1655 2023-04-19 18:00:58.818617 pymemuc-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     2432 1970-01-01 00:00:00.000000 pymemuc-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1057 2023-05-26 04:32:01.749582 pymemuc-0.2.7/LICENSE
+-rw-r--r--   0        0        0     1586 2023-05-26 04:32:01.749582 pymemuc-0.2.7/README.md
+-rw-r--r--   0        0        0      386 2023-05-26 04:32:01.757582 pymemuc-0.2.7/pymemuc/__init__.py
+-rw-r--r--   0        0        0    22761 2023-05-26 04:32:01.757582 pymemuc-0.2.7/pymemuc/_command.py
+-rw-r--r--   0        0        0      465 2023-05-26 04:32:01.757582 pymemuc-0.2.7/pymemuc/_constants.py
+-rw-r--r--   0        0        0     4984 2023-05-26 04:32:01.757582 pymemuc-0.2.7/pymemuc/_control.py
+-rw-r--r--   0        0        0     1150 2023-05-26 04:32:01.757582 pymemuc-0.2.7/pymemuc/_decorators.py
+-rw-r--r--   0        0        0    13670 2023-05-26 04:32:01.757582 pymemuc-0.2.7/pymemuc/_manage.py
+-rw-r--r--   0        0        0     3980 2023-05-26 04:32:01.757582 pymemuc-0.2.7/pymemuc/_memuc.py
+-rw-r--r--   0        0        0      891 2023-05-26 04:32:01.757582 pymemuc-0.2.7/pymemuc/exceptions.py
+-rw-r--r--   0        0        0     2216 2023-05-26 04:32:01.757582 pymemuc-0.2.7/pymemuc/pymemuc.py
+-rw-r--r--   0        0        0      379 2023-05-26 04:32:01.757582 pymemuc-0.2.7/pymemuc/vminfo.py
+-rw-r--r--   0        0        0     1665 2023-05-26 04:32:28.577600 pymemuc-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     2394 1970-01-01 00:00:00.000000 pymemuc-0.2.7/PKG-INFO
```

### Comparing `pymemuc-0.2.6/LICENSE` & `pymemuc-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pymemuc-0.2.6/README.md` & `pymemuc-0.2.7/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # pymemuc
 
-[![GitHub](https://img.shields.io/github/license/marmig0404/pymemuc)](LICENSE) [![Documentation Status](https://readthedocs.org/projects/pymemuc/badge/?version=latest)][full_doc] [![PyPI](https://img.shields.io/pypi/v/pymemuc) ![PyPI - Downloads](https://img.shields.io/pypi/dm/pymemuc)][pypi_link] [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pymemuc)][python_link] [![CodeFactor](https://www.codefactor.io/repository/github/marmig0404/pymemuc/badge)][codefactor_link]
+[![GitHub](https://img.shields.io/github/license/martinmiglio/pymemuc)](LICENSE) [![Documentation Status](https://readthedocs.org/projects/pymemuc/badge/?version=latest)][full_doc] [![PyPI](https://img.shields.io/pypi/v/pymemuc) ![PyPI - Downloads](https://img.shields.io/pypi/dm/pymemuc)][pypi_link] [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pymemuc)][python_link] [![CodeFactor](https://www.codefactor.io/repository/github/martinmiglio/pymemuc/badge)][codefactor_link]
 
 A wrapper for [MEmu Command (MEMUC)][memuc_docs] in python.
 
 Allows for easy interaction with MEmu VMs, including VM image management, VM control, running VM commands and ADB interaction.
 
 ## Installation
 
@@ -38,11 +38,11 @@
 
 ## Documentation
 
 See the [API documentation][full_doc].
 
 [python_link]: https://www.python.org/
 [pypi_link]: https://pypi.org/project/pymemuc/
-[codefactor_link]: https://www.codefactor.io/repository/github/marmig0404/pymemuc
+[codefactor_link]: https://www.codefactor.io/repository/github/martinmiglio/pymemuc
 [memuc_docs]: https://www.memuplay.com/blog/memucommand-reference-manual.html
 [demo_notebook]: demo/demo.ipynb
 [full_doc]: https://pymemuc.martinmiglio.dev/
```

### Comparing `pymemuc-0.2.6/pymemuc/_command.py` & `pymemuc-0.2.7/pymemuc/_command.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """This module contains functions for commanding running virtual machines with memuc.exe.
 Functions for interacting with running VMs are defined here."""
-from typing import TYPE_CHECKING, Literal, Union
+from typing import TYPE_CHECKING, Literal, Tuple, Union
 
 from .exceptions import PyMemucError, PyMemucIndexError, PyMemucTimeoutExpired
 
 if TYPE_CHECKING:
     from pymemuc import PyMemuc
 
 
@@ -322,15 +322,15 @@
 
 
 def execute_command_vm(
     self: "PyMemuc",
     command,
     vm_index: Union[int, None] = None,
     vm_name: Union[str, None] = None,
-) -> tuple[int, str]:
+) -> Tuple[int, str]:
     """Execute a command on a VM, must specify either a vm index or a vm name
 
     :param command: Command to execute
     :type command: str
     :param vm_index: VM index. Defaults to None.
     :type vm_index: int, optional
     :param vm_name: VM name. Defaults to None.
@@ -382,15 +382,15 @@
         raise PyMemucError(f"Failed to change GPS location: {output}")
     return True
 
 
 # TODO: fix parsing of the output
 def get_public_ip_vm(
     self: "PyMemuc", vm_index: Union[int, None] = None, vm_name: Union[str, None] = None
-) -> tuple[int, str]:
+) -> Tuple[int, str]:
     """Get the public IP of a VM, must specify either a vm index or a vm name
 
     :param vm_index: VM index. Defaults to None.
     :type vm_index: int, optional
     :param vm_name: VM name. Defaults to None.
     :type vm_name: str, optional
     :raises PyMemucIndexError: an error if neither a vm index or a vm name is specified
@@ -500,15 +500,15 @@
 
 # TODO: debug this, it doesn't work
 def set_accelerometer_vm(
     self: "PyMemuc",
     value: tuple[float, float, float],
     vm_index: Union[int, None] = None,
     vm_name: Union[str, None] = None,
-) -> tuple[int, str]:
+) -> Tuple[int, str]:
     """Set the accelerometer on a VM, must specify either a vm index or a vm name
 
     :param value: the accelerometer value to set
     :type value: tuple[float, float, float]
     :param vm_index: VM index. Defaults to None.
     :type vm_index: int, optional
     :param vm_name: VM name. Defaults to None.
@@ -544,15 +544,15 @@
 
 
 def create_app_shortcut_vm(
     self: "PyMemuc",
     package_name: str,
     vm_index: Union[int, None] = None,
     vm_name: Union[str, None] = None,
-) -> tuple[int, str]:
+) -> Tuple[int, str]:
     """Create an app shortcut on a VM, must specify either a vm index or a vm name
 
     :param package_name: Package name
     :type package_name: str
     :param vm_index: VM index. Defaults to None.
     :type vm_index: int, optional
     :param vm_name: VM name. Defaults to None.
```

### Comparing `pymemuc-0.2.6/pymemuc/_control.py` & `pymemuc-0.2.7/pymemuc/_control.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.2.6/pymemuc/_decorators.py` & `pymemuc-0.2.7/pymemuc/_decorators.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.2.6/pymemuc/_manage.py` & `pymemuc-0.2.7/pymemuc/_manage.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.2.6/pymemuc/_memuc.py` & `pymemuc-0.2.7/pymemuc/_memuc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """This module contains functions for directly interacting with memuc.exe."""
 from contextlib import suppress
 from os.path import join, normpath
 from subprocess import PIPE, STDOUT, CalledProcessError, Popen, TimeoutExpired
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Tuple
 
 from ._constants import WIN32, WINREG_EN
 from .exceptions import PyMemucError, PyMemucException, PyMemucTimeoutExpired
 
 if WINREG_EN:
+    # pylint: disable=import-error
     from winreg import HKEY_LOCAL_MACHINE, ConnectRegistry, OpenKey, QueryValueEx
 
 if WIN32:
     from subprocess import STARTF_USESHOWWINDOW, STARTUPINFO, SW_HIDE
 
     ST_INFO = STARTUPINFO()
     ST_INFO.dwFlags = STARTF_USESHOWWINDOW
@@ -41,15 +42,15 @@
             akey = OpenKey(ConnectRegistry(None, HKEY_LOCAL_MACHINE), key)
             return str(join(normpath(QueryValueEx(akey, "InstallLocation")[0]), "Memu"))
     raise PyMemucError("MEmuc not found, is it installed?")
 
 
 def memuc_run(
     self: "PyMemuc", args: list[str], non_blocking=False, timeout=None
-) -> tuple[int, str]:
+) -> Tuple[int, str]:
     """run a command with memuc.exe.
     Memuc can support non-blocking commands, returning a task id.
     A timeout can be specified if memuc is expected to hang,
     but this will not work with non-blocking commands.
 
     :param args: a list of arguments to pass to memuc.exe
     :type args: list[str]
@@ -93,15 +94,15 @@
                         print(f"\t\t{line}")
             return (0, result)
     except CalledProcessError as err:
         raise PyMemucError(err) from err
 
 
 # TODO: add output parsing
-def check_task_status(self: "PyMemuc", task_id: str) -> tuple[int, str]:
+def check_task_status(self: "PyMemuc", task_id: str) -> Tuple[int, str]:
     """Check the status of a task
 
     :param task_id: Asynchronous task ID
     :type task_id: str
     :return: the return code and the output of the command.
     :rtype: tuple[int, str]
     """
```

### Comparing `pymemuc-0.2.6/pymemuc/exceptions.py` & `pymemuc-0.2.7/pymemuc/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.2.6/pymemuc/pymemuc.py` & `pymemuc-0.2.7/pymemuc/pymemuc.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.2.6/pyproject.toml` & `pymemuc-0.2.7/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pymemuc"
-version = "v0.2.6"
+version = "v0.2.7"
 description = "A Memuc.exe wrapper for Python"
 readme = "README.md"
 authors = ["Martin Miglio <code@martinmiglio.dev>"]
 license = "MIT"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 keywords = ["memu", "memuc", "wrapper", "api"]
-repository = "https://github.com/marmig0404/pymemuc"
+repository = "https://github.com/martinmiglio/pymemuc"
 documentation = "https://pymemuc.readthedocs.io/"
 
 
 [tool.poetry.dependencies]
 python = "^3.9"
 
 
@@ -28,15 +28,15 @@
 pre-commit = "^3.2.1"
 black = "^23.1.0"
 prospector = "^1.9.0"
 ipykernel = "^6.22.0"
 
 
 [tool.poetry.group.docs.dependencies]
-sphinx = "^6.1.3"
+sphinx = ">=6.1.3,<8.0.0"
 sphinxext-opengraph = "^0.8.1"
 sphinx-autobuild = "^2021.3.14"
 sphinx-copybutton = "^0.5.1"
 furo = "^2023.3.27"
 sphinx-intl = "^2.1.0"
```

### Comparing `pymemuc-0.2.6/PKG-INFO` & `pymemuc-0.2.7/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: pymemuc
-Version: 0.2.6
+Version: 0.2.7
 Summary: A Memuc.exe wrapper for Python
-Home-page: https://github.com/marmig0404/pymemuc
+Home-page: https://github.com/martinmiglio/pymemuc
 License: MIT
 Keywords: memu,memuc,wrapper,api
 Author: Martin Miglio
 Author-email: code@martinmiglio.dev
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Project-URL: Documentation, https://pymemuc.readthedocs.io/
-Project-URL: Repository, https://github.com/marmig0404/pymemuc
+Project-URL: Repository, https://github.com/martinmiglio/pymemuc
 Description-Content-Type: text/markdown
 
 # pymemuc
 
-[![GitHub](https://img.shields.io/github/license/marmig0404/pymemuc)](LICENSE) [![Documentation Status](https://readthedocs.org/projects/pymemuc/badge/?version=latest)][full_doc] [![PyPI](https://img.shields.io/pypi/v/pymemuc) ![PyPI - Downloads](https://img.shields.io/pypi/dm/pymemuc)][pypi_link] [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pymemuc)][python_link] [![CodeFactor](https://www.codefactor.io/repository/github/marmig0404/pymemuc/badge)][codefactor_link]
+[![GitHub](https://img.shields.io/github/license/martinmiglio/pymemuc)](LICENSE) [![Documentation Status](https://readthedocs.org/projects/pymemuc/badge/?version=latest)][full_doc] [![PyPI](https://img.shields.io/pypi/v/pymemuc) ![PyPI - Downloads](https://img.shields.io/pypi/dm/pymemuc)][pypi_link] [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pymemuc)][python_link] [![CodeFactor](https://www.codefactor.io/repository/github/martinmiglio/pymemuc/badge)][codefactor_link]
 
 A wrapper for [MEmu Command (MEMUC)][memuc_docs] in python.
 
 Allows for easy interaction with MEmu VMs, including VM image management, VM control, running VM commands and ADB interaction.
 
 ## Installation
 
@@ -60,12 +59,12 @@
 
 ## Documentation
 
 See the [API documentation][full_doc].
 
 [python_link]: https://www.python.org/
 [pypi_link]: https://pypi.org/project/pymemuc/
-[codefactor_link]: https://www.codefactor.io/repository/github/marmig0404/pymemuc
+[codefactor_link]: https://www.codefactor.io/repository/github/martinmiglio/pymemuc
 [memuc_docs]: https://www.memuplay.com/blog/memucommand-reference-manual.html
 [demo_notebook]: demo/demo.ipynb
 [full_doc]: https://pymemuc.martinmiglio.dev/
```

