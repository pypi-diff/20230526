# Comparing `tmp/astro-synthesizer-0.0.3.tar.gz` & `tmp/astro-synthesizer-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro-synthesizer-0.0.3.tar", last modified: Wed May  3 10:41:09 2023, max compression
+gzip compressed data, was "astro-synthesizer-0.0.4.tar", last modified: Fri May 26 16:03:00 2023, max compression
```

## Comparing `astro-synthesizer-0.0.3.tar` & `astro-synthesizer-0.0.4.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 jz        (1000) jz        (1000)        0 2023-05-03 10:41:09.895515 astro-synthesizer-0.0.3/
--rw-rw-r--   0 jz        (1000) jz        (1000)    35149 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.3/LICENSE
--rw-rw-r--   0 jz        (1000) jz        (1000)    43841 2023-05-03 10:41:09.895515 astro-synthesizer-0.0.3/PKG-INFO
--rw-rw-r--   0 jz        (1000) jz        (1000)     2796 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.3/README.md
-drwxrwxr-x   0 jz        (1000) jz        (1000)        0 2023-05-03 10:41:09.887515 astro-synthesizer-0.0.3/astro_synthesizer.egg-info/
--rw-rw-r--   0 jz        (1000) jz        (1000)    43841 2023-05-03 10:41:09.000000 astro-synthesizer-0.0.3/astro_synthesizer.egg-info/PKG-INFO
--rw-rw-r--   0 jz        (1000) jz        (1000)     1191 2023-05-03 10:41:09.000000 astro-synthesizer-0.0.3/astro_synthesizer.egg-info/SOURCES.txt
--rw-rw-r--   0 jz        (1000) jz        (1000)        1 2023-05-03 10:41:09.000000 astro-synthesizer-0.0.3/astro_synthesizer.egg-info/dependency_links.txt
--rw-rw-r--   0 jz        (1000) jz        (1000)       63 2023-05-03 10:41:09.000000 astro-synthesizer-0.0.3/astro_synthesizer.egg-info/entry_points.txt
--rw-rw-r--   0 jz        (1000) jz        (1000)       78 2023-05-03 10:41:09.000000 astro-synthesizer-0.0.3/astro_synthesizer.egg-info/requires.txt
--rw-rw-r--   0 jz        (1000) jz        (1000)       12 2023-05-03 10:41:09.000000 astro-synthesizer-0.0.3/astro_synthesizer.egg-info/top_level.txt
--rw-rw-r--   0 jz        (1000) jz        (1000)      864 2023-05-03 10:39:54.000000 astro-synthesizer-0.0.3/pyproject.toml
--rw-rw-r--   0 jz        (1000) jz        (1000)       38 2023-05-03 10:41:09.895515 astro-synthesizer-0.0.3/setup.cfg
--rw-rw-r--   0 jz        (1000) jz        (1000)       38 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.3/setup.py
-drwxrwxr-x   0 jz        (1000) jz        (1000)        0 2023-05-03 10:41:09.887515 astro-synthesizer-0.0.3/synthesizer/
--rw-rw-r--   0 jz        (1000) jz        (1000)      919 2023-05-03 10:40:23.000000 astro-synthesizer-0.0.3/synthesizer/__main__.py
-drwxrwxr-x   0 jz        (1000) jz        (1000)        0 2023-05-03 10:41:09.887515 astro-synthesizer-0.0.3/synthesizer/dustmixer/
--rw-rw-r--   0 jz        (1000) jz        (1000)       28 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.3/synthesizer/dustmixer/__init__.py
--rw-rw-r--   0 jz        (1000) jz        (1000)     4887 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.3/synthesizer/dustmixer/bhcoat.py
--rw-rw-r--   0 jz        (1000) jz        (1000)     5773 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.3/synthesizer/dustmixer/bhmie.py
--rw-rw-r--   0 jz        (1000) jz        (1000)    34563 2023-04-26 10:11:51.000000 astro-synthesizer-0.0.3/synthesizer/dustmixer/dustmixer.py
-drwxrwxr-x   0 jz        (1000) jz        (1000)        0 2023-05-03 10:41:09.891515 astro-synthesizer-0.0.3/synthesizer/gridder/
--rw-rw-r--   0 jz        (1000) jz        (1000)      165 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.3/synthesizer/gridder/__init__.py
--rw-rw-r--   0 jz        (1000) jz        (1000)     5170 2023-04-13 15:55:46.000000 astro-synthesizer-0.0.3/synthesizer/gridder/amr_reader.py
--rw-rw-r--   0 jz        (1000) jz        (1000)    20285 2023-04-14 07:03:56.000000 astro-synthesizer-0.0.3/synthesizer/gridder/analytical.py
--rw-rw-r--   0 jz        (1000) jz        (1000)      819 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.3/synthesizer/gridder/custom_model.py
--rw-rw-r--   0 jz        (1000) jz        (1000)    26881 2023-05-03 10:40:33.000000 astro-synthesizer-0.0.3/synthesizer/gridder/gridder.py
--rw-rw-r--   0 jz        (1000) jz        (1000)    13982 2023-04-14 08:05:22.000000 astro-synthesizer-0.0.3/synthesizer/gridder/models.py
--rw-rw-r--   0 jz        (1000) jz        (1000)    12533 2023-04-08 22:10:38.000000 astro-synthesizer-0.0.3/synthesizer/gridder/sph_reader.py
--rw-rw-r--   0 jz        (1000) jz        (1000)     3922 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.3/synthesizer/gridder/vector_field.py
--rw-rw-r--   0 jz        (1000) jz        (1000)    14290 2023-05-03 10:40:10.000000 astro-synthesizer-0.0.3/synthesizer/parser.py
--rw-rw-r--   0 jz        (1000) jz        (1000)    44280 2023-05-03 10:40:31.000000 astro-synthesizer-0.0.3/synthesizer/pipeline.py
-drwxrwxr-x   0 jz        (1000) jz        (1000)        0 2023-05-03 10:41:09.891515 astro-synthesizer-0.0.3/synthesizer/raytrace/
--rw-rw-r--   0 jz        (1000) jz        (1000)       29 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.3/synthesizer/raytrace/__init__.py
--rw-rw-r--   0 jz        (1000) jz        (1000)    15204 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.3/synthesizer/raytrace/radmc3d.py
-drwxrwxr-x   0 jz        (1000) jz        (1000)        0 2023-05-03 10:41:09.891515 astro-synthesizer-0.0.3/synthesizer/synobs/
--rw-rw-r--   0 jz        (1000) jz        (1000)       66 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.3/synthesizer/synobs/__init__.py
--rw-rw-r--   0 jz        (1000) jz        (1000)    19644 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.3/synthesizer/synobs/scripter.py
--rw-rw-r--   0 jz        (1000) jz        (1000)     2861 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.3/synthesizer/synobs/syn_imager.py
-drwxrwxr-x   0 jz        (1000) jz        (1000)        0 2023-05-03 10:41:09.895515 astro-synthesizer-0.0.3/synthesizer/synobs/templates/
--rw-rw-r--   0 jz        (1000) jz        (1000)     1519 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.3/synthesizer/synobs/templates/alma_1.3mm.py
--rw-rw-r--   0 jz        (1000) jz        (1000)     1698 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.3/synthesizer/synobs/templates/alma_1.3mm_pol.py
--rw-rw-r--   0 jz        (1000) jz        (1000)     1692 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.3/synthesizer/synobs/templates/alma_3mm.py
--rw-rw-r--   0 jz        (1000) jz        (1000)     1619 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.3/synthesizer/synobs/templates/vla_18mm.py
--rw-rw-r--   0 jz        (1000) jz        (1000)     1588 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.3/synthesizer/synobs/templates/vla_7mm.py
--rw-rw-r--   0 jz        (1000) jz        (1000)     1597 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.3/synthesizer/synobs/templates/vla_9mm.py
--rw-rw-r--   0 jz        (1000) jz        (1000)    27401 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.3/synthesizer/utils.py
+drwxrwxr-x   0 jz        (1000) jz        (1000)        0 2023-05-26 16:03:00.436069 astro-synthesizer-0.0.4/
+-rw-rw-r--   0 jz        (1000) jz        (1000)    35149 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.4/LICENSE
+-rw-rw-r--   0 jz        (1000) jz        (1000)    43841 2023-05-26 16:03:00.436069 astro-synthesizer-0.0.4/PKG-INFO
+-rw-rw-r--   0 jz        (1000) jz        (1000)     2796 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.4/README.md
+drwxrwxr-x   0 jz        (1000) jz        (1000)        0 2023-05-26 16:03:00.428069 astro-synthesizer-0.0.4/astro_synthesizer.egg-info/
+-rw-rw-r--   0 jz        (1000) jz        (1000)    43841 2023-05-26 16:03:00.000000 astro-synthesizer-0.0.4/astro_synthesizer.egg-info/PKG-INFO
+-rw-rw-r--   0 jz        (1000) jz        (1000)     1191 2023-05-26 16:03:00.000000 astro-synthesizer-0.0.4/astro_synthesizer.egg-info/SOURCES.txt
+-rw-rw-r--   0 jz        (1000) jz        (1000)        1 2023-05-26 16:03:00.000000 astro-synthesizer-0.0.4/astro_synthesizer.egg-info/dependency_links.txt
+-rw-rw-r--   0 jz        (1000) jz        (1000)       63 2023-05-26 16:03:00.000000 astro-synthesizer-0.0.4/astro_synthesizer.egg-info/entry_points.txt
+-rw-rw-r--   0 jz        (1000) jz        (1000)       78 2023-05-26 16:03:00.000000 astro-synthesizer-0.0.4/astro_synthesizer.egg-info/requires.txt
+-rw-rw-r--   0 jz        (1000) jz        (1000)       12 2023-05-26 16:03:00.000000 astro-synthesizer-0.0.4/astro_synthesizer.egg-info/top_level.txt
+-rw-rw-r--   0 jz        (1000) jz        (1000)      864 2023-05-26 16:02:24.000000 astro-synthesizer-0.0.4/pyproject.toml
+-rw-rw-r--   0 jz        (1000) jz        (1000)       38 2023-05-26 16:03:00.436069 astro-synthesizer-0.0.4/setup.cfg
+-rw-rw-r--   0 jz        (1000) jz        (1000)       38 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.4/setup.py
+drwxrwxr-x   0 jz        (1000) jz        (1000)        0 2023-05-26 16:03:00.432069 astro-synthesizer-0.0.4/synthesizer/
+-rw-rw-r--   0 jz        (1000) jz        (1000)      919 2023-05-26 16:02:41.000000 astro-synthesizer-0.0.4/synthesizer/__main__.py
+drwxrwxr-x   0 jz        (1000) jz        (1000)        0 2023-05-26 16:03:00.432069 astro-synthesizer-0.0.4/synthesizer/dustmixer/
+-rw-rw-r--   0 jz        (1000) jz        (1000)       28 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.4/synthesizer/dustmixer/__init__.py
+-rw-rw-r--   0 jz        (1000) jz        (1000)     4887 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.4/synthesizer/dustmixer/bhcoat.py
+-rw-rw-r--   0 jz        (1000) jz        (1000)     5773 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.4/synthesizer/dustmixer/bhmie.py
+-rw-rw-r--   0 jz        (1000) jz        (1000)    34563 2023-05-13 12:49:17.000000 astro-synthesizer-0.0.4/synthesizer/dustmixer/dustmixer.py
+drwxrwxr-x   0 jz        (1000) jz        (1000)        0 2023-05-26 16:03:00.432069 astro-synthesizer-0.0.4/synthesizer/gridder/
+-rw-rw-r--   0 jz        (1000) jz        (1000)      165 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.4/synthesizer/gridder/__init__.py
+-rw-rw-r--   0 jz        (1000) jz        (1000)     5170 2023-04-13 15:55:46.000000 astro-synthesizer-0.0.4/synthesizer/gridder/amr_reader.py
+-rw-rw-r--   0 jz        (1000) jz        (1000)    20279 2023-05-22 09:37:54.000000 astro-synthesizer-0.0.4/synthesizer/gridder/analytical.py
+-rw-rw-r--   0 jz        (1000) jz        (1000)      819 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.4/synthesizer/gridder/custom_model.py
+-rw-rw-r--   0 jz        (1000) jz        (1000)    26984 2023-05-22 09:37:28.000000 astro-synthesizer-0.0.4/synthesizer/gridder/gridder.py
+-rw-rw-r--   0 jz        (1000) jz        (1000)    13982 2023-04-14 08:05:22.000000 astro-synthesizer-0.0.4/synthesizer/gridder/models.py
+-rw-rw-r--   0 jz        (1000) jz        (1000)    12533 2023-04-08 22:10:38.000000 astro-synthesizer-0.0.4/synthesizer/gridder/sph_reader.py
+-rw-rw-r--   0 jz        (1000) jz        (1000)     3922 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.4/synthesizer/gridder/vector_field.py
+-rw-rw-r--   0 jz        (1000) jz        (1000)    14521 2023-05-26 16:02:48.000000 astro-synthesizer-0.0.4/synthesizer/parser.py
+-rw-rw-r--   0 jz        (1000) jz        (1000)    45011 2023-05-22 09:45:53.000000 astro-synthesizer-0.0.4/synthesizer/pipeline.py
+drwxrwxr-x   0 jz        (1000) jz        (1000)        0 2023-05-26 16:03:00.432069 astro-synthesizer-0.0.4/synthesizer/raytrace/
+-rw-rw-r--   0 jz        (1000) jz        (1000)       29 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.4/synthesizer/raytrace/__init__.py
+-rw-rw-r--   0 jz        (1000) jz        (1000)    15204 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.4/synthesizer/raytrace/radmc3d.py
+drwxrwxr-x   0 jz        (1000) jz        (1000)        0 2023-05-26 16:03:00.432069 astro-synthesizer-0.0.4/synthesizer/synobs/
+-rw-rw-r--   0 jz        (1000) jz        (1000)       66 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.4/synthesizer/synobs/__init__.py
+-rw-rw-r--   0 jz        (1000) jz        (1000)    19644 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.4/synthesizer/synobs/scripter.py
+-rw-rw-r--   0 jz        (1000) jz        (1000)     2861 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.4/synthesizer/synobs/syn_imager.py
+drwxrwxr-x   0 jz        (1000) jz        (1000)        0 2023-05-26 16:03:00.436069 astro-synthesizer-0.0.4/synthesizer/synobs/templates/
+-rw-rw-r--   0 jz        (1000) jz        (1000)     1519 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.4/synthesizer/synobs/templates/alma_1.3mm.py
+-rw-rw-r--   0 jz        (1000) jz        (1000)     1698 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.4/synthesizer/synobs/templates/alma_1.3mm_pol.py
+-rw-rw-r--   0 jz        (1000) jz        (1000)     1692 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.4/synthesizer/synobs/templates/alma_3mm.py
+-rw-rw-r--   0 jz        (1000) jz        (1000)     1619 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.4/synthesizer/synobs/templates/vla_18mm.py
+-rw-rw-r--   0 jz        (1000) jz        (1000)     1588 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.4/synthesizer/synobs/templates/vla_7mm.py
+-rw-rw-r--   0 jz        (1000) jz        (1000)     1597 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.4/synthesizer/synobs/templates/vla_9mm.py
+-rw-rw-r--   0 jz        (1000) jz        (1000)    27401 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.4/synthesizer/utils.py
```

### Comparing `astro-synthesizer-0.0.3/LICENSE` & `astro-synthesizer-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `astro-synthesizer-0.0.3/PKG-INFO` & `astro-synthesizer-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-synthesizer
-Version: 0.0.3
+Version: 0.0.4
 Summary: Generate astronomical synthetic observations from the command-line 
 Author-email: Joaquin Zamponi <jzamponi@mpe.mpg.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `astro-synthesizer-0.0.3/README.md` & `astro-synthesizer-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `astro-synthesizer-0.0.3/astro_synthesizer.egg-info/PKG-INFO` & `astro-synthesizer-0.0.4/astro_synthesizer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-synthesizer
-Version: 0.0.3
+Version: 0.0.4
 Summary: Generate astronomical synthetic observations from the command-line 
 Author-email: Joaquin Zamponi <jzamponi@mpe.mpg.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `astro-synthesizer-0.0.3/astro_synthesizer.egg-info/SOURCES.txt` & `astro-synthesizer-0.0.4/astro_synthesizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astro-synthesizer-0.0.3/pyproject.toml` & `astro-synthesizer-0.0.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "astro-synthesizer"
