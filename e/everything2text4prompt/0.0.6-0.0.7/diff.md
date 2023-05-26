# Comparing `tmp/everything2text4prompt-0.0.6.tar.gz` & `tmp/everything2text4prompt-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "everything2text4prompt-0.0.6.tar", last modified: Fri May 26 15:45:44 2023, max compression
+gzip compressed data, was "everything2text4prompt-0.0.7.tar", last modified: Fri May 26 16:20:12 2023, max compression
```

## Comparing `everything2text4prompt-0.0.6.tar` & `everything2text4prompt-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 15:45:44.059115 everything2text4prompt-0.0.6/
--rw-rw-rw-   0        0        0     1089 2023-05-18 13:27:55.000000 everything2text4prompt-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     1052 2023-05-26 15:45:44.058129 everything2text4prompt-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      658 2023-05-18 13:34:54.000000 everything2text4prompt-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 15:45:44.040166 everything2text4prompt-0.0.6/everything2text4prompt/
--rw-rw-rw-   0        0        0      125 2023-05-26 15:42:05.000000 everything2text4prompt-0.0.6/everything2text4prompt/__init__.py
--rw-rw-rw-   0        0        0     2372 2023-05-26 15:42:05.000000 everything2text4prompt-0.0.6/everything2text4prompt/everything2text4prompt.py
--rw-rw-rw-   0        0        0      369 2023-05-26 15:42:05.000000 everything2text4prompt-0.0.6/everything2text4prompt/pdf_util.py
-drwxrwxrwx   0        0        0        0 2023-05-26 15:45:44.055154 everything2text4prompt-0.0.6/everything2text4prompt/playground/
--rw-rw-rw-   0        0        0      754 2023-05-19 14:34:30.000000 everything2text4prompt-0.0.6/everything2text4prompt/playground/test_split_mp3.py
--rw-rw-rw-   0        0        0      340 2023-05-19 15:00:50.000000 everything2text4prompt-0.0.6/everything2text4prompt/playground/test_whisper.py
--rw-rw-rw-   0        0        0     1062 2023-05-26 15:42:05.000000 everything2text4prompt-0.0.6/everything2text4prompt/podcast_util.py
--rw-rw-rw-   0        0        0     2075 2023-05-26 15:42:05.000000 everything2text4prompt-0.0.6/everything2text4prompt/util.py
--rw-rw-rw-   0        0        0     2235 2023-05-26 15:42:05.000000 everything2text4prompt-0.0.6/everything2text4prompt/youtube_util.py
-drwxrwxrwx   0        0        0        0 2023-05-26 15:45:44.051166 everything2text4prompt-0.0.6/everything2text4prompt.egg-info/
--rw-rw-rw-   0        0        0     1052 2023-05-26 15:45:43.000000 everything2text4prompt-0.0.6/everything2text4prompt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      585 2023-05-26 15:45:43.000000 everything2text4prompt-0.0.6/everything2text4prompt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 15:45:43.000000 everything2text4prompt-0.0.6/everything2text4prompt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-05-26 15:45:43.000000 everything2text4prompt-0.0.6/everything2text4prompt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-05-26 15:45:43.000000 everything2text4prompt-0.0.6/everything2text4prompt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-26 15:45:44.059115 everything2text4prompt-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      768 2023-05-26 15:44:54.000000 everything2text4prompt-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 16:20:12.595820 everything2text4prompt-0.0.7/
+-rw-rw-rw-   0        0        0     1089 2023-05-18 13:27:55.000000 everything2text4prompt-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     1052 2023-05-26 16:20:12.594822 everything2text4prompt-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      658 2023-05-18 13:34:54.000000 everything2text4prompt-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 16:20:12.560448 everything2text4prompt-0.0.7/everything2text4prompt/
+-rw-rw-rw-   0        0        0      234 2023-05-26 16:18:10.000000 everything2text4prompt-0.0.7/everything2text4prompt/__init__.py
+-rw-rw-rw-   0        0        0     2385 2023-05-26 16:18:53.000000 everything2text4prompt-0.0.7/everything2text4prompt/everything2text4prompt.py
+-rw-rw-rw-   0        0        0      452 2023-05-26 16:14:35.000000 everything2text4prompt-0.0.7/everything2text4prompt/pdf_util.py
+drwxrwxrwx   0        0        0        0 2023-05-26 16:20:12.592826 everything2text4prompt-0.0.7/everything2text4prompt/playground/
+-rw-rw-rw-   0        0        0      754 2023-05-19 14:34:30.000000 everything2text4prompt-0.0.7/everything2text4prompt/playground/test_split_mp3.py
+-rw-rw-rw-   0        0        0      340 2023-05-19 15:00:50.000000 everything2text4prompt-0.0.7/everything2text4prompt/playground/test_whisper.py
+-rw-rw-rw-   0        0        0     1183 2023-05-26 16:14:59.000000 everything2text4prompt-0.0.7/everything2text4prompt/podcast_util.py
+-rw-rw-rw-   0        0        0     2075 2023-05-26 15:42:05.000000 everything2text4prompt-0.0.7/everything2text4prompt/util.py
+-rw-rw-rw-   0        0        0     2444 2023-05-26 16:18:25.000000 everything2text4prompt-0.0.7/everything2text4prompt/youtube_util.py
+drwxrwxrwx   0        0        0        0 2023-05-26 16:20:12.572686 everything2text4prompt-0.0.7/everything2text4prompt.egg-info/
+-rw-rw-rw-   0        0        0     1052 2023-05-26 16:20:12.000000 everything2text4prompt-0.0.7/everything2text4prompt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      585 2023-05-26 16:20:12.000000 everything2text4prompt-0.0.7/everything2text4prompt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 16:20:12.000000 everything2text4prompt-0.0.7/everything2text4prompt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-05-26 16:20:12.000000 everything2text4prompt-0.0.7/everything2text4prompt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-05-26 16:20:12.000000 everything2text4prompt-0.0.7/everything2text4prompt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 16:20:12.595820 everything2text4prompt-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      785 2023-05-26 16:19:25.000000 everything2text4prompt-0.0.7/setup.py
```

### Comparing `everything2text4prompt-0.0.6/LICENSE` & `everything2text4prompt-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `everything2text4prompt-0.0.6/PKG-INFO` & `everything2text4prompt-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: everything2text4prompt
-Version: 0.0.6
+Version: 0.0.7
 Summary: Convert many medium into text, and the text format is specialized for prompt input
 Home-page: https://github.com/michaelthwan/everything2text4prompt
 Author: michaethwan
 Author-email: michaelthwan@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `everything2text4prompt-0.0.6/README.md` & `everything2text4prompt-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `everything2text4prompt-0.0.6/everything2text4prompt/everything2text4prompt.py` & `everything2text4prompt-0.0.7/everything2text4prompt/everything2text4prompt.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import openai
 
-from pdf_util import get_pdf_data
-# from podcast_util import convert_podcast_transcript
-from youtube_util import get_youtube_data
+from .pdf_util import PDFUtil
+# from .podcast_util import convert_podcast_transcript
+from .youtube_util import YoutubeUtil
 
 
 class Everything2Text4Prompt:
     def __init__(self, openai_api_key, is_azure=False):
         self.openai_api_key = openai_api_key
         self.is_azure = is_azure
         openai.api_key = self.openai_api_key
 
     def convert_text(self, medium, target_source) -> (str, bool, str):
         if medium == "youtube":
-            return get_youtube_data(target_source)
+            return YoutubeUtil.get_youtube_data(target_source)
         # elif medium == "podcast":
         #     return convert_podcast_transcript(target_source)
         elif medium == "pdf":
-            return get_pdf_data(target_source)
+            return PDFUtil.get_pdf_data(target_source)
         else:
             raise Exception("Unsupported medium")
 
 
 if __name__ == "__main__":
     openai_api_key = ""
     converter = Everything2Text4Prompt(openai_api_key)
```

