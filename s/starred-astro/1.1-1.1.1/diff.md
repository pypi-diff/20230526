# Comparing `tmp/starred-astro-1.1.tar.gz` & `tmp/starred-astro-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starred-astro-1.1.tar", last modified: Fri May 26 09:14:37 2023, max compression
+gzip compressed data, was "starred-astro-1.1.1.tar", last modified: Fri May 26 15:54:24 2023, max compression
```

## Comparing `starred-astro-1.1.tar` & `starred-astro-1.1.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 kevinmicha   (501) staff       (20)        0 2023-05-26 09:14:37.725083 starred-astro-1.1/
--rw-r--r--   0 kevinmicha   (501) staff       (20)      860 2023-05-06 17:28:47.000000 starred-astro-1.1/AUTHORS.md
--rw-r--r--   0 kevinmicha   (501) staff       (20)    35143 2023-02-21 14:20:52.000000 starred-astro-1.1/LICENSE
--rw-r--r--   0 kevinmicha   (501) staff       (20)     4827 2023-05-26 09:14:37.724919 starred-astro-1.1/PKG-INFO
--rw-r--r--   0 kevinmicha   (501) staff       (20)     3914 2023-05-15 08:43:52.000000 starred-astro-1.1/README.md
--rw-r--r--   0 kevinmicha   (501) staff       (20)       38 2023-05-26 09:14:37.725138 starred-astro-1.1/setup.cfg
--rw-r--r--   0 kevinmicha   (501) staff       (20)     1063 2023-05-26 09:13:24.000000 starred-astro-1.1/setup.py
-drwxr-xr-x   0 kevinmicha   (501) staff       (20)        0 2023-05-26 09:14:37.719558 starred-astro-1.1/starred/
--rw-r--r--   0 kevinmicha   (501) staff       (20)      352 2022-08-02 12:24:07.000000 starred-astro-1.1/starred/__init__.py
-drwxr-xr-x   0 kevinmicha   (501) staff       (20)        0 2023-05-26 09:14:37.720697 starred-astro-1.1/starred/deconvolution/
--rw-r--r--   0 kevinmicha   (501) staff       (20)      112 2023-02-21 14:19:09.000000 starred-astro-1.1/starred/deconvolution/__init__.py
--rw-r--r--   0 kevinmicha   (501) staff       (20)    21721 2023-05-01 15:42:17.000000 starred-astro-1.1/starred/deconvolution/deconvolution.py
--rw-r--r--   0 kevinmicha   (501) staff       (20)     8175 2023-05-22 14:05:49.000000 starred-astro-1.1/starred/deconvolution/loss.py
--rw-r--r--   0 kevinmicha   (501) staff       (20)     3907 2023-02-23 18:35:26.000000 starred-astro-1.1/starred/deconvolution/parameters.py
-drwxr-xr-x   0 kevinmicha   (501) staff       (20)        0 2023-05-26 09:14:37.721418 starred-astro-1.1/starred/plots/
--rw-r--r--   0 kevinmicha   (501) staff       (20)       89 2023-02-24 15:47:18.000000 starred-astro-1.1/starred/plots/__init__.py
--rw-r--r--   0 kevinmicha   (501) staff       (20)     4793 2023-02-21 14:19:09.000000 starred-astro-1.1/starred/plots/f2n.py
--rw-r--r--   0 kevinmicha   (501) staff       (20)    14377 2023-05-15 08:43:11.000000 starred-astro-1.1/starred/plots/plot_function.py
-drwxr-xr-x   0 kevinmicha   (501) staff       (20)        0 2023-05-26 09:14:37.722342 starred-astro-1.1/starred/psf/
--rw-r--r--   0 kevinmicha   (501) staff       (20)      103 2022-08-02 12:51:20.000000 starred-astro-1.1/starred/psf/__init__.py
--rw-r--r--   0 kevinmicha   (501) staff       (20)     7811 2023-05-22 14:05:49.000000 starred-astro-1.1/starred/psf/loss.py
--rw-r--r--   0 kevinmicha   (501) staff       (20)     3993 2023-03-02 10:26:30.000000 starred-astro-1.1/starred/psf/parameters.py
--rw-r--r--   0 kevinmicha   (501) staff       (20)    18769 2023-04-19 10:18:52.000000 starred-astro-1.1/starred/psf/psf.py
-drwxr-xr-x   0 kevinmicha   (501) staff       (20)        0 2023-05-26 09:14:37.724170 starred-astro-1.1/starred/utils/
--rw-r--r--   0 kevinmicha   (501) staff       (20)      184 2023-02-24 15:47:08.000000 starred-astro-1.1/starred/utils/__init__.py
--rw-r--r--   0 kevinmicha   (501) staff       (20)     3147 2023-03-02 10:26:30.000000 starred-astro-1.1/starred/utils/ds9reg.py
--rw-r--r--   0 kevinmicha   (501) staff       (20)     8872 2023-04-19 10:18:52.000000 starred-astro-1.1/starred/utils/generic_utils.py
--rw-r--r--   0 kevinmicha   (501) staff       (20)     1762 2023-04-19 10:18:52.000000 starred-astro-1.1/starred/utils/inference_base.py
--rw-r--r--   0 kevinmicha   (501) staff       (20)     3963 2023-04-19 10:18:52.000000 starred-astro-1.1/starred/utils/jax_utils.py
--rw-r--r--   0 kevinmicha   (501) staff       (20)     6258 2023-04-19 10:18:52.000000 starred-astro-1.1/starred/utils/noise_utils.py
--rw-r--r--   0 kevinmicha   (501) staff       (20)    10436 2023-05-15 08:43:11.000000 starred-astro-1.1/starred/utils/optimization.py
--rw-r--r--   0 kevinmicha   (501) staff       (20)     4549 2023-04-19 10:18:52.000000 starred-astro-1.1/starred/utils/parameters.py
-drwxr-xr-x   0 kevinmicha   (501) staff       (20)        0 2023-05-26 09:14:37.724735 starred-astro-1.1/starred_astro.egg-info/
--rw-r--r--   0 kevinmicha   (501) staff       (20)     4827 2023-05-26 09:14:37.000000 starred-astro-1.1/starred_astro.egg-info/PKG-INFO
--rw-r--r--   0 kevinmicha   (501) staff       (20)      738 2023-05-26 09:14:37.000000 starred-astro-1.1/starred_astro.egg-info/SOURCES.txt
--rw-r--r--   0 kevinmicha   (501) staff       (20)        1 2023-05-26 09:14:37.000000 starred-astro-1.1/starred_astro.egg-info/dependency_links.txt
--rw-r--r--   0 kevinmicha   (501) staff       (20)        8 2023-05-26 09:14:37.000000 starred-astro-1.1/starred_astro.egg-info/top_level.txt
+drwxr-xr-x   0 kevinmicha   (501) staff       (20)        0 2023-05-26 15:54:24.583905 starred-astro-1.1.1/
+-rw-r--r--   0 kevinmicha   (501) staff       (20)      860 2023-05-06 17:28:47.000000 starred-astro-1.1.1/AUTHORS.md
+-rw-r--r--   0 kevinmicha   (501) staff       (20)    35143 2023-02-21 14:20:52.000000 starred-astro-1.1.1/LICENSE
+-rw-r--r--   0 kevinmicha   (501) staff       (20)     4134 2023-05-26 15:54:24.583747 starred-astro-1.1.1/PKG-INFO
+-rw-r--r--   0 kevinmicha   (501) staff       (20)     3282 2023-05-26 15:51:07.000000 starred-astro-1.1.1/README.md
+-rw-r--r--   0 kevinmicha   (501) staff       (20)       38 2023-05-26 15:54:24.583956 starred-astro-1.1.1/setup.cfg
+-rw-r--r--   0 kevinmicha   (501) staff       (20)     1065 2023-05-26 15:54:19.000000 starred-astro-1.1.1/setup.py
+drwxr-xr-x   0 kevinmicha   (501) staff       (20)        0 2023-05-26 15:54:24.578306 starred-astro-1.1.1/starred/
+-rw-r--r--   0 kevinmicha   (501) staff       (20)      352 2022-08-02 12:24:07.000000 starred-astro-1.1.1/starred/__init__.py
+drwxr-xr-x   0 kevinmicha   (501) staff       (20)        0 2023-05-26 15:54:24.579479 starred-astro-1.1.1/starred/deconvolution/
+-rw-r--r--   0 kevinmicha   (501) staff       (20)      112 2023-02-21 14:19:09.000000 starred-astro-1.1.1/starred/deconvolution/__init__.py
+-rw-r--r--   0 kevinmicha   (501) staff       (20)    21721 2023-05-01 15:42:17.000000 starred-astro-1.1.1/starred/deconvolution/deconvolution.py
+-rw-r--r--   0 kevinmicha   (501) staff       (20)     8175 2023-05-22 14:05:49.000000 starred-astro-1.1.1/starred/deconvolution/loss.py
+-rw-r--r--   0 kevinmicha   (501) staff       (20)     3907 2023-02-23 18:35:26.000000 starred-astro-1.1.1/starred/deconvolution/parameters.py
+drwxr-xr-x   0 kevinmicha   (501) staff       (20)        0 2023-05-26 15:54:24.580259 starred-astro-1.1.1/starred/plots/
+-rw-r--r--   0 kevinmicha   (501) staff       (20)       89 2023-02-24 15:47:18.000000 starred-astro-1.1.1/starred/plots/__init__.py
+-rw-r--r--   0 kevinmicha   (501) staff       (20)     4793 2023-02-21 14:19:09.000000 starred-astro-1.1.1/starred/plots/f2n.py
+-rw-r--r--   0 kevinmicha   (501) staff       (20)    14377 2023-05-15 08:43:11.000000 starred-astro-1.1.1/starred/plots/plot_function.py
+drwxr-xr-x   0 kevinmicha   (501) staff       (20)        0 2023-05-26 15:54:24.581239 starred-astro-1.1.1/starred/psf/
+-rw-r--r--   0 kevinmicha   (501) staff       (20)      103 2022-08-02 12:51:20.000000 starred-astro-1.1.1/starred/psf/__init__.py
+-rw-r--r--   0 kevinmicha   (501) staff       (20)     7811 2023-05-22 14:05:49.000000 starred-astro-1.1.1/starred/psf/loss.py
+-rw-r--r--   0 kevinmicha   (501) staff       (20)     3993 2023-03-02 10:26:30.000000 starred-astro-1.1.1/starred/psf/parameters.py
+-rw-r--r--   0 kevinmicha   (501) staff       (20)    18769 2023-04-19 10:18:52.000000 starred-astro-1.1.1/starred/psf/psf.py
+drwxr-xr-x   0 kevinmicha   (501) staff       (20)        0 2023-05-26 15:54:24.583077 starred-astro-1.1.1/starred/utils/
+-rw-r--r--   0 kevinmicha   (501) staff       (20)      184 2023-02-24 15:47:08.000000 starred-astro-1.1.1/starred/utils/__init__.py
+-rw-r--r--   0 kevinmicha   (501) staff       (20)     3147 2023-03-02 10:26:30.000000 starred-astro-1.1.1/starred/utils/ds9reg.py
+-rw-r--r--   0 kevinmicha   (501) staff       (20)     8872 2023-04-19 10:18:52.000000 starred-astro-1.1.1/starred/utils/generic_utils.py
+-rw-r--r--   0 kevinmicha   (501) staff       (20)     1762 2023-04-19 10:18:52.000000 starred-astro-1.1.1/starred/utils/inference_base.py
+-rw-r--r--   0 kevinmicha   (501) staff       (20)     3963 2023-04-19 10:18:52.000000 starred-astro-1.1.1/starred/utils/jax_utils.py
+-rw-r--r--   0 kevinmicha   (501) staff       (20)     6258 2023-04-19 10:18:52.000000 starred-astro-1.1.1/starred/utils/noise_utils.py
+-rw-r--r--   0 kevinmicha   (501) staff       (20)    10436 2023-05-15 08:43:11.000000 starred-astro-1.1.1/starred/utils/optimization.py
+-rw-r--r--   0 kevinmicha   (501) staff       (20)     4549 2023-04-19 10:18:52.000000 starred-astro-1.1.1/starred/utils/parameters.py
+drwxr-xr-x   0 kevinmicha   (501) staff       (20)        0 2023-05-26 15:54:24.583564 starred-astro-1.1.1/starred_astro.egg-info/
+-rw-r--r--   0 kevinmicha   (501) staff       (20)     4134 2023-05-26 15:54:24.000000 starred-astro-1.1.1/starred_astro.egg-info/PKG-INFO
+-rw-r--r--   0 kevinmicha   (501) staff       (20)      738 2023-05-26 15:54:24.000000 starred-astro-1.1.1/starred_astro.egg-info/SOURCES.txt
+-rw-r--r--   0 kevinmicha   (501) staff       (20)        1 2023-05-26 15:54:24.000000 starred-astro-1.1.1/starred_astro.egg-info/dependency_links.txt
+-rw-r--r--   0 kevinmicha   (501) staff       (20)        8 2023-05-26 15:54:24.000000 starred-astro-1.1.1/starred_astro.egg-info/top_level.txt
```

### Comparing `starred-astro-1.1/AUTHORS.md` & `starred-astro-1.1.1/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `starred-astro-1.1/LICENSE` & `starred-astro-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `starred-astro-1.1/PKG-INFO` & `starred-astro-1.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starred-astro
-Version: 1.1
+Version: 1.1.1
 Summary: A two-channel deconvolution method with Starlet regularization
 Author: Kevin Michalewicz
 Author-email: kevinmicha@hotmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires: astropy
 Requires: dill
