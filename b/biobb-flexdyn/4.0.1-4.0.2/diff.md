# Comparing `tmp/biobb_flexdyn-4.0.1.tar.gz` & `tmp/biobb_flexdyn-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/biobb_flexdyn-4.0.1.tar", last modified: Wed Apr 12 15:47:58 2023, max compression
+gzip compressed data, was "dist/biobb_flexdyn-4.0.2.tar", last modified: Fri May 26 08:20:26 2023, max compression
```

## Comparing `biobb_flexdyn-4.0.1.tar` & `biobb_flexdyn-4.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-12 15:47:58.000000 biobb_flexdyn-4.0.1/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11357 2023-03-31 13:41:20.000000 biobb_flexdyn-4.0.1/LICENSE
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1004 2023-04-12 15:47:58.000000 biobb_flexdyn-4.0.1/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5623 2023-04-12 15:46:02.000000 biobb_flexdyn-4.0.1/README.md
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-12 15:47:58.000000 biobb_flexdyn-4.0.1/biobb_flexdyn/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       67 2023-04-12 15:45:49.000000 biobb_flexdyn-4.0.1/biobb_flexdyn/__init__.py
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-12 15:47:58.000000 biobb_flexdyn-4.0.1/biobb_flexdyn/flexdyn/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      128 2023-04-12 15:32:08.000000 biobb_flexdyn-4.0.1/biobb_flexdyn/flexdyn/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    15411 2023-04-12 15:32:08.000000 biobb_flexdyn-4.0.1/biobb_flexdyn/flexdyn/concoord_disco.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11996 2023-04-12 15:32:08.000000 biobb_flexdyn-4.0.1/biobb_flexdyn/flexdyn/concoord_dist.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6914 2023-04-12 15:32:08.000000 biobb_flexdyn-4.0.1/biobb_flexdyn/flexdyn/imod_imc.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5537 2023-04-12 15:32:08.000000 biobb_flexdyn-4.0.1/biobb_flexdyn/flexdyn/imod_imode.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6228 2023-04-12 15:32:08.000000 biobb_flexdyn-4.0.1/biobb_flexdyn/flexdyn/imod_imove.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6927 2023-04-12 15:32:08.000000 biobb_flexdyn-4.0.1/biobb_flexdyn/flexdyn/nolb_nma.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6114 2023-04-12 15:32:08.000000 biobb_flexdyn-4.0.1/biobb_flexdyn/flexdyn/prody_anm.py
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-12 15:47:58.000000 biobb_flexdyn-4.0.1/biobb_flexdyn.egg-info/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1004 2023-04-12 15:47:58.000000 biobb_flexdyn-4.0.1/biobb_flexdyn.egg-info/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      564 2023-04-12 15:47:58.000000 biobb_flexdyn-4.0.1/biobb_flexdyn.egg-info/SOURCES.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        1 2023-04-12 15:47:58.000000 biobb_flexdyn-4.0.1/biobb_flexdyn.egg-info/dependency_links.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      379 2023-04-12 15:47:58.000000 biobb_flexdyn-4.0.1/biobb_flexdyn.egg-info/entry_points.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       20 2023-04-12 15:47:58.000000 biobb_flexdyn-4.0.1/biobb_flexdyn.egg-info/requires.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       14 2023-04-12 15:47:58.000000 biobb_flexdyn-4.0.1/biobb_flexdyn.egg-info/top_level.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       38 2023-04-12 15:47:58.000000 biobb_flexdyn-4.0.1/setup.cfg
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1865 2023-04-12 15:45:38.000000 biobb_flexdyn-4.0.1/setup.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-05-26 08:20:26.000000 biobb_flexdyn-4.0.2/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573    11357 2023-03-31 13:41:20.000000 biobb_flexdyn-4.0.2/LICENSE
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     1104 2023-05-26 08:20:26.000000 biobb_flexdyn-4.0.2/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     5623 2023-05-26 08:18:31.000000 biobb_flexdyn-4.0.2/README.md
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-05-26 08:20:26.000000 biobb_flexdyn-4.0.2/biobb_flexdyn/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       67 2023-05-26 08:18:18.000000 biobb_flexdyn-4.0.2/biobb_flexdyn/__init__.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-05-26 08:20:26.000000 biobb_flexdyn-4.0.2/biobb_flexdyn/flexdyn/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573      128 2023-04-12 15:32:08.000000 biobb_flexdyn-4.0.2/biobb_flexdyn/flexdyn/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    15447 2023-05-26 08:00:28.000000 biobb_flexdyn-4.0.2/biobb_flexdyn/flexdyn/concoord_disco.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11996 2023-04-12 15:32:08.000000 biobb_flexdyn-4.0.2/biobb_flexdyn/flexdyn/concoord_dist.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     6914 2023-04-12 15:32:08.000000 biobb_flexdyn-4.0.2/biobb_flexdyn/flexdyn/imod_imc.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     5537 2023-04-12 15:32:08.000000 biobb_flexdyn-4.0.2/biobb_flexdyn/flexdyn/imod_imode.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     6228 2023-04-12 15:32:08.000000 biobb_flexdyn-4.0.2/biobb_flexdyn/flexdyn/imod_imove.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     6927 2023-04-12 15:32:08.000000 biobb_flexdyn-4.0.2/biobb_flexdyn/flexdyn/nolb_nma.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     6114 2023-04-12 15:32:08.000000 biobb_flexdyn-4.0.2/biobb_flexdyn/flexdyn/prody_anm.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-05-26 08:20:26.000000 biobb_flexdyn-4.0.2/biobb_flexdyn.egg-info/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     1104 2023-05-26 08:20:26.000000 biobb_flexdyn-4.0.2/biobb_flexdyn.egg-info/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) 1791188573      564 2023-05-26 08:20:26.000000 biobb_flexdyn-4.0.2/biobb_flexdyn.egg-info/SOURCES.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573        1 2023-05-26 08:20:26.000000 biobb_flexdyn-4.0.2/biobb_flexdyn.egg-info/dependency_links.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573      379 2023-05-26 08:20:26.000000 biobb_flexdyn-4.0.2/biobb_flexdyn.egg-info/entry_points.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       20 2023-05-26 08:20:26.000000 biobb_flexdyn-4.0.2/biobb_flexdyn.egg-info/requires.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       14 2023-05-26 08:20:26.000000 biobb_flexdyn-4.0.2/biobb_flexdyn.egg-info/top_level.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       38 2023-05-26 08:20:26.000000 biobb_flexdyn-4.0.2/setup.cfg
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     1963 2023-05-26 08:18:05.000000 biobb_flexdyn-4.0.2/setup.py
```

### Comparing `biobb_flexdyn-4.0.1/LICENSE` & `biobb_flexdyn-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `biobb_flexdyn-4.0.1/PKG-INFO` & `biobb_flexdyn-4.0.2/biobb_flexdyn.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
-Name: biobb_flexdyn
-Version: 4.0.1
+Name: biobb-flexdyn
+Version: 4.0.2
 Summary: biobb_flexdyn is a BioBB category for studies on the conformational landscape of native proteins.
 Home-page: https://github.com/bioexcel/biobb_flexdyn
 Author: Biobb developers
 Author-email: adam.hospital@irbbarcelona.org
 Project-URL: Documentation, http://biobb_flexdyn.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: 3D-Bioinfo ELIXIR FlexDyn Bioinformatics Workflows BioExcel Compatibility Flexibility Ensembles Protein Structure
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Requires-Python: >=3.7,<3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `biobb_flexdyn-4.0.1/README.md` & `biobb_flexdyn-4.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_flexdyn?label=Version)](https://GitHub.com/bioexcel/biobb_flexdyn/tags/)
 [![](https://img.shields.io/pypi/v/biobb-flexdyn.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-flexdyn/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_flexdyn?label=Conda)](https://anaconda.org/bioconda/biobb_flexdyn)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_flexdyn?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_flexdyn)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_flexdyn?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_flexdyn:4.0.1--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_flexdyn:4.0.2--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_flexdyn)
 [![](https://img.shields.io/pypi/pyversions/biobb-flexdyn.svg?label=Python%20Versions)](https://pypi.org/project/biobb-flexdyn/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_flexdyn)
 
 [![](https://readthedocs.org/projects/biobb-flexdyn/badge/?version=latest&label=Docs)](https://biobb-flexdyn.readthedocs.io/en/latest/?badge=latest)
@@ -30,60 +30,60 @@
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](http://biobb_flexdyn.readthedocs.io/en/latest/).
 
 ### Version
-v4.0.1 2023.1
+v4.0.2 2023.1
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA or DOCKER.
 
 * Installation:
 
 
-        pip install "biobb_flexdyn>=4.0.1"
+        pip install "biobb_flexdyn>=4.0.2"
 
 
 * Usage: [Python API documentation](https://biobb-flexdyn.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_flexdyn>=4.0.1"
+        conda install -c bioconda "biobb_flexdyn>=4.0.2"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-flexdyn.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-flexdyn.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_flexdyn:4.0.1--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_flexdyn:4.0.2--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_flexdyn:4.0.1--pyhdfd78af_0
+        docker run quay.io/biocontainers/biobb_flexdyn:4.0.2--pyhdfd78af_0
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_flexdyn.sif https://depot.galaxyproject.org/singularity/biobb_flexdyn:4.0.1--pyhdfd78af_0
+        singularity pull --name biobb_flexdyn.sif https://depot.galaxyproject.org/singularity/biobb_flexdyn:4.0.2--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_flexdyn.sif <command>
```

### Comparing `biobb_flexdyn-4.0.1/biobb_flexdyn/flexdyn/concoord_disco.py` & `biobb_flexdyn-4.0.2/biobb_flexdyn/flexdyn/concoord_disco.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,16 +126,17 @@
 
         # Copy auxiliary files (MARGINS, ATOMS, BONDS) according to the VdW property to the working dir
         concoord_lib = os.getenv("CONCOORDLIB")
 
         # MARGINS_li.DAT, MARGINS_oplsaa.DAT, MARGINS_oplsua.DAT, MARGINS_oplsx.DAT, MARGINS_repel.DAT, MARGINS_yamber2.DAT
         # 1 (OPLS-UA -united atoms- parameters), 2 (OPLS-AA -all atoms- parameters), 3 (PROLSQ repel parameters), 4 (Yamber2 parameters), 5 (Li et al. parameters), 6 (OPLS-X parameters -recommended for NMR structure determination-).
         vdw_values = ["vdw_values", "oplsua", "oplsaa", "repel", "yamber2", "li", "oplsx"]
-        margins_file = concoord_lib + "/MARGINS_" + vdw_values[self.vdw] + ".DAT"
-        atoms_file = concoord_lib + "/ATOMS_" + vdw_values[self.vdw] + ".DAT"
+        vdw_index = int(self.vdw)
+        margins_file = concoord_lib + "/MARGINS_" + vdw_values[vdw_index] + ".DAT"
+        atoms_file = concoord_lib + "/ATOMS_" + vdw_values[vdw_index] + ".DAT"
         bonds_file = concoord_lib + "/BONDS.DAT"
         shutil.copy2(margins_file, self.stage_io_dict.get("unique_dir"))
         shutil.copy2(margins_file, self.stage_io_dict.get("unique_dir")+"/MARGINS.DAT")
         shutil.copy2(atoms_file, self.stage_io_dict.get("unique_dir"))
         shutil.copy2(bonds_file, self.stage_io_dict.get("unique_dir"))
 
         # Command line
```

### Comparing `biobb_flexdyn-4.0.1/biobb_flexdyn/flexdyn/concoord_dist.py` & `biobb_flexdyn-4.0.2/biobb_flexdyn/flexdyn/concoord_dist.py`

 * *Files identical despite different names*

### Comparing `biobb_flexdyn-4.0.1/biobb_flexdyn/flexdyn/imod_imc.py` & `biobb_flexdyn-4.0.2/biobb_flexdyn/flexdyn/imod_imc.py`

 * *Files identical despite different names*

### Comparing `biobb_flexdyn-4.0.1/biobb_flexdyn/flexdyn/imod_imode.py` & `biobb_flexdyn-4.0.2/biobb_flexdyn/flexdyn/imod_imode.py`

 * *Files identical despite different names*

### Comparing `biobb_flexdyn-4.0.1/biobb_flexdyn/flexdyn/imod_imove.py` & `biobb_flexdyn-4.0.2/biobb_flexdyn/flexdyn/imod_imove.py`

 * *Files identical despite different names*

### Comparing `biobb_flexdyn-4.0.1/biobb_flexdyn/flexdyn/nolb_nma.py` & `biobb_flexdyn-4.0.2/biobb_flexdyn/flexdyn/nolb_nma.py`

 * *Files identical despite different names*

### Comparing `biobb_flexdyn-4.0.1/biobb_flexdyn/flexdyn/prody_anm.py` & `biobb_flexdyn-4.0.2/biobb_flexdyn/flexdyn/prody_anm.py`

 * *Files identical despite different names*

### Comparing `biobb_flexdyn-4.0.1/biobb_flexdyn.egg-info/PKG-INFO` & `biobb_flexdyn-4.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
-Name: biobb-flexdyn
-Version: 4.0.1
+Name: biobb_flexdyn
+Version: 4.0.2
 Summary: biobb_flexdyn is a BioBB category for studies on the conformational landscape of native proteins.
 Home-page: https://github.com/bioexcel/biobb_flexdyn
 Author: Biobb developers
 Author-email: adam.hospital@irbbarcelona.org
 Project-URL: Documentation, http://biobb_flexdyn.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: 3D-Bioinfo ELIXIR FlexDyn Bioinformatics Workflows BioExcel Compatibility Flexibility Ensembles Protein Structure
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Requires-Python: >=3.7,<3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `biobb_flexdyn-4.0.1/biobb_flexdyn.egg-info/SOURCES.txt` & `biobb_flexdyn-4.0.2/biobb_flexdyn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biobb_flexdyn-4.0.1/setup.py` & `biobb_flexdyn-4.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="biobb_flexdyn",
-    version="4.0.1",
+    version="4.0.2",
     author="Biobb developers",
     author_email="adam.hospital@irbbarcelona.org",
     description="biobb_flexdyn is a BioBB category for studies on the conformational landscape of native proteins.",
     long_description="biobb_flexdyn allows the generation of protein conformational ensembles from 3D structures and the analysis of its molecular flexibility.",
     long_description_content_type="text/markdown",
     keywords="3D-Bioinfo ELIXIR FlexDyn Bioinformatics Workflows BioExcel Compatibility Flexibility Ensembles Protein Structure",
     url="https://github.com/bioexcel/biobb_flexdyn",
@@ -31,12 +31,14 @@
             "nolb_nma = biobb_flexdyn.flexdyn.nolb_nma:main",
             "prody_anm = biobb_flexdyn.flexdyn.prody_anm:main"
         ]
     },
     classifiers=(
         "Development Status :: 3 - Alpha",
         "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: POSIX",
     ),
 )
```

