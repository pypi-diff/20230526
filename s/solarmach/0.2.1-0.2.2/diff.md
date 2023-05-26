# Comparing `tmp/solarmach-0.2.1.tar.gz` & `tmp/solarmach-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/gieseler/uni/serpentine/solarmach/dist/.tmp-lhamsoxp/solarmach-0.2.1.tar", last modified: Fri May 12 08:06:14 2023, max compression
+gzip compressed data, was "solarmach-0.2.2.tar", last modified: Fri May 26 10:24:46 2023, max compression
```

## Comparing `solarmach-0.2.1.tar` & `solarmach-0.2.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-12 08:06:14.629089 solarmach-0.2.1/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1478 2022-03-14 11:21:13.000000 solarmach-0.2.1/LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      457 2022-01-10 16:26:49.000000 solarmach-0.2.1/MANIFEST.in
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     6117 2023-05-12 08:06:14.629089 solarmach-0.2.1/PKG-INFO
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     5268 2023-04-27 13:45:25.000000 solarmach-0.2.1/README.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     3370 2022-03-30 15:50:45.000000 solarmach-0.2.1/code_of_conduct.md
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-12 08:06:14.617089 solarmach-0.2.1/docs/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      634 2022-01-10 16:26:49.000000 solarmach-0.2.1/docs/Makefile
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2300 2022-03-14 11:55:52.000000 solarmach-0.2.1/docs/conf.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      300 2022-03-14 11:56:45.000000 solarmach-0.2.1/docs/index.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      760 2022-01-10 16:26:49.000000 solarmach-0.2.1/docs/make.bat
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-12 08:06:14.621089 solarmach-0.2.1/examples/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)  1915936 2023-04-27 13:41:04.000000 solarmach-0.2.1/examples/example.ipynb
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   348683 2022-03-14 16:09:27.000000 solarmach-0.2.1/examples/solarmach.png
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-12 08:06:14.625089 solarmach-0.2.1/licenses/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1478 2022-03-14 11:21:13.000000 solarmach-0.2.1/licenses/LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1659 2022-01-10 16:26:49.000000 solarmach-0.2.1/licenses/TEMPLATE_LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      134 2022-01-10 16:26:49.000000 solarmach-0.2.1/pyproject.toml
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      106 2023-05-12 08:03:40.000000 solarmach-0.2.1/requirements.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2127 2023-05-12 08:06:14.629089 solarmach-0.2.1/setup.cfg
--rwxrwxr-x   0 gieseler  (1000) gieseler  (1000)      660 2022-03-14 12:48:51.000000 solarmach-0.2.1/setup.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-12 08:06:14.625089 solarmach-0.2.1/solarmach/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    51602 2023-05-11 14:20:54.000000 solarmach-0.2.1/solarmach/__init__.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    23221 2023-05-11 14:20:54.000000 solarmach-0.2.1/solarmach/pfss_utilities.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-12 08:06:14.629089 solarmach-0.2.1/solarmach/tests/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      108 2022-01-10 16:26:49.000000 solarmach-0.2.1/solarmach/tests/__init__.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1695 2022-11-09 14:33:28.000000 solarmach-0.2.1/solarmach/tests/test.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      345 2023-05-12 08:06:14.000000 solarmach-0.2.1/solarmach/version.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-12 08:06:14.625089 solarmach-0.2.1/solarmach.egg-info/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     6117 2023-05-12 08:06:14.000000 solarmach-0.2.1/solarmach.egg-info/PKG-INFO
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      584 2023-05-12 08:06:14.000000 solarmach-0.2.1/solarmach.egg-info/SOURCES.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2023-05-12 08:06:14.000000 solarmach-0.2.1/solarmach.egg-info/dependency_links.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2022-03-17 17:20:48.000000 solarmach-0.2.1/solarmach.egg-info/not-zip-safe
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      191 2023-05-12 08:06:14.000000 solarmach-0.2.1/solarmach.egg-info/requires.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)       10 2023-05-12 08:06:14.000000 solarmach-0.2.1/solarmach.egg-info/top_level.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1292 2022-03-14 12:48:29.000000 solarmach-0.2.1/tox.ini
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-26 10:24:46.044977 solarmach-0.2.2/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1478 2022-03-14 11:21:13.000000 solarmach-0.2.2/LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      457 2022-01-10 16:26:49.000000 solarmach-0.2.2/MANIFEST.in
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     6700 2023-05-26 10:24:46.044977 solarmach-0.2.2/PKG-INFO
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     5851 2023-05-25 11:54:23.000000 solarmach-0.2.2/README.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     3370 2022-03-30 15:50:45.000000 solarmach-0.2.2/code_of_conduct.md
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-26 10:24:46.032977 solarmach-0.2.2/docs/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      634 2022-01-10 16:26:49.000000 solarmach-0.2.2/docs/Makefile
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2300 2022-03-14 11:55:52.000000 solarmach-0.2.2/docs/conf.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      300 2022-03-14 11:56:45.000000 solarmach-0.2.2/docs/index.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      760 2022-01-10 16:26:49.000000 solarmach-0.2.2/docs/make.bat
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-26 10:24:46.036977 solarmach-0.2.2/examples/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)  1915936 2023-04-27 13:41:04.000000 solarmach-0.2.2/examples/example.ipynb
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   348683 2022-03-14 16:09:27.000000 solarmach-0.2.2/examples/solarmach.png
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-26 10:24:46.040977 solarmach-0.2.2/licenses/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1478 2022-03-14 11:21:13.000000 solarmach-0.2.2/licenses/LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1659 2022-01-10 16:26:49.000000 solarmach-0.2.2/licenses/TEMPLATE_LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      134 2022-01-10 16:26:49.000000 solarmach-0.2.2/pyproject.toml
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      106 2023-05-12 08:03:40.000000 solarmach-0.2.2/requirements.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2127 2023-05-26 10:24:46.044977 solarmach-0.2.2/setup.cfg
+-rwxrwxr-x   0 gieseler  (1000) gieseler  (1000)      660 2022-03-14 12:48:51.000000 solarmach-0.2.2/setup.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-26 10:24:46.040977 solarmach-0.2.2/solarmach/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    53052 2023-05-26 09:06:15.000000 solarmach-0.2.2/solarmach/__init__.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    22465 2023-05-26 09:01:52.000000 solarmach-0.2.2/solarmach/pfss_utilities.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-26 10:24:46.044977 solarmach-0.2.2/solarmach/tests/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      108 2022-01-10 16:26:49.000000 solarmach-0.2.2/solarmach/tests/__init__.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1695 2022-11-09 14:33:28.000000 solarmach-0.2.2/solarmach/tests/test.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      345 2023-05-26 10:24:45.000000 solarmach-0.2.2/solarmach/version.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-26 10:24:46.044977 solarmach-0.2.2/solarmach.egg-info/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     6700 2023-05-26 10:24:45.000000 solarmach-0.2.2/solarmach.egg-info/PKG-INFO
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      584 2023-05-26 10:24:46.000000 solarmach-0.2.2/solarmach.egg-info/SOURCES.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2023-05-26 10:24:45.000000 solarmach-0.2.2/solarmach.egg-info/dependency_links.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2022-03-17 17:20:48.000000 solarmach-0.2.2/solarmach.egg-info/not-zip-safe
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      191 2023-05-26 10:24:45.000000 solarmach-0.2.2/solarmach.egg-info/requires.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)       10 2023-05-26 10:24:45.000000 solarmach-0.2.2/solarmach.egg-info/top_level.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1292 2022-03-14 12:48:29.000000 solarmach-0.2.2/tox.ini
```

### Comparing `solarmach-0.2.1/LICENSE.rst` & `solarmach-0.2.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solarmach-0.2.1/PKG-INFO` & `solarmach-0.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solarmach
-Version: 0.2.1
+Version: 0.2.2
 Summary: Multi-spacecraft longitudinal configuration plotter
 Home-page: https://github.com/jgieseler/solarmach
 Author: Jan Gieseler
 Author-email: jan.gieseler@utu.fi
 License: BSD 3-clause
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -104,41 +104,47 @@
    
    # obtain data as Pandas DataFrame
    display(sm.coord_table)
 
 .. image:: https://github.com/jgieseler/solarmach/raw/main/examples/solarmach.png
   :alt: Example output figure
   
