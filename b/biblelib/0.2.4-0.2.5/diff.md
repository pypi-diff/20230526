# Comparing `tmp/biblelib-0.2.4.tar.gz` & `tmp/biblelib-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biblelib-0.2.4.tar", max compression
+gzip compressed data, was "biblelib-0.2.5.tar", max compression
```

## Comparing `biblelib-0.2.4.tar` & `biblelib-0.2.5.tar`

### file list

```diff
@@ -1,12 +1,26 @@
--rw-r--r--   0        0        0     1069 2022-11-08 02:07:02.605762 biblelib-0.2.4/LICENSE
--rw-r--r--   0        0        0     1456 2023-02-22 20:32:41.129105 biblelib-0.2.4/README.md
--rw-r--r--   0        0        0      207 2022-11-11 00:55:36.561996 biblelib-0.2.4/biblelib/__init__.py
--rw-r--r--   0        0        0      351 2022-11-15 05:28:29.397816 biblelib-0.2.4/biblelib/books/__init__.py
--rw-r--r--   0        0        0    12572 2022-11-17 00:28:07.163981 biblelib-0.2.4/biblelib/books/books.py
--rw-r--r--   0        0        0     5680 2022-11-08 02:07:02.611067 biblelib-0.2.4/biblelib/books/books.tsv
--rw-r--r--   0        0        0      652 2023-02-22 20:40:42.788533 biblelib-0.2.4/biblelib/words/__init__.py
--rw-r--r--   0        0        0     5347 2023-02-22 20:39:04.876394 biblelib-0.2.4/biblelib/words/bcvwpid.py
--rw-r--r--   0        0        0     4432 2022-11-17 00:30:21.039343 biblelib-0.2.4/biblelib/words/mappings.py
--rw-r--r--   0        0        0     1189 2023-02-22 20:49:34.775196 biblelib-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     2147 1970-01-01 00:00:00.000000 biblelib-0.2.4/setup.py
--rw-r--r--   0        0        0     2251 1970-01-01 00:00:00.000000 biblelib-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     3326 2023-05-12 17:59:15.958698 biblelib-0.2.5/LICENSE.md
+-rw-r--r--   0        0        0     3337 2023-05-12 17:50:39.199097 biblelib-0.2.5/LICENSE.md~
+-rw-r--r--   0        0        0     2048 2023-05-12 17:45:43.797503 biblelib-0.2.5/README.md
+-rw-r--r--   0        0        0      207 2022-11-11 00:55:36.561996 biblelib-0.2.5/biblelib/__init__.py
+-rw-r--r--   0        0        0      946 2023-05-12 17:25:25.324552 biblelib-0.2.5/biblelib/book/ReadMe.md
+-rw-r--r--   0        0        0      350 2023-03-24 13:53:37.422750 biblelib-0.2.5/biblelib/book/__init__.py
+-rw-r--r--   0        0        0    12780 2023-04-22 23:14:16.335752 biblelib-0.2.5/biblelib/book/book.py
+-rw-r--r--   0        0        0     4755 2023-05-12 17:23:39.309175 biblelib-0.2.5/biblelib/book/books.tsv
+-rw-r--r--   0        0        0      474 2023-04-09 04:44:24.570950 biblelib-0.2.5/biblelib/unit/__init__.py
+-rw-r--r--   0        0        0     5788 2023-04-10 12:29:36.110427 biblelib-0.2.5/biblelib/unit/book.py
+-rw-r--r--   0        0        0     1770 2023-03-30 03:30:47.201892 biblelib-0.2.5/biblelib/unit/bookchapters.tsv
+-rw-r--r--   0        0        0     6972 2023-04-10 12:30:22.815665 biblelib-0.2.5/biblelib/unit/chapter.py
+-rw-r--r--   0        0        0     1770 2023-03-24 23:24:06.076120 biblelib-0.2.5/biblelib/unit/chapters.tsv
+-rw-r--r--   0        0        0    23363 2023-03-30 03:30:50.093429 biblelib-0.2.5/biblelib/unit/chapterverses.tsv
+-rw-r--r--   0        0        0    29962 2023-03-30 03:30:33.249866 biblelib-0.2.5/biblelib/unit/tempchapter.py
+-rw-r--r--   0        0        0     3332 2023-03-30 05:04:49.035453 biblelib-0.2.5/biblelib/unit/unit.py
+-rw-r--r--   0        0        0     1240 2023-03-24 18:41:28.150962 biblelib-0.2.5/biblelib/unit/verse.py
+-rw-r--r--   0        0        0     1348 2023-05-12 17:27:37.060726 biblelib-0.2.5/biblelib/versification/ReadMe.md
+-rw-r--r--   0        0        0   431827 2021-10-25 18:19:51.303000 biblelib-0.2.5/biblelib/versification/vref-bcv.txt
+-rw-r--r--   0        0        0   431827 2021-10-25 18:19:51.303000 biblelib-0.2.5/biblelib/versification/vref.txt
+-rw-r--r--   0        0        0      199 2023-05-08 18:22:24.370434 biblelib-0.2.5/biblelib/versification/vrefmap.py
+-rw-r--r--   0        0        0      734 2023-04-22 22:19:35.460574 biblelib-0.2.5/biblelib/word/__init__.py
+-rw-r--r--   0        0        0    15164 2023-05-26 17:58:56.202838 biblelib-0.2.5/biblelib/word/bcvwpid.py
+-rw-r--r--   0        0        0     4432 2022-11-17 00:30:21.039343 biblelib-0.2.5/biblelib/word/mappings.py
+-rw-r--r--   0        0        0     1189 2023-05-26 18:13:11.208830 biblelib-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     2843 1970-01-01 00:00:00.000000 biblelib-0.2.5/PKG-INFO
```

### Comparing `biblelib-0.2.4/biblelib/books/books.py` & `biblelib-0.2.5/biblelib/book/book.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,28 @@
 * (forthcoming) the canons that recognize this book, ordered
 * (forthcoming) the chapter contents of each book and their final
   verse. This is tradition-specific: Gen 31 has 55 verses in ESV, but
   54 in BHS.
 
 
 Examples:
