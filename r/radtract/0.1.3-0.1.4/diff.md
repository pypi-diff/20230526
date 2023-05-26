# Comparing `tmp/radtract-0.1.3.tar.gz` & `tmp/radtract-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radtract-0.1.3.tar", last modified: Wed May 24 07:48:49 2023, max compression
+gzip compressed data, was "radtract-0.1.4.tar", last modified: Fri May 26 08:20:21 2023, max compression
```

## Comparing `radtract-0.1.3.tar` & `radtract-0.1.4.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxr-x   0 neher     (1000) neher     (1000)        0 2023-05-24 07:48:49.939323 radtract-0.1.3/
-drwxrwxr-x   0 neher     (1000) neher     (1000)        0 2023-05-24 07:48:49.939323 radtract-0.1.3/LICENSES/
--rw-rw-r--   0 neher     (1000) neher     (1000)    10280 2023-05-24 07:39:53.000000 radtract-0.1.3/LICENSES/Apache-2.0.txt
--rw-rw-r--   0 neher     (1000) neher     (1000)      154 2023-05-24 07:39:53.000000 radtract-0.1.3/MANIFEST.in
--rw-rw-r--   0 neher     (1000) neher     (1000)    13004 2023-05-24 07:48:49.939323 radtract-0.1.3/PKG-INFO
--rw-rw-r--   0 neher     (1000) neher     (1000)     1736 2023-05-24 07:39:53.000000 radtract-0.1.3/README.md
--rw-rw-r--   0 neher     (1000) neher     (1000)     1098 2023-05-24 07:47:55.000000 radtract-0.1.3/pyproject.toml
-drwxrwxr-x   0 neher     (1000) neher     (1000)        0 2023-05-24 07:48:49.939323 radtract-0.1.3/radtract/
--rw-rw-r--   0 neher     (1000) neher     (1000)      357 2023-05-24 07:42:57.000000 radtract-0.1.3/radtract/__init__.py
--rw-rw-r--   0 neher     (1000) neher     (1000)    12193 2023-05-24 07:39:53.000000 radtract-0.1.3/radtract/features.py
--rw-rw-r--   0 neher     (1000) neher     (1000)    28575 2023-05-24 07:39:53.000000 radtract-0.1.3/radtract/parcellation.py
--rw-rw-r--   0 neher     (1000) neher     (1000)     3626 2023-05-24 07:39:53.000000 radtract-0.1.3/radtract/pyrad.yaml
-drwxrwxr-x   0 neher     (1000) neher     (1000)        0 2023-05-24 07:48:49.939323 radtract-0.1.3/radtract.egg-info/
--rw-rw-r--   0 neher     (1000) neher     (1000)    13004 2023-05-24 07:48:49.000000 radtract-0.1.3/radtract.egg-info/PKG-INFO
--rw-rw-r--   0 neher     (1000) neher     (1000)      364 2023-05-24 07:48:49.000000 radtract-0.1.3/radtract.egg-info/SOURCES.txt
--rw-rw-r--   0 neher     (1000) neher     (1000)        1 2023-05-24 07:48:49.000000 radtract-0.1.3/radtract.egg-info/dependency_links.txt
--rw-rw-r--   0 neher     (1000) neher     (1000)      110 2023-05-24 07:48:49.000000 radtract-0.1.3/radtract.egg-info/entry_points.txt
--rw-rw-r--   0 neher     (1000) neher     (1000)       77 2023-05-24 07:48:49.000000 radtract-0.1.3/radtract.egg-info/requires.txt
--rw-rw-r--   0 neher     (1000) neher     (1000)        9 2023-05-24 07:48:49.000000 radtract-0.1.3/radtract.egg-info/top_level.txt
--rw-rw-r--   0 neher     (1000) neher     (1000)       38 2023-05-24 07:48:49.939323 radtract-0.1.3/setup.cfg
-drwxrwxr-x   0 neher     (1000) neher     (1000)        0 2023-05-24 07:48:49.939323 radtract-0.1.3/tests/
--rw-rw-r--   0 neher     (1000) neher     (1000)     4930 2023-05-24 07:39:54.000000 radtract-0.1.3/tests/test_radtract.py
+drwxrwxr-x   0 neher     (1000) neher     (1000)        0 2023-05-26 08:20:21.110918 radtract-0.1.4/
+drwxrwxr-x   0 neher     (1000) neher     (1000)        0 2023-05-26 08:20:21.110918 radtract-0.1.4/LICENSES/
+-rw-rw-r--   0 neher     (1000) neher     (1000)    10280 2023-05-24 07:39:53.000000 radtract-0.1.4/LICENSES/Apache-2.0.txt
+-rw-rw-r--   0 neher     (1000) neher     (1000)      154 2023-05-24 07:39:53.000000 radtract-0.1.4/MANIFEST.in
+-rw-rw-r--   0 neher     (1000) neher     (1000)    15632 2023-05-26 08:20:21.110918 radtract-0.1.4/PKG-INFO
+-rw-rw-r--   0 neher     (1000) neher     (1000)     4157 2023-05-26 08:18:16.000000 radtract-0.1.4/README.md
+-rw-rw-r--   0 neher     (1000) neher     (1000)     1393 2023-05-26 08:11:23.000000 radtract-0.1.4/pyproject.toml
+drwxrwxr-x   0 neher     (1000) neher     (1000)        0 2023-05-26 08:20:21.110918 radtract-0.1.4/radtract/
+-rw-rw-r--   0 neher     (1000) neher     (1000)      357 2023-05-26 08:11:23.000000 radtract-0.1.4/radtract/__init__.py
+-rw-rw-r--   0 neher     (1000) neher     (1000)    12193 2023-05-24 07:39:53.000000 radtract-0.1.4/radtract/features.py
+-rw-rw-r--   0 neher     (1000) neher     (1000)    22994 2023-05-24 10:34:33.000000 radtract-0.1.4/radtract/parcellation.py
+-rw-rw-r--   0 neher     (1000) neher     (1000)     3626 2023-05-24 07:39:53.000000 radtract-0.1.4/radtract/pyrad.yaml
+-rw-rw-r--   0 neher     (1000) neher     (1000)     6925 2023-05-24 10:41:28.000000 radtract-0.1.4/radtract/tractdensity.py
+drwxrwxr-x   0 neher     (1000) neher     (1000)        0 2023-05-26 08:20:21.110918 radtract-0.1.4/radtract.egg-info/
+-rw-rw-r--   0 neher     (1000) neher     (1000)    15632 2023-05-26 08:20:21.000000 radtract-0.1.4/radtract.egg-info/PKG-INFO
+-rw-rw-r--   0 neher     (1000) neher     (1000)      389 2023-05-26 08:20:21.000000 radtract-0.1.4/radtract.egg-info/SOURCES.txt
+-rw-rw-r--   0 neher     (1000) neher     (1000)        1 2023-05-26 08:20:21.000000 radtract-0.1.4/radtract.egg-info/dependency_links.txt
+-rw-rw-r--   0 neher     (1000) neher     (1000)      152 2023-05-26 08:20:21.000000 radtract-0.1.4/radtract.egg-info/entry_points.txt
+-rw-rw-r--   0 neher     (1000) neher     (1000)       77 2023-05-26 08:20:21.000000 radtract-0.1.4/radtract.egg-info/requires.txt
+-rw-rw-r--   0 neher     (1000) neher     (1000)        9 2023-05-26 08:20:21.000000 radtract-0.1.4/radtract.egg-info/top_level.txt
+-rw-rw-r--   0 neher     (1000) neher     (1000)       38 2023-05-26 08:20:21.110918 radtract-0.1.4/setup.cfg
+drwxrwxr-x   0 neher     (1000) neher     (1000)        0 2023-05-26 08:20:21.110918 radtract-0.1.4/tests/
+-rw-rw-r--   0 neher     (1000) neher     (1000)     4928 2023-05-26 08:11:23.000000 radtract-0.1.4/tests/test_radtract.py
```

### Comparing `radtract-0.1.3/LICENSES/Apache-2.0.txt` & `radtract-0.1.4/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `radtract-0.1.3/pyproject.toml` & `radtract-0.1.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -4,43 +4,53 @@
 
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "radtract"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
-  { name="Peter Neher", email="p.neher@dkfz.de" },
+  { name="Peter Neher", email="p.neher@dkfz-heidelberg.de" },
 ]
-description = "Radiomics Tractometry for advanced along-tract analysis of diffusion MRI"
+maintainers = [
+  { name="Peter Neher", email="p.neher@dkfz-heidelberg.de" },
+]
+
+description = "Radiomic Tractometry for advanced along-tract analysis of diffusion-weighted MRI"
+keywords = ["tractometry", "radiomics", "tractography", "diffusion-weighted MRI"]
+
 readme = "README.md"
 dependencies = [
     'numpy',
     'pandas',
     'argparse',
     'scikit-image',
     'scikit-learn',
     'nibabel',
     'vtk',
     'dipy',
     'pyradiomics',
 ]
 license = { file="LICENSES/Apache-2.0.txt" }
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 
 classifiers = [
     'Programming Language :: Python :: 3',
     'Operating System :: OS Independent',
     'Development Status :: 5 - Production/Stable',
 ]
 
+[project.urls]
+Repository = "https://github.com/MIC-DKFZ/radtract"
+
 [project.scripts]
 radtract_parcellate = "radtract.parcellation:main"
 radtract_features = "radtract.features:main"
+radtract_tdi = "radtract.tractdensity:main"
 
 [tool.setuptools.package-data]
 radtract = ["*.yaml"]
 
 [tool.setuptools.packages.find]
 include = ["radtract*"]
 exclude = ["LICENSES*", "tests*"]
```

