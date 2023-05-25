# Comparing `tmp/aij-1.1.2.tar.gz` & `tmp/aij-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aij-1.1.2.tar", last modified: Thu May 25 22:50:54 2023, max compression
+gzip compressed data, was "aij-1.1.3.tar", last modified: Thu May 25 23:28:38 2023, max compression
```

## Comparing `aij-1.1.2.tar` & `aij-1.1.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 22:50:54.896662 aij-1.1.2/
--rw-rw-rw-   0        0        0     1100 2023-05-21 18:35:40.000000 aij-1.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0    30052 2023-05-25 22:50:54.894589 aij-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0    27745 2023-05-21 18:35:40.000000 aij-1.1.2/README.md
--rw-rw-rw-   0        0        0     6993 2023-05-25 22:50:44.000000 aij-1.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-25 22:50:54.897688 aij-1.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-25 22:50:54.831571 aij-1.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-25 22:50:54.870575 aij-1.1.2/src/aij.egg-info/
--rw-rw-rw-   0        0        0    30052 2023-05-25 22:50:54.000000 aij-1.1.2/src/aij.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      553 2023-05-25 22:50:54.000000 aij-1.1.2/src/aij.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 22:50:54.000000 aij-1.1.2/src/aij.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      247 2023-05-25 22:50:54.000000 aij-1.1.2/src/aij.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      491 2023-05-25 22:50:54.000000 aij-1.1.2/src/aij.egg-info/requires.txt
--rw-rw-rw-   0        0        0      105 2023-05-25 22:50:54.000000 aij-1.1.2/src/aij.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-25 22:50:54.871578 aij-1.1.2/src/animation/
--rw-rw-rw-   0        0        0     5739 2023-05-25 21:36:22.000000 aij-1.1.2/src/animation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 22:50:54.872579 aij-1.1.2/src/chat/
--rw-rw-rw-   0        0        0      680 2023-05-21 20:35:30.000000 aij-1.1.2/src/chat/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 22:50:54.875107 aij-1.1.2/src/download/
--rw-rw-rw-   0        0        0     8301 2023-05-24 21:25:22.000000 aij-1.1.2/src/download/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 22:50:54.876112 aij-1.1.2/src/face/
--rw-rw-rw-   0        0        0     8295 2023-05-25 16:52:45.000000 aij-1.1.2/src/face/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 22:50:54.878107 aij-1.1.2/src/intro/
--rw-rw-rw-   0        0        0     4532 2023-05-24 21:19:40.000000 aij-1.1.2/src/intro/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 22:50:54.881138 aij-1.1.2/src/messaging/
--rw-rw-rw-   0        0        0     5060 2023-05-23 19:12:37.000000 aij-1.1.2/src/messaging/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 22:50:54.882128 aij-1.1.2/src/news/
--rw-rw-rw-   0        0        0    10270 2023-05-25 21:21:31.000000 aij-1.1.2/src/news/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 22:50:54.884126 aij-1.1.2/src/setup/
--rw-rw-rw-   0        0        0     3925 2023-05-24 22:31:30.000000 aij-1.1.2/src/setup/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 22:50:54.885127 aij-1.1.2/src/stream/
--rw-rw-rw-   0        0        0     1093 2023-05-24 23:06:34.000000 aij-1.1.2/src/stream/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 22:50:54.887127 aij-1.1.2/src/transcribe/
--rw-rw-rw-   0        0        0     2215 2023-05-25 21:10:13.000000 aij-1.1.2/src/transcribe/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 22:50:54.888128 aij-1.1.2/src/translate/
--rw-rw-rw-   0        0        0     2393 2023-05-25 21:47:13.000000 aij-1.1.2/src/translate/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 22:50:54.890127 aij-1.1.2/src/voice/
--rw-rw-rw-   0        0        0     2332 2023-05-25 22:34:55.000000 aij-1.1.2/src/voice/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 22:50:54.891128 aij-1.1.2/src/webcam/
--rw-rw-rw-   0        0        0    18706 2023-05-24 23:40:36.000000 aij-1.1.2/src/webcam/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 22:50:54.893358 aij-1.1.2/src/webcam2/
--rw-rw-rw-   0        0        0     3351 2023-05-25 22:17:56.000000 aij-1.1.2/src/webcam2/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 23:28:38.746877 aij-1.1.3/
+-rw-rw-rw-   0        0        0     1100 2023-05-21 18:35:40.000000 aij-1.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0    30052 2023-05-25 23:28:38.745463 aij-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0    27745 2023-05-21 18:35:40.000000 aij-1.1.3/README.md
+-rw-rw-rw-   0        0        0     6993 2023-05-25 23:28:24.000000 aij-1.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-25 23:28:38.746877 aij-1.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-25 23:28:38.668489 aij-1.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-25 23:28:38.715068 aij-1.1.3/src/aij.egg-info/
+-rw-rw-rw-   0        0        0    30052 2023-05-25 23:28:38.000000 aij-1.1.3/src/aij.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      553 2023-05-25 23:28:38.000000 aij-1.1.3/src/aij.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 23:28:38.000000 aij-1.1.3/src/aij.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      247 2023-05-25 23:28:38.000000 aij-1.1.3/src/aij.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      491 2023-05-25 23:28:38.000000 aij-1.1.3/src/aij.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      105 2023-05-25 23:28:38.000000 aij-1.1.3/src/aij.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-25 23:28:38.717062 aij-1.1.3/src/animation/
+-rw-rw-rw-   0        0        0     5739 2023-05-25 21:36:22.000000 aij-1.1.3/src/animation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 23:28:38.719065 aij-1.1.3/src/chat/
+-rw-rw-rw-   0        0        0      680 2023-05-21 20:35:30.000000 aij-1.1.3/src/chat/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 23:28:38.721085 aij-1.1.3/src/download/
+-rw-rw-rw-   0        0        0     8301 2023-05-24 21:25:22.000000 aij-1.1.3/src/download/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 23:28:38.723079 aij-1.1.3/src/face/
+-rw-rw-rw-   0        0        0     8295 2023-05-25 16:52:45.000000 aij-1.1.3/src/face/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 23:28:38.725080 aij-1.1.3/src/intro/
+-rw-rw-rw-   0        0        0     4532 2023-05-24 21:19:40.000000 aij-1.1.3/src/intro/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 23:28:38.727077 aij-1.1.3/src/messaging/
+-rw-rw-rw-   0        0        0     5060 2023-05-23 19:12:37.000000 aij-1.1.3/src/messaging/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 23:28:38.729563 aij-1.1.3/src/news/
+-rw-rw-rw-   0        0        0    10270 2023-05-25 21:21:31.000000 aij-1.1.3/src/news/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 23:28:38.731817 aij-1.1.3/src/setup/
+-rw-rw-rw-   0        0        0     3925 2023-05-24 22:31:30.000000 aij-1.1.3/src/setup/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 23:28:38.733823 aij-1.1.3/src/stream/
+-rw-rw-rw-   0        0        0     1093 2023-05-24 23:06:34.000000 aij-1.1.3/src/stream/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 23:28:38.735130 aij-1.1.3/src/transcribe/
+-rw-rw-rw-   0        0        0     2215 2023-05-25 21:10:13.000000 aij-1.1.3/src/transcribe/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 23:28:38.736123 aij-1.1.3/src/translate/
+-rw-rw-rw-   0        0        0     2393 2023-05-25 21:47:13.000000 aij-1.1.3/src/translate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 23:28:38.738656 aij-1.1.3/src/voice/
+-rw-rw-rw-   0        0        0     2239 2023-05-25 23:23:39.000000 aij-1.1.3/src/voice/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 23:28:38.740654 aij-1.1.3/src/webcam/
+-rw-rw-rw-   0        0        0    18706 2023-05-24 23:40:36.000000 aij-1.1.3/src/webcam/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 23:28:38.742659 aij-1.1.3/src/webcam2/
+-rw-rw-rw-   0        0        0     3351 2023-05-25 22:17:56.000000 aij-1.1.3/src/webcam2/__init__.py
```

### Comparing `aij-1.1.2/LICENSE.txt` & `aij-1.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aij-1.1.2/PKG-INFO` & `aij-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij
-Version: 1.1.2
+Version: 1.1.3
 Summary: AI Journalist
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-1.1.2/README.md` & `aij-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `aij-1.1.2/pyproject.toml` & `aij-1.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "aij"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.1.02"
+version = "1.1.03"
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "AI Journalist"  # Optional
 
 # This is an optional longer description of your project that represents
```

