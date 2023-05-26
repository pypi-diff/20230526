# Comparing `tmp/paste-bio-1.3.0.tar.gz` & `tmp/paste-bio-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\maxru\Code\GitHub\paste\dist\tmpm_pc710n\paste-bio-1.3.0.tar", last modified: Fri Jul 22 03:50:32 2022, max compression
+gzip compressed data, was "paste-bio-1.4.0.tar", last modified: Fri May 26 20:39:50 2023, max compression
```

## Comparing `paste-bio-1.3.0.tar` & `paste-bio-1.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2022-07-22 03:50:32.151600 paste-bio-1.3.0/
--rw-rw-rw-   0        0        0     1557 2021-03-15 15:32:27.000000 paste-bio-1.3.0/LICENSE
--rw-rw-rw-   0        0        0     9028 2022-07-22 03:50:32.151600 paste-bio-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     8456 2022-06-20 05:08:08.000000 paste-bio-1.3.0/README.md
--rw-rw-rw-   0        0        0      103 2021-03-22 20:11:42.000000 paste-bio-1.3.0/pyproject.toml
--rw-rw-rw-   0        0        0      729 2022-07-22 03:50:32.167224 paste-bio-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0       37 2021-03-22 20:31:51.000000 paste-bio-1.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-07-22 03:50:32.049237 paste-bio-1.3.0/src/
-drwxrwxrwx   0        0        0        0 2022-07-22 03:50:32.104707 paste-bio-1.3.0/src/paste/
--rw-rw-rw-   0        0        0    15127 2022-04-09 07:21:32.000000 paste-bio-1.3.0/src/paste/PASTE.py
--rw-rw-rw-   0        0        0      224 2022-07-22 03:06:25.000000 paste-bio-1.3.0/src/paste/__init__.py
--rw-rw-rw-   0        0        0     5177 2022-07-22 03:18:01.000000 paste-bio-1.3.0/src/paste/helper.py
--rw-rw-rw-   0        0        0     6962 2022-07-22 03:16:39.000000 paste-bio-1.3.0/src/paste/visualization.py
-drwxrwxrwx   0        0        0        0 2022-07-22 03:50:32.151600 paste-bio-1.3.0/src/paste_bio.egg-info/
--rw-rw-rw-   0        0        0     9028 2022-07-22 03:50:31.000000 paste-bio-1.3.0/src/paste_bio.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2022-07-22 03:50:32.000000 paste-bio-1.3.0/src/paste_bio.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-22 03:50:31.000000 paste-bio-1.3.0/src/paste_bio.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-04-09 07:24:24.000000 paste-bio-1.3.0/src/paste_bio.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        6 2022-07-22 03:50:31.000000 paste-bio-1.3.0/src/paste_bio.egg-info/top_level.txt
+drwxr-xr-x   0 mland      (503) staff       (20)        0 2023-05-26 20:39:50.288244 paste-bio-1.4.0/
+-rw-r--r--   0 mland      (503) staff       (20)     1528 2023-01-03 19:43:34.000000 paste-bio-1.4.0/LICENSE
+-rw-r--r--   0 mland      (503) staff       (20)     9063 2023-05-26 20:39:50.288362 paste-bio-1.4.0/PKG-INFO
+-rw-r--r--   0 mland      (503) staff       (20)     8506 2023-05-26 17:50:41.000000 paste-bio-1.4.0/README.md
+-rw-r--r--   0 mland      (503) staff       (20)      103 2023-01-03 19:43:34.000000 paste-bio-1.4.0/pyproject.toml
+-rw-r--r--   0 mland      (503) staff       (20)      699 2023-05-26 20:39:50.288943 paste-bio-1.4.0/setup.cfg
+-rw-r--r--   0 mland      (503) staff       (20)       37 2023-01-03 19:43:34.000000 paste-bio-1.4.0/setup.py
+drwxr-xr-x   0 mland      (503) staff       (20)        0 2023-05-26 20:39:50.281737 paste-bio-1.4.0/src/
+drwxr-xr-x   0 mland      (503) staff       (20)        0 2023-05-26 20:39:50.285667 paste-bio-1.4.0/src/paste/
+-rw-r--r--   0 mland      (503) staff       (20)    17816 2023-05-26 20:21:42.000000 paste-bio-1.4.0/src/paste/PASTE.py
+-rw-r--r--   0 mland      (503) staff       (20)      222 2023-01-03 19:43:34.000000 paste-bio-1.4.0/src/paste/__init__.py
+-rw-r--r--   0 mland      (503) staff       (20)     5017 2023-01-03 19:43:34.000000 paste-bio-1.4.0/src/paste/helper.py
+-rw-r--r--   0 mland      (503) staff       (20)     6775 2023-01-03 19:43:34.000000 paste-bio-1.4.0/src/paste/visualization.py
+drwxr-xr-x   0 mland      (503) staff       (20)        0 2023-05-26 20:39:50.287972 paste-bio-1.4.0/src/paste_bio.egg-info/
+-rw-r--r--   0 mland      (503) staff       (20)     9063 2023-05-26 20:39:50.000000 paste-bio-1.4.0/src/paste_bio.egg-info/PKG-INFO
+-rw-r--r--   0 mland      (503) staff       (20)      323 2023-05-26 20:39:50.000000 paste-bio-1.4.0/src/paste_bio.egg-info/SOURCES.txt
+-rw-r--r--   0 mland      (503) staff       (20)        1 2023-05-26 20:39:50.000000 paste-bio-1.4.0/src/paste_bio.egg-info/dependency_links.txt
+-rw-r--r--   0 mland      (503) staff       (20)        1 2023-01-03 19:43:34.000000 paste-bio-1.4.0/src/paste_bio.egg-info/not-zip-safe
+-rw-r--r--   0 mland      (503) staff       (20)        6 2023-05-26 20:39:50.000000 paste-bio-1.4.0/src/paste_bio.egg-info/top_level.txt
```

### Comparing `paste-bio-1.3.0/LICENSE` & `paste-bio-1.4.0/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-BSD 3-Clause License
-
-Copyright (c) 2020, Princeton University
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-1. Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright notice,
-   this list of conditions and the following disclaimer in the documentation
-   and/or other materials provided with the distribution.
-
-3. Neither the name of the copyright holder nor the names of its
-   contributors may be used to endorse or promote products derived from
-   this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+BSD 3-Clause License
+
+Copyright (c) 2020, Princeton University
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its
+   contributors may be used to endorse or promote products derived from
+   this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `paste-bio-1.3.0/PKG-INFO` & `paste-bio-1.4.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,183 +1,168 @@
-Metadata-Version: 2.1
-Name: paste-bio
-Version: 1.3.0
-Summary: A computational method to align and integrate spatial transcriptomics experiments.
-Home-page: https://github.com/raphael-group/paste
-Author: Max Land
-Author-email: max.ruikang.land@gmail.com
-Project-URL: Bug Tracker, https://github.com/raphael-group/paste/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![PyPI](https://img.shields.io/pypi/v/paste-bio.svg)](https://pypi.org/project/paste-bio)
-[![Downloads](https://pepy.tech/badge/paste-bio)](https://pepy.tech/project/paste-bio)
-[![Documentation Status](https://readthedocs.org/projects/paste-bio/badge/?version=latest)](https://paste-bio.readthedocs.io/en/stable/?badge=stable)
-
-# PASTE
-
-![PASTE Overview](https://github.com/raphael-group/paste/blob/main/docs/source/_static/images/paste_overview.png)
-
-PASTE is a computational method that leverages both gene expression similarity and spatial distances between spots to align and integrate spatial transcriptomics data. In particular, there are two methods:
-1. `pairwise_align`: align spots across pairwise slices.
-2. `center_align`: integrate multiple slices into one center slice.
-
-You can read full paper [here](https://www.nature.com/articles/s41592-022-01459-6). 
-
-Additional examples and the code to reproduce the paper's analyses can be found [here](https://github.com/raphael-group/paste_reproducibility). Preprocessed datasets used in the paper can be found on [zenodo](https://doi.org/10.5281/zenodo.6334774).
-
-PASTE is actively being worked on with future updates coming. 
-
-### Recent News
-
-* PASTE is now published in [Nature Methods](https://www.nature.com/articles/s41592-022-01459-6)!
-
-* The code to reproduce the analisys can be found [here](https://github.com/raphael-group/paste_reproducibility).
-
-* As of version 1.2.0, PASTE now supports GPU implementation via Pytorch. For more details, see the GPU section of the [Tutorial notebook](docs/source/notebooks/getting-started.ipynb).
-
-### Installation
-
-The easiest way is to install PASTE on pypi: https://pypi.org/project/paste-bio/. 
-
-`pip install paste-bio` 
-
-Or you can install PASTE on bioconda: https://anaconda.org/bioconda/paste-bio.
-
-`conda install -c bioconda paste-bio`
-
-Check out Tutorial.ipynb for an example of how to use PASTE.
-
-Alternatively, you can clone the respository and try the following example in a
-notebook or the command line. 
-
-### Quick Start
-
-To use PASTE we require at least two slices of spatial-omics data (both
-expression and coordinates) that are in
-anndata format (i.e. read in by scanpy/squidpy). We have included a breast
-cancer dataset from [1] in the [sample_data folder](sample_data/) of this repo 
-that we will use as an example below to show how to use PASTE.
-
-```python
-import matplotlib.pyplot as plt
-import matplotlib.patches as mpatches
-import numpy as np
-import scanpy as sc
-import paste as pst
-
-# Load Slices
-data_dir = './sample_data/' # change this path to the data you wish to analyze
-
-# Assume that the coordinates of slices are named slice_name + "_coor.csv"
-def load_slices(data_dir, slice_names=["slice1", "slice2"]):
-    slices = []  
-    for slice_name in slice_names:
-        slice_i = sc.read_csv(data_dir + slice_name + ".csv")
-        slice_i_coor = np.genfromtxt(data_dir + slice_name + "_coor.csv", delimiter = ',')
-        slice_i.obsm['spatial'] = slice_i_coor
-        # Preprocess slices
-        sc.pp.filter_genes(slice_i, min_counts = 15)
-        sc.pp.filter_cells(slice_i, min_counts = 100)
-        slices.append(slice_i)
-    return slices
-
-slices = load_slices(data_dir)
-slice1, slice2 = slices
-
-# Pairwise align the slices
-pi12 = pst.pairwise_align(slice1, slice2)
-
-# To visualize the alignment you can stack the slices 
-# according to the alignment pi
-slices, pis = [slice1, slice2], [pi12]
-new_slices = pst.stack_slices_pairwise(slices, pis)
-
-slice_colors = ['#e41a1c','#377eb8']
-plt.figure(figsize=(7,7))
-for i in range(len(new_slices)):
-    pst.plot_slice(new_slices[i],slice_colors[i],s=400)
-plt.legend(handles=[mpatches.Patch(color=slice_colors[0], label='1'),mpatches.Patch(color=slice_colors[1], label='2')])
-plt.gca().invert_yaxis()
-plt.axis('off')
-plt.show()
-
-# Center align slices
-## We have to reload the slices as pairwise_alignment modifies the slices.
-slices = load_slices(data_dir)
-slice1, slice2 = slices
-
-# Construct a center slice
-## choose one of the slices as the coordinate reference for the center slice,
-## i.e. the center slice will have the same number of spots as this slice and
-## the same coordinates.
-initial_slice = slice1.copy()    
-slices = [slice1, slice2]
-lmbda = len(slices)*[1/len(slices)] # set hyperparameter to be uniform
-
-## Possible to pass in an initial pi (as keyword argument pis_init) 
-## to improve performance, see Tutorial.ipynb notebook for more details.
-center_slice, pis = pst.center_align(initial_slice, slices, lmbda) 
-
-## The low dimensional representation of our center slice is held 
-## in the matrices W and H, which can be used for downstream analyses
-W = center_slice.uns['paste_W']
-H = center_slice.uns['paste_H']
-```
-
-### GPU implementation
-PASTE now is compatible with gpu via Pytorch. All we need to do is add the following two parameters to our main functions:
-```
-pi12 = pst.pairwise_align(slice1, slice2, backend = ot.backend.TorchBackend(), use_gpu = True)
-
-center_slice, pis = pst.center_align(initial_slice, slices, lmbda, backend = ot.backend.TorchBackend(), use_gpu = True) 
-```
-For more details, see the GPU section of the [Tutorial notebook](docs/source/notebooks/getting-started.ipynb).
-
-### Command Line
-
-We provide the option of running PASTE from the command line. 
-
-First, clone the repository:
-
-`git clone https://github.com/raphael-group/paste.git`
-
-Next, when providing files, you will need to provide two separate files: the gene expression data followed by spatial data (both as .csv) for the code to initialize one slice object.
-
-Sample execution (based on this repo): `python paste-cmd-line.py -m center -f ./sample_data/slice1.csv ./sample_data/slice1_coor.csv ./sample_data/slice2.csv ./sample_data/slice2_coor.csv ./sample_data/slice3.csv ./sample_data/slice3_coor.csv`
-
-Note: `pairwise` will return pairwise alignment between each consecutive pair of slices (e.g. \[slice1,slice2\], \[slice2,slice3\]).
-
-| Flag | Name | Description | Default Value |
-| --- | --- | --- | --- |
-| -m | mode | Select either `pairwise` or `center` | (str) `pairwise` |
-| -f | files | Path to data files (.csv) | None |
-| -d | direc | Directory to store output files | Current Directory |
-| -a | alpha | Alpha parameter for PASTE | (float) `0.1` |
-| -c | cost | Expression dissimilarity cost (`kl` or `Euclidean`) | (str) `kl` |
-| -p | n_components | n_components for NMF step in `center_align` | (int) `15` |
-| -l | lmbda | Lambda parameter in `center_align` | (floats) probability vector of length `n`  |
-| -i | intial_slice | Specify which file is also the intial slice in `center_align` | (int) `1` |
-| -t | threshold | Convergence threshold for `center_align` | (float) `0.001` |
-| -x | coordinates | Output new coordinates (toggle to turn on) | `False` |
-| -w | weights | Weights files of spots in each slice (.csv) | None |
-| -s | start | Initial alignments for OT. If not given uses uniform (.csv structure similar to alignment output) | None |
-
-`pairwise_align` outputs a (.csv) file containing mapping of spots between each consecutive pair of slices. The rows correspond to spots of the first slice, and cols the second.
-
-`center_align` outputs two files containing the low dimensional representation (NMF decomposition) of the center slice gene expression, and files containing a mapping of spots between the center slice (rows) to each input slice (cols).
-
-### Sample Dataset
-
-Added sample spatial transcriptomics dataset consisting of four breast cancer slice courtesy of:
-
-[1] Ståhl, Patrik & Salmén, Fredrik & Vickovic, Sanja & Lundmark, Anna & Fernandez Navarro, Jose & Magnusson, Jens & Giacomello, Stefania & Asp, Michaela & Westholm, Jakub & Huss, Mikael & Mollbrink, Annelie & Linnarsson, Sten & Codeluppi, Simone & Borg, Åke & Pontén, Fredrik & Costea, Paul & Sahlén, Pelin Akan & Mulder, Jan & Bergmann, Olaf & Frisén, Jonas. (2016). Visualization and analysis of gene expression in tissue sections by spatial transcriptomics. Science. 353. 78-82. 10.1126/science.aaf2403. 
-
-Note: Original data is (.tsv), but we converted it to (.csv).
-
-### References
-
-Ron Zeira, Max Land, Alexander Strzalkowski and Benjamin J. Raphael. "Alignment and integration of spatial transcriptomics data". Nature Methods (2022). https://doi.org/10.1038/s41592-022-01459-6
+[![PyPI](https://img.shields.io/pypi/v/paste-bio.svg)](https://pypi.org/project/paste-bio)
+[![Downloads](https://pepy.tech/badge/paste-bio)](https://pepy.tech/project/paste-bio)
+[![Documentation Status](https://readthedocs.org/projects/paste-bio/badge/?version=latest)](https://paste-bio.readthedocs.io/en/stable/?badge=stable)
+[![Anaconda](https://anaconda.org/bioconda/paste-bio/badges/version.svg)](https://anaconda.org/bioconda/paste-bio/badges/version.svg)
+[![bioconda-downloads](https://anaconda.org/bioconda/paste-bio/badges/downloads.svg)](https://anaconda.org/bioconda/paste-bio/badges/downloads.svg)
+
+# PASTE
+
+![PASTE Overview](https://github.com/raphael-group/paste/blob/main/docs/source/_static/images/paste_overview.png)
+
+PASTE is a computational method that leverages both gene expression similarity and spatial distances between spots to align and integrate spatial transcriptomics data. In particular, there are two methods:
+1. `pairwise_align`: align spots across pairwise slices.
+2. `center_align`: integrate multiple slices into one center slice.
+
+You can read full paper [here](https://www.nature.com/articles/s41592-022-01459-6). 
+
+Additional examples and the code to reproduce the paper's analyses can be found [here](https://github.com/raphael-group/paste_reproducibility). Preprocessed datasets used in the paper can be found on [zenodo](https://doi.org/10.5281/zenodo.6334774).
+
+### Recent News
+
+* PASTE is now published in [Nature Methods](https://www.nature.com/articles/s41592-022-01459-6)!
+
+* The code to reproduce the analisys can be found [here](https://github.com/raphael-group/paste_reproducibility).
+
+* As of version 1.2.0, PASTE now supports GPU implementation via Pytorch. For more details, see the GPU section of the [Tutorial notebook](docs/source/notebooks/getting-started.ipynb).
+
+### Installation
+
+The easiest way is to install PASTE on pypi: https://pypi.org/project/paste-bio/. 
+
+`pip install paste-bio` 
+
+Or you can install PASTE on bioconda: https://anaconda.org/bioconda/paste-bio.
+
+`conda install -c bioconda paste-bio`
+
+Check out Tutorial.ipynb for an example of how to use PASTE.
+
+Alternatively, you can clone the respository and try the following example in a
+notebook or the command line. 
+
+### Quick Start
+
+To use PASTE we require at least two slices of spatial-omics data (both
+expression and coordinates) that are in
+anndata format (i.e. read in by scanpy/squidpy). We have included a breast
+cancer dataset from [1] in the [sample_data folder](sample_data/) of this repo 
+that we will use as an example below to show how to use PASTE.
+
+```python
+import matplotlib.pyplot as plt
+import matplotlib.patches as mpatches
+import numpy as np
+import scanpy as sc
+import paste as pst
+
+# Load Slices
+data_dir = './sample_data/' # change this path to the data you wish to analyze
+
+# Assume that the coordinates of slices are named slice_name + "_coor.csv"
+def load_slices(data_dir, slice_names=["slice1", "slice2"]):
+    slices = []  
+    for slice_name in slice_names:
+        slice_i = sc.read_csv(data_dir + slice_name + ".csv")
+        slice_i_coor = np.genfromtxt(data_dir + slice_name + "_coor.csv", delimiter = ',')
+        slice_i.obsm['spatial'] = slice_i_coor
+        # Preprocess slices
+        sc.pp.filter_genes(slice_i, min_counts = 15)
+        sc.pp.filter_cells(slice_i, min_counts = 100)
+        slices.append(slice_i)
+    return slices
+
+slices = load_slices(data_dir)
+slice1, slice2 = slices
+
+# Pairwise align the slices
+pi12 = pst.pairwise_align(slice1, slice2)
+
+# To visualize the alignment you can stack the slices 
+# according to the alignment pi
+slices, pis = [slice1, slice2], [pi12]
+new_slices = pst.stack_slices_pairwise(slices, pis)
+
+slice_colors = ['#e41a1c','#377eb8']
+plt.figure(figsize=(7,7))
+for i in range(len(new_slices)):
+    pst.plot_slice(new_slices[i],slice_colors[i],s=400)
+plt.legend(handles=[mpatches.Patch(color=slice_colors[0], label='1'),mpatches.Patch(color=slice_colors[1], label='2')])
+plt.gca().invert_yaxis()
+plt.axis('off')
+plt.show()
+
+# Center align slices
+## We have to reload the slices as pairwise_alignment modifies the slices.
+slices = load_slices(data_dir)
+slice1, slice2 = slices
+
+# Construct a center slice
+## choose one of the slices as the coordinate reference for the center slice,
+## i.e. the center slice will have the same number of spots as this slice and
+## the same coordinates.
+initial_slice = slice1.copy()    
+slices = [slice1, slice2]
+lmbda = len(slices)*[1/len(slices)] # set hyperparameter to be uniform
+
+## Possible to pass in an initial pi (as keyword argument pis_init) 
+## to improve performance, see Tutorial.ipynb notebook for more details.
+center_slice, pis = pst.center_align(initial_slice, slices, lmbda) 
+
+## The low dimensional representation of our center slice is held 
+## in the matrices W and H, which can be used for downstream analyses
+W = center_slice.uns['paste_W']
+H = center_slice.uns['paste_H']
+```
+
+### GPU implementation
+PASTE now is compatible with gpu via Pytorch. All we need to do is add the following two parameters to our main functions:
+```
+pi12 = pst.pairwise_align(slice1, slice2, backend = ot.backend.TorchBackend(), use_gpu = True)
+
+center_slice, pis = pst.center_align(initial_slice, slices, lmbda, backend = ot.backend.TorchBackend(), use_gpu = True) 
+```
+For more details, see the GPU section of the [Tutorial notebook](docs/source/notebooks/getting-started.ipynb).
+
+### Command Line
+
+We provide the option of running PASTE from the command line. 
+
+First, clone the repository:
+
+`git clone https://github.com/raphael-group/paste.git`
+
+Next, when providing files, you will need to provide two separate files: the gene expression data followed by spatial data (both as .csv) for the code to initialize one slice object.
+
+Sample execution (based on this repo): `python paste-cmd-line.py -m center -f ./sample_data/slice1.csv ./sample_data/slice1_coor.csv ./sample_data/slice2.csv ./sample_data/slice2_coor.csv ./sample_data/slice3.csv ./sample_data/slice3_coor.csv`
+
+Note: `pairwise` will return pairwise alignment between each consecutive pair of slices (e.g. \[slice1,slice2\], \[slice2,slice3\]).
+
+| Flag | Name | Description | Default Value |
+| --- | --- | --- | --- |
+| -m | mode | Select either `pairwise` or `center` | (str) `pairwise` |
+| -f | files | Path to data files (.csv) | None |
+| -d | direc | Directory to store output files | Current Directory |
+| -a | alpha | Alpha parameter for PASTE | (float) `0.1` |
+| -c | cost | Expression dissimilarity cost (`kl` or `Euclidean`) | (str) `kl` |
+| -p | n_components | n_components for NMF step in `center_align` | (int) `15` |
+| -l | lmbda | Lambda parameter in `center_align` | (floats) probability vector of length `n`  |
+| -i | intial_slice | Specify which file is also the intial slice in `center_align` | (int) `1` |
+| -t | threshold | Convergence threshold for `center_align` | (float) `0.001` |
+| -x | coordinates | Output new coordinates (toggle to turn on) | `False` |
+| -w | weights | Weights files of spots in each slice (.csv) | None |
+| -s | start | Initial alignments for OT. If not given uses uniform (.csv structure similar to alignment output) | None |
+
+`pairwise_align` outputs a (.csv) file containing mapping of spots between each consecutive pair of slices. The rows correspond to spots of the first slice, and cols the second.
+
+`center_align` outputs two files containing the low dimensional representation (NMF decomposition) of the center slice gene expression, and files containing a mapping of spots between the center slice (rows) to each input slice (cols).
+
+### Sample Dataset
+
+Added sample spatial transcriptomics dataset consisting of four breast cancer slice courtesy of:
+
+[1] Ståhl, Patrik & Salmén, Fredrik & Vickovic, Sanja & Lundmark, Anna & Fernandez Navarro, Jose & Magnusson, Jens & Giacomello, Stefania & Asp, Michaela & Westholm, Jakub & Huss, Mikael & Mollbrink, Annelie & Linnarsson, Sten & Codeluppi, Simone & Borg, Åke & Pontén, Fredrik & Costea, Paul & Sahlén, Pelin Akan & Mulder, Jan & Bergmann, Olaf & Frisén, Jonas. (2016). Visualization and analysis of gene expression in tissue sections by spatial transcriptomics. Science. 353. 78-82. 10.1126/science.aaf2403. 
+
+Note: Original data is (.tsv), but we converted it to (.csv).
+
+### References
+
+Ron Zeira, Max Land, Alexander Strzalkowski and Benjamin J. Raphael. "Alignment and integration of spatial transcriptomics data". Nature Methods (2022). https://doi.org/10.1038/s41592-022-01459-6
```

### Comparing `paste-bio-1.3.0/README.md` & `paste-bio-1.4.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,168 +1,183 @@
-[![PyPI](https://img.shields.io/pypi/v/paste-bio.svg)](https://pypi.org/project/paste-bio)
-[![Downloads](https://pepy.tech/badge/paste-bio)](https://pepy.tech/project/paste-bio)
-[![Documentation Status](https://readthedocs.org/projects/paste-bio/badge/?version=latest)](https://paste-bio.readthedocs.io/en/stable/?badge=stable)
-
-# PASTE
-
-![PASTE Overview](https://github.com/raphael-group/paste/blob/main/docs/source/_static/images/paste_overview.png)
-
-PASTE is a computational method that leverages both gene expression similarity and spatial distances between spots to align and integrate spatial transcriptomics data. In particular, there are two methods:
-1. `pairwise_align`: align spots across pairwise slices.
-2. `center_align`: integrate multiple slices into one center slice.
-
-You can read full paper [here](https://www.nature.com/articles/s41592-022-01459-6). 
-
-Additional examples and the code to reproduce the paper's analyses can be found [here](https://github.com/raphael-group/paste_reproducibility). Preprocessed datasets used in the paper can be found on [zenodo](https://doi.org/10.5281/zenodo.6334774).
-
-PASTE is actively being worked on with future updates coming. 
-
-### Recent News
-
-* PASTE is now published in [Nature Methods](https://www.nature.com/articles/s41592-022-01459-6)!
-
-* The code to reproduce the analisys can be found [here](https://github.com/raphael-group/paste_reproducibility).
-
-* As of version 1.2.0, PASTE now supports GPU implementation via Pytorch. For more details, see the GPU section of the [Tutorial notebook](docs/source/notebooks/getting-started.ipynb).
-
-### Installation
-
-The easiest way is to install PASTE on pypi: https://pypi.org/project/paste-bio/. 
-
-`pip install paste-bio` 
-
-Or you can install PASTE on bioconda: https://anaconda.org/bioconda/paste-bio.
-
-`conda install -c bioconda paste-bio`
-
-Check out Tutorial.ipynb for an example of how to use PASTE.
-
-Alternatively, you can clone the respository and try the following example in a
-notebook or the command line. 
-
-### Quick Start
-
-To use PASTE we require at least two slices of spatial-omics data (both
-expression and coordinates) that are in
-anndata format (i.e. read in by scanpy/squidpy). We have included a breast
-cancer dataset from [1] in the [sample_data folder](sample_data/) of this repo 
-that we will use as an example below to show how to use PASTE.
-
-```python
-import matplotlib.pyplot as plt
-import matplotlib.patches as mpatches
-import numpy as np
-import scanpy as sc
-import paste as pst
-
-# Load Slices
-data_dir = './sample_data/' # change this path to the data you wish to analyze
-
-# Assume that the coordinates of slices are named slice_name + "_coor.csv"
-def load_slices(data_dir, slice_names=["slice1", "slice2"]):
-    slices = []  
-    for slice_name in slice_names:
-        slice_i = sc.read_csv(data_dir + slice_name + ".csv")
-        slice_i_coor = np.genfromtxt(data_dir + slice_name + "_coor.csv", delimiter = ',')
-        slice_i.obsm['spatial'] = slice_i_coor
-        # Preprocess slices
-        sc.pp.filter_genes(slice_i, min_counts = 15)
-        sc.pp.filter_cells(slice_i, min_counts = 100)
-        slices.append(slice_i)
-    return slices
-
-slices = load_slices(data_dir)
-slice1, slice2 = slices
-
-# Pairwise align the slices
-pi12 = pst.pairwise_align(slice1, slice2)
-
-# To visualize the alignment you can stack the slices 
-# according to the alignment pi
-slices, pis = [slice1, slice2], [pi12]
-new_slices = pst.stack_slices_pairwise(slices, pis)
-
-slice_colors = ['#e41a1c','#377eb8']
-plt.figure(figsize=(7,7))
-for i in range(len(new_slices)):
-    pst.plot_slice(new_slices[i],slice_colors[i],s=400)
-plt.legend(handles=[mpatches.Patch(color=slice_colors[0], label='1'),mpatches.Patch(color=slice_colors[1], label='2')])
-plt.gca().invert_yaxis()
-plt.axis('off')
-plt.show()
-
-# Center align slices
-## We have to reload the slices as pairwise_alignment modifies the slices.
-slices = load_slices(data_dir)
-slice1, slice2 = slices
-
-# Construct a center slice
-## choose one of the slices as the coordinate reference for the center slice,
-## i.e. the center slice will have the same number of spots as this slice and
-## the same coordinates.
-initial_slice = slice1.copy()    
-slices = [slice1, slice2]
-lmbda = len(slices)*[1/len(slices)] # set hyperparameter to be uniform
-
-## Possible to pass in an initial pi (as keyword argument pis_init) 
-## to improve performance, see Tutorial.ipynb notebook for more details.
-center_slice, pis = pst.center_align(initial_slice, slices, lmbda) 
-
-## The low dimensional representation of our center slice is held 
-## in the matrices W and H, which can be used for downstream analyses
-W = center_slice.uns['paste_W']
-H = center_slice.uns['paste_H']
-```
-
-### GPU implementation
-PASTE now is compatible with gpu via Pytorch. All we need to do is add the following two parameters to our main functions:
-```
-pi12 = pst.pairwise_align(slice1, slice2, backend = ot.backend.TorchBackend(), use_gpu = True)
-
-center_slice, pis = pst.center_align(initial_slice, slices, lmbda, backend = ot.backend.TorchBackend(), use_gpu = True) 
-```
-For more details, see the GPU section of the [Tutorial notebook](docs/source/notebooks/getting-started.ipynb).
-
-### Command Line
-
-We provide the option of running PASTE from the command line. 
-
-First, clone the repository:
-
-`git clone https://github.com/raphael-group/paste.git`
-
-Next, when providing files, you will need to provide two separate files: the gene expression data followed by spatial data (both as .csv) for the code to initialize one slice object.
-
-Sample execution (based on this repo): `python paste-cmd-line.py -m center -f ./sample_data/slice1.csv ./sample_data/slice1_coor.csv ./sample_data/slice2.csv ./sample_data/slice2_coor.csv ./sample_data/slice3.csv ./sample_data/slice3_coor.csv`
-
-Note: `pairwise` will return pairwise alignment between each consecutive pair of slices (e.g. \[slice1,slice2\], \[slice2,slice3\]).
-
-| Flag | Name | Description | Default Value |
-| --- | --- | --- | --- |
-| -m | mode | Select either `pairwise` or `center` | (str) `pairwise` |
-| -f | files | Path to data files (.csv) | None |
-| -d | direc | Directory to store output files | Current Directory |
-| -a | alpha | Alpha parameter for PASTE | (float) `0.1` |
-| -c | cost | Expression dissimilarity cost (`kl` or `Euclidean`) | (str) `kl` |
-| -p | n_components | n_components for NMF step in `center_align` | (int) `15` |
-| -l | lmbda | Lambda parameter in `center_align` | (floats) probability vector of length `n`  |
-| -i | intial_slice | Specify which file is also the intial slice in `center_align` | (int) `1` |
-| -t | threshold | Convergence threshold for `center_align` | (float) `0.001` |
-| -x | coordinates | Output new coordinates (toggle to turn on) | `False` |
-| -w | weights | Weights files of spots in each slice (.csv) | None |
-| -s | start | Initial alignments for OT. If not given uses uniform (.csv structure similar to alignment output) | None |
-
-`pairwise_align` outputs a (.csv) file containing mapping of spots between each consecutive pair of slices. The rows correspond to spots of the first slice, and cols the second.
-
-`center_align` outputs two files containing the low dimensional representation (NMF decomposition) of the center slice gene expression, and files containing a mapping of spots between the center slice (rows) to each input slice (cols).
-
-### Sample Dataset
-
-Added sample spatial transcriptomics dataset consisting of four breast cancer slice courtesy of:
-
-[1] Ståhl, Patrik & Salmén, Fredrik & Vickovic, Sanja & Lundmark, Anna & Fernandez Navarro, Jose & Magnusson, Jens & Giacomello, Stefania & Asp, Michaela & Westholm, Jakub & Huss, Mikael & Mollbrink, Annelie & Linnarsson, Sten & Codeluppi, Simone & Borg, Åke & Pontén, Fredrik & Costea, Paul & Sahlén, Pelin Akan & Mulder, Jan & Bergmann, Olaf & Frisén, Jonas. (2016). Visualization and analysis of gene expression in tissue sections by spatial transcriptomics. Science. 353. 78-82. 10.1126/science.aaf2403. 
-
-Note: Original data is (.tsv), but we converted it to (.csv).
-
-### References
-
-Ron Zeira, Max Land, Alexander Strzalkowski and Benjamin J. Raphael. "Alignment and integration of spatial transcriptomics data". Nature Methods (2022). https://doi.org/10.1038/s41592-022-01459-6
+Metadata-Version: 2.1
+Name: paste-bio
+Version: 1.4.0
+Summary: A computational method to align and integrate spatial transcriptomics experiments.
+Home-page: https://github.com/raphael-group/paste
+Author: Max Land
+Author-email: max.ruikang.land@gmail.com
+Project-URL: Bug Tracker, https://github.com/raphael-group/paste/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![PyPI](https://img.shields.io/pypi/v/paste-bio.svg)](https://pypi.org/project/paste-bio)
+[![Downloads](https://pepy.tech/badge/paste-bio)](https://pepy.tech/project/paste-bio)
+[![Documentation Status](https://readthedocs.org/projects/paste-bio/badge/?version=latest)](https://paste-bio.readthedocs.io/en/stable/?badge=stable)
+[![Anaconda](https://anaconda.org/bioconda/paste-bio/badges/version.svg)](https://anaconda.org/bioconda/paste-bio/badges/version.svg)
+[![bioconda-downloads](https://anaconda.org/bioconda/paste-bio/badges/downloads.svg)](https://anaconda.org/bioconda/paste-bio/badges/downloads.svg)
+
+# PASTE
+
+![PASTE Overview](https://github.com/raphael-group/paste/blob/main/docs/source/_static/images/paste_overview.png)
+
+PASTE is a computational method that leverages both gene expression similarity and spatial distances between spots to align and integrate spatial transcriptomics data. In particular, there are two methods:
+1. `pairwise_align`: align spots across pairwise slices.
+2. `center_align`: integrate multiple slices into one center slice.
+
+You can read full paper [here](https://www.nature.com/articles/s41592-022-01459-6). 
+
+Additional examples and the code to reproduce the paper's analyses can be found [here](https://github.com/raphael-group/paste_reproducibility). Preprocessed datasets used in the paper can be found on [zenodo](https://doi.org/10.5281/zenodo.6334774).
+
+### Recent News
+
+* PASTE is now published in [Nature Methods](https://www.nature.com/articles/s41592-022-01459-6)!
+
+* The code to reproduce the analisys can be found [here](https://github.com/raphael-group/paste_reproducibility).
+
+* As of version 1.2.0, PASTE now supports GPU implementation via Pytorch. For more details, see the GPU section of the [Tutorial notebook](docs/source/notebooks/getting-started.ipynb).
+
+### Installation
+
+The easiest way is to install PASTE on pypi: https://pypi.org/project/paste-bio/. 
+
+`pip install paste-bio` 
+
+Or you can install PASTE on bioconda: https://anaconda.org/bioconda/paste-bio.
+
+`conda install -c bioconda paste-bio`
+
+Check out Tutorial.ipynb for an example of how to use PASTE.
+
+Alternatively, you can clone the respository and try the following example in a
+notebook or the command line. 
+
+### Quick Start
+
+To use PASTE we require at least two slices of spatial-omics data (both
+expression and coordinates) that are in
+anndata format (i.e. read in by scanpy/squidpy). We have included a breast
+cancer dataset from [1] in the [sample_data folder](sample_data/) of this repo 
+that we will use as an example below to show how to use PASTE.
+
+```python
+import matplotlib.pyplot as plt
+import matplotlib.patches as mpatches
+import numpy as np
+import scanpy as sc
+import paste as pst
+
+# Load Slices
+data_dir = './sample_data/' # change this path to the data you wish to analyze
+
+# Assume that the coordinates of slices are named slice_name + "_coor.csv"
+def load_slices(data_dir, slice_names=["slice1", "slice2"]):
+    slices = []  
+    for slice_name in slice_names:
+        slice_i = sc.read_csv(data_dir + slice_name + ".csv")
+        slice_i_coor = np.genfromtxt(data_dir + slice_name + "_coor.csv", delimiter = ',')
+        slice_i.obsm['spatial'] = slice_i_coor
+        # Preprocess slices
+        sc.pp.filter_genes(slice_i, min_counts = 15)
+        sc.pp.filter_cells(slice_i, min_counts = 100)
+        slices.append(slice_i)
+    return slices
+
+slices = load_slices(data_dir)
+slice1, slice2 = slices
+
+# Pairwise align the slices
+pi12 = pst.pairwise_align(slice1, slice2)
+
+# To visualize the alignment you can stack the slices 
+# according to the alignment pi
+slices, pis = [slice1, slice2], [pi12]
+new_slices = pst.stack_slices_pairwise(slices, pis)
+
+slice_colors = ['#e41a1c','#377eb8']
+plt.figure(figsize=(7,7))
+for i in range(len(new_slices)):
+    pst.plot_slice(new_slices[i],slice_colors[i],s=400)
+plt.legend(handles=[mpatches.Patch(color=slice_colors[0], label='1'),mpatches.Patch(color=slice_colors[1], label='2')])
+plt.gca().invert_yaxis()
+plt.axis('off')
+plt.show()
+
+# Center align slices
+## We have to reload the slices as pairwise_alignment modifies the slices.
+slices = load_slices(data_dir)
+slice1, slice2 = slices
+
+# Construct a center slice
+## choose one of the slices as the coordinate reference for the center slice,
+## i.e. the center slice will have the same number of spots as this slice and
+## the same coordinates.
+initial_slice = slice1.copy()    
+slices = [slice1, slice2]
+lmbda = len(slices)*[1/len(slices)] # set hyperparameter to be uniform
+
+## Possible to pass in an initial pi (as keyword argument pis_init) 
+## to improve performance, see Tutorial.ipynb notebook for more details.
+center_slice, pis = pst.center_align(initial_slice, slices, lmbda) 
+
+## The low dimensional representation of our center slice is held 
+## in the matrices W and H, which can be used for downstream analyses
+W = center_slice.uns['paste_W']
+H = center_slice.uns['paste_H']
+```
+
+### GPU implementation
+PASTE now is compatible with gpu via Pytorch. All we need to do is add the following two parameters to our main functions:
+```
+pi12 = pst.pairwise_align(slice1, slice2, backend = ot.backend.TorchBackend(), use_gpu = True)
+
+center_slice, pis = pst.center_align(initial_slice, slices, lmbda, backend = ot.backend.TorchBackend(), use_gpu = True) 
+```
+For more details, see the GPU section of the [Tutorial notebook](docs/source/notebooks/getting-started.ipynb).
+
+### Command Line
+
+We provide the option of running PASTE from the command line. 
+
+First, clone the repository:
+
+`git clone https://github.com/raphael-group/paste.git`
+
+Next, when providing files, you will need to provide two separate files: the gene expression data followed by spatial data (both as .csv) for the code to initialize one slice object.
+
+Sample execution (based on this repo): `python paste-cmd-line.py -m center -f ./sample_data/slice1.csv ./sample_data/slice1_coor.csv ./sample_data/slice2.csv ./sample_data/slice2_coor.csv ./sample_data/slice3.csv ./sample_data/slice3_coor.csv`
+
+Note: `pairwise` will return pairwise alignment between each consecutive pair of slices (e.g. \[slice1,slice2\], \[slice2,slice3\]).
+
+| Flag | Name | Description | Default Value |
+| --- | --- | --- | --- |
+| -m | mode | Select either `pairwise` or `center` | (str) `pairwise` |
+| -f | files | Path to data files (.csv) | None |
+| -d | direc | Directory to store output files | Current Directory |
+| -a | alpha | Alpha parameter for PASTE | (float) `0.1` |
+| -c | cost | Expression dissimilarity cost (`kl` or `Euclidean`) | (str) `kl` |
+| -p | n_components | n_components for NMF step in `center_align` | (int) `15` |
+| -l | lmbda | Lambda parameter in `center_align` | (floats) probability vector of length `n`  |
+| -i | intial_slice | Specify which file is also the intial slice in `center_align` | (int) `1` |
+| -t | threshold | Convergence threshold for `center_align` | (float) `0.001` |
+| -x | coordinates | Output new coordinates (toggle to turn on) | `False` |
+| -w | weights | Weights files of spots in each slice (.csv) | None |
+| -s | start | Initial alignments for OT. If not given uses uniform (.csv structure similar to alignment output) | None |
+
+`pairwise_align` outputs a (.csv) file containing mapping of spots between each consecutive pair of slices. The rows correspond to spots of the first slice, and cols the second.
+
+`center_align` outputs two files containing the low dimensional representation (NMF decomposition) of the center slice gene expression, and files containing a mapping of spots between the center slice (rows) to each input slice (cols).
+
+### Sample Dataset
+
+Added sample spatial transcriptomics dataset consisting of four breast cancer slice courtesy of:
+
+[1] Ståhl, Patrik & Salmén, Fredrik & Vickovic, Sanja & Lundmark, Anna & Fernandez Navarro, Jose & Magnusson, Jens & Giacomello, Stefania & Asp, Michaela & Westholm, Jakub & Huss, Mikael & Mollbrink, Annelie & Linnarsson, Sten & Codeluppi, Simone & Borg, Åke & Pontén, Fredrik & Costea, Paul & Sahlén, Pelin Akan & Mulder, Jan & Bergmann, Olaf & Frisén, Jonas. (2016). Visualization and analysis of gene expression in tissue sections by spatial transcriptomics. Science. 353. 78-82. 10.1126/science.aaf2403. 
+
+Note: Original data is (.tsv), but we converted it to (.csv).
+
+### References
+
+Ron Zeira, Max Land, Alexander Strzalkowski and Benjamin J. Raphael. "Alignment and integration of spatial transcriptomics data". Nature Methods (2022). https://doi.org/10.1038/s41592-022-01459-6
```

### Comparing `paste-bio-1.3.0/setup.cfg` & `paste-bio-1.4.0/setup.cfg`

 * *Files 27% similar despite different names*

```diff
@@ -1,46 +1,44 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 2070 6173 7465 2d62 696f 0d0a 7665   = paste-bio..ve
-00000020: 7273 696f 6e20 3d20 312e 332e 300d 0a61  rsion = 1.3.0..a
-00000030: 7574 686f 7220 3d20 4d61 7820 4c61 6e64  uthor = Max Land
-00000040: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
-00000050: 206d 6178 2e72 7569 6b61 6e67 2e6c 616e   max.ruikang.lan
-00000060: 6440 676d 6169 6c2e 636f 6d0d 0a64 6573  d@gmail.com..des
-00000070: 6372 6970 7469 6f6e 203d 2041 2063 6f6d  cription = A com
-00000080: 7075 7461 7469 6f6e 616c 206d 6574 686f  putational metho
-00000090: 6420 746f 2061 6c69 676e 2061 6e64 2069  d to align and i
-000000a0: 6e74 6567 7261 7465 2073 7061 7469 616c  ntegrate spatial
-000000b0: 2074 7261 6e73 6372 6970 746f 6d69 6373   transcriptomics
-000000c0: 2065 7870 6572 696d 656e 7473 2e0d 0a6c   experiments...l
-000000d0: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
-000000e0: 3d20 6669 6c65 3a20 5245 4144 4d45 2e6d  = file: README.m
-000000f0: 640d 0a6c 6f6e 675f 6465 7363 7269 7074  d..long_descript
-00000100: 696f 6e5f 636f 6e74 656e 745f 7479 7065  ion_content_type
-00000110: 203d 2074 6578 742f 6d61 726b 646f 776e   = text/markdown
-00000120: 0d0a 7572 6c20 3d20 6874 7470 733a 2f2f  ..url = https://
-00000130: 6769 7468 7562 2e63 6f6d 2f72 6170 6861  github.com/rapha
-00000140: 656c 2d67 726f 7570 2f70 6173 7465 0d0a  el-group/paste..
-00000150: 7072 6f6a 6563 745f 7572 6c73 203d 200d  project_urls = .
-00000160: 0a09 4275 6720 5472 6163 6b65 7220 3d20  ..Bug Tracker = 
-00000170: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000180: 6f6d 2f72 6170 6861 656c 2d67 726f 7570  om/raphael-group
-00000190: 2f70 6173 7465 2f69 7373 7565 730d 0a63  /paste/issues..c
-000001a0: 6c61 7373 6966 6965 7273 203d 200d 0a09  lassifiers = ...
-000001b0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-000001c0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-000001d0: 3a20 330d 0a09 4c69 6365 6e73 6520 3a3a  : 3...License ::
-000001e0: 204f 5349 2041 7070 726f 7665 6420 3a3a   OSI Approved ::
-000001f0: 2042 5344 204c 6963 656e 7365 0d0a 094f   BSD License...O
-00000200: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
-00000210: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
-00000220: 740d 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a  t....[options]..
-00000230: 7061 636b 6167 655f 6469 7220 3d20 0d0a  package_dir = ..
-00000240: 093d 2073 7263 0d0a 7061 636b 6167 6573  .= src..packages
-00000250: 203d 2066 696e 643a 0d0a 7079 7468 6f6e   = find:..python
-00000260: 5f72 6571 7569 7265 7320 3d20 3e3d 332e  _requires = >=3.
-00000270: 360d 0a7a 6970 5f73 6166 6520 3d20 4661  6..zip_safe = Fa
-00000280: 6c73 650d 0a0d 0a5b 6f70 7469 6f6e 732e  lse....[options.
-00000290: 7061 636b 6167 6573 2e66 696e 645d 0d0a  packages.find]..
-000002a0: 7768 6572 6520 3d20 7372 630d 0a0d 0a5b  where = src....[
-000002b0: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
-000002c0: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
-000002d0: 6520 3d20 300d 0a0d 0a                   e = 0....
+00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
+00000010: 3d20 7061 7374 652d 6269 6f0a 7665 7273  = paste-bio.vers
+00000020: 696f 6e20 3d20 312e 342e 300a 6175 7468  ion = 1.4.0.auth
+00000030: 6f72 203d 204d 6178 204c 616e 640a 6175  or = Max Land.au
+00000040: 7468 6f72 5f65 6d61 696c 203d 206d 6178  thor_email = max
+00000050: 2e72 7569 6b61 6e67 2e6c 616e 6440 676d  .ruikang.land@gm
+00000060: 6169 6c2e 636f 6d0a 6465 7363 7269 7074  ail.com.descript
+00000070: 696f 6e20 3d20 4120 636f 6d70 7574 6174  ion = A computat
+00000080: 696f 6e61 6c20 6d65 7468 6f64 2074 6f20  ional method to 
+00000090: 616c 6967 6e20 616e 6420 696e 7465 6772  align and integr
+000000a0: 6174 6520 7370 6174 6961 6c20 7472 616e  ate spatial tran
+000000b0: 7363 7269 7074 6f6d 6963 7320 6578 7065  scriptomics expe
+000000c0: 7269 6d65 6e74 732e 0a6c 6f6e 675f 6465  riments..long_de
+000000d0: 7363 7269 7074 696f 6e20 3d20 6669 6c65  scription = file
+000000e0: 3a20 5245 4144 4d45 2e6d 640a 6c6f 6e67  : README.md.long
+000000f0: 5f64 6573 6372 6970 7469 6f6e 5f63 6f6e  _description_con
+00000100: 7465 6e74 5f74 7970 6520 3d20 7465 7874  tent_type = text
+00000110: 2f6d 6172 6b64 6f77 6e0a 7572 6c20 3d20  /markdown.url = 
+00000120: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000130: 6f6d 2f72 6170 6861 656c 2d67 726f 7570  om/raphael-group
+00000140: 2f70 6173 7465 0a70 726f 6a65 6374 5f75  /paste.project_u
+00000150: 726c 7320 3d20 0a09 4275 6720 5472 6163  rls = ..Bug Trac
+00000160: 6b65 7220 3d20 6874 7470 733a 2f2f 6769  ker = https://gi
+00000170: 7468 7562 2e63 6f6d 2f72 6170 6861 656c  thub.com/raphael
+00000180: 2d67 726f 7570 2f70 6173 7465 2f69 7373  -group/paste/iss
+00000190: 7565 730a 636c 6173 7369 6669 6572 7320  ues.classifiers 
+000001a0: 3d20 0a09 5072 6f67 7261 6d6d 696e 6720  = ..Programming 
+000001b0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+000001c0: 6f6e 203a 3a20 330a 094c 6963 656e 7365  on :: 3..License
+000001d0: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
+000001e0: 203a 3a20 4253 4420 4c69 6365 6e73 650a   :: BSD License.
+000001f0: 094f 7065 7261 7469 6e67 2053 7973 7465  .Operating Syste
+00000200: 6d20 3a3a 204f 5320 496e 6465 7065 6e64  m :: OS Independ
+00000210: 656e 740a 0a5b 6f70 7469 6f6e 735d 0a70  ent..[options].p
+00000220: 6163 6b61 6765 5f64 6972 203d 200a 093d  ackage_dir = ..=
+00000230: 2073 7263 0a70 6163 6b61 6765 7320 3d20   src.packages = 
+00000240: 6669 6e64 3a0a 7079 7468 6f6e 5f72 6571  find:.python_req
+00000250: 7569 7265 7320 3d20 3e3d 332e 360a 7a69  uires = >=3.6.zi
+00000260: 705f 7361 6665 203d 2046 616c 7365 0a0a  p_safe = False..
+00000270: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
+00000280: 732e 6669 6e64 5d0a 7768 6572 6520 3d20  s.find].where = 
+00000290: 7372 630a 0a5b 6567 675f 696e 666f 5d0a  src..[egg_info].
+000002a0: 7461 675f 6275 696c 6420 3d20 0a74 6167  tag_build = .tag
+000002b0: 5f64 6174 6520 3d20 300a 0a              _date = 0..
```

### Comparing `paste-bio-1.3.0/src/paste/PASTE.py` & `paste-bio-1.4.0/src/paste/PASTE.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,352 +1,434 @@
-from typing import List, Tuple, Optional
-import numpy as np
-from anndata import AnnData
-import ot
-from sklearn.decomposition import NMF
-from .helper import intersect, kl_divergence_backend, to_dense_array, extract_data_matrix
-
-def pairwise_align(
-    sliceA: AnnData, 
-    sliceB: AnnData, 
-    alpha: float = 0.1, 
-    dissimilarity: str ='kl', 
-    use_rep: Optional[str] = None, 
-    G_init = None, 
-    a_distribution = None, 
-    b_distribution = None, 
-    norm: bool = False, 
-    numItermax: int = 200, 
-    backend = ot.backend.NumpyBackend(), 
-    use_gpu: bool = False, 
-    return_obj: bool = False, 
-    verbose: bool = False, 
-    gpu_verbose: bool = True, 
-    **kwargs) -> Tuple[np.ndarray, Optional[int]]:
-    """
-    Calculates and returns optimal alignment of two slices. 
-    
-    Args:
-        sliceA: Slice A to align.
-        sliceB: Slice B to align.
-        alpha:  Alignment tuning parameter. Note: 0 <= alpha <= 1.
-        dissimilarity: Expression dissimilarity measure: ``'kl'`` or ``'euclidean'``.
-        use_rep: If ``None``, uses ``slice.X`` to calculate dissimilarity between spots, otherwise uses the representation given by ``slice.obsm[use_rep]``.
-        G_init (array-like, optional): Initial mapping to be used in FGW-OT, otherwise default is uniform mapping.
-        a_distribution (array-like, optional): Distribution of sliceA spots, otherwise default is uniform.
-        b_distribution (array-like, optional): Distribution of sliceB spots, otherwise default is uniform.
-        numItermax: Max number of iterations during FGW-OT.
-        norm: If ``True``, scales spatial distances such that neighboring spots are at distance 1. Otherwise, spatial distances remain unchanged.
-        backend: Type of backend to run calculations. For list of backends available on system: ``ot.backend.get_backend_list()``.
-        use_gpu: If ``True``, use gpu. Otherwise, use cpu. Currently we only have gpu support for Pytorch.
-        return_obj: If ``True``, additionally returns objective function output of FGW-OT.
-        verbose: If ``True``, FGW-OT is verbose.
-        gpu_verbose: If ``True``, print whether gpu is being used to user.
-   
-    Returns:
-        - Alignment of spots.
-
-        If ``return_obj = True``, additionally returns:
-        
-        - Objective function output of FGW-OT.
-    """
-    
-    # Determine if gpu or cpu is being used
-    if use_gpu:
-        try:
-            import torch
-        except:
-             print("We currently only have gpu support for Pytorch. Please install torch.")
-                
-        if isinstance(backend,ot.backend.TorchBackend):
-            if torch.cuda.is_available():
-                if gpu_verbose:
-                    print("gpu is available, using gpu.")
-            else:
-                if gpu_verbose:
-                    print("gpu is not available, resorting to torch cpu.")
-                use_gpu = False
-        else:
-            print("We currently only have gpu support for Pytorch, please set backend = ot.backend.TorchBackend(). Reverting to selected backend cpu.")
-            use_gpu = False
-    else:
-        if gpu_verbose:
-            print("Using selected backend cpu. If you want to use gpu, set use_gpu = True.")
-            
-    # subset for common genes
-    common_genes = intersect(sliceA.var.index, sliceB.var.index)
-    sliceA = sliceA[:, common_genes]
-    sliceB = sliceB[:, common_genes]
-    
-    # Backend
-    nx = backend    
-    
-    # Calculate spatial distances
-    coordinatesA = sliceA.obsm['spatial'].copy()
-    coordinatesA = nx.from_numpy(coordinatesA)
-    coordinatesB = sliceB.obsm['spatial'].copy()
-    coordinatesB = nx.from_numpy(coordinatesB)
-    
-    if isinstance(nx,ot.backend.TorchBackend):
-        coordinatesA = coordinatesA.float()
-        coordinatesB = coordinatesB.float()
-    D_A = ot.dist(coordinatesA,coordinatesA, metric='euclidean')
-    D_B = ot.dist(coordinatesB,coordinatesB, metric='euclidean')
-
-    if isinstance(nx,ot.backend.TorchBackend) and use_gpu:
-        D_A = D_A.cuda()
-        D_B = D_B.cuda()
-    
-    # Calculate expression dissimilarity
-    A_X, B_X = nx.from_numpy(to_dense_array(extract_data_matrix(sliceA,use_rep))), nx.from_numpy(to_dense_array(extract_data_matrix(sliceB,use_rep)))
-
-    if isinstance(nx,ot.backend.TorchBackend) and use_gpu:
-        A_X = A_X.cuda()
-        B_X = B_X.cuda()
-
-    if dissimilarity.lower()=='euclidean' or dissimilarity.lower()=='euc':
-        M = ot.dist(A_X,B_X)
-    else:
-        s_A = A_X + 0.01
-        s_B = B_X + 0.01
-        M = kl_divergence_backend(s_A, s_B)
-        M = nx.from_numpy(M)
-    
-    if isinstance(nx,ot.backend.TorchBackend) and use_gpu:
-        M = M.cuda()
-    
-    # init distributions
-    if a_distribution is None:
-        a = nx.ones((sliceA.shape[0],))/sliceA.shape[0]
-    else:
-        a = nx.from_numpy(a_distribution)
-        
-    if b_distribution is None:
-        b = nx.ones((sliceB.shape[0],))/sliceB.shape[0]
-    else:
-        b = nx.from_numpy(b_distribution)
-
-    if isinstance(nx,ot.backend.TorchBackend) and use_gpu:
-        a = a.cuda()
-        b = b.cuda()
-    
-    if norm:
-        D_A /= nx.min(D_A[D_A>0])
-        D_B /= nx.min(D_B[D_B>0])
-    
-    # Run OT
-    if G_init is not None:
-        G_init = nx.from_numpy(G_init)
-        if isinstance(nx,ot.backend.TorchBackend):
-            G_init = G_init.float()
-            if use_gpu:
-                G_init.cuda()
-    pi, logw = my_fused_gromov_wasserstein(M, D_A, D_B, a, b, G_init = G_init, loss_fun='square_loss', alpha= alpha, log=True, numItermax=numItermax,verbose=verbose, use_gpu = use_gpu)
-    pi = nx.to_numpy(pi)
-    obj = nx.to_numpy(logw['fgw_dist'])
-    if isinstance(backend,ot.backend.TorchBackend) and use_gpu:
-        torch.cuda.empty_cache()
-
-    if return_obj:
-        return pi, obj
-    return pi
-
-
-def center_align(
-    A: AnnData, 
-    slices: List[AnnData], 
-    lmbda = None, 
-    alpha: float = 0.1, 
-    n_components: int = 15, 
-    threshold: float = 0.001, 
-    max_iter: int = 10, 
-    dissimilarity: str ='kl', 
-    norm: bool = False, 
-    random_seed: Optional[int] = None, 
-    pis_init: Optional[List[np.ndarray]] = None, 
-    distributions = None, 
-    backend = ot.backend.NumpyBackend(), 
-    use_gpu: bool = False, 
-    verbose: bool = False, 
-    gpu_verbose: bool = True) -> Tuple[AnnData, List[np.ndarray]]:
-    """
-    Computes center alignment of slices.
-    
-    Args:
-        A: Slice to use as the initialization for center alignment; Make sure to include gene expression and spatial information.
-        slices: List of slices to use in the center alignment.
-        lmbda (array-like, optional): List of probability weights assigned to each slice; If ``None``, use uniform weights.
-        alpha:  Alignment tuning parameter. Note: 0 <= alpha <= 1.
-        n_components: Number of components in NMF decomposition.
-        threshold: Threshold for convergence of W and H during NMF decomposition.
-        max_iter: Maximum number of iterations for our center alignment algorithm.
-        dissimilarity: Expression dissimilarity measure: ``'kl'`` or ``'euclidean'``.
-        norm:  If ``True``, scales spatial distances such that neighboring spots are at distance 1. Otherwise, spatial distances remain unchanged.
-        random_seed: Set random seed for reproducibility.
-        pis_init: Initial list of mappings between 'A' and 'slices' to solver. Otherwise, default will automatically calculate mappings.
-        distributions (List[array-like], optional): Distributions of spots for each slice. Otherwise, default is uniform.
-        backend: Type of backend to run calculations. For list of backends available on system: ``ot.backend.get_backend_list()``.
-        use_gpu: If ``True``, use gpu. Otherwise, use cpu. Currently we only have gpu support for Pytorch.
-        verbose: If ``True``, FGW-OT is verbose.
-        gpu_verbose: If ``True``, print whether gpu is being used to user.
-
-    Returns:
-        - Inferred center slice with full and low dimensional representations (W, H) of the gene expression matrix.
-        - List of pairwise alignment mappings of the center slice (rows) to each input slice (columns).
-    """
-    
-    # Determine if gpu or cpu is being used
-    if use_gpu:
-        try:
-            import torch
-        except:
-             print("We currently only have gpu support for Pytorch. Please install torch.")
-                
-        if isinstance(backend,ot.backend.TorchBackend):
-            if torch.cuda.is_available():
-                if gpu_verbose:
-                    print("gpu is available, using gpu.")
-            else:
-                if gpu_verbose:
-                    print("gpu is not available, resorting to torch cpu.")
-                use_gpu = False
-        else:
-            print("We currently only have gpu support for Pytorch, please set backend = ot.backend.TorchBackend(). Reverting to selected backend cpu.")
-            use_gpu = False
-    else:
-        if gpu_verbose:
-            print("Using selected backend cpu. If you want to use gpu, set use_gpu = True.")
-    
-    if lmbda is None:
-        lmbda = len(slices)*[1/len(slices)]
-    
-    if distributions is None:
-        distributions = len(slices)*[None]
-    
-    # get common genes
-    common_genes = A.var.index
-    for s in slices:
-        common_genes = intersect(common_genes, s.var.index)
-
-    # subset common genes
-    A = A[:, common_genes]
-    for i in range(len(slices)):
-        slices[i] = slices[i][:, common_genes]
-    print('Filtered all slices for common genes. There are ' + str(len(common_genes)) + ' common genes.')
-
-    # Run initial NMF
-    if dissimilarity.lower()=='euclidean' or dissimilarity.lower()=='euc':
-        model = NMF(n_components=n_components, init='random', random_state = random_seed, verbose = verbose)
-    else:
-        model = NMF(n_components=n_components, solver = 'mu', beta_loss = 'kullback-leibler', init='random', random_state = random_seed, verbose = verbose)
-    
-    if pis_init is None:
-        pis = [None for i in range(len(slices))]
-        W = model.fit_transform(A.X)
-    else:
-        pis = pis_init
-        W = model.fit_transform(A.shape[0]*sum([lmbda[i]*np.dot(pis[i], to_dense_array(slices[i].X)) for i in range(len(slices))]))
-    H = model.components_
-    center_coordinates = A.obsm['spatial']
-    
-    if not isinstance(center_coordinates, np.ndarray):
-        print("Warning: A.obsm['spatial'] is not of type numpy array.")
-    
-    # Initialize center_slice
-    center_slice = AnnData(np.dot(W,H))
-    center_slice.var.index = common_genes
-    center_slice.obs.index = A.obs.index
-    center_slice.obsm['spatial'] = center_coordinates
-    
-    # Minimize R
-    iteration_count = 0
-    R = 0
-    R_diff = 100
-    while R_diff > threshold and iteration_count < max_iter:
-        print("Iteration: " + str(iteration_count))
-        pis, r = center_ot(W, H, slices, center_coordinates, common_genes, alpha, backend, use_gpu, dissimilarity = dissimilarity, norm = norm, G_inits = pis, distributions=distributions, verbose = verbose)
-        W, H = center_NMF(W, H, slices, pis, lmbda, n_components, random_seed, dissimilarity = dissimilarity, verbose = verbose)
-        R_new = np.dot(r,lmbda)
-        iteration_count += 1
-        R_diff = abs(R - R_new)
-        print("Objective ",R_new)
-        print("Difference: " + str(R_diff) + "\n")
-        R = R_new
-    center_slice = A.copy()
-    center_slice.X = np.dot(W, H)
-    center_slice.uns['paste_W'] = W
-    center_slice.uns['paste_H'] = H
-    center_slice.uns['full_rank'] = center_slice.shape[0]*sum([lmbda[i]*np.dot(pis[i], to_dense_array(slices[i].X)) for i in range(len(slices))])
-    center_slice.uns['obj'] = R
-    return center_slice, pis
-
-#--------------------------- HELPER METHODS -----------------------------------
-
-def center_ot(W, H, slices, center_coordinates, common_genes, alpha, backend, use_gpu, dissimilarity = 'kl', norm = False, G_inits = None, distributions=None, verbose = False):
-    center_slice = AnnData(np.dot(W,H))
-    center_slice.var.index = common_genes
-    center_slice.obsm['spatial'] = center_coordinates
-
-    if distributions is None:
-        distributions = len(slices)*[None]
-
-    pis = []
-    r = []
-    print('Solving Pairwise Slice Alignment Problem.')
-    for i in range(len(slices)):
-        p, r_q = pairwise_align(center_slice, slices[i], alpha = alpha, dissimilarity = dissimilarity, norm = norm, return_obj = True, G_init = G_inits[i], b_distribution=distributions[i], backend = backend, use_gpu = use_gpu, verbose = verbose, gpu_verbose = False)
-        pis.append(p)
-        r.append(r_q)
-    return pis, np.array(r)
-
-def center_NMF(W, H, slices, pis, lmbda, n_components, random_seed, dissimilarity = 'kl', verbose = False):
-    print('Solving Center Mapping NMF Problem.')
-    n = W.shape[0]
-    B = n*sum([lmbda[i]*np.dot(pis[i], to_dense_array(slices[i].X)) for i in range(len(slices))])
-    if dissimilarity.lower()=='euclidean' or dissimilarity.lower()=='euc':
-        model = NMF(n_components=n_components, init='random', random_state = random_seed, verbose = verbose)
-    else:
-        model = NMF(n_components=n_components, solver = 'mu', beta_loss = 'kullback-leibler', init='random', random_state = random_seed, verbose = verbose)
-    W_new = model.fit_transform(B)
-    H_new = model.components_
-    return W_new, H_new
-
-def my_fused_gromov_wasserstein(M, C1, C2, p, q, G_init = None, loss_fun='square_loss', alpha=0.5, armijo=False, log=False,numItermax=200, use_gpu = False, **kwargs):
-    """
-    Adapted fused_gromov_wasserstein with the added capability of defining a G_init (inital mapping).
-    Also added capability of utilizing different POT backends to speed up computation.
-    
-    For more info, see: https://pythonot.github.io/gen_modules/ot.gromov.html
-    """
-
-    p, q = ot.utils.list_to_array(p, q)
-
-    p0, q0, C10, C20, M0 = p, q, C1, C2, M
-    nx = ot.backend.get_backend(p0, q0, C10, C20, M0)
-
-    constC, hC1, hC2 = ot.gromov.init_matrix(C1, C2, p, q, loss_fun)
-
-    if G_init is None:
-        G0 = p[:, None] * q[None, :]
-    else:
-        G0 = (1/nx.sum(G_init)) * G_init
-        if use_gpu:
-            G0 = G0.cuda()
-
-    def f(G):
-        return ot.gromov.gwloss(constC, hC1, hC2, G)
-
-    def df(G):
-        return ot.gromov.gwggrad(constC, hC1, hC2, G)
-
-    if log:
-        res, log = ot.gromov.cg(p, q, (1 - alpha) * M, alpha, f, df, G0, armijo=armijo, C1=C1, C2=C2, constC=constC, log=True, **kwargs)
-
-        fgw_dist = log['loss'][-1]
-
-        log['fgw_dist'] = fgw_dist
-        log['u'] = log['u']
-        log['v'] = log['v']
-        return res, log
-
-    else:
-        return ot.gromov.cg(p, q, (1 - alpha) * M, alpha, f, df, G0, armijo=armijo, C1=C1, C2=C2, constC=constC, **kwargs)
+from typing import List, Tuple, Optional
+import numpy as np
+from anndata import AnnData
+import ot
+from sklearn.decomposition import NMF
+from .helper import intersect, kl_divergence_backend, to_dense_array, extract_data_matrix
+
+def pairwise_align(
+    sliceA: AnnData, 
+    sliceB: AnnData, 
+    alpha: float = 0.1, 
+    dissimilarity: str ='kl', 
+    use_rep: Optional[str] = None, 
+    G_init = None, 
+    a_distribution = None, 
+    b_distribution = None, 
+    norm: bool = False, 
+    numItermax: int = 200, 
+    backend = ot.backend.NumpyBackend(), 
+    use_gpu: bool = False, 
+    return_obj: bool = False, 
+    verbose: bool = False, 
+    gpu_verbose: bool = True, 
+    **kwargs) -> Tuple[np.ndarray, Optional[int]]:
+    """
+    Calculates and returns optimal alignment of two slices. 
+    
+    Args:
+        sliceA: Slice A to align.
+        sliceB: Slice B to align.
+        alpha:  Alignment tuning parameter. Note: 0 <= alpha <= 1.
+        dissimilarity: Expression dissimilarity measure: ``'kl'`` or ``'euclidean'``.
+        use_rep: If ``None``, uses ``slice.X`` to calculate dissimilarity between spots, otherwise uses the representation given by ``slice.obsm[use_rep]``.
+        G_init (array-like, optional): Initial mapping to be used in FGW-OT, otherwise default is uniform mapping.
+        a_distribution (array-like, optional): Distribution of sliceA spots, otherwise default is uniform.
+        b_distribution (array-like, optional): Distribution of sliceB spots, otherwise default is uniform.
+        numItermax: Max number of iterations during FGW-OT.
+        norm: If ``True``, scales spatial distances such that neighboring spots are at distance 1. Otherwise, spatial distances remain unchanged.
+        backend: Type of backend to run calculations. For list of backends available on system: ``ot.backend.get_backend_list()``.
+        use_gpu: If ``True``, use gpu. Otherwise, use cpu. Currently we only have gpu support for Pytorch.
+        return_obj: If ``True``, additionally returns objective function output of FGW-OT.
+        verbose: If ``True``, FGW-OT is verbose.
+        gpu_verbose: If ``True``, print whether gpu is being used to user.
+   
+    Returns:
+        - Alignment of spots.
+
+        If ``return_obj = True``, additionally returns:
+        
+        - Objective function output of FGW-OT.
+    """
+    
+    # Determine if gpu or cpu is being used
+    if use_gpu:
+        try:
+            import torch
+        except:
+             print("We currently only have gpu support for Pytorch. Please install torch.")
+                
+        if isinstance(backend,ot.backend.TorchBackend):
+            if torch.cuda.is_available():
+                if gpu_verbose:
+                    print("gpu is available, using gpu.")
+            else:
+                if gpu_verbose:
+                    print("gpu is not available, resorting to torch cpu.")
+                use_gpu = False
+        else:
+            print("We currently only have gpu support for Pytorch, please set backend = ot.backend.TorchBackend(). Reverting to selected backend cpu.")
+            use_gpu = False
+    else:
+        if gpu_verbose:
+            print("Using selected backend cpu. If you want to use gpu, set use_gpu = True.")
+            
+    # subset for common genes
+    common_genes = intersect(sliceA.var.index, sliceB.var.index)
+    sliceA = sliceA[:, common_genes]
+    sliceB = sliceB[:, common_genes]
+
+    # check if slices are valid
+    for s in [sliceA, sliceB]:
+        if not len(s):
+            raise ValueError(f"Found empty `AnnData`:\n{sliceA}.")
+
+    
+    # Backend
+    nx = backend    
+    
+    # Calculate spatial distances
+    coordinatesA = sliceA.obsm['spatial'].copy()
+    coordinatesA = nx.from_numpy(coordinatesA)
+    coordinatesB = sliceB.obsm['spatial'].copy()
+    coordinatesB = nx.from_numpy(coordinatesB)
+    
+    if isinstance(nx,ot.backend.TorchBackend):
+        coordinatesA = coordinatesA.float()
+        coordinatesB = coordinatesB.float()
+    D_A = ot.dist(coordinatesA,coordinatesA, metric='euclidean')
+    D_B = ot.dist(coordinatesB,coordinatesB, metric='euclidean')
+
+    if isinstance(nx,ot.backend.TorchBackend) and use_gpu:
+        D_A = D_A.cuda()
+        D_B = D_B.cuda()
+    
+    # Calculate expression dissimilarity
+    A_X, B_X = nx.from_numpy(to_dense_array(extract_data_matrix(sliceA,use_rep))), nx.from_numpy(to_dense_array(extract_data_matrix(sliceB,use_rep)))
+
+    if isinstance(nx,ot.backend.TorchBackend) and use_gpu:
+        A_X = A_X.cuda()
+        B_X = B_X.cuda()
+
+    if dissimilarity.lower()=='euclidean' or dissimilarity.lower()=='euc':
+        M = ot.dist(A_X,B_X)
+    else:
+        s_A = A_X + 0.01
+        s_B = B_X + 0.01
+        M = kl_divergence_backend(s_A, s_B)
+        M = nx.from_numpy(M)
+    
+    if isinstance(nx,ot.backend.TorchBackend) and use_gpu:
+        M = M.cuda()
+    
+    # init distributions
+    if a_distribution is None:
+        a = nx.ones((sliceA.shape[0],))/sliceA.shape[0]
+    else:
+        a = nx.from_numpy(a_distribution)
+        
+    if b_distribution is None:
+        b = nx.ones((sliceB.shape[0],))/sliceB.shape[0]
+    else:
+        b = nx.from_numpy(b_distribution)
+
+    if isinstance(nx,ot.backend.TorchBackend) and use_gpu:
+        a = a.cuda()
+        b = b.cuda()
+    
+    if norm:
+        D_A /= nx.min(D_A[D_A>0])
+        D_B /= nx.min(D_B[D_B>0])
+    
+    # Run OT
+    if G_init is not None:
+        G_init = nx.from_numpy(G_init)
+        if isinstance(nx,ot.backend.TorchBackend):
+            G_init = G_init.float()
+            if use_gpu:
+                G_init.cuda()
+    pi, logw = my_fused_gromov_wasserstein(M, D_A, D_B, a, b, G_init = G_init, loss_fun='square_loss', alpha= alpha, log=True, numItermax=numItermax,verbose=verbose, use_gpu = use_gpu)
+    pi = nx.to_numpy(pi)
+    obj = nx.to_numpy(logw['fgw_dist'])
+    if isinstance(backend,ot.backend.TorchBackend) and use_gpu:
+        torch.cuda.empty_cache()
+
+    if return_obj:
+        return pi, obj
+    return pi
+
+
+def center_align(
+    A: AnnData, 
+    slices: List[AnnData], 
+    lmbda = None, 
+    alpha: float = 0.1, 
+    n_components: int = 15, 
+    threshold: float = 0.001, 
+    max_iter: int = 10, 
+    dissimilarity: str ='kl', 
+    norm: bool = False, 
+    random_seed: Optional[int] = None, 
+    pis_init: Optional[List[np.ndarray]] = None, 
+    distributions = None, 
+    backend = ot.backend.NumpyBackend(), 
+    use_gpu: bool = False, 
+    verbose: bool = False, 
+    gpu_verbose: bool = True) -> Tuple[AnnData, List[np.ndarray]]:
+    """
+    Computes center alignment of slices.
+    
+    Args:
+        A: Slice to use as the initialization for center alignment; Make sure to include gene expression and spatial information.
+        slices: List of slices to use in the center alignment.
+        lmbda (array-like, optional): List of probability weights assigned to each slice; If ``None``, use uniform weights.
+        alpha:  Alignment tuning parameter. Note: 0 <= alpha <= 1.
+        n_components: Number of components in NMF decomposition.
+        threshold: Threshold for convergence of W and H during NMF decomposition.
+        max_iter: Maximum number of iterations for our center alignment algorithm.
+        dissimilarity: Expression dissimilarity measure: ``'kl'`` or ``'euclidean'``.
+        norm:  If ``True``, scales spatial distances such that neighboring spots are at distance 1. Otherwise, spatial distances remain unchanged.
+        random_seed: Set random seed for reproducibility.
+        pis_init: Initial list of mappings between 'A' and 'slices' to solver. Otherwise, default will automatically calculate mappings.
+        distributions (List[array-like], optional): Distributions of spots for each slice. Otherwise, default is uniform.
+        backend: Type of backend to run calculations. For list of backends available on system: ``ot.backend.get_backend_list()``.
+        use_gpu: If ``True``, use gpu. Otherwise, use cpu. Currently we only have gpu support for Pytorch.
+        verbose: If ``True``, FGW-OT is verbose.
+        gpu_verbose: If ``True``, print whether gpu is being used to user.
+
+    Returns:
+        - Inferred center slice with full and low dimensional representations (W, H) of the gene expression matrix.
+        - List of pairwise alignment mappings of the center slice (rows) to each input slice (columns).
+    """
+    
+    # Determine if gpu or cpu is being used
+    if use_gpu:
+        try:
+            import torch
+        except:
+             print("We currently only have gpu support for Pytorch. Please install torch.")
+                
+        if isinstance(backend,ot.backend.TorchBackend):
+            if torch.cuda.is_available():
+                if gpu_verbose:
+                    print("gpu is available, using gpu.")
+            else:
+                if gpu_verbose:
+                    print("gpu is not available, resorting to torch cpu.")
+                use_gpu = False
+        else:
+            print("We currently only have gpu support for Pytorch, please set backend = ot.backend.TorchBackend(). Reverting to selected backend cpu.")
+            use_gpu = False
+    else:
+        if gpu_verbose:
+            print("Using selected backend cpu. If you want to use gpu, set use_gpu = True.")
+    
+    if lmbda is None:
+        lmbda = len(slices)*[1/len(slices)]
+    
+    if distributions is None:
+        distributions = len(slices)*[None]
+    
+    # get common genes
+    common_genes = A.var.index
+    for s in slices:
+        common_genes = intersect(common_genes, s.var.index)
+
+    # subset common genes
+    A = A[:, common_genes]
+    for i in range(len(slices)):
+        slices[i] = slices[i][:, common_genes]
+    print('Filtered all slices for common genes. There are ' + str(len(common_genes)) + ' common genes.')
+
+    # Run initial NMF
+    if dissimilarity.lower()=='euclidean' or dissimilarity.lower()=='euc':
+        model = NMF(n_components=n_components, init='random', random_state = random_seed, verbose = verbose)
+    else:
+        model = NMF(n_components=n_components, solver = 'mu', beta_loss = 'kullback-leibler', init='random', random_state = random_seed, verbose = verbose)
+    
+    if pis_init is None:
+        pis = [None for i in range(len(slices))]
+        W = model.fit_transform(A.X)
+    else:
+        pis = pis_init
+        W = model.fit_transform(A.shape[0]*sum([lmbda[i]*np.dot(pis[i], to_dense_array(slices[i].X)) for i in range(len(slices))]))
+    H = model.components_
+    center_coordinates = A.obsm['spatial']
+    
+    if not isinstance(center_coordinates, np.ndarray):
+        print("Warning: A.obsm['spatial'] is not of type numpy array.")
+    
+    # Initialize center_slice
+    center_slice = AnnData(np.dot(W,H))
+    center_slice.var.index = common_genes
+    center_slice.obs.index = A.obs.index
+    center_slice.obsm['spatial'] = center_coordinates
+    
+    # Minimize R
+    iteration_count = 0
+    R = 0
+    R_diff = 100
+    while R_diff > threshold and iteration_count < max_iter:
+        print("Iteration: " + str(iteration_count))
+        pis, r = center_ot(W, H, slices, center_coordinates, common_genes, alpha, backend, use_gpu, dissimilarity = dissimilarity, norm = norm, G_inits = pis, distributions=distributions, verbose = verbose)
+        W, H = center_NMF(W, H, slices, pis, lmbda, n_components, random_seed, dissimilarity = dissimilarity, verbose = verbose)
+        R_new = np.dot(r,lmbda)
+        iteration_count += 1
+        R_diff = abs(R - R_new)
+        print("Objective ",R_new)
+        print("Difference: " + str(R_diff) + "\n")
+        R = R_new
+    center_slice = A.copy()
+    center_slice.X = np.dot(W, H)
+    center_slice.uns['paste_W'] = W
+    center_slice.uns['paste_H'] = H
+    center_slice.uns['full_rank'] = center_slice.shape[0]*sum([lmbda[i]*np.dot(pis[i], to_dense_array(slices[i].X)) for i in range(len(slices))])
+    center_slice.uns['obj'] = R
+    return center_slice, pis
+
+#--------------------------- HELPER METHODS -----------------------------------
+
+def center_ot(W, H, slices, center_coordinates, common_genes, alpha, backend, use_gpu, dissimilarity = 'kl', norm = False, G_inits = None, distributions=None, verbose = False):
+    center_slice = AnnData(np.dot(W,H))
+    center_slice.var.index = common_genes
+    center_slice.obsm['spatial'] = center_coordinates
+
+    if distributions is None:
+        distributions = len(slices)*[None]
+
+    pis = []
+    r = []
+    print('Solving Pairwise Slice Alignment Problem.')
+    for i in range(len(slices)):
+        p, r_q = pairwise_align(center_slice, slices[i], alpha = alpha, dissimilarity = dissimilarity, norm = norm, return_obj = True, G_init = G_inits[i], b_distribution=distributions[i], backend = backend, use_gpu = use_gpu, verbose = verbose, gpu_verbose = False)
+        pis.append(p)
+        r.append(r_q)
+    return pis, np.array(r)
+
+def center_NMF(W, H, slices, pis, lmbda, n_components, random_seed, dissimilarity = 'kl', verbose = False):
+    print('Solving Center Mapping NMF Problem.')
+    n = W.shape[0]
+    B = n*sum([lmbda[i]*np.dot(pis[i], to_dense_array(slices[i].X)) for i in range(len(slices))])
+    if dissimilarity.lower()=='euclidean' or dissimilarity.lower()=='euc':
+        model = NMF(n_components=n_components, init='random', random_state = random_seed, verbose = verbose)
+    else:
+        model = NMF(n_components=n_components, solver = 'mu', beta_loss = 'kullback-leibler', init='random', random_state = random_seed, verbose = verbose)
+    W_new = model.fit_transform(B)
+    H_new = model.components_
+    return W_new, H_new
+
+def my_fused_gromov_wasserstein(M, C1, C2, p, q, G_init = None, loss_fun='square_loss', alpha=0.5, armijo=False, log=False,numItermax=200, tol_rel=1e-9, tol_abs=1e-9, use_gpu = False, **kwargs):
+    """
+    Adapted fused_gromov_wasserstein with the added capability of defining a G_init (inital mapping).
+    Also added capability of utilizing different POT backends to speed up computation.
+    
+    For more info, see: https://pythonot.github.io/gen_modules/ot.gromov.html
+    """
+
+    p, q = ot.utils.list_to_array(p, q)
+
+    p0, q0, C10, C20, M0 = p, q, C1, C2, M
+    nx = ot.backend.get_backend(p0, q0, C10, C20, M0)
+
+    constC, hC1, hC2 = ot.gromov.init_matrix(C1, C2, p, q, loss_fun)
+
+    if G_init is None:
+        G0 = p[:, None] * q[None, :]
+    else:
+        G0 = (1/nx.sum(G_init)) * G_init
+        if use_gpu:
+            G0 = G0.cuda()
+
+    def f(G):
+        return ot.gromov.gwloss(constC, hC1, hC2, G)
+
+    def df(G):
+        return ot.gromov.gwggrad(constC, hC1, hC2, G)
+    
+    if loss_fun == 'kl_loss':
+        armijo = True  # there is no closed form line-search with KL
+
+    if armijo:
+        def line_search(cost, G, deltaG, Mi, cost_G, **kwargs):
+            return ot.optim.line_search_armijo(cost, G, deltaG, Mi, cost_G, nx=nx, **kwargs)
+    else:
+        def line_search(cost, G, deltaG, Mi, cost_G, **kwargs):
+            return solve_gromov_linesearch(G, deltaG, cost_G, C1, C2, M=0., reg=1., nx=nx, **kwargs)
+
+    if log:
+        res, log = ot.optim.cg(p, q, (1 - alpha) * M, alpha, f, df, G0, line_search, log=True, numItermax=numItermax, stopThr=tol_rel, stopThr2=tol_abs, **kwargs)
+
+        fgw_dist = log['loss'][-1]
+
+        log['fgw_dist'] = fgw_dist
+        log['u'] = log['u']
+        log['v'] = log['v']
+        return res, log
+
+    else:
+        return ot.optim.cg(p, q, (1 - alpha) * M, alpha, f, df, G0, line_search, numItermax=numItermax, stopThr=tol_rel, stopThr2=tol_abs, **kwargs)
+
+def solve_gromov_linesearch(G, deltaG, cost_G, C1, C2, M, reg,
+                            alpha_min=None, alpha_max=None, nx=None, **kwargs):
+    """
+    Solve the linesearch in the FW iterations
+
+    Parameters
+    ----------
+
+    G : array-like, shape(ns,nt)
+        The transport map at a given iteration of the FW
+    deltaG : array-like (ns,nt)
+        Difference between the optimal map found by linearization in the FW algorithm and the value at a given iteration
+    cost_G : float
+        Value of the cost at `G`
+    C1 : array-like (ns,ns), optional
+        Structure matrix in the source domain.
+    C2 : array-like (nt,nt), optional
+        Structure matrix in the target domain.
+    M : array-like (ns,nt)
+        Cost matrix between the features.
+    reg : float
+        Regularization parameter.
+    alpha_min : float, optional
+        Minimum value for alpha
+    alpha_max : float, optional
+        Maximum value for alpha
+    nx : backend, optional
+        If let to its default value None, a backend test will be conducted.
+    Returns
+    -------
+    alpha : float
+        The optimal step size of the FW
+    fc : int
+        nb of function call. Useless here
+    cost_G : float
+        The value of the cost for the next iteration
+
+
+    .. _references-solve-linesearch:
+    References
+    ----------
+    .. [24] Vayer Titouan, Chapel Laetitia, Flamary Rémi, Tavenard Romain and Courty Nicolas
+        "Optimal Transport for structured data with application on graphs"
+        International Conference on Machine Learning (ICML). 2019.
+    """
+    if nx is None:
+        G, deltaG, C1, C2, M = ot.utils.list_to_array(G, deltaG, C1, C2, M)
+
+        if isinstance(M, int) or isinstance(M, float):
+            nx = ot.backend.get_backend(G, deltaG, C1, C2)
+        else:
+            nx = ot.backend.get_backend(G, deltaG, C1, C2, M)
+
+    dot = nx.dot(nx.dot(C1, deltaG), C2.T)
+    a = -2 * reg * nx.sum(dot * deltaG)
+    b = nx.sum(M * deltaG) - 2 * reg * (nx.sum(dot * G) + nx.sum(nx.dot(nx.dot(C1, G), C2.T) * deltaG))
+
+    alpha = ot.optim.solve_1d_linesearch_quad(a, b)
+    if alpha_min is not None or alpha_max is not None:
+        alpha = np.clip(alpha, alpha_min, alpha_max)
+
+    # the new cost is deduced from the line search quadratic function
+    cost_G = cost_G + a * (alpha ** 2) + b * alpha
+
+    return alpha, 1, cost_G
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `paste-bio-1.3.0/src/paste/helper.py` & `paste-bio-1.4.0/src/paste/helper.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,161 +1,161 @@
-from typing import List
-from anndata import AnnData
-import numpy as np
-import scipy
-import ot
-
-def filter_for_common_genes(
-    slices: List[AnnData]) -> None:
-    """
-    Filters for the intersection of genes between all slices.
-
-    Args:
-        slices: List of slices.
-    """
-    assert len(slices) > 0, "Cannot have empty list."
-
-    common_genes = slices[0].var.index
-    for s in slices:
-        common_genes = intersect(common_genes, s.var.index)
-    for i in range(len(slices)):
-        slices[i] = slices[i][:, common_genes]
-    print('Filtered all slices for common genes. There are ' + str(len(common_genes)) + ' common genes.')
-
-def match_spots_using_spatial_heuristic(
-    X,
-    Y,
-    use_ot: bool = True) -> np.ndarray:
-    """
-    Calculates and returns a mapping of spots using a spatial heuristic.
-
-    Args:
-        X (array-like, optional): Coordinates for spots X.
-        Y (array-like, optional): Coordinates for spots Y.
-        use_ot: If ``True``, use optimal transport ``ot.emd()`` to calculate mapping. Otherwise, use Scipy's ``min_weight_full_bipartite_matching()`` algorithm.
-
-    Returns:
-        Mapping of spots using a spatial heuristic.
-    """
-    n1,n2=len(X),len(Y)
-    X,Y = norm_and_center_coordinates(X),norm_and_center_coordinates(Y)
-    dist = scipy.spatial.distance_matrix(X,Y)
-    if use_ot:
-        pi = ot.emd(np.ones(n1)/n1, np.ones(n2)/n2, dist)
-    else:
-        row_ind, col_ind = scipy.sparse.csgraph.min_weight_full_bipartite_matching(scipy.sparse.csr_matrix(dist))
-        pi = np.zeros((n1,n2))
-        pi[row_ind, col_ind] = 1/max(n1,n2)
-        if n1<n2: pi[:, [(j not in col_ind) for j in range(n2)]] = 1/(n1*n2)
-        elif n2<n1: pi[[(i not in row_ind) for i in range(n1)], :] = 1/(n1*n2)
-    return pi
-
-def kl_divergence(X, Y):
-    """
-    Returns pairwise KL divergence (over all pairs of samples) of two matrices X and Y.
-
-    Args:
-        X: np array with dim (n_samples by n_features)
-        Y: np array with dim (m_samples by n_features)
-
-    Returns:
-        D: np array with dim (n_samples by m_samples). Pairwise KL divergence matrix.
-    """
-    assert X.shape[1] == Y.shape[1], "X and Y do not have the same number of features."
-
-    X = X/X.sum(axis=1, keepdims=True)
-    Y = Y/Y.sum(axis=1, keepdims=True)
-    log_X = np.log(X)
-    log_Y = np.log(Y)
-    X_log_X = np.matrix([np.dot(X[i],log_X[i].T) for i in range(X.shape[0])])
-    D = X_log_X.T - np.dot(X,log_Y.T)
-    return np.asarray(D)
-
-def kl_divergence_backend(X, Y):
-    """
-    Returns pairwise KL divergence (over all pairs of samples) of two matrices X and Y.
-
-    Takes advantage of POT backend to speed up computation.
-
-    Args:
-        X: np array with dim (n_samples by n_features)
-        Y: np array with dim (m_samples by n_features)
-
-    Returns:
-        D: np array with dim (n_samples by m_samples). Pairwise KL divergence matrix.
-    """
-    assert X.shape[1] == Y.shape[1], "X and Y do not have the same number of features."
-
-    nx = ot.backend.get_backend(X,Y)
-
-    X = X/nx.sum(X,axis=1, keepdims=True)
-    Y = Y/nx.sum(Y,axis=1, keepdims=True)
-    log_X = nx.log(X)
-    log_Y = nx.log(Y)
-    X_log_X = nx.einsum('ij,ij->i',X,log_X)
-    X_log_X = nx.reshape(X_log_X,(1,X_log_X.shape[0]))
-    D = X_log_X.T - nx.dot(X,log_Y.T)
-    return nx.to_numpy(D)
-
-
-def intersect(lst1, lst2):
-    """
-    Gets and returns intersection of two lists.
-
-    Args:
-        lst1: List
-        lst2: List
-
-    Returns:
-        lst3: List of common elements.
-    """
-
-    temp = set(lst2)
-    lst3 = [value for value in lst1 if value in temp]
-    return lst3
-
-def norm_and_center_coordinates(X):
-    """
-    Normalizes and centers coordinates at the origin.
-
-    Args:
-        X: Numpy array
-
-    Returns:
-        X_new: Updated coordiantes.
-    """
-    return (X-X.mean(axis=0))/min(scipy.spatial.distance.pdist(X))
-
-def apply_trsf(
-    M: np.ndarray,
-    translation: List[float],
-    points: np.ndarray) -> np.ndarray:
-    """
-    Apply a rotation from a 2x2 rotation matrix `M` together with
-    a translation from a translation vector of length 2 `translation` to a list of
-    `points`.
-
-    Args:
-        M (nd.array): a 2x2 rotation matrix.
-        translation (nd.array): a translation vector of length 2.
-        points (nd.array): a nx2 array of `n` points 2D positions.
-
-    Returns:
-        (nd.array) a nx2 matrix of the `n` points transformed.
-    """
-    if not isinstance(translation, np.ndarray):
-        translation = np.array(translation)
-    trsf = np.identity(3)
-    trsf[:-1, :-1] = M
-    tr = np.identity(3)
-    tr[:-1, -1] = -translation
-    trsf = trsf @ tr
-
-    flo = points.T
-    flo_pad = np.pad(flo, ((0, 1), (0, 0)), constant_values=1)
-    return ((trsf @ flo_pad)[:-1]).T
-
-## Covert a sparse matrix into a dense np array
-to_dense_array = lambda X: X.toarray() if isinstance(X,scipy.sparse.csr.spmatrix) else np.array(X)
-
-## Returns the data matrix or representation
+from typing import List
+from anndata import AnnData
+import numpy as np
+import scipy
+import ot
+
+def filter_for_common_genes(
+    slices: List[AnnData]) -> None:
+    """
+    Filters for the intersection of genes between all slices.
+
+    Args:
+        slices: List of slices.
+    """
+    assert len(slices) > 0, "Cannot have empty list."
+
+    common_genes = slices[0].var.index
+    for s in slices:
+        common_genes = intersect(common_genes, s.var.index)
+    for i in range(len(slices)):
+        slices[i] = slices[i][:, common_genes]
+    print('Filtered all slices for common genes. There are ' + str(len(common_genes)) + ' common genes.')
+
+def match_spots_using_spatial_heuristic(
+    X,
+    Y,
+    use_ot: bool = True) -> np.ndarray:
+    """
+    Calculates and returns a mapping of spots using a spatial heuristic.
+
+    Args:
+        X (array-like, optional): Coordinates for spots X.
+        Y (array-like, optional): Coordinates for spots Y.
+        use_ot: If ``True``, use optimal transport ``ot.emd()`` to calculate mapping. Otherwise, use Scipy's ``min_weight_full_bipartite_matching()`` algorithm.
+
+    Returns:
+        Mapping of spots using a spatial heuristic.
+    """
+    n1,n2=len(X),len(Y)
+    X,Y = norm_and_center_coordinates(X),norm_and_center_coordinates(Y)
+    dist = scipy.spatial.distance_matrix(X,Y)
+    if use_ot:
+        pi = ot.emd(np.ones(n1)/n1, np.ones(n2)/n2, dist)
+    else:
+        row_ind, col_ind = scipy.sparse.csgraph.min_weight_full_bipartite_matching(scipy.sparse.csr_matrix(dist))
+        pi = np.zeros((n1,n2))
+        pi[row_ind, col_ind] = 1/max(n1,n2)
+        if n1<n2: pi[:, [(j not in col_ind) for j in range(n2)]] = 1/(n1*n2)
+        elif n2<n1: pi[[(i not in row_ind) for i in range(n1)], :] = 1/(n1*n2)
+    return pi
+
+def kl_divergence(X, Y):
+    """
+    Returns pairwise KL divergence (over all pairs of samples) of two matrices X and Y.
+
+    Args:
+        X: np array with dim (n_samples by n_features)
+        Y: np array with dim (m_samples by n_features)
+
+    Returns:
+        D: np array with dim (n_samples by m_samples). Pairwise KL divergence matrix.
+    """
+    assert X.shape[1] == Y.shape[1], "X and Y do not have the same number of features."
+
+    X = X/X.sum(axis=1, keepdims=True)
+    Y = Y/Y.sum(axis=1, keepdims=True)
+    log_X = np.log(X)
+    log_Y = np.log(Y)
+    X_log_X = np.matrix([np.dot(X[i],log_X[i].T) for i in range(X.shape[0])])
+    D = X_log_X.T - np.dot(X,log_Y.T)
+    return np.asarray(D)
+
+def kl_divergence_backend(X, Y):
+    """
+    Returns pairwise KL divergence (over all pairs of samples) of two matrices X and Y.
+
+    Takes advantage of POT backend to speed up computation.
+
+    Args:
+        X: np array with dim (n_samples by n_features)
+        Y: np array with dim (m_samples by n_features)
+
+    Returns:
+        D: np array with dim (n_samples by m_samples). Pairwise KL divergence matrix.
+    """
+    assert X.shape[1] == Y.shape[1], "X and Y do not have the same number of features."
+
+    nx = ot.backend.get_backend(X,Y)
+
+    X = X/nx.sum(X,axis=1, keepdims=True)
+    Y = Y/nx.sum(Y,axis=1, keepdims=True)
+    log_X = nx.log(X)
+    log_Y = nx.log(Y)
+    X_log_X = nx.einsum('ij,ij->i',X,log_X)
+    X_log_X = nx.reshape(X_log_X,(1,X_log_X.shape[0]))
+    D = X_log_X.T - nx.dot(X,log_Y.T)
+    return nx.to_numpy(D)
+
+
+def intersect(lst1, lst2):
+    """
+    Gets and returns intersection of two lists.
+
+    Args:
+        lst1: List
+        lst2: List
+
+    Returns:
+        lst3: List of common elements.
+    """
+
+    temp = set(lst2)
+    lst3 = [value for value in lst1 if value in temp]
+    return lst3
+
+def norm_and_center_coordinates(X):
+    """
+    Normalizes and centers coordinates at the origin.
+
+    Args:
+        X: Numpy array
+
+    Returns:
+        X_new: Updated coordiantes.
+    """
+    return (X-X.mean(axis=0))/min(scipy.spatial.distance.pdist(X))
+
+def apply_trsf(
+    M: np.ndarray,
+    translation: List[float],
+    points: np.ndarray) -> np.ndarray:
+    """
+    Apply a rotation from a 2x2 rotation matrix `M` together with
+    a translation from a translation vector of length 2 `translation` to a list of
+    `points`.
+
+    Args:
+        M (nd.array): A 2x2 rotation matrix.
+        translation (nd.array): A translation vector of length 2.
+        points (nd.array): A nx2 array of `n` points 2D positions.
+
+    Returns:
+        (nd.array) A nx2 matrix of the `n` points transformed.
+    """
+    if not isinstance(translation, np.ndarray):
+        translation = np.array(translation)
+    trsf = np.identity(3)
+    trsf[:-1, :-1] = M
+    tr = np.identity(3)
+    tr[:-1, -1] = -translation
+    trsf = trsf @ tr
+
+    flo = points.T
+    flo_pad = np.pad(flo, ((0, 1), (0, 0)), constant_values=1)
+    return ((trsf @ flo_pad)[:-1]).T
+
+## Covert a sparse matrix into a dense np array
+to_dense_array = lambda X: X.toarray() if isinstance(X,scipy.sparse.csr.spmatrix) else np.array(X)
+
+## Returns the data matrix or representation
 extract_data_matrix = lambda adata,rep: adata.X if rep is None else adata.obsm[rep]
```

### Comparing `paste-bio-1.3.0/src/paste_bio.egg-info/PKG-INFO` & `paste-bio-1.4.0/src/paste_bio.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,183 +1,183 @@
-Metadata-Version: 2.1
-Name: paste-bio
-Version: 1.3.0
-Summary: A computational method to align and integrate spatial transcriptomics experiments.
-Home-page: https://github.com/raphael-group/paste
-Author: Max Land
-Author-email: max.ruikang.land@gmail.com
-Project-URL: Bug Tracker, https://github.com/raphael-group/paste/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![PyPI](https://img.shields.io/pypi/v/paste-bio.svg)](https://pypi.org/project/paste-bio)
-[![Downloads](https://pepy.tech/badge/paste-bio)](https://pepy.tech/project/paste-bio)
-[![Documentation Status](https://readthedocs.org/projects/paste-bio/badge/?version=latest)](https://paste-bio.readthedocs.io/en/stable/?badge=stable)
-
-# PASTE
-
-![PASTE Overview](https://github.com/raphael-group/paste/blob/main/docs/source/_static/images/paste_overview.png)
-
-PASTE is a computational method that leverages both gene expression similarity and spatial distances between spots to align and integrate spatial transcriptomics data. In particular, there are two methods:
-1. `pairwise_align`: align spots across pairwise slices.
-2. `center_align`: integrate multiple slices into one center slice.
-
-You can read full paper [here](https://www.nature.com/articles/s41592-022-01459-6). 
-
-Additional examples and the code to reproduce the paper's analyses can be found [here](https://github.com/raphael-group/paste_reproducibility). Preprocessed datasets used in the paper can be found on [zenodo](https://doi.org/10.5281/zenodo.6334774).
-
-PASTE is actively being worked on with future updates coming. 
-
-### Recent News
-
-* PASTE is now published in [Nature Methods](https://www.nature.com/articles/s41592-022-01459-6)!
-
-* The code to reproduce the analisys can be found [here](https://github.com/raphael-group/paste_reproducibility).
-
-* As of version 1.2.0, PASTE now supports GPU implementation via Pytorch. For more details, see the GPU section of the [Tutorial notebook](docs/source/notebooks/getting-started.ipynb).
-
-### Installation
-
-The easiest way is to install PASTE on pypi: https://pypi.org/project/paste-bio/. 
-
-`pip install paste-bio` 
-
-Or you can install PASTE on bioconda: https://anaconda.org/bioconda/paste-bio.
-
-`conda install -c bioconda paste-bio`
-
-Check out Tutorial.ipynb for an example of how to use PASTE.
-
-Alternatively, you can clone the respository and try the following example in a
-notebook or the command line. 
-
-### Quick Start
-
-To use PASTE we require at least two slices of spatial-omics data (both
-expression and coordinates) that are in
-anndata format (i.e. read in by scanpy/squidpy). We have included a breast
-cancer dataset from [1] in the [sample_data folder](sample_data/) of this repo 
-that we will use as an example below to show how to use PASTE.
-
-```python
-import matplotlib.pyplot as plt
-import matplotlib.patches as mpatches
-import numpy as np
-import scanpy as sc
-import paste as pst
-
-# Load Slices
-data_dir = './sample_data/' # change this path to the data you wish to analyze
-
-# Assume that the coordinates of slices are named slice_name + "_coor.csv"
-def load_slices(data_dir, slice_names=["slice1", "slice2"]):
-    slices = []  
-    for slice_name in slice_names:
-        slice_i = sc.read_csv(data_dir + slice_name + ".csv")
-        slice_i_coor = np.genfromtxt(data_dir + slice_name + "_coor.csv", delimiter = ',')
-        slice_i.obsm['spatial'] = slice_i_coor
-        # Preprocess slices
-        sc.pp.filter_genes(slice_i, min_counts = 15)
-        sc.pp.filter_cells(slice_i, min_counts = 100)
-        slices.append(slice_i)
-    return slices
-
-slices = load_slices(data_dir)
-slice1, slice2 = slices
-
-# Pairwise align the slices
-pi12 = pst.pairwise_align(slice1, slice2)
-
-# To visualize the alignment you can stack the slices 
-# according to the alignment pi
-slices, pis = [slice1, slice2], [pi12]
-new_slices = pst.stack_slices_pairwise(slices, pis)
-
-slice_colors = ['#e41a1c','#377eb8']
-plt.figure(figsize=(7,7))
-for i in range(len(new_slices)):
-    pst.plot_slice(new_slices[i],slice_colors[i],s=400)
-plt.legend(handles=[mpatches.Patch(color=slice_colors[0], label='1'),mpatches.Patch(color=slice_colors[1], label='2')])
-plt.gca().invert_yaxis()
-plt.axis('off')
-plt.show()
-
-# Center align slices
-## We have to reload the slices as pairwise_alignment modifies the slices.
-slices = load_slices(data_dir)
-slice1, slice2 = slices
-
-# Construct a center slice
-## choose one of the slices as the coordinate reference for the center slice,
-## i.e. the center slice will have the same number of spots as this slice and
-## the same coordinates.
-initial_slice = slice1.copy()    
-slices = [slice1, slice2]
-lmbda = len(slices)*[1/len(slices)] # set hyperparameter to be uniform
-
-## Possible to pass in an initial pi (as keyword argument pis_init) 
-## to improve performance, see Tutorial.ipynb notebook for more details.
-center_slice, pis = pst.center_align(initial_slice, slices, lmbda) 
-
-## The low dimensional representation of our center slice is held 
-## in the matrices W and H, which can be used for downstream analyses
-W = center_slice.uns['paste_W']
-H = center_slice.uns['paste_H']
-```
-
-### GPU implementation
-PASTE now is compatible with gpu via Pytorch. All we need to do is add the following two parameters to our main functions:
-```
-pi12 = pst.pairwise_align(slice1, slice2, backend = ot.backend.TorchBackend(), use_gpu = True)
-
-center_slice, pis = pst.center_align(initial_slice, slices, lmbda, backend = ot.backend.TorchBackend(), use_gpu = True) 
-```
-For more details, see the GPU section of the [Tutorial notebook](docs/source/notebooks/getting-started.ipynb).
-
-### Command Line
-
-We provide the option of running PASTE from the command line. 
-
-First, clone the repository:
-
-`git clone https://github.com/raphael-group/paste.git`
-
-Next, when providing files, you will need to provide two separate files: the gene expression data followed by spatial data (both as .csv) for the code to initialize one slice object.
-
-Sample execution (based on this repo): `python paste-cmd-line.py -m center -f ./sample_data/slice1.csv ./sample_data/slice1_coor.csv ./sample_data/slice2.csv ./sample_data/slice2_coor.csv ./sample_data/slice3.csv ./sample_data/slice3_coor.csv`
-
-Note: `pairwise` will return pairwise alignment between each consecutive pair of slices (e.g. \[slice1,slice2\], \[slice2,slice3\]).
-
-| Flag | Name | Description | Default Value |
-| --- | --- | --- | --- |
-| -m | mode | Select either `pairwise` or `center` | (str) `pairwise` |
-| -f | files | Path to data files (.csv) | None |
-| -d | direc | Directory to store output files | Current Directory |
-| -a | alpha | Alpha parameter for PASTE | (float) `0.1` |
-| -c | cost | Expression dissimilarity cost (`kl` or `Euclidean`) | (str) `kl` |
-| -p | n_components | n_components for NMF step in `center_align` | (int) `15` |
-| -l | lmbda | Lambda parameter in `center_align` | (floats) probability vector of length `n`  |
-| -i | intial_slice | Specify which file is also the intial slice in `center_align` | (int) `1` |
-| -t | threshold | Convergence threshold for `center_align` | (float) `0.001` |
-| -x | coordinates | Output new coordinates (toggle to turn on) | `False` |
-| -w | weights | Weights files of spots in each slice (.csv) | None |
-| -s | start | Initial alignments for OT. If not given uses uniform (.csv structure similar to alignment output) | None |
-
-`pairwise_align` outputs a (.csv) file containing mapping of spots between each consecutive pair of slices. The rows correspond to spots of the first slice, and cols the second.
-
-`center_align` outputs two files containing the low dimensional representation (NMF decomposition) of the center slice gene expression, and files containing a mapping of spots between the center slice (rows) to each input slice (cols).
-
-### Sample Dataset
-
-Added sample spatial transcriptomics dataset consisting of four breast cancer slice courtesy of:
-
-[1] Ståhl, Patrik & Salmén, Fredrik & Vickovic, Sanja & Lundmark, Anna & Fernandez Navarro, Jose & Magnusson, Jens & Giacomello, Stefania & Asp, Michaela & Westholm, Jakub & Huss, Mikael & Mollbrink, Annelie & Linnarsson, Sten & Codeluppi, Simone & Borg, Åke & Pontén, Fredrik & Costea, Paul & Sahlén, Pelin Akan & Mulder, Jan & Bergmann, Olaf & Frisén, Jonas. (2016). Visualization and analysis of gene expression in tissue sections by spatial transcriptomics. Science. 353. 78-82. 10.1126/science.aaf2403. 
-
-Note: Original data is (.tsv), but we converted it to (.csv).
-
-### References
-
-Ron Zeira, Max Land, Alexander Strzalkowski and Benjamin J. Raphael. "Alignment and integration of spatial transcriptomics data". Nature Methods (2022). https://doi.org/10.1038/s41592-022-01459-6
+Metadata-Version: 2.1
+Name: paste-bio
+Version: 1.4.0
+Summary: A computational method to align and integrate spatial transcriptomics experiments.
+Home-page: https://github.com/raphael-group/paste
+Author: Max Land
+Author-email: max.ruikang.land@gmail.com
+Project-URL: Bug Tracker, https://github.com/raphael-group/paste/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![PyPI](https://img.shields.io/pypi/v/paste-bio.svg)](https://pypi.org/project/paste-bio)
+[![Downloads](https://pepy.tech/badge/paste-bio)](https://pepy.tech/project/paste-bio)
+[![Documentation Status](https://readthedocs.org/projects/paste-bio/badge/?version=latest)](https://paste-bio.readthedocs.io/en/stable/?badge=stable)
+[![Anaconda](https://anaconda.org/bioconda/paste-bio/badges/version.svg)](https://anaconda.org/bioconda/paste-bio/badges/version.svg)
+[![bioconda-downloads](https://anaconda.org/bioconda/paste-bio/badges/downloads.svg)](https://anaconda.org/bioconda/paste-bio/badges/downloads.svg)
+
+# PASTE
+
+![PASTE Overview](https://github.com/raphael-group/paste/blob/main/docs/source/_static/images/paste_overview.png)
+
+PASTE is a computational method that leverages both gene expression similarity and spatial distances between spots to align and integrate spatial transcriptomics data. In particular, there are two methods:
+1. `pairwise_align`: align spots across pairwise slices.
+2. `center_align`: integrate multiple slices into one center slice.
+
+You can read full paper [here](https://www.nature.com/articles/s41592-022-01459-6). 
+
+Additional examples and the code to reproduce the paper's analyses can be found [here](https://github.com/raphael-group/paste_reproducibility). Preprocessed datasets used in the paper can be found on [zenodo](https://doi.org/10.5281/zenodo.6334774).
+
+### Recent News
+
+* PASTE is now published in [Nature Methods](https://www.nature.com/articles/s41592-022-01459-6)!
+
+* The code to reproduce the analisys can be found [here](https://github.com/raphael-group/paste_reproducibility).
+
+* As of version 1.2.0, PASTE now supports GPU implementation via Pytorch. For more details, see the GPU section of the [Tutorial notebook](docs/source/notebooks/getting-started.ipynb).
+
+### Installation
+
+The easiest way is to install PASTE on pypi: https://pypi.org/project/paste-bio/. 
+
+`pip install paste-bio` 
+
+Or you can install PASTE on bioconda: https://anaconda.org/bioconda/paste-bio.
+
+`conda install -c bioconda paste-bio`
+
+Check out Tutorial.ipynb for an example of how to use PASTE.
+
+Alternatively, you can clone the respository and try the following example in a
+notebook or the command line. 
+
+### Quick Start
+
+To use PASTE we require at least two slices of spatial-omics data (both
+expression and coordinates) that are in
+anndata format (i.e. read in by scanpy/squidpy). We have included a breast
+cancer dataset from [1] in the [sample_data folder](sample_data/) of this repo 
+that we will use as an example below to show how to use PASTE.
+
+```python
+import matplotlib.pyplot as plt
+import matplotlib.patches as mpatches
+import numpy as np
+import scanpy as sc
+import paste as pst
+
+# Load Slices
+data_dir = './sample_data/' # change this path to the data you wish to analyze
+
+# Assume that the coordinates of slices are named slice_name + "_coor.csv"
+def load_slices(data_dir, slice_names=["slice1", "slice2"]):
+    slices = []  
+    for slice_name in slice_names:
+        slice_i = sc.read_csv(data_dir + slice_name + ".csv")
+        slice_i_coor = np.genfromtxt(data_dir + slice_name + "_coor.csv", delimiter = ',')
+        slice_i.obsm['spatial'] = slice_i_coor
+        # Preprocess slices
+        sc.pp.filter_genes(slice_i, min_counts = 15)
+        sc.pp.filter_cells(slice_i, min_counts = 100)
+        slices.append(slice_i)
+    return slices
+
+slices = load_slices(data_dir)
+slice1, slice2 = slices
+
+# Pairwise align the slices
+pi12 = pst.pairwise_align(slice1, slice2)
+
+# To visualize the alignment you can stack the slices 
+# according to the alignment pi
+slices, pis = [slice1, slice2], [pi12]
+new_slices = pst.stack_slices_pairwise(slices, pis)
+
+slice_colors = ['#e41a1c','#377eb8']
+plt.figure(figsize=(7,7))
+for i in range(len(new_slices)):
+    pst.plot_slice(new_slices[i],slice_colors[i],s=400)
+plt.legend(handles=[mpatches.Patch(color=slice_colors[0], label='1'),mpatches.Patch(color=slice_colors[1], label='2')])
+plt.gca().invert_yaxis()
+plt.axis('off')
+plt.show()
+
+# Center align slices
+## We have to reload the slices as pairwise_alignment modifies the slices.
+slices = load_slices(data_dir)
+slice1, slice2 = slices
+
+# Construct a center slice
+## choose one of the slices as the coordinate reference for the center slice,
+## i.e. the center slice will have the same number of spots as this slice and
+## the same coordinates.
+initial_slice = slice1.copy()    
+slices = [slice1, slice2]
+lmbda = len(slices)*[1/len(slices)] # set hyperparameter to be uniform
+
+## Possible to pass in an initial pi (as keyword argument pis_init) 
+## to improve performance, see Tutorial.ipynb notebook for more details.
+center_slice, pis = pst.center_align(initial_slice, slices, lmbda) 
+
+## The low dimensional representation of our center slice is held 
+## in the matrices W and H, which can be used for downstream analyses
+W = center_slice.uns['paste_W']
+H = center_slice.uns['paste_H']
+```
+
+### GPU implementation
+PASTE now is compatible with gpu via Pytorch. All we need to do is add the following two parameters to our main functions:
+```
+pi12 = pst.pairwise_align(slice1, slice2, backend = ot.backend.TorchBackend(), use_gpu = True)
+
+center_slice, pis = pst.center_align(initial_slice, slices, lmbda, backend = ot.backend.TorchBackend(), use_gpu = True) 
+```
+For more details, see the GPU section of the [Tutorial notebook](docs/source/notebooks/getting-started.ipynb).
+
+### Command Line
+
+We provide the option of running PASTE from the command line. 
+
+First, clone the repository:
+
+`git clone https://github.com/raphael-group/paste.git`
+
+Next, when providing files, you will need to provide two separate files: the gene expression data followed by spatial data (both as .csv) for the code to initialize one slice object.
+
+Sample execution (based on this repo): `python paste-cmd-line.py -m center -f ./sample_data/slice1.csv ./sample_data/slice1_coor.csv ./sample_data/slice2.csv ./sample_data/slice2_coor.csv ./sample_data/slice3.csv ./sample_data/slice3_coor.csv`
+
+Note: `pairwise` will return pairwise alignment between each consecutive pair of slices (e.g. \[slice1,slice2\], \[slice2,slice3\]).
+
+| Flag | Name | Description | Default Value |
+| --- | --- | --- | --- |
+| -m | mode | Select either `pairwise` or `center` | (str) `pairwise` |
+| -f | files | Path to data files (.csv) | None |
+| -d | direc | Directory to store output files | Current Directory |
+| -a | alpha | Alpha parameter for PASTE | (float) `0.1` |
+| -c | cost | Expression dissimilarity cost (`kl` or `Euclidean`) | (str) `kl` |
+| -p | n_components | n_components for NMF step in `center_align` | (int) `15` |
+| -l | lmbda | Lambda parameter in `center_align` | (floats) probability vector of length `n`  |
+| -i | intial_slice | Specify which file is also the intial slice in `center_align` | (int) `1` |
+| -t | threshold | Convergence threshold for `center_align` | (float) `0.001` |
+| -x | coordinates | Output new coordinates (toggle to turn on) | `False` |
+| -w | weights | Weights files of spots in each slice (.csv) | None |
+| -s | start | Initial alignments for OT. If not given uses uniform (.csv structure similar to alignment output) | None |
+
+`pairwise_align` outputs a (.csv) file containing mapping of spots between each consecutive pair of slices. The rows correspond to spots of the first slice, and cols the second.
+
+`center_align` outputs two files containing the low dimensional representation (NMF decomposition) of the center slice gene expression, and files containing a mapping of spots between the center slice (rows) to each input slice (cols).
+
+### Sample Dataset
+
+Added sample spatial transcriptomics dataset consisting of four breast cancer slice courtesy of:
+
+[1] Ståhl, Patrik & Salmén, Fredrik & Vickovic, Sanja & Lundmark, Anna & Fernandez Navarro, Jose & Magnusson, Jens & Giacomello, Stefania & Asp, Michaela & Westholm, Jakub & Huss, Mikael & Mollbrink, Annelie & Linnarsson, Sten & Codeluppi, Simone & Borg, Åke & Pontén, Fredrik & Costea, Paul & Sahlén, Pelin Akan & Mulder, Jan & Bergmann, Olaf & Frisén, Jonas. (2016). Visualization and analysis of gene expression in tissue sections by spatial transcriptomics. Science. 353. 78-82. 10.1126/science.aaf2403. 
+
+Note: Original data is (.tsv), but we converted it to (.csv).
+
+### References
+
+Ron Zeira, Max Land, Alexander Strzalkowski and Benjamin J. Raphael. "Alignment and integration of spatial transcriptomics data". Nature Methods (2022). https://doi.org/10.1038/s41592-022-01459-6
```

