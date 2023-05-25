# Comparing `tmp/aij-1.0.9.tar.gz` & `tmp/aij-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aij-1.0.9.tar", last modified: Sun May 21 20:06:42 2023, max compression
+gzip compressed data, was "aij-1.1.1.tar", last modified: Thu May 25 22:44:45 2023, max compression
```

## Comparing `aij-1.0.9.tar` & `aij-1.1.1.tar`

### file list

```diff
@@ -1,28 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 20:06:42.797595 aij-1.0.9/
--rw-rw-rw-   0        0        0     1100 2023-05-21 18:35:40.000000 aij-1.0.9/LICENSE.txt
--rw-rw-rw-   0        0        0    30052 2023-05-21 20:06:42.795586 aij-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0    27745 2023-05-21 18:35:40.000000 aij-1.0.9/README.md
--rw-rw-rw-   0        0        0     6423 2023-05-21 20:06:32.000000 aij-1.0.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-21 20:06:42.797595 aij-1.0.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-21 20:06:42.729812 aij-1.0.9/src/
-drwxrwxrwx   0        0        0        0 2023-05-21 20:06:42.777360 aij-1.0.9/src/aij.egg-info/
--rw-rw-rw-   0        0        0    30052 2023-05-21 20:06:42.000000 aij-1.0.9/src/aij.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      382 2023-05-21 20:06:42.000000 aij-1.0.9/src/aij.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 20:06:42.000000 aij-1.0.9/src/aij.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2023-05-21 20:06:42.000000 aij-1.0.9/src/aij.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      252 2023-05-21 20:06:42.000000 aij-1.0.9/src/aij.egg-info/requires.txt
--rw-rw-rw-   0        0        0       46 2023-05-21 20:06:42.000000 aij-1.0.9/src/aij.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-21 20:06:42.778997 aij-1.0.9/src/chat/
--rw-rw-rw-   0        0        0      561 2023-05-21 19:57:44.000000 aij-1.0.9/src/chat/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-21 20:06:42.781183 aij-1.0.9/src/intro/
--rw-rw-rw-   0        0        0     4607 2023-05-21 19:15:32.000000 aij-1.0.9/src/intro/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-21 20:06:42.784075 aij-1.0.9/src/messaging/
--rw-rw-rw-   0        0        0     4444 2023-05-21 19:19:30.000000 aij-1.0.9/src/messaging/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-21 20:06:42.786822 aij-1.0.9/src/news/
--rw-rw-rw-   0        0        0     9588 2023-05-21 19:19:41.000000 aij-1.0.9/src/news/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-21 20:06:42.788524 aij-1.0.9/src/setup/
--rw-rw-rw-   0        0        0     3080 2023-05-21 19:19:56.000000 aij-1.0.9/src/setup/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-21 20:06:42.791048 aij-1.0.9/src/speech/
--rw-rw-rw-   0        0        0     1289 2023-05-21 19:35:54.000000 aij-1.0.9/src/speech/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-21 20:06:42.793600 aij-1.0.9/src/webcam/
--rw-rw-rw-   0        0        0    17592 2023-05-21 19:07:03.000000 aij-1.0.9/src/webcam/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 22:44:45.742538 aij-1.1.1/
+-rw-rw-rw-   0        0        0     1100 2023-05-21 18:35:40.000000 aij-1.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0    30052 2023-05-25 22:44:45.742538 aij-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    27745 2023-05-21 18:35:40.000000 aij-1.1.1/README.md
+-rw-rw-rw-   0        0        0     6939 2023-05-25 22:44:32.000000 aij-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-25 22:44:45.743542 aij-1.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-25 22:44:45.679369 aij-1.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-25 22:44:45.718998 aij-1.1.1/src/aij.egg-info/
+-rw-rw-rw-   0        0        0    30052 2023-05-25 22:44:45.000000 aij-1.1.1/src/aij.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      553 2023-05-25 22:44:45.000000 aij-1.1.1/src/aij.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 22:44:45.000000 aij-1.1.1/src/aij.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      197 2023-05-25 22:44:45.000000 aij-1.1.1/src/aij.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      491 2023-05-25 22:44:45.000000 aij-1.1.1/src/aij.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      105 2023-05-25 22:44:45.000000 aij-1.1.1/src/aij.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-25 22:44:45.720001 aij-1.1.1/src/animation/
+-rw-rw-rw-   0        0        0     5739 2023-05-25 21:36:22.000000 aij-1.1.1/src/animation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 22:44:45.722001 aij-1.1.1/src/chat/
+-rw-rw-rw-   0        0        0      680 2023-05-21 20:35:30.000000 aij-1.1.1/src/chat/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 22:44:45.723000 aij-1.1.1/src/download/
+-rw-rw-rw-   0        0        0     8301 2023-05-24 21:25:22.000000 aij-1.1.1/src/download/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 22:44:45.724998 aij-1.1.1/src/face/
+-rw-rw-rw-   0        0        0     8295 2023-05-25 16:52:45.000000 aij-1.1.1/src/face/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 22:44:45.726000 aij-1.1.1/src/intro/
+-rw-rw-rw-   0        0        0     4532 2023-05-24 21:19:40.000000 aij-1.1.1/src/intro/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 22:44:45.726997 aij-1.1.1/src/messaging/
+-rw-rw-rw-   0        0        0     5060 2023-05-23 19:12:37.000000 aij-1.1.1/src/messaging/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 22:44:45.728514 aij-1.1.1/src/news/
+-rw-rw-rw-   0        0        0    10270 2023-05-25 21:21:31.000000 aij-1.1.1/src/news/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 22:44:45.730529 aij-1.1.1/src/setup/
+-rw-rw-rw-   0        0        0     3925 2023-05-24 22:31:30.000000 aij-1.1.1/src/setup/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 22:44:45.731525 aij-1.1.1/src/stream/
+-rw-rw-rw-   0        0        0     1093 2023-05-24 23:06:34.000000 aij-1.1.1/src/stream/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 22:44:45.734529 aij-1.1.1/src/transcribe/
+-rw-rw-rw-   0        0        0     2215 2023-05-25 21:10:13.000000 aij-1.1.1/src/transcribe/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 22:44:45.735527 aij-1.1.1/src/translate/
+-rw-rw-rw-   0        0        0     2393 2023-05-25 21:47:13.000000 aij-1.1.1/src/translate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 22:44:45.737537 aij-1.1.1/src/voice/
+-rw-rw-rw-   0        0        0     2332 2023-05-25 22:34:55.000000 aij-1.1.1/src/voice/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 22:44:45.738544 aij-1.1.1/src/webcam/
+-rw-rw-rw-   0        0        0    18706 2023-05-24 23:40:36.000000 aij-1.1.1/src/webcam/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 22:44:45.740536 aij-1.1.1/src/webcam2/
+-rw-rw-rw-   0        0        0     3351 2023-05-25 22:17:56.000000 aij-1.1.1/src/webcam2/__init__.py
```

### Comparing `aij-1.0.9/LICENSE.txt` & `aij-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aij-1.0.9/PKG-INFO` & `aij-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij
-Version: 1.0.9
+Version: 1.1.1
 Summary: AI Journalist
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-1.0.9/README.md` & `aij-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `aij-1.0.9/pyproject.toml` & `aij-1.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "aij"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.0.9"
+version = "1.1.01"
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "AI Journalist"  # Optional
 
 # This is an optional longer description of your project that represents
@@ -100,30 +100,53 @@
     "requests",
     "setuptools",
     "wheel",
     "pipenv",
     "pylint",
     "autopep8",
     "pyinstaller",
+    "black",
+    "coveralls",
+    "coverage",
+    "flake8",
+    "mypy",
+    "pep8-naming",
+    "pre-commit",
     "pytest",
     "pytest-cov",
+    "pytest-mock",
+    "pytest-profiling",
     "opencv-python",
     "mediapipe",
     "pandas",
     "gtts",
     "pygame",
     "cairosvg",
     "pika",
     "newsapi-python",
     "openai",
     "openai-whisper",
     "langchain",
     "plyer",
     "python-dotenv",
-    "kivy[dev]"
+    "kivy[dev]",
+    "docker",
+    "youtube_dl",
+    "python_ffmpeg",
+    "psutil",
+    "flask",
+    "flask-socketio",
+    "flask-cors",
+    "flask-sqlalchemy",
+    "deepface",
+    "speechbrain",
+    "soundfile",
+    "transformers",
+    "langchain",
+    "pytube3"
 ]
 
 # List additional groups of dependencies here (e.g. development
 # dependencies). Users will be able to install these using the "extras"
 # syntax, for example:
 #
 #   $ pip install sampleproject[dev]
@@ -151,17 +174,21 @@
 "Say Thanks!" = "http://saythanks.io/to/aij"
 "Source" = "https://github.com/codesapienbe/aij"
 
 # The following would provide a command line executable called `sample`
 # which executes the function `main` from this package when invoked.
 [project.scripts]  # Optional
 aij = "webcam:main"
-aijn = "news:main"
-aiji = "intro:main"
-aijt = "speech:main"
+aijnews = "news:main"
+aijintro = "intro:main"
+aijtranscribe = "transcribe:main"
+aijchat = "chat:main"
+aijtube = "download:main"
+aijinit = "setup:main"
+aijvoice = "voice:main"
 
 # This is configuration specific to the `setuptools` build backend.
 # If you are using a different build backend, you will need to change this.
 [tool.setuptools]
 # If there are data files included in your packages that need to be
 # installed, specify them here.
 package-data = { "db" = ["*.dat"] }
```

