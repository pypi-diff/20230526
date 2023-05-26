# Comparing `tmp/glypy-1.0.8.tar.gz` & `tmp/glypy-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glypy-1.0.8.tar", last modified: Sat Mar 18 18:14:15 2023, max compression
+gzip compressed data, was "glypy-1.0.9.tar", last modified: Fri May 26 13:50:20 2023, max compression
```

## Comparing `glypy-1.0.8.tar` & `glypy-1.0.9.tar`

### file list

```diff
@@ -1,160 +1,161 @@
-drwxrwxrwx   0        0        0        0 2023-03-18 18:14:15.750165 glypy-1.0.8/
--rw-rw-rw-   0        0        0    11558 2023-03-18 18:10:44.000000 glypy-1.0.8/LICENSE
--rw-rw-rw-   0        0        0      451 2023-03-18 18:10:44.000000 glypy-1.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0      410 2023-03-18 18:10:44.000000 glypy-1.0.8/NOTICE
--rw-rw-rw-   0        0        0     3769 2023-03-18 18:14:15.750165 glypy-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2897 2023-03-18 18:10:44.000000 glypy-1.0.8/README.rst
--rw-rw-rw-   0        0        0       86 2023-03-18 18:10:44.000000 glypy-1.0.8/pyproject.toml
--rw-rw-rw-   0        0        0      168 2023-03-18 18:14:15.750165 glypy-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     5333 2023-03-18 18:10:44.000000 glypy-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-18 18:14:15.671339 glypy-1.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-03-18 18:14:15.686965 glypy-1.0.8/src/glypy/
--rw-rw-rw-   0        0        0      808 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-18 18:14:15.686965 glypy-1.0.8/src/glypy/_c/
--rw-rw-rw-   0        0        0        0 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/_c/__init__.py
--rw-rw-rw-   0        0        0     3810 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/_c/compat.h
--rw-rw-rw-   0        0        0      517 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/_c/compat.pxd
-drwxrwxrwx   0        0        0        0 2023-03-18 18:14:15.686965 glypy-1.0.8/src/glypy/_c/structure/
--rw-rw-rw-   0        0        0        0 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/_c/structure/__init__.py
--rw-rw-rw-   0        0        0      469 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/_c/structure/base.pxd
--rw-rw-rw-   0        0        0      917 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/_c/structure/base.pyx
--rw-rw-rw-   0        0        0   290017 2023-03-18 18:14:09.000000 glypy-1.0.8/src/glypy/_c/structure/glycan_composition.c
--rw-rw-rw-   0        0        0      579 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/_c/structure/glycan_composition.pxd
--rw-rw-rw-   0        0        0     4697 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/_c/structure/glycan_composition.pyx
--rw-rw-rw-   0        0        0      632 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/_c/structure/monosaccharide.pxd
--rw-rw-rw-   0        0        0   215677 2023-03-18 18:14:09.000000 glypy-1.0.8/src/glypy/_c/utils.c
--rw-rw-rw-   0        0        0      155 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/_c/utils.pxd
--rw-rw-rw-   0        0        0     7709 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/_c/utils.pyx
-drwxrwxrwx   0        0        0        0 2023-03-18 18:14:15.702591 glypy-1.0.8/src/glypy/algorithms/
--rw-rw-rw-   0        0        0      124 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/algorithms/__init__.py
--rw-rw-rw-   0        0        0     6876 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/algorithms/canonicalize.py
--rw-rw-rw-   0        0        0    37734 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/algorithms/database.py
--rw-rw-rw-   0        0        0    29573 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/algorithms/similarity.py
--rw-rw-rw-   0        0        0     5517 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/algorithms/storage.py
-drwxrwxrwx   0        0        0        0 2023-03-18 18:14:15.702591 glypy-1.0.8/src/glypy/algorithms/subtree_search/
--rw-rw-rw-   0        0        0      542 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/algorithms/subtree_search/__init__.py
--rw-rw-rw-   0        0        0    20500 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/algorithms/subtree_search/common_subgraph.py
--rw-rw-rw-   0        0        0    15781 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/algorithms/subtree_search/inclusion.py
-drwxrwxrwx   0        0        0        0 2023-03-18 18:14:15.702591 glypy-1.0.8/src/glypy/composition/
--rw-rw-rw-   0        0        0      278 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/composition/__init__.py
--rw-rw-rw-   0        0        0     3374 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/composition/atomic_data.py
--rw-rw-rw-   0        0        0      868 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/composition/base.py
--rw-rw-rw-   0        0        0   614345 2023-03-18 18:14:10.000000 glypy-1.0.8/src/glypy/composition/ccomposition.c
--rw-rw-rw-   0        0        0      946 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/composition/ccomposition.pxd
--rw-rw-rw-   0        0        0    22632 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/composition/ccomposition.pyx
--rw-rw-rw-   0        0        0     3810 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/composition/compat.h
--rw-rw-rw-   0        0        0      224 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/composition/compat.pxd
--rw-rw-rw-   0        0        0    20144 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/composition/composition.py
--rw-rw-rw-   0        0        0     7154 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/composition/composition_transform.py
--rw-rw-rw-   0        0        0   113966 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/composition/mass_dict.py
--rw-rw-rw-   0        0        0     4398 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/composition/molecular_graph.py
--rw-rw-rw-   0        0        0     6012 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/composition/structure_composition.py
-drwxrwxrwx   0        0        0        0 2023-03-18 18:14:15.702591 glypy-1.0.8/src/glypy/enzyme/
--rw-rw-rw-   0        0        0      954 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/enzyme/__init__.py
--rw-rw-rw-   0        0        0     9335 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/enzyme/ec.py
--rw-rw-rw-   0        0        0     5852 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/enzyme/glycome.py
--rw-rw-rw-   0        0        0     9187 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/enzyme/graph.py
--rw-rw-rw-   0        0        0    22509 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/enzyme/pathways.py
-drwxrwxrwx   0        0        0        0 2023-03-18 18:14:15.718903 glypy-1.0.8/src/glypy/io/
--rw-rw-rw-   0        0        0      416 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/io/__init__.py
--rw-rw-rw-   0        0        0     3496 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/io/_glycordf.py
--rw-rw-rw-   0        0        0     3074 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/io/byonic.py
--rw-rw-rw-   0        0        0    16642 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/io/cfg.py
-drwxrwxrwx   0        0        0        0 2023-03-18 18:14:15.718903 glypy-1.0.8/src/glypy/io/data/
--rw-rw-rw-   0        0        0   921734 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/io/data/enzyme.json
--rw-rw-rw-   0        0        0   409190 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/io/data/glycan.owl
--rw-rw-rw-   0        0        0     3903 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/io/file_utils.py
--rw-rw-rw-   0        0        0     2043 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/io/format_constants_map.py
--rw-rw-rw-   0        0        0    97017 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/io/glycoct.py
--rw-rw-rw-   0        0        0     8456 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/io/glycoct_xml.py
--rw-rw-rw-   0        0        0    11838 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/io/glycomedb.py
--rw-rw-rw-   0        0        0     8438 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/io/glyconnect.py
--rw-rw-rw-   0        0        0    36055 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/io/glyspace.py
--rw-rw-rw-   0        0        0    39021 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/io/gws.py
--rw-rw-rw-   0        0        0    51878 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/io/iupac.py
--rw-rw-rw-   0        0        0    12764 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/io/linear_code.py
--rw-rw-rw-   0        0        0     1896 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/io/monosaccharidedb.py
-drwxrwxrwx   0        0        0        0 2023-03-18 18:14:15.718903 glypy-1.0.8/src/glypy/io/nomenclature/
--rw-rw-rw-   0        0        0       36 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/io/nomenclature/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-18 18:14:15.718903 glypy-1.0.8/src/glypy/io/nomenclature/data/
--rw-rw-rw-   0        0        0     6640 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/io/nomenclature/data/monosaccharide_schematic.json
--rw-rw-rw-   0        0        0     2156 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/io/nomenclature/data/monosaccharide_synonyms.json
--rw-rw-rw-   0        0        0    10658 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/io/nomenclature/identity.py
--rw-rw-rw-   0        0        0      846 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/io/nomenclature/synonyms.py
--rw-rw-rw-   0        0        0     3733 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/io/tree_builder_utils.py
-drwxrwxrwx   0        0        0        0 2023-03-18 18:14:15.718903 glypy-1.0.8/src/glypy/io/wurcs/
--rw-rw-rw-   0        0        0      548 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/io/wurcs/__init__.py
--rw-rw-rw-   0        0        0      623 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/io/wurcs/basetype_conversion.py
--rw-rw-rw-   0        0        0    12181 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/io/wurcs/carbon_descriptors.py
--rw-rw-rw-   0        0        0     4240 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/io/wurcs/node_type.py
--rw-rw-rw-   0        0        0     7334 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/io/wurcs/parser.py
--rw-rw-rw-   0        0        0     7235 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/io/wurcs/substituent_conversion.py
--rw-rw-rw-   0        0        0      588 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/io/wurcs/utils.py
--rw-rw-rw-   0        0        0     5148 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/io/wurcs/writer.py
-drwxrwxrwx   0        0        0        0 2023-03-18 18:14:15.734537 glypy-1.0.8/src/glypy/plot/
--rw-rw-rw-   0        0        0      673 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/plot/__init__.py
--rw-rw-rw-   0        0        0     4125 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/plot/buchheim.py
--rw-rw-rw-   0        0        0    20064 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/plot/cfg_symbols.py
--rw-rw-rw-   0        0        0     4668 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/plot/common.py
--rw-rw-rw-   0        0        0    29279 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/plot/draw_tree.py
--rw-rw-rw-   0        0        0    23090 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/plot/fragment_annotation.py
--rw-rw-rw-   0        0        0     7804 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/plot/geometry.py
--rw-rw-rw-   0        0        0     1454 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/plot/iupac_symbols.py
--rw-rw-rw-   0        0        0     3049 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/plot/snfg_symbols.py
--rw-rw-rw-   0        0        0     7022 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/plot/symbolic_nomenclature.py
--rw-rw-rw-   0        0        0     7870 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/plot/topological_layout.py
-drwxrwxrwx   0        0        0        0 2023-03-18 18:14:15.734537 glypy-1.0.8/src/glypy/structure/
--rw-rw-rw-   0        0        0      442 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/structure/__init__.py
--rw-rw-rw-   0        0        0      910 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/structure/base.py
--rw-rw-rw-   0        0        0     5253 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/structure/constants.py
--rw-rw-rw-   0        0        0    19882 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/structure/crossring_fragments.py
-drwxrwxrwx   0        0        0        0 2023-03-18 18:14:15.734537 glypy-1.0.8/src/glypy/structure/data/
--rw-rw-rw-   0        0        0     2977 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/structure/data/glycans.hjson
--rw-rw-rw-   0        0        0     4685 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/structure/data/monosaccharides.hjson
--rw-rw-rw-   0        0        0    27946 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/structure/data/motifs.hjson
--rw-rw-rw-   0        0        0    12573 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/structure/fragment.py
--rw-rw-rw-   0        0        0    58470 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/structure/glycan.py
--rw-rw-rw-   0        0        0    58326 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/structure/glycan_composition.py
--rw-rw-rw-   0        0        0    29170 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/structure/link.py
--rw-rw-rw-   0        0        0     2523 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/structure/modification.py
--rw-rw-rw-   0        0        0    69664 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/structure/monosaccharide.py
--rw-rw-rw-   0        0        0     4701 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/structure/named_structures.py
--rw-rw-rw-   0        0        0     8813 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/structure/stereochemistry.py
--rw-rw-rw-   0        0        0    18433 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/structure/substituent.py
-drwxrwxrwx   0        0        0        0 2023-03-18 18:14:15.750165 glypy-1.0.8/src/glypy/utils/
--rw-rw-rw-   0        0        0      617 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/utils/__init__.py
--rw-rw-rw-   0        0        0     9045 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/utils/base.py
--rw-rw-rw-   0        0        0   534285 2023-03-18 18:12:18.000000 glypy-1.0.8/src/glypy/utils/cenum.c
--rw-rw-rw-   0        0        0      636 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/utils/cenum.pxd
--rw-rw-rw-   0        0        0     8336 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/utils/cenum.pyx
--rw-rw-rw-   0        0        0     5066 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/utils/compat.py
--rw-rw-rw-   0        0        0     8649 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/utils/enum.py
--rw-rw-rw-   0        0        0     1958 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/utils/lazy.py
--rw-rw-rw-   0        0        0     5917 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/utils/multimap.py
--rw-rw-rw-   0        0        0       19 2023-03-18 18:10:44.000000 glypy-1.0.8/src/glypy/version.py
-drwxrwxrwx   0        0        0        0 2023-03-18 18:14:15.686965 glypy-1.0.8/src/glypy.egg-info/
--rw-rw-rw-   0        0        0     3769 2023-03-18 18:14:10.000000 glypy-1.0.8/src/glypy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4381 2023-03-18 18:14:10.000000 glypy-1.0.8/src/glypy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-18 18:14:10.000000 glypy-1.0.8/src/glypy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-18 18:12:18.000000 glypy-1.0.8/src/glypy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      133 2023-03-18 18:14:10.000000 glypy-1.0.8/src/glypy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-03-18 18:14:10.000000 glypy-1.0.8/src/glypy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-18 18:14:15.750165 glypy-1.0.8/tests/
--rw-rw-rw-   0        0        0     4605 2023-03-18 18:10:44.000000 glypy-1.0.8/tests/test_composition.py
--rw-rw-rw-   0        0        0     2973 2023-03-18 18:10:44.000000 glypy-1.0.8/tests/test_databases.py
--rw-rw-rw-   0        0        0     2162 2023-03-18 18:10:44.000000 glypy-1.0.8/tests/test_enzyme.py
--rw-rw-rw-   0        0        0    16718 2023-03-18 18:10:44.000000 glypy-1.0.8/tests/test_glycan.py
--rw-rw-rw-   0        0        0    14204 2023-03-18 18:10:44.000000 glypy-1.0.8/tests/test_glycan_composition.py
--rw-rw-rw-   0        0        0     5858 2023-03-18 18:10:44.000000 glypy-1.0.8/tests/test_glycoct.py
--rw-rw-rw-   0        0        0     3217 2023-03-18 18:10:44.000000 glypy-1.0.8/tests/test_glyspace.py
--rw-rw-rw-   0        0        0     5552 2023-03-18 18:10:44.000000 glypy-1.0.8/tests/test_iupac.py
--rw-rw-rw-   0        0        0      633 2023-03-18 18:10:44.000000 glypy-1.0.8/tests/test_lazy.py
--rw-rw-rw-   0        0        0      998 2023-03-18 18:10:44.000000 glypy-1.0.8/tests/test_linear_code.py
--rw-rw-rw-   0        0        0     4534 2023-03-18 18:10:44.000000 glypy-1.0.8/tests/test_link.py
--rw-rw-rw-   0        0        0    11029 2023-03-18 18:10:44.000000 glypy-1.0.8/tests/test_monosaccharide.py
--rw-rw-rw-   0        0        0     2465 2023-03-18 18:10:44.000000 glypy-1.0.8/tests/test_nomenclature.py
--rw-rw-rw-   0        0        0     3145 2023-03-18 18:10:44.000000 glypy-1.0.8/tests/test_plots.py
--rw-rw-rw-   0        0        0     4331 2023-03-18 18:10:44.000000 glypy-1.0.8/tests/test_similarity_algorithms.py
--rw-rw-rw-   0        0        0     3668 2023-03-18 18:10:44.000000 glypy-1.0.8/tests/test_subtree_search.py
--rw-rw-rw-   0        0        0     5057 2023-03-18 18:10:44.000000 glypy-1.0.8/tests/test_wurcs.py
--rw-rw-rw-   0        0        0    16538 2023-03-18 18:10:44.000000 glypy-1.0.8/tests/tests_legacy.py
+drwxrwxrwx   0        0        0        0 2023-05-26 13:50:20.491516 glypy-1.0.9/
+-rw-rw-rw-   0        0        0    11558 2023-05-26 13:47:26.000000 glypy-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0      451 2023-05-26 13:47:26.000000 glypy-1.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      410 2023-05-26 13:47:26.000000 glypy-1.0.9/NOTICE
+-rw-rw-rw-   0        0        0     3769 2023-05-26 13:50:20.491516 glypy-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2897 2023-05-26 13:47:26.000000 glypy-1.0.9/README.rst
+-rw-rw-rw-   0        0        0       86 2023-05-26 13:47:26.000000 glypy-1.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0      168 2023-05-26 13:50:20.491516 glypy-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     5333 2023-05-26 13:47:26.000000 glypy-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 13:50:19.076253 glypy-1.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-05-26 13:50:19.091943 glypy-1.0.9/src/glypy/
+-rw-rw-rw-   0        0        0      808 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 13:50:19.091943 glypy-1.0.9/src/glypy/_c/
+-rw-rw-rw-   0        0        0        0 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/_c/__init__.py
+-rw-rw-rw-   0        0        0     3810 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/_c/compat.h
+-rw-rw-rw-   0        0        0      517 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/_c/compat.pxd
+drwxrwxrwx   0        0        0        0 2023-05-26 13:50:19.463352 glypy-1.0.9/src/glypy/_c/structure/
+-rw-rw-rw-   0        0        0        0 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/_c/structure/__init__.py
+-rw-rw-rw-   0        0        0      469 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/_c/structure/base.pxd
+-rw-rw-rw-   0        0        0      917 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/_c/structure/base.pyx
+-rw-rw-rw-   0        0        0   293057 2023-05-26 13:50:12.000000 glypy-1.0.9/src/glypy/_c/structure/glycan_composition.c
+-rw-rw-rw-   0        0        0      579 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/_c/structure/glycan_composition.pxd
+-rw-rw-rw-   0        0        0     4810 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/_c/structure/glycan_composition.pyx
+-rw-rw-rw-   0        0        0      632 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/_c/structure/monosaccharide.pxd
+-rw-rw-rw-   0        0        0   217084 2023-05-26 13:50:12.000000 glypy-1.0.9/src/glypy/_c/utils.c
+-rw-rw-rw-   0        0        0      155 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/_c/utils.pxd
+-rw-rw-rw-   0        0        0     7709 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/_c/utils.pyx
+drwxrwxrwx   0        0        0        0 2023-05-26 13:50:19.463352 glypy-1.0.9/src/glypy/algorithms/
+-rw-rw-rw-   0        0        0      124 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/algorithms/__init__.py
+-rw-rw-rw-   0        0        0     6876 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/algorithms/canonicalize.py
+-rw-rw-rw-   0        0        0    37734 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/algorithms/database.py
+-rw-rw-rw-   0        0        0    29573 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/algorithms/similarity.py
+-rw-rw-rw-   0        0        0     5517 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/algorithms/storage.py
+drwxrwxrwx   0        0        0        0 2023-05-26 13:50:19.463352 glypy-1.0.9/src/glypy/algorithms/subtree_search/
+-rw-rw-rw-   0        0        0      542 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/algorithms/subtree_search/__init__.py
+-rw-rw-rw-   0        0        0    20500 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/algorithms/subtree_search/common_subgraph.py
+-rw-rw-rw-   0        0        0    15781 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/algorithms/subtree_search/inclusion.py
+drwxrwxrwx   0        0        0        0 2023-05-26 13:50:19.463352 glypy-1.0.9/src/glypy/composition/
+-rw-rw-rw-   0        0        0      278 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/composition/__init__.py
+-rw-rw-rw-   0        0        0     3374 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/composition/atomic_data.py
+-rw-rw-rw-   0        0        0      868 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/composition/base.py
+-rw-rw-rw-   0        0        0   615910 2023-05-26 13:50:13.000000 glypy-1.0.9/src/glypy/composition/ccomposition.c
+-rw-rw-rw-   0        0        0      946 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/composition/ccomposition.pxd
+-rw-rw-rw-   0        0        0    22632 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/composition/ccomposition.pyx
+-rw-rw-rw-   0        0        0     3810 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/composition/compat.h
+-rw-rw-rw-   0        0        0      224 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/composition/compat.pxd
+-rw-rw-rw-   0        0        0    20144 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/composition/composition.py
+-rw-rw-rw-   0        0        0     7154 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/composition/composition_transform.py
+-rw-rw-rw-   0        0        0   113966 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/composition/mass_dict.py
+-rw-rw-rw-   0        0        0     4398 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/composition/molecular_graph.py
+-rw-rw-rw-   0        0        0     6012 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/composition/structure_composition.py
+drwxrwxrwx   0        0        0        0 2023-05-26 13:50:19.478966 glypy-1.0.9/src/glypy/enzyme/
+-rw-rw-rw-   0        0        0      954 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/enzyme/__init__.py
+-rw-rw-rw-   0        0        0     9335 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/enzyme/ec.py
+-rw-rw-rw-   0        0        0     5852 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/enzyme/glycome.py
+-rw-rw-rw-   0        0        0     9187 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/enzyme/graph.py
+-rw-rw-rw-   0        0        0    22509 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/enzyme/pathways.py
+drwxrwxrwx   0        0        0        0 2023-05-26 13:50:19.478966 glypy-1.0.9/src/glypy/io/
+-rw-rw-rw-   0        0        0      416 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/io/__init__.py
+-rw-rw-rw-   0        0        0     3496 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/io/_glycordf.py
+-rw-rw-rw-   0        0        0     3079 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/io/byonic.py
+-rw-rw-rw-   0        0        0    16642 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/io/cfg.py
+drwxrwxrwx   0        0        0        0 2023-05-26 13:50:19.478966 glypy-1.0.9/src/glypy/io/data/
+-rw-rw-rw-   0        0        0   921734 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/io/data/enzyme.json
+-rw-rw-rw-   0        0        0   409190 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/io/data/glycan.owl
+-rw-rw-rw-   0        0        0     3903 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/io/file_utils.py
+-rw-rw-rw-   0        0        0     2043 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/io/format_constants_map.py
+-rw-rw-rw-   0        0        0    97017 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/io/glycoct.py
+-rw-rw-rw-   0        0        0     8456 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/io/glycoct_xml.py
+-rw-rw-rw-   0        0        0    11838 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/io/glycomedb.py
+-rw-rw-rw-   0        0        0     9293 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/io/glyconnect.py
+-rw-rw-rw-   0        0        0    36055 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/io/glyspace.py
+-rw-rw-rw-   0        0        0    17394 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/io/gnome.py
+-rw-rw-rw-   0        0        0    39021 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/io/gws.py
+-rw-rw-rw-   0        0        0    51878 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/io/iupac.py
+-rw-rw-rw-   0        0        0    12764 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/io/linear_code.py
+-rw-rw-rw-   0        0        0     1896 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/io/monosaccharidedb.py
+drwxrwxrwx   0        0        0        0 2023-05-26 13:50:19.494591 glypy-1.0.9/src/glypy/io/nomenclature/
+-rw-rw-rw-   0        0        0       36 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/io/nomenclature/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 13:50:19.494591 glypy-1.0.9/src/glypy/io/nomenclature/data/
+-rw-rw-rw-   0        0        0     6640 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/io/nomenclature/data/monosaccharide_schematic.json
+-rw-rw-rw-   0        0        0     2156 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/io/nomenclature/data/monosaccharide_synonyms.json
+-rw-rw-rw-   0        0        0    10658 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/io/nomenclature/identity.py
+-rw-rw-rw-   0        0        0      846 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/io/nomenclature/synonyms.py
+-rw-rw-rw-   0        0        0     3733 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/io/tree_builder_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-26 13:50:19.494591 glypy-1.0.9/src/glypy/io/wurcs/
+-rw-rw-rw-   0        0        0      548 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/io/wurcs/__init__.py
+-rw-rw-rw-   0        0        0      623 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/io/wurcs/basetype_conversion.py
+-rw-rw-rw-   0        0        0    12181 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/io/wurcs/carbon_descriptors.py
+-rw-rw-rw-   0        0        0     4240 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/io/wurcs/node_type.py
+-rw-rw-rw-   0        0        0     7334 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/io/wurcs/parser.py
+-rw-rw-rw-   0        0        0     7857 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/io/wurcs/substituent_conversion.py
+-rw-rw-rw-   0        0        0      588 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/io/wurcs/utils.py
+-rw-rw-rw-   0        0        0     5148 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/io/wurcs/writer.py
+drwxrwxrwx   0        0        0        0 2023-05-26 13:50:19.494591 glypy-1.0.9/src/glypy/plot/
+-rw-rw-rw-   0        0        0      673 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/plot/__init__.py
+-rw-rw-rw-   0        0        0     4125 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/plot/buchheim.py
+-rw-rw-rw-   0        0        0    20064 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/plot/cfg_symbols.py
+-rw-rw-rw-   0        0        0     4668 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/plot/common.py
+-rw-rw-rw-   0        0        0    29279 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/plot/draw_tree.py
+-rw-rw-rw-   0        0        0    23090 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/plot/fragment_annotation.py
+-rw-rw-rw-   0        0        0     7804 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/plot/geometry.py
+-rw-rw-rw-   0        0        0     1454 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/plot/iupac_symbols.py
+-rw-rw-rw-   0        0        0     3049 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/plot/snfg_symbols.py
+-rw-rw-rw-   0        0        0     7022 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/plot/symbolic_nomenclature.py
+-rw-rw-rw-   0        0        0     7870 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/plot/topological_layout.py
+drwxrwxrwx   0        0        0        0 2023-05-26 13:50:20.475937 glypy-1.0.9/src/glypy/structure/
+-rw-rw-rw-   0        0        0      442 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/structure/__init__.py
+-rw-rw-rw-   0        0        0      910 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/structure/base.py
+-rw-rw-rw-   0        0        0     5253 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/structure/constants.py
+-rw-rw-rw-   0        0        0    19882 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/structure/crossring_fragments.py
+drwxrwxrwx   0        0        0        0 2023-05-26 13:50:20.475937 glypy-1.0.9/src/glypy/structure/data/
+-rw-rw-rw-   0        0        0     2977 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/structure/data/glycans.hjson
+-rw-rw-rw-   0        0        0     4685 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/structure/data/monosaccharides.hjson
+-rw-rw-rw-   0        0        0    27946 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/structure/data/motifs.hjson
+-rw-rw-rw-   0        0        0    12573 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/structure/fragment.py
+-rw-rw-rw-   0        0        0    58470 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/structure/glycan.py
+-rw-rw-rw-   0        0        0    58326 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/structure/glycan_composition.py
+-rw-rw-rw-   0        0        0    29170 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/structure/link.py
+-rw-rw-rw-   0        0        0     2523 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/structure/modification.py
+-rw-rw-rw-   0        0        0    69664 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/structure/monosaccharide.py
+-rw-rw-rw-   0        0        0     4701 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/structure/named_structures.py
+-rw-rw-rw-   0        0        0     8813 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/structure/stereochemistry.py
+-rw-rw-rw-   0        0        0    18433 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/structure/substituent.py
+drwxrwxrwx   0        0        0        0 2023-05-26 13:50:20.475937 glypy-1.0.9/src/glypy/utils/
+-rw-rw-rw-   0        0        0      617 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/utils/__init__.py
+-rw-rw-rw-   0        0        0     9045 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/utils/base.py
+-rw-rw-rw-   0        0        0   535990 2023-05-26 13:48:31.000000 glypy-1.0.9/src/glypy/utils/cenum.c
+-rw-rw-rw-   0        0        0      636 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/utils/cenum.pxd
+-rw-rw-rw-   0        0        0     8336 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/utils/cenum.pyx
+-rw-rw-rw-   0        0        0     5066 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/utils/compat.py
+-rw-rw-rw-   0        0        0     8649 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/utils/enum.py
+-rw-rw-rw-   0        0        0     1958 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/utils/lazy.py
+-rw-rw-rw-   0        0        0     5917 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/utils/multimap.py
+-rw-rw-rw-   0        0        0       19 2023-05-26 13:47:26.000000 glypy-1.0.9/src/glypy/version.py
+drwxrwxrwx   0        0        0        0 2023-05-26 13:50:19.091943 glypy-1.0.9/src/glypy.egg-info/
+-rw-rw-rw-   0        0        0     3769 2023-05-26 13:50:13.000000 glypy-1.0.9/src/glypy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4403 2023-05-26 13:50:13.000000 glypy-1.0.9/src/glypy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 13:50:13.000000 glypy-1.0.9/src/glypy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-26 13:48:31.000000 glypy-1.0.9/src/glypy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      133 2023-05-26 13:50:13.000000 glypy-1.0.9/src/glypy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-26 13:50:13.000000 glypy-1.0.9/src/glypy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-26 13:50:20.491516 glypy-1.0.9/tests/
+-rw-rw-rw-   0        0        0     4605 2023-05-26 13:47:26.000000 glypy-1.0.9/tests/test_composition.py
+-rw-rw-rw-   0        0        0     2973 2023-05-26 13:47:26.000000 glypy-1.0.9/tests/test_databases.py
+-rw-rw-rw-   0        0        0     2162 2023-05-26 13:47:26.000000 glypy-1.0.9/tests/test_enzyme.py
+-rw-rw-rw-   0        0        0    16718 2023-05-26 13:47:26.000000 glypy-1.0.9/tests/test_glycan.py
+-rw-rw-rw-   0        0        0    14204 2023-05-26 13:47:26.000000 glypy-1.0.9/tests/test_glycan_composition.py
+-rw-rw-rw-   0        0        0     5858 2023-05-26 13:47:26.000000 glypy-1.0.9/tests/test_glycoct.py
+-rw-rw-rw-   0        0        0     3217 2023-05-26 13:47:26.000000 glypy-1.0.9/tests/test_glyspace.py
+-rw-rw-rw-   0        0        0     5552 2023-05-26 13:47:26.000000 glypy-1.0.9/tests/test_iupac.py
+-rw-rw-rw-   0        0        0      633 2023-05-26 13:47:26.000000 glypy-1.0.9/tests/test_lazy.py
+-rw-rw-rw-   0        0        0      998 2023-05-26 13:47:26.000000 glypy-1.0.9/tests/test_linear_code.py
+-rw-rw-rw-   0        0        0     4534 2023-05-26 13:47:26.000000 glypy-1.0.9/tests/test_link.py
+-rw-rw-rw-   0        0        0    11029 2023-05-26 13:47:26.000000 glypy-1.0.9/tests/test_monosaccharide.py
+-rw-rw-rw-   0        0        0     2465 2023-05-26 13:47:26.000000 glypy-1.0.9/tests/test_nomenclature.py
+-rw-rw-rw-   0        0        0     3145 2023-05-26 13:47:26.000000 glypy-1.0.9/tests/test_plots.py
+-rw-rw-rw-   0        0        0     4331 2023-05-26 13:47:26.000000 glypy-1.0.9/tests/test_similarity_algorithms.py
+-rw-rw-rw-   0        0        0     3668 2023-05-26 13:47:26.000000 glypy-1.0.9/tests/test_subtree_search.py
+-rw-rw-rw-   0        0        0     5057 2023-05-26 13:47:26.000000 glypy-1.0.9/tests/test_wurcs.py
+-rw-rw-rw-   0        0        0    16538 2023-05-26 13:47:26.000000 glypy-1.0.9/tests/tests_legacy.py
```

### Comparing `glypy-1.0.8/LICENSE` & `glypy-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/PKG-INFO` & `glypy-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glypy
-Version: 1.0.8
+Version: 1.0.9
 Summary: A Glycoinformatics Toolkit
 Home-page: https://github.com/mobiusklein/glypy
 Maintainer: Joshua Klein
 Maintainer-email: jaklein@bu.edu
 Project-URL: Documentation, https://glypy.readthedocs.io/
 Project-URL: Repository, https://github.com/mobiusklein/glypy
 Keywords: glycomics glycan carbohydrate glycoinformatics glypy n-linked o-linked glycosaminoglycan
