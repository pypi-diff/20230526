# Comparing `tmp/duckduckgo_search-3.4.1.tar.gz` & `tmp/duckduckgo_search-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckduckgo_search-3.4.1.tar", last modified: Thu May 25 21:11:40 2023, max compression
+gzip compressed data, was "duckduckgo_search-3.5.0.tar", last modified: Fri May 26 21:24:18 2023, max compression
```

## Comparing `duckduckgo_search-3.4.1.tar` & `duckduckgo_search-3.5.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:11:40.197756 duckduckgo_search-3.4.1/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-05-25 21:11:23.000000 duckduckgo_search-3.4.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    14676 2023-05-25 21:11:40.197756 duckduckgo_search-3.4.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)    13561 2023-05-25 21:11:23.000000 duckduckgo_search-3.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:11:40.197756 duckduckgo_search-3.4.1/duckduckgo_search/
--rwxr-xr-x   0 runner    (1001) docker     (123)      607 2023-05-25 21:11:23.000000 duckduckgo_search-3.4.1/duckduckgo_search/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      138 2023-05-25 21:11:23.000000 duckduckgo_search-3.4.1/duckduckgo_search/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15809 2023-05-25 21:11:23.000000 duckduckgo_search-3.4.1/duckduckgo_search/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-05-25 21:11:23.000000 duckduckgo_search-3.4.1/duckduckgo_search/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    27457 2023-05-25 21:11:23.000000 duckduckgo_search-3.4.1/duckduckgo_search/duckduckgo_search.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       22 2023-05-25 21:11:23.000000 duckduckgo_search-3.4.1/duckduckgo_search/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:11:40.197756 duckduckgo_search-3.4.1/duckduckgo_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14676 2023-05-25 21:11:40.000000 duckduckgo_search-3.4.1/duckduckgo_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-25 21:11:40.000000 duckduckgo_search-3.4.1/duckduckgo_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 21:11:40.000000 duckduckgo_search-3.4.1/duckduckgo_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-25 21:11:40.000000 duckduckgo_search-3.4.1/duckduckgo_search.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-25 21:11:40.000000 duckduckgo_search-3.4.1/duckduckgo_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-25 21:11:40.000000 duckduckgo_search-3.4.1/duckduckgo_search.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-25 21:11:23.000000 duckduckgo_search-3.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 21:11:40.197756 duckduckgo_search-3.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:11:40.197756 duckduckgo_search-3.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-05-25 21:11:23.000000 duckduckgo_search-3.4.1/tests/test_duckduckgo_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:24:18.935401 duckduckgo_search-3.5.0/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-05-26 21:23:58.000000 duckduckgo_search-3.5.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    15131 2023-05-26 21:24:18.935401 duckduckgo_search-3.5.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14016 2023-05-26 21:23:58.000000 duckduckgo_search-3.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:24:18.935401 duckduckgo_search-3.5.0/duckduckgo_search/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      607 2023-05-26 21:23:58.000000 duckduckgo_search-3.5.0/duckduckgo_search/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      138 2023-05-26 21:23:58.000000 duckduckgo_search-3.5.0/duckduckgo_search/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16092 2023-05-26 21:23:58.000000 duckduckgo_search-3.5.0/duckduckgo_search/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-05-26 21:23:58.000000 duckduckgo_search-3.5.0/duckduckgo_search/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30418 2023-05-26 21:23:58.000000 duckduckgo_search-3.5.0/duckduckgo_search/duckduckgo_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       22 2023-05-26 21:23:58.000000 duckduckgo_search-3.5.0/duckduckgo_search/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:24:18.935401 duckduckgo_search-3.5.0/duckduckgo_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15131 2023-05-26 21:24:18.000000 duckduckgo_search-3.5.0/duckduckgo_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-26 21:24:18.000000 duckduckgo_search-3.5.0/duckduckgo_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 21:24:18.000000 duckduckgo_search-3.5.0/duckduckgo_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-26 21:24:18.000000 duckduckgo_search-3.5.0/duckduckgo_search.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-26 21:24:18.000000 duckduckgo_search-3.5.0/duckduckgo_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-26 21:24:18.000000 duckduckgo_search-3.5.0/duckduckgo_search.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-26 21:23:58.000000 duckduckgo_search-3.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 21:24:18.935401 duckduckgo_search-3.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:24:18.935401 duckduckgo_search-3.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-05-26 21:23:58.000000 duckduckgo_search-3.5.0/tests/test_duckduckgo_search.py
```

### Comparing `duckduckgo_search-3.4.1/LICENSE.md` & `duckduckgo_search-3.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.4.1/PKG-INFO` & `duckduckgo_search-3.5.0/duckduckgo_search.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: duckduckgo_search
-Version: 3.4.1
+Name: duckduckgo-search
+Version: 3.5.0
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -208,36 +208,46 @@
     """DuckDuckGo text search generator. Query params: https://duckduckgo.com/params
 
     Args:
         keywords: keywords for query.
         region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
         safesearch: on, moderate, off. Defaults to "moderate".
         timelimit: d, w, m, y. Defaults to None.
-
+        backend: api, html, lite. Defaults to api.
+            api - collect data from https://duckduckgo.com,
+            html - collect data from https://html.duckduckgo.com,
+            lite - collect data from https://lite.duckduckgo.com.
     Yields:
         dict with search results.
 
     """
 ```
 ***Example***
 ```python
 from duckduckgo_search import DDGS
 
 ddgs = DDGS()
 
