# Comparing `tmp/starred-astro-1.0.tar.gz` & `tmp/starred-astro-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starred-astro-1.0.tar", last modified: Mon May 22 14:24:39 2023, max compression
+gzip compressed data, was "starred-astro-1.1.tar", last modified: Fri May 26 09:14:37 2023, max compression
```

## Comparing `starred-astro-1.0.tar` & `starred-astro-1.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 kevinmicha   (501) staff       (20)        0 2023-05-22 14:24:39.329350 starred-astro-1.0/
--rw-r--r--   0 kevinmicha   (501) staff       (20)      860 2023-05-06 17:28:47.000000 starred-astro-1.0/AUTHORS.md
--rw-r--r--   0 kevinmicha   (501) staff       (20)    35143 2023-02-21 14:20:52.000000 starred-astro-1.0/LICENSE
--rw-r--r--   0 kevinmicha   (501) staff       (20)      441 2023-05-22 14:24:39.329181 starred-astro-1.0/PKG-INFO
--rw-r--r--   0 kevinmicha   (501) staff       (20)     3914 2023-05-15 08:43:52.000000 starred-astro-1.0/README.md
--rw-r--r--   0 kevinmicha   (501) staff       (20)       38 2023-05-22 14:24:39.329400 starred-astro-1.0/setup.cfg
--rw-r--r--   0 kevinmicha   (501) staff       (20)      855 2023-05-22 14:24:08.000000 starred-astro-1.0/setup.py
-drwxr-xr-x   0 kevinmicha   (501) staff       (20)        0 2023-05-22 14:24:39.322870 starred-astro-1.0/starred/
--rw-r--r--   0 kevinmicha   (501) staff       (20)      352 2022-08-02 12:24:07.000000 starred-astro-1.0/starred/__init__.py
-drwxr-xr-x   0 kevinmicha   (501) staff       (20)        0 2023-05-22 14:24:39.324156 starred-astro-1.0/starred/deconvolution/
--rw-r--r--   0 kevinmicha   (501) staff       (20)      112 2023-02-21 14:19:09.000000 starred-astro-1.0/starred/deconvolution/__init__.py
--rw-r--r--   0 kevinmicha   (501) staff       (20)    21721 2023-05-01 15:42:17.000000 starred-astro-1.0/starred/deconvolution/deconvolution.py
--rw-r--r--   0 kevinmicha   (501) staff       (20)     8175 2023-05-22 14:05:49.000000 starred-astro-1.0/starred/deconvolution/loss.py
--rw-r--r--   0 kevinmicha   (501) staff       (20)     3907 2023-02-23 18:35:26.000000 starred-astro-1.0/starred/deconvolution/parameters.py
-drwxr-xr-x   0 kevinmicha   (501) staff       (20)        0 2023-05-22 14:24:39.324829 starred-astro-1.0/starred/plots/
--rw-r--r--   0 kevinmicha   (501) staff       (20)       89 2023-02-24 15:47:18.000000 starred-astro-1.0/starred/plots/__init__.py
--rw-r--r--   0 kevinmicha   (501) staff       (20)     4793 2023-02-21 14:19:09.000000 starred-astro-1.0/starred/plots/f2n.py
--rw-r--r--   0 kevinmicha   (501) staff       (20)    14377 2023-05-15 08:43:11.000000 starred-astro-1.0/starred/plots/plot_function.py
-drwxr-xr-x   0 kevinmicha   (501) staff       (20)        0 2023-05-22 14:24:39.326509 starred-astro-1.0/starred/psf/
--rw-r--r--   0 kevinmicha   (501) staff       (20)      103 2022-08-02 12:51:20.000000 starred-astro-1.0/starred/psf/__init__.py
--rw-r--r--   0 kevinmicha   (501) staff       (20)     7811 2023-05-22 14:05:49.000000 starred-astro-1.0/starred/psf/loss.py
--rw-r--r--   0 kevinmicha   (501) staff       (20)     3993 2023-03-02 10:26:30.000000 starred-astro-1.0/starred/psf/parameters.py
--rw-r--r--   0 kevinmicha   (501) staff       (20)    18769 2023-04-19 10:18:52.000000 starred-astro-1.0/starred/psf/psf.py
-drwxr-xr-x   0 kevinmicha   (501) staff       (20)        0 2023-05-22 14:24:39.328475 starred-astro-1.0/starred/utils/
--rw-r--r--   0 kevinmicha   (501) staff       (20)      184 2023-02-24 15:47:08.000000 starred-astro-1.0/starred/utils/__init__.py
--rw-r--r--   0 kevinmicha   (501) staff       (20)     3147 2023-03-02 10:26:30.000000 starred-astro-1.0/starred/utils/ds9reg.py
--rw-r--r--   0 kevinmicha   (501) staff       (20)     8872 2023-04-19 10:18:52.000000 starred-astro-1.0/starred/utils/generic_utils.py
--rw-r--r--   0 kevinmicha   (501) staff       (20)     1762 2023-04-19 10:18:52.000000 starred-astro-1.0/starred/utils/inference_base.py
--rw-r--r--   0 kevinmicha   (501) staff       (20)     3963 2023-04-19 10:18:52.000000 starred-astro-1.0/starred/utils/jax_utils.py
--rw-r--r--   0 kevinmicha   (501) staff       (20)     6258 2023-04-19 10:18:52.000000 starred-astro-1.0/starred/utils/noise_utils.py
--rw-r--r--   0 kevinmicha   (501) staff       (20)    10436 2023-05-15 08:43:11.000000 starred-astro-1.0/starred/utils/optimization.py
--rw-r--r--   0 kevinmicha   (501) staff       (20)     4549 2023-04-19 10:18:52.000000 starred-astro-1.0/starred/utils/parameters.py
-drwxr-xr-x   0 kevinmicha   (501) staff       (20)        0 2023-05-22 14:24:39.328994 starred-astro-1.0/starred_astro.egg-info/
--rw-r--r--   0 kevinmicha   (501) staff       (20)      441 2023-05-22 14:24:39.000000 starred-astro-1.0/starred_astro.egg-info/PKG-INFO
--rw-r--r--   0 kevinmicha   (501) staff       (20)      738 2023-05-22 14:24:39.000000 starred-astro-1.0/starred_astro.egg-info/SOURCES.txt
--rw-r--r--   0 kevinmicha   (501) staff       (20)        1 2023-05-22 14:24:39.000000 starred-astro-1.0/starred_astro.egg-info/dependency_links.txt
--rw-r--r--   0 kevinmicha   (501) staff       (20)        8 2023-05-22 14:24:39.000000 starred-astro-1.0/starred_astro.egg-info/top_level.txt
+drwxr-xr-x   0 kevinmicha   (501) staff       (20)        0 2023-05-26 09:14:37.725083 starred-astro-1.1/
+-rw-r--r--   0 kevinmicha   (501) staff       (20)      860 2023-05-06 17:28:47.000000 starred-astro-1.1/AUTHORS.md
+-rw-r--r--   0 kevinmicha   (501) staff       (20)    35143 2023-02-21 14:20:52.000000 starred-astro-1.1/LICENSE
+-rw-r--r--   0 kevinmicha   (501) staff       (20)     4827 2023-05-26 09:14:37.724919 starred-astro-1.1/PKG-INFO
+-rw-r--r--   0 kevinmicha   (501) staff       (20)     3914 2023-05-15 08:43:52.000000 starred-astro-1.1/README.md
+-rw-r--r--   0 kevinmicha   (501) staff       (20)       38 2023-05-26 09:14:37.725138 starred-astro-1.1/setup.cfg
+-rw-r--r--   0 kevinmicha   (501) staff       (20)     1063 2023-05-26 09:13:24.000000 starred-astro-1.1/setup.py
+drwxr-xr-x   0 kevinmicha   (501) staff       (20)        0 2023-05-26 09:14:37.719558 starred-astro-1.1/starred/
+-rw-r--r--   0 kevinmicha   (501) staff       (20)      352 2022-08-02 12:24:07.000000 starred-astro-1.1/starred/__init__.py
+drwxr-xr-x   0 kevinmicha   (501) staff       (20)        0 2023-05-26 09:14:37.720697 starred-astro-1.1/starred/deconvolution/
+-rw-r--r--   0 kevinmicha   (501) staff       (20)      112 2023-02-21 14:19:09.000000 starred-astro-1.1/starred/deconvolution/__init__.py
+-rw-r--r--   0 kevinmicha   (501) staff       (20)    21721 2023-05-01 15:42:17.000000 starred-astro-1.1/starred/deconvolution/deconvolution.py
+-rw-r--r--   0 kevinmicha   (501) staff       (20)     8175 2023-05-22 14:05:49.000000 starred-astro-1.1/starred/deconvolution/loss.py
+-rw-r--r--   0 kevinmicha   (501) staff       (20)     3907 2023-02-23 18:35:26.000000 starred-astro-1.1/starred/deconvolution/parameters.py
+drwxr-xr-x   0 kevinmicha   (501) staff       (20)        0 2023-05-26 09:14:37.721418 starred-astro-1.1/starred/plots/
+-rw-r--r--   0 kevinmicha   (501) staff       (20)       89 2023-02-24 15:47:18.000000 starred-astro-1.1/starred/plots/__init__.py
+-rw-r--r--   0 kevinmicha   (501) staff       (20)     4793 2023-02-21 14:19:09.000000 starred-astro-1.1/starred/plots/f2n.py
+-rw-r--r--   0 kevinmicha   (501) staff       (20)    14377 2023-05-15 08:43:11.000000 starred-astro-1.1/starred/plots/plot_function.py
+drwxr-xr-x   0 kevinmicha   (501) staff       (20)        0 2023-05-26 09:14:37.722342 starred-astro-1.1/starred/psf/
+-rw-r--r--   0 kevinmicha   (501) staff       (20)      103 2022-08-02 12:51:20.000000 starred-astro-1.1/starred/psf/__init__.py
+-rw-r--r--   0 kevinmicha   (501) staff       (20)     7811 2023-05-22 14:05:49.000000 starred-astro-1.1/starred/psf/loss.py
+-rw-r--r--   0 kevinmicha   (501) staff       (20)     3993 2023-03-02 10:26:30.000000 starred-astro-1.1/starred/psf/parameters.py
+-rw-r--r--   0 kevinmicha   (501) staff       (20)    18769 2023-04-19 10:18:52.000000 starred-astro-1.1/starred/psf/psf.py
+drwxr-xr-x   0 kevinmicha   (501) staff       (20)        0 2023-05-26 09:14:37.724170 starred-astro-1.1/starred/utils/
+-rw-r--r--   0 kevinmicha   (501) staff       (20)      184 2023-02-24 15:47:08.000000 starred-astro-1.1/starred/utils/__init__.py
+-rw-r--r--   0 kevinmicha   (501) staff       (20)     3147 2023-03-02 10:26:30.000000 starred-astro-1.1/starred/utils/ds9reg.py
+-rw-r--r--   0 kevinmicha   (501) staff       (20)     8872 2023-04-19 10:18:52.000000 starred-astro-1.1/starred/utils/generic_utils.py
+-rw-r--r--   0 kevinmicha   (501) staff       (20)     1762 2023-04-19 10:18:52.000000 starred-astro-1.1/starred/utils/inference_base.py
+-rw-r--r--   0 kevinmicha   (501) staff       (20)     3963 2023-04-19 10:18:52.000000 starred-astro-1.1/starred/utils/jax_utils.py
+-rw-r--r--   0 kevinmicha   (501) staff       (20)     6258 2023-04-19 10:18:52.000000 starred-astro-1.1/starred/utils/noise_utils.py
+-rw-r--r--   0 kevinmicha   (501) staff       (20)    10436 2023-05-15 08:43:11.000000 starred-astro-1.1/starred/utils/optimization.py
+-rw-r--r--   0 kevinmicha   (501) staff       (20)     4549 2023-04-19 10:18:52.000000 starred-astro-1.1/starred/utils/parameters.py
+drwxr-xr-x   0 kevinmicha   (501) staff       (20)        0 2023-05-26 09:14:37.724735 starred-astro-1.1/starred_astro.egg-info/
+-rw-r--r--   0 kevinmicha   (501) staff       (20)     4827 2023-05-26 09:14:37.000000 starred-astro-1.1/starred_astro.egg-info/PKG-INFO
+-rw-r--r--   0 kevinmicha   (501) staff       (20)      738 2023-05-26 09:14:37.000000 starred-astro-1.1/starred_astro.egg-info/SOURCES.txt
+-rw-r--r--   0 kevinmicha   (501) staff       (20)        1 2023-05-26 09:14:37.000000 starred-astro-1.1/starred_astro.egg-info/dependency_links.txt
+-rw-r--r--   0 kevinmicha   (501) staff       (20)        8 2023-05-26 09:14:37.000000 starred-astro-1.1/starred_astro.egg-info/top_level.txt
```

### Comparing `starred-astro-1.0/AUTHORS.md` & `starred-astro-1.1/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `starred-astro-1.0/LICENSE` & `starred-astro-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `starred-astro-1.0/README.md` & `starred-astro-1.1/README.md`

 * *Files identical despite different names*

### Comparing `starred-astro-1.0/setup.py` & `starred-astro-1.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,17 +9,24 @@
         self.test_suite = True
 
     def run_tests(self):
         import pytest
         errno = pytest.main(self.test_args)
         sys.exit(errno)
 