@@ -30,89 +30,85 @@
 method powered by Starlet regularization and JAX automatic
 differentiation. It uses a Point Spread Function (PSF) narrower than the
 original one as kernel.
 
 Installation
 ------------
 
-Through Anaconda
-~~~~~~~~~~~~~~~~
+Through PyPI
+~~~~~~~~~~~~
 
-We provide an Anaconda environment that satisfies all the dependencies
-in ``starred-env.yml``.
+STARRED releases are distributed through the Python Package Index
+(PyPI). To install the latest version use ``pip``:
 
 .. code:: bash
 
-   git clone https://gitlab.com/cosmograil/starred.git
-   cd starred
-   conda env create -f starred-env.yml
-   conda activate starred-env
-   pip install .
-
-In case you have an NVIDIA GPU, this should automatically download the
-right version of JAX as well as cuDNN. Next, you can run the tests to
-make sure your installation is working correctly.
+   $ pip install starred-astro
+
+STARRED runs much faster on GPUs, so make sure you install a version of
+JAX that is compatible with your version of CUDA and cuDNN:
 
 .. code:: bash
 
-   # While still in the STARRED directory:
-   pytest . 
+   $ pip install "jax[cuda11_cudnn86]" -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
 
-Manually handling the dependencies
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+Requirements
+------------
 
