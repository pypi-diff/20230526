# Comparing `tmp/news_crawlers-3.4.3.tar.gz` & `tmp/news_crawlers-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "news_crawlers-3.4.3.tar", last modified: Fri May 26 11:35:39 2023, max compression
+gzip compressed data, was "news_crawlers-3.5.0.tar", last modified: Fri May 26 12:07:56 2023, max compression
```

## Comparing `news_crawlers-3.4.3.tar` & `news_crawlers-3.5.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:35:39.630068 news_crawlers-3.4.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:35:39.626067 news_crawlers-3.4.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:35:39.626067 news_crawlers-3.4.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    17931 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7030 2023-05-26 11:35:39.630068 news_crawlers-3.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:35:39.626067 news_crawlers-3.4.3/news_crawlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/news_crawlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/news_crawlers/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/news_crawlers/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:35:39.630068 news_crawlers-3.4.3/news_crawlers/news_crawlers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/news_crawlers/news_crawlers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/news_crawlers/news_crawlers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/news_crawlers/news_crawlers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/news_crawlers/news_crawlers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/news_crawlers/news_crawlers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/news_crawlers/news_crawlers.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8372 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/news_crawlers/notificators.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/news_crawlers/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/news_crawlers/scrape.py
--rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/news_crawlers/spiders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:35:39.630068 news_crawlers-3.4.3/news_crawlers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7030 2023-05-26 11:35:39.000000 news_crawlers-3.4.3/news_crawlers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-26 11:35:39.000000 news_crawlers-3.4.3/news_crawlers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 11:35:39.000000 news_crawlers-3.4.3/news_crawlers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-26 11:35:39.000000 news_crawlers-3.4.3/news_crawlers.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-26 11:35:39.000000 news_crawlers-3.4.3/news_crawlers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-26 11:35:39.000000 news_crawlers-3.4.3/news_crawlers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/news_crawlers.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/prepare_venv.bat
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-26 11:35:32.000000 news_crawlers-3.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 11:35:39.630068 news_crawlers-3.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:35:39.630068 news_crawlers-3.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/tests/mocks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:35:39.630068 news_crawlers-3.4.3/tests/res/
--rw-r--r--   0 runner    (1001) docker     (123)   122203 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/tests/res/avtonet_test_html.html
--rw-r--r--   0 runner    (1001) docker     (123)   230281 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/tests/res/bolha_test_html.html
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/tests/test_avtonet_spider.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/tests/test_bolha_spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/tests/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/tests/test_notificators.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/tests/test_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/tests/test_scrape.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/tests/test_spiders.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-26 11:35:28.000000 news_crawlers-3.4.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:07:56.204143 news_crawlers-3.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:07:56.196143 news_crawlers-3.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:07:56.200143 news_crawlers-3.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-26 12:07:45.000000 news_crawlers-3.5.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-26 12:07:45.000000 news_crawlers-3.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-26 12:07:45.000000 news_crawlers-3.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    17931 2023-05-26 12:07:45.000000 news_crawlers-3.5.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-26 12:07:45.000000 news_crawlers-3.5.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-26 12:07:45.000000 news_crawlers-3.5.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-26 12:07:45.000000 news_crawlers-3.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7030 2023-05-26 12:07:56.204143 news_crawlers-3.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-05-26 12:07:45.000000 news_crawlers-3.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:07:56.200143 news_crawlers-3.5.0/news_crawlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:07:45.000000 news_crawlers-3.5.0/news_crawlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-05-26 12:07:45.000000 news_crawlers-3.5.0/news_crawlers/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-26 12:07:45.000000 news_crawlers-3.5.0/news_crawlers/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:07:56.200143 news_crawlers-3.5.0/news_crawlers/news_crawlers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-05-26 12:07:45.000000 news_crawlers-3.5.0/news_crawlers/news_crawlers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-26 12:07:45.000000 news_crawlers-3.5.0/news_crawlers/news_crawlers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:07:45.000000 news_crawlers-3.5.0/news_crawlers/news_crawlers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-26 12:07:45.000000 news_crawlers-3.5.0/news_crawlers/news_crawlers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:07:45.000000 news_crawlers-3.5.0/news_crawlers/news_crawlers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-26 12:07:45.000000 news_crawlers-3.5.0/news_crawlers/news_crawlers.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8372 2023-05-26 12:07:45.000000 news_crawlers-3.5.0/news_crawlers/notificators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-26 12:07:45.000000 news_crawlers-3.5.0/news_crawlers/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-26 12:07:45.000000 news_crawlers-3.5.0/news_crawlers/scrape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-05-26 12:07:45.000000 news_crawlers-3.5.0/news_crawlers/spiders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:07:56.200143 news_crawlers-3.5.0/news_crawlers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7030 2023-05-26 12:07:56.000000 news_crawlers-3.5.0/news_crawlers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-26 12:07:56.000000 news_crawlers-3.5.0/news_crawlers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 12:07:56.000000 news_crawlers-3.5.0/news_crawlers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-26 12:07:56.000000 news_crawlers-3.5.0/news_crawlers.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-26 12:07:56.000000 news_crawlers-3.5.0/news_crawlers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-26 12:07:56.000000 news_crawlers-3.5.0/news_crawlers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-26 12:07:45.000000 news_crawlers-3.5.0/news_crawlers.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-26 12:07:45.000000 news_crawlers-3.5.0/prepare_venv.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-26 12:07:48.000000 news_crawlers-3.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 12:07:56.204143 news_crawlers-3.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-26 12:07:45.000000 news_crawlers-3.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:07:56.204143 news_crawlers-3.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:07:45.000000 news_crawlers-3.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-26 12:07:45.000000 news_crawlers-3.5.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-26 12:07:45.000000 news_crawlers-3.5.0/tests/mocks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:07:56.204143 news_crawlers-3.5.0/tests/res/
+-rw-r--r--   0 runner    (1001) docker     (123)   122203 2023-05-26 12:07:45.000000 news_crawlers-3.5.0/tests/res/avtonet_test_html.html
+-rw-r--r--   0 runner    (1001) docker     (123)   230281 2023-05-26 12:07:45.000000 news_crawlers-3.5.0/tests/res/bolha_test_html.html
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-26 12:07:45.000000 news_crawlers-3.5.0/tests/test_avtonet_spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-26 12:07:45.000000 news_crawlers-3.5.0/tests/test_bolha_spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-05-26 12:07:45.000000 news_crawlers-3.5.0/tests/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-05-26 12:07:45.000000 news_crawlers-3.5.0/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-05-26 12:07:45.000000 news_crawlers-3.5.0/tests/test_notificators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-26 12:07:45.000000 news_crawlers-3.5.0/tests/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-26 12:07:45.000000 news_crawlers-3.5.0/tests/test_scrape.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-26 12:07:45.000000 news_crawlers-3.5.0/tests/test_spiders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-26 12:07:45.000000 news_crawlers-3.5.0/tox.ini
```

### Comparing `news_crawlers-3.4.3/.github/workflows/main.yml` & `news_crawlers-3.5.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `news_crawlers-3.4.3/.pre-commit-config.yaml` & `news_crawlers-3.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `news_crawlers-3.4.3/.pylintrc` & `news_crawlers-3.5.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `news_crawlers-3.4.3/LICENSE.txt` & `news_crawlers-3.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `news_crawlers-3.4.3/PKG-INFO` & `news_crawlers-3.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: news_crawlers
-Version: 3.4.3
+Version: 3.5.0
 Summary: An extensible python library to create web crawlers which alert users on news.
 Author-email: Jost Prevc <jost.prevc@gmail.com>
 License: MIT
 Keywords: crawler,news
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `news_crawlers-3.4.3/README.md` & `news_crawlers-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `news_crawlers-3.4.3/news_crawlers/__main__.py` & `news_crawlers-3.5.0/news_crawlers/__main__.py`

 * *Files identical despite different names*

### Comparing `news_crawlers-3.4.3/news_crawlers/configuration.py` & `news_crawlers-3.5.0/news_crawlers/configuration.py`

 * *Files identical despite different names*

### Comparing `news_crawlers-3.4.3/news_crawlers/news_crawlers.egg-info/PKG-INFO` & `news_crawlers-3.5.0/news_crawlers/news_crawlers.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `news_crawlers-3.4.3/news_crawlers/news_crawlers.yaml` & `news_crawlers-3.5.0/news_crawlers/news_crawlers.yaml`

 * *Files identical despite different names*