-    >>> from biblelib import books
-    >>> allbooks = books.Books()
+    >>> from biblelib import book
+    >>> allbooks = book.Books()
     >>> allbooks["MRK"]
     <Book: MRK>
     >>> allbooks["MRK"].osisID
     'Mark'
     >>>
     # retrive a Book instance from an OSIS ID
     >>> allbooks.fromosis("Matt").name
     'Matthew'
+    # convert number from Logos scheme to USFM: Tobit should be 68,
+    # not 40
+    >>> allbooks.fromlogos("bible.40").usfmnumber
+    '68'
 
 See the tests `Biblelib/tests` for additional examples.
 
 To do:
 
     Add other canons: [Logos' Canon Comparison
     interactive](https://ref.ly/logosres/interactive:canon-comparison?pos=index.html)
@@ -239,14 +243,15 @@
             if logosID.startswith("bible."):
                 logosID = int(logosID[6:])
             else:
                 logosID = int(logosID)
         if not self.logosmap:
             # initialize on demand
             self.logosmap = {b.logosID: b for _, b in self.data.items()}
+        assert logosID in self.logosmap, f"Invalid logosID {logosID}"
         return self.logosmap[logosID]
 
     def fromosis(self, osisID: str) -> Book:
         """Return the book instance for an OSIS identifier.
 
         Args:
             osisID: the OSIS identifier to use in looking up the Book,
```

### Comparing `biblelib-0.2.4/biblelib/books/books.tsv` & `biblelib-0.2.5/biblelib/book/books.tsv`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,8 @@
 logosID	usfmnumber	usfmname	osisID	name	altname
-# Data from https://ubsicap.github.io/usfm/identification/books.html
-# - Logos Bible datatype number. This supports ordinal sorting
-#   according to Protestant canon order. Other orders need other support.
-# - USFM Number (but really a string)
-# - USFM Identifier
-# - OSIS ID
-# - 'standard' English Name
-# - Long English Name/Alternate names (delimited by '/')
-#
-# Numerous alternate names in other canons are not included
-# Order of items here must match properties in Book for loading to
-# work correctly
-#
-# Excluded by design:
-# - Different published Bibles have different names for books
-#   (e.g. 1SA is '1 Kings' in Douay-Rheims). So 'name' here is a
-#   conventional one: more data would be required to capture published
-#   names in other editions.
-# - Some Clear data has a two-letter abbreviation, perhaps originating
-#   with Andi Wu (Gen = 'gn', Lev = 'lx', etc. ). Non-normative so excluded
 1	1	GEN	Gen	Genesis
 2	2	EXO	Exod	Exodus
 3	3	LEV	Lev	Leviticus
 4	4	NUM	Num	Numbers
 5	5	DEU	Deut	Deuteronomy
 6	6	JOS	Josh	Joshua
 7	7	JDG	Judg	Judges
```

### Comparing `biblelib-0.2.4/biblelib/words/mappings.py` & `biblelib-0.2.5/biblelib/word/mappings.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.2.4/pyproject.toml` & `biblelib-0.2.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "biblelib"
-version = "0.2.4"
+version = "0.2.5"
 description = "Utilities for working with metadata for Bible books, references, pericopes, and other units."
 authors = ["Sean Boisen <sean.boisen@gmail.com>"]
 repository = "https://github.com/Clear-Bible/Biblelib/"
 # documentation = "https://sboisen.github.io/Biblelib/"
 readme = "README.md"
 packages = [
   {include = "biblelib"}
```

### Comparing `biblelib-0.2.4/setup.py` & `biblelib-0.2.5/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,36 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+# Biblelib
 
-packages = \
-['biblelib', 'biblelib.books', 'biblelib.words']
+[![Release](https://img.shields.io/github/v/release/Clear-Bible/Biblelib)](https://img.shields.io/github/v/release/Clear-Bible/Biblelib)
+[![Build status](https://img.shields.io/github/workflow/status/sboisen/Biblelib/merge-to-main)](https://img.shields.io/github/workflow/status/sboisen/Biblelib/merge-to-main)
+[![codecov](https://codecov.io/gh/sboisen/Biblelib/branch/main/graph/badge.svg)](https://codecov.io/gh/sboisen/Biblelib)
+[![Commit activity](https://img.shields.io/github/commit-activity/m/sboisen/Biblelib)](https://img.shields.io/github/commit-activity/m/sboisen/Biblelib)
+[![Docs](https://img.shields.io/badge/docs-gh--pages-blue)](https://sboisen.github.io/Biblelib/)
+[![Code style with black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Imports with isort](https://img.shields.io/badge/%20imports-isort-%231674b1)](https://pycqa.github.io/isort/)
+[![License](https://img.shields.io/github/license/sboisen/Biblelib)](https://img.shields.io/github/license/sboisen/Biblelib)
 
-package_data = \
-{'': ['*']}
+Utilities for working with Bible books, references, pericopes, and
+other units. Note this does _not_ include any actual Bible texts.
 
-setup_kwargs = {
-    'name': 'biblelib',
-    'version': '0.2.4',
-    'description': 'Utilities for working with metadata for Bible books, references, pericopes, and other units.',
-    'long_description': '# Biblelib\n\n[![Release](https://img.shields.io/github/v/release/sboisen/Biblelib)](https://img.shields.io/github/v/release/sboisen/Biblelib)\n[![Build status](https://img.shields.io/github/workflow/status/sboisen/Biblelib/merge-to-main)](https://img.shields.io/github/workflow/status/sboisen/Biblelib/merge-to-main)\n[![codecov](https://codecov.io/gh/sboisen/Biblelib/branch/main/graph/badge.svg)](https://codecov.io/gh/sboisen/Biblelib)\n[![Commit activity](https://img.shields.io/github/commit-activity/m/sboisen/Biblelib)](https://img.shields.io/github/commit-activity/m/sboisen/Biblelib)\n[![Docs](https://img.shields.io/badge/docs-gh--pages-blue)](https://sboisen.github.io/Biblelib/)\n[![Code style with black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Imports with isort](https://img.shields.io/badge/%20imports-isort-%231674b1)](https://pycqa.github.io/isort/)\n[![License](https://img.shields.io/github/license/sboisen/Biblelib)](https://img.shields.io/github/license/sboisen/Biblelib)\n\nUtilities for working with Bible books, references, pericopes, and\nother units. Note this does _not_ include any actual Bible texts.\n\n- **Github repository**: <https://github.com/Clear-Bible/Biblelib\n- **Documentation** may *eventually* arrive at\n  <https://clear-bible.github.io/Biblelib/> but can be found in the\n  `docs` directory, and built using `mkdocs`.\n\n## Installation\n\n```bash\n$ pip install biblelib\n```\n',
-    'author': 'Sean Boisen',
-    'author_email': 'sean.boisen@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/Clear-Bible/Biblelib/',
-    'packages': packages,
-    'package_data': package_data,
-    'python_requires': '>=3.8,<=3.11',
-}
+- **Github repository**: <https://github.com/Clear-Bible/Biblelib
+- **Documentation** may *eventually* arrive at
+  <https://clear-bible.github.io/Biblelib/> but can be found in the
+  `docs` directory, and built using `mkdocs`.
 
+## Installation
 
-setup(**setup_kwargs)
+```bash
+$ pip install biblelib
+```
+## Acknowledgements
+
+* Book abbreviations incorporate public conventions developed by
+    * [Unified Standard Format Markers
+      3.0.0](https://ubsicap.github.io/usfm/index.html) (USFM), which
+      is © Copyright 2018, United Bible Societies.
+    * [The Open Scripture Information Standard
+      (OSIS)](https://crosswire.org/osis/)
+    * [Logos Bible Software](http://www.logos.com/)
+* Versification information included consulting sources from:
+    * [The Copenhagen Alliance for Open Biblical Resources](http://copenhagen-alliance.org/)
+    * [Paratext](https://paratext.org/)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `biblelib-0.2.4/PKG-INFO` & `biblelib-0.2.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biblelib
-Version: 0.2.4
+Version: 0.2.5
 Summary: Utilities for working with metadata for Bible books, references, pericopes, and other units.
 Home-page: https://github.com/Clear-Bible/Biblelib/
 Author: Sean Boisen
 Author-email: sean.boisen@gmail.com
 Requires-Python: >=3.8,<=3.11
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Project-URL: Repository, https://github.com/Clear-Bible/Biblelib/
 Description-Content-Type: text/markdown
 
 # Biblelib
 
-[![Release](https://img.shields.io/github/v/release/sboisen/Biblelib)](https://img.shields.io/github/v/release/sboisen/Biblelib)
+[![Release](https://img.shields.io/github/v/release/Clear-Bible/Biblelib)](https://img.shields.io/github/v/release/Clear-Bible/Biblelib)
 [![Build status](https://img.shields.io/github/workflow/status/sboisen/Biblelib/merge-to-main)](https://img.shields.io/github/workflow/status/sboisen/Biblelib/merge-to-main)
 [![codecov](https://codecov.io/gh/sboisen/Biblelib/branch/main/graph/badge.svg)](https://codecov.io/gh/sboisen/Biblelib)
 [![Commit activity](https://img.shields.io/github/commit-activity/m/sboisen/Biblelib)](https://img.shields.io/github/commit-activity/m/sboisen/Biblelib)
 [![Docs](https://img.shields.io/badge/docs-gh--pages-blue)](https://sboisen.github.io/Biblelib/)
 [![Code style with black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports with isort](https://img.shields.io/badge/%20imports-isort-%231674b1)](https://pycqa.github.io/isort/)
 [![License](https://img.shields.io/github/license/sboisen/Biblelib)](https://img.shields.io/github/license/sboisen/Biblelib)
@@ -37,8 +37,20 @@
   `docs` directory, and built using `mkdocs`.
 
 ## Installation
 
 ```bash
 $ pip install biblelib
 ```
+## Acknowledgements
+
+* Book abbreviations incorporate public conventions developed by
+    * [Unified Standard Format Markers
+      3.0.0](https://ubsicap.github.io/usfm/index.html) (USFM), which
+      is © Copyright 2018, United Bible Societies.
+    * [The Open Scripture Information Standard
+      (OSIS)](https://crosswire.org/osis/)
+    * [Logos Bible Software](http://www.logos.com/)
+* Versification information included consulting sources from:
+    * [The Copenhagen Alliance for Open Biblical Resources](http://copenhagen-alliance.org/)
+    * [Paratext](https://paratext.org/)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