### Comparing `aij-1.0.9/src/aij.egg-info/PKG-INFO` & `aij-1.1.1/src/aij.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij
-Version: 1.0.9
+Version: 1.1.1
 Summary: AI Journalist
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-1.0.9/src/intro/__init__.py` & `aij-1.1.1/src/intro/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import cv2
 import os
 import random
 import numpy as np
 import threading
 from pygame import mixer
 
+# import ffmpeg and extract audio from the video
+import ffmpeg
+
 user_profile = os.environ['USERPROFILE']
 SEP = os.path.sep
 
-
 class AnimationThread(threading.Thread):
     """
     This class represents a thread that generates an animation video
     """
 
     def __init__(self):
         """
@@ -99,22 +101,19 @@
 
             # Write the frame to the video writer
             self.video_writer.write(frame)
 
         # Release the video writer
         self.video_writer.release()
 
-        # merge the audio and video files
-        os.system(
-            'ffmpeg -i animation.mp4 -i ' + self.audio_intro_abs +
-            ' -c:v copy -c:a aac -strict experimental animation_with_audio.mp4')
+        
+        ffmpeg.input('animation.mp4').output('animation_with_audio.mp4').run()
 
         # Print the path of the animation video
-        print('Animation video generated at: ' +
-            os.getcwd() + SEP + 'animation_with_audio.mp4')
+        print('Animation video generated at ' + os.path.abspath('animation_with_audio.mp4'))
 
 
 def main():
     """
     This function is the entry point of the program
     @param: None
     @return: None
