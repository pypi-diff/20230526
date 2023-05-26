# Comparing `tmp/CGOL-0.9.3.tar.gz` & `tmp/CGOL-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CGOL-0.9.3.tar", last modified: Wed Jan  4 17:04:34 2023, max compression
+gzip compressed data, was "CGOL-0.9.4.tar", last modified: Fri May 26 18:50:32 2023, max compression
```

## Comparing `CGOL-0.9.3.tar` & `CGOL-0.9.4.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 neido     (1000) neido     (1000)        0 2023-01-04 17:04:34.516486 CGOL-0.9.3/
--rw-r--r--   0 neido     (1000) neido     (1000)    35149 2022-12-31 13:18:27.000000 CGOL-0.9.3/LICENSE
--rw-r--r--   0 neido     (1000) neido     (1000)     5629 2023-01-04 17:04:34.516486 CGOL-0.9.3/PKG-INFO
--rw-r--r--   0 neido     (1000) neido     (1000)     4822 2023-01-04 17:00:48.000000 CGOL-0.9.3/README.md
--rw-r--r--   0 neido     (1000) neido     (1000)      972 2023-01-04 17:04:13.000000 CGOL-0.9.3/pyproject.toml
--rw-r--r--   0 neido     (1000) neido     (1000)       38 2023-01-04 17:04:34.516486 CGOL-0.9.3/setup.cfg
-drwxr-xr-x   0 neido     (1000) neido     (1000)        0 2023-01-04 17:04:34.513153 CGOL-0.9.3/src/
-drwxr-xr-x   0 neido     (1000) neido     (1000)        0 2023-01-04 17:04:34.513153 CGOL-0.9.3/src/CGOL.egg-info/
--rw-r--r--   0 neido     (1000) neido     (1000)     5629 2023-01-04 17:04:34.000000 CGOL-0.9.3/src/CGOL.egg-info/PKG-INFO
--rw-r--r--   0 neido     (1000) neido     (1000)      340 2023-01-04 17:04:34.000000 CGOL-0.9.3/src/CGOL.egg-info/SOURCES.txt
--rw-r--r--   0 neido     (1000) neido     (1000)        1 2023-01-04 17:04:34.000000 CGOL-0.9.3/src/CGOL.egg-info/dependency_links.txt
--rw-r--r--   0 neido     (1000) neido     (1000)       44 2023-01-04 17:04:34.000000 CGOL-0.9.3/src/CGOL.egg-info/entry_points.txt
--rw-r--r--   0 neido     (1000) neido     (1000)       13 2023-01-04 17:04:34.000000 CGOL-0.9.3/src/CGOL.egg-info/requires.txt
--rw-r--r--   0 neido     (1000) neido     (1000)        9 2023-01-04 17:04:34.000000 CGOL-0.9.3/src/CGOL.egg-info/top_level.txt
-drwxr-xr-x   0 neido     (1000) neido     (1000)        0 2023-01-04 17:04:34.513153 CGOL-0.9.3/src/cgol/
--rw-r--r--   0 neido     (1000) neido     (1000)      196 2023-01-04 16:46:39.000000 CGOL-0.9.3/src/cgol/__init__.py
--rw-r--r--   0 neido     (1000) neido     (1000)       81 2023-01-02 21:45:14.000000 CGOL-0.9.3/src/cgol/__main__.py
--rw-r--r--   0 neido     (1000) neido     (1000)    15780 2023-01-04 16:46:45.000000 CGOL-0.9.3/src/cgol/game.py
--rw-r--r--   0 neido     (1000) neido     (1000)     7856 2023-01-04 09:13:02.000000 CGOL-0.9.3/src/cgol/parser.py
--rw-r--r--   0 neido     (1000) neido     (1000)     5888 2023-01-04 16:45:10.000000 CGOL-0.9.3/src/cgol/utils.py
--rw-r--r--   0 neido     (1000) neido     (1000)    10940 2023-01-04 08:57:09.000000 CGOL-0.9.3/src/cgol/world.py
+drwxr-xr-x   0 neido     (1000) neido     (1000)        0 2023-05-26 18:50:32.717456 CGOL-0.9.4/
+-rw-r--r--   0 neido     (1000) neido     (1000)    35149 2023-05-26 18:45:16.000000 CGOL-0.9.4/LICENSE
+-rw-r--r--   0 neido     (1000) neido     (1000)     5626 2023-05-26 18:50:32.714123 CGOL-0.9.4/PKG-INFO
+-rw-r--r--   0 neido     (1000) neido     (1000)     4819 2023-05-26 18:45:32.000000 CGOL-0.9.4/README.md
+-rw-r--r--   0 neido     (1000) neido     (1000)     1025 2023-05-26 18:50:19.000000 CGOL-0.9.4/pyproject.toml
+-rw-r--r--   0 neido     (1000) neido     (1000)       38 2023-05-26 18:50:32.717456 CGOL-0.9.4/setup.cfg
+drwxr-xr-x   0 neido     (1000) neido     (1000)        0 2023-05-26 18:50:32.714123 CGOL-0.9.4/src/
+drwxr-xr-x   0 neido     (1000) neido     (1000)        0 2023-05-26 18:50:32.714123 CGOL-0.9.4/src/CGOL.egg-info/
+-rw-r--r--   0 neido     (1000) neido     (1000)     5626 2023-05-26 18:50:32.000000 CGOL-0.9.4/src/CGOL.egg-info/PKG-INFO
+-rw-r--r--   0 neido     (1000) neido     (1000)      358 2023-05-26 18:50:32.000000 CGOL-0.9.4/src/CGOL.egg-info/SOURCES.txt
+-rw-r--r--   0 neido     (1000) neido     (1000)        1 2023-05-26 18:50:32.000000 CGOL-0.9.4/src/CGOL.egg-info/dependency_links.txt
+-rw-r--r--   0 neido     (1000) neido     (1000)       44 2023-05-26 18:50:32.000000 CGOL-0.9.4/src/CGOL.egg-info/entry_points.txt
+-rw-r--r--   0 neido     (1000) neido     (1000)       13 2023-05-26 18:50:32.000000 CGOL-0.9.4/src/CGOL.egg-info/requires.txt
+-rw-r--r--   0 neido     (1000) neido     (1000)        5 2023-05-26 18:50:32.000000 CGOL-0.9.4/src/CGOL.egg-info/top_level.txt
+drwxr-xr-x   0 neido     (1000) neido     (1000)        0 2023-05-26 18:50:32.714123 CGOL-0.9.4/src/cgol/
+-rw-r--r--   0 neido     (1000) neido     (1000)      196 2023-05-26 18:45:16.000000 CGOL-0.9.4/src/cgol/__init__.py
+-rw-r--r--   0 neido     (1000) neido     (1000)       81 2023-05-26 18:45:16.000000 CGOL-0.9.4/src/cgol/__main__.py
+-rw-r--r--   0 neido     (1000) neido     (1000)    15834 2023-05-26 18:46:52.000000 CGOL-0.9.4/src/cgol/game.py
+-rw-r--r--   0 neido     (1000) neido     (1000)     6162 2023-05-26 18:46:02.000000 CGOL-0.9.4/src/cgol/icon.png
+-rw-r--r--   0 neido     (1000) neido     (1000)     7856 2023-05-26 18:45:16.000000 CGOL-0.9.4/src/cgol/parser.py
+-rw-r--r--   0 neido     (1000) neido     (1000)     5888 2023-05-26 18:45:16.000000 CGOL-0.9.4/src/cgol/utils.py
+-rw-r--r--   0 neido     (1000) neido     (1000)    10940 2023-05-26 18:45:16.000000 CGOL-0.9.4/src/cgol/world.py
```

### Comparing `CGOL-0.9.3/LICENSE` & `CGOL-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `CGOL-0.9.3/PKG-INFO` & `CGOL-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CGOL
-Version: 0.9.3
+Version: 0.9.4
 Summary: A whack Conway's Game of Life implementation.
 Author-email: Neido <reg@neido.de>
 Maintainer-email: Neido <reg@neido.de>
 License: GPL-3
 Project-URL: Homepage, https://github.com/INeido/CGOL/
 Project-URL: Repository, https://github.com/INeido/CGOL/
 Project-URL: Issues, https://github.com/INeido/CGOL/issues
@@ -23,17 +23,17 @@
 
 A Conway's Game of Life implementation using numpy and pygame.
 
 ![](https://github.com/INeido/CGOL/blob/main/samples/logo.png?raw=true)
 
 ## Description
 
-This project has no particular aim. It is a purely a personal project and barely maintained.
+This project has no particular aim. It is a purely personal project and barely maintained.
 
-It is a CLI based [Conway's Game of Life](https://en.wikipedia.org/wiki/Conway%27s_Game_of_Life): implementation using numpy for fast calculations and pygame for an interactive simulation.
+It is a CLI based [Conway's Game of Life](https://en.wikipedia.org/wiki/Conway%27s_Game_of_Life) implementation using numpy for fast calculations and pygame for an interactive simulation.
 
 No Hashlife or Quicklife algorithm support (yet).
 
 ---
 
 Rules of Conway's Game of Life
 1. Any live cell with two or three live neighbors survives.
```

