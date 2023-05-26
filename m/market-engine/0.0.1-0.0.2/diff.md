# Comparing `tmp/market-engine-0.0.1.tar.gz` & `tmp/market-engine-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "market-engine-0.0.1.tar", last modified: Fri May 26 19:12:45 2023, max compression
+gzip compressed data, was "market-engine-0.0.2.tar", last modified: Fri May 26 19:23:26 2023, max compression
```

## Comparing `market-engine-0.0.1.tar` & `market-engine-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 19:12:45.429746 market-engine-0.0.1/
--rw-rw-rw-   0        0        0      216 2023-05-26 19:12:45.429746 market-engine-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-26 19:12:45.427746 market-engine-0.0.1/market_engine/
--rw-rw-rw-   0        0        0        0 2023-05-26 19:06:03.000000 market-engine-0.0.1/market_engine/__init__.py
--rw-rw-rw-   0        0        0     1084 2023-05-26 19:04:00.000000 market-engine-0.0.1/market_engine/common.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:12:45.428745 market-engine-0.0.1/market_engine.egg-info/
--rw-rw-rw-   0        0        0      216 2023-05-26 19:12:45.000000 market-engine-0.0.1/market_engine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-05-26 19:12:45.000000 market-engine-0.0.1/market_engine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 19:12:45.000000 market-engine-0.0.1/market_engine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      235 2023-05-26 19:12:45.000000 market-engine-0.0.1/market_engine.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-26 19:12:45.000000 market-engine-0.0.1/market_engine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-26 19:12:45.429746 market-engine-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      724 2023-05-26 19:11:20.000000 market-engine-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 19:23:26.410428 market-engine-0.0.2/
+-rw-rw-rw-   0        0        0      216 2023-05-26 19:23:26.410428 market-engine-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-26 19:23:26.405424 market-engine-0.0.2/market_engine/
+-rw-rw-rw-   0        0        0        0 2023-05-26 19:06:03.000000 market-engine-0.0.2/market_engine/__init__.py
+-rw-rw-rw-   0        0        0     1084 2023-05-26 19:04:00.000000 market-engine-0.0.2/market_engine/common.py
+drwxrwxrwx   0        0        0        0 2023-05-26 19:23:26.409428 market-engine-0.0.2/market_engine/modules/
+-rw-rw-rw-   0        0        0    14005 2023-05-26 19:04:00.000000 market-engine-0.0.2/market_engine/modules/MarketAPI.py
+-rw-rw-rw-   0        0        0     6987 2023-05-26 19:04:00.000000 market-engine-0.0.2/market_engine/modules/MarketDB.py
+-rw-rw-rw-   0        0        0    14971 2023-05-26 19:04:00.000000 market-engine-0.0.2/market_engine/modules/MarketData.py
+-rw-rw-rw-   0        0        0        0 2023-05-26 19:04:43.000000 market-engine-0.0.2/market_engine/modules/__init__.py
+-rw-rw-rw-   0        0        0    38904 2023-05-26 19:04:00.000000 market-engine-0.0.2/market_engine/modules/categories.py
+drwxrwxrwx   0        0        0        0 2023-05-26 19:23:26.407428 market-engine-0.0.2/market_engine.egg-info/
+-rw-rw-rw-   0        0        0      216 2023-05-26 19:23:26.000000 market-engine-0.0.2/market_engine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      417 2023-05-26 19:23:26.000000 market-engine-0.0.2/market_engine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 19:23:26.000000 market-engine-0.0.2/market_engine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      235 2023-05-26 19:23:26.000000 market-engine-0.0.2/market_engine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-26 19:23:26.000000 market-engine-0.0.2/market_engine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 19:23:26.410428 market-engine-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      737 2023-05-26 19:23:16.000000 market-engine-0.0.2/setup.py
```

### Comparing `market-engine-0.0.1/market_engine/common.py` & `market-engine-0.0.2/market_engine/common.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.0.1/setup.py` & `market-engine-0.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from setuptools import setup
+from setuptools import setup, find_packages
 
 setup(
     name='market-engine',
-    version='0.0.1',
+    version='0.0.2',
     description='Engine for easily getting the orders, statistics, and other stats from warframe.market.',
     author='Jacob McBride',
     author_email='jake55111@gmail.com',
-    packages=['market_engine'],
+    packages=find_packages(),
     install_requires=[
         'aiohttp~=3.8.4',
         'discord~=2.2.2',
         'aiolimiter~=1.0.0',
         'redis~=4.5.4',
         'requests~=2.29.0',
         'beautifulsoup4~=4.12.2',
```