```

### Comparing `aij-1.0.9/src/messaging/__init__.py` & `aij-1.1.1/src/messaging/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,17 +7,19 @@
 from kivy.app import App
 from kivy.core.window import Window
 from kivy.uix.boxlayout import BoxLayout
 from kivy.uix.button import Button
 from kivy.uix.label import Label
 
 from dotenv import load_dotenv
+import docker
 
 load_dotenv()  # take environment variables from .env.
 
+
 class AIJMessagingServer(App):
     """
     A class to create a GUI for the publisher and subscriber
     """
 
     def build(self):
         """
@@ -55,19 +57,37 @@
         # change the background color of the button to red
         self.publisher_button.background_color = rgb
 
     def start(self, instance):
         """
         Initialize the RabbitMQ server
         """
-        # run os.system() as a thread to start the RabbitMQ server
-        rabbit_mq_thread = Thread(target=os.system, args=('rabbitmq-server',))
-
-        # start the thread
-        rabbit_mq_thread.start()
+        client = docker.from_env()
+        # docker run -d --hostname my-rabbit --name some-rabbit rabbitmq:3
+        client.containers.run(
+            "rabbitmq:3", 
+            name='aij-messaging-server',
+            hostname='aij-messaging-server',
+            ports={'5672/tcp': 5672},
+            environment={'RABBITMQ_DEFAULT_USER': 'admin', 'RABBITMQ_DEFAULT_PASS': 'admin'},
+            volumes={
+                
+            },
+            detach=True
+        )
+
+        # print all containers
+        containers = client.containers.list()
+
+        for container in containers:
+            print(
+                container.name,
+                container.id,
+                container.status
+            )
 
         # change the text of the button to 'Stop'
         self.publisher_button.text = 'Stop'
 
         # bind the button click event to the stop method
         self.publisher_button.bind(on_press=self.stop)
 
@@ -77,16 +97,18 @@
         # bind the keyboard key event to the on_keyboard method
         Window.bind(on_keyboard=self.on_keyboard)
 
     def stop(self, instance):
         """
         Stop the RabbitMQ server
         """
-        # stop the thread by searching for the process id of the RabbitMQ server
-        os.system('taskkill /F /IM rabbitmq-server.exe')
+        # stop the container with the name 'aij-messaging-server' and remove it
+        client = docker.from_env()
+        container = client.containers.get('aij-messaging-server')
+        container.stop()
 
         # change the text of the button to 'Start'
         self.publisher_button.text = 'Start'
 
         # bind the button click event to the start method
         self.publisher_button.bind(on_press=self.start)
```

### Comparing `aij-1.0.9/src/news/__init__.py` & `aij-1.1.1/src/news/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # using Kivy to create a GUI for the publisher and subscriber
 from kivy.app import App
 from kivy.core.window import Window
 from kivy.uix.boxlayout import BoxLayout
 from kivy.uix.button import Button
 from kivy.uix.label import Label
 
-
+import docker
 from dotenv import load_dotenv
 
 load_dotenv()  # take environment variables from .env.
 
 class NewsPublisher:
     """
     A class to publish news articles to a RabbitMQ queue using the NewsAPI
