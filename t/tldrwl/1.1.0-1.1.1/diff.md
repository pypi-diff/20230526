# Comparing `tmp/tldrwl-1.1.0.tar.gz` & `tmp/tldrwl-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tldrwl-1.1.0.tar", last modified: Fri May 26 08:56:00 2023, max compression
+gzip compressed data, was "tldrwl-1.1.1.tar", last modified: Fri May 26 18:49:13 2023, max compression
```

## Comparing `tldrwl-1.1.0.tar` & `tldrwl-1.1.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:56:00.909322 tldrwl-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-26 08:55:47.000000 tldrwl-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16703 2023-05-26 08:56:00.909322 tldrwl-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16450 2023-05-26 08:55:47.000000 tldrwl-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-26 08:55:47.000000 tldrwl-1.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 08:56:00.909322 tldrwl-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-26 08:55:47.000000 tldrwl-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:56:00.901322 tldrwl-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:55:47.000000 tldrwl-1.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:56:00.901322 tldrwl-1.1.0/tests/manual/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:55:47.000000 tldrwl-1.1.0/tests/manual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-26 08:55:47.000000 tldrwl-1.1.0/tests/manual/inject_urls_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-26 08:55:47.000000 tldrwl-1.1.0/tests/manual/super_short_text_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-26 08:55:47.000000 tldrwl-1.1.0/tests/manual/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-05-26 08:55:47.000000 tldrwl-1.1.0/tests/manual/text_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-26 08:55:47.000000 tldrwl-1.1.0/tests/manual/webpage_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-26 08:55:47.000000 tldrwl-1.1.0/tests/manual/youtube_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:56:00.905322 tldrwl-1.1.0/tldrwl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:55:47.000000 tldrwl-1.1.0/tldrwl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-26 08:55:47.000000 tldrwl-1.1.0/tldrwl/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-05-26 08:55:47.000000 tldrwl-1.1.0/tldrwl/ai_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-26 08:55:47.000000 tldrwl-1.1.0/tldrwl/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-26 08:55:47.000000 tldrwl-1.1.0/tldrwl/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-26 08:55:47.000000 tldrwl-1.1.0/tldrwl/register.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-26 08:55:47.000000 tldrwl-1.1.0/tldrwl/summarize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:56:00.909322 tldrwl-1.1.0/tldrwl/summarizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:55:47.000000 tldrwl-1.1.0/tldrwl/summarizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-26 08:55:47.000000 tldrwl-1.1.0/tldrwl/summarizers/gpt_35_turbo_text_summarizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-26 08:55:47.000000 tldrwl-1.1.0/tldrwl/summarizers/text_ada_001_text_summarizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-05-26 08:55:47.000000 tldrwl-1.1.0/tldrwl/summarizers/text_summarizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:56:00.909322 tldrwl-1.1.0/tldrwl/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:55:47.000000 tldrwl-1.1.0/tldrwl/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-26 08:55:47.000000 tldrwl-1.1.0/tldrwl/transformers/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-05-26 08:55:47.000000 tldrwl-1.1.0/tldrwl/transformers/webpage_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-26 08:55:47.000000 tldrwl-1.1.0/tldrwl/transformers/youtube_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:56:00.905322 tldrwl-1.1.0/tldrwl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16703 2023-05-26 08:56:00.000000 tldrwl-1.1.0/tldrwl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-26 08:56:00.000000 tldrwl-1.1.0/tldrwl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 08:56:00.000000 tldrwl-1.1.0/tldrwl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-26 08:56:00.000000 tldrwl-1.1.0/tldrwl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-26 08:56:00.000000 tldrwl-1.1.0/tldrwl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:49:13.951544 tldrwl-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-26 18:48:58.000000 tldrwl-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16704 2023-05-26 18:49:13.951544 tldrwl-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16451 2023-05-26 18:48:58.000000 tldrwl-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-26 18:48:58.000000 tldrwl-1.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 18:49:13.951544 tldrwl-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-26 18:48:58.000000 tldrwl-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:49:13.947544 tldrwl-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:48:58.000000 tldrwl-1.1.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:49:13.947544 tldrwl-1.1.1/tests/manual/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:48:58.000000 tldrwl-1.1.1/tests/manual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-26 18:48:58.000000 tldrwl-1.1.1/tests/manual/inject_urls_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-26 18:48:58.000000 tldrwl-1.1.1/tests/manual/super_short_text_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-26 18:48:58.000000 tldrwl-1.1.1/tests/manual/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-05-26 18:48:58.000000 tldrwl-1.1.1/tests/manual/text_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-26 18:48:58.000000 tldrwl-1.1.1/tests/manual/webpage_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-26 18:48:58.000000 tldrwl-1.1.1/tests/manual/youtube_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:49:13.947544 tldrwl-1.1.1/tldrwl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:48:58.000000 tldrwl-1.1.1/tldrwl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-26 18:48:58.000000 tldrwl-1.1.1/tldrwl/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-05-26 18:48:58.000000 tldrwl-1.1.1/tldrwl/ai_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-26 18:48:58.000000 tldrwl-1.1.1/tldrwl/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-26 18:48:58.000000 tldrwl-1.1.1/tldrwl/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-26 18:48:58.000000 tldrwl-1.1.1/tldrwl/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-26 18:48:58.000000 tldrwl-1.1.1/tldrwl/summarize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:49:13.951544 tldrwl-1.1.1/tldrwl/summarizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:48:58.000000 tldrwl-1.1.1/tldrwl/summarizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-26 18:48:58.000000 tldrwl-1.1.1/tldrwl/summarizers/gpt_35_turbo_text_summarizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-26 18:48:58.000000 tldrwl-1.1.1/tldrwl/summarizers/text_ada_001_text_summarizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-05-26 18:48:58.000000 tldrwl-1.1.1/tldrwl/summarizers/text_summarizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:49:13.951544 tldrwl-1.1.1/tldrwl/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:48:58.000000 tldrwl-1.1.1/tldrwl/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-26 18:48:58.000000 tldrwl-1.1.1/tldrwl/transformers/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-05-26 18:48:58.000000 tldrwl-1.1.1/tldrwl/transformers/webpage_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-26 18:48:58.000000 tldrwl-1.1.1/tldrwl/transformers/youtube_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:49:13.951544 tldrwl-1.1.1/tldrwl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16704 2023-05-26 18:49:13.000000 tldrwl-1.1.1/tldrwl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-26 18:49:13.000000 tldrwl-1.1.1/tldrwl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:49:13.000000 tldrwl-1.1.1/tldrwl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-26 18:49:13.000000 tldrwl-1.1.1/tldrwl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-26 18:49:13.000000 tldrwl-1.1.1/tldrwl.egg-info/top_level.txt
```

### Comparing `tldrwl-1.1.0/PKG-INFO` & `tldrwl-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: tldrwl
-Version: 1.1.0
+Version: 1.1.1
 Summary: Too long, didn't read/watch/listen
 Home-page: https://github.com/jrodal98/tldrwl
 Author: Jacob Rodal
 Author-email: dev@jrodal.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
