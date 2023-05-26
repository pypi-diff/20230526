# Comparing `tmp/blue-engine-0.0.2.tar.gz` & `tmp/blue-engine-0.0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blue-engine-0.0.2.tar", last modified: Sun May 21 05:14:00 2023, max compression
+gzip compressed data, was "blue-engine-0.0.3.5.tar", last modified: Fri May 26 07:47:14 2023, max compression
```

## Comparing `blue-engine-0.0.2.tar` & `blue-engine-0.0.3.5.tar`

### file list

```diff
@@ -1,26 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 05:14:00.893861 blue-engine-0.0.2/
--rw-rw-rw-   0        0        0       68 2023-05-21 04:57:53.000000 blue-engine-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      472 2023-05-21 05:14:00.844849 blue-engine-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-21 05:14:00.644799 blue-engine-0.0.2/blue_engine.egg-info/
--rw-rw-rw-   0        0        0      472 2023-05-21 05:13:59.000000 blue-engine-0.0.2/blue_engine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      500 2023-05-21 05:14:00.000000 blue-engine-0.0.2/blue_engine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 05:13:59.000000 blue-engine-0.0.2/blue_engine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-05-21 05:13:59.000000 blue-engine-0.0.2/blue_engine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1073 2023-05-21 05:11:18.000000 blue-engine-0.0.2/license.txt
--rw-rw-rw-   0        0        0       42 2023-05-21 05:14:00.894862 blue-engine-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      702 2023-05-21 05:13:54.000000 blue-engine-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-21 05:14:00.536770 blue-engine-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-21 05:14:00.840848 blue-engine-0.0.2/src/blueEngine/
--rw-rw-rw-   0        0        0        0 2023-05-07 14:20:14.000000 blue-engine-0.0.2/src/blueEngine/__init__.py
--rw-rw-rw-   0        0        0     2232 2023-05-20 04:56:49.000000 blue-engine-0.0.2/src/blueEngine/app.py
--rw-rw-rw-   0        0        0     2272 2023-05-20 07:28:36.000000 blue-engine-0.0.2/src/blueEngine/camera.py
--rw-rw-rw-   0        0        0       89 2023-05-20 05:02:59.000000 blue-engine-0.0.2/src/blueEngine/component.py
--rw-rw-rw-   0        0        0      359 2023-05-11 07:14:39.000000 blue-engine-0.0.2/src/blueEngine/light.py
--rw-rw-rw-   0        0        0      287 2023-05-11 12:59:41.000000 blue-engine-0.0.2/src/blueEngine/mesh.py
--rw-rw-rw-   0        0        0     2243 2023-05-20 05:19:16.000000 blue-engine-0.0.2/src/blueEngine/model.py
--rw-rw-rw-   0        0        0      795 2023-05-20 07:59:10.000000 blue-engine-0.0.2/src/blueEngine/scene.py
--rw-rw-rw-   0        0        0      634 2023-05-11 07:33:57.000000 blue-engine-0.0.2/src/blueEngine/shader_program.py
--rw-rw-rw-   0        0        0     1034 2023-05-11 14:19:28.000000 blue-engine-0.0.2/src/blueEngine/texture.py
--rw-rw-rw-   0        0        0      493 2023-05-20 05:10:43.000000 blue-engine-0.0.2/src/blueEngine/transfrom.py
--rw-rw-rw-   0        0        0      612 2023-05-11 07:41:36.000000 blue-engine-0.0.2/src/blueEngine/vao.py
--rw-rw-rw-   0        0        0     2436 2023-05-11 12:57:47.000000 blue-engine-0.0.2/src/blueEngine/vbo.py
+drwxrwxrwx   0        0        0        0 2023-05-26 07:47:13.977826 blue-engine-0.0.3.5/
+-rw-rw-rw-   0        0        0       68 2023-05-21 04:57:53.000000 blue-engine-0.0.3.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      482 2023-05-26 07:47:13.974825 blue-engine-0.0.3.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-26 07:47:12.617485 blue-engine-0.0.3.5/blueEngine/
+-rw-rw-rw-   0        0        0      207 2023-05-26 06:36:53.000000 blue-engine-0.0.3.5/blueEngine/BETime.py
+-rw-rw-rw-   0        0        0        0 2023-05-07 14:20:14.000000 blue-engine-0.0.3.5/blueEngine/__init__.py
+-rw-rw-rw-   0        0        0     2374 2023-05-25 03:43:59.000000 blue-engine-0.0.3.5/blueEngine/app.py
+-rw-rw-rw-   0        0        0     2272 2023-05-20 07:28:36.000000 blue-engine-0.0.3.5/blueEngine/camera.py
+-rw-rw-rw-   0        0        0      145 2023-05-26 06:26:49.000000 blue-engine-0.0.3.5/blueEngine/canvas.py
+-rw-rw-rw-   0        0        0       89 2023-05-26 05:14:05.000000 blue-engine-0.0.3.5/blueEngine/component.py
+-rw-rw-rw-   0        0        0      236 2023-05-22 13:59:34.000000 blue-engine-0.0.3.5/blueEngine/errors.py
+-rw-rw-rw-   0        0        0      352 2023-05-26 05:04:34.000000 blue-engine-0.0.3.5/blueEngine/font_component.py
+-rw-rw-rw-   0        0        0      361 2023-05-26 06:24:16.000000 blue-engine-0.0.3.5/blueEngine/gobject.py
+-rw-rw-rw-   0        0        0     2262 2023-05-25 04:22:31.000000 blue-engine-0.0.3.5/blueEngine/input.py
+-rw-rw-rw-   0        0        0      359 2023-05-11 07:14:39.000000 blue-engine-0.0.3.5/blueEngine/light.py
+-rw-rw-rw-   0        0        0      287 2023-05-11 12:59:41.000000 blue-engine-0.0.3.5/blueEngine/mesh.py
+-rw-rw-rw-   0        0        0     2558 2023-05-26 06:26:29.000000 blue-engine-0.0.3.5/blueEngine/model.py
+-rw-rw-rw-   0        0        0      869 2023-05-25 19:13:25.000000 blue-engine-0.0.3.5/blueEngine/scene.py
+-rw-rw-rw-   0        0        0      634 2023-05-11 07:33:57.000000 blue-engine-0.0.3.5/blueEngine/shader_program.py
+-rw-rw-rw-   0        0        0        0 2023-05-26 06:22:27.000000 blue-engine-0.0.3.5/blueEngine/textobject.py
+-rw-rw-rw-   0        0        0     1034 2023-05-11 14:19:28.000000 blue-engine-0.0.3.5/blueEngine/texture.py
+-rw-rw-rw-   0        0        0      493 2023-05-20 05:10:43.000000 blue-engine-0.0.3.5/blueEngine/transfrom.py
+-rw-rw-rw-   0        0        0       86 2023-05-23 05:53:48.000000 blue-engine-0.0.3.5/blueEngine/utils.py
+-rw-rw-rw-   0        0        0      612 2023-05-11 07:41:36.000000 blue-engine-0.0.3.5/blueEngine/vao.py
+-rw-rw-rw-   0        0        0     2407 2023-05-25 03:44:26.000000 blue-engine-0.0.3.5/blueEngine/vbo.py
+drwxrwxrwx   0        0        0        0 2023-05-26 07:47:13.884803 blue-engine-0.0.3.5/blue_engine.egg-info/
+-rw-rw-rw-   0        0        0      482 2023-05-26 07:47:08.000000 blue-engine-0.0.3.5/blue_engine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      695 2023-05-26 07:47:09.000000 blue-engine-0.0.3.5/blue_engine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 07:47:08.000000 blue-engine-0.0.3.5/blue_engine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-23 06:47:43.000000 blue-engine-0.0.3.5/blue_engine.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       39 2023-05-26 07:47:08.000000 blue-engine-0.0.3.5/blue_engine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-26 07:47:08.000000 blue-engine-0.0.3.5/blue_engine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1070 2023-05-21 05:17:33.000000 blue-engine-0.0.3.5/license.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 07:47:13.978826 blue-engine-0.0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      801 2023-05-26 07:31:52.000000 blue-engine-0.0.3.5/setup.py
```

### Comparing `blue-engine-0.0.2/license.txt` & `blue-engine-0.0.3.5/license.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright <YEAR> <COPYRIGHT HOLDER>
+Copyright 2023 Debojyoti Ganguly
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `blue-engine-0.0.2/setup.py` & `blue-engine-0.0.3.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,24 +4,26 @@
     with open('readme.md') as f:
         README = f.read()
     return README
 
 
 setup(
     name='blue-engine',
-    version='0.0.2',
+    version='0.0.3.5',
     description='',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/MrBlueBlobGuy/Blue-Engine',
     author='Debojyoti Ganguly',
     author_email='debojyotiganguly70@gmail.com',
     license='Zlib',
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.10",
     ],
-    packages=['src.blueEngine'],
+    packages=['blueEngine'],
     include_package_data=True,
+    install_requires=['pygame', 'moderngl', 'pyglm', 'numpy', 'noise', 'lupa'],
+    zip_safe=False
 )
```

