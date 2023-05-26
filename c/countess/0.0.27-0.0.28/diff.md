# Comparing `tmp/countess-0.0.27.tar.gz` & `tmp/countess-0.0.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "countess-0.0.27.tar", last modified: Mon May 15 02:02:20 2023, max compression
+gzip compressed data, was "countess-0.0.28.tar", last modified: Fri May 26 07:10:38 2023, max compression
```

## Comparing `countess-0.0.27.tar` & `countess-0.0.28.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-15 02:02:20.799201 countess-0.0.27/
--rw-rw-r--   0 nick      (1000) nick      (1000)     1469 2022-12-12 02:15:43.000000 countess-0.0.27/LICENSE.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)       26 2023-04-27 04:47:23.000000 countess-0.0.27/MANIFEST.in
--rw-rw-r--   0 nick      (1000) nick      (1000)     3528 2023-05-15 02:02:20.799201 countess-0.0.27/PKG-INFO
--rw-rw-r--   0 nick      (1000) nick      (1000)     2877 2023-05-12 00:34:43.000000 countess-0.0.27/README.md
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-15 02:02:20.795201 countess-0.0.27/countess/
--rw-rw-r--   0 nick      (1000) nick      (1000)       43 2023-05-12 00:34:51.000000 countess-0.0.27/countess/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-15 02:02:20.795201 countess-0.0.27/countess/core/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-08-11 05:48:22.000000 countess-0.0.27/countess/core/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)      736 2023-04-21 06:08:37.000000 countess-0.0.27/countess/core/cmd.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     4271 2023-04-21 06:08:37.000000 countess-0.0.27/countess/core/config.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1910 2023-04-21 06:08:37.000000 countess-0.0.27/countess/core/logger.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    16367 2023-05-12 03:32:05.000000 countess-0.0.27/countess/core/parameters.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     5024 2023-04-21 06:08:37.000000 countess-0.0.27/countess/core/pipeline.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    13178 2023-05-14 22:59:52.000000 countess-0.0.27/countess/core/plugins.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-15 02:02:20.795201 countess-0.0.27/countess/gui/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-04-21 06:08:37.000000 countess-0.0.27/countess/gui/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    21614 2023-05-14 22:59:52.000000 countess-0.0.27/countess/gui/config.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     5947 2023-04-26 02:29:55.000000 countess-0.0.27/countess/gui/logger.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    34675 2023-05-14 22:59:52.000000 countess-0.0.27/countess/gui/main.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-15 02:02:20.799201 countess-0.0.27/countess/plugins/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-04-21 06:08:37.000000 countess-0.0.27/countess/plugins/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     5795 2023-05-14 22:59:52.000000 countess-0.0.27/countess/plugins/csv.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     3711 2023-05-14 22:59:52.000000 countess-0.0.27/countess/plugins/data_table.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1194 2023-04-26 02:29:55.000000 countess-0.0.27/countess/plugins/expression.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2160 2023-05-12 00:43:06.000000 countess-0.0.27/countess/plugins/fastq.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     4385 2023-05-14 22:59:52.000000 countess-0.0.27/countess/plugins/group_by.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1744 2023-04-26 02:29:55.000000 countess-0.0.27/countess/plugins/hdf5.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     3051 2023-05-14 22:59:52.000000 countess-0.0.27/countess/plugins/join.py
--rw-rw-r--   0 nick      (1000) nick      (1000)      347 2023-04-26 02:29:55.000000 countess-0.0.27/countess/plugins/log_score.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2583 2023-05-15 02:00:14.000000 countess-0.0.27/countess/plugins/mutagenize.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     5520 2023-05-14 22:59:52.000000 countess-0.0.27/countess/plugins/pivot.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1477 2023-05-12 00:28:26.000000 countess-0.0.27/countess/plugins/python.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     6776 2023-05-14 22:59:52.000000 countess-0.0.27/countess/plugins/regex.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2039 2023-05-14 22:59:52.000000 countess-0.0.27/countess/plugins/sequence.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2496 2023-05-14 22:59:52.000000 countess-0.0.27/countess/plugins/variant.py
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-08-11 05:39:01.000000 countess-0.0.27/countess/py.typed
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-15 02:02:20.799201 countess-0.0.27/countess/utils/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-09-26 22:30:04.000000 countess-0.0.27/countess/utils/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    12859 2023-05-12 02:00:10.000000 countess-0.0.27/countess/utils/variant.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-15 02:02:20.795201 countess-0.0.27/countess.egg-info/
--rw-rw-r--   0 nick      (1000) nick      (1000)     3528 2023-05-15 02:02:20.000000 countess-0.0.27/countess.egg-info/PKG-INFO
--rw-rw-r--   0 nick      (1000) nick      (1000)     1054 2023-05-15 02:02:20.000000 countess-0.0.27/countess.egg-info/SOURCES.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)        1 2023-05-15 02:02:20.000000 countess-0.0.27/countess.egg-info/dependency_links.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)      997 2023-05-15 02:02:20.000000 countess-0.0.27/countess.egg-info/entry_points.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)      239 2023-05-15 02:02:20.000000 countess-0.0.27/countess.egg-info/requires.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)        9 2023-05-15 02:02:20.000000 countess-0.0.27/countess.egg-info/top_level.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)     2697 2023-05-09 09:16:21.000000 countess-0.0.27/pyproject.toml
--rw-rw-r--   0 nick      (1000) nick      (1000)     1444 2023-05-15 02:02:20.799201 countess-0.0.27/setup.cfg
--rw-rw-r--   0 nick      (1000) nick      (1000)       39 2023-04-21 06:08:37.000000 countess-0.0.27/setup.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-15 02:02:20.799201 countess-0.0.27/tests/
--rw-rw-r--   0 nick      (1000) nick      (1000)      636 2023-04-21 06:08:37.000000 countess-0.0.27/tests/test_gui.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-26 07:10:38.627911 countess-0.0.28/
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1469 2022-12-12 02:15:43.000000 countess-0.0.28/LICENSE.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)       26 2023-05-25 01:44:18.000000 countess-0.0.28/MANIFEST.in
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3477 2023-05-26 07:10:38.627911 countess-0.0.28/PKG-INFO
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2877 2023-05-26 07:08:39.000000 countess-0.0.28/README.md
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-26 07:10:38.623911 countess-0.0.28/countess/
+-rw-rw-r--   0 nick      (1000) nick      (1000)       43 2023-05-26 07:08:45.000000 countess-0.0.28/countess/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-26 07:10:38.623911 countess-0.0.28/countess/core/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-08-11 05:48:22.000000 countess-0.0.28/countess/core/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)      415 2023-05-25 01:44:18.000000 countess-0.0.28/countess/core/cmd.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     4157 2023-05-25 01:44:18.000000 countess-0.0.28/countess/core/config.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1910 2023-05-25 01:44:18.000000 countess-0.0.28/countess/core/logger.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    16461 2023-05-26 07:02:31.000000 countess-0.0.28/countess/core/parameters.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     5938 2023-05-26 07:05:39.000000 countess-0.0.28/countess/core/pipeline.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    13181 2023-05-26 07:05:55.000000 countess-0.0.28/countess/core/plugins.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-26 07:10:38.623911 countess-0.0.28/countess/gui/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-05-25 01:44:18.000000 countess-0.0.28/countess/gui/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    18762 2023-05-26 07:05:55.000000 countess-0.0.28/countess/gui/config.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     5947 2023-05-25 01:44:18.000000 countess-0.0.28/countess/gui/logger.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    34169 2023-05-26 07:05:56.000000 countess-0.0.28/countess/gui/main.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    12797 2023-05-26 06:50:03.000000 countess-0.0.28/countess/gui/tabular.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-26 07:10:38.627911 countess-0.0.28/countess/plugins/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-05-25 01:44:18.000000 countess-0.0.28/countess/plugins/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     5969 2023-05-26 07:05:55.000000 countess-0.0.28/countess/plugins/csv.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3711 2023-05-26 07:05:55.000000 countess-0.0.28/countess/plugins/data_table.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1236 2023-05-25 01:44:18.000000 countess-0.0.28/countess/plugins/expression.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2160 2023-05-25 01:44:18.000000 countess-0.0.28/countess/plugins/fastq.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     4385 2023-05-26 07:05:55.000000 countess-0.0.28/countess/plugins/group_by.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1744 2023-05-25 01:44:18.000000 countess-0.0.28/countess/plugins/hdf5.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3051 2023-05-26 07:05:55.000000 countess-0.0.28/countess/plugins/join.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)      347 2023-05-25 01:44:18.000000 countess-0.0.28/countess/plugins/log_score.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2562 2023-05-25 01:44:18.000000 countess-0.0.28/countess/plugins/mutagenize.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     5520 2023-05-26 07:05:55.000000 countess-0.0.28/countess/plugins/pivot.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1477 2023-05-25 01:44:18.000000 countess-0.0.28/countess/plugins/python.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     6784 2023-05-26 07:05:55.000000 countess-0.0.28/countess/plugins/regex.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2039 2023-05-26 07:05:55.000000 countess-0.0.28/countess/plugins/sequence.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2496 2023-05-26 07:05:55.000000 countess-0.0.28/countess/plugins/variant.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-08-11 05:39:01.000000 countess-0.0.28/countess/py.typed
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-26 07:10:38.627911 countess-0.0.28/countess/utils/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-09-26 22:30:04.000000 countess-0.0.28/countess/utils/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    12859 2023-05-25 01:44:18.000000 countess-0.0.28/countess/utils/variant.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-26 07:10:38.623911 countess-0.0.28/countess.egg-info/
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3477 2023-05-26 07:10:38.000000 countess-0.0.28/countess.egg-info/PKG-INFO
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1068 2023-05-26 07:10:38.000000 countess-0.0.28/countess.egg-info/SOURCES.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)        1 2023-05-26 07:10:38.000000 countess-0.0.28/countess.egg-info/dependency_links.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)      997 2023-05-26 07:10:38.000000 countess-0.0.28/countess.egg-info/entry_points.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)      201 2023-05-26 07:10:38.000000 countess-0.0.28/countess.egg-info/requires.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)        9 2023-05-26 07:10:38.000000 countess-0.0.28/countess.egg-info/top_level.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2809 2023-05-26 06:01:26.000000 countess-0.0.28/pyproject.toml
+-rw-rw-r--   0 nick      (1000) nick      (1000)       38 2023-05-26 07:10:38.627911 countess-0.0.28/setup.cfg
+-rw-rw-r--   0 nick      (1000) nick      (1000)       39 2023-05-25 01:44:18.000000 countess-0.0.28/setup.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-26 07:10:38.627911 countess-0.0.28/tests/
+-rw-rw-r--   0 nick      (1000) nick      (1000)      480 2023-05-25 01:44:18.000000 countess-0.0.28/tests/test_gui.py
```

### Comparing `countess-0.0.27/LICENSE.txt` & `countess-0.0.28/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `countess-0.0.27/PKG-INFO` & `countess-0.0.28/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: countess
-Version: 0.0.27
+Version: 0.0.28
 Summary: CountESS
-Author: CountESS Developers
 Author-email: Nick Moore <nick@zoic.org>, Alan Rubin <alan@rubin.id.au>
-Maintainer: Nick Moore
 Maintainer-email: Nick Moore <nick@zoic.org>
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: hdf
 License-File: LICENSE.txt
 
-# CountESS 0.0.27
+# CountESS 0.0.28
 
 This is CountESS, a modular, Python 3 reimplementation of Enrich2.
 
 ## License
 
 BSD 3-clause.  See [LICENSE.txt](LICENSE.txt)
```