-See `example notebook <https://github.com/jgieseler/solarmach/blob/main/examples/example.ipynb>`_ for all options!
+See example notebooks in next section for all options!
   
-Example Notebook
-----------------
+Example Notebooks
+-----------------
 
 **solarmach** can easily be run in a Jupyter Notebook. 
 
-- `Download example notebook <https://github.com/jgieseler/solarmach/raw/main/examples/example.ipynb>`_
-
-- Try it online: |binder|
-  
-.. |binder| image:: https://mybinder.org/badge_logo.svg
- :target: https://mybinder.org/v2/gh/jgieseler/solarmach/main?labpath=examples%2Fexample.ipynb
+- `Show simple example notebook <https://nbviewer.org/github/jgieseler/solarmach/blob/main/examples/example.ipynb>`_ |nbviewer1|
+ 
+- `Show extended example notebook <https://nbviewer.org/github/serpentine-h2020/serpentine/blob/main/notebooks/solarmach/solarmach.ipynb>`_ |nbviewer2| (provided by `SERPENTINE <https://serpentine-h2020.eu>`_ project)
+ 
+ 
+.. |nbviewer1| image:: https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg
+ :target: https://nbviewer.org/github/jgieseler/solarmach/blob/main/examples/example.ipynb
+ 
+.. |nbviewer2| image:: https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg
+ :target: https://nbviewer.org/github/serpentine-h2020/serpentine/blob/main/notebooks/solarmach/solarmach.ipynb
  
 Citation
 --------
 
 Please cite the following paper if you use **solarmach** in your publication:
 
 Gieseler, J., Dresing, N., Palmroos, C., von Forstner, J.L.F., Price, D.J., Vainio, R. et al. (2022).
 Solar-MACH: An open-source tool to analyze solar magnetic connection configurations. *Front. Astronomy Space Sci.* 9. `doi:10.3389/fspas.2022.1058810 <https://doi.org/10.3389/fspas.2022.1058810>`_ 
  
 Acknowledgements
 ----------------
  
 The Solar-MACH tool was originally developed at Kiel University, Germany and further discussed within the `ESA Heliophysics Archives USer (HAUS) <https://www.cosmos.esa.int/web/esdc/archives-user-groups/heliophysics>`_ group.
 
+This project has received funding from the European Union’s Horizon 2020 research and innovation programme under grant agreement No 101004159.
+
 Powered by: |matplotlib| |sunpy|
 
 .. |matplotlib| image:: https://matplotlib.org/stable/_static/logo2_compressed.svg
    :height: 25px
    :target: https://matplotlib.org
 .. |sunpy| image:: https://raw.githubusercontent.com/sunpy/sunpy-logo/master/generated/sunpy_logo_landscape.svg
    :height: 30px
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `solarmach-0.2.1/README.rst` & `solarmach-0.2.2/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -80,41 +80,47 @@
    
    # obtain data as Pandas DataFrame
    display(sm.coord_table)
 
 .. image:: https://github.com/jgieseler/solarmach/raw/main/examples/solarmach.png
   :alt: Example output figure
   
-See `example notebook <https://github.com/jgieseler/solarmach/blob/main/examples/example.ipynb>`_ for all options!
+See example notebooks in next section for all options!
   
-Example Notebook
-----------------
+Example Notebooks
+-----------------
 
 **solarmach** can easily be run in a Jupyter Notebook. 
 
-- `Download example notebook <https://github.com/jgieseler/solarmach/raw/main/examples/example.ipynb>`_
-
-- Try it online: |binder|
-  
-.. |binder| image:: https://mybinder.org/badge_logo.svg
- :target: https://mybinder.org/v2/gh/jgieseler/solarmach/main?labpath=examples%2Fexample.ipynb
+- `Show simple example notebook <https://nbviewer.org/github/jgieseler/solarmach/blob/main/examples/example.ipynb>`_ |nbviewer1|
+ 
+- `Show extended example notebook <https://nbviewer.org/github/serpentine-h2020/serpentine/blob/main/notebooks/solarmach/solarmach.ipynb>`_ |nbviewer2| (provided by `SERPENTINE <https://serpentine-h2020.eu>`_ project)
+ 
+ 
+.. |nbviewer1| image:: https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg
+ :target: https://nbviewer.org/github/jgieseler/solarmach/blob/main/examples/example.ipynb
+ 
+.. |nbviewer2| image:: https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg
+ :target: https://nbviewer.org/github/serpentine-h2020/serpentine/blob/main/notebooks/solarmach/solarmach.ipynb
  
 Citation
 --------
 
 Please cite the following paper if you use **solarmach** in your publication:
 
 Gieseler, J., Dresing, N., Palmroos, C., von Forstner, J.L.F., Price, D.J., Vainio, R. et al. (2022).
 Solar-MACH: An open-source tool to analyze solar magnetic connection configurations. *Front. Astronomy Space Sci.* 9. `doi:10.3389/fspas.2022.1058810 <https://doi.org/10.3389/fspas.2022.1058810>`_ 
  
 Acknowledgements
 ----------------
  
 The Solar-MACH tool was originally developed at Kiel University, Germany and further discussed within the `ESA Heliophysics Archives USer (HAUS) <https://www.cosmos.esa.int/web/esdc/archives-user-groups/heliophysics>`_ group.
 
+This project has received funding from the European Union’s Horizon 2020 research and innovation programme under grant agreement No 101004159.
+
 Powered by: |matplotlib| |sunpy|
 
 .. |matplotlib| image:: https://matplotlib.org/stable/_static/logo2_compressed.svg
    :height: 25px
    :target: https://matplotlib.org
 .. |sunpy| image:: https://raw.githubusercontent.com/sunpy/sunpy-logo/master/generated/sunpy_logo_landscape.svg
    :height: 30px
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `solarmach-0.2.1/code_of_conduct.md` & `solarmach-0.2.2/code_of_conduct.md`

 * *Files identical despite different names*

### Comparing `solarmach-0.2.1/docs/Makefile` & `solarmach-0.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `solarmach-0.2.1/docs/conf.py` & `solarmach-0.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `solarmach-0.2.1/docs/make.bat` & `solarmach-0.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `solarmach-0.2.1/examples/example.ipynb` & `solarmach-0.2.2/examples/example.ipynb`

 * *Files identical despite different names*

### Comparing `solarmach-0.2.1/examples/solarmach.png` & `solarmach-0.2.2/examples/solarmach.png`

 * *Files identical despite different names*

### Comparing `solarmach-0.2.1/licenses/LICENSE.rst` & `solarmach-0.2.2/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solarmach-0.2.1/licenses/TEMPLATE_LICENSE.rst` & `solarmach-0.2.2/licenses/TEMPLATE_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solarmach-0.2.1/setup.cfg` & `solarmach-0.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `solarmach-0.2.1/setup.py` & `solarmach-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `solarmach-0.2.1/solarmach/__init__.py` & `solarmach-0.2.2/solarmach/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,16 +18,15 @@
 import pandas as pd
 import scipy.constants as const
 from astropy.coordinates import SkyCoord
 from matplotlib.legend_handler import HandlerPatch
 from sunpy import log
 from sunpy.coordinates import frames, get_horizons_coord
 