### Comparing `blue-engine-0.0.2/src/blueEngine/app.py` & `blue-engine-0.0.3.5/blueEngine/app.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,38 +5,39 @@
 from mesh import Mesh
 from camera import Camera
 from light import Light
 from model import *
 from scene import Scene
 
 class app:
-    def __init__(self, size, title, framerate, flags=None) -> None:
+    def __init__(self, size, title, framerate, flags=None, icon_path = 'images/BlueEngineLogo.png') -> None:
         self.size = size
         self.title = title
         self.flags = flags
         self.framerate = framerate
         self.clock = pygame.time.Clock()
         self.scene = None
         self.camera = None
         self.light = None
-
+        self.icon = pygame.image.load(icon_path)
         self.time = 0
         self.delta_time = 0
 
         self.ctx = None
         
         self.run()
 
     def run(self):
         pygame.init()
-        pygame.display.gl_set_attribute(pygame.GL_CONTEXT_MAJOR_VERSION, 3)
+        pygame.display.gl_set_attribute(pygame.GL_CONTEXT_MAJOR_VERSION, 4)
         pygame.display.gl_set_attribute(pygame.GL_CONTEXT_MINOR_VERSION, 3)
         pygame.display.gl_set_attribute(pygame.GL_CONTEXT_PROFILE_MASK, pygame.GL_CONTEXT_PROFILE_CORE)
         pygame.display.set_mode(self.size, flags=pygame.OPENGL|pygame.DOUBLEBUF|pygame.RESIZABLE)
         pygame.display.set_caption(self.title)
