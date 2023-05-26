# Comparing `tmp/discopy-1.1.1.tar.gz` & `tmp/discopy-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discopy-1.1.1.tar", last modified: Wed May 24 09:47:47 2023, max compression
+gzip compressed data, was "discopy-1.1.2.tar", last modified: Fri May 26 07:43:50 2023, max compression
```

## Comparing `discopy-1.1.1.tar` & `discopy-1.1.2.tar`

### file list

```diff
@@ -1,55 +1,274 @@
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-24 09:47:47.934155 discopy-1.1.1/
--rw-r--r--   0 aleumi     (502) staff       (20)     1520 2023-04-18 08:36:50.000000 discopy-1.1.1/LICENSE
--rw-r--r--   0 aleumi     (502) staff       (20)     5160 2023-05-24 09:47:47.934454 discopy-1.1.1/PKG-INFO
--rw-r--r--   0 aleumi     (502) staff       (20)     4532 2023-05-24 09:11:24.000000 discopy-1.1.1/README.md
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-24 09:47:47.806580 discopy-1.1.1/discopy/
--rw-r--r--   0 aleumi     (502) staff       (20)      424 2023-05-24 09:43:27.000000 discopy-1.1.1/discopy/__init__.py
--rw-r--r--   0 aleumi     (502) staff       (20)     5758 2023-05-23 16:32:40.000000 discopy-1.1.1/discopy/balanced.py
--rw-r--r--   0 aleumi     (502) staff       (20)     8328 2023-05-24 09:11:24.000000 discopy-1.1.1/discopy/braided.py
--rw-r--r--   0 aleumi     (502) staff       (20)    28200 2023-05-23 16:32:41.000000 discopy-1.1.1/discopy/cat.py
--rw-r--r--   0 aleumi     (502) staff       (20)    10182 2023-05-24 09:11:24.000000 discopy-1.1.1/discopy/closed.py
--rw-r--r--   0 aleumi     (502) staff       (20)     4417 2023-05-24 09:11:24.000000 discopy-1.1.1/discopy/compact.py
--rw-r--r--   0 aleumi     (502) staff       (20)     1487 2023-05-24 09:11:24.000000 discopy-1.1.1/discopy/config.py
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-24 09:47:47.823189 discopy-1.1.1/discopy/drawing/
--rw-r--r--   0 aleumi     (502) staff       (20)     1060 2023-05-23 16:32:40.000000 discopy-1.1.1/discopy/drawing/__init__.py
--rw-r--r--   0 aleumi     (502) staff       (20)    13920 2023-05-23 16:33:01.000000 discopy-1.1.1/discopy/drawing/grid.py
--rw-r--r--   0 aleumi     (502) staff       (20)    36769 2023-05-24 09:11:24.000000 discopy-1.1.1/discopy/drawing/legacy.py
--rw-r--r--   0 aleumi     (502) staff       (20)    11613 2023-05-24 09:11:24.000000 discopy-1.1.1/discopy/frobenius.py
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-24 09:47:47.837362 discopy-1.1.1/discopy/grammar/
--rw-r--r--   0 aleumi     (502) staff       (20)      225 2023-04-18 08:36:50.000000 discopy-1.1.1/discopy/grammar/__init__.py
--rw-r--r--   0 aleumi     (502) staff       (20)     9405 2023-05-24 09:11:24.000000 discopy-1.1.1/discopy/grammar/categorial.py
--rw-r--r--   0 aleumi     (502) staff       (20)     6890 2023-04-18 08:36:50.000000 discopy-1.1.1/discopy/grammar/cfg.py
--rw-r--r--   0 aleumi     (502) staff       (20)      926 2023-04-18 08:36:50.000000 discopy-1.1.1/discopy/grammar/dependency.py
--rw-r--r--   0 aleumi     (502) staff       (20)     7162 2023-05-24 09:11:24.000000 discopy-1.1.1/discopy/grammar/pregroup.py
--rw-r--r--   0 aleumi     (502) staff       (20)     2410 2023-05-24 09:11:24.000000 discopy-1.1.1/discopy/grammar/thue.py
--rw-r--r--   0 aleumi     (502) staff       (20)    48280 2023-05-24 09:11:24.000000 discopy-1.1.1/discopy/hypergraph.py
--rw-r--r--   0 aleumi     (502) staff       (20)    14028 2023-05-24 09:11:24.000000 discopy-1.1.1/discopy/interaction.py
--rw-r--r--   0 aleumi     (502) staff       (20)     8050 2023-05-24 09:11:24.000000 discopy-1.1.1/discopy/markov.py
--rw-r--r--   0 aleumi     (502) staff       (20)    16146 2023-05-24 09:11:24.000000 discopy-1.1.1/discopy/matrix.py
--rw-r--r--   0 aleumi     (502) staff       (20)     1555 2023-05-24 09:11:24.000000 discopy-1.1.1/discopy/messages.py
--rw-r--r--   0 aleumi     (502) staff       (20)    35222 2023-05-24 09:11:24.000000 discopy-1.1.1/discopy/monoidal.py
--rw-r--r--   0 aleumi     (502) staff       (20)     6871 2023-05-23 16:31:13.000000 discopy-1.1.1/discopy/pivotal.py
--rw-r--r--   0 aleumi     (502) staff       (20)     7845 2023-05-23 16:32:40.000000 discopy-1.1.1/discopy/python.py
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-24 09:47:47.928962 discopy-1.1.1/discopy/quantum/
--rw-r--r--   0 aleumi     (502) staff       (20)      667 2023-04-18 08:36:50.000000 discopy-1.1.1/discopy/quantum/__init__.py
--rw-r--r--   0 aleumi     (502) staff       (20)     5238 2023-04-18 08:36:50.000000 discopy-1.1.1/discopy/quantum/ansatze.py
--rw-r--r--   0 aleumi     (502) staff       (20)    11626 2023-04-18 08:36:50.000000 discopy-1.1.1/discopy/quantum/channel.py
--rw-r--r--   0 aleumi     (502) staff       (20)    32818 2023-05-24 09:11:24.000000 discopy-1.1.1/discopy/quantum/circuit.py
--rw-r--r--   0 aleumi     (502) staff       (20)    24488 2023-05-24 09:11:24.000000 discopy-1.1.1/discopy/quantum/gates.py
--rw-r--r--   0 aleumi     (502) staff       (20)    15738 2023-05-24 07:55:57.000000 discopy-1.1.1/discopy/quantum/pennylane.py
--rw-r--r--   0 aleumi     (502) staff       (20)    16429 2023-05-24 07:55:57.000000 discopy-1.1.1/discopy/quantum/tk.py
--rw-r--r--   0 aleumi     (502) staff       (20)    13451 2023-05-23 16:32:40.000000 discopy-1.1.1/discopy/quantum/zx.py
--rw-r--r--   0 aleumi     (502) staff       (20)     6916 2023-05-23 16:31:12.000000 discopy-1.1.1/discopy/ribbon.py
--rw-r--r--   0 aleumi     (502) staff       (20)    25765 2023-05-24 09:11:24.000000 discopy-1.1.1/discopy/rigid.py
--rw-r--r--   0 aleumi     (502) staff       (20)     9007 2023-05-24 09:11:24.000000 discopy-1.1.1/discopy/symmetric.py
--rw-r--r--   0 aleumi     (502) staff       (20)    23082 2023-05-24 09:11:24.000000 discopy-1.1.1/discopy/tensor.py
--rw-r--r--   0 aleumi     (502) staff       (20)     7593 2023-05-23 16:32:41.000000 discopy-1.1.1/discopy/traced.py
--rw-r--r--   0 aleumi     (502) staff       (20)    20851 2023-05-24 09:11:24.000000 discopy-1.1.1/discopy/utils.py
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-24 09:47:47.815242 discopy-1.1.1/discopy.egg-info/
--rw-r--r--   0 aleumi     (502) staff       (20)     5160 2023-05-24 09:47:46.000000 discopy-1.1.1/discopy.egg-info/PKG-INFO
--rw-r--r--   0 aleumi     (502) staff       (20)     1055 2023-05-24 09:47:47.000000 discopy-1.1.1/discopy.egg-info/SOURCES.txt
--rw-r--r--   0 aleumi     (502) staff       (20)        1 2023-05-24 09:47:46.000000 discopy-1.1.1/discopy.egg-info/dependency_links.txt
--rw-r--r--   0 aleumi     (502) staff       (20)      412 2023-05-24 09:47:46.000000 discopy-1.1.1/discopy.egg-info/requires.txt
--rw-r--r--   0 aleumi     (502) staff       (20)        8 2023-05-24 09:47:46.000000 discopy-1.1.1/discopy.egg-info/top_level.txt
--rw-r--r--   0 aleumi     (502) staff       (20)      208 2023-05-24 09:47:47.938768 discopy-1.1.1/setup.cfg
--rw-r--r--   0 aleumi     (502) staff       (20)     2185 2023-05-24 09:37:47.000000 discopy-1.1.1/setup.py
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:50.251029 discopy-1.1.2/
+-rw-r--r--   0 aleumi     (502) staff       (20)       33 2023-05-26 07:41:40.000000 discopy-1.1.2/.gitattributes
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:49.822315 discopy-1.1.2/.github/
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:49.850671 discopy-1.1.2/.github/workflows/
+-rw-r--r--   0 aleumi     (502) staff       (20)     1606 2023-05-26 07:41:40.000000 discopy-1.1.2/.github/workflows/build_test.yml
+-rw-r--r--   0 aleumi     (502) staff       (20)      183 2023-05-26 07:41:40.000000 discopy-1.1.2/.gitignore
+-rw-r--r--   0 aleumi     (502) staff       (20)    20606 2023-05-26 07:41:40.000000 discopy-1.1.2/.pylintrc
+-rw-r--r--   0 aleumi     (502) staff       (20)      744 2023-05-26 07:41:40.000000 discopy-1.1.2/.readthedocs.yaml
+-rw-r--r--   0 aleumi     (502) staff       (20)     1171 2023-05-26 07:41:40.000000 discopy-1.1.2/CONTRIBUTING.md
+-rw-r--r--   0 aleumi     (502) staff       (20)     1520 2023-05-26 07:41:40.000000 discopy-1.1.2/LICENSE
+-rw-r--r--   0 aleumi     (502) staff       (20)     5596 2023-05-26 07:43:50.251977 discopy-1.1.2/PKG-INFO
+-rw-r--r--   0 aleumi     (502) staff       (20)     4532 2023-05-26 07:41:40.000000 discopy-1.1.2/README.md
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:49.885085 discopy-1.1.2/discopy/
+-rw-r--r--   0 aleumi     (502) staff       (20)      499 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/__init__.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     5758 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/balanced.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     8328 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/braided.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    28200 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/cat.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    10182 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/closed.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     4417 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/compact.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     1487 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/config.py
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:49.894222 discopy-1.1.2/discopy/drawing/
+-rw-r--r--   0 aleumi     (502) staff       (20)     1060 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/drawing/__init__.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    13920 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/drawing/grid.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    36769 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/drawing/legacy.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    11613 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/frobenius.py
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:49.901668 discopy-1.1.2/discopy/grammar/
+-rw-r--r--   0 aleumi     (502) staff       (20)      225 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/grammar/__init__.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     9405 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/grammar/categorial.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     6890 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/grammar/cfg.py
+-rw-r--r--   0 aleumi     (502) staff       (20)      926 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/grammar/dependency.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     7162 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/grammar/pregroup.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     2410 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/grammar/thue.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    48318 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/hypergraph.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    14028 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/interaction.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     8050 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/markov.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    16146 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/matrix.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     1555 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/messages.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    35222 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/monoidal.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     6871 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/pivotal.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     7845 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/python.py
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:49.916584 discopy-1.1.2/discopy/quantum/
+-rw-r--r--   0 aleumi     (502) staff       (20)      667 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/quantum/__init__.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     5238 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/quantum/ansatze.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    11626 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/quantum/channel.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    32818 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/quantum/circuit.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    24488 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/quantum/gates.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    15738 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/quantum/pennylane.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    16429 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/quantum/tk.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    13451 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/quantum/zx.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     6916 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/ribbon.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    25765 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/rigid.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     9007 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/symmetric.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    23082 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/tensor.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     7593 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/traced.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    20851 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/utils.py
+-rw-r--r--   0 aleumi     (502) staff       (20)      160 2023-05-26 07:43:49.000000 discopy-1.1.2/discopy/version.py
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:49.891931 discopy-1.1.2/discopy.egg-info/
+-rw-r--r--   0 aleumi     (502) staff       (20)     5596 2023-05-26 07:43:49.000000 discopy-1.1.2/discopy.egg-info/PKG-INFO
+-rw-r--r--   0 aleumi     (502) staff       (20)     6584 2023-05-26 07:43:49.000000 discopy-1.1.2/discopy.egg-info/SOURCES.txt
+-rw-r--r--   0 aleumi     (502) staff       (20)        1 2023-05-26 07:43:49.000000 discopy-1.1.2/discopy.egg-info/dependency_links.txt
+-rw-r--r--   0 aleumi     (502) staff       (20)      412 2023-05-26 07:43:49.000000 discopy-1.1.2/discopy.egg-info/requires.txt
+-rw-r--r--   0 aleumi     (502) staff       (20)        8 2023-05-26 07:43:49.000000 discopy-1.1.2/discopy.egg-info/top_level.txt
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:49.922870 discopy-1.1.2/docs/
+-rw-r--r--   0 aleumi     (502) staff       (20)      634 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/Makefile
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:49.926526 discopy-1.1.2/docs/_ext/
+-rw-r--r--   0 aleumi     (502) staff       (20)      684 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_ext/bases-fullname.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     3939 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_ext/youtube.py
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:49.930633 discopy-1.1.2/docs/_static/
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:49.938638 discopy-1.1.2/docs/_static/balanced/
+-rw-r--r--   0 aleumi     (502) staff       (20)    14901 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/balanced/ribbon_twist.png
+-rw-r--r--   0 aleumi     (502) staff       (20)    13367 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/balanced/twist.png
+-rw-r--r--   0 aleumi     (502) staff       (20)    11712 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/balanced/twist_dual_rail.png
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:49.940632 discopy-1.1.2/docs/_static/braided/
+-rw-r--r--   0 aleumi     (502) staff       (20)     8951 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/braided/hexagons.png
+-rw-r--r--   0 aleumi     (502) staff       (20)     9432 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/braided/inverse.png
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:49.944285 discopy-1.1.2/docs/_static/closed/
+-rw-r--r--   0 aleumi     (502) staff       (20)    15711 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/closed/curry-left.png
+-rw-r--r--   0 aleumi     (502) staff       (20)    15643 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/closed/curry-right.png
+-rw-r--r--   0 aleumi     (502) staff       (20)    19051 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/closed/uncurry.png
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:49.950817 discopy-1.1.2/docs/_static/compact/
+-rw-r--r--   0 aleumi     (502) staff       (20)    14358 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/compact/reidemeister.png
+-rw-r--r--   0 aleumi     (502) staff       (20)    10190 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/compact/snake.png
+-rw-r--r--   0 aleumi     (502) staff       (20)    14358 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/compact/yanking.png
+-rw-r--r--   0 aleumi     (502) staff       (20)    14061 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/compact/yanking_cup_and_cap.png
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:49.953606 discopy-1.1.2/docs/_static/drawing/
+-rw-r--r--   0 aleumi     (502) staff       (20)     5271 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/drawing/diagramize.png
+-rw-r--r--   0 aleumi     (502) staff       (20)     3578 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/drawing/example.html
+-rw-r--r--   0 aleumi     (502) staff       (20)    10626 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/drawing/frobenius-axioms.png
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:49.960041 discopy-1.1.2/docs/_static/frobenius/
+-rw-r--r--   0 aleumi     (502) staff       (20)    17147 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/frobenius/comonoid.png
+-rw-r--r--   0 aleumi     (502) staff       (20)    14853 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/frobenius/frobenius.png
+-rw-r--r--   0 aleumi     (502) staff       (20)    17266 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/frobenius/monoid.png
+-rw-r--r--   0 aleumi     (502) staff       (20)     9884 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/frobenius/special.png
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:49.963013 discopy-1.1.2/docs/_static/grammar/
+-rw-r--r--   0 aleumi     (502) staff       (20)     9591 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/grammar/cfg-example.png
+-rw-r--r--   0 aleumi     (502) staff       (20)     7224 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/grammar/pregroup-example.png
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:49.968364 discopy-1.1.2/docs/_static/hypergraph/
+-rw-r--r--   0 aleumi     (502) staff       (20)    16894 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/hypergraph/box.png
+-rw-r--r--   0 aleumi     (502) staff       (20)    20670 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/hypergraph/diagram.png
+-rw-r--r--   0 aleumi     (502) staff       (20)    15394 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/hypergraph/unfuse.png
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:49.982288 discopy-1.1.2/docs/_static/int/
+-rw-r--r--   0 aleumi     (502) staff       (20)    16145 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/int/alice-loves-bob.png
+-rw-r--r--   0 aleumi     (502) staff       (20)    18363 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/int/braid.png
+-rw-r--r--   0 aleumi     (502) staff       (20)    16332 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/int/composition.png
+-rw-r--r--   0 aleumi     (502) staff       (20)     8274 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/int/dagger.png
+-rw-r--r--   0 aleumi     (502) staff       (20)    16257 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/int/idl.png
+-rw-r--r--   0 aleumi     (502) staff       (20)    16615 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/int/idr.png
+-rw-r--r--   0 aleumi     (502) staff       (20)    16069 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/int/int-snake-equations.png
+-rw-r--r--   0 aleumi     (502) staff       (20)    22712 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/int/simplify.png
+-rw-r--r--   0 aleumi     (502) staff       (20)    16278 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/int/tensor.png
+-rw-r--r--   0 aleumi     (502) staff       (20)   105662 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/logo.ico
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:49.985865 discopy-1.1.2/docs/_static/markov/
+-rw-r--r--   0 aleumi     (502) staff       (20)    13158 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/markov/associativity.png
+-rw-r--r--   0 aleumi     (502) staff       (20)    14407 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/markov/bialgebra.png
+-rw-r--r--   0 aleumi     (502) staff       (20)    10317 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/markov/copy_and_apply.png
+-rw-r--r--   0 aleumi     (502) staff       (20)     8979 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/markov/counit.png
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:50.009502 discopy-1.1.2/docs/_static/monoidal/
+-rw-r--r--   0 aleumi     (502) staff       (20)     2875 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/monoidal/Eckmann-Hilton.gif
+-rw-r--r--   0 aleumi     (502) staff       (20)    12008 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/monoidal/EckmannHilton.gif
+-rw-r--r--   0 aleumi     (502) staff       (20)     3504 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/monoidal/arrow-example.png
+-rw-r--r--   0 aleumi     (502) staff       (20)     2166 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/monoidal/box-example.png
+-rw-r--r--   0 aleumi     (502) staff       (20)    14662 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/monoidal/bubble-example.png
+-rw-r--r--   0 aleumi     (502) staff       (20)    10047 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/monoidal/foliate-example-1.png
+-rw-r--r--   0 aleumi     (502) staff       (20)     7535 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/monoidal/foliate-example-1a.png
+-rw-r--r--   0 aleumi     (502) staff       (20)     7221 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/monoidal/foliate-example-1b.png
+-rw-r--r--   0 aleumi     (502) staff       (20)     4433 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/monoidal/foliate-example-2.png
+-rw-r--r--   0 aleumi     (502) staff       (20)     7089 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/monoidal/functor-example.png
+-rw-r--r--   0 aleumi     (502) staff       (20)     2617 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/monoidal/id-example.png
+-rw-r--r--   0 aleumi     (502) staff       (20)   404531 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/monoidal/spiral.gif
+-rw-r--r--   0 aleumi     (502) staff       (20)     2888 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/monoidal/tensor-example.png
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:50.012289 discopy-1.1.2/docs/_static/optics/
+-rw-r--r--   0 aleumi     (502) staff       (20)     7259 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/optics/fusion.png
+-rw-r--r--   0 aleumi     (502) staff       (20)    15302 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/optics/spider-decomp.png
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:50.018124 discopy-1.1.2/docs/_static/pivotal/
+-rw-r--r--   0 aleumi     (502) staff       (20)    10105 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/pivotal/axiom.png
+-rw-r--r--   0 aleumi     (502) staff       (20)     6542 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/pivotal/box-conjugate.png
+-rw-r--r--   0 aleumi     (502) staff       (20)     7722 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/pivotal/conjugate.png
+-rw-r--r--   0 aleumi     (502) staff       (20)     6710 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/pivotal/dagger-transpose.png
+-rw-r--r--   0 aleumi     (502) staff       (20)     8451 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/pivotal/dagger.png
+-rw-r--r--   0 aleumi     (502) staff       (20)    10350 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/pivotal/trace.png
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:50.020097 discopy-1.1.2/docs/_static/quantum/
+-rw-r--r--   0 aleumi     (502) staff       (20)    13104 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/quantum/circuit-example.png
+-rw-r--r--   0 aleumi     (502) staff       (20)    17758 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/quantum/functor-example.png
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:50.023476 discopy-1.1.2/docs/_static/ribbon/
+-rw-r--r--   0 aleumi     (502) staff       (20)     6787 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/ribbon/strict.png
+-rw-r--r--   0 aleumi     (502) staff       (20)    15078 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/ribbon/twist-untwist.png
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:50.044074 discopy-1.1.2/docs/_static/rigid/
+-rw-r--r--   0 aleumi     (502) staff       (20)     2296 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/rigid/cap.png
+-rw-r--r--   0 aleumi     (502) staff       (20)     3223 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/rigid/caps.png
+-rw-r--r--   0 aleumi     (502) staff       (20)     2352 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/rigid/cup.png
+-rw-r--r--   0 aleumi     (502) staff       (20)     3131 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/rigid/cups.png
+-rw-r--r--   0 aleumi     (502) staff       (20)     8834 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/rigid/curry.png
+-rw-r--r--   0 aleumi     (502) staff       (20)     4537 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/rigid/diagram-example.png
+-rw-r--r--   0 aleumi     (502) staff       (20)    10267 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/rigid/functor-example.png
+-rw-r--r--   0 aleumi     (502) staff       (20)    11845 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/rigid/rotate.png
+-rw-r--r--   0 aleumi     (502) staff       (20)     9160 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/rigid/transpose.png
+-rw-r--r--   0 aleumi     (502) staff       (20)    13976 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/rigid/transpose_box.png
+-rw-r--r--   0 aleumi     (502) staff       (20)     5315 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/rigid/typed-snake-equation.png
+-rw-r--r--   0 aleumi     (502) staff       (20)     5315 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/snake-equation.png
+-rw-r--r--   0 aleumi     (502) staff       (20)   963196 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/spiral.gif
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:50.054391 discopy-1.1.2/docs/_static/symmetric/
+-rw-r--r--   0 aleumi     (502) staff       (20)    13136 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/symmetric/decorator.png
+-rw-r--r--   0 aleumi     (502) staff       (20)     9819 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/symmetric/hexagons.png
+-rw-r--r--   0 aleumi     (502) staff       (20)     6665 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/symmetric/inverse.png
+-rw-r--r--   0 aleumi     (502) staff       (20)     7307 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/symmetric/naturality.png
+-rw-r--r--   0 aleumi     (502) staff       (20)    10124 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/symmetric/yang-baxter.png
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:50.065539 discopy-1.1.2/docs/_static/tensor/
+-rw-r--r--   0 aleumi     (502) staff       (20)    17466 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/tensor/chain-rule.png
+-rw-r--r--   0 aleumi     (502) staff       (20)     4810 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/tensor/frobenius-example.png
+-rw-r--r--   0 aleumi     (502) staff       (20)    10998 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/tensor/men-are-mortal.png
+-rw-r--r--   0 aleumi     (502) staff       (20)     9312 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/tensor/product-rule.png
+-rw-r--r--   0 aleumi     (502) staff       (20)    13435 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/tensor/rewrite.png
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:50.081929 discopy-1.1.2/docs/_static/traced/
+-rw-r--r--   0 aleumi     (502) staff       (20)    10121 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/traced/golden.png
+-rw-r--r--   0 aleumi     (502) staff       (20)    10550 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/traced/right-nat-trace.png
+-rw-r--r--   0 aleumi     (502) staff       (20)     9691 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/traced/sliding-left.png
+-rw-r--r--   0 aleumi     (502) staff       (20)     9887 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/traced/sliding-right.png
+-rw-r--r--   0 aleumi     (502) staff       (20)    10411 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/traced/tightening-left.png
+-rw-r--r--   0 aleumi     (502) staff       (20)    10550 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/traced/tightening-right.png
+-rw-r--r--   0 aleumi     (502) staff       (20)    10247 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/traced/trace.png
+-rw-r--r--   0 aleumi     (502) staff       (20)    12964 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/traced/yanking.png
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:50.084145 discopy-1.1.2/docs/_style/
+-rw-r--r--   0 aleumi     (502) staff       (20)     1811 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_style/custom.css
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:50.091308 discopy-1.1.2/docs/_templates/
+-rw-r--r--   0 aleumi     (502) staff       (20)      185 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_templates/class.rst
+-rw-r--r--   0 aleumi     (502) staff       (20)      100 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_templates/function.rst
+-rw-r--r--   0 aleumi     (502) staff       (20)       66 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_templates/module.rst
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:50.112736 discopy-1.1.2/docs/api/
+-rw-r--r--   0 aleumi     (502) staff       (20)     4581 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/api/architecture.html
+-rw-r--r--   0 aleumi     (502) staff       (20)    56460 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/api/architecture.png
+-rw-r--r--   0 aleumi     (502) staff       (20)      168 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/api/drawing.rst
+-rw-r--r--   0 aleumi     (502) staff       (20)      256 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/api/grammar.rst
+-rw-r--r--   0 aleumi     (502) staff       (20)      302 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/api/quantum.rst
+-rw-r--r--   0 aleumi     (502) staff       (20)      222 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/api/semantics.rst
+-rw-r--r--   0 aleumi     (502) staff       (20)      458 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/api/syntax.rst
+-rw-r--r--   0 aleumi     (502) staff       (20)     3037 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/conf.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    13274 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/discopy.bib
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:50.118645 discopy-1.1.2/docs/extra/
+-rw-r--r--   0 aleumi     (502) staff       (20)       57 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/extra/bibliography.rst
+-rw-r--r--   0 aleumi     (502) staff       (20)     1059 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/extra/blogs.md
+-rw-r--r--   0 aleumi     (502) staff       (20)     6077 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/extra/papers.md
+-rw-r--r--   0 aleumi     (502) staff       (20)     1492 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/extra/talks.rst
+-rw-r--r--   0 aleumi     (502) staff       (20)      780 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/index.rst
+-rw-r--r--   0 aleumi     (502) staff       (20)      795 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/make.bat
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:50.136865 discopy-1.1.2/docs/notebooks/
+-rw-r--r--   0 aleumi     (502) staff       (20)   483325 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/notebooks/21-05-03-tallcat.ipynb
+-rw-r--r--   0 aleumi     (502) staff       (20)  1593241 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/notebooks/21-05-05-tallcat.ipynb
+-rw-r--r--   0 aleumi     (502) staff       (20)    42815 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/notebooks/diag-diff.ipynb
+-rw-r--r--   0 aleumi     (502) staff       (20)   179435 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/notebooks/diagrams.ipynb
+-rw-r--r--   0 aleumi     (502) staff       (20)   185975 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/notebooks/qnlp.ipynb
+-rw-r--r--   0 aleumi     (502) staff       (20)      140 2023-05-26 07:41:40.000000 discopy-1.1.2/pyproject.toml
+-rw-r--r--   0 aleumi     (502) staff       (20)     1703 2023-05-26 07:43:50.260715 discopy-1.1.2/setup.cfg
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:49.839776 discopy-1.1.2/test/
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:50.139445 discopy-1.1.2/test/drawing/
+-rw-r--r--   0 aleumi     (502) staff       (20)     5571 2023-05-26 07:41:40.000000 discopy-1.1.2/test/drawing/legacy.py
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:50.142325 discopy-1.1.2/test/grammar/
+-rw-r--r--   0 aleumi     (502) staff       (20)     7756 2023-05-26 07:41:40.000000 discopy-1.1.2/test/grammar/categorial.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     2049 2023-05-26 07:41:40.000000 discopy-1.1.2/test/grammar/pregroup.py
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:50.150706 discopy-1.1.2/test/quantum/
+-rw-r--r--   0 aleumi     (502) staff       (20)      425 2023-05-26 07:41:40.000000 discopy-1.1.2/test/quantum/ansatze.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     1551 2023-05-26 07:41:40.000000 discopy-1.1.2/test/quantum/channel.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    25046 2023-05-26 07:41:40.000000 discopy-1.1.2/test/quantum/circuit.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     2510 2023-05-26 07:41:40.000000 discopy-1.1.2/test/quantum/eval.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     4296 2023-05-26 07:41:40.000000 discopy-1.1.2/test/quantum/tk.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     5804 2023-05-26 07:41:40.000000 discopy-1.1.2/test/quantum/zx.py
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:50.161254 discopy-1.1.2/test/semantics/
+-rw-r--r--   0 aleumi     (502) staff       (20)     1201 2023-05-26 07:41:40.000000 discopy-1.1.2/test/semantics/matrix.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     1304 2023-05-26 07:41:40.000000 discopy-1.1.2/test/semantics/python.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     8105 2023-05-26 07:41:40.000000 discopy-1.1.2/test/semantics/tensor.py
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:50.162827 discopy-1.1.2/test/src/
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:50.181503 discopy-1.1.2/test/src/imgs/
+-rw-r--r--   0 aleumi     (502) staff       (20)    12008 2023-05-26 07:41:40.000000 discopy-1.1.2/test/src/imgs/EckmannHilton.gif
+-rw-r--r--   0 aleumi     (502) staff       (20)     7553 2023-05-26 07:41:40.000000 discopy-1.1.2/test/src/imgs/bell-state.png
+-rw-r--r--   0 aleumi     (502) staff       (20)    16964 2023-05-26 07:41:40.000000 discopy-1.1.2/test/src/imgs/bialgebra.png
+-rw-r--r--   0 aleumi     (502) staff       (20)    25004 2023-05-26 07:41:40.000000 discopy-1.1.2/test/src/imgs/crack-eggs.png
+-rw-r--r--   0 aleumi     (502) staff       (20)     2411 2023-05-26 07:41:40.000000 discopy-1.1.2/test/src/imgs/empty_diagram.png
+-rw-r--r--   0 aleumi     (502) staff       (20)     5907 2023-05-26 07:41:40.000000 discopy-1.1.2/test/src/imgs/long-controlled.png
+-rw-r--r--   0 aleumi     (502) staff       (20)     8810 2023-05-26 07:41:40.000000 discopy-1.1.2/test/src/imgs/sentence-as-diagram.png
+-rw-r--r--   0 aleumi     (502) staff       (20)     5315 2023-05-26 07:41:40.000000 discopy-1.1.2/test/src/imgs/snake-equation.png
+-rw-r--r--   0 aleumi     (502) staff       (20)    10800 2023-05-26 07:41:40.000000 discopy-1.1.2/test/src/imgs/spiral.png
+-rw-r--r--   0 aleumi     (502) staff       (20)     6051 2023-05-26 07:41:40.000000 discopy-1.1.2/test/src/imgs/typed-snake-equation.png
+-rw-r--r--   0 aleumi     (502) staff       (20)     9525 2023-05-26 07:41:40.000000 discopy-1.1.2/test/src/imgs/who-ansatz.png
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:50.210883 discopy-1.1.2/test/src/tikz/
+-rw-r--r--   0 aleumi     (502) staff       (20)     2228 2023-05-26 07:41:40.000000 discopy-1.1.2/test/src/tikz/bell-state.tikz
+-rw-r--r--   0 aleumi     (502) staff       (20)      153 2023-05-26 07:41:40.000000 discopy-1.1.2/test/src/tikz/bell-state.tikzstyles
+-rw-r--r--   0 aleumi     (502) staff       (20)     4906 2023-05-26 07:41:40.000000 discopy-1.1.2/test/src/tikz/bialgebra.tikz
+-rw-r--r--   0 aleumi     (502) staff       (20)      150 2023-05-26 07:41:40.000000 discopy-1.1.2/test/src/tikz/bialgebra.tikzstyles
+-rw-r--r--   0 aleumi     (502) staff       (20)     2441 2023-05-26 07:41:40.000000 discopy-1.1.2/test/src/tikz/copy.tikz
+-rw-r--r--   0 aleumi     (502) staff       (20)       86 2023-05-26 07:41:40.000000 discopy-1.1.2/test/src/tikz/copy.tikzstyles
+-rw-r--r--   0 aleumi     (502) staff       (20)     3441 2023-05-26 07:41:40.000000 discopy-1.1.2/test/src/tikz/crack-eggs.tikz
+-rw-r--r--   0 aleumi     (502) staff       (20)     3338 2023-05-26 07:41:40.000000 discopy-1.1.2/test/src/tikz/long-controlled.tikz
+-rw-r--r--   0 aleumi     (502) staff       (20)     2223 2023-05-26 07:41:40.000000 discopy-1.1.2/test/src/tikz/snake-equation.tikz
+-rw-r--r--   0 aleumi     (502) staff       (20)     1906 2023-05-26 07:41:40.000000 discopy-1.1.2/test/src/tikz/spiral.tikz
+-rw-r--r--   0 aleumi     (502) staff       (20)      260 2023-05-26 07:41:40.000000 discopy-1.1.2/test/src/tikz/spiral.tikzstyles
+-rw-r--r--   0 aleumi     (502) staff       (20)     3435 2023-05-26 07:41:40.000000 discopy-1.1.2/test/src/tikz/who-ansatz.tikz
+-rw-r--r--   0 aleumi     (502) staff       (20)    15562 2023-05-26 07:41:40.000000 discopy-1.1.2/test/src/tree2diagram.pickle
+-rw-r--r--   0 aleumi     (502) staff       (20)     6324 2023-05-26 07:41:40.000000 discopy-1.1.2/test/src/zx-graph.json
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:50.250191 discopy-1.1.2/test/syntax/
+-rw-r--r--   0 aleumi     (502) staff       (20)      258 2023-05-26 07:41:40.000000 discopy-1.1.2/test/syntax/balanced.py
+-rw-r--r--   0 aleumi     (502) staff       (20)      487 2023-05-26 07:41:40.000000 discopy-1.1.2/test/syntax/braided.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     7650 2023-05-26 07:41:40.000000 discopy-1.1.2/test/syntax/cat.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     1413 2023-05-26 07:41:40.000000 discopy-1.1.2/test/syntax/closed.py
+-rw-r--r--   0 aleumi     (502) staff       (20)      828 2023-05-26 07:41:40.000000 discopy-1.1.2/test/syntax/compact.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     1750 2023-05-26 07:41:40.000000 discopy-1.1.2/test/syntax/frobenius.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     1934 2023-05-26 07:41:40.000000 discopy-1.1.2/test/syntax/hypergraph.py
+-rw-r--r--   0 aleumi     (502) staff       (20)      659 2023-05-26 07:41:40.000000 discopy-1.1.2/test/syntax/interaction.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     1532 2023-05-26 07:41:40.000000 discopy-1.1.2/test/syntax/markov.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    10159 2023-05-26 07:41:40.000000 discopy-1.1.2/test/syntax/monoidal.py
+-rw-r--r--   0 aleumi     (502) staff       (20)      176 2023-05-26 07:41:40.000000 discopy-1.1.2/test/syntax/pivotal.py
+-rw-r--r--   0 aleumi     (502) staff       (20)      553 2023-05-26 07:41:40.000000 discopy-1.1.2/test/syntax/ribbon.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     3278 2023-05-26 07:41:40.000000 discopy-1.1.2/test/syntax/rigid.py
+-rw-r--r--   0 aleumi     (502) staff       (20)      962 2023-05-26 07:41:40.000000 discopy-1.1.2/test/syntax/symmetric.py
+-rw-r--r--   0 aleumi     (502) staff       (20)      354 2023-05-26 07:41:40.000000 discopy-1.1.2/test/syntax/traced.py
+-rw-r--r--   0 aleumi     (502) staff       (20)      953 2023-05-26 07:41:40.000000 discopy-1.1.2/test/syntax/utils.py
```

### Comparing `discopy-1.1.1/LICENSE` & `discopy-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `discopy-1.1.1/PKG-INFO` & `discopy-1.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,33 @@
 Metadata-Version: 2.1
 Name: discopy
-Version: 1.1.1
+Version: 1.1.2
 Summary: The Python toolkit for computing with string diagrams.
 Home-page: https://discopy.org
-Download-URL: https://github.com/discopy/discopy/archive/1.1.1.tar.gz
-Author: Alexis Toumi
-Author-email: alexis@toumi.email
+Download-URL: https://pypi.org/project/discopy
+Author: DisCoPy
+Author-email: contact@discopy.org
+License: BSD 3
 Project-URL: Documentation, https://docs.discopy.org
-Project-URL: Source, https://github.com/discopy/discopy
-Project-URL: Tracker, https://github.com/discopy/discopy/issues
-Keywords: diagrams category-theory quantum-computing nlp
+Project-URL: Source Code, https://github.com/discopy/discopy
+Project-URL: Issue Tracker, https://github.com/discopy/discopy/issues
+Keywords: category theory,string diagrams,natural language processing,quantum computing
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: docs
-License-File: LICENSE
 
 
 ![snake equation](https://github.com/discopy/discopy/raw/main/docs/_static/snake-equation.png)
 
 # DisCoPy
 
 [![build](https://github.com/discopy/discopy/actions/workflows/build_test.yml/badge.svg)](https://github.com/discopy/discopy/actions/workflows/build_test.yml)
```