-# New addition to imports, contains the necessary functions to run pfss-extrapolation for sub-source surface magnetic field
-from solarmach.pfss_utilities import *
+from solarmach.pfss_utilities import calculate_pfss_solution, get_field_line_coords, get_gong_map, multicolorline, sphere, spheric2cartesian, vary_flines
 
 # pd.options.display.max_rows = None
 # pd.options.display.float_format = '{:.1f}'.format
 # if needed, rather use the following to have the desired display:
 """
 with pd.option_context('display.float_format', '{:0.2f}'.format):
     display(df)
@@ -356,15 +355,15 @@
         plt.rcParams['font.size'] = 15
         plt.rcParams['agg.path.chunksize'] = 20000
 
         fig, ax = plt.subplots(subplot_kw=dict(projection='polar'), figsize=figsize, dpi=dpi)
         self.ax = ax
 
         # build array of values for radius (in spherical coordinates!) given in AU!
-        r_array = np.arange(0.007, (self.max_dist*3)/np.cos(np.deg2rad(self.max_dist_lat)) + 0.3, 0.001)
+        r_array = np.arange(0.007, (self.max_dist+0.1)/np.cos(np.deg2rad(self.max_dist_lat)) + 3.0, 0.001)
         # take into account solar differential rotation wrt. latitude. Thus move calculation of omega to the per-body section below
         # omega = np.radians(360. / (25.38 * 24 * 60 * 60))  # solar rot-angle in rad/sec, sidereal period
 
         E_long = self.pos_E.lon.value
 
         for i, body_id in enumerate(self.body_dict):
             body_lab = self.body_dict[body_id][1]
@@ -431,46 +430,77 @@
                                 facecolor='black', lw=1.8, zorder=5, overhang=0.2)
 
             if plot_spirals:
                 ax.plot(alpha_ref, r_array * np.cos(np.deg2rad(ref_lat)), '--k', label=f'field line connecting to\nref. long. (vsw={reference_vsw} km/s)')
 
         if long_sector is not None:
             if type(long_sector) == list and len(long_sector)==2:
-                # long_sector_width = abs(180 - abs(abs(self.long_sector[0] - self.long_sector[1]) - 180))
-                # cone_dist = self.max_dist+0.3
-                # plt.bar(np.deg2rad(self.long_sector[0]), cone_dist, width=np.deg2rad(long_sector_width), align='edge', bottom=0.0, color=self.long_sector_color, alpha=0.5)
-
                 delta_ref1 = long_sector[0]
                 if delta_ref1 < 0.:
                     delta_ref1 = delta_ref1 + 360.
                 delta_ref2 = long_sector[1]
                 if delta_ref2 < 0.:
                     delta_ref2 = delta_ref2 + 360.
 
+                # Check that we are considering the same rotation
+                if delta_ref2 < delta_ref1:
+                    delta_ref2 += 360
+
                 long_sector_lat = [0, 0]  # maybe later add option to have different latitudes, so that the long_sector plane is out of the ecliptic
                 # take into account solar differential rotation wrt. latitude
                 omega_ref1 = self.solar_diff_rot(long_sector_lat[0])
                 omega_ref2 = self.solar_diff_rot(long_sector_lat[1])
 
+                # Build an r_array for the second spiral for while loop to iterate forwards
+                r_array2 = np.copy(r_array)
+
                 if long_sector_vsw is not None:
+                    # Calculate the first spiral's angles along r
                     alpha_ref1 = np.deg2rad(delta_ref1) + omega_ref1 / (long_sector_vsw[0] / AU) * (self.target_solar_radius*aconst.R_sun.to(u.AU).value - r_array) * np.cos(np.deg2rad(long_sector_lat[0]))
-                    alpha_ref2 = np.deg2rad(delta_ref2) + omega_ref2 / (long_sector_vsw[1] / AU) * (self.target_solar_radius*aconst.R_sun.to(u.AU).value - r_array) * np.cos(np.deg2rad(long_sector_lat[1]))
+                    alpha_ref2 = np.deg2rad(delta_ref2) + omega_ref2 / (long_sector_vsw[1] / AU) * (self.target_solar_radius*aconst.R_sun.to(u.AU).value - r_array2) * np.cos(np.deg2rad(long_sector_lat[1]))
+
+                    # Save the last angle as a starting point for reference for the while loop
+                    alpha_init = alpha_ref2[-1]
+
+                    # Check that reference angle of the first loop is ahead
+                    if alpha_ref1[-1] > alpha_ref2[-1]:
+                        alpha_ref1_comp = alpha_ref1[-1] - 2*np.pi
+                    else:
+                        alpha_ref1_comp = alpha_ref1[-1]
+
+                    # While the second spiral is behind the first spiral in angle, extend the second spiral
+                    while alpha_ref2[-1] > alpha_ref1_comp:
+                        r_array2 = np.append(r_array2, r_array2[-1] + 0.1)
+                        alpha_ref2 = np.append(alpha_ref2, np.deg2rad(delta_ref2) + omega_ref2 / (long_sector_vsw[1] / AU) * (self.target_solar_radius*aconst.R_sun.to(u.AU).value - r_array2[-1]) * np.cos(np.deg2rad(long_sector_lat[1])))
+
+                    # Interpolate the first spiral's angles to the coarser second spiral's angles (outside the plot)
+                    alpha_ref1 = np.interp(r_array2, r_array, alpha_ref1)
+
                 else:
                     # if no solar wind speeds for Parker spirals are provided, use straight lines:
-                    alpha_ref1 = [np.deg2rad(delta_ref1)] * len(r_array)
-                    alpha_ref2 = [np.deg2rad(delta_ref2)] * len(r_array)
+                    alpha_ref1 = np.array([np.deg2rad(delta_ref1)] * len(r_array))
+                    alpha_ref2 = np.array([np.deg2rad(delta_ref2)] * len(r_array))
 
-                c1 = plt.polar(alpha_ref1, r_array * np.cos(np.deg2rad(long_sector_lat[0])), lw=0, color=long_sector_color, alpha=0.5)[0]
+                c1 = plt.polar(alpha_ref1, r_array2 * np.cos(np.deg2rad(long_sector_lat[0])), lw=0, color=long_sector_color, alpha=0.5)[0]
                 x1 = c1.get_xdata()
                 y1 = c1.get_ydata()
-                c2 = plt.polar(alpha_ref2, r_array * np.cos(np.deg2rad(long_sector_lat[1])), lw=0, color=long_sector_color, alpha=0.5)[0]
+                c2 = plt.polar(alpha_ref2, r_array2 * np.cos(np.deg2rad(long_sector_lat[1])), lw=0, color=long_sector_color, alpha=0.5)[0]
                 x2 = c2.get_xdata()
                 y2 = c2.get_ydata()
 
-                plt.fill_betweenx(y1, x1, x2, lw=0, color=long_sector_color, alpha=0.5)
+                # Check that plotted are is between the two spirals, and do not fill after potential crossing
+                clause1 = x1 < x2
+                clause2 = alpha_ref1[clause1] < alpha_ref2[clause1]
+
+                # Take only the points that fill the above clauses
+                y1_fill = y1[clause1][clause2]
+                x1_fill = x1[clause1][clause2]
+                x2_fill = x2[clause1][clause2]
+
+                plt.fill_betweenx(y1_fill, x1_fill, x2_fill, lw=0, color=long_sector_color, alpha=0.5)
             else:
                 print("Ill-defined 'long_sector'. It should be a 2-element list defining the start and end longitude of the cone in degrees; e.g. 'long_sector=[15,45]'")
 
         if background_spirals is not None:
             if type(background_spirals) == list and len(background_spirals)>=2:
                 # maybe later add option to have a non-zero latitude, so that the field lines are out of the ecliptic
                 background_spirals_lat = 0
@@ -487,15 +517,15 @@
                 else:
                     background_spirals_c = 'grey'
 
                 if len(background_spirals)>=5:
                     background_spirals_alpha = background_spirals[4]
                 else:
                     background_spirals_alpha = 0.5
-                
+
                 for l in np.arange(0, 360, 360/background_spirals[0]):
                     alpha_ref = np.deg2rad(l) + omega_ref / (background_spirals[1] / AU) * (self.target_solar_radius*aconst.R_sun.to(u.AU).value - r_array) * np.cos(np.deg2rad(background_spirals_lat))
                     ax.plot(alpha_ref, r_array * np.cos(np.deg2rad(background_spirals_lat)), ls=background_spirals_ls, c=background_spirals_c, alpha=background_spirals_alpha)
             else:
                 print("Ill-defined 'background_spirals'. It should be a list with at least 2 elements defining the number of field lines and the solar wind speed used for them in km/s; e.g. 'background_spirals=[10, 400]'")
 
         leg1 = ax.legend(loc=(1.2, 0.7), fontsize=13)
@@ -612,31 +642,29 @@
         ax2.set_theta_offset(np.deg2rad(long_offset - E_long))
         gridlines = ax2.xaxis.get_gridlines()
         for xax in gridlines:
             xax.set_color('darkgreen')
 
         return ax2
 
-
-
-    def plot_pfss(self, 
+    def plot_pfss(self,
                   rss=2.5,
-                  pfss_solution = None,
-                  figsize = (15,10),
-                  dpi = 200,
-                  return_plot_object = False,
+                  pfss_solution=None,
+                  figsize=(15, 10),
+                  dpi=200,
+                  return_plot_object=False,
                   vary=False, n_varies=1,
-                  long_offset = 270,
-                  reference_vsw = 400.,
-                  numbered_markers = False,
-                  plot_spirals = True,
-                  long_sector = None,
-                  long_sector_vsw = None,
-                  long_sector_color = None,
-                  hide_logo = False):
+                  long_offset=270,
+                  reference_vsw=400.,
+                  numbered_markers=False,
+                  plot_spirals=True,
+                  long_sector=None,
+                  long_sector_vsw=None,
+                  long_sector_color=None,
+                  hide_logo=False):
         """
         Produces a figure of the heliosphere in polar coordinates with logarithmic r-axis outside the pfss.
         Also tracks an open field line down to photosphere given a point on the pfss.
 
         rss : float
                 source surface height of the potential field in solar radii. default 2.5
         pfss_solution : .fits
