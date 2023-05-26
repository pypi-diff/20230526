# Comparing `tmp/pyimclsts-0.1.2.tar.gz` & `tmp/pyimclsts-0.1.2.1.tar.gz`

## Comparing `pyimclsts-0.1.2.tar` & `pyimclsts-0.1.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 pyimclsts-0.1.2/CHANGELOG.md
--rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 pyimclsts-0.1.2/example/followRef.py
--rw-r--r--   0        0        0     4388 2020-02-02 00:00:00.000000 pyimclsts-0.1.2/example/lsf2csv.py
--rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 pyimclsts-0.1.2/example/selectedlsf2csv.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyimclsts-0.1.2/src/pyimclsts/__init__.py
--rw-r--r--   0        0        0    16631 2020-02-02 00:00:00.000000 pyimclsts-0.1.2/src/pyimclsts/_base.py
--rw-r--r--   0        0        0    11407 2020-02-02 00:00:00.000000 pyimclsts-0.1.2/src/pyimclsts/core.py
--rw-r--r--   0        0        0    17497 2020-02-02 00:00:00.000000 pyimclsts-0.1.2/src/pyimclsts/extract.py
--rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 pyimclsts-0.1.2/src/pyimclsts/extractutils.py
--rw-r--r--   0        0        0    35089 2020-02-02 00:00:00.000000 pyimclsts-0.1.2/src/pyimclsts/network.py
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 pyimclsts-0.1.2/.gitignore
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 pyimclsts-0.1.2/LICENSE
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 pyimclsts-0.1.2/README.md
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 pyimclsts-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4043 2020-02-02 00:00:00.000000 pyimclsts-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 pyimclsts-0.1.2.1/CHANGELOG.md
+-rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 pyimclsts-0.1.2.1/example/followRef.py
+-rw-r--r--   0        0        0     4388 2020-02-02 00:00:00.000000 pyimclsts-0.1.2.1/example/lsf2csv.py
+-rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 pyimclsts-0.1.2.1/example/selectedlsf2csv.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyimclsts-0.1.2.1/src/pyimclsts/__init__.py
+-rw-r--r--   0        0        0    16631 2020-02-02 00:00:00.000000 pyimclsts-0.1.2.1/src/pyimclsts/_base.py
+-rw-r--r--   0        0        0    11407 2020-02-02 00:00:00.000000 pyimclsts-0.1.2.1/src/pyimclsts/core.py
+-rw-r--r--   0        0        0    17497 2020-02-02 00:00:00.000000 pyimclsts-0.1.2.1/src/pyimclsts/extract.py
+-rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 pyimclsts-0.1.2.1/src/pyimclsts/extractutils.py
+-rw-r--r--   0        0        0    36125 2020-02-02 00:00:00.000000 pyimclsts-0.1.2.1/src/pyimclsts/network.py
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 pyimclsts-0.1.2.1/.gitignore
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 pyimclsts-0.1.2.1/LICENSE
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 pyimclsts-0.1.2.1/README.md
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 pyimclsts-0.1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 pyimclsts-0.1.2.1/PKG-INFO
```

### Comparing `pyimclsts-0.1.2/CHANGELOG.md` & `pyimclsts-0.1.2.1/CHANGELOG.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Change log:
 
+## Version 0.1.2.1
+
+### Changed
+    - _peers table now keeps track of entity of unknown vehicles and waits for their announcement to "upgrade" their entry.
+### Fixed
+    - Fixed wrong subscription in .update_peers()
+
 ## Version 0.1.2
 
 ### Added
     - subscriber now has a method called .print_information()
     - subscriber now has a method called .stop()
     - .subscribe_async() can subscribe to categories of messages
```

### Comparing `pyimclsts-0.1.2/example/followRef.py` & `pyimclsts-0.1.2.1/example/followRef.py`

 * *Files identical despite different names*

### Comparing `pyimclsts-0.1.2/example/lsf2csv.py` & `pyimclsts-0.1.2.1/example/lsf2csv.py`

 * *Files identical despite different names*

### Comparing `pyimclsts-0.1.2/example/selectedlsf2csv.py` & `pyimclsts-0.1.2.1/example/selectedlsf2csv.py`

 * *Files identical despite different names*

### Comparing `pyimclsts-0.1.2/src/pyimclsts/_base.py` & `pyimclsts-0.1.2.1/src/pyimclsts/_base.py`

 * *Files identical despite different names*

### Comparing `pyimclsts-0.1.2/src/pyimclsts/core.py` & `pyimclsts-0.1.2.1/src/pyimclsts/core.py`

 * *Files identical despite different names*

### Comparing `pyimclsts-0.1.2/src/pyimclsts/extract.py` & `pyimclsts-0.1.2.1/src/pyimclsts/extract.py`

 * *Files identical despite different names*

### Comparing `pyimclsts-0.1.2/src/pyimclsts/extractutils.py` & `pyimclsts-0.1.2.1/src/pyimclsts/extractutils.py`

 * *Files identical despite different names*

### Comparing `pyimclsts-0.1.2/src/pyimclsts/network.py` & `pyimclsts-0.1.2.1/src/pyimclsts/network.py`

 * *Files 2% similar despite different names*

```diff
@@ -493,14 +493,16 @@
             self._msg_manager = message_bus_st(IO_interface, big_endian)
         self._subscriptions = dict()
         self._subscripted_all = []
         self._periodic = []
         self._call_once = []
 
         # a dictionary of {vehicle name : {'src' : 1, 'entities' : { 1 : 'Entity name'...} ...}}
