# Comparing `tmp/acwater-0.3.1.tar.gz` & `tmp/acwater-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acwater-0.3.1.tar", last modified: Fri May 26 11:52:17 2023, max compression
+gzip compressed data, was "acwater-0.3.2.tar", last modified: Fri May 26 16:38:31 2023, max compression
```

## Comparing `acwater-0.3.1.tar` & `acwater-0.3.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxr-x   0 alvarado  (9086) alvarado  (9086)        0 2023-05-26 11:52:17.423237 acwater-0.3.1/
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      292 2022-03-07 14:51:52.000000 acwater-0.3.1/.editorconfig
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     3516 2022-03-07 14:51:52.000000 acwater-0.3.1/.gitignore
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     4210 2023-02-07 14:14:47.000000 acwater-0.3.1/.gitlab-ci.yml
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      206 2023-02-20 10:38:31.000000 acwater-0.3.1/AUTHORS.rst
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     3570 2023-02-20 10:38:31.000000 acwater-0.3.1/CONTRIBUTING.rst
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      137 2023-02-20 10:38:31.000000 acwater-0.3.1/HISTORY.rst
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      259 2022-03-07 14:51:52.000000 acwater-0.3.1/ISSUE_TEMPLATE.md
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     3475 2023-02-20 10:38:31.000000 acwater-0.3.1/LICENSE
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      263 2023-03-10 13:52:20.000000 acwater-0.3.1/MANIFEST.in
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     2298 2023-03-10 13:52:20.000000 acwater-0.3.1/Makefile
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     3840 2023-05-26 11:52:17.423237 acwater-0.3.1/PKG-INFO
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     2775 2023-05-26 11:22:49.000000 acwater-0.3.1/README.md
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     2856 2023-05-26 11:51:04.000000 acwater-0.3.1/README.rst
-drwxrwxr-x   0 alvarado  (9086) alvarado  (9086)        0 2023-05-26 11:52:17.419237 acwater-0.3.1/acwater/
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      169 2023-05-26 11:12:12.000000 acwater-0.3.1/acwater/__init__.py
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     9463 2023-05-26 11:05:53.000000 acwater-0.3.1/acwater/acwater.py
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      436 2022-03-07 14:51:52.000000 acwater-0.3.1/acwater/cli.py
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     3458 2023-02-20 10:38:31.000000 acwater-0.3.1/acwater/enpt_config.py
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)    15155 2023-02-20 10:38:31.000000 acwater-0.3.1/acwater/level1_enmap.py
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     6790 2023-03-10 13:52:20.000000 acwater-0.3.1/acwater/polymer_enmap.py
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     7988 2023-02-20 10:38:31.000000 acwater-0.3.1/acwater/writer.py
-drwxrwxr-x   0 alvarado  (9086) alvarado  (9086)        0 2023-05-26 11:52:17.419237 acwater-0.3.1/acwater.egg-info/
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     3840 2023-05-26 11:52:17.000000 acwater-0.3.1/acwater.egg-info/PKG-INFO
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      957 2023-05-26 11:52:17.000000 acwater-0.3.1/acwater.egg-info/SOURCES.txt
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)        1 2023-05-26 11:52:17.000000 acwater-0.3.1/acwater.egg-info/dependency_links.txt
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)       45 2023-05-26 11:52:17.000000 acwater-0.3.1/acwater.egg-info/entry_points.txt
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)        1 2022-03-09 17:10:38.000000 acwater-0.3.1/acwater.egg-info/not-zip-safe
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)        8 2023-05-26 11:52:17.000000 acwater-0.3.1/acwater.egg-info/top_level.txt
-drwxrwxr-x   0 alvarado  (9086) alvarado  (9086)        0 2023-05-26 11:52:17.423237 acwater-0.3.1/docs/
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      608 2022-03-07 14:51:52.000000 acwater-0.3.1/docs/Makefile
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     1007 2022-03-07 14:51:52.000000 acwater-0.3.1/docs/acwater.rst
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)       28 2022-03-07 14:51:52.000000 acwater-0.3.1/docs/authors.rst
--rwxrwxr-x   0 alvarado  (9086) alvarado  (9086)     4781 2022-03-07 14:51:52.000000 acwater-0.3.1/docs/conf.py
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)       33 2022-03-07 14:51:52.000000 acwater-0.3.1/docs/contributing.rst
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)       28 2022-03-07 14:51:52.000000 acwater-0.3.1/docs/history.rst
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      342 2022-03-07 14:51:52.000000 acwater-0.3.1/docs/index.rst
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     7916 2023-03-10 14:10:00.000000 acwater-0.3.1/docs/installation.rst
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      790 2022-03-07 14:51:52.000000 acwater-0.3.1/docs/instructions_dev.rst
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      769 2022-03-07 14:51:52.000000 acwater-0.3.1/docs/make.bat
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)       58 2022-03-07 14:51:52.000000 acwater-0.3.1/docs/modules.rst
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)       27 2022-03-07 14:51:52.000000 acwater-0.3.1/docs/readme.rst
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     1397 2022-03-07 14:51:52.000000 acwater-0.3.1/docs/tutorial.rst
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)       69 2022-03-07 14:51:52.000000 acwater-0.3.1/docs/usage.rst
--rwxrwxr-x   0 alvarado  (9086) alvarado  (9086)      175 2022-03-07 14:51:52.000000 acwater-0.3.1/environment.yml
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      559 2022-03-07 14:51:52.000000 acwater-0.3.1/polymer_env.yml
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)        6 2022-03-07 14:51:52.000000 acwater-0.3.1/requirements.txt
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      134 2022-03-07 14:51:52.000000 acwater-0.3.1/requirements_dev.txt
-drwxrwxr-x   0 alvarado  (9086) alvarado  (9086)        0 2023-05-26 11:52:17.423237 acwater-0.3.1/sciadrive/
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)        0 2022-03-07 14:51:52.000000 acwater-0.3.1/sciadrive/__init__.py
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)    24739 2023-02-20 10:38:31.000000 acwater-0.3.1/sciadrive/build_ascii.py
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     6678 2023-05-26 11:07:04.000000 acwater-0.3.1/sciadrive/example_ascii.py
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)    56150 2022-03-07 14:51:52.000000 acwater-0.3.1/sciadrive/extraction_reshape.csv
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     3635 2023-02-20 10:38:31.000000 acwater-0.3.1/sciadrive/reshape_spektrum.py
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      390 2023-05-26 11:52:17.423237 acwater-0.3.1/setup.cfg
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     1567 2023-05-26 11:12:55.000000 acwater-0.3.1/setup.py
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      308 2023-02-20 10:38:31.000000 acwater-0.3.1/tox.ini
+drwxrwxr-x   0 alvarado  (9086) alvarado  (9086)        0 2023-05-26 16:38:31.975360 acwater-0.3.2/
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      292 2022-03-07 14:51:52.000000 acwater-0.3.2/.editorconfig
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     3516 2022-03-07 14:51:52.000000 acwater-0.3.2/.gitignore
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     4210 2023-02-07 14:14:47.000000 acwater-0.3.2/.gitlab-ci.yml
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      206 2023-02-20 10:38:31.000000 acwater-0.3.2/AUTHORS.rst
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     3570 2023-02-20 10:38:31.000000 acwater-0.3.2/CONTRIBUTING.rst
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      137 2023-02-20 10:38:31.000000 acwater-0.3.2/HISTORY.rst
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      259 2022-03-07 14:51:52.000000 acwater-0.3.2/ISSUE_TEMPLATE.md
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     3475 2023-02-20 10:38:31.000000 acwater-0.3.2/LICENSE
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      263 2023-03-10 13:52:20.000000 acwater-0.3.2/MANIFEST.in
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     2298 2023-03-10 13:52:20.000000 acwater-0.3.2/Makefile
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     3840 2023-05-26 16:38:31.975360 acwater-0.3.2/PKG-INFO
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     2775 2023-05-26 11:22:49.000000 acwater-0.3.2/README.md
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     2856 2023-05-26 11:51:04.000000 acwater-0.3.2/README.rst
+drwxrwxr-x   0 alvarado  (9086) alvarado  (9086)        0 2023-05-26 16:38:31.971361 acwater-0.3.2/acwater/
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      169 2023-05-26 16:38:17.000000 acwater-0.3.2/acwater/__init__.py
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     9467 2023-05-26 16:34:35.000000 acwater-0.3.2/acwater/acwater.py
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      436 2022-03-07 14:51:52.000000 acwater-0.3.2/acwater/cli.py
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     3458 2023-02-20 10:38:31.000000 acwater-0.3.2/acwater/enpt_config.py
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)    15155 2023-02-20 10:38:31.000000 acwater-0.3.2/acwater/level1_enmap.py
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     6790 2023-03-10 13:52:20.000000 acwater-0.3.2/acwater/polymer_enmap.py
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     7988 2023-02-20 10:38:31.000000 acwater-0.3.2/acwater/writer.py
+drwxrwxr-x   0 alvarado  (9086) alvarado  (9086)        0 2023-05-26 16:38:31.971361 acwater-0.3.2/acwater.egg-info/
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     3840 2023-05-26 16:38:31.000000 acwater-0.3.2/acwater.egg-info/PKG-INFO
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      957 2023-05-26 16:38:31.000000 acwater-0.3.2/acwater.egg-info/SOURCES.txt
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)        1 2023-05-26 16:38:31.000000 acwater-0.3.2/acwater.egg-info/dependency_links.txt
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)       45 2023-05-26 16:38:31.000000 acwater-0.3.2/acwater.egg-info/entry_points.txt
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)        1 2022-03-09 17:10:38.000000 acwater-0.3.2/acwater.egg-info/not-zip-safe
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)        8 2023-05-26 16:38:31.000000 acwater-0.3.2/acwater.egg-info/top_level.txt
+drwxrwxr-x   0 alvarado  (9086) alvarado  (9086)        0 2023-05-26 16:38:31.975360 acwater-0.3.2/docs/
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      608 2022-03-07 14:51:52.000000 acwater-0.3.2/docs/Makefile
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     1007 2022-03-07 14:51:52.000000 acwater-0.3.2/docs/acwater.rst
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)       28 2022-03-07 14:51:52.000000 acwater-0.3.2/docs/authors.rst
+-rwxrwxr-x   0 alvarado  (9086) alvarado  (9086)     4781 2022-03-07 14:51:52.000000 acwater-0.3.2/docs/conf.py
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)       33 2022-03-07 14:51:52.000000 acwater-0.3.2/docs/contributing.rst
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)       28 2022-03-07 14:51:52.000000 acwater-0.3.2/docs/history.rst
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      342 2022-03-07 14:51:52.000000 acwater-0.3.2/docs/index.rst
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     7916 2023-03-10 14:10:00.000000 acwater-0.3.2/docs/installation.rst
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      790 2022-03-07 14:51:52.000000 acwater-0.3.2/docs/instructions_dev.rst
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      769 2022-03-07 14:51:52.000000 acwater-0.3.2/docs/make.bat
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)       58 2022-03-07 14:51:52.000000 acwater-0.3.2/docs/modules.rst
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)       27 2022-03-07 14:51:52.000000 acwater-0.3.2/docs/readme.rst
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     1397 2022-03-07 14:51:52.000000 acwater-0.3.2/docs/tutorial.rst
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)       69 2022-03-07 14:51:52.000000 acwater-0.3.2/docs/usage.rst
+-rwxrwxr-x   0 alvarado  (9086) alvarado  (9086)      175 2022-03-07 14:51:52.000000 acwater-0.3.2/environment.yml
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      559 2022-03-07 14:51:52.000000 acwater-0.3.2/polymer_env.yml
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)        6 2022-03-07 14:51:52.000000 acwater-0.3.2/requirements.txt
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      134 2022-03-07 14:51:52.000000 acwater-0.3.2/requirements_dev.txt
+drwxrwxr-x   0 alvarado  (9086) alvarado  (9086)        0 2023-05-26 16:38:31.975360 acwater-0.3.2/sciadrive/
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)        0 2022-03-07 14:51:52.000000 acwater-0.3.2/sciadrive/__init__.py
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)    24739 2023-02-20 10:38:31.000000 acwater-0.3.2/sciadrive/build_ascii.py
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     6678 2023-05-26 11:07:04.000000 acwater-0.3.2/sciadrive/example_ascii.py
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)    56150 2022-03-07 14:51:52.000000 acwater-0.3.2/sciadrive/extraction_reshape.csv
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     3635 2023-02-20 10:38:31.000000 acwater-0.3.2/sciadrive/reshape_spektrum.py
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      390 2023-05-26 16:38:31.975360 acwater-0.3.2/setup.cfg
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     1567 2023-05-26 16:38:17.000000 acwater-0.3.2/setup.py
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      308 2023-02-20 10:38:31.000000 acwater-0.3.2/tox.ini
```

### Comparing `acwater-0.3.1/.gitignore` & `acwater-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `acwater-0.3.1/.gitlab-ci.yml` & `acwater-0.3.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `acwater-0.3.1/CONTRIBUTING.rst` & `acwater-0.3.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `acwater-0.3.1/LICENSE` & `acwater-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `acwater-0.3.1/Makefile` & `acwater-0.3.2/Makefile`

 * *Files identical despite different names*

### Comparing `acwater-0.3.1/PKG-INFO` & `acwater-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acwater
-Version: 0.3.1
+Version: 0.3.2
 Summary: Atmospheric correction of EnMAP satellite data over water using Polymer algorithm
 Home-page: https://gitlab.awi.de/phytooptics/acwater
 Author: Leonado Alvarado
 Author-email: leonardo.alvarado@awi.de
 License: GNU General Public License v3
 Keywords: acwater
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `acwater-0.3.1/README.md` & `acwater-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `acwater-0.3.1/README.rst` & `acwater-0.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `acwater-0.3.1/acwater/acwater.py` & `acwater-0.3.2/acwater/acwater.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,16 +188,16 @@
         enmap_l2a_swir = np.ones(enmap_l1b.swir.data.shape, dtype=float) / config.scale_factor_boa_ref
     elif detector == 'merge' or detector == 'vnswir':
         enmap_l2a_vnir = product.Rw[:, :, ibands_vnir]
         enmap_l2a_swir = product.Rw[:, :, ibands_swir]
         enmap_l2a_swir = enmap_l1b.transform_vnir_to_swir_raster(enmap_l2a_swir)
 
     # Feature for other products can be returned separately as in:
-    # return enmap_l2a_vnir, enmap_l2a_swir, product.logchl, product.bbs, product.bitmask, product.Rgli, product.Rnir
+    # return enmap_l2a_vnir, enmap_l2a_swir, product.logchl, product.logfb, product.bitmask, product.Rgli, product.Rnir
     # or combined in an additional output as in
     enmap_products = {'polymer_logchl' : product.logchl,
-                    'polymer_logfb' : product.bbs,
+                    'polymer_logfb' : product.logfb,
                     'polymer_rgli' : product.Rgli ,
                     'polymer_rnir' : product.Rnir ,
                     'polymer_bitmask' : np.array(product.bitmask, dtype=np.int16) }
 
     return enmap_l2a_vnir, enmap_l2a_swir, enmap_products
```

