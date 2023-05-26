# Comparing `tmp/freyja_plot-0.2.0.tar.gz` & `tmp/freyja_plot-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freyja_plot-0.2.0.tar", max compression
+gzip compressed data, was "freyja_plot-0.3.0.tar", max compression
```

## Comparing `freyja_plot-0.2.0.tar` & `freyja_plot-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
--rwxr-xr-x   0        0        0     1065 2023-05-01 17:02:13.516327 freyja_plot-0.2.0/LICENSE
--rwxr-xr-x   0        0        0     6088 2023-05-16 20:41:59.765968 freyja_plot-0.2.0/README.md
--rwxr-xr-x   0        0        0     1004 2023-05-01 21:27:35.768186 freyja_plot-0.2.0/example/create_test_plots.py
--rwxr-xr-x   0        0        0  3598080 2023-05-01 18:11:39.770519 freyja_plot-0.2.0/example/example_images/batch_comparison_example.html
--rwxr-xr-x   0        0        0    39533 2023-05-01 20:24:24.676588 freyja_plot-0.2.0/example/example_images/batch_comparison_example.png
--rwxr-xr-x   0        0        0    51128 2023-05-01 21:08:17.397157 freyja_plot-0.2.0/example/example_images/batch_comparison_selection_example.png
--rwxr-xr-x   0        0        0    44892 2023-05-01 20:24:24.114256 freyja_plot-0.2.0/example/example_images/superlineage_example.png
--rwxr-xr-x   0        0        0    18144 2023-05-01 17:34:35.679310 freyja_plot-0.2.0/example/wastewater-freyja-aggregated.tsv
--rwxr-xr-x   0        0        0    30790 2023-05-01 17:46:00.523531 freyja_plot-0.2.0/example/wastewater-freyja-compare1.tsv
--rwxr-xr-x   0        0        0    23696 2023-05-01 17:46:24.707912 freyja_plot-0.2.0/example/wastewater-freyja-compare2.tsv
--rwxr-xr-x   0        0        0       96 2023-05-01 17:13:37.160319 freyja_plot-0.2.0/freyja_plot/__init__.py
--rwxr-xr-x   0        0        0    26782 2023-05-17 20:55:25.401722 freyja_plot-0.2.0/freyja_plot/freyja_plot.py
--rwxr-xr-x   0        0        0      543 2023-05-02 13:03:11.643983 freyja_plot-0.2.0/freyja_plot/main.py
--rwxr-xr-x   0        0        0       89 2023-05-01 17:14:03.847868 freyja_plot-0.2.0/freyja_plot/version.py
--rwxr-xr-x   0        0        0      678 2023-05-16 20:05:35.590367 freyja_plot-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6963 1970-01-01 00:00:00.000000 freyja_plot-0.2.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1065 2023-05-01 17:02:13.516327 freyja_plot-0.3.0/LICENSE
+-rwxr-xr-x   0        0        0     6088 2023-05-16 20:41:59.765968 freyja_plot-0.3.0/README.md
+-rwxr-xr-x   0        0        0     1004 2023-05-01 21:27:35.768186 freyja_plot-0.3.0/example/create_test_plots.py
+-rwxr-xr-x   0        0        0  3598080 2023-05-01 18:11:39.770519 freyja_plot-0.3.0/example/example_images/batch_comparison_example.html
+-rwxr-xr-x   0        0        0    39533 2023-05-01 20:24:24.676588 freyja_plot-0.3.0/example/example_images/batch_comparison_example.png
+-rwxr-xr-x   0        0        0    51128 2023-05-01 21:08:17.397157 freyja_plot-0.3.0/example/example_images/batch_comparison_selection_example.png
+-rwxr-xr-x   0        0        0    44892 2023-05-01 20:24:24.114256 freyja_plot-0.3.0/example/example_images/superlineage_example.png
+-rwxr-xr-x   0        0        0  3589836 2023-05-26 17:46:38.886774 freyja_plot-0.3.0/example/summarized_example.html
+-rwxr-xr-x   0        0        0  3604336 2023-05-26 17:46:39.685812 freyja_plot-0.3.0/example/superlineage_example.html
+-rwxr-xr-x   0        0        0    18144 2023-05-01 17:34:35.679310 freyja_plot-0.3.0/example/wastewater-freyja-aggregated.tsv
+-rwxr-xr-x   0        0        0    30790 2023-05-01 17:46:00.523531 freyja_plot-0.3.0/example/wastewater-freyja-compare1.tsv
+-rwxr-xr-x   0        0        0    23696 2023-05-01 17:46:24.707912 freyja_plot-0.3.0/example/wastewater-freyja-compare2.tsv
+-rwxr-xr-x   0        0        0       96 2023-05-01 17:13:37.160319 freyja_plot-0.3.0/freyja_plot/__init__.py
+-rwxr-xr-x   0        0        0    49759 2023-05-26 17:46:40.438003 freyja_plot-0.3.0/freyja_plot/freyja_plot.py
+-rwxr-xr-x   0        0        0      581 2023-05-26 17:46:40.453585 freyja_plot-0.3.0/freyja_plot/main.py
+-rwxr-xr-x   0        0        0       89 2023-05-01 17:14:03.847868 freyja_plot-0.3.0/freyja_plot/version.py
+-rwxr-xr-x   0        0        0      694 2023-05-26 17:54:32.825066 freyja_plot-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6998 1970-01-01 00:00:00.000000 freyja_plot-0.3.0/PKG-INFO
```

### Comparing `freyja_plot-0.2.0/LICENSE` & `freyja_plot-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `freyja_plot-0.2.0/README.md` & `freyja_plot-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `freyja_plot-0.2.0/example/create_test_plots.py` & `freyja_plot-0.3.0/example/create_test_plots.py`

 * *Files identical despite different names*

### Comparing `freyja_plot-0.2.0/example/example_images/batch_comparison_example.html` & `freyja_plot-0.3.0/example/example_images/batch_comparison_example.html`

 * *Files identical despite different names*

### Comparing `freyja_plot-0.2.0/example/example_images/batch_comparison_example.png` & `freyja_plot-0.3.0/example/example_images/batch_comparison_example.png`

 * *Files identical despite different names*

### Comparing `freyja_plot-0.2.0/example/example_images/batch_comparison_selection_example.png` & `freyja_plot-0.3.0/example/example_images/batch_comparison_selection_example.png`

 * *Files identical despite different names*

### Comparing `freyja_plot-0.2.0/example/example_images/superlineage_example.png` & `freyja_plot-0.3.0/example/example_images/superlineage_example.png`

 * *Files identical despite different names*

### Comparing `freyja_plot-0.2.0/example/wastewater-freyja-aggregated.tsv` & `freyja_plot-0.3.0/example/wastewater-freyja-aggregated.tsv`

 * *Files identical despite different names*

### Comparing `freyja_plot-0.2.0/example/wastewater-freyja-compare1.tsv` & `freyja_plot-0.3.0/example/wastewater-freyja-compare1.tsv`

 * *Files identical despite different names*

### Comparing `freyja_plot-0.2.0/example/wastewater-freyja-compare2.tsv` & `freyja_plot-0.3.0/example/wastewater-freyja-compare2.tsv`

 * *Files identical despite different names*

### Comparing `freyja_plot-0.2.0/freyja_plot/main.py` & `freyja_plot-0.3.0/freyja_plot/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,7 +6,10 @@
     parser = ArgumentParser(description=dedent("""
         A python module for plotting aggregated `freyja demix` lineage abundances. 
         `freyja_plot` is not currently set up for CLI, but conceivably could be in the future. 
         For now, it is best used as a module in a python script. 
     """))
     parser.add_argument('-V', '--version', action='version', version="%(prog)s ("+__version__+")")
     parser.parse_args()
