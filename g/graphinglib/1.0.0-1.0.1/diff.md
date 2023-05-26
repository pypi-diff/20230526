# Comparing `tmp/graphinglib-1.0.0.tar.gz` & `tmp/graphinglib-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphinglib-1.0.0.tar", max compression
+gzip compressed data, was "graphinglib-1.0.1.tar", max compression
```

## Comparing `graphinglib-1.0.0.tar` & `graphinglib-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1068 2023-05-25 00:22:48.960531 graphinglib-1.0.0/LICENSE
--rw-r--r--   0        0        0     3453 2023-05-25 00:22:48.960531 graphinglib-1.0.0/README.md
--rw-r--r--   0        0        0      420 2023-05-25 00:22:48.968531 graphinglib-1.0.0/graphinglib/__init__.py
--rw-r--r--   0        0        0     9254 2023-05-25 00:22:48.968531 graphinglib-1.0.0/graphinglib/data_plotting_1d.py
--rw-r--r--   0        0        0     2911 2023-05-25 00:22:48.968531 graphinglib-1.0.0/graphinglib/data_plotting_2d.py
--rw-r--r--   0        0        0     2005 2023-05-25 00:22:48.972531 graphinglib-1.0.0/graphinglib/default_styles/horrible.yml
--rw-r--r--   0        0        0     1893 2023-05-25 00:22:48.972531 graphinglib-1.0.0/graphinglib/default_styles/plain.yml
--rw-r--r--   0        0        0     6959 2023-05-25 00:22:48.972531 graphinglib-1.0.0/graphinglib/figure.py
--rw-r--r--   0        0        0      441 2023-05-25 00:22:48.972531 graphinglib-1.0.0/graphinglib/file_manager.py
--rw-r--r--   0        0        0    16464 2023-05-25 00:22:48.972531 graphinglib-1.0.0/graphinglib/fits.py
--rw-r--r--   0        0        0     8962 2023-05-25 00:22:48.972531 graphinglib-1.0.0/graphinglib/graph_elements.py
--rw-r--r--   0        0        0     3651 2023-05-25 00:22:48.972531 graphinglib-1.0.0/graphinglib/legend_artists.py
--rw-r--r--   0        0        0      527 2023-05-25 00:22:48.972531 graphinglib-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4065 1970-01-01 00:00:00.000000 graphinglib-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-26 15:00:41.736563 graphinglib-1.0.1/LICENSE
+-rw-r--r--   0        0        0     3506 2023-05-26 15:00:41.736563 graphinglib-1.0.1/README.md
+-rw-r--r--   0        0        0      420 2023-05-26 15:00:41.748564 graphinglib-1.0.1/graphinglib/__init__.py
+-rw-r--r--   0        0        0     9322 2023-05-26 15:00:41.748564 graphinglib-1.0.1/graphinglib/data_plotting_1d.py
+-rw-r--r--   0        0        0     2911 2023-05-26 15:00:41.748564 graphinglib-1.0.1/graphinglib/data_plotting_2d.py
+-rw-r--r--   0        0        0     2065 2023-05-26 15:00:41.748564 graphinglib-1.0.1/graphinglib/default_styles/horrible.yml
+-rw-r--r--   0        0        0     1955 2023-05-26 15:00:41.748564 graphinglib-1.0.1/graphinglib/default_styles/plain.yml
+-rw-r--r--   0        0        0     6959 2023-05-26 15:00:41.748564 graphinglib-1.0.1/graphinglib/figure.py
+-rw-r--r--   0        0        0      441 2023-05-26 15:00:41.748564 graphinglib-1.0.1/graphinglib/file_manager.py
+-rw-r--r--   0        0        0    16464 2023-05-26 15:00:41.748564 graphinglib-1.0.1/graphinglib/fits.py
+-rw-r--r--   0        0        0     9673 2023-05-26 15:00:41.748564 graphinglib-1.0.1/graphinglib/graph_elements.py
+-rw-r--r--   0        0        0     3651 2023-05-26 15:00:41.748564 graphinglib-1.0.1/graphinglib/legend_artists.py
+-rw-r--r--   0        0        0      578 2023-05-26 15:00:41.748564 graphinglib-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4151 1970-01-01 00:00:00.000000 graphinglib-1.0.1/PKG-INFO
```

### Comparing `graphinglib-1.0.0/LICENSE` & `graphinglib-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `graphinglib-1.0.0/README.md` & `graphinglib-1.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,20 @@
 
 GraphingLib is an object oriented library combining the functionalities of Matplotlib and Scipy. With this library it is possible to create scientific graphs to visualise data while fitting the data with simple, single-line commmands.
 
 GraphingLib also provides the ability to create multiple predefined themes for different applications. Once those themes are specified, they can be applied to figures with a one-word parameter.
 
 ## 2. Installation
 
+From PyPI with
+
+```text
+pip install graphinglib
+```
+
 From source with
 
 ```text
 pip install git+https://github.com/GraphingLib/GraphingLib.git
 ```
 
 ## 3. Quick usage
```

