# Comparing `tmp/cini-0.4.0.tar.gz` & `tmp/cini-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cini-0.4.0.tar", last modified: Tue Sep 27 06:37:40 2022, max compression
+gzip compressed data, was "dist/cini-0.5.0.tar", last modified: Fri May 26 07:46:05 2023, max compression
```

## Comparing `cini-0.4.0.tar` & `cini-0.5.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 afita     (1000) afita     (1000)        0 2022-09-27 06:37:40.000000 cini-0.4.0/
--rw-rw-r--   0 afita     (1000) afita     (1000)      296 2022-09-27 06:37:40.000000 cini-0.4.0/PKG-INFO
--rw-rw-r--   0 afita     (1000) afita     (1000)       38 2022-09-27 06:37:40.000000 cini-0.4.0/setup.cfg
--rw-rw-r--   0 afita     (1000) afita     (1000)      400 2022-09-27 06:35:47.000000 cini-0.4.0/setup.py
-drwxrwxr-x   0 afita     (1000) afita     (1000)        0 2022-09-27 06:37:40.000000 cini-0.4.0/cini/
--rw-rw-r--   0 afita     (1000) afita     (1000)      648 2022-06-23 07:48:15.000000 cini-0.4.0/cini/__init__.py
--rw-rw-r--   0 afita     (1000) afita     (1000)    30946 2022-09-27 06:34:24.000000 cini-0.4.0/cini/models.py
-drwxrwxr-x   0 afita     (1000) afita     (1000)        0 2022-09-27 06:37:40.000000 cini-0.4.0/cini.egg-info/
--rw-rw-r--   0 afita     (1000) afita     (1000)        5 2022-09-27 06:37:40.000000 cini-0.4.0/cini.egg-info/top_level.txt
--rw-rw-r--   0 afita     (1000) afita     (1000)      163 2022-09-27 06:37:40.000000 cini-0.4.0/cini.egg-info/SOURCES.txt
--rw-rw-r--   0 afita     (1000) afita     (1000)      296 2022-09-27 06:37:40.000000 cini-0.4.0/cini.egg-info/PKG-INFO
--rw-rw-r--   0 afita     (1000) afita     (1000)        1 2022-09-27 06:37:40.000000 cini-0.4.0/cini.egg-info/dependency_links.txt
--rw-rw-r--   0 afita     (1000) afita     (1000)     1634 2022-06-23 07:48:15.000000 cini-0.4.0/README.rst
+drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2023-05-26 07:46:05.000000 cini-0.5.0/
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      400 2023-05-26 07:45:31.000000 cini-0.5.0/setup.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)       38 2023-05-26 07:46:05.000000 cini-0.5.0/setup.cfg
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     1634 2020-12-28 08:44:17.000000 cini-0.5.0/README.rst
+drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2023-05-26 07:46:05.000000 cini-0.5.0/cini/
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      648 2020-12-28 08:44:17.000000 cini-0.5.0/cini/__init__.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)    31183 2023-05-26 07:45:18.000000 cini-0.5.0/cini/models.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      307 2023-05-26 07:46:05.000000 cini-0.5.0/PKG-INFO
+drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2023-05-26 07:46:05.000000 cini-0.5.0/cini.egg-info/
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)        5 2023-05-26 07:46:05.000000 cini-0.5.0/cini.egg-info/top_level.txt
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      163 2023-05-26 07:46:05.000000 cini-0.5.0/cini.egg-info/SOURCES.txt
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)        1 2023-05-26 07:46:05.000000 cini-0.5.0/cini.egg-info/dependency_links.txt
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      307 2023-05-26 07:46:05.000000 cini-0.5.0/cini.egg-info/PKG-INFO
```

### Comparing `cini-0.4.0/cini/__init__.py` & `cini-0.5.0/cini/__init__.py`

 * *Files identical despite different names*

### Comparing `cini-0.4.0/cini/models.py` & `cini-0.5.0/cini/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         linea.num_circuitos = 2
         linea.num_conductores = 1
         linea.seccion = 80
         linea.despliegue = 'AP'
         str(linea.cini)  # 'I20221LY'
     """
     def __init__(self):
-        self.tension = None
+        self._tension = None
         """Tension en kV
         """
         self.num_circuitos = None
         """Número de circuitos
         """
         self.num_conductores = None
         """Número de conductores
@@ -77,14 +77,24 @@
 
             - Tensada sobre postes: ``AP``
             - Apoyada sobre fachada: ``AF``
             - Subterránea: ``S``
         """
 
     @property
+    def tension(self):
+        return self._tension
+
+    @tension.setter
+    def tension(self, value):
+        if 3000 >= value >= 4000:
+            value = int(round(value / 1000.0) * 1000)
+        self._tension = value
+
+    @property
     def cini(self):
         """Obtiene el CINI de la linea
         :returns :py:class:`CINI`
         """
         c = CINI()
         c.positions[1] = '2'
         c.positions[2] = '0'
```

### Comparing `cini-0.4.0/README.rst` & `cini-0.5.0/README.rst`

 * *Files identical despite different names*

