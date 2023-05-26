# Comparing `tmp/gbwhere-0.1.1.tar.gz` & `tmp/gbwhere-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gbwhere-0.1.1.tar", max compression
+gzip compressed data, was "gbwhere-0.1.2.tar", max compression
```

## Comparing `gbwhere-0.1.1.tar` & `gbwhere-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      161 2023-05-25 23:47:18.280210 gbwhere-0.1.1/README.md
--rw-r--r--   0        0        0      390 2023-05-25 23:47:23.224177 gbwhere-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      245 2023-05-25 22:20:14.815199 gbwhere-0.1.1/where/cli.py
--rw-r--r--   0        0        0      327 2023-05-25 21:02:29.222307 gbwhere-0.1.1/where/exceptions.py
--rw-r--r--   0        0        0     3494 2023-05-25 22:09:28.355512 gbwhere-0.1.1/where/finder.py
--rw-r--r--   0        0        0     3490 2023-05-25 22:22:17.738380 gbwhere-0.1.1/where/utils.py
--rw-r--r--   0        0        0      581 1970-01-01 00:00:00.000000 gbwhere-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1218 2023-05-26 00:05:24.372830 gbwhere-0.1.2/README.md
+-rw-r--r--   0        0        0      390 2023-05-26 00:05:49.612660 gbwhere-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      245 2023-05-25 22:20:14.815199 gbwhere-0.1.2/where/cli.py
+-rw-r--r--   0        0        0      327 2023-05-25 21:02:29.222307 gbwhere-0.1.2/where/exceptions.py
+-rw-r--r--   0        0        0     3494 2023-05-25 22:09:28.355512 gbwhere-0.1.2/where/finder.py
+-rw-r--r--   0        0        0     3490 2023-05-25 22:22:17.738380 gbwhere-0.1.2/where/utils.py
+-rw-r--r--   0        0        0     1638 1970-01-01 00:00:00.000000 gbwhere-0.1.2/PKG-INFO
```

### Comparing `gbwhere-0.1.1/where/finder.py` & `gbwhere-0.1.2/where/finder.py`

 * *Files identical despite different names*

### Comparing `gbwhere-0.1.1/where/utils.py` & `gbwhere-0.1.2/where/utils.py`

 * *Files identical despite different names*

