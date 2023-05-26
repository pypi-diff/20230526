# Comparing `tmp/Qsim_trapped_ions-1.0.4.tar.gz` & `tmp/Qsim_trapped_ions-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Qsim_trapped_ions-1.0.4.tar", last modified: Fri May 26 06:12:07 2023, max compression
+gzip compressed data, was "Qsim_trapped_ions-1.0.5.tar", last modified: Fri May 26 06:23:30 2023, max compression
```

## Comparing `Qsim_trapped_ions-1.0.4.tar` & `Qsim_trapped_ions-1.0.5.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 06:12:07.780077 Qsim_trapped_ions-1.0.4/
--rw-rw-rw-   0        0        0     4294 2023-05-26 06:12:07.779072 Qsim_trapped_ions-1.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-26 06:12:07.737583 Qsim_trapped_ions-1.0.4/Qsim/
-drwxrwxrwx   0        0        0        0 2023-05-26 06:12:07.741596 Qsim_trapped_ions-1.0.4/Qsim/ion_chain/
--rw-rw-rw-   0        0        0      131 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.4/Qsim/ion_chain/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 06:12:07.744907 Qsim_trapped_ions-1.0.4/Qsim/ion_chain/eigendiagram/
--rw-rw-rw-   0        0        0     7825 2023-04-22 20:45:12.000000 Qsim_trapped_ions-1.0.4/Qsim/ion_chain/eigendiagram/exci_diagram.py
--rw-rw-rw-   0        0        0      111 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.4/Qsim/ion_chain/eigendiagram/init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 06:12:07.749440 Qsim_trapped_ions-1.0.4/Qsim/ion_chain/interaction/
--rw-rw-rw-   0        0        0      131 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.4/Qsim/ion_chain/interaction/__init__.py
--rw-rw-rw-   0        0        0     2853 2023-03-27 05:10:36.000000 Qsim_trapped_ions-1.0.4/Qsim/ion_chain/interaction/pure_spin.py
--rw-rw-rw-   0        0        0     7440 2023-02-19 21:26:44.000000 Qsim_trapped_ions-1.0.4/Qsim/ion_chain/interaction/spin_phonon.py
--rw-rw-rw-   0        0        0    30412 2023-05-26 06:01:34.000000 Qsim_trapped_ions-1.0.4/Qsim/ion_chain/ion_system.py
-drwxrwxrwx   0        0        0        0 2023-05-26 06:12:07.753600 Qsim_trapped_ions-1.0.4/Qsim/ion_chain/ising/
--rw-rw-rw-   0        0        0      131 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.4/Qsim/ion_chain/ising/__init__.py
--rw-rw-rw-   0        0        0     1569 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.4/Qsim/ion_chain/ising/ising_c.py
--rw-rw-rw-   0        0        0     4045 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.4/Qsim/ion_chain/ising/ising_ps.py
-drwxrwxrwx   0        0        0        0 2023-05-26 06:12:07.765197 Qsim_trapped_ions-1.0.4/Qsim/ion_chain/transfer/
--rw-rw-rw-   0        0        0      131 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.4/Qsim/ion_chain/transfer/__init__.py
--rw-rw-rw-   0        0        0    15712 2023-03-07 21:30:48.000000 Qsim_trapped_ions-1.0.4/Qsim/ion_chain/transfer/anharmonic_transfer - 副本.py
--rw-rw-rw-   0        0        0    15800 2023-03-08 00:56:56.000000 Qsim_trapped_ions-1.0.4/Qsim/ion_chain/transfer/anharmonic_transfer.py
--rw-rw-rw-   0        0        0     3037 2023-02-20 05:11:39.000000 Qsim_trapped_ions-1.0.4/Qsim/ion_chain/transfer/chaos.py
--rw-rw-rw-   0        0        0     3063 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.4/Qsim/ion_chain/transfer/elec_transfer.py
--rw-rw-rw-   0        0        0    13991 2023-03-05 19:12:10.000000 Qsim_trapped_ions-1.0.4/Qsim/ion_chain/transfer/exci_operators.py
--rw-rw-rw-   0        0        0     4323 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.4/Qsim/ion_chain/transfer/exci_transfer.py
--rw-rw-rw-   0        0        0     5700 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.4/Qsim/ion_chain/transfer/multi_core.py
-drwxrwxrwx   0        0        0        0 2023-05-26 06:12:07.768714 Qsim_trapped_ions-1.0.4/Qsim/operator/
--rw-rw-rw-   0        0        0      131 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.4/Qsim/operator/__init__.py
--rw-rw-rw-   0        0        0     7121 2023-03-05 17:06:10.000000 Qsim_trapped_ions-1.0.4/Qsim/operator/phonon.py
--rw-rw-rw-   0        0        0     6429 2023-02-27 23:34:30.000000 Qsim_trapped_ions-1.0.4/Qsim/operator/spin.py
-drwxrwxrwx   0        0        0        0 2023-05-26 06:12:07.776047 Qsim_trapped_ions-1.0.4/Qsim_trapped_ions.egg-info/
--rw-rw-rw-   0        0        0     4294 2023-05-26 06:12:07.000000 Qsim_trapped_ions-1.0.4/Qsim_trapped_ions.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      988 2023-05-26 06:12:07.000000 Qsim_trapped_ions-1.0.4/Qsim_trapped_ions.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 06:12:07.000000 Qsim_trapped_ions-1.0.4/Qsim_trapped_ions.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-26 06:12:07.000000 Qsim_trapped_ions-1.0.4/Qsim_trapped_ions.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-26 06:12:07.000000 Qsim_trapped_ions-1.0.4/Qsim_trapped_ions.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-26 06:12:07.780077 Qsim_trapped_ions-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1207 2023-05-26 05:56:05.000000 Qsim_trapped_ions-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-26 06:12:07.778069 Qsim_trapped_ions-1.0.4/test/
--rw-rw-rw-   0        0        0      147 2023-05-26 03:52:59.000000 Qsim_trapped_ions-1.0.4/test/test.py
+drwxrwxrwx   0        0        0        0 2023-05-26 06:23:30.562648 Qsim_trapped_ions-1.0.5/
+-rw-rw-rw-   0        0        0     4294 2023-05-26 06:23:30.562648 Qsim_trapped_ions-1.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-26 06:23:30.516680 Qsim_trapped_ions-1.0.5/Qsim/
+drwxrwxrwx   0        0        0        0 2023-05-26 06:23:30.523463 Qsim_trapped_ions-1.0.5/Qsim/ion_chain/
+-rw-rw-rw-   0        0        0      131 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.5/Qsim/ion_chain/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 06:23:30.526745 Qsim_trapped_ions-1.0.5/Qsim/ion_chain/eigendiagram/
+-rw-rw-rw-   0        0        0     7825 2023-04-22 20:45:12.000000 Qsim_trapped_ions-1.0.5/Qsim/ion_chain/eigendiagram/exci_diagram.py
+-rw-rw-rw-   0        0        0      111 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.5/Qsim/ion_chain/eigendiagram/init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 06:23:30.531099 Qsim_trapped_ions-1.0.5/Qsim/ion_chain/interaction/
+-rw-rw-rw-   0        0        0      131 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.5/Qsim/ion_chain/interaction/__init__.py
+-rw-rw-rw-   0        0        0     2853 2023-03-27 05:10:36.000000 Qsim_trapped_ions-1.0.5/Qsim/ion_chain/interaction/pure_spin.py
+-rw-rw-rw-   0        0        0     7440 2023-02-19 21:26:44.000000 Qsim_trapped_ions-1.0.5/Qsim/ion_chain/interaction/spin_phonon.py
+-rw-rw-rw-   0        0        0    30412 2023-05-26 06:01:34.000000 Qsim_trapped_ions-1.0.5/Qsim/ion_chain/ion_system.py
+drwxrwxrwx   0        0        0        0 2023-05-26 06:23:30.535031 Qsim_trapped_ions-1.0.5/Qsim/ion_chain/ising/
+-rw-rw-rw-   0        0        0      131 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.5/Qsim/ion_chain/ising/__init__.py
+-rw-rw-rw-   0        0        0     1569 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.5/Qsim/ion_chain/ising/ising_c.py
+-rw-rw-rw-   0        0        0     4045 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.5/Qsim/ion_chain/ising/ising_ps.py
+drwxrwxrwx   0        0        0        0 2023-05-26 06:23:30.547958 Qsim_trapped_ions-1.0.5/Qsim/ion_chain/transfer/
+-rw-rw-rw-   0        0        0      131 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.5/Qsim/ion_chain/transfer/__init__.py
+-rw-rw-rw-   0        0        0    15712 2023-03-07 21:30:48.000000 Qsim_trapped_ions-1.0.5/Qsim/ion_chain/transfer/anharmonic_transfer - 副本.py
+-rw-rw-rw-   0        0        0    15800 2023-03-08 00:56:56.000000 Qsim_trapped_ions-1.0.5/Qsim/ion_chain/transfer/anharmonic_transfer.py
+-rw-rw-rw-   0        0        0     3037 2023-02-20 05:11:39.000000 Qsim_trapped_ions-1.0.5/Qsim/ion_chain/transfer/chaos.py
+-rw-rw-rw-   0        0        0     3063 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.5/Qsim/ion_chain/transfer/elec_transfer.py
+-rw-rw-rw-   0        0        0    13991 2023-03-05 19:12:10.000000 Qsim_trapped_ions-1.0.5/Qsim/ion_chain/transfer/exci_operators.py
+-rw-rw-rw-   0        0        0     4323 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.5/Qsim/ion_chain/transfer/exci_transfer.py
+-rw-rw-rw-   0        0        0     5700 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.5/Qsim/ion_chain/transfer/multi_core.py
+drwxrwxrwx   0        0        0        0 2023-05-26 06:23:30.551484 Qsim_trapped_ions-1.0.5/Qsim/operator/
+-rw-rw-rw-   0        0        0      131 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.5/Qsim/operator/__init__.py
+-rw-rw-rw-   0        0        0     7121 2023-03-05 17:06:10.000000 Qsim_trapped_ions-1.0.5/Qsim/operator/phonon.py
+-rw-rw-rw-   0        0        0     6429 2023-02-27 23:34:30.000000 Qsim_trapped_ions-1.0.5/Qsim/operator/spin.py
+drwxrwxrwx   0        0        0        0 2023-05-26 06:23:30.559288 Qsim_trapped_ions-1.0.5/Qsim_trapped_ions.egg-info/
+-rw-rw-rw-   0        0        0     4294 2023-05-26 06:23:30.000000 Qsim_trapped_ions-1.0.5/Qsim_trapped_ions.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      999 2023-05-26 06:23:30.000000 Qsim_trapped_ions-1.0.5/Qsim_trapped_ions.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 06:23:30.000000 Qsim_trapped_ions-1.0.5/Qsim_trapped_ions.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-26 06:23:30.000000 Qsim_trapped_ions-1.0.5/Qsim_trapped_ions.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-26 06:23:30.000000 Qsim_trapped_ions-1.0.5/Qsim_trapped_ions.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4035 2023-05-23 09:08:47.000000 Qsim_trapped_ions-1.0.5/README.rst
+-rw-rw-rw-   0        0        0       42 2023-05-26 06:23:30.562648 Qsim_trapped_ions-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1201 2023-05-26 06:23:11.000000 Qsim_trapped_ions-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 06:23:30.561640 Qsim_trapped_ions-1.0.5/test/
+-rw-rw-rw-   0        0        0      147 2023-05-26 03:52:59.000000 Qsim_trapped_ions-1.0.5/test/test.py
```

### Comparing `Qsim_trapped_ions-1.0.4/PKG-INFO` & `Qsim_trapped_ions-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Qsim_trapped_ions
-Version: 1.0.4
+Version: 1.0.5
 Summary: Numerical simulation of trapped ion quantum dynamics
 Home-page: https://github.com/TrappedIonRice/Open-Quantum-system-simulation
 Author: Mingjian Zhu
 Author-email: mz40@rice.edu
 
 # Open-Quantum-system-simulation
 package: ion_chain