@@ -244,19 +244,43 @@
             f'key: {key}\n'
             f'scancode: {scancode}\n'
             f'codepoint: {codepoint}\n'
             f'modifier: {modifier}\n'
         )
 
 
+def pre_init():
+    """
+    This function is called before the server is initialized
+    """
+    client = docker.from_env()
+
+    # print all containers
+    containers = client.containers.list()
+
+    for container in containers:
+        print(
+            container.name,
+            container.id,
+            container.status
+        )
+
+    # if there is no docker container running named aij-messaging-server then run the server script 'aijinit'
+    if not any(container.name == 'aij-messaging-server' for container in containers):
+        os.system('aijinit')
+
+
 def main():
     """
     The main function to run the server and publish the news articles to the RabbitMQ queue
     """
     print('Server is being initialized...')
+    
+    # initialize the server if it is not already initialized
+    pre_init()
 
     # create an instance of the AIJKivy class
     app = AIJKivy()
     app.run()
 
     print('Server is now running...')
```

### Comparing `aij-1.0.9/src/webcam/__init__.py` & `aij-1.1.1/src/webcam/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,18 +11,21 @@
 import mediapipe as mp
 
 from gtts import gTTS
 from pygame import mixer
 
 from newsapi import NewsApiClient        
 
+import docker
 from dotenv import load_dotenv
 
 load_dotenv()  # take environment variables from .env.
 
+from deepface import DeepFace
+
 # Constants and global variables
 api = NewsApiClient(api_key=os.environ['NEWSAPI_ORG'])
 user_profile = os.environ['USERPROFILE']
 SEP = os.path.sep
 LOGO_URL = "https://raw.githubusercontent.com/codesapienbe/aij-webcam/master/logo.png"
 CSV_URL = "https://raw.githubusercontent.com/codesapienbe/aij-webcam/master/news.csv"
 