### Comparing `countess-0.0.27/README.md` & `countess-0.0.28/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# CountESS 0.0.27
+# CountESS 0.0.28
 
 This is CountESS, a modular, Python 3 reimplementation of Enrich2.
 
 ## License
 
 BSD 3-clause.  See [LICENSE.txt](LICENSE.txt)
```

### Comparing `countess-0.0.27/countess/core/config.py` & `countess-0.0.28/countess/core/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,33 +58,29 @@
         # XXX check version and hash_digest and emit warnings.
 
         node = PipelineNode(
             name=section_name,
             plugin=plugin,
             position=position,
             notes=notes,
+            is_dirty=True,
         )
         pipeline_graph.nodes.append(node)
 
         for key, val in config_dict.items():
             if key.startswith("_parent."):
                 node.add_parent(nodes_by_name[val])
 
-        nodes_by_name[section_name] = node
-
-        if plugin:
-            # XXX progress callback for preruns.
-            node.prepare(logger)
-
-            for key, val in config_dict.items():
-                if key.startswith("_"):
-                    continue
-                node.configure_plugin(key, ast.literal_eval(val), base_dir)
+        node.config = [
+            (key, ast.literal_eval(val), base_dir)
+            for key, val in config_dict.items()
+            if not key.startswith("_")
+        ]
 
