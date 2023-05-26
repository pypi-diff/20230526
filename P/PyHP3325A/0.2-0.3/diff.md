# Comparing `tmp/PyHP3325A-0.2.tar.gz` & `tmp/PyHP3325A-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyHP3325A-0.2.tar", last modified: Tue May 23 22:44:38 2023, max compression
+gzip compressed data, was "PyHP3325A-0.3.tar", last modified: Wed May 24 13:30:34 2023, max compression
```

## Comparing `PyHP3325A-0.2.tar` & `PyHP3325A-0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 22:44:38.682266 PyHP3325A-0.2/
--rw-rw-rw-   0        0        0     1091 2023-01-16 20:41:41.000000 PyHP3325A-0.2/LICENSE
--rw-rw-rw-   0        0        0      335 2023-05-23 22:44:38.682266 PyHP3325A-0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-23 22:44:38.668264 PyHP3325A-0.2/PyHP3325A/
--rw-rw-rw-   0        0        0     7827 2023-05-23 10:07:19.000000 PyHP3325A-0.2/PyHP3325A/HP3325A.py
--rw-rw-rw-   0        0        0       28 2023-05-23 09:12:55.000000 PyHP3325A-0.2/PyHP3325A/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 22:44:38.681266 PyHP3325A-0.2/PyHP3325A.egg-info/
--rw-rw-rw-   0        0        0      335 2023-05-23 22:44:38.000000 PyHP3325A-0.2/PyHP3325A.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-05-23 22:44:38.000000 PyHP3325A-0.2/PyHP3325A.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 22:44:38.000000 PyHP3325A-0.2/PyHP3325A.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-23 22:44:38.000000 PyHP3325A-0.2/PyHP3325A.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-23 22:44:38.000000 PyHP3325A-0.2/PyHP3325A.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      128 2023-05-23 08:52:04.000000 PyHP3325A-0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-23 22:44:38.683267 PyHP3325A-0.2/setup.cfg
--rw-rw-rw-   0        0        0      886 2023-05-23 22:44:30.000000 PyHP3325A-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 13:30:34.110942 PyHP3325A-0.3/
+-rw-rw-rw-   0        0        0     1091 2023-01-16 20:41:41.000000 PyHP3325A-0.3/LICENSE
+-rw-rw-rw-   0        0        0      335 2023-05-24 13:30:34.109942 PyHP3325A-0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-24 13:30:34.083941 PyHP3325A-0.3/PyHP3325A/
+-rw-rw-rw-   0        0        0     7827 2023-05-24 13:29:51.000000 PyHP3325A-0.3/PyHP3325A/HP3325A.py
+-rw-rw-rw-   0        0        0       28 2023-05-23 09:12:55.000000 PyHP3325A-0.3/PyHP3325A/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 13:30:34.105945 PyHP3325A-0.3/PyHP3325A.egg-info/
+-rw-rw-rw-   0        0        0      335 2023-05-24 13:30:33.000000 PyHP3325A-0.3/PyHP3325A.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-05-24 13:30:33.000000 PyHP3325A-0.3/PyHP3325A.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 13:30:33.000000 PyHP3325A-0.3/PyHP3325A.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-24 13:30:33.000000 PyHP3325A-0.3/PyHP3325A.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-24 13:30:33.000000 PyHP3325A-0.3/PyHP3325A.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      128 2023-05-23 08:52:04.000000 PyHP3325A-0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-24 13:30:34.111943 PyHP3325A-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      934 2023-05-24 13:27:18.000000 PyHP3325A-0.3/setup.py
```

### Comparing `PyHP3325A-0.2/LICENSE` & `PyHP3325A-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PyHP3325A-0.2/PyHP3325A/HP3325A.py` & `PyHP3325A-0.3/PyHP3325A/HP3325A.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,17 +46,17 @@
     class Units:
         class Amplitude:
             class _U:
                 def __init__(self, command: str) -> None:
                     self.command = command
             Vp = _U('VO')
             mV = _U('MV')
-            Vrms: _U('VR')
-            mVrms: _U('MR')
-            dBm: _U('DB')
+            Vrms= _U('VR')
+            mVrms= _U('MR')
+            dBm= _U('DB')
 
         class Offset:
             class _U:
                 def __init__(self, command: str) -> None:
                     self.command = command
             Vp = _U('VO')
             mV = _U('MV')
```

### Comparing `PyHP3325A-0.2/setup.py` & `PyHP3325A-0.3/setup.py`

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
+                                    'workspace.code-workspace'
+                                    'tests.py')),
     url=f"https://github.com/Minu-IU3IRR/{project_name}",
     bugtrack_url = f'https://github.com/Minu-IU3IRR/{project_name}/issues',
     license='MIT',
     author='Manuel Minutello',
     description='HP3478A python interface',
     long_description=open('README.md').read(),
     install_requires=['PyAR488'],
```

