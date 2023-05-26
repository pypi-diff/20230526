# Comparing `tmp/aij-1.1.3.tar.gz` & `tmp/aij-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aij-1.1.3.tar", last modified: Thu May 25 23:28:38 2023, max compression
+gzip compressed data, was "aij-1.1.4.tar", last modified: Fri May 26 21:02:21 2023, max compression
```

## Comparing `aij-1.1.3.tar` & `aij-1.1.4.tar`

### file list

```diff
@@ -1,42 +1,56 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 23:28:38.746877 aij-1.1.3/
--rw-rw-rw-   0        0        0     1100 2023-05-21 18:35:40.000000 aij-1.1.3/LICENSE.txt
--rw-rw-rw-   0        0        0    30052 2023-05-25 23:28:38.745463 aij-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0    27745 2023-05-21 18:35:40.000000 aij-1.1.3/README.md
--rw-rw-rw-   0        0        0     6993 2023-05-25 23:28:24.000000 aij-1.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-25 23:28:38.746877 aij-1.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-25 23:28:38.668489 aij-1.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-25 23:28:38.715068 aij-1.1.3/src/aij.egg-info/
--rw-rw-rw-   0        0        0    30052 2023-05-25 23:28:38.000000 aij-1.1.3/src/aij.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      553 2023-05-25 23:28:38.000000 aij-1.1.3/src/aij.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 23:28:38.000000 aij-1.1.3/src/aij.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      247 2023-05-25 23:28:38.000000 aij-1.1.3/src/aij.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      491 2023-05-25 23:28:38.000000 aij-1.1.3/src/aij.egg-info/requires.txt
--rw-rw-rw-   0        0        0      105 2023-05-25 23:28:38.000000 aij-1.1.3/src/aij.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-25 23:28:38.717062 aij-1.1.3/src/animation/
--rw-rw-rw-   0        0        0     5739 2023-05-25 21:36:22.000000 aij-1.1.3/src/animation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 23:28:38.719065 aij-1.1.3/src/chat/
--rw-rw-rw-   0        0        0      680 2023-05-21 20:35:30.000000 aij-1.1.3/src/chat/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 23:28:38.721085 aij-1.1.3/src/download/
--rw-rw-rw-   0        0        0     8301 2023-05-24 21:25:22.000000 aij-1.1.3/src/download/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 23:28:38.723079 aij-1.1.3/src/face/
--rw-rw-rw-   0        0        0     8295 2023-05-25 16:52:45.000000 aij-1.1.3/src/face/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 23:28:38.725080 aij-1.1.3/src/intro/
--rw-rw-rw-   0        0        0     4532 2023-05-24 21:19:40.000000 aij-1.1.3/src/intro/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 23:28:38.727077 aij-1.1.3/src/messaging/
--rw-rw-rw-   0        0        0     5060 2023-05-23 19:12:37.000000 aij-1.1.3/src/messaging/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 23:28:38.729563 aij-1.1.3/src/news/
--rw-rw-rw-   0        0        0    10270 2023-05-25 21:21:31.000000 aij-1.1.3/src/news/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 23:28:38.731817 aij-1.1.3/src/setup/
--rw-rw-rw-   0        0        0     3925 2023-05-24 22:31:30.000000 aij-1.1.3/src/setup/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 23:28:38.733823 aij-1.1.3/src/stream/
--rw-rw-rw-   0        0        0     1093 2023-05-24 23:06:34.000000 aij-1.1.3/src/stream/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 23:28:38.735130 aij-1.1.3/src/transcribe/
--rw-rw-rw-   0        0        0     2215 2023-05-25 21:10:13.000000 aij-1.1.3/src/transcribe/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 23:28:38.736123 aij-1.1.3/src/translate/
--rw-rw-rw-   0        0        0     2393 2023-05-25 21:47:13.000000 aij-1.1.3/src/translate/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 23:28:38.738656 aij-1.1.3/src/voice/
--rw-rw-rw-   0        0        0     2239 2023-05-25 23:23:39.000000 aij-1.1.3/src/voice/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 23:28:38.740654 aij-1.1.3/src/webcam/
--rw-rw-rw-   0        0        0    18706 2023-05-24 23:40:36.000000 aij-1.1.3/src/webcam/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 23:28:38.742659 aij-1.1.3/src/webcam2/
--rw-rw-rw-   0        0        0     3351 2023-05-25 22:17:56.000000 aij-1.1.3/src/webcam2/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 21:02:21.758662 aij-1.1.4/
+-rw-rw-rw-   0        0        0     1100 2023-05-21 18:35:40.000000 aij-1.1.4/LICENSE.txt
+-rw-rw-rw-   0        0        0    30052 2023-05-26 21:02:21.757667 aij-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0    27745 2023-05-21 18:35:40.000000 aij-1.1.4/README.md
+-rw-rw-rw-   0        0        0     7018 2023-05-26 21:02:09.000000 aij-1.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-26 21:02:21.758662 aij-1.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-26 21:02:21.684180 aij-1.1.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-26 21:02:21.719184 aij-1.1.4/src/aij.egg-info/
+-rw-rw-rw-   0        0        0    30052 2023-05-26 21:02:21.000000 aij-1.1.4/src/aij.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      727 2023-05-26 21:02:21.000000 aij-1.1.4/src/aij.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 21:02:21.000000 aij-1.1.4/src/aij.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      247 2023-05-26 21:02:21.000000 aij-1.1.4/src/aij.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      502 2023-05-26 21:02:21.000000 aij-1.1.4/src/aij.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      167 2023-05-26 21:02:21.000000 aij-1.1.4/src/aij.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-26 21:02:21.720183 aij-1.1.4/src/animation/
+-rw-rw-rw-   0        0        0     5739 2023-05-25 21:36:22.000000 aij-1.1.4/src/animation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 21:02:21.722707 aij-1.1.4/src/chat/
+-rw-rw-rw-   0        0        0     3861 2023-05-26 12:12:18.000000 aij-1.1.4/src/chat/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 21:02:21.723707 aij-1.1.4/src/download/
+-rw-rw-rw-   0        0        0     8301 2023-05-24 21:25:22.000000 aij-1.1.4/src/download/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 21:02:21.725706 aij-1.1.4/src/emotion/
+-rw-rw-rw-   0        0        0     2537 2023-05-26 12:58:13.000000 aij-1.1.4/src/emotion/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 21:02:21.727706 aij-1.1.4/src/entity/
+-rw-rw-rw-   0        0        0      651 2023-05-26 12:48:48.000000 aij-1.1.4/src/entity/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 21:02:21.728706 aij-1.1.4/src/face/
+-rw-rw-rw-   0        0        0     7696 2023-05-26 11:57:56.000000 aij-1.1.4/src/face/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 21:02:21.731100 aij-1.1.4/src/fact_check/
+-rw-rw-rw-   0        0        0      765 2023-05-26 12:46:38.000000 aij-1.1.4/src/fact_check/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 21:02:21.732103 aij-1.1.4/src/intro/
+-rw-rw-rw-   0        0        0     4532 2023-05-24 21:19:40.000000 aij-1.1.4/src/intro/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 21:02:21.734099 aij-1.1.4/src/knowledge/
+-rw-rw-rw-   0        0        0      807 2023-05-26 12:39:25.000000 aij-1.1.4/src/knowledge/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 21:02:21.736109 aij-1.1.4/src/language/
+-rw-rw-rw-   0        0        0      507 2023-05-26 12:36:22.000000 aij-1.1.4/src/language/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 21:02:21.737109 aij-1.1.4/src/messaging/
+-rw-rw-rw-   0        0        0     5060 2023-05-23 19:12:37.000000 aij-1.1.4/src/messaging/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 21:02:21.739113 aij-1.1.4/src/news/
+-rw-rw-rw-   0        0        0    10270 2023-05-25 21:21:31.000000 aij-1.1.4/src/news/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 21:02:21.740109 aij-1.1.4/src/scrape/
+-rw-rw-rw-   0        0        0     1823 2023-05-26 12:53:00.000000 aij-1.1.4/src/scrape/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 21:02:21.742114 aij-1.1.4/src/sentiment/
+-rw-rw-rw-   0        0        0      549 2023-05-26 12:50:27.000000 aij-1.1.4/src/sentiment/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 21:02:21.744109 aij-1.1.4/src/setup/
+-rw-rw-rw-   0        0        0     3925 2023-05-24 22:31:30.000000 aij-1.1.4/src/setup/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 21:02:21.745109 aij-1.1.4/src/stream/
+-rw-rw-rw-   0        0        0     1093 2023-05-24 23:06:34.000000 aij-1.1.4/src/stream/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 21:02:21.747111 aij-1.1.4/src/transcribe/
+-rw-rw-rw-   0        0        0     2215 2023-05-25 21:10:13.000000 aij-1.1.4/src/transcribe/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 21:02:21.748110 aij-1.1.4/src/translate/
+-rw-rw-rw-   0        0        0     2393 2023-05-25 21:47:13.000000 aij-1.1.4/src/translate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 21:02:21.751172 aij-1.1.4/src/voice/
+-rw-rw-rw-   0        0        0     2239 2023-05-25 23:23:39.000000 aij-1.1.4/src/voice/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 21:02:21.752653 aij-1.1.4/src/webcam/
+-rw-rw-rw-   0        0        0    18760 2023-05-26 11:58:38.000000 aij-1.1.4/src/webcam/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 21:02:21.754666 aij-1.1.4/src/webcam2/
+-rw-rw-rw-   0        0        0     3351 2023-05-25 22:17:56.000000 aij-1.1.4/src/webcam2/__init__.py
```

### Comparing `aij-1.1.3/LICENSE.txt` & `aij-1.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aij-1.1.3/PKG-INFO` & `aij-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij
-Version: 1.1.3
+Version: 1.1.4
 Summary: AI Journalist
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-1.1.3/README.md` & `aij-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `aij-1.1.3/pyproject.toml` & `aij-1.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "aij"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.1.03"
+version = "1.1.04"
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "AI Journalist"  # Optional
 
 # This is an optional longer description of your project that represents
@@ -138,15 +138,17 @@
     "flask-cors",
     "flask-sqlalchemy",
     "deepface",
     "speechbrain",
     "soundfile",
     "transformers",
     "langchain",
-    "pytube3"
+    "pytube3",
+    "nltk",
+    "spacy"
 ]
 
 # List additional groups of dependencies here (e.g. development
 # dependencies). Users will be able to install these using the "extras"
 # syntax, for example:
 #
 #   $ pip install sampleproject[dev]
```