```

### Comparing `glypy-1.0.8/README.rst` & `glypy-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/setup.py` & `glypy-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/__init__.py` & `glypy-1.0.9/src/glypy/__init__.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/_c/compat.h` & `glypy-1.0.9/src/glypy/_c/compat.h`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/_c/compat.pxd` & `glypy-1.0.9/src/glypy/_c/compat.pxd`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/_c/structure/base.pyx` & `glypy-1.0.9/src/glypy/_c/structure/base.pyx`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/_c/structure/glycan_composition.c` & `glypy-1.0.9/src/glypy/_c/structure/glycan_composition.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.35 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "include_dirs": [
             "src/glypy/_c/"
@@ -21,16 +21,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -90,16 +90,20 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
@@ -215,15 +219,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -254,15 +258,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -1386,22 +1390,30 @@
 #define __Pyx_PyObject_GenericGetAttr PyObject_GenericGetAttr
 #endif
 
 /* SetVTable.proto */
 static int __Pyx_SetVtable(PyObject *dict, void *vtable);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
+#define __PYX_HAVE_RT_ImportType_proto_0_29_35
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
+#endif
+enum __Pyx_ImportType_CheckSize_0_29_35 {
+   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
 #endif
 
 /* GetVTable.proto */
 static void* __Pyx_GetVtable(PyObject *dict);
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
@@ -1478,18 +1490,18 @@
 #endif
 #define __Pyx_PyException_Check(obj) __Pyx_TypeCheck(obj, PyExc_Exception)
 
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
 /* VoidPtrImport.proto */
-static int __Pyx_ImportVoidPtr(PyObject *module, const char *name, void **p, const char *sig);
+static int __Pyx_ImportVoidPtr_0_29_35(PyObject *module, const char *name, void **p, const char *sig);
 
 /* FunctionImport.proto */
-static int __Pyx_ImportFunction(PyObject *module, const char *funcname, void (**f)(void), const char *sig);
+static int __Pyx_ImportFunction_0_29_35(PyObject *module, const char *funcname, void (**f)(void), const char *sig);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 static PyObject *__pyx_f_5glypy_2_c_9structure_18glycan_composition_16_CompositionBase__getitem_fast(struct __pyx_obj_5glypy_2_c_9structure_18glycan_composition__CompositionBase *__pyx_v_self, PyObject *__pyx_v_key, int __pyx_skip_dispatch); /* proto*/
 static PyObject *__pyx_f_5glypy_2_c_9structure_18glycan_composition_16_CompositionBase__setitem_fast(struct __pyx_obj_5glypy_2_c_9structure_18glycan_composition__CompositionBase *__pyx_v_self, PyObject *__pyx_v_key, PyObject *__pyx_v_value, int __pyx_skip_dispatch); /* proto*/
 static void __pyx_f_5glypy_2_c_9structure_18glycan_composition_16_CompositionBase__add_from(struct __pyx_obj_5glypy_2_c_9structure_18glycan_composition__CompositionBase *__pyx_v_self, struct __pyx_obj_5glypy_2_c_9structure_18glycan_composition__CompositionBase *__pyx_v_other); /* proto*/
@@ -3737,22 +3749,23 @@
   PyObject *__pyx_v_name = NULL;
   PyObject *__pyx_v_cnt = NULL;
   PyObject *__pyx_v_part = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
-  long __pyx_t_3;
-  PyObject *__pyx_t_4 = NULL;
+  int __pyx_t_3;
+  long __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
-  Py_ssize_t __pyx_t_7;
+  PyObject *__pyx_t_6 = NULL;
+  int __pyx_t_7;
   Py_ssize_t __pyx_t_8;
   Py_ssize_t __pyx_t_9;
-  PyObject *__pyx_t_10;
+  Py_ssize_t __pyx_t_10;
+  PyObject *__pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_reformat", 0);
 
   /* "glypy/_c/structure/glycan_composition.pyx":128
  *         tuple token
@@ -3779,248 +3792,285 @@
   __pyx_t_1 = 0;
 
   /* "glypy/_c/structure/glycan_composition.pyx":130
  *     tokens = []
  *     strings = []
  *     i = 0             # <<<<<<<<<<<<<<
  *     while PyDict_Next(self, &i, &k, &v):
- *         count = PyInt_AsLong(<object>v)
+ *         if not isinstance(<object>v, int):
  */
   __pyx_v_i = 0;
 
   /* "glypy/_c/structure/glycan_composition.pyx":131
  *     strings = []
  *     i = 0
  *     while PyDict_Next(self, &i, &k, &v):             # <<<<<<<<<<<<<<
- *         count = PyInt_AsLong(<object>v)
- *         if count != 0:
+ *         if not isinstance(<object>v, int):
+ *             count = PyInt_AsLong(int(<object>v))
  */
   while (1) {
     __pyx_t_2 = (PyDict_Next(__pyx_v_self, (&__pyx_v_i), (&__pyx_v_k), (&__pyx_v_v)) != 0);
     if (!__pyx_t_2) break;
 
     /* "glypy/_c/structure/glycan_composition.pyx":132
  *     i = 0
  *     while PyDict_Next(self, &i, &k, &v):
- *         count = PyInt_AsLong(<object>v)             # <<<<<<<<<<<<<<
+ *         if not isinstance(<object>v, int):             # <<<<<<<<<<<<<<
+ *             count = PyInt_AsLong(int(<object>v))
+ *         else:
+ */
+    __pyx_t_2 = PyInt_Check(((PyObject *)__pyx_v_v)); 
+    __pyx_t_3 = ((!(__pyx_t_2 != 0)) != 0);
+    if (__pyx_t_3) {
+
+      /* "glypy/_c/structure/glycan_composition.pyx":133
+ *     while PyDict_Next(self, &i, &k, &v):
+ *         if not isinstance(<object>v, int):
+ *             count = PyInt_AsLong(int(<object>v))             # <<<<<<<<<<<<<<
+ *         else:
+ *             count = PyInt_AsLong(<object>v)
+ */
+      __pyx_t_1 = __Pyx_PyNumber_Int(((PyObject *)__pyx_v_v)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 133, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __pyx_t_4 = PyInt_AsLong(__pyx_t_1); if (unlikely(__pyx_t_4 == ((long)-1L) && PyErr_Occurred())) __PYX_ERR(0, 133, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __pyx_v_count = __pyx_t_4;
+
+      /* "glypy/_c/structure/glycan_composition.pyx":132
+ *     i = 0
+ *     while PyDict_Next(self, &i, &k, &v):
+ *         if not isinstance(<object>v, int):             # <<<<<<<<<<<<<<
+ *             count = PyInt_AsLong(int(<object>v))
+ *         else:
+ */
+      goto __pyx_L5;
+    }
+
+    /* "glypy/_c/structure/glycan_composition.pyx":135
+ *             count = PyInt_AsLong(int(<object>v))
+ *         else:
+ *             count = PyInt_AsLong(<object>v)             # <<<<<<<<<<<<<<
  *         if count != 0:
  *             key = <object>k
  */
-    __pyx_t_3 = PyInt_AsLong(((PyObject *)__pyx_v_v)); if (unlikely(__pyx_t_3 == ((long)-1L) && PyErr_Occurred())) __PYX_ERR(0, 132, __pyx_L1_error)
-    __pyx_v_count = __pyx_t_3;
+    /*else*/ {
+      __pyx_t_4 = PyInt_AsLong(((PyObject *)__pyx_v_v)); if (unlikely(__pyx_t_4 == ((long)-1L) && PyErr_Occurred())) __PYX_ERR(0, 135, __pyx_L1_error)
+      __pyx_v_count = __pyx_t_4;
+    }
+    __pyx_L5:;
 
-    /* "glypy/_c/structure/glycan_composition.pyx":133
- *     while PyDict_Next(self, &i, &k, &v):
- *         count = PyInt_AsLong(<object>v)
+    /* "glypy/_c/structure/glycan_composition.pyx":136
+ *         else:
+ *             count = PyInt_AsLong(<object>v)
  *         if count != 0:             # <<<<<<<<<<<<<<
  *             key = <object>k
  *             PyList_Append(tokens, (key.mass(), str(key), (<object>v)))
  */
-    __pyx_t_2 = ((__pyx_v_count != 0) != 0);
-    if (__pyx_t_2) {
+    __pyx_t_3 = ((__pyx_v_count != 0) != 0);
+    if (__pyx_t_3) {
 
-      /* "glypy/_c/structure/glycan_composition.pyx":134
- *         count = PyInt_AsLong(<object>v)
+      /* "glypy/_c/structure/glycan_composition.pyx":137
+ *             count = PyInt_AsLong(<object>v)
  *         if count != 0:
  *             key = <object>k             # <<<<<<<<<<<<<<
  *             PyList_Append(tokens, (key.mass(), str(key), (<object>v)))
  *     PyList_Sort(tokens)
  */
       __pyx_t_1 = ((PyObject *)__pyx_v_k);
       __Pyx_INCREF(__pyx_t_1);
       __Pyx_XDECREF_SET(__pyx_v_key, __pyx_t_1);
       __pyx_t_1 = 0;
 
-      /* "glypy/_c/structure/glycan_composition.pyx":135
+      /* "glypy/_c/structure/glycan_composition.pyx":138
  *         if count != 0:
  *             key = <object>k
  *             PyList_Append(tokens, (key.mass(), str(key), (<object>v)))             # <<<<<<<<<<<<<<
  *     PyList_Sort(tokens)
  *     i = 0
  */
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_key, __pyx_n_s_mass); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 135, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_5 = NULL;
-      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
-        __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
-        if (likely(__pyx_t_5)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
-          __Pyx_INCREF(__pyx_t_5);
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_key, __pyx_n_s_mass); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 138, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __pyx_t_6 = NULL;
+      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
+        __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
+        if (likely(__pyx_t_6)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+          __Pyx_INCREF(__pyx_t_6);
           __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_4, function);
+          __Pyx_DECREF_SET(__pyx_t_5, function);
         }
       }
-      __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
-      __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 135, __pyx_L1_error)
+      __pyx_t_1 = (__pyx_t_6) ? __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_6) : __Pyx_PyObject_CallNoArg(__pyx_t_5);
+      __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 138, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyString_Type)), __pyx_v_key); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 135, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 135, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __pyx_t_5 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyString_Type)), __pyx_v_key); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 138, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
+      __pyx_t_6 = PyTuple_New(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 138, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GIVEREF(__pyx_t_1);
-      PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_1);
-      __Pyx_GIVEREF(__pyx_t_4);
-      PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_4);
+      PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_1);
+      __Pyx_GIVEREF(__pyx_t_5);
+      PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_5);
       __Pyx_INCREF(((PyObject *)__pyx_v_v));
       __Pyx_GIVEREF(((PyObject *)__pyx_v_v));
-      PyTuple_SET_ITEM(__pyx_t_5, 2, ((PyObject *)__pyx_v_v));
+      PyTuple_SET_ITEM(__pyx_t_6, 2, ((PyObject *)__pyx_v_v));
       __pyx_t_1 = 0;
-      __pyx_t_4 = 0;
-      __pyx_t_6 = PyList_Append(__pyx_v_tokens, __pyx_t_5); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 135, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __pyx_t_5 = 0;
+      __pyx_t_7 = PyList_Append(__pyx_v_tokens, __pyx_t_6); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(0, 138, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-      /* "glypy/_c/structure/glycan_composition.pyx":133
- *     while PyDict_Next(self, &i, &k, &v):
- *         count = PyInt_AsLong(<object>v)
+      /* "glypy/_c/structure/glycan_composition.pyx":136
+ *         else:
+ *             count = PyInt_AsLong(<object>v)
  *         if count != 0:             # <<<<<<<<<<<<<<
  *             key = <object>k
  *             PyList_Append(tokens, (key.mass(), str(key), (<object>v)))
  */
     }
   }
 
-  /* "glypy/_c/structure/glycan_composition.pyx":136
+  /* "glypy/_c/structure/glycan_composition.pyx":139
  *             key = <object>k
  *             PyList_Append(tokens, (key.mass(), str(key), (<object>v)))
  *     PyList_Sort(tokens)             # <<<<<<<<<<<<<<
  *     i = 0
  *     n = PyList_GET_SIZE(tokens)
  */
-  __pyx_t_6 = PyList_Sort(__pyx_v_tokens); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_t_7 = PyList_Sort(__pyx_v_tokens); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(0, 139, __pyx_L1_error)
 
-  /* "glypy/_c/structure/glycan_composition.pyx":137
+  /* "glypy/_c/structure/glycan_composition.pyx":140
  *             PyList_Append(tokens, (key.mass(), str(key), (<object>v)))
  *     PyList_Sort(tokens)
  *     i = 0             # <<<<<<<<<<<<<<
  *     n = PyList_GET_SIZE(tokens)
  *     for i in range(n):
  */
   __pyx_v_i = 0;
 
-  /* "glypy/_c/structure/glycan_composition.pyx":138
+  /* "glypy/_c/structure/glycan_composition.pyx":141
  *     PyList_Sort(tokens)
  *     i = 0
  *     n = PyList_GET_SIZE(tokens)             # <<<<<<<<<<<<<<
  *     for i in range(n):
  *         token = <tuple>PyList_GET_ITEM(tokens, i)
  */
   __pyx_v_n = PyList_GET_SIZE(__pyx_v_tokens);
 
-  /* "glypy/_c/structure/glycan_composition.pyx":139
+  /* "glypy/_c/structure/glycan_composition.pyx":142
  *     i = 0
  *     n = PyList_GET_SIZE(tokens)
  *     for i in range(n):             # <<<<<<<<<<<<<<
  *         token = <tuple>PyList_GET_ITEM(tokens, i)
  *         name = <object>PyTuple_GET_ITEM(token, 1)
  */
-  __pyx_t_7 = __pyx_v_n;
-  __pyx_t_8 = __pyx_t_7;
-  for (__pyx_t_9 = 0; __pyx_t_9 < __pyx_t_8; __pyx_t_9+=1) {
-    __pyx_v_i = __pyx_t_9;
+  __pyx_t_8 = __pyx_v_n;
+  __pyx_t_9 = __pyx_t_8;
+  for (__pyx_t_10 = 0; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
+    __pyx_v_i = __pyx_t_10;
 
-    /* "glypy/_c/structure/glycan_composition.pyx":140
+    /* "glypy/_c/structure/glycan_composition.pyx":143
  *     n = PyList_GET_SIZE(tokens)
  *     for i in range(n):
  *         token = <tuple>PyList_GET_ITEM(tokens, i)             # <<<<<<<<<<<<<<
  *         name = <object>PyTuple_GET_ITEM(token, 1)
  *         cnt = <object>PyTuple_GET_ITEM(token, 2)
  */
-    __pyx_t_10 = PyList_GET_ITEM(__pyx_v_tokens, __pyx_v_i);
-    __pyx_t_5 = ((PyObject *)__pyx_t_10);
-    __Pyx_INCREF(__pyx_t_5);
-    __Pyx_XDECREF_SET(__pyx_v_token, ((PyObject*)__pyx_t_5));
-    __pyx_t_5 = 0;
+    __pyx_t_11 = PyList_GET_ITEM(__pyx_v_tokens, __pyx_v_i);
+    __pyx_t_6 = ((PyObject *)__pyx_t_11);
+    __Pyx_INCREF(__pyx_t_6);
+    __Pyx_XDECREF_SET(__pyx_v_token, ((PyObject*)__pyx_t_6));
+    __pyx_t_6 = 0;
 
-    /* "glypy/_c/structure/glycan_composition.pyx":141
+    /* "glypy/_c/structure/glycan_composition.pyx":144
  *     for i in range(n):
  *         token = <tuple>PyList_GET_ITEM(tokens, i)
  *         name = <object>PyTuple_GET_ITEM(token, 1)             # <<<<<<<<<<<<<<
  *         cnt = <object>PyTuple_GET_ITEM(token, 2)
  *         part = "%s:%d" % (name, cnt)
  */
-    __pyx_t_10 = PyTuple_GET_ITEM(__pyx_v_token, 1);
-    __pyx_t_5 = ((PyObject *)__pyx_t_10);
-    __Pyx_INCREF(__pyx_t_5);
-    __Pyx_XDECREF_SET(__pyx_v_name, __pyx_t_5);
-    __pyx_t_5 = 0;
+    __pyx_t_11 = PyTuple_GET_ITEM(__pyx_v_token, 1);
+    __pyx_t_6 = ((PyObject *)__pyx_t_11);
+    __Pyx_INCREF(__pyx_t_6);
+    __Pyx_XDECREF_SET(__pyx_v_name, __pyx_t_6);
+    __pyx_t_6 = 0;
 
-    /* "glypy/_c/structure/glycan_composition.pyx":142
+    /* "glypy/_c/structure/glycan_composition.pyx":145
  *         token = <tuple>PyList_GET_ITEM(tokens, i)
  *         name = <object>PyTuple_GET_ITEM(token, 1)
  *         cnt = <object>PyTuple_GET_ITEM(token, 2)             # <<<<<<<<<<<<<<
  *         part = "%s:%d" % (name, cnt)
  *         PyList_Append(strings, part)
  */
-    __pyx_t_10 = PyTuple_GET_ITEM(__pyx_v_token, 2);
-    __pyx_t_5 = ((PyObject *)__pyx_t_10);
-    __Pyx_INCREF(__pyx_t_5);
-    __Pyx_XDECREF_SET(__pyx_v_cnt, __pyx_t_5);
-    __pyx_t_5 = 0;
+    __pyx_t_11 = PyTuple_GET_ITEM(__pyx_v_token, 2);
+    __pyx_t_6 = ((PyObject *)__pyx_t_11);
+    __Pyx_INCREF(__pyx_t_6);
+    __Pyx_XDECREF_SET(__pyx_v_cnt, __pyx_t_6);
+    __pyx_t_6 = 0;
 
-    /* "glypy/_c/structure/glycan_composition.pyx":143
+    /* "glypy/_c/structure/glycan_composition.pyx":146
  *         name = <object>PyTuple_GET_ITEM(token, 1)
  *         cnt = <object>PyTuple_GET_ITEM(token, 2)
  *         part = "%s:%d" % (name, cnt)             # <<<<<<<<<<<<<<
  *         PyList_Append(strings, part)
  *     return "{%s}" % '; '.join(strings)
  */
-    __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 143, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 146, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
     __Pyx_INCREF(__pyx_v_name);
     __Pyx_GIVEREF(__pyx_v_name);
-    PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_name);
+    PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_v_name);
     __Pyx_INCREF(__pyx_v_cnt);
     __Pyx_GIVEREF(__pyx_v_cnt);
-    PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_v_cnt);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_s_d, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 143, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __Pyx_XDECREF_SET(__pyx_v_part, ((PyObject*)__pyx_t_4));
-    __pyx_t_4 = 0;
+    PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_v_cnt);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_s_d, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 146, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_XDECREF_SET(__pyx_v_part, ((PyObject*)__pyx_t_5));
+    __pyx_t_5 = 0;
 
-    /* "glypy/_c/structure/glycan_composition.pyx":144
+    /* "glypy/_c/structure/glycan_composition.pyx":147
  *         cnt = <object>PyTuple_GET_ITEM(token, 2)
  *         part = "%s:%d" % (name, cnt)
  *         PyList_Append(strings, part)             # <<<<<<<<<<<<<<
  *     return "{%s}" % '; '.join(strings)
  */
-    __pyx_t_6 = PyList_Append(__pyx_v_strings, __pyx_v_part); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 144, __pyx_L1_error)
+    __pyx_t_7 = PyList_Append(__pyx_v_strings, __pyx_v_part); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(0, 147, __pyx_L1_error)
   }
 
-  /* "glypy/_c/structure/glycan_composition.pyx":145
+  /* "glypy/_c/structure/glycan_composition.pyx":148
  *         part = "%s:%d" % (name, cnt)
  *         PyList_Append(strings, part)
  *     return "{%s}" % '; '.join(strings)             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_4 = __Pyx_PyString_Join(__pyx_kp_s_, __pyx_v_strings); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 145, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_s, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 145, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyString_Join(__pyx_kp_s_, __pyx_v_strings); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 148, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (!(likely(PyString_CheckExact(__pyx_t_5))||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "str", Py_TYPE(__pyx_t_5)->tp_name), 0))) __PYX_ERR(0, 145, __pyx_L1_error)
-  __pyx_r = ((PyObject*)__pyx_t_5);
-  __pyx_t_5 = 0;
+  __pyx_t_6 = __Pyx_PyString_Format(__pyx_kp_s_s, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 148, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (!(likely(PyString_CheckExact(__pyx_t_6))||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "str", Py_TYPE(__pyx_t_6)->tp_name), 0))) __PYX_ERR(0, 148, __pyx_L1_error)
+  __pyx_r = ((PyObject*)__pyx_t_6);
+  __pyx_t_6 = 0;
   goto __pyx_L0;
 
   /* "glypy/_c/structure/glycan_composition.pyx":118
  * 
  * 
  * cdef str _reformat(dict self):             # <<<<<<<<<<<<<<
  *     cdef:
  *         list tokens, strings
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("glypy._c.structure.glycan_composition._reformat", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_tokens);
   __Pyx_XDECREF(__pyx_v_strings);
   __Pyx_XDECREF(__pyx_v_key);
   __Pyx_XDECREF(__pyx_v_token);
@@ -4213,15 +4263,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
@@ -4301,15 +4351,15 @@
   {&__pyx_n_s_total_composition, __pyx_k_total_composition, sizeof(__pyx_k_total_composition), 0, 0, 1, 1},
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
   {&__pyx_n_s_update_from_typed_map, __pyx_k_update_from_typed_map, sizeof(__pyx_k_update_from_typed_map), 0, 0, 1, 1},
   {&__pyx_n_s_value, __pyx_k_value, sizeof(__pyx_k_value), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 139, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 142, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
@@ -4412,28 +4462,26 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule("glypy.composition.ccomposition"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5glypy_11composition_12ccomposition_CComposition = __Pyx_ImportType(__pyx_t_1, "glypy.composition.ccomposition", "CComposition", sizeof(struct __pyx_obj_5glypy_11composition_12ccomposition_CComposition), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5glypy_11composition_12ccomposition_CComposition) __PYX_ERR(2, 2, __pyx_L1_error)
+  __pyx_ptype_5glypy_11composition_12ccomposition_CComposition = __Pyx_ImportType_0_29_35(__pyx_t_1, "glypy.composition.ccomposition", "CComposition", sizeof(struct __pyx_obj_5glypy_11composition_12ccomposition_CComposition), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_5glypy_11composition_12ccomposition_CComposition),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5glypy_11composition_12ccomposition_CComposition) __PYX_ERR(2, 2, __pyx_L1_error)
   __pyx_vtabptr_5glypy_11composition_12ccomposition_CComposition = (struct __pyx_vtabstruct_5glypy_11composition_12ccomposition_CComposition*)__Pyx_GetVtable(__pyx_ptype_5glypy_11composition_12ccomposition_CComposition->tp_dict); if (unlikely(!__pyx_vtabptr_5glypy_11composition_12ccomposition_CComposition)) __PYX_ERR(2, 2, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -4445,19 +4493,19 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_variable_import_code", 0);
   /*--- Variable import code ---*/
   __pyx_t_1 = PyImport_ImportModule("glypy.composition.ccomposition"); if (!__pyx_t_1) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_ImportVoidPtr(__pyx_t_1, "_atom", (void **)&__pyx_vp_5glypy_11composition_12ccomposition__atom, "PyObject *") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportVoidPtr(__pyx_t_1, "_formula", (void **)&__pyx_vp_5glypy_11composition_12ccomposition__formula, "PyObject *") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportVoidPtr(__pyx_t_1, "_isotope_string", (void **)&__pyx_vp_5glypy_11composition_12ccomposition__isotope_string, "PyObject *") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportVoidPtr(__pyx_t_1, "isotope_pattern", (void **)&__pyx_vp_5glypy_11composition_12ccomposition_isotope_pattern, "PyObject *") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportVoidPtr(__pyx_t_1, "formula_pattern", (void **)&__pyx_vp_5glypy_11composition_12ccomposition_formula_pattern, "PyObject *") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportVoidPtr_0_29_35(__pyx_t_1, "_atom", (void **)&__pyx_vp_5glypy_11composition_12ccomposition__atom, "PyObject *") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportVoidPtr_0_29_35(__pyx_t_1, "_formula", (void **)&__pyx_vp_5glypy_11composition_12ccomposition__formula, "PyObject *") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportVoidPtr_0_29_35(__pyx_t_1, "_isotope_string", (void **)&__pyx_vp_5glypy_11composition_12ccomposition__isotope_string, "PyObject *") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportVoidPtr_0_29_35(__pyx_t_1, "isotope_pattern", (void **)&__pyx_vp_5glypy_11composition_12ccomposition_isotope_pattern, "PyObject *") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportVoidPtr_0_29_35(__pyx_t_1, "formula_pattern", (void **)&__pyx_vp_5glypy_11composition_12ccomposition_formula_pattern, "PyObject *") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -4469,15 +4517,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_import_code", 0);
   /*--- Function import code ---*/
   __pyx_t_1 = PyImport_ImportModule("glypy._c.utils"); if (!__pyx_t_1) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_ImportFunction(__pyx_t_1, "_prepare_glycan_composition_string", (void (**)(void))&__pyx_f_5glypy_2_c_5utils__prepare_glycan_composition_string, "PyObject *(PyObject *, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_35(__pyx_t_1, "_prepare_glycan_composition_string", (void (**)(void))&__pyx_f_5glypy_2_c_5utils__prepare_glycan_composition_string, "PyObject *(PyObject *, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -5506,61 +5554,79 @@
     return 0;
 bad:
     Py_XDECREF(ob);
     return -1;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+#ifndef __PYX_HAVE_RT_ImportType_0_29_35
+#define __PYX_HAVE_RT_ImportType_0_29_35
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -6100,15 +6166,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -6296,15 +6362,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -6571,17 +6637,17 @@
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
 }
 
 /* VoidPtrImport */
-#ifndef __PYX_HAVE_RT_ImportVoidPtr
-#define __PYX_HAVE_RT_ImportVoidPtr
-static int __Pyx_ImportVoidPtr(PyObject *module, const char *name, void **p, const char *sig) {
+#ifndef __PYX_HAVE_RT_ImportVoidPtr_0_29_35
+#define __PYX_HAVE_RT_ImportVoidPtr_0_29_35
+static int __Pyx_ImportVoidPtr_0_29_35(PyObject *module, const char *name, void **p, const char *sig) {
     PyObject *d = 0;
     PyObject *cobj = 0;
     d = PyObject_GetAttrString(module, (char *)"__pyx_capi__");
     if (!d)
         goto bad;
     cobj = PyDict_GetItemString(d, name);
     if (!cobj) {
@@ -6620,17 +6686,17 @@
 bad:
     Py_XDECREF(d);
     return -1;
 }
 #endif
 
 /* FunctionImport */
-#ifndef __PYX_HAVE_RT_ImportFunction
-#define __PYX_HAVE_RT_ImportFunction
-static int __Pyx_ImportFunction(PyObject *module, const char *funcname, void (**f)(void), const char *sig) {
+#ifndef __PYX_HAVE_RT_ImportFunction_0_29_35
+#define __PYX_HAVE_RT_ImportFunction_0_29_35
+static int __Pyx_ImportFunction_0_29_35(PyObject *module, const char *funcname, void (**f)(void), const char *sig) {
     PyObject *d = 0;
     PyObject *cobj = 0;
     union {
         void (*fp)(void);
         void *p;
     } tmp;
     d = PyObject_GetAttrString(module, (char *)"__pyx_capi__");
```

