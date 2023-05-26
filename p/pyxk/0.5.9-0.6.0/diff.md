# Comparing `tmp/pyxk-0.5.9.tar.gz` & `tmp/pyxk-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxk-0.5.9.tar", last modified: Thu May 25 09:12:20 2023, max compression
+gzip compressed data, was "pyxk-0.6.0.tar", last modified: Fri May 26 01:13:28 2023, max compression
```

## Comparing `pyxk-0.5.9.tar` & `pyxk-0.6.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-25 09:12:20.693999 pyxk-0.5.9/
--rw-rw----   0 root         (0) everybody  (9997)     1079 2022-09-01 11:31:05.000000 pyxk-0.5.9/LICENSE
--rw-rw----   0 root         (0) everybody  (9997)      345 2023-05-25 09:12:20.693999 pyxk-0.5.9/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)        4 2023-03-31 15:33:16.000000 pyxk-0.5.9/README.md
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-25 09:12:20.673999 pyxk-0.5.9/pyxk/
--rw-rw----   0 root         (0) everybody  (9997)      491 2023-05-23 04:42:38.000000 pyxk-0.5.9/pyxk/__init__.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-25 09:12:20.683999 pyxk-0.5.9/pyxk/aclient/
--rw-rw----   0 root         (0) everybody  (9997)       49 2023-05-23 04:42:38.000000 pyxk-0.5.9/pyxk/aclient/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)    19056 2023-05-25 04:45:25.000000 pyxk-0.5.9/pyxk/aclient/client.py
--rw-rw----   0 root         (0) everybody  (9997)      615 2023-05-23 04:42:38.000000 pyxk-0.5.9/pyxk/aclient/typedef.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-25 09:12:20.683999 pyxk-0.5.9/pyxk/aes/
--rw-rw----   0 root         (0) everybody  (9997)       79 2023-05-23 04:42:38.000000 pyxk-0.5.9/pyxk/aes/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     3633 2023-05-23 04:42:38.000000 pyxk-0.5.9/pyxk/aes/_fmtdata.py
--rw-rw----   0 root         (0) everybody  (9997)     4695 2023-05-23 04:42:38.000000 pyxk-0.5.9/pyxk/aes/cryptor.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-25 09:12:20.683999 pyxk-0.5.9/pyxk/m3u8downloader/
--rw-rw----   0 root         (0) everybody  (9997)       66 2023-05-23 04:42:38.000000 pyxk-0.5.9/pyxk/m3u8downloader/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     3391 2023-05-23 04:42:38.000000 pyxk-0.5.9/pyxk/m3u8downloader/enter_point.py
--rw-rw----   0 root         (0) everybody  (9997)     4907 2023-05-23 04:42:38.000000 pyxk-0.5.9/pyxk/m3u8downloader/m3u8download.py
--rw-rw----   0 root         (0) everybody  (9997)     2968 2023-05-23 04:42:38.000000 pyxk-0.5.9/pyxk/m3u8downloader/m3u8parse.py
--rw-rw----   0 root         (0) everybody  (9997)    11879 2023-05-23 04:42:38.000000 pyxk-0.5.9/pyxk/m3u8downloader/main.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-25 09:12:20.693999 pyxk-0.5.9/pyxk/requests/
--rw-rw----   0 root         (0) everybody  (9997)      247 2023-05-23 04:42:38.000000 pyxk-0.5.9/pyxk/requests/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     7480 2023-05-23 04:42:38.000000 pyxk-0.5.9/pyxk/requests/api.py
--rw-rw----   0 root         (0) everybody  (9997)     3502 2023-05-23 04:42:38.000000 pyxk-0.5.9/pyxk/requests/entry_point.py
--rw-rw----   0 root         (0) everybody  (9997)    15235 2023-05-24 06:43:11.000000 pyxk-0.5.9/pyxk/requests/sessions.py
--rw-rw----   0 root         (0) everybody  (9997)    19033 2023-05-23 04:42:38.000000 pyxk-0.5.9/pyxk/utils.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-25 09:12:20.673999 pyxk-0.5.9/pyxk.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)      345 2023-05-25 09:12:20.000000 pyxk-0.5.9/pyxk.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      627 2023-05-25 09:12:20.000000 pyxk-0.5.9/pyxk.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-05-25 09:12:20.000000 pyxk-0.5.9/pyxk.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       99 2023-05-25 09:12:20.000000 pyxk-0.5.9/pyxk.egg-info/entry_points.txt
--rw-rw----   0 root         (0) everybody  (9997)       55 2023-05-25 09:12:20.000000 pyxk-0.5.9/pyxk.egg-info/requires.txt
--rw-rw----   0 root         (0) everybody  (9997)        5 2023-05-25 09:12:20.000000 pyxk-0.5.9/pyxk.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-05-25 09:12:20.693999 pyxk-0.5.9/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)      927 2023-05-25 09:11:55.000000 pyxk-0.5.9/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-26 01:13:28.854000 pyxk-0.6.0/
+-rw-rw----   0 root         (0) everybody  (9997)     1079 2022-09-01 11:31:05.000000 pyxk-0.6.0/LICENSE
+-rw-rw----   0 root         (0) everybody  (9997)      345 2023-05-26 01:13:28.854000 pyxk-0.6.0/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)        4 2023-03-31 15:33:16.000000 pyxk-0.6.0/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-26 01:13:28.844000 pyxk-0.6.0/pyxk/
+-rw-rw----   0 root         (0) everybody  (9997)      491 2023-05-25 11:04:02.000000 pyxk-0.6.0/pyxk/__init__.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-26 01:13:28.844000 pyxk-0.6.0/pyxk/aclient/
+-rw-rw----   0 root         (0) everybody  (9997)       49 2023-05-25 11:04:02.000000 pyxk-0.6.0/pyxk/aclient/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)    19094 2023-05-26 01:02:43.000000 pyxk-0.6.0/pyxk/aclient/client.py
+-rw-rw----   0 root         (0) everybody  (9997)      615 2023-05-25 11:04:02.000000 pyxk-0.6.0/pyxk/aclient/typedef.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-26 01:13:28.844000 pyxk-0.6.0/pyxk/aes/
+-rw-rw----   0 root         (0) everybody  (9997)       55 2023-05-26 01:05:16.000000 pyxk-0.6.0/pyxk/aes/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     3633 2023-05-25 11:04:02.000000 pyxk-0.6.0/pyxk/aes/_fmtdata.py
+-rw-rw----   0 root         (0) everybody  (9997)     4695 2023-05-25 11:04:02.000000 pyxk-0.6.0/pyxk/aes/cryptor.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-26 01:13:28.844000 pyxk-0.6.0/pyxk/m3u8/
+-rw-rw----   0 root         (0) everybody  (9997)       56 2023-05-26 00:55:14.000000 pyxk-0.6.0/pyxk/m3u8/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     3350 2023-05-26 00:55:58.000000 pyxk-0.6.0/pyxk/m3u8/enter_point.py
+-rw-rw----   0 root         (0) everybody  (9997)     4906 2023-05-26 00:45:09.000000 pyxk-0.6.0/pyxk/m3u8/m3u8download.py
+-rw-rw----   0 root         (0) everybody  (9997)     3035 2023-05-26 00:53:56.000000 pyxk-0.6.0/pyxk/m3u8/m3u8parse.py
+-rw-rw----   0 root         (0) everybody  (9997)    11859 2023-05-26 00:48:52.000000 pyxk-0.6.0/pyxk/m3u8/main.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-26 01:13:28.854000 pyxk-0.6.0/pyxk/requests/
+-rw-rw----   0 root         (0) everybody  (9997)      247 2023-05-25 11:04:02.000000 pyxk-0.6.0/pyxk/requests/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     7480 2023-05-25 11:04:02.000000 pyxk-0.6.0/pyxk/requests/api.py
+-rw-rw----   0 root         (0) everybody  (9997)     3502 2023-05-25 11:04:02.000000 pyxk-0.6.0/pyxk/requests/entry_point.py
+-rw-rw----   0 root         (0) everybody  (9997)    15235 2023-05-25 11:04:02.000000 pyxk-0.6.0/pyxk/requests/sessions.py
+-rw-rw----   0 root         (0) everybody  (9997)    19033 2023-05-25 11:04:02.000000 pyxk-0.6.0/pyxk/utils.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-26 01:13:28.844000 pyxk-0.6.0/pyxk.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)      345 2023-05-26 01:13:28.000000 pyxk-0.6.0/pyxk.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      577 2023-05-26 01:13:28.000000 pyxk-0.6.0/pyxk.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-05-26 01:13:28.000000 pyxk-0.6.0/pyxk.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       89 2023-05-26 01:13:28.000000 pyxk-0.6.0/pyxk.egg-info/entry_points.txt
+-rw-rw----   0 root         (0) everybody  (9997)       55 2023-05-26 01:13:28.000000 pyxk-0.6.0/pyxk.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)        5 2023-05-26 01:13:28.000000 pyxk-0.6.0/pyxk.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-05-26 01:13:28.854000 pyxk-0.6.0/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)      917 2023-05-26 00:58:31.000000 pyxk-0.6.0/setup.py
```

### Comparing `pyxk-0.5.9/LICENSE` & `pyxk-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.9/pyxk/aclient/client.py` & `pyxk-0.6.0/pyxk/aclient/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,40 +9,39 @@
     Mapping,
     Pattern
 )
 from types import MethodType
 from itertools import zip_longest
 from multidict import CIMultiDict
 
