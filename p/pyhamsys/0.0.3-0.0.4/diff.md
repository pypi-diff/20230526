# Comparing `tmp/pyhamsys-0.0.3.tar.gz` & `tmp/pyhamsys-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhamsys-0.0.3.tar", last modified: Fri Apr 21 06:33:20 2023, max compression
+gzip compressed data, was "pyhamsys-0.0.4.tar", last modified: Fri May 26 10:26:24 2023, max compression
```

## Comparing `pyhamsys-0.0.3.tar` & `pyhamsys-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 cchandre   (503) staff       (20)        0 2023-04-21 06:33:20.774245 pyhamsys-0.0.3/
--rw-r--r--   0 cchandre   (503) staff       (20)     1304 2023-04-07 06:56:17.000000 pyhamsys-0.0.3/LICENSE
--rw-r--r--   0 cchandre   (503) staff       (20)     5807 2023-04-21 06:33:20.773885 pyhamsys-0.0.3/PKG-INFO
--rw-r--r--   0 cchandre   (503) staff       (20)     4992 2023-04-13 08:59:07.000000 pyhamsys-0.0.3/README.md
-drwxr-xr-x   0 cchandre   (503) staff       (20)        0 2023-04-21 06:33:20.769672 pyhamsys-0.0.3/pyhamsys/
-drwxr-xr-x   0 cchandre   (503) staff       (20)        0 2023-04-21 06:33:20.771217 pyhamsys-0.0.3/pyhamsys/src/
-drwxr-xr-x   0 cchandre   (503) staff       (20)        0 2023-04-21 06:33:20.773235 pyhamsys-0.0.3/pyhamsys/src/pyhamsys.egg-info/
--rw-r--r--   0 cchandre   (503) staff       (20)     5807 2023-04-21 06:33:20.000000 pyhamsys-0.0.3/pyhamsys/src/pyhamsys.egg-info/PKG-INFO
--rw-r--r--   0 cchandre   (503) staff       (20)      275 2023-04-21 06:33:20.000000 pyhamsys-0.0.3/pyhamsys/src/pyhamsys.egg-info/SOURCES.txt
--rw-r--r--   0 cchandre   (503) staff       (20)        1 2023-04-21 06:33:20.000000 pyhamsys-0.0.3/pyhamsys/src/pyhamsys.egg-info/dependency_links.txt
--rw-r--r--   0 cchandre   (503) staff       (20)       12 2023-04-21 06:33:20.000000 pyhamsys-0.0.3/pyhamsys/src/pyhamsys.egg-info/requires.txt
--rw-r--r--   0 cchandre   (503) staff       (20)        9 2023-04-21 06:33:20.000000 pyhamsys-0.0.3/pyhamsys/src/pyhamsys.egg-info/top_level.txt
--rw-r--r--   0 cchandre   (503) staff       (20)    11726 2023-04-13 08:59:07.000000 pyhamsys-0.0.3/pyhamsys/src/pyhamsys.py
--rw-r--r--   0 cchandre   (503) staff       (20)       38 2023-04-21 06:33:20.774363 pyhamsys-0.0.3/setup.cfg
--rw-r--r--   0 cchandre   (503) staff       (20)     1129 2023-04-21 06:31:31.000000 pyhamsys-0.0.3/setup.py
+drwxr-xr-x   0 cchandre   (501) staff       (20)        0 2023-05-26 10:26:24.841128 pyhamsys-0.0.4/
+-rw-r--r--   0 cchandre   (501) staff       (20)     1304 2023-04-05 14:49:59.000000 pyhamsys-0.0.4/LICENSE
+-rw-r--r--   0 cchandre   (501) staff       (20)     5873 2023-05-26 10:26:24.840744 pyhamsys-0.0.4/PKG-INFO
+-rw-r--r--   0 cchandre   (501) staff       (20)     5058 2023-05-19 14:15:47.000000 pyhamsys-0.0.4/README.md
+drwxr-xr-x   0 cchandre   (501) staff       (20)        0 2023-05-26 10:26:24.836509 pyhamsys-0.0.4/pyhamsys/
+drwxr-xr-x   0 cchandre   (501) staff       (20)        0 2023-05-26 10:26:24.837970 pyhamsys-0.0.4/pyhamsys/src/
+drwxr-xr-x   0 cchandre   (501) staff       (20)        0 2023-05-26 10:26:24.840311 pyhamsys-0.0.4/pyhamsys/src/pyhamsys.egg-info/
+-rw-r--r--   0 cchandre   (501) staff       (20)     5873 2023-05-26 10:26:24.000000 pyhamsys-0.0.4/pyhamsys/src/pyhamsys.egg-info/PKG-INFO
+-rw-r--r--   0 cchandre   (501) staff       (20)      275 2023-05-26 10:26:24.000000 pyhamsys-0.0.4/pyhamsys/src/pyhamsys.egg-info/SOURCES.txt
+-rw-r--r--   0 cchandre   (501) staff       (20)        1 2023-05-26 10:26:24.000000 pyhamsys-0.0.4/pyhamsys/src/pyhamsys.egg-info/dependency_links.txt
+-rw-r--r--   0 cchandre   (501) staff       (20)       12 2023-05-26 10:26:24.000000 pyhamsys-0.0.4/pyhamsys/src/pyhamsys.egg-info/requires.txt
+-rw-r--r--   0 cchandre   (501) staff       (20)        9 2023-05-26 10:26:24.000000 pyhamsys-0.0.4/pyhamsys/src/pyhamsys.egg-info/top_level.txt
+-rw-r--r--   0 cchandre   (501) staff       (20)    11819 2023-05-26 10:24:22.000000 pyhamsys-0.0.4/pyhamsys/src/pyhamsys.py
+-rw-r--r--   0 cchandre   (501) staff       (20)       38 2023-05-26 10:26:24.841255 pyhamsys-0.0.4/setup.cfg
+-rw-r--r--   0 cchandre   (501) staff       (20)     1129 2023-05-26 10:26:08.000000 pyhamsys-0.0.4/setup.py
```

### Comparing `pyhamsys-0.0.3/LICENSE` & `pyhamsys-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhamsys-0.0.3/PKG-INFO` & `pyhamsys-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhamsys
-Version: 0.0.3
+Version: 0.0.4
 Summary: Some tools for Hamiltonian systems
 Home-page: http://github.com/cchandre/pyhamsys
 Author: Cristel Chandre
 Author-email: cristel.chandre@cnrs.fr
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Education
@@ -80,9 +80,9 @@
 
 Returns:
    - If *times* is a float of integer, the output is a tuple (*t*, *y* or *x*) where *y* is the value of the state vector and *y* = [*t*, *x*] if autonomous is False.
    - If *times* is a list or array, returns the times and values of *y* or *x* at *times*. 
    - If *times* is a list or array with a single element, returns the times and values of *y* or *x* at all computed times. 
 
 References:
-  - Hairer, Lubich, Wanner, 2003, *Geometric-Preseving Algorithms for Ordinary Differential Equations* (Springer)
-  - McLachlan, 2022, *Tuning symplectic integrators is easy and worthwhile*, [arxiv:2104.10269](https://arxiv.org/abs/2104.10269)
+  - Hairer, Lubich, Wanner, 2003, *Geometric Numerical Integration: Structure-Preserving Algorithms for Ordinary Differential Equations* (Springer)
+  - McLachlan, *Tuning symplectic integrators is easy and worthwhile*, Commun. Comput. Phys. 31, 987 (2022); [arxiv:2104.10269](https://arxiv.org/abs/2104.10269)
```

### Comparing `pyhamsys-0.0.3/README.md` & `pyhamsys-0.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -58,9 +58,9 @@
 
 Returns:
    - If *times* is a float of integer, the output is a tuple (*t*, *y* or *x*) where *y* is the value of the state vector and *y* = [*t*, *x*] if autonomous is False.
    - If *times* is a list or array, returns the times and values of *y* or *x* at *times*. 
    - If *times* is a list or array with a single element, returns the times and values of *y* or *x* at all computed times. 
 
 References:
-  - Hairer, Lubich, Wanner, 2003, *Geometric-Preseving Algorithms for Ordinary Differential Equations* (Springer)
-  - McLachlan, 2022, *Tuning symplectic integrators is easy and worthwhile*, [arxiv:2104.10269](https://arxiv.org/abs/2104.10269)
+  - Hairer, Lubich, Wanner, 2003, *Geometric Numerical Integration: Structure-Preserving Algorithms for Ordinary Differential Equations* (Springer)
+  - McLachlan, *Tuning symplectic integrators is easy and worthwhile*, Commun. Comput. Phys. 31, 987 (2022); [arxiv:2104.10269](https://arxiv.org/abs/2104.10269)
```

### Comparing `pyhamsys-0.0.3/pyhamsys/src/pyhamsys.egg-info/PKG-INFO` & `pyhamsys-0.0.4/pyhamsys/src/pyhamsys.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhamsys
-Version: 0.0.3
+Version: 0.0.4
 Summary: Some tools for Hamiltonian systems
 Home-page: http://github.com/cchandre/pyhamsys
 Author: Cristel Chandre
 Author-email: cristel.chandre@cnrs.fr
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Education
@@ -80,9 +80,9 @@
 
 Returns:
    - If *times* is a float of integer, the output is a tuple (*t*, *y* or *x*) where *y* is the value of the state vector and *y* = [*t*, *x*] if autonomous is False.
    - If *times* is a list or array, returns the times and values of *y* or *x* at *times*. 
    - If *times* is a list or array with a single element, returns the times and values of *y* or *x* at all computed times. 
 
 References:
-  - Hairer, Lubich, Wanner, 2003, *Geometric-Preseving Algorithms for Ordinary Differential Equations* (Springer)
-  - McLachlan, 2022, *Tuning symplectic integrators is easy and worthwhile*, [arxiv:2104.10269](https://arxiv.org/abs/2104.10269)
+  - Hairer, Lubich, Wanner, 2003, *Geometric Numerical Integration: Structure-Preserving Algorithms for Ordinary Differential Equations* (Springer)
+  - McLachlan, *Tuning symplectic integrators is easy and worthwhile*, Commun. Comput. Phys. 31, 987 (2022); [arxiv:2104.10269](https://arxiv.org/abs/2104.10269)
```

### Comparing `pyhamsys-0.0.3/pyhamsys/src/pyhamsys.py` & `pyhamsys-0.0.4/pyhamsys/src/pyhamsys.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,21 +189,25 @@
 			alpha_s = [0.04706710064597251, 0.07181481672222451, 0.1129421186948636, 0.128108341856638, 0.1545976638231982, -0.4278843305285221, 0.4133542887856252]
 		elif self.name == 'ABA864':
 			alpha_s = [0.07113342649822312, 0.1119502609739741, 0.129203166982666, 0.1815796929159088, 0.3398320688569059, -0.3663966873688647, 0.03269807114118675]
 		elif self.name == 'ABA1064':
 			alpha_s = [0.03809449742241219, 0.05776438341466301, 0.08753433270225074, 0.116911820440748, 0.0907158752847932, 0.1263544726941979, 0.3095552309573282, -0.3269306129163933]
 		else:
 			raise NameError(f'{self.name} integrator not defined')
-		self.alpha_s = xp.concatenate((alpha_s, xp.flip(alpha_s)))
-		self.alpha_s *= self.step
-		self.alpha_o = xp.tile([1, 0], len(alpha_s))
-		self.alpha_s = xp.concatenate((alpha_s, xp.flip(alpha_s)))
-		self.alpha_s *= self.step
-		self.alpha_o = xp.tile([1, 0], len(alpha_s))
-	
+		if self.name == 'Simple':
+			self.alpha_s = [self.step]
+			self.alpha_o = [1]
+		else:
+			self.alpha_s = xp.concatenate((alpha_s, xp.flip(alpha_s)))
+			self.alpha_s *= self.step
+			self.alpha_o = xp.tile([1, 0], len(alpha_s))
+			self.alpha_s = xp.concatenate((alpha_s, xp.flip(alpha_s)))
+			self.alpha_s *= self.step
+			self.alpha_o = xp.tile([1, 0], len(alpha_s))
+
 	def _integrate(self, chi:Callable, chi_star:Callable, y):
 		for h, st in zip(self.alpha_s, self.alpha_o):
 			y = chi(h, y) if st==0 else chi_star(h, y)
 		return y
 	
 	def integrate(self, chi:Callable, chi_star:Callable, y:xp.ndarray, times:Union[int, float, list, xp.ndarray], command:Callable=None, autonomous:bool=True) -> Tuple[Union[float, xp.ndarray], xp.ndarray]:
 		"""
```

### Comparing `pyhamsys-0.0.3/setup.py` & `pyhamsys-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pyhamsys',
-    version='0.0.3',
+    version='0.0.4',
     description='Some tools for Hamiltonian systems',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     url='http://github.com/cchandre/pyhamsys',
     classifiers=[
       'Programming Language :: Python :: 3',
```

