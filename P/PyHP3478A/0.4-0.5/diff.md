# Comparing `tmp/PyHP3478A-0.4.tar.gz` & `tmp/PyHP3478A-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyHP3478A-0.4.tar", last modified: Tue May 23 22:42:00 2023, max compression
+gzip compressed data, was "PyHP3478A-0.5.tar", last modified: Wed May 24 13:25:27 2023, max compression
```

## Comparing `PyHP3478A-0.4.tar` & `PyHP3478A-0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 22:42:00.690962 PyHP3478A-0.4/
--rw-rw-rw-   0        0        0     1091 2023-01-16 20:41:41.000000 PyHP3478A-0.4/LICENSE
--rw-rw-rw-   0        0        0      335 2023-05-23 22:42:00.690962 PyHP3478A-0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-23 22:42:00.675957 PyHP3478A-0.4/PyHP3478A/
--rw-rw-rw-   0        0        0     6932 2023-05-03 19:05:17.000000 PyHP3478A-0.4/PyHP3478A/HP3478A.py
--rw-rw-rw-   0        0        0       28 2023-05-03 19:05:17.000000 PyHP3478A-0.4/PyHP3478A/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 22:42:00.689961 PyHP3478A-0.4/PyHP3478A.egg-info/
--rw-rw-rw-   0        0        0      335 2023-05-23 22:42:00.000000 PyHP3478A-0.4/PyHP3478A.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-05-23 22:42:00.000000 PyHP3478A-0.4/PyHP3478A.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 22:42:00.000000 PyHP3478A-0.4/PyHP3478A.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-23 22:42:00.000000 PyHP3478A-0.4/PyHP3478A.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-23 22:42:00.000000 PyHP3478A-0.4/PyHP3478A.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      128 2023-05-03 19:14:02.000000 PyHP3478A-0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-05-23 22:42:00.690962 PyHP3478A-0.4/setup.cfg
--rw-rw-rw-   0        0        0      886 2023-05-23 22:41:36.000000 PyHP3478A-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 13:25:27.704304 PyHP3478A-0.5/
+-rw-rw-rw-   0        0        0     1091 2023-01-16 20:41:41.000000 PyHP3478A-0.5/LICENSE
+-rw-rw-rw-   0        0        0      335 2023-05-24 13:25:27.702302 PyHP3478A-0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-24 13:25:27.671300 PyHP3478A-0.5/PyHP3478A/
+-rw-rw-rw-   0        0        0     7092 2023-05-24 13:25:14.000000 PyHP3478A-0.5/PyHP3478A/HP3478A.py
+-rw-rw-rw-   0        0        0       28 2023-05-03 19:05:17.000000 PyHP3478A-0.5/PyHP3478A/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 13:25:27.698304 PyHP3478A-0.5/PyHP3478A.egg-info/
+-rw-rw-rw-   0        0        0      335 2023-05-24 13:25:27.000000 PyHP3478A-0.5/PyHP3478A.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-05-24 13:25:27.000000 PyHP3478A-0.5/PyHP3478A.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 13:25:27.000000 PyHP3478A-0.5/PyHP3478A.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-24 13:25:27.000000 PyHP3478A-0.5/PyHP3478A.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-24 13:25:27.000000 PyHP3478A-0.5/PyHP3478A.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      128 2023-05-03 19:14:02.000000 PyHP3478A-0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-24 13:25:27.704304 PyHP3478A-0.5/setup.cfg
+-rw-rw-rw-   0        0        0      935 2023-05-24 13:19:54.000000 PyHP3478A-0.5/setup.py
```

### Comparing `PyHP3478A-0.4/LICENSE` & `PyHP3478A-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `PyHP3478A-0.4/PyHP3478A/HP3478A.py` & `PyHP3478A-0.5/PyHP3478A/HP3478A.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 class HP3478A:
     """HP3478A made simple with Python and the AR488 project!
     use the PyAR488 module to comunicate with the AR488 board and make you lab bench smart
     -> written by Minu"""
     from PyAR488 import AR488
+    from time import sleep
 
     class Exceptions:
         class StatusByteException(Exception):
             def __init__(self) -> None:
                 super().__init__('error reading instrument status byte')
         class InvalidDigits(Exception):
             def __init__(self) -> None:
@@ -124,17 +125,19 @@
             response = int(response)
         except ValueError:
             raise self.Exceptions.StatusByteException()
         
         return self.StatusByte(response)
     
     def measure(self, new_measurement:Measure._MeasurementFunction, send:bool = True):
+        """set measurement with meter.measure(meter.Measurements.x) where x can be I_DC, V_AC ecc..."""
         command_string = new_measurement.code
         if send:
             self._write(command_string)
+            self.sleep(1)
         return command_string
     
     def trigger(self, new_trigger:Trigger._TriggerFunction, send:bool = True):
         command_string = new_trigger.code
         if send:
             self._write(command_string)
         return command_string
```

### Comparing `PyHP3478A-0.4/setup.py` & `PyHP3478A-0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 
 setup(
     name=project_name,
     version=local_build_version,
     packages=find_packages(exclude=('_INTERNAL_build.py',
                                     '_INTERNAL_version.json',
                                     '.gitignore',
-                                    'workspace.code-workspace')),
+                                    'workspace.code-workspace',
+                                    'tests.py')),
     url=f"https://github.com/Minu-IU3IRR/{project_name}",
     bugtrack_url = f'https://github.com/Minu-IU3IRR/{project_name}/issues',
     license='MIT',
     author='Manuel Minutello',
     description='HP3478A python interface',
     long_description=open('README.md').read(),
     install_requires=['PyAR488'],
```