-import aiohttp
-
+from pyxk.utils import (
+    chardet,
+    LazyLoader,
+    get_user_agent,
+    default_headers,
+)
 from pyxk.aclient.typedef import (
     StrOrURL,
     Session,
     Response,
     EventLoop,
     CIMDict,
     Timeout,
     RequestCallback
 )
-from pyxk.utils import (
-    chardet,
-    LazyLoader,
-    get_user_agent,
-    default_headers,
-)
+
 _copy = LazyLoader("_copy", globals(), "copy")
 _yarl = LazyLoader("_yarl", globals(), "yarl")
+aiohttp = LazyLoader("aiohttp", globals(), "aiohttp")
 _selector = LazyLoader("_selector", globals(), "parsel.selector")
 aiohttp_client_exceptions = LazyLoader("aiohttp_client_exceptions", globals(), "aiohttp.client_exceptions")
 
 __all__ = ["Client"]
 
 
-
 class Client:
     """异步下载器 - 类变量
 
     :params: limit: aiohttp 并发控制
     :params: timeout: 请求超时时间
     :params: req_kwargs: start_request请求参数
     :params: async_sleep: 异步休眠时间
```

### Comparing `pyxk-0.5.9/pyxk/aclient/typedef.py` & `pyxk-0.6.0/pyxk/aclient/typedef.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.9/pyxk/aes/_fmtdata.py` & `pyxk-0.6.0/pyxk/aes/_fmtdata.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.9/pyxk/aes/cryptor.py` & `pyxk-0.6.0/pyxk/aes/cryptor.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.9/pyxk/m3u8downloader/enter_point.py` & `pyxk-0.6.0/pyxk/m3u8/enter_point.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import click
-from pyxk import LazyLoader, get_user_agent
+from pyxk.utils import LazyLoader, get_user_agent
 
-m3u8downloader = LazyLoader("m3u8downloader", globals(), "pyxk.m3u8downloader")
+_m3u8= LazyLoader("_m3u8", globals(), "pyxk.m3u8")
 
 
 @click.group(invoke_without_command=False, chain=False)
 @click.option("-o", "--output", "output", type=str, default=None, help="M3U8存储路径")
 @click.option("--reload", is_flag=True, help="重载m3u8资源")
 @click.option("--reserve", is_flag=True, help="保留m3u8资源")
 @click.option("-h", "--headers", "headers", type=(str, str), multiple=True, help="Request Headers")
@@ -29,15 +29,15 @@
 @click.option("--reserve", is_flag=True, help="保留m3u8资源")
 @click.option("-h", "--headers", "headers", type=(str, str), multiple=True, help="Request Headers")
 @click.option("--no-verify", "verify", is_flag=True, default=True, help="Request Verify")
 @click.option("-l", "--limit", "limit", type=int, default=None, help="下载并发量")
 @click.option("-ua", "--user-agent", "user_agent", type=str, default=None, help="User-Agent")
 def file(obj, content, url, output, reload, reserve, headers, verify, limit, user_agent):
     """下载m3u8资源 - m3u8 content"""
-    m3u8downloader.load_content(
+    _m3u8.load_content(
         content=content,
         url=url,
         output=output or obj["output"],
         reload=reload,
         reserve=reserve,
         headers=dict(headers or obj["headers"]),
         verify=verify,
@@ -53,15 +53,15 @@
 @click.option("--reserve", is_flag=True, help="保留m3u8资源")
 @click.option("-h", "--headers", "headers", type=(str, str), multiple=True, help="Request Headers")
 @click.option("--no-verify", "verify", is_flag=True, default=True, help="Request Verify")
 @click.option("-l", "--limit", "limit", type=int, default=None, help="下载并发量")
 @click.option("-ua", "--user-agent", "user_agent", type=str, default=None, help="User-Agent")
 def url(obj, _url, output, reload, reserve, headers, verify, limit, user_agent):
     """下载m3u8资源 - m3u8 url"""
-    m3u8downloader.load_url(
+    _m3u8.load_url(
         url=_url,
         output=output or obj["output"],
         reload=reload,
         reserve=reserve,
         headers=dict(headers or obj["headers"]),
         verify=verify,
         limit=limit or obj["limit"],
```

### Comparing `pyxk-0.5.9/pyxk/m3u8downloader/m3u8download.py` & `pyxk-0.6.0/pyxk/m3u8/m3u8download.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 
     :params: m3u8keys: m3u8资源加密密钥
     :params: segments: m3u8 segments
     :params: progress: rich.progress.Progress
     :params: download: rich.progress.Progress
     """
     timeout = 30
