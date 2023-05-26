# Comparing `tmp/nerfvis-0.1.5.tar.gz` & `tmp/nerfvis-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nerfvis-0.1.5.tar", last modified: Fri May 12 20:16:44 2023, max compression
+gzip compressed data, was "nerfvis-0.1.6.tar", last modified: Fri May 26 18:58:51 2023, max compression
```

## Comparing `nerfvis-0.1.5.tar` & `nerfvis-0.1.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-12 20:16:44.096757 nerfvis-0.1.5/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1260 2022-02-04 19:47:59.000000 nerfvis-0.1.5/LICENSE.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)      337 2022-09-11 08:09:28.000000 nerfvis-0.1.5/MANIFEST.in
--rw-rw-r--   0 alex      (1000) alex      (1000)      251 2023-05-12 20:16:44.096757 nerfvis-0.1.5/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     7483 2022-09-16 22:22:13.000000 nerfvis-0.1.5/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-12 20:16:44.096757 nerfvis-0.1.5/nerfvis/
--rw-rw-r--   0 alex      (1000) alex      (1000)       94 2022-08-24 01:42:22.000000 nerfvis-0.1.5/nerfvis/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)   805091 2022-09-16 22:19:33.000000 nerfvis-0.1.5/nerfvis/index.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    60471 2023-05-12 20:11:07.000000 nerfvis-0.1.5/nerfvis/scene.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-12 20:16:44.096757 nerfvis-0.1.5/nerfvis/utils/
--rw-rw-r--   0 alex      (1000) alex      (1000)     7202 2022-09-11 01:40:00.000000 nerfvis-0.1.5/nerfvis/utils/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)  2003887 2022-08-23 04:07:45.000000 nerfvis-0.1.5/nerfvis/utils/_rotation.c
--rw-rw-r--   0 alex      (1000) alex      (1000)    87588 2022-08-23 02:49:39.000000 nerfvis-0.1.5/nerfvis/utils/_rotation.pyx
--rw-rw-r--   0 alex      (1000) alex      (1000)    12573 2022-02-04 19:47:59.000000 nerfvis-0.1.5/nerfvis/utils/sh.py
--rw-rw-r--   0 alex      (1000) alex      (1000)       22 2023-05-12 20:11:17.000000 nerfvis-0.1.5/nerfvis/version.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-12 20:16:44.096757 nerfvis-0.1.5/nerfvis.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)      251 2023-05-12 20:16:44.000000 nerfvis-0.1.5/nerfvis.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)      366 2023-05-12 20:16:44.000000 nerfvis-0.1.5/nerfvis.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-05-12 20:16:44.000000 nerfvis-0.1.5/nerfvis.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        8 2023-05-12 20:16:44.000000 nerfvis-0.1.5/nerfvis.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       59 2022-08-23 04:10:40.000000 nerfvis-0.1.5/pyproject.toml
--rw-rw-r--   0 alex      (1000) alex      (1000)       79 2023-05-12 20:16:44.100757 nerfvis-0.1.5/setup.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)     1742 2022-09-11 08:10:30.000000 nerfvis-0.1.5/setup.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-26 18:58:51.011531 nerfvis-0.1.6/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1260 2022-02-04 19:47:59.000000 nerfvis-0.1.6/LICENSE.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)      337 2022-09-11 08:09:28.000000 nerfvis-0.1.6/MANIFEST.in
+-rw-rw-r--   0 alex      (1000) alex      (1000)      251 2023-05-26 18:58:51.011531 nerfvis-0.1.6/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7483 2022-09-16 22:22:13.000000 nerfvis-0.1.6/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-26 18:58:51.007531 nerfvis-0.1.6/nerfvis/
+-rw-rw-r--   0 alex      (1000) alex      (1000)       94 2022-08-24 01:42:22.000000 nerfvis-0.1.6/nerfvis/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)   805091 2022-09-16 22:19:33.000000 nerfvis-0.1.6/nerfvis/index.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    61127 2023-05-26 18:57:33.000000 nerfvis-0.1.6/nerfvis/scene.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-26 18:58:51.011531 nerfvis-0.1.6/nerfvis/utils/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7202 2022-09-11 01:40:00.000000 nerfvis-0.1.6/nerfvis/utils/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)  2003887 2022-08-23 04:07:45.000000 nerfvis-0.1.6/nerfvis/utils/_rotation.c
+-rw-rw-r--   0 alex      (1000) alex      (1000)    87588 2022-08-23 02:49:39.000000 nerfvis-0.1.6/nerfvis/utils/_rotation.pyx
+-rw-rw-r--   0 alex      (1000) alex      (1000)    12573 2022-02-04 19:47:59.000000 nerfvis-0.1.6/nerfvis/utils/sh.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)       22 2023-05-26 18:53:08.000000 nerfvis-0.1.6/nerfvis/version.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-26 18:58:51.007531 nerfvis-0.1.6/nerfvis.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      251 2023-05-26 18:58:50.000000 nerfvis-0.1.6/nerfvis.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)      366 2023-05-26 18:58:50.000000 nerfvis-0.1.6/nerfvis.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-05-26 18:58:50.000000 nerfvis-0.1.6/nerfvis.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        8 2023-05-26 18:58:50.000000 nerfvis-0.1.6/nerfvis.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       59 2022-08-23 04:10:40.000000 nerfvis-0.1.6/pyproject.toml
+-rw-rw-r--   0 alex      (1000) alex      (1000)       79 2023-05-26 18:58:51.011531 nerfvis-0.1.6/setup.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1742 2022-09-11 08:10:30.000000 nerfvis-0.1.6/setup.py
```

### Comparing `nerfvis-0.1.5/LICENSE.txt` & `nerfvis-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nerfvis-0.1.5/README.md` & `nerfvis-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `nerfvis-0.1.5/nerfvis/index.html` & `nerfvis-0.1.6/nerfvis/index.html`

 * *Files identical despite different names*