### Comparing `aij-1.1.3/src/aij.egg-info/PKG-INFO` & `aij-1.1.4/src/aij.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij
-Version: 1.1.3
+Version: 1.1.4
 Summary: AI Journalist
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-1.1.3/src/aij.egg-info/SOURCES.txt` & `aij-1.1.4/src/aij.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -6,18 +6,25 @@
 src/aij.egg-info/dependency_links.txt
 src/aij.egg-info/entry_points.txt
 src/aij.egg-info/requires.txt
 src/aij.egg-info/top_level.txt
 src/animation/__init__.py
 src/chat/__init__.py
 src/download/__init__.py
+src/emotion/__init__.py
+src/entity/__init__.py
 src/face/__init__.py
+src/fact_check/__init__.py
 src/intro/__init__.py
+src/knowledge/__init__.py
+src/language/__init__.py
 src/messaging/__init__.py
 src/news/__init__.py
+src/scrape/__init__.py
+src/sentiment/__init__.py
 src/setup/__init__.py
 src/stream/__init__.py
 src/transcribe/__init__.py
 src/translate/__init__.py
 src/voice/__init__.py
 src/webcam/__init__.py
 src/webcam2/__init__.py
```

### Comparing `aij-1.1.3/src/animation/__init__.py` & `aij-1.1.4/src/animation/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.3/src/download/__init__.py` & `aij-1.1.4/src/download/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.3/src/face/__init__.py` & `aij-1.1.4/src/face/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,376 +1,210 @@
 from datetime import datetime
