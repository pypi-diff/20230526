# Comparing `tmp/vgd_counterfactuals-0.1.4.tar.gz` & `tmp/vgd_counterfactuals-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vgd_counterfactuals-0.1.4.tar", max compression
+gzip compressed data, was "vgd_counterfactuals-0.1.5.tar", max compression
```

## Comparing `vgd_counterfactuals-0.1.4.tar` & `vgd_counterfactuals-0.1.5.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rwxr-xr-x   0        0        0     1070 2023-04-28 11:58:50.318682 vgd_counterfactuals-0.1.4/LICENSE
--rwxr-xr-x   0        0        0     6577 2023-05-19 11:40:29.896952 vgd_counterfactuals-0.1.4/README.rst
--rw-r--r--   0        0        0    75715 2023-04-30 10:49:40.133365 vgd_counterfactuals-0.1.4/banner.png
--rwxr-xr-x   0        0        0     1514 2023-05-19 11:40:29.888952 vgd_counterfactuals-0.1.4/pyproject.toml
--rwxr-xr-x   0        0        0        5 2023-05-19 11:40:29.896952 vgd_counterfactuals-0.1.4/vgd_counterfactuals/VERSION
--rwxr-xr-x   0        0        0       39 2023-04-30 10:06:54.410920 vgd_counterfactuals-0.1.4/vgd_counterfactuals/__init__.py
--rw-r--r--   0        0        0    10221 2023-05-16 07:28:31.190627 vgd_counterfactuals-0.1.4/vgd_counterfactuals/base.py
--rwxr-xr-x   0        0        0     5290 2023-04-28 11:58:50.338682 vgd_counterfactuals-0.1.4/vgd_counterfactuals/cli.py
--rw-r--r--   0        0        0     1950 2023-05-01 15:19:29.825180 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/00_quickstart.py
--rw-r--r--   0        0        0     3422 2023-05-01 15:37:09.041204 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/01_visualization.py
--rw-r--r--   0        0        0      471 2023-05-01 15:26:26.262286 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/README.rst
--rw-r--r--   0        0        0        0 2023-05-01 14:39:31.031283 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/__init__.py
--rw-r--r--   0        0        0      847 2023-05-01 15:19:38.033191 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/analysis.py
--rw-r--r--   0        0        0     2191 2023-05-01 15:19:38.025191 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/code.py
--rw-r--r--   0        0        0      778 2023-05-01 15:19:39.289193 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.json
--rw-r--r--   0        0        0    17914 2023-05-01 15:19:39.289193 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.png
--rw-r--r--   0        0        0      968 2023-05-01 15:19:38.169191 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.json
--rw-r--r--   0        0        0    17705 2023-05-01 15:19:38.169191 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.png
--rw-r--r--   0        0        0      968 2023-05-01 15:19:38.281191 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.json
--rw-r--r--   0        0        0    18723 2023-05-01 15:19:38.281191 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.png
--rw-r--r--   0        0        0      975 2023-05-01 15:19:38.393192 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.json
--rw-r--r--   0        0        0    19578 2023-05-01 15:19:38.393192 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.png
--rw-r--r--   0        0        0      974 2023-05-01 15:19:38.501192 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.json
--rw-r--r--   0        0        0    18471 2023-05-01 15:19:38.501192 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.png
--rw-r--r--   0        0        0      972 2023-05-01 15:19:38.617192 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.json
--rw-r--r--   0        0        0    19414 2023-05-01 15:19:38.617192 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.png
--rw-r--r--   0        0        0      978 2023-05-01 15:19:38.729192 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.json
--rw-r--r--   0        0        0    20003 2023-05-01 15:19:38.729192 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.png
--rw-r--r--   0        0        0      971 2023-05-01 15:19:38.841192 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.json
--rw-r--r--   0        0        0    23908 2023-05-01 15:19:38.841192 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.png
--rw-r--r--   0        0        0      970 2023-05-01 15:19:38.953192 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.json
--rw-r--r--   0        0        0    19642 2023-05-01 15:19:38.953192 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.png
--rw-r--r--   0        0        0      977 2023-05-01 15:19:39.065193 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.json
--rw-r--r--   0        0        0    19682 2023-05-01 15:19:39.065193 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.png
--rw-r--r--   0        0        0      969 2023-05-01 15:19:39.177193 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.json
--rw-r--r--   0        0        0    20380 2023-05-01 15:19:39.177193 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.png
--rw-r--r--   0        0        0   221293 2023-05-01 15:19:40.353194 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals.pdf
--rw-r--r--   0        0        0        2 2023-05-01 15:19:40.353194 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_data.json
--rw-r--r--   0        0        0      555 2023-05-01 15:19:40.353194 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_meta.json
--rw-r--r--   0        0        0     1328 2023-05-01 15:19:40.357194 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_out.log
--rw-r--r--   0        0        0     1334 2023-04-28 11:58:50.342682 vgd_counterfactuals-0.1.4/vgd_counterfactuals/experiments/README.rst
--rw-r--r--   0        0        0      209 2023-04-28 11:58:50.346682 vgd_counterfactuals-0.1.4/vgd_counterfactuals/experiments/results/README.rst
--rwxr-xr-x   0        0        0      729 2023-04-28 11:58:50.342682 vgd_counterfactuals-0.1.4/vgd_counterfactuals/experiments/template_experiment.py
--rw-r--r--   0        0        0      614 2023-04-28 11:58:50.342682 vgd_counterfactuals-0.1.4/vgd_counterfactuals/experiments/template_experiment_sub.py
--rw-r--r--   0        0        0        0 2023-04-28 12:00:41.971495 vgd_counterfactuals-0.1.4/vgd_counterfactuals/generate/__init__.py
--rw-r--r--   0        0        0      176 2023-04-30 07:11:09.422132 vgd_counterfactuals-0.1.4/vgd_counterfactuals/generate/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     6996 2023-05-19 08:56:41.054361 vgd_counterfactuals-0.1.4/vgd_counterfactuals/generate/__pycache__/molecules.cpython-310.pyc
--rw-r--r--   0        0        0     9753 2023-05-19 08:57:53.758885 vgd_counterfactuals-0.1.4/vgd_counterfactuals/generate/molecules.py
--rwxr-xr-x   0        0        0    19773 2023-04-14 06:32:11.000000 vgd_counterfactuals-0.1.4/vgd_counterfactuals/generate/smiles_one_step_changes.py
--rwxr-xr-x   0        0        0      997 2023-04-28 11:58:50.346682 vgd_counterfactuals-0.1.4/vgd_counterfactuals/templates/article.tex.j2
--rw-r--r--   0        0        0      490 2023-05-01 15:26:26.262286 vgd_counterfactuals-0.1.4/vgd_counterfactuals/testing.py
--rwxr-xr-x   0        0        0     5201 2023-05-01 15:30:16.327226 vgd_counterfactuals-0.1.4/vgd_counterfactuals/utils.py
--rw-r--r--   0        0        0     3370 2023-05-01 16:09:36.020519 vgd_counterfactuals-0.1.4/vgd_counterfactuals/visualization.py
--rw-r--r--   0        0        0     7622 1970-01-01 00:00:00.000000 vgd_counterfactuals-0.1.4/PKG-INFO
+-rwxr-xr-x   0        0        0     1070 2023-04-28 11:58:50.318682 vgd_counterfactuals-0.1.5/LICENSE
+-rwxr-xr-x   0        0        0     6577 2023-05-26 08:35:07.821730 vgd_counterfactuals-0.1.5/README.rst
+-rw-r--r--   0        0        0    75715 2023-04-30 10:49:40.133365 vgd_counterfactuals-0.1.5/banner.png
+-rwxr-xr-x   0        0        0     1514 2023-05-26 08:35:07.801729 vgd_counterfactuals-0.1.5/pyproject.toml
+-rwxr-xr-x   0        0        0        5 2023-05-26 08:35:07.821730 vgd_counterfactuals-0.1.5/vgd_counterfactuals/VERSION
+-rwxr-xr-x   0        0        0       39 2023-04-30 10:06:54.410920 vgd_counterfactuals-0.1.5/vgd_counterfactuals/__init__.py
+-rw-r--r--   0        0        0    10551 2023-05-26 08:35:02.917681 vgd_counterfactuals-0.1.5/vgd_counterfactuals/base.py
+-rwxr-xr-x   0        0        0     5290 2023-04-28 11:58:50.338682 vgd_counterfactuals-0.1.5/vgd_counterfactuals/cli.py
+-rw-r--r--   0        0        0     1950 2023-05-01 15:19:29.825180 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/00_quickstart.py
+-rw-r--r--   0        0        0     3422 2023-05-01 15:37:09.041204 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/01_visualization.py
+-rw-r--r--   0        0        0      471 2023-05-01 15:26:26.262286 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/README.rst
+-rw-r--r--   0        0        0        0 2023-05-01 14:39:31.031283 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/__init__.py
+-rw-r--r--   0        0        0      847 2023-05-01 15:19:38.033191 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/analysis.py
+-rw-r--r--   0        0        0     2191 2023-05-01 15:19:38.025191 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/code.py
+-rw-r--r--   0        0        0      778 2023-05-01 15:19:39.289193 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.json
+-rw-r--r--   0        0        0    17914 2023-05-01 15:19:39.289193 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.png
+-rw-r--r--   0        0        0      968 2023-05-01 15:19:38.169191 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.json
+-rw-r--r--   0        0        0    17705 2023-05-01 15:19:38.169191 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.png
+-rw-r--r--   0        0        0      968 2023-05-01 15:19:38.281191 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.json
+-rw-r--r--   0        0        0    18723 2023-05-01 15:19:38.281191 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.png
+-rw-r--r--   0        0        0      975 2023-05-01 15:19:38.393192 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.json
+-rw-r--r--   0        0        0    19578 2023-05-01 15:19:38.393192 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.png
+-rw-r--r--   0        0        0      974 2023-05-01 15:19:38.501192 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.json
+-rw-r--r--   0        0        0    18471 2023-05-01 15:19:38.501192 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.png
+-rw-r--r--   0        0        0      972 2023-05-01 15:19:38.617192 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.json
+-rw-r--r--   0        0        0    19414 2023-05-01 15:19:38.617192 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.png
+-rw-r--r--   0        0        0      978 2023-05-01 15:19:38.729192 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.json
+-rw-r--r--   0        0        0    20003 2023-05-01 15:19:38.729192 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.png
+-rw-r--r--   0        0        0      971 2023-05-01 15:19:38.841192 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.json
+-rw-r--r--   0        0        0    23908 2023-05-01 15:19:38.841192 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.png
+-rw-r--r--   0        0        0      970 2023-05-01 15:19:38.953192 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.json
+-rw-r--r--   0        0        0    19642 2023-05-01 15:19:38.953192 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.png
+-rw-r--r--   0        0        0      977 2023-05-01 15:19:39.065193 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.json
+-rw-r--r--   0        0        0    19682 2023-05-01 15:19:39.065193 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.png
+-rw-r--r--   0        0        0      969 2023-05-01 15:19:39.177193 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.json
+-rw-r--r--   0        0        0    20380 2023-05-01 15:19:39.177193 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.png
+-rw-r--r--   0        0        0   221293 2023-05-01 15:19:40.353194 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals.pdf
+-rw-r--r--   0        0        0        2 2023-05-01 15:19:40.353194 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_data.json
+-rw-r--r--   0        0        0      555 2023-05-01 15:19:40.353194 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_meta.json
+-rw-r--r--   0        0        0     1328 2023-05-01 15:19:40.357194 vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_out.log
+-rw-r--r--   0        0        0     1334 2023-04-28 11:58:50.342682 vgd_counterfactuals-0.1.5/vgd_counterfactuals/experiments/README.rst
+-rw-r--r--   0        0        0      209 2023-04-28 11:58:50.346682 vgd_counterfactuals-0.1.5/vgd_counterfactuals/experiments/results/README.rst
+-rwxr-xr-x   0        0        0      729 2023-04-28 11:58:50.342682 vgd_counterfactuals-0.1.5/vgd_counterfactuals/experiments/template_experiment.py
+-rw-r--r--   0        0        0      614 2023-04-28 11:58:50.342682 vgd_counterfactuals-0.1.5/vgd_counterfactuals/experiments/template_experiment_sub.py
+-rw-r--r--   0        0        0        0 2023-04-28 12:00:41.971495 vgd_counterfactuals-0.1.5/vgd_counterfactuals/generate/__init__.py
+-rw-r--r--   0        0        0      176 2023-04-30 07:11:09.422132 vgd_counterfactuals-0.1.5/vgd_counterfactuals/generate/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     8355 2023-05-26 08:30:52.863182 vgd_counterfactuals-0.1.5/vgd_counterfactuals/generate/__pycache__/molecules.cpython-310.pyc
+-rw-r--r--   0        0        0    11111 2023-05-26 08:30:51.243165 vgd_counterfactuals-0.1.5/vgd_counterfactuals/generate/molecules.py
+-rwxr-xr-x   0        0        0    19773 2023-04-14 06:32:11.000000 vgd_counterfactuals-0.1.5/vgd_counterfactuals/generate/smiles_one_step_changes.py
+-rwxr-xr-x   0        0        0      997 2023-04-28 11:58:50.346682 vgd_counterfactuals-0.1.5/vgd_counterfactuals/templates/article.tex.j2
+-rw-r--r--   0        0        0      490 2023-05-01 15:26:26.262286 vgd_counterfactuals-0.1.5/vgd_counterfactuals/testing.py
+-rwxr-xr-x   0        0        0     5201 2023-05-01 15:30:16.327226 vgd_counterfactuals-0.1.5/vgd_counterfactuals/utils.py
+-rw-r--r--   0        0        0     3370 2023-05-01 16:09:36.020519 vgd_counterfactuals-0.1.5/vgd_counterfactuals/visualization.py
+-rw-r--r--   0        0        0     7622 1970-01-01 00:00:00.000000 vgd_counterfactuals-0.1.5/PKG-INFO
```

### Comparing `vgd_counterfactuals-0.1.4/LICENSE` & `vgd_counterfactuals-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.4/README.rst` & `vgd_counterfactuals-0.1.5/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
    :target: https://www.python.org/
    :alt: made with python
 
 .. |python-version| image:: https://img.shields.io/badge/Python-3.8.0-green.svg
    :target: https://www.python.org/
    :alt: python 3.8
 
-.. |version| image:: https://img.shields.io/badge/version-0.1.4-orange.svg
+.. |version| image:: https://img.shields.io/badge/version-0.1.5-orange.svg
    :target: https://www.python.org/
    :alt: version
 
 .. image:: banner.png
    :alt: banner image
 
 ===================