### Comparing `nerfvis-0.1.5/nerfvis/scene.py` & `nerfvis-0.1.6/nerfvis/scene.py`

 * *Files 2% similar despite different names*

```diff
@@ -365,14 +365,15 @@
         :param scale:  float, scale, default 1.0 (common param)
         :param visible: bool, whether mesh should be visible on init, default true
                         (depends on GET parameter in web version) (common param)
         :param unlit: bool, whether mesh should be rendered unlit. Default true (common param)
         :param time: int, time at which the mesh should be displayed; -1=always display (default)
                     (common param)
         """
+        assert points.ndim == 2 and points.shape[1] == 3, "points must be (N, 3)"
         self._add_common(name, **kwargs)
         points = _to_np_array(points)
         self.fields[name] = "points"
         self.fields[_f(name, "points")] = points.astype(np.float32)
         if point_size != 1.0:
             self.fields[_f(name, "point_size")] = np.float32(point_size)
         self._update_bb(points, **kwargs)
@@ -401,34 +402,39 @@
                         (depends on GET parameter in web version) (common param)
         :param unlit: bool, whether mesh should be rendered unlit.
                             Use this if you want to render vertex colors directly
                             without lighting. Default false. (common param)
         :param time: int, time at which the mesh should be displayed; -1=always display (default)
                     (common param)
         """
+        assert points.ndim == 2 and points.shape[1] == 3, "points must be (N, 3)"
         self._add_common(name, **kwargs)
         points = _to_np_array(points)
         self.fields[name] = "mesh"
         self.fields[_f(name, "points")] = points.astype(np.float32)
         if face_size is not None:
             self.fields[_f(name, "face_size")] = int(face_size)
             assert face_size >= 1 and face_size <= 3
         if faces is not None:
+            assert faces.ndim == 2 and faces.shape[1] == face_size, \
+                    f"faces must be (N, face_size={face_size})"
+        if faces is not None:
             self.fields[_f(name, "faces")] = _to_np_array(faces).astype(np.int32)
         self._update_bb(points, **kwargs)
 
     def add_image(self,
                   name : str,
                   image : Union[str, np.ndarray],
                   r: np.ndarray,
                   t: np.ndarray,
                   focal_length : float = 1111.11,
                   z: float = -0.1,
                   image_size : int = 64,
-                  opengl: Optional[bool] = None):
+                  opengl: Optional[bool] = None,
+                  **kwargs):
         """
         Add an image (as plane mesh with vertex colors)
 
         :param name: an identifier for this object
         :param path: path to the image
         :param r: (3,) or (4,) or (3, 3) or None, optional
                   C2W rotations for each camera, either as axis-angle,
@@ -438,18 +444,20 @@
         :param z: the depth at which to draw the frustum far points.
                   use negative values for OpenGL coordinates (original NeRF)
                   or positive values for OpenCV coordinates (NSVF).
                   If not given, tries to infer a good value. Else defaults to -0.3
                   NOTE: kind of weirdly (but to be consistent
                   with add_camera_frustum),for OpenGL, z needs to be negative,
                   while for OpenCV it should be positive.
-        :param image_size: size of image for display (only if using path)
+        :param image_size: size of image for display.
+                           NOTE: do not make this too large or it may crash!
         :param opengl: if True use OpenGL coordinates (NeRF default);
                        else use OpenCV. Default: depends on if set_opencv()
                        was used.
+        :param time: int, time at which the mesh should be displayed; -1=always display (default)
         """
         if opengl is None:
             opengl = not self.default_opencv
         from PIL import Image  # pip install pillow
         if isinstance(image, str):
             im = Image.open(str(image))
         else:
@@ -497,17 +505,19 @@
         t = _to_np_array(t).astype(np.float32)
 
         grid_i = (r * grid.reshape(-1, 1, 3)).sum(-1) + t
         grid_i = grid_i.astype(np.float32).copy()
         self.add_mesh(
             name,
             grid_i,
-            faces=faces,
+            faces=faces.reshape(-1, 3),
+            face_size=3,
             vert_color=im.reshape(-1, 3).astype(np.float32) / 255.0,
             unlit=True,
+            **kwargs
         )
 
 
     def add_camera_frustum(
                  self, name : str,
                  focal_length : Optional[float] = None,
                  image_width : Optional[float] = None,
@@ -560,15 +570,17 @@
             self.fields[_f(name, "image_height")] = np.float32(image_height)
         if connect:
             self.fields[_f(name, "connect")] = 1
 
         if r is not None:
             assert t is not None, "r,t should be both set or both unset"
             r = _to_np_array(r)
-            if r.ndim == 1 or (r.ndim == 2 and t.ndim == 1):
+            if t is not None:
+                t = _to_np_array(t)
+            if r.ndim == 1 or (r.ndim == 2 and t is not None and t.ndim == 1):
                 r = r[None]
             if r.ndim == 3 and r.shape[1] == 3 and r.shape[2] == 3:
                 # Matrix
                 r = utils.Rotation.from_matrix(r).as_rotvec()
             elif r.ndim == 2 and r.shape[1] == 4 and t:
                 # Quaternion
                 r = utils.Rotation.from_quat(r).as_rotvec()
```

### Comparing `nerfvis-0.1.5/nerfvis/utils/__init__.py` & `nerfvis-0.1.6/nerfvis/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfvis-0.1.5/nerfvis/utils/_rotation.c` & `nerfvis-0.1.6/nerfvis/utils/_rotation.c`

 * *Files identical despite different names*

### Comparing `nerfvis-0.1.5/nerfvis/utils/_rotation.pyx` & `nerfvis-0.1.6/nerfvis/utils/_rotation.pyx`

 * *Files identical despite different names*

### Comparing `nerfvis-0.1.5/nerfvis/utils/sh.py` & `nerfvis-0.1.6/nerfvis/utils/sh.py`

 * *Files identical despite different names*

### Comparing `nerfvis-0.1.5/setup.py` & `nerfvis-0.1.6/setup.py`

 * *Files identical despite different names*

