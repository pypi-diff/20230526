# Comparing `tmp/redis-rqueue-1.0.1.tar.gz` & `tmp/redis-rqueue-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis-rqueue-1.0.1.tar", last modified: Thu May  4 15:22:15 2023, max compression
+gzip compressed data, was "redis-rqueue-1.0.2.tar", last modified: Fri May 26 17:39:22 2023, max compression
```

## Comparing `redis-rqueue-1.0.1.tar` & `redis-rqueue-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 vitor      (501) staff       (20)        0 2023-05-04 15:22:15.229093 redis-rqueue-1.0.1/
--rw-r--r--   0 vitor      (501) staff       (20)       79 2023-05-04 15:22:15.228970 redis-rqueue-1.0.1/PKG-INFO
--rw-r--r--   0 vitor      (501) staff       (20)       15 2023-05-04 14:20:49.000000 redis-rqueue-1.0.1/README.md
--rw-r--r--   0 vitor      (501) staff       (20)      263 2023-05-04 15:21:29.000000 redis-rqueue-1.0.1/pyproject.toml
--rw-r--r--   0 vitor      (501) staff       (20)       10 2023-04-27 18:10:37.000000 redis-rqueue-1.0.1/requirements.txt
--rw-r--r--   0 vitor      (501) staff       (20)       38 2023-05-04 15:22:15.229132 redis-rqueue-1.0.1/setup.cfg
-drwxr-xr-x   0 vitor      (501) staff       (20)        0 2023-05-04 15:22:15.227207 redis-rqueue-1.0.1/src/
-drwxr-xr-x   0 vitor      (501) staff       (20)        0 2023-05-04 15:22:15.228281 redis-rqueue-1.0.1/src/redis_rqueue.egg-info/
--rw-r--r--   0 vitor      (501) staff       (20)       79 2023-05-04 15:22:15.000000 redis-rqueue-1.0.1/src/redis_rqueue.egg-info/PKG-INFO
--rw-r--r--   0 vitor      (501) staff       (20)      292 2023-05-04 15:22:15.000000 redis-rqueue-1.0.1/src/redis_rqueue.egg-info/SOURCES.txt
--rw-r--r--   0 vitor      (501) staff       (20)        1 2023-05-04 15:22:15.000000 redis-rqueue-1.0.1/src/redis_rqueue.egg-info/dependency_links.txt
--rw-r--r--   0 vitor      (501) staff       (20)       11 2023-05-04 15:22:15.000000 redis-rqueue-1.0.1/src/redis_rqueue.egg-info/requires.txt
--rw-r--r--   0 vitor      (501) staff       (20)        7 2023-05-04 15:22:15.000000 redis-rqueue-1.0.1/src/redis_rqueue.egg-info/top_level.txt
-drwxr-xr-x   0 vitor      (501) staff       (20)        0 2023-05-04 15:22:15.228695 redis-rqueue-1.0.1/src/rqueue/
--rw-r--r--   0 vitor      (501) staff       (20)       67 2023-05-04 13:16:59.000000 redis-rqueue-1.0.1/src/rqueue/__init__.py
--rw-r--r--   0 vitor      (501) staff       (20)     3490 2023-05-04 15:16:27.000000 redis-rqueue-1.0.1/src/rqueue/queue_executor.py
+drwxr-xr-x   0 vitor      (501) staff       (20)        0 2023-05-26 17:39:22.891910 redis-rqueue-1.0.2/
+-rw-r--r--   0 vitor      (501) staff       (20)       79 2023-05-26 17:39:22.891735 redis-rqueue-1.0.2/PKG-INFO
+-rw-r--r--   0 vitor      (501) staff       (20)       15 2023-05-26 17:37:27.000000 redis-rqueue-1.0.2/README.md
+-rw-r--r--   0 vitor      (501) staff       (20)      263 2023-05-26 17:38:11.000000 redis-rqueue-1.0.2/pyproject.toml
+-rw-r--r--   0 vitor      (501) staff       (20)       12 2023-05-26 17:38:02.000000 redis-rqueue-1.0.2/requirements.txt
+-rw-r--r--   0 vitor      (501) staff       (20)       38 2023-05-26 17:39:22.891954 redis-rqueue-1.0.2/setup.cfg
+drwxr-xr-x   0 vitor      (501) staff       (20)        0 2023-05-26 17:39:22.889653 redis-rqueue-1.0.2/src/
+drwxr-xr-x   0 vitor      (501) staff       (20)        0 2023-05-26 17:39:22.890816 redis-rqueue-1.0.2/src/redis_rqueue.egg-info/
+-rw-r--r--   0 vitor      (501) staff       (20)       79 2023-05-26 17:39:22.000000 redis-rqueue-1.0.2/src/redis_rqueue.egg-info/PKG-INFO
+-rw-r--r--   0 vitor      (501) staff       (20)      292 2023-05-26 17:39:22.000000 redis-rqueue-1.0.2/src/redis_rqueue.egg-info/SOURCES.txt
+-rw-r--r--   0 vitor      (501) staff       (20)        1 2023-05-26 17:39:22.000000 redis-rqueue-1.0.2/src/redis_rqueue.egg-info/dependency_links.txt
+-rw-r--r--   0 vitor      (501) staff       (20)       13 2023-05-26 17:39:22.000000 redis-rqueue-1.0.2/src/redis_rqueue.egg-info/requires.txt
+-rw-r--r--   0 vitor      (501) staff       (20)        7 2023-05-26 17:39:22.000000 redis-rqueue-1.0.2/src/redis_rqueue.egg-info/top_level.txt
+drwxr-xr-x   0 vitor      (501) staff       (20)        0 2023-05-26 17:39:22.891206 redis-rqueue-1.0.2/src/rqueue/
+-rw-r--r--   0 vitor      (501) staff       (20)       67 2023-05-26 17:37:27.000000 redis-rqueue-1.0.2/src/rqueue/__init__.py
+-rw-r--r--   0 vitor      (501) staff       (20)     3490 2023-05-26 17:37:27.000000 redis-rqueue-1.0.2/src/rqueue/queue_executor.py
```

### Comparing `redis-rqueue-1.0.1/src/rqueue/queue_executor.py` & `redis-rqueue-1.0.2/src/rqueue/queue_executor.py`

 * *Files identical despite different names*