```

### Comparing `vgd_counterfactuals-0.1.4/banner.png` & `vgd_counterfactuals-0.1.5/banner.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.4/pyproject.toml` & `vgd_counterfactuals-0.1.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.2.0b2"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "vgd_counterfactuals"
-version = "0.1.4"
+version = "0.1.5"
 description = "Counterfactual explanations for GNNs based on the visual graph dataset format"
 license = "MIT license"
 authors = ["Jonas Teufel <jonseb1998@gmail.com>"]
 maintainers = ["Jonas Teufel <jonseb1998@gmail.com>"]
 readme = "README.rst"
 keywords = ["graph neural networks", "counterfactuals", "explainable AI"]
 packages = [
```

### Comparing `vgd_counterfactuals-0.1.4/vgd_counterfactuals/base.py` & `vgd_counterfactuals-0.1.5/vgd_counterfactuals/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
     def __init__(self,
                  model,
                  processing: ProcessingBase,
                  neighborhood_func: t.Callable,
                  distance_func: t.Callable[[t.Any, t.Any], float],
                  logger: logging.Logger = NULL_LOGGER,
-                 num_processes: int = 2,
+                 num_processes: t.Optional[int] = None,
                  batch_size: int = 5_000,
                  ):
         self.model = model
         self.processing = processing
         self.neighborhood_func = neighborhood_func
         self.distance_func = distance_func
         self.logger = logger
@@ -98,18 +98,25 @@
         graph = self.processing.process(original)
         original_prediction = self.model.predict_graph(graph)
 
         # Based on the original we need ALL possible neighbors of this in a k-neighborhood
         # 16.05.23 - For a larger neighborhood size the number of counterfactuals increases exponentially
         # and generating them takes forever. That is why we use multiprocessing to do the generation in
         # parallel and hopefully be a bit faster.
-        with multiprocessing.Pool(processes=self.num_processes) as pool:
-            neighbors_set = set([original])
+        neighbors_set = set([original])
+        if self.num_processes is not None:
+            with multiprocessing.Pool(processes=self.num_processes) as pool:
+                for i in range(k_neighborhood):
+                    neighbors_set = set(itertools.chain(*pool.map(self.neighborhood_func, neighbors_set)))
+        else:
             for i in range(k_neighborhood):
-                neighbors_set = set(itertools.chain(*pool.map(self.neighborhood_func, neighbors_set)))
+                neighbors = []
+                for value in neighbors_set:
+                    neighbors += self.neighborhood_func(value)
+                neighbors_set = neighbors_set.union(set(neighbors))
 
         # This will be a list of the domain-spec. representations of all the generated neighbors of
         # the original graph.
         neighbors: t.List[tv.DomainRepr] = list(neighbors_set)
         graphs = [self.processing.process(value) for value in neighbors]
 
         # 16.05.23 - I have noticed that for larger neighborhood sizes there can be A LOT of counterfactuals
```

### Comparing `vgd_counterfactuals-0.1.4/vgd_counterfactuals/cli.py` & `vgd_counterfactuals-0.1.5/vgd_counterfactuals/cli.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/00_quickstart.py` & `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/00_quickstart.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/01_visualization.py` & `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/01_visualization.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/analysis.py` & `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/analysis.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/code.py` & `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/code.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.json` & `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.png` & `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.json` & `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.png` & `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.json` & `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.png` & `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.json` & `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.png` & `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.json` & `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.png` & `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.json` & `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.png` & `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.json` & `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.png` & `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.json` & `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.png` & `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.json` & `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.png` & `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.json` & `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.png` & `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.json` & `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.png` & `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals.pdf` & `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals.pdf`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_meta.json` & `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_meta.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_out.log` & `vgd_counterfactuals-0.1.5/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_out.log`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.4/vgd_counterfactuals/experiments/README.rst` & `vgd_counterfactuals-0.1.5/vgd_counterfactuals/experiments/README.rst`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.4/vgd_counterfactuals/experiments/template_experiment.py` & `vgd_counterfactuals-0.1.5/vgd_counterfactuals/experiments/template_experiment.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.4/vgd_counterfactuals/experiments/template_experiment_sub.py` & `vgd_counterfactuals-0.1.5/vgd_counterfactuals/experiments/template_experiment_sub.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.4/vgd_counterfactuals/generate/__pycache__/molecules.cpython-310.pyc` & `vgd_counterfactuals-0.1.5/vgd_counterfactuals/generate/__pycache__/molecules.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri May 19 08:56:40 2023 UTC, .py size: 9777 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,438 +1,523 @@
-00000000: 6f0d 0d0a 0000 0000 c839 6764 3126 0000  o........9gd1&..
+00000000: 6f0d 0d0a 0000 0000 3b6e 7064 672b 0000  o.......;npdg+..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0009 0000 0040 0000 0073 4201 0000 6400  .....@...sB...d.
+00000020: 000b 0000 0040 0000 0073 8601 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
-00000050: 6d06 5a06 0100 6404 6405 6406 6407 6408  m.Z...d.d.d.d.d.
-00000060: 6406 6409 9c06 5a07 6423 640b 6504 6a08  d.d...Z.d#d.e.j.
-00000070: 640c 6509 6604 640d 640e 8405 5a0a 6424  d.e.f.d.d...Z.d$
-00000080: 640b 6504 6a08 640c 6509 6604 6410 6411  d.e.j.d.e.f.d.d.
-00000090: 8405 5a0b 6507 650a 650b 6602 6602 6412  ..Z.e.e.e.f.f.d.
-000000a0: 6509 6413 6502 6a0c 6502 6a0d 6504 6a08  e.d.e.j.e.j.e.j.
-000000b0: 6701 650e 6602 1900 1900 6414 6502 6a0f  g.e.f.....d.e.j.
-000000c0: 6509 1900 6606 6415 6416 8405 5a10 6425  e...f.d.d...Z.d%
-000000d0: 640b 6504 6a08 6418 6511 6414 6512 6606  d.e.j.d.e.d.e.f.
-000000e0: 6419 641a 8405 5a13 640b 6504 6a08 641b  d.d...Z.d.e.j.d.
-000000f0: 6502 6a14 6509 6511 6602 1900 641c 6502  e.j.e.e.f...d.e.
-00000100: 6a14 6511 6502 6a0f 6511 1900 6602 1900  j.e.e.j.e...f...
-00000110: 6414 6502 6a15 6509 1900 6608 641d 641e  d.e.j.e...f.d.d.
-00000120: 8404 5a16 640b 6504 6a08 641c 6502 6a14  ..Z.d.e.j.d.e.j.
-00000130: 6511 6502 6a0f 6511 1900 6602 1900 6414  e.e.j.e...f...d.
-00000140: 6502 6a15 6509 1900 6606 641f 6420 8404  e.j.e...f.d.d ..
-00000150: 5a17 640b 6504 6a08 6414 6502 6a15 6509  Z.d.e.j.d.e.j.e.
-00000160: 1900 6604 6421 6422 8404 5a18 6401 5300  ..f.d!d"..Z.d.S.
-00000170: 2926 e900 0000 004e 2901 da04 4368 656d  )&.....N)...Chem
-00000180: 2901 da0b 696e 7665 7274 5f64 6963 74e9  )...invert_dict.
-00000190: 0400 0000 e905 0000 00e9 0600 0000 e901  ................
-000001a0: 0000 00e9 0700 0000 2906 da01 43da 014e  ........)...C..N
-000001b0: da01 4fda 0146 da02 436c da01 53fa 0e2a  ..O..F..Cl..S..*
-000001c0: 313d 2a2a 323d 2a2a 3d2a 312a 32da 036d  1=**2=**=*1*2..m
-000001d0: 6f6c da07 7061 7474 6572 6e63 0200 0000  ol..patternc....
-000001e0: 0000 0000 0000 0000 0400 0000 0300 0000  ................
-000001f0: 4300 0000 f318 0000 0074 00a0 017c 01a1  C........t...|..
-00000200: 017d 027c 00a0 027c 02a1 017d 037c 0353  .}.|...|...}.|.S
-00000210: 0029 017a 830a 2020 2020 4368 6563 6b73  .).z..    Checks
-00000220: 2069 6620 7468 6520 6769 7665 6e20 6d6f   if the given mo
-00000230: 6c65 6375 6c65 2060 606d 6f6c 6060 2069  lecule ``mol`` i
-00000240: 7320 6120 6272 6964 6765 2068 6561 6420  s a bridge head 
-00000250: 6361 7262 6f6e 2073 7472 7563 7475 7265  carbon structure
-00000260: 2077 6869 6368 2061 7070 6172 656e 746c   which apparentl
-00000270: 7920 646f 6573 206e 6f74 0a20 2020 2061  y does not.    a
-00000280: 7070 6561 7220 696e 2063 6865 6d69 7374  ppear in chemist
-00000290: 7279 2e0a 2020 2020 a903 7202 0000 00da  ry..    ..r.....
-000002a0: 0d4d 6f6c 4672 6f6d 536d 6172 7473 da11  .MolFromSmarts..
-000002b0: 4861 7353 7562 7374 7275 6374 4d61 7463  HasSubstructMatc
-000002c0: 68a9 0472 1000 0000 7211 0000 00da 0673  h..r....r......s
-000002d0: 6d61 7274 73da 0869 735f 6d61 7463 68a9  marts..is_match.
-000002e0: 0072 1900 0000 fa54 2f6d 6564 6961 2f73  .r.....T/media/s
-000002f0: 7364 2f50 726f 6772 616d 6d69 6e67 2f76  sd/Programming/v
-00000300: 6764 5f63 6f75 6e74 6572 6661 6374 7561  gd_counterfactua
-00000310: 6c73 2f76 6764 5f63 6f75 6e74 6572 6661  ls/vgd_counterfa
-00000320: 6374 7561 6c73 2f67 656e 6572 6174 652f  ctuals/generate/
-00000330: 6d6f 6c65 6375 6c65 732e 7079 da15 6973  molecules.py..is
-00000340: 5f62 7269 6467 655f 6865 6164 5f63 6172  _bridge_head_car
-00000350: 626f 6e14 0000 0073 0600 0000 0a05 0a01  bon....s........
-00000360: 0401 721b 0000 00da 0353 4e4e 6302 0000  ..r......SNNc...
-00000370: 0000 0000 0000 0000 0004 0000 0003 0000  ................
-00000380: 0043 0000 0072 1200 0000 2901 4e72 1300  .C...r....).Nr..
-00000390: 0000 7216 0000 0072 1900 0000 7219 0000  ..r....r....r...
-000003a0: 0072 1a00 0000 da1b 6973 5f6e 6974 726f  .r......is_nitro
-000003b0: 6765 6e5f 6e69 7472 6f67 656e 5f73 756c  gen_nitrogen_sul
-000003c0: 6675 721e 0000 0073 0600 0000 0a01 0a01  fur....s........
-000003d0: 0401 721d 0000 00da 0673 6d69 6c65 73da  ..r......smiles.
-000003e0: 0b6d 6f6c 5f66 696c 7465 7273 da06 7265  .mol_filters..re
-000003f0: 7475 726e 6303 0000 0000 0000 0000 0000  turnc...........
-00000400: 0006 0000 0007 0000 0003 0000 0073 9400  .............s..
-00000410: 0000 7400 8300 7d03 7401 a002 7c00 a101  ..t...}.t...|...
-00000420: 8900 7403 8800 8301 7d04 7c03 a004 7405  ..t.....}.|...t.
-00000430: 8800 7c01 7c04 6401 8d03 a101 0100 7c03  ..|.|.d.......|.
-00000440: a004 7406 8800 7c04 6402 8d02 a101 0100  ..t...|.d.......
-00000450: 7c03 a004 7407 8800 6403 8d01 a101 0100  |...t...d.......
-00000460: 6700 7d05 7c03 4400 5d1c 7d00 7401 a002  g.}.|.D.].}.t...
-00000470: 7c00 a101 8900 7408 8700 6601 6404 6405  |.....t...f.d.d.
-00000480: 8408 7c02 4400 8301 8301 7242 7409 6406  ..|.D.....rBt.d.
-00000490: 8301 0100 712b 7c05 a00a 7c00 a101 0100  ....q+|...|.....
-000004a0: 712b 7c05 5300 2907 61b1 0300 000a 2020  q+|.S.).a.....  
-000004b0: 2020 4769 7665 6e20 6120 6060 736d 696c    Given a ``smil
-000004c0: 6573 6060 2072 6570 7265 7365 6e74 6174  es`` representat
-000004d0: 696f 6e20 6f66 2061 206d 6f6c 6563 756c  ion of a molecul
-000004e0: 652c 2074 6869 7320 6675 6e63 7469 6f6e  e, this function
-000004f0: 2077 696c 6c20 7265 7475 726e 2061 206c   will return a l
-00000500: 6973 7420 6f66 2074 6865 2053 4d49 4c45  ist of the SMILE
-00000510: 530a 2020 2020 7265 7072 6573 656e 7461  S.    representa
-00000520: 7469 6f6e 7320 6f66 2061 6c6c 2074 6865  tions of all the
-00000530: 2076 616c 6964 206d 6f6c 6563 756c 6573   valid molecules
-00000540: 2077 6974 6869 6e20 6120 312d 6564 6974   within a 1-edit
-00000550: 206e 6569 6768 626f 7268 6f6f 642e 204f   neighborhood. O
-00000560: 7074 696f 6e61 6c6c 792c 2061 206c 6973  ptionally, a lis
-00000570: 7420 6f66 2062 6f6f 6c65 616e 0a20 2020  t of boolean.   
-00000580: 2066 756e 6374 696f 6e73 2063 616e 2062   functions can b
-00000590: 6520 7072 6f76 6964 6564 2066 6f72 2060  e provided for `
-000005a0: 606d 6f6c 5f66 696c 7465 7273 6060 2074  `mol_filters`` t
-000005b0: 6f20 6675 7274 6865 7220 6c69 6d69 7420  o further limit 
-000005c0: 7468 6520 6b69 6e64 7320 6f66 206d 6f6c  the kinds of mol
-000005d0: 6563 756c 6573 2069 6e63 6c75 6465 6420  ecules included 
-000005e0: 696e 2074 6865 0a20 2020 2072 6573 756c  in the.    resul
-000005f0: 742e 0a0a 2020 2020 3a70 6172 616d 2073  t...    :param s
-00000600: 6d69 6c65 733a 2054 6865 2053 4d49 4c45  miles: The SMILE
-00000610: 5320 7374 7269 6e67 2072 6570 7265 7365  S string represe
-00000620: 6e74 6174 696f 6e20 6f66 0a20 2020 203a  ntation of.    :
-00000630: 7061 7261 6d20 6174 6f6d 5f76 616c 656e  param atom_valen
-00000640: 6365 5f6d 6170 3a20 4120 6469 6374 696f  ce_map: A dictio
-00000650: 6e61 7279 2c20 7768 6f73 6520 6b65 7973  nary, whose keys
-00000660: 2061 7265 2073 7472 696e 6773 2074 6861   are strings tha
-00000670: 7420 6964 656e 7469 6679 2061 746f 6d20  t identify atom 
-00000680: 7479 7065 7320 6f66 2074 6865 2053 4d49  types of the SMI
-00000690: 4c45 530a 2020 2020 2020 2020 6e6f 7461  LES.        nota
-000006a0: 7469 6f6e 2028 4f2c 204e 2c20 436c 202e  tion (O, N, Cl .
-000006b0: 2e2e 2920 616e 6420 7468 6520 7661 6c75  ..) and the valu
-000006c0: 6573 2061 7265 2074 6865 2069 6e74 6567  es are the integ
-000006d0: 6572 2076 616c 656e 6365 206f 6620 7468  er valence of th
-000006e0: 6520 636f 7272 6573 706f 6e64 696e 6720  e corresponding 
-000006f0: 6174 6f6d 2e20 4f6e 6c79 0a20 2020 2020  atom. Only.     
-00000700: 2020 2061 746f 6d73 2074 6861 7420 6172     atoms that ar
-00000710: 6520 6c69 7374 6564 2069 6e20 7468 6973  e listed in this
-00000720: 2064 6963 7420 7769 6c6c 2062 6520 636f   dict will be co
-00000730: 6e73 6964 6572 6564 2066 6f72 2065 6469  nsidered for edi
-00000740: 7420 6f70 6572 6174 696f 6e73 2073 7563  t operations suc
-00000750: 6820 6173 2061 6464 696e 6720 6f72 0a20  h as adding or. 
-00000760: 2020 2020 2020 2072 6570 6c61 6369 6e67         replacing
-00000770: 2061 6e64 2061 746f 6d21 0a20 2020 203a   and atom!.    :
-00000780: 7061 7261 6d20 6d6f 6c5f 6669 6c74 6572  param mol_filter
-00000790: 733a 2041 206c 6973 7420 6f66 2066 756e  s: A list of fun
-000007a0: 6374 696f 6e73 2077 6869 6368 2065 6163  ctions which eac
-000007b0: 6820 7461 6b65 2061 204d 6f6c 206f 626a  h take a Mol obj
-000007c0: 6563 7420 6173 2069 6e70 7574 2061 6e64  ect as input and
-000007d0: 2072 6574 7572 6e20 6120 626f 6f6c 6561   return a boolea
-000007e0: 6e20 7661 6c75 650a 2020 2020 2020 2020  n value.        
-000007f0: 746f 2064 6574 6572 6d69 6e65 2077 6865  to determine whe
-00000800: 7468 6572 2074 6861 7420 6174 6f6d 2073  ther that atom s
-00000810: 686f 756c 6420 6265 2065 7863 6c75 6465  hould be exclude
-00000820: 6420 2854 7275 6529 206f 7220 6e6f 7420  d (True) or not 
-00000830: 2846 616c 7365 292e 0a0a 2020 2020 3a72  (False)...    :r
-00000840: 6574 7572 6e73 3a20 4120 6c69 7374 206f  eturns: A list o
-00000850: 6620 7374 7269 6e67 730a 2020 2020 2903  f strings.    ).
-00000860: 7210 0000 00da 1061 746f 6d5f 7661 6c65  r......atom_vale
-00000870: 6e63 655f 6d61 70da 1866 7265 655f 7661  nce_map..free_va
-00000880: 6c65 6e63 655f 696e 6469 6365 735f 6d61  lence_indices_ma
-00000890: 7029 0272 1000 0000 7222 0000 00a9 0172  p).r....r".....r
-000008a0: 1000 0000 6301 0000 0000 0000 0000 0000  ....c...........
-000008b0: 0002 0000 0004 0000 0013 0000 0073 1400  .............s..
-000008c0: 0000 6700 7c00 5d06 7d01 7c01 8800 8301  ..g.|.].}.|.....
-000008d0: 9102 7102 5300 7219 0000 0072 1900 0000  ..q.S.r....r....
-000008e0: 2902 da02 2e30 da04 6675 6e63 7223 0000  )....0..funcr#..
-000008f0: 0072 1900 0000 721a 0000 00da 0a3c 6c69  .r....r......<li
-00000900: 7374 636f 6d70 3e56 0000 0073 0200 0000  stcomp>V...s....
-00000910: 1400 7a24 6765 745f 6e65 6967 6862 6f72  ..z$get_neighbor
-00000920: 686f 6f64 2e3c 6c6f 6361 6c73 3e2e 3c6c  hood.<locals>.<l
-00000930: 6973 7463 6f6d 703e 5429 0bda 0373 6574  istcomp>T)...set
-00000940: 7202 0000 00da 0d4d 6f6c 4672 6f6d 536d  r......MolFromSm
-00000950: 696c 6573 da14 6765 745f 6672 6565 5f76  iles..get_free_v
-00000960: 616c 656e 6365 5f6d 6170 da06 7570 6461  alence_map..upda
-00000970: 7465 da18 6765 745f 7661 6c69 645f 6174  te..get_valid_at
-00000980: 6f6d 5f61 6464 6974 696f 6e73 da18 6765  om_additions..ge
-00000990: 745f 7661 6c69 645f 626f 6e64 5f61 6464  t_valid_bond_add
-000009a0: 6974 696f 6e73 da17 6765 745f 7661 6c69  itions..get_vali
-000009b0: 645f 626f 6e64 5f72 656d 6f76 616c 73da  d_bond_removals.
-000009c0: 0361 6e79 da05 7072 696e 74da 0661 7070  .any..print..app
-000009d0: 656e 6429 0672 1e00 0000 7221 0000 0072  end).r....r!...r
-000009e0: 1f00 0000 da0d 6e65 6967 6862 6f72 735f  ......neighbors_
-000009f0: 7365 7472 2200 0000 da12 6e65 6967 6862  setr".....neighb
-00000a00: 6f72 735f 6669 6c74 6572 6564 7219 0000  ors_filteredr...
-00000a10: 0072 2300 0000 721a 0000 00da 1067 6574  .r#...r......get
-00000a20: 5f6e 6569 6768 626f 7268 6f6f 6424 0000  _neighborhood$..
-00000a30: 0073 2e00 0000 0617 0a02 0801 0602 0201  .s..............
-00000a40: 0201 0201 08fd 0606 0201 0201 08fe 0605  ................
-00000a50: 0201 08ff 0408 0801 0a01 1601 0801 0201  ................
-00000a60: 0c02 0402 7233 0000 00e9 0800 0000 da0b  ....r3..........
-00000a70: 6d61 785f 7661 6c65 6e63 6563 0200 0000  max_valencec....
-00000a80: 0000 0000 0000 0000 0300 0000 0400 0000  ................
-00000a90: 0300 0000 7332 0000 0069 007d 0274 0064  ....s2...i.}.t.d
-00000aa0: 017c 0183 0244 005d 0f89 0087 0066 0164  .|...D.].....f.d
-00000ab0: 0264 0384 087c 00a0 01a1 0044 0083 017c  .d...|.....D...|
-00000ac0: 0288 003c 0071 077c 0253 0029 044e 7207  ...<.q.|.S.).Nr.
-00000ad0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-00000ae0: 0200 0000 0400 0000 1300 0000 7320 0000  ............s ..
-00000af0: 0067 007c 005d 0c7d 017c 01a0 00a1 0088  .g.|.].}.|......
-00000b00: 006b 0572 027c 01a0 01a1 0091 0271 0253  .k.r.|.......q.S
-00000b10: 0072 1900 0000 2902 da10 4765 744e 756d  .r....)...GetNum
-00000b20: 496d 706c 6963 6974 4873 da06 4765 7449  ImplicitHs..GetI
-00000b30: 6478 2902 7224 0000 00da 0461 746f 6da9  dx).r$.....atom.
-00000b40: 01da 0169 7219 0000 0072 1a00 0000 7226  ...ir....r....r&
-00000b50: 0000 0062 0000 0073 0c00 0000 0600 0202  ...b...s........
-00000b60: 0a01 02fd 0601 06ff 7a28 6765 745f 6672  ........z(get_fr
-00000b70: 6565 5f76 616c 656e 6365 5f6d 6170 2e3c  ee_valence_map.<
-00000b80: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
-00000b90: 703e 2902 da05 7261 6e67 65da 0847 6574  p>)...range..Get
-00000ba0: 4174 6f6d 7329 0372 1000 0000 7235 0000  Atoms).r....r5..
-00000bb0: 00da 0672 6573 756c 7472 1900 0000 7239  ...resultr....r9
-00000bc0: 0000 0072 1a00 0000 7229 0000 005f 0000  ...r....r)..._..
-00000bd0: 0073 0c00 0000 0401 0e01 0a01 0602 0cfe  .s..............
-00000be0: 0406 7229 0000 0072 2100 0000 7222 0000  ..r)...r!...r"..
-00000bf0: 0063 0300 0000 0000 0000 0000 0000 0e00  .c..............
-00000c00: 0000 0800 0000 4300 0000 73a4 0000 0074  ......C...s....t
-00000c10: 0083 007d 0374 016a 026a 0374 016a 026a  ...}.t.j.j.t.j.j
-00000c20: 0474 016a 026a 0564 019c 037d 047c 04a0  .t.j.j.d...}.|..
-00000c30: 06a1 0044 005d 3c5c 027d 057d 067c 027c  ...D.]<\.}.}.|.|
-00000c40: 0519 0044 005d 337d 077c 01a0 06a1 0044  ...D.]3}.|.....D
-00000c50: 005d 2c5c 027d 087d 0974 01a0 077c 00a1  .],\.}.}.t...|..
-00000c60: 017d 0a7c 0aa0 0874 01a0 097c 08a1 01a1  .}.|...t...|....
-00000c70: 017d 0b7c 0aa0 0a7c 077c 0b7c 06a1 0301  .}.|...|.|.|....
-00000c80: 0074 016a 0b7c 0a64 0264 038d 027d 0c7c  .t.j.|.d.d...}.|
-00000c90: 0c72 4371 2174 01a0 0c7c 0aa1 017d 0d7c  .rCq!t...|...}.|
-00000ca0: 03a0 0d7c 0da1 0101 0071 2171 1b71 137c  ...|.....q!q.q.|
-00000cb0: 0353 0029 047a b60a 2020 2020 4769 7665  .S.).z..    Give
-00000cc0: 6e20 6120 6d6f 6c65 6375 6c65 2060 606d  n a molecule ``m
-00000cd0: 6f6c 6060 2c20 7468 6973 2066 756e 6374  ol``, this funct
-00000ce0: 696f 6e20 7769 6c6c 2072 6574 7572 6e20  ion will return 
-00000cf0: 6120 6c69 7374 206f 6620 534d 494c 4553  a list of SMILES
-00000d00: 2073 7472 696e 6773 2074 6861 7420 7265   strings that re
-00000d10: 7072 6573 656e 7420 7661 6c69 640a 2020  present valid.  
-00000d20: 2020 6174 6f6d 2061 6464 6974 696f 6e73    atom additions
-00000d30: 2074 6f20 7468 6520 6261 7365 206d 6f6c   to the base mol
-00000d40: 6563 756c 652e 0a0a 2020 2020 3a72 6574  ecule...    :ret
-00000d50: 7572 6e73 3a20 4120 6c69 7374 206f 6620  urns: A list of 
-00000d60: 7374 7269 6e67 732e 0a20 2020 20a9 0372  strings..    ..r
-00000d70: 0700 0000 e902 0000 00e9 0300 0000 54a9  ..............T.
-00000d80: 01da 0b63 6174 6368 4572 726f 7273 290e  ...catchErrors).
-00000d90: 7227 0000 0072 0200 0000 da08 426f 6e64  r'...r......Bond
-00000da0: 5479 7065 da06 5349 4e47 4c45 da06 444f  Type..SINGLE..DO
-00000db0: 5542 4c45 da06 5452 4950 4c45 da05 6974  UBLE..TRIPLE..it
-00000dc0: 656d 73da 0552 574d 6f6c da07 4164 6441  ems..RWMol..AddA
-00000dd0: 746f 6dda 0441 746f 6dda 0741 6464 426f  tom..Atom..AddBo
-00000de0: 6e64 da0b 5361 6e69 7469 7a65 4d6f 6cda  nd..SanitizeMol.
-00000df0: 0b4d 6f6c 546f 536d 696c 6573 da03 6164  .MolToSmiles..ad
-00000e00: 6429 0e72 1000 0000 7221 0000 0072 2200  d).r....r!...r".
-00000e10: 0000 da07 7265 7375 6c74 73da 1376 616c  ....results..val
-00000e20: 7565 5f62 6f6e 645f 7479 7065 5f6d 6170  ue_bond_type_map
-00000e30: 723a 0000 00da 0962 6f6e 645f 7479 7065  r:.....bond_type
-00000e40: 7238 0000 00da 0765 6c65 6d65 6e74 da07  r8.....element..
-00000e50: 7661 6c65 6e63 65da 076e 6577 5f6d 6f6c  valence..new_mol
-00000e60: da03 6964 78da 1373 616e 6974 697a 6174  ..idx..sanitizat
-00000e70: 696f 6e5f 7265 7375 6c74 721e 0000 0072  ion_resultr....r
-00000e80: 1900 0000 7219 0000 0072 1a00 0000 722b  ....r....r....r+
-00000e90: 0000 006b 0000 0073 2600 0000 060a 0603  ...k...s&.......
-00000ea0: 0601 0601 06fd 1005 0c02 1001 0a01 1001  ................
-00000eb0: 0e01 0e01 0401 0201 0a02 0c01 02f7 02ff  ................
-00000ec0: 040c 722b 0000 0063 0200 0000 0000 0000  ..r+...c........
-00000ed0: 0000 0000 1000 0000 0700 0000 4300 0000  ............C...
-00000ee0: 7336 0100 0074 0083 007d 0264 0174 016a  s6...t...}.d.t.j
-00000ef0: 026a 0374 016a 026a 0474 016a 026a 0564  .j.t.j.j.t.j.j.d
-00000f00: 029c 047d 0374 067c 0383 017d 047c 01a0  ...}.t.|...}.|..
-00000f10: 07a1 0044 005d 805c 027d 057d 0674 08a0  ...D.].\.}.}.t..
-00000f20: 097c 0664 03a1 0244 005d 755c 027d 077d  .|.d...D.]u\.}.}
-00000f30: 087c 00a0 0a7c 07a1 01a0 0ba1 0072 357c  .|...|.......r5|
-00000f40: 00a0 0a7c 08a1 01a0 0ba1 0072 3571 2274  ...|.......r5q"t
-00000f50: 01a0 0c7c 00a1 01a0 0d7c 077c 08a1 027d  ...|.....|.|...}
-00000f60: 0974 01a0 0e7c 00a1 017d 0a74 016a 0f7c  .t...|...}.t.j.|
-00000f70: 0a64 0464 058d 0201 007c 0964 0175 0172  .d.d.....|.d.u.r
-00000f80: 787c 09a0 10a1 007d 0b7c 0b7c 03a0 11a1  x|.....}.|.|....
-00000f90: 0076 0172 5971 227c 047c 0b19 007d 0c7c  .v.rYq"|.|...}.|
-00000fa0: 0c7c 0537 007d 0c7c 0c64 066b 0472 6671  .|.7.}.|.d.k.rfq
-00000fb0: 227c 09a0 12a1 007d 0d7c 09a0 137c 037c  "|.....}.|...|.|
-00000fc0: 0c19 00a1 0101 007c 0aa0 147c 0d7c 09a1  .......|...|.|..
-00000fd0: 0201 006e 0b7c 037c 0519 007d 0b7c 0aa0  ...n.|.|...}.|..
-00000fe0: 157c 077c 087c 0ba1 0301 0074 016a 167c  .|.|.|.....t.j.|
-00000ff0: 0a64 0464 078d 027d 0e7c 0e72 8d71 2274  .d.d...}.|.r.q"t
-00001000: 01a0 177c 0aa1 017d 0f7c 02a0 187c 0fa1  ...|...}.|...|..
-00001010: 0101 0071 2271 187c 0253 0029 0861 4003  ...q"q.|.S.).a@.
-00001020: 0000 0a20 2020 2047 6976 656e 2061 206d  ...    Given a m
-00001030: 6f6c 6563 756c 6520 6060 6d6f 6c60 602c  olecule ``mol``,
-00001040: 2074 6869 7320 6675 6e63 7469 6f6e 2077   this function w
-00001050: 696c 6c20 7265 7475 726e 2061 206c 6973  ill return a lis
-00001060: 7420 6f66 2053 4d49 4c45 5320 7374 7269  t of SMILES stri
-00001070: 6e67 7320 7768 6963 6820 7265 7375 6c74  ngs which result
-00001080: 7320 6672 6f6d 2076 616c 6964 0a20 2020  s from valid.   
-00001090: 2062 6f6e 6420 6164 6469 7469 6f6e 7320   bond additions 
-000010a0: 746f 2074 6861 7420 6261 7365 206d 6f6c  to that base mol
-000010b0: 6563 756c 652e 2056 616c 6964 2062 6f6e  ecule. Valid bon
-000010c0: 6420 6164 6469 7469 6f6e 7320 696e 2074  d additions in t
-000010d0: 6869 7320 6361 7365 2061 7265 2064 6566  his case are def
-000010e0: 696e 6564 2061 7320 616c 6c6f 7765 6420  ined as allowed 
-000010f0: 696e 0a20 2020 2074 6572 6d73 206f 6620  in.    terms of 
-00001100: 7468 6520 6174 6f6d 2076 616c 656e 6365  the atom valence
-00001110: 732e 2062 6f6e 6420 6164 6469 7469 6f6e  s. bond addition
-00001120: 7320 6d61 7920 636f 6e6e 6563 7420 7477  s may connect tw
-00001130: 6f20 6174 6f6d 7320 7768 6963 6820 6172  o atoms which ar
-00001140: 6520 6e6f 7420 7965 7420 6469 7265 6374  e not yet direct
-00001150: 6c79 2063 6f6e 6e65 6374 6564 0a20 2020  ly connected.   
-00001160: 206f 7220 7570 6772 6164 6520 616e 2065   or upgrade an e
-00001170: 7869 7374 696e 6720 626f 6e64 2028 7369  xisting bond (si
-00001180: 6e67 6c65 2074 6f20 646f 7562 6c65 292e  ngle to double).
-00001190: 0a0a 2020 2020 416c 736f 2064 6973 616c  ..    Also disal
-000011a0: 6c6f 7765 6420 6172 6520 626f 6e64 7320  lowed are bonds 
-000011b0: 6265 7477 6565 6e20 7477 6f20 6174 6f6d  between two atom
-000011c0: 7320 7768 6963 6820 6172 6520 7468 656d  s which are them
-000011d0: 7365 6c76 6573 2061 6c72 6561 6479 2070  selves already p
-000011e0: 6172 7420 6f66 2061 2072 696e 672e 0a0a  art of a ring...
-000011f0: 2020 2020 3a70 6172 616d 206d 6f6c 3a20      :param mol: 
-00001200: 5468 6520 6261 7365 206d 6f6c 6563 756c  The base molecul
-00001210: 650a 2020 2020 3a70 6172 616d 2066 7265  e.    :param fre
-00001220: 655f 7661 6c65 6e63 655f 696e 6469 6365  e_valence_indice
-00001230: 735f 6d61 703a 2041 2064 6963 7420 7768  s_map: A dict wh
-00001240: 6f73 6520 6b65 7973 2061 7265 2069 6e74  ose keys are int
-00001250: 6567 6572 7320 7374 6172 7469 6e67 2066  egers starting f
-00001260: 726f 6d20 302e 2054 4865 206b 6579 2076  rom 0. THe key v
-00001270: 616c 7565 730a 2020 2020 2020 2020 7265  alues.        re
-00001280: 7072 6573 656e 7420 7468 6520 2a66 7265  present the *fre
-00001290: 6520 6e75 6d62 6572 206f 6620 7661 6c65  e number of vale
-000012a0: 6e63 6573 2a2e 2054 6865 2076 616c 7565  nces*. The value
-000012b0: 7320 6172 6520 6c69 7374 7320 6f66 2061  s are lists of a
-000012c0: 746f 6d20 696e 6469 6365 7320 7768 6572  tom indices wher
-000012d0: 6520 6561 6368 2061 746f 6d20 696e 0a20  e each atom in. 
-000012e0: 2020 2020 2020 2074 6865 206c 6973 7420         the list 
-000012f0: 6861 7320 746f 2068 6176 6520 7468 6520  has to have the 
-00001300: 636f 7272 6573 706f 6e64 696e 6720 6e75  corresponding nu
-00001310: 6d62 6572 206f 6620 6672 6565 2076 616c  mber of free val
-00001320: 656e 6365 7320 6769 7665 6e20 6279 2074  ences given by t
-00001330: 6865 2064 6963 7420 6b65 792e 0a0a 2020  he dict key...  
-00001340: 2020 3a72 6574 7572 6e73 3a20 4120 6c69    :returns: A li
-00001350: 7374 206f 6620 7374 7269 6e67 730a 2020  st of strings.  
-00001360: 2020 4ea9 0472 0100 0000 7207 0000 0072    N..r....r....r
-00001370: 3f00 0000 7240 0000 0072 3f00 0000 54a9  ?...r@...r?...T.
-00001380: 01da 1263 6c65 6172 4172 6f6d 6174 6963  ...clearAromatic
-00001390: 466c 6167 7372 4000 0000 7241 0000 0029  Flagsr@...rA...)
-000013a0: 1972 2700 0000 7202 0000 0072 4300 0000  .r'...r....rC...
-000013b0: 7244 0000 0072 4500 0000 7246 0000 0072  rD...rE...rF...r
-000013c0: 0300 0000 7247 0000 00da 0969 7465 7274  ....rG.....itert
-000013d0: 6f6f 6c73 da0c 636f 6d62 696e 6174 696f  ools..combinatio
-000013e0: 6e73 da0e 4765 7441 746f 6d57 6974 6849  ns..GetAtomWithI
-000013f0: 6478 da08 4973 496e 5269 6e67 da03 4d6f  dx..IsInRing..Mo
-00001400: 6cda 1347 6574 426f 6e64 4265 7477 6565  l..GetBondBetwee
-00001410: 6e41 746f 6d73 7248 0000 00da 084b 656b  nAtomsrH.....Kek
-00001420: 756c 697a 65da 0b47 6574 426f 6e64 5479  ulize..GetBondTy
-00001430: 7065 da06 7661 6c75 6573 7237 0000 00da  pe..valuesr7....
-00001440: 0b53 6574 426f 6e64 5479 7065 da0b 5265  .SetBondType..Re
-00001450: 706c 6163 6542 6f6e 6472 4b00 0000 724c  placeBondrK...rL
-00001460: 0000 0072 4d00 0000 724e 0000 0029 1072  ...rM...rN...).r
-00001470: 1000 0000 7222 0000 0072 4f00 0000 7250  ....r"...rO...rP
-00001480: 0000 00da 1362 6f6e 645f 7479 7065 5f76  .....bond_type_v
-00001490: 616c 7565 5f6d 6170 7253 0000 00da 0561  alue_maprS.....a
-000014a0: 746f 6d73 da05 6174 6f6d 31da 0561 746f  toms..atom1..ato
-000014b0: 6d32 da04 626f 6e64 7254 0000 0072 5100  m2..bondrT...rQ.
-000014c0: 0000 da0a 626f 6e64 5f76 616c 7565 da05  ....bond_value..
-000014d0: 696e 6465 7872 5600 0000 721e 0000 0072  indexrV...r....r
-000014e0: 1900 0000 7219 0000 0072 1a00 0000 722c  ....r....r....r,
-000014f0: 0000 008d 0000 0073 4400 0000 0612 0203  .......sD.......
-00001500: 0601 0601 0601 06fc 0806 1002 1401 1c03  ................
-00001510: 0201 1202 0a01 0e02 0801 0801 0c01 0201  ................
-00001520: 0802 0801 0801 0201 0802 0e01 0e01 0803  ................
-00001530: 0e01 0e02 0401 0201 0a02 0c01 02df 0423  ...............#
-00001540: 722c 0000 0063 0100 0000 0000 0000 0000  r,...c..........
-00001550: 0000 0f00 0000 0700 0000 4300 0000 7362  ..........C...sb
-00001560: 0100 0074 0083 007d 0164 0174 016a 026a  ...t...}.d.t.j.j
-00001570: 0374 016a 026a 0474 016a 026a 0564 029c  .t.j.j.t.j.j.d..
-00001580: 047d 0274 067c 0283 017d 0364 0344 005d  .}.t.|...}.d.D.]
-00001590: 987d 047c 00a0 07a1 0044 005d 917d 057c  .}.|.....D.].}.|
-000015a0: 05a0 08a1 007c 05a0 09a1 0002 027d 067d  .....|.......}.}
-000015b0: 0774 01a0 0a7c 00a1 01a0 0b7c 067c 07a1  .t...|.....|.|..
-000015c0: 027d 057c 05a0 0ca1 007d 087c 087c 02a0  .}.|.....}.|.|..
-000015d0: 0da1 0076 0172 3b71 1c74 01a0 0e7c 00a1  ...v.r;q.t...|..
-000015e0: 017d 0974 016a 0f7c 0964 0464 058d 0201  .}.t.j.|.d.d....
-000015f0: 007c 037c 0819 007d 0a7c 0a7c 0438 007d  .|.|...}.|.|.8.}
-00001600: 0a7c 0a64 066b 0272 5a7c 09a0 107c 067c  .|.d.k.rZ|...|.|
-00001610: 07a1 0201 006e 177c 0a64 066b 0472 707c  .....n.|.d.k.rp|
-00001620: 05a0 117c 027c 0a19 00a1 0101 007c 05a0  ...|.|.......|..
-00001630: 12a1 007d 0b7c 09a0 137c 0b7c 05a1 0201  ...}.|...|.|....
-00001640: 006e 0171 1c74 016a 147c 0964 0464 078d  .n.q.t.j.|.d.d..
-00001650: 027d 0c7c 0c72 7b71 1c74 01a0 157c 09a1  .}.|.r{q.t...|..
-00001660: 017d 0d64 087c 0d76 0072 a874 167c 0da0  .}.d.|.v.r.t.|..
-00001670: 1764 08a1 0174 1864 098d 027d 0e74 187c  .d...t.d...}.t.|
-00001680: 0e64 0619 0083 0164 0a6b 0472 9671 1c74  .d.....d.k.r.q.t
-00001690: 1874 01a0 197c 0e64 0a19 00a1 01a0 1aa1  .t...|.d........
-000016a0: 0083 0164 0b6b 0072 a471 1c7c 0e64 0a19  ...d.k.r.q.|.d..
-000016b0: 007d 0d7c 01a0 1b7c 0da1 0101 0071 1c71  .}.|...|.....q.q
-000016c0: 167c 0153 0029 0c61 a201 0000 0a20 2020  .|.S.).a.....   
-000016d0: 2047 6976 656e 2061 206d 6f6c 6563 756c   Given a molecul
-000016e0: 6520 6060 6d6f 6c60 602c 2074 6869 7320  e ``mol``, this 
-000016f0: 6675 6e63 7469 6f6e 2077 696c 6c20 7265  function will re
-00001700: 7475 726e 2061 206c 6973 7420 6f66 2053  turn a list of S
-00001710: 4d49 4c45 5320 7374 7269 6e67 7320 7768  MILES strings wh
-00001720: 6963 6820 7265 7072 6573 656e 7420 7661  ich represent va
-00001730: 6c69 640a 2020 2020 626f 6e64 2072 656d  lid.    bond rem
-00001740: 6f76 616c 732e 2041 2062 6f6e 6420 7265  ovals. A bond re
-00001750: 6d6f 7661 6c20 6973 2065 6974 6865 7220  moval is either 
-00001760: 6120 646f 776e 6772 6164 6520 6f66 2061  a downgrade of a
-00001770: 6e20 6578 6973 7469 6e67 2062 6f6e 6420  n existing bond 
-00001780: 2865 2e67 2e20 646f 7562 6c65 2074 6f20  (e.g. double to 
-00001790: 7369 6e67 6c65 2920 6f72 2074 6865 0a20  single) or the. 
-000017a0: 2020 2072 656d 6f76 616c 206f 6620 6120     removal of a 
-000017b0: 7369 6e67 6c65 2062 6f6e 6420 7768 6963  single bond whic
-000017c0: 6820 776f 756c 6420 6d65 616e 2074 6f20  h would mean to 
-000017d0: 6469 7363 6f6e 6e65 6374 2061 7420 6d6f  disconnect at mo
-000017e0: 7374 2061 2073 696e 676c 6520 6174 6f6d  st a single atom
-000017f0: 2066 726f 6d20 7468 6520 7265 7374 206f   from the rest o
-00001800: 6620 7468 650a 2020 2020 6d6f 6c65 6375  f the.    molecu
-00001810: 6c65 210a 0a20 2020 203a 7061 7261 6d20  le!..    :param 
-00001820: 6d6f 6c3a 2054 6865 2062 6173 6520 6d6f  mol: The base mo
-00001830: 6c65 6375 6c65 2066 6f72 2074 6865 2072  lecule for the r
-00001840: 656d 6f76 616c 732e 0a0a 2020 2020 3a72  emovals...    :r
-00001850: 6574 7572 6e73 3a20 4120 6c69 7374 206f  eturns: A list o
-00001860: 6620 7374 7269 6e67 730a 2020 2020 4e72  f strings.    Nr
-00001870: 5700 0000 723e 0000 0054 7258 0000 0072  W...r>...TrX...r
-00001880: 0100 0000 7241 0000 00da 012e 2901 da03  ....rA......)...
-00001890: 6b65 7972 0700 0000 723f 0000 0029 1c72  keyr....r?...).r
-000018a0: 2700 0000 7202 0000 0072 4300 0000 7244  '...r....rC...rD
-000018b0: 0000 0072 4500 0000 7246 0000 0072 0300  ...rE...rF...r..
-000018c0: 0000 da08 4765 7442 6f6e 6473 da0f 4765  ....GetBonds..Ge
-000018d0: 7442 6567 696e 4174 6f6d 4964 78da 0d47  tBeginAtomIdx..G
-000018e0: 6574 456e 6441 746f 6d49 6478 725e 0000  etEndAtomIdxr^..
-000018f0: 0072 5f00 0000 7261 0000 0072 6200 0000  .r_...ra...rb...
-00001900: 7248 0000 0072 6000 0000 da0a 5265 6d6f  rH...r`.....Remo
-00001910: 7665 426f 6e64 7263 0000 0072 3700 0000  veBondrc...r7...
-00001920: 7264 0000 0072 4c00 0000 724d 0000 00da  rd...rL...rM....
-00001930: 0673 6f72 7465 64da 0573 706c 6974 da03  .sorted..split..
-00001940: 6c65 6e72 2800 0000 723c 0000 0072 4e00  lenr(...r<...rN.
-00001950: 0000 290f 7210 0000 0072 4f00 0000 7250  ..).r....rO...rP
-00001960: 0000 0072 6500 0000 7253 0000 0072 6900  ...re...rS...ri.
-00001970: 0000 7267 0000 0072 6800 0000 7251 0000  ..rg...rh...rQ..
-00001980: 0072 5400 0000 726a 0000 0072 6b00 0000  .rT...rj...rk...
-00001990: 7256 0000 0072 1e00 0000 da05 7061 7274  rV...r......part
-000019a0: 7372 1900 0000 7219 0000 0072 1a00 0000  sr....r....r....
-000019b0: 722d 0000 00d0 0000 0073 4e00 0000 060c  r-.......sN.....
-000019c0: 0203 0601 0601 0601 06fc 0806 0802 0c01  ................
-000019d0: 1201 1201 0802 0c01 0201 0a02 0e01 0802  ................
-000019e0: 0801 0802 0e01 0802 0e01 0801 0e01 0203  ................
-000019f0: 0e02 0401 0201 0a02 0801 1201 1001 0201  ................
-00001a00: 1a06 0201 0802 0c02 02d4 042e 722d 0000  ............r-..
-00001a10: 0029 0172 0f00 0000 2901 721c 0000 0029  .).r....).r....)
-00001a20: 0172 3400 0000 2919 725a 0000 00da 0674  .r4...).rZ.....t
-00001a30: 7970 696e 67da 0174 da05 7264 6b69 7472  yping..t..rdkitr
-00001a40: 0200 0000 da19 7667 645f 636f 756e 7465  ......vgd_counte
-00001a50: 7266 6163 7475 616c 732e 7574 696c 7372  rfactuals.utilsr
-00001a60: 0300 0000 da18 4445 4641 554c 545f 4154  ......DEFAULT_AT
-00001a70: 4f4d 5f56 414c 454e 4345 5f4d 4150 725e  OM_VALENCE_MAPr^
-00001a80: 0000 00da 0373 7472 721b 0000 0072 1d00  .....strr....r..
-00001a90: 0000 da08 5365 7175 656e 6365 da08 4361  ....Sequence..Ca
-00001aa0: 6c6c 6162 6c65 da04 626f 6f6c da04 4c69  llable..bool..Li
-00001ab0: 7374 7233 0000 00da 0369 6e74 da04 6469  str3.....int..di
-00001ac0: 6374 7229 0000 00da 0444 6963 74da 0353  ctr).....Dict..S
-00001ad0: 6574 722b 0000 0072 2c00 0000 722d 0000  etr+...r,...r-..
-00001ae0: 0072 1900 0000 7219 0000 0072 1900 0000  .r....r....r....
-00001af0: 721a 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-00001b00: 0000 0073 4c00 0000 0800 0801 0c01 0c02  ...sL...........
-00001b10: 0204 0201 0202 0201 0201 0201 06f9 160c  ................
-00001b20: 160a 0207 0202 0201 02fe 08fe 1602 02fe  ................
-00001b30: 0806 0afa 1a3b 080c 0c01 02ff 1202 02fe  .....;..........
-00001b40: 0803 0afd 0822 1201 02ff 0802 0afe 0843  .....".........C
-00001b50: 0801 0eff                                ....
+00000050: 6d06 5a06 0100 6400 6404 6c05 6d07 5a07  m.Z...d.d.l.m.Z.
+00000060: 0100 6400 6405 6c08 6d09 5a09 0100 6406  ..d.d.l.m.Z...d.
+00000070: 6407 6408 6409 640a 6408 640b 9c06 5a0a  d.d.d.d.d.d...Z.
+00000080: 0900 642a 640c 6504 6a0b 640d 6504 6a0b  ..d*d.e.j.d.e.j.
+00000090: 640e 650c 640f 6502 6a0d 650e 650e 6602  d.e.d.e.j.e.e.f.
+000000a0: 1900 6608 6410 6411 8405 5a0f 642b 6413  ..f.d.d...Z.d+d.
+000000b0: 6504 6a0b 6414 650e 6604 6415 6416 8405  e.j.d.e.f.d.d...
+000000c0: 5a10 642c 6413 6504 6a0b 6414 650e 6604  Z.d,d.e.j.d.e.f.
+000000d0: 6418 6419 8405 5a11 650a 6510 6511 6602  d.d...Z.e.e.e.f.
+000000e0: 6602 641a 650e 641b 6502 6a12 6502 6a13  f.d.e.d.e.j.e.j.
+000000f0: 6504 6a0b 6701 6514 6602 1900 1900 640f  e.j.g.e.f.....d.
+00000100: 6502 6a15 650e 1900 6606 641c 641d 8405  e.j.e...f.d.d...
+00000110: 5a16 642d 6413 6504 6a0b 641f 650c 640f  Z.d-d.e.j.d.e.d.
+00000120: 6517 6606 6420 6421 8405 5a18 6413 6504  e.f.d d!..Z.d.e.
+00000130: 6a0b 6422 6502 6a19 650e 650c 6602 1900  j.d"e.j.e.e.f...
+00000140: 6423 6502 6a19 650c 6502 6a15 650c 1900  d#e.j.e.e.j.e...
+00000150: 6602 1900 640f 6502 6a1a 650e 1900 6608  f...d.e.j.e...f.
+00000160: 6424 6425 8404 5a1b 6413 6504 6a0b 6423  d$d%..Z.d.e.j.d#
+00000170: 6502 6a19 650c 6502 6a15 650c 1900 6602  e.j.e.e.j.e...f.
+00000180: 1900 640f 6502 6a1a 650e 1900 6606 6426  ..d.e.j.e...f.d&
+00000190: 6427 8404 5a1c 6413 6504 6a0b 640f 6502  d'..Z.d.e.j.d.e.
+000001a0: 6a1a 650e 1900 6604 6428 6429 8404 5a1d  j.e...f.d(d)..Z.
+000001b0: 6401 5300 292e e900 0000 004e 2901 da04  d.S.)......N)...
+000001c0: 4368 656d 2901 da06 7264 464d 4353 2901  Chem)...rdFMCS).
+000001d0: da07 416c 6c43 6865 6d29 01da 0b69 6e76  ..AllChem)...inv
+000001e0: 6572 745f 6469 6374 e904 0000 00e9 0500  ert_dict........
+000001f0: 0000 e906 0000 00e9 0100 0000 e907 0000  ................
+00000200: 0029 06da 0143 da01 4eda 014f da01 46da  .)...C..N..O..F.
+00000210: 0243 6cda 0153 da04 6d6f 6c31 da04 6d6f  .Cl..S..mol1..mo
+00000220: 6c32 da06 7261 6469 7573 da06 7265 7475  l2..radius..retu
+00000230: 726e 6303 0000 0000 0000 0000 0000 000d  rnc.............
+00000240: 0000 0007 0000 0003 0000 0073 2c01 0000  ...........s,...
+00000250: 7c00 7c01 6602 4400 5d19 7d03 7c03 a000  |.|.f.D.].}.|...
+00000260: a100 4400 5d12 7d04 7401 6401 6402 8400  ..D.].}.t.d.d...
+00000270: 7c04 a002 a100 4400 8301 8301 7d05 7c04  |.....D.....}.|.
+00000280: a003 7c05 a101 0100 710a 7104 7404 6a05  ..|.....q.q.t.j.
+00000290: 7c00 7c01 6702 7404 6a06 6a07 6403 8d02  |.|.g.t.j.j.d...
+000002a0: 7d06 7408 a009 7c06 6a0a a101 7d07 6700  }.t...|.j...}.g.
+000002b0: 7d08 7c00 7c01 6602 4400 5d5e 7d03 7c03  }.|.|.f.D.]^}.|.
+000002c0: a00b 7c07 a101 8901 740c 8700 8701 6602  ..|.....t.....f.
+000002d0: 6404 6405 8408 7c03 a000 a100 4400 8301  d.d...|.....D...
+000002e0: 8301 7d09 740d 7c02 8301 4400 5d20 7d0a  ..}.t.|...D.] }.
+000002f0: 6700 7d0b 7c09 4400 5d12 7d0c 7c03 a00e  g.}.|.D.].}.|...
+00000300: 7c0c a101 7d04 7c0b 6406 6405 8400 7c04  |...}.|.d.d...|.
+00000310: a00f a100 4400 8301 3700 7d0b 7154 7c09  ....D...7.}.qT|.
+00000320: a010 740c 7c0b 8301 a101 0100 714e 7c03  ..t.|.......qN|.
+00000330: a000 a100 4400 5d07 7d04 7c04 a003 6407  ....D.].}.|...d.
+00000340: a101 0100 7173 7411 7c09 8301 6407 6b03  ....qst.|...d.k.
+00000350: 728e 7c08 a012 7408 6a13 7c03 7414 7c09  r.|...t.j.|.t.|.
+00000360: 8301 6408 8d02 a101 0100 7135 7c08 a012  ..d.......q5|...
+00000370: 6409 a101 0100 7135 7c08 5300 290a 7a05  d.....q5|.S.).z.
+00000380: 0a20 2020 2063 0100 0000 0000 0000 0000  .    c..........
+00000390: 0000 0200 0000 0400 0000 7300 0000 7320  ..........s...s 
+000003a0: 0000 0081 007c 005d 0b7d 017c 01a0 00a1  .....|.].}.|....
+000003b0: 007c 01a0 01a1 0017 0056 0001 0071 0264  .|.......V...q.d
+000003c0: 0053 00a9 014e 2902 da0b 4765 7442 6f6e  .S...N)...GetBon
+000003d0: 6454 7970 65da 0a47 6574 426f 6e64 4469  dType..GetBondDi
+000003e0: 7229 02da 022e 30da 0462 6f6e 64a9 0072  r)....0..bond..r
+000003f0: 1a00 0000 fa54 2f6d 6564 6961 2f73 7364  .....T/media/ssd
+00000400: 2f50 726f 6772 616d 6d69 6e67 2f76 6764  /Programming/vgd
+00000410: 5f63 6f75 6e74 6572 6661 6374 7561 6c73  _counterfactuals
+00000420: 2f76 6764 5f63 6f75 6e74 6572 6661 6374  /vgd_counterfact
+00000430: 7561 6c73 2f67 656e 6572 6174 652f 6d6f  uals/generate/mo
+00000440: 6c65 6375 6c65 732e 7079 da09 3c67 656e  lecules.py..<gen
+00000450: 6578 7072 3e1e 0000 0073 0400 0000 0280  expr>....s......
+00000460: 1e00 7a27 6d6f 6c65 6375 6c65 5f64 6966  ..z'molecule_dif
+00000470: 6665 7265 6e63 6573 2e3c 6c6f 6361 6c73  ferences.<locals
+00000480: 3e2e 3c67 656e 6578 7072 3e29 01da 0b61  >.<genexpr>)...a
+00000490: 746f 6d43 6f6d 7061 7265 6301 0000 0000  tomComparec.....
+000004a0: 0000 0000 0000 0002 0000 0004 0000 0013  ................
+000004b0: 0000 0073 2000 0000 6700 7c00 5d0c 7d01  ...s ...g.|.].}.
+000004c0: 7c01 a000 a100 0400 8900 8801 7601 7202  |...........v.r.
+000004d0: 8800 9102 7102 5300 721a 0000 00a9 01da  ....q.S.r.......
+000004e0: 0647 6574 4964 78a9 0272 1800 0000 da04  .GetIdx..r......
+000004f0: 6174 6f6d a902 da05 696e 6465 78da 056d  atom....index..m
+00000500: 6174 6368 721a 0000 0072 1b00 0000 da0a  atchr....r......
+00000510: 3c6c 6973 7463 6f6d 703e 2a00 0000 7302  <listcomp>*...s.
+00000520: 0000 0020 007a 286d 6f6c 6563 756c 655f  ... .z(molecule_
+00000530: 6469 6666 6572 656e 6365 732e 3c6c 6f63  differences.<loc
+00000540: 616c 733e 2e3c 6c69 7374 636f 6d70 3e63  als>.<listcomp>c
+00000550: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00000560: 0400 0000 5300 0000 7314 0000 0067 007c  ....S...s....g.|
+00000570: 005d 067d 017c 01a0 00a1 0091 0271 0253  .].}.|.......q.S
+00000580: 0072 1a00 0000 721e 0000 0029 0272 1800  .r....r....).r..
+00000590: 0000 da01 6172 1a00 0000 721a 0000 0072  ....ar....r....r
+000005a0: 1b00 0000 7225 0000 002f 0000 00f3 0200  ....r%.../......
+000005b0: 0000 1400 7201 0000 0029 01da 0a61 746f  ....r....)...ato
+000005c0: 6d73 546f 5573 65da 0029 15da 0847 6574  msToUse..)...Get
+000005d0: 4174 6f6d 73da 0373 756d da08 4765 7442  Atoms..sum..GetB
+000005e0: 6f6e 6473 da0a 5365 7449 736f 746f 7065  onds..SetIsotope
+000005f0: 7203 0000 00da 0746 696e 644d 4353 da0b  r......FindMCS..
+00000600: 4174 6f6d 436f 6d70 6172 65da 0f43 6f6d  AtomCompare..Com
+00000610: 7061 7265 4973 6f74 6f70 6573 7202 0000  pareIsotopesr...
+00000620: 00da 0d4d 6f6c 4672 6f6d 536d 6172 7473  ...MolFromSmarts
+00000630: da0c 736d 6172 7473 5374 7269 6e67 da11  ..smartsString..
+00000640: 4765 7453 7562 7374 7275 6374 4d61 7463  GetSubstructMatc
+00000650: 68da 0373 6574 da05 7261 6e67 65da 0e47  h..set..range..G
+00000660: 6574 4174 6f6d 5769 7468 4964 78da 0c47  etAtomWithIdx..G
+00000670: 6574 4e65 6967 6862 6f72 73da 0675 7064  etNeighbors..upd
+00000680: 6174 65da 036c 656e da06 6170 7065 6e64  ate..len..append
+00000690: da13 4d6f 6c46 7261 676d 656e 7454 6f53  ..MolFragmentToS
+000006a0: 6d69 6c65 73da 046c 6973 7429 0d72 1100  miles..list).r..
+000006b0: 0000 7212 0000 0072 1300 0000 da03 6d6f  ..r....r......mo
+000006c0: 6c72 2100 0000 da05 7661 6c75 65da 036d  lr!.....value..m
+000006d0: 6373 da13 636f 6d6d 6f6e 5f73 7562 7374  cs..common_subst
+000006e0: 7275 6374 7572 65da 0772 6573 756c 7473  ructure..results
+000006f0: da0b 6e6f 6e5f 6d61 7463 6865 73da 0172  ..non_matches..r
+00000700: da09 6e65 6967 6862 6f72 73da 0a61 746f  ..neighbors..ato
+00000710: 6d5f 696e 6465 7872 1a00 0000 7222 0000  m_indexr....r"..
+00000720: 0072 1b00 0000 da14 6d6f 6c65 6375 6c65  .r......molecule
+00000730: 5f64 6966 6665 7265 6e63 6573 1600 0000  _differences....
+00000740: 7334 0000 000c 060c 0116 010c 0102 fe04  s4..............
+00000750: 0406 0106 0106 fe0c 0404 020c 010a 011c  ................
+00000760: 010c 0104 0108 010a 0118 0110 020c 020c  ................
+00000770: 010c 021a 010c 0204 0272 4600 0000 fa0e  .........rF.....
+00000780: 2a31 3d2a 2a32 3d2a 2a3d 2a31 2a32 723d  *1=**2=**=*1*2r=
+00000790: 0000 00da 0770 6174 7465 726e 6302 0000  .....patternc...
+000007a0: 0000 0000 0000 0000 0004 0000 0003 0000  ................
+000007b0: 0043 0000 00f3 1800 0000 7400 a001 7c01  .C........t...|.
+000007c0: a101 7d02 7c00 a002 7c02 a101 7d03 7c03  ..}.|...|...}.|.
+000007d0: 5300 2901 7a83 0a20 2020 2043 6865 636b  S.).z..    Check
+000007e0: 7320 6966 2074 6865 2067 6976 656e 206d  s if the given m
+000007f0: 6f6c 6563 756c 6520 6060 6d6f 6c60 6020  olecule ``mol`` 
+00000800: 6973 2061 2062 7269 6467 6520 6865 6164  is a bridge head
+00000810: 2063 6172 626f 6e20 7374 7275 6374 7572   carbon structur
+00000820: 6520 7768 6963 6820 6170 7061 7265 6e74  e which apparent
+00000830: 6c79 2064 6f65 7320 6e6f 740a 2020 2020  ly does not.    
+00000840: 6170 7065 6172 2069 6e20 6368 656d 6973  appear in chemis
+00000850: 7472 792e 0a20 2020 20a9 0372 0200 0000  try..    ..r....
+00000860: 7231 0000 00da 1148 6173 5375 6273 7472  r1.....HasSubstr
+00000870: 7563 744d 6174 6368 a904 723d 0000 0072  uctMatch..r=...r
+00000880: 4800 0000 da06 736d 6172 7473 da08 6973  H.....smarts..is
+00000890: 5f6d 6174 6368 721a 0000 0072 1a00 0000  _matchr....r....
+000008a0: 721b 0000 00da 1569 735f 6272 6964 6765  r......is_bridge
+000008b0: 5f68 6561 645f 6361 7262 6f6e 3e00 0000  _head_carbon>...
+000008c0: 7306 0000 000a 050a 0104 0172 4f00 0000  s..........rO...
+000008d0: da03 534e 4e63 0200 0000 0000 0000 0000  ..SNNc..........
+000008e0: 0000 0400 0000 0300 0000 4300 0000 7249  ..........C...rI
+000008f0: 0000 0072 1500 0000 724a 0000 0072 4c00  ...r....rJ...rL.
+00000900: 0000 721a 0000 0072 1a00 0000 721b 0000  ..r....r....r...
+00000910: 00da 1b69 735f 6e69 7472 6f67 656e 5f6e  ...is_nitrogen_n
+00000920: 6974 726f 6765 6e5f 7375 6c66 7572 4800  itrogen_sulfurH.
+00000930: 0000 7306 0000 000a 010a 0104 0172 5100  ..s..........rQ.
+00000940: 0000 da06 736d 696c 6573 da0b 6d6f 6c5f  ....smiles..mol_
+00000950: 6669 6c74 6572 7363 0300 0000 0000 0000  filtersc........
+00000960: 0000 0000 0600 0000 0700 0000 0300 0000  ................
+00000970: 738c 0000 0074 0083 007d 0374 01a0 027c  s....t...}.t...|
+00000980: 00a1 0189 0074 0388 0083 017d 047c 03a0  .....t.....}.|..
+00000990: 0474 0588 007c 017c 0464 018d 03a1 0101  .t...|.|.d......
+000009a0: 007c 03a0 0474 0688 007c 0464 028d 02a1  .|...t...|.d....
+000009b0: 0101 007c 03a0 0474 0788 0064 038d 01a1  ...|...t...d....
+000009c0: 0101 0067 007d 057c 0344 005d 187d 0074  ...g.}.|.D.].}.t
+000009d0: 01a0 027c 00a1 0189 0074 0887 0066 0164  ...|.....t...f.d
+000009e0: 0464 0584 087c 0244 0083 0183 0172 3e71  .d...|.D.....r>q
+000009f0: 2b7c 05a0 097c 00a1 0101 0071 2b7c 0553  +|...|.....q+|.S
+00000a00: 0029 0661 b103 0000 0a20 2020 2047 6976  .).a.....    Giv
+00000a10: 656e 2061 2060 6073 6d69 6c65 7360 6020  en a ``smiles`` 
+00000a20: 7265 7072 6573 656e 7461 7469 6f6e 206f  representation o
+00000a30: 6620 6120 6d6f 6c65 6375 6c65 2c20 7468  f a molecule, th
+00000a40: 6973 2066 756e 6374 696f 6e20 7769 6c6c  is function will
+00000a50: 2072 6574 7572 6e20 6120 6c69 7374 206f   return a list o
+00000a60: 6620 7468 6520 534d 494c 4553 0a20 2020  f the SMILES.   
+00000a70: 2072 6570 7265 7365 6e74 6174 696f 6e73   representations
+00000a80: 206f 6620 616c 6c20 7468 6520 7661 6c69   of all the vali
+00000a90: 6420 6d6f 6c65 6375 6c65 7320 7769 7468  d molecules with
+00000aa0: 696e 2061 2031 2d65 6469 7420 6e65 6967  in a 1-edit neig
+00000ab0: 6862 6f72 686f 6f64 2e20 4f70 7469 6f6e  hborhood. Option
+00000ac0: 616c 6c79 2c20 6120 6c69 7374 206f 6620  ally, a list of 
+00000ad0: 626f 6f6c 6561 6e0a 2020 2020 6675 6e63  boolean.    func
+00000ae0: 7469 6f6e 7320 6361 6e20 6265 2070 726f  tions can be pro
+00000af0: 7669 6465 6420 666f 7220 6060 6d6f 6c5f  vided for ``mol_
+00000b00: 6669 6c74 6572 7360 6020 746f 2066 7572  filters`` to fur
+00000b10: 7468 6572 206c 696d 6974 2074 6865 206b  ther limit the k
+00000b20: 696e 6473 206f 6620 6d6f 6c65 6375 6c65  inds of molecule
+00000b30: 7320 696e 636c 7564 6564 2069 6e20 7468  s included in th
+00000b40: 650a 2020 2020 7265 7375 6c74 2e0a 0a20  e.    result... 
+00000b50: 2020 203a 7061 7261 6d20 736d 696c 6573     :param smiles
+00000b60: 3a20 5468 6520 534d 494c 4553 2073 7472  : The SMILES str
+00000b70: 696e 6720 7265 7072 6573 656e 7461 7469  ing representati
+00000b80: 6f6e 206f 660a 2020 2020 3a70 6172 616d  on of.    :param
+00000b90: 2061 746f 6d5f 7661 6c65 6e63 655f 6d61   atom_valence_ma
+00000ba0: 703a 2041 2064 6963 7469 6f6e 6172 792c  p: A dictionary,
+00000bb0: 2077 686f 7365 206b 6579 7320 6172 6520   whose keys are 
+00000bc0: 7374 7269 6e67 7320 7468 6174 2069 6465  strings that ide
+00000bd0: 6e74 6966 7920 6174 6f6d 2074 7970 6573  ntify atom types
+00000be0: 206f 6620 7468 6520 534d 494c 4553 0a20   of the SMILES. 
+00000bf0: 2020 2020 2020 206e 6f74 6174 696f 6e20         notation 
+00000c00: 284f 2c20 4e2c 2043 6c20 2e2e 2e29 2061  (O, N, Cl ...) a
+00000c10: 6e64 2074 6865 2076 616c 7565 7320 6172  nd the values ar
+00000c20: 6520 7468 6520 696e 7465 6765 7220 7661  e the integer va
+00000c30: 6c65 6e63 6520 6f66 2074 6865 2063 6f72  lence of the cor
+00000c40: 7265 7370 6f6e 6469 6e67 2061 746f 6d2e  responding atom.
+00000c50: 204f 6e6c 790a 2020 2020 2020 2020 6174   Only.        at
+00000c60: 6f6d 7320 7468 6174 2061 7265 206c 6973  oms that are lis
+00000c70: 7465 6420 696e 2074 6869 7320 6469 6374  ted in this dict
+00000c80: 2077 696c 6c20 6265 2063 6f6e 7369 6465   will be conside
+00000c90: 7265 6420 666f 7220 6564 6974 206f 7065  red for edit ope
+00000ca0: 7261 7469 6f6e 7320 7375 6368 2061 7320  rations such as 
+00000cb0: 6164 6469 6e67 206f 720a 2020 2020 2020  adding or.      
+00000cc0: 2020 7265 706c 6163 696e 6720 616e 6420    replacing and 
+00000cd0: 6174 6f6d 210a 2020 2020 3a70 6172 616d  atom!.    :param
+00000ce0: 206d 6f6c 5f66 696c 7465 7273 3a20 4120   mol_filters: A 
+00000cf0: 6c69 7374 206f 6620 6675 6e63 7469 6f6e  list of function
+00000d00: 7320 7768 6963 6820 6561 6368 2074 616b  s which each tak
+00000d10: 6520 6120 4d6f 6c20 6f62 6a65 6374 2061  e a Mol object a
+00000d20: 7320 696e 7075 7420 616e 6420 7265 7475  s input and retu
+00000d30: 726e 2061 2062 6f6f 6c65 616e 2076 616c  rn a boolean val
+00000d40: 7565 0a20 2020 2020 2020 2074 6f20 6465  ue.        to de
+00000d50: 7465 726d 696e 6520 7768 6574 6865 7220  termine whether 
+00000d60: 7468 6174 2061 746f 6d20 7368 6f75 6c64  that atom should
+00000d70: 2062 6520 6578 636c 7564 6564 2028 5472   be excluded (Tr
+00000d80: 7565 2920 6f72 206e 6f74 2028 4661 6c73  ue) or not (Fals
+00000d90: 6529 2e0a 0a20 2020 203a 7265 7475 726e  e)...    :return
+00000da0: 733a 2041 206c 6973 7420 6f66 2073 7472  s: A list of str
+00000db0: 696e 6773 0a20 2020 2029 0372 3d00 0000  ings.    ).r=...
+00000dc0: da10 6174 6f6d 5f76 616c 656e 6365 5f6d  ..atom_valence_m
+00000dd0: 6170 da18 6672 6565 5f76 616c 656e 6365  ap..free_valence
+00000de0: 5f69 6e64 6963 6573 5f6d 6170 2902 723d  _indices_map).r=
+00000df0: 0000 0072 5500 0000 a901 723d 0000 0063  ...rU.....r=...c
+00000e00: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00000e10: 0400 0000 1300 0000 7314 0000 0067 007c  ........s....g.|
+00000e20: 005d 067d 017c 0188 0083 0191 0271 0253  .].}.|.......q.S
+00000e30: 0072 1a00 0000 721a 0000 0029 0272 1800  .r....r....).r..
+00000e40: 0000 da04 6675 6e63 7256 0000 0072 1a00  ....funcrV...r..
+00000e50: 0000 721b 0000 0072 2500 0000 8000 0000  ..r....r%.......
+00000e60: 7227 0000 007a 2467 6574 5f6e 6569 6768  r'...z$get_neigh
+00000e70: 626f 7268 6f6f 642e 3c6c 6f63 616c 733e  borhood.<locals>
+00000e80: 2e3c 6c69 7374 636f 6d70 3e29 0a72 3400  .<listcomp>).r4.
+00000e90: 0000 7202 0000 00da 0d4d 6f6c 4672 6f6d  ..r......MolFrom
+00000ea0: 536d 696c 6573 da14 6765 745f 6672 6565  Smiles..get_free
+00000eb0: 5f76 616c 656e 6365 5f6d 6170 7238 0000  _valence_mapr8..
+00000ec0: 00da 1867 6574 5f76 616c 6964 5f61 746f  ...get_valid_ato
+00000ed0: 6d5f 6164 6469 7469 6f6e 73da 1867 6574  m_additions..get
+00000ee0: 5f76 616c 6964 5f62 6f6e 645f 6164 6469  _valid_bond_addi
+00000ef0: 7469 6f6e 73da 1767 6574 5f76 616c 6964  tions..get_valid
+00000f00: 5f62 6f6e 645f 7265 6d6f 7661 6c73 da03  _bond_removals..
+00000f10: 616e 7972 3a00 0000 2906 7252 0000 0072  anyr:...).rR...r
+00000f20: 5400 0000 7253 0000 00da 0d6e 6569 6768  T...rS.....neigh
+00000f30: 626f 7273 5f73 6574 7255 0000 00da 126e  bors_setrU.....n
+00000f40: 6569 6768 626f 7273 5f66 696c 7465 7265  eighbors_filtere
+00000f50: 6472 1a00 0000 7256 0000 0072 1b00 0000  dr....rV...r....
+00000f60: da10 6765 745f 6e65 6967 6862 6f72 686f  ..get_neighborho
+00000f70: 6f64 4e00 0000 732c 0000 0006 170a 0208  odN...s,........
+00000f80: 0106 0202 0102 0102 0108 fd06 0602 0102  ................
+00000f90: 0108 fe06 0502 0108 ff04 0808 010a 0116  ................
+00000fa0: 0102 010c 0204 0272 6000 0000 e908 0000  .......r`.......
+00000fb0: 00da 0b6d 6178 5f76 616c 656e 6365 6302  ...max_valencec.
+00000fc0: 0000 0000 0000 0000 0000 0003 0000 0004  ................
+00000fd0: 0000 0003 0000 0073 3200 0000 6900 7d02  .......s2...i.}.
+00000fe0: 7400 6401 7c01 8302 4400 5d0f 8900 8700  t.d.|...D.].....
+00000ff0: 6601 6402 6403 8408 7c00 a001 a100 4400  f.d.d...|.....D.
+00001000: 8301 7c02 8800 3c00 7107 7c02 5300 2904  ..|...<.q.|.S.).
+00001010: 4e72 0900 0000 6301 0000 0000 0000 0000  Nr....c.........
+00001020: 0000 0002 0000 0004 0000 0013 0000 0073  ...............s
+00001030: 2000 0000 6700 7c00 5d0c 7d01 7c01 a000   ...g.|.].}.|...
+00001040: a100 8800 6b05 7202 7c01 a001 a100 9102  ....k.r.|.......
+00001050: 7102 5300 721a 0000 0029 02da 1047 6574  q.S.r....)...Get
+00001060: 4e75 6d49 6d70 6c69 6369 7448 7372 1f00  NumImplicitHsr..
+00001070: 0000 7220 0000 00a9 01da 0169 721a 0000  ..r .......ir...
+00001080: 0072 1b00 0000 7225 0000 008b 0000 0073  .r....r%.......s
+00001090: 0c00 0000 0600 0202 0a01 02fd 0601 06ff  ................
+000010a0: 7a28 6765 745f 6672 6565 5f76 616c 656e  z(get_free_valen
+000010b0: 6365 5f6d 6170 2e3c 6c6f 6361 6c73 3e2e  ce_map.<locals>.
+000010c0: 3c6c 6973 7463 6f6d 703e 2902 7235 0000  <listcomp>).r5..
+000010d0: 0072 2a00 0000 2903 723d 0000 0072 6200  .r*...).r=...rb.
+000010e0: 0000 da06 7265 7375 6c74 721a 0000 0072  ....resultr....r
+000010f0: 6400 0000 721b 0000 0072 5900 0000 8800  d...r....rY.....
+00001100: 0000 730c 0000 0004 010e 010a 0106 020c  ..s.............
+00001110: fe04 0672 5900 0000 7254 0000 0072 5500  ...rY...rT...rU.
+00001120: 0000 6303 0000 0000 0000 0000 0000 000e  ..c.............
+00001130: 0000 0008 0000 0043 0000 0073 a400 0000  .......C...s....
+00001140: 7400 8300 7d03 7401 6a02 6a03 7401 6a02  t...}.t.j.j.t.j.
+00001150: 6a04 7401 6a02 6a05 6401 9c03 7d04 7c04  j.t.j.j.d...}.|.
+00001160: a006 a100 4400 5d3c 5c02 7d05 7d06 7c02  ....D.]<\.}.}.|.
+00001170: 7c05 1900 4400 5d33 7d07 7c01 a006 a100  |...D.]3}.|.....
+00001180: 4400 5d2c 5c02 7d08 7d09 7401 a007 7c00  D.],\.}.}.t...|.
+00001190: a101 7d0a 7c0a a008 7401 a009 7c08 a101  ..}.|...t...|...
+000011a0: a101 7d0b 7c0a a00a 7c07 7c0b 7c06 a103  ..}.|...|.|.|...
+000011b0: 0100 7401 6a0b 7c0a 6402 6403 8d02 7d0c  ..t.j.|.d.d...}.
+000011c0: 7c0c 7243 7121 7401 a00c 7c0a a101 7d0d  |.rCq!t...|...}.
+000011d0: 7c03 a00d 7c0d a101 0100 7121 711b 7113  |...|.....q!q.q.
+000011e0: 7c03 5300 2904 7ab6 0a20 2020 2047 6976  |.S.).z..    Giv
+000011f0: 656e 2061 206d 6f6c 6563 756c 6520 6060  en a molecule ``
+00001200: 6d6f 6c60 602c 2074 6869 7320 6675 6e63  mol``, this func
+00001210: 7469 6f6e 2077 696c 6c20 7265 7475 726e  tion will return
+00001220: 2061 206c 6973 7420 6f66 2053 4d49 4c45   a list of SMILE
+00001230: 5320 7374 7269 6e67 7320 7468 6174 2072  S strings that r
+00001240: 6570 7265 7365 6e74 2076 616c 6964 0a20  epresent valid. 
+00001250: 2020 2061 746f 6d20 6164 6469 7469 6f6e     atom addition
+00001260: 7320 746f 2074 6865 2062 6173 6520 6d6f  s to the base mo
+00001270: 6c65 6375 6c65 2e0a 0a20 2020 203a 7265  lecule...    :re
+00001280: 7475 726e 733a 2041 206c 6973 7420 6f66  turns: A list of
+00001290: 2073 7472 696e 6773 2e0a 2020 2020 a903   strings..    ..
+000012a0: 7209 0000 00e9 0200 0000 e903 0000 0054  r..............T
+000012b0: a901 da0b 6361 7463 6845 7272 6f72 7329  ....catchErrors)
+000012c0: 0e72 3400 0000 7202 0000 00da 0842 6f6e  .r4...r......Bon
+000012d0: 6454 7970 65da 0653 494e 474c 45da 0644  dType..SINGLE..D
+000012e0: 4f55 424c 45da 0654 5249 504c 45da 0569  OUBLE..TRIPLE..i
+000012f0: 7465 6d73 da05 5257 4d6f 6cda 0741 6464  tems..RWMol..Add
+00001300: 4174 6f6d da04 4174 6f6d da07 4164 6442  Atom..Atom..AddB
+00001310: 6f6e 64da 0b53 616e 6974 697a 654d 6f6c  ond..SanitizeMol
+00001320: da0b 4d6f 6c54 6f53 6d69 6c65 73da 0361  ..MolToSmiles..a
+00001330: 6464 290e 723d 0000 0072 5400 0000 7255  dd).r=...rT...rU
+00001340: 0000 0072 4100 0000 da13 7661 6c75 655f  ...rA.....value_
+00001350: 626f 6e64 5f74 7970 655f 6d61 7072 6500  bond_type_mapre.
+00001360: 0000 da09 626f 6e64 5f74 7970 6572 2100  ....bond_typer!.
+00001370: 0000 da07 656c 656d 656e 74da 0776 616c  ....element..val
+00001380: 656e 6365 da07 6e65 775f 6d6f 6cda 0369  ence..new_mol..i
+00001390: 6478 da13 7361 6e69 7469 7a61 7469 6f6e  dx..sanitization
+000013a0: 5f72 6573 756c 7472 5200 0000 721a 0000  _resultrR...r...
+000013b0: 0072 1a00 0000 721b 0000 0072 5a00 0000  .r....r....rZ...
+000013c0: 9400 0000 7326 0000 0006 0a06 0306 0106  ....s&..........
+000013d0: 0106 fd10 050c 0210 010a 0110 010e 010e  ................
+000013e0: 0104 0102 010a 020c 0102 f702 ff04 0c72  ...............r
+000013f0: 5a00 0000 6302 0000 0000 0000 0000 0000  Z...c...........
+00001400: 0010 0000 0007 0000 0043 0000 0073 3601  .........C...s6.
+00001410: 0000 7400 8300 7d02 6401 7401 6a02 6a03  ..t...}.d.t.j.j.
+00001420: 7401 6a02 6a04 7401 6a02 6a05 6402 9c04  t.j.j.t.j.j.d...
+00001430: 7d03 7406 7c03 8301 7d04 7c01 a007 a100  }.t.|...}.|.....
+00001440: 4400 5d80 5c02 7d05 7d06 7408 a009 7c06  D.].\.}.}.t...|.
+00001450: 6403 a102 4400 5d75 5c02 7d07 7d08 7c00  d...D.]u\.}.}.|.
+00001460: a00a 7c07 a101 a00b a100 7235 7c00 a00a  ..|.......r5|...
+00001470: 7c08 a101 a00b a100 7235 7122 7401 a00c  |.......r5q"t...
+00001480: 7c00 a101 a00d 7c07 7c08 a102 7d09 7401  |.....|.|...}.t.
+00001490: a00e 7c00 a101 7d0a 7401 6a0f 7c0a 6404  ..|...}.t.j.|.d.
+000014a0: 6405 8d02 0100 7c09 6401 7501 7278 7c09  d.....|.d.u.rx|.
+000014b0: a010 a100 7d0b 7c0b 7c03 a011 a100 7601  ....}.|.|.....v.
+000014c0: 7259 7122 7c04 7c0b 1900 7d0c 7c0c 7c05  rYq"|.|...}.|.|.
+000014d0: 3700 7d0c 7c0c 6406 6b04 7266 7122 7c09  7.}.|.d.k.rfq"|.
+000014e0: a012 a100 7d0d 7c09 a013 7c03 7c0c 1900  ....}.|...|.|...
+000014f0: a101 0100 7c0a a014 7c0d 7c09 a102 0100  ....|...|.|.....
+00001500: 6e0b 7c03 7c05 1900 7d0b 7c0a a015 7c07  n.|.|...}.|...|.
+00001510: 7c08 7c0b a103 0100 7401 6a16 7c0a 6404  |.|.....t.j.|.d.
+00001520: 6407 8d02 7d0e 7c0e 728d 7122 7401 a017  d...}.|.r.q"t...
+00001530: 7c0a a101 7d0f 7c02 a018 7c0f a101 0100  |...}.|...|.....
+00001540: 7122 7118 7c02 5300 2908 6140 0300 000a  q"q.|.S.).a@....
+00001550: 2020 2020 4769 7665 6e20 6120 6d6f 6c65      Given a mole
+00001560: 6375 6c65 2060 606d 6f6c 6060 2c20 7468  cule ``mol``, th
+00001570: 6973 2066 756e 6374 696f 6e20 7769 6c6c  is function will
+00001580: 2072 6574 7572 6e20 6120 6c69 7374 206f   return a list o
+00001590: 6620 534d 494c 4553 2073 7472 696e 6773  f SMILES strings
+000015a0: 2077 6869 6368 2072 6573 756c 7473 2066   which results f
+000015b0: 726f 6d20 7661 6c69 640a 2020 2020 626f  rom valid.    bo
+000015c0: 6e64 2061 6464 6974 696f 6e73 2074 6f20  nd additions to 
+000015d0: 7468 6174 2062 6173 6520 6d6f 6c65 6375  that base molecu
+000015e0: 6c65 2e20 5661 6c69 6420 626f 6e64 2061  le. Valid bond a
+000015f0: 6464 6974 696f 6e73 2069 6e20 7468 6973  dditions in this
+00001600: 2063 6173 6520 6172 6520 6465 6669 6e65   case are define
+00001610: 6420 6173 2061 6c6c 6f77 6564 2069 6e0a  d as allowed in.
+00001620: 2020 2020 7465 726d 7320 6f66 2074 6865      terms of the
+00001630: 2061 746f 6d20 7661 6c65 6e63 6573 2e20   atom valences. 
+00001640: 626f 6e64 2061 6464 6974 696f 6e73 206d  bond additions m
+00001650: 6179 2063 6f6e 6e65 6374 2074 776f 2061  ay connect two a
+00001660: 746f 6d73 2077 6869 6368 2061 7265 206e  toms which are n
+00001670: 6f74 2079 6574 2064 6972 6563 746c 7920  ot yet directly 
+00001680: 636f 6e6e 6563 7465 640a 2020 2020 6f72  connected.    or
+00001690: 2075 7067 7261 6465 2061 6e20 6578 6973   upgrade an exis
+000016a0: 7469 6e67 2062 6f6e 6420 2873 696e 676c  ting bond (singl
+000016b0: 6520 746f 2064 6f75 626c 6529 2e0a 0a20  e to double)... 
+000016c0: 2020 2041 6c73 6f20 6469 7361 6c6c 6f77     Also disallow
+000016d0: 6564 2061 7265 2062 6f6e 6473 2062 6574  ed are bonds bet
+000016e0: 7765 656e 2074 776f 2061 746f 6d73 2077  ween two atoms w
+000016f0: 6869 6368 2061 7265 2074 6865 6d73 656c  hich are themsel
+00001700: 7665 7320 616c 7265 6164 7920 7061 7274  ves already part
+00001710: 206f 6620 6120 7269 6e67 2e0a 0a20 2020   of a ring...   
+00001720: 203a 7061 7261 6d20 6d6f 6c3a 2054 6865   :param mol: The
+00001730: 2062 6173 6520 6d6f 6c65 6375 6c65 0a20   base molecule. 
+00001740: 2020 203a 7061 7261 6d20 6672 6565 5f76     :param free_v
+00001750: 616c 656e 6365 5f69 6e64 6963 6573 5f6d  alence_indices_m
+00001760: 6170 3a20 4120 6469 6374 2077 686f 7365  ap: A dict whose
+00001770: 206b 6579 7320 6172 6520 696e 7465 6765   keys are intege
+00001780: 7273 2073 7461 7274 696e 6720 6672 6f6d  rs starting from
+00001790: 2030 2e20 5448 6520 6b65 7920 7661 6c75   0. THe key valu
+000017a0: 6573 0a20 2020 2020 2020 2072 6570 7265  es.        repre
+000017b0: 7365 6e74 2074 6865 202a 6672 6565 206e  sent the *free n
+000017c0: 756d 6265 7220 6f66 2076 616c 656e 6365  umber of valence
+000017d0: 732a 2e20 5468 6520 7661 6c75 6573 2061  s*. The values a
+000017e0: 7265 206c 6973 7473 206f 6620 6174 6f6d  re lists of atom
+000017f0: 2069 6e64 6963 6573 2077 6865 7265 2065   indices where e
+00001800: 6163 6820 6174 6f6d 2069 6e0a 2020 2020  ach atom in.    
+00001810: 2020 2020 7468 6520 6c69 7374 2068 6173      the list has
+00001820: 2074 6f20 6861 7665 2074 6865 2063 6f72   to have the cor
+00001830: 7265 7370 6f6e 6469 6e67 206e 756d 6265  responding numbe
+00001840: 7220 6f66 2066 7265 6520 7661 6c65 6e63  r of free valenc
+00001850: 6573 2067 6976 656e 2062 7920 7468 6520  es given by the 
+00001860: 6469 6374 206b 6579 2e0a 0a20 2020 203a  dict key...    :
+00001870: 7265 7475 726e 733a 2041 206c 6973 7420  returns: A list 
+00001880: 6f66 2073 7472 696e 6773 0a20 2020 204e  of strings.    N
+00001890: a904 7201 0000 0072 0900 0000 7268 0000  ..r....r....rh..
+000018a0: 0072 6900 0000 7268 0000 0054 a901 da12  .ri...rh...T....
+000018b0: 636c 6561 7241 726f 6d61 7469 6346 6c61  clearAromaticFla
+000018c0: 6773 7269 0000 0072 6a00 0000 2919 7234  gsri...rj...).r4
+000018d0: 0000 0072 0200 0000 726c 0000 0072 6d00  ...r....rl...rm.
+000018e0: 0000 726e 0000 0072 6f00 0000 7205 0000  ..rn...ro...r...
+000018f0: 0072 7000 0000 da09 6974 6572 746f 6f6c  .rp.....itertool
+00001900: 73da 0c63 6f6d 6269 6e61 7469 6f6e 7372  s..combinationsr
+00001910: 3600 0000 da08 4973 496e 5269 6e67 da03  6.....IsInRing..
+00001920: 4d6f 6cda 1347 6574 426f 6e64 4265 7477  Mol..GetBondBetw
+00001930: 6565 6e41 746f 6d73 7271 0000 00da 084b  eenAtomsrq.....K
+00001940: 656b 756c 697a 6572 1600 0000 da06 7661  ekulizer......va
+00001950: 6c75 6573 721f 0000 00da 0b53 6574 426f  luesr......SetBo
+00001960: 6e64 5479 7065 da0b 5265 706c 6163 6542  ndType..ReplaceB
+00001970: 6f6e 6472 7400 0000 7275 0000 0072 7600  ondrt...ru...rv.
+00001980: 0000 7277 0000 0029 1072 3d00 0000 7255  ..rw...).r=...rU
+00001990: 0000 0072 4100 0000 7278 0000 00da 1362  ...rA...rx.....b
+000019a0: 6f6e 645f 7479 7065 5f76 616c 7565 5f6d  ond_type_value_m
+000019b0: 6170 727b 0000 00da 0561 746f 6d73 da05  apr{.....atoms..
+000019c0: 6174 6f6d 31da 0561 746f 6d32 7219 0000  atom1..atom2r...
+000019d0: 0072 7c00 0000 7279 0000 00da 0a62 6f6e  .r|...ry.....bon
+000019e0: 645f 7661 6c75 6572 2300 0000 727e 0000  d_valuer#...r~..
+000019f0: 0072 5200 0000 721a 0000 0072 1a00 0000  .rR...r....r....
+00001a00: 721b 0000 0072 5b00 0000 b600 0000 7344  r....r[.......sD
+00001a10: 0000 0006 1202 0306 0106 0106 0106 fc08  ................
+00001a20: 0610 0214 011c 0302 0112 020a 010e 0208  ................
+00001a30: 0108 010c 0102 0108 0208 0108 0102 0108  ................
+00001a40: 020e 010e 0108 030e 010e 0204 0102 010a  ................
+00001a50: 020c 0102 df04 2372 5b00 0000 6301 0000  ......#r[...c...
+00001a60: 0000 0000 0000 0000 000f 0000 0007 0000  ................
+00001a70: 0043 0000 0073 6201 0000 7400 8300 7d01  .C...sb...t...}.
+00001a80: 6401 7401 6a02 6a03 7401 6a02 6a04 7401  d.t.j.j.t.j.j.t.
+00001a90: 6a02 6a05 6402 9c04 7d02 7406 7c02 8301  j.j.d...}.t.|...
+00001aa0: 7d03 6403 4400 5d98 7d04 7c00 a007 a100  }.d.D.].}.|.....
+00001ab0: 4400 5d91 7d05 7c05 a008 a100 7c05 a009  D.].}.|.....|...
+00001ac0: a100 0202 7d06 7d07 7401 a00a 7c00 a101  ....}.}.t...|...
+00001ad0: a00b 7c06 7c07 a102 7d05 7c05 a00c a100  ..|.|...}.|.....
+00001ae0: 7d08 7c08 7c02 a00d a100 7601 723b 711c  }.|.|.....v.r;q.
+00001af0: 7401 a00e 7c00 a101 7d09 7401 6a0f 7c09  t...|...}.t.j.|.
+00001b00: 6404 6405 8d02 0100 7c03 7c08 1900 7d0a  d.d.....|.|...}.
+00001b10: 7c0a 7c04 3800 7d0a 7c0a 6406 6b02 725a  |.|.8.}.|.d.k.rZ
+00001b20: 7c09 a010 7c06 7c07 a102 0100 6e17 7c0a  |...|.|.....n.|.
+00001b30: 6406 6b04 7270 7c05 a011 7c02 7c0a 1900  d.k.rp|...|.|...
+00001b40: a101 0100 7c05 a012 a100 7d0b 7c09 a013  ....|.....}.|...
+00001b50: 7c0b 7c05 a102 0100 6e01 711c 7401 6a14  |.|.....n.q.t.j.
+00001b60: 7c09 6404 6407 8d02 7d0c 7c0c 727b 711c  |.d.d...}.|.r{q.
+00001b70: 7401 a015 7c09 a101 7d0d 6408 7c0d 7600  t...|...}.d.|.v.
+00001b80: 72a8 7416 7c0d a017 6408 a101 7418 6409  r.t.|...d...t.d.
+00001b90: 8d02 7d0e 7418 7c0e 6406 1900 8301 640a  ..}.t.|.d.....d.
+00001ba0: 6b04 7296 711c 7418 7401 a019 7c0e 640a  k.r.q.t.t...|.d.
+00001bb0: 1900 a101 a01a a100 8301 640b 6b00 72a4  ..........d.k.r.
+00001bc0: 711c 7c0e 640a 1900 7d0d 7c01 a01b 7c0d  q.|.d...}.|...|.
+00001bd0: a101 0100 711c 7116 7c01 5300 290c 61a2  ....q.q.|.S.).a.
+00001be0: 0100 000a 2020 2020 4769 7665 6e20 6120  ....    Given a 
+00001bf0: 6d6f 6c65 6375 6c65 2060 606d 6f6c 6060  molecule ``mol``
+00001c00: 2c20 7468 6973 2066 756e 6374 696f 6e20  , this function 
+00001c10: 7769 6c6c 2072 6574 7572 6e20 6120 6c69  will return a li
+00001c20: 7374 206f 6620 534d 494c 4553 2073 7472  st of SMILES str
+00001c30: 696e 6773 2077 6869 6368 2072 6570 7265  ings which repre
+00001c40: 7365 6e74 2076 616c 6964 0a20 2020 2062  sent valid.    b
+00001c50: 6f6e 6420 7265 6d6f 7661 6c73 2e20 4120  ond removals. A 
+00001c60: 626f 6e64 2072 656d 6f76 616c 2069 7320  bond removal is 
+00001c70: 6569 7468 6572 2061 2064 6f77 6e67 7261  either a downgra
+00001c80: 6465 206f 6620 616e 2065 7869 7374 696e  de of an existin
+00001c90: 6720 626f 6e64 2028 652e 672e 2064 6f75  g bond (e.g. dou
+00001ca0: 626c 6520 746f 2073 696e 676c 6529 206f  ble to single) o
+00001cb0: 7220 7468 650a 2020 2020 7265 6d6f 7661  r the.    remova
+00001cc0: 6c20 6f66 2061 2073 696e 676c 6520 626f  l of a single bo
+00001cd0: 6e64 2077 6869 6368 2077 6f75 6c64 206d  nd which would m
+00001ce0: 6561 6e20 746f 2064 6973 636f 6e6e 6563  ean to disconnec
+00001cf0: 7420 6174 206d 6f73 7420 6120 7369 6e67  t at most a sing
+00001d00: 6c65 2061 746f 6d20 6672 6f6d 2074 6865  le atom from the
+00001d10: 2072 6573 7420 6f66 2074 6865 0a20 2020   rest of the.   
+00001d20: 206d 6f6c 6563 756c 6521 0a0a 2020 2020   molecule!..    
+00001d30: 3a70 6172 616d 206d 6f6c 3a20 5468 6520  :param mol: The 
+00001d40: 6261 7365 206d 6f6c 6563 756c 6520 666f  base molecule fo
+00001d50: 7220 7468 6520 7265 6d6f 7661 6c73 2e0a  r the removals..
+00001d60: 0a20 2020 203a 7265 7475 726e 733a 2041  .    :returns: A
+00001d70: 206c 6973 7420 6f66 2073 7472 696e 6773   list of strings
+00001d80: 0a20 2020 204e 727f 0000 0072 6700 0000  .    Nr....rg...
+00001d90: 5472 8000 0000 7201 0000 0072 6a00 0000  Tr....r....rj...
+00001da0: da01 2e29 01da 036b 6579 7209 0000 0072  ...)...keyr....r
+00001db0: 6800 0000 291c 7234 0000 0072 0200 0000  h...).r4...r....
+00001dc0: 726c 0000 0072 6d00 0000 726e 0000 0072  rl...rm...rn...r
+00001dd0: 6f00 0000 7205 0000 0072 2c00 0000 da0f  o...r....r,.....
+00001de0: 4765 7442 6567 696e 4174 6f6d 4964 78da  GetBeginAtomIdx.
+00001df0: 0d47 6574 456e 6441 746f 6d49 6478 7285  .GetEndAtomIdxr.
+00001e00: 0000 0072 8600 0000 7216 0000 0072 8800  ...r....r....r..
+00001e10: 0000 7271 0000 0072 8700 0000 da0a 5265  ..rq...r......Re
+00001e20: 6d6f 7665 426f 6e64 7289 0000 0072 1f00  moveBondr....r..
+00001e30: 0000 728a 0000 0072 7500 0000 7276 0000  ..r....ru...rv..
+00001e40: 00da 0673 6f72 7465 64da 0573 706c 6974  ...sorted..split
+00001e50: 7239 0000 0072 5800 0000 722a 0000 0072  r9...rX...r*...r
+00001e60: 7700 0000 290f 723d 0000 0072 4100 0000  w...).r=...rA...
+00001e70: 7278 0000 0072 8b00 0000 727b 0000 0072  rx...r....r{...r
+00001e80: 1900 0000 728d 0000 0072 8e00 0000 7279  ....r....r....ry
+00001e90: 0000 0072 7c00 0000 728f 0000 0072 2300  ...r|...r....r#.
+00001ea0: 0000 727e 0000 0072 5200 0000 da05 7061  ..r~...rR.....pa
+00001eb0: 7274 7372 1a00 0000 721a 0000 0072 1b00  rtsr....r....r..
+00001ec0: 0000 725c 0000 00f9 0000 0073 4e00 0000  ..r\.......sN...
+00001ed0: 060c 0203 0601 0601 0601 06fc 0806 0802  ................
+00001ee0: 0c01 1201 1201 0802 0c01 0201 0a02 0e01  ................
+00001ef0: 0802 0801 0802 0e01 0802 0e01 0801 0e01  ................
+00001f00: 0203 0e02 0401 0201 0a02 0801 1201 1001  ................
+00001f10: 0201 1a06 0201 0802 0c02 02d4 042e 725c  ..............r\
+00001f20: 0000 0029 0172 0100 0000 2901 7247 0000  ...).r....).rG..
+00001f30: 0029 0172 5000 0000 2901 7261 0000 0029  .).rP...).ra...)
+00001f40: 1e72 8200 0000 da06 7479 7069 6e67 da01  .r......typing..
+00001f50: 74da 0572 646b 6974 7202 0000 00da 0a72  t..rdkitr......r
+00001f60: 646b 6974 2e43 6865 6d72 0300 0000 7204  dkit.Chemr....r.
+00001f70: 0000 00da 1976 6764 5f63 6f75 6e74 6572  .....vgd_counter
+00001f80: 6661 6374 7561 6c73 2e75 7469 6c73 7205  factuals.utilsr.
+00001f90: 0000 00da 1844 4546 4155 4c54 5f41 544f  .....DEFAULT_ATO
+00001fa0: 4d5f 5641 4c45 4e43 455f 4d41 5072 8500  M_VALENCE_MAPr..
+00001fb0: 0000 da03 696e 74da 0554 7570 6c65 da03  ....int..Tuple..
+00001fc0: 7374 7272 4600 0000 724f 0000 0072 5100  strrF...rO...rQ.
+00001fd0: 0000 da08 5365 7175 656e 6365 da08 4361  ....Sequence..Ca
+00001fe0: 6c6c 6162 6c65 da04 626f 6f6c da04 4c69  llable..bool..Li
+00001ff0: 7374 7260 0000 00da 0464 6963 7472 5900  str`.....dictrY.
+00002000: 0000 da04 4469 6374 da03 5365 7472 5a00  ....Dict..SetrZ.
+00002010: 0000 725b 0000 0072 5c00 0000 721a 0000  ..r[...r\...r...
+00002020: 0072 1a00 0000 721a 0000 0072 1b00 0000  .r....r....r....
+00002030: da08 3c6d 6f64 756c 653e 0100 0000 7360  ..<module>....s`
+00002040: 0000 0008 0008 010c 010c 010c 010c 0202  ................
+00002050: 0402 0102 0202 0102 0102 0106 f902 0e0a  ................
+00002060: fe04 0102 ff02 0202 fe0c 030a fd16 2816  ..............(.
+00002070: 0a02 0702 0202 0102 fe08 fe16 0202 fe08  ................
+00002080: 060a fa1a 3a08 0c0c 0102 ff12 0202 fe08  ....:...........
+00002090: 030a fd08 2212 0102 ff08 020a fe08 4308  ....".........C.
+000020a0: 010e ff                                  ...
```

### Comparing `vgd_counterfactuals-0.1.4/vgd_counterfactuals/generate/molecules.py` & `vgd_counterfactuals-0.1.5/vgd_counterfactuals/generate/molecules.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,68 @@
 import itertools
 import typing as t
 from rdkit import Chem
+from rdkit.Chem import rdFMCS
+from rdkit.Chem import AllChem
 
 from vgd_counterfactuals.utils import invert_dict
 
 
 DEFAULT_ATOM_VALENCE_MAP = {
     'C': 4,
     'N': 5,
     # 'P': 5,
     'O': 6,
     'F': 1,
     'Cl': 7,
     'S': 6,
-
 }
 
 
+
+def molecule_differences(mol1: Chem.Mol,
+                         mol2: Chem.Mol,
+                         radius: int = 0,
+                         ) -> t.Tuple[str, str]:
+    """
+    """
+    for mol in [mol1, mol2]:
+        for atom in mol.GetAtoms():
+            value = sum(bond.GetBondType() + bond.GetBondDir() for bond in atom.GetBonds())
+            atom.SetIsotope(value)
+
+    mcs = rdFMCS.FindMCS(
+        [mol1, mol2],
+        atomCompare=rdFMCS.AtomCompare.CompareIsotopes,
+    )
+    common_substructure = Chem.MolFromSmarts(mcs.smartsString)
+
+    results = []
+    for mol in [mol1, mol2]:
+        match = mol.GetSubstructMatch(common_substructure)
+        non_matches = set([index for atom in mol.GetAtoms() if (index := atom.GetIdx()) not in match])
+        for r in range(radius):
+            neighbors = []
+            for atom_index in non_matches:
+                atom = mol.GetAtomWithIdx(atom_index)
+                neighbors += [a.GetIdx() for a in atom.GetNeighbors()]
+
+            non_matches.update(set(neighbors))
+
+        for atom in mol.GetAtoms():
+            atom.SetIsotope(0)
+
+        if len(non_matches) != 0:
+            results.append(Chem.MolFragmentToSmiles(mol, atomsToUse=list(non_matches)))
+        else:
+            results.append('')
+
+    return results
+
+
 def is_bridge_head_carbon(mol: Chem.Mol, pattern: str = '*1=**2=**=*1*2'):
     """
     Checks if the given molecule ``mol`` is a bridge head carbon structure which apparently does not
     appear in chemistry.
     """
     smarts = Chem.MolFromSmarts(pattern)
     is_match = mol.HasSubstructMatch(smarts)
```

### Comparing `vgd_counterfactuals-0.1.4/vgd_counterfactuals/generate/smiles_one_step_changes.py` & `vgd_counterfactuals-0.1.5/vgd_counterfactuals/generate/smiles_one_step_changes.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.4/vgd_counterfactuals/templates/article.tex.j2` & `vgd_counterfactuals-0.1.5/vgd_counterfactuals/templates/article.tex.j2`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.4/vgd_counterfactuals/utils.py` & `vgd_counterfactuals-0.1.5/vgd_counterfactuals/utils.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.4/vgd_counterfactuals/visualization.py` & `vgd_counterfactuals-0.1.5/vgd_counterfactuals/visualization.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.4/PKG-INFO` & `vgd_counterfactuals-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vgd-counterfactuals
-Version: 0.1.4
+Version: 0.1.5
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
 
-.. |version| image:: https://img.shields.io/badge/version-0.1.4-orange.svg
+.. |version| image:: https://img.shields.io/badge/version-0.1.5-orange.svg
    :target: https://www.python.org/
    :alt: version
 
 .. image:: banner.png
    :alt: banner image
 
 ===================
```

