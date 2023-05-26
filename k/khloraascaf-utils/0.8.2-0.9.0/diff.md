# Comparing `tmp/khloraascaf_utils-0.8.2.tar.gz` & `tmp/khloraascaf_utils-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "khloraascaf_utils-0.8.2.tar", last modified: Sun May 21 21:20:44 2023, max compression
+gzip compressed data, was "khloraascaf_utils-0.9.0.tar", last modified: Fri May 26 00:36:31 2023, max compression
```

## Comparing `khloraascaf_utils-0.8.2.tar` & `khloraascaf_utils-0.9.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:20:44.974427 khloraascaf_utils-0.8.2/
--rw-rw-rw-   0 root         (0) root         (0)    34916 2023-05-21 21:20:23.000000 khloraascaf_utils-0.8.2/LICENCE
--rw-r--r--   0 root         (0) root         (0)    43838 2023-05-21 21:20:44.974427 khloraascaf_utils-0.8.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2535 2023-05-21 21:20:23.000000 khloraascaf_utils-0.8.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1245 2023-05-21 21:20:23.000000 khloraascaf_utils-0.8.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-21 21:20:44.974427 khloraascaf_utils-0.8.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:20:44.970427 khloraascaf_utils-0.8.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:20:44.972427 khloraascaf_utils-0.8.2/src/khloraascaf_utils/
--rw-rw-rw-   0 root         (0) root         (0)       71 2023-05-21 21:20:23.000000 khloraascaf_utils-0.8.2/src/khloraascaf_utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9489 2023-05-21 21:20:23.000000 khloraascaf_utils-0.8.2/src/khloraascaf_utils/artificial_data.py
--rw-rw-rw-   0 root         (0) root         (0)     7243 2023-05-21 21:20:23.000000 khloraascaf_utils-0.8.2/src/khloraascaf_utils/asm_graph_to_fasta.py
--rw-rw-rw-   0 root         (0) root         (0)     2817 2023-05-21 21:20:23.000000 khloraascaf_utils-0.8.2/src/khloraascaf_utils/contigs_attributes.py
--rw-rw-rw-   0 root         (0) root         (0)    13859 2023-05-21 21:20:23.000000 khloraascaf_utils-0.8.2/src/khloraascaf_utils/to_networkx.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:20:44.973427 khloraascaf_utils-0.8.2/src/khloraascaf_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)    43838 2023-05-21 21:20:44.000000 khloraascaf_utils-0.8.2/src/khloraascaf_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      552 2023-05-21 21:20:44.000000 khloraascaf_utils-0.8.2/src/khloraascaf_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-21 21:20:44.000000 khloraascaf_utils-0.8.2/src/khloraascaf_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-21 21:20:44.000000 khloraascaf_utils-0.8.2/src/khloraascaf_utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-21 21:20:44.000000 khloraascaf_utils-0.8.2/src/khloraascaf_utils.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:20:44.973427 khloraascaf_utils-0.8.2/tests/
--rw-rw-rw-   0 root         (0) root         (0)     4112 2023-05-21 21:20:23.000000 khloraascaf_utils-0.8.2/tests/test_artificial_data.py
--rw-rw-rw-   0 root         (0) root         (0)     3590 2023-05-21 21:20:23.000000 khloraascaf_utils-0.8.2/tests/test_asm_graph_to_fasta.py
--rw-rw-rw-   0 root         (0) root         (0)     1806 2023-05-21 21:20:23.000000 khloraascaf_utils-0.8.2/tests/test_contigs_attributes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 00:36:31.213596 khloraascaf_utils-0.9.0/
+-rw-rw-rw-   0 root         (0) root         (0)    34916 2023-05-26 00:36:09.000000 khloraascaf_utils-0.9.0/LICENCE
+-rw-r--r--   0 root         (0) root         (0)    43838 2023-05-26 00:36:31.213596 khloraascaf_utils-0.9.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2535 2023-05-26 00:36:09.000000 khloraascaf_utils-0.9.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1247 2023-05-26 00:36:09.000000 khloraascaf_utils-0.9.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-26 00:36:31.213596 khloraascaf_utils-0.9.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 00:36:31.209596 khloraascaf_utils-0.9.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 00:36:31.211596 khloraascaf_utils-0.9.0/src/khloraascaf_utils/
+-rw-rw-rw-   0 root         (0) root         (0)       71 2023-05-26 00:36:09.000000 khloraascaf_utils-0.9.0/src/khloraascaf_utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9489 2023-05-26 00:36:09.000000 khloraascaf_utils-0.9.0/src/khloraascaf_utils/artificial_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     7243 2023-05-26 00:36:09.000000 khloraascaf_utils-0.9.0/src/khloraascaf_utils/asm_graph_to_fasta.py
+-rw-rw-rw-   0 root         (0) root         (0)     2797 2023-05-26 00:36:09.000000 khloraascaf_utils-0.9.0/src/khloraascaf_utils/contigs_attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)    14820 2023-05-26 00:36:09.000000 khloraascaf_utils-0.9.0/src/khloraascaf_utils/to_networkx.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 00:36:31.212596 khloraascaf_utils-0.9.0/src/khloraascaf_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    43838 2023-05-26 00:36:31.000000 khloraascaf_utils-0.9.0/src/khloraascaf_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      552 2023-05-26 00:36:31.000000 khloraascaf_utils-0.9.0/src/khloraascaf_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 00:36:31.000000 khloraascaf_utils-0.9.0/src/khloraascaf_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2023-05-26 00:36:31.000000 khloraascaf_utils-0.9.0/src/khloraascaf_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-26 00:36:31.000000 khloraascaf_utils-0.9.0/src/khloraascaf_utils.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 00:36:31.213596 khloraascaf_utils-0.9.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     4112 2023-05-26 00:36:09.000000 khloraascaf_utils-0.9.0/tests/test_artificial_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3590 2023-05-26 00:36:09.000000 khloraascaf_utils-0.9.0/tests/test_asm_graph_to_fasta.py
+-rw-rw-rw-   0 root         (0) root         (0)     1806 2023-05-26 00:36:09.000000 khloraascaf_utils-0.9.0/tests/test_contigs_attributes.py
```

### Comparing `khloraascaf_utils-0.8.2/LICENCE` & `khloraascaf_utils-0.9.0/LICENCE`

 * *Files identical despite different names*

### Comparing `khloraascaf_utils-0.8.2/PKG-INFO` & `khloraascaf_utils-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khloraascaf_utils
-Version: 0.8.2
+Version: 0.9.0
 Summary: Python utilities for khloraascaf python package.
 Author-email: vepain <victor.epain@laposte.net>
 License: ### GNU GENERAL PUBLIC LICENSE
         
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc.
@@ -677,16 +677,16 @@
         library, you may consider it more useful to permit linking proprietary
         applications with the library. If this is what you want to do, use the
         GNU Lesser General Public License instead of this License. But first,
         please read <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Project-URL: Homepage, https://gitlab.com/khloraa_scaffolding/khloraascaf_utils
 Project-URL: Repository, https://gitlab.com/khloraa_scaffolding/khloraascaf_utils