@@ -645,17 +673,17 @@
                 draws an arrow pointing radially outward, input in degrees
 
         """
 
         if not pfss_solution:
             raise Exception("A PFSS solution is required for solar magnetic field extrapolation!")
 
-        # Constants 
+        # Constants
         AU = const.au / 1000  # km
-        sun_radius = aconst.R_sun.value # meters
+        sun_radius = aconst.R_sun.value  # meters
 
         # r_scaler scales distances from astronomical units to solar radii. unit = [solar radii / AU]
         r_scaler = (AU*1000)/sun_radius
 
         # carrington longitude of the Earth
         E_long = self.pos_E.lon.value
 
@@ -665,27 +693,27 @@
         plt.rcParams['font.size'] = 15
         plt.rcParams['agg.path.chunksize'] = 20000
 
         # init the figure and axes
         fig, ax = plt.subplots(subplot_kw=dict(projection='polar'), figsize=figsize, dpi=dpi)
 
         # maximum distance anything will be plotted
-        r_max = r_scaler * 5 # 5 AU in units of solar radii
+        r_max = r_scaler * 5  # 5 AU in units of solar radii
 
         # setting the title
         ax.set_title(self.date + '\n', pad=30, fontsize=26)
 
         # Plot the source_surface and solar surface
         full_circle_radians = 2*np.pi*np.linspace(0, 1, 200)
         ax.plot(full_circle_radians, np.ones(200)*rss, c='k', ls='--', zorder=3)
         ax.plot(full_circle_radians, np.ones(200), c='darkorange', lw=2.5, zorder=1)
 
         # Plot the 30 and 60 deg lines on the Sun
-        ax.plot(full_circle_radians, np.ones(len(full_circle_radians))*0.866, c='darkgray', lw=1.5, ls=":", zorder=3) #cos(30deg) = 0.866(O)
-        ax.plot(full_circle_radians, np.ones(len(full_circle_radians))*0.500, c='darkgray', lw=1.5, ls=":", zorder=3) #cos(60deg) = 0.5(0)
+        ax.plot(full_circle_radians, np.ones(len(full_circle_radians))*0.866, c='darkgray', lw=1.5, ls=":", zorder=3)  # cos(30deg) = 0.866(O)
+        ax.plot(full_circle_radians, np.ones(len(full_circle_radians))*0.500, c='darkgray', lw=1.5, ls=":", zorder=3)  # cos(60deg) = 0.5(0)
 
         # Gather field line objects, photospheric footpoints and magnetic polarities in these lists
         # fieldlines is a class attribute, so that the field lines can be neasily 3D plotted with another method
         self.fieldlines = []
         photospheric_footpoints = []
         fieldline_polarities = []
 
@@ -707,15 +735,15 @@
             dist_body = pos.radius.value
 
             body_long = pos.lon.value
             body_lat = pos.lat.value
 
             # take into account solar differential rotation wrt. latitude
             omega = self.solar_diff_rot(body_lat)
- 
+
             # The radial coordinates (outside source surface) for each object
             r_array = np.linspace(r_scaler*dist_body*np.cos(np.deg2rad(body_lat)), rss, 1000)
 
             # plot body positions
             if numbered_markers:
                 ax.plot(np.deg2rad(body_long), r_scaler*dist_body*np.cos(np.deg2rad(body_lat)), 'o', ms=15, color=body_color, label=body_lab)
                 ax.annotate(i+1, xy=(np.deg2rad(body_long), r_scaler*dist_body*np.cos(np.deg2rad(body_lat))), color='white',
@@ -733,15 +761,15 @@
                 alpha_body = np.deg2rad(body_long) + omega / (1000*body_vsw / sun_radius) * (r_scaler*dist_body - r_array) * np.cos(np.deg2rad(body_lat))
                 ax.plot(alpha_body, r_array * np.cos(np.deg2rad(body_lat)), color=body_color)
 
             # acquire an array of (r,lon,lat) coordinates of the open field lines under the pfss
             # based on the footpoint(s) of the sc
             if vary:
 
-                # Triplets contain 35 tuples of (r,lon,lat) 
+                # Triplets contain 35 tuples of (r,lon,lat)
                 fline_triplets, fline_objects, varyfline_triplets, varyfline_objects = vary_flines(alpha_body[-1], np.deg2rad(body_lat), pfss_solution, n_varies, rss)
 
                 # Collect field line objects to a list
                 self.fieldlines.append(fline_objects[0])
                 for varyfline in varyfline_objects:
                     self.fieldlines.append(varyfline)
 
@@ -751,15 +779,15 @@
                     v_fl_lon = triplet[1]
                     v_fl_lat = triplet[2]
 
                     fieldline = multicolorline(np.deg2rad(v_fl_lon), np.cos(np.deg2rad(v_fl_lat))*v_fl_r, ax=ax, cvals=v_fl_lat, vmin=-90, vmax=90)
 
             else:
                 # If no varying, then just get one field line from get_field_line_coords()
-                # Note that even in the case of a singular fieldline object, this function returns a list 
+                # Note that even in the case of a singular fieldline object, this function returns a list
                 fline_triplets, fline_objects = get_field_line_coords(alpha_body[-1], np.deg2rad(body_lat), pfss_solution, rss)
 
                 # Collect field line objects to a list
                 self.fieldlines.append(fline_objects[0])
 
             # The middlemost field lines are always plotted regardless if varying or no
             fl_r   = fline_triplets[0][0]
@@ -769,39 +797,38 @@
             # Plot the color coded field line
             fieldline = multicolorline(np.deg2rad(fl_lon), np.cos(np.deg2rad(fl_lat))*fl_r, ax=ax, cvals=fl_lat, vmin=-90, vmax=90)
 
             # Finally, save the photospheric footpoint of the middlemost field lines as a tuple and magnetic polarity as +1/-1
             photospheric_footpoints.append((fl_lon[0], fl_lat[0]))
             fieldline_polarities.append(int(fline_objects[0].polarity))
 
-
         # Reference longitude and corresponding parker spiral arm
         if self.reference_long:
             delta_ref = self.reference_long
             if delta_ref < 0.:
                 delta_ref = delta_ref + 360.
             if self.reference_lat is None:
                 ref_lat = 0.
             else:
                 ref_lat = self.reference_lat
 
             # take into account solar differential rotation wrt. latitude
             omega_ref = self.solar_diff_rot(ref_lat)
 
             # old eq. for alpha_ref contained redundant dist_e variable:
-            #alpha_ref = np.deg2rad(delta_ref) + omega_ref / (1000*reference_vsw / sun_radius) * (r_scaler*self.target_solar_radius*aconst.R_sun.to(u.AU).value - reference_array) * np.cos(np.deg2rad(ref_lat))
+            # alpha_ref = np.deg2rad(delta_ref) + omega_ref / (1000*reference_vsw / sun_radius) * (r_scaler*self.target_solar_radius*aconst.R_sun.to(u.AU).value - reference_array) * np.cos(np.deg2rad(ref_lat))
             alpha_ref = np.deg2rad(delta_ref) + omega_ref / (1000*reference_vsw / sun_radius) * (rss - reference_array) * np.cos(np.deg2rad(ref_lat))
 
             # old arrow style:
             arrow_dist = rss-1
             ref_arr = plt.arrow(np.deg2rad(delta_ref), 1, 0, arrow_dist, head_width=0.1, head_length=0.4, edgecolor='black',
                                 facecolor='black', lw=2.0, zorder=5, overhang=0.2)
 
             if plot_spirals:
-                ax.plot(alpha_ref, reference_array * np.cos(np.deg2rad(ref_lat)), ls='--', lw=1.8, color='k', 
+                ax.plot(alpha_ref, reference_array * np.cos(np.deg2rad(ref_lat)), ls='--', lw=1.8, color='k',
                         label=f'field line connecting to\nref. long. (vsw={reference_vsw} km/s)', zorder=1)
 
         if long_sector is not None:
             if type(long_sector) == list and len(long_sector)==2:
 
                 delta_ref1 = long_sector[0]
                 if delta_ref1 < 0.:
@@ -867,16 +894,16 @@
         # if self.coord_sys=='Stonyhurst':
         #     ax.set_xticks(np.pi/180. * np.linspace(180, -180, 8, endpoint=False))
         #     ax.set_thetalim(-np.pi, np.pi)
 
         # Spin the angular coordinate so that earth is at 6 o'clock
         ax.set_theta_offset(np.deg2rad(long_offset - E_long))
 
-        # For some reason we need to specify 'ylim' here 
-        ax.set_ylim(0,r_max)
+        # For some reason we need to specify 'ylim' here
+        ax.set_ylim(0, r_max)
         ax.set_rscale('symlog', linthresh=rss)
         ax.set_rmax(r_max)
         ax.set_rticks([1.0, rss, 10.0, 100.0])
         ax.set_rlabel_position(-22.5)  # Move radial labels away from plotted line
         ax.tick_params(which='major', labelsize=22,)
 
         rlabels = ['1', str(rss), r'$10^1$', r'$10^2$']
@@ -910,39 +937,36 @@
             st.pyplot(fig)  # , dpi=200)
         else:
             plt.show()
 
         if return_plot_object:
             return fig, ax
 
-
-    def pfss_3d(self, active_area=(None,None,None,None), color_code='object'):
+    def pfss_3d(self, active_area=(None, None, None, None), color_code='object'):
         """
         https://plotly.github.io/plotly.py-docs/generated/plotly.graph_objects.Scatter3d.html
         https://plotly.com/python-api-reference/generated/plotly.graph_objects.Figure.html
         https://plotly.com/python-api-reference/plotly.graph_objects.html
         https://fslab.org/XPlot/chart/plotly-3d-line-plots.html
 
         Opens up an interactive 3d-plot of the Sun and FieldLine objects. Also shows the flare area if provided.
 
         params
         -------
         active_area: (lonmax, lonmin, latmax, latmin)
                     A tuple of the max and min of longitude and latitude in degrees