+
+if __name__ == "__main__":
+    main()
```

### Comparing `freyja_plot-0.2.0/pyproject.toml` & `freyja_plot-0.3.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "freyja-plot"
-version = "0.2.0"
+version = "0.3.0"
 description = "Plotting lineage abundance for individual samples from aggregated freyja demix results"
 authors = ["Sam Kunkleman <skunklem@uncc.edu>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     {include = "freyja_plot"},
     {include = "example"}
@@ -13,14 +13,15 @@
 keywords = ["freyja","plot","lineage","abundance","covid"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pandas = "^2.0.1"
 plotly = "^5.14.1"
 kaleido = "0.1.0"
+pyyaml = "^6.0"
 
 [tool.poetry.scripts]
 freyja_plot = 'freyja_plot.main:main'
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `freyja_plot-0.2.0/PKG-INFO` & `freyja_plot-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freyja-plot
-Version: 0.2.0
+Version: 0.3.0
 Summary: Plotting lineage abundance for individual samples from aggregated freyja demix results
 Home-page: https://github.com/enviro-lab/freyja-plot.git
 License: MIT
 Keywords: freyja,plot,lineage,abundance,covid
 Author: Sam Kunkleman
 Author-email: skunklem@uncc.edu
 Requires-Python: >=3.8,<4.0
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: kaleido (==0.1.0)
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: plotly (>=5.14.1,<6.0.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
 Project-URL: Repository, https://github.com/enviro-lab/freyja-plot.git
 Description-Content-Type: text/markdown
 
 # freyja-plot
 Plotting lineage abundance for individual samples from aggregated freyja demix results
 
 ![Example Lineage Abundance Plot](example/example_images/batch_comparison_selection_example.png "These samples had some issues on plate1 or else the 'plate1' and 'plate2' versions of each sample would look more similar.")
```

