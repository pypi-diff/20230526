# Comparing `tmp/news_crawlers-3.4.2.tar.gz` & `tmp/news_crawlers-3.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "news_crawlers-3.4.2.tar", last modified: Sat Feb 18 22:27:38 2023, max compression
+gzip compressed data, was "news_crawlers-3.4.3.tar", last modified: Fri May 26 11:35:39 2023, max compression
```

## Comparing `news_crawlers-3.4.2.tar` & `news_crawlers-3.4.3.tar`

### file list

```diff
@@ -1,52 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 22:27:38.322678 news_crawlers-3.4.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 22:27:38.306678 news_crawlers-3.4.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 22:27:38.314678 news_crawlers-3.4.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-02-18 22:27:27.000000 news_crawlers-3.4.2/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-02-18 22:27:27.000000 news_crawlers-3.4.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-02-18 22:27:27.000000 news_crawlers-3.4.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    17931 2023-02-18 22:27:27.000000 news_crawlers-3.4.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-02-18 22:27:27.000000 news_crawlers-3.4.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-02-18 22:27:27.000000 news_crawlers-3.4.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-02-18 22:27:27.000000 news_crawlers-3.4.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7030 2023-02-18 22:27:38.322678 news_crawlers-3.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-02-18 22:27:27.000000 news_crawlers-3.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 22:27:38.314678 news_crawlers-3.4.2/news_crawlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-18 22:27:27.000000 news_crawlers-3.4.2/news_crawlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-02-18 22:27:27.000000 news_crawlers-3.4.2/news_crawlers/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-02-18 22:27:27.000000 news_crawlers-3.4.2/news_crawlers/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 22:27:38.318678 news_crawlers-3.4.2/news_crawlers/news_crawlers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-02-18 22:27:27.000000 news_crawlers-3.4.2/news_crawlers/news_crawlers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-02-18 22:27:27.000000 news_crawlers-3.4.2/news_crawlers/news_crawlers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-18 22:27:27.000000 news_crawlers-3.4.2/news_crawlers/news_crawlers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-02-18 22:27:27.000000 news_crawlers-3.4.2/news_crawlers/news_crawlers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-18 22:27:27.000000 news_crawlers-3.4.2/news_crawlers/news_crawlers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-02-18 22:27:27.000000 news_crawlers-3.4.2/news_crawlers/news_crawlers.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8372 2023-02-18 22:27:27.000000 news_crawlers-3.4.2/news_crawlers/notificators.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-02-18 22:27:27.000000 news_crawlers-3.4.2/news_crawlers/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-02-18 22:27:27.000000 news_crawlers-3.4.2/news_crawlers/scrape.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-02-18 22:27:27.000000 news_crawlers-3.4.2/news_crawlers/spiders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 22:27:38.318678 news_crawlers-3.4.2/news_crawlers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7030 2023-02-18 22:27:38.000000 news_crawlers-3.4.2/news_crawlers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-02-18 22:27:38.000000 news_crawlers-3.4.2/news_crawlers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-18 22:27:38.000000 news_crawlers-3.4.2/news_crawlers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-02-18 22:27:38.000000 news_crawlers-3.4.2/news_crawlers.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-02-18 22:27:38.000000 news_crawlers-3.4.2/news_crawlers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-18 22:27:38.000000 news_crawlers-3.4.2/news_crawlers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-02-18 22:27:27.000000 news_crawlers-3.4.2/news_crawlers.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-02-18 22:27:27.000000 news_crawlers-3.4.2/prepare_venv.bat
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-02-18 22:27:31.000000 news_crawlers-3.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-18 22:27:38.322678 news_crawlers-3.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-18 22:27:27.000000 news_crawlers-3.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 22:27:38.322678 news_crawlers-3.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-18 22:27:27.000000 news_crawlers-3.4.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-02-18 22:27:27.000000 news_crawlers-3.4.2/tests/mocks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 22:27:38.322678 news_crawlers-3.4.2/tests/res/
--rw-r--r--   0 runner    (1001) docker     (123)   122203 2023-02-18 22:27:27.000000 news_crawlers-3.4.2/tests/res/avtonet_test_html.html
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-02-18 22:27:27.000000 news_crawlers-3.4.2/tests/test_avtonet_spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-02-18 22:27:27.000000 news_crawlers-3.4.2/tests/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-02-18 22:27:27.000000 news_crawlers-3.4.2/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-02-18 22:27:27.000000 news_crawlers-3.4.2/tests/test_notificators.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-02-18 22:27:27.000000 news_crawlers-3.4.2/tests/test_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-02-18 22:27:27.000000 news_crawlers-3.4.2/tests/test_scrape.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-02-18 22:27:27.000000 news_crawlers-3.4.2/tests/test_spiders.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-02-18 22:27:27.000000 news_crawlers-3.4.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:35:39.630068 news_crawlers-3.4.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:35:39.626067 news_crawlers-3.4.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:35:39.626067 news_crawlers-3.4.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    17931 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7030 2023-05-26 11:35:39.630068 news_crawlers-3.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:35:39.626067 news_crawlers-3.4.3/news_crawlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/news_crawlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/news_crawlers/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/news_crawlers/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:35:39.630068 news_crawlers-3.4.3/news_crawlers/news_crawlers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/news_crawlers/news_crawlers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/news_crawlers/news_crawlers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/news_crawlers/news_crawlers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/news_crawlers/news_crawlers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/news_crawlers/news_crawlers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/news_crawlers/news_crawlers.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8372 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/news_crawlers/notificators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/news_crawlers/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/news_crawlers/scrape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/news_crawlers/spiders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:35:39.630068 news_crawlers-3.4.3/news_crawlers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7030 2023-05-26 11:35:39.000000 news_crawlers-3.4.3/news_crawlers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-26 11:35:39.000000 news_crawlers-3.4.3/news_crawlers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 11:35:39.000000 news_crawlers-3.4.3/news_crawlers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-26 11:35:39.000000 news_crawlers-3.4.3/news_crawlers.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-26 11:35:39.000000 news_crawlers-3.4.3/news_crawlers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-26 11:35:39.000000 news_crawlers-3.4.3/news_crawlers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/news_crawlers.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/prepare_venv.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-26 11:35:32.000000 news_crawlers-3.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 11:35:39.630068 news_crawlers-3.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:35:39.630068 news_crawlers-3.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/tests/mocks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:35:39.630068 news_crawlers-3.4.3/tests/res/
+-rw-r--r--   0 runner    (1001) docker     (123)   122203 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/tests/res/avtonet_test_html.html
+-rw-r--r--   0 runner    (1001) docker     (123)   230281 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/tests/res/bolha_test_html.html
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/tests/test_avtonet_spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/tests/test_bolha_spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/tests/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/tests/test_notificators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/tests/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/tests/test_scrape.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/tests/test_spiders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/tox.ini
```

### Comparing `news_crawlers-3.4.2/.github/workflows/main.yml` & `news_crawlers-3.4.3/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `news_crawlers-3.4.2/.pre-commit-config.yaml` & `news_crawlers-3.4.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `news_crawlers-3.4.2/.pylintrc` & `news_crawlers-3.4.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `news_crawlers-3.4.2/LICENSE.txt` & `news_crawlers-3.4.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `news_crawlers-3.4.2/PKG-INFO` & `news_crawlers-3.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: news_crawlers
-Version: 3.4.2
+Version: 3.4.3
 Summary: An extensible python library to create web crawlers which alert users on news.
 Author-email: Jost Prevc <jost.prevc@gmail.com>
 License: MIT
 Keywords: crawler,news
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `news_crawlers-3.4.2/README.md` & `news_crawlers-3.4.3/README.md`

 * *Files identical despite different names*