### Comparing `everything2text4prompt-0.0.6/everything2text4prompt/playground/test_split_mp3.py` & `everything2text4prompt-0.0.7/everything2text4prompt/playground/test_split_mp3.py`

 * *Files identical despite different names*

### Comparing `everything2text4prompt-0.0.6/everything2text4prompt/podcast_util.py` & `everything2text4prompt-0.0.7/everything2text4prompt/podcast_util.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 import re
 
 import openai
 import requests
 
 from .util import chunk_mp3, PodcastData
 
+class PodcastUtil:
+    @staticmethod
+    def convert_podcast_transcript(podcast_url):
+        def download_mp3(url: str, file_path: str):
+            with open(file_path, "wb") as file:
+                response = requests.get(url)
+                file.write(response.content)
 
-def convert_podcast_transcript(podcast_url):
-    def download_mp3(url: str, file_path: str):
-        with open(file_path, "wb") as file:
-            response = requests.get(url)
-            file.write(response.content)
-
-    content = requests.get(podcast_url)
-    mp3_url = re.findall("(?P<url>\;https?://[^\s]+)", content.text)[0].split(';')[1]
-    print(f"mp3_url: {mp3_url}")
-    mp3_file_path = "temp.mp3"
-    download_mp3(mp3_url, mp3_file_path)
-    print(f"Downloaded mp3 file")
-    file_part_list = chunk_mp3(mp3_file_path)
-    transcript_list = []
-    for file_part in file_part_list:
-        file = open(file_part, "rb")
-        print(f"Calling openai whisper-1 for {file_part}")
-        transcript = openai.Audio.transcribe("whisper-1", file)
-        transcript_list.append(transcript)
-    print(transcript_list)
-    title = description = ""  # TODO
-    return PodcastData(" ".join(transcript_list), title, description), True, "Success"
+        content = requests.get(podcast_url)
+        mp3_url = re.findall("(?P<url>\;https?://[^\s]+)", content.text)[0].split(';')[1]
+        print(f"mp3_url: {mp3_url}")
+        mp3_file_path = "temp.mp3"
+        download_mp3(mp3_url, mp3_file_path)
+        print(f"Downloaded mp3 file")
+        file_part_list = chunk_mp3(mp3_file_path)
+        transcript_list = []
+        for file_part in file_part_list:
+            file = open(file_part, "rb")
+            print(f"Calling openai whisper-1 for {file_part}")
+            transcript = openai.Audio.transcribe("whisper-1", file)
+            transcript_list.append(transcript)
+        print(transcript_list)
+        title = description = ""  # TODO
+        return PodcastData(" ".join(transcript_list), title, description), True, "Success"
```

### Comparing `everything2text4prompt-0.0.6/everything2text4prompt/util.py` & `everything2text4prompt-0.0.7/everything2text4prompt/util.py`

 * *Files identical despite different names*

### Comparing `everything2text4prompt-0.0.6/everything2text4prompt/youtube_util.py` & `everything2text4prompt-0.0.7/everything2text4prompt/youtube_util.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,65 +1,67 @@
 import requests
 from bs4 import BeautifulSoup
 from youtube_transcript_api import YouTubeTranscriptApi
 
