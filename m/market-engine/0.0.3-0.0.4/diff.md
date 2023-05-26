# Comparing `tmp/market-engine-0.0.3.tar.gz` & `tmp/market-engine-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "market-engine-0.0.3.tar", last modified: Fri May 26 19:28:02 2023, max compression
+gzip compressed data, was "market-engine-0.0.4.tar", last modified: Fri May 26 19:30:56 2023, max compression
```

## Comparing `market-engine-0.0.3.tar` & `market-engine-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 19:28:02.173118 market-engine-0.0.3/
--rw-rw-rw-   0        0        0      216 2023-05-26 19:28:02.173118 market-engine-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-26 19:28:02.168119 market-engine-0.0.3/market_engine/
--rw-rw-rw-   0        0        0        0 2023-05-26 19:06:03.000000 market-engine-0.0.3/market_engine/__init__.py
--rw-rw-rw-   0        0        0     1084 2023-05-26 19:04:00.000000 market-engine-0.0.3/market_engine/common.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:28:02.172120 market-engine-0.0.3/market_engine/modules/
--rw-rw-rw-   0        0        0    14007 2023-05-26 19:26:37.000000 market-engine-0.0.3/market_engine/modules/MarketAPI.py
--rw-rw-rw-   0        0        0     6989 2023-05-26 19:26:52.000000 market-engine-0.0.3/market_engine/modules/MarketDB.py
--rw-rw-rw-   0        0        0    14973 2023-05-26 19:26:44.000000 market-engine-0.0.3/market_engine/modules/MarketData.py
--rw-rw-rw-   0        0        0        0 2023-05-26 19:04:43.000000 market-engine-0.0.3/market_engine/modules/__init__.py
--rw-rw-rw-   0        0        0    38904 2023-05-26 19:04:00.000000 market-engine-0.0.3/market_engine/modules/categories.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:28:02.170119 market-engine-0.0.3/market_engine.egg-info/
--rw-rw-rw-   0        0        0      216 2023-05-26 19:28:02.000000 market-engine-0.0.3/market_engine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      417 2023-05-26 19:28:02.000000 market-engine-0.0.3/market_engine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 19:28:02.000000 market-engine-0.0.3/market_engine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      235 2023-05-26 19:28:02.000000 market-engine-0.0.3/market_engine.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-26 19:28:02.000000 market-engine-0.0.3/market_engine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-26 19:28:02.173118 market-engine-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      737 2023-05-26 19:27:02.000000 market-engine-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 19:30:56.023705 market-engine-0.0.4/
+-rw-rw-rw-   0        0        0      216 2023-05-26 19:30:56.023705 market-engine-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-26 19:30:56.016704 market-engine-0.0.4/market_engine/
+-rw-rw-rw-   0        0        0        0 2023-05-26 19:06:03.000000 market-engine-0.0.4/market_engine/__init__.py
+-rw-rw-rw-   0        0        0      932 2023-05-26 19:30:35.000000 market-engine-0.0.4/market_engine/common.py
+drwxrwxrwx   0        0        0        0 2023-05-26 19:30:56.022704 market-engine-0.0.4/market_engine/modules/
+-rw-rw-rw-   0        0        0    14007 2023-05-26 19:26:37.000000 market-engine-0.0.4/market_engine/modules/MarketAPI.py
+-rw-rw-rw-   0        0        0     6989 2023-05-26 19:26:52.000000 market-engine-0.0.4/market_engine/modules/MarketDB.py
+-rw-rw-rw-   0        0        0    14973 2023-05-26 19:26:44.000000 market-engine-0.0.4/market_engine/modules/MarketData.py
+-rw-rw-rw-   0        0        0        0 2023-05-26 19:04:43.000000 market-engine-0.0.4/market_engine/modules/__init__.py
+-rw-rw-rw-   0        0        0    38904 2023-05-26 19:04:00.000000 market-engine-0.0.4/market_engine/modules/categories.py
+drwxrwxrwx   0        0        0        0 2023-05-26 19:30:56.019705 market-engine-0.0.4/market_engine.egg-info/
+-rw-rw-rw-   0        0        0      216 2023-05-26 19:30:55.000000 market-engine-0.0.4/market_engine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      417 2023-05-26 19:30:55.000000 market-engine-0.0.4/market_engine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 19:30:55.000000 market-engine-0.0.4/market_engine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      235 2023-05-26 19:30:55.000000 market-engine-0.0.4/market_engine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-26 19:30:55.000000 market-engine-0.0.4/market_engine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 19:30:56.023705 market-engine-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      737 2023-05-26 19:30:45.000000 market-engine-0.0.4/setup.py
```

### Comparing `market-engine-0.0.3/market_engine/common.py` & `market-engine-0.0.4/market_engine/common.py`

 * *Files 17% similar despite different names*

```diff
@@ -26,20 +26,14 @@
         yield
         connection.commit()
     except Exception as e:
         connection.rollback()
         raise e
 
 
-# Load configuration
-config = configparser.ConfigParser()
-config.read("config.ini")
-
-OUTPUT_DIRECTORY = config.get("Output", "output_directory")
-
 logging.basicConfig(level=logging.INFO, format="%(asctime)s - %(levelname)s - %(message)s")
 logger = logging.getLogger()
 
 rate_limiter = AsyncLimiter(3, 1)  # 3 requests per 1 second
 
 
 async def clear_cache():
```

### Comparing `market-engine-0.0.3/market_engine/modules/MarketAPI.py` & `market-engine-0.0.4/market_engine/modules/MarketAPI.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.0.3/market_engine/modules/MarketDB.py` & `market-engine-0.0.4/market_engine/modules/MarketDB.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.0.3/market_engine/modules/MarketData.py` & `market-engine-0.0.4/market_engine/modules/MarketData.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.0.3/market_engine/modules/categories.py` & `market-engine-0.0.4/market_engine/modules/categories.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.0.3/setup.py` & `market-engine-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='market-engine',
-    version='0.0.3',
+    version='0.0.4',
     description='Engine for easily getting the orders, statistics, and other stats from warframe.market.',
     author='Jacob McBride',
     author_email='jake55111@gmail.com',
     packages=find_packages(),
     install_requires=[
         'aiohttp~=3.8.4',
         'discord~=2.2.2',
```