-If you want to use an existing environment, just omit the Anaconda
-commands above:
+STARRED requires the following Python packages:
 
-.. code:: bash
+-  ``astropy``
 
-   git clone https://gitlab.com/cosmograil/starred
-   cd starred 
-   pip install .
+-  ``dill``
 
-or if you need to install it for your user only:
+-  ``jax``
 
-.. code:: bash
+-  ``jaxlib``
 
-   python setup.py install --user 
+-  ``jaxopt``
 
-STARRED runs much faster on GPUs, so make sure you install a version of
-JAX that is compatible with your version of Cuda and CuDNN:
+-  ``matplotlib``
 
-.. code:: bash
+-  ``numpy``
 
-   pip install "jax[cuda11_cudnn86]" -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
+-  ``scikit-image``
 
-Requirements
-------------
+-  ``scipy``
+
+-  ``optax``
 
-STARRED requires the following Python packages: \* ``astropy`` \*
-``dill`` \* ``jax`` \* ``jaxlib`` \* ``jaxopt`` \* ``matplotlib`` \*
-``numpy`` \* ``scikit-image`` \* ``scipy`` \* ``optax`` \* ``tqdm``
+-  ``tqdm``
 
 Example Notebooks and Documentation
 -----------------------------------
 
 The full documentation can be found
 `here <https://cosmograil.gitlab.io/starred/>`__.
 
 Example notebooks are located in the
 `notebooks <https://gitlab.com/cosmograil/starred/-/tree/main/notebooks>`__