-
-from typing import Optional
+from glob import glob
 import os
-
 import sys
+from typing import Optional
 import threading
-
 from deepface.basemodels.SFace import cv
-
 import requests
-
-
 from deepface import DeepFace
-
-
 import cv2
-
-
-import matplotlib.pyplot as plt
-
-
 import numpy as np
 import pandas as pd
-
-
-from glob import glob
-
-
-import cv2
-
-
-from deepface import DeepFace
-import pandas as pd
-
-
 import matplotlib.pyplot as plt
-
-
-import numpy as np
-
-
+import cv2
 import docker
 
-
 user_profile = os.environ['USERPROFILE']
-
-
 SEP = os.path.sep
-
-
 LOGO_URL = "https://raw.githubusercontent.com/codesapienbe/aij-webcam/master/logo.png"
-
-
 SCREEN_WIDTH = 1280
-
-
 SCREEN_HEIGHT = 720
-
-
 SCREEN_FPS = 30
-
-
 SCREEN_START_X = 0
-
-
 SCREEN_START_Y = 0
-
-
 SCREEN_MAXIMIZE = True
-
-
 APP_TITLE = 'AIJ'
 
-
 start = datetime.now().strftime("%Y%m%d%H%M%S")
-
 start_dt = datetime.now()
-
 config_home = user_profile + SEP + '.aij'
