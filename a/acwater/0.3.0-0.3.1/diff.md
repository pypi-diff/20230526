# Comparing `tmp/acwater-0.3.0.tar.gz` & `tmp/acwater-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acwater-0.3.0.tar", last modified: Mon Feb 20 11:34:48 2023, max compression
+gzip compressed data, was "acwater-0.3.1.tar", last modified: Fri May 26 11:52:17 2023, max compression
```

## Comparing `acwater-0.3.0.tar` & `acwater-0.3.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxr-x   0 alvarado  (9086) alvarado  (9086)        0 2023-02-20 11:34:48.768115 acwater-0.3.0/
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      292 2022-03-07 14:51:52.000000 acwater-0.3.0/.editorconfig
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     3516 2022-03-07 14:51:52.000000 acwater-0.3.0/.gitignore
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     4210 2023-02-07 14:14:47.000000 acwater-0.3.0/.gitlab-ci.yml
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      206 2023-02-20 10:38:31.000000 acwater-0.3.0/AUTHORS.rst
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     3570 2023-02-20 10:38:31.000000 acwater-0.3.0/CONTRIBUTING.rst
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      137 2023-02-20 10:38:31.000000 acwater-0.3.0/HISTORY.rst
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      259 2022-03-07 14:51:52.000000 acwater-0.3.0/ISSUE_TEMPLATE.md
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     3475 2023-02-20 10:38:31.000000 acwater-0.3.0/LICENSE
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      263 2023-02-20 10:41:21.000000 acwater-0.3.0/MANIFEST.in
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     2298 2023-02-20 10:41:21.000000 acwater-0.3.0/Makefile
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     2562 2023-02-20 11:34:48.768115 acwater-0.3.0/PKG-INFO
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     1509 2023-02-20 10:38:31.000000 acwater-0.3.0/README.md
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     1578 2022-03-07 14:51:52.000000 acwater-0.3.0/README.rst
-drwxrwxr-x   0 alvarado  (9086) alvarado  (9086)        0 2023-02-20 11:34:48.764115 acwater-0.3.0/acwater/
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      169 2023-02-20 10:38:31.000000 acwater-0.3.0/acwater/__init__.py
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     9439 2023-02-20 10:56:15.000000 acwater-0.3.0/acwater/acwater.py
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      436 2022-03-07 14:51:52.000000 acwater-0.3.0/acwater/cli.py
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     3458 2023-02-20 10:38:31.000000 acwater-0.3.0/acwater/enpt_config.py
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)    15155 2023-02-20 10:38:31.000000 acwater-0.3.0/acwater/level1_enmap.py
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     6790 2023-02-20 10:41:21.000000 acwater-0.3.0/acwater/polymer_enmap.py
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     7988 2023-02-20 10:38:31.000000 acwater-0.3.0/acwater/writer.py
-drwxrwxr-x   0 alvarado  (9086) alvarado  (9086)        0 2023-02-20 11:34:48.764115 acwater-0.3.0/acwater.egg-info/
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     2562 2023-02-20 11:34:48.000000 acwater-0.3.0/acwater.egg-info/PKG-INFO
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      957 2023-02-20 11:34:48.000000 acwater-0.3.0/acwater.egg-info/SOURCES.txt
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)        1 2023-02-20 11:34:48.000000 acwater-0.3.0/acwater.egg-info/dependency_links.txt
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)       45 2023-02-20 11:34:48.000000 acwater-0.3.0/acwater.egg-info/entry_points.txt
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)        1 2022-03-09 17:10:38.000000 acwater-0.3.0/acwater.egg-info/not-zip-safe
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)        8 2023-02-20 11:34:48.000000 acwater-0.3.0/acwater.egg-info/top_level.txt
-drwxrwxr-x   0 alvarado  (9086) alvarado  (9086)        0 2023-02-20 11:34:48.764115 acwater-0.3.0/docs/
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      608 2022-03-07 14:51:52.000000 acwater-0.3.0/docs/Makefile
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     1007 2022-03-07 14:51:52.000000 acwater-0.3.0/docs/acwater.rst
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)       28 2022-03-07 14:51:52.000000 acwater-0.3.0/docs/authors.rst
--rwxrwxr-x   0 alvarado  (9086) alvarado  (9086)     4781 2022-03-07 14:51:52.000000 acwater-0.3.0/docs/conf.py
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)       33 2022-03-07 14:51:52.000000 acwater-0.3.0/docs/contributing.rst
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)       28 2022-03-07 14:51:52.000000 acwater-0.3.0/docs/history.rst
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      342 2022-03-07 14:51:52.000000 acwater-0.3.0/docs/index.rst
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     6036 2022-12-14 10:58:02.000000 acwater-0.3.0/docs/installation.rst
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      790 2022-03-07 14:51:52.000000 acwater-0.3.0/docs/instructions_dev.rst
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      769 2022-03-07 14:51:52.000000 acwater-0.3.0/docs/make.bat
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)       58 2022-03-07 14:51:52.000000 acwater-0.3.0/docs/modules.rst
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)       27 2022-03-07 14:51:52.000000 acwater-0.3.0/docs/readme.rst
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     1397 2022-03-07 14:51:52.000000 acwater-0.3.0/docs/tutorial.rst
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)       69 2022-03-07 14:51:52.000000 acwater-0.3.0/docs/usage.rst
--rwxrwxr-x   0 alvarado  (9086) alvarado  (9086)      175 2022-03-07 14:51:52.000000 acwater-0.3.0/environment.yml
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      559 2022-03-07 14:51:52.000000 acwater-0.3.0/polymer_env.yml
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)        6 2022-03-07 14:51:52.000000 acwater-0.3.0/requirements.txt
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      134 2022-03-07 14:51:52.000000 acwater-0.3.0/requirements_dev.txt
-drwxrwxr-x   0 alvarado  (9086) alvarado  (9086)        0 2023-02-20 11:34:48.768115 acwater-0.3.0/sciadrive/
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)        0 2022-03-07 14:51:52.000000 acwater-0.3.0/sciadrive/__init__.py
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)    24739 2023-02-20 10:38:31.000000 acwater-0.3.0/sciadrive/build_ascii.py
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     6624 2023-02-20 10:38:31.000000 acwater-0.3.0/sciadrive/example_ascii.py
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)    56150 2022-03-07 14:51:52.000000 acwater-0.3.0/sciadrive/extraction_reshape.csv
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     3635 2023-02-20 10:38:31.000000 acwater-0.3.0/sciadrive/reshape_spektrum.py
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      390 2023-02-20 11:34:48.768115 acwater-0.3.0/setup.cfg
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     1567 2023-02-20 10:38:31.000000 acwater-0.3.0/setup.py
--rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      308 2023-02-20 10:38:31.000000 acwater-0.3.0/tox.ini
+drwxrwxr-x   0 alvarado  (9086) alvarado  (9086)        0 2023-05-26 11:52:17.423237 acwater-0.3.1/
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      292 2022-03-07 14:51:52.000000 acwater-0.3.1/.editorconfig
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     3516 2022-03-07 14:51:52.000000 acwater-0.3.1/.gitignore
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     4210 2023-02-07 14:14:47.000000 acwater-0.3.1/.gitlab-ci.yml
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      206 2023-02-20 10:38:31.000000 acwater-0.3.1/AUTHORS.rst
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     3570 2023-02-20 10:38:31.000000 acwater-0.3.1/CONTRIBUTING.rst
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      137 2023-02-20 10:38:31.000000 acwater-0.3.1/HISTORY.rst
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      259 2022-03-07 14:51:52.000000 acwater-0.3.1/ISSUE_TEMPLATE.md
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     3475 2023-02-20 10:38:31.000000 acwater-0.3.1/LICENSE
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      263 2023-03-10 13:52:20.000000 acwater-0.3.1/MANIFEST.in
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     2298 2023-03-10 13:52:20.000000 acwater-0.3.1/Makefile
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     3840 2023-05-26 11:52:17.423237 acwater-0.3.1/PKG-INFO
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     2775 2023-05-26 11:22:49.000000 acwater-0.3.1/README.md
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     2856 2023-05-26 11:51:04.000000 acwater-0.3.1/README.rst
+drwxrwxr-x   0 alvarado  (9086) alvarado  (9086)        0 2023-05-26 11:52:17.419237 acwater-0.3.1/acwater/
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      169 2023-05-26 11:12:12.000000 acwater-0.3.1/acwater/__init__.py
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     9463 2023-05-26 11:05:53.000000 acwater-0.3.1/acwater/acwater.py
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      436 2022-03-07 14:51:52.000000 acwater-0.3.1/acwater/cli.py
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     3458 2023-02-20 10:38:31.000000 acwater-0.3.1/acwater/enpt_config.py
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)    15155 2023-02-20 10:38:31.000000 acwater-0.3.1/acwater/level1_enmap.py
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     6790 2023-03-10 13:52:20.000000 acwater-0.3.1/acwater/polymer_enmap.py
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     7988 2023-02-20 10:38:31.000000 acwater-0.3.1/acwater/writer.py
+drwxrwxr-x   0 alvarado  (9086) alvarado  (9086)        0 2023-05-26 11:52:17.419237 acwater-0.3.1/acwater.egg-info/
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     3840 2023-05-26 11:52:17.000000 acwater-0.3.1/acwater.egg-info/PKG-INFO
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      957 2023-05-26 11:52:17.000000 acwater-0.3.1/acwater.egg-info/SOURCES.txt
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)        1 2023-05-26 11:52:17.000000 acwater-0.3.1/acwater.egg-info/dependency_links.txt
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)       45 2023-05-26 11:52:17.000000 acwater-0.3.1/acwater.egg-info/entry_points.txt
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)        1 2022-03-09 17:10:38.000000 acwater-0.3.1/acwater.egg-info/not-zip-safe
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)        8 2023-05-26 11:52:17.000000 acwater-0.3.1/acwater.egg-info/top_level.txt
+drwxrwxr-x   0 alvarado  (9086) alvarado  (9086)        0 2023-05-26 11:52:17.423237 acwater-0.3.1/docs/
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      608 2022-03-07 14:51:52.000000 acwater-0.3.1/docs/Makefile
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     1007 2022-03-07 14:51:52.000000 acwater-0.3.1/docs/acwater.rst
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)       28 2022-03-07 14:51:52.000000 acwater-0.3.1/docs/authors.rst
+-rwxrwxr-x   0 alvarado  (9086) alvarado  (9086)     4781 2022-03-07 14:51:52.000000 acwater-0.3.1/docs/conf.py
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)       33 2022-03-07 14:51:52.000000 acwater-0.3.1/docs/contributing.rst
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)       28 2022-03-07 14:51:52.000000 acwater-0.3.1/docs/history.rst
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      342 2022-03-07 14:51:52.000000 acwater-0.3.1/docs/index.rst
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     7916 2023-03-10 14:10:00.000000 acwater-0.3.1/docs/installation.rst
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      790 2022-03-07 14:51:52.000000 acwater-0.3.1/docs/instructions_dev.rst
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      769 2022-03-07 14:51:52.000000 acwater-0.3.1/docs/make.bat
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)       58 2022-03-07 14:51:52.000000 acwater-0.3.1/docs/modules.rst
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)       27 2022-03-07 14:51:52.000000 acwater-0.3.1/docs/readme.rst
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     1397 2022-03-07 14:51:52.000000 acwater-0.3.1/docs/tutorial.rst
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)       69 2022-03-07 14:51:52.000000 acwater-0.3.1/docs/usage.rst
+-rwxrwxr-x   0 alvarado  (9086) alvarado  (9086)      175 2022-03-07 14:51:52.000000 acwater-0.3.1/environment.yml
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      559 2022-03-07 14:51:52.000000 acwater-0.3.1/polymer_env.yml
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)        6 2022-03-07 14:51:52.000000 acwater-0.3.1/requirements.txt
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      134 2022-03-07 14:51:52.000000 acwater-0.3.1/requirements_dev.txt
+drwxrwxr-x   0 alvarado  (9086) alvarado  (9086)        0 2023-05-26 11:52:17.423237 acwater-0.3.1/sciadrive/
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)        0 2022-03-07 14:51:52.000000 acwater-0.3.1/sciadrive/__init__.py
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)    24739 2023-02-20 10:38:31.000000 acwater-0.3.1/sciadrive/build_ascii.py
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     6678 2023-05-26 11:07:04.000000 acwater-0.3.1/sciadrive/example_ascii.py
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)    56150 2022-03-07 14:51:52.000000 acwater-0.3.1/sciadrive/extraction_reshape.csv
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     3635 2023-02-20 10:38:31.000000 acwater-0.3.1/sciadrive/reshape_spektrum.py
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      390 2023-05-26 11:52:17.423237 acwater-0.3.1/setup.cfg
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)     1567 2023-05-26 11:12:55.000000 acwater-0.3.1/setup.py
+-rw-rw-r--   0 alvarado  (9086) alvarado  (9086)      308 2023-02-20 10:38:31.000000 acwater-0.3.1/tox.ini
```

### Comparing `acwater-0.3.0/.gitignore` & `acwater-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `acwater-0.3.0/.gitlab-ci.yml` & `acwater-0.3.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `acwater-0.3.0/CONTRIBUTING.rst` & `acwater-0.3.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `acwater-0.3.0/LICENSE` & `acwater-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `acwater-0.3.0/Makefile` & `acwater-0.3.1/Makefile`

 * *Files identical despite different names*

### Comparing `acwater-0.3.0/acwater/acwater.py` & `acwater-0.3.1/acwater/acwater.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,17 @@
 # You should have received a copy of the GNU Lesser General Public License along
 # with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 """ The acwater module calls Polymer (Hygeos) using EnPT (GFZ/EnMAP) parameters.
 
 """
 
-from polymer.main import run_atm_corr, Level2
+from polymer.main import run_atm_corr
+
+from polymer.level2 import Level2
 
 from acwater.polymer_enmap import params_enmap, filter_bands
 
 from acwater.level1_enmap import Level1_ENMAP
 
 from enpt.options.config import EnPTConfig
 
@@ -179,15 +181,15 @@
                            thres_Rcloud=0.2,
                            thres_Rcloud_std=0.04
                            )
 
 
     if detector == 'vnir':
         enmap_l2a_vnir = product.Rw[:, :, ibands_vnir]
-        enmap_l2a_swir = np.ones(enmap_l1b.swir.data.shape, dtype=np.float) / config.scale_factor_boa_ref
+        enmap_l2a_swir = np.ones(enmap_l1b.swir.data.shape, dtype=float) / config.scale_factor_boa_ref
     elif detector == 'merge' or detector == 'vnswir':
         enmap_l2a_vnir = product.Rw[:, :, ibands_vnir]
         enmap_l2a_swir = product.Rw[:, :, ibands_swir]
         enmap_l2a_swir = enmap_l1b.transform_vnir_to_swir_raster(enmap_l2a_swir)
 
     # Feature for other products can be returned separately as in:
     # return enmap_l2a_vnir, enmap_l2a_swir, product.logchl, product.bbs, product.bitmask, product.Rgli, product.Rnir
```

### Comparing `acwater-0.3.0/acwater/enpt_config.py` & `acwater-0.3.1/acwater/enpt_config.py`

 * *Files identical despite different names*

### Comparing `acwater-0.3.0/acwater/level1_enmap.py` & `acwater-0.3.1/acwater/level1_enmap.py`

 * *Files identical despite different names*

### Comparing `acwater-0.3.0/acwater/polymer_enmap.py` & `acwater-0.3.1/acwater/polymer_enmap.py`

 * *Files identical despite different names*

### Comparing `acwater-0.3.0/acwater/writer.py` & `acwater-0.3.1/acwater/writer.py`

 * *Files identical despite different names*

### Comparing `acwater-0.3.0/acwater.egg-info/SOURCES.txt` & `acwater-0.3.1/acwater.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acwater-0.3.0/docs/Makefile` & `acwater-0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `acwater-0.3.0/docs/acwater.rst` & `acwater-0.3.1/docs/acwater.rst`

 * *Files identical despite different names*

### Comparing `acwater-0.3.0/docs/conf.py` & `acwater-0.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `acwater-0.3.0/docs/installation.rst` & `acwater-0.3.1/docs/installation.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,74 @@
 .. _installation:
 
 Installation
 =============
 
-**ACwater Polymer** installation consists basically in cloning and installing
-the module and its dependencies using a python package manager.
-The aim is to install Polymer, ACwater, and EnPT in the same environment.
+The installation process for **ACwater** involves cloning and installing the module and its
+dependencies using a Python package manager. The objective is to install EnPT, Polymer,
+and ACwater in the same environment.
 
 =================
 User
 =================
 
 Linux Debian/Ubuntu
+=================
+
+=========================================================================================================
+
+**Installing ACwater/EnPT as standalone package (no GUI)**
+
+1. Install **EnPT** using mamba forge as decribed in https://enmap.git-pages.gfz-potsdam.de/GFZ_Tools_EnMAP_BOX/EnPT/doc/installation.html
+
+2. Using the previously created enpt conda environment (as described above), first install some dependencies:
+
+.. code:: console
+
+    mamba activate enpt
+    mamba install -c conda-forge cdsapi cython ecmwf-api-client gdal netcdf4 pygrib pyhdf xarray
+
+3. Then register at the HYGEOS support forum, download polymer from there, unpack it and run the following commands from the unpacked root directory of polymer:
+
+.. code:: console
+
+    make
+    make auxdata_common
+    make ancillary
+    mkdir -p ANCILLARY/ERA5/
+    pip install -e .
+
+Ancillary data
+=================
+
+The **ERA5 reanalysis data** is the default option for ancillary data in ACwater Polymer.
+Please register at the `CDS registration page`_ and install the `CDS API key`_
+by creating a key file with your registration data, as follows:
+
+.. _CDS registration page: https://cds.climate.copernicus.eu
+.. _CDS API key: https://cds.climate.copernicus.eu/api-how-to
+
+.. code:: console
+
+    CDS_API_KEY="copy your key here"
+    touch $HOME/.cdsapirc
+    echo "url: https://cds.climate.copernicus.eu/api/v2" >> $HOME/.cdsapirc
+    echo "key: $CDS_API_KEY" >> $HOME/.cdsapirc
+
+.. _`Polymer server`: http://download.hygeos.com/POLYMER/auxdata
+
+4. Install **ACwater**
+
+.. code:: console
+
+    pip install acwater>=0.3.0
+    
+============================================================================================================
+
+**Installing ACwater/EnPT along with the EnMAP-Box (a QGIS plugin) which provides a GUI for EnPT**
 
 **Install** QGIS as in `QGIS instructions`_
 
 .. _QGIS instructions: https://www.qgis.org/en/site/forusers/alldownloads.html#debian-ubuntu
 
 .. code:: console
 
@@ -42,15 +95,15 @@
 .. _EnMap-box plugin: https://enmap-box.readthedocs.io/en/latest/usr_section/usr_installation.html#install-or-update-the-enmap-box
 
 
 **Install** EnMap-Box using the Plugin manager
 
 
 Install Conda
---------------------------------
+===========================================
 
 Current suggested installation is using a virtual environment, here with the environment
 and package manager `miniconda`_.
 
 .. code:: console
 
     wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
@@ -71,15 +124,15 @@
 .. code:: console
 
     conda create -c conda-forge --name enpt python=3
     conda activate enpt
     conda install -c conda-forge enpt
 
 Polymer (by HYGEOS)
------------------------------
+===========================================
 
 **Obtain** polymer by first subscribing to the `Polymer forum`_.
 Then, download and decompress the polymer package.
 
 .. code:: console
 
     tar -xvf polymer-v4.13.tar.gz
@@ -113,15 +166,15 @@
 **Install** Polymer using the package manager:
 
 .. code:: console
 
     pip3 install -e .
 
 Ancillary data
----------------
+===========================================
 
 **Download** parameterization data via the command bellow. Basically, the
 necessary data (190 Mb) are downloaded from the `Polymer server`_ and stored in
 the local polymer directory. Be sure to be in the polymer directory, e.g. *polymer*.
 
 .. code:: console
 
@@ -148,15 +201,15 @@
     echo "url: https://cds.climate.copernicus.eu/api/v2" >> $HOME/.cdsapirc
     echo "key: $CDS_API_KEY" >> $HOME/.cdsapirc
 
 .. _`Polymer server`: http://download.hygeos.com/POLYMER/auxdata
 
 
 ACwater Polymer
---------------------------------
+===========================================
 
 **Clone** and **install** the source code of the wrapper module ACwater for running Polymer with the EnPT.
 
 .. code:: console
 
     git clone https://gitlab.awi.de/phytooptics/acwater.git
     cd acwater
```

### Comparing `acwater-0.3.0/docs/instructions_dev.rst` & `acwater-0.3.1/docs/instructions_dev.rst`

 * *Files identical despite different names*

### Comparing `acwater-0.3.0/docs/make.bat` & `acwater-0.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `acwater-0.3.0/docs/tutorial.rst` & `acwater-0.3.1/docs/tutorial.rst`

 * *Files identical despite different names*

### Comparing `acwater-0.3.0/polymer_env.yml` & `acwater-0.3.1/polymer_env.yml`

 * *Files identical despite different names*

### Comparing `acwater-0.3.0/sciadrive/build_ascii.py` & `acwater-0.3.1/sciadrive/build_ascii.py`

 * *Files identical despite different names*

### Comparing `acwater-0.3.0/sciadrive/example_ascii.py` & `acwater-0.3.1/sciadrive/example_ascii.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,17 +38,21 @@
 This script runs Polymer using formatted text/ASCII-file
 
 """
 # todo: cli
 
 # from polymer.ancillary_era5 import Ancillary_ERA5
 
-from polymer.main import run_atm_corr, Level1, Level2
-from polymer.level1_ascii import Level1_ASCII
+from polymer.main import run_atm_corr
+
+from polymer.level1 import Level1
 
+from polymer.level2 import Level2
+
+from polymer.level1_ascii import Level1_ASCII
 
 def example_ascii():
     """
     Process an ASCII file (here for SCIATRAN-simulated ENMAP)
     using custom calibration coefficients
     returns in-memory level2 (do not write file)
     """
```

### Comparing `acwater-0.3.0/sciadrive/extraction_reshape.csv` & `acwater-0.3.1/sciadrive/extraction_reshape.csv`

 * *Files identical despite different names*

### Comparing `acwater-0.3.0/sciadrive/reshape_spektrum.py` & `acwater-0.3.1/sciadrive/reshape_spektrum.py`

 * *Files identical despite different names*

### Comparing `acwater-0.3.0/setup.py` & `acwater-0.3.1/setup.py`

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
-    version='0.3.0',
+    version='0.3.1',
     zip_safe=False,
 )
```