### Comparing `radtract-0.1.3/radtract/features.py` & `radtract-0.1.4/radtract/features.py`

 * *Files identical despite different names*

### Comparing `radtract-0.1.3/radtract/parcellation.py` & `radtract-0.1.4/radtract/parcellation.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from nibabel.affines import apply_affine
 from skimage.morphology import binary_dilation, binary_closing
 from sklearn.svm import SVC
 from dipy.segment.clustering import QuickBundles
 from dipy.segment.metric import AveragePointwiseEuclideanMetric
 from dipy.segment.featurespeed import ResampleFeature
 import numpy as np
-import vtk
 from dipy.tracking.streamline import transform_streamlines
 from dipy.io.streamline import load_trk
 from dipy.align.reslice import reslice
 from scipy.spatial import cKDTree
 import os
 import argparse
 import joblib
@@ -29,161 +28,14 @@
     :return: streamlines in dipy format
     """
     fib = load_trk(filename, "same", bbox_valid_check=False)
     streamlines = fib.streamlines
     return streamlines
 
 
-def intersect_image(spacing, si, ei, sf, ef):
-    """
-    Calculate the intersection of a line segment with a voxel grid.
-    :param spacing:
-    :param si: start index
-    :param ei: end index
-    :param sf: continuous start index
-    :param ef: continuous end index
-    :return: list of tuples (voxel index, length of segment in voxel)
-    """
-
-    out = []
-    if np.array_equal(si, ei):
-        d = np.empty(3)
-        for i in range(3):
-            d[i] = (sf[i]-ef[i])*spacing[i]
-
-        out.append((si, np.linalg.norm(d)))
-        return out
-
-    bounds = np.empty(6)
-
-    entrance_point = np.empty(3)
-    exit_point = np.empty(3)
-
-    start_point = np.empty(3)
-    end_point = np.empty(3)
-
-    t0 = vtk.reference(-1)
-    t1 = vtk.reference(-1)
-    for i in range(3):
-        start_point[i] = sf[i]
-        end_point[i] = ef[i]
-
-        if si[i] > ei[i]:
-            t = si[i]
-            si[i] = ei[i]
-            ei[i] = t
-
-    for x in range(si[0], ei[0]+1):
-        for y in range(si[1], ei[1]+1):
-            for z in range(si[2], ei[2]+1):
-                bounds[0] = x - 0.5
-                bounds[1] = x + 0.5
-                bounds[2] = y - 0.5
-                bounds[3] = y + 0.5
-                bounds[4] = z - 0.5
-                bounds[5] = z + 0.5
-
-                entry_plane = vtk.reference(-1)
-                exit_plane = vtk.reference(-1)
-
-                hit = vtk.vtkBox.IntersectWithLine(bounds, start_point, end_point, t0, t1, entrance_point, exit_point, entry_plane, exit_plane)
-                if hit > 0:
-                    if entry_plane >= 0 and exit_plane >= 0:
-                        d = np.empty(3)
-                        for i in range(3):
-                            d[i] = (exit_point[i] - entrance_point[i])*spacing[i]
-                        out.append(((x, y, z), np.linalg.norm(d)))
-                    elif entry_plane >= 0:
-                        d = np.empty(3)
-                        for i in range(3):
-                            d[i] = (ef[i] - entrance_point[i])*spacing[i]
-                        out.append(((x, y, z), np.linalg.norm(d)))
-                    elif exit_plane >= 0:
-                        d = np.empty(3)
-                        for i in range(3):
-                            d[i] = (exit_point[i]-sf[i])*spacing[i]
-                        out.append(((x, y, z), np.linalg.norm(d)))
-    return out
-
-
-def tract_envelope(streamlines: nib.streamlines.array_sequence.ArraySequence,
-                   reference_image: nib.Nifti1Image,
-                   do_closing: bool = False,
-                   out_image_filename: str = None):
-    """
-    Convenience function for tract_density that calculates the binary bundle envelope.
-    :param streamlines: input streamlines
-    :param reference_image: defines geometry of output image
-    :param do_closing: morphological closing of the binary image to remove holes
-    :param out_image_filename: if not None, the output image will be saved to this file
-    :return:
-    """
-    return tract_density(streamlines, reference_image, True, do_closing, out_image_filename)
-
-
-def tract_density(streamlines: nib.streamlines.array_sequence.ArraySequence,
-                  reference_image: nib.Nifti1Image,
-                  binary: bool = False,
-                  do_closing: bool = False,
-                  out_image_filename: str = None):
-    """
-    Calculate the tract density image for a set of streamlines using the true length of each streamline segment in each voxel.
-    :param streamlines: input streamlines
-    :param reference_image: defines geometry of output image
-    :param binary: if true, the output image will be a binary image with 1 for voxels that are part of the bundle and 0 outside
-    :param do_closing: morphological closing of the binary image to remove holes
-    :param out_image_filename: if not None, the output image will be saved to this file
-    :return:
-    """
-    if binary:
-        print('Calculating bundle envelope')
-    else:
-        print('Calculating tract density image')
-
-    if type(streamlines) is str:
-        streamlines = load_trk_streamlines(streamlines)
-    if type(reference_image) is str:
-        reference_image = nib.load(reference_image)
-
-    image_data = np.copy(reference_image.get_fdata())
-    image_data.fill(0)
-    affine = reference_image.affine
-    spacing = reference_image.header['pixdim'][1:4]
-    streamlines = transform_streamlines(streamlines, np.linalg.inv(affine))
-
-    for s in streamlines:
-        num_points = len(s)
-        for j in range(num_points-1):
-            start_index_cont = s[j]
-            start_index = np.round(start_index_cont).astype('int64')
-
-            end_index_cont = s[j+1]
-            end_index = np.round(end_index_cont).astype('int64')
-
-            segments = intersect_image(spacing, start_index, end_index, start_index_cont, end_index_cont)
-            for seg in segments:
-                if binary:
-                    image_data[seg[0][0], seg[0][1], seg[0][2]] = 1
-                else:
-                    image_data[seg[0][0], seg[0][1], seg[0][2]] += seg[1]
-
-    if binary and do_closing:
-        image_data = binary_closing(image_data)
-    if binary:
-        image_data = image_data.astype('uint8')
-        tdi = nib.Nifti1Image(image_data, header=reference_image.header, affine=reference_image.affine, dtype='uint8')
-    else:
-        tdi = nib.Nifti1Image(image_data, header=reference_image.header, affine=reference_image.affine)
-    if out_image_filename is not None:
-        nib.save(tdi, out_image_filename)
-    print('done')
-
-    return tdi
-
-
 def estimate_num_parcels(streamlines: nib.streamlines.array_sequence.ArraySequence,
                          reference_image: nib.Nifti1Image,
                          num_voxels: int = 5):
     """
     Estimates the number of parcels when aiming for a parcel size in tract direction of about 'num_voxels' voxels.
     :param streamlines: input streamlines
     :param reference_image: us this image geometry