-keywords = 'Bella Ciao'
+keywords = 'live free or die'
 ddgs_text_gen = ddgs.text(keywords, region='wt-wt', safesearch='Off', timelimit='y')
 for r in ddgs_text_gen:
 	print(r)
 
 # Searching for pdf files
 keywords = 'russia filetype:pdf'
 ddgs_text_gen = ddgs.text(keywords, region='wt-wt', safesearch='Off', timelimit='y')
 for r in ddgs_text_gen:
 	print(r)
+
+# Using lite backend and limit the number of results to 10
+from itertools import islice
+
+ddgs_text_gen = DDGS().text("notes from a dead house", backend="lite")
+for r in islice(ddgs_text_gen, 10):
+	print(r)
 ```
 
 
 [Go To TOP](#TOP)
 
 ## 2. answers() - instant answers by duckduckgo.com
```

### Comparing `duckduckgo_search-3.4.1/README.md` & `duckduckgo_search-3.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -183,36 +183,46 @@
     """DuckDuckGo text search generator. Query params: https://duckduckgo.com/params
 
     Args:
         keywords: keywords for query.
         region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
         safesearch: on, moderate, off. Defaults to "moderate".
         timelimit: d, w, m, y. Defaults to None.
-
+        backend: api, html, lite. Defaults to api.
+            api - collect data from https://duckduckgo.com,
+            html - collect data from https://html.duckduckgo.com,
+            lite - collect data from https://lite.duckduckgo.com.
     Yields:
         dict with search results.
 
     """
 ```
 ***Example***
 ```python
 from duckduckgo_search import DDGS
 
 ddgs = DDGS()
 
-keywords = 'Bella Ciao'
+keywords = 'live free or die'
 ddgs_text_gen = ddgs.text(keywords, region='wt-wt', safesearch='Off', timelimit='y')
 for r in ddgs_text_gen:
 	print(r)
 
 # Searching for pdf files
 keywords = 'russia filetype:pdf'
 ddgs_text_gen = ddgs.text(keywords, region='wt-wt', safesearch='Off', timelimit='y')
 for r in ddgs_text_gen:
 	print(r)
+
+# Using lite backend and limit the number of results to 10
+from itertools import islice
+
+ddgs_text_gen = DDGS().text("notes from a dead house", backend="lite")
+for r in islice(ddgs_text_gen, 10):
+	print(r)
 ```
 
 
 [Go To TOP](#TOP)
 
 ## 2. answers() - instant answers by duckduckgo.com
```