-            node.prerun(logger)
+        nodes_by_name[section_name] = node
 
     return pipeline_graph
 
 
 def write_config(pipeline_graph: PipelineGraph, filename: str):
     """Write `pipeline_graph`'s configuration out to `filename`"""
 
@@ -99,15 +95,16 @@
                     "_module": node.plugin.__module__,
                     "_class": node.plugin.__class__.__name__,
                     "_version": node.plugin.version,
                     "_hash": node.plugin.hash(),
                 }
             )
         if node.position:
-            cp[node.name]["_position"] = " ".join(str(int(x * 1000)) for x in node.position)
+            xx, yy = node.position
+            cp[node.name]["_position"] = "%d %d" % (xx * 1000, yy * 1000)
         if node.notes:
             cp[node.name]["_notes"] = node.notes
         for n, parent in enumerate(node.parent_nodes):
             cp[node.name][f"_parent.{n}"] = parent.name
         if node.plugin:
             for k, v in node.plugin.get_parameters(base_dir):
                 cp[node.name][k] = repr(v)
```

### Comparing `countess-0.0.27/countess/core/logger.py` & `countess-0.0.28/countess/core/logger.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.27/countess/core/parameters.py` & `countess-0.0.28/countess/core/parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,15 +184,20 @@
                             break
                         digest.update(data)
             return digest.hexdigest()
         except IOError:
             return "0"
 
     def get_parameters(self, key, base_dir="."):
-        return ((key, os.path.relpath(self.value, base_dir)),)
+        if self.value:
+            relpath = os.path.relpath(self.value, base_dir)
+        else:
+            relpath = None
+
+        return [(key, relpath)]
 
     def copy(self):
         return self.__class__(self.label, self.value, self.read_only, file_types=self.file_types)
 
     def get_hash_value(self) -> str:
         # For reproducability, we don't actually care about the filename, just
         # its hash.
```

### Comparing `countess-0.0.27/countess/core/pipeline.py` & `countess-0.0.28/countess/core/pipeline.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,17 +11,22 @@
 class PipelineNode:
     name: str
     plugin: Optional[BasePlugin] = None
     position: Optional[tuple[float, float]] = None
     notes: Optional[str] = None
     parent_nodes: set["PipelineNode"] = field(default_factory=set)
     child_nodes: set["PipelineNode"] = field(default_factory=set)
+    config: Optional[list[tuple[str, str, str]]] = None
     result: Any = None
     is_dirty: bool = True
 
+    # XXX config is a cache for config loaded from the file
+    # at config load time, if it is present it is loaded the
+    # first time the plugin is prerun.
+
     def __hash__(self):
         return id(self)
 
     def is_ancestor_of(self, node):
         return (self in node.parent_nodes) or any(
             (self.is_ancestor_of(n) for n in node.parent_nodes)
         )
@@ -46,32 +51,52 @@
             try:
                 self.result = self.plugin.run(input_data, logger, row_limit)
             except Exception as exc:  # pylint: disable=W0718
                 logger.exception(exc)
         else:
             self.result = input_data
 
+    def load_config(self, logger: Logger):
+        assert isinstance(self.plugin, BasePlugin)
+        if self.config:
+            for key, val, base_dir in self.config:
+                try:
+                    self.plugin.set_parameter(key, val, base_dir)
+                except (KeyError, ValueError) as exc:
+                    logger.warning(f"Parameter {key}={val} Not Found")
+                    print(exc)
+            self.config = None
+
     def prepare(self, logger: Logger):
         assert isinstance(logger, Logger)
+
         input_data = self.get_input_data()
         if self.plugin:
             try:
                 self.plugin.prepare(input_data, logger)
+                self.load_config(logger)
             except Exception as exc:  # pylint: disable=W0718
                 logger.exception(exc)
+
         else:
             self.result = input_data
 
     def prerun(self, logger: Logger, row_limit=PRERUN_ROW_LIMIT):
         assert isinstance(logger, Logger)
+
         if self.is_dirty and self.plugin:
+            logger.info(f"Prerun {self.name} Start")
             for parent_node in self.parent_nodes:
                 parent_node.prerun(logger, row_limit)
+            self.prepare(logger)
+            self.load_config(logger)
+
             self.execute(logger, row_limit)
             self.is_dirty = False
+            logger.info(f"Prerun {self.name} Done")
 
     def mark_dirty(self):
         self.is_dirty = True
         for child_node in self.child_nodes:
             if not child_node.is_dirty:
                 child_node.mark_dirty()
 
