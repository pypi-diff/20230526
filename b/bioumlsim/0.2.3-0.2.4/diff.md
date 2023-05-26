# Comparing `tmp/bioumlsim-0.2.3.tar.gz` & `tmp/bioumlsim-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioumlsim-0.2.3.tar", last modified: Thu May 18 18:58:02 2023, max compression
+gzip compressed data, was "bioumlsim-0.2.4.tar", last modified: Fri May 26 10:53:54 2023, max compression
```

## Comparing `bioumlsim-0.2.3.tar` & `bioumlsim-0.2.4.tar`

### file list

```diff
@@ -1,17 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 18:58:02.903016 bioumlsim-0.2.3/
--rw-rw-rw-   0        0        0     1088 2023-05-17 07:27:39.000000 bioumlsim-0.2.3/LICENSE
--rw-rw-rw-   0        0        0      771 2023-05-18 18:58:02.904016 bioumlsim-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0       60 2023-05-17 07:27:39.000000 bioumlsim-0.2.3/README.md
--rw-rw-rw-   0        0        0      185 2023-05-17 10:21:02.000000 bioumlsim-0.2.3/pyproject.toml
--rw-rw-rw-   0        0        0      798 2023-05-18 18:58:02.910015 bioumlsim-0.2.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-18 18:58:02.855019 bioumlsim-0.2.3/src/
--rw-rw-rw-   0        0        0        0 2023-05-17 07:30:52.000000 bioumlsim-0.2.3/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 18:58:02.902015 bioumlsim-0.2.3/src/bioumlsim.egg-info/
--rw-rw-rw-   0        0        0      771 2023-05-18 18:58:02.000000 bioumlsim-0.2.3/src/bioumlsim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-05-18 18:58:02.000000 bioumlsim-0.2.3/src/bioumlsim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 18:58:02.000000 bioumlsim-0.2.3/src/bioumlsim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-17 10:19:31.000000 bioumlsim-0.2.3/src/bioumlsim.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       20 2023-05-18 18:58:02.000000 bioumlsim-0.2.3/src/bioumlsim.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-05-18 18:58:02.000000 bioumlsim-0.2.3/src/bioumlsim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3469 2023-05-18 18:55:37.000000 bioumlsim-0.2.3/src/bioumlsim.py
--rw-rw-rw-   0        0        0      388 2023-05-18 18:51:14.000000 bioumlsim-0.2.3/src/test.py
+drwxrwxrwx   0        0        0        0 2023-05-26 10:53:54.301473 bioumlsim-0.2.4/
+-rw-rw-rw-   0        0        0     1088 2023-05-17 07:27:39.000000 bioumlsim-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0       18 2023-05-26 09:58:37.000000 bioumlsim-0.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      771 2023-05-26 10:53:54.302476 bioumlsim-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0       60 2023-05-17 07:27:39.000000 bioumlsim-0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 10:53:54.266592 bioumlsim-0.2.4/java/
+-rw-rw-rw-   0        0        0   386547 2023-05-26 08:30:49.000000 bioumlsim-0.2.4/java/biouml.plugins.sbml_0.9.10.jar
+-rw-rw-rw-   0        0        0   615951 2023-05-26 08:30:49.000000 bioumlsim-0.2.4/java/biouml.plugins.simulation_0.9.10.jar
+-rw-rw-rw-   0        0        0  2085692 2023-05-26 08:30:49.000000 bioumlsim-0.2.4/java/biouml.workbench_0.9.10.jar
+-rw-rw-rw-   0        0        0   581945 2023-05-26 08:30:49.000000 bioumlsim-0.2.4/java/colt.jar
+-rw-rw-rw-   0        0        0   396595 2023-05-26 08:30:49.000000 bioumlsim-0.2.4/java/com.developmentontheedge.beans-3.0.4.jar
+-rw-rw-rw-   0        0        0    94331 2023-05-26 08:30:48.000000 bioumlsim-0.2.4/java/com.developmentontheedge.util_0.9.10.jar
+-rw-rw-rw-   0        0        0    31222 2023-05-26 08:30:49.000000 bioumlsim-0.2.4/java/com.eclipsesource.json_0.9.4.jar
+-rw-rw-rw-   0        0        0   575606 2023-05-26 08:30:49.000000 bioumlsim-0.2.4/java/org.apache.commons.collections_3.2.1.jar
+-rw-rw-rw-   0        0        0   262026 2023-05-26 08:30:48.000000 bioumlsim-0.2.4/java/org.apache.commons.lang_2.4.0.jar
+-rw-rw-rw-   0        0        0   421287 2023-05-26 08:30:49.000000 bioumlsim-0.2.4/java/org.apache.velocity_1.6.2.jar
+-rw-rw-rw-   0        0        0    58013 2023-05-26 08:30:48.000000 bioumlsim-0.2.4/java/org.json-20170516.jar
+-rw-rw-rw-   0        0        0  1251757 2023-05-26 08:30:49.000000 bioumlsim-0.2.4/java/ru.biosoft.access_0.9.10.jar
+-rw-rw-rw-   0        0        0    14541 2023-05-26 08:30:49.000000 bioumlsim-0.2.4/java/ru.biosoft.exception-1.0.0.jar
+-rw-rw-rw-   0        0        0   231950 2023-05-26 08:30:48.000000 bioumlsim-0.2.4/java/ru.biosoft.graph_0.9.10.jar
+-rw-rw-rw-   0        0        0   197773 2023-05-26 08:30:48.000000 bioumlsim-0.2.4/java/ru.biosoft.graphics_0.9.10.jar
+-rw-rw-rw-   0        0        0    26578 2023-05-26 08:30:49.000000 bioumlsim-0.2.4/java/ru.biosoft.jobcontrol-2.0.0.jar
+-rw-rw-rw-   0        0        0   163699 2023-05-26 08:30:48.000000 bioumlsim-0.2.4/java/ru.biosoft.math_0.9.10.jar
+-rw-rw-rw-   0        0        0    20343 2023-05-26 08:30:49.000000 bioumlsim-0.2.4/java/src.jar
+-rw-rw-rw-   0        0        0   299064 2023-05-26 08:30:49.000000 bioumlsim-0.2.4/java/streamex-0.7.0.jar
+-rw-rw-rw-   0        0        0      185 2023-05-17 10:21:02.000000 bioumlsim-0.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0       55 2023-05-17 13:19:23.000000 bioumlsim-0.2.4/requirements_dev.txt
+-rw-rw-rw-   0        0        0      827 2023-05-26 10:53:54.314716 bioumlsim-0.2.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-26 10:53:54.272593 bioumlsim-0.2.4/src/
+-rw-rw-rw-   0        0        0        0 2023-05-17 07:30:52.000000 bioumlsim-0.2.4/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 10:53:54.300477 bioumlsim-0.2.4/src/bioumlsim.egg-info/
+-rw-rw-rw-   0        0        0      771 2023-05-26 10:53:54.000000 bioumlsim-0.2.4/src/bioumlsim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      996 2023-05-26 10:53:54.000000 bioumlsim-0.2.4/src/bioumlsim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 10:53:54.000000 bioumlsim-0.2.4/src/bioumlsim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-17 10:19:31.000000 bioumlsim-0.2.4/src/bioumlsim.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       20 2023-05-26 10:53:54.000000 bioumlsim-0.2.4/src/bioumlsim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-05-26 10:53:54.000000 bioumlsim-0.2.4/src/bioumlsim.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2909 2023-05-26 08:34:47.000000 bioumlsim-0.2.4/src/bioumlsim.py
+-rw-rw-rw-   0        0        0      390 2023-05-22 19:11:01.000000 bioumlsim-0.2.4/src/test.py
+-rw-rw-rw-   0        0        0        3 2023-05-26 09:41:30.000000 bioumlsim-0.2.4/text.txt
```

### Comparing `bioumlsim-0.2.3/LICENSE` & `bioumlsim-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.2.3/PKG-INFO` & `bioumlsim-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioumlsim
-Version: 0.2.3
+Version: 0.2.4
 Summary: Python interface for simulation with BioUML
 Home-page: https://www.biouml.org/
 Author: Ilya Kiselev, Biosoft.ru
 Author-email: 4x3cut0r@gmail.com
 Project-URL: Bug Tracker, https://github.com/Biosoft-ru/bioumlsim/issues
 Project-URL: Source Code, https://github.com/Biosoft-ru/bioumlsim
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bioumlsim-0.2.3/src/bioumlsim.egg-info/PKG-INFO` & `bioumlsim-0.2.4/src/bioumlsim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioumlsim
-Version: 0.2.3
+Version: 0.2.4
 Summary: Python interface for simulation with BioUML
 Home-page: https://www.biouml.org/
 Author: Ilya Kiselev, Biosoft.ru
 Author-email: 4x3cut0r@gmail.com
 Project-URL: Bug Tracker, https://github.com/Biosoft-ru/bioumlsim/issues
 Project-URL: Source Code, https://github.com/Biosoft-ru/bioumlsim
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bioumlsim-0.2.3/src/bioumlsim.py` & `bioumlsim-0.2.4/src/bioumlsim.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,50 +1,39 @@
 import jpype
 import jpype.imports
 import numpy