-from util import YoutubeData
+from .util import YoutubeData
 
 
-def get_youtube_data(target_source: str) -> (str, bool, str):
-    transcript = title = description = None
-    try:
-        title, description = get_video_info(target_source)
-        transcript = convert_youtube_transcript(target_source)
-    except Exception as e:
-        return YoutubeData(transcript, title, description), False, str(e)
-    return YoutubeData(transcript, title, description), True, ""
+class YoutubeUtil:
+    @staticmethod
+    def get_youtube_data(target_source: str) -> (str, bool, str):
+        transcript = title = description = None
+        try:
+            title, description = YoutubeUtil.get_video_info(target_source)
+            transcript = YoutubeUtil.convert_youtube_transcript(target_source)
+        except Exception as e:
+            return YoutubeData(transcript, title, description), False, str(e)
+        return YoutubeData(transcript, title, description), True, ""
+
+    @staticmethod
+    def get_video_info(target_source):
+        url = f"https://www.youtube.com/watch?v={target_source}"
+        response = requests.get(url)
+
+        if response.status_code != 200:
+            return None
+
+        soup = BeautifulSoup(response.content, "html.parser")
+
+        title = soup.find("meta", itemprop="name")["content"]
+        description = soup.find("meta", itemprop="description")["content"]
+
+        return title, description
+
+    @staticmethod
+    def convert_youtube_transcript(target_source) -> str:
+        def extract_video_id_from_url(url):
+            return url.split("v=")[1]
+
+        def is_url(url):
+            return "youtube.com" in url
+
+        if is_url(target_source):
+            video_id = extract_video_id_from_url(target_source)
+        else:
+            video_id = target_source
+
+        preferred_lang = ['en', 'zh', 'zh-Hans', 'zh-Hant', 'ja', 'it', 'de', 'fr']
+        try:
+            transcript = YouTubeTranscriptApi.get_transcript(video_id, preferred_lang)
+        except Exception as e:
+            import youtube_transcript_api
+            if isinstance(e, youtube_transcript_api._errors.TranscriptsDisabled):
+                raise Exception(e)
+            transcript_list = YouTubeTranscriptApi.list_transcripts(video_id)
+            transcript = transcript_list.find_generated_transcript(preferred_lang)
+        text = " ".join([entry['text'] for entry in transcript])
 
