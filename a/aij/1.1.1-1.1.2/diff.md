# Comparing `tmp/aij-1.1.1.tar.gz` & `tmp/aij-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aij-1.1.1.tar", last modified: Thu May 25 22:44:45 2023, max compression
+gzip compressed data, was "aij-1.1.2.tar", last modified: Thu May 25 22:50:54 2023, max compression
```

## Comparing `aij-1.1.1.tar` & `aij-1.1.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 22:44:45.742538 aij-1.1.1/
--rw-rw-rw-   0        0        0     1100 2023-05-21 18:35:40.000000 aij-1.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0    30052 2023-05-25 22:44:45.742538 aij-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0    27745 2023-05-21 18:35:40.000000 aij-1.1.1/README.md
--rw-rw-rw-   0        0        0     6939 2023-05-25 22:44:32.000000 aij-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-25 22:44:45.743542 aij-1.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-25 22:44:45.679369 aij-1.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-25 22:44:45.718998 aij-1.1.1/src/aij.egg-info/
--rw-rw-rw-   0        0        0    30052 2023-05-25 22:44:45.000000 aij-1.1.1/src/aij.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      553 2023-05-25 22:44:45.000000 aij-1.1.1/src/aij.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 22:44:45.000000 aij-1.1.1/src/aij.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      197 2023-05-25 22:44:45.000000 aij-1.1.1/src/aij.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      491 2023-05-25 22:44:45.000000 aij-1.1.1/src/aij.egg-info/requires.txt
--rw-rw-rw-   0        0        0      105 2023-05-25 22:44:45.000000 aij-1.1.1/src/aij.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-25 22:44:45.720001 aij-1.1.1/src/animation/
--rw-rw-rw-   0        0        0     5739 2023-05-25 21:36:22.000000 aij-1.1.1/src/animation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 22:44:45.722001 aij-1.1.1/src/chat/
--rw-rw-rw-   0        0        0      680 2023-05-21 20:35:30.000000 aij-1.1.1/src/chat/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 22:44:45.723000 aij-1.1.1/src/download/
--rw-rw-rw-   0        0        0     8301 2023-05-24 21:25:22.000000 aij-1.1.1/src/download/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 22:44:45.724998 aij-1.1.1/src/face/
--rw-rw-rw-   0        0        0     8295 2023-05-25 16:52:45.000000 aij-1.1.1/src/face/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 22:44:45.726000 aij-1.1.1/src/intro/
--rw-rw-rw-   0        0        0     4532 2023-05-24 21:19:40.000000 aij-1.1.1/src/intro/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 22:44:45.726997 aij-1.1.1/src/messaging/
--rw-rw-rw-   0        0        0     5060 2023-05-23 19:12:37.000000 aij-1.1.1/src/messaging/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 22:44:45.728514 aij-1.1.1/src/news/
--rw-rw-rw-   0        0        0    10270 2023-05-25 21:21:31.000000 aij-1.1.1/src/news/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 22:44:45.730529 aij-1.1.1/src/setup/
--rw-rw-rw-   0        0        0     3925 2023-05-24 22:31:30.000000 aij-1.1.1/src/setup/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 22:44:45.731525 aij-1.1.1/src/stream/
--rw-rw-rw-   0        0        0     1093 2023-05-24 23:06:34.000000 aij-1.1.1/src/stream/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 22:44:45.734529 aij-1.1.1/src/transcribe/
--rw-rw-rw-   0        0        0     2215 2023-05-25 21:10:13.000000 aij-1.1.1/src/transcribe/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 22:44:45.735527 aij-1.1.1/src/translate/
--rw-rw-rw-   0        0        0     2393 2023-05-25 21:47:13.000000 aij-1.1.1/src/translate/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 22:44:45.737537 aij-1.1.1/src/voice/
--rw-rw-rw-   0        0        0     2332 2023-05-25 22:34:55.000000 aij-1.1.1/src/voice/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 22:44:45.738544 aij-1.1.1/src/webcam/
--rw-rw-rw-   0        0        0    18706 2023-05-24 23:40:36.000000 aij-1.1.1/src/webcam/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 22:44:45.740536 aij-1.1.1/src/webcam2/
--rw-rw-rw-   0        0        0     3351 2023-05-25 22:17:56.000000 aij-1.1.1/src/webcam2/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 22:50:54.896662 aij-1.1.2/
+-rw-rw-rw-   0        0        0     1100 2023-05-21 18:35:40.000000 aij-1.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0    30052 2023-05-25 22:50:54.894589 aij-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0    27745 2023-05-21 18:35:40.000000 aij-1.1.2/README.md
+-rw-rw-rw-   0        0        0     6993 2023-05-25 22:50:44.000000 aij-1.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-25 22:50:54.897688 aij-1.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-25 22:50:54.831571 aij-1.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-25 22:50:54.870575 aij-1.1.2/src/aij.egg-info/
+-rw-rw-rw-   0        0        0    30052 2023-05-25 22:50:54.000000 aij-1.1.2/src/aij.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      553 2023-05-25 22:50:54.000000 aij-1.1.2/src/aij.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 22:50:54.000000 aij-1.1.2/src/aij.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      247 2023-05-25 22:50:54.000000 aij-1.1.2/src/aij.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      491 2023-05-25 22:50:54.000000 aij-1.1.2/src/aij.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      105 2023-05-25 22:50:54.000000 aij-1.1.2/src/aij.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-25 22:50:54.871578 aij-1.1.2/src/animation/
+-rw-rw-rw-   0        0        0     5739 2023-05-25 21:36:22.000000 aij-1.1.2/src/animation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 22:50:54.872579 aij-1.1.2/src/chat/
+-rw-rw-rw-   0        0        0      680 2023-05-21 20:35:30.000000 aij-1.1.2/src/chat/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 22:50:54.875107 aij-1.1.2/src/download/
+-rw-rw-rw-   0        0        0     8301 2023-05-24 21:25:22.000000 aij-1.1.2/src/download/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 22:50:54.876112 aij-1.1.2/src/face/
+-rw-rw-rw-   0        0        0     8295 2023-05-25 16:52:45.000000 aij-1.1.2/src/face/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 22:50:54.878107 aij-1.1.2/src/intro/
+-rw-rw-rw-   0        0        0     4532 2023-05-24 21:19:40.000000 aij-1.1.2/src/intro/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 22:50:54.881138 aij-1.1.2/src/messaging/
+-rw-rw-rw-   0        0        0     5060 2023-05-23 19:12:37.000000 aij-1.1.2/src/messaging/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 22:50:54.882128 aij-1.1.2/src/news/
+-rw-rw-rw-   0        0        0    10270 2023-05-25 21:21:31.000000 aij-1.1.2/src/news/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 22:50:54.884126 aij-1.1.2/src/setup/
+-rw-rw-rw-   0        0        0     3925 2023-05-24 22:31:30.000000 aij-1.1.2/src/setup/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 22:50:54.885127 aij-1.1.2/src/stream/
+-rw-rw-rw-   0        0        0     1093 2023-05-24 23:06:34.000000 aij-1.1.2/src/stream/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 22:50:54.887127 aij-1.1.2/src/transcribe/
+-rw-rw-rw-   0        0        0     2215 2023-05-25 21:10:13.000000 aij-1.1.2/src/transcribe/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 22:50:54.888128 aij-1.1.2/src/translate/
+-rw-rw-rw-   0        0        0     2393 2023-05-25 21:47:13.000000 aij-1.1.2/src/translate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 22:50:54.890127 aij-1.1.2/src/voice/
+-rw-rw-rw-   0        0        0     2332 2023-05-25 22:34:55.000000 aij-1.1.2/src/voice/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 22:50:54.891128 aij-1.1.2/src/webcam/
+-rw-rw-rw-   0        0        0    18706 2023-05-24 23:40:36.000000 aij-1.1.2/src/webcam/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 22:50:54.893358 aij-1.1.2/src/webcam2/
+-rw-rw-rw-   0        0        0     3351 2023-05-25 22:17:56.000000 aij-1.1.2/src/webcam2/__init__.py
```

### Comparing `aij-1.1.1/LICENSE.txt` & `aij-1.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aij-1.1.1/PKG-INFO` & `aij-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij
-Version: 1.1.1
+Version: 1.1.2
 Summary: AI Journalist
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-1.1.1/README.md` & `aij-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `aij-1.1.1/pyproject.toml` & `aij-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "aij"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.1.01"
+version = "1.1.02"
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "AI Journalist"  # Optional
 
 # This is an optional longer description of your project that represents
@@ -174,16 +174,18 @@
 "Say Thanks!" = "http://saythanks.io/to/aij"
 "Source" = "https://github.com/codesapienbe/aij"
 
 # The following would provide a command line executable called `sample`
 # which executes the function `main` from this package when invoked.
 [project.scripts]  # Optional
 aij = "webcam:main"
+aij2 = "webcam2:main"
 aijnews = "news:main"
 aijintro = "intro:main"
+aijtranslate = "translate:main"
 aijtranscribe = "transcribe:main"
 aijchat = "chat:main"
 aijtube = "download:main"
 aijinit = "setup:main"
 aijvoice = "voice:main"
 
 # This is configuration specific to the `setuptools` build backend.
```