-[![PyPI version](https://badge.fury.io/py/tldrwl.svg)](https://badge.fury.io/py/tldrwl)
+[![PyPI](https://img.shields.io/pypi/v/tldrwl.svg)](https://pypi.python.org/pypi/tldrwl)
 
 # tldrwl (too long, didn't read/watch/listen)
 
 ## Install
 
 ```
 pip install tldrwl
```

### Comparing `tldrwl-1.1.0/README.md` & `tldrwl-1.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![PyPI version](https://badge.fury.io/py/tldrwl.svg)](https://badge.fury.io/py/tldrwl)
+[![PyPI](https://img.shields.io/pypi/v/tldrwl.svg)](https://pypi.python.org/pypi/tldrwl)
 
 # tldrwl (too long, didn't read/watch/listen)
 
 ## Install
 
 ```
 pip install tldrwl
```

### Comparing `tldrwl-1.1.0/setup.py` & `tldrwl-1.1.1/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 with open("requirements.txt") as f:
     install_requires = f.read().splitlines()
 
 setuptools.setup(
     name="tldrwl",
-    version="1.1.0",
+    version="1.1.1",
     author="Jacob Rodal",
     author_email="dev@jrodal.com",
     description="Too long, didn't read/watch/listen",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jrodal98/tldrwl",
     packages=setuptools.find_packages(),
```

### Comparing `tldrwl-1.1.0/tests/manual/test_helper.py` & `tldrwl-1.1.1/tests/manual/test_helper.py`

 * *Files identical despite different names*

### Comparing `tldrwl-1.1.0/tests/manual/text_test.py` & `tldrwl-1.1.1/tests/manual/text_test.py`

 * *Files identical despite different names*

### Comparing `tldrwl-1.1.0/tldrwl/__main__.py` & `tldrwl-1.1.1/tldrwl/__main__.py`

 * *Files identical despite different names*

### Comparing `tldrwl-1.1.0/tldrwl/ai_interface.py` & `tldrwl-1.1.1/tldrwl/ai_interface.py`

 * *Files identical despite different names*

### Comparing `tldrwl-1.1.0/tldrwl/exception.py` & `tldrwl-1.1.1/tldrwl/exception.py`

 * *Files identical despite different names*

### Comparing `tldrwl-1.1.0/tldrwl/logger.py` & `tldrwl-1.1.1/tldrwl/logger.py`

 * *Files identical despite different names*

### Comparing `tldrwl-1.1.0/tldrwl/register.py` & `tldrwl-1.1.1/tldrwl/register.py`

 * *Files identical despite different names*

### Comparing `tldrwl-1.1.0/tldrwl/summarize.py` & `tldrwl-1.1.1/tldrwl/summarize.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 class Summarizer(AiInterface):
     def __init__(self, *, text_summarizer: Optional[TextSummarizer] = None) -> None:
         super().__init__()
         self._logger = logging.getLogger(__name__)
         self._summarizer = text_summarizer or Gpt35TurboTextSummarizer()
 
     async def _transform_text(self, text: str) -> str:
-        if YoutubeTransformer.get_video_id(text):
+        if YoutubeTransformer.is_youtube_url(text):
             self._logger.debug(f"Using YoutubeSummarizer on {text}")
             return await YoutubeTransformer(text).get_text()
         elif WebpageTransformer.is_url(text):
             self._logger.debug(f"Using WebpageSummarizer on {text}")
             return await WebpageTransformer(text).get_text()
         elif len(text) < 500:
             self._logger.debug("Text is short... searching for urls")
```

### Comparing `tldrwl-1.1.0/tldrwl/summarizers/gpt_35_turbo_text_summarizer.py` & `tldrwl-1.1.1/tldrwl/summarizers/gpt_35_turbo_text_summarizer.py`

 * *Files identical despite different names*

### Comparing `tldrwl-1.1.0/tldrwl/summarizers/text_ada_001_text_summarizer.py` & `tldrwl-1.1.1/tldrwl/summarizers/text_ada_001_text_summarizer.py`

 * *Files identical despite different names*

### Comparing `tldrwl-1.1.0/tldrwl/summarizers/text_summarizer.py` & `tldrwl-1.1.1/tldrwl/summarizers/text_summarizer.py`

 * *Files identical despite different names*

### Comparing `tldrwl-1.1.0/tldrwl/transformers/webpage_transformer.py` & `tldrwl-1.1.1/tldrwl/transformers/webpage_transformer.py`

 * *Files identical despite different names*

### Comparing `tldrwl-1.1.0/tldrwl/transformers/youtube_transformer.py` & `tldrwl-1.1.1/tldrwl/transformers/youtube_transformer.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,27 +7,32 @@
 
 from youtube_transcript_api import YouTubeTranscriptApi  # pyright: ignore
 from youtube_transcript_api.formatters import TextFormatter  # pyright: ignore
 
 from tldrwl.transformers.transformer import Transformer
 
 from tldrwl.exception import TldrwlVideoUrlParsingException
+from tldrwl.transformers.webpage_transformer import WebpageTransformer
 
 
 class YoutubeTransformer(Transformer):
     _pattern: Pattern[str] = re.compile(
         r"(?:[?&]v=|\/embed\/|\/1\/|\/v\/|https:\/\/(?:www\.)?youtu\.be\/)([^&\n?#]+)"
     )
 
     def __init__(self, url: str) -> None:
         super().__init__()
         self._url = url
         self._logger = logging.getLogger(__name__)
 
     @classmethod
+    def is_youtube_url(cls, url: str) -> bool:
+        return WebpageTransformer.is_url(url) and cls.get_video_id(url) is not None
+
+    @classmethod
     def get_video_id(cls, url: str) -> Optional[str]:
         match = cls._pattern.search(url)
         if match:
             return match.group(1)
         return None
 
     async def get_text(self) -> str:
```

### Comparing `tldrwl-1.1.0/tldrwl.egg-info/PKG-INFO` & `tldrwl-1.1.1/tldrwl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: tldrwl
-Version: 1.1.0
+Version: 1.1.1
 Summary: Too long, didn't read/watch/listen
 Home-page: https://github.com/jrodal98/tldrwl
 Author: Jacob Rodal
 Author-email: dev@jrodal.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
-[![PyPI version](https://badge.fury.io/py/tldrwl.svg)](https://badge.fury.io/py/tldrwl)
+[![PyPI](https://img.shields.io/pypi/v/tldrwl.svg)](https://pypi.python.org/pypi/tldrwl)
 
 # tldrwl (too long, didn't read/watch/listen)
 
 ## Install
 
 ```
 pip install tldrwl
```

### Comparing `tldrwl-1.1.0/tldrwl.egg-info/SOURCES.txt` & `tldrwl-1.1.1/tldrwl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