### Comparing `aij-1.1.2/src/aij.egg-info/PKG-INFO` & `aij-1.1.3/src/aij.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij
-Version: 1.1.2
+Version: 1.1.3
 Summary: AI Journalist
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-1.1.2/src/aij.egg-info/SOURCES.txt` & `aij-1.1.3/src/aij.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aij-1.1.2/src/animation/__init__.py` & `aij-1.1.3/src/animation/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.2/src/chat/__init__.py` & `aij-1.1.3/src/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.2/src/download/__init__.py` & `aij-1.1.3/src/download/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.2/src/face/__init__.py` & `aij-1.1.3/src/face/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.2/src/intro/__init__.py` & `aij-1.1.3/src/intro/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.2/src/messaging/__init__.py` & `aij-1.1.3/src/messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.2/src/news/__init__.py` & `aij-1.1.3/src/news/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.2/src/setup/__init__.py` & `aij-1.1.3/src/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.2/src/stream/__init__.py` & `aij-1.1.3/src/stream/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.2/src/transcribe/__init__.py` & `aij-1.1.3/src/transcribe/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.2/src/translate/__init__.py` & `aij-1.1.3/src/translate/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.2/src/voice/__init__.py` & `aij-1.1.3/src/voice/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,47 +1,46 @@
 import pika
 import speech_recognition as sr