### Comparing `news_crawlers-3.4.2/news_crawlers/__main__.py` & `news_crawlers-3.4.3/news_crawlers/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,21 +37,24 @@
         spiders_to_run = list(scrape_configuration.spiders.keys())
 
     try:
         crawled_data = scrape.scrape(spiders_to_run, scrape_configuration.spiders, cache_folder)
         logger.debug("Scraping done.")
 
         # get difference with cached data
+        logger.debug("Checking for difference with items that were obtained previously...")
         diff = scrape.check_diff(cache_folder, crawled_data)
 
-        # send notifications to users (only if difference with cached data is found)
-        scrape.notify(diff, scrape_configuration.spiders)
-
         if diff:
             logger.debug(f"Found new items: {diff}")
+
+            # send notifications to users (only if difference with cached data is found)
+            logger.debug("Sending notifications")
+            scrape.notify(diff, scrape_configuration.spiders)
+            logger.debug("Notifications sent succesfully.")
         else:
             logger.debug("No new items were found.")
 
     except Exception as exc:  # pylint: disable=broad-except
         logger.exception("Exception occurred when running crawlers.", exc_info=exc)
     else:
         logger.debug("Crawlers were run successfully.")
```

### Comparing `news_crawlers-3.4.2/news_crawlers/configuration.py` & `news_crawlers-3.4.3/news_crawlers/configuration.py`

 * *Files identical despite different names*

### Comparing `news_crawlers-3.4.2/news_crawlers/news_crawlers.egg-info/PKG-INFO` & `news_crawlers-3.4.3/news_crawlers/news_crawlers.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `news_crawlers-3.4.2/news_crawlers/news_crawlers.yaml` & `news_crawlers-3.4.3/news_crawlers/news_crawlers.yaml`

 * *Files identical despite different names*