### Comparing `news_crawlers-3.4.3/news_crawlers/notificators.py` & `news_crawlers-3.5.0/news_crawlers/notificators.py`

 * *Files identical despite different names*

### Comparing `news_crawlers-3.4.3/news_crawlers/scrape.py` & `news_crawlers-3.5.0/news_crawlers/scrape.py`

 * *Files identical despite different names*

### Comparing `news_crawlers-3.4.3/news_crawlers/spiders.py` & `news_crawlers-3.5.0/news_crawlers/spiders.py`

 * *Files 7% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
 class CarobniSvetSpider(Spider):
     name = "carobni_svet"
 
     @staticmethod
     def _get_images(bs_content: bs4.BeautifulSoup) -> list[dict]:
 
-        image_elements = bs_content.select("div[id=galerija]")[0].select("img")
+        image_elements = bs_content.select("ul[id=images]")[0].select("img")
 
         image_urls = [image.get("src") for image in image_elements]
 
         return [{"type": "image", "data": image_url} for image_url in image_urls]
 
     @staticmethod
     def _get_blog(bs_content: bs4.BeautifulSoup) -> list[dict]:
@@ -179,18 +179,18 @@
             listing_el = listing.select("a.link")
             price_el = listing.select("strong.price")
 
             if not listing_el or not price_el:
                 continue
 
             title = listing_el[0].text
