# Comparing `tmp/yetanotherpicsearch-1.9.1.tar.gz` & `tmp/yetanotherpicsearch-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yetanotherpicsearch-1.9.1.tar", max compression
+gzip compressed data, was "yetanotherpicsearch-1.9.2.tar", max compression
```

## Comparing `yetanotherpicsearch-1.9.1.tar` & `yetanotherpicsearch-1.9.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    35149 2023-05-25 16:43:59.139602 yetanotherpicsearch-1.9.1/LICENSE
--rw-r--r--   0        0        0     2041 2023-05-25 16:43:59.139602 yetanotherpicsearch-1.9.1/README.md
--rw-r--r--   0        0        0     9488 2023-05-25 16:43:59.139602 yetanotherpicsearch-1.9.1/YetAnotherPicSearch/__init__.py
--rw-r--r--   0        0        0     2089 2023-05-25 16:43:59.139602 yetanotherpicsearch-1.9.1/YetAnotherPicSearch/ascii2d.py
--rw-r--r--   0        0        0      657 2023-05-25 16:43:59.139602 yetanotherpicsearch-1.9.1/YetAnotherPicSearch/baidu.py
--rw-r--r--   0        0        0     2781 2023-05-25 16:43:59.139602 yetanotherpicsearch-1.9.1/YetAnotherPicSearch/config.py
--rw-r--r--   0        0        0     5086 2023-05-25 16:43:59.139602 yetanotherpicsearch-1.9.1/YetAnotherPicSearch/ehentai.py
--rw-r--r--   0        0        0     1195 2023-05-25 16:43:59.139602 yetanotherpicsearch-1.9.1/YetAnotherPicSearch/google.py
--rw-r--r--   0        0        0     1959 2023-05-25 16:43:59.139602 yetanotherpicsearch-1.9.1/YetAnotherPicSearch/iqdb.py
--rw-r--r--   0        0        0     3132 2023-05-25 16:43:59.139602 yetanotherpicsearch-1.9.1/YetAnotherPicSearch/nhentai.py
--rw-r--r--   0        0        0      924 2023-05-25 16:43:59.139602 yetanotherpicsearch-1.9.1/YetAnotherPicSearch/nhentai_model.py
--rw-r--r--   0        0        0     6003 2023-05-25 16:43:59.139602 yetanotherpicsearch-1.9.1/YetAnotherPicSearch/saucenao.py
--rw-r--r--   0        0        0     6656 2023-05-25 16:43:59.139602 yetanotherpicsearch-1.9.1/YetAnotherPicSearch/utils.py
--rw-r--r--   0        0        0     1827 2023-05-25 16:43:59.139602 yetanotherpicsearch-1.9.1/YetAnotherPicSearch/whatanime.py
--rw-r--r--   0        0        0     1075 2023-05-25 16:43:59.139602 yetanotherpicsearch-1.9.1/YetAnotherPicSearch/yandex.py
--rw-r--r--   0        0        0     1432 2023-05-25 16:43:59.147602 yetanotherpicsearch-1.9.1/pyproject.toml
--rw-r--r--   0        0        0     3458 1970-01-01 00:00:00.000000 yetanotherpicsearch-1.9.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-26 15:29:43.898918 yetanotherpicsearch-1.9.2/LICENSE
+-rw-r--r--   0        0        0     2041 2023-05-26 15:29:43.898918 yetanotherpicsearch-1.9.2/README.md
+-rw-r--r--   0        0        0     9390 2023-05-26 15:29:43.898918 yetanotherpicsearch-1.9.2/YetAnotherPicSearch/__init__.py
+-rw-r--r--   0        0        0     2089 2023-05-26 15:29:43.898918 yetanotherpicsearch-1.9.2/YetAnotherPicSearch/ascii2d.py
+-rw-r--r--   0        0        0      657 2023-05-26 15:29:43.898918 yetanotherpicsearch-1.9.2/YetAnotherPicSearch/baidu.py
+-rw-r--r--   0        0        0     2781 2023-05-26 15:29:43.898918 yetanotherpicsearch-1.9.2/YetAnotherPicSearch/config.py
+-rw-r--r--   0        0        0     5086 2023-05-26 15:29:43.898918 yetanotherpicsearch-1.9.2/YetAnotherPicSearch/ehentai.py
+-rw-r--r--   0        0        0     1195 2023-05-26 15:29:43.898918 yetanotherpicsearch-1.9.2/YetAnotherPicSearch/google.py
+-rw-r--r--   0        0        0     1959 2023-05-26 15:29:43.898918 yetanotherpicsearch-1.9.2/YetAnotherPicSearch/iqdb.py
+-rw-r--r--   0        0        0     3132 2023-05-26 15:29:43.898918 yetanotherpicsearch-1.9.2/YetAnotherPicSearch/nhentai.py
+-rw-r--r--   0        0        0      924 2023-05-26 15:29:43.898918 yetanotherpicsearch-1.9.2/YetAnotherPicSearch/nhentai_model.py
+-rw-r--r--   0        0        0     6003 2023-05-26 15:29:43.898918 yetanotherpicsearch-1.9.2/YetAnotherPicSearch/saucenao.py
+-rw-r--r--   0        0        0     6751 2023-05-26 15:29:43.898918 yetanotherpicsearch-1.9.2/YetAnotherPicSearch/utils.py
+-rw-r--r--   0        0        0     1827 2023-05-26 15:29:43.898918 yetanotherpicsearch-1.9.2/YetAnotherPicSearch/whatanime.py
+-rw-r--r--   0        0        0     1075 2023-05-26 15:29:43.898918 yetanotherpicsearch-1.9.2/YetAnotherPicSearch/yandex.py
+-rw-r--r--   0        0        0     1432 2023-05-26 15:29:43.906918 yetanotherpicsearch-1.9.2/pyproject.toml
+-rw-r--r--   0        0        0     3458 1970-01-01 00:00:00.000000 yetanotherpicsearch-1.9.2/PKG-INFO
```

### Comparing `yetanotherpicsearch-1.9.1/LICENSE` & `yetanotherpicsearch-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yetanotherpicsearch-1.9.1/README.md` & `yetanotherpicsearch-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `yetanotherpicsearch-1.9.1/YetAnotherPicSearch/__init__.py` & `yetanotherpicsearch-1.9.2/YetAnotherPicSearch/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 from cachetools import TTLCache
 from httpx import AsyncClient
 from nonebot.adapters.onebot.v11 import (
     ActionFailed,
     Bot,
     GroupMessageEvent,
-    LifecycleMetaEvent,
     Message,
     MessageEvent,
     PrivateMessageEvent,
 )
 from nonebot.log import logger
 from nonebot.matcher import Matcher
 from nonebot.plugin.on import on_message
@@ -40,18 +39,14 @@
     TTLCache,
     filename="pic_search_cache",
     maxsize=config.cache_expire * 100,
     ttl=config.cache_expire * 24 * 60 * 60,
 )
 
 
-def check_first_connect(_: LifecycleMetaEvent) -> bool:
-    return True
-
-
 def contains_image(event: MessageEvent) -> bool:
     message = event.reply.message if event.reply else event.message
     return bool([i for i in message if i.type == "image"])
 
 
 def message_needs_handling(bot: Bot, event: MessageEvent) -> bool:
     plain_text = event.message.extract_plain_text().strip()
```

