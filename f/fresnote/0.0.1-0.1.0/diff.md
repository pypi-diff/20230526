# Comparing `tmp/fresnote-0.0.1.tar.gz` & `tmp/fresnote-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fresnote-0.0.1.tar", last modified: Tue May 23 09:54:31 2023, max compression
+gzip compressed data, was "dist/fresnote-0.1.0.tar", last modified: Fri May 26 13:28:27 2023, max compression
```

## Comparing `fresnote-0.0.1.tar` & `fresnote-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 dkioroglou (545410601) gbiurko  (545410250)        0 2023-05-23 09:54:31.198454 fresnote-0.0.1/
--rw-r--r--   0 dkioroglou (545410601) gbiurko  (545410250)    20849 2023-05-19 08:57:52.000000 fresnote-0.0.1/LICENSE
--rw-r--r--   0 dkioroglou (545410601) gbiurko  (545410250)     1167 2023-05-23 09:54:31.198454 fresnote-0.0.1/PKG-INFO
--rw-r--r--   0 dkioroglou (545410601) gbiurko  (545410250)      525 2023-05-19 08:57:52.000000 fresnote-0.0.1/README.md
-drwxr-xr-x   0 dkioroglou (545410601) gbiurko  (545410250)        0 2023-05-23 09:54:31.198454 fresnote-0.0.1/fresnote.egg-info/
--rw-r--r--   0 dkioroglou (545410601) gbiurko  (545410250)     1167 2023-05-23 09:54:31.000000 fresnote-0.0.1/fresnote.egg-info/PKG-INFO
--rw-r--r--   0 dkioroglou (545410601) gbiurko  (545410250)      251 2023-05-23 09:54:31.000000 fresnote-0.0.1/fresnote.egg-info/SOURCES.txt
--rw-r--r--   0 dkioroglou (545410601) gbiurko  (545410250)        1 2023-05-23 09:54:31.000000 fresnote-0.0.1/fresnote.egg-info/dependency_links.txt
--rw-r--r--   0 dkioroglou (545410601) gbiurko  (545410250)       55 2023-05-23 09:54:31.000000 fresnote-0.0.1/fresnote.egg-info/entry_points.txt
--rw-r--r--   0 dkioroglou (545410601) gbiurko  (545410250)        1 2023-05-19 10:20:10.000000 fresnote-0.0.1/fresnote.egg-info/not-zip-safe
--rw-r--r--   0 dkioroglou (545410601) gbiurko  (545410250)       41 2023-05-23 09:54:31.000000 fresnote-0.0.1/fresnote.egg-info/requires.txt
--rw-r--r--   0 dkioroglou (545410601) gbiurko  (545410250)        1 2023-05-23 09:54:31.000000 fresnote-0.0.1/fresnote.egg-info/top_level.txt
--rw-r--r--   0 dkioroglou (545410601) gbiurko  (545410250)       38 2023-05-23 09:54:31.198454 fresnote-0.0.1/setup.cfg
--rw-r--r--   0 dkioroglou (545410601) gbiurko  (545410250)     1625 2023-05-23 09:53:18.000000 fresnote-0.0.1/setup.py
+drwxr-xr-x   0 dkioroglou (545410601) gbiurko  (545410250)        0 2023-05-26 13:28:27.143805 fresnote-0.1.0/
+-rw-r--r--   0 dkioroglou (545410601) gbiurko  (545410250)    20849 2023-05-19 08:57:52.000000 fresnote-0.1.0/LICENSE
+-rw-r--r--   0 dkioroglou (545410601) gbiurko  (545410250)     1429 2023-05-26 13:28:27.143805 fresnote-0.1.0/PKG-INFO
+-rw-r--r--   0 dkioroglou (545410601) gbiurko  (545410250)      787 2023-05-26 13:24:53.000000 fresnote-0.1.0/README.md
+drwxr-xr-x   0 dkioroglou (545410601) gbiurko  (545410250)        0 2023-05-26 13:28:27.143805 fresnote-0.1.0/fresnote.egg-info/
+-rw-r--r--   0 dkioroglou (545410601) gbiurko  (545410250)     1429 2023-05-26 13:28:27.000000 fresnote-0.1.0/fresnote.egg-info/PKG-INFO
+-rw-r--r--   0 dkioroglou (545410601) gbiurko  (545410250)      251 2023-05-26 13:28:27.000000 fresnote-0.1.0/fresnote.egg-info/SOURCES.txt
+-rw-r--r--   0 dkioroglou (545410601) gbiurko  (545410250)        1 2023-05-26 13:28:27.000000 fresnote-0.1.0/fresnote.egg-info/dependency_links.txt
+-rw-r--r--   0 dkioroglou (545410601) gbiurko  (545410250)       55 2023-05-26 13:28:27.000000 fresnote-0.1.0/fresnote.egg-info/entry_points.txt
+-rw-r--r--   0 dkioroglou (545410601) gbiurko  (545410250)        1 2023-05-23 10:17:59.000000 fresnote-0.1.0/fresnote.egg-info/not-zip-safe
+-rw-r--r--   0 dkioroglou (545410601) gbiurko  (545410250)       41 2023-05-26 13:28:27.000000 fresnote-0.1.0/fresnote.egg-info/requires.txt
+-rw-r--r--   0 dkioroglou (545410601) gbiurko  (545410250)        1 2023-05-26 13:28:27.000000 fresnote-0.1.0/fresnote.egg-info/top_level.txt
+-rw-r--r--   0 dkioroglou (545410601) gbiurko  (545410250)       38 2023-05-26 13:28:27.143805 fresnote-0.1.0/setup.cfg
+-rw-r--r--   0 dkioroglou (545410601) gbiurko  (545410250)     1625 2023-05-26 13:28:15.000000 fresnote-0.1.0/setup.py
```

### Comparing `fresnote-0.0.1/LICENSE` & `fresnote-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fresnote-0.0.1/PKG-INFO` & `fresnote-0.1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fresnote
-Version: 0.0.1
+Version: 0.1.0
 Summary: Flask based notebook for personal and research projects.
 Home-page: UNKNOWN
 Author: Dimitrios Kioroglou
 Author-email: <d.kioroglou@hotmail.com>
 License: CC-BY-NC-SA-4.0
 Keywords: flask,notebook,research,reporting
 Platform: UNKNOWN