### Comparing `graphinglib-1.0.0/graphinglib/data_plotting_1d.py` & `graphinglib-1.0.1/graphinglib/data_plotting_1d.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,16 +53,16 @@
     ) -> Self:
         x_data = np.linspace(x_min, x_max, number_of_points)
         y_data = func(x_data)
         return cls(x_data, y_data, label, color, line_width, line_style)
 
     def add_errorbars(
         self,
-        x_error: ArrayLike,
-        y_error: ArrayLike,
+        x_error: Optional[ArrayLike] = None,
+        y_error: Optional[ArrayLike] = None,
         cap_width: float = "default",
         errorbars_color: str = "default",
         errorbars_line_width: float = "default",
         cap_thickness: float = "default",
     ) -> None:
         self.errorbars = True
         self.x_error = x_error
@@ -129,16 +129,16 @@
         y_data = func(x_data)
         return cls(
             x_data, y_data, label, face_color, edge_color, marker_size, marker_style
         )
 
     def add_errorbars(
         self,
-        x_error: ArrayLike,
-        y_error: ArrayLike,
+        x_error: Optional[ArrayLike] = None,
+        y_error: Optional[ArrayLike] = None,
         cap_width: float = "default",
         errorbars_color: str = "default",
         errorbars_line_width: float = "default",
         cap_thickness: float = "default",
     ) -> None:
         self.errorbars = True
         self.x_error = x_error
```

### Comparing `graphinglib-1.0.0/graphinglib/data_plotting_2d.py` & `graphinglib-1.0.1/graphinglib/data_plotting_2d.py`

 * *Files identical despite different names*

### Comparing `graphinglib-1.0.0/graphinglib/default_styles/horrible.yml` & `graphinglib-1.0.1/graphinglib/default_styles/horrible.yml`

 * *Files 5% similar despite different names*

```diff
@@ -119,7 +119,12 @@
   res_line_width: 1
   res_line_style: "--"
 
 Heatmap:
   aspect_ratio: "equal"
   origin_position: "lower"
   color_map: "prism"
+
+Text:
+  color: "orange"
+  h_align: "right"
+  v_align: "top"
```

### Comparing `graphinglib-1.0.0/graphinglib/default_styles/plain.yml` & `graphinglib-1.0.1/graphinglib/default_styles/plain.yml`

 * *Files 6% similar despite different names*

```diff
@@ -113,8 +113,13 @@
   color: "r"
   line_width: 1
   line_style: "-"
 
 Heatmap:
   aspect_ratio: "equal"
   origin_position: "upper"
