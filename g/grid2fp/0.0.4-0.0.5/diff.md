# Comparing `tmp/grid2fp-0.0.4.tar.gz` & `tmp/grid2fp-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grid2fp-0.0.4.tar", last modified: Thu May 25 20:19:04 2023, max compression
+gzip compressed data, was "grid2fp-0.0.5.tar", last modified: Fri May 26 15:24:38 2023, max compression
```

## Comparing `grid2fp-0.0.4.tar` & `grid2fp-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:19:04.602119 grid2fp-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-25 20:18:33.000000 grid2fp-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-25 20:19:04.602119 grid2fp-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-25 20:18:33.000000 grid2fp-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:19:04.602119 grid2fp-0.0.4/grid2fp/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-25 20:18:33.000000 grid2fp-0.0.4/grid2fp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-05-25 20:18:33.000000 grid2fp-0.0.4/grid2fp/grid2fp.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-25 20:18:33.000000 grid2fp-0.0.4/grid2fp/grid_segment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:19:04.602119 grid2fp-0.0.4/grid2fp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-25 20:19:04.000000 grid2fp-0.0.4/grid2fp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-25 20:19:04.000000 grid2fp-0.0.4/grid2fp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 20:19:04.000000 grid2fp-0.0.4/grid2fp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-25 20:19:04.000000 grid2fp-0.0.4/grid2fp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-25 20:19:04.000000 grid2fp-0.0.4/grid2fp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 20:19:04.602119 grid2fp-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-25 20:18:33.000000 grid2fp-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:19:04.602119 grid2fp-0.0.4/test/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-25 20:18:33.000000 grid2fp-0.0.4/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-25 20:18:33.000000 grid2fp-0.0.4/test/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:24:38.847999 grid2fp-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-26 15:24:05.000000 grid2fp-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-05-26 15:24:38.847999 grid2fp-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-26 15:24:05.000000 grid2fp-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:24:38.847999 grid2fp-0.0.5/grid2fp/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-26 15:24:05.000000 grid2fp-0.0.5/grid2fp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-05-26 15:24:05.000000 grid2fp-0.0.5/grid2fp/grid2fp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-26 15:24:05.000000 grid2fp-0.0.5/grid2fp/grid_segment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:24:38.847999 grid2fp-0.0.5/grid2fp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-05-26 15:24:38.000000 grid2fp-0.0.5/grid2fp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-26 15:24:38.000000 grid2fp-0.0.5/grid2fp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:24:38.000000 grid2fp-0.0.5/grid2fp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-26 15:24:38.000000 grid2fp-0.0.5/grid2fp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-26 15:24:38.000000 grid2fp-0.0.5/grid2fp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 15:24:38.847999 grid2fp-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-26 15:24:05.000000 grid2fp-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:24:38.847999 grid2fp-0.0.5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-26 15:24:05.000000 grid2fp-0.0.5/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-26 15:24:05.000000 grid2fp-0.0.5/test/test_integration.py
```

### Comparing `grid2fp-0.0.4/LICENSE` & `grid2fp-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `grid2fp-0.0.4/grid2fp/grid2fp.py` & `grid2fp-0.0.5/grid2fp/grid2fp.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,15 +10,23 @@
 from grid2fp.grid_segment import grid_segment
 
 
 class grid2fp:
     """The grid2fp class."""
 
     def __init__(
-        self, csv_file=None, diagram=None, eccentricity=0.9, scale=10, out_file=None
+        self,
+        csv_file=None,
+        diagram=None,
+        eccentricity=0.9,
+        scale=10,
+        out_file=None,
+        draw_crossings=True,
+        string_color="black",
+        crossing_color="white",
     ) -> None:
         """Init for the grid2fp object.
 
         Parameters
         ----------
         csv_file : str, optional
             The location of grid diagram as csv, by default None
@@ -39,14 +47,17 @@
                 reader = csv.reader(csvfile)
                 for row in reader:
                     self.diagram.append(row)
 
         if diagram:
             self.diagram = diagram
         self.eccentricity = eccentricity
+        self.draw_crossings = draw_crossings
+        self.string_color = string_color
+        self.crossing_color = crossing_color
         self.scale = scale
         self.segments = []
         self.__get_segments()
         if out_file:
             d = self.draw()
             d.save_svg(out_file)
 
@@ -61,95 +72,101 @@
             the y coord
 
         Returns
         -------
         tuple
             rotated cord as tuple
         """
-        r = math.sqrt(2) / 2
-        return ((x * r - y * r) * self.scale, (x * r + y * r) * self.scale)
+        r = 1 / math.sqrt(2)
+        return (-x * r - y * r) * self.scale, (-x * r + y * r) * self.scale
 
     def __get_segments(self):
         """Parse the grid for segments."""
-        self.segments = []
         self.segments.extend(self.__get_segments_horizontal())
         self.segments.extend(self.__get_segments_vertical())
-        # Get horizontal
 
     def __get_segments_horizontal(self):
         """Parse the grid for horizontal segments.
 
         Returns
         -------
         grid_segment
             The segment.
         """
         segments = []
-        dlen = len(self.diagram)
         for i, row in enumerate(self.diagram):
             seg = None
             for j, c in enumerate(row):
                 if c.strip() != "":
                     if seg is None:
                         seg = grid_segment()
                     if c.strip().lower() == "x":
-                        seg.sink = self.__rotate(dlen - j, i)
+                        seg.sink = (j, i)
                     if c.strip().lower() == "o":
-                        seg.source = self.__rotate(dlen - j, i)
+                        seg.source = (j, i)
             if seg is not None:
                 segments.append(seg)
         return segments
 
     def __get_segments_vertical(self):
         """Parse the grid for vertical segments.
 
         Returns
         -------
         grid_segment
             The segment.
         """
         segments = []
-        dlen = len(self.diagram)
-        # Get vertical
         for j, c in enumerate(self.diagram[0]):
             seg = None
             for i, row in enumerate(self.diagram):
                 if row[j].strip() != "":
                     if seg is None:
                         seg = grid_segment()
                     if row[j].strip().lower() == "x":
-                        seg.source = self.__rotate(dlen - j, i)
+                        seg.source = (j, i)
                     if row[j].strip().lower() == "o":
-                        seg.sink = self.__rotate(dlen - j, i)
+                        seg.sink = (j, i)
             if seg is not None:
                 segments.append(seg)
         return segments
 
     def __draw_segment(self, step):
         """Draws a segment of the front projection as a Bézier curve.
 
         Parameters
         ----------
         step : grid_segment
             The segment to draw.
 
         Returns
         -------
-        Path
-            The svg path segment.
+        Group
+            The svg path segments contained in a group.
         """
+        x, y = self.__rotate(step.source[0], step.source[1])
+        x2, y2 = self.__rotate(step.sink[0], step.sink[1])
+        delta_x = x2 - x
+        x_ctr1 = x + (self.eccentricity * delta_x)
+        x_ctr2 = x2 - (self.eccentricity * delta_x)
+        g = draw.Group()
+        if self.draw_crossings:
+            p = draw.Path(
+                stroke_width=0.2 * self.scale,
+                stroke=self.crossing_color,
+            )
+            p.M(x, y)
+            p.C(x_ctr1, y, x_ctr2, y2, x2, y2)
+            g.append(p)
         p = draw.Path()
-        p.M(step.source[0], step.source[1])
-        delta_x = step.sink[0] - step.source[0]
-        x_ctr1 = step.source[0] + (self.eccentricity * delta_x)
-        x_ctr2 = step.sink[0] - (self.eccentricity * delta_x)
-        y_ctr1 = step.source[1]
-        y_ctr2 = step.sink[1]
-        p.C(x_ctr1, y_ctr1, x_ctr2, y_ctr2, step.sink[0], step.sink[1])
-        return p
+        p.M(x, y)
+        p.C(x_ctr1, y, x_ctr2, y2, x2, y2)
+        g.append(p)
+
+        return g
 
     def draw(self, pixel_scale=2):
         """Draws the front projection of the given grid as an SVG.
 
         Parameters
         ----------
         pixel_scale : int, optional
@@ -168,17 +185,17 @@
                 self.scale * math.sqrt(2) * len(self.diagram[0]),
                 self.scale * math.sqrt(2) * len(self.diagram[0]),
                 origin=(0, 0),
                 id_prefix="d",
             )
             g = draw.Group(
                 stroke_width=0.1 * self.scale,
-                stroke="black",
+                stroke=self.string_color,
                 fill="none",
-                transform=f"translate({self.scale*len(self.diagram[0])/2},{0.1*self.scale})",
+                transform=f"translate({self.scale* math.sqrt(2)*len(self.diagram[0])},{self.scale* math.sqrt(2)*len(self.diagram[0])/2})",
             )
             for step in self.segments:
                 p = self.__draw_segment(step)
                 g.append(p)
             d.append(g)
 
             d.set_pixel_scale(pixel_scale)
```