-
 config_abs = config_home + SEP + 'config.json'
-
 image_home = user_profile + SEP + '.aij' + SEP + 'image'
-
 logo_abs = image_home + SEP + 'logo.png'
-
 csv_home = user_profile + SEP + '.aij' + SEP + 'news'
-
 csv_abs = csv_home + SEP + 'news.csv'
-
 audio_home = user_profile + SEP + '.aij' + SEP + 'audio'
-
 screenshot_home = user_profile + SEP + '.aij' + SEP + 'screenshot'
-
 audio_abs = audio_home + SEP + start + '.mp3'
-
 video_home = user_profile + SEP + '.aij' + SEP + 'video'
-
 face_home = user_profile + SEP + '.aij' + SEP + 'face'
-
 news_df = Optional[pd.DataFrame]
-
 weather_df = Optional[pd.DataFrame]
 
-
 backends = [
-
-
-
     "opencv",
     "ssd",
-
-
-
     "dlib",
     "mtcnn",
     "retinaface",
     "mediapipe"
-
-
-
 ]
 
-
 default_backend = backends[0]
 
-
 models = [
-
-
-
     "VGG-Face",
-
-
     "Facenet",
-
-
-
     "Facenet512",
-
-
-
     "OpenFace",
-
-
-
     "DeepFace",
-
-
-
     "DeepID",
-
-
-
     "ArcFace",
-
-
-
     "Dlib",
-
-
-
     "SFace",
-
-
-
 ]
 
-
 default_model = models[0]
 
 
 def pre_init():
     """
     This function is called before the server is initialized
     """
 
     client = docker.from_env()
-
     # print all containers
-
     containers = client.containers.list()
 
     for container in containers:
-
         print(
             container.name,
             container.id,
             container.status
         )
 
     # if there is no docker container running named aij-messaging-server then run the server script 'aijinit'
 
     if not any(container.name == 'aij-messaging-server' for container in containers):
-
         os.system('aijinit')
 
 
 def download_logo():
     """
     Download the logo.png file to userprofile/.aij/images/logo.png
     """
 
     logo_remote_response = requests.get(
         LOGO_URL, allow_redirects=True, stream=True, timeout=10)
 
     if logo_remote_response.status_code == 200:
-
         # save the logo.png file if the response is ok and the file does not exist
-
         if not os.path.exists(logo_abs):
-
             with open(logo_abs, 'wb') as logo_file:
-
                 logo_file.write(logo_remote_response.content)
 
 
 def draw_text(image, x, y, text, color):
     """
-
     Draw text on the image
     """
 
     # draw a black rectangle on the image
 
     cv2.rectangle(
         image,
-
         (x, y - 25),
-
         # until the end of screen width
-
         (x + image.shape[1], y),
-
         (0, 0, 0),
-
         -1
-
     )
 
     # draw the text on the image
-
     cv2.putText(
         image,
-
         text,
-
         (x, y),
-
         cv2.FONT_HERSHEY_SIMPLEX,
-
         font_size / 12,
         color,
-
         2,
-
         cv2.LINE_AA
-
     )
 
 
 def draw_box(image, x, y, color):
     """
-
     Draw a box on the image
     """
-
     cv2.rectangle(
         image,
-
         (x, y),
-
         (x + box_size, y + box_size),
         color,
-
         2
-
     )
 
 
 def draw_button(image, x, y, text, color):
     """
-
     Draw a button on the image and write text on it
     """
 
     cv2.rectangle(
         image,
-
         (x, y),
-
         (x + box_size, y + box_size),
         color,
-
         2
-
     )
 
     cv2.putText(
         image,
-
         text,
-
         (x + 5, y + 30),
-
         cv2.FONT_HERSHEY_SIMPLEX,
-
         font_size,
         color,
-
         2,
-
         cv2.LINE_AA
-
     )
 
 
 def draw_zoomed_text(image, x, y, text, color):
     """
-
     Draw zoomed text on the image
     """