+try:
+    import pypandoc
+    long_description = pypandoc.convert_file('README.md', 'rst')
+except(IOError, ImportError):
+    long_description = open('README.md').read()
+
 setup(
     name='starred-astro',
-    version='1.0',
+    version='1.1',
     author='Kevin Michalewicz',
     author_email='kevinmicha@hotmail.com',
     description='A two-channel deconvolution method with Starlet regularization',
+    long_description=long_description,
     packages=['starred', 'starred.deconvolution', 'starred.plots', 'starred.psf', 'starred.utils'],
     requires=['astropy', 'dill', 'galsim', 'jax', 'jaxlib', 'jaxopt', 'matplotlib', 'numpy', 'scikitimage', 'scipy', 'optax', 'tqdm'],
     cmdclass={'test': PyTest}
 )
```

### Comparing `starred-astro-1.0/starred/deconvolution/deconvolution.py` & `starred-astro-1.1/starred/deconvolution/deconvolution.py`

 * *Files identical despite different names*

### Comparing `starred-astro-1.0/starred/deconvolution/loss.py` & `starred-astro-1.1/starred/deconvolution/loss.py`

 * *Files identical despite different names*

### Comparing `starred-astro-1.0/starred/deconvolution/parameters.py` & `starred-astro-1.1/starred/deconvolution/parameters.py`

 * *Files identical despite different names*

### Comparing `starred-astro-1.0/starred/plots/f2n.py` & `starred-astro-1.1/starred/plots/f2n.py`

 * *Files identical despite different names*

### Comparing `starred-astro-1.0/starred/plots/plot_function.py` & `starred-astro-1.1/starred/plots/plot_function.py`

 * *Files identical despite different names*

### Comparing `starred-astro-1.0/starred/psf/loss.py` & `starred-astro-1.1/starred/psf/loss.py`

 * *Files identical despite different names*

### Comparing `starred-astro-1.0/starred/psf/parameters.py` & `starred-astro-1.1/starred/psf/parameters.py`

 * *Files identical despite different names*

### Comparing `starred-astro-1.0/starred/psf/psf.py` & `starred-astro-1.1/starred/psf/psf.py`

 * *Files identical despite different names*

### Comparing `starred-astro-1.0/starred/utils/ds9reg.py` & `starred-astro-1.1/starred/utils/ds9reg.py`

 * *Files identical despite different names*

### Comparing `starred-astro-1.0/starred/utils/generic_utils.py` & `starred-astro-1.1/starred/utils/generic_utils.py`

 * *Files identical despite different names*

### Comparing `starred-astro-1.0/starred/utils/inference_base.py` & `starred-astro-1.1/starred/utils/inference_base.py`

 * *Files identical despite different names*

### Comparing `starred-astro-1.0/starred/utils/jax_utils.py` & `starred-astro-1.1/starred/utils/jax_utils.py`

 * *Files identical despite different names*

### Comparing `starred-astro-1.0/starred/utils/noise_utils.py` & `starred-astro-1.1/starred/utils/noise_utils.py`

 * *Files identical despite different names*

### Comparing `starred-astro-1.0/starred/utils/optimization.py` & `starred-astro-1.1/starred/utils/optimization.py`

 * *Files identical despite different names*

### Comparing `starred-astro-1.0/starred/utils/parameters.py` & `starred-astro-1.1/starred/utils/parameters.py`

 * *Files identical despite different names*

### Comparing `starred-astro-1.0/starred_astro.egg-info/SOURCES.txt` & `starred-astro-1.1/starred_astro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