```

### Comparing `radtract-0.1.3/radtract/pyrad.yaml` & `radtract-0.1.4/radtract/pyrad.yaml`

 * *Files identical despite different names*

### Comparing `radtract-0.1.3/tests/test_radtract.py` & `radtract-0.1.4/tests/test_radtract.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # Copyright © 2023 German Cancer Research Center (DKFZ), Division of Medical Image Computing
 #
 # SPDX-License-Identifier: Apache-2.0
 
 import numpy as np
 import pandas as pd
-from radtract import parcellation, features
+from radtract import parcellation, features, tractdensity
 import nibabel as nib
 import os
-import tempfile
 
 
 def load_data():
     data_folder = os.path.dirname(__file__) + '/test_data/'
     beginnings = nib.load(data_folder + 'test_tract_b.nii.gz')
     envelope = nib.load(data_folder + 'test_tract_envelope.nii.gz')
     centerline_parcellation = nib.load(data_folder + 'centerline_parcellation.nii.gz')
@@ -26,15 +25,15 @@
     os.makedirs(p, exist_ok=True)
     return p
 
 
 def test_envelope():
     streamlines, beginnings, envelope, _, _ = load_data()
 
-    new_envelope = parcellation.tract_envelope(streamlines, reference_image=beginnings, out_image_filename=get_results_path() + 'test_tract_envelope.nii.gz')
+    new_envelope = tractdensity.tract_envelope(streamlines, reference_image=beginnings, out_image_filename=get_results_path() + 'test_tract_envelope.nii.gz')
 
     assert np.equal(new_envelope.get_fdata(), envelope.get_fdata()).all(), 'envelope test 1 failed'
     new_envelope = nib.load(get_results_path() + 'test_tract_envelope.nii.gz')
     assert np.equal(new_envelope.get_fdata(), envelope.get_fdata()).all(), 'envelope test 2 failed'
 
 
 def test_centerline_parcellation():
```