-
+import os, sys
 import docker
 from dotenv import load_dotenv
 
 load_dotenv()  # take environment variables from .env.
 
 class VoiceToTextServer:
     def __init__(self, source_lang='en-US'):
         self.source_lang = source_lang
         self.timer = 0
         self.connection = pika.BlockingConnection(
             pika.ConnectionParameters('localhost'))
         self.channel = self.connection.channel()
         self.channel.queue_declare(queue='speech_to_text_stream')
         self.r = sr.Recognizer()
-        self.r.energy_threshold = 4000
         self.r.dynamic_energy_threshold = True
 
     def start(self):
+        # start listening to mic stream
         with sr.Microphone() as source:
             self.r.adjust_for_ambient_noise(source)
-            audio = self.r.listen(source, timeout=5)
+            audio = self.r.listen(source, timeout=30, phrase_time_limit=5)
 
             try:
-                recognized_text = self.r.recognize_google(
-                    audio_data=audio, language=self.source_lang)
+                recognized_text = self.r.recognize_whisper_api(
+                    audio_data=audio, 
+                    model="whisper-1",
+                    api_key=os.getenv('WHISPER_API_KEY')
+                )
                 self.channel.basic_publish(
                     exchange='', routing_key='speech_to_text_stream', body=recognized_text)
                 print(recognized_text)
 
             except sr.UnknownValueError as e:
-                print(
-                    f"Google Speech Recognition could not understand audio; {e}")
                 self.reconnect()
 
             except sr.RequestError as e:
-                print(
-                    f"Could not request results from Google Speech Recognition service; {e}")
                 self.reconnect()
 
         self.start()
 
     def reconnect(self):
         
         # if self.connection.is_open:
```

### Comparing `aij-1.1.2/src/webcam/__init__.py` & `aij-1.1.3/src/webcam/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.2/src/webcam2/__init__.py` & `aij-1.1.3/src/webcam2/__init__.py`

 * *Files identical despite different names*