### Comparing `discopy-1.1.1/README.md` & `discopy-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `discopy-1.1.1/discopy/balanced.py` & `discopy-1.1.2/discopy/balanced.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.1/discopy/braided.py` & `discopy-1.1.2/discopy/braided.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.1/discopy/cat.py` & `discopy-1.1.2/discopy/cat.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.1/discopy/closed.py` & `discopy-1.1.2/discopy/closed.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.1/discopy/compact.py` & `discopy-1.1.2/discopy/compact.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.1/discopy/config.py` & `discopy-1.1.2/discopy/config.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.1/discopy/drawing/__init__.py` & `discopy-1.1.2/discopy/drawing/__init__.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.1/discopy/drawing/grid.py` & `discopy-1.1.2/discopy/drawing/grid.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.1/discopy/drawing/legacy.py` & `discopy-1.1.2/discopy/drawing/legacy.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.1/discopy/frobenius.py` & `discopy-1.1.2/discopy/frobenius.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.1/discopy/grammar/categorial.py` & `discopy-1.1.2/discopy/grammar/categorial.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.1/discopy/grammar/cfg.py` & `discopy-1.1.2/discopy/grammar/cfg.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.1/discopy/grammar/dependency.py` & `discopy-1.1.2/discopy/grammar/dependency.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.1/discopy/grammar/pregroup.py` & `discopy-1.1.2/discopy/grammar/pregroup.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.1/discopy/grammar/thue.py` & `discopy-1.1.2/discopy/grammar/thue.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.1/discopy/hypergraph.py` & `discopy-1.1.2/discopy/hypergraph.py`

 * *Files 0% similar despite different names*