### Comparing `glypy-1.0.8/src/glypy/_c/structure/glycan_composition.pxd` & `glypy-1.0.9/src/glypy/_c/structure/glycan_composition.pxd`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/_c/structure/glycan_composition.pyx` & `glypy-1.0.9/src/glypy/_c/structure/glycan_composition.pyx`

 * *Files 5% similar despite different names*

```diff
@@ -125,15 +125,18 @@
         int count
         tuple token
 
     tokens = []
     strings = []
     i = 0
     while PyDict_Next(self, &i, &k, &v):
-        count = PyInt_AsLong(<object>v)
+        if not isinstance(<object>v, int):
+            count = PyInt_AsLong(int(<object>v))
+        else:
+            count = PyInt_AsLong(<object>v)
         if count != 0:
             key = <object>k
             PyList_Append(tokens, (key.mass(), str(key), (<object>v)))
     PyList_Sort(tokens)
     i = 0
     n = PyList_GET_SIZE(tokens)
     for i in range(n):
```

### Comparing `glypy-1.0.8/src/glypy/_c/structure/monosaccharide.pxd` & `glypy-1.0.9/src/glypy/_c/structure/monosaccharide.pxd`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/_c/utils.c` & `glypy-1.0.9/src/glypy/_c/utils.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.35 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "C:\\hostedtoolcache\\windows\\Python\\3.9.13\\x64\\lib\\site-packages\\glypy\\_c\\compat.h"
         ],
