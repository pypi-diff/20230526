# Comparing `tmp/ogscm-2.4.7.tar.gz` & `tmp/ogscm-2.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ogscm-2.4.7.tar", max compression
+gzip compressed data, was "ogscm-2.4.8.tar", max compression
```

## Comparing `ogscm-2.4.7.tar` & `ogscm-2.4.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1510 2023-05-22 13:15:50.275640 ogscm-2.4.7/LICENSE
--rw-r--r--   0        0        0    11903 2023-05-22 13:15:50.275640 ogscm-2.4.7/README.md
--rw-r--r--   0        0        0       81 2023-05-22 13:15:50.275640 ogscm-2.4.7/ogscm/__init__.py
--rw-r--r--   0        0        0      118 2023-05-22 13:15:50.278973 ogscm-2.4.7/ogscm/app/__init__.py
--rw-r--r--   0        0        0     3942 2023-05-22 13:15:50.278973 ogscm-2.4.7/ogscm/app/builder.py
--rw-r--r--   0        0        0     1600 2023-05-22 13:15:50.278973 ogscm-2.4.7/ogscm/app/deployer.py
--rw-r--r--   0        0        0      402 2023-05-22 13:15:50.278973 ogscm-2.4.7/ogscm/building_blocks/__init__.py
--rw-r--r--   0        0        0     1477 2023-05-22 13:15:50.278973 ogscm-2.4.7/ogscm/building_blocks/ccache.py
--rw-r--r--   0        0        0     3312 2023-05-22 13:15:50.278973 ogscm-2.4.7/ogscm/building_blocks/lmod.py
--rw-r--r--   0        0        0     7047 2023-05-22 13:15:50.278973 ogscm-2.4.7/ogscm/building_blocks/ogs.py
--rw-r--r--   0        0        0     3245 2023-05-22 13:15:50.278973 ogscm-2.4.7/ogscm/building_blocks/ogs_base.py
--rw-r--r--   0        0        0     4124 2023-05-22 13:15:50.278973 ogscm-2.4.7/ogscm/building_blocks/osu_benchmarks.py
--rw-r--r--   0        0        0     5228 2023-05-22 13:15:50.278973 ogscm-2.4.7/ogscm/building_blocks/paraview.py
--rw-r--r--   0        0        0     3643 2023-05-22 13:15:50.278973 ogscm-2.4.7/ogscm/building_blocks/pm_easybuild.py
--rw-r--r--   0        0        0    10303 2023-05-25 10:55:11.905500 ogscm-2.4.7/ogscm/cli.py
--rw-r--r--   0        0        0      148 2023-05-22 13:15:50.278973 ogscm-2.4.7/ogscm/common.py
--rw-r--r--   0        0        0      645 2023-05-22 13:15:50.278973 ogscm-2.4.7/ogscm/config.py
--rw-r--r--   0        0        0        0 2023-05-22 13:15:50.278973 ogscm-2.4.7/ogscm/recipes/__init__.py
--rw-r--r--   0        0        0      733 2023-05-22 13:15:50.278973 ogscm-2.4.7/ogscm/recipes/_template.py
--rw-r--r--   0        0        0     3065 2023-05-22 13:15:50.278973 ogscm-2.4.7/ogscm/recipes/compiler.py
--rw-r--r--   0        0        0      116 2023-05-22 13:15:50.278973 ogscm-2.4.7/ogscm/recipes/files/jupyterlab-gitlab_settings.json
--rw-r--r--   0        0        0     2742 2023-05-22 13:15:50.278973 ogscm-2.4.7/ogscm/recipes/mpi-entrypoint.sh
--rw-r--r--   0        0        0     6535 2023-05-22 13:15:50.278973 ogscm-2.4.7/ogscm/recipes/mpi.py
--rw-r--r--   0        0        0    22872 2023-05-22 13:15:50.278973 ogscm-2.4.7/ogscm/recipes/ogs.py
--rw-r--r--   0        0        0     3471 2023-05-22 13:15:50.278973 ogscm-2.4.7/ogscm/recipes/ogs_jupyter.py
--rw-r--r--   0        0        0     1083 2023-05-22 13:15:50.278973 ogscm-2.4.7/ogscm/recipes/ogs_vscode.py
--rw-r--r--   0        0        0     1090 2023-05-22 13:15:50.278973 ogscm-2.4.7/ogscm/recipes/ogs_web.py
--rw-r--r--   0        0        0      665 2023-05-22 13:15:50.278973 ogscm-2.4.7/ogscm/recipes/python_vtk.py
--rw-r--r--   0        0        0      123 2023-05-22 13:15:50.278973 ogscm-2.4.7/ogscm/version.py
--rw-r--r--   0        0        0      661 2023-05-25 10:55:11.905500 ogscm-2.4.7/pyproject.toml
--rw-r--r--   0        0        0    12827 1970-01-01 00:00:00.000000 ogscm-2.4.7/PKG-INFO
+-rw-r--r--   0        0        0     1510 2023-05-26 13:26:47.209535 ogscm-2.4.8/LICENSE
+-rw-r--r--   0        0        0    11903 2023-05-26 13:26:47.209535 ogscm-2.4.8/README.md
+-rw-r--r--   0        0        0       81 2023-05-26 13:26:47.209535 ogscm-2.4.8/ogscm/__init__.py
+-rw-r--r--   0        0        0      118 2023-05-26 13:26:47.209535 ogscm-2.4.8/ogscm/app/__init__.py
+-rw-r--r--   0        0        0     3942 2023-05-26 13:26:47.209535 ogscm-2.4.8/ogscm/app/builder.py
+-rw-r--r--   0        0        0     1600 2023-05-26 13:26:47.209535 ogscm-2.4.8/ogscm/app/deployer.py
+-rw-r--r--   0        0        0      402 2023-05-26 13:26:47.209535 ogscm-2.4.8/ogscm/building_blocks/__init__.py
+-rw-r--r--   0        0        0     1477 2023-05-26 13:26:47.209535 ogscm-2.4.8/ogscm/building_blocks/ccache.py
+-rw-r--r--   0        0        0     3312 2023-05-26 13:26:47.209535 ogscm-2.4.8/ogscm/building_blocks/lmod.py
+-rw-r--r--   0        0        0     7047 2023-05-26 13:26:47.209535 ogscm-2.4.8/ogscm/building_blocks/ogs.py
+-rw-r--r--   0        0        0     3245 2023-05-26 13:26:47.209535 ogscm-2.4.8/ogscm/building_blocks/ogs_base.py
+-rw-r--r--   0        0        0     4124 2023-05-26 13:26:47.209535 ogscm-2.4.8/ogscm/building_blocks/osu_benchmarks.py
+-rw-r--r--   0        0        0     5228 2023-05-26 13:26:47.209535 ogscm-2.4.8/ogscm/building_blocks/paraview.py
+-rw-r--r--   0        0        0     3643 2023-05-26 13:26:47.209535 ogscm-2.4.8/ogscm/building_blocks/pm_easybuild.py
+-rw-r--r--   0        0        0    10303 2023-05-26 13:26:47.209535 ogscm-2.4.8/ogscm/cli.py
+-rw-r--r--   0        0        0      148 2023-05-26 13:26:47.209535 ogscm-2.4.8/ogscm/common.py
+-rw-r--r--   0        0        0      645 2023-05-26 13:26:47.209535 ogscm-2.4.8/ogscm/config.py
+-rw-r--r--   0        0        0        0 2023-05-26 13:26:47.209535 ogscm-2.4.8/ogscm/recipes/__init__.py
+-rw-r--r--   0        0        0      733 2023-05-26 13:26:47.209535 ogscm-2.4.8/ogscm/recipes/_template.py
+-rw-r--r--   0        0        0     3065 2023-05-26 13:26:47.209535 ogscm-2.4.8/ogscm/recipes/compiler.py
+-rw-r--r--   0        0        0      116 2023-05-26 13:26:47.209535 ogscm-2.4.8/ogscm/recipes/files/jupyterlab-gitlab_settings.json
+-rw-r--r--   0        0        0     2742 2023-05-26 13:26:47.209535 ogscm-2.4.8/ogscm/recipes/mpi-entrypoint.sh
+-rw-r--r--   0        0        0     6535 2023-05-26 13:26:47.209535 ogscm-2.4.8/ogscm/recipes/mpi.py
+-rw-r--r--   0        0        0    22872 2023-05-26 13:26:47.209535 ogscm-2.4.8/ogscm/recipes/ogs.py
+-rw-r--r--   0        0        0     3471 2023-05-26 13:26:47.209535 ogscm-2.4.8/ogscm/recipes/ogs_jupyter.py
+-rw-r--r--   0        0        0     1083 2023-05-26 13:26:47.209535 ogscm-2.4.8/ogscm/recipes/ogs_vscode.py
+-rw-r--r--   0        0        0     1090 2023-05-26 13:26:47.209535 ogscm-2.4.8/ogscm/recipes/ogs_web.py
+-rw-r--r--   0        0        0      665 2023-05-26 13:26:47.209535 ogscm-2.4.8/ogscm/recipes/python_vtk.py
+-rw-r--r--   0        0        0      123 2023-05-26 13:26:47.209535 ogscm-2.4.8/ogscm/version.py
+-rw-r--r--   0        0        0      661 2023-05-26 13:26:47.209535 ogscm-2.4.8/pyproject.toml
+-rw-r--r--   0        0        0    12827 1970-01-01 00:00:00.000000 ogscm-2.4.8/PKG-INFO
```

### Comparing `ogscm-2.4.7/LICENSE` & `ogscm-2.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ogscm-2.4.7/README.md` & `ogscm-2.4.8/README.md`

 * *Files identical despite different names*

### Comparing `ogscm-2.4.7/ogscm/app/builder.py` & `ogscm-2.4.8/ogscm/app/builder.py`

 * *Files identical despite different names*

### Comparing `ogscm-2.4.7/ogscm/app/deployer.py` & `ogscm-2.4.8/ogscm/app/deployer.py`

 * *Files identical despite different names*

### Comparing `ogscm-2.4.7/ogscm/building_blocks/ccache.py` & `ogscm-2.4.8/ogscm/building_blocks/ccache.py`

 * *Files identical despite different names*

### Comparing `ogscm-2.4.7/ogscm/building_blocks/lmod.py` & `ogscm-2.4.8/ogscm/building_blocks/lmod.py`

 * *Files identical despite different names*

### Comparing `ogscm-2.4.7/ogscm/building_blocks/ogs.py` & `ogscm-2.4.8/ogscm/building_blocks/ogs.py`

 * *Files identical despite different names*

### Comparing `ogscm-2.4.7/ogscm/building_blocks/ogs_base.py` & `ogscm-2.4.8/ogscm/building_blocks/ogs_base.py`

 * *Files identical despite different names*

### Comparing `ogscm-2.4.7/ogscm/building_blocks/osu_benchmarks.py` & `ogscm-2.4.8/ogscm/building_blocks/osu_benchmarks.py`

 * *Files identical despite different names*

### Comparing `ogscm-2.4.7/ogscm/building_blocks/paraview.py` & `ogscm-2.4.8/ogscm/building_blocks/paraview.py`

 * *Files identical despite different names*

### Comparing `ogscm-2.4.7/ogscm/building_blocks/pm_easybuild.py` & `ogscm-2.4.8/ogscm/building_blocks/pm_easybuild.py`

 * *Files identical despite different names*

### Comparing `ogscm-2.4.7/ogscm/cli.py` & `ogscm-2.4.8/ogscm/cli.py`

 * *Files identical despite different names*

### Comparing `ogscm-2.4.7/ogscm/config.py` & `ogscm-2.4.8/ogscm/config.py`

 * *Files identical despite different names*

### Comparing `ogscm-2.4.7/ogscm/recipes/_template.py` & `ogscm-2.4.8/ogscm/recipes/_template.py`

 * *Files identical despite different names*

### Comparing `ogscm-2.4.7/ogscm/recipes/compiler.py` & `ogscm-2.4.8/ogscm/recipes/compiler.py`

 * *Files identical despite different names*

### Comparing `ogscm-2.4.7/ogscm/recipes/mpi-entrypoint.sh` & `ogscm-2.4.8/ogscm/recipes/mpi-entrypoint.sh`

 * *Files identical despite different names*

### Comparing `ogscm-2.4.7/ogscm/recipes/mpi.py` & `ogscm-2.4.8/ogscm/recipes/mpi.py`

 * *Files identical despite different names*

### Comparing `ogscm-2.4.7/ogscm/recipes/ogs.py` & `ogscm-2.4.8/ogscm/recipes/ogs.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -319,14 +319,20 @@
 
 versions_master = json.loads(
     requests.get(
         f"https://gitlab.opengeosys.org/ogs/ogs/-/raw/master/web/data/versions.json?inline=false"
     ).text
 )
 