```diff
@@ -1061,18 +1061,18 @@
     def to_graph(self) -> Graph:
         """
         Translate a hypergraph into a labeled graph with nodes for inputs,
         outputs, boxes, domain, codomain and spiders.
         """
         graph = Graph()
         graph.add_nodes_from(
-            Node("spider", i=i, obj=obj)
+            (Node("spider", i=i, obj=obj), dict(box=None))
             for i, obj in enumerate(self.spider_types))
         graph.add_nodes_from(
-            (Node("input", i=i, obj=obj), dict(i=i))
+            (Node("input", i=i, obj=obj), dict(i=i, box=None))
             for i, obj in enumerate(self.dom))
         graph.add_edges_from(
             (Node("input", i=i, obj=obj), Node("spider", i=j, obj=obj))
             for i, (j, obj) in enumerate(
                 zip(self.wires[:len(self.dom)], self.dom)))
         for i, (box, (dom_wires, cod_wires)) in enumerate(
                 zip(self.boxes, self.box_wires)):
@@ -1087,15 +1087,15 @@
                     if case == "dom":
                         graph.add_edge(spider_node, port_node)
                         graph.add_edge(port_node, box_node)
                     else:
                         graph.add_edge(box_node, port_node)
                         graph.add_edge(port_node, spider_node)
         graph.add_nodes_from(
-            (Node("output", i=i, obj=obj), dict(i=i))
+            (Node("output", i=i, obj=obj), dict(i=i, box=None))
             for i, obj in enumerate(self.cod))
         graph.add_edges_from(
             (Node("spider", i=j, obj=obj), Node("output", i=i, obj=obj))
             for i, (j, obj) in enumerate(
                 zip(self.wires[len(self.wires) - len(self.cod):], self.cod)))
         return graph
```