### Comparing `news_crawlers-3.4.2/news_crawlers/notificators.py` & `news_crawlers-3.4.3/news_crawlers/notificators.py`

 * *Files identical despite different names*

### Comparing `news_crawlers-3.4.2/news_crawlers/scrape.py` & `news_crawlers-3.4.3/news_crawlers/scrape.py`

 * *Files identical despite different names*

### Comparing `news_crawlers-3.4.2/news_crawlers.egg-info/PKG-INFO` & `news_crawlers-3.4.3/news_crawlers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: news-crawlers
-Version: 3.4.2
+Version: 3.4.3
 Summary: An extensible python library to create web crawlers which alert users on news.
 Author-email: Jost Prevc <jost.prevc@gmail.com>
 License: MIT
 Keywords: crawler,news
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `news_crawlers-3.4.2/news_crawlers.egg-info/SOURCES.txt` & `news_crawlers-3.4.3/news_crawlers.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -27,16 +27,19 @@
 news_crawlers.egg-info/top_level.txt
 news_crawlers/news_crawlers.egg-info/PKG-INFO
 news_crawlers/news_crawlers.egg-info/SOURCES.txt
 news_crawlers/news_crawlers.egg-info/dependency_links.txt
 news_crawlers/news_crawlers.egg-info/requires.txt
 news_crawlers/news_crawlers.egg-info/top_level.txt
 tests/__init__.py
+tests/conftest.py
 tests/mocks.py
 tests/test_avtonet_spider.py
+tests/test_bolha_spider.py
 tests/test_configuration.py
 tests/test_main.py
 tests/test_notificators.py
 tests/test_scheduler.py
 tests/test_scrape.py
 tests/test_spiders.py
-tests/res/avtonet_test_html.html
+tests/res/avtonet_test_html.html
+tests/res/bolha_test_html.html
```

### Comparing `news_crawlers-3.4.2/news_crawlers.yaml` & `news_crawlers-3.4.3/news_crawlers.yaml`

 * *Files identical despite different names*

### Comparing `news_crawlers-3.4.2/pyproject.toml` & `news_crawlers-3.4.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools", "setuptools-scm",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "news_crawlers"
-version = "3.4.2"
+version = "3.4.3"
 description = "An extensible python library to create web crawlers which alert users on news."
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = [ "crawler", "news",]
 classifiers = [ "Programming Language :: Python :: 3",]
 dependencies = [ "beautifulsoup4", "pydantic", "PyYAML", "requests", "schedule", "importlib_metadata",]
 [[project.authors]]