-
-def get_video_info(target_source):
-    url = f"https://www.youtube.com/watch?v={target_source}"
-    response = requests.get(url)
-
-    if response.status_code != 200:
-        return None
-
-    soup = BeautifulSoup(response.content, "html.parser")
-
-    title = soup.find("meta", itemprop="name")["content"]
-    description = soup.find("meta", itemprop="description")["content"]
-
-    return title, description
-
-
-def convert_youtube_transcript(target_source) -> YoutubeData:
-    def extract_video_id_from_url(url):
-        return url.split("v=")[1]
-
-    def is_url(url):
-        return "youtube.com" in url
-
-    if is_url(target_source):
-        video_id = extract_video_id_from_url(target_source)
-    else:
-        video_id = target_source
-
-    preferred_lang = ['en', 'zh', 'zh-Hans', 'zh-Hant', 'ja', 'it', 'de', 'fr']
-    try:
-        transcript = YouTubeTranscriptApi.get_transcript(video_id, preferred_lang)
-    except Exception as e:
-        import youtube_transcript_api
-        if isinstance(e, youtube_transcript_api._errors.TranscriptsDisabled):
-            return "", False, "Transcripts are disabled for this video"
-        transcript_list = YouTubeTranscriptApi.list_transcripts(video_id)
-        transcript = transcript_list.find_generated_transcript(preferred_lang)
-    text = " ".join([entry['text'] for entry in transcript])
-
-    return text
+        return text
 
 
 if __name__ == '__main__':
     target_source = 'lSTEhG021Jc'
-    youtube_data, is_success, error_msg = get_youtube_data(target_source)
+    youtube_data, is_success, error_msg = YoutubeUtil.get_youtube_data(target_source)
     youtube_data: YoutubeData
     print(youtube_data.title)
     print(youtube_data.description)
     print(youtube_data.shorten_transcript)
```

### Comparing `everything2text4prompt-0.0.6/everything2text4prompt.egg-info/PKG-INFO` & `everything2text4prompt-0.0.7/everything2text4prompt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: everything2text4prompt
-Version: 0.0.6
+Version: 0.0.7
 Summary: Convert many medium into text, and the text format is specialized for prompt input
 Home-page: https://github.com/michaelthwan/everything2text4prompt
 Author: michaethwan
 Author-email: michaelthwan@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `everything2text4prompt-0.0.6/everything2text4prompt.egg-info/SOURCES.txt` & `everything2text4prompt-0.0.7/everything2text4prompt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `everything2text4prompt-0.0.6/setup.py` & `everything2text4prompt-0.0.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="everything2text4prompt",
-    version="0.0.6",
+    version="0.0.7",
     description="Convert many medium into text, and the text format is specialized for prompt input",
     # package_dir={'': 'everything2text4prompt'},
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/michaelthwan/everything2text4prompt",
     author="michaethwan",
     author_email="michaelthwan@gmail.com",
     license="MIT",
     python_requires=">=3.8",
     install_requires=[
         "openai>=0.27.6",
         "youtube-transcript-api>=0.6.0",
-        "pypdf"
+        "bs4",
+        "pypdf",
     ]
 )
```