@@ -140,13 +165,14 @@
         # might be easier to just keep a set of nodes and sort through
         # them for output nodes, or something.
 
         for node in self.traverse_nodes():
             # XXX TODO there's some opportunity for easy parallelization here,
             # by pushing each node into a pool as soon as its parents are
             # complete.
+            node.prepare(logger)
             node.execute(logger)
 
     def reset(self):
         for node in self.nodes:
             node.result = None
             node.is_dirty = True
```

### Comparing `countess-0.0.27/countess/core/plugins.py` & `countess-0.0.28/countess/core/plugins.py`

 * *Files 0% similar despite different names*

```diff
@@ -346,15 +346,15 @@
                 },
             ),
             min_size=1,
         )
     }
 
     def prepare_df(self, df, logger):
-        super().prepare(df, logger)
+        super().prepare_df(df, logger)
         for pp in self.parameters["scores"]:
             for ppp in pp.counts:
                 ppp.choices = self.input_columns
 
     def run_df(self, df: pd.DataFrame, logger: Logger) -> pd.DataFrame:
         assert isinstance(self.parameters["scores"], ArrayParam)
         score_cols = []
```

### Comparing `countess-0.0.27/countess/gui/config.py` & `countess-0.0.28/countess/gui/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 # TK based GUI for CountESS
 import math
 import tkinter as tk
 from functools import partial
-from tkinter import filedialog, ttk
+from tkinter import filedialog
 from typing import Mapping, MutableMapping, Optional
 
 import numpy as np
-import pandas as pd
-from pandas.api.types import is_numeric_dtype  # type: ignore
 
 from ..core.parameters import (
     ArrayParam,
     BaseParam,
     BooleanParam,
     ChoiceParam,
     FileArrayParam,
@@ -45,14 +43,15 @@
         self,
         tk_parent: tk.Widget,
         parameter: BaseParam,
         callback=None,
         delete_callback=None,
         level=0,
     ):
+        self.tk_parent = tk_parent
         self.parameter = parameter
         self.callback = callback
         self.button = None
         self.level = level
         self.subwrapper_buttons: list[tk.Button] = []
         self.column_labels: list[tk.Label] = []
 
@@ -62,53 +61,50 @@
         self.entry: Optional[tk.Widget] = None
         self.label: Optional[tk.Widget] = None
         self.row_labels: list[tk.Widget] = []
 
         if isinstance(parameter, ArrayParam):
             self.label = None
         else:
-            self.label = ttk.Label(tk_parent, text=parameter.label)
+            self.label = tk.Label(tk_parent, text=parameter.label)
 
         if isinstance(parameter, ChoiceParam):
             self.var = tk.StringVar(tk_parent, value=parameter.value)
-            self.entry = ttk.Combobox(tk_parent, textvariable=self.var)
-            self.entry["values"] = parameter.choices
-            self.entry.state(["readonly"])  # don't allow other options
+            choices = parameter.choices or [""]
+            self.entry = tk.OptionMenu(tk_parent, self.var, *choices)
         elif isinstance(parameter, BooleanParam):
             self.entry = tk.Button(tk_parent, width=2, command=self.toggle_checkbox_callback)
             self.set_checkbox_value()
         elif isinstance(parameter, FileParam):
-            self.var = tk.StringVar(tk_parent, value=parameter.value)
-            self.entry = ttk.Entry(tk_parent, textvariable=self.var)
-            self.entry.state(["readonly"])
+            self.entry = tk.Label(tk_parent, text=parameter.value)
             self.button = tk.Button(
                 tk_parent, text="Select", width=3, command=self.change_file_callback
             )
         elif isinstance(parameter, TextParam):
             # tk.Text widget doesn't have a variable, for whatever reason,
             # so we use a different method!
             # XXX is this a simpler way to handle other kinds of fields too?
             self.entry = tk.Text(tk_parent, height=10)
             self.entry.insert("1.0", parameter.value)
             if parameter.read_only:
-                self.entry["state"] = "disabled"
+                self.entry["state"] = tk.DISABLED
             else:
                 self.entry.bind("<<Modified>>", self.widget_modified_callback)
         elif isinstance(parameter, SimpleParam):
             self.var = tk.StringVar(tk_parent, value=parameter.value)
-            self.entry = ttk.Entry(tk_parent, textvariable=self.var)
+            self.entry = tk.Entry(tk_parent, textvariable=self.var)
             if parameter.read_only:
-                self.entry.state(["readonly"])
+                self.entry["state"] = tk.DISABLED
 
         elif (
             isinstance(parameter, ArrayParam)
             and self.level == 0
             and not isinstance(parameter.param, TabularMultiParam)
         ):
-            self.entry = ttk.Frame(tk_parent)
+            self.entry = tk.Frame(tk_parent)
             self.entry.columnconfigure(0, weight=1)
             drc = self.delete_row_callback if not parameter.read_only else None
             self.update_subwrappers_framed(parameter.params, drc)
             if not parameter.read_only:
                 self.button = tk.Button(
                     self.entry,
                     text=f"Add {parameter.param.label}",
@@ -142,15 +138,15 @@
                 # XXX hack because the empty labelframe collapses
                 # for some reason.
                 tk.Label(self.entry, text="").grid()
 
                 self.update_subwrappers(parameter.params, drc)
 
         elif isinstance(parameter, (ArrayParam, MultiParam)):
-            self.entry = ttk.Frame(tk_parent)
+            self.entry = tk.Frame(tk_parent)
             self.entry.columnconfigure(0, weight=0)
             self.entry.columnconfigure(1, weight=0)
             self.entry.columnconfigure(2, weight=1)
             if isinstance(parameter, ArrayParam):
                 drc = self.delete_row_callback if not parameter.read_only else None
                 self.update_subwrappers(parameter.params, drc)
                 self.button = tk.Button(
@@ -210,23 +206,28 @@
                     if self.parameter.max_size is not None
                     and len(self.subwrappers) >= self.parameter.max_size
                     else tk.NORMAL
                 )
         elif isinstance(self.parameter, MultiParam):
             self.update_subwrappers(self.parameter.params.values(), None)
         elif isinstance(self.parameter, ChoiceParam):
-            self.entry["values"] = self.parameter.choices
+            self.entry.destroy()
+            choices = self.parameter.choices or [""]
+            self.entry = tk.OptionMenu(self.tk_parent, self.var, *choices)
+            self.entry.grid(sticky=tk.EW, padx=10, pady=5)
         elif isinstance(self.parameter, BooleanParam):
             self.set_checkbox_value()
         elif isinstance(self.parameter, TextParam):
             if self.parameter.read_only:
                 self.entry["state"] = "normal"
             self.entry.replace("1.0", tk.END, self.parameter.value)
             if self.parameter.read_only:
                 self.entry["state"] = "disabled"
+        elif isinstance(self.parameter, FileParam):
+            self.entry["text"] = self.parameter.value
         else:
             self.var.set(self.parameter.value)
 
         if self.label:
             self.label["text"] = self.parameter.label
 
     def cull_subwrappers(self, params):
@@ -314,15 +315,15 @@
                     label_frame,
                     p,
                     self.callback,
                     delete_row_callback,
                     level=self.level + 1,
                 )
                 if delete_row_callback:
-                    button = ttk.Button(
+                    button = tk.Button(
                         label_frame_label,
                         text=UNICODE_CROSS,
                         width=2,
                         command=partial(_command_drc, p, label_frame),
                     )
                     button.grid(row=0, column=1, padx=10)
 
@@ -440,21 +441,21 @@
     output_text = None
     preview = None
 
     def __init__(self, tk_parent: tk.Widget, plugin: BasePlugin, change_callback=None):
         self.plugin = plugin
         self.change_callback = change_callback
 
-        self.frame = ttk.Frame(tk_parent)
+        self.frame = tk.Frame(tk_parent)
         self.frame.columnconfigure(0, weight=1)
         self.frame.grid(sticky=tk.NSEW)
 
         self.wrapper_cache: MutableMapping[str, ParameterWrapper] = {}
 
-        self.subframe = ttk.Frame(self.frame)
+        self.subframe = tk.Frame(self.frame)
         self.subframe.columnconfigure(0, weight=0)
         self.subframe.columnconfigure(1, weight=0)
         self.subframe.columnconfigure(2, weight=1)
         self.subframe.grid(row=1, sticky=tk.NSEW)
 
         self.update()
 
@@ -480,75 +481,7 @@
             self.wrapper_cache[key].set_row(n + 1)
 
         # Remove any parameter wrappers no longer needed
         for key, wrapper in list(self.wrapper_cache.items()):
             if key not in self.plugin.parameters:
                 wrapper.destroy()
                 del self.wrapper_cache[key]
-
-
-class DataFramePreview:
-    """Provides a visual preview of a Dask dataframe arranged as a table."""
-
-    # XXX uses a treeview, which seemed like a good match but actually a grid-layout
-    # of custom styled labels might work better.
-
-    def __init__(self, tk_parent, ddf: Optional[pd.DataFrame] = None, max_rows: int = 10000):
-        self.frame = ttk.Frame(tk_parent)
-        self.label = ttk.Label(self.frame, text="DataFrame Preview")
-        self.max_rows = max_rows
-
-        self.treeview = ttk.Treeview(self.frame, selectmode=tk.NONE)
-
-        self.scrollbar_x = ttk.Scrollbar(
-            self.frame, orient=tk.HORIZONTAL, command=self.treeview.xview
-        )
-        self.scrollbar_y = ttk.Scrollbar(
-            self.frame, orient=tk.VERTICAL, command=self.treeview.yview
-        )
-        self.treeview.configure(xscrollcommand=self.scrollbar_x.set)
-        self.treeview.configure(yscrollcommand=self.scrollbar_y.set)
-
-        self.frame.grid(sticky=tk.NSEW)
-
-        self.frame.columnconfigure(0, weight=1)
-        self.frame.rowconfigure(1, weight=1)
-        self.label.grid(row=0, columnspan=2)
-        self.treeview.grid(row=1, column=0, sticky=tk.NSEW)
-        self.scrollbar_x.grid(row=2, column=0, sticky=tk.EW)
-        self.scrollbar_y.grid(row=1, column=1, stick=tk.NS)
-
-        if ddf is not None:
-            self.update(ddf)
-
-    def update(self, ddf: pd.DataFrame):
-        if len(ddf) > self.max_rows:
-            self.label["text"] = f"DataFrame Preview ({self.max_rows} rows out of {len(ddf)})"
-            ddf = ddf[0:1000]
-        else:
-            self.label["text"] = f"DataFrame Preview {len(ddf)} rows"
-
-        # XXX could handle multiindex columns more elegantly than this
-        # (but maybe not in a ttk.Treeview)
-        column_names = ["__".join(c) if isinstance(c, tuple) else c for c in ddf.columns]
-
-        self.treeview["columns"] = column_names
-
-        for n, (column_name, column_dtype) in enumerate(zip(column_names, ddf.dtypes)):
-            self.treeview.heading(n, text=f"{column_name} ({column_dtype.name})")
-            # XXX it'd be nicer if we could do "real" decimal point alignment
-            anchor = tk.E if is_numeric_dtype(column_dtype) else tk.W
-            # XXX type signature appears to be wrong, or at least overly restrictive.
-            # I think I'm going to replace treeview anyway so I'm ignoring it for now.
-            self.treeview.column(
-                n, anchor=anchor, width=100, minwidth=100, stretch=tk.YES
-            )  # type: ignore
-
-        for row in self.treeview.get_children():
-            self.treeview.delete(row)
-
-        for n, (index, *values) in enumerate(ddf.itertuples()):
-            values = ["—" if is_nan(v) else str(v) for v in values]
-            self.treeview.insert("", n, text=index, values=values)
-
-    def destroy(self):
-        self.frame.destroy()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `countess-0.0.27/countess/gui/logger.py` & `countess-0.0.28/countess/gui/logger.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.27/countess/gui/main.py` & `countess-0.0.28/countess/gui/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,26 +2,27 @@
 import random
 import re
 import sys
 import tkinter as tk
 import webbrowser
 from enum import Enum, IntFlag
 from functools import partial
-from tkinter import filedialog, font, messagebox, ttk
+from tkinter import filedialog, messagebox
 from typing import Optional
 
 import pandas as pd
 
 from countess import VERSION
 from countess.core.config import export_config_graphviz, read_config, write_config
 from countess.core.logger import ConsoleLogger
 from countess.core.pipeline import PipelineGraph, PipelineNode
 from countess.core.plugins import get_plugin_classes
-from countess.gui.config import DataFramePreview, PluginConfigurator
+from countess.gui.config import PluginConfigurator
 from countess.gui.logger import LoggerFrame
+from countess.gui.tabular import TabularDataFrame
 
 # import faulthandler
 # faulthandler.enable(all_threads=True)
 
 
 def _limit(value, min_value, max_value):
     return max(min_value, min(max_value, value))
@@ -238,21 +239,21 @@
 
         self.columnconfigure(0, weight=1)
 
         label_frame = tk.LabelFrame(self, text=title, padx=10, pady=10)
         label_frame.grid(row=1, column=0, sticky=tk.EW, padx=10, pady=10)
 
         for n, plugin_class in enumerate(plugin_classes):
-            label_text = plugin_class.description.split(". ")[0]
-            ttk.Button(
+            label_text = plugin_class.description.split(". ")[0].strip()
+            tk.Button(
                 label_frame,
                 text=plugin_class.name,
                 command=lambda plugin_class=plugin_class: callback(plugin_class),
             ).grid(row=n + 1, column=0, sticky=tk.EW)
-            ttk.Label(label_frame, text=label_text).grid(row=n + 1, column=1, sticky=tk.W, padx=10)
+            tk.Label(label_frame, text=label_text).grid(row=n + 1, column=1, sticky=tk.W, padx=10)
 
 
 class FlippyCanvas(FixedUnbindMixin, tk.Canvas):
     """A canvas which flips all its children's X and Y
     coordinates when it goes from portrait to landscape.
     Place children with .place(relx=, rely=) for best results."""
 
@@ -598,19 +599,19 @@
             else:
                 self.show_preview_subframe()
 
     def show_config_subframe(self):
         if self.config_canvas:
             self.config_canvas.destroy()
         self.config_canvas = tk.Canvas(self.frame)
-        self.config_scrollbar = ttk.Scrollbar(
+        self.config_scrollbar = tk.Scrollbar(
             self.frame, orient=tk.VERTICAL, command=self.config_canvas.yview
         )
         self.config_canvas.configure(yscrollcommand=self.config_scrollbar.set, bd=0)
-        self.config_canvas.grid(row=3, sticky=tk.NSEW)
+        self.config_canvas.grid(row=3, column=0, sticky=tk.NSEW)
         self.config_scrollbar.grid(row=3, column=1, sticky=tk.NS)
 
         self.node.prepare(self.logger)
 
         if self.node.plugin:
             if self.node.notes:
                 self.show_notes_widget(self.node.notes)
@@ -626,24 +627,24 @@
                 self.node.plugin.name,
                 self.node.plugin.version,
                 descr,
             )
             if self.node.plugin.link:
                 tk.Button(
                     self.frame, text=UNICODE_INFO, fg="blue", command=self.on_info_button_press
-                ).grid(row=1, column=1, sticky=tk.SE, padx=10)
+                ).place(anchor=tk.NE, relx=1, y=50)
             self.node.prepare(self.logger)
             self.node.plugin.update()
             self.configurator = PluginConfigurator(
                 self.config_canvas, self.node.plugin, self.config_change_callback
             )
             self.config_subframe = self.configurator.frame
         else:
             self.config_subframe = PluginChooserFrame(
-                self.frame, "Choose Plugin", self.choose_plugin
+                self.config_canvas, "Choose Plugin", self.choose_plugin
             )
         self.config_subframe_id = self.config_canvas.create_window(
             (0, 0), window=self.config_subframe, anchor=tk.NW
         )
         self.config_subframe.bind(
             "<Configure>",
             lambda e: self.config_canvas.configure(scrollregion=self.config_canvas.bbox("all")),
@@ -671,15 +672,16 @@
         self.notes_widget.bind("<<Modified>>", self.notes_modified_callback)
         self.notes_widget.grid(row=2, columnspan=2, sticky=tk.EW, padx=10, pady=5)
 
     def show_preview_subframe(self):
         if self.preview_subframe:
             self.preview_subframe.destroy()
         if isinstance(self.node.result, pd.DataFrame):
-            self.preview_subframe = DataFramePreview(self.frame, self.node.result).frame
+            self.preview_subframe = TabularDataFrame(self.frame)
+            self.preview_subframe.set_dataframe(self.node.result)
         elif isinstance(self.node.result, str):
             self.preview_subframe = tk.Frame(self.frame)
             self.preview_subframe.rowconfigure(1, weight=1)
             n_lines = len(self.node.result.splitlines())
             tk.Label(self.preview_subframe, text=f"Text Preview {n_lines} Lines").grid(
                 sticky=tk.NSEW
             )
@@ -691,18 +693,18 @@
             self.preview_subframe = tk.Frame(self.frame)
             self.preview_subframe.columnconfigure(0, weight=1)
             tk.Label(self.preview_subframe, text="no result").grid(sticky=tk.EW)
 
         self.preview_subframe.grid(row=4, columnspan=2, sticky=tk.NSEW)
 
         self.logger_subframe.grid(row=5, columnspan=2, sticky=tk.NSEW)
-        # if self.logger.count > 0:
-        #    self.logger_subframe.grid(row=5, columnspan=2, sticky=tk.NSEW)
-        # else:
-        #    self.logger_subframe.grid_forget()
+        if self.logger.count > 0:
+            self.logger_subframe.grid(row=5, columnspan=2, sticky=tk.NSEW)
+        else:
+            self.logger_subframe.grid_forget()
 
     def name_changed_callback(self, *_):
         name = self.name_var.get()
         self.node.name = name
         self.change_callback(self.node)
 
     def notes_modified_callback(self, *_):
@@ -789,14 +791,15 @@
 
         self.frame = tk.Frame(tk_parent)
         self.frame.grid(sticky=tk.NSEW)
 
         self.canvas = FlippyCanvas(self.frame, bg="skyblue")
         self.subframe = tk.Frame(self.frame)
         self.subframe.columnconfigure(0, weight=1)
+        self.subframe.columnconfigure(1, weight=0)
         self.subframe.rowconfigure(0, weight=0)
         self.subframe.rowconfigure(1, weight=0)
         self.subframe.rowconfigure(2, weight=0)
         self.subframe.rowconfigure(3, weight=1)
         self.subframe.rowconfigure(4, weight=2)
         self.subframe.rowconfigure(5, weight=0)
 
@@ -887,32 +890,15 @@
         else:
             y = event.height // 4
             self.canvas.place(x=0, y=0, w=event.width, h=y)
             self.subframe.place(x=0, y=y, w=event.width, h=event.height - y)
 
 
 def make_root():
-    try:
-        import ttkthemes  # pylint: disable=C0415
-
-        root = ttkthemes.ThemedTk()
-        themes = set(root.get_themes())
-        for t in ["winnative", "aqua", "clam"]:
-            if t in themes:
-                root.set_theme(t)
-    except ImportError:
-        root = tk.Tk()
-        # XXX some kind of ttk style setup goes here as a fallback
-
-    # Set up treeview font and row heights.
-    linespace = font.Font(None, 10).metrics()["linespace"]
-    style = ttk.Style()
-    style.configure("Treeview", font=(None, 10), rowheight=linespace)
-    style.configure("Treeview.Heading", font=(None, 10, "bold"), rowheight=linespace)
-
+    root = tk.Tk()
     root.title(f"CountESS {VERSION}")
     root.rowconfigure(0, weight=0)
     root.rowconfigure(1, weight=1)
     root.columnconfigure(0, weight=1)
 
     # Try to start off maximized, but this option doesn't exist
     # in all Tks or all platforms.
```

### Comparing `countess-0.0.27/countess/plugins/csv.py` & `countess-0.0.28/countess/plugins/csv.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,48 +51,56 @@
 
     parameters = {
         "delimiter": ChoiceParam("Delimiter", ",", choices=[",", ";", "TAB", "|", "WHITESPACE"]),
         "quoting": ChoiceParam(
             "Quoting", "None", choices=["None", "Double-Quote", "Quote with Escape"]
         ),
         "comment": ChoiceParam("Comment", "None", choices=["None", "#", ";"]),
+        "header": BooleanParam("CSV file has header row?", True),
+        "filename_column": StringParam("Filename Column", ""),
         "columns": ArrayParam(
             "Columns",
             MultiParam(
                 "Column",
                 {
                     "name": StringParam("Column Name", ""),
                     "type": DataTypeOrNoneChoiceParam("Column Type"),
                     "index": BooleanParam("Index?", False),
                 },
             ),
         ),
-        "header": BooleanParam("CSV file has header row?", True),
-        "filename_column": StringParam("Filename Column", ""),
     }
 
     def read_file_to_dataframe(self, file_params, logger, row_limit=None):
         filename = file_params["filename"].value
 
         options = {
             "header": 0 if self.parameters["header"].value else None,
         }
         if row_limit is not None:
             options["nrows"] = row_limit
 
+        index_col_numbers = []
+
         if len(self.parameters["columns"]):
             options["names"] = []
             options["dtype"] = {}
             options["usecols"] = []
 
             for n, pp in enumerate(self.parameters["columns"]):
                 options["names"].append(pp["name"].value or f"column_{n}")
                 if not pp["type"].is_none():
-                    options["dtype"][n] = pp["type"].get_selected_type()
+                    if pp["index"].value:
+                        index_col_numbers.append(len(options["usecols"]))
                     options["usecols"].append(n)
+                    options["dtype"][n] = pp["type"].get_selected_type()
+
+        if not options["dtype"]:
+            logger.warning("No Columns Selected")
+            return pd.DataFrame()
 
         delimiter = self.parameters["delimiter"].value
         if delimiter == "TAB":
             options["delimiter"] = "\t"
         elif delimiter == "WHITESPACE":
             options["delim_whitespace"] = True
         else:
@@ -125,19 +133,16 @@
                 if not self.parameters["columns"][n]["name"].value:
                     self.parameters["columns"][n]["name"].value = str(col)
 
         filename_column = self.parameters["filename_column"].value
         if filename_column:
             df[filename_column] = filename
 
-        index_cols = [
-            df.columns[n] for n, pp in enumerate(self.parameters["columns"]) if pp["index"].value
-        ]
-        if index_cols:
-            df = df.set_index(index_cols)
+        if index_col_numbers:
+            df = df.set_index([df.columns[n] for n in index_col_numbers])
 
         return df
 
 
 class SaveCsvPlugin(PandasBasePlugin):
     name = "CSV Save"
     description = "Save data as CSV or similar delimited text files"
```

### Comparing `countess-0.0.27/countess/plugins/data_table.py` & `countess-0.0.28/countess/plugins/data_table.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.27/countess/plugins/expression.py` & `countess-0.0.28/countess/plugins/expression.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from countess.core.logger import Logger
 from countess.core.parameters import TextParam
 from countess.core.plugins import PandasTransformPlugin
 
 
 def process(df: pd.DataFrame, codes, logger: Logger):
     for code in codes:
+        if not code:
+            continue
         try:
             result = df.eval(code)
         except Exception as exc:  # pylint: disable=W0718
             logger.error(str(exc))
             continue
 
         if isinstance(result, pd.Series):
```

### Comparing `countess-0.0.27/countess/plugins/fastq.py` & `countess-0.0.28/countess/plugins/fastq.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.27/countess/plugins/group_by.py` & `countess-0.0.28/countess/plugins/group_by.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.27/countess/plugins/hdf5.py` & `countess-0.0.28/countess/plugins/hdf5.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.27/countess/plugins/join.py` & `countess-0.0.28/countess/plugins/join.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.27/countess/plugins/mutagenize.py` & `countess-0.0.28/countess/plugins/mutagenize.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,9 +64,9 @@
                 ),
                 0,
                 row_limit,
             ),
             columns=["sequence", "position", "reference", "variation"],
         )
         if self.parameters["remove"].value:
-            df = df.drop(columns="hgvs").groupby("sequence").agg("first")
+            df = df.groupby("sequence").agg("first")
         return df
```

### Comparing `countess-0.0.27/countess/plugins/pivot.py` & `countess-0.0.28/countess/plugins/pivot.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.27/countess/plugins/python.py` & `countess-0.0.28/countess/plugins/python.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.27/countess/plugins/regex.py` & `countess-0.0.28/countess/plugins/regex.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
                     "drop_unmatch": BooleanParam("Drop Unmatched Rows", False),
                 },
             ),
         ),
     }
 
     def apply_func(self, column_name, compiled_re, output_params, logger, row):
-        value = str(row[column_name])
+        value = str(row.get(column_name, ""))
         match = compiled_re.match(value)
         if match:
             return [1] + [
                 output_params[n].datatype.cast_value(g) for n, g in enumerate(match.groups())
             ]
         else:
             logger.warning("Didn't Match", detail=repr(value))
```

### Comparing `countess-0.0.27/countess/plugins/sequence.py` & `countess-0.0.28/countess/plugins/sequence.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.27/countess/plugins/variant.py` & `countess-0.0.28/countess/plugins/variant.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.27/countess/utils/variant.py` & `countess-0.0.28/countess/utils/variant.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.27/countess.egg-info/PKG-INFO` & `countess-0.0.28/countess.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: countess
-Version: 0.0.27
+Version: 0.0.28
 Summary: CountESS