-Project-URL: Documentation, https://khloraascaf_utils.readthedocs.io
-Project-URL: Changelog, https://khloraascaf_utils.readthedocs.io/en/latest/changelog.html
+Project-URL: Documentation, https://khloraascaf-utils.readthedocs.io
+Project-URL: Changelog, https://khloraascaf-utils.readthedocs.io/en/latest/changelog.html
 Keywords: Scaffolding,Chloroplast,Assembly,DNA repeats
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -705,15 +705,15 @@
 [![Documentation Status](https://readthedocs.org/projects/khloraascaf-utils/badge/?version=latest)](https://khloraascaf-utils.readthedocs.io/en/latest/?badge=latest)
 
  <img src="docs/img/logo_transp.png" alt="revsymg logo"
 width="200" height="200">
 
 `khloraascaf_utils` is a Python utilities package for [khloraascaf](https://pypi.org/project/khloraascaf/) Python package.
 
-Please have a look to the [documentation website](https://khloraascaf_utils.readthedocs.io) for more details.
+Please have a look to the [documentation website](https://khloraascaf-utils.readthedocs.io) for more details.
 
 ## Quick installation
 
 To install the `khloraascaf_utils` package from the [PyPI repository](https://pypi.org/project/khloraascaf_utils/), run the `pip` command :
 ```sh
 pip install khloraascaf_utils
 ```
```

### Comparing `khloraascaf_utils-0.8.2/README.md` & `khloraascaf_utils-0.9.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 [![Documentation Status](https://readthedocs.org/projects/khloraascaf-utils/badge/?version=latest)](https://khloraascaf-utils.readthedocs.io/en/latest/?badge=latest)
 
  <img src="docs/img/logo_transp.png" alt="revsymg logo"
 width="200" height="200">
 
 `khloraascaf_utils` is a Python utilities package for [khloraascaf](https://pypi.org/project/khloraascaf/) Python package.
 
-Please have a look to the [documentation website](https://khloraascaf_utils.readthedocs.io) for more details.
+Please have a look to the [documentation website](https://khloraascaf-utils.readthedocs.io) for more details.
 
 ## Quick installation
 
 To install the `khloraascaf_utils` package from the [PyPI repository](https://pypi.org/project/khloraascaf_utils/), run the `pip` command :
 ```sh
 pip install khloraascaf_utils
 ```
```

### Comparing `khloraascaf_utils-0.8.2/pyproject.toml` & `khloraascaf_utils-0.9.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 
 name = "khloraascaf_utils"
-version = "0.8.2"
+version = "0.9.0"
 authors = [{ name = "vepain", email = "victor.epain@laposte.net" }]
 description = "Python utilities for khloraascaf python package."
 keywords = ["Scaffolding", "Chloroplast", "Assembly", "DNA repeats"]
 readme = "README.md"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
@@ -17,22 +17,22 @@
     "Operating System :: Unix",
     "Programming Language :: Python :: 3.9",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 license = { file = "LICENCE" }
 requires-python = ">=3.9"
 dependencies = [
-    "khloraascaf >=1.8.0, <1.9",
+    "khloraascaf >=1.10.0, <1.11",
     "networkx >=3.0, <3.1",
     "biopython >=1.81, <1.82",
 ]
 
 [project.urls]
 
 Homepage = "https://gitlab.com/khloraa_scaffolding/khloraascaf_utils"
 Repository = "https://gitlab.com/khloraa_scaffolding/khloraascaf_utils"
-Documentation = "https://khloraascaf_utils.readthedocs.io"
-Changelog = "https://khloraascaf_utils.readthedocs.io/en/latest/changelog.html"
+Documentation = "https://khloraascaf-utils.readthedocs.io"
+Changelog = "https://khloraascaf-utils.readthedocs.io/en/latest/changelog.html"
 
 [tool.setuptools.package-data]
 
 khloraascaf_utils = ["py.typed"]
```

### Comparing `khloraascaf_utils-0.8.2/src/khloraascaf_utils/artificial_data.py` & `khloraascaf_utils-0.9.0/src/khloraascaf_utils/artificial_data.py`

 * *Files identical despite different names*

### Comparing `khloraascaf_utils-0.8.2/src/khloraascaf_utils/asm_graph_to_fasta.py` & `khloraascaf_utils-0.9.0/src/khloraascaf_utils/asm_graph_to_fasta.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from Bio import Seq, SeqIO
 from khloraascaf.assembly_graph import AssemblyGraph, rev_oriented_contig
 from khloraascaf.inputs import IdCT, IdLT, read_contig_links_file
 from khloraascaf.outputs import OrCT
 from revsymg.index_lib import FORWARD_INT, IndexT, IndOrT, OrT
 
 
-# TODO subcommand cli from files to sequences
+# TODO subcommand CLI from files to sequences
 
 # ============================================================================ #
 #                                     CLASS                                    #
 # ============================================================================ #
 class SequenceGraph():
     """Assembly graph enriched with region sequences.
 
@@ -31,15 +31,15 @@
     ```
     """
 
     def __init__(self, asm_graph: AssemblyGraph, contig_sequences_file: Path,
                  contig_links_file: Path, link_sequences_file: Path):
         """The Initialiser."""
         #
-        # Canonical couple of oriented contig for each link id (forward)
+        # Canonical couple of oriented contig for each link ID (forward)
         #
         self.__orc_link_to_id: dict[tuple[OrCT, OrCT], IdLT] = {}
         #
         # Sequence for each forward link identifier
         # OPTIMIZE stop keeping in hard memory: index method?
         self.__link_sequences: dict[IdLT, Seq.Seq] = {}
```

### Comparing `khloraascaf_utils-0.8.2/src/khloraascaf_utils/contigs_attributes.py` & `khloraascaf_utils-0.9.0/src/khloraascaf_utils/contigs_attributes.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,25 +26,26 @@
 Thus, the disjoint union alignment length can equals :math:`0` to :math:`|s|`.
 """
 
 # ============================================================================ #
 #                                   CONSTANTS                                  #
 # ============================================================================ #
 __DECIMAL_CONTEXT = Context(prec=3)
+CEIL_LIMIT = __DECIMAL_CONTEXT.create_decimal_from_float(0.1)
 
 
 # ============================================================================ #
 #                                   FUNCTIONS                                  #
 # ============================================================================ #
 def cov_to_mult(cov_contig: CovT, cov_unique: CovT) -> MultT:
     r"""Set multiplicity according to the given coverages.
 
     .. math::
 
-        mult = max\left(1, \left\lceil \frac{c_{cov}}{s_{cov}} - 0.9 \right\rceil\right)
+        mult = max\left(1, \left\lceil \frac{c_{cov}}{s_{cov}} - 0.1 \right\rceil\right)
 
     Parameters
     ----------
     cov_contig : CovT
         Contig's coverage
     cov_unique : CovT
         Unique contig's coverage
@@ -54,22 +55,19 @@
     MultT
         Contig's multiplicities
 
     Warnings
     --------
     Because of floating operation the result may vary a little.
     """  # noqa
-    mult_contig = (
+    cov_normalised_by_s = (
         __DECIMAL_CONTEXT.create_decimal_from_float(cov_contig)
         / __DECIMAL_CONTEXT.create_decimal_from_float(cov_unique)
     )
-    fraction = mult_contig - int(mult_contig)
-    if fraction > 0.1:
-        return max(1, ceil(mult_contig))
-    return max(1, floor(mult_contig))
+    return max(1, ceil(cov_normalised_by_s - CEIL_LIMIT))
 
 
 def dis_union_align_len_to_presence_score(align_length: DisUnionAlignLenT,
                                           contig_length: LenT) -> PresScoreT:
     r"""Calculate the presence score of contig.
 
     .. math::
```

### Comparing `khloraascaf_utils-0.8.2/src/khloraascaf_utils/to_networkx.py` & `khloraascaf_utils-0.9.0/src/khloraascaf_utils/to_networkx.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 # -*- coding=utf-8 -*-
 
 """NetworkX and GraphML utilities."""
 
 from __future__ import annotations
 
 from collections.abc import Iterable
-from pathlib import Path
 
+from khloraascaf import DR_REGION_ID, IR_REGION_ID, MetadataDebug
 from khloraascaf.ilp.dirf_sets import DirFT, dirf, dirf_builder, dirf_other
 from khloraascaf.ilp.invf_sets import InvFT, invf, invf_builder, invf_other
 from khloraascaf.multiplied_doubled_contig_graph import (
     CIND_IND,
     COCC_IND,
     COR_IND,
     CTG_ID_ATTR,
     MULT_ATTR,
     PRESSCORE_ATTR,
     MDCGraph,
     MDCGraphIDContainer,
     OccOrCT,
 )
 from khloraascaf.outputs import ORIENT_INT_STR, read_map_of_regions
-from khloraascaf.utils_debug import read_vertices_of_regions
+from khloraascaf.utils_debug import (
+    DIRF_CODE,
+    INVF_CODE,
+    read_found_repeated_fragments,
+    read_vertices_of_regions,
+)
 from networkx import DiGraph
 from revsymg.index_lib import FORWARD_INT, REVERSE_INT, IndexT
 
 
 # DOCU docstring constants
-# DOCU new function
+# DOCU new functions
 # ============================================================================ #
 #                                   CONSTANTS                                  #
 # ============================================================================ #
 # ---------------------------------------------------------------------------- #
 #                              Graph Relation Type                             #
 # ---------------------------------------------------------------------------- #
 RELATION_ATTR = 'relation'
@@ -53,20 +58,20 @@
 
 # ---------------------------------------------------------------------------- #
 #                                   Solution                                   #
 # ---------------------------------------------------------------------------- #
 SOLUTION_PATH_PREFIX_ATTR = 'solution_path'
 """Prefix to write the solution path on the edges."""
 
-SOLUTION_INVF_PREFIX_ATTR = 'solution_invf'
-"""Prefix to write the solution inverted fragments."""
-
-SOLUTION_DIRF_PREFIX_ATTR = 'solution_dirf'
+SOLUTION_DIRF_PREFIX_ATTR = f'solution_{DIRF_CODE}'
 """Prefix to write the solution direct fragments."""
 
+SOLUTION_INVF_PREFIX_ATTR = f'solution_{INVF_CODE}'
+"""Prefix to write the solution inverted fragments."""
+
 SOLUTION_REGION_IND = 'solution_region'
 """Prefix for the vertices' region index attribute."""
 
 
 # ---------------------------------------------------------------------------- #
 #                                  File Output                                 #
 # ---------------------------------------------------------------------------- #
@@ -161,72 +166,92 @@
         f'{occorc[COCC_IND]}'
     )
 
 
 # ---------------------------------------------------------------------------- #
 #                         Add Vertices Of Regions Paths                        #
 # ---------------------------------------------------------------------------- #
-def add_vertices_of_regions_in_nxdigraph(nxgraph: DiGraph,
-                                         vertices_of_regions_path: Path,
-                                         map_of_regions_path: Path,
-                                         attribute_suffix: str):
+def add_result_in_nxdigraph_from_debug(nxgraph: DiGraph,
+                                       debug_metadata: MetadataDebug):
     """Add the solution in the nx DiGraph.
 
     Parameters
     ----------
     nxgraph : DiGraph
         NetworkX DiGraph
-    vertices_of_regions_path : Path
-        Vertices for each region
-    map_of_regions_path : Path
-        Order of oriented regions
-    attribute_suffix : str
-        Suffix for the attribute name
+    debug_metadata: MetadataDebug
+        Debug metadata
+
+    Notes
+    -----
+    The repeated fragments added into the graph are these of the last
+    scaffolding, e.g. for the ilp combination ir-dr,
+    the repeated fragments of dr are added
+    while for ir-dr-sc no repeated fragments are added.
     """
-    #
+    attribute_suffix = '-'.join(debug_metadata.ilp_combination())
+    # ------------------------------------------------------------------------ #
     # Record vertices and oriented regions path
-    #
+    # ------------------------------------------------------------------------ #
     vertices_regions: tuple[tuple[OccOrCT, ...], ...] = tuple(
-        read_vertices_of_regions(vertices_of_regions_path),
+        read_vertices_of_regions(debug_metadata.vertices_of_regions()),
     )
     first_region_discovered: list[bool] = [False] * len(vertices_regions)
-    #
+
+    # ------------------------------------------------------------------------ #
     # Add the solutions path and repeated fragments
-    #
+    # ------------------------------------------------------------------------ #
     vertex_path: list[OccOrCT] = []
-    for reg_ind, reg_or in read_map_of_regions(map_of_regions_path):
+    for reg_ind, reg_or in read_map_of_regions(debug_metadata.map_of_regions()):
+
         previous_end = len(vertex_path) - 1
         if reg_or == FORWARD_INT:
             if first_region_discovered[reg_ind]:
                 vertex_path.extend(
                     dirf_other(v) for v in vertices_regions[reg_ind]
                 )
-                add_solution_dirf_in_nxdigraph(
-                    nxgraph,
-                    (dirf_builder(v)[0] for v in vertices_regions[reg_ind]),
-                    attribute_suffix,
-                )
             else:
                 vertex_path.extend(vertices_regions[reg_ind])
         elif reg_or == REVERSE_INT:
             # Special case: if reverse, then it is the second IR
             vertex_path.extend(
-                (invf_other(v) for v in reversed(vertices_regions[reg_ind])),
-            )
-            add_solution_invf_in_nxdigraph(
-                nxgraph,
-                (invf_builder(v)[0] for v in vertices_regions[reg_ind]),
-                attribute_suffix,
+                invf_other(v) for v in reversed(vertices_regions[reg_ind])
             )
+
         add_solution_vertices_region_index(
             nxgraph, vertex_path[previous_end + 1:], reg_ind, attribute_suffix)
         first_region_discovered[reg_ind] = True
+
     vertex_path.append(vertex_path[0])
     add_solution_path_in_nxdigraph(nxgraph, vertex_path, attribute_suffix)
 
+    # ------------------------------------------------------------------------ #
+    # Add repeated fragments
+    # ------------------------------------------------------------------------ #
+    if debug_metadata.ilp_combination()[-1] == DR_REGION_ID:
+        add_solution_dirf_in_nxdigraph(
+            nxgraph,
+            (
+                dirf_builder(v)[0]
+                for _, v in read_found_repeated_fragments(
+                    debug_metadata.repeat_fragments())
+            ),
+            attribute_suffix,
+        )
+    elif debug_metadata.ilp_combination()[-1] == IR_REGION_ID:
+        add_solution_invf_in_nxdigraph(
+            nxgraph,
+            (
+                invf_builder(v)[0]
+                for _, v in read_found_repeated_fragments(
+                    debug_metadata.repeat_fragments())
+            ),
+            attribute_suffix,
+        )
+
 
 # ---------------------------------------------------------------------------- #
 #                           Add Vertex Path Solution                           #
 # ---------------------------------------------------------------------------- #
 def add_solution_path_in_nxdigraph(nxgraph: DiGraph,
                                    vertex_path: Iterable[OccOrCT],
                                    attribute_suffix: str):
```

### Comparing `khloraascaf_utils-0.8.2/src/khloraascaf_utils.egg-info/PKG-INFO` & `khloraascaf_utils-0.9.0/src/khloraascaf_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khloraascaf-utils
-Version: 0.8.2
+Version: 0.9.0
 Summary: Python utilities for khloraascaf python package.
 Author-email: vepain <victor.epain@laposte.net>
 License: ### GNU GENERAL PUBLIC LICENSE
         
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc.
@@ -677,16 +677,16 @@
         library, you may consider it more useful to permit linking proprietary
         applications with the library. If this is what you want to do, use the
         GNU Lesser General Public License instead of this License. But first,
         please read <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Project-URL: Homepage, https://gitlab.com/khloraa_scaffolding/khloraascaf_utils
 Project-URL: Repository, https://gitlab.com/khloraa_scaffolding/khloraascaf_utils
-Project-URL: Documentation, https://khloraascaf_utils.readthedocs.io
-Project-URL: Changelog, https://khloraascaf_utils.readthedocs.io/en/latest/changelog.html
+Project-URL: Documentation, https://khloraascaf-utils.readthedocs.io
+Project-URL: Changelog, https://khloraascaf-utils.readthedocs.io/en/latest/changelog.html
 Keywords: Scaffolding,Chloroplast,Assembly,DNA repeats
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -705,15 +705,15 @@
 [![Documentation Status](https://readthedocs.org/projects/khloraascaf-utils/badge/?version=latest)](https://khloraascaf-utils.readthedocs.io/en/latest/?badge=latest)
 
  <img src="docs/img/logo_transp.png" alt="revsymg logo"
 width="200" height="200">
 
 `khloraascaf_utils` is a Python utilities package for [khloraascaf](https://pypi.org/project/khloraascaf/) Python package.
 
-Please have a look to the [documentation website](https://khloraascaf_utils.readthedocs.io) for more details.
+Please have a look to the [documentation website](https://khloraascaf-utils.readthedocs.io) for more details.
 
 ## Quick installation
 
 To install the `khloraascaf_utils` package from the [PyPI repository](https://pypi.org/project/khloraascaf_utils/), run the `pip` command :
 ```sh
 pip install khloraascaf_utils
 ```
```

### Comparing `khloraascaf_utils-0.8.2/src/khloraascaf_utils.egg-info/SOURCES.txt` & `khloraascaf_utils-0.9.0/src/khloraascaf_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `khloraascaf_utils-0.8.2/tests/test_artificial_data.py` & `khloraascaf_utils-0.9.0/tests/test_artificial_data.py`

 * *Files identical despite different names*

### Comparing `khloraascaf_utils-0.8.2/tests/test_asm_graph_to_fasta.py` & `khloraascaf_utils-0.9.0/tests/test_asm_graph_to_fasta.py`

 * *Files identical despite different names*

### Comparing `khloraascaf_utils-0.8.2/tests/test_contigs_attributes.py` & `khloraascaf_utils-0.9.0/tests/test_contigs_attributes.py`

 * *Files identical despite different names*