### Comparing `aij-1.1.1/src/aij.egg-info/PKG-INFO` & `aij-1.1.2/src/aij.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij
-Version: 1.1.1
+Version: 1.1.2
 Summary: AI Journalist
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-1.1.1/src/aij.egg-info/SOURCES.txt` & `aij-1.1.2/src/aij.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aij-1.1.1/src/animation/__init__.py` & `aij-1.1.2/src/animation/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.1/src/chat/__init__.py` & `aij-1.1.2/src/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.1/src/download/__init__.py` & `aij-1.1.2/src/download/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.1/src/face/__init__.py` & `aij-1.1.2/src/face/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.1/src/intro/__init__.py` & `aij-1.1.2/src/intro/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.1/src/messaging/__init__.py` & `aij-1.1.2/src/messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.1/src/news/__init__.py` & `aij-1.1.2/src/news/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.1/src/setup/__init__.py` & `aij-1.1.2/src/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.1/src/stream/__init__.py` & `aij-1.1.2/src/stream/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.1/src/transcribe/__init__.py` & `aij-1.1.2/src/transcribe/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.1/src/translate/__init__.py` & `aij-1.1.2/src/translate/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.1/src/voice/__init__.py` & `aij-1.1.2/src/voice/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.1/src/webcam/__init__.py` & `aij-1.1.2/src/webcam/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.1/src/webcam2/__init__.py` & `aij-1.1.2/src/webcam2/__init__.py`

 * *Files identical despite different names*