### Comparing `yetanotherpicsearch-1.9.1/YetAnotherPicSearch/ascii2d.py` & `yetanotherpicsearch-1.9.2/YetAnotherPicSearch/ascii2d.py`

 * *Files identical despite different names*

### Comparing `yetanotherpicsearch-1.9.1/YetAnotherPicSearch/baidu.py` & `yetanotherpicsearch-1.9.2/YetAnotherPicSearch/baidu.py`

 * *Files identical despite different names*

### Comparing `yetanotherpicsearch-1.9.1/YetAnotherPicSearch/config.py` & `yetanotherpicsearch-1.9.2/YetAnotherPicSearch/config.py`

 * *Files identical despite different names*

### Comparing `yetanotherpicsearch-1.9.1/YetAnotherPicSearch/ehentai.py` & `yetanotherpicsearch-1.9.2/YetAnotherPicSearch/ehentai.py`

 * *Files identical despite different names*

### Comparing `yetanotherpicsearch-1.9.1/YetAnotherPicSearch/google.py` & `yetanotherpicsearch-1.9.2/YetAnotherPicSearch/google.py`

 * *Files identical despite different names*

### Comparing `yetanotherpicsearch-1.9.1/YetAnotherPicSearch/iqdb.py` & `yetanotherpicsearch-1.9.2/YetAnotherPicSearch/iqdb.py`

 * *Files identical despite different names*