+import os
 
 class BioUMLSim:
     
     bioUMLPath = None
     atol = 1E-8
     rtol = 1E-8
     engine = None
-    
-    def __init__(self, path = 'C:/BioUML_2023.1'):
-        """
-        Code copied from runJVM method
-        """
-        self.bioUMLPath = path
-        print("JVM is starting up")
-        jpype.startJVM(classpath=[self.bioUMLPath+'/plugins/*',self.bioUMLPath+'/plugins/cern.jet.random_1.3.0/colt.jar'], convertStrings=True)
- 
-    def runJVM(path):
-        """
-        Starts up Java Virtual Machine and adds all BioUML jars to classpath 
-        Args:
-            path (str): path to BioUML installation
-        """
+
+    def __init__(self, path = 'C:/lib'):
         self.bioUMLPath = path
         print("JVM is starting up")
-        jpype.startJVM(classpath=[self.bioUMLPath+'/plugins/*',self.bioUMLPath+'/plugins/cern.jet.random_1.3.0/colt.jar'])
-       
+        jpype.startJVM(classpath=[path+'/*'], convertStrings=True)
+        path = os.path.abspath(__file__)
+        print(path)
+        
     def load(self, file):
         """
         Loads SBML file and transforms it into object which represents mathematical model.
         Args:
             file (str): path to file
         Returns:
             model
         """
         print(f"SBML file is loading: {file}.")
-        diagram = jpype.JClass("biouml.plugins.sbml.SbmlModelFactory").readDiagram(file)
+        diagram = jpype.JClass("biouml.plugins.sbml.SbmlModelFactory").readDiagram(file, False)
         self.engine = jpype.JClass("biouml.plugins.simulation.java.JavaSimulationEngine")()
         self.engine.setDiagram(diagram)
-        self.engine.setClassPath(self.bioUMLPath +'/plugins/biouml.plugins.simulation/src.jar')
-        self.engine.setOutputDir(self.bioUMLPath+'/temp')
+        self.engine.setClassPath(self.bioUMLPath +'/src.jar')
         self.engine.disableLog()
         self.engine.setAbsTolerance(self.atol)
         self.engine.setRelTolerance(self.rtol)
         return Model(self.engine, self.engine.createModel())
     
 class Model:
```

