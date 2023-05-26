# Comparing `tmp/celltypist-1.5.0.tar.gz` & `tmp/celltypist-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/celltypist-1.5.0.tar", last modified: Tue May 16 20:07:29 2023, max compression
+gzip compressed data, was "dist/celltypist-1.5.1.tar", last modified: Fri May 26 20:12:55 2023, max compression
```

## Comparing `celltypist-1.5.0.tar` & `celltypist-1.5.1.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-sr-x   0 cx1      (20436) team205   (1403)        0 2023-05-16 20:07:29.661369 celltypist-1.5.0/
--rw-r--r--   0 cx1      (20436) team205   (1403)      256 2022-01-08 15:31:17.000000 celltypist-1.5.0/.gitignore
--rw-r--r--   0 cx1      (20436) team205   (1403)     2301 2023-05-16 19:57:02.000000 celltypist-1.5.0/CHANGELOG.md
--rw-r--r--   0 cx1      (20436) team205   (1403)     5120 2022-06-20 15:29:01.000000 celltypist-1.5.0/CITATION.cff
--rw-r--r--   0 cx1      (20436) team205   (1403)      579 2022-05-31 18:44:35.000000 celltypist-1.5.0/Dockerfile
--rw-r--r--   0 cx1      (20436) team205   (1403)     1056 2021-05-01 12:32:36.000000 celltypist-1.5.0/LICENSE
--rw-r--r--   0 cx1      (20436) team205   (1403)      153 2021-12-25 19:53:33.000000 celltypist-1.5.0/MANIFEST.in
--rw-r--r--   0 cx1      (20436) team205   (1403)    79562 2023-05-16 20:07:29.657960 celltypist-1.5.0/PKG-INFO
--rw-r--r--   0 cx1      (20436) team205   (1403)    71919 2023-05-16 08:14:33.000000 celltypist-1.5.0/README.md
-drwxr-sr-x   0 cx1      (20436) team205   (1403)        0 2023-05-16 20:07:26.994779 celltypist-1.5.0/celltypist/
--rw-r--r--   0 cx1      (20436) team205   (1403)      342 2023-05-16 19:55:17.000000 celltypist-1.5.0/celltypist/__init__.py
--rw-r--r--   0 cx1      (20436) team205   (1403)     6109 2022-08-22 09:17:16.000000 celltypist-1.5.0/celltypist/annotate.py
--rw-r--r--   0 cx1      (20436) team205   (1403)    27204 2022-08-22 12:28:50.000000 celltypist-1.5.0/celltypist/classifier.py
--rw-r--r--   0 cx1      (20436) team205   (1403)     7421 2022-01-26 22:00:20.000000 celltypist-1.5.0/celltypist/command_line.py
-drwxr-sr-x   0 cx1      (20436) team205   (1403)        0 2023-05-16 20:07:27.211304 celltypist-1.5.0/celltypist/contro/
--rw-r--r--   0 cx1      (20436) team205   (1403)        0 2023-05-02 08:46:42.000000 celltypist-1.5.0/celltypist/contro/__init__.py
--rw-r--r--   0 cx1      (20436) team205   (1403)    33894 2023-05-15 20:57:38.000000 celltypist-1.5.0/celltypist/contro/align.py
--rw-r--r--   0 cx1      (20436) team205   (1403)    26363 2023-05-02 08:46:42.000000 celltypist-1.5.0/celltypist/contro/distance.py
--rw-r--r--   0 cx1      (20436) team205   (1403)    11379 2023-05-02 08:46:42.000000 celltypist-1.5.0/celltypist/contro/distances.py
--rw-r--r--   0 cx1      (20436) team205   (1403)     8310 2023-05-15 21:15:07.000000 celltypist-1.5.0/celltypist/contro/harmonize.py
--rw-r--r--   0 cx1      (20436) team205   (1403)    15932 2023-05-02 08:46:42.000000 celltypist-1.5.0/celltypist/contro/integrate.py
--rw-r--r--   0 cx1      (20436) team205   (1403)     9926 2023-05-02 08:46:42.000000 celltypist-1.5.0/celltypist/contro/pct.py
--rw-r--r--   0 cx1      (20436) team205   (1403)    30047 2023-05-02 08:46:42.000000 celltypist-1.5.0/celltypist/contro/plot.py
--rw-r--r--   0 cx1      (20436) team205   (1403)      109 2023-05-02 08:46:42.000000 celltypist-1.5.0/celltypist/contro/symbols.py
-drwxr-sr-x   0 cx1      (20436) team205   (1403)        0 2023-05-16 20:07:26.698247 celltypist-1.5.0/celltypist/data/
-drwxr-sr-x   0 cx1      (20436) team205   (1403)        0 2023-05-16 20:07:27.290115 celltypist-1.5.0/celltypist/data/samples/
--rw-r--r--   0 cx1      (20436) team205   (1403)   557901 2022-01-27 10:03:11.000000 celltypist-1.5.0/celltypist/data/samples/Ensembl105_Human2Mouse_Genes.csv
--rw-r--r--   0 cx1      (20436) team205   (1403) 53473636 2021-05-01 12:32:37.000000 celltypist-1.5.0/celltypist/data/samples/sample_cell_by_gene.csv
--rw-r--r--   0 cx1      (20436) team205   (1403)      226 2021-05-01 12:32:37.000000 celltypist-1.5.0/celltypist/logger.py
--rw-r--r--   0 cx1      (20436) team205   (1403)    20972 2022-12-14 17:45:50.000000 celltypist-1.5.0/celltypist/models.py
--rw-r--r--   0 cx1      (20436) team205   (1403)    10071 2023-05-02 08:46:42.000000 celltypist-1.5.0/celltypist/plot.py
--rw-r--r--   0 cx1      (20436) team205   (1403)     4157 2022-08-22 08:57:00.000000 celltypist-1.5.0/celltypist/samples.py
--rw-r--r--   0 cx1      (20436) team205   (1403)    19188 2023-05-02 08:46:42.000000 celltypist-1.5.0/celltypist/train.py
-drwxr-sr-x   0 cx1      (20436) team205   (1403)        0 2023-05-16 20:07:27.059097 celltypist-1.5.0/celltypist.egg-info/
--rw-r--r--   0 cx1      (20436) team205   (1403)    79562 2023-05-16 20:07:21.000000 celltypist-1.5.0/celltypist.egg-info/PKG-INFO
--rw-r--r--   0 cx1      (20436) team205   (1403)     1921 2023-05-16 20:07:23.000000 celltypist-1.5.0/celltypist.egg-info/SOURCES.txt
--rw-r--r--   0 cx1      (20436) team205   (1403)        1 2023-05-16 20:07:21.000000 celltypist-1.5.0/celltypist.egg-info/dependency_links.txt
--rw-r--r--   0 cx1      (20436) team205   (1403)       61 2023-05-16 20:07:21.000000 celltypist-1.5.0/celltypist.egg-info/entry_points.txt
--rw-r--r--   0 cx1      (20436) team205   (1403)      140 2023-05-16 20:07:21.000000 celltypist-1.5.0/celltypist.egg-info/requires.txt
--rw-r--r--   0 cx1      (20436) team205   (1403)       11 2023-05-16 20:07:21.000000 celltypist-1.5.0/celltypist.egg-info/top_level.txt
-drwxr-sr-x   0 cx1      (20436) team205   (1403)        0 2023-05-16 20:07:28.856781 celltypist-1.5.0/docs/
--rw-r--r--   0 cx1      (20436) team205   (1403)      638 2021-05-01 12:32:37.000000 celltypist-1.5.0/docs/Makefile
-drwxr-sr-x   0 cx1      (20436) team205   (1403)        0 2023-05-16 20:07:29.148406 celltypist-1.5.0/docs/notebook/
--rw-r--r--   0 cx1      (20436) team205   (1403)   376236 2022-08-23 10:52:31.000000 celltypist-1.5.0/docs/notebook/celltypist_tutorial.ipynb
--rw-r--r--   0 cx1      (20436) team205   (1403)   552805 2022-08-23 13:32:51.000000 celltypist-1.5.0/docs/notebook/celltypist_tutorial_cv.ipynb
--rw-r--r--   0 cx1      (20436) team205   (1403)  1512368 2023-05-16 11:01:52.000000 celltypist-1.5.0/docs/notebook/celltypist_tutorial_harmonisation.ipynb
--rw-r--r--   0 cx1      (20436) team205   (1403)  3075328 2023-05-16 19:05:14.000000 celltypist-1.5.0/docs/notebook/celltypist_tutorial_integration.ipynb
--rw-r--r--   0 cx1      (20436) team205   (1403)   629323 2022-08-23 12:38:41.000000 celltypist-1.5.0/docs/notebook/celltypist_tutorial_ml.ipynb
--rw-r--r--   0 cx1      (20436) team205   (1403)      225 2023-05-02 08:46:43.000000 celltypist-1.5.0/docs/requirements.txt
-drwxr-sr-x   0 cx1      (20436) team205   (1403)        0 2023-05-16 20:07:29.586987 celltypist-1.5.0/docs/source/
-drwxr-sr-x   0 cx1      (20436) team205   (1403)        0 2023-05-16 20:07:26.710626 celltypist-1.5.0/docs/source/_static/
-drwxr-sr-x   0 cx1      (20436) team205   (1403)        0 2023-05-16 20:07:29.613639 celltypist-1.5.0/docs/source/_static/img/
--rw-r--r--   0 cx1      (20436) team205   (1403)    67929 2021-11-02 03:08:25.000000 celltypist-1.5.0/docs/source/_static/img/logo_celltypist.png
--rw-r--r--   0 cx1      (20436) team205   (1403)       83 2022-08-05 12:50:13.000000 celltypist-1.5.0/docs/source/celltypist.annotate.rst
--rw-r--r--   0 cx1      (20436) team205   (1403)      156 2022-08-05 13:11:23.000000 celltypist-1.5.0/docs/source/celltypist.classifier.AnnotationResult.rst
--rw-r--r--   0 cx1      (20436) team205   (1403)      153 2022-08-05 13:12:18.000000 celltypist-1.5.0/docs/source/celltypist.classifier.Classifier.rst
--rw-r--r--   0 cx1      (20436) team205   (1403)      162 2023-05-02 08:46:43.000000 celltypist-1.5.0/docs/source/celltypist.contro.align.DistanceAlignment.rst
--rw-r--r--   0 cx1      (20436) team205   (1403)      154 2023-05-02 08:46:43.000000 celltypist-1.5.0/docs/source/celltypist.contro.distance.Distance.rst
--rw-r--r--   0 cx1      (20436) team205   (1403)      161 2023-05-02 08:46:43.000000 celltypist-1.5.0/docs/source/celltypist.contro.pct.PredictiveClusteringTree.rst
--rw-r--r--   0 cx1      (20436) team205   (1403)       80 2023-05-02 08:46:43.000000 celltypist-1.5.0/docs/source/celltypist.dotplot.rst
--rw-r--r--   0 cx1      (20436) team205   (1403)       87 2023-05-02 08:46:43.000000 celltypist-1.5.0/docs/source/celltypist.harmonize.rst
--rw-r--r--   0 cx1      (20436) team205   (1403)       85 2023-05-02 08:46:43.000000 celltypist-1.5.0/docs/source/celltypist.integrate.rst
--rw-r--r--   0 cx1      (20436) team205   (1403)      139 2022-08-05 13:13:01.000000 celltypist-1.5.0/docs/source/celltypist.models.Model.rst
--rw-r--r--   0 cx1      (20436) team205   (1403)      101 2022-08-05 13:30:15.000000 celltypist-1.5.0/docs/source/celltypist.models.download_models.rst
--rw-r--r--   0 cx1      (20436) team205   (1403)      101 2022-08-05 12:49:53.000000 celltypist-1.5.0/docs/source/celltypist.samples.downsample_adata.rst
--rw-r--r--   0 cx1      (20436) team205   (1403)       86 2023-05-02 08:46:43.000000 celltypist-1.5.0/docs/source/celltypist.sankeyplot.rst
--rw-r--r--   0 cx1      (20436) team205   (1403)       78 2022-08-05 12:50:03.000000 celltypist-1.5.0/docs/source/celltypist.train.rst
--rw-r--r--   0 cx1      (20436) team205   (1403)       82 2023-05-02 08:46:43.000000 celltypist-1.5.0/docs/source/celltypist.treeplot.rst
--rw-r--r--   0 cx1      (20436) team205   (1403)     2872 2023-05-02 08:46:43.000000 celltypist-1.5.0/docs/source/conf.py
--rw-r--r--   0 cx1      (20436) team205   (1403)     1602 2023-05-02 08:46:43.000000 celltypist-1.5.0/docs/source/index.rst
--rw-r--r--   0 cx1      (20436) team205   (1403)      140 2023-05-02 08:46:43.000000 celltypist-1.5.0/requirements.txt
--rw-r--r--   0 cx1      (20436) team205   (1403)       38 2023-05-16 20:07:29.663373 celltypist-1.5.0/setup.cfg
--rw-r--r--   0 cx1      (20436) team205   (1403)     1519 2023-05-02 08:46:43.000000 celltypist-1.5.0/setup.py
+drwxr-sr-x   0 cx1      (20436) team205   (1403)        0 2023-05-26 20:12:55.731689 celltypist-1.5.1/
+-rw-r--r--   0 cx1      (20436) team205   (1403)      256 2022-01-08 15:31:17.000000 celltypist-1.5.1/.gitignore
+-rw-r--r--   0 cx1      (20436) team205   (1403)     2379 2023-05-26 15:25:14.000000 celltypist-1.5.1/CHANGELOG.md
+-rw-r--r--   0 cx1      (20436) team205   (1403)     5120 2022-06-20 15:29:01.000000 celltypist-1.5.1/CITATION.cff
+-rw-r--r--   0 cx1      (20436) team205   (1403)      579 2022-05-31 18:44:35.000000 celltypist-1.5.1/Dockerfile
+-rw-r--r--   0 cx1      (20436) team205   (1403)     1056 2021-05-01 12:32:36.000000 celltypist-1.5.1/LICENSE
+-rw-r--r--   0 cx1      (20436) team205   (1403)      153 2021-12-25 19:53:33.000000 celltypist-1.5.1/MANIFEST.in
+-rw-r--r--   0 cx1      (20436) team205   (1403)    79562 2023-05-26 20:12:55.728300 celltypist-1.5.1/PKG-INFO
+-rw-r--r--   0 cx1      (20436) team205   (1403)    71919 2023-05-16 08:14:33.000000 celltypist-1.5.1/README.md
+drwxr-sr-x   0 cx1      (20436) team205   (1403)        0 2023-05-26 20:12:53.075768 celltypist-1.5.1/celltypist/
+-rw-r--r--   0 cx1      (20436) team205   (1403)      342 2023-05-26 15:22:13.000000 celltypist-1.5.1/celltypist/__init__.py
+-rw-r--r--   0 cx1      (20436) team205   (1403)     6109 2022-08-22 09:17:16.000000 celltypist-1.5.1/celltypist/annotate.py
+-rw-r--r--   0 cx1      (20436) team205   (1403)    27204 2022-08-22 12:28:50.000000 celltypist-1.5.1/celltypist/classifier.py
+-rw-r--r--   0 cx1      (20436) team205   (1403)     7421 2022-01-26 22:00:20.000000 celltypist-1.5.1/celltypist/command_line.py
+drwxr-sr-x   0 cx1      (20436) team205   (1403)        0 2023-05-26 20:12:53.321554 celltypist-1.5.1/celltypist/contro/
+-rw-r--r--   0 cx1      (20436) team205   (1403)        0 2023-05-02 08:46:42.000000 celltypist-1.5.1/celltypist/contro/__init__.py
+-rw-r--r--   0 cx1      (20436) team205   (1403)    33894 2023-05-15 20:57:38.000000 celltypist-1.5.1/celltypist/contro/align.py
+-rw-r--r--   0 cx1      (20436) team205   (1403)    26363 2023-05-02 08:46:42.000000 celltypist-1.5.1/celltypist/contro/distance.py
+-rw-r--r--   0 cx1      (20436) team205   (1403)    11379 2023-05-02 08:46:42.000000 celltypist-1.5.1/celltypist/contro/distances.py
+-rw-r--r--   0 cx1      (20436) team205   (1403)     8310 2023-05-15 21:15:07.000000 celltypist-1.5.1/celltypist/contro/harmonize.py
+-rw-r--r--   0 cx1      (20436) team205   (1403)    15932 2023-05-02 08:46:42.000000 celltypist-1.5.1/celltypist/contro/integrate.py
+-rw-r--r--   0 cx1      (20436) team205   (1403)     9960 2023-05-26 14:15:16.000000 celltypist-1.5.1/celltypist/contro/pct.py
+-rw-r--r--   0 cx1      (20436) team205   (1403)    30047 2023-05-02 08:46:42.000000 celltypist-1.5.1/celltypist/contro/plot.py
+-rw-r--r--   0 cx1      (20436) team205   (1403)      109 2023-05-02 08:46:42.000000 celltypist-1.5.1/celltypist/contro/symbols.py
+drwxr-sr-x   0 cx1      (20436) team205   (1403)        0 2023-05-26 20:12:52.798330 celltypist-1.5.1/celltypist/data/
+drwxr-sr-x   0 cx1      (20436) team205   (1403)        0 2023-05-26 20:12:53.410906 celltypist-1.5.1/celltypist/data/samples/
+-rw-r--r--   0 cx1      (20436) team205   (1403)   557901 2022-01-27 10:03:11.000000 celltypist-1.5.1/celltypist/data/samples/Ensembl105_Human2Mouse_Genes.csv
+-rw-r--r--   0 cx1      (20436) team205   (1403) 53473636 2021-05-01 12:32:37.000000 celltypist-1.5.1/celltypist/data/samples/sample_cell_by_gene.csv
+-rw-r--r--   0 cx1      (20436) team205   (1403)      226 2021-05-01 12:32:37.000000 celltypist-1.5.1/celltypist/logger.py
+-rw-r--r--   0 cx1      (20436) team205   (1403)    20972 2022-12-14 17:45:50.000000 celltypist-1.5.1/celltypist/models.py
+-rw-r--r--   0 cx1      (20436) team205   (1403)    10071 2023-05-02 08:46:42.000000 celltypist-1.5.1/celltypist/plot.py
+-rw-r--r--   0 cx1      (20436) team205   (1403)     4157 2022-08-22 08:57:00.000000 celltypist-1.5.1/celltypist/samples.py
+-rw-r--r--   0 cx1      (20436) team205   (1403)    19188 2023-05-02 08:46:42.000000 celltypist-1.5.1/celltypist/train.py
+drwxr-sr-x   0 cx1      (20436) team205   (1403)        0 2023-05-26 20:12:53.144167 celltypist-1.5.1/celltypist.egg-info/
+-rw-r--r--   0 cx1      (20436) team205   (1403)    79562 2023-05-26 20:12:47.000000 celltypist-1.5.1/celltypist.egg-info/PKG-INFO
+-rw-r--r--   0 cx1      (20436) team205   (1403)     1921 2023-05-26 20:12:49.000000 celltypist-1.5.1/celltypist.egg-info/SOURCES.txt
+-rw-r--r--   0 cx1      (20436) team205   (1403)        1 2023-05-26 20:12:47.000000 celltypist-1.5.1/celltypist.egg-info/dependency_links.txt
+-rw-r--r--   0 cx1      (20436) team205   (1403)       61 2023-05-26 20:12:47.000000 celltypist-1.5.1/celltypist.egg-info/entry_points.txt
+-rw-r--r--   0 cx1      (20436) team205   (1403)      140 2023-05-26 20:12:47.000000 celltypist-1.5.1/celltypist.egg-info/requires.txt
+-rw-r--r--   0 cx1      (20436) team205   (1403)       11 2023-05-26 20:12:47.000000 celltypist-1.5.1/celltypist.egg-info/top_level.txt
+drwxr-sr-x   0 cx1      (20436) team205   (1403)        0 2023-05-26 20:12:54.907161 celltypist-1.5.1/docs/
+-rw-r--r--   0 cx1      (20436) team205   (1403)      638 2021-05-01 12:32:37.000000 celltypist-1.5.1/docs/Makefile
+drwxr-sr-x   0 cx1      (20436) team205   (1403)        0 2023-05-26 20:12:55.198731 celltypist-1.5.1/docs/notebook/
+-rw-r--r--   0 cx1      (20436) team205   (1403)   376236 2022-08-23 10:52:31.000000 celltypist-1.5.1/docs/notebook/celltypist_tutorial.ipynb
+-rw-r--r--   0 cx1      (20436) team205   (1403)   552805 2022-08-23 13:32:51.000000 celltypist-1.5.1/docs/notebook/celltypist_tutorial_cv.ipynb
+-rw-r--r--   0 cx1      (20436) team205   (1403)  1512368 2023-05-16 11:01:52.000000 celltypist-1.5.1/docs/notebook/celltypist_tutorial_harmonisation.ipynb
+-rw-r--r--   0 cx1      (20436) team205   (1403)  3075328 2023-05-16 19:05:14.000000 celltypist-1.5.1/docs/notebook/celltypist_tutorial_integration.ipynb
+-rw-r--r--   0 cx1      (20436) team205   (1403)   629323 2022-08-23 12:38:41.000000 celltypist-1.5.1/docs/notebook/celltypist_tutorial_ml.ipynb
+-rw-r--r--   0 cx1      (20436) team205   (1403)      225 2023-05-02 08:46:43.000000 celltypist-1.5.1/docs/requirements.txt
+drwxr-sr-x   0 cx1      (20436) team205   (1403)        0 2023-05-26 20:12:55.629197 celltypist-1.5.1/docs/source/
+drwxr-sr-x   0 cx1      (20436) team205   (1403)        0 2023-05-26 20:12:52.809245 celltypist-1.5.1/docs/source/_static/
+drwxr-sr-x   0 cx1      (20436) team205   (1403)        0 2023-05-26 20:12:55.692237 celltypist-1.5.1/docs/source/_static/img/
+-rw-r--r--   0 cx1      (20436) team205   (1403)    67929 2021-11-02 03:08:25.000000 celltypist-1.5.1/docs/source/_static/img/logo_celltypist.png
+-rw-r--r--   0 cx1      (20436) team205   (1403)       83 2022-08-05 12:50:13.000000 celltypist-1.5.1/docs/source/celltypist.annotate.rst
+-rw-r--r--   0 cx1      (20436) team205   (1403)      156 2022-08-05 13:11:23.000000 celltypist-1.5.1/docs/source/celltypist.classifier.AnnotationResult.rst
+-rw-r--r--   0 cx1      (20436) team205   (1403)      153 2022-08-05 13:12:18.000000 celltypist-1.5.1/docs/source/celltypist.classifier.Classifier.rst
+-rw-r--r--   0 cx1      (20436) team205   (1403)      162 2023-05-02 08:46:43.000000 celltypist-1.5.1/docs/source/celltypist.contro.align.DistanceAlignment.rst
+-rw-r--r--   0 cx1      (20436) team205   (1403)      154 2023-05-02 08:46:43.000000 celltypist-1.5.1/docs/source/celltypist.contro.distance.Distance.rst
+-rw-r--r--   0 cx1      (20436) team205   (1403)      161 2023-05-02 08:46:43.000000 celltypist-1.5.1/docs/source/celltypist.contro.pct.PredictiveClusteringTree.rst
+-rw-r--r--   0 cx1      (20436) team205   (1403)       80 2023-05-02 08:46:43.000000 celltypist-1.5.1/docs/source/celltypist.dotplot.rst
+-rw-r--r--   0 cx1      (20436) team205   (1403)       87 2023-05-02 08:46:43.000000 celltypist-1.5.1/docs/source/celltypist.harmonize.rst
+-rw-r--r--   0 cx1      (20436) team205   (1403)       85 2023-05-02 08:46:43.000000 celltypist-1.5.1/docs/source/celltypist.integrate.rst
+-rw-r--r--   0 cx1      (20436) team205   (1403)      139 2022-08-05 13:13:01.000000 celltypist-1.5.1/docs/source/celltypist.models.Model.rst
+-rw-r--r--   0 cx1      (20436) team205   (1403)      101 2022-08-05 13:30:15.000000 celltypist-1.5.1/docs/source/celltypist.models.download_models.rst
+-rw-r--r--   0 cx1      (20436) team205   (1403)      101 2022-08-05 12:49:53.000000 celltypist-1.5.1/docs/source/celltypist.samples.downsample_adata.rst
+-rw-r--r--   0 cx1      (20436) team205   (1403)       86 2023-05-02 08:46:43.000000 celltypist-1.5.1/docs/source/celltypist.sankeyplot.rst
+-rw-r--r--   0 cx1      (20436) team205   (1403)       78 2022-08-05 12:50:03.000000 celltypist-1.5.1/docs/source/celltypist.train.rst
+-rw-r--r--   0 cx1      (20436) team205   (1403)       82 2023-05-02 08:46:43.000000 celltypist-1.5.1/docs/source/celltypist.treeplot.rst
+-rw-r--r--   0 cx1      (20436) team205   (1403)     2872 2023-05-02 08:46:43.000000 celltypist-1.5.1/docs/source/conf.py
+-rw-r--r--   0 cx1      (20436) team205   (1403)     1602 2023-05-02 08:46:43.000000 celltypist-1.5.1/docs/source/index.rst
+-rw-r--r--   0 cx1      (20436) team205   (1403)      140 2023-05-02 08:46:43.000000 celltypist-1.5.1/requirements.txt
+-rw-r--r--   0 cx1      (20436) team205   (1403)       38 2023-05-26 20:12:55.733969 celltypist-1.5.1/setup.cfg
+-rw-r--r--   0 cx1      (20436) team205   (1403)     1519 2023-05-02 08:46:43.000000 celltypist-1.5.1/setup.py
```

### Comparing `celltypist-1.5.0/CHANGELOG.md` & `celltypist-1.5.1/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Changelog
 *********************************