### Comparing `yetanotherpicsearch-1.9.1/YetAnotherPicSearch/nhentai.py` & `yetanotherpicsearch-1.9.2/YetAnotherPicSearch/nhentai.py`

 * *Files identical despite different names*

### Comparing `yetanotherpicsearch-1.9.1/YetAnotherPicSearch/nhentai_model.py` & `yetanotherpicsearch-1.9.2/YetAnotherPicSearch/nhentai_model.py`

 * *Files identical despite different names*

### Comparing `yetanotherpicsearch-1.9.1/YetAnotherPicSearch/saucenao.py` & `yetanotherpicsearch-1.9.2/YetAnotherPicSearch/saucenao.py`

 * *Files identical despite different names*

### Comparing `yetanotherpicsearch-1.9.1/YetAnotherPicSearch/utils.py` & `yetanotherpicsearch-1.9.2/YetAnotherPicSearch/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,18 +121,20 @@
     if uid_match := uid_search.search(url):
         return confuse_url(f"https://pixiv.net/u/{uid_match[1]}")
 
     if URL(url).host == "danbooru.donmai.us":
         return confuse_url(url.replace("/post/show/", "/posts/"))
 
     if URL(url).host in [
-        "exhentai.org",
         "e-hentai.org",
-        "nhentai.net",
+        "exhentai.org",
         "graph.baidu.com",
+        "nhentai.net",
+        "www.google.com",
+        "yandex.com",
     ]:
         flag = len(url) > 1024
         async with AsyncClient(headers=DEFAULT_HEADERS) as session:
             if not flag:
                 resp = await session.post("https://yww.uy/shorten", json={"url": url})
                 if resp.status_code < 400:
                     return resp.json()["url"]  # type: ignore
@@ -185,21 +187,21 @@
         return wrapper
 
     return decorator
 
 
 def preprocess_search_query(query: str) -> str:
     query = re.sub(r"●|・|~|～|〜|、|×|:::|\s+-\s+|\[中国翻訳]", " ", query)
-    # 去除独立的英文、日文、中文字符
+    # 去除独立的英文、日文、中文字符，但不去除带连字符的
     for i in [
         r"\b[A-Za-z]\b",
         r"\b[\u4e00-\u9fff]\b",
         r"\b[\u3040-\u309f\u30a0-\u30ff]\b",
     ]:
-        query = re.sub(i, "", query)
+        query = re.sub(rf"(?<!-){i}(?!-)", "", query)
 
     return query.strip()
 
 
 def filter_results_with_ratio(
     res: Union[EHentaiResponse, NHentaiResponse], title: str
 ) -> Union[List[EHentaiItem], List[NHentaiItem]]:
```

### Comparing `yetanotherpicsearch-1.9.1/YetAnotherPicSearch/whatanime.py` & `yetanotherpicsearch-1.9.2/YetAnotherPicSearch/whatanime.py`

 * *Files identical despite different names*

### Comparing `yetanotherpicsearch-1.9.1/YetAnotherPicSearch/yandex.py` & `yetanotherpicsearch-1.9.2/YetAnotherPicSearch/yandex.py`

 * *Files identical despite different names*

### Comparing `yetanotherpicsearch-1.9.1/pyproject.toml` & `yetanotherpicsearch-1.9.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "YetAnotherPicSearch"
-version = "1.9.1"
+version = "1.9.2"
 description = "Yet Another Picture Search Nonebot Plugin"
 authors = ["NekoAria"]
 license = "GPL-3.0-only"
 readme = "README.md"
 packages = [
     { include = "YetAnotherPicSearch" },
 ]
```

### Comparing `yetanotherpicsearch-1.9.1/PKG-INFO` & `yetanotherpicsearch-1.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetanotherpicsearch
-Version: 1.9.1
+Version: 1.9.2
 Summary: Yet Another Picture Search Nonebot Plugin
 Home-page: https://github.com/NekoAria/YetAnotherPicSearch
 License: GPL-3.0-only
 Keywords: nonebot,ascii2d,baidu,e-hentai,google,iqdb,saucenao,tracemoe,yandex,anime,danbooru,doujin,pixiv
 Author: NekoAria
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

