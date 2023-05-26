# Comparing `tmp/preppy-4.2.1-py2.py3-none-any.whl.zip` & `tmp/preppy-4.2.2-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 17892 bytes, number of entries: 7
--rw-r--r--  2.0 unx    58945 b- defN 23-Mar-14 12:57 preppy.py
--rw-r--r--  2.0 unx     1707 b- defN 23-Mar-14 12:57 preppy-4.2.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      258 b- defN 23-Mar-14 12:57 preppy-4.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Mar-14 12:57 preppy-4.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       39 b- defN 23-Mar-14 12:57 preppy-4.2.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 23-Mar-14 12:57 preppy-4.2.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      545 b- defN 23-Mar-14 12:57 preppy-4.2.1.dist-info/RECORD
-7 files, 61611 bytes uncompressed, 16926 bytes compressed:  72.5%
+Zip file size: 18218 bytes, number of entries: 7
+-rw-r--r--  2.0 unx    60676 b- defN 23-May-26 14:01 preppy.py
+-rw-r--r--  2.0 unx     1707 b- defN 23-May-26 14:10 preppy-4.2.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      258 b- defN 23-May-26 14:10 preppy-4.2.2.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-26 14:10 preppy-4.2.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       39 b- defN 23-May-26 14:10 preppy-4.2.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 23-May-26 14:10 preppy-4.2.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      545 b- defN 23-May-26 14:10 preppy-4.2.2.dist-info/RECORD
+7 files, 63342 bytes uncompressed, 17252 bytes compressed:  72.8%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: preppy.py
 Comment: 
 
-Filename: preppy-4.2.1.dist-info/LICENSE.txt
+Filename: preppy-4.2.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: preppy-4.2.1.dist-info/METADATA
+Filename: preppy-4.2.2.dist-info/METADATA
 Comment: 
 
-Filename: preppy-4.2.1.dist-info/WHEEL
+Filename: preppy-4.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: preppy-4.2.1.dist-info/entry_points.txt
+Filename: preppy-4.2.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: preppy-4.2.1.dist-info/top_level.txt
+Filename: preppy-4.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: preppy-4.2.1.dist-info/RECORD
+Filename: preppy-4.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## preppy.py

```diff
@@ -29,15 +29,15 @@
 The command line options let you run modules with hand-input parameters -
 useful for basic testing - and also to batch-compile or clean directories.
 As with python scripts, it is a good idea to compile prep files on installation,
 since unix applications may run as a different user and not have the needed
 permission to store compiled modules.
 
 """
-VERSION = '4.2.1'
+VERSION = '4.2.2'
 __version__ = VERSION
 
 USAGE = """
 The command line interface lets you test, compile and clean up:
 
     preppy modulename [arg1=value1, arg2=value2.....]
        - shorthand for 'preppy run ...', see below.
@@ -70,14 +70,15 @@
 isPy33 = isPy3 and sys.version_info.minor>=3
 isPy34 = isPy3 and sys.version_info.minor>=4
 isPy37 = isPy3 and sys.version_info.minor>=7
 isPy38 = isPy3 and sys.version_info.minor>=8
 isPy39 = isPy3 and sys.version_info.minor>=9
 isPy310 = isPy3 and sys.version_info.minor>=10
 isPy311 = isPy3 and sys.version_info.minor>=11
+isPy312 = isPy3 and sys.version_info.minor>=12
 _usePyCache = isPy3 and False                   #change if you don't have legacy ie python 2.7 usage
 from xml.sax.saxutils import escape as xmlEscape
 from collections import namedtuple
 Token = namedtuple('Token','kind start end')
 _verbose = int(os.environ.get('RL_verbose','0'))
 
 from keyword import iskeyword
@@ -1325,49 +1326,84 @@
 def installImporter():
     "This lets us import prep files directly"
     # the python import mechanics are only invoked if you call this,
     # since preppy has very few dependencies and I don't want to
     #add to them.
     global _preppy_importer
     if _preppy_importer is None:
-        class PreppyImporter(object):
-            "This allows prep files to be imported."
-            def __init__(self):
-                self.prepPath = None
-
-            def find_module(self, name, path=None):
-                if self.prepPath: return
-                if path:
-                    for p in path:
-                        prepPath = os.path.join(p,name.split('.')[-1] + '.prep')
-                        if os.path.isfile(prepPath): break
-                    else:
-                        return
-                else:
-                    prepPath = name + '.prep'
-                    if not os.path.isfile(prepPath): return
-
-                self.prepPath = prepPath
-                return self
-
-            def load_module(self,name):
-                if not self.prepPath: return
-                try:
-                    #compile WITHOUT IMPORTING to avoid triggering recursion
+        if isPy312:
+            import importlib.abc
+            import importlib.machinery
+            class _PreppyLoader(importlib.abc.Loader):
+                def create_module(self, spec):
+                    #print(f'+++++ create_module({spec!r})')
+                    name = spec.name
                     try:
-                        m = compileModule(self.prepPath, verbose=_verbose, importModule=0, existing_module=sys.modules.get(name,None))
+                        m = compileModule(spec.origin, verbose=_verbose, importModule=0, existing_module=sys.modules.get(name,None))
                     except:
                         traceback.print_exc()
                         raise
-                    m.__loader__ = self
+                    m.__loader__ = spec.loader
                     m.__name__ = name
                     sys.modules[name] = m
                     return m
-                finally:
+
+                def exec_module(self, module):
+                    pass
+
+            class PreppyImporter(importlib.abc.MetaPathFinder):
+                def find_spec(self, name, path, target=None):
+                    #print(f'+++++ find_spec({name!r},{path!r})')
+                    prepName = name.split('.')[-1] + '.prep'
+                    if not path:
+                        path = sys.path[:]
+                        if '' in path: path.remove('')
+                        path.insert(0,os.getcwd())
+                    for p in path:
+                        if p=='':
+                            p = os.getcwd()
+                        found = os.path.join(p,prepName)
+                        if os.path.isfile(found):
+                            return importlib.machinery.ModuleSpec(name, _PreppyLoader(), origin=found)
+        else:
+            class PreppyImporter(object):
+                "This allows prep files to be imported."
+                def __init__(self):
                     self.prepPath = None
+
+                def find_module(self, name, path=None):
+                    if self.prepPath: return
+                    if path:
+                        for p in path:
+                            prepPath = os.path.join(p,name.split('.')[-1] + '.prep')
+                            if os.path.isfile(prepPath): break
+                        else:
+                            return
+                    else:
+                        prepPath = name + '.prep'
+                        if not os.path.isfile(prepPath): return
+
+                    self.prepPath = prepPath
+                    return self
+
+                def load_module(self,name):
+                    if not self.prepPath: return
+                    try:
+                        #compile WITHOUT IMPORTING to avoid triggering recursion
+                        try:
+                            m = compileModule(self.prepPath, verbose=_verbose, importModule=0, existing_module=sys.modules.get(name,None))
+                        except:
+                            traceback.print_exc()
+                            raise
+                        m.__loader__ = self
+                        m.__name__ = name
+                        sys.modules[name] = m
+                        return m
+                    finally:
+                        self.prepPath = None
         _preppy_importer = PreppyImporter()
         sys.meta_path.insert(0,_preppy_importer)
 
 def uninstallImporter():
     global _preppy_importer
     try:
         sys.meta_path.remove(_preppy_importer)
```

## Comparing `preppy-4.2.1.dist-info/LICENSE.txt` & `preppy-4.2.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