```

### Comparing `Qsim_trapped_ions-1.0.4/Qsim/ion_chain/eigendiagram/exci_diagram.py` & `Qsim_trapped_ions-1.0.5/Qsim/ion_chain/eigendiagram/exci_diagram.py`

 * *Files identical despite different names*

### Comparing `Qsim_trapped_ions-1.0.4/Qsim/ion_chain/interaction/pure_spin.py` & `Qsim_trapped_ions-1.0.5/Qsim/ion_chain/interaction/pure_spin.py`

 * *Files identical despite different names*

### Comparing `Qsim_trapped_ions-1.0.4/Qsim/ion_chain/interaction/spin_phonon.py` & `Qsim_trapped_ions-1.0.5/Qsim/ion_chain/interaction/spin_phonon.py`

 * *Files identical despite different names*

### Comparing `Qsim_trapped_ions-1.0.4/Qsim/ion_chain/ion_system.py` & `Qsim_trapped_ions-1.0.5/Qsim/ion_chain/ion_system.py`

 * *Files identical despite different names*

### Comparing `Qsim_trapped_ions-1.0.4/Qsim/ion_chain/ising/ising_c.py` & `Qsim_trapped_ions-1.0.5/Qsim/ion_chain/ising/ising_c.py`

 * *Files identical despite different names*

### Comparing `Qsim_trapped_ions-1.0.4/Qsim/ion_chain/ising/ising_ps.py` & `Qsim_trapped_ions-1.0.5/Qsim/ion_chain/ising/ising_ps.py`

 * *Files identical despite different names*

### Comparing `Qsim_trapped_ions-1.0.4/Qsim/ion_chain/transfer/anharmonic_transfer - 副本.py` & `Qsim_trapped_ions-1.0.5/Qsim/ion_chain/transfer/anharmonic_transfer - 副本.py`

 * *Files identical despite different names*

### Comparing `Qsim_trapped_ions-1.0.4/Qsim/ion_chain/transfer/anharmonic_transfer.py` & `Qsim_trapped_ions-1.0.5/Qsim/ion_chain/transfer/anharmonic_transfer.py`

 * *Files identical despite different names*

### Comparing `Qsim_trapped_ions-1.0.4/Qsim/ion_chain/transfer/chaos.py` & `Qsim_trapped_ions-1.0.5/Qsim/ion_chain/transfer/chaos.py`

 * *Files identical despite different names*

### Comparing `Qsim_trapped_ions-1.0.4/Qsim/ion_chain/transfer/elec_transfer.py` & `Qsim_trapped_ions-1.0.5/Qsim/ion_chain/transfer/elec_transfer.py`

 * *Files identical despite different names*

### Comparing `Qsim_trapped_ions-1.0.4/Qsim/ion_chain/transfer/exci_operators.py` & `Qsim_trapped_ions-1.0.5/Qsim/ion_chain/transfer/exci_operators.py`

 * *Files identical despite different names*

### Comparing `Qsim_trapped_ions-1.0.4/Qsim/ion_chain/transfer/exci_transfer.py` & `Qsim_trapped_ions-1.0.5/Qsim/ion_chain/transfer/exci_transfer.py`

 * *Files identical despite different names*

### Comparing `Qsim_trapped_ions-1.0.4/Qsim/ion_chain/transfer/multi_core.py` & `Qsim_trapped_ions-1.0.5/Qsim/ion_chain/transfer/multi_core.py`

 * *Files identical despite different names*

### Comparing `Qsim_trapped_ions-1.0.4/Qsim/operator/phonon.py` & `Qsim_trapped_ions-1.0.5/Qsim/operator/phonon.py`

 * *Files identical despite different names*

### Comparing `Qsim_trapped_ions-1.0.4/Qsim/operator/spin.py` & `Qsim_trapped_ions-1.0.5/Qsim/operator/spin.py`

 * *Files identical despite different names*

### Comparing `Qsim_trapped_ions-1.0.4/Qsim_trapped_ions.egg-info/PKG-INFO` & `Qsim_trapped_ions-1.0.5/Qsim_trapped_ions.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Qsim-trapped-ions
-Version: 1.0.4
+Version: 1.0.5
 Summary: Numerical simulation of trapped ion quantum dynamics
 Home-page: https://github.com/TrappedIonRice/Open-Quantum-system-simulation
 Author: Mingjian Zhu
 Author-email: mz40@rice.edu
 
 # Open-Quantum-system-simulation
 package: ion_chain