-Author: CountESS Developers
 Author-email: Nick Moore <nick@zoic.org>, Alan Rubin <alan@rubin.id.au>
-Maintainer: Nick Moore
 Maintainer-email: Nick Moore <nick@zoic.org>
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: hdf
 License-File: LICENSE.txt
 
-# CountESS 0.0.27
+# CountESS 0.0.28
 
 This is CountESS, a modular, Python 3 reimplementation of Enrich2.
 
 ## License
 
 BSD 3-clause.  See [LICENSE.txt](LICENSE.txt)
```

### Comparing `countess-0.0.27/countess.egg-info/SOURCES.txt` & `countess-0.0.28/countess.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 LICENSE.txt
 MANIFEST.in
 README.md
 pyproject.toml
-setup.cfg
 setup.py
 countess/__init__.py
 countess/py.typed
 countess.egg-info/PKG-INFO
 countess.egg-info/SOURCES.txt
 countess.egg-info/dependency_links.txt
 countess.egg-info/entry_points.txt
@@ -19,14 +18,15 @@
 countess/core/parameters.py
 countess/core/pipeline.py
 countess/core/plugins.py
 countess/gui/__init__.py
 countess/gui/config.py
 countess/gui/logger.py
 countess/gui/main.py
+countess/gui/tabular.py
 countess/plugins/__init__.py
 countess/plugins/csv.py
 countess/plugins/data_table.py
 countess/plugins/expression.py
 countess/plugins/fastq.py
 countess/plugins/group_by.py
 countess/plugins/hdf5.py
