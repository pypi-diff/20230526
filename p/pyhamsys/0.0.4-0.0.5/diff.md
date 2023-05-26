# Comparing `tmp/pyhamsys-0.0.4.tar.gz` & `tmp/pyhamsys-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhamsys-0.0.4.tar", last modified: Fri May 26 10:26:24 2023, max compression
+gzip compressed data, was "pyhamsys-0.0.5.tar", last modified: Fri May 26 10:32:36 2023, max compression
```

## Comparing `pyhamsys-0.0.4.tar` & `pyhamsys-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 cchandre   (501) staff       (20)        0 2023-05-26 10:26:24.841128 pyhamsys-0.0.4/
--rw-r--r--   0 cchandre   (501) staff       (20)     1304 2023-04-05 14:49:59.000000 pyhamsys-0.0.4/LICENSE
--rw-r--r--   0 cchandre   (501) staff       (20)     5873 2023-05-26 10:26:24.840744 pyhamsys-0.0.4/PKG-INFO
--rw-r--r--   0 cchandre   (501) staff       (20)     5058 2023-05-19 14:15:47.000000 pyhamsys-0.0.4/README.md
-drwxr-xr-x   0 cchandre   (501) staff       (20)        0 2023-05-26 10:26:24.836509 pyhamsys-0.0.4/pyhamsys/
-drwxr-xr-x   0 cchandre   (501) staff       (20)        0 2023-05-26 10:26:24.837970 pyhamsys-0.0.4/pyhamsys/src/
-drwxr-xr-x   0 cchandre   (501) staff       (20)        0 2023-05-26 10:26:24.840311 pyhamsys-0.0.4/pyhamsys/src/pyhamsys.egg-info/
--rw-r--r--   0 cchandre   (501) staff       (20)     5873 2023-05-26 10:26:24.000000 pyhamsys-0.0.4/pyhamsys/src/pyhamsys.egg-info/PKG-INFO
--rw-r--r--   0 cchandre   (501) staff       (20)      275 2023-05-26 10:26:24.000000 pyhamsys-0.0.4/pyhamsys/src/pyhamsys.egg-info/SOURCES.txt
--rw-r--r--   0 cchandre   (501) staff       (20)        1 2023-05-26 10:26:24.000000 pyhamsys-0.0.4/pyhamsys/src/pyhamsys.egg-info/dependency_links.txt
--rw-r--r--   0 cchandre   (501) staff       (20)       12 2023-05-26 10:26:24.000000 pyhamsys-0.0.4/pyhamsys/src/pyhamsys.egg-info/requires.txt
--rw-r--r--   0 cchandre   (501) staff       (20)        9 2023-05-26 10:26:24.000000 pyhamsys-0.0.4/pyhamsys/src/pyhamsys.egg-info/top_level.txt
--rw-r--r--   0 cchandre   (501) staff       (20)    11819 2023-05-26 10:24:22.000000 pyhamsys-0.0.4/pyhamsys/src/pyhamsys.py
--rw-r--r--   0 cchandre   (501) staff       (20)       38 2023-05-26 10:26:24.841255 pyhamsys-0.0.4/setup.cfg
--rw-r--r--   0 cchandre   (501) staff       (20)     1129 2023-05-26 10:26:08.000000 pyhamsys-0.0.4/setup.py
+drwxr-xr-x   0 cchandre   (501) staff       (20)        0 2023-05-26 10:32:36.451190 pyhamsys-0.0.5/
+-rw-r--r--   0 cchandre   (501) staff       (20)     1304 2023-04-05 14:49:59.000000 pyhamsys-0.0.5/LICENSE
+-rw-r--r--   0 cchandre   (501) staff       (20)     5873 2023-05-26 10:32:36.450817 pyhamsys-0.0.5/PKG-INFO
+-rw-r--r--   0 cchandre   (501) staff       (20)     5058 2023-05-19 14:15:47.000000 pyhamsys-0.0.5/README.md
+drwxr-xr-x   0 cchandre   (501) staff       (20)        0 2023-05-26 10:32:36.446026 pyhamsys-0.0.5/pyhamsys/
+drwxr-xr-x   0 cchandre   (501) staff       (20)        0 2023-05-26 10:32:36.447859 pyhamsys-0.0.5/pyhamsys/src/
+drwxr-xr-x   0 cchandre   (501) staff       (20)        0 2023-05-26 10:32:36.450346 pyhamsys-0.0.5/pyhamsys/src/pyhamsys.egg-info/
+-rw-r--r--   0 cchandre   (501) staff       (20)     5873 2023-05-26 10:32:36.000000 pyhamsys-0.0.5/pyhamsys/src/pyhamsys.egg-info/PKG-INFO
+-rw-r--r--   0 cchandre   (501) staff       (20)      275 2023-05-26 10:32:36.000000 pyhamsys-0.0.5/pyhamsys/src/pyhamsys.egg-info/SOURCES.txt
+-rw-r--r--   0 cchandre   (501) staff       (20)        1 2023-05-26 10:32:36.000000 pyhamsys-0.0.5/pyhamsys/src/pyhamsys.egg-info/dependency_links.txt
+-rw-r--r--   0 cchandre   (501) staff       (20)       12 2023-05-26 10:32:36.000000 pyhamsys-0.0.5/pyhamsys/src/pyhamsys.egg-info/requires.txt
+-rw-r--r--   0 cchandre   (501) staff       (20)        9 2023-05-26 10:32:36.000000 pyhamsys-0.0.5/pyhamsys/src/pyhamsys.egg-info/top_level.txt
+-rw-r--r--   0 cchandre   (501) staff       (20)    11841 2023-05-26 10:32:26.000000 pyhamsys-0.0.5/pyhamsys/src/pyhamsys.py
+-rw-r--r--   0 cchandre   (501) staff       (20)       38 2023-05-26 10:32:36.451353 pyhamsys-0.0.5/setup.cfg
+-rw-r--r--   0 cchandre   (501) staff       (20)     1129 2023-05-26 10:31:09.000000 pyhamsys-0.0.5/setup.py
```

### Comparing `pyhamsys-0.0.4/LICENSE` & `pyhamsys-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhamsys-0.0.4/PKG-INFO` & `pyhamsys-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhamsys
-Version: 0.0.4
+Version: 0.0.5
 Summary: Some tools for Hamiltonian systems
 Home-page: http://github.com/cchandre/pyhamsys
 Author: Cristel Chandre
 Author-email: cristel.chandre@cnrs.fr
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Education
```

### Comparing `pyhamsys-0.0.4/README.md` & `pyhamsys-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pyhamsys-0.0.4/pyhamsys/src/pyhamsys.egg-info/PKG-INFO` & `pyhamsys-0.0.5/pyhamsys/src/pyhamsys.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhamsys
-Version: 0.0.4
+Version: 0.0.5
 Summary: Some tools for Hamiltonian systems
 Home-page: http://github.com/cchandre/pyhamsys
 Author: Cristel Chandre
 Author-email: cristel.chandre@cnrs.fr
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Education
```

### Comparing `pyhamsys-0.0.4/pyhamsys/src/pyhamsys.py` & `pyhamsys-0.0.5/pyhamsys/src/pyhamsys.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,15 +187,15 @@
 			alpha_s = [0.0378593198406116,  0.053859832783850, 0.048775800318585, 0.135207369686421, -0.161075257952980, 0.104540892120091, 0.209700510951356, -0.204785822176643, 0.074641362659228, 0.069119764509130, 0.037297935860413, 0.291269757886391, -0.300064001014902, 0.103652534528448]
 		elif self.name == 'ABA104':
 			alpha_s = [0.04706710064597251, 0.07181481672222451, 0.1129421186948636, 0.128108341856638, 0.1545976638231982, -0.4278843305285221, 0.4133542887856252]
 		elif self.name == 'ABA864':
 			alpha_s = [0.07113342649822312, 0.1119502609739741, 0.129203166982666, 0.1815796929159088, 0.3398320688569059, -0.3663966873688647, 0.03269807114118675]
 		elif self.name == 'ABA1064':
 			alpha_s = [0.03809449742241219, 0.05776438341466301, 0.08753433270225074, 0.116911820440748, 0.0907158752847932, 0.1263544726941979, 0.3095552309573282, -0.3269306129163933]
-		else:
+		elif self.name != 'Simple':
 			raise NameError(f'{self.name} integrator not defined')
 		if self.name == 'Simple':
 			self.alpha_s = [self.step]
 			self.alpha_o = [1]
 		else:
 			self.alpha_s = xp.concatenate((alpha_s, xp.flip(alpha_s)))
 			self.alpha_s *= self.step
```

### Comparing `pyhamsys-0.0.4/setup.py` & `pyhamsys-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pyhamsys',
-    version='0.0.4',
+    version='0.0.5',
     description='Some tools for Hamiltonian systems',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     url='http://github.com/cchandre/pyhamsys',
     classifiers=[
       'Programming Language :: Python :: 3',
```