```

### Comparing `Qsim_trapped_ions-1.0.4/Qsim_trapped_ions.egg-info/SOURCES.txt` & `Qsim_trapped_ions-1.0.5/Qsim_trapped_ions.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+README.rst
 setup.py
 Qsim/ion_chain/__init__.py
 Qsim/ion_chain/ion_system.py
 Qsim/ion_chain/eigendiagram/exci_diagram.py
 Qsim/ion_chain/eigendiagram/init__.py
 Qsim/ion_chain/interaction/__init__.py
 Qsim/ion_chain/interaction/pure_spin.py
```

### Comparing `Qsim_trapped_ions-1.0.4/setup.py` & `Qsim_trapped_ions-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 
 @author: zhumj
 """
 
 from setuptools import setup
 
 def readme_file():
-    with open(".\\Qsim\\README.rst") as rf:
+    with open(".\\README.rst") as rf:
         return rf.read()
     
 setup(name = 'Qsim_trapped_ions', 
-      version = '1.0.4', 
+      version = '1.0.5', 
       description = 'Numerical simulation of trapped ion quantum dynamics',
       package_dir = {
             'Qsim': 'Qsim',
             'Qsim.ion_chain': 'Qsim/ion_chain',
             'Qsim.operator': 'Qsim/operator',
             'Qsim.ion_chain.eigendiagram': 'Qsim/ion_chain/eigendiagram',
             'Qsim.ion_chain.interaction': 'Qsim/ion_chain/interaction',
```