-
     cv2.putText(
         image,
-
         text,
-
         (x, y),
-
         cv2.FONT_HERSHEY_SIMPLEX,
-
         font_size,
         color,
-
         2,
-
         cv2.LINE_AA
-
     )
 
 
 def draw_logo(logo_path, img):
     if os.path.exists(logo_path):
-
         logo = cv2.imread(logo_path)
-
         # Resize the logo to match the height of the main image and keep the aspect ratio
-
         # resize the logo to 100px height and keep the aspect ratio
-
         logo_resized = cv2.resize(
             logo, (48, 48), interpolation=cv2.INTER_AREA)
-
         # get the height and width of the logo
-
         logo_height, logo_width, _ = logo_resized.shape
-
         # calculate the x and y coordinates of the logo
-
         x = 5
-
         y = 5
-
         # draw the logo on the main image
-
         img[y:y + logo_height, x:x + logo_width] = logo_resized
-
         return img
 
 
 def draw_emoji(current_emotion, img):
     emoji_home = user_profile + SEP + '.aij' + SEP + 'emojis'
 
     # find all emojis
@@ -378,126 +212,75 @@
         ".png") and emoji.startswith(current_emotion)]
     emj = cv2.imread(emoji_home + SEP + matching_emoji[0])
 
     # resize the emj to 64px height and keep the aspect ratio
     emj_resized = cv2.resize(emj, (64, 64), interpolation=cv2.INTER_AREA)
 
     # get the height and width of the emj
-
     emj_height, emj_width, _ = emj_resized.shape
-
     # get the height and width of the main image
-
     image_height, image_width, _ = img.shape
-
     # calculate the x and y coordinates of the emj
-
     x = image_width - emj_width - 5
-
     y = image_height - emj_height - 5
-
     # draw the emj on the main image
-
     img[y:y + emj_height, x:x + emj_width] = emj_resized
-
     return img
 
 
 # do not wait for the directories to be created
 thread_download_logo = threading.Thread(target=download_logo)
-
 thread_download_logo.start()
 
-
 default_backend = "opencv"
-
-
 default_model = "VGG-Face"
 
-
 cam = cv2.VideoCapture(0)
-
-
-# set the width and height, and UNSUCCESSFULLY set the exposure time
-
-
 cam.set(cv2.CAP_PROP_FRAME_WIDTH, SCREEN_WIDTH)
-
-
 cam.set(cv2.CAP_PROP_FRAME_HEIGHT, SCREEN_HEIGHT)
-
-
 cam.set(cv2.CAP_PROP_FPS, SCREEN_FPS)
 
-
 # Define min window size to be recognized as a face
-
-
 MIN_FACE_FRAME_WIDTH = 50
-
-
 MIN_FACE_FRAME_HEIGHT = 50
-
-
 FRAME_COUNTER = 0
-
 current_emotion = "neutral"
 
-
 while cam.isOpened():
 
     ret, img = cam.read()
-
     img = cv2.flip(img, 1)  # Flip vertically
-
     gray = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
 
     # increase the frame counter
-
     FRAME_COUNTER += 1
 
     try:
-
         # after each 5 seconds detect faces
-
         if FRAME_COUNTER >= SCREEN_FPS:
-
             # reset the frame counter
-
             FRAME_COUNTER = 0
-
             # predict the emotion
-
             emotion = DeepFace.analyze(img_path=img, actions=[
-
-
                 'emotion'], detector_backend=default_backend, align=True, silent=True)
 
             # get the emotion data from the dictionary
-
             emotion_data = emotion[0]['emotion']
-
             # convert to dataframe
-
             emotion_df = pd.DataFrame(emotion_data, index=[0])
-
             # get the dominant emotion
-
             emotion_label = emotion_df.idxmax(axis=1)[0]
-
             # add the emotion to the emotion history
             current_emotion = emotion_label
 
     except Exception as e:
-
         # draw error message if no face detected
         pass
 
     img = draw_emoji(current_emotion, img)
-
     img = draw_logo(logo_abs, img)
 
     cv2.imshow('Emotion Recognition', img)
 
     if cv2.waitKey(1) & 0xFF == ord('q'):
         cam.release()
         break