### Comparing `discopy-1.1.1/discopy/interaction.py` & `discopy-1.1.2/discopy/interaction.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.1/discopy/markov.py` & `discopy-1.1.2/discopy/markov.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.1/discopy/matrix.py` & `discopy-1.1.2/discopy/matrix.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.1/discopy/messages.py` & `discopy-1.1.2/discopy/messages.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.1/discopy/monoidal.py` & `discopy-1.1.2/discopy/monoidal.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.1/discopy/pivotal.py` & `discopy-1.1.2/discopy/pivotal.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.1/discopy/python.py` & `discopy-1.1.2/discopy/python.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.1/discopy/quantum/__init__.py` & `discopy-1.1.2/discopy/quantum/__init__.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.1/discopy/quantum/ansatze.py` & `discopy-1.1.2/discopy/quantum/ansatze.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.1/discopy/quantum/channel.py` & `discopy-1.1.2/discopy/quantum/channel.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.1/discopy/quantum/circuit.py` & `discopy-1.1.2/discopy/quantum/circuit.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.1/discopy/quantum/gates.py` & `discopy-1.1.2/discopy/quantum/gates.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.1/discopy/quantum/pennylane.py` & `discopy-1.1.2/discopy/quantum/pennylane.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.1/discopy/quantum/tk.py` & `discopy-1.1.2/discopy/quantum/tk.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.1/discopy/quantum/zx.py` & `discopy-1.1.2/discopy/quantum/zx.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.1/discopy/ribbon.py` & `discopy-1.1.2/discopy/ribbon.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.1/discopy/rigid.py` & `discopy-1.1.2/discopy/rigid.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.1/discopy/symmetric.py` & `discopy-1.1.2/discopy/symmetric.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.1/discopy/tensor.py` & `discopy-1.1.2/discopy/tensor.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.1/discopy/traced.py` & `discopy-1.1.2/discopy/traced.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.1/discopy/utils.py` & `discopy-1.1.2/discopy/utils.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.1/discopy.egg-info/PKG-INFO` & `discopy-1.1.2/discopy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,33 @@
 Metadata-Version: 2.1
 Name: discopy
