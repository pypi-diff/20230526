# Comparing `tmp/gwaves-0.0.3-py3-none-any.whl.zip` & `tmp/gwaves-0.0.3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 6291 bytes, number of entries: 7
+Zip file size: 6318 bytes, number of entries: 7
 -rw-rw-r--  2.0 unx       50 b- defN 22-Dec-10 03:00 gwaves/__init__.py
 -rw-rw-r--  2.0 unx     7883 b- defN 22-Dec-10 03:00 gwaves/gwaves_.py
--rw-rw-r--  2.0 unx     1067 b- defN 23-May-26 03:25 gwaves-0.0.3.dist-info/LICENSE
--rw-rw-r--  2.0 unx     5638 b- defN 23-May-26 03:25 gwaves-0.0.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-26 03:25 gwaves-0.0.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-May-26 03:25 gwaves-0.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      527 b- defN 23-May-26 03:25 gwaves-0.0.3.dist-info/RECORD
-7 files, 15264 bytes uncompressed, 5359 bytes compressed:  64.9%
+-rw-rw-r--  2.0 unx     1067 b- defN 23-May-26 03:29 gwaves-0.0.3.1.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     5643 b- defN 23-May-26 03:29 gwaves-0.0.3.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-26 03:29 gwaves-0.0.3.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-May-26 03:29 gwaves-0.0.3.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      537 b- defN 23-May-26 03:29 gwaves-0.0.3.1.dist-info/RECORD
+7 files, 15279 bytes uncompressed, 5366 bytes compressed:  64.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: gwaves/__init__.py
 Comment: 
 
 Filename: gwaves/gwaves_.py
 Comment: 
 
-Filename: gwaves-0.0.3.dist-info/LICENSE
+Filename: gwaves-0.0.3.1.dist-info/LICENSE
 Comment: 
 
-Filename: gwaves-0.0.3.dist-info/METADATA
+Filename: gwaves-0.0.3.1.dist-info/METADATA
 Comment: 
 
-Filename: gwaves-0.0.3.dist-info/WHEEL
+Filename: gwaves-0.0.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: gwaves-0.0.3.dist-info/top_level.txt
+Filename: gwaves-0.0.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: gwaves-0.0.3.dist-info/RECORD
+Filename: gwaves-0.0.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `gwaves-0.0.3.dist-info/LICENSE` & `gwaves-0.0.3.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `gwaves-0.0.3.dist-info/METADATA` & `gwaves-0.0.3.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwaves
-Version: 0.0.3
+Version: 0.0.3.1
 Summary: Library for getting music in high quality from YouTube
 Home-page: https://github.com/perseu912/gwaves
 Author: Reinan Br
 Author-email: slimchatuba@gmail.com
 License: MIT License
 Keywords: kit tools dev works
 Description-Content-Type: text/markdown
@@ -27,16 +27,19 @@
 <img alt="CodeFactor Grade" src="https://img.shields.io/codefactor/grade/github/reinanbr/gwaves?logo=codefactor"><img alt="Code Climate maintainability" src="https://img.shields.io/codeclimate/maintainability-percentage/reinanbr/dreams"><img alt="GitHub Pipenv locked Python version" src="https://img.shields.io/github/pipenv/locked/python-version/reinanbr/gwaves">
 <br/>
 <a href='https://pypi.org/project/dreams/'><img src='https://img.shields.io/pypi/v/gwaves'></a><img alt="PyPI - License" src="https://img.shields.io/pypi/l/gwaves?color=b"><a href="https://doi.org/10.5281/zenodo.7966690"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.7966690.svg" alt="DOI"></a>
 
 <hr>
 
 
+
 </div>
+
 ## installing:
+
 ```sh
 pip3 install gwaves -U
 ```
 
 ## importing
 ```py
 import gwaves as gw
```

### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: gwaves Version: 0.0.3 Summary: Library for getting
-music in high quality from YouTube Home-page: https://github.com/perseu912/
-gwaves Author: Reinan Br Author-email: slimchatuba@gmail.com License: MIT
-License Keywords: kit tools dev works Description-Content-Type: text/markdown
-License-File: LICENSE Requires-Dist: scipy Requires-Dist: requests Requires-
-Dist: pandas Requires-Dist: bs4 Requires-Dist: h5py Requires-Dist: matplotlib
-Requires-Dist: numpy Requires-Dist: soundfile Requires-Dist: astropy Requires-
-Dist: openpyxl Requires-Dist: lxml
+Metadata-Version: 2.1 Name: gwaves Version: 0.0.3.1 Summary: Library for
+getting music in high quality from YouTube Home-page: https://github.com/
+perseu912/gwaves Author: Reinan Br Author-email: slimchatuba@gmail.com License:
+MIT License Keywords: kit tools dev works Description-Content-Type: text/
+markdown License-File: LICENSE Requires-Dist: scipy Requires-Dist: requests
+Requires-Dist: pandas Requires-Dist: bs4 Requires-Dist: h5py Requires-Dist:
+matplotlib Requires-Dist: numpy Requires-Dist: soundfile Requires-Dist: astropy
+Requires-Dist: openpyxl Requires-Dist: lxml
                              ****** gwaves ******
              A python lib for works with gravitational waves data
  [CodeFactor Grade][Code Climate maintainability][GitHub Pipenv locked Python
                                    version]
          [https://img.shields.io/pypi/v/gwaves][PyPI - License][DOI]
 ===============================================================================
 ## installing: ```sh pip3 install gwaves -U ``` ## importing ```py import
```