+        pygame.display.set_icon(self.icon)
         pygame.event.set_grab(True)
         pygame.mouse.set_visible(False)
 
         self.ctx=moderngl.create_context()
         self.ctx.enable(flags=moderngl.DEPTH_TEST|moderngl.CULL_FACE)
         
         self.light = Light()
@@ -47,15 +48,15 @@
 
         self.loop()
         
 
     def loop(self):
         while True:
             self.get_time()
-            pygame.display.set_caption(f'{self.title} @ {self.clock.get_fps()}')
+            pygame.display.set_caption(f'{self.title} @ {int(self.clock.get_fps())} fps')
             self.render()
             self.camera.update()
             self.check_events()
             self.delta_time = self.clock.tick(self.framerate)
 
     def render(self):
         self.ctx.clear(0.18, 0.20, 0.31)
```

### Comparing `blue-engine-0.0.2/src/blueEngine/camera.py` & `blue-engine-0.0.3.5/blueEngine/camera.py`

 * *Files identical despite different names*

### Comparing `blue-engine-0.0.2/src/blueEngine/model.py` & `blue-engine-0.0.3.5/blueEngine/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,16 @@
-import numpy as np
 import glm
+
+from errors import *
 from transfrom import Transfrom
+from gobject import GameObject
 
-class BaseModel:
-    def __init__(self, app, vao_name, tex_id, position=(0, 0, 0), rotation = (0, 0, 0), scale = (1, 1, 1)) -> None:
+class BaseModel(GameObject):
+    def __init__(self, app, vao_name, tex_id, parent = None, position=(0, 0, 0), rotation = (0, 0, 0), scale = (1, 1, 1)) -> None:
+        super().__init__(parent)
         self.app = app
         self.components = {'transform':Transfrom(self, scale, rotation, position)}
         self.m_model = self.get_model_matrix()
         self.tex_id = tex_id
         self.vao = app.mesh.vao.vaos[vao_name]
         self.program = self.vao.program
         self.camera = self.app.camera