```

### Comparing `aij-1.1.3/src/intro/__init__.py` & `aij-1.1.4/src/intro/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.3/src/messaging/__init__.py` & `aij-1.1.4/src/messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.3/src/news/__init__.py` & `aij-1.1.4/src/news/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.3/src/setup/__init__.py` & `aij-1.1.4/src/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.3/src/stream/__init__.py` & `aij-1.1.4/src/stream/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.3/src/transcribe/__init__.py` & `aij-1.1.4/src/transcribe/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.3/src/translate/__init__.py` & `aij-1.1.4/src/translate/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.3/src/voice/__init__.py` & `aij-1.1.4/src/voice/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.3/src/webcam/__init__.py` & `aij-1.1.4/src/webcam/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,23 +9,21 @@
 
 import cv2
 import mediapipe as mp
 
 from gtts import gTTS
 from pygame import mixer
 
-from newsapi import NewsApiClient        
+from newsapi import NewsApiClient
 
 import docker
 from dotenv import load_dotenv
 
 load_dotenv()  # take environment variables from .env.
 
-from deepface import DeepFace
-
 # Constants and global variables
 api = NewsApiClient(api_key=os.environ['NEWSAPI_ORG'])
 user_profile = os.environ['USERPROFILE']
 SEP = os.path.sep
 LOGO_URL = "https://raw.githubusercontent.com/codesapienbe/aij-webcam/master/logo.png"
 CSV_URL = "https://raw.githubusercontent.com/codesapienbe/aij-webcam/master/news.csv"
 
@@ -49,14 +47,15 @@
 audio_home = user_profile + SEP + '.aij' + SEP + 'audio'
 screenshot_home = user_profile + SEP + '.aij' + SEP + 'screenshot'
 audio_abs = audio_home + SEP + start + '.mp3'
 video_home = user_profile + SEP + '.aij' + SEP + 'video'
 news_df = Optional[pd.DataFrame]
 weather_df = Optional[pd.DataFrame]
 
+
 def pre_init():
     """
     This function is called before the server is initialized
     """
     client = docker.from_env()
 
     # print all containers
@@ -81,47 +80,53 @@
     api_key = os.environ['WEATHERAPI_COM']
     region = os.environ['WEATHERAPI_COM_REGION']
     response = requests.get(
         f'http://api.weatherapi.com/v1/current.json?key={api_key}&q={region}&aqi=no'
     )
     return response.json()
 
+
 def get_weather_temp_c(weather):
     """
     Get the temperature in Celsius
     """
     return weather['current']['temp_c']
 
+
 def get_weather_temp_f(weather):
     """
     Get the temperature in Fahrenheit
     """
     return weather['current']['temp_f']
 
+
 def get_weather_to_df(weather):
     """
     Convert the weather to a dataframe
     """
     # map all the articles to a list
     current = weather['current']
 
     # create a dataframe
-    df = pd.DataFrame(current, columns=['temp_c', 'temp_f', 'condition', 'wind_mph', 'wind_kph', 'wind_degree', 'wind_dir', 'pressure_mb', 'pressure_in', 'precip_mm', 'precip_in', 'humidity', 'cloud', 'feelslike_c', 'feelslike_f', 'vis_km', 'vis_miles', 'uv', 'gust_mph', 'gust_kph'])
+    df = pd.DataFrame(current, columns=['temp_c', 'temp_f', 'condition', 'wind_mph', 'wind_kph', 'wind_degree', 'wind_dir', 'pressure_mb', 'pressure_in',
+                      'precip_mm', 'precip_in', 'humidity', 'cloud', 'feelslike_c', 'feelslike_f', 'vis_km', 'vis_miles', 'uv', 'gust_mph', 'gust_kph'])
 
     return df
 
+
 def get_top_headlines():
     """
     Get the top headlines from the newsapi.org API
     """
     response = api.get_top_headlines(
         sources='bbc-news, cnn, fox-news, google-news, the-new-york-times, the-wall-street-journal, the-washington-post, time, usa-today, wired'
     )
     return response
 
+
 def news_to_df(news):
     """
     Convert the news to a dataframe
     """
     # map all the articles to a list
     articles = list(map(lambda x: x['title'], news['articles']))
 
@@ -137,53 +142,59 @@
     return df
 
 
 def download_logo():
     """
     Download the logo.png file to userprofile/.aij/images/logo.png
     """
-    logo_remote_response = requests.get(LOGO_URL, allow_redirects=True, stream=True, timeout=10)
+    logo_remote_response = requests.get(
+        LOGO_URL, allow_redirects=True, stream=True, timeout=10)
 
     if logo_remote_response.status_code == 200:
         # save the logo.png file if the response is ok and the file does not exist
         if not os.path.exists(logo_abs):
             with open(logo_abs, 'wb') as logo_file:
                 logo_file.write(logo_remote_response.content)
 