-        
+
         color_code: str
                     Choose either 'polarity' or 'object'
         """
 
-        import plotly.graph_objects as go
         import plotly.express as px
-
-        from plotly.graph_objects import Line
-
+        import plotly.graph_objects as go
         from astropy.constants import R_sun
+        from plotly.graph_objects import Line
 
         # Flare site (or whatever area of interest) is plotted at this height
         FLARE_HEIGHT = 1.005
 
         object_names = list(self.body_dict.keys())
 
         # choose the color coding as either polarity or object
@@ -956,107 +980,105 @@
             # Plotly doesn't like color 'b', so check if that exists and change it to more specific identifier
             for i, color in enumerate(color_list):
                 if color=='b':
                     color_list[i] = "blue"
 
         elif color_code=='polarity':
 
-            colors = {0: 'black', 
-                      -1: 'blue', 
+            colors = {0: 'black',
+                      -1: 'blue',
                       1: 'red'}
 
         else:
             raise Exception(f"Invalid color_code=={color_code}. Choose either 'polarity' or 'object'.")
-        
+
         # create the sun object, a sphere, for plotting
-        sun = sphere(radius=1, clr='#ffff55') # '#ffff00'
+        sun = sphere(radius=1, clr='#ffff55')  # '#ffff00'
 
         # and add it to the list of traces
         # traces are all the objects that will be plotted
         traces = [sun]
 
         # go through field lines, assign a color to them and append them to the list of traces
         for i, field_line in enumerate(self.fieldlines):
+            coords = field_line.coords
+            coords.representation_type = "cartesian"
 
-                coords = field_line.coords
-                coords.representation_type = "cartesian"
-
-                if color_code=="polarity":
-                    color = colors.get(field_line.polarity)
-                if color_code=='object':
-                    color = color_list[i//modulator]
-
-                # New object's lines being plotted
-                if i%modulator==0: 
-                    line_label = object_names[i//modulator]
-                    show_in_legend = True
-                else:
-                    show_in_legend = False
-
-                fieldline_trace = go.Scatter3d(x=coords.x/R_sun, y=coords.y/R_sun, z=coords.z/R_sun, 
-                                            mode='lines', 
-                                            line = Line(color = color, width = 3.5),
-                                            name = line_label,
-                                            showlegend = show_in_legend
-                                            )
+            if color_code=="polarity":
+                color = colors.get(field_line.polarity)
+            if color_code=='object':
+                color = color_list[i//modulator]
+
+            # New object's lines being plotted
+            if i%modulator==0:
+                line_label = object_names[i//modulator]
+                show_in_legend = True
+            else:
+                show_in_legend = False
 
-                traces.append(fieldline_trace)
+            fieldline_trace = go.Scatter3d(x=coords.x/R_sun, y=coords.y/R_sun, z=coords.z/R_sun,
+                                           mode='lines',
+                                           line=Line(color=color, width=3.5),
+                                           name=line_label,
+                                           showlegend=show_in_legend
+                                           )
 
+            traces.append(fieldline_trace)
 
         if active_area[0]:
 
             # the flare area is bound by the extreme values of longitude and latitude
             lonmax, lonmin = np.deg2rad(active_area[0]), np.deg2rad(active_area[1])
             latmax, latmin = np.deg2rad(active_area[2]), np.deg2rad(active_area[3])
 
             # the perimeter of flare area in four segments
             perimeter1 = (np.linspace(lonmin, lonmax, 10), [latmax]*10)
             perimeter2 = (np.linspace(lonmin, lonmax, 10), [latmin]*10)
             perimeter3 = ([lonmax]*10, np.linspace(latmin, latmax, 10))
             perimeter4 = ([lonmin]*10, np.linspace(latmin, latmax, 10))
 
             # the perimeter in terms of elevation and azimuthal angles
-            perimeter_phis = np.append(np.append(np.append(perimeter1[0],perimeter2[0]),perimeter3[0]),perimeter4[0])
-            perimeter_thetas = np.append(np.append(np.append(perimeter1[1],perimeter2[1]),perimeter3[1]),perimeter4[1])
+            perimeter_phis = np.append(np.append(np.append(perimeter1[0], perimeter2[0]), perimeter3[0]), perimeter4[0])
+            perimeter_thetas = np.append(np.append(np.append(perimeter1[1], perimeter2[1]), perimeter3[1]), perimeter4[1])
 
             # the perimeter in terms of cartesian components
             perimeter_cartesian = spheric2cartesian([FLARE_HEIGHT]*40, theta=perimeter_thetas, phi=perimeter_phis)
 
             # flare area object
-            active_area = go.Scatter3d(x=perimeter_cartesian[0], y=perimeter_cartesian[1], z=perimeter_cartesian[2], 
-                                    mode='lines', 
-                                    line = Line(color = 'purple', width = 5.5),
-                                    name = "Active Area"
-                                    )
+            active_area = go.Scatter3d(x=perimeter_cartesian[0], y=perimeter_cartesian[1], z=perimeter_cartesian[2],
+                                       mode='lines',
+                                       line=Line(color='purple', width=5.5),
+                                       name="Active Area"
+                                       )
 
             traces.append(active_area)
 
         # the 0-latitude line, i.e. the equator
-        equator_sphericals = (np.ones(101)*FLARE_HEIGHT,np.zeros(101),np.linspace(0,2*np.pi,101))
-        equator_cartesians = spheric2cartesian(equator_sphericals[0],equator_sphericals[1],equator_sphericals[2])
+        equator_sphericals = (np.ones(101)*FLARE_HEIGHT, np.zeros(101), np.linspace(0, 2*np.pi, 101))
+        equator_cartesians = spheric2cartesian(equator_sphericals[0], equator_sphericals[1], equator_sphericals[2])
 
-        equator_line = go.Scatter3d(x=equator_cartesians[0], y=equator_cartesians[1], z=equator_cartesians[2], 
-                                    mode='lines', 
-                                    line = Line(color = 'black', width = 5.5),
-                                    name = "0 Latitude"
-                                )
+        equator_line = go.Scatter3d(x=equator_cartesians[0], y=equator_cartesians[1], z=equator_cartesians[2],
+                                    mode='lines',
+                                    line=Line(color='black', width=5.5),
+                                    name="0 Latitude"
+                                    )
 
         traces.append(equator_line)
 
         # create the figure
         fig = go.Figure(data=traces)
 
         # additional figure settings, like aspect mode, extreme values of axes etc...
         fig.update_layout(scene_aspectmode='cube')
-        fig.update_layout(scene = dict(
-                        xaxis = dict(nticks=4, range=[-2.5,2.5],), 
-                        yaxis = dict(nticks=4, range=[-2.5,2.5],), 
-                        zaxis = dict(nticks=4, range=[-2.5,2.5],),), 
-                        width=1280, height=720, 
-                        margin=dict(r=20, l=10, b=10, t=10))
+        fig.update_layout(scene=dict(
+                          xaxis=dict(nticks=4, range=[-2.5, 2.5],),
+                          yaxis=dict(nticks=4, range=[-2.5, 2.5],),
+                          zaxis=dict(nticks=4, range=[-2.5, 2.5],),),
+                          width=1280, height=720,
+                          margin=dict(r=20, l=10, b=10, t=10))
 
         fig.show()
 
         return 0
 
 
 def _isstreamlit():
@@ -1074,8 +1096,7 @@
         if not get_script_run_ctx():
             use_streamlit = False
         else:
             use_streamlit = True
     except ModuleNotFoundError:
         use_streamlit = False
     return use_streamlit
-
```

### Comparing `solarmach-0.2.1/solarmach/pfss_utilities.py` & `solarmach-0.2.2/solarmach/pfss_utilities.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,28 @@
 
 from pkg_resources import get_distribution, DistributionNotFound
 try:
     __version__ = get_distribution(__name__).version
 except DistributionNotFound:
     pass  # package is not installed
 
+import glob
 import os
 import pickle
-import glob
-
-import numpy as np
-import matplotlib.pyplot as plt
-
-import sunpy.map
-from sunpy.net import Fido, attrs as a
 
 import astropy.constants as aconst
 import astropy.units as u
+import matplotlib.pyplot as plt
+import numpy as np
+import pfsspy
+import sunpy.map
 from astropy.coordinates import SkyCoord
+from sunpy.net import Fido
+from sunpy.net import attrs as a
 
-import pfsspy
 
 # @st_cache_decorator
 def get_pfss_hmimap(filepath, email, carrington_rot, date, rss=2.5, nrho=35):
     """
     Downloading hmi map or calculating the PFSS solution
 
     params