+if local_args.mkl:
+    Stage0 += mkl(eula=True, mklvars=False)
+    # For 32-bit mkl_link_tool:
+    Stage0 += packages(apt=["lib32stdc++6"], yum=["libstdc++.i686"])
+    cmake_args.append("-DOGS_USE_MKL=ON")
+
 if local_args.ogs != "clean":
     cmake_version = versions_master["tested_version"]["cmake"]
     if "cmake" in versions["tested_version"]:
         cmake_version = versions["tested_version"]["cmake"]
     Stage0 += cmake(eula=True, version=cmake_version)
     if local_args.pm == "system":
         if local_args.mfront:
@@ -600,20 +606,14 @@
             "PYTHONPATH": "/usr/local/tfel/lib/python3.8/site-packages:$PYTHONPATH",
         }
     )
     Stage0 += tfel_env
     Stage1 += tfel_env
     cmake_args.append("-DOGS_USE_MFRONT=ON")
 
-if local_args.mkl:
-    Stage0 += mkl(eula=True, mklvars=False)
-    # For 32-bit mkl_link_tool:
-    Stage0 += packages(apt=["lib32stdc++6"], yum=["libstdc++.i686"])
-    cmake_args.append("-DOGS_USE_MKL=ON")
-
 # Used to fix RPATH in petsc.so build as external dependency
 Stage0 += packages(ospackages=["patchelf"])
 
 if local_args.ccache:
     Stage0 += ccache(cache_size="15G")
 if local_args.ogs != "off" and local_args.ogs != "clean":
     mount_args = ""