```

### Comparing `countess-0.0.27/countess.egg-info/entry_points.txt` & `countess-0.0.28/countess.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `countess-0.0.27/pyproject.toml` & `countess-0.0.28/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -21,24 +21,22 @@
 ]
 dependencies = [
     'fqfa~=1.2.3',
     'more_itertools~=9.1.0',
     'numpy~=1.24.2',
     'pandas~=2.0.0',
     'rapidfuzz~=2.15.1',
-    'ttkthemes~=3.2.2',
 ]
 
 [project.optional-dependencies]
 dev = [
     'black<24',
     'build==0.10.0',
     'mypy~=1.0.1',
     'pylint~=2.16',
-    'types-ttkthemes~=3.2',
     'twine==4.0.2',
     'pandas-stubs~=2.0.0',
     'pytest~=7.2',
 ]
 
 hdf = [
      'tables~=3.8.0',
@@ -65,14 +63,23 @@
 
 [project.entry-points.gui_scripts]
 countess_gui = "countess.gui.main:main"
 
 [project.entry-points.console_scripts]
 countess_cmd = "countess.core.cmd:main"
 
+[tool.setuptools]
+packages = [
+    'countess',
+    'countess.core',
+    'countess.gui',
+    'countess.plugins',
+    'countess.utils',
+]
+
 [tool.setuptools.dynamic]
 version = { attr = "countess.VERSION" }
 readme = { file = "README.md", content-type="text/markdown" }
 
 [tool.pylint]
 disable = [
     "consider-using-f-string",
@@ -84,13 +91,14 @@
     "invalid-name",
     "no-else-return",
     "too-many-ancestors",
     "too-many-arguments",
     "too-many-branches",
     "too-many-instance-attributes",
     "too-many-locals",
+    "too-many-statements",
     "too-many-public-methods",
     "unidiomatic-typecheck",
 ]
 
 [tool.black]
 line-length = 100
```