-            href = listing_el[0].attrs["href"]
+            url = "https://www.bolha.com" + listing_el[0].attrs["href"]
             price = price_el[0].get_text(strip=True)
 
-            found_items.append({"query": query_name, "title": title, "price": price, "link": href})
+            found_items.append({"query": query_name, "title": title, "price": price, "url": url})
 
         return found_items
 
 
 def get_spider_by_name(name: str) -> type[Spider]:
     """
     Finds spider class with the 'name' attribute equal to the one specified.
```

### Comparing `news_crawlers-3.4.3/news_crawlers.egg-info/PKG-INFO` & `news_crawlers-3.5.0/news_crawlers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: news-crawlers
-Version: 3.4.3
+Version: 3.5.0
 Summary: An extensible python library to create web crawlers which alert users on news.
 Author-email: Jost Prevc <jost.prevc@gmail.com>
 License: MIT
 Keywords: crawler,news
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `news_crawlers-3.4.3/news_crawlers.egg-info/SOURCES.txt` & `news_crawlers-3.5.0/news_crawlers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `news_crawlers-3.4.3/news_crawlers.yaml` & `news_crawlers-3.5.0/news_crawlers.yaml`

 * *Files identical despite different names*

### Comparing `news_crawlers-3.4.3/pyproject.toml` & `news_crawlers-3.5.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools", "setuptools-scm",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "news_crawlers"
-version = "3.4.3"
+version = "3.5.0"
 description = "An extensible python library to create web crawlers which alert users on news."
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = [ "crawler", "news",]
 classifiers = [ "Programming Language :: Python :: 3",]
 dependencies = [ "beautifulsoup4", "pydantic", "PyYAML", "requests", "schedule", "importlib_metadata",]
 [[project.authors]]
```

### Comparing `news_crawlers-3.4.3/tests/mocks.py` & `news_crawlers-3.5.0/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `news_crawlers-3.4.3/tests/res/avtonet_test_html.html` & `news_crawlers-3.5.0/tests/res/avtonet_test_html.html`

 * *Files identical despite different names*

### Comparing `news_crawlers-3.4.3/tests/res/bolha_test_html.html` & `news_crawlers-3.5.0/tests/res/bolha_test_html.html`

 * *Files identical despite different names*

### Comparing `news_crawlers-3.4.3/tests/test_avtonet_spider.py` & `news_crawlers-3.5.0/tests/test_avtonet_spider.py`

 * *Files identical despite different names*

### Comparing `news_crawlers-3.4.3/tests/test_bolha_spider.py` & `news_crawlers-3.5.0/tests/test_bolha_spider.py`

 * *Files identical despite different names*

### Comparing `news_crawlers-3.4.3/tests/test_configuration.py` & `news_crawlers-3.5.0/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `news_crawlers-3.4.3/tests/test_main.py` & `news_crawlers-3.5.0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `news_crawlers-3.4.3/tests/test_notificators.py` & `news_crawlers-3.5.0/tests/test_notificators.py`

 * *Files identical despite different names*

### Comparing `news_crawlers-3.4.3/tests/test_scheduler.py` & `news_crawlers-3.5.0/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `news_crawlers-3.4.3/tests/test_scrape.py` & `news_crawlers-3.5.0/tests/test_scrape.py`

 * *Files identical despite different names*

### Comparing `news_crawlers-3.4.3/tox.ini` & `news_crawlers-3.5.0/tox.ini`

 * *Files identical despite different names*