### Comparing `grid2fp-0.0.4/setup.py` & `grid2fp-0.0.5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import logging
 
 logger = logging.getLogger(__name__)
 
-version = "0.0.4"
+version = "0.0.5"
 
 try:
     with open("README.md", "r") as f:
         long_desc = f.read()
 except:
     logger.warning("Could not open README.md.  long_description will be set to None.")
     long_desc = None
```

### Comparing `grid2fp-0.0.4/test/test_integration.py` & `grid2fp-0.0.5/test/test_integration.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,25 +15,26 @@
     """TODO: Update Testcase description."""
     grid2fp(csv_file=file_location / "un.csv", out_file=file_location / "un.svg")
     assert 1 == 1
 
 
 def test_random():
     """TODO: Update Testcase description."""
-    g = grid2fp(csv_file=file_location / "random.csv")
+    g = grid2fp(csv_file=file_location / "random.csv",string_color = "pink",
+        crossing_color="purple")
     d = g.draw()
     d.save_svg(file_location / "random.svg")
     assert 1 == 1
 
 
 def test_trefoil():
     g = grid2fp(csv_file=file_location / "trefoil.csv")
     d = g.draw()
     d.save_svg(file_location / "trefoil.svg")
     assert 1 == 1
 
 
-def test_trefoil():
+def test_fig1():
     g = grid2fp(csv_file=file_location / "fig1_from_paper.csv")
     d = g.draw()
     d.save_svg(file_location / "fig1_from_paper.svg")
     assert 1 == 1
```

