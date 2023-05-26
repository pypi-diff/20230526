# Comparing `tmp/TimePrintOnPYPI-1.4.tar.gz` & `tmp/TimePrintOnPYPI-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TimePrintOnPYPI-1.4.tar", last modified: Thu May 25 21:04:59 2023, max compression
+gzip compressed data, was "TimePrintOnPYPI-1.5.tar", last modified: Fri May 26 15:03:03 2023, max compression
```

## Comparing `TimePrintOnPYPI-1.4.tar` & `TimePrintOnPYPI-1.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 21:04:59.578278 TimePrintOnPYPI-1.4/
--rw-rw-rw-   0        0        0     1262 2023-05-25 21:04:59.577278 TimePrintOnPYPI-1.4/PKG-INFO
--rw-rw-rw-   0        0        0      774 2023-05-25 21:04:36.000000 TimePrintOnPYPI-1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 21:04:59.560213 TimePrintOnPYPI-1.4/TimePrint/
--rw-rw-rw-   0        0        0     1685 2023-05-25 21:04:41.000000 TimePrintOnPYPI-1.4/TimePrint/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 21:04:59.574269 TimePrintOnPYPI-1.4/TimePrintOnPYPI.egg-info/
--rw-rw-rw-   0        0        0     1262 2023-05-25 21:04:59.000000 TimePrintOnPYPI-1.4/TimePrintOnPYPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      196 2023-05-25 21:04:59.000000 TimePrintOnPYPI-1.4/TimePrintOnPYPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 21:04:59.000000 TimePrintOnPYPI-1.4/TimePrintOnPYPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-25 21:04:59.000000 TimePrintOnPYPI-1.4/TimePrintOnPYPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-25 21:04:59.578278 TimePrintOnPYPI-1.4/setup.cfg
--rw-rw-rw-   0        0        0      733 2023-05-25 21:04:45.000000 TimePrintOnPYPI-1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 15:03:03.979627 TimePrintOnPYPI-1.5/
+-rw-rw-rw-   0        0        0     2407 2023-05-26 15:03:03.978623 TimePrintOnPYPI-1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1919 2023-05-26 15:02:00.000000 TimePrintOnPYPI-1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 15:03:03.952224 TimePrintOnPYPI-1.5/TimePrint/
+-rw-rw-rw-   0        0        0     1720 2023-05-26 15:02:48.000000 TimePrintOnPYPI-1.5/TimePrint/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 15:03:03.976360 TimePrintOnPYPI-1.5/TimePrintOnPYPI.egg-info/
+-rw-rw-rw-   0        0        0     2407 2023-05-26 15:03:03.000000 TimePrintOnPYPI-1.5/TimePrintOnPYPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      196 2023-05-26 15:03:03.000000 TimePrintOnPYPI-1.5/TimePrintOnPYPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 15:03:03.000000 TimePrintOnPYPI-1.5/TimePrintOnPYPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-26 15:03:03.000000 TimePrintOnPYPI-1.5/TimePrintOnPYPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 15:03:03.980623 TimePrintOnPYPI-1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1012 2023-05-26 15:02:34.000000 TimePrintOnPYPI-1.5/setup.py
```

### Comparing `TimePrintOnPYPI-1.4/TimePrint/__init__.py` & `TimePrintOnPYPI-1.5/TimePrint/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,54 @@
 import time
 import sys
-def TP(saniye: int, metin: str):
+def TP(seconds: int, text: str):
     """
     Usage;
+
     TimePrint.TP(seconds,"text")
-    Example TimePrint.TP(1,"Hello") 
+
+    Example: TimePrint.TP(1,"Hello")
     Writes Hello In 1 Seconds
 
     """
-    for karakter in metin:
-        sys.stdout.write(karakter)
+    for character in text:
+        sys.stdout.write(character)
         sys.stdout.flush()
-        time.sleep(int(saniye)/len(metin))
+        time.sleep(int(seconds)/len(text))
     print("")
-def P(metin:str):
+def P(text:str):
     """
     Usage;
     TimePrint.P("text")
     Example TimePrint.P("Hello") writes
     Hello in 0.001 seconds
     You can use this for just
     write effect.
     
     """
-    for karakter in metin:
-        sys.stdout.write(karakter)
+    for character in text:
+        sys.stdout.write(character)
         sys.stdout.flush()
         time.sleep(0.001)
     print("")    
 def info():
     print("      _______ _____ __  __ ______     _____  _____  _____ _   _ _______  ")
     print("     |__   __|_   _|  \/  |  ____|   |  __ \|  __ \|_   _| \ | |__   __| ")
     print("        | |    | | | \  / | |__      | |__) | |__) | | | |  \| |  | |   ")
     print("        | |    | | | |\/| |  __|     |  ___/|  _  /  | | | . ` |  | |   ")
     print("        | |   _| |_| |  | | |____    | |    | | \ \ _| |_| |\  |  | |   ")
     print("        |_|  |_____|_|  |_|______|   |_|    |_|  \_\_____|_| \_|  |_|   ")
     print("\nAuthor: Osman TUNA")
     print("Author Email: osmntn08@gmail.com")
     print("Project Page: https://github.com/SForces/TimePrint")
-    print("Version: 1.4")
-def timetag(format: str):
+    print("Version: 1.5")
+def Timetag(format: str):
     """
     Example Usages;
 
     "%H:%M" Returns --> 12:56 = (Hours:Minutes)
     "%H:%M:%S" Returns --> 12:56:24 = (Hours:Minutes:Seconds)
     "%d.%m.%y" Returns --> 10.02.2023 = (Day.Month.Year)
 
+    using strftime from time
     """
     return time.strftime(format, time.localtime())
```