@@ -14,19 +14,23 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-# fresnote
-**F**lask **RES**earch **NOTE**book
+# Flask RESearch NOTEbook
 
 Shield: [![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]
 
+**Fresnote** is a browser-based note-taking application that uses Flask as a backend and Boostrap as a front-end. It is suitable for managing personal and research projects by assisting in the organization of the results and the analytical pipeline in a modular manner.
+
+
+# License
+
 This work is licensed under a
 [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].
 
 [![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]
 
 [cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
 [cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
```

### Comparing `fresnote-0.0.1/fresnote.egg-info/PKG-INFO` & `fresnote-0.1.0/fresnote.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fresnote
-Version: 0.0.1
+Version: 0.1.0
 Summary: Flask based notebook for personal and research projects.
 Home-page: UNKNOWN
 Author: Dimitrios Kioroglou
 Author-email: <d.kioroglou@hotmail.com>
 License: CC-BY-NC-SA-4.0
 Keywords: flask,notebook,research,reporting
 Platform: UNKNOWN
@@ -14,19 +14,23 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-# fresnote
-**F**lask **RES**earch **NOTE**book
+# Flask RESearch NOTEbook
 
 Shield: [![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]
 
+**Fresnote** is a browser-based note-taking application that uses Flask as a backend and Boostrap as a front-end. It is suitable for managing personal and research projects by assisting in the organization of the results and the analytical pipeline in a modular manner.
+
+
+# License
+
 This work is licensed under a
 [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].
 
 [![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]
 
 [cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
 [cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
```

### Comparing `fresnote-0.0.1/setup.py` & `fresnote-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         return contents.read()
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.1.0'
 DESCRIPTION = 'Flask based notebook for personal and research projects.'
 LONG_DESCRIPTION = 'A Flask-based notebook for managing and sharing personal and research projects.'
 
 # Setting up
 setup(
     name="fresnote",
     version=VERSION,
```