-Version: 1.1.1
+Version: 1.1.2
 Summary: The Python toolkit for computing with string diagrams.
 Home-page: https://discopy.org
-Download-URL: https://github.com/discopy/discopy/archive/1.1.1.tar.gz
-Author: Alexis Toumi
-Author-email: alexis@toumi.email
+Download-URL: https://pypi.org/project/discopy
+Author: DisCoPy
+Author-email: contact@discopy.org
+License: BSD 3
 Project-URL: Documentation, https://docs.discopy.org
-Project-URL: Source, https://github.com/discopy/discopy
-Project-URL: Tracker, https://github.com/discopy/discopy/issues
-Keywords: diagrams category-theory quantum-computing nlp
+Project-URL: Source Code, https://github.com/discopy/discopy
+Project-URL: Issue Tracker, https://github.com/discopy/discopy/issues
+Keywords: category theory,string diagrams,natural language processing,quantum computing
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: docs
-License-File: LICENSE
 
 
 ![snake equation](https://github.com/discopy/discopy/raw/main/docs/_static/snake-equation.png)
 
 # DisCoPy
 
 [![build](https://github.com/discopy/discopy/actions/workflows/build_test.yml/badge.svg)](https://github.com/discopy/discopy/actions/workflows/build_test.yml)
```

