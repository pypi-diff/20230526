# Comparing `tmp/jupyterlab-training-0.4.0.tar.gz` & `tmp/jupyterlab-training-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterlab-training-0.4.0.tar", last modified: Fri May 26 07:18:07 2023, max compression
+gzip compressed data, was "jupyterlab-training-0.4.1.tar", last modified: Fri May 26 07:27:39 2023, max compression
```

## Comparing `jupyterlab-training-0.4.0.tar` & `jupyterlab-training-0.4.1.tar`

### file list

```diff
@@ -1,9 +1,13 @@
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-26 07:18:07.793664 jupyterlab-training-0.4.0/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      305 2023-05-26 07:18:07.793664 jupyterlab-training-0.4.0/PKG-INFO
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-26 07:18:07.793664 jupyterlab-training-0.4.0/jupyterlab_training.egg-info/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      305 2023-05-26 07:18:07.000000 jupyterlab-training-0.4.0/jupyterlab_training.egg-info/PKG-INFO
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      186 2023-05-26 07:18:07.000000 jupyterlab-training-0.4.0/jupyterlab_training.egg-info/SOURCES.txt
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)        1 2023-05-26 07:18:07.000000 jupyterlab-training-0.4.0/jupyterlab_training.egg-info/dependency_links.txt
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)        1 2023-05-26 07:18:07.000000 jupyterlab-training-0.4.0/jupyterlab_training.egg-info/top_level.txt
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      456 2023-05-26 07:16:25.000000 jupyterlab-training-0.4.0/pyproject.toml
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       38 2023-05-26 07:18:07.793664 jupyterlab-training-0.4.0/setup.cfg
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-26 07:27:39.844007 jupyterlab-training-0.4.1/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      305 2023-05-26 07:27:39.844007 jupyterlab-training-0.4.1/PKG-INFO
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       53 2023-05-26 07:19:07.000000 jupyterlab-training-0.4.1/README.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      456 2023-05-26 07:26:49.000000 jupyterlab-training-0.4.1/pyproject.toml
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       38 2023-05-26 07:27:39.844007 jupyterlab-training-0.4.1/setup.cfg
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-26 07:27:39.840007 jupyterlab-training-0.4.1/src/
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-26 07:27:39.844007 jupyterlab-training-0.4.1/src/jupyterlab_training/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1906 2023-05-26 07:13:15.000000 jupyterlab-training-0.4.1/src/jupyterlab_training/__init__.py
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-26 07:27:39.844007 jupyterlab-training-0.4.1/src/jupyterlab_training.egg-info/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      305 2023-05-26 07:27:39.000000 jupyterlab-training-0.4.1/src/jupyterlab_training.egg-info/PKG-INFO
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      248 2023-05-26 07:27:39.000000 jupyterlab-training-0.4.1/src/jupyterlab_training.egg-info/SOURCES.txt
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)        1 2023-05-26 07:27:39.000000 jupyterlab-training-0.4.1/src/jupyterlab_training.egg-info/dependency_links.txt
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       20 2023-05-26 07:27:39.000000 jupyterlab-training-0.4.1/src/jupyterlab_training.egg-info/top_level.txt
```