@@ -22,18 +25,23 @@
         m_model = glm.rotate(m_model, self.components['transform'].rotation.z, glm.vec3(0, 0, 1))
         m_model = glm.scale(m_model, self.components['transform'].scale)
         return m_model
     
     def render(self):
         self.update()
         self.vao.render()
+    def get_component(self, component:str):
+        try:
+            return self.components[component]
+        except KeyError:
+            raise ChildComponentNotExistsException(component)
 
 class Cube(BaseModel):
-    def __init__(self, app, vao_name='cube', tex_id=0, position = (0, 0, 0), rotation = (0, 0, 0), scale = (1, 1, 1)) -> None:
-        super().__init__(app, vao_name, tex_id, position, rotation, scale)
+    def __init__(self, app, parent = None, vao_name='cube', tex_id=0, position = (0, 0, 0), rotation = (0, 0, 0), scale = (1, 1, 1)) -> None:
+        super().__init__(app, vao_name, tex_id, parent, position, rotation, scale)
         self.on_init()
 
     def update(self):
         self.texture.use()
         self.program['m_model'].write(self.m_model)
         self.program['m_view'].write(self.camera.m_view)
         self.program['camPos'].write(self.camera.position)
```

### Comparing `blue-engine-0.0.2/src/blueEngine/scene.py` & `blue-engine-0.0.3.5/blueEngine/scene.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from model import *
 import threading
+from input import Input, InputAxis
+
 class Scene:
     def __init__(self, app) -> None:
         self.app = app
         self.objects = []
+        self.input_axes = Input() 
         self.load()
 
     def add_object(self, object):
         self.objects.append(object)
 
     def load(self):
         app = self.app
```

### Comparing `blue-engine-0.0.2/src/blueEngine/shader_program.py` & `blue-engine-0.0.3.5/blueEngine/shader_program.py`

 * *Files identical despite different names*

### Comparing `blue-engine-0.0.2/src/blueEngine/texture.py` & `blue-engine-0.0.3.5/blueEngine/texture.py`

 * *Files identical despite different names*

### Comparing `blue-engine-0.0.2/src/blueEngine/vao.py` & `blue-engine-0.0.3.5/blueEngine/vao.py`

 * *Files identical despite different names*

### Comparing `blue-engine-0.0.2/src/blueEngine/vbo.py` & `blue-engine-0.0.3.5/blueEngine/vbo.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import numpy as np
-import moderngl
 
 class VBO:
     def __init__(self, ctx):
         self.vbos = {}
         self.vbos['cube'] = CubeVBO(ctx)
         
     def destroy(self):
@@ -67,11 +66,7 @@
                    ( 0, 1, 0) * 6,
                    ( 0,-1, 0) * 6,]
         normals = np.array(normals, dtype='f4').reshape(36, 3)
 
         vertex_data = np.hstack([normals, vertex_data])
         vertex_data = np.hstack([tex_coord_data, vertex_data])
         return vertex_data
-
-
-
-
```