-folder: \* `Ground-based narrow PSF
-generation <https://gitlab.com/cosmograil/starred/-/blob/main/notebooks/1_WFI%20narrow%20PSF%20generation.ipynb>`__
-\* `Ground-based joint
-deconvolution <https://gitlab.com/cosmograil/starred/-/blob/main/notebooks/2_DESJ0602-4335%20joint%20deconvolution.ipynb>`__
-\* `Another ground-based joint
-deconvolution <https://gitlab.com/cosmograil/starred/-/blob/main/notebooks/3_Another%20lensed%20quasar%20-%20joint%20deconvolution.ipynb>`__
-\* `JWST PSF generation and
-deconvolution <https://gitlab.com/cosmograil/starred/-/blob/main/notebooks/4_JWST%20deconvolution.ipynb>`__
-\* `DES2038 joint
-deconvolution <https://gitlab.com/cosmograil/starred/-/blob/main/notebooks/5_DES2038_from_WFI_joint_deconvolution.ipynb>`__
-\* `HST PSF
-reconstruction <https://gitlab.com/cosmograil/starred/-/blob/main/notebooks/6_HST-PSF%20reconstruction.ipynb>`__
+folder:
+
+-  `Ground-based narrow PSF
+   generation <https://gitlab.com/cosmograil/starred/-/blob/main/notebooks/1_WFI%20narrow%20PSF%20generation.ipynb>`__
+
+-  `Ground-based joint
+   deconvolution <https://gitlab.com/cosmograil/starred/-/blob/main/notebooks/2_DESJ0602-4335%20joint%20deconvolution.ipynb>`__
+
+-  `Another ground-based joint
+   deconvolution <https://gitlab.com/cosmograil/starred/-/blob/main/notebooks/3_Another%20lensed%20quasar%20-%20joint%20deconvolution.ipynb>`__
+
+-  `JWST PSF generation and
+   deconvolution <https://gitlab.com/cosmograil/starred/-/blob/main/notebooks/4_JWST%20deconvolution.ipynb>`__
+
+-  `DES2038 joint
+   deconvolution <https://gitlab.com/cosmograil/starred/-/blob/main/notebooks/5_DES2038_from_WFI_joint_deconvolution.ipynb>`__
+
+-  `HST PSF
+   reconstruction <https://gitlab.com/cosmograil/starred/-/blob/main/notebooks/6_HST-PSF%20reconstruction.ipynb>`__
 
 Attribution
 -----------
 
 If you use this code, please cite `Michalewicz et
 al. 2023 <https://joss.theoj.org/papers/10.21105/joss.05340>`__ as
 indicated in the