### Comparing `CGOL-0.9.3/README.md` & `CGOL-0.9.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 A Conway's Game of Life implementation using numpy and pygame.
 
 ![](https://github.com/INeido/CGOL/blob/main/samples/logo.png?raw=true)
 
 ## Description
 
-This project has no particular aim. It is a purely a personal project and barely maintained.
+This project has no particular aim. It is a purely personal project and barely maintained.
 
-It is a CLI based [Conway's Game of Life](https://en.wikipedia.org/wiki/Conway%27s_Game_of_Life): implementation using numpy for fast calculations and pygame for an interactive simulation.
+It is a CLI based [Conway's Game of Life](https://en.wikipedia.org/wiki/Conway%27s_Game_of_Life) implementation using numpy for fast calculations and pygame for an interactive simulation.
 
 No Hashlife or Quicklife algorithm support (yet).
 
 ---
 
 Rules of Conway's Game of Life
 1. Any live cell with two or three live neighbors survives.
```

### Comparing `CGOL-0.9.3/pyproject.toml` & `CGOL-0.9.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "CGOL"
-version = "0.9.3"
+version = "0.9.4"
 description = "A whack Conway's Game of Life implementation."
 readme = "README.md"
 requires-python = ">=3"
 license = {text = "GPL-3"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "Development Status :: 4 - Beta",
@@ -31,8 +31,11 @@
 
 [project.urls]
 Homepage = "https://github.com/INeido/CGOL/"
 Repository = "https://github.com/INeido/CGOL/"
 Issues = "https://github.com/INeido/CGOL/issues"
 
 [project.scripts]
-cgol = "cgol.__main__:main"
+cgol = "cgol.__main__:main"
+
+[tool.setuptools.package-data]
+cgol = ["icon.png"]
```

### Comparing `CGOL-0.9.3/src/CGOL.egg-info/PKG-INFO` & `CGOL-0.9.4/src/CGOL.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CGOL
-Version: 0.9.3
+Version: 0.9.4
 Summary: A whack Conway's Game of Life implementation.
 Author-email: Neido <reg@neido.de>
 Maintainer-email: Neido <reg@neido.de>
 License: GPL-3
 Project-URL: Homepage, https://github.com/INeido/CGOL/
 Project-URL: Repository, https://github.com/INeido/CGOL/
 Project-URL: Issues, https://github.com/INeido/CGOL/issues
@@ -23,17 +23,17 @@
 
 A Conway's Game of Life implementation using numpy and pygame.
 
 ![](https://github.com/INeido/CGOL/blob/main/samples/logo.png?raw=true)
 
 ## Description
 
-This project has no particular aim. It is a purely a personal project and barely maintained.
+This project has no particular aim. It is a purely personal project and barely maintained.
 
-It is a CLI based [Conway's Game of Life](https://en.wikipedia.org/wiki/Conway%27s_Game_of_Life): implementation using numpy for fast calculations and pygame for an interactive simulation.
+It is a CLI based [Conway's Game of Life](https://en.wikipedia.org/wiki/Conway%27s_Game_of_Life) implementation using numpy for fast calculations and pygame for an interactive simulation.
 
 No Hashlife or Quicklife algorithm support (yet).
 
 ---
 
 Rules of Conway's Game of Life
 1. Any live cell with two or three live neighbors survives.
```

### Comparing `CGOL-0.9.3/src/cgol/game.py` & `CGOL-0.9.4/src/cgol/game.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 Github Repo:
 https://github.com/INeido/CGOL
 """
 from .world import *
 from .utils import *
 from .parser import *
+import pkg_resources
 import pygame
 import numpy
 
 
 class Game:
     """Game
     ====
@@ -74,15 +75,15 @@
         self.get_borders()
 
     def setup_pygame(self, rw, rh) -> None:
         """Creates and configures pygame instance.
         """
         pygame.init()
         pygame.display.set_caption("CGOL", "CGOL")
-        icon = pygame.image.load('src/img/icon.png')
+        icon = pygame.image.load(pkg_resources.resource_filename("cgol", "icon.png"))
         pygame.display.set_icon(icon)
         self.dis = pygame.display.set_mode((rw, rh), pygame.RESIZABLE, 8,)
         self.clock = pygame.time.Clock()
 
     def get_borders(self) -> None:
         """Determines the visible edges of the grid based on the current viewport.
```

### Comparing `CGOL-0.9.3/src/cgol/parser.py` & `CGOL-0.9.4/src/cgol/parser.py`

 * *Files identical despite different names*

### Comparing `CGOL-0.9.3/src/cgol/utils.py` & `CGOL-0.9.4/src/cgol/utils.py`

 * *Files identical despite different names*

### Comparing `CGOL-0.9.3/src/cgol/world.py` & `CGOL-0.9.4/src/cgol/world.py`

 * *Files identical despite different names*