### Comparing `duckduckgo_search-3.4.1/duckduckgo_search/__init__.py` & `duckduckgo_search-3.5.0/duckduckgo_search/__init__.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.4.1/duckduckgo_search/cli.py` & `duckduckgo_search-3.5.0/duckduckgo_search/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -142,15 +142,15 @@
 @cli.command()
 def version():
     print(__version__)
     return __version__
 
 
 @cli.command()
-@click.option("-k", "--keywords", help="text search, keywords for query")
+@click.option("-k", "--keywords", required=True, help="text search, keywords for query")
 @click.option(
     "-r",
     "--region",
     default="wt-wt",
     help="wt-wt, us-en, uk-en, ru-ru, etc. - search region https://duckduckgo.com/params",
 )
 @click.option(
@@ -182,14 +182,21 @@
 @click.option(
     "-d",
     "--download",
     is_flag=True,
     default=False,
     help="download results to 'keywords' folder",
 )
+@click.option(
+    "-b",
+    "--backend",
+    default="api",
+    type=click.Choice(["api", "html", "lite"]),
+    help="which backend to use, default=api",
+)
 def text(keywords, output, download, max_results, *args, **kwargs):
     data = []
     for r in DDGS().text(keywords=keywords, *args, **kwargs):
         if len(data) >= max_results:
             break
         data.append(r)
     keywords = sanitize_keywords(keywords)
@@ -201,15 +208,17 @@
     elif output == "json":
         save_json(f"{filename}.json", data)
     if download:
         download_results(keywords, data)
 
 
 @cli.command()
-@click.option("-k", "--keywords", help="answers search, keywords for query")
+@click.option(
+    "-k", "--keywords", required=True, help="answers search, keywords for query"
+)
 @click.option(
     "-o",
     "--output",
     default="print",
     help="csv, json (save the results to a csv or json file)",
 )
 def answers(keywords, output, *args, **kwargs):
@@ -222,15 +231,15 @@
     elif output == "csv":
         save_csv(f"{filename}.csv", data)
     elif output == "json":
         save_json(f"{filename}.json", data)
 
 
 @cli.command()
-@click.option("-k", "--keywords", help="keywords for query")
+@click.option("-k", "--keywords", required=True, help="keywords for query")
 @click.option(
     "-r",
     "--region",
     default="wt-wt",
     help="wt-wt, us-en, uk-en, ru-ru, etc. - search region https://duckduckgo.com/params",
 )
 @click.option(
@@ -329,15 +338,15 @@
     elif output == "json":
         save_json(f"{filename}.json", data)
     if download:
         download_results(keywords, data, images=True)
 
 
 @cli.command()
-@click.option("-k", "--keywords", help="keywords for query")
+@click.option("-k", "--keywords", required=True, help="keywords for query")
 @click.option(
     "-r",
     "--region",
     default="wt-wt",
     help="wt-wt, us-en, uk-en, ru-ru, etc. - search region https://duckduckgo.com/params",
 )
 @click.option(
@@ -393,15 +402,15 @@
     elif output == "csv":
         save_csv(f"{filename}.csv", data)
     elif output == "json":
         save_json(f"{filename}.json", data)
 
 
 @cli.command()
-@click.option("-k", "--keywords", help="keywords for query")
+@click.option("-k", "--keywords", required=True, help="keywords for query")
 @click.option(
     "-r",
     "--region",
     default="wt-wt",
     help="wt-wt, us-en, uk-en, ru-ru, etc. - search region https://duckduckgo.com/params",
 )
 @click.option(
@@ -442,15 +451,15 @@
     elif output == "csv":
         save_csv(f"{filename}.csv", data)
     elif output == "json":
         save_json(f"{filename}.json", data)
 
 
 @cli.command()
-@click.option("-k", "--keywords", help="keywords for query")
+@click.option("-k", "--keywords", required=True, help="keywords for query")
 @click.option(
     "-p",
     "--place",
     default=None,
     help="simplified search - if set, the other parameters are not used",
 )
 @click.option("-s", "--street", default=None, help="house number/street")
@@ -500,15 +509,15 @@
     elif output == "csv":
         save_csv(f"{filename}.csv", data)
     elif output == "json":
         save_json(f"{filename}.json", data)
 
 
 @cli.command()
-@click.option("-k", "--keywords", help="text for translation")
+@click.option("-k", "--keywords", required=True, help="text for translation")
 @click.option(
     "-f",
     "--from_",
     help="What language to translate from (defaults automatically)",
 )
 @click.option(
     "-t",
@@ -531,15 +540,15 @@
     elif output == "csv":
         save_csv(f"{filename}.csv", data)
     elif output == "json":
         save_json(f"{filename}.json", data)
 
 
 @cli.command()
-@click.option("-k", "--keywords", help="keywords for query")
+@click.option("-k", "--keywords", required=True, help="keywords for query")
 @click.option(
     "-r",
     "--region",
     default="wt-wt",
     help="wt-wt, us-en, uk-en, ru-ru, etc. - search region https://duckduckgo.com/params",
 )
 @click.option(
```

### Comparing `duckduckgo_search-3.4.1/duckduckgo_search/compat.py` & `duckduckgo_search-3.5.0/duckduckgo_search/compat.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.4.1/duckduckgo_search/duckduckgo_search.py` & `duckduckgo_search-3.5.0/duckduckgo_search/duckduckgo_search.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 import re
 from collections import deque
 from dataclasses import dataclass
 from datetime import datetime
 from decimal import Decimal
 from html import unescape
+from itertools import cycle
 from time import sleep
 from typing import Deque, Dict, Iterator, Optional, Set
 from urllib.parse import unquote
 
 import requests
 from lxml import html
 from requests.models import Response
@@ -94,21 +95,50 @@
 
     def _normalize(self, raw_html: str) -> str:
         """strip HTML tags"""
         if raw_html:
             return unescape(re.sub(REGEX_STRIP_TAGS, "", raw_html))
         return ""
 
-    '''
     def text(
         self,
         keywords: str,
         region: str = "wt-wt",
         safesearch: str = "moderate",
         timelimit: Optional[str] = None,
+        backend: str = "api",
+    ) -> Iterator[dict]:
+        """DuckDuckGo text search generator. Query params: https://duckduckgo.com/params
+
+        Args:
+            keywords: keywords for query.
+            region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
+            safesearch: on, moderate, off. Defaults to "moderate".
+            timelimit: d, w, m, y. Defaults to None.
+            backend: api, html, lite. Defaults to api.
+                api - collect data from https://duckduckgo.com,
+                html - collect data from https://html.duckduckgo.com,
+                lite - collect data from https://lite.duckduckgo.com.
+        Yields:
+            dict with search results.
+
+        """
+        if backend == "api":
+            yield from self._text_api(keywords, region, safesearch, timelimit)
+        elif backend == "html":
+            yield from self._text_html(keywords, region, safesearch, timelimit)
+        elif backend == "lite":
+            yield from self._text_lite(keywords, region, timelimit)
+
+    def _text_api(
+        self,
+        keywords: str,
+        region: str = "wt-wt",
+        safesearch: str = "moderate",
+        timelimit: Optional[str] = None,
     ) -> Iterator[dict]:
         """DuckDuckGo text search generator. Query params: https://duckduckgo.com/params
 
         Args:
             keywords: keywords for query.
             region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
             safesearch: on, moderate, off. Defaults to "moderate".
@@ -118,14 +148,15 @@
             dict with search results.
 
         """
         assert keywords, "keywords is mandatory"
 
         vqd = self._get_vqd(keywords)
         assert vqd, "error in getting vqd"
+        sleep(0.75)
 
         payload = {
             "q": keywords,  #
             "kl": region,
             "l": region,
             "s": 0,
             "df": timelimit,
@@ -140,53 +171,45 @@
             payload["sp"] = "0"
             payload["ex"] = "-1"
         elif safesearch == "on":  # strict
             payload["sp"] = "0"
             payload["p"] = "1"
 
         cache = set()
-        for _ in range(10):
+        for s in ("0", "20", "70", "120"):
+            payload["s"] = s
             resp = self._get_url(
                 "GET", "https://links.duckduckgo.com/d.js", params=payload
             )
             if resp is None:
                 break
             try:
                 page_data = resp.json().get("results", None)
             except Exception:
                 break
             if page_data is None:
                 break
 
-            result_exists = False
             for row in page_data:
-                if "n" in row:
-                    payload["s"] = row["n"].split("s=")[-1].split("&")[0]
                 href = row.get("u", None)
                 if (
                     href
                     and href not in cache
                     and href != f"http://www.google.com/search?q={keywords}"
                 ):
                     cache.add(href)
                     body = self._normalize(row["a"])
                     if body:
-                        result_exists = True
                         yield {
                             "title": self._normalize(row["t"]),
                             "href": href,
                             "body": body,
                         }
-                elif result_exists is False:
-                    break
-            if result_exists is False:
-                break
-    '''
 
-    def text(
+    def _text_html(
         self,
         keywords: str,
         region: str = "wt-wt",
         safesearch: str = "moderate",
         timelimit: Optional[str] = None,
     ) -> Iterator[dict]:
         """DuckDuckGo text search generator. Query params: https://duckduckgo.com/params
@@ -202,59 +225,119 @@
 
         """
         assert keywords, "keywords is mandatory"
 
         safesearch_base = {"on": 1, "moderate": -1, "off": -2}
         payload = {
             "q": keywords,
-            "l": region,
+            "kl": region,
             "p": safesearch_base[safesearch.lower()],
             "df": timelimit,
         }
         cache: Set[str] = set()
         for _ in range(10):
             resp = self._get_url(
                 "POST", "https://html.duckduckgo.com/html", data=payload
             )
             if resp is None:
                 break
+
             tree = html.fromstring(resp.content)
             if tree.xpath('//div[@class="no-results"]/text()'):
                 return
-            result_exists = False
+
             for e in tree.xpath('//div[contains(@class, "results_links")]'):
                 href = e.xpath('.//a[contains(@class, "result__a")]/@href')
                 href = href[0] if href else None
                 if (
                     href
                     and href not in cache
                     and href != f"http://www.google.com/search?q={keywords}"
                 ):
                     cache.add(href)
                     title = e.xpath('.//a[contains(@class, "result__a")]/text()')
                     body = e.xpath('.//a[contains(@class, "result__snippet")]//text()')
-                    result_exists = True
                     yield {
                         "title": self._normalize(title[0]) if title else None,
                         "href": href,
                         "body": self._normalize("".join(body)) if body else None,
                     }
 
-            if result_exists is False:
-                break
-
             next_page = tree.xpath('.//div[@class="nav-link"]')
             next_page = next_page[-1] if next_page else None
             if next_page is None:
                 return
 
             names = next_page.xpath('.//input[@type="hidden"]/@name')
             values = next_page.xpath('.//input[@type="hidden"]/@value')
             payload = {n: v for n, v in zip(names, values)}
-            sleep(1)
+            sleep(0.75)
+
+    def _text_lite(
+        self,
+        keywords: str,
+        region: str = "wt-wt",
+        timelimit: Optional[str] = None,
+    ) -> Iterator[dict]:
+        """DuckDuckGo text search generator. Query params: https://duckduckgo.com/params
+
+        Args:
+            keywords: keywords for query.
+            region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
+            timelimit: d, w, m, y. Defaults to None.
+
+        Yields:
+            dict with search results.
+
+        """
+        assert keywords, "keywords is mandatory"
+
+        payload = {
+            "q": keywords,
+            "kl": region,
+            "df": timelimit,
+        }
+        cache: Set[str] = set()
+        for s in ("0", "20", "70", "120"):
+            payload["s"] = s
+            resp = self._get_url(
+                "POST", "https://lite.duckduckgo.com/lite/", data=payload
+            )
+            if resp is None:
+                break
+
+            tree = html.fromstring(resp.content)
+            if "No more results." in tree.xpath("//table[1]//text()"):
+                return
+
+            result_exists = False
+            for i, e in zip(cycle(range(1, 5)), tree.xpath("//table[last()]//tr")):
+                if i == 1:
+                    href = e.xpath(".//a//@href")
+                    href = href[0] if href else None
+                    if (
+                        href is None
+                        or href in cache
+                        or href == f"http://www.google.com/search?q={keywords}"
+                    ):
+                        continue
+                    title = e.xpath(".//a//text()")[0]
+                elif i == 2:
+                    body = e.xpath(".//td[@class='result-snippet']//text()")
+                    body = "".join(body).strip()
+                elif i == 3:
+                    result_exists = True
+                    yield {
+                        "href": href,
+                        "title": title,
+                        "body": body,
+                    }
+            if result_exists is False:
+                break
+            sleep(0.75)
 
     def images(
         self,
         keywords: str,
         region: str = "wt-wt",
         safesearch: str = "moderate",
         timelimit: Optional[str] = None,
@@ -286,14 +369,15 @@
             dict with image search results.
 
         """
         assert keywords, "keywords is mandatory"
 
         vqd = self._get_vqd(keywords)
         assert vqd, "error in getting vqd"
+        sleep(0.75)
 
         safesearch_base = {"on": 1, "moderate": 1, "off": -1}
         timelimit = f"time:{timelimit}" if timelimit else ""
         size = f"size:{size}" if size else ""
         color = f"color:{color}" if color else ""
         type_image = f"type:{type_image}" if type_image else ""
         layout = f"layout:{layout}" if layout else ""
```

### Comparing `duckduckgo_search-3.4.1/duckduckgo_search.egg-info/PKG-INFO` & `duckduckgo_search-3.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: duckduckgo-search
-Version: 3.4.1
+Name: duckduckgo_search
+Version: 3.5.0
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -208,36 +208,46 @@
     """DuckDuckGo text search generator. Query params: https://duckduckgo.com/params
 
     Args:
         keywords: keywords for query.
         region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
         safesearch: on, moderate, off. Defaults to "moderate".
         timelimit: d, w, m, y. Defaults to None.
-
+        backend: api, html, lite. Defaults to api.
+            api - collect data from https://duckduckgo.com,
+            html - collect data from https://html.duckduckgo.com,
+            lite - collect data from https://lite.duckduckgo.com.
     Yields:
         dict with search results.
 
     """
 ```
 ***Example***
 ```python
 from duckduckgo_search import DDGS
 
 ddgs = DDGS()
 
-keywords = 'Bella Ciao'
+keywords = 'live free or die'
 ddgs_text_gen = ddgs.text(keywords, region='wt-wt', safesearch='Off', timelimit='y')
 for r in ddgs_text_gen:
 	print(r)
 
 # Searching for pdf files
 keywords = 'russia filetype:pdf'
 ddgs_text_gen = ddgs.text(keywords, region='wt-wt', safesearch='Off', timelimit='y')
 for r in ddgs_text_gen:
 	print(r)
+
+# Using lite backend and limit the number of results to 10
+from itertools import islice
+
+ddgs_text_gen = DDGS().text("notes from a dead house", backend="lite")
+for r in islice(ddgs_text_gen, 10):
+	print(r)
 ```
 
 
 [Go To TOP](#TOP)
 
 ## 2. answers() - instant answers by duckduckgo.com
```

### Comparing `duckduckgo_search-3.4.1/pyproject.toml` & `duckduckgo_search-3.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.4.1/tests/test_duckduckgo_search.py` & `duckduckgo_search-3.5.0/tests/test_duckduckgo_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,32 @@
     counter = 0
     for i, x in enumerate(results_gen):
         counter += 1
         if i >= 25:
             break
     assert counter >= 25
 
+def test_text_html():
+    results_gen = DDGS().text("cat", backend="html")
+    counter = 0
+    for i, x in enumerate(results_gen):
+        counter += 1
+        if i >= 25:
+            break
+    assert counter >= 25
+
+def test_text_lite():
+    results_gen = DDGS().text("cat", backend="lite")
+    counter = 0
+    for i, x in enumerate(results_gen):
+        counter += 1
+        if i >= 25:
+            break
+    assert counter >= 25
+
 
 def test_images():
     results_gen = DDGS().images("cat")
     counter = 0
     for i, x in enumerate(results_gen):
         counter += 1
         if i >= 150:
```