@@ -41,15 +40,15 @@
             The Carrington rotation corresponding to the hmi map
     date: str
             The date of the map. Format = 'YYYY/MM/DD'
     rss: float (default = 2.5)
             The height of the potential field source surface for the solution.
     nrho: int (default = 35)
             The resolution of the PFSS-solved field line objects
-    
+
     returns
     -------
     output: hmi_synoptic_map object
             The PFSS-solution
     """
 
     time = a.Time(date, date)
@@ -99,17 +98,16 @@
     vmin, vmax: int (default = -90, 90)
 
     returns
     -------
     line: LineCollection object
     """
 
-    import matplotlib.colors as mcolors
     import cmasher as cmr
-
+    import matplotlib.colors as mcolors
     from matplotlib.collections import LineCollection
 
     # Create a set of line segments so that we can color them individually
     # This creates the points as a N x 1 x 2 array so that we can stack points
     # together easily to get the segments. The segments array for line collection
     # needs to be (numlines) x (points per line) x 2 (for x and y)
     points = np.array([x, y]).T.reshape(-1, 1, 2)
@@ -178,43 +176,43 @@
     coordlist = []
     flinelist = []
     for i in range(coord_triplets):
 
         # Inits for finding another seed point if we hit null or closed line
         turn = 'lon'
         sign_switch = 1
-        
+
         # Steps to the next corner, steps taken
-        corner_tracker = [1,0]
-        
+        corner_tracker = [1, 0]
+
         init_lon, init_lat = longitude[i], latitude[i]
 
         # Keep tracing the field line until a valid one is found
-        while(True):
+        while (True):
 
             # Trace a field line downward from the point lon,lat on the pfss
             fline = trace_field_line(longitude[i], latitude[i], hmimap, seedheight=seedheight)
 
             radius0 = fline.coords.radius[0].value
             radius9 = fline.coords.radius[-1].value
             bool_key = (radius0==radius9)
 
             # If fline is not a valid field line, then spiral out from init_point and try again
             # Also check if this is a null line (all coordinates identical)
             # Also check if polarity is 0, meaning that the field line is NOT open
-            if( (len(fline.coords) < 10) or bool_key or fline.polarity==0): #fline.polarity==0 
+            if ((len(fline.coords) < 10) or bool_key or fline.polarity==0):  # fline.polarity==0
 
                 longitude[i], latitude[i], sign_switch, corner_tracker, turn = spiral_out(longitude[i], latitude[i], sign_switch, corner_tracker, turn)
 
             # If there was nothing wrong, break the loop and proceed with the traced field line
             else:
                 break
 
             # Check that we are not too far from the original coordinate
-            if(corner_tracker[0] >= 10):
+            if (corner_tracker[0] >= 10):
                 print(f"no open field line found in the vicinity of {init_lon},{init_lat}")
                 break
 
         # Get the field line coordinate values in the correct order
         # Start on the photopshere, end at the pfss
         fl_r, fl_lon, fl_lat = get_coord_values(fline)
 