### Comparing `acwater-0.3.1/acwater/enpt_config.py` & `acwater-0.3.2/acwater/enpt_config.py`

 * *Files identical despite different names*

### Comparing `acwater-0.3.1/acwater/level1_enmap.py` & `acwater-0.3.2/acwater/level1_enmap.py`

 * *Files identical despite different names*

### Comparing `acwater-0.3.1/acwater/polymer_enmap.py` & `acwater-0.3.2/acwater/polymer_enmap.py`

 * *Files identical despite different names*

### Comparing `acwater-0.3.1/acwater/writer.py` & `acwater-0.3.2/acwater/writer.py`

 * *Files identical despite different names*

### Comparing `acwater-0.3.1/acwater.egg-info/PKG-INFO` & `acwater-0.3.2/acwater.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acwater
-Version: 0.3.1
+Version: 0.3.2
 Summary: Atmospheric correction of EnMAP satellite data over water using Polymer algorithm
 Home-page: https://gitlab.awi.de/phytooptics/acwater
 Author: Leonado Alvarado
 Author-email: leonardo.alvarado@awi.de
 License: GNU General Public License v3
 Keywords: acwater
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `acwater-0.3.1/acwater.egg-info/SOURCES.txt` & `acwater-0.3.2/acwater.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acwater-0.3.1/docs/Makefile` & `acwater-0.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `acwater-0.3.1/docs/acwater.rst` & `acwater-0.3.2/docs/acwater.rst`

 * *Files identical despite different names*

### Comparing `acwater-0.3.1/docs/conf.py` & `acwater-0.3.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `acwater-0.3.1/docs/installation.rst` & `acwater-0.3.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `acwater-0.3.1/docs/instructions_dev.rst` & `acwater-0.3.2/docs/instructions_dev.rst`

 * *Files identical despite different names*

### Comparing `acwater-0.3.1/docs/make.bat` & `acwater-0.3.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `acwater-0.3.1/docs/tutorial.rst` & `acwater-0.3.2/docs/tutorial.rst`

 * *Files identical despite different names*

### Comparing `acwater-0.3.1/polymer_env.yml` & `acwater-0.3.2/polymer_env.yml`

 * *Files identical despite different names*

### Comparing `acwater-0.3.1/sciadrive/build_ascii.py` & `acwater-0.3.2/sciadrive/build_ascii.py`

 * *Files identical despite different names*

### Comparing `acwater-0.3.1/sciadrive/example_ascii.py` & `acwater-0.3.2/sciadrive/example_ascii.py`

 * *Files identical despite different names*

### Comparing `acwater-0.3.1/sciadrive/extraction_reshape.csv` & `acwater-0.3.2/sciadrive/extraction_reshape.csv`

 * *Files identical despite different names*

### Comparing `acwater-0.3.1/sciadrive/reshape_spektrum.py` & `acwater-0.3.2/sciadrive/reshape_spektrum.py`

 * *Files identical despite different names*

### Comparing `acwater-0.3.1/setup.py` & `acwater-0.3.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -44,10 +44,10 @@
     keywords='acwater',
     name='acwater',
     packages=find_packages(include=['acwater', 'acwater.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://gitlab.awi.de/phytooptics/acwater',
-    version='0.3.1',
+    version='0.3.2',
     zip_safe=False,
 )
```