```

### Comparing `news_crawlers-3.4.2/tests/mocks.py` & `news_crawlers-3.4.3/tests/mocks.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Contains various mock classes which can be used in tests.
 """
-import dataclasses
 import pathlib
+from typing import Callable
 
 
 # pylint: disable=unused-argument
 
 
 class HttpsSessionMock:
     """
@@ -43,27 +43,42 @@
     def login(self, user, password):
         pass
 
     def sendmail(self, user, recipients, message):
         self.simulated_messages.append(message)
 
 
-def mock_get_raw_html() -> str:
-    mock_html_path = pathlib.Path(__file__).parent / "res" / "avtonet_test_html.html"
+def mock_get_raw_html(mock_html: str) -> str:
+    mock_html_path = pathlib.Path(__file__).parent / "res" / mock_html
 
     with open(mock_html_path, encoding="utf8") as file:
         html_content = file.read()
 
     return html_content
 
 
-@dataclasses.dataclass
 class MockRequestObject:
-    text = mock_get_raw_html()
+    def __init__(self, mock_html):
+        self.mock_html = mock_html
+        self.request_counter = 0
 
+    @property
+    def text(self) -> str:
+        self.request_counter += 1
+        return mock_get_raw_html(self.mock_html)
 
-def mock_requests_get(url, headers, timeout) -> MockRequestObject:
-    return MockRequestObject()
+    @property
+    def status_code(self) -> int:
+        return 200 if self.request_counter < 1 else 404
+
+
+def mock_requests_get(mock_html: str) -> Callable[[str, str, str], MockRequestObject]:
+    mock_request_obj = MockRequestObject(mock_html)
+
+    def mock_request_func(url: str, headers: str, timeout: str) -> MockRequestObject:
+        return mock_request_obj
+
+    return mock_request_func
 
 
 def send_text_mock(obj, subject, message):
     pass
```

### Comparing `news_crawlers-3.4.2/tests/res/avtonet_test_html.html` & `news_crawlers-3.4.3/tests/res/avtonet_test_html.html`

 * *Files identical despite different names*

### Comparing `news_crawlers-3.4.2/tests/test_configuration.py` & `news_crawlers-3.4.3/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `news_crawlers-3.4.2/tests/test_main.py` & `news_crawlers-3.4.3/tests/test_main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import json
 import os
 import pathlib
 import re
 
-import requests
 import pytest
 
 from news_crawlers.__main__ import main
 from news_crawlers import notificators
 from tests import mocks
 
 # pylint: disable=unused-argument
@@ -70,16 +69,16 @@
     assert not log_path.exists()
 
     main(("--log", str(log_path), "scrape", "--config", str(tmp_path / "news_crawlers.yaml")))
 
     assert log_path.exists()
 
 
+@pytest.mark.usefixtures("mock_request_avtonet")
 def test_running_scrape_command_returns_expected_items(monkeypatch, tmp_path: pathlib.Path, avtonet_dummy_config):
-    monkeypatch.setattr(requests, "get", mocks.mock_requests_get)
     monkeypatch.setattr(notificators.EmailNotificator, "send_text", mocks.send_text_mock)
 
     envs = {"EMAIL_USER": "dummy_email", "EMAIL_PASS": "dummy_pass"}
     monkeypatch.setattr(os, "environ", envs)
 
     main(
         (
```

### Comparing `news_crawlers-3.4.2/tests/test_notificators.py` & `news_crawlers-3.4.3/tests/test_notificators.py`

 * *Files identical despite different names*

### Comparing `news_crawlers-3.4.2/tests/test_scheduler.py` & `news_crawlers-3.4.3/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `news_crawlers-3.4.2/tests/test_scrape.py` & `news_crawlers-3.4.3/tests/test_scrape.py`

 * *Files identical despite different names*

### Comparing `news_crawlers-3.4.2/tox.ini` & `news_crawlers-3.4.3/tox.ini`

 * *Files identical despite different names*