@@ -24,16 +24,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -93,16 +93,20 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
@@ -218,15 +222,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -257,15 +261,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -1191,22 +1195,30 @@
                                   int lineno, const char *filename,
                                   int full_traceback, int nogil);
 
 /* DivInt[long].proto */
 static CYTHON_INLINE long __Pyx_div_long(long, long);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
+#define __PYX_HAVE_RT_ImportType_proto_0_29_35
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
+#endif
+enum __Pyx_ImportType_CheckSize_0_29_35 {
+   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
 #endif
 
 /* PyDictVersioning.proto */
 #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 #define __PYX_DICT_VERSION_INIT  ((PY_UINT64_T) -1)
 #define __PYX_GET_DICT_VERSION(dict)  (((PyDictObject*)(dict))->ma_version_tag)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)\
@@ -3570,22 +3582,21 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(1, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(1, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -4262,28 +4273,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -4417,61 +4428,79 @@
     long q = a / b;
     long r = a - q*b;
     q -= ((r != 0) & ((r ^ b) < 0));
     return q;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+#ifndef __PYX_HAVE_RT_ImportType_0_29_35
+#define __PYX_HAVE_RT_ImportType_0_29_35
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -4814,15 +4843,15 @@
                         } else if (8 * sizeof(size_t) >= 4 * PyLong_SHIFT) {
                             return (size_t) (((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -5010,15 +5039,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -5282,15 +5311,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `glypy-1.0.8/src/glypy/_c/utils.pyx` & `glypy-1.0.9/src/glypy/_c/utils.pyx`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/algorithms/canonicalize.py` & `glypy-1.0.9/src/glypy/algorithms/canonicalize.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/algorithms/database.py` & `glypy-1.0.9/src/glypy/algorithms/database.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/algorithms/similarity.py` & `glypy-1.0.9/src/glypy/algorithms/similarity.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/algorithms/storage.py` & `glypy-1.0.9/src/glypy/algorithms/storage.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/algorithms/subtree_search/__init__.py` & `glypy-1.0.9/src/glypy/algorithms/subtree_search/__init__.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/algorithms/subtree_search/common_subgraph.py` & `glypy-1.0.9/src/glypy/algorithms/subtree_search/common_subgraph.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/algorithms/subtree_search/inclusion.py` & `glypy-1.0.9/src/glypy/algorithms/subtree_search/inclusion.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/composition/atomic_data.py` & `glypy-1.0.9/src/glypy/composition/atomic_data.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/composition/base.py` & `glypy-1.0.9/src/glypy/composition/base.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/composition/ccomposition.c` & `glypy-1.0.9/src/glypy/composition/ccomposition.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.35 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "C:\\hostedtoolcache\\windows\\Python\\3.9.13\\x64\\lib\\site-packages\\glypy\\composition\\compat.h"
         ],
@@ -24,16 +24,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -93,16 +93,20 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
@@ -218,15 +222,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -257,15 +261,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -1502,22 +1506,30 @@
 #define __Pyx_PyObject_GenericGetAttr PyObject_GenericGetAttr
 #endif
 
 /* SetVTable.proto */
 static int __Pyx_SetVtable(PyObject *dict, void *vtable);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
+#define __PYX_HAVE_RT_ImportType_proto_0_29_35
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
+#endif
+enum __Pyx_ImportType_CheckSize_0_29_35 {
+   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
@@ -10446,15 +10458,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {"composition_sum", (PyCFunction)__pyx_pw_5glypy_11composition_12ccomposition_3composition_sum, METH_O, 0},
   {"calculate_mass", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_5glypy_11composition_12ccomposition_5calculate_mass, METH_VARARGS|METH_KEYWORDS, __pyx_doc_5glypy_11composition_12ccomposition_4calculate_mass},
@@ -10737,32 +10749,29 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(1, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(1, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(2, 8, __pyx_L1_error)
+  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(2, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(3, 15, __pyx_L1_error)
+  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(3, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -12018,28 +12027,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -13176,61 +13185,79 @@
     return 0;
 bad:
     Py_XDECREF(ob);
     return -1;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+#ifndef __PYX_HAVE_RT_ImportType_0_29_35
+#define __PYX_HAVE_RT_ImportType_0_29_35
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -13626,15 +13653,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -13898,15 +13925,15 @@
                         } else if (8 * sizeof(size_t) >= 4 * PyLong_SHIFT) {
                             return (size_t) (((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -14094,15 +14121,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `glypy-1.0.8/src/glypy/composition/ccomposition.pxd` & `glypy-1.0.9/src/glypy/composition/ccomposition.pxd`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/composition/ccomposition.pyx` & `glypy-1.0.9/src/glypy/composition/ccomposition.pyx`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/composition/compat.h` & `glypy-1.0.9/src/glypy/composition/compat.h`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/composition/composition.py` & `glypy-1.0.9/src/glypy/composition/composition.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/composition/composition_transform.py` & `glypy-1.0.9/src/glypy/composition/composition_transform.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/composition/mass_dict.py` & `glypy-1.0.9/src/glypy/composition/mass_dict.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/composition/molecular_graph.py` & `glypy-1.0.9/src/glypy/composition/molecular_graph.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/composition/structure_composition.py` & `glypy-1.0.9/src/glypy/composition/structure_composition.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/enzyme/__init__.py` & `glypy-1.0.9/src/glypy/enzyme/__init__.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/enzyme/ec.py` & `glypy-1.0.9/src/glypy/enzyme/ec.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/enzyme/glycome.py` & `glypy-1.0.9/src/glypy/enzyme/glycome.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/enzyme/graph.py` & `glypy-1.0.9/src/glypy/enzyme/graph.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/enzyme/pathways.py` & `glypy-1.0.9/src/glypy/enzyme/pathways.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/io/_glycordf.py` & `glypy-1.0.9/src/glypy/io/_glycordf.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/io/byonic.py` & `glypy-1.0.9/src/glypy/io/byonic.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     "Hex": FrozenMonosaccharideResidue.from_iupac_lite("Hex"),
     "HexNAc": FrozenMonosaccharideResidue.from_iupac_lite('HexNAc'),
     "dHex": FrozenMonosaccharideResidue.from_iupac_lite('dHex'),
     "NeuAc": FrozenMonosaccharideResidue.from_iupac_lite("NeuAc"),
     "NeuGc": FrozenMonosaccharideResidue.from_iupac_lite("NeuGc"),
     "S": SubstituentResidue("sulfate"),
     "Sulfo": SubstituentResidue("sulfate"),
-    "S": SubstituentResidue("sulfate"),
+    "Sulpho": SubstituentResidue("sulfate"),
     "P": SubstituentResidue("phosphate"),
     "Ac": SubstituentResidue("acetyl"),
     "Acetyl": SubstituentResidue("acetyl"),
     "Phospho": SubstituentResidue("phosphate"),
     "Na": MolecularComposition("Na1H-1", Composition("Na1H-1")),
     "Sodium": MolecularComposition("Na1H-1", Composition("Na1H-1")),
     "GlcA": FrozenMonosaccharideResidue.from_iupac_lite("HexA"),
```

### Comparing `glypy-1.0.8/src/glypy/io/cfg.py` & `glypy-1.0.9/src/glypy/io/cfg.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/io/data/enzyme.json` & `glypy-1.0.9/src/glypy/io/data/enzyme.json`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/io/data/glycan.owl` & `glypy-1.0.9/src/glypy/io/data/glycan.owl`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/io/file_utils.py` & `glypy-1.0.9/src/glypy/io/file_utils.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/io/format_constants_map.py` & `glypy-1.0.9/src/glypy/io/format_constants_map.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/io/glycoct.py` & `glypy-1.0.9/src/glypy/io/glycoct.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/io/glycoct_xml.py` & `glypy-1.0.9/src/glypy/io/glycoct_xml.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/io/glycomedb.py` & `glypy-1.0.9/src/glypy/io/glycomedb.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/io/glyconnect.py` & `glypy-1.0.9/src/glypy/io/glyconnect.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,53 +2,72 @@
 Glyconnect
 ----------
 
 A simple dialect of the Glyconnect/GlycoMod glycan composition notation.
 '''
 import re
 
+from typing import Dict, Union, Optional, List, Tuple
+
 from urllib.parse import quote
 from dataclasses import dataclass, field
 from typing import List, Optional, Type, Generic, TypeVar
 
 from glypy.structure.glycan_composition import (
     FrozenGlycanComposition,
     FrozenMonosaccharideResidue,
     SubstituentResidue)
 from glypy.structure.glycan import Glycan
-from glypy.utils import invert_dict
 
 
 try:
     import requests
 except ImportError:
     requests = None
 
 #: The set of defined symbols and their mappings.
-defined_symbols = {
+defined_symbols: Dict[str, Union[SubstituentResidue, FrozenMonosaccharideResidue]] = {
     "Hex": FrozenMonosaccharideResidue.from_iupac_lite("Hex"),
     "HexNAc": FrozenMonosaccharideResidue.from_iupac_lite('HexNAc'),
     "dHex": FrozenMonosaccharideResidue.from_iupac_lite('dHex'),
     "NeuAc": FrozenMonosaccharideResidue.from_iupac_lite("NeuAc"),
     "NeuGc": FrozenMonosaccharideResidue.from_iupac_lite("NeuGc"),
     "S": SubstituentResidue("sulfate"),
+    "Su": SubstituentResidue("sulfate"),
+    "Sulpho": SubstituentResidue("sulfate"),
     "P": SubstituentResidue("phosphate"),
     "Ph": SubstituentResidue("phosphate"),
+    "Phospho": SubstituentResidue("phosphate"),
     "Xyl": FrozenMonosaccharideResidue.from_iupac_lite("Xyl"),
     "HexA": FrozenMonosaccharideResidue.from_iupac_lite("HexA"),
     "Pent": FrozenMonosaccharideResidue.from_iupac_lite("Pen"),
     "Kdn": FrozenMonosaccharideResidue.from_iupac_lite("Kdn"),
-    "Su": SubstituentResidue("sulfate"),
 }
 
 
-monosaccharide_to_symbol = invert_dict(defined_symbols)
+def _invert_mapping(table: Dict[str, Union[SubstituentResidue, FrozenMonosaccharideResidue]]) -> Dict[Union[SubstituentResidue, FrozenMonosaccharideResidue], str]:
+    inverted = {}
+    for k, v in table.items():
+        if v in inverted:
+            if len(k) > len(inverted[v]):
+                continue
+        inverted[v] = k
+    return inverted
+
+
+monosaccharide_to_symbol = _invert_mapping(defined_symbols)
+
+
+def _generate_pattern(symbols: List[str]) -> re.Pattern:
+    symbols = sorted(symbols, key=len, reverse=True)
+    return re.compile(f"({'|'.join(symbols)})(\d+?)")
 
 
 tokenizer = re.compile(r"([^:\s]+):(\d+)")
+undelimited_tokenizer = _generate_pattern(defined_symbols)
 
 
 def loads(string):
     '''Parse a GlyConnect glycan composition into a :class:`~.FrozenGlycanComposition`
 
     Parameters
     ----------
@@ -60,14 +79,16 @@
     :class:`~.FrozenGlycanComposition`
 
     Raises
     ------
     :class:`KeyError`: Raised if a key isn't defined by the GlyConnect dialect
     '''
     tokens = tokenizer.findall(string)
+    if not tokens:
+        tokens = undelimited_tokenizer.findall(string)
     gc = FrozenGlycanComposition()
     for mono, count in tokens:
         mono = defined_symbols[mono]
         count = int(count)
         gc[mono] += count
     return gc
```

### Comparing `glypy-1.0.8/src/glypy/io/glyspace.py` & `glypy-1.0.9/src/glypy/io/glyspace.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/io/gws.py` & `glypy-1.0.9/src/glypy/io/gws.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/io/iupac.py` & `glypy-1.0.9/src/glypy/io/iupac.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/io/linear_code.py` & `glypy-1.0.9/src/glypy/io/linear_code.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/io/monosaccharidedb.py` & `glypy-1.0.9/src/glypy/io/monosaccharidedb.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/io/nomenclature/data/monosaccharide_schematic.json` & `glypy-1.0.9/src/glypy/io/nomenclature/data/monosaccharide_schematic.json`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/io/nomenclature/data/monosaccharide_synonyms.json` & `glypy-1.0.9/src/glypy/io/nomenclature/data/monosaccharide_synonyms.json`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/io/nomenclature/identity.py` & `glypy-1.0.9/src/glypy/io/nomenclature/identity.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/io/nomenclature/synonyms.py` & `glypy-1.0.9/src/glypy/io/nomenclature/synonyms.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/io/tree_builder_utils.py` & `glypy-1.0.9/src/glypy/io/tree_builder_utils.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/io/wurcs/__init__.py` & `glypy-1.0.9/src/glypy/io/wurcs/__init__.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/io/wurcs/basetype_conversion.py` & `glypy-1.0.9/src/glypy/io/wurcs/basetype_conversion.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/io/wurcs/carbon_descriptors.py` & `glypy-1.0.9/src/glypy/io/wurcs/carbon_descriptors.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/io/wurcs/node_type.py` & `glypy-1.0.9/src/glypy/io/wurcs/node_type.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/io/wurcs/parser.py` & `glypy-1.0.9/src/glypy/io/wurcs/parser.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/io/wurcs/substituent_conversion.py` & `glypy-1.0.9/src/glypy/io/wurcs/substituent_conversion.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,63 @@
 import re
 from collections import namedtuple
+from typing import List
 
 from glypy.composition import molecular_graph, Composition, formula
 from glypy.structure import Substituent
 
 
-def tokenize_alin(code):
+def tokenize_alin(code: str) -> List[str]:
+    STATE_ALIN = 0
+    STATE_ISO = 1
     tokens = []
     current_token = ''
     i = 0
     n = len(code)
-    connector_symbols = ('=', '/', '#', '$')
+    connector_symbols = ('/', '$')
+    bond_symbols = ('=', '#')
+    state = STATE_ALIN
     while i < n:
         c = code[i]
         is_asterisk = c == '*'
         if c.isalpha() or is_asterisk:
             if c.isupper() or is_asterisk:
-                if current_token:
+                if current_token and state == STATE_ALIN:
                     tokens.append(current_token)
                     current_token = ''
                 current_token += c
+                state = STATE_ALIN
         elif c in ('^', '~'):
+            if current_token:
+                tokens.append(current_token)
+                current_token = ''
             current_token += code[i:i + 2]
             i += 2
+            state = STATE_ISO
             continue
         elif c in connector_symbols:
             if current_token:
                 tokens.append(current_token)
                 current_token = ''
             current_token += c
+        elif c in bond_symbols:
+            if current_token:
+                tokens.append(current_token)
+                current_token = ''
+            tokens.append(c)
         elif c.isdigit():
             current_token += c
 
         i += 1
     if current_token:
         tokens.append(current_token)
     return tokens
 
 
-def parse_alin(code):
+def parse_alin(code: str) -> molecular_graph.MolecularGraph:
     graph = molecular_graph.MolecularGraph()
     last_vertex = None
     bond_type = 1
 
     node_id_counter = 0
     for i, token in enumerate(tokenize_alin(code), 1):
         if token[0] in ('/', '$'):
@@ -60,44 +75,46 @@
             if "*" in token:
                 properties["is_backbone_carbon"] = True
                 token = 'C'
             node_id_counter += 1
             vertex = molecular_graph.Atom(token, node_id_counter, **properties)
             graph.add_vertex(vertex)
             if last_vertex is not None:
-                graph.add_edge(molecular_graph.Bond([last_vertex.id, vertex.id], bond_type))
+                graph.add_edge(
+                    molecular_graph.Bond([last_vertex.id, vertex.id], bond_type))
             bond_type = 1
             last_vertex = vertex
     return graph
 
 
-def alin_to_substituent(alin):
+def alin_to_substituent(alin: str) -> Substituent:
     if "*" in alin:
         name_query = alin.replace("*", "")
     else:
         name_query = alin
     try:
         record = map_to_substituent[name_query]
         name = record.name
     except KeyError:
-        raise KeyError("Could not locate name for substituent described by %r" % (alin,))
+        raise KeyError(
+            "Could not locate name for substituent described by %r" % (alin,))
     graph = parse_alin(alin)
     composition = Composition()
     unpaired_electrons = 2 if alin.startswith("*") else 1
     for node in graph:
         if node.data.get("is_backbone_carbon"):
             unpaired_electrons -= 1
             continue
         composition[node.element.symbol] += 1
         unpaired_electrons += node.unpaired_electrons
     composition["H"] += unpaired_electrons
     return Substituent(name, composition=composition)
 
 
-def substituent_to_alin(substituent):
+def substituent_to_alin(substituent: Substituent) -> str:
     try:
         name = substituent.name
     except AttributeError:
         name = str(substituent)
     record = substituent_to_map[name]
     return record.map_for_bmu
```

### Comparing `glypy-1.0.8/src/glypy/io/wurcs/utils.py` & `glypy-1.0.9/src/glypy/io/wurcs/utils.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/io/wurcs/writer.py` & `glypy-1.0.9/src/glypy/io/wurcs/writer.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/plot/__init__.py` & `glypy-1.0.9/src/glypy/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/plot/buchheim.py` & `glypy-1.0.9/src/glypy/plot/buchheim.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/plot/cfg_symbols.py` & `glypy-1.0.9/src/glypy/plot/cfg_symbols.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/plot/common.py` & `glypy-1.0.9/src/glypy/plot/common.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/plot/draw_tree.py` & `glypy-1.0.9/src/glypy/plot/draw_tree.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/plot/fragment_annotation.py` & `glypy-1.0.9/src/glypy/plot/fragment_annotation.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/plot/geometry.py` & `glypy-1.0.9/src/glypy/plot/geometry.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/plot/iupac_symbols.py` & `glypy-1.0.9/src/glypy/plot/iupac_symbols.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/plot/snfg_symbols.py` & `glypy-1.0.9/src/glypy/plot/snfg_symbols.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/plot/symbolic_nomenclature.py` & `glypy-1.0.9/src/glypy/plot/symbolic_nomenclature.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/plot/topological_layout.py` & `glypy-1.0.9/src/glypy/plot/topological_layout.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/structure/base.py` & `glypy-1.0.9/src/glypy/structure/base.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/structure/constants.py` & `glypy-1.0.9/src/glypy/structure/constants.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/structure/crossring_fragments.py` & `glypy-1.0.9/src/glypy/structure/crossring_fragments.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/structure/data/glycans.hjson` & `glypy-1.0.9/src/glypy/structure/data/glycans.hjson`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/structure/data/monosaccharides.hjson` & `glypy-1.0.9/src/glypy/structure/data/monosaccharides.hjson`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/structure/data/motifs.hjson` & `glypy-1.0.9/src/glypy/structure/data/motifs.hjson`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/structure/fragment.py` & `glypy-1.0.9/src/glypy/structure/fragment.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/structure/glycan.py` & `glypy-1.0.9/src/glypy/structure/glycan.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/structure/glycan_composition.py` & `glypy-1.0.9/src/glypy/structure/glycan_composition.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/structure/link.py` & `glypy-1.0.9/src/glypy/structure/link.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/structure/modification.py` & `glypy-1.0.9/src/glypy/structure/modification.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/structure/monosaccharide.py` & `glypy-1.0.9/src/glypy/structure/monosaccharide.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/structure/named_structures.py` & `glypy-1.0.9/src/glypy/structure/named_structures.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/structure/stereochemistry.py` & `glypy-1.0.9/src/glypy/structure/stereochemistry.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/structure/substituent.py` & `glypy-1.0.9/src/glypy/structure/substituent.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/utils/__init__.py` & `glypy-1.0.9/src/glypy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/utils/base.py` & `glypy-1.0.9/src/glypy/utils/base.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/utils/cenum.c` & `glypy-1.0.9/src/glypy/utils/cenum.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.35 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "include_dirs": [
             "src/glypy/_c/"
@@ -21,16 +21,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -90,16 +90,20 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
@@ -215,15 +219,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -254,15 +258,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -1509,22 +1513,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
+#define __PYX_HAVE_RT_ImportType_proto_0_29_35
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
+#endif
+enum __Pyx_ImportType_CheckSize_0_29_35 {
+   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
 #endif
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
@@ -8790,15 +8802,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_5glypy_5utils_5cenum_IntEnumValue __pyx_vtable_5glypy_5utils_5cenum_IntEnumValue;
 
 static PyObject *__pyx_tp_new_5glypy_5utils_5cenum_IntEnumValue(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_5glypy_5utils_5cenum_IntEnumValue *p;
@@ -8904,15 +8916,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_5glypy_5utils_5cenum_EnumMeta __pyx_vtable_5glypy_5utils_5cenum_EnumMeta;
 
 static PyObject *__pyx_tp_new_5glypy_5utils_5cenum_EnumMeta(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_5glypy_5utils_5cenum_EnumMeta *p;
@@ -9133,15 +9145,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_5glypy_5utils_5cenum___pyx_scope_struct____iter__ *__pyx_freelist_5glypy_5utils_5cenum___pyx_scope_struct____iter__[8];
 static int __pyx_freecount_5glypy_5utils_5cenum___pyx_scope_struct____iter__ = 0;
 
@@ -9254,15 +9266,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
@@ -9525,32 +9537,29 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(4, 8, __pyx_L1_error)
+  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(4, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(5, 15, __pyx_L1_error)
+  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(5, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -10877,28 +10886,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -11375,61 +11384,79 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+#ifndef __PYX_HAVE_RT_ImportType_0_29_35
+#define __PYX_HAVE_RT_ImportType_0_29_35
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -11746,15 +11773,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -12018,15 +12045,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -13422,15 +13449,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static int __pyx_Generator_init(void) {
     __pyx_GeneratorType_type.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
     __pyx_GeneratorType_type.tp_iter = PyObject_SelfIter;
     __pyx_GeneratorType = __Pyx_FetchCommonType(&__pyx_GeneratorType_type);
```

### Comparing `glypy-1.0.8/src/glypy/utils/cenum.pxd` & `glypy-1.0.9/src/glypy/utils/cenum.pxd`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/utils/cenum.pyx` & `glypy-1.0.9/src/glypy/utils/cenum.pyx`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/utils/compat.py` & `glypy-1.0.9/src/glypy/utils/compat.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/utils/enum.py` & `glypy-1.0.9/src/glypy/utils/enum.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/utils/lazy.py` & `glypy-1.0.9/src/glypy/utils/lazy.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy/utils/multimap.py` & `glypy-1.0.9/src/glypy/utils/multimap.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/src/glypy.egg-info/PKG-INFO` & `glypy-1.0.9/src/glypy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glypy
-Version: 1.0.8
+Version: 1.0.9
 Summary: A Glycoinformatics Toolkit
 Home-page: https://github.com/mobiusklein/glypy
 Maintainer: Joshua Klein
 Maintainer-email: jaklein@bu.edu
 Project-URL: Documentation, https://glypy.readthedocs.io/
 Project-URL: Repository, https://github.com/mobiusklein/glypy
 Keywords: glycomics glycan carbohydrate glycoinformatics glypy n-linked o-linked glycosaminoglycan
```

### Comparing `glypy-1.0.8/src/glypy.egg-info/SOURCES.txt` & `glypy-1.0.9/src/glypy.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 src/glypy/io/file_utils.py
 src/glypy/io/format_constants_map.py
 src/glypy/io/glycoct.py
 src/glypy/io/glycoct_xml.py
 src/glypy/io/glycomedb.py
 src/glypy/io/glyconnect.py
 src/glypy/io/glyspace.py
+src/glypy/io/gnome.py
 src/glypy/io/gws.py
 src/glypy/io/iupac.py
 src/glypy/io/linear_code.py
 src/glypy/io/monosaccharidedb.py
 src/glypy/io/tree_builder_utils.py
 src/glypy/io/data/enzyme.json
 src/glypy/io/data/glycan.owl
```

### Comparing `glypy-1.0.8/tests/test_composition.py` & `glypy-1.0.9/tests/test_composition.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/tests/test_databases.py` & `glypy-1.0.9/tests/test_databases.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/tests/test_enzyme.py` & `glypy-1.0.9/tests/test_enzyme.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/tests/test_glycan.py` & `glypy-1.0.9/tests/test_glycan.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/tests/test_glycan_composition.py` & `glypy-1.0.9/tests/test_glycan_composition.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/tests/test_glycoct.py` & `glypy-1.0.9/tests/test_glycoct.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/tests/test_glyspace.py` & `glypy-1.0.9/tests/test_glyspace.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/tests/test_iupac.py` & `glypy-1.0.9/tests/test_iupac.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/tests/test_lazy.py` & `glypy-1.0.9/tests/test_lazy.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/tests/test_linear_code.py` & `glypy-1.0.9/tests/test_linear_code.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/tests/test_link.py` & `glypy-1.0.9/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/tests/test_monosaccharide.py` & `glypy-1.0.9/tests/test_monosaccharide.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/tests/test_nomenclature.py` & `glypy-1.0.9/tests/test_nomenclature.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/tests/test_plots.py` & `glypy-1.0.9/tests/test_plots.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/tests/test_similarity_algorithms.py` & `glypy-1.0.9/tests/test_similarity_algorithms.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/tests/test_subtree_search.py` & `glypy-1.0.9/tests/test_subtree_search.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/tests/test_wurcs.py` & `glypy-1.0.9/tests/test_wurcs.py`

 * *Files identical despite different names*

### Comparing `glypy-1.0.8/tests/tests_legacy.py` & `glypy-1.0.9/tests/tests_legacy.py`

 * *Files identical despite different names*