@@ -225,31 +223,31 @@
 
     return coordlist, flinelist
 
 
 def vary_flines(lon, lat, hmimap, n_varies, rss):
     """
     Finds a set of sub-pfss fieldlines connected to or very near a single footpoint on the pfss.
-    
+
     lon: longitude of the footpoint [rad]
     lat: latitude of the footpoint [rad]
-    
+
     n_varies:   tuple that holds the amount of circles and the number of dummy flines per circle
-                if type(n_varies)=int, consider that as the amount of circles, and set the 
+                if type(n_varies)=int, consider that as the amount of circles, and set the
                 amount of dummy flines per circle to 16
 
     params
     -------
     lon: int/float
             The longitude of the footpoint in radians
     lat: int/float
             The latitude of the footpoint in radians
     hmimap: hmi_synoptic_map object
             The pfss-solution used to calculate the field lines
-    n_varies: list[int,int] or int 
+    n_varies: list[int,int] or int
             A list that holds the amount of circles and the number of dummy flines per circle
             if type(n_varies)=int, consider that as the amount of circles, and set the
             amount of dummy flines per circle to 16
     rss: float
             Heliocentric height of the source surface
 
     returns
@@ -261,48 +259,48 @@
     varycoords: list[float,float,float]
             List of coordinate triplets of the varied field lines
     varyflines: list[FieldLine-object]
             List of Fieldline objects of the varied field lines
     """
 
     # Field lines per n_circles (circle)
-    if isinstance(n_varies,list):
+    if isinstance(n_varies, list):
         n_circles = n_varies[0]
         n_flines = n_varies[1]
     else:
         n_circles = n_varies
         n_flines = 16
 
     # First produce new points around the given lonlat_pair
     lons, lats= np.array([lon]), np.array([lat])
     increments = np.array([0.03, 0.05, 0.07, 0.09, 0.11, 0.13, 0.15, 0.17, 0.19, 0.21, 0.23, 0.25, 0.27, 0.29])
     for circle in range(n_circles):
 
-        newlons, newlats = circle_around(lon,lat,n_flines,r=increments[circle])
-        lons, lats = np.append(lons,newlons), np.append(lats,newlats)
+        newlons, newlats = circle_around(lon, lat, n_flines, r=increments[circle])
+        lons, lats = np.append(lons, newlons), np.append(lats, newlats)
 
     pointlist = np.array([lons, lats])
 
     # Trace fieldlines from all of these points
-    varycoords, varyflines = get_field_line_coords(pointlist[0],pointlist[1],hmimap, rss)
+    varycoords, varyflines = get_field_line_coords(pointlist[0], pointlist[1], hmimap, rss)
 
     # Because the original fieldlines and the varied ones are all in the same arrays,
     # Extract the varied ones to their own arrays
     coordlist, flinelist = [], []
 
     # Total amount of flines = 1 + (circles) * (fieldlines_per_circle)
     total_per_fp = n_flines*n_circles+1
     erased_indices = []
     for i in range(len(varycoords)):
         # n_flines*n_circles = the amount of extra field lines between each "original" field line
         if i%(total_per_fp)==0:
             erased_indices.append(i)
             # pop(i) removes the ith element from the list and returns it
             # -> we append it to the list of original footpoint fieldlines
-            coordlist.append(varycoords[i]) #.pop(i)
+            coordlist.append(varycoords[i])  # .pop(i)
             flinelist.append(varyflines[i])
 
     # Really ugly quick fix to erase values from varycoords and varyflines
     for increment, index in enumerate(erased_indices):
         varycoords.pop(index-increment)
         varyflines.pop(index-increment)
 
@@ -320,20 +318,20 @@
             Longitude and latitude of the seedpoint
     hmimap: hmimap-object
 
     seedheight: float
             The height at which field line tracing is started (in solar radii)
     rad: bool, (default True)
             Wether or not input coordinates are in radians. If False, consider them degrees
-    
+
     Returns:
     --------
     field_lines: FieldLine or list[FieldLine]
             A FieldLine object, or a list of them, if input coordinates were a list