+
 def download_news_csv() -> None:
     """
     Download the news.csv file to userprofile/.aij/news/news.csv
     """
-    csv_remote_response = requests.get(CSV_URL, allow_redirects=True, stream=True, timeout=10)
+    csv_remote_response = requests.get(
+        CSV_URL, allow_redirects=True, stream=True, timeout=10)
 
     if csv_remote_response.status_code == 200:
         # save the news.csv file if the response is ok and the file does not exist
         if not os.path.exists(csv_abs):
             with open(csv_abs, 'wb') as csv_file:
                 csv_file.write(csv_remote_response.content)
 
+
 def make_directories(paths: list):
     """
     Create directories if not exists
     """
     for path in paths:
         if not os.path.exists(path):
             os.mkdir(path)
 
+
 # do not wait for the directories to be created
 thread_download_logo = threading.Thread(target=download_logo)
 thread_download_news_csv = threading.Thread(target=download_news_csv)
 thread_download_logo.start()
 thread_download_news_csv.start()
 
 # make sure the directories are created before proceeding
 thread_download_logo.join()
 thread_download_news_csv.join()
 
-make_directories([config_home, image_home, csv_home, audio_home, screenshot_home, video_home])
+make_directories([config_home, image_home, csv_home,
+                 audio_home, screenshot_home, video_home])
 
 # if the internet connection is not available then use the local news.csv file
 network_status = os.system('ping -n 1 www.google.com')
 if network_status == 0:
     # get the top headlines from the newsapi.org API
     news = get_top_headlines()
     # convert the news to a dataframe
@@ -221,14 +232,15 @@
 
 direction = 0
 font_size = 12
 box_size = 50
 is_news_sliding = True
 is_news_playing = True
 
+
 def generate_audio_from_news():
     """
     Convert text to speech and play it
     """
     # initialize tts, create mp3 and play
     tts = gTTS(text=titles, lang='en')
 
@@ -254,15 +266,15 @@
         # high quality audio
         frequency=44100,
         # 16 bits per sample
         size=-16,
         # 2 channels (stereo)
         channels=2,
         # strong buffer to prevent audio stuttering
-        buffer=4096*2,
+        buffer=4096 * 2,
     )
     mixer.music.load(audio_abs)
     mixer.music.play()
 
 
 def pause_news_from_audio():
     """
@@ -375,15 +387,16 @@
         font_size,
         color,
         2,
         cv2.LINE_AA
     )
 
 
-thread_generate_audio_from_news = threading.Thread(target=generate_audio_from_news)
+thread_generate_audio_from_news = threading.Thread(
+    target=generate_audio_from_news)
 thread_play_news_from_audio = threading.Thread(target=play_news_from_audio)
 
 # make sure the audio file is generated before playing it
 thread_generate_audio_from_news.start()
 thread_generate_audio_from_news.join()
 thread_play_news_from_audio.start()
 
@@ -480,15 +493,15 @@
                     is_news_playing = True
 
         else:
             # if no hands are detected then move the text to the left
             font_size = 12
             color = standard_text_color
             box_size = 50
-            
+
         if is_news_playing:
             resume_news_from_audio()
         else:
             pause_news_from_audio()
 
         if is_news_sliding and direction == 0:
             titles = titles[1:] + titles[0]
@@ -506,15 +519,16 @@
             draw_text(image, image.shape[1] - 250, 30, weather, color)
 
         # if there is a logo then draw it
         if os.path.exists(logo_abs):
             logo = cv2.imread(logo_abs)
             # Resize the logo to match the height of the main image and keep the aspect ratio
             # resize the logo to 100px height and keep the aspect ratio
-            logo_resized = cv2.resize(logo, (100, 100), interpolation=cv2.INTER_AREA)
+            logo_resized = cv2.resize(
+                logo, (100, 100), interpolation=cv2.INTER_AREA)
             # get the height and width of the logo
             logo_height, logo_width, _ = logo_resized.shape
             # get the height and width of the main image
             image_height, image_width, _ = image.shape
             # calculate the x and y coordinates of the logo
             x = image_width - logo_width - 10
             y = image_height - logo_height - 30
```

### Comparing `aij-1.1.3/src/webcam2/__init__.py` & `aij-1.1.4/src/webcam2/__init__.py`

 * *Files identical despite different names*

