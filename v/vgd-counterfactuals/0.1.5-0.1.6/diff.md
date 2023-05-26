# Comparing `tmp/vgd_counterfactuals-0.1.5.tar.gz` & `tmp/vgd_counterfactuals-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vgd_counterfactuals-0.1.5.tar", max compression
+gzip compressed data, was "vgd_counterfactuals-0.1.6.tar", max compression
```

## Comparing `vgd_counterfactuals-0.1.5.tar` & `vgd_counterfactuals-0.1.6.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rwxr-xr-x   0        0        0     1070 2023-04-28 11:58:50.318682 vgd_counterfactuals-0.1.5/LICENSE
--rwxr-xr-x   0        0        0     6577 2023-05-26 08:35:07.821730 vgd_counterfactuals-0.1.5/README.rst
--rw-r--r--   0        0        0    75715 2023-04-30 10:49:40.133365 vgd_counterfactuals-0.1.5/banner.png
--rwxr-xr-x   0        0        0     1514 2023-05-26 08:35:07.801729 vgd_counterfactuals-0.1.5/pyproject.toml
--rwxr-xr-x   0        0        0        5 2023-05-26 08:35:07.821730 vgd_counterfactuals-0.1.5/vgd_counterfactuals/VERSION
--rwxr-xr-x   0        0        0       39 2023-04-30 10:06:54.410920 vgd_counterfactuals-0.1.5/vgd_counterfactuals/__init__.py
--rw-r--r--   0        0        0    10551 2023-05-26 08:35:02.917681 vgd_counterfactuals-0.1.5/vgd_counterfactuals/base.py
--rwxr-xr-x   0        0        0     5290 2023-04-28 11:58:50.338682 vgd_counterfactuals-0.1.5/vgd_counterfactuals/cli.py
--rw-r--r--   0        0        0     1950 2023-05-01 15:19:29.825180 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/00_quickstart.py
--rw-r--r--   0        0        0     3422 2023-05-01 15:37:09.041204 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/01_visualization.py
--rw-r--r--   0        0        0      471 2023-05-01 15:26:26.262286 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/README.rst
--rw-r--r--   0        0        0        0 2023-05-01 14:39:31.031283 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/__init__.py
--rw-r--r--   0        0        0      847 2023-05-01 15:19:38.033191 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/analysis.py
--rw-r--r--   0        0        0     2191 2023-05-01 15:19:38.025191 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/code.py
--rw-r--r--   0        0        0      778 2023-05-01 15:19:39.289193 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.json
--rw-r--r--   0        0        0    17914 2023-05-01 15:19:39.289193 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.png
--rw-r--r--   0        0        0      968 2023-05-01 15:19:38.169191 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.json
--rw-r--r--   0        0        0    17705 2023-05-01 15:19:38.169191 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.png
--rw-r--r--   0        0        0      968 2023-05-01 15:19:38.281191 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.json
--rw-r--r--   0        0        0    18723 2023-05-01 15:19:38.281191 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.png
--rw-r--r--   0        0        0      975 2023-05-01 15:19:38.393192 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.json
--rw-r--r--   0        0        0    19578 2023-05-01 15:19:38.393192 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.png
--rw-r--r--   0        0        0      974 2023-05-01 15:19:38.501192 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.json
--rw-r--r--   0        0        0    18471 2023-05-01 15:19:38.501192 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.png
--rw-r--r--   0        0        0      972 2023-05-01 15:19:38.617192 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.json
--rw-r--r--   0        0        0    19414 2023-05-01 15:19:38.617192 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.png
--rw-r--r--   0        0        0      978 2023-05-01 15:19:38.729192 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.json
--rw-r--r--   0        0        0    20003 2023-05-01 15:19:38.729192 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.png
--rw-r--r--   0        0        0      971 2023-05-01 15:19:38.841192 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.json
--rw-r--r--   0        0        0    23908 2023-05-01 15:19:38.841192 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.png
--rw-r--r--   0        0        0      970 2023-05-01 15:19:38.953192 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.json
--rw-r--r--   0        0        0    19642 2023-05-01 15:19:38.953192 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.png
--rw-r--r--   0        0        0      977 2023-05-01 15:19:39.065193 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.json
--rw-r--r--   0        0        0    19682 2023-05-01 15:19:39.065193 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.png
--rw-r--r--   0        0        0      969 2023-05-01 15:19:39.177193 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.json
--rw-r--r--   0        0        0    20380 2023-05-01 15:19:39.177193 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.png
--rw-r--r--   0        0        0   221293 2023-05-01 15:19:40.353194 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals.pdf
--rw-r--r--   0        0        0        2 2023-05-01 15:19:40.353194 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_data.json
--rw-r--r--   0        0        0      555 2023-05-01 15:19:40.353194 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_meta.json
--rw-r--r--   0        0        0     1328 2023-05-01 15:19:40.357194 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_out.log
--rw-r--r--   0        0        0     1334 2023-04-28 11:58:50.342682 vgd_counterfactuals-0.1.5/vgd_counterfactuals/experiments/README.rst
--rw-r--r--   0        0        0      209 2023-04-28 11:58:50.346682 vgd_counterfactuals-0.1.5/vgd_counterfactuals/experiments/results/README.rst
--rwxr-xr-x   0        0        0      729 2023-04-28 11:58:50.342682 vgd_counterfactuals-0.1.5/vgd_counterfactuals/experiments/template_experiment.py
--rw-r--r--   0        0        0      614 2023-04-28 11:58:50.342682 vgd_counterfactuals-0.1.5/vgd_counterfactuals/experiments/template_experiment_sub.py
--rw-r--r--   0        0        0        0 2023-04-28 12:00:41.971495 vgd_counterfactuals-0.1.5/vgd_counterfactuals/generate/__init__.py
--rw-r--r--   0        0        0      176 2023-04-30 07:11:09.422132 vgd_counterfactuals-0.1.5/vgd_counterfactuals/generate/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     8355 2023-05-26 08:30:52.863182 vgd_counterfactuals-0.1.5/vgd_counterfactuals/generate/__pycache__/molecules.cpython-310.pyc
--rw-r--r--   0        0        0    11111 2023-05-26 08:30:51.243165 vgd_counterfactuals-0.1.5/vgd_counterfactuals/generate/molecules.py
--rwxr-xr-x   0        0        0    19773 2023-04-14 06:32:11.000000 vgd_counterfactuals-0.1.5/vgd_counterfactuals/generate/smiles_one_step_changes.py
--rwxr-xr-x   0        0        0      997 2023-04-28 11:58:50.346682 vgd_counterfactuals-0.1.5/vgd_counterfactuals/templates/article.tex.j2
--rw-r--r--   0        0        0      490 2023-05-01 15:26:26.262286 vgd_counterfactuals-0.1.5/vgd_counterfactuals/testing.py
--rwxr-xr-x   0        0        0     5201 2023-05-01 15:30:16.327226 vgd_counterfactuals-0.1.5/vgd_counterfactuals/utils.py
--rw-r--r--   0        0        0     3370 2023-05-01 16:09:36.020519 vgd_counterfactuals-0.1.5/vgd_counterfactuals/visualization.py
--rw-r--r--   0        0        0     7622 1970-01-01 00:00:00.000000 vgd_counterfactuals-0.1.5/PKG-INFO
+-rwxr-xr-x   0        0        0     1070 2023-04-28 11:58:50.318682 vgd_counterfactuals-0.1.6/LICENSE
+-rwxr-xr-x   0        0        0     6577 2023-05-26 18:55:18.237103 vgd_counterfactuals-0.1.6/README.rst
+-rw-r--r--   0        0        0    75715 2023-04-30 10:49:40.133365 vgd_counterfactuals-0.1.6/banner.png
+-rwxr-xr-x   0        0        0     1514 2023-05-26 18:55:18.229103 vgd_counterfactuals-0.1.6/pyproject.toml
+-rwxr-xr-x   0        0        0        5 2023-05-26 18:55:18.237103 vgd_counterfactuals-0.1.6/vgd_counterfactuals/VERSION
+-rwxr-xr-x   0        0        0       39 2023-04-30 10:06:54.410920 vgd_counterfactuals-0.1.6/vgd_counterfactuals/__init__.py
+-rw-r--r--   0        0        0    11840 2023-05-26 18:53:16.524275 vgd_counterfactuals-0.1.6/vgd_counterfactuals/base.py
+-rwxr-xr-x   0        0        0     5290 2023-04-28 11:58:50.338682 vgd_counterfactuals-0.1.6/vgd_counterfactuals/cli.py
+-rw-r--r--   0        0        0     1950 2023-05-01 15:19:29.825180 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/00_quickstart.py
+-rw-r--r--   0        0        0     3422 2023-05-01 15:37:09.041204 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/01_visualization.py
+-rw-r--r--   0        0        0      471 2023-05-01 15:26:26.262286 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/README.rst
+-rw-r--r--   0        0        0        0 2023-05-01 14:39:31.031283 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/__init__.py
+-rw-r--r--   0        0        0      847 2023-05-01 15:19:38.033191 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/analysis.py
+-rw-r--r--   0        0        0     2191 2023-05-01 15:19:38.025191 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/code.py
+-rw-r--r--   0        0        0      778 2023-05-01 15:19:39.289193 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.json
+-rw-r--r--   0        0        0    17914 2023-05-01 15:19:39.289193 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.png
+-rw-r--r--   0        0        0      968 2023-05-01 15:19:38.169191 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.json
+-rw-r--r--   0        0        0    17705 2023-05-01 15:19:38.169191 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.png
+-rw-r--r--   0        0        0      968 2023-05-01 15:19:38.281191 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.json
+-rw-r--r--   0        0        0    18723 2023-05-01 15:19:38.281191 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.png
+-rw-r--r--   0        0        0      975 2023-05-01 15:19:38.393192 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.json
+-rw-r--r--   0        0        0    19578 2023-05-01 15:19:38.393192 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.png
+-rw-r--r--   0        0        0      974 2023-05-01 15:19:38.501192 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.json
+-rw-r--r--   0        0        0    18471 2023-05-01 15:19:38.501192 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.png
+-rw-r--r--   0        0        0      972 2023-05-01 15:19:38.617192 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.json
+-rw-r--r--   0        0        0    19414 2023-05-01 15:19:38.617192 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.png
+-rw-r--r--   0        0        0      978 2023-05-01 15:19:38.729192 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.json
+-rw-r--r--   0        0        0    20003 2023-05-01 15:19:38.729192 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.png
+-rw-r--r--   0        0        0      971 2023-05-01 15:19:38.841192 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.json
+-rw-r--r--   0        0        0    23908 2023-05-01 15:19:38.841192 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.png
+-rw-r--r--   0        0        0      970 2023-05-01 15:19:38.953192 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.json
+-rw-r--r--   0        0        0    19642 2023-05-01 15:19:38.953192 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.png
+-rw-r--r--   0        0        0      977 2023-05-01 15:19:39.065193 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.json
+-rw-r--r--   0        0        0    19682 2023-05-01 15:19:39.065193 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.png
+-rw-r--r--   0        0        0      969 2023-05-01 15:19:39.177193 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.json
+-rw-r--r--   0        0        0    20380 2023-05-01 15:19:39.177193 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.png
+-rw-r--r--   0        0        0   221293 2023-05-01 15:19:40.353194 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals.pdf
+-rw-r--r--   0        0        0        2 2023-05-01 15:19:40.353194 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_data.json
+-rw-r--r--   0        0        0      555 2023-05-01 15:19:40.353194 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_meta.json
+-rw-r--r--   0        0        0     1328 2023-05-01 15:19:40.357194 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_out.log
+-rw-r--r--   0        0        0     1334 2023-04-28 11:58:50.342682 vgd_counterfactuals-0.1.6/vgd_counterfactuals/experiments/README.rst
+-rw-r--r--   0        0        0      209 2023-04-28 11:58:50.346682 vgd_counterfactuals-0.1.6/vgd_counterfactuals/experiments/results/README.rst
+-rwxr-xr-x   0        0        0      729 2023-04-28 11:58:50.342682 vgd_counterfactuals-0.1.6/vgd_counterfactuals/experiments/template_experiment.py
+-rw-r--r--   0        0        0      614 2023-04-28 11:58:50.342682 vgd_counterfactuals-0.1.6/vgd_counterfactuals/experiments/template_experiment_sub.py
+-rw-r--r--   0        0        0        0 2023-04-28 12:00:41.971495 vgd_counterfactuals-0.1.6/vgd_counterfactuals/generate/__init__.py
+-rw-r--r--   0        0        0      176 2023-04-30 07:11:09.422132 vgd_counterfactuals-0.1.6/vgd_counterfactuals/generate/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     8355 2023-05-26 08:30:52.863182 vgd_counterfactuals-0.1.6/vgd_counterfactuals/generate/__pycache__/molecules.cpython-310.pyc
+-rw-r--r--   0        0        0    11111 2023-05-26 08:30:51.243165 vgd_counterfactuals-0.1.6/vgd_counterfactuals/generate/molecules.py
+-rwxr-xr-x   0        0        0    19773 2023-04-14 06:32:11.000000 vgd_counterfactuals-0.1.6/vgd_counterfactuals/generate/smiles_one_step_changes.py
+-rwxr-xr-x   0        0        0      997 2023-04-28 11:58:50.346682 vgd_counterfactuals-0.1.6/vgd_counterfactuals/templates/article.tex.j2
+-rw-r--r--   0        0        0      490 2023-05-01 15:26:26.262286 vgd_counterfactuals-0.1.6/vgd_counterfactuals/testing.py
+-rwxr-xr-x   0        0        0     5201 2023-05-01 15:30:16.327226 vgd_counterfactuals-0.1.6/vgd_counterfactuals/utils.py
+-rw-r--r--   0        0        0     3370 2023-05-01 16:09:36.020519 vgd_counterfactuals-0.1.6/vgd_counterfactuals/visualization.py
+-rw-r--r--   0        0        0     7622 1970-01-01 00:00:00.000000 vgd_counterfactuals-0.1.6/PKG-INFO
```

### Comparing `vgd_counterfactuals-0.1.5/LICENSE` & `vgd_counterfactuals-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.5/README.rst` & `vgd_counterfactuals-0.1.6/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
    :target: https://www.python.org/
    :alt: made with python
 
 .. |python-version| image:: https://img.shields.io/badge/Python-3.8.0-green.svg
    :target: https://www.python.org/
    :alt: python 3.8
 