-    
+
     '''
     from pfsspy import tracing
 
     # if lat0 and lon0 are given in deg for some reason, transform them to rad
     if not rad:
         lat0 = np.deg2rad(lat0)
         lon0 = np.deg2rad(lon0)
@@ -357,71 +355,70 @@
     else:
         return field_lines
 
 
 def spiral_out(lon, lat, sign_switch, corner_tracker, turn):
     """
     Moves the seeding point in an outward spiral.
-    
+
     Parameters
     ---------
     lon, lat: float
             the carrington coordinates on a surface of a sphere (sun or pfss)
     sign_switch: int
-            -1 or 1, dictates the direction in which lon or lat is 
+            -1 or 1, dictates the direction in which lon or lat is
             incremented
     corner_tracker: tuple
             first entry is steps_unti_corner, int that tells how many steps to the next corner of a spiral
             the second entry is steps taken on a given spiral turn
     turn: str
             indicates which is to be incremented, lon or lat
-            
+
     returns
     -----------
     lon, lat: float
             new coordinate pair
     """
-    
+
     # In radians, 1 rad \approx 57.3 deg
     step = 0.01
-    
+
     # Keeps track of how many steps until it's time to turn
     steps_until_corner, steps_moved = corner_tracker[0], corner_tracker[1]
 
     if turn=='lon':
-        
+
         lon = lon + step*sign_switch
         lat = lat
-        
+
         steps_moved += 1
-        
+
         # We have arrived in a corner, time to move in lat direction
         if steps_until_corner == steps_moved:
             steps_moved = 0
             turn = 'lat'
 
         return lon, lat, sign_switch, [steps_until_corner, steps_moved], turn
 
-
     if turn=='lat':
-        
+
         lon = lon
         lat = lat + step*sign_switch
-        
+
         steps_moved += 1
 
         # Hit a corner; start moving in the lon direction
         if steps_until_corner == steps_moved:
             steps_moved = 0
             steps_until_corner += 1
             turn = 'lon'
             sign_switch = sign_switch*(-1)
-        
+
         return lon, lat, sign_switch, [steps_until_corner, steps_moved], turn
-        
+
 
 def get_coord_values(field_line):
     """
     Gets the coordinate values from FieldLine object and makes sure that they are in the right order.
 
     params
     -------
@@ -509,58 +506,58 @@
     if fl_r[0] > fl_r[-1]:
         coordinates = np.flip(coordinates)
 
     return coordinates
 
 
 def spheric2cartesian(r, theta, phi):
-        """
-        Does a coordinate transformation from spherical to cartesian
+    """
+    Does a coordinate transformation from spherical to cartesian
 
-        r : the distance to the origin
-        theta : the elevation angle (goes from -pi to pi)
-        phi : the azimuth angle (goes from 0 to 2pi)
-        """
-
-        x = r * np.cos(phi) * np.cos(theta)
-        y = r * np.sin(phi) * np.cos(theta)
-        z = r * np.sin(theta)
+    r : the distance to the origin
+    theta : the elevation angle (goes from -pi to pi)
+    phi : the azimuth angle (goes from 0 to 2pi)
+    """
+
+    x = r * np.cos(phi) * np.cos(theta)
+    y = r * np.sin(phi) * np.cos(theta)
+    z = r * np.sin(theta)
 
-        return x, y, z
+    return x, y, z
 
 
 def sphere(radius, clr, dist=0):
     """
     Constructs a sphere with a given radius and color.
 
     params
     ---------
     radius : float, int
             The radius of the sphere
-    
+
     clr : str
             The color code for the sphere
-    
+
     dist : float, int
             The displacement of the sphere, if not centered at origin
     """
 
     import plotly.graph_objects as go
-    
+
     # Set up 100 points. First, do angles
-    phi = np.linspace(0,2*np.pi,100) # phi, the azimuthal angle goes from 0 to 2pi
-    theta = np.linspace(0,np.pi,100) # theta, the elevation angle goes from 0 to pi
-    
+    phi = np.linspace(0, 2*np.pi, 100)  # phi, the azimuthal angle goes from 0 to 2pi
+    theta = np.linspace(0, np.pi, 100)  # theta, the elevation angle goes from 0 to pi
+
     # Set up coordinates for points on the sphere
-    x0 = dist + radius * np.outer(np.cos(phi),np.sin(theta))
-    y0 = radius * np.outer(np.sin(phi),np.sin(theta))
-    z0 = radius * np.outer(np.ones(100),np.cos(theta))
-    
+    x0 = dist + radius * np.outer(np.cos(phi), np.sin(theta))
+    y0 = radius * np.outer(np.sin(phi), np.sin(theta))
+    z0 = radius * np.outer(np.ones(100), np.cos(theta))
+
     # Set up trace (the object that is then plottable)
-    trace= go.Surface(x=x0, y=y0, z=z0, colorscale=[[0,clr], [1,clr]], showscale=False, name="Sun")
+    trace= go.Surface(x=x0, y=y0, z=z0, colorscale=[[0, clr], [1, clr]], showscale=False, name="Sun")
 
     return trace
 
 
 def calculate_pfss_solution(gong_map, rss, nrho=35):
     """
     Calculates a Potential Field Source Surface solution based on a GONG map and
@@ -591,36 +588,36 @@
 
 
 def load_gong_map(filepath=None):
     """
     https://gong.nso.edu/data/magmap/
     https://docs.sunpy.org/en/v4.0.6/generated/api/sunpy.net.dataretriever.GONGClient.html
     https://gong2.nso.edu/oQR/zqs/202104/mrzqs210413/
-    
+
     """
 
     if not filepath:
         filepath = os.getcwd()
 
     # Load a GONG (Global Oscillation Network Group) synoptic magnetic map
-    if isinstance(filepath,str):
+    if isinstance(filepath, str):
 
         # Acquire a GONG map from which the pfss solution is calculated from
         gong_map = sunpy.map.Map(filepath)
 
     return gong_map
 
 
 def download_gong_map(timestr, filepath=None):
     """
     Gets the download link for a GONG synoptic map
     """
 
-    from sunpy.net import Fido, attrs
     import pandas as pd
+    from sunpy.net import Fido, attrs
 
     if filepath is None:
         filepath = os.getcwd()
 
     desired_time = pd.to_datetime(timestr, yearfirst=True)
     desired_time_plus_hour = desired_time + pd.Timedelta(hours=1)
 
@@ -630,15 +627,15 @@
 
     print(f"Downloaded file to:\n{file.data[0]}")
     return file.data[0]
 
 
 def construct_gongmap_filename(timestr, directory):
     """
-    Constructs a default filepath for 
+    Constructs a default filepath
     """
 
     yy = timestr[2:4]
     mm = timestr[5:7]
     dd = timestr[8:10]
     hh = timestr[11:13]
 
@@ -655,29 +652,30 @@
     if len(filepaths) == 1:
         print(f"Automatic file search based on given time found {filepaths[0]}")
         return filepaths[0]
     else:
         print(f"Automatic file search based on given time failed in directory {directory}")
         return directory
 
+
 def get_gong_map(time:str, filepath:str=None, autodownload=True):
     """
     A wrapper for functions load_gong_map() and download_gong_map().
     Returns a gong map if one is found or autodownload is True. If no map found and
     autodownload is False, then return None.
-    
+
     Parameters:
     -----------
     timestr : {str}
                 A pandas-compatible timestring, e.g., '2010-11-29 12:45'
     filepath : {str}, optional, default=None
                 The path to the gong map file with the name of the file, e.g., 'use/xyz/gong_maps/mrzqs211009t0814c2249_105.fits.gz'
                 If no filepath provided, use the current directory.
     autodownload : {bool}, optional, default=True
-                If file is not found, download it automatically. 
+                If file is not found, download it automatically.
     """
 
     # Try to construct a filename from current working directory and given datetime
     if not filepath or filepath[-8:] not in (".fits.gz"):
         filepath = construct_gongmap_filename(timestr=time, directory=filepath)
 
     try:
@@ -688,29 +686,7 @@
             print("Downloading...")
             new_filepath = download_gong_map(time, filepath=filepath)
             gong_map = load_gong_map(filepath=new_filepath)
         else:
             return None
 
     return gong_map
-
-
-def _isstreamlit():
-    """
-    Function to check whether python code is run within streamlit
-
-    Returns
-    -------
-    use_streamlit : boolean
-        True if code is run within streamlit, else False
-    """
-    # https://discuss.streamlit.io/t/how-to-check-if-code-is-run-inside-streamlit-and-not-e-g-ipython/23439
-    try:
-        from streamlit.runtime.scriptrunner import get_script_run_ctx
-        if not get_script_run_ctx():
-            use_streamlit = False
-        else:
-            use_streamlit = True
-    except ModuleNotFoundError:
-        use_streamlit = False
-    return use_streamlit
-
```

### Comparing `solarmach-0.2.1/solarmach/tests/test.py` & `solarmach-0.2.2/solarmach/tests/test.py`

 * *Files identical despite different names*

### Comparing `solarmach-0.2.1/solarmach.egg-info/PKG-INFO` & `solarmach-0.2.2/solarmach.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solarmach
-Version: 0.2.1
+Version: 0.2.2
 Summary: Multi-spacecraft longitudinal configuration plotter
 Home-page: https://github.com/jgieseler/solarmach
 Author: Jan Gieseler
 Author-email: jan.gieseler@utu.fi
 License: BSD 3-clause
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -104,41 +104,47 @@
    
    # obtain data as Pandas DataFrame
    display(sm.coord_table)
 
 .. image:: https://github.com/jgieseler/solarmach/raw/main/examples/solarmach.png
   :alt: Example output figure
   
-See `example notebook <https://github.com/jgieseler/solarmach/blob/main/examples/example.ipynb>`_ for all options!
+See example notebooks in next section for all options!
   
-Example Notebook
-----------------
+Example Notebooks
+-----------------
 
 **solarmach** can easily be run in a Jupyter Notebook. 
 
-- `Download example notebook <https://github.com/jgieseler/solarmach/raw/main/examples/example.ipynb>`_
-
-- Try it online: |binder|
-  
-.. |binder| image:: https://mybinder.org/badge_logo.svg
- :target: https://mybinder.org/v2/gh/jgieseler/solarmach/main?labpath=examples%2Fexample.ipynb
+- `Show simple example notebook <https://nbviewer.org/github/jgieseler/solarmach/blob/main/examples/example.ipynb>`_ |nbviewer1|
+ 
+- `Show extended example notebook <https://nbviewer.org/github/serpentine-h2020/serpentine/blob/main/notebooks/solarmach/solarmach.ipynb>`_ |nbviewer2| (provided by `SERPENTINE <https://serpentine-h2020.eu>`_ project)
+ 
+ 
+.. |nbviewer1| image:: https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg
+ :target: https://nbviewer.org/github/jgieseler/solarmach/blob/main/examples/example.ipynb
+ 
+.. |nbviewer2| image:: https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg
+ :target: https://nbviewer.org/github/serpentine-h2020/serpentine/blob/main/notebooks/solarmach/solarmach.ipynb
  
 Citation
 --------
 
 Please cite the following paper if you use **solarmach** in your publication:
 
 Gieseler, J., Dresing, N., Palmroos, C., von Forstner, J.L.F., Price, D.J., Vainio, R. et al. (2022).
 Solar-MACH: An open-source tool to analyze solar magnetic connection configurations. *Front. Astronomy Space Sci.* 9. `doi:10.3389/fspas.2022.1058810 <https://doi.org/10.3389/fspas.2022.1058810>`_ 
  
 Acknowledgements
 ----------------
  
 The Solar-MACH tool was originally developed at Kiel University, Germany and further discussed within the `ESA Heliophysics Archives USer (HAUS) <https://www.cosmos.esa.int/web/esdc/archives-user-groups/heliophysics>`_ group.
 
+This project has received funding from the European Union’s Horizon 2020 research and innovation programme under grant agreement No 101004159.
+
 Powered by: |matplotlib| |sunpy|
 
 .. |matplotlib| image:: https://matplotlib.org/stable/_static/logo2_compressed.svg
    :height: 25px
    :target: https://matplotlib.org
 .. |sunpy| image:: https://raw.githubusercontent.com/sunpy/sunpy-logo/master/generated/sunpy_logo_landscape.svg
    :height: 30px
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `solarmach-0.2.1/solarmach.egg-info/SOURCES.txt` & `solarmach-0.2.2/solarmach.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `solarmach-0.2.1/tox.ini` & `solarmach-0.2.2/tox.ini`

 * *Files identical despite different names*