@@ -46,14 +49,34 @@
 audio_home = user_profile + SEP + '.aij' + SEP + 'audio'
 screenshot_home = user_profile + SEP + '.aij' + SEP + 'screenshot'
 audio_abs = audio_home + SEP + start + '.mp3'
 video_home = user_profile + SEP + '.aij' + SEP + 'video'
 news_df = Optional[pd.DataFrame]
 weather_df = Optional[pd.DataFrame]
 
+def pre_init():
+    """
+    This function is called before the server is initialized
+    """
+    client = docker.from_env()
+
+    # print all containers
+    containers = client.containers.list()
+
+    for container in containers:
+        print(
+            container.name,
+            container.id,
+            container.status
+        )
+
+    # if there is no docker container running named aij-messaging-server then run the server script 'aijinit'
+    if not any(container.name == 'aij-messaging-server' for container in containers):
+        os.system('aijinit')
+
 
 def get_weather():
     """
     Get the weather from the weatherapi.com API
     """
     api_key = os.environ['WEATHERAPI_COM']
     region = os.environ['WEATHERAPI_COM_REGION']
@@ -109,14 +132,15 @@
     df['title_length'] = df['title'].apply(lambda x: len(x))
 
     # add a column for the number of words in the title
     df['title_words'] = df['title'].apply(lambda x: len(x.split(' ')))
 
     return df
 
+
 def download_logo():
     """
     Download the logo.png file to userprofile/.aij/images/logo.png
     """
     logo_remote_response = requests.get(LOGO_URL, allow_redirects=True, stream=True, timeout=10)
 
     if logo_remote_response.status_code == 200:
@@ -194,15 +218,16 @@
 zoomed_text_color = (0, 255, 0)
 standard_text_color = (255, 255, 255)
 color = standard_text_color
 
 direction = 0
 font_size = 12
 box_size = 50
-news_are_being_played = False
+is_news_sliding = True
+is_news_playing = True
 
 def generate_audio_from_news():
     """
     Convert text to speech and play it
     """
     # initialize tts, create mp3 and play
     tts = gTTS(text=titles, lang='en')
@@ -399,67 +424,79 @@
                     mp_drawing_styles.get_default_hand_connections_style())
 
                 # if left hand is raised then move the text to the left
                 if hand_landmarks.landmark[mp_hands.HandLandmark.WRIST].x < 0.2 and len(results.multi_hand_landmarks) == 1:
                     for i in range(30):
                         # move the text to the left
                         pass
-                    titles = titles[1:] + titles[0]
                     direction = 0
                     font_size = 12
                     color = standard_text_color
                     box_size = 50
+                    is_news_sliding = True
 
                 # if right hand is raised then move the text to the right
                 elif hand_landmarks.landmark[mp_hands.HandLandmark.WRIST].x > 0.8 and len(results.multi_hand_landmarks) == 1:
                     for i in range(30):
                         # move the text to the left
                         pass
                     direction = 1
                     font_size = 12
                     color = standard_text_color
                     box_size = 50
+                    is_news_sliding = True
 
                 # if both hands are raised and all fingers are up then increase the font size to 36pt and change the color
                 elif 0.2 < hand_landmarks.landmark[mp_hands.HandLandmark.WRIST].x < 0.8 and len(results.multi_hand_landmarks) == 2 and hand_landmarks.landmark[mp_hands.HandLandmark.THUMB_TIP].y < hand_landmarks.landmark[mp_hands.HandLandmark.THUMB_IP].y and hand_landmarks.landmark[mp_hands.HandLandmark.INDEX_FINGER_TIP].y < hand_landmarks.landmark[mp_hands.HandLandmark.INDEX_FINGER_PIP].y and hand_landmarks.landmark[mp_hands.HandLandmark.MIDDLE_FINGER_TIP].y < hand_landmarks.landmark[mp_hands.HandLandmark.MIDDLE_FINGER_PIP].y and hand_landmarks.landmark[mp_hands.HandLandmark.RING_FINGER_TIP].y < hand_landmarks.landmark[mp_hands.HandLandmark.RING_FINGER_PIP].y and hand_landmarks.landmark[mp_hands.HandLandmark.PINKY_TIP].y < hand_landmarks.landmark[mp_hands.HandLandmark.PINKY_PIP].y:
                     for i in range(30):
                         # move the text to the left
                         pass
                     font_size = 36
                     color = zoomed_text_color
                     box_size = 100