-.. |version| image:: https://img.shields.io/badge/version-0.1.5-orange.svg
+.. |version| image:: https://img.shields.io/badge/version-0.1.6-orange.svg
    :target: https://www.python.org/
    :alt: version
 
 .. image:: banner.png
    :alt: banner image
 
 ===================
```

### Comparing `vgd_counterfactuals-0.1.5/banner.png` & `vgd_counterfactuals-0.1.6/banner.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.5/pyproject.toml` & `vgd_counterfactuals-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.2.0b2"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "vgd_counterfactuals"
-version = "0.1.5"
+version = "0.1.6"
 description = "Counterfactual explanations for GNNs based on the visual graph dataset format"
 license = "MIT license"
 authors = ["Jonas Teufel <jonseb1998@gmail.com>"]
 maintainers = ["Jonas Teufel <jonseb1998@gmail.com>"]
 readme = "README.rst"
 keywords = ["graph neural networks", "counterfactuals", "explainable AI"]
 packages = [
```

### Comparing `vgd_counterfactuals-0.1.5/vgd_counterfactuals/base.py` & `vgd_counterfactuals-0.1.6/vgd_counterfactuals/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,33 +46,36 @@
     DEFAULT_IMAGE_HEIGHT = 1000
 
     def __init__(self,
                  model,
                  processing: ProcessingBase,
                  neighborhood_func: t.Callable,
                  distance_func: t.Callable[[t.Any, t.Any], float],
+                 predict_func: t.Optional[t.Callable] = lambda model, graphs: model.predict_graphs(graphs),
                  logger: logging.Logger = NULL_LOGGER,
                  num_processes: t.Optional[int] = None,
                  batch_size: int = 5_000,
                  ):
         self.model = model
         self.processing = processing
         self.neighborhood_func = neighborhood_func
         self.distance_func = distance_func
+        self.predict_func = predict_func
         self.logger = logger
         self.num_processes = num_processes
         self.batch_size = batch_size
 
     def generate(self,
                  original: tv.DomainRepr,
                  path: str,
                  k_results: int = 5,
                  k_neighborhood: int = 1,
                  image_width: int = DEFAULT_IMAGE_WIDTH,
                  image_height: int = DEFAULT_IMAGE_HEIGHT,
+                 reverse: bool = False,
                  ) -> tv.VisGraphIndexDict:
         """
         Creates the ``k_results`` top counterfactuals for the prediction of the ``original`` element. The
         resulting top counterfactuals will be created as VGD elements into the folder given by the
         absolute ``path``.
 
         :param original: The domain-specific representation of the graph, for whose prediction results the
@@ -84,62 +87,56 @@
         :param k_neighborhood: The integer number of how large a graph edit neighborhood to explore. Default
             value is 1, in which case only the immediate neighbors (single edits) will be explored for
             possible counterfactuals. If this value would be 2, for example, the single-edit neighborhood
             of each of those neighbors would be explored as well.
             NOTE: Computational load rises exponentially, increasing this value is not encouraged.
         :param image_height: The integer width in pixels for the visualization images.
         :param image_width: The integer height in pixels for the visualization images.
+        :param reverse: A boolean flag which will reverse the distance function if set.
 
         :returns: The visual graph dataset index_data_map for the created VGD elements of all the
             generated counterfactuals.
         """
         # To be able to generate counterfactuals at all we first need to start from
         # the prediction of the original element. To get this prediction we first need
         # to convert the domain-specific representation into a GraphDict
         graph = self.processing.process(original)
         original_prediction = self.model.predict_graph(graph)
 
-        # Based on the original we need ALL possible neighbors of this in a k-neighborhood
-        # 16.05.23 - For a larger neighborhood size the number of counterfactuals increases exponentially
-        # and generating them takes forever. That is why we use multiprocessing to do the generation in
-        # parallel and hopefully be a bit faster.
-        neighbors_set = set([original])
-        if self.num_processes is not None:
-            with multiprocessing.Pool(processes=self.num_processes) as pool:
-                for i in range(k_neighborhood):
-                    neighbors_set = set(itertools.chain(*pool.map(self.neighborhood_func, neighbors_set)))
-        else:
-            for i in range(k_neighborhood):
-                neighbors = []
-                for value in neighbors_set:
-                    neighbors += self.neighborhood_func(value)
-                neighbors_set = neighbors_set.union(set(neighbors))
-
-        # This will be a list of the domain-spec. representations of all the generated neighbors of
-        # the original graph.
-        neighbors: t.List[tv.DomainRepr] = list(neighbors_set)
+        # 26.05.23 - Instead of having the implementation here, it is now in its own function which will
+        # return a list of all the valid k-edit neighbors.
+        # Moving this had two purposes: (1) it's cleaner code and (2) now I have the potential to cache
+        # the results, which I have realized is a functionality I'll need in the future.
+        neighbors: t.List[tv.DomainRepr] = self.get_neighbors(original, k_neighborhood)
         graphs = [self.processing.process(value) for value in neighbors]
 
         # 16.05.23 - I have noticed that for larger neighborhood sizes there can be A LOT of counterfactuals
         # so many that a model cannot possibly predict them all at once without causing a memory overflow
         # for the resulting vector. This is why we need to process this in a batched manner now!
         # NOTE: One might think that this could be parallelized as well, like the counterfactual generation
         # itself, but that would actually not work because we cant serialize the model to send it to another
         # process and loading the model from memory takes so long that it would not make sense to do that
         # in each process either.
         predictions = []
         for graph_batch in Batched(graphs, batch_size=self.batch_size):
-            predictions += self.model.predict_graphs(graph_batch)
+            # 26.05.2023 - Instead of calling "predict_graphs" directly, the way in which a model prediction
+            # is made is now further decoupled through a generic function "predict_func" that can be
+            # provided by the user, but which by default will still do the same thing and internally
+            # simply call "predict_graphs".
+            # This change was necessary, because I have realized that I needed to introduce the same
+            # decoupling to the web interface and this was the best solution to keep it consistent for
+            # the counterfactuals.
+            predictions += self.predict_func(self.model, graph_batch)
 
         distances = [self.distance_func(original_prediction, pred) for pred in predictions]
 
         sorted_results = sorted(
             zip(distances, neighbors, predictions, graphs),
             key=lambda tupl: tupl[0],  # sort by distance
-            reverse=True,  # sort in descending order
+            reverse=not reverse,  # sort in descending order by default
         )
         # If there are less neighbors in total than the desired number of results, we can only
         # provide as many as there are.
         num = min(len(sorted_results), k_results)
         top_results = sorted_results[:num]
 
         # For these top results we now want to create a visual graph dataset folder so that they can be
@@ -151,24 +148,44 @@
                 name=value,
                 output_path=path,
                 width=image_width,
                 height=image_height,
                 additional_metadata={
                     'distance': distance,
                     'prediction': prediction
-                }
+                },
+                additional_graph_data={},
             )
 
         metadata_map, index_data_map = load_visual_graph_dataset(
             path=path,
             logger=self.logger,
             log_step=10,
         )
         return index_data_map
 