```

### Comparing `ogscm-2.4.7/ogscm/recipes/ogs_jupyter.py` & `ogscm-2.4.8/ogscm/recipes/ogs_jupyter.py`

 * *Files identical despite different names*

### Comparing `ogscm-2.4.7/ogscm/recipes/ogs_vscode.py` & `ogscm-2.4.8/ogscm/recipes/ogs_vscode.py`

 * *Files identical despite different names*

### Comparing `ogscm-2.4.7/ogscm/recipes/ogs_web.py` & `ogscm-2.4.8/ogscm/recipes/ogs_web.py`

 * *Files identical despite different names*

### Comparing `ogscm-2.4.7/ogscm/recipes/python_vtk.py` & `ogscm-2.4.8/ogscm/recipes/python_vtk.py`

 * *Files identical despite different names*

### Comparing `ogscm-2.4.7/pyproject.toml` & `ogscm-2.4.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ogscm"
-version = "2.4.7"
+version = "2.4.8"
 description = "OGS Container Maker"
 authors = ["Lars Bilke <lars.bilke@ufz.de>"]
 license = "BSD 3-clause"
 repository = "https://gitlab.opengeosys.org/ogs/container-maker"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `ogscm-2.4.7/PKG-INFO` & `ogscm-2.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogscm
-Version: 2.4.7
+Version: 2.4.8
 Summary: OGS Container Maker
 Home-page: https://gitlab.opengeosys.org/ogs/container-maker
 License: BSD 3-clause
 Author: Lars Bilke
 Author-email: lars.bilke@ufz.de
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
```