```

### Comparing `starred-astro-1.1/README.md` & `starred-astro-1.1.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -6,76 +6,72 @@
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.05340/status.svg)](https://doi.org/10.21105/joss.05340)
 
 
 STARlet REgularized Deconvolution (STARRED) is a Python deconvolution method powered by Starlet regularization and JAX automatic differentiation. It uses a Point Spread Function (PSF) narrower than the original one as kernel. 
 
 ## Installation 
-### Through Anaconda
-We provide an Anaconda environment that satisfies all the dependencies in `starred-env.yml`. 
-```bash
-git clone https://gitlab.com/cosmograil/starred.git
-cd starred
-conda env create -f starred-env.yml
-conda activate starred-env
-pip install .
-```
-In case you have an NVIDIA GPU, this should automatically download the right version of JAX as well as cuDNN.
-Next, you can run the tests to make sure your installation is working correctly.
 
-```bash
-# While still in the STARRED directory:
-pytest . 
-```
+### Through PyPI
 
-### Manually handling the dependencies
-If you want to use an existing environment, just omit the Anaconda commands above:
-```bash
-git clone https://gitlab.com/cosmograil/starred
-cd starred 
-pip install .
-```
+STARRED releases are distributed through the Python Package Index (PyPI). To install the latest version use `pip`:
 
-or if you need to install it for your user only: 
 ```bash
-python setup.py install --user 
+$ pip install starred-astro
 ```
 
 STARRED runs much faster on GPUs, so make sure you install a version of JAX that is compatible 
-with your version of Cuda and CuDNN: 
+with your version of CUDA and cuDNN: 
 ``` bash 
-pip install "jax[cuda11_cudnn86]" -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
+$ pip install "jax[cuda11_cudnn86]" -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
 ```
 
 ## Requirements 
 
-STARRED requires the following Python packages: 
+STARRED requires the following Python packages:
+
 * `astropy`
+
 * `dill`
+
 * `jax`
+
 * `jaxlib`
+
 * `jaxopt`
+
 * `matplotlib`
+
 * `numpy`
+
 * `scikit-image`
+
 * `scipy`
+
 * `optax`
+
 * `tqdm`
     
 
 
 ## Example Notebooks and Documentation
 The full documentation can be found [here](https://cosmograil.gitlab.io/starred/). 
 
 Example notebooks are located in the [notebooks](https://gitlab.com/cosmograil/starred/-/tree/main/notebooks) folder: 
+
 * [Ground-based narrow PSF generation](https://gitlab.com/cosmograil/starred/-/blob/main/notebooks/1_WFI%20narrow%20PSF%20generation.ipynb)
+
 * [Ground-based joint deconvolution](https://gitlab.com/cosmograil/starred/-/blob/main/notebooks/2_DESJ0602-4335%20joint%20deconvolution.ipynb)
+
 * [Another ground-based joint deconvolution](https://gitlab.com/cosmograil/starred/-/blob/main/notebooks/3_Another%20lensed%20quasar%20-%20joint%20deconvolution.ipynb)
+
 * [JWST PSF generation and deconvolution](https://gitlab.com/cosmograil/starred/-/blob/main/notebooks/4_JWST%20deconvolution.ipynb)
+
 * [DES2038 joint deconvolution](https://gitlab.com/cosmograil/starred/-/blob/main/notebooks/5_DES2038_from_WFI_joint_deconvolution.ipynb)
+
 * [HST PSF reconstruction](https://gitlab.com/cosmograil/starred/-/blob/main/notebooks/6_HST-PSF%20reconstruction.ipynb)
 
 ## Attribution
 
 If you use this code, please cite [Michalewicz et al. 2023](https://joss.theoj.org/papers/10.21105/joss.05340) as indicated in the [documentation](https://cosmograil.gitlab.io/starred/citing.html).
 
 ## License
```

### Comparing `starred-astro-1.1/setup.py` & `starred-astro-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     import pypandoc
     long_description = pypandoc.convert_file('README.md', 'rst')
 except(IOError, ImportError):
     long_description = open('README.md').read()
 
 setup(
     name='starred-astro',
-    version='1.1',
+    version='1.1.1',
     author='Kevin Michalewicz',
     author_email='kevinmicha@hotmail.com',
     description='A two-channel deconvolution method with Starlet regularization',
     long_description=long_description,
     packages=['starred', 'starred.deconvolution', 'starred.plots', 'starred.psf', 'starred.utils'],
     requires=['astropy', 'dill', 'galsim', 'jax', 'jaxlib', 'jaxopt', 'matplotlib', 'numpy', 'scikitimage', 'scipy', 'optax', 'tqdm'],
     cmdclass={'test': PyTest}
```

### Comparing `starred-astro-1.1/starred/deconvolution/deconvolution.py` & `starred-astro-1.1.1/starred/deconvolution/deconvolution.py`

 * *Files identical despite different names*

### Comparing `starred-astro-1.1/starred/deconvolution/loss.py` & `starred-astro-1.1.1/starred/deconvolution/loss.py`

 * *Files identical despite different names*

### Comparing `starred-astro-1.1/starred/deconvolution/parameters.py` & `starred-astro-1.1.1/starred/deconvolution/parameters.py`

 * *Files identical despite different names*

### Comparing `starred-astro-1.1/starred/plots/f2n.py` & `starred-astro-1.1.1/starred/plots/f2n.py`

 * *Files identical despite different names*

### Comparing `starred-astro-1.1/starred/plots/plot_function.py` & `starred-astro-1.1.1/starred/plots/plot_function.py`

 * *Files identical despite different names*

### Comparing `starred-astro-1.1/starred/psf/loss.py` & `starred-astro-1.1.1/starred/psf/loss.py`

 * *Files identical despite different names*

### Comparing `starred-astro-1.1/starred/psf/parameters.py` & `starred-astro-1.1.1/starred/psf/parameters.py`

 * *Files identical despite different names*

### Comparing `starred-astro-1.1/starred/psf/psf.py` & `starred-astro-1.1.1/starred/psf/psf.py`

 * *Files identical despite different names*

### Comparing `starred-astro-1.1/starred/utils/ds9reg.py` & `starred-astro-1.1.1/starred/utils/ds9reg.py`

 * *Files identical despite different names*

### Comparing `starred-astro-1.1/starred/utils/generic_utils.py` & `starred-astro-1.1.1/starred/utils/generic_utils.py`

 * *Files identical despite different names*

### Comparing `starred-astro-1.1/starred/utils/inference_base.py` & `starred-astro-1.1.1/starred/utils/inference_base.py`

 * *Files identical despite different names*

### Comparing `starred-astro-1.1/starred/utils/jax_utils.py` & `starred-astro-1.1.1/starred/utils/jax_utils.py`

 * *Files identical despite different names*

### Comparing `starred-astro-1.1/starred/utils/noise_utils.py` & `starred-astro-1.1.1/starred/utils/noise_utils.py`

 * *Files identical despite different names*

### Comparing `starred-astro-1.1/starred/utils/optimization.py` & `starred-astro-1.1.1/starred/utils/optimization.py`

 * *Files identical despite different names*

### Comparing `starred-astro-1.1/starred/utils/parameters.py` & `starred-astro-1.1.1/starred/utils/parameters.py`

 * *Files identical despite different names*

### Comparing `starred-astro-1.1/starred_astro.egg-info/PKG-INFO` & `starred-astro-1.1.1/starred_astro.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starred-astro
-Version: 1.1
+Version: 1.1.1
 Summary: A two-channel deconvolution method with Starlet regularization
 Author: Kevin Michalewicz
 Author-email: kevinmicha@hotmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires: astropy
 Requires: dill
@@ -30,89 +30,85 @@
 method powered by Starlet regularization and JAX automatic
 differentiation. It uses a Point Spread Function (PSF) narrower than the
 original one as kernel.
 
 Installation
 ------------
 
-Through Anaconda
-~~~~~~~~~~~~~~~~
+Through PyPI
+~~~~~~~~~~~~
 
-We provide an Anaconda environment that satisfies all the dependencies
-in ``starred-env.yml``.
+STARRED releases are distributed through the Python Package Index
+(PyPI). To install the latest version use ``pip``:
 
 .. code:: bash
 
-   git clone https://gitlab.com/cosmograil/starred.git
-   cd starred
-   conda env create -f starred-env.yml
-   conda activate starred-env
-   pip install .
-
-In case you have an NVIDIA GPU, this should automatically download the
-right version of JAX as well as cuDNN. Next, you can run the tests to
-make sure your installation is working correctly.
+   $ pip install starred-astro
+
+STARRED runs much faster on GPUs, so make sure you install a version of
+JAX that is compatible with your version of CUDA and cuDNN:
 
 .. code:: bash
 
-   # While still in the STARRED directory:
-   pytest . 
+   $ pip install "jax[cuda11_cudnn86]" -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
 
-Manually handling the dependencies
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+Requirements
+------------
 
-If you want to use an existing environment, just omit the Anaconda
-commands above:
+STARRED requires the following Python packages:
 
-.. code:: bash
+-  ``astropy``
 
-   git clone https://gitlab.com/cosmograil/starred
-   cd starred 
-   pip install .
+-  ``dill``
 
-or if you need to install it for your user only:
+-  ``jax``
 
-.. code:: bash
+-  ``jaxlib``
 
-   python setup.py install --user 
+-  ``jaxopt``
 
-STARRED runs much faster on GPUs, so make sure you install a version of
-JAX that is compatible with your version of Cuda and CuDNN:
+-  ``matplotlib``
 
-.. code:: bash
+-  ``numpy``
 
-   pip install "jax[cuda11_cudnn86]" -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
+-  ``scikit-image``
 
-Requirements
-------------
+-  ``scipy``
+
+-  ``optax``
 
-STARRED requires the following Python packages: \* ``astropy`` \*
-``dill`` \* ``jax`` \* ``jaxlib`` \* ``jaxopt`` \* ``matplotlib`` \*
-``numpy`` \* ``scikit-image`` \* ``scipy`` \* ``optax`` \* ``tqdm``
+-  ``tqdm``
 
 Example Notebooks and Documentation
 -----------------------------------
 
 The full documentation can be found
 `here <https://cosmograil.gitlab.io/starred/>`__.
 
 Example notebooks are located in the
 `notebooks <https://gitlab.com/cosmograil/starred/-/tree/main/notebooks>`__
-folder: \* `Ground-based narrow PSF
-generation <https://gitlab.com/cosmograil/starred/-/blob/main/notebooks/1_WFI%20narrow%20PSF%20generation.ipynb>`__
-\* `Ground-based joint
-deconvolution <https://gitlab.com/cosmograil/starred/-/blob/main/notebooks/2_DESJ0602-4335%20joint%20deconvolution.ipynb>`__
-\* `Another ground-based joint
-deconvolution <https://gitlab.com/cosmograil/starred/-/blob/main/notebooks/3_Another%20lensed%20quasar%20-%20joint%20deconvolution.ipynb>`__
-\* `JWST PSF generation and
-deconvolution <https://gitlab.com/cosmograil/starred/-/blob/main/notebooks/4_JWST%20deconvolution.ipynb>`__
-\* `DES2038 joint
-deconvolution <https://gitlab.com/cosmograil/starred/-/blob/main/notebooks/5_DES2038_from_WFI_joint_deconvolution.ipynb>`__
-\* `HST PSF
-reconstruction <https://gitlab.com/cosmograil/starred/-/blob/main/notebooks/6_HST-PSF%20reconstruction.ipynb>`__
+folder:
+
+-  `Ground-based narrow PSF
+   generation <https://gitlab.com/cosmograil/starred/-/blob/main/notebooks/1_WFI%20narrow%20PSF%20generation.ipynb>`__
+
+-  `Ground-based joint
+   deconvolution <https://gitlab.com/cosmograil/starred/-/blob/main/notebooks/2_DESJ0602-4335%20joint%20deconvolution.ipynb>`__
+
+-  `Another ground-based joint
+   deconvolution <https://gitlab.com/cosmograil/starred/-/blob/main/notebooks/3_Another%20lensed%20quasar%20-%20joint%20deconvolution.ipynb>`__
+
+-  `JWST PSF generation and
+   deconvolution <https://gitlab.com/cosmograil/starred/-/blob/main/notebooks/4_JWST%20deconvolution.ipynb>`__
+
+-  `DES2038 joint
+   deconvolution <https://gitlab.com/cosmograil/starred/-/blob/main/notebooks/5_DES2038_from_WFI_joint_deconvolution.ipynb>`__
+
+-  `HST PSF
+   reconstruction <https://gitlab.com/cosmograil/starred/-/blob/main/notebooks/6_HST-PSF%20reconstruction.ipynb>`__
 
 Attribution
 -----------
 
 If you use this code, please cite `Michalewicz et
 al. 2023 <https://joss.theoj.org/papers/10.21105/joss.05340>`__ as
 indicated in the
```

### Comparing `starred-astro-1.1/starred_astro.egg-info/SOURCES.txt` & `starred-astro-1.1.1/starred_astro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