+    def get_neighbors(self, original: tv.DomainRepr, k_neighborhood):
+        # Based on the original we need ALL possible neighbors of this in a k-neighborhood
+        # 16.05.23 - For a larger neighborhood size the number of counterfactuals increases exponentially
+        # and generating them takes forever. That is why we use multiprocessing to do the generation in
+        # parallel and hopefully be a bit faster.
+        neighbors_set = {original}
+        if self.num_processes is not None:
+            with multiprocessing.Pool(processes=self.num_processes) as pool:
+                for i in range(k_neighborhood):
+                    neighbors_set = set(itertools.chain(*pool.map(self.neighborhood_func, neighbors_set)))
+        else:
+            for i in range(k_neighborhood):
+                neighbors = []
+                for value in neighbors_set:
+                    neighbors += self.neighborhood_func(value)
+                neighbors_set = neighbors_set.union(set(neighbors))
+
+        return list(neighbors_set)
+
     def create(self,
                value: tv.DomainRepr,
                path: str,
                index: str,
                image_width=DEFAULT_IMAGE_WIDTH,
                image_height=DEFAULT_IMAGE_HEIGHT,
                ) -> tv.VgdElementDict:
```

### Comparing `vgd_counterfactuals-0.1.5/vgd_counterfactuals/cli.py` & `vgd_counterfactuals-0.1.6/vgd_counterfactuals/cli.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/00_quickstart.py` & `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/00_quickstart.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/01_visualization.py` & `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/01_visualization.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/analysis.py` & `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/analysis.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/code.py` & `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/code.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.json` & `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.png` & `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.json` & `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.png` & `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.json` & `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.png` & `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.json` & `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.png` & `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.json` & `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.png` & `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.json` & `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.png` & `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.json` & `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.png` & `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.json` & `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.png` & `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.json` & `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.png` & `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.json` & `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.png` & `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.json` & `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.png` & `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals.pdf` & `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals.pdf`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_meta.json` & `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_meta.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_out.log` & `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_out.log`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.5/vgd_counterfactuals/experiments/README.rst` & `vgd_counterfactuals-0.1.6/vgd_counterfactuals/experiments/README.rst`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.5/vgd_counterfactuals/experiments/template_experiment.py` & `vgd_counterfactuals-0.1.6/vgd_counterfactuals/experiments/template_experiment.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.5/vgd_counterfactuals/experiments/template_experiment_sub.py` & `vgd_counterfactuals-0.1.6/vgd_counterfactuals/experiments/template_experiment_sub.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.5/vgd_counterfactuals/generate/__pycache__/molecules.cpython-310.pyc` & `vgd_counterfactuals-0.1.6/vgd_counterfactuals/generate/__pycache__/molecules.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.5/vgd_counterfactuals/generate/molecules.py` & `vgd_counterfactuals-0.1.6/vgd_counterfactuals/generate/molecules.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.5/vgd_counterfactuals/generate/smiles_one_step_changes.py` & `vgd_counterfactuals-0.1.6/vgd_counterfactuals/generate/smiles_one_step_changes.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.5/vgd_counterfactuals/templates/article.tex.j2` & `vgd_counterfactuals-0.1.6/vgd_counterfactuals/templates/article.tex.j2`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.5/vgd_counterfactuals/utils.py` & `vgd_counterfactuals-0.1.6/vgd_counterfactuals/utils.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.5/vgd_counterfactuals/visualization.py` & `vgd_counterfactuals-0.1.6/vgd_counterfactuals/visualization.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.5/PKG-INFO` & `vgd_counterfactuals-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vgd-counterfactuals
-Version: 0.1.5
+Version: 0.1.6
 Summary: Counterfactual explanations for GNNs based on the visual graph dataset format
 License: MIT
 Keywords: graph neural networks,counterfactuals,explainable AI
 Author: Jonas Teufel
 Author-email: jonseb1998@gmail.com
 Maintainer: Jonas Teufel
 Maintainer-email: jonseb1998@gmail.com
@@ -32,15 +32,15 @@
    :target: https://www.python.org/
    :alt: made with python
 
 .. |python-version| image:: https://img.shields.io/badge/Python-3.8.0-green.svg
    :target: https://www.python.org/
    :alt: python 3.8
 
-.. |version| image:: https://img.shields.io/badge/version-0.1.5-orange.svg
+.. |version| image:: https://img.shields.io/badge/version-0.1.6-orange.svg
    :target: https://www.python.org/
    :alt: version
 
 .. image:: banner.png
    :alt: banner image
 
 ===================
```