+## CellTypist 1.5.1 (May 26, 2023)
+Fix error in not importing spmatrix in pct
 ## CellTypist 1.5.0 (May 16, 2023)
 A more mature release before the formal CellTypist v2
 ## CellTypist 1.4.0 (May 2, 2023)
 - Add modules of cell type harmonisation and integration (a release before the formal CellTypist v2)
 ## CellTypist 1.3.0 (December 14, 2022)
 - Transfer numpy matrix to array during prediction for compatibility with sklearn >= 1.0 [#50](https://github.com/Teichlab/celltypist/issues/50)
 ## CellTypist 1.2.0 (August 22, 2022)
```

### Comparing `celltypist-1.5.0/CITATION.cff` & `celltypist-1.5.1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.0/Dockerfile` & `celltypist-1.5.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.0/LICENSE` & `celltypist-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.0/PKG-INFO` & `celltypist-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: celltypist
-Version: 1.5.0
+Version: 1.5.1
 Summary: A tool for semi-automatic cell type classification, harmonization and integration
 Home-page: https://github.com/Teichlab/celltypist
 Author: Chuan Xu
 Author-email: cx1@sanger.ac.uk
 License: UNKNOWN
 Description: <p align="left"><img src="https://github.com/Teichlab/celltypist/blob/main/docs/source/_static/img/logo_celltypist.png" width="250" height="85"></p>
```

### Comparing `celltypist-1.5.0/README.md` & `celltypist-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.0/celltypist/annotate.py` & `celltypist-1.5.1/celltypist/annotate.py`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.0/celltypist/classifier.py` & `celltypist-1.5.1/celltypist/classifier.py`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.0/celltypist/command_line.py` & `celltypist-1.5.1/celltypist/command_line.py`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.0/celltypist/contro/align.py` & `celltypist-1.5.1/celltypist/contro/align.py`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.0/celltypist/contro/distance.py` & `celltypist-1.5.1/celltypist/contro/distance.py`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.0/celltypist/contro/distances.py` & `celltypist-1.5.1/celltypist/contro/distances.py`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.0/celltypist/contro/harmonize.py` & `celltypist-1.5.1/celltypist/contro/harmonize.py`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.0/celltypist/contro/integrate.py` & `celltypist-1.5.1/celltypist/contro/integrate.py`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.0/celltypist/contro/pct.py` & `celltypist-1.5.1/celltypist/contro/pct.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from sklearn.tree._tree import TREE_LEAF, TREE_UNDEFINED
 from sklearn.tree import DecisionTreeRegressor
 from sklearn import __version__ as skv
 import numpy as np
 from scipy.stats import f
+from scipy.sparse import spmatrix
 from typing import Optional, Union
 from .. import logger
 
 class PredictiveClusteringTree(DecisionTreeRegressor):
     """
     Class that uses predictive clustering trees (PCT) for multi-output prediction.
     Note this is a specialized PCT with the prototype as the mean vector and the distance measure as the (sum of) intra-cluster variance.
```

### Comparing `celltypist-1.5.0/celltypist/contro/plot.py` & `celltypist-1.5.1/celltypist/contro/plot.py`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.0/celltypist/data/samples/Ensembl105_Human2Mouse_Genes.csv` & `celltypist-1.5.1/celltypist/data/samples/Ensembl105_Human2Mouse_Genes.csv`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.0/celltypist/data/samples/sample_cell_by_gene.csv` & `celltypist-1.5.1/celltypist/data/samples/sample_cell_by_gene.csv`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.0/celltypist/models.py` & `celltypist-1.5.1/celltypist/models.py`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.0/celltypist/plot.py` & `celltypist-1.5.1/celltypist/plot.py`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.0/celltypist/samples.py` & `celltypist-1.5.1/celltypist/samples.py`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.0/celltypist/train.py` & `celltypist-1.5.1/celltypist/train.py`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.0/celltypist.egg-info/PKG-INFO` & `celltypist-1.5.1/celltypist.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: celltypist
-Version: 1.5.0
+Version: 1.5.1
 Summary: A tool for semi-automatic cell type classification, harmonization and integration
 Home-page: https://github.com/Teichlab/celltypist
 Author: Chuan Xu
 Author-email: cx1@sanger.ac.uk
 License: UNKNOWN
 Description: <p align="left"><img src="https://github.com/Teichlab/celltypist/blob/main/docs/source/_static/img/logo_celltypist.png" width="250" height="85"></p>
```

### Comparing `celltypist-1.5.0/celltypist.egg-info/SOURCES.txt` & `celltypist-1.5.1/celltypist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.0/docs/Makefile` & `celltypist-1.5.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.0/docs/notebook/celltypist_tutorial.ipynb` & `celltypist-1.5.1/docs/notebook/celltypist_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.0/docs/notebook/celltypist_tutorial_cv.ipynb` & `celltypist-1.5.1/docs/notebook/celltypist_tutorial_cv.ipynb`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.0/docs/notebook/celltypist_tutorial_harmonisation.ipynb` & `celltypist-1.5.1/docs/notebook/celltypist_tutorial_harmonisation.ipynb`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.0/docs/notebook/celltypist_tutorial_integration.ipynb` & `celltypist-1.5.1/docs/notebook/celltypist_tutorial_integration.ipynb`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.0/docs/notebook/celltypist_tutorial_ml.ipynb` & `celltypist-1.5.1/docs/notebook/celltypist_tutorial_ml.ipynb`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.0/docs/source/_static/img/logo_celltypist.png` & `celltypist-1.5.1/docs/source/_static/img/logo_celltypist.png`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.0/docs/source/conf.py` & `celltypist-1.5.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.0/docs/source/index.rst` & `celltypist-1.5.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.0/setup.py` & `celltypist-1.5.1/setup.py`

 * *Files identical despite different names*

