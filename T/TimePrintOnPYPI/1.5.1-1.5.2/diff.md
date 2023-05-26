# Comparing `tmp/TimePrintOnPYPI-1.5.1.tar.gz` & `tmp/TimePrintOnPYPI-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TimePrintOnPYPI-1.5.1.tar", last modified: Fri May 26 15:20:40 2023, max compression
+gzip compressed data, was "TimePrintOnPYPI-1.5.2.tar", last modified: Fri May 26 15:30:35 2023, max compression
```

## Comparing `TimePrintOnPYPI-1.5.1.tar` & `TimePrintOnPYPI-1.5.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 15:20:40.947131 TimePrintOnPYPI-1.5.1/
--rw-rw-rw-   0        0        0     4611 2023-05-26 15:20:40.946135 TimePrintOnPYPI-1.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     4121 2023-05-26 15:19:49.000000 TimePrintOnPYPI-1.5.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 15:20:40.925088 TimePrintOnPYPI-1.5.1/TimePrint/
--rw-rw-rw-   0        0        0     1722 2023-05-26 15:19:57.000000 TimePrintOnPYPI-1.5.1/TimePrint/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 15:20:40.944137 TimePrintOnPYPI-1.5.1/TimePrintOnPYPI.egg-info/
--rw-rw-rw-   0        0        0     4611 2023-05-26 15:20:40.000000 TimePrintOnPYPI-1.5.1/TimePrintOnPYPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      196 2023-05-26 15:20:40.000000 TimePrintOnPYPI-1.5.1/TimePrintOnPYPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 15:20:40.000000 TimePrintOnPYPI-1.5.1/TimePrintOnPYPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-26 15:20:40.000000 TimePrintOnPYPI-1.5.1/TimePrintOnPYPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-26 15:20:40.947131 TimePrintOnPYPI-1.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1013 2023-05-26 15:20:27.000000 TimePrintOnPYPI-1.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 15:30:35.135335 TimePrintOnPYPI-1.5.2/
+-rw-rw-rw-   0        0        0     4611 2023-05-26 15:30:35.135335 TimePrintOnPYPI-1.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4121 2023-05-26 15:19:49.000000 TimePrintOnPYPI-1.5.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 15:30:35.114717 TimePrintOnPYPI-1.5.2/TimePrint/
+-rw-rw-rw-   0        0        0     1744 2023-05-26 15:30:10.000000 TimePrintOnPYPI-1.5.2/TimePrint/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 15:30:35.132237 TimePrintOnPYPI-1.5.2/TimePrintOnPYPI.egg-info/
+-rw-rw-rw-   0        0        0     4611 2023-05-26 15:30:35.000000 TimePrintOnPYPI-1.5.2/TimePrintOnPYPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      196 2023-05-26 15:30:35.000000 TimePrintOnPYPI-1.5.2/TimePrintOnPYPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 15:30:35.000000 TimePrintOnPYPI-1.5.2/TimePrintOnPYPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-26 15:30:35.000000 TimePrintOnPYPI-1.5.2/TimePrintOnPYPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 15:30:35.136334 TimePrintOnPYPI-1.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     1013 2023-05-26 15:30:17.000000 TimePrintOnPYPI-1.5.2/setup.py
```

### Comparing `TimePrintOnPYPI-1.5.1/PKG-INFO` & `TimePrintOnPYPI-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TimePrintOnPYPI
-Version: 1.5.1
+Version: 1.5.2
 Summary: A package for printing text with time delay between characters
 Home-page: https://github.com/SForces/TimePrint
 Author: Osman TUNA
 Author-email: osmntn08@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `TimePrintOnPYPI-1.5.1/README.md` & `TimePrintOnPYPI-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `TimePrintOnPYPI-1.5.1/TimePrint/__init__.py` & `TimePrintOnPYPI-1.5.2/TimePrint/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,18 +14,23 @@
         sys.stdout.write(character)
         sys.stdout.flush()
         time.sleep(int(seconds)/len(text))
     print("")
 def P(text:str):
     """
     Usage;
+
     TimePrint.P("text")
-    Example TimePrint.P("Hello") writes
+
+    For Example: TimePrint.P("Hello") Writes
+
     Hello in 0.001 seconds
+
     You can use this for just
+
     write effect.
     
     """
     for character in text:
         sys.stdout.write(character)
         sys.stdout.flush()
         time.sleep(0.001)
@@ -36,19 +41,21 @@
     print("        | |    | | | \  / | |__      | |__) | |__) | | | |  \| |  | |   ")
     print("        | |    | | | |\/| |  __|     |  ___/|  _  /  | | | . ` |  | |   ")
     print("        | |   _| |_| |  | | |____    | |    | | \ \ _| |_| |\  |  | |   ")
     print("        |_|  |_____|_|  |_|______|   |_|    |_|  \_\_____|_| \_|  |_|   ")
     print("\nAuthor: Osman TUNA")
     print("Author Email: osmntn08@gmail.com")
     print("Project Page: https://github.com/SForces/TimePrint")
-    print("Version: 1.5.1")
+    print("Version: 1.5.2")
 def Timetag(format: str):
     """
     Example Usages;
 
     "%H:%M" Returns --> 12:56 = (Hours:Minutes)
-    "%H:%M:%S" Returns --> 12:56:24 = (Hours:Minutes:Seconds)
-    "%d.%m.%y" Returns --> 10.02.2023 = (Day.Month.Year)
 
+    "%H:%M:%S" Returns --> 12:56:24 = (Hours:Minutes:Seconds) 
+
+    "%d.%m.%y" Returns --> 10.02.2023 = (Day.Month.Year)
+    
     using strftime from time
     """
-    return time.strftime(format, time.localtime())
+    return time.strftime(format, time.localtime())
```

### Comparing `TimePrintOnPYPI-1.5.1/TimePrintOnPYPI.egg-info/PKG-INFO` & `TimePrintOnPYPI-1.5.2/TimePrintOnPYPI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TimePrintOnPYPI
-Version: 1.5.1
+Version: 1.5.2
 Summary: A package for printing text with time delay between characters
 Home-page: https://github.com/SForces/TimePrint
 Author: Osman TUNA
 Author-email: osmntn08@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `TimePrintOnPYPI-1.5.1/setup.py` & `TimePrintOnPYPI-1.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         print("Need Help ? Contact Me From e-mail: osmntn08@gmail.com")
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='TimePrintOnPYPI',
-    version='1.5.1',
+    version='1.5.2',
     description='A package for printing text with time delay between characters',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/SForces/TimePrint',
     author='Osman TUNA',
     author_email='osmntn08@gmail.com',
     license='MIT',
```

