# Comparing `tmp/gerador_posts-0.1.0.tar.gz` & `tmp/gerador_posts-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gerador_posts-0.1.0.tar", last modified: Thu May 25 21:50:58 2023, max compression
+gzip compressed data, was "gerador_posts-0.1.1.tar", last modified: Thu May 25 23:49:27 2023, max compression
```

## Comparing `gerador_posts-0.1.0.tar` & `gerador_posts-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 cecivieira  (1000) cecivieira  (1000)        0 2023-05-25 21:50:58.452872 gerador_posts-0.1.0/
--rw-rw-r--   0 cecivieira  (1000) cecivieira  (1000)     1076 2023-05-25 21:40:24.000000 gerador_posts-0.1.0/LICENSE
--rw-rw-r--   0 cecivieira  (1000) cecivieira  (1000)     1386 2023-05-25 21:50:58.452872 gerador_posts-0.1.0/PKG-INFO
--rw-rw-r--   0 cecivieira  (1000) cecivieira  (1000)     1001 2023-05-25 21:41:43.000000 gerador_posts-0.1.0/README.md
-drwxrwxr-x   0 cecivieira  (1000) cecivieira  (1000)        0 2023-05-25 21:50:58.452872 gerador_posts-0.1.0/gerador_posts/
--rw-rw-r--   0 cecivieira  (1000) cecivieira  (1000)        0 2023-05-25 21:40:24.000000 gerador_posts-0.1.0/gerador_posts/__init__.py
--rw-rw-r--   0 cecivieira  (1000) cecivieira  (1000)       86 2023-05-25 21:40:24.000000 gerador_posts-0.1.0/gerador_posts/__main__.py
--rw-rw-r--   0 cecivieira  (1000) cecivieira  (1000)     1189 2023-05-25 21:40:24.000000 gerador_posts-0.1.0/gerador_posts/configuracao.py
--rw-rw-r--   0 cecivieira  (1000) cecivieira  (1000)      418 2023-05-25 21:40:24.000000 gerador_posts-0.1.0/gerador_posts/gerador_posts.py
--rw-rw-r--   0 cecivieira  (1000) cecivieira  (1000)      831 2023-05-25 21:40:24.000000 gerador_posts-0.1.0/gerador_posts/tratar_dados.py
-drwxrwxr-x   0 cecivieira  (1000) cecivieira  (1000)        0 2023-05-25 21:50:58.452872 gerador_posts-0.1.0/gerador_posts.egg-info/
--rw-rw-r--   0 cecivieira  (1000) cecivieira  (1000)     1386 2023-05-25 21:50:58.000000 gerador_posts-0.1.0/gerador_posts.egg-info/PKG-INFO
--rw-rw-r--   0 cecivieira  (1000) cecivieira  (1000)      429 2023-05-25 21:50:58.000000 gerador_posts-0.1.0/gerador_posts.egg-info/SOURCES.txt
--rw-rw-r--   0 cecivieira  (1000) cecivieira  (1000)        1 2023-05-25 21:50:58.000000 gerador_posts-0.1.0/gerador_posts.egg-info/dependency_links.txt
--rw-rw-r--   0 cecivieira  (1000) cecivieira  (1000)       74 2023-05-25 21:50:58.000000 gerador_posts-0.1.0/gerador_posts.egg-info/entry_points.txt
--rw-rw-r--   0 cecivieira  (1000) cecivieira  (1000)        1 2023-05-25 21:50:58.000000 gerador_posts-0.1.0/gerador_posts.egg-info/not-zip-safe
--rw-rw-r--   0 cecivieira  (1000) cecivieira  (1000)       44 2023-05-25 21:50:58.000000 gerador_posts-0.1.0/gerador_posts.egg-info/requires.txt
--rw-rw-r--   0 cecivieira  (1000) cecivieira  (1000)       14 2023-05-25 21:50:58.000000 gerador_posts-0.1.0/gerador_posts.egg-info/top_level.txt
--rw-rw-r--   0 cecivieira  (1000) cecivieira  (1000)       38 2023-05-25 21:50:58.452872 gerador_posts-0.1.0/setup.cfg
--rw-rw-r--   0 cecivieira  (1000) cecivieira  (1000)      873 2023-05-25 21:50:13.000000 gerador_posts-0.1.0/setup.py
+drwxrwxr-x   0 cecivieira  (1000) cecivieira  (1000)        0 2023-05-25 23:49:27.074545 gerador_posts-0.1.1/
+-rw-rw-r--   0 cecivieira  (1000) cecivieira  (1000)     1076 2023-05-25 21:40:24.000000 gerador_posts-0.1.1/LICENSE
+-rw-rw-r--   0 cecivieira  (1000) cecivieira  (1000)     1386 2023-05-25 23:49:27.074545 gerador_posts-0.1.1/PKG-INFO
+-rw-rw-r--   0 cecivieira  (1000) cecivieira  (1000)     1001 2023-05-25 21:41:43.000000 gerador_posts-0.1.1/README.md
+drwxrwxr-x   0 cecivieira  (1000) cecivieira  (1000)        0 2023-05-25 23:49:27.074545 gerador_posts-0.1.1/gerador_posts/
+-rw-rw-r--   0 cecivieira  (1000) cecivieira  (1000)        0 2023-05-25 21:40:24.000000 gerador_posts-0.1.1/gerador_posts/__init__.py
+-rw-rw-r--   0 cecivieira  (1000) cecivieira  (1000)       86 2023-05-25 21:40:24.000000 gerador_posts-0.1.1/gerador_posts/__main__.py
+-rw-rw-r--   0 cecivieira  (1000) cecivieira  (1000)     1189 2023-05-25 21:40:24.000000 gerador_posts-0.1.1/gerador_posts/configuracao.py
+-rw-rw-r--   0 cecivieira  (1000) cecivieira  (1000)      418 2023-05-25 21:40:24.000000 gerador_posts-0.1.1/gerador_posts/gerador_posts.py
+-rw-rw-r--   0 cecivieira  (1000) cecivieira  (1000)      831 2023-05-25 21:40:24.000000 gerador_posts-0.1.1/gerador_posts/tratar_dados.py
+drwxrwxr-x   0 cecivieira  (1000) cecivieira  (1000)        0 2023-05-25 23:49:27.074545 gerador_posts-0.1.1/gerador_posts.egg-info/
+-rw-rw-r--   0 cecivieira  (1000) cecivieira  (1000)     1386 2023-05-25 23:49:27.000000 gerador_posts-0.1.1/gerador_posts.egg-info/PKG-INFO
+-rw-rw-r--   0 cecivieira  (1000) cecivieira  (1000)      429 2023-05-25 23:49:27.000000 gerador_posts-0.1.1/gerador_posts.egg-info/SOURCES.txt
+-rw-rw-r--   0 cecivieira  (1000) cecivieira  (1000)        1 2023-05-25 23:49:27.000000 gerador_posts-0.1.1/gerador_posts.egg-info/dependency_links.txt
+-rw-rw-r--   0 cecivieira  (1000) cecivieira  (1000)       74 2023-05-25 23:49:27.000000 gerador_posts-0.1.1/gerador_posts.egg-info/entry_points.txt
+-rw-rw-r--   0 cecivieira  (1000) cecivieira  (1000)        1 2023-05-25 21:50:58.000000 gerador_posts-0.1.1/gerador_posts.egg-info/not-zip-safe
+-rw-rw-r--   0 cecivieira  (1000) cecivieira  (1000)       44 2023-05-25 23:49:27.000000 gerador_posts-0.1.1/gerador_posts.egg-info/requires.txt
+-rw-rw-r--   0 cecivieira  (1000) cecivieira  (1000)       14 2023-05-25 23:49:27.000000 gerador_posts-0.1.1/gerador_posts.egg-info/top_level.txt
+-rw-rw-r--   0 cecivieira  (1000) cecivieira  (1000)       38 2023-05-25 23:49:27.074545 gerador_posts-0.1.1/setup.cfg
+-rw-rw-r--   0 cecivieira  (1000) cecivieira  (1000)     1032 2023-05-25 23:49:24.000000 gerador_posts-0.1.1/setup.py
```

### Comparing `gerador_posts-0.1.0/LICENSE` & `gerador_posts-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gerador_posts-0.1.0/PKG-INFO` & `gerador_posts-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gerador_posts
-Version: 0.1.0
+Version: 0.1.1
 Summary: Gerador de posts baseado em templates e dados 
 Home-page: https://github.com/cecivieira/gerador-posts
 Author: Ana Cecília Vieira
 Author-email: cecivieira@gmail.com
 License: MIT
 Keywords: jinja2,yaml,templates
 Platform: UNKNOWN
```

### Comparing `gerador_posts-0.1.0/README.md` & `gerador_posts-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `gerador_posts-0.1.0/gerador_posts/configuracao.py` & `gerador_posts-0.1.1/gerador_posts/configuracao.py`

 * *Files identical despite different names*

### Comparing `gerador_posts-0.1.0/gerador_posts/tratar_dados.py` & `gerador_posts-0.1.1/gerador_posts/tratar_dados.py`

 * *Files identical despite different names*

### Comparing `gerador_posts-0.1.0/gerador_posts.egg-info/PKG-INFO` & `gerador_posts-0.1.1/gerador_posts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gerador-posts
-Version: 0.1.0
+Version: 0.1.1
 Summary: Gerador de posts baseado em templates e dados 
 Home-page: https://github.com/cecivieira/gerador-posts
 Author: Ana Cecília Vieira
 Author-email: cecivieira@gmail.com
 License: MIT
 Keywords: jinja2,yaml,templates
 Platform: UNKNOWN
```