-    maximum_retry = 999
-    error_status_code = list(range(403, 411))
+    maximum_retry = 30
+    error_status_code = list(range(404, 411))
     until_request_succeed = True
 
     def __init__(
         self,
         *,
         m3obj,
         m3u8keys: Optional[dict] = None,
```

### Comparing `pyxk-0.5.9/pyxk/m3u8downloader/m3u8parse.py` & `pyxk-0.6.0/pyxk/m3u8/m3u8parse.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """m3u8资源解析器"""
 from typing import Optional
 
-import m3u8
 from m3u8.model import M3U8
+from pyxk.utils import LazyLoader
 
+m3u8 = LazyLoader("m3u8", globals(), "m3u8")
 
 
 class M3U8Parae:
     """m3u8资源 解析器
 
     :params: *
     :params: content: m3u8 content
```

### Comparing `pyxk-0.5.9/pyxk/m3u8downloader/main.py` & `pyxk-0.6.0/pyxk/m3u8/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     hash256,
     make_open,
     LazyLoader,
     progress_column,
     download_column,
     human_playtime
 )
-from pyxk.m3u8downloader.m3u8parse import M3U8Parae
-from pyxk.m3u8downloader.m3u8download import Downloader
+from pyxk.m3u8.m3u8parse import M3U8Parae
+from pyxk.m3u8.m3u8download import Downloader
 
 _rich_box = LazyLoader("_rich_box", globals(), "rich.box")
 _rich_live = LazyLoader("_rich_live", globals(), "rich.live")
 _rich_table = LazyLoader("_rich_table", globals(), "rich.table")
 _rich_panel = LazyLoader("_rich_panel", globals(), "rich.panel")
 _rich_console = LazyLoader("_rich_console", globals(), "rich.console")
 _requests = LazyLoader("_requests", globals(), "pyxk.requests")
```

### Comparing `pyxk-0.5.9/pyxk/requests/api.py` & `pyxk-0.6.0/pyxk/requests/api.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.9/pyxk/requests/entry_point.py` & `pyxk-0.6.0/pyxk/requests/entry_point.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.9/pyxk/requests/sessions.py` & `pyxk-0.6.0/pyxk/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.9/pyxk/utils.py` & `pyxk-0.6.0/pyxk/utils.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.9/pyxk.egg-info/SOURCES.txt` & `pyxk-0.6.0/pyxk.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 pyxk.egg-info/top_level.txt
 pyxk/aclient/__init__.py
 pyxk/aclient/client.py
 pyxk/aclient/typedef.py
 pyxk/aes/__init__.py
 pyxk/aes/_fmtdata.py
 pyxk/aes/cryptor.py
-pyxk/m3u8downloader/__init__.py
-pyxk/m3u8downloader/enter_point.py
-pyxk/m3u8downloader/m3u8download.py
-pyxk/m3u8downloader/m3u8parse.py
-pyxk/m3u8downloader/main.py
+pyxk/m3u8/__init__.py
+pyxk/m3u8/enter_point.py
+pyxk/m3u8/m3u8download.py
+pyxk/m3u8/m3u8parse.py
+pyxk/m3u8/main.py
 pyxk/requests/__init__.py
 pyxk/requests/api.py
 pyxk/requests/entry_point.py
 pyxk/requests/sessions.py
```

### Comparing `pyxk-0.5.9/setup.py` & `pyxk-0.6.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyxk",
-    version="0.5.9",
+    version="0.6.0",
     author="pengke",
     install_requires=[
         "requests",
         "pycryptodome",
         "rich",
         "m3u8",
         "aiohttp",
         "aiofiles",
         "click",
     ],
     entry_points={
         'console_scripts': [
-            'm3u8 = pyxk.m3u8downloader.enter_point:main',
+            'm3u8 = pyxk.m3u8.enter_point:main',
             'req = pyxk.requests.entry_point:main'
         ],
     },
     author_email="925330867@qq.com",
     description="pyxk",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