-version = "0.0.3"
+version = "0.0.4"
 description = "Generate astronomical synthetic observations from the command-line "
 readme = "README.md"
 authors = [{ name = "Joaquin Zamponi", email = "jzamponi@mpe.mpg.de" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `astro-synthesizer-0.0.3/synthesizer/__main__.py` & `astro-synthesizer-0.0.4/synthesizer/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,11 +21,11 @@
                     python3-matplotlib, python3-astropy, python3-mayavi,
                     python3-radmc3dPy
 
 """
 
 from synthesizer import parser
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 if __name__ == "__main__":
     parser.parser()
```

### Comparing `astro-synthesizer-0.0.3/synthesizer/dustmixer/bhcoat.py` & `astro-synthesizer-0.0.4/synthesizer/dustmixer/bhcoat.py`

 * *Files identical despite different names*

### Comparing `astro-synthesizer-0.0.3/synthesizer/dustmixer/bhmie.py` & `astro-synthesizer-0.0.4/synthesizer/dustmixer/bhmie.py`

 * *Files identical despite different names*

### Comparing `astro-synthesizer-0.0.3/synthesizer/dustmixer/dustmixer.py` & `astro-synthesizer-0.0.4/synthesizer/dustmixer/dustmixer.py`

 * *Files identical despite different names*

### Comparing `astro-synthesizer-0.0.3/synthesizer/gridder/amr_reader.py` & `astro-synthesizer-0.0.4/synthesizer/gridder/amr_reader.py`

 * *Files identical despite different names*

### Comparing `astro-synthesizer-0.0.3/synthesizer/gridder/analytical.py` & `astro-synthesizer-0.0.4/synthesizer/gridder/analytical.py`

 * *Files 1% similar despite different names*

```diff
@@ -275,15 +275,15 @@
             for iz in range(self.ncells):
                 for iy in range(self.ncells):
                     for ix in range(self.ncells):
                         f.write(f'{self.vfield.vx[ix, iy, iz]:13.6e} ' +\
                                 f'{self.vfield.vy[ix, iy, iz]:13.6e} ' +\
                                 f'{self.vfield.vz[ix, iy, iz]:13.6e}\n')
 
-    def plot_midplane(self, field, data=None):
+    def plot_2d(self, field, data=None):
         """ Plot the density midplane at z=0 using Matplotlib """
         try:
             from matplotlib.colors import LogNorm
             utils.print_(f'Plotting the density grid midplane')
             plt.rcParams['xtick.direction'] = 'in'
             plt.rcParams['ytick.direction'] = 'in'
             plt.rcParams['xtick.top'] = True
```

### Comparing `astro-synthesizer-0.0.3/synthesizer/gridder/custom_model.py` & `astro-synthesizer-0.0.4/synthesizer/gridder/custom_model.py`

 * *Files identical despite different names*

### Comparing `astro-synthesizer-0.0.3/synthesizer/gridder/gridder.py` & `astro-synthesizer-0.0.4/synthesizer/gridder/gridder.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 from synthesizer.gridder.amr_reader  import *
 from synthesizer import utils
 
 
 class Grid():
     """ 
         Base class for different grid geometries.
+
+        To Do: Abstract tecartesian and spherical grid object methods 
+               using this base class
     """
     pass
 
 class CartesianGrid(Grid):
     def __init__(self, ncells, bbox=None, rout=None, nspec=1, csubl=0, 
             sootline=300, g2d=100, temp=False, vfield=None):
         """ 
@@ -475,15 +478,15 @@
             for iz in range(self.nx):
                 for iy in range(self.ny):
                     for ix in range(self.nz):
                         f.write(f'{self.vfield.vx[ix, iy, iz]:13.6e} ' +\
                                 f'{self.vfield.vy[ix, iy, iz]:13.6e} ' +\
                                 f'{self.vfield.vz[ix, iy, iz]:13.6e}\n')
 
-    def plot_midplane(self, field, data=None):
+    def plot_2d(self, field, data=None):
         """ Plot the density midplane at z=0 using Matplotlib """
         try:
             from matplotlib.colors import LogNorm
             utils.print_(f'Plotting the density grid midplane')
             plt.rcParams['xtick.direction'] = 'in'
             plt.rcParams['ytick.direction'] = 'in'
             plt.rcParams['xtick.top'] = True
```

### Comparing `astro-synthesizer-0.0.3/synthesizer/gridder/models.py` & `astro-synthesizer-0.0.4/synthesizer/gridder/models.py`

 * *Files identical despite different names*

### Comparing `astro-synthesizer-0.0.3/synthesizer/gridder/sph_reader.py` & `astro-synthesizer-0.0.4/synthesizer/gridder/sph_reader.py`

 * *Files identical despite different names*

### Comparing `astro-synthesizer-0.0.3/synthesizer/gridder/vector_field.py` & `astro-synthesizer-0.0.4/synthesizer/gridder/vector_field.py`

 * *Files identical despite different names*

### Comparing `astro-synthesizer-0.0.3/synthesizer/parser.py` & `astro-synthesizer-0.0.4/synthesizer/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,14 +110,17 @@
 
     parser.add_argument('--nang', action='store', type=int, default=181,
         help='Number of scattering angles used to sample the dust efficiencies')
 
     parser.add_argument('--show-opacity', action='store_true', default=False, 
         help='Plot the resulting dust opacities.')
 
+    parser.add_argument('--show-dust-eff', action='store_true', default=False, 
+        help='Plot the resulting dust efficiencies for a single grain size.')
+
     parser.add_argument('--show-nk', action='store_true', default=False, 
         help='Plot the input dust optical constants.')
 
     parser.add_argument('--nopb', action='store_true', default=False, 
         help='Disable printing of an opacity progressbar. ' +\
             'Useful when logging to file. ')
 
@@ -237,15 +240,15 @@
 
     parser.add_argument('-ow', '--overwrite', action='store_true', 
         default=False, help='Overwrite opacities, RADMC3D and CASA input files')
 
     parser.add_argument('--quiet', action='store_true', default=False,
         help='Disable verbosity. Do not output anything.')
 
-    parser.add_argument('--version', action='version', version='%(prog)s 0.0.3')
+    parser.add_argument('--version', action='version', version='%(prog)s 0.0.4')
 
 
 
     # Store the command-line given arguments
     cli = parser.parse_args()
 
     # Initialize the pipeline
@@ -269,15 +272,18 @@
             tau=cli.tau, show_particles=cli.show_particles, 
             alignment=cli.alignment,
         )
 
     # Generate the dust opacity tables
     if cli.opacity:
         pipeline.dustmixer(
-            show_nk=cli.show_nk, show_opac=cli.show_opacity, pb=not cli.nopb
+            show_nk=cli.show_nk, 
+            show_dust_eff=cli.show_dust_eff, 
+            show_opac=cli.show_opacity, 
+            pb=not cli.nopb
         )
 
     # Run a thermal Monte-Carlo
     if cli.monte_carlo:
         pipeline.monte_carlo(nphot=cli.nphot, radmc3d_cmds=cli.radmc3d)
 
     # Run a ray-tracing on the new grid and generate an image
```

### Comparing `astro-synthesizer-0.0.3/synthesizer/pipeline.py` & `astro-synthesizer-0.0.4/synthesizer/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,19 +218,19 @@
             self.grid.write_temperature_file()
 
         if vector_field is not None or alignment:
             self.grid.write_vector_field(morphology=vector_field)
 
         # Plot the density midplane
         if show_2d:
-            self.grid.plot_midplane('density')
+            self.grid.plot_2d('density')
 
         # Plot the temperature midplane
         if show_2d and temperature:
-            self.grid.plot_midplane('temperature')
+            self.grid.plot_2d('temperature')
 
         # Render the density volume in 3D using Mayavi
         if show_3d:
             self.grid.plot_3d('density', tau=tau)
 
         # Render the temperature volume in 3D using Mayavi
         if show_3d and temperature:
@@ -251,15 +251,21 @@
                 self.grid.render(dust_temperature=True)
 
         # Register the pipeline step 
         self.steps.append('create_grid')
 
 
     @utils.elapsed_time
-    def dustmixer(self, show_nk=False, pb=True, show_opac=False, savefig=None):
+    def dustmixer(self, 
+            show_nk=False, 
+            show_dust_eff=False, 
+            show_opac=False, 
+            pb=True, 
+            savefig=None
+        ):
         """
             Call dustmixer to generate dust opacity tables. 
             New dust materials can be manually defined here if desired.
         """
 
         print('')
         utils.print_("Calculating dust opacities ...\n", bold=True)
@@ -380,14 +386,17 @@
             except Exception as e:
                 utils.print_(e, red=True)
                 raise ValueError(f'Material = {self.material} not found.')
 
         if show_opac or savefig is not None:
             mix.plot_opacities(show=show_opac, savefig=savefig)
 
+        if show_dust_eff:
+            mix.plot_efficiencies()
+
         mix.write_opacity_file(name=self._get_opac_name(self.csubl))
 
         if self.alignment:
             mix.write_align_factor(name=self._get_opac_name(self.csubl))
 
         # Store the current dust opacity in the pipeline instance
         self.kappa = mix._get_kappa_at_lam(self.lam) 
@@ -665,15 +674,16 @@
         else:
             self.sizeau = int(2 * self._get_bbox() * u.cm.to(u.au))
 
         # Explicitly the model rotate by 180.
         # Only for the current model. This line should be later removed.
         self.incl = 180 - int(self.incl)
 
-        # To do: What's the diff. between passing noscat and setting scatmode=0
+        # To do: Double check that this is correct. noscat does include 
+        # k_sca in the extincion opacity but maybe scatmode=0 doesn't 
         if noscat: self.scatmode = 0
 
         # Generate a 2D optical depth map
         if self.tau:
             self.plot_tau(show)
             
         # Set the RADMC3D command by concatenating options
@@ -969,14 +979,16 @@
 
         # Integrate density weigthed by the dust opacity along the line-of-sight
         dl = np.diff(amr)[0]
         nx = int(np.cbrt(rho.size))
         rho = rho.reshape((nx, nx, nx))
         tau2d = np.sum(rho * self._get_opacity() * dl, axis=0).T
 
+        # To do: implement this for cases with two or more dust populations
+
         if show:
             plt.rcParams['font.family'] = 'Times New Roman'
             plt.rcParams['xtick.direction'] = 'in'
             plt.rcParams['ytick.direction'] = 'in'
             plt.rcParams['xtick.top'] = True
             plt.rcParams['ytick.right'] = True
             plt.rcParams['xtick.minor.visible'] = True
@@ -993,37 +1005,51 @@
     @utils.elapsed_time
     def plot_grid_2d(self, temp=False):
         """ Plot the grid's density and temperature midplanes from files,
             in case they are not currently available from pipeline.grid
         """
         utils.file_exists('dust_density.inp')
         utils.print_('Reading density from dust_density.inp')
-        dens = np.loadtxt('dust_density.inp', skiprows=3).T
+        dens = np.loadtxt('dust_density.inp').T
+        ncells = int(dens[1])
+        nspec = int(dens[2])
+        if nspec == 1:
+            dens = dens[3:]
+        else: 
+            utils.print_('Found two dust species, I plot only the first one')
+            dens = dens[3: ncells+3]
         nx = int(np.cbrt(dens.size))
         dens = dens.reshape((nx, nx, nx))
         bbox = self._get_bbox()
         grid = gridder.CartesianGrid(nx, bbox)
-        grid.plot_midplane('density', data=dens)
+        grid.plot_2d('density', data=dens)
 
         if temp: 
             utils.file_exists('dust_temperature.dat')
             utils.print_('Reading temperature from dust_temperature.dat')
             temp = np.loadtxt('dust_temperature.dat', skiprows=3)
             temp = temp.reshape((nx, nx, nx))
             grid = gridder.CartesianGrid(nx, bbox)
-            grid.plot_midplane('temperature', data=temp)
+            grid.plot_2d('temperature', data=temp)
         
     @utils.elapsed_time
     def plot_grid_3d(self, temp=False):
         """ Render the grid's density and temperature in 3D from files,
             in case they are not currently available from pipeline.grid
         """
         utils.file_exists('dust_density.inp')
         utils.print_('Reading density from dust_density.inp')
-        dens = np.loadtxt('dust_density.inp', skiprows=3).T
+        dens = np.loadtxt('dust_density.inp').T
+        ncells = int(dens[1])
+        nspec = int(dens[2])
+        if nspec == 1:
+            dens = dens[3:]
+        else: 
+            utils.print_('Found two dust species, I plot only the first one')
+            dens = dens[3: ncells+3]
         nx = int(np.cbrt(dens.size))
         dens = dens.reshape((nx, nx, nx))
         bbox = self._get_bbox()
         utils.print_(r'Rendering a box of {nx}^3 pixels')
         grid = gridder.CartesianGrid(nx, bbox)
         grid.plot_3d('density', data=dens)
```

### Comparing `astro-synthesizer-0.0.3/synthesizer/raytrace/radmc3d.py` & `astro-synthesizer-0.0.4/synthesizer/raytrace/radmc3d.py`

 * *Files identical despite different names*

### Comparing `astro-synthesizer-0.0.3/synthesizer/synobs/scripter.py` & `astro-synthesizer-0.0.4/synthesizer/synobs/scripter.py`

 * *Files identical despite different names*

### Comparing `astro-synthesizer-0.0.3/synthesizer/synobs/syn_imager.py` & `astro-synthesizer-0.0.4/synthesizer/synobs/syn_imager.py`

 * *Files identical despite different names*

### Comparing `astro-synthesizer-0.0.3/synthesizer/synobs/templates/alma_1.3mm.py` & `astro-synthesizer-0.0.4/synthesizer/synobs/templates/alma_1.3mm.py`

 * *Files identical despite different names*

### Comparing `astro-synthesizer-0.0.3/synthesizer/synobs/templates/alma_1.3mm_pol.py` & `astro-synthesizer-0.0.4/synthesizer/synobs/templates/alma_1.3mm_pol.py`

 * *Files identical despite different names*

### Comparing `astro-synthesizer-0.0.3/synthesizer/synobs/templates/alma_3mm.py` & `astro-synthesizer-0.0.4/synthesizer/synobs/templates/alma_3mm.py`

 * *Files identical despite different names*

### Comparing `astro-synthesizer-0.0.3/synthesizer/synobs/templates/vla_18mm.py` & `astro-synthesizer-0.0.4/synthesizer/synobs/templates/vla_18mm.py`

 * *Files identical despite different names*

### Comparing `astro-synthesizer-0.0.3/synthesizer/synobs/templates/vla_7mm.py` & `astro-synthesizer-0.0.4/synthesizer/synobs/templates/vla_7mm.py`

 * *Files identical despite different names*

### Comparing `astro-synthesizer-0.0.3/synthesizer/synobs/templates/vla_9mm.py` & `astro-synthesizer-0.0.4/synthesizer/synobs/templates/vla_9mm.py`

 * *Files identical despite different names*

### Comparing `astro-synthesizer-0.0.3/synthesizer/utils.py` & `astro-synthesizer-0.0.4/synthesizer/utils.py`

 * *Files identical despite different names*