+        # However, it can temporarily contains int keys denoting src to (temporarily) store information
+        # of vehicles of unknown name
         self._peers = dict()
         # a dictionary of {2: 'vehicle name'}
         self._src2name = dict()
         
         self.subscribe_async(self._abort, _pg.messages.Abort)
         
         self.call_once(self._queryEntityList, delay=1)
@@ -585,33 +587,51 @@
                     name = self._src2name.get(src, None)
                     if name is not None:
                         # if it exists, update; else, create entry
                         if self._peers.get(name, None) is not None:
                             self._peers[name]['EntityList'] = entList
                         else:
                             self._peers[name] = {'EntityList' : entList}
+                    else:
+                        if self._peers.get(src, None) is not None:
+                            self._peers[src]['EntityList'] = entList
+                        else:
+                            self._peers[src] = {'EntityList' : entList}
             
-            elif isinstance(msg, _pg.messages.EntityList):
+            elif isinstance(msg, _pg.messages.EntityInfo):
                 name = self._src2name.get(src, None)
+                
                 if name is not None:
                     # if it exists, update; else, create entry
                     if self._peers.get(name, None) is not None:
                         self._peers[name]['EntityList'][msg.label] = msg.id
                     else:
                         self._peers[name] = {'EntityList' : {msg.label : msg.id}}
+                else:
+                    if self._peers.get(src, None) is not None:
+                        self._peers[src]['EntityList'][msg.label] = msg.id
+                    else:
+                        self._peers[src] = {'EntityList' : {msg.label : msg.id}}
 
             elif isinstance(msg, _pg.messages.Announce):
                 name = msg.sys_name
 
                 self._src2name[src] = name
-                # if it exists, update; else, create entry
-                if self._peers.get(name, None) is not None:
+                
+                temp_value = self._peers.pop(src, None)
+                # check if an int key exists. If it does upgrade it to a normal entry
+                if temp_value is not None:
+                    self._peers[name] = temp_value
                     self._peers[name]['src'] = src
                 else:
-                    self._peers[name] = {'src' : src}
+                    # if it exists, update; else, create entry
+                    if self._peers.get(name, None) is not None:
+                        self._peers[name]['src'] = src
+                    else:
+                        self._peers[name] = {'src' : src}
         else:
             pass
     
     def _get_src(self, vehicle_name : str):
         return self._peers[vehicle_name].get('src', None) if self._peers.get(vehicle_name, None) is not None else None
     
     def _get_src_ent(self, vehicle_name : str, entityName : str):
```

### Comparing `pyimclsts-0.1.2/.gitignore` & `pyimclsts-0.1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pyimclsts-0.1.2/LICENSE` & `pyimclsts-0.1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyimclsts-0.1.2/README.md` & `pyimclsts-0.1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pyimclsts-0.1.2/pyproject.toml` & `pyimclsts-0.1.2.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyimclsts"
-version = "0.1.2"
+version = "0.1.2.1"
 authors = [
   { name = "Choi Wang Dzak" },
 ]
 description = "Python bindings of the IMC message schema"
 readme = "README.md"
 license = {file = "LICENSE"}
 keywords = ["IMC", "IMC message protocol", "LSTS"]
```

### Comparing `pyimclsts-0.1.2/PKG-INFO` & `pyimclsts-0.1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyimclsts
-Version: 0.1.2
+Version: 0.1.2.1
 Summary: Python bindings of the IMC message schema
 Project-URL: Homepage, https://github.com/choiwd/pyimctrans
 Project-URL: Bug Tracker, https://github.com/choiwd/pyimctrans/issues
 Author: Choi Wang Dzak
 License: Copyright (c) 2023 Laboratório de Sistemas e Tecnologia Subaquática
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