-  color_map: "coolwarm"
+  color_map: "coolwarm"
+
+Text:
+  color: "k"
+  h_align: "center"
+  v_align: "baseline"
```

### Comparing `graphinglib-1.0.0/graphinglib/figure.py` & `graphinglib-1.0.1/graphinglib/figure.py`

 * *Files identical despite different names*

### Comparing `graphinglib-1.0.0/graphinglib/fits.py` & `graphinglib-1.0.1/graphinglib/fits.py`

 * *Files identical despite different names*

### Comparing `graphinglib-1.0.0/graphinglib/graph_elements.py` & `graphinglib-1.0.1/graphinglib/graph_elements.py`

 * *Files 7% similar despite different names*

```diff
@@ -197,29 +197,50 @@
         self._show_coordinates = True
         self.text_color = text_color
         self.font_size = font_size
         self.h_align = h_align
         self.v_align = v_align
 
     def _plot_element(self, axes: plt.Axes, z_order: int) -> None:
+        size = self.font_size if self.font_size != "same as figure" else None
+        prefix = " " if self.h_align == "left" else ""
+        postfix = " " if self.h_align == "right" else ""
+        point_label = prefix + self.label + postfix
         axes.scatter(
             self.x,
             self.y,
             c=self.color,
             edgecolors=self.edge_color,
             s=self.marker_size,
             marker=self.marker_style,
             linewidths=self.line_width,
             zorder=z_order,
         )
+        axes.annotate(
+            point_label,
+            (self.x, self.y),
+            color=self.text_color,
+            fontsize=size,
+            horizontalalignment=self.h_align,
+            verticalalignment=self.v_align,
+            zorder=z_order,
+        )
         if self._show_coordinates:
-            size = self.font_size if self.font_size != "same as figure" else None
             prefix = " " if self.h_align == "left" else ""
             postfix = " " if self.h_align == "right" else ""
-            point_label = prefix + f"({self.x:.3f}, {self.y:.3f})" + postfix
+            if self.label is not None:
+                point_label = (
+                    prefix
+                    + self.label
+                    + " : "
+                    + f"({self.x:.3f}, {self.y:.3f})"
+                    + postfix
+                )
+            else:
+                point_label = prefix + f"({self.x:.3f}, {self.y:.3f})" + postfix
             axes.annotate(
                 point_label,
                 (self.x, self.y),
                 color=self.text_color,
                 fontsize=size,
                 horizontalalignment=self.h_align,
                 verticalalignment=self.v_align,
```

### Comparing `graphinglib-1.0.0/graphinglib/legend_artists.py` & `graphinglib-1.0.1/graphinglib/legend_artists.py`

 * *Files identical despite different names*

### Comparing `graphinglib-1.0.0/pyproject.toml` & `graphinglib-1.0.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "graphinglib"
-version = "1.0.0"
+version = "1.0.1"
 description = "An object oriented wrapper combining the functionalities of Matplotlib and Scipy"
 license = "MIT"
-authors = ["Gustave Coulombe", "Yannick Lapointe"]
+authors = ["Gustave Coulombe <magikgus@gmail.com>", "Yannick Lapointe <yannicklapointe77@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 numpy = "^1.24.2"
 scipy = "^1.10.1"
 matplotlib = "^3.7.1"
```

### Comparing `graphinglib-1.0.0/PKG-INFO` & `graphinglib-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: graphinglib
-Version: 1.0.0
+Version: 1.0.1
 Summary: An object oriented wrapper combining the functionalities of Matplotlib and Scipy
 License: MIT
 Author: Gustave Coulombe
+Author-email: magikgus@gmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
@@ -23,14 +24,20 @@
 
 GraphingLib is an object oriented library combining the functionalities of Matplotlib and Scipy. With this library it is possible to create scientific graphs to visualise data while fitting the data with simple, single-line commmands.
 
 GraphingLib also provides the ability to create multiple predefined themes for different applications. Once those themes are specified, they can be applied to figures with a one-word parameter.
 
 ## 2. Installation
 
+From PyPI with
+
+```text
+pip install graphinglib
+```
+
 From source with
 
 ```text
 pip install git+https://github.com/GraphingLib/GraphingLib.git
 ```
 
 ## 3. Quick usage
```