+                    is_news_sliding = False
 
                 # if both hands are raised and all fingers are closed then stop the news
                 if 0.2 < hand_landmarks.landmark[mp_hands.HandLandmark.WRIST].x < 0.8 and len(results.multi_hand_landmarks) == 2 and hand_landmarks.landmark[mp_hands.HandLandmark.THUMB_TIP].y > hand_landmarks.landmark[mp_hands.HandLandmark.THUMB_IP].y and hand_landmarks.landmark[mp_hands.HandLandmark.INDEX_FINGER_TIP].y > hand_landmarks.landmark[mp_hands.HandLandmark.INDEX_FINGER_PIP].y and hand_landmarks.landmark[mp_hands.HandLandmark.MIDDLE_FINGER_TIP].y > hand_landmarks.landmark[mp_hands.HandLandmark.MIDDLE_FINGER_PIP].y and hand_landmarks.landmark[mp_hands.HandLandmark.RING_FINGER_TIP].y > hand_landmarks.landmark[mp_hands.HandLandmark.RING_FINGER_PIP].y and hand_landmarks.landmark[mp_hands.HandLandmark.PINKY_TIP].y > hand_landmarks.landmark[mp_hands.HandLandmark.PINKY_PIP].y:
+                    for i in range(30):
+                        # move the text to the left
+                        pass
                     # stop sliding the news
                     # stop the news
-                    pause_news_from_audio()
+                    is_news_sliding = False
+                    is_news_playing = False
                     direction = 2
                     font_size = 12
                     color = standard_text_color
                     box_size = 50
 
                 # if both hands are raised, thumb and index finger are open then increase the font size to 36pt and change the color
                 if 0.2 < hand_landmarks.landmark[mp_hands.HandLandmark.WRIST].x < 0.8 and len(results.multi_hand_landmarks) == 2 and hand_landmarks.landmark[mp_hands.HandLandmark.THUMB_TIP].y < hand_landmarks.landmark[mp_hands.HandLandmark.THUMB_IP].y and hand_landmarks.landmark[mp_hands.HandLandmark.INDEX_FINGER_TIP].y < hand_landmarks.landmark[mp_hands.HandLandmark.INDEX_FINGER_PIP].y and hand_landmarks.landmark[mp_hands.HandLandmark.MIDDLE_FINGER_TIP].y > hand_landmarks.landmark[mp_hands.HandLandmark.MIDDLE_FINGER_PIP].y and hand_landmarks.landmark[mp_hands.HandLandmark.RING_FINGER_TIP].y > hand_landmarks.landmark[mp_hands.HandLandmark.RING_FINGER_PIP].y and hand_landmarks.landmark[mp_hands.HandLandmark.PINKY_TIP].y > hand_landmarks.landmark[mp_hands.HandLandmark.PINKY_PIP].y:
                     # rewind the news
-                    resume_news_from_audio()
                     direction = 0
                     font_size = 12
                     color = standard_text_color
                     box_size = 50
+                    is_news_sliding = True
+                    is_news_playing = True
 
         else:
             # if no hands are detected then move the text to the left
             font_size = 12
             color = standard_text_color
             box_size = 50
+            
+        if is_news_playing:
+            resume_news_from_audio()
+        else:
+            pause_news_from_audio()
 
-        if direction == 0:
+        if is_news_sliding and direction == 0:
             titles = titles[1:] + titles[0]
-        elif direction == 1:
+        elif is_news_sliding and direction == 1:
             titles = titles[-1] + titles[:-1]
         elif direction == 2:
             pass
 
         # draw the text
         draw_text(image, 2, image.shape[0] - 10, titles, color)
```

