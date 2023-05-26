# Comparing `tmp/feabas-0.1.1.tar.gz` & `tmp/feabas-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feabas-0.1.1.tar", last modified: Mon Mar 20 19:01:00 2023, max compression
+gzip compressed data, was "feabas-1.0.0.tar", last modified: Fri May 26 20:28:17 2023, max compression
```

## Comparing `feabas-0.1.1.tar` & `feabas-1.0.0.tar`

### file list

```diff
@@ -1,27 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-03-20 19:00:59.993193 feabas-0.1.1/
--rw-rw-rw-   0        0        0     1086 2022-03-04 21:08:46.000000 feabas-0.1.1/LICENSE
--rw-rw-rw-   0        0        0       28 2022-03-04 23:35:51.000000 feabas-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0      703 2023-03-20 19:00:59.991191 feabas-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      257 2023-03-16 01:55:19.000000 feabas-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-20 19:00:59.966544 feabas-0.1.1/feabas/
--rw-rw-rw-   0        0        0       23 2022-12-26 00:25:37.000000 feabas-0.1.1/feabas/__init__.py
--rw-rw-rw-   0        0        0    27692 2023-03-16 01:55:19.000000 feabas-0.1.1/feabas/aligner.py
--rw-rw-rw-   0        0        0    33962 2023-03-16 01:55:19.000000 feabas-0.1.1/feabas/common.py
--rw-rw-rw-   0        0        0     1659 2023-03-16 01:55:19.000000 feabas-0.1.1/feabas/constant.py
--rw-rw-rw-   0        0        0    41696 2023-03-16 01:55:19.000000 feabas-0.1.1/feabas/dal.py
--rw-rw-rw-   0        0        0    38578 2023-03-16 01:55:19.000000 feabas-0.1.1/feabas/matcher.py
--rw-rw-rw-   0        0        0    16672 2023-03-16 01:55:19.000000 feabas-0.1.1/feabas/material.py
--rw-rw-rw-   0        0        0   108527 2023-03-16 01:58:35.000000 feabas-0.1.1/feabas/mesh.py
--rw-rw-rw-   0        0        0    56657 2023-03-16 01:55:19.000000 feabas-0.1.1/feabas/optimizer.py
--rw-rw-rw-   0        0        0    26551 2023-03-16 01:55:19.000000 feabas-0.1.1/feabas/renderer.py
--rw-rw-rw-   0        0        0    46503 2023-03-16 01:55:19.000000 feabas-0.1.1/feabas/spatial.py
--rw-rw-rw-   0        0        0    67355 2023-03-16 01:55:19.000000 feabas-0.1.1/feabas/stitcher.py
--rw-rw-rw-   0        0        0     7662 2023-03-16 01:55:19.000000 feabas-0.1.1/feabas/visualization.py
-drwxrwxrwx   0        0        0        0 2023-03-20 19:00:59.989195 feabas-0.1.1/feabas.egg-info/
--rw-rw-rw-   0        0        0      703 2023-03-20 19:00:59.000000 feabas-0.1.1/feabas.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      426 2023-03-20 19:00:59.000000 feabas-0.1.1/feabas.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-20 19:00:59.000000 feabas-0.1.1/feabas.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-03-20 19:00:59.000000 feabas-0.1.1/feabas.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-03-20 19:00:59.000000 feabas-0.1.1/feabas.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-20 19:00:59.994193 feabas-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      885 2023-03-20 18:58:36.000000 feabas-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 20:28:17.287808 feabas-1.0.0/
+-rw-rw-rw-   0        0        0     1132 2023-05-25 22:40:48.000000 feabas-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0      102 2023-05-25 03:23:35.000000 feabas-1.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    24991 2023-05-26 20:28:17.284803 feabas-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0    24305 2023-05-26 20:12:32.000000 feabas-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 20:28:17.090378 feabas-1.0.0/configs/
+-rw-rw-rw-   0        0        0     4397 2023-05-26 02:02:16.000000 feabas-1.0.0/configs/default_alignment_configs.yaml
+-rw-rw-rw-   0        0        0     1769 2023-05-26 04:06:57.000000 feabas-1.0.0/configs/default_material_table.json
+-rw-rw-rw-   0        0        0     3926 2023-05-23 22:12:10.000000 feabas-1.0.0/configs/default_stitching_configs.yaml
+-rw-rw-rw-   0        0        0     1417 2023-05-25 22:40:48.000000 feabas-1.0.0/configs/default_thumbnail_configs.yaml
+-rw-rw-rw-   0        0        0      422 2023-05-25 22:40:48.000000 feabas-1.0.0/configs/general_configs.yaml
+drwxrwxrwx   0        0        0        0 2023-05-26 20:28:17.233806 feabas-1.0.0/feabas/
+-rw-rw-rw-   0        0        0       23 2022-12-26 00:25:37.000000 feabas-1.0.0/feabas/__init__.py
+-rw-rw-rw-   0        0        0    30628 2023-05-26 19:32:01.000000 feabas-1.0.0/feabas/aligner.py
+-rw-rw-rw-   0        0        0    17351 2023-05-15 02:09:34.000000 feabas-1.0.0/feabas/caching.py
+-rw-rw-rw-   0        0        0    21850 2023-05-25 22:40:48.000000 feabas-1.0.0/feabas/common.py
+-rw-rw-rw-   0        0        0     3938 2023-05-25 22:40:48.000000 feabas-1.0.0/feabas/config.py
+-rw-rw-rw-   0        0        0     1659 2023-03-16 01:55:19.000000 feabas-1.0.0/feabas/constant.py
+-rw-rw-rw-   0        0        0    42661 2023-05-22 19:15:16.000000 feabas-1.0.0/feabas/dal.py
+-rw-rw-rw-   0        0        0     3919 2023-05-19 01:45:40.000000 feabas-1.0.0/feabas/logging.py
+-rw-rw-rw-   0        0        0    39736 2023-05-24 22:57:21.000000 feabas-1.0.0/feabas/matcher.py
+-rw-rw-rw-   0        0        0    16701 2023-05-26 04:06:28.000000 feabas-1.0.0/feabas/material.py
+-rw-rw-rw-   0        0        0   108574 2023-05-26 19:06:46.000000 feabas-1.0.0/feabas/mesh.py
+-rw-rw-rw-   0        0        0    11316 2023-05-26 16:05:44.000000 feabas-1.0.0/feabas/mipmap.py
+-rw-rw-rw-   0        0        0    61117 2023-05-26 18:36:13.000000 feabas-1.0.0/feabas/optimizer.py
+-rw-rw-rw-   0        0        0    26598 2023-05-19 01:53:53.000000 feabas-1.0.0/feabas/renderer.py
+-rw-rw-rw-   0        0        0    51419 2023-05-23 06:03:53.000000 feabas-1.0.0/feabas/spatial.py
+-rw-rw-rw-   0        0        0    68921 2023-05-19 15:37:02.000000 feabas-1.0.0/feabas/stitcher.py
+-rw-rw-rw-   0        0        0    34402 2023-05-26 17:34:14.000000 feabas-1.0.0/feabas/thumbnail.py
+-rw-rw-rw-   0        0        0     7662 2023-03-16 01:55:19.000000 feabas-1.0.0/feabas/visualization.py
+drwxrwxrwx   0        0        0        0 2023-05-26 20:28:17.250805 feabas-1.0.0/feabas.egg-info/
+-rw-rw-rw-   0        0        0    24991 2023-05-26 20:28:16.000000 feabas-1.0.0/feabas.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      851 2023-05-26 20:28:16.000000 feabas-1.0.0/feabas.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 20:28:16.000000 feabas-1.0.0/feabas.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       99 2023-05-26 20:28:16.000000 feabas-1.0.0/feabas.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-26 20:28:16.000000 feabas-1.0.0/feabas.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-26 20:28:17.266805 feabas-1.0.0/scripts/
+-rw-rw-rw-   0        0        0    21378 2023-05-26 19:32:11.000000 feabas-1.0.0/scripts/align_main.py
+-rw-rw-rw-   0        0        0    12888 2023-05-26 16:09:49.000000 feabas-1.0.0/scripts/stitch_main.py
+-rw-rw-rw-   0        0        0    15004 2023-05-26 18:06:49.000000 feabas-1.0.0/scripts/thumbnail_main.py
+-rw-rw-rw-   0        0        0       42 2023-05-26 20:28:17.288805 feabas-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1008 2023-05-26 19:43:57.000000 feabas-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 20:28:17.279805 feabas-1.0.0/tools/
+-rw-rw-rw-   0        0        0     1670 2023-05-26 18:17:21.000000 feabas-1.0.0/tools/convert_manual_thumbnail_matches.py
+-rw-rw-rw-   0        0        0     3797 2023-05-24 22:25:49.000000 feabas-1.0.0/tools/visualize_align_match_coverage.py
```

### Comparing `feabas-0.1.1/LICENSE` & `feabas-1.0.0/LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Yuelong Wu
+Copyright (c) 2022 Yuelong Wu, Center for Brain Science, Harvard University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `feabas-0.1.1/feabas/aligner.py` & `feabas-1.0.0/feabas/aligner.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,20 +9,21 @@
 from scipy import sparse
 import scipy.sparse.csgraph as csgraph
 import yaml
 import time
 
 from feabas.mesh import Mesh
 from feabas import dal
+from feabas import logging
 from feabas.spatial import scale_coordinates
 from feabas.matcher import section_matcher
 from feabas.optimizer import SLM
 import feabas.constant as const
-from feabas.common import str_to_numpy_ascii, Match
-
+from feabas.common import str_to_numpy_ascii, Match, rearrange_section_order
+from feabas.config import DEFAULT_RESOLUTION
 
 
 def read_matches_from_h5(match_name, target_resolution=None):
     with h5py.File(match_name, 'r') as f:
         xy0 = f['xy0'][()]
         xy1 = f['xy1'][()]
         weight = f['weight'][()].ravel()
@@ -51,30 +52,30 @@
         out_dir(str): output directory to save the results.
         conf: the alignment configurations. Could be the path to a YAML config
             file or a dictionary containing the settings.
     """
     outname = os.path.join(out_dir, os.path.basename(match_name))
     if os.path.isfile(outname):
         return None
-    if isinstance(conf, str) and conf.endswith('.yaml'):
+    if isinstance(conf, str) and conf.lower().endswith('.yaml'):
         with open(conf, 'r') as f:
             conf = yaml.safe_load(f)
     if 'matching' in conf:
         conf = conf['matching']
     elif conf is None:
         conf = {}
     elif not isinstance(conf, dict):
         raise TypeError('configuration type not supported.')
     match_name_delimiter = conf.get('match_name_delimiter', '__to__')
-    resolution = conf.get('working_resolution', const.DEFAULT_RESOLUTION)
-    loader_config = conf.get('loader_config', {})
-    matcher_config = conf.get('matcher_config', {})
+    working_mip_level = conf.get('working_mip_level', 0)
+    resolution = DEFAULT_RESOLUTION * (2 ** working_mip_level)
+    loader_config = conf.get('loader_config', {}).copy()
+    matcher_config = conf.get('matcher_config', {}).copy()
     secnames = os.path.splitext(os.path.basename(match_name))[0].split(match_name_delimiter)
     if 'cache_size' in loader_config and loader_config['cache_size'] is not None:
-        loader_config = loader_config.copy()
         loader_config['cache_size'] = loader_config['cache_size'] // (2 * matcher_config.get('num_workers',1))
     if isinstance(meshes, str):
         meshes = (os.path.join(meshes, secnames[0]+'.h5'), os.path.join(meshes, secnames[1]+'.h5'))
     if isinstance(meshes, (tuple, list)):
         mesh0, mesh1 = meshes
         if isinstance(mesh0, str):
             mesh0 = Mesh.from_h5(mesh0)
@@ -153,23 +154,26 @@
             if self._mesh_dir is None:
                 raise RuntimeError('mesh_dir not defined.')
             slist = glob.glob(os.path.join(self._mesh_dir, '*.h5'))
             if bool(slist):
                 section_list = sorted([os.path.basename(s).replace('.h5', '') for s in slist])
             else:
                 raise RuntimeError('no section found.')
+            section_order_file = kwargs.get('section_order_file', os.path.join(self._mesh_dir, 'section_order.txt'))
+            section_list = rearrange_section_order(section_list, section_order_file)
         assert len(section_list) == len(set(section_list))
         self.section_list = tuple(section_list)
         self._mesh_cache_size = kwargs.get('mesh_cache_size', self.num_sections)
         self._link_cache_size = kwargs.get('link_cache_size', None)
         self._match_name_delimiter = kwargs.get('match_name_delimiter', '__to__')
         lock_flags = kwargs.get('lock_flags', None)
         mesh_cache = kwargs.get('mesh_cache', {})
         link_cache = kwargs.get('link_cache', {})
-        self._resolution = kwargs.get('resolution', const.DEFAULT_RESOLUTION)
+        mip_level = kwargs.get('mip_level', 0)
+        self._resolution = DEFAULT_RESOLUTION * (2 ** mip_level)
         self._mesh_cache = OrderedDict()
         self._mesh_cache.update(mesh_cache)
         self._link_cache = OrderedDict()
         self._link_cache.update(link_cache)
         self.lock_flags = defaultdict(lambda: False)
         if isinstance(lock_flags, dict):
             self.lock_flags.update(lock_flags)
@@ -185,14 +189,15 @@
                     match_list = [os.path.basename(m).replace('.h5', '') for m in mlist]
             if match_list is None:
                 if bool(self._link_cache):
                     match_list = list(self._link_cache.keys())
                 else:
                     raise RuntimeError('no match list found.')
         self.match_list = self.filtered_match_list(match_list=match_list)
+        self._logger = None
 
 
     def normalize_mesh_resoltion(self):
         for mshes in self._mesh_cache.values():
             for msh in mshes:
                 msh.change_resolution(self._resolution)
 
@@ -201,16 +206,22 @@
         if secnames is None:
             secnames = list(self._mesh_cache.keys())
         for mshname in secnames:
             if mshname not in self._mesh_cache:
                 continue
             mshes = self._mesh_cache[mshname]
             lock_flag = self.lock_flags[mshname]
+            outcast_flg = [m.is_outcast for m in mshes]
+            if np.all(outcast_flg):
+                self.lock_flags[mshname] = False
             for msh in mshes:
-                msh.locked = lock_flag
+                if not msh.is_outcast:
+                    msh.locked = lock_flag
+                else:
+                    msh.locked = False
 
 
     def init_dict(self, secnames=None, include_cache=False, check_lock=False, **kwargs):
         init_dict = {}
         init_dict['mesh_dir'] = self._mesh_dir
         init_dict['mesh_out_dir'] = self._mesh_out_dir
         init_dict['match_dir'] = self._match_dir
@@ -262,17 +273,26 @@
 
 
     def dump_first_mesh(self):
         """self._mesh_cache is a FIFO cache"""
         cached_name, cached_Ms = self._mesh_cache.popitem(last=False)
         rel_match_names = self.secname_to_matchname_mapper[cached_name]
         if self._mesh_out_dir is not None:
-            cached_M = Mesh.combine_mesh(cached_Ms, save_material=True)
-            outname = os.path.join(self._mesh_out_dir, cached_name+'.h5')
-            cached_M.save_to_h5(outname, vertex_flags=const.MESH_GEARS, save_material=True)
+            anchored_meshes = [m for m in cached_Ms if not m.is_outcast]
+            if len(anchored_meshes) != len(cached_Ms):
+                logger = logging.get_logger(self._logger)
+                if len(anchored_meshes) == 0:
+                    self.lock_flags[cached_name] = False
+                    logger.warning(f'{cached_name}: not anchored.')
+                else:
+                    logger.warning(f'{cached_name}: partially not anchored.')
+            if len(anchored_meshes) > 0:
+                cached_M = Mesh.combine_mesh(anchored_meshes, save_material=True)
+                outname = os.path.join(self._mesh_out_dir, cached_name+'.h5')
+                cached_M.save_to_h5(outname, vertex_flags=const.MESH_GEARS, save_material=True)
         for matchname in rel_match_names:
             self.dump_link(matchname)
 
 
     def get_link(self, matchname):
         if matchname in self._link_cache:
             self._link_cache.move_to_end(matchname, last=True)
@@ -363,18 +383,22 @@
 
     def optimize_slide_window(self, **kwargs):
         num_workers = kwargs.pop('num_workers', 1)
         locked_section = kwargs.pop('locked_section', None)
         start_loc = kwargs.pop('start_loc', 'L') # L or R or M
         window_size = kwargs.get('window_size', None)
         func_name = 'optimize_slide_window'
+        if kwargs.get('logger', None) is not None:
+            self._logger = kwargs['logger']
         if (window_size is None) or window_size > self.num_sections:
             window_size = self.num_sections
             start_loc = 'L'
-        buffer_size = kwargs.get('buffer_size', window_size//4)
+            buffer_size = 0
+        else:
+            buffer_size = kwargs.get('buffer_size', window_size//4)
         if locked_section is not None:
             self.unlock_all()
             if not isinstance(locked_section, str):
                 locked_section = self.section_list[int(locked_section)]   # indexing by id
             self.update_lock_flags({locked_section: True})
             locked_idx = self.secname_to_id(locked_section)
             init_idx0 = locked_idx - window_size//2
@@ -397,40 +421,50 @@
             indices0 = np.arange(init_idx0, self.num_sections, window_size-buffer_size)
             for idx0 in indices0:
                 seclst = self.section_list[init_idx0:(idx0+window_size)]
                 if np.all([self.lock_flags[s] for s in seclst]):
                     continue
                 cst = self.optimize_section_list(seclst, **kwargs)
                 if cst is not None:
-                    costs['_'.join((self.section_list[idx0], seclst[-1]))] = cst
-                self.update_lock_flags({s:True for s in seclst[:-buffer_size]})
+                    costs.update(cst)
+                if buffer_size > 0:
+                    self.update_lock_flags({s:True for s in seclst[:-buffer_size]})
+                else:
+                    self.update_lock_flags({s:True for s in seclst})
             else:
                 self.flush_meshes()
         elif start_loc == 'R':
             indices1 = np.arange(self.num_sections, 0, buffer_size-window_size)
             for idx1 in indices1:
                 idx0 = max(0, idx1 - window_size)
                 seclst = self.section_list[idx0:]
                 if np.all([self.lock_flags[s] for s in seclst]):
                     continue
                 cst = self.optimize_section_list(seclst, **kwargs)
                 if cst is not None:
-                    costs['_'.join((self.section_list[idx0], seclst[-1]))] = cst
-                self.update_lock_flags({s:True for s in seclst[buffer_size:]})
+                    costs.update(cst)
+                if buffer_size > 0:
+                    self.update_lock_flags({s:True for s in seclst[buffer_size:]})
+                else:
+                    self.update_lock_flags({s:True for s in seclst})
             else:
                 self.flush_meshes()
         else:
             assert window_size > 2 * buffer_size + 1
             seclst = self.section_list[init_idx0:(init_idx0+window_size)]
             cst = self.optimize_section_list(seclst, **kwargs)
             if cst is not None:
-                costs['_'.join((seclst[0], seclst[-1]))] = cst
-            self.flush_meshes()
-            sections_to_lock = seclst[buffer_size:-buffer_size]
+                costs.update(cst)
+            if buffer_size > 0:
+                sections_to_lock = seclst[buffer_size:-buffer_size]
+            else:
+                sections_to_lock = seclst
             self.update_lock_flags({s:True for s in sections_to_lock})
+            self.flush_meshes()
+            kwargs.setdefault('need_anchor', True)
             lock_id0, lock_id1 = self.secname_to_id(sections_to_lock[0]), self.secname_to_id(sections_to_lock[-1])
             matchlist_l = self.filtered_match_list(secnames=self.section_list[lock_id0:], check_lock=True)
             seclist_l = self.filter_section_list_from_matches(match_list=matchlist_l)
             kwargs_l = kwargs.copy()
             init_dict_l = self.init_dict(secnames=seclist_l, check_lock=True)
             kwargs_l['start_loc'] = 'L'
             matchlist_r = self.filtered_match_list(secnames=self.section_list[:lock_id1], check_lock=True)
@@ -452,39 +486,62 @@
                 costs.update(cst)
         return costs
 
 
     def optimize_section_list(self, section_list, **kwargs):
         target_gear = kwargs.get('target_gear', const.MESH_GEAR_MOVING)
         optimize_rigid = kwargs.get('optimize_rigid', True)
-        rigid_params = kwargs.get('rigid_params', {})
+        rigid_params = kwargs.get('rigid_params', {}).copy()
         optimize_elastic = kwargs.get('optimize_elastic', True)
-        elastic_params = kwargs.get('elastic_params', {})
+        elastic_params = kwargs.get('elastic_params', {}).copy()
         residue_len = kwargs.get('residue_len', 0)
         residue_mode = kwargs.get('residue_mode', None)
+        logger_info = kwargs.get('logger', None)
+        need_anchor = kwargs.get('need_anchor', False)
+        logger = logging.get_logger(logger_info)
+        residue = {}
+        if len(section_list) == 0:
+            logger.info('no section to optimize.')
+            return residue
         optm = self.initialize_SLM(section_list)
+        if len(optm.meshes) == 0:
+            logger.info(f'{section_list[0]} -> {section_list[-1]}: all sections settled.')
+            return residue
+        outcasts = optm.flag_outcasts()
+        if np.all(outcasts):
+            logger.error(f'{optm.meshes[0].name} -> {optm.meshes[-1].name}: disconnected due to lack of matches. abort.')
+            return residue
+        if need_anchor and (not np.any(optm.lock_flags)):
+            logger.error(f'{optm.meshes[0].name} -> {optm.meshes[-1].name}: disconnected due to lack of matches. abort.')
+            return residue
         cost = None
         t0 = time.time()
         if optimize_rigid:
             optm.optimize_affine_cascade(target_gear=target_gear, **rigid_params)
             if target_gear != const.MESH_GEAR_FIXED:
                 optm.anneal(gear=(target_gear, const.MESH_GEAR_FIXED), mode=const.ANNEAL_CONNECTED_RIGID)
         if optimize_elastic:
+            if 'callback_settings' in elastic_params:
+                elastic_params['callback_settings'].setdefault('early_stop_thresh', DEFAULT_RESOLUTION / self._resolution)
             cost = optm.optimize_elastic(target_gear=target_gear, **elastic_params)
             if (residue_mode is not None) and (residue_len > 0):
                 if residue_mode == 'huber':
                     optm.set_link_residue_huber(residue_len)
                 else:
                     optm.set_link_residue_threshold(residue_len)
                 weight_modified, _ = optm.adjust_link_weight_by_residue(gear=(target_gear, target_gear))
                 if weight_modified:
                     cost1 = optm.optimize_elastic(target_gear=target_gear, **elastic_params)
                     cost = (cost[0], cost1[-1])
-        print(f'{optm.meshes[0].name} -> {optm.meshes[-1].name}: cost {cost} | {time.time()-t0} sec')
-        return cost
+        for matchname, lnks in self._link_cache.items():
+            dxy = np.concatenate([lnk.dxy(gear=1) for lnk in lnks], axis=0)
+            dis = np.sum(dxy ** 2, axis=1)**0.5
+            residue[matchname] = (dis.max(), dis.mean())
+        logger.info(f'{optm.meshes[0].name} -> {optm.meshes[-1].name}: cost {cost} | {time.time()-t0} sec')
+        return residue
 
 
     def update_lock_flags(self, flags):
         self.lock_flags.update(flags)
         self.normalize_mesh_lock_status(secnames=list(flags.keys()))
 
 
@@ -555,15 +612,14 @@
         A = self.section_connection_matrix
         ref_flag = A.dot(sel_flag) & (~sel_flag) & self.locked_array
         combined_flag = sel_flag | ref_flag
         return [s for flg, s in zip(combined_flag, self.section_list) if flg]
         
 
 
-
     @property
     def secname_to_matchname_mapper(self):
         if not hasattr(self, '_secname_to_matchname_mapper'):
             self._secname_to_matchname_mapper = defaultdict(set)
             for matchname in self.match_list:
                 names = self.matchname_to_secnames(matchname)
                 self._secname_to_matchname_mapper[names[0]].add(matchname)
```

### Comparing `feabas-0.1.1/feabas/constant.py` & `feabas-1.0.0/feabas/constant.py`

 * *Files identical despite different names*

### Comparing `feabas-0.1.1/feabas/dal.py` & `feabas-1.0.0/feabas/dal.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 import os
 import re
 
 import cv2
 import numpy as np
 from rtree import index
 
-from feabas import common
-import feabas.constant as const
+from feabas import common, caching
+from feabas.config import DEFAULT_RESOLUTION
 
 
 # bbox :int: [xmin, ymin, xmax, ymax]
 
 ##------------------------------ tile dividers -------------------------------##
 # tile divider functions to divide an image tile to smaller block for caching
 # Args:
@@ -79,18 +79,18 @@
     return divider
 
 
 ##------------------------------ image loaders -------------------------------##
 
 def get_loader_from_json(json_info, loader_type=None, **kwargs):
     if isinstance(json_info, str):
-        if json_info.endswith('.json'):
+        if json_info.lower().endswith('.json'):
             with open(json_info, 'r') as f:
                 json_obj = json.load(f)
-        elif json_info.endswith('.txt'): # could use tab separated txt, not recommend
+        elif json_info.lower().endswith('.txt'): # could use tab separated txt, not recommend
             if loader_type == 'StaticImageLoader':
                 loader = StaticImageLoader.from_coordinate_file(json_info)
             else:
                 loader = MosaicLoader.from_coordinate_file(json_info)
             json_obj = loader.init_dict()
         else:
             json_obj = json.loads(json_info)
@@ -120,34 +120,36 @@
         dtype: datatype of the output images. Default to None same as input.
         number_of_channels: # of channels of the output images. Default to
             None same as input.
         apply_CLAHE(bool): whether to apply CLAHE on output images.
         inverse(bool): whether to invert images.
         fillval(scalar): fill value for missing data.
         cache_size(int): length of image cache.
+        cache_capacity(float): capacity of image cache in MiB.
         cache_border_margin(int)/cache_block_size(int): the border width
             for _tile_divider_border caching, or the square block size for
             _tile_divider_block caching. If neither is set, cache
             the entile image with _tile_divider_blank.
         resolution(float): resolution of the images. default to 4nm
     """
     def __init__(self, **kwargs):
         self._dtype = kwargs.get('dtype', None)
         self._number_of_channels = kwargs.get('number_of_channels', None)
         self._apply_CLAHE = kwargs.get('apply_CLAHE', False)
         self._CLAHE = cv2.createCLAHE(clipLimit=2.0, tileGridSize=(8,8))
         self._inverse = kwargs.get('inverse', False)
         self._default_fillval = kwargs.get('fillval', 0)
         self._cache_size = kwargs.get('cache_size', 0)
+        self._cache_capacity = kwargs.get('cache_capacity', None)
         self._use_cache = (self._cache_size is None) or (self._cache_size > 0)
         self._init_tile_divider(**kwargs)
         self._cache_type = kwargs.get('cache_type', 'mfu')
-        self._cache = common.generate_cache(self._cache_type, maxlen=self._cache_size)
+        self._cache = caching.generate_cache(self._cache_type, maxlen=self._cache_size, maxbytes=self._cache_capacity)
         self._preprocess = kwargs.get('preprocess', None)
-        self.resolution = kwargs.get('resolution', const.DEFAULT_RESOLUTION)
+        self.resolution = kwargs.get('resolution', DEFAULT_RESOLUTION)
         self._read_counter = 0
 
 
     def clear_cache(self, instant_gc=False):
         # instant_gc: when True, instantly call garbage collection
         self._cache.clear(instant_gc)
 
@@ -319,15 +321,15 @@
             self._tile_divider = _tile_divider_blank
             self._tile_divider_type = 'blank'
 
 
     @staticmethod
     def _load_settings_from_json(jsonname):
         if isinstance(jsonname, str):
-            if jsonname.endswith('.json'):
+            if jsonname.lower().endswith('.json'):
                 with open(jsonname, 'r') as f:
                     json_obj = json.load(f)
             else:
                 json_obj = json.loads(jsonname)
         elif isinstance(jsonname, dict):
             json_obj = jsonname
         else:
@@ -359,32 +361,37 @@
     def _read_image(self, imgpath, **kwargs):
         number_of_channels = kwargs.get('number_of_channels', self._number_of_channels)
         dtype = kwargs.get('dtype', self._dtype)
         apply_CLAHE = kwargs.get('apply_CLAHE', self._apply_CLAHE)
         inverse = kwargs.get('inverse', self._inverse)
         if number_of_channels == 3:
             img = common.imread(imgpath, flag=cv2.IMREAD_COLOR)
+        elif number_of_channels == 1:
+            img = common.imread(imgpath, flag=cv2.IMREAD_GRAYSCALE)
         else:
             img = common.imread(imgpath, flag=cv2.IMREAD_UNCHANGED)
         self._read_counter += 1
         if img is None:
             raise RuntimeError(f'Image file {imgpath} not valid!')
-        if (number_of_channels == 1) and (len(img.shape) > 2) and (img.shape[-1] > 1):
-            img = img.mean(axis=-1)
-        if dtype is not None:
-            img = img.astype(dtype, copy=False)
-        else:
+        if dtype is None:
             dtype = img.dtype
+        if (number_of_channels == 1) and (len(img.shape) > 2) and (img.shape[-1] > 1):
+            img = img.mean(axis=-1).astype(dtype)
         if apply_CLAHE:
-            img = self._CLAHE.apply(img)
+            if len(img.shape) > 2:
+                img = cv2.cvtColor(img, cv2.COLOR_RGB2Lab)
+                img[:,:,0] = self._CLAHE.apply(img[:,:,0])
+                img = cv2.cvtColor(img, cv2.COLOR_Lab2RGB)
+            else:
+                img = self._CLAHE.apply(img)
         if self._preprocess is not None:
             img = self._preprocess(img)
         if inverse:
             img = common.inverse_image(img, dtype)
-        return img
+        return img.astype(dtype, copy=False)
 
 
     def _export_dict(self, **kwargs):
         """turn the loader settings to a dict used in self.save_to_json"""
         return self._settings_dict(**kwargs)
 
 
@@ -476,14 +483,16 @@
         divider = self._tile_divider(imght, imgwd, x0=x0, y0=y0)
         new_cache = False
         for bid, blkbbox in divider.items():
             if (bid > 0) and (bid not in cache_dict):
                 if img is None:
                     img = self._read_image(imgpath, **kwargs)
                 blk = img[blkbbox[1]:blkbbox[3], blkbbox[0]:blkbbox[2],...]
+                if blk.size != img.size:
+                    blk = blk.copy()
                 cache_dict[bid] = blk
                 new_cache = True
         if new_cache:
             self._cache[imgpath] = ((0, 0, imgwd,imght), cache_dict)
 
 
     def _get_cached_dict(self, imgpath):
@@ -619,19 +628,22 @@
                 image_not_in_list = '{} not in the image loader list'.format(filepath)
                 raise KeyError(image_not_in_list)
         if fileid in self._cache:
             cache_dict = self._cache[fileid]
         else:
             cache_dict = {}
         new_cache = False
-        for bid, blkbbox in self.divider(fileid).items():
+        divider = self.divider(fileid)
+        for bid, blkbbox in divider.items():
             if (bid > 0) and (bid not in cache_dict):
                 if img is None:
                     img = self._read_image(fileid, **kwargs)
                 blk = img[blkbbox[1]:blkbbox[3], blkbbox[0]:blkbbox[2],...]
+                if blk.size != img.size:
+                    blk = blk.copy()
                 cache_dict[bid] = blk
                 new_cache = True
         if new_cache:
             self._cache[fileid] = cache_dict
 
 
     def _export_dict(self, output_controls=True, cache_settings=True, image_list=True):
@@ -927,15 +939,15 @@
         else:
             self._src_number_of_channels = img.shape[-1]
         self._number_of_channels = kwargs.get('number_of_channels', max(1, self._src_number_of_channels))
         self._clahe_img = None
         self._preprocess = kwargs.get('preprocess', None)
         self._inverse = kwargs.get('inverse', False)
         self._default_fillval = kwargs.get('fillval', 0)
-        self.resolution = kwargs.get('resolution', const.DEFAULT_RESOLUTION)
+        self.resolution = kwargs.get('resolution', DEFAULT_RESOLUTION)
         self.x0 = kwargs.get('x0', 0)
         self.y0 = kwargs.get('y0', 0)
 
 
     @classmethod
     def from_filepath(cls, imgpath, **kwargs):
         img = common.imread(imgpath, flag=cv2.IMREAD_UNCHANGED)
@@ -956,15 +968,20 @@
             return_empty=return_empty, return_index=False, fillval=fillval)
 
 
     @property
     def clahe_img(self):
         if self._clahe_img is None:
             clahe_filter = cv2.createCLAHE(clipLimit=2.0, tileGridSize=(8,8))
-            self._clahe_img = clahe_filter.apply(self.img)
+            if len(self.img.shape) > 2:
+                img = cv2.cvtColor(self.img, cv2.COLOR_RGB2Lab)
+                img[:,:,0] = clahe_filter.apply(img[:,:,0])
+                self._clahe_img = cv2.cvtColor(img, cv2.COLOR_Lab2RGB)
+            else:
+                self._clahe_img = clahe_filter.apply(self.img)
         return self._clahe_img
 
 
     def _read_image(self, **kwargs):
         number_of_channels = kwargs.get('number_of_channels', self._number_of_channels)
         if number_of_channels is None:
             number_of_channels = self._src_number_of_channels
@@ -975,18 +992,18 @@
             img = self.clahe_img
         else:
             img = self._img
         if (self._src_number_of_channels <= 1) and (number_of_channels > 1):
             img = np.tile(img.reshape(img.shape[0], img.shape[1], 1), (1,1,number_of_channels))
         elif (self._src_number_of_channels > 1) and (number_of_channels == 1):
             img = img.mean(axis=-1)
-        if (dtype is not None) and (np.dtype(dtype) != img.dtype):
-            img = img.astype(dtype)
         if self._preprocess is not None:
             img = self._preprocess(img)
+        if (dtype is not None) and (np.dtype(dtype) != img.dtype):
+            img = img.astype(dtype)
         if inverse:
             img = common.inverse_image(img, dtype)
         return img
 
 
     def clear_cache(self, instant_gc=False):
         self._clahe_img = None
```

### Comparing `feabas-0.1.1/feabas/matcher.py` & `feabas-1.0.0/feabas/matcher.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 
 
 def xcorr_fft(img0, img1, conf_mode=const.FFT_CONF_MIRROR, **kwargs):
     """
     find the displacements between two image(-stack)s from the Fourier based
     cross-correlation.
     Args:
-        img0(ndarray): the first image, N x H0 x W0.
-        img1(ndarray): the second image, N x H1 x W1.
+        img0(ndarray): the first image, N x H0 x W0 (x C).
+        img1(ndarray): the second image, N x H1 x W1 (x C).
     Kwargs:
         sigma: if set to larger than 0, will apply masked Difference of Gassian
             filter to the images before cross-correlation
         mask0: mask for DoG filter for the first image.
         mask1: mask for DoG filter for the second image.
         normalize (bool): whether to normalize the cross-correlation. The inputs
             of the function are expected to be band-pass filtered, therefore
@@ -39,32 +39,40 @@
         conf: the confidence value of the cross-correlation between 0 and 1.
     """
     sigma = kwargs.get('sigma', 0)
     mask0 = kwargs.get('mask0', None)
     mask1 = kwargs.get('mask1', None)
     normalize = kwargs.get('normalize', False)
     pad = kwargs.get('pad', True)
+    if len(img0.shape) > 3:
+        img0 = np.moveaxis(img0, -1, 1)
+    if len(img1.shape) > 3:
+        img1 = np.moveaxis(img1, -1, 1)
     if sigma > 0:
         img0 = common.masked_dog_filter(img0, sigma, mask=mask0)
         img1 = common.masked_dog_filter(img1, sigma, mask=mask1)
     imgshp0 = img0.shape[-2:]
     imgshp1 = img1.shape[-2:]
     if pad:
         fftshp = [next_fast_len(s0 + s1 - 1) for s0, s1 in zip(imgshp0, imgshp1)]
     else:
         fftshp = [next_fast_len(max(s0, s1)) for s0, s1 in zip(imgshp0, imgshp1)]
-    F0 = fft.rfft2(img0, s=fftshp)
-    F1 = fft.rfft2(img1, s=fftshp)
-    C = fft.irfft2(np.conj(F0) * F1, s=fftshp)
-    C = C.reshape(-1, np.prod(fftshp))
+    F0 = fft.rfft2(img0, s=fftshp, axes=(-2,-1))
+    F1 = fft.rfft2(img1, s=fftshp, axes=(-2,-1))
+    FF = np.conj(F0) * F1
+    if len(FF.shape) > 3:
+        FF = FF.mean(axis=1)
+    C = fft.irfft2(FF, s=fftshp, axes=(-2,-1))
+    Nimg = C.shape[0]
+    C = C.reshape(Nimg, -1)
     if normalize:
         if mask0 is None:
-            mask0 = np.ones_like(img0)
+            mask0 = np.ones_like(img0, shape=img0.shape[-2:])
         if mask1 is None:
-            mask1 = np.ones_like(img1)
+            mask1 = np.ones_like(img1, shape=img1.shape[-2:])
         M0 = fft.rfft2(mask0, s=fftshp)
         M1 = fft.rfft2(mask1, s=fftshp)
         NC = fft.irfft2(np.conj(M0) * M1, s=fftshp)
         NC = NC.reshape(-1, np.prod(fftshp))
         NC = (NC / (NC.max(axis=-1, keepdims=True).clip(1, None))).clip(0.1, None)
         C = C / NC
     indx = np.argmax(C, axis=-1)
@@ -72,16 +80,19 @@
     dy = dy + (imgshp0[0] - imgshp1[0]) / 2
     dx = dx + (imgshp0[1] - imgshp1[1]) / 2
     dy = dy - np.round(dy / fftshp[0]) * fftshp[0]
     dx = dx - np.round(dx / fftshp[1]) * fftshp[1]
     if conf_mode == const.FFT_CONF_NONE:
         conf = np.ones_like(dx, dtype=np.float32)
     elif conf_mode == const.FFT_CONF_MIRROR:
-        C_mirror = np.abs(fft.irfft2(F0 * F1, s=fftshp))
-        C_mirror = C_mirror.reshape(-1, np.prod(fftshp))
+        FF = F0 * F1
+        if len(FF.shape) > 3:
+            FF = FF.mean(axis=1)
+        C_mirror = np.abs(fft.irfft2(FF, s=fftshp, axes=(-2,-1)))
+        C_mirror = C_mirror.reshape(Nimg, -1)
         if normalize:
             NC = fft.irfft2(M0 * M1, s=fftshp)
             NC = NC.reshape(-1, np.prod(fftshp))
             NC = (NC / (NC.max(axis=-1, keepdims=True).clip(1, None))).clip(0.1, None)
             C_mirror = C_mirror / NC
         mx_rl = C.max(axis=-1)
         mx_mr = C_mirror.max(axis=-1)
@@ -103,15 +114,17 @@
     mask1 = kwargs.get('mask1', None)
     conf_mode = kwargs.get('conf_mode', const.FFT_CONF_MIRROR)
     conf_thresh = kwargs.get('conf_thresh', 0.3)
     divide_factor = kwargs.get('divide_factor', 6)
     if sigma > 0:
         img0 = common.masked_dog_filter(img0, sigma, mask=mask0)
         img1 = common.masked_dog_filter(img1, sigma, mask=mask1)
-    tx, ty, conf = xcorr_fft(img0, img1, conf_mode=conf_mode, pad=True)
+    img0_t = np.expand_dims(img0, 0)
+    img1_t = np.expand_dims(img1, 0)
+    tx, ty, conf = xcorr_fft(img0_t, img1_t, conf_mode=conf_mode, pad=True)
     tx, ty, conf = tx.item(), ty.item(), conf.item()
     if conf > conf_thresh:
         return tx, ty, conf
     # divide the image for another shot (avoid local artifacts)
     imgshp0 = img0.shape[-2:]
     imgshp1 = img1.shape[-2:]
     imgshp = np.minimum(imgshp0, imgshp1)
@@ -151,26 +164,27 @@
 
 
 def stitching_matcher(img0, img1, **kwargs):
     """
     given two images with rectangular shape, return the displacement vectors on a
     grid of sample points. Mostly for stitching matching.
     """
-    sigma = kwargs.get('sigma', 2.5)
-    mask0 = kwargs.get('mask0', None)
-    mask1 = kwargs.get('mask1', None)
+    sigma = kwargs.pop('sigma', 2.5)
+    mask0 = kwargs.pop('mask0', None)
+    mask1 = kwargs.pop('mask1', None)
+    coarse_downsample = kwargs.pop('coarse_downsample', 1)
+    fine_downsample = kwargs.pop('fine_downsample', 1)
+    spacings = kwargs.pop('spacings', None)
+    residue_len = kwargs.pop('residue_len', 5)
     conf_mode = kwargs.get('conf_mode', const.FFT_CONF_MIRROR)
     conf_thresh = kwargs.get('conf_thresh', 0.3)
-    residue_mode = kwargs.get('residue_mode', 'huber')
-    residue_len = kwargs.get('residue_len', 5)
-    opt_tol = kwargs.get('opt_tol', None)
-    coarse_downsample = kwargs.get('coarse_downsample', 1)
-    fine_downsample = kwargs.get('fine_downsample', 1)
-    spacings = kwargs.get('spacings', None)
     min_num_blocks = kwargs.get('min_num_blocks', 2)
+    kwargs.setdefault('residue_mode', 'huber')
+    kwargs.setdefault('opt_tol', None)
+    
     if spacings is None:
         imgshp = np.minimum(img0.shape, img1.shape)
         smx = max(imgshp) * 0.25
         smn = max(min(75, min(imgshp)/3), 25)
         if smn > smx:
             spacings = np.array([smn])
         else:
@@ -242,17 +256,15 @@
     mesh0 = Mesh.from_bbox(img_loader0.bounds, cartesian=True,
         mesh_size=min_spacing, min_num_blocks=min_num_blocks, uid=0)
     mesh1 = Mesh.from_bbox(img_loader1.bounds, cartesian=True,
         mesh_size=min_spacing, min_num_blocks=min_num_blocks, uid=1)
     mesh0.apply_translation((tx0, ty0), const.MESH_GEAR_FIXED)
     mesh0.lock()
     xy0, xy1, weight, strain = iterative_xcorr_matcher_w_mesh(mesh0, mesh1, img_loader0, img_loader1,
-        conf_mode=conf_mode, conf_thresh=conf_thresh, residue_mode=residue_mode,
-        residue_len=residue_len, opt_tol=opt_tol, spacings=spacings,
-        distributor='cartesian_bbox', min_num_blocks=min_num_blocks)
+        spacings=spacings, distributor='cartesian_bbox', residue_len=residue_len, **kwargs)
     if (fine_downsample != 1) and (xy0 is not None):
         xy0 = spatial.scale_coordinates(xy0, 1/fine_downsample)
         xy1 = spatial.scale_coordinates(xy1, 1/fine_downsample)
     return xy0, xy1, weight, strain
 
 
 def section_matcher(mesh0, mesh1, image_loader0, image_loader1, **kwargs):
@@ -364,15 +376,16 @@
     min_boundary_distance = kwargs.get('min_boundary_distance', 0)
     boundary_tolerance = kwargs.get('boundary_tolerance', None)
     shrink_factor = kwargs.get('shrink_factor', 1)
     allow_dwell = kwargs.get('allow_dwell', 0)
     compute_strain = kwargs.get('compute_strain', True)
     batch_size = kwargs.pop('batch_size', None)
     initial_matches = kwargs.get('initial_matches', None)
-    to_pad = kwargs.get('pad', None)
+    to_pad = kwargs.pop('pad', None)
+    max_spacing_skip = kwargs.get('max_spacing_skip', 1)
     continue_on_flip = kwargs.get('continue_on_flip', True)
     if num_workers > 1 and batch_size is not None:
         batch_size = max(1, batch_size / num_workers)
         if isinstance(image_loader0, dal.AbstractImageLoader):
             loader_dict0 = image_loader0.init_dict()
             loader_dict1 = image_loader1.init_dict()
         else:
@@ -408,14 +421,18 @@
             opt.optimize_Newton_Raphson(maxepoch=5, tol=1e-4, batch_num_matches=np.inf, continue_on_flip=continue_on_flip)
     spacings = np.sort(spacings)[::-1]
     sp = np.max(spacings)
     sp_indx = 0
     initialized = False
     spacing_enlarged = False
     dwelled = 0
+    if to_pad is None:
+        pad = True
+    else:
+        pad = to_pad
     while sp_indx < spacings.size:
         if sp == spacings[-1]:
             mnb = min_num_blocks
         else:
             mnb = 1
         if distributor == 'cartesian_bbox':
             bboxes0, bboxes1 = distributor_cartesian_bbox(mesh0, mesh1, sp,
@@ -443,18 +460,14 @@
             batch_size_s = None
         if num_workers > 1:
             if batch_size_s is None:
                 batch_size_s = max(1, num_blocks/num_workers)
             else:
                 batch_size_s = min(max(1, num_blocks/num_workers), batch_size_s)
             num_batchs = int(np.ceil(num_blocks / batch_size_s))
-            if to_pad is None:
-                pad = not initialized
-            else:
-                pad = to_pad
             if num_batchs == 1:
                 xy0, xy1, conf = bboxes_mesh_renderer_matcher(mesh0, mesh1,
                     image_loader0, image_loader1, bboxes0, bboxes1,
                     batch_size=batch_size, pad=pad, **kwargs)
             else:
                 batch_indices = np.linspace(0, num_blocks, num=num_batchs+1, endpoint=True)
                 batch_indices = np.unique(batch_indices.astype(np.int32))
@@ -489,15 +502,15 @@
                     return invalid_output
                 xy0 = np.concatenate(xy0, axis=0)
                 xy1 = np.concatenate(xy1, axis=0)
                 conf = np.concatenate(conf, axis=0)
         else:
             xy0, xy1, conf = bboxes_mesh_renderer_matcher(mesh0, mesh1,
                 image_loader0, image_loader1, bboxes0, bboxes1,
-                batch_size=batch_size, pad=(not initialized), **kwargs)
+                batch_size=batch_size, pad=pad, **kwargs)
         if np.all(conf <= conf_thresh):
             if not initialized:
                 return invalid_output
             else:
                 break
         opt.clear_links()
         xy0 = xy0[conf > conf_thresh]
@@ -509,23 +522,35 @@
         else:
             opt_tol_t = opt_tol
         min_block_size = min_block_size_multiplier * max_dis
         next_pos = np.searchsorted(-spacings, -min_block_size) - 1
         if (not spacing_enlarged) and (next_pos < 0):
             spacing_enlarged = True
             sp = np.ceil(min_block_size)
+            if to_pad is None:
+                pad = True
             continue
         spacing_enlarged = True
         if next_pos > sp_indx:
+            next_pos = min(next_pos, sp_indx + 1 + max_spacing_skip)
+            if to_pad is None:
+                if next_pos > sp_indx + 1:
+                    pad = True
+                else:
+                    pad = False
             sp_indx = next_pos
             dwelled = 0
         elif dwelled >= allow_dwell:
+            if to_pad is None:
+                pad = True
             sp_indx += 1
             dwelled = 0
         else:
+            if to_pad is None:
+                pad = True
             dwelled += 1
         opt.add_link_from_coordinates(mesh0.uid, mesh1.uid, xy0, xy1,
                         gear=(const.MESH_GEAR_MOVING, const.MESH_GEAR_MOVING), weight=wt,
                         check_duplicates=False)
         if max_dis > 0.1:
             if linear_system:
                 opt.optimize_linear(tol=opt_tol_t, batch_num_matches=np.inf, continue_on_flip=continue_on_flip)
@@ -597,32 +622,37 @@
     xy1 = []
     conf = []
     for block_indices0, block_indices1 in zip(batched_block_indices0, batched_block_indices1):
         stack0 = []
         stack1 = []
         xy_ctr0 = []
         xy_ctr1 = []
+        wt_ratio = []
         for bbox0, bbox1 in zip(block_indices0, block_indices1):
             img0 = render0.crop(bbox0, mode=render_mode, log_sigma=sigma, remap_interp=cv2.INTER_LINEAR)
             if img0 is None:
                 continue
             img1 = render1.crop(bbox1, mode=render_mode, log_sigma=sigma, remap_interp=cv2.INTER_LINEAR)
             if img1 is None:
                 continue
             stack0.append(img0)
             stack1.append(img1)
             xy_ctr0.append(((bbox0[0]+bbox0[2]-1)/2, (bbox0[1]+bbox0[3]-1)/2))
             xy_ctr1.append(((bbox1[0]+bbox1[2]-1)/2, (bbox1[1]+bbox1[3]-1)/2))
+            wd0, ht0 = bbox0[2] - bbox0[0], bbox0[3] - bbox0[1]
+            wd1, ht1 = bbox1[2] - bbox1[0], bbox1[3] - bbox1[1]
+            wt_ratio.append((wd0 / (wd0 + wd1), ht0 / (ht0 + ht1)))
         dx, dy, conf_b = xcorr_fft(np.stack(stack0, axis=0), np.stack(stack1, axis=0),
             conf_mode=conf_mode, pad=pad)
         xy_ctr0 = np.array(xy_ctr0)
         xy_ctr1 = np.array(xy_ctr1)
+        wt_ratio = np.array(wt_ratio)
         dxy = np.stack((dx, dy), axis=-1)
-        xy0_b = xy_ctr0 - dxy/2
-        xy1_b = xy_ctr1 + dxy/2
+        xy0_b = xy_ctr0 - dxy * wt_ratio
+        xy1_b = xy_ctr1 + dxy * (1-wt_ratio)
         xy0.append(xy0_b)
         xy1.append(xy1_b)
         conf.append(conf_b)
     if len(xy0) > 0:
         xy0 = np.concatenate(xy0, axis=0)
         xy1 = np.concatenate(xy1, axis=0)
         conf = np.concatenate(conf, axis=0)
@@ -700,15 +730,15 @@
         rxx, ryy = np.meshgrid(np.arange(rx_mn, rx_mx, spacing), np.arange(ry_mn, ry_mx, spacing))
         rv = np.stack((rxx.ravel(), ryy.ravel()), axis=-1)
         cntrs.append(shpgeo.MultiPoint(rv).intersection(reg))
     cntrs = unary_union(cntrs)
     if hasattr(cntrs, 'geoms'):
         bcnters = np.array([(p.x, p.y) for p in cntrs.geoms])
     else:
-        bcnters = np.array((cntrs.x, cntrs.y))
+        bcnters = np.array([(cntrs.x, cntrs.y)])
     bboxes0 = np.concatenate((bcnters-blk_hfsz0, bcnters+blk_hfsz0), axis=-1)
     bboxes1 = np.concatenate((bcnters-blk_hfsz1, bcnters+blk_hfsz1), axis=-1)
     if zorder:
         x_rnd = np.round((bcnters[:,0] - bcnters[:,0].min()) / spacing)
         y_rnd = np.round((bcnters[:,1] - bcnters[:,1].min()) / spacing)
         idx = common.z_order(np.stack((x_rnd, y_rnd), axis=-1))
         bboxes0 = bboxes0[idx]
@@ -721,15 +751,16 @@
     shrink_factor = kwargs.get('shrink_factor', 1)
     min_boundary_distance = kwargs.get('min_boundary_distance', 0)
     zorder = kwargs.get('zorder', False)
     region0 = mesh0.shapely_regions(gear=gear)
     region1 = mesh1.shapely_regions(gear=gear)
     reg_crx = region0.intersection(region1)
     if min_boundary_distance > 0:
-        reg_crx = reg_crx.buffer(-min_boundary_distance)
+        reg_crx = reg_crx.simplify(min_boundary_distance/3, preserve_topology=True)
+        reg_crx = reg_crx.buffer(-min_boundary_distance * 0.8, join_style=2)
     if reg_crx.area == 0:
         return None, None
     roi = reg_crx
     G = spatial.Geometry(roi=roi, regions={'default': reg_crx})
     mshsz = spacing
     M = Mesh.from_PSLG(**G.PSLG(), mesh_size=mshsz, min_mesh_angle=20)
     bcnters = M.triangle_centers(cache=False)
```

### Comparing `feabas-0.1.1/feabas/material.py` & `feabas-1.0.0/feabas/material.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 class Material:
     """
     Class to represent a material with a predefined material model &  mechanical
     properties.
     Kwargs:
         enable_mesh(bool): if enable_mesh set to False, the material is treated
-            as holes and no mesh will be generated on it.
+            as excluded region and no mesh will be generated on it.
         area_constraint(float): maximum triangle area constraint multiplier used
             to feed into triangulation function for meshing. The actual area
             constraint would be this value multiplied by the size settings
             during meshing. If set to 0, no constraint applied.
         render(bool): whether to render.
         render_weight(float): when mesh collides, materials with larger render
             weight have higher priority when render.
@@ -50,15 +50,15 @@
         if isinstance(mat_type, str):
             mat_type = const.MATERIAL_MODEL_LIST.index(mat_type.upper())
         self._type = mat_type
         self._stiffness_multiplier = kwargs.get('stiffness_multiplier', 1.0)
         self._poisson_ratio = kwargs.get('poisson_ratio', 0.0)
         self.mask_label = kwargs.get('mask_label', None)
         stiffness_func_factory = kwargs.get('stiffness_func_factory', None)
-        stiffness_func_params = kwargs.get('stiffness_func_params', {})
+        stiffness_func_params = kwargs.get('stiffness_func_params', {}).copy()
         self.update_stiffness_func(stiffness_func_factory, stiffness_func_params)
         uid = kwargs.get('uid', None)
         if uid is None:
             self.uid = Material.uid
             Material.uid += 1
         else:
             self.uid = uid
@@ -263,15 +263,15 @@
 
     @property
     def is_linear(self):
         return (self._type == const.MATERIAL_MODEL_ENG) and (self._stiffness_func is None)
 
 
 
-MATERIAL_HOLE = Material(enable_mesh=False,
+MATERIAL_EXCLUDE = Material(enable_mesh=False,
                          uid=0,
                          mask_label=255,
                          stiffness_multiplier=0.0,
                          render=False,
                          render_weight=1.0e-6)
 
 MATERIAL_DEFAULT = Material(enable_mesh=True,
@@ -302,16 +302,16 @@
             default_factory = lambda: default_material
         elif 'default' in table:
             default_factory = lambda: table['default']
         else:
             table['default'] = MATERIAL_DEFAULT
             default_factory = lambda: MATERIAL_DEFAULT
         self._table = defaultdict(default_factory)
-        if 'hole' not in table:
-            table['hole'] =  MATERIAL_HOLE
+        if 'exclude' not in table:
+            table['exclude'] =  MATERIAL_EXCLUDE
         self._table.update(table)
 
 
     @classmethod
     def from_json(cls, jsonname, stream=False, default_material=None):
         if stream:
             dct = json.loads(jsonname)
@@ -389,13 +389,13 @@
         for val in self._table.values():
             id_tabel[val.uid] = val
         return id_tabel
 
 
 
 # stiffness function factories.
-# stress = 1: no change; stress = 0: flip.
+# strain = 1: no change; strain = 0: flip.
 def asymmetrical_elasticity(**params):
-    stress = params.get('stress', [0, 0.75, 1, 1.01])
+    strain = params.get('strain', [0, 0.75, 1, 1.01])
     stiffness = params.get('stiffness', [1.5, 1, 0.5, 0])
-    f = interp1d(stress, stiffness, kind='linear', bounds_error=False, fill_value=(stiffness[0], stiffness[-1]))
+    f = interp1d(strain, stiffness, kind='linear', bounds_error=False, fill_value=(stiffness[0], stiffness[-1]))
     return f
```

### Comparing `feabas-0.1.1/feabas/mesh.py` & `feabas-1.0.0/feabas/mesh.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,17 @@
 import scipy.sparse.csgraph as csgraph
 from scipy.spatial import KDTree
 import shapely
 import shapely.geometry as shpgeo
 from shapely.ops import polygonize, unary_union
 import triangle
 
-from feabas import common, material, spatial
+from feabas import common, material, spatial, caching
 import feabas.constant as const
+from feabas.config import DEFAULT_RESOLUTION
 
 
 def gear_constant_to_str(gear_const):
     if isinstance(gear_const, (tuple, list)):
         gear_str = '_'.join([gear_constant_to_str(s) for s in gear_const])
     elif gear_const == const.MESH_GEAR_INITIAL:
         gear_str = 'INITIAL'
@@ -64,15 +65,15 @@
         const.MESH_GEAR_MOVING: the property is also related to the position of moving
             vertice positions;
         'TBD': the vertices on which the property is caculated is determined on
             the fly. If 'gear' is provided in the keyward argument, use that;
             otherwise, use self._current_gear.
     cache: If False, no caching;
         If True, save to self as an attribute (default);
-        If type of common.Cache, save to the cache object with key;
+        If type of caching.Cache, save to the cache object with key;
         If type defaultdict,  save to cache object with key under dict[prop_name].
     assign_value: if kwargs assign_value is given, instead of computing the property,
         directly return that value and force cache it if required.
     no_compute: if set to True, only probe if there exists cached value. If not,
         directly return None without compute. Otherwise return cached value.
         default to False.
     """
@@ -163,15 +164,15 @@
                     elif no_compute:
                         return None
                     else:
                         prop = func(self, **kwargs)
                     return prop
             else:
                 cache_key = self.caching_keys(gear=cgear)
-                if isinstance(cache, common.CacheNull):
+                if isinstance(cache, caching.CacheNull):
                     key = (*cache_key, prop_name0)
                     if not force_update and (key in cache):
                         prop = cache[key]
                         if prop is not None:
                             return prop
                     if assign_mode:
                         prop = prop0
@@ -249,15 +250,15 @@
         if np.any(indx!=np.arange(indx.size)):
             triangles = triangles[indx]
             material_ids = material_ids[indx]
             if isinstance(self._stiffness_multiplier, np.ndarray):
                 self._stiffness_multiplier = self._stiffness_multiplier[indx]
         self.triangles = triangles
         self._material_ids = material_ids
-        self._resolution = kwargs.get('resolution', const.DEFAULT_RESOLUTION)
+        self._resolution = kwargs.get('resolution', DEFAULT_RESOLUTION)
         self._epsilon = kwargs.get('epsilon', const.EPSILON0)
         self._name = kwargs.get('name', '')
         if isinstance(self._name, np.ndarray):
             self._name = common.numpy_to_str_ascii(self._name)
         self.token = kwargs.get('token', None)
         self._default_cache = kwargs.get('cache', defaultdict(lambda: True))
         if self.token is None:
@@ -274,14 +275,15 @@
         uid = kwargs.get('uid', None)   # numbering of the mesh
         if uid is None:
             self.uid = float(Mesh.uid_counter)
             Mesh.uid_counter += 1
         else:
             self.uid = float(uid)
             Mesh.uid_counter = float(max(Mesh.uid_counter, uid) + 1)
+        self.is_outcast = False
 
 
     @classmethod
     def from_PSLG(cls, vertices, segments, markers=None, **kwargs):
         """
         initialize from PSLG (feabas.spatial.Geometry.PSLG).
         Args:
@@ -291,16 +293,16 @@
             markers (dict of lists): marker points for each region names.
         Kwargs:
             mesh_size: the maximum edge length allowed in the mesh.
             min_mesh_angle: minimum angle allowed in mesh. May negatively affect
                 meshing performance, default to 0.
         """
         material_table = kwargs.get('material_table', material.MaterialTable())
-        resolution = kwargs.get('resolution', const.DEFAULT_RESOLUTION)
-        mesh_size = kwargs.get('mesh_size', (400*const.DEFAULT_RESOLUTION/resolution))
+        resolution = kwargs.get('resolution', DEFAULT_RESOLUTION)
+        mesh_size = kwargs.get('mesh_size', (400*DEFAULT_RESOLUTION/resolution))
         min_angle = kwargs.get('min_mesh_angle', 0)
         mesh_area = mesh_size ** 2
         regions = []
         holes = []
         regions_no_steiner = []
         if segments is not None:
             PSLG = {'vertices': vertices, 'segments': segments}
@@ -372,16 +374,16 @@
 
     @classmethod
     def from_polygon_equilateral(cls, mask, **kwargs):
         """
         initialize an equilateral mesh that covers the (Multi)Polygon region
         defined by mask.
         """
-        resolution = kwargs.get('resolution', const.DEFAULT_RESOLUTION)
-        mesh_size = kwargs.get('mesh_size', (400*const.DEFAULT_RESOLUTION/resolution))
+        resolution = kwargs.get('resolution', DEFAULT_RESOLUTION)
+        mesh_size = kwargs.get('mesh_size', (400*DEFAULT_RESOLUTION/resolution))
         vertices = spatial.generate_equilat_grid_mask(mask, mesh_size)
         triangles = triangle.delaunay(vertices)
         edges = Mesh.triangle2edge(triangles, directional=True)
         edge_len = np.sum(np.diff(vertices[edges], axis=-2)**2, axis=-1)**0.5
         indx = ~np.any(edge_len.reshape(3, -1) > 1.25 * mesh_size, axis=0)
         triangles = triangles[indx]
         return cls(vertices, triangles, **kwargs)
@@ -389,16 +391,16 @@
 
     @classmethod
     def from_bbox(cls, bbox, cartesian=False, **kwargs):
         # generate mesh with rectangular boundary defined by bbox
         # [xmin, ymin, xmax, ymax]
         if cartesian:
             # return a mesh from cartetian grids
-            resolution = kwargs.get('resolution', const.DEFAULT_RESOLUTION)
-            mesh_size = kwargs.get('mesh_size', (100*const.DEFAULT_RESOLUTION/resolution)) # tentative block size
+            resolution = kwargs.get('resolution', DEFAULT_RESOLUTION)
+            mesh_size = kwargs.get('mesh_size', (100*DEFAULT_RESOLUTION/resolution)) # tentative block size
             max_aspect_ratio = kwargs.get('max_aspect_ratio', 2) # the maximum aspect ratio of each block
             min_num_blocks = kwargs.get('min_num_blocks', 1) # minimum number of blocks on each side
             xmin, ymin, xmax, ymax = bbox
             ht = ymax - ymin
             wd = xmax - xmin
             Nx = max(np.round(wd / mesh_size), min_num_blocks)
             Ny = max(np.round(ht / mesh_size), min_num_blocks)
@@ -433,16 +435,16 @@
             bbox: [xmin, ymin, xmax, ymax]
         Kwargs:
             bd_width: border width. in pixel or ratio to the size of the bbox
             roundup_bbox(bool): if extend the bounding box size to make it
                 multiples of the mesh size. Otherwise, adjust the mesh size
             mesh_growth: increase of the mesh size in the interior region.
         """
-        resolution = kwargs.get('resolution', const.DEFAULT_RESOLUTION)
-        mesh_size = kwargs.get('mesh_size', (400*const.DEFAULT_RESOLUTION/resolution))
+        resolution = kwargs.get('resolution', DEFAULT_RESOLUTION)
+        mesh_size = kwargs.get('mesh_size', (400*DEFAULT_RESOLUTION/resolution))
         tan_theta = np.tan(55*np.pi/180) / 2
         xmin, ymin, xmax, ymax = bbox
         ht = ymax - ymin
         wd = xmax - xmin
         if np.array(bd_width, copy=False).size > 1:
             bd_width_x = bd_width[0]
             bd_width_y = bd_width[1]
@@ -1159,15 +1161,15 @@
         else:
             if keys_to_probe is None:
                 current_keys = self.caching_keys(gear=gear)
                 if include_hash:
                     keys_to_probe = (current_keys[0], *[s for s in current_keys[1:] if isinstance(s, tuple)])
                 else:
                     keys_to_probe = (current_keys[0], *[s for s in current_keys[1:] if isinstance(s, str)])
-            if isinstance(cache, common.CacheNull):
+            if isinstance(cache, caching.CacheNull):
                 if len(cache) == 0:
                     return
                 keys_to_delete = []
                 for key in cache:
                     if (len(keys_to_probe) == 1) and (keys_to_probe[0] == key[0]):
                         keys_to_delete.append(key)
                     else:
@@ -2093,15 +2095,15 @@
             for pr in polygons_rings:
                 if pr.contains(pts):
                     winding_number += 1
             if winding_number % 2:
                 polygons_tokeep.append(pp)
         polygon_odd_wind = unary_union(polygons_tokeep + thickened)
         polygon_odd_wind = polygon_odd_wind.buffer(self._epsilon/10, join_style=2)
-        polygon_odd_wind = polygon_odd_wind.buffer(-self._epsilon/2, join_style=2, mitre_limit=10)
+        polygon_odd_wind = polygon_odd_wind.buffer(-self._epsilon/2, join_style=2, mitre_limit=10).buffer(0)
         segments, tids0 = self.segments_w_triangle_ids(tri_mask=tri_mask)
         collided_segments = []
         rest_of_segments = []
         for seg, tid in zip(segments, tids0):
             lineseg = shpgeo.LineString(vertices[seg])
             if polygon_odd_wind.intersects(lineseg):
                 collided_segments.append((seg, tid))
```

### Comparing `feabas-0.1.1/feabas/optimizer.py` & `feabas-1.0.0/feabas/optimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from collections import defaultdict
 import gc
 import h5py
 import numpy as np
 from scipy import sparse
+import time
 
 from feabas import spatial, common
 import feabas.constant as const
 from feabas.mesh import Mesh
 
 
 class Link:
@@ -36,14 +37,16 @@
 
 
     @classmethod
     def from_coordinates(cls, mesh0, mesh1, xy0, xy1,
                          gear=(const.MESH_GEAR_INITIAL, const.MESH_GEAR_INITIAL),
                          weight=None,
                          **kwargs):
+        if xy0.size == 0:
+            return None, None
         tid0, B0 = mesh0.cart2bary(xy0, gear[0], tid=None, **kwargs)
         indx0 = tid0 >= 0
         if not np.any(indx0):
             return None, None
         elif not np.all(indx0):
             tid0 = tid0[indx0]
             B0 = B0[indx0]
@@ -271,21 +274,19 @@
     def weight(self, use_mask=False):
         if use_mask:
             return self._weight[self.mask] * self._residue_weight[self.mask]
         else:
             return self._weight * self._residue_weight
 
 
-
     @property
     def default_name(self):
         return '_'.join(str(s) for s in self.uids)
 
 
-
     @property
     def locked(self):
         return [self.meshes[0].locked, self.meshes[1].locked]
 
 
     @property
     def relevant(self):
@@ -790,14 +791,16 @@
         linked_pairs[idxt] = -1
         modified = False
         while np.any(to_optimize):
             # first find the mesh that has the most robust links to optimized ones
             link_wt_sum = Adj.dot(~to_optimize) * to_optimize
             if not np.any(link_wt_sum > 0):
                 link_wt_sum = Adj.dot(np.ones_like(to_optimize)) * to_optimize
+                if not np.any(link_wt_sum > 0):
+                    break
             idx0 = np.argmax(link_wt_sum)
             pair_locked_flag = ~to_optimize[linked_pairs]
             link_filter = np.nonzero(np.any(linked_pairs==idx0, axis=-1)
                 & np.any(pair_locked_flag, axis=-1))[0]
             if link_filter.size == 0:
                 to_optimize[idx0] = False
                 continue
@@ -859,14 +862,15 @@
             auto_clear(bool): automatically clear the stiffness term after
                 optimization is done. In some occasions, like flip checking
                 in Newton_Raphson method, this could be set to False.
         """
         maxiter = kwargs.get('maxiter', None)
         tol = kwargs.get('tol', 1e-7)
         atol = kwargs.get('atol', None)
+        callback_settings = kwargs.get('callback_settings', {}).copy()
         shape_gear = kwargs.get('shape_gear', const.MESH_GEAR_FIXED)
         targt_gear = kwargs.get('target_gear', const.MESH_GEAR_MOVING)
         start_gear = kwargs.get('start_gear', targt_gear)
         stiffness_lambda = kwargs.get('stiffness_lambda', self._stiffness_lambda)
         crosslink_lambda = kwargs.get('crosslink_lambda', self._crosslink_lambda)
         inner_cache = kwargs.get('inner_cache', self._shared_cache)
         cont_on_flip = kwargs.get('continue_on_flip', False)
@@ -912,23 +916,24 @@
                     stf_sz = 2 * m.num_vertices
                     if gio >= 0:
                         indx0.append(np.arange(crnt_offet, crnt_offet+stf_sz))
                         indx1.append(np.arange(gio, gio+stf_sz))
                     crnt_offet += stf_sz
                 indx0 = np.concatenate(indx0, axis=None)
                 indx1 = np.concatenate(indx1, axis=None)
-                T_m = sparse.csr_matrix((np.ones_like(indx0, dtype=np.float32), 
+                T_m = sparse.csr_matrix((np.ones_like(indx0, dtype=np.float32),
                                         (indx1, indx0)), shape=(grouped_dof, A.shape[0]))
                 A = T_m @ A @ T_m.transpose() / np.mean(g_cnt)
                 b = T_m @ b / np.mean(g_cnt)
             else:
                 groupings = None
         A_diag = A.diagonal()
         M = sparse.diags(1/(A_diag.clip(min(1.0, A_diag.max()/1000),None))) # Jacobi precondition
-        dd, _ = sparse.linalg.bicgstab(A, b, tol=tol, maxiter=maxiter, atol=atol, M=M)
+        # dd, _ = sparse.linalg.bicgstab(A, b, tol=tol, maxiter=maxiter, atol=atol, M=M)
+        dd = bicgstab(A, b, tol=tol, maxiter=maxiter, atol=atol, M=M, **callback_settings)
         cost = (np.linalg.norm(b), np.linalg.norm(A.dot(dd) - b))
         if cost[1] < cost[0]:
             index_offsets = self.index_offsets
             for k, m in enumerate(self.meshes):
                 if m.locked or (m.uid not in index_offsets):
                     continue
                 if groupings is None:
@@ -986,14 +991,15 @@
         anneal_mode = SLM.expand_to_list(kwargs.get('anneal_mode', None), maxepoch)
         inner_cache = kwargs.get('inner_cache', self._shared_cache)
         cont_on_flip = kwargs.get('continue_on_flip', False)
         crosslink_shrink = kwargs.get('crosslink_shrink', 0.25)
         shrink_trial = kwargs.get('shrink_trial', 3)
         groupings = kwargs.get('groupings', None)
         batch_num_matches = kwargs.get('batch_num_matches', None)
+        callback_settings = kwargs.get('callback_settings', {}).copy()
         shape_gear = const.MESH_GEAR_FIXED
         start_gear = const.MESH_GEAR_MOVING
         if cont_on_flip:
             target_gear = const.MESH_GEAR_MOVING
         else:
             target_gear = const.MESH_GEAR_STAGING
         # initialize cost and check flipped triangles
@@ -1021,16 +1027,16 @@
         while ke < maxepoch:
             step_cost = self.optimize_linear(maxiter=maxiter[ke],
                 tol=step_tol[ke], atol=step_atol[ke],
                 shape_gear=shape_gear, start_gear=start_gear, target_gear=target_gear,
                 stiffness_lambda=stiffness_lambda[ke],
                 crosslink_lambda=crosslink_lambda[ke]*cshrink,
                 inner_cache=inner_cache, continue_on_flip=cont_on_flip,
-                batch_num_matches=batch_num_matches, groupings=groupings, 
-                auto_clear=False)
+                batch_num_matches=batch_num_matches, groupings=groupings,
+                auto_clear=False, callback_settings=callback_settings)
             if (step_cost[0] is None) or (step_cost[0] < step_cost[1]):
                 break
             if anneal_mode[ke] is not None:
                 self.anneal(gear=(target_gear, shape_gear), mode=anneal_mode[ke])
             stiff_m, _ = self.stiffness_matrix(gear=(shape_gear,target_gear),
                 force_update=True, to_cache=True,
                 inner_cache=inner_cache, check_flip=check_flip,
@@ -1091,14 +1097,38 @@
         if stiff_m is None:
             return None
         stiffness_lambda, crosslink_lambda = self.relative_lambda(stiffness_lambda, crosslink_lambda)
         Cs_rht, Cs_rht = self._crosslink_terms
         return np.linalg.norm(crosslink_lambda * Cs_rht - stiffness_lambda * stress_v)
 
 
+    def flag_outcasts(self):
+        """
+        outcasts are defined as: 1) meshes not connected to any locked meshes
+        (if there is any); or 2) meshes in the minority of the subsystems if
+        all meshes are free-floating.
+        """
+        outcasts = np.zeros(self.num_meshes, dtype=bool)
+        labels, n = self.connected_subsystems
+        outcast0 = [m.is_outcast for m in self.meshes]
+        if n == 1:
+            return outcast0
+        lock_flags = self.lock_flags
+        if np.any(outcast0) or np.any(lock_flags):
+            locked_label = labels[lock_flags]
+            outcasts = ~np.isin(labels, locked_label)
+        else:
+            u, cnt = np.unique(labels, return_counts=True)
+            indx = np.argmax(cnt)
+            outcasts = labels != u[indx]
+        for m, flg in zip(self.meshes, outcasts):
+            m.is_outcast = flg
+        return outcasts
+
+
     @property
     def is_linear(self):
         linearity = True
         for m in self.meshes:
             if m.locked:
                 continue
             if not m.is_linear:
@@ -1206,14 +1236,17 @@
         """
         return [lnk for lnk in self.links if (self.link_is_relevant(lnk) == 1)]
 
 
     def match_residues(self, gear=const.MESH_GEAR_MOVING, use_mask=False, quantile=1):
         dis = []
         for lnk in self.links:
+            if use_mask and not lnk.relevant:
+                dis.append(np.nan)
+                continue
             dxy = np.sum(lnk.dxy(gear=gear, use_mask=use_mask)**2, axis=-1)**0.5
             if quantile == 1:
                 dis.append(np.max(dxy))
             elif quantile == 0:
                 dis.append(np.min(dxy))
             else:
                 dis.append(np.quantile(dxy, quantile))
@@ -1282,15 +1315,15 @@
         elif isinstance(link, common.Match):
             link_initialized = False
         else:
             raise TypeError
         if link_initialized:
             xy0 = link.xy0(gear=working_gear, use_mask=False, combine=True)
             xy1 = link.xy1(gear=working_gear, use_mask=False, combine=True)
-            weight = link._weight
+            weight = link.weight(use_mask=False)
             if link.name == link.default_name:
                 name = None
             else:
                 name = link.name
         else:
             xy0 = link.xy0
             xy1 = link.xy1
@@ -1320,14 +1353,93 @@
     def expand_to_list(elem, list_len):
         if (not hasattr(elem, '__len__')) or isinstance(elem, str):
             return [elem] * list_len
         else:
             return elem
 
 
+class EarlyStopFlag(Exception):
+    pass
+
+
+class SLM_Callback:
+    """
+    call back function class fed to bicgstab optimizer.
+    Args:
+        A, b: equation terms to solve x: Ax = b.
+    Kwargs:
+        timeout: timeout time for the optimizer (in seconds);
+        early_stop_thresh: the threshold for the differences between two
+            consecutive solutions below which it is considered small update;
+        eval_step: skip step to evaluate the callback function;
+        chances: if the number of consecutive iterations with enlarged cost or
+            small updates is larger than this number, envoke early stopping.
+    """
+    def __init__(self, A, b, timeout=None, early_stop_thresh=None, chances=5, eval_step=10):
+        self._A = A
+        self._b = b
+        self._timout = timeout
+        self._early_stop_thresh = early_stop_thresh
+        self._eval_step = eval_step
+        self._t0 = time.time()
+        self._last_x = 0
+        self._last_cost = np.inf
+        self.min_cost = np.inf
+        self.solution = None
+        self._count = 0
+        self._chances = chances
+        self._exit_count = 0
+
+
+    def callback(self, x):
+        if self._count % self._eval_step == 0:
+            cost = np.linalg.norm(self._A.dot(x) - self._b)
+            if cost < self.min_cost:
+                self.min_cost = cost
+                self.solution = x
+            if self._timout is not None:
+                t = time.time() - self._t0
+                if t > self._timout:
+                    raise EarlyStopFlag
+            if self._chances is not None:
+                if cost > self._last_cost:
+                    self._exit_count += 1
+                elif self._early_stop_thresh is not None:
+                    dis = np.max(np.abs(x - self._last_x))
+                    if dis <= self._early_stop_thresh:
+                        self._exit_count += 1
+                    else:
+                        self._exit_count = 0
+                else:
+                    self._exit_count = 0
+                if self._exit_count > self._chances:
+                    raise EarlyStopFlag
+                self._last_x = x.copy()
+                self._last_cost = cost
+        self._count += 1
+        return False
+
+
+def bicgstab(A, b, tol=1e-07, atol=None, maxiter=None, M=None, **kwargs):
+    timeout = kwargs.get('timeout', None)
+    early_stop_thresh = kwargs.get('early_stop_thresh', None)
+    chances = kwargs.get('chances', None)
+    eval_step = kwargs.get('eval_step', 10)
+    cb = SLM_Callback(A, b, timeout=timeout, early_stop_thresh=early_stop_thresh, chances=chances, eval_step=eval_step)
+    callback = cb.callback
+    try:
+        x, _ = sparse.linalg.bicgstab(A, b, tol=tol, maxiter=maxiter, atol=atol, M=M, callback=callback)
+        cost0 = np.linalg.norm(A.dot(x) - b)
+        if cost0 > cb.min_cost:
+            x = cb.solution
+    except EarlyStopFlag:
+        x = cb.solution
+    return x
+
+
 
 def transform_mesh(mesh_unlocked, mesh_locked, **kwargs):
     err_thresh = kwargs.pop('err_thresh', None)
     kwargs.setdefault('continue_on_flip', True)
     uid_mov = mesh_unlocked.uid
     locked_mov = mesh_unlocked.locked
     mesh_locked = mesh_locked.copy(override_dict={'locked': True, 'uid': 0})
```

### Comparing `feabas-0.1.1/feabas/renderer.py` & `feabas-1.0.0/feabas/renderer.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import os
 import shapely.geometry as shpgeo
 from shapely.ops import unary_union
 
 import feabas.constant as const
 from feabas.mesh import Mesh
 from feabas import common, spatial, dal
+from feabas.config import DEFAULT_RESOLUTION
 
 
 class MeshRenderer:
     """
     A class to apply transforms according to a Mesh and render images.
     """
     def __init__(self, interpolators, **kwargs):
@@ -23,15 +24,15 @@
         self._offset = np.array(kwargs.get('offset', np.zeros((1,2))), copy=False).reshape(1,2)
         self._region_tree = kwargs.get('region_tree', None)
         self._weight_params = kwargs.get('weight_params', const.MESH_TRIFINDER_WHATEVER)
         self.weight_generator = kwargs.get('weight_generator', [None for _ in range(n_region)])
         self.weight_multiplier = kwargs.get('weight_multiplier', [None for _ in range(n_region)])
         self._collision_region = kwargs.get('collision_region', None)
         self._image_loader = kwargs.get('image_loader', None)
-        self.resolution = kwargs.get('resolution', const.DEFAULT_RESOLUTION)
+        self.resolution = kwargs.get('resolution', DEFAULT_RESOLUTION)
         self._default_fillval = kwargs.get('fillval', None)
         self._dtype = kwargs.get('dtype', None)
 
 
     @classmethod
     def from_mesh(cls, srcmesh, gear=(const.MESH_GEAR_MOVING, const.MESH_GEAR_INITIAL), **kwargs):
         include_flipped = kwargs.get('include_flipped', False)
@@ -476,43 +477,48 @@
     keywords = ['{ROW_IND}', '{COL_IND}', '{X_MIN}', '{Y_MIN}', '{X_MAX}', '{Y_MAX}']
     resolution = image_loader.resolution
     mesh.change_resolution(resolution / scale)
     kwargs.setdefault('target_resolution', resolution / scale)
     tileht, tilewd = tile_size
     if canvas_bbox is None:
         gx_min, gy_min, gx_max, gy_max = mesh.bbox(gear=const.MESH_GEAR_MOVING)
+        x0, y0 = 0, 0
     else:
         gx_min, gy_min, gx_max, gy_max = canvas_bbox
+        x0, y0 = gx_min, gy_min
+        gx_max = gx_max - gx_min
+        gy_max = gy_max - gy_min
+        gx_min, gy_min = 0, 0
     tx_max = int(np.ceil(gx_max  / tilewd))
     ty_max = int(np.ceil(gy_max  / tileht))
     tx_min = int(np.floor(gx_min  / tilewd))
     ty_min = int(np.floor(gy_min  / tileht))
     cols, rows = np.meshgrid(np.arange(tx_min, tx_max), np.arange(ty_min, ty_max))
     cols, rows = cols.ravel(), rows.ravel()
     idxz = common.z_order(np.stack((rows, cols), axis=-1))
     cols, rows = cols[idxz], rows[idxz]
     filenames = []
     bboxes = []
     region = mesh.shapely_regions(gear=const.MESH_GEAR_MOVING, offsetting=True)
     for r, c in zip(rows, cols):
-        bbox = (c*tilewd, r*tileht, (c+1)*tilewd, (r+1)*tileht)
+        bbox = (c*tilewd + x0, r*tileht + y0, (c+1)*tilewd + x0, (r+1)*tileht + y0)
         if not region.intersects(shpgeo.box(*bbox)):
             continue
         bboxes.append(bbox)
         xmin, ymin, xmax, ymax = bbox
         keyword_replaces = [str(r+one_based), str(c+one_based), str(xmin), str(ymin), str(xmax), str(ymax)]
         fname = pattern
         for kw, kwr in zip(keywords, keyword_replaces):
             fname = fname.replace(kw, kwr)
         filenames.append(prefix + fname)
     rendered = {}
     num_tiles = len(filenames)
     if num_tiles == 0:
         pass
-    elif (num_workers > 1) or (num_tiles == 1):
+    elif (num_workers > 1) and (num_tiles > 1):
         num_tile_per_job = max(1, num_tiles // num_workers)
         if max_tile_per_job is not None:
             num_tile_per_job = min(num_tile_per_job, max_tile_per_job)
         N_jobs = round(num_tiles / num_tile_per_job)
         indices = np.round(np.linspace(0, num_tiles, num=N_jobs+1, endpoint=True))
         indices = np.unique(indices).astype(np.uint32)
         bboxes_list = []
@@ -533,40 +539,35 @@
             for msh, bbox, fnames in zip(submeshes, bboxes_list, filenames_list):
                 msh_dict = msh.get_init_dict(save_material=True, vertex_flags=(const.MESH_GEAR_INITIAL, const.MESH_GEAR_MOVING))
                 job = executor.submit(target_func, msh_dict, bbox, fnames)
                 jobs.append(job)
             for job in as_completed(jobs):
                 rendered.update(job.result())
     else:
-        renderer = MeshRenderer.from_mesh(mesh, **kwargs)
-        renderer.link_image_loader(image_loader)
-        for fname, bbox in zip(filenames, bboxes):
-            imgt = renderer.crop(bbox)
-            if imgt is not None:
-                common.imwrite(fname, imgt)
-                rendered[os.path.basename(fname)] = bbox
+        rendered = subprocess_render_mesh_tiles(image_loader, mesh, bboxes, filenames, **kwargs)
     return rendered
 
 
 def subprocess_render_mesh_tiles(imgloader, mesh, bboxes, outnames, **kwargs):
     target_resolution = kwargs.pop('target_resolution')
     if isinstance(imgloader, (str, dict)):
-        image_loader = dal.get_loader_from_json(imgloader)
+        imgloader = dal.get_loader_from_json(imgloader)
     if isinstance(mesh, str):
         M = Mesh.from_h5(mesh)
     elif isinstance(mesh, dict):
         M = Mesh(**mesh)
     else:
         M = mesh
     M.change_resolution(target_resolution)
     renderer = MeshRenderer.from_mesh(M, **kwargs)
-    renderer.link_image_loader(image_loader)
+    renderer.link_image_loader(imgloader)
+    fillval = kwargs.get('fillval', renderer.default_fillval)
     rendered = {}
     for fname, bbox in zip(outnames, bboxes):
         if os.path.isfile(fname):
-            rendered[os.path.basename(fname)] = bbox
+            rendered[fname] = bbox
             continue
-        imgt = renderer.crop(bbox)
-        if imgt is not None:
+        imgt = renderer.crop(bbox, **kwargs)
+        if (imgt is not None) and np.any(imgt != fillval, axis=None):
             common.imwrite(fname, imgt)
-            rendered[os.path.basename(fname)] = bbox
+            rendered[fname] = bbox
     return rendered
```

### Comparing `feabas-0.1.1/feabas/spatial.py` & `feabas-1.0.0/feabas/spatial.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from collections import defaultdict, OrderedDict
 
 import cv2
 import h5py
 import numpy as np
 import shapely.geometry as shpgeo
 from shapely.ops import unary_union, linemerge, polygonize
-from shapely import wkb
+from shapely import wkb, get_coordinates
 
 from feabas import dal, common, material
 import feabas.constant as const
+from feabas.config import DEFAULT_RESOLUTION
 
 
 JOIN_STYLE = shpgeo.JOIN_STYLE.mitre
 
 
 def fit_affine(pts0, pts1, return_rigid=False, weight=None, svd_clip=(1,1), avoid_flip=True):
     # pts0 = pts1 @ A
@@ -38,15 +39,14 @@
     r1 = np.linalg.matrix_rank(pts0_pad)
     A = res[0]
     r = min(res[2], r1)
     if avoid_flip and np.linalg.det(A) < 0:
         r = 2
     if r == 1:
         A = np.eye(3)
-        A[-1,:2] = mm0 - mm1
     elif r == 2:
         pts0_rot90 = pts0[:,::-1] * np.array([1,-1])
         pts1_rot90 = pts1[:,::-1] * np.array([1,-1])
         pts0 = np.concatenate((pts0, pts0_rot90), axis=0)
         pts1 = np.concatenate((pts1, pts1_rot90), axis=0)
         pts0_pad = np.insert(pts0/std_scl, 2, 1, axis=-1)
         pts1_pad = np.insert(pts1/std_scl, 2, 1, axis=-1)
@@ -90,39 +90,60 @@
     if not np.any(mask):
         return (), None
     mask = mask.astype(np.uint8, copy=False)
     if cv2.__version__ < '4':
         _, contours, hierarchy = cv2.findContours(mask, cv2.RETR_CCOMP, approx_mode)
     else:
         contours, hierarchy = cv2.findContours(mask, cv2.RETR_CCOMP, approx_mode)
+    contours = _pad_concave_corner(contours)
     return contours, hierarchy
 
 
+def _pad_concave_corner(countours):
+    padded = []
+    for ct in countours:
+        xy0 = ct.squeeze()
+        xy1 = np.roll(xy0, 1, axis=0)
+        stp = xy1 - xy0
+        diag_indx = np.nonzero(np.all(stp != 0, axis=-1))[0]
+        if diag_indx.size > 0:
+            dxy = stp[diag_indx]
+            dxy = (dxy + dxy[:,::-1] * np.array([-1, 1])) / 2
+            txy = xy0[diag_indx] + dxy
+            xy0 = np.insert(xy0, diag_indx, txy, axis=0)
+            stp0 = (np.roll(xy0, 1, axis=0) - xy0 != 0) | (np.roll(xy0, -1, axis=0) - xy0 != 0)
+            keep_indx = np.all(stp0, axis=-1)
+            xy0 = xy0[keep_indx]
+        padded.append(xy0)
+    return padded
+
+
 
 def countours_to_polygon(contours, hierarchy, offset, scale, upsample):
     """
     convert opencv contours to shapely (Multi)Polygons.
     Args:
         contours, hierarchy: output from find_countours.
     Kwargs:
         offsets: x, y translation offset to add to the output polygon.
         scale: scaling factor of the geometries.
         upsample: upsample factor for better accuracy.
     """
     polygons_staging = {}
     holes = {}
-    buffer_r = 0.5 * scale / upsample # expand by half pixel
+    buffer_r = 0.51 * scale / upsample # expand by half pixel
     for indx, ct in enumerate(contours):
         number_of_points = ct.shape[0]
         if number_of_points < 3:
             continue
         xy = scale_coordinates(ct.reshape(number_of_points, -1), scale=1/upsample)
         xy = scale_coordinates(xy + np.asarray(offset), scale=scale)
         lr = shpgeo.polygon.LinearRing(xy)
-        pp = shpgeo.Polygon(lr)
+        # lr = smooth_zigzag(lr, scale=scale)
+        pp = shpgeo.Polygon(lr).buffer(0)
         if lr.is_ccw:
             holes[indx] = pp
         else:
             polygons_staging[indx] = pp
     if len(polygons_staging) == 0:
         return None     # no region found
     hierarchy = hierarchy.reshape(-1, 4)
@@ -198,14 +219,16 @@
         for name, lbl in labels.items():
             if lbl is None:
                 continue
             if len(tile.shape) > 2: # RGB
                 mask = np.all(tile == np.array(lbl), axis=-1)
             else:
                 mask = (tile == lbl)
+            if not np.any(mask, axis=None):
+                continue
             if upsample != 1:
                 mask = (cv2.resize(255*mask.astype(np.uint8), None, fx=upsample, fy=upsample, interpolation=cv2.INTER_LINEAR)) > 127
             ct, h = find_contours(mask)
             p_lbl = countours_to_polygon(ct, h, offset=np.array(offset), scale=scale, upsample=upsample)
             if p_lbl is not None:
                 polygons[name] = p_lbl
     return polygons, extent
@@ -277,14 +300,68 @@
         return new_list
     elif hasattr(poly, 'area') and poly.area == 0:
         return shpgeo.Polygon()
     else:
         raise TypeError
 
 
+def smooth_zigzag(boundary, roi=None, scale=1.0, tol=0.5):
+    """
+    smooth the zigzag border of a polygon defined by bit-map images.
+    boundary (shapely.geometry.LineString): boundary of the polygon
+    """
+    tol = tol * scale
+    boundary = boundary.simplify(1.0e-3 * tol, preserve_topology=False)
+    if hasattr(boundary, 'geoms'):
+        boundaries = list(l for l in boundary.geoms)
+    else:
+        boundaries = [boundary]
+    smoothened = []
+    for lr in boundaries:
+        if lr.length == 0:
+            continue
+        vertices = get_coordinates(lr)
+        if vertices.shape[0] <= 2:
+            smoothened.append(lr)
+            continue
+        if np.all(vertices[0] == vertices[-1]):
+            is_closed = True
+        else:
+            is_closed = False
+        vpts = [pt for pt in shpgeo.MultiPoint(vertices).geoms]
+        mid_points = (vertices[:-1] + vertices[1:]) / 2
+        if is_closed:
+            ml = shpgeo.LinearRing(mid_points)
+        else:
+            ml = shpgeo.LineString(mid_points)
+        dis = ml.distance(vpts)
+        to_keep = dis >= tol
+        if roi is not None:
+            dis0 = roi.distance(vpts)
+            to_keep = to_keep | (dis0 < tol)
+        if not is_closed:
+            to_keep[0] = True
+            to_keep[-1] = True
+        vindx = 2 * (np.nonzero(to_keep)[0])
+        mindx = 2 * np.arange(mid_points.shape[0]) + 1
+        vertices_new = np.concatenate((vertices[to_keep], mid_points), axis=0)
+        sindx = np.argsort(np.concatenate((vindx, mindx)))
+        vertices_new = vertices_new[sindx]
+        if is_closed:
+            lr_new = shpgeo.LinearRing(vertices_new)
+        else:
+            lr_new = shpgeo.LineString(vertices_new)
+        lr_new = lr_new.simplify(1.0e-3 * tol, preserve_topology=False)
+        smoothened.append(lr_new)
+    if len(smoothened) == 1:
+        smoothened = smoothened[0]
+    else:
+        smoothened = unary_union(smoothened)
+    return smoothened
+
 
 def clean_up_small_regions(regions, roi=None, area_thresh=4, buffer=1e-3):
     if area_thresh == 0:
         return regions, shpgeo.Polygon()
     if not isinstance(regions, dict):
         regions_dict = {k: rg for k, rg in enumerate(regions)}
     else:
@@ -426,15 +503,15 @@
     """
     def __init__(self, roi=None, regions=None, **kwargs):
         if regions is None:
             regions = {}
         self._roi = roi
         self._default_region = None
         self._regions = regions
-        self._resolution = kwargs.get('resolution', const.DEFAULT_RESOLUTION)
+        self._resolution = kwargs.get('resolution', DEFAULT_RESOLUTION)
         self._zorder = kwargs.get('zorder', list(self._regions.keys()))
         self._committed = False
         self._epsilon = kwargs.get('epsilon', const.EPSILON0) # small value used for buffer
 
 
     @classmethod
     def from_image_mosaic(cls, image_loader, material_table=None, region_names=None, **kwargs):
@@ -450,15 +527,15 @@
                 that defines the region names and labels.
             region_names(OrderedDict): OrderedDict mapping region names to their
                 corresponding labels, in addition to material_table.
             dilate(float): dilation radius to grow regions.
             scale(float): if image_loader is not a MosaicLoader, use this to
                 define scaling factor.
         """
-        resolution = kwargs.get('resolution', const.DEFAULT_RESOLUTION)
+        resolution = kwargs.get('resolution', DEFAULT_RESOLUTION)
         oor_label = kwargs.get('oor_label', None)
         roi_erosion = kwargs.get('roi_erosion', 0.5)
         dilate = kwargs.get('dilate', 0.1)
         scale = kwargs.get('scale', 1.0) # may change if imageloader has different resolution
         name2label = OrderedDict() # region name to label mapping
         if material_table is not None:
             name2label = material_table.name_to_label_mapping
@@ -543,15 +620,15 @@
                     self._zorder.append(lbl)
                 else:
                     self._zorder.insert(pos, lbl)
         self._committed = False
 
 
     def add_regions_from_image(self, image, material_table=None, region_names=None, **kwargs):
-        resolution = kwargs.get('resolution', const.DEFAULT_RESOLUTION)
+        resolution = kwargs.get('resolution', DEFAULT_RESOLUTION)
         dilate = kwargs.get('dilate', 0.1)
         scale = kwargs.get('scale', 1.0)
         mode = kwargs.get('mode', 'u')
         pos = kwargs.get('pos', None)
         if isinstance(image, dal.MosaicLoader):
             scale = image.resolution / resolution
         dilate = dilate * scale
@@ -584,15 +661,15 @@
             self._roi = self._roi.intersection(roi)
         else:
             self._roi = self._roi.union(roi)
         self._committed = False
 
 
     def modify_roi_from_image(self, image, roi_label=0, **kwargs):
-        resolution = kwargs.get('resolution', const.DEFAULT_RESOLUTION)
+        resolution = kwargs.get('resolution', DEFAULT_RESOLUTION)
         roi_erosion = kwargs.get('roi_erosion', 0)
         scale = kwargs.get('scale', 1.0)
         mode = kwargs.get('mode', 'r')
         if isinstance(image, dal.MosaicLoader):
             scale = image.resolution / resolution
         roi_erosion = roi_erosion * scale
         poly, extent = images_to_polygons(image, {'roi': roi_label}, scale=scale)
@@ -642,18 +719,18 @@
             filled_cover = []
             for linestr in covered_boundary.geoms:
                 area_sign = shpgeo.LinearRing(linestr).is_ccw
                 if area_sign:
                     filled_cover.append(shpgeo.Polygon(linestr))
             holes = unary_union(filled_cover).difference(covered)
             if holes.area > 0:
-                if 'hole' in self._regions:
-                    self._regions['hole'] = (self._regions['hole'].union(holes)).buffer(0)
+                if 'exclude' in self._regions:
+                    self._regions['exclude'] = (self._regions['exclude'].union(holes)).buffer(0)
                 else:
-                    self._regions['hole'] = holes.buffer(0)
+                    self._regions['exclude'] = holes.buffer(0)
         self._committed = True
 
 
     def collect_boundaries(self, **kwargs):
         if not self._committed:
             self.commit(**kwargs)
         boundaries = []
@@ -723,15 +800,16 @@
         if self._committed:
             import warnings
             warnings.warn('Geometry alread commited. Simplification aborted', RuntimeWarning)
             return self
         if not isinstance(region_tol, dict):
             region_tols = defaultdict(lambda: region_tol)
         else:
-            region_tols = region_tol
+            region_tols = region_tol.copy()
+        region_tols.setdefault('default', np.inf)
         if method == const.SPATIAL_SIMPLIFY_SEGMENT:
             G = self.simplify_by_segments(region_tols, roi_tol=roi_tol,
                 inplace=inplace, scale=scale, area_thresh=area_thresh)
         elif method == const.SPATIAL_SIMPLIFY_REGION:
             G = self.simplify_by_regions(region_tols, roi_tol=roi_tol,
                 inplace=inplace, scale=scale, area_thresh=area_thresh)
         else:
@@ -777,15 +855,15 @@
         polygons_formalized = list(polygonize(bu0))
         polygons_formalized, _ = clean_up_small_regions(polygons_formalized, area_thresh=area_thresh, buffer=self._epsilon)
         formalized_polygon_areas = [p.area for p in polygons_formalized]
         min_poly_area = np.min(formalized_polygon_areas)
         boundaries = OrderedDict()
         poly_assigned = np.zeros(len(polygons_formalized), dtype=bool)
         for lbl in reversed(self._zorder):
-            if lbl not in polygons_cleaned:
+            if (lbl == 'default') or (lbl not in polygons_cleaned):
                 continue
             poly = polygons_cleaned[lbl]
             if poly.area == 0:
                 continue
             bndr = []
             area_left = poly.area
             for kf, pf in enumerate(polygons_formalized):
@@ -797,49 +875,62 @@
                     continue
                 area_ints = pf.intersection(poly).area
                 if  area_ints / formalized_polygon_areas[kf] > 0.99:
                     bndr.append(pf.boundary)
                     poly_assigned[kf] = True
                     area_left -= area_ints
             boundaries[lbl] = unary_union(bndr)
+        if not np.all(poly_assigned):
+            left_overs = unary_union([pf for pf, flg in zip(polygons_formalized, poly_assigned) if not flg])
+            boundaries['default'] = left_overs.boundary
         b_merged = unary_union(boundaries.values())
         if hasattr(b_merged, 'geoms'):
             b_merged = linemerge(b_merged)
         if not hasattr(b_merged, 'geoms'):
             bag_of_segs = [b_merged]
         else:
             bag_of_segs = list(b_merged.geoms)
-        region_names = sorted(list(self._regions.keys()), key=lambda s:region_tols[s])
+        region_names = sorted(list(self._regions.keys()), key=lambda s:region_tols[s]) + ['default']
         segs_in_regions = defaultdict(list)
         for seg_idx, seg in enumerate(bag_of_segs):
             for lbl, bndr in boundaries.items():
                 if bndr.intersects(seg) and bndr.intersection(seg).length > 0:
                     segs_in_regions[lbl].append(seg_idx)
         simplify_order = []
         simplify_tol = []
         for lbl in region_names:
             if lbl not in segs_in_regions:
                 continue
             tol = region_tols[lbl]
             slist = [s for s in segs_in_regions[lbl] if s not in simplify_order]
             simplify_order.extend(slist)
             simplify_tol.extend([tol]*len(slist))
+        bag_of_segs = [smooth_zigzag(s) for s in bag_of_segs]
         for sidx, tol in zip(simplify_order, simplify_tol):
+            if np.isinf(tol):
+                continue
+            seg_target = unary_union([s for k, s in enumerate(bag_of_segs) if (k==sidx)])
             segs_except_target = unary_union([s for k, s in enumerate(bag_of_segs) if (k!=sidx)])
             segs_all = unary_union(bag_of_segs)
             # fix segments other than the one to be simplified by duplicating them
             segs_combined = unary_union([segs_except_target, segs_all])
             segs_simplified = segs_combined.simplify(tol*scale, preserve_topology=True)
             seg_new = segs_simplified.difference(segs_except_target)
+            tol_g = tol*scale
+            while not seg_target.boundary.difference(seg_new.boundary).is_empty:
+                tol_g /= 1.414
+                segs_simplified = segs_combined.simplify(tol_g, preserve_topology=True)
+                seg_new = segs_simplified.difference(segs_except_target)
             if hasattr(seg_new, 'geoms'):
                 seg_new = linemerge(seg_new)
             if seg_new.length > 0:
                 bag_of_segs[sidx] = seg_new
         regions_new = {} # reassemble boundaries
-        for lbl, sidx in segs_in_regions.items():
+        for lbl in self._regions:
+            sidx = segs_in_regions[lbl]
             boundaries_new = unary_union([bag_of_segs[s] for s in sidx])
             polys = list(polygonize(boundaries_new))
             cnt = np.zeros(len(polys), dtype=np.uint16)
             for p0 in polys:
                 p0c = shpgeo.Polygon(p0.exterior)
                 for k1, p1 in enumerate(polys):
                     if p0 is p1:
@@ -847,14 +938,17 @@
                     if p0c.contains(p1):
                         cnt[k1] += 1
             pp_updated = unary_union([p for k, p in enumerate(polys) if (cnt[k]%2 == 0)])
             if inplace:
                 self._regions[lbl] = pp_updated
             else:
                 regions_new[lbl] = pp_updated
+        roi = unary_union(list(polygonize(bag_of_segs)))
+        if inplace:
+            self._roi = roi
         if inplace:
             return self
         else:
             return Geometry(roi=roi, regions=regions_new,
                 resolution=self._resolution, zorder=self._zorder)
 
 
@@ -896,15 +990,15 @@
         polygons_formalized = list(polygonize(bu0))
         polygons_formalized, modified_area = clean_up_small_regions(polygons_formalized, area_thresh=area_thresh, buffer=self._epsilon)
         formalized_polygon_areas = [p.difference(modified_area).area for p in polygons_formalized]
         min_poly_area = np.min(formalized_polygon_areas)
         boundaries = OrderedDict()
         poly_assigned = np.zeros(len(polygons_formalized), dtype=bool)
         for lbl in reversed(self._zorder):
-            if lbl not in polygons_cleaned:
+            if (lbl == 'default') or (lbl not in polygons_cleaned):
                 continue
             poly = polygons_cleaned[lbl]
             if poly.area == 0:
                 continue
             bndr = []
             area_left = poly.area
             for kf, pf in enumerate(polygons_formalized):
@@ -916,46 +1010,57 @@
                     continue
                 area_ints = pf.intersection(poly).area
                 if  area_ints / formalized_polygon_areas[kf] > 0.99:
                     bndr.append(pf.boundary)
                     poly_assigned[kf] = True
                     area_left -= area_ints
             boundaries[lbl] = unary_union(bndr)
+        if not np.all(poly_assigned):
+            left_overs = unary_union([pf for pf, flg in zip(polygons_formalized, poly_assigned) if not flg])
+            boundaries['default'] = left_overs.boundary
         b_merged = unary_union(list(boundaries.values()))
         if hasattr(b_merged, 'geoms'):
             b_merged = linemerge(b_merged)
         if not hasattr(b_merged, 'geoms'):
             bag_of_segs = [b_merged]
         else:
             bag_of_segs = list(b_merged.geoms)
-        region_names = sorted(list(self._regions.keys()), key=lambda s:region_tols[s])
+        region_names = sorted(list(self._regions.keys()), key=lambda s:region_tols[s]) + ['default']
         region_names_lut = {rn:krn for krn, rn in enumerate(region_names)}
         labels_of_segs = defaultdict(list)
         for seg_idx, seg in enumerate(bag_of_segs):
             for lbl, bndr in boundaries.items():
                 if bndr.intersects(seg) and bndr.intersection(seg).length > 0:
                     labels_of_segs[seg_idx].append(region_names_lut[lbl])
         seg_groups = defaultdict(list)
         for seg_idx, lbl_ids in labels_of_segs.items():
-            seg_groups[tuple(lbl_ids)].append(bag_of_segs[seg_idx])
-        seg_groups = {lbl_id: linemerge(lines) for lbl_id, lines in seg_groups.items()}
+            seg_groups[tuple(sorted(lbl_ids))].append(bag_of_segs[seg_idx])
+        seg_groups = {lbl_id: smooth_zigzag(linemerge(lines)) for lbl_id, lines in seg_groups.items()}
         group_indices = sorted(seg_groups.keys())
         group_tols = [region_tols[region_names[lbl[0]]] for lbl in group_indices]
         for gidx, tol in zip(group_indices, group_tols):
+            if np.isinf(tol):
+                continue
+            seg_target = unary_union([s for k, s in seg_groups.items() if (k==gidx)])
             segs_except_target = unary_union([s for k, s in seg_groups.items() if (k!=gidx)])
             segs_all = unary_union(list(seg_groups.values()))
             # fix segments other than the one to be simplified by duplicating them
             segs_combined = unary_union([segs_except_target, segs_all])
             segs_simplified = segs_combined.simplify(tol*scale, preserve_topology=True)
             seg_new = segs_simplified.difference(segs_except_target)
+            tol_g = tol*scale
+            while not seg_target.boundary.difference(seg_new.boundary).is_empty:
+                tol_g /= 1.414
+                segs_simplified = segs_combined.simplify(tol_g, preserve_topology=True)
+                seg_new = segs_simplified.difference(segs_except_target)
             if hasattr(seg_new, 'geoms'):
                 seg_new = linemerge(seg_new)
             seg_groups[gidx] = seg_new
         regions_new = {} # reassemble boundaries
-        for lbl in region_names:
+        for lbl in self._regions:
             lbl_id = region_names_lut[lbl]
             boundaries_new = unary_union([s for gidx, s in seg_groups.items() if lbl_id in gidx])
             polys = list(polygonize(boundaries_new))
             cnt = np.zeros(len(polys), dtype=np.uint16)
             for p0 in polys:
                 p0c = shpgeo.Polygon(p0.exterior)
                 for k1, p1 in enumerate(polys):
@@ -964,14 +1069,17 @@
                     if p0c.contains(p1):
                         cnt[k1] += 1
             pp_updated = unary_union([p for k, p in enumerate(polys) if (cnt[k]%2 == 0)])
             if inplace:
                 self._regions[lbl] = pp_updated
             else:
                 regions_new[lbl] = pp_updated
+        roi = unary_union(list(polygonize(list(seg_groups.values()))))
+        if inplace:
+            self._roi = roi
         if inplace:
             return self
         else:
             return Geometry(roi=roi, regions=regions_new,
                 resolution=self._resolution, zorder=self._zorder)
 
 
@@ -1061,14 +1169,23 @@
                 'segments': segments,
                 'markers': markers,
                 'resolution': self._resolution,
                 'epsilon': self._epsilon}
         return PSLG
 
 
+    @property
+    def region_default(self):
+        mask = self._roi
+        for lb, pp in self._regions.items():
+            if lb != 'default':
+                mask = mask.difference(pp)
+        return mask
+
+
     @staticmethod
     def region_names_from_material_dict(material_dict):
         if isinstance(material_dict, str):
             if '.json' in material_dict:
                 MT = material.MaterialTable.from_json(material_dict, stream=False)
             else:
                 MT = material.MaterialTable.from_json(material_dict, stream=True)
```

### Comparing `feabas-0.1.1/feabas/stitcher.py` & `feabas-1.0.0/feabas/stitcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import cv2
 from collections import defaultdict, namedtuple
 from concurrent.futures.process import ProcessPoolExecutor
 from concurrent.futures import as_completed
 from functools import partial
 import gc
 import h5py
 import matplotlib.tri
@@ -11,21 +12,22 @@
 from rtree import index
 from scipy.interpolate import interp1d
 from scipy.ndimage import gaussian_filter, binary_dilation
 from scipy import sparse
 import scipy.sparse.csgraph as csgraph
 
 from feabas.dal import StaticImageLoader
+from feabas import logging
 from feabas.matcher import stitching_matcher
 from feabas.mesh import Mesh
 from feabas.optimizer import SLM
-from feabas import common
+from feabas import common, caching
 from feabas.spatial import scale_coordinates
 import feabas.constant as const
-
+from feabas.config import DEFAULT_RESOLUTION
 
 class Stitcher:
     """
     Class to handle everything related to 2d stitching.
 
     Args:
         imgpaths(list): fullpaths of the image file list
@@ -37,14 +39,15 @@
             paths and root_dir will be prepended to generate the fullpaths.
     """
   ## ------------------------- initialization & IO ------------------------- ##
     def __init__(self, imgpaths, bboxes, **kwargs):
         root_dir = kwargs.get('root_dir', None)
         groupings = kwargs.get('groupings', None)
         self._connected_subsystem = kwargs.get('connected_subsystem', None)
+        self.resolution = kwargs.get('resolution', DEFAULT_RESOLUTION)
         if bool(root_dir):
             self.imgrootdir = root_dir
             self.imgrelpaths = imgpaths
         else:
             self.imgrootdir = os.path.dirname(os.path.commonprefix(imgpaths))
             self.imgrelpaths = [os.path.relpath(s, self.imgrootdir) for s in imgpaths]
         bboxes = np.round(bboxes).astype(np.int32)
@@ -60,16 +63,16 @@
         self._optimizer = None
         self._default_mesh_cache = None
         self.set_groupings(groupings)
 
 
     @classmethod
     def from_coordinate_file(cls, filename, **kwargs):
-        imgpaths, bboxes, root_dir, _ = common.parse_coordinate_files(filename, **kwargs)
-        return cls(imgpaths, bboxes, root_dir=root_dir)
+        imgpaths, bboxes, root_dir, resolution = common.parse_coordinate_files(filename, **kwargs)
+        return cls(imgpaths, bboxes, root_dir=root_dir, resolution=resolution)
 
 
     @classmethod
     def from_h5(cls, filename, load_matches=True, load_meshes=True, selected=None):
         """
         selected (ndarray of int): if provided, only load tiles whose indices
         are in selected.
@@ -82,23 +85,27 @@
                 groupings = f['groupings'][()]
             else:
                 groupings = None
             if 'connected_subsystem' in f:
                 connected_subsystem = f['connected_subsystem'][()]
             else:
                 connected_subsystem = None
+            if 'resolution' in f:
+                resolution = f['resolution'][()]
+            else:
+                resolution = DEFAULT_RESOLUTION
         if selected is not None:
             imgpaths = [s for k, s in enumerate(imgpaths) if k in selected]
             bboxes = bboxes[selected]
             groupings = groupings[selected]
             check_order = True
         else:
             check_order = False
         obj = cls(imgpaths, bboxes, root_dir=root_dir, groupings=groupings,
-            connected_subsystem=connected_subsystem)
+            connected_subsystem=connected_subsystem, resolution=resolution)
         if load_matches:
             obj.load_matches_from_h5(filename, check_order=check_order)
         if load_meshes:
             obj.load_meshes_from_h5(filename, check_order=check_order)
         return obj
 
 
@@ -108,14 +115,15 @@
         compression = kwargs.get('compression', True)
         with h5py.File(fname, 'w') as f:
             if compression:
                 create_dataset = partial(f.create_dataset, compression='gzip')
             else:
                 create_dataset = f.create_dataset
             f.create_dataset('imgrootdir', data=common.str_to_numpy_ascii(self.imgrootdir))
+            f.create_dataset('resolution', data=self.resolution)
             imgnames_encoded = common.str_to_numpy_ascii('\n'.join(self.imgrelpaths))
             create_dataset('imgrelpaths', data=imgnames_encoded)
             create_dataset('init_bboxes', data=self.init_bboxes)
             if self._groupings is not None:
                 create_dataset('groupings', data=self._groupings)
             if self.connected_subsystem is not None:
                 create_dataset('connected_subsystem', data=self._connected_subsystem)
@@ -263,20 +271,22 @@
   ## ------------------------------ matching ------------------------------- ##
     def dispatch_matchers(self, **kwargs):
         """
         run matching between overlapping tiles.
         """
         overwrite = kwargs.pop('overwrite', False)
         num_workers = kwargs.pop('num_workers', 1)
-        verbose = kwargs.pop('verbose', False)
         num_overlaps_per_job = kwargs.get('num_overlaps_per_job', 180) # 180 roughly number of overlaps in an MultiSEM mFoV
-        loader_config = kwargs.pop('loader_config', {})
+        loader_config = kwargs.pop('loader_config', {}).copy()
+        logger_info = kwargs.get('logger', None)
+        logger = logging.get_logger(logger_info)
         if bool(loader_config.get('cache_size', None)) and (num_workers > 1):
-            loader_config = loader_config.copy()
             loader_config['cache_size'] = int(np.ceil(loader_config['cache_size'] / num_workers))
+        if bool(loader_config.get('cache_capacity', None)) and (num_workers > 1):
+            loader_config['cache_capacity'] = loader_config['cache_capacity'] / num_workers
         loader_config['number_of_channels'] = 1 # only gray-scale matching are supported
         target_func = partial(Stitcher.subprocess_match_list_of_overlaps,
                               root_dir=self.imgrootdir, loader_config=loader_config,
                               **kwargs)
         if overwrite:
             self.matches = {}
             self.match_strains = {}
@@ -303,26 +313,25 @@
                 ovlp_g = overlaps[idx0:idx1] # global indices of overlaps
                 mapper, ovlp = np.unique(ovlp_g, return_inverse=True, axis=None)
                 ovlp = ovlp.reshape(ovlp_g.shape)
                 bboxes = self.init_bboxes[mapper]
                 imgpaths = [self.imgrelpaths[s] for s in mapper]
                 job = executor.submit(target_func, ovlp, imgpaths, bboxes, index_mapper=mapper)
                 jobs.append(job)
-            verbose_counter = 0
+            matched_counter = 0
             for job in as_completed(jobs):
                 matches, match_strains, ouch = job.result()
                 err_raised = err_raised or ouch
                 num_new_matches += len(matches)
                 self.matches.update(matches)
                 self.match_strains.update(match_strains)
-                if verbose:
-                    verbose_counter += len(matches)
-                    if verbose_counter > (len(overlaps)/10):
-                        print(f'\tmatching in progress: {num_new_matches}/{len(overlaps)}')
-                        verbose_counter = 0
+                matched_counter += len(matches)
+                if matched_counter > (len(overlaps)/10):
+                    logger.debug(f'matching in progress: {num_new_matches}/{len(overlaps)}')
+                    matched_counter = 0
         return num_new_matches, err_raised
 
 
     def find_overlaps(self):
         overlaps = []
         tree = index.Index(interleaved=True)
         for k, bbox in enumerate(self.init_bboxes):
@@ -376,17 +385,19 @@
         """
         root_dir = kwargs.get('root_dir', None)
         min_width = kwargs.get('min_overlap_width', 0)
         maskout_val = kwargs.get('maskout_val', None)
         index_mapper = kwargs.get('index_mapper', None)
         margin = kwargs.get('margin', 1.0)
         image_to_mask_path = kwargs.get('image_to_mask_path', None)
-        loader_config = kwargs.get('loader_config', {})
-        matcher_config = kwargs.get('matcher_config', {})
+        loader_config = kwargs.get('loader_config', {}).copy()
+        matcher_config = kwargs.get('matcher_config', {}).copy()
         instant_gc = kwargs.get('instant_gc', False)
+        logger_info = kwargs.get('logger', None)
+        logger = logging.get_logger(logger_info)
         margin_ratio_switch = 2
         err_raised = False
         if len(overlaps) == 0:
             return {}, {}, err_raised
         bboxes_overlap, wds = common.bbox_intersections(bboxes[overlaps[:,0]], bboxes[overlaps[:,1]])
         if 'cache_border_margin' not in loader_config:
             loader_config = loader_config.copy()
@@ -412,14 +423,15 @@
                                   'preprocess': None,
                                   'fillval': 1})
             mask_loader = StaticImageLoader(mask_paths, bboxes, root_dir=None, **loader_config)
         else:
             mask_exist = np.zeros(len(imgpaths), dtype=bool)
         matches = {}
         strains = {}
+        error_messages = []
         for indices, bbox_ov, wd in zip(overlaps, bboxes_overlap, wds):
             if wd <= min_width:
                 continue
             if margin < margin_ratio_switch:
                 real_margin = int(margin * wd)
             else:
                 real_margin = int(margin)
@@ -462,17 +474,21 @@
                 if index_mapper is not None:
                     idx0 = index_mapper[idx0]
                     idx1 = index_mapper[idx1]
                 matches[(idx0, idx1)] = (xy0, xy1, weight)
                 strains[(idx0, idx1)] = strain
             except Exception as err:
                 if not err_raised:
-                    print(image_loader.imgrootdir, err)
+                    error_messages.append(f'{image_loader.imgrootdir}: {err}')
                     err_raised = True
-                print(f'error: {image_loader.imgrelpaths[idx0]} <-> {image_loader.imgrelpaths[idx1]}')
+                error_messages.append(f'\t{image_loader.imgrelpaths[idx0]} <-> {image_loader.imgrelpaths[idx1]}')
+        if err_raised:
+            msg = '\n'.join(error_messages)
+            logger.error(msg)
+        image_loader.clear_cache()
         if instant_gc:
             gc.collect()
         return matches, strains, err_raised
 
 
   ## -------------------------- mesh relaxation ---------------------------- ##
     def initialize_meshes(self, mesh_sizes, **kwargs):
@@ -505,17 +521,17 @@
             cache_size: size of cache that save the intermediate results of
                 the meshes.
         """
         border_width = kwargs.get('border_width', None)
         interior_growth = kwargs.get('interior_growth', 3.0)
         match_soften = kwargs.get('match_soften', None)
         soft_top = kwargs.get('soft_top', 0.2)
-        soft_top_width = kwargs.get('soft_top_width', 0.1)
+        soft_top_width = kwargs.get('soft_top_width', 0.0)
         soft_left = kwargs.get('soft_left', 0.2)
-        soft_left_width = kwargs.get('soft_top_width', 0.0)
+        soft_left_width = kwargs.get('soft_left_width', 0.0)
         cache_size = kwargs.get('cache_size', None)
         groupings = self.groupings(normalize=True)
         if (not kwargs.get('force_update', False)) and (self.meshes is not None):
             return
         if (not hasattr(mesh_sizes, '__len__')) or (len(mesh_sizes) == 1) or (len(self.matches) == 0):
             tile_mesh_sizes = np.full(self.num_tiles, np.max(mesh_sizes))
         else:
@@ -594,15 +610,15 @@
             tile_soft_factors = soften_func(avg_strain)
         meshes = []
         mesh_indx = np.full(self.num_tiles, -1)
         mesh_params_ptr = {} # map the parameters of the mesh to
         if self._default_mesh_cache is None:
             default_caches = {}
             for gear in const.MESH_GEARS:
-                default_caches[gear] = defaultdict(lambda: common.CacheFIFO(maxlen=cache_size))
+                default_caches[gear] = defaultdict(lambda: caching.CacheFIFO(maxlen=cache_size))
             self._default_mesh_cache = default_caches
         else:
             default_caches = self._default_mesh_cache
         for k, tile_size in enumerate(self.tile_sizes):
             tmsz = tile_mesh_sizes[k]
             tbwd = tile_border_widths[k]
             tsf = tile_soft_factors[k]
@@ -741,25 +757,25 @@
         sel_uids, sel_match_uids = np.unique(match_uids, return_inverse=True)
         sel_match_uids = sel_match_uids.reshape(-1,2)
         sel_grps = groupings[sel_uids]
         sel_meshes = [self.meshes[s].copy(override_dict={'uid':k}) for k,s in enumerate(sel_uids)]
         if self._default_mesh_cache is None:
             default_caches = {}
             for gear in const.MESH_GEARS:
-                default_caches[gear] = defaultdict(lambda: common.CacheFIFO(maxlen=cache_size))
+                default_caches[gear] = defaultdict(lambda: caching.CacheFIFO(maxlen=cache_size))
             self._default_mesh_cache = default_caches
         else:
             default_caches = self._default_mesh_cache
         for M0 in sel_meshes:
             for gear in const.MESH_GEARS:
                 M0.set_default_cache(cache=default_caches[gear], gear=gear)
         opt = SLM(sel_meshes)
         for uids0, uids1 in zip(match_uids, sel_match_uids):
-            match = self.matches[tuple(uids0)]
-            xy0, xy1, weight = match
+            mtch = self.matches[tuple(uids0)]
+            xy0, xy1, weight = mtch
             opt.add_link_from_coordinates(uids1[0], uids1[1], xy0, xy1,
                 weight=weight, check_duplicates=False)
         cost = opt.optimize_linear(groupings=sel_grps, **kwargs)
         for g, m in zip(groupings, self.meshes):
             sel_idx = np.nonzero(sel_grps == g)[0]
             if sel_idx.size == 0:
                 continue
@@ -812,14 +828,15 @@
 
     def connect_isolated_subsystem(self, **kwargs):
         """
         translate blocks of tiles that are connected by links as a whole so that
         disconnected blocks roughly maintain the initial relative positions.
         """
         gear = (const.MESH_GEAR_INITIAL, const.MESH_GEAR_MOVING)
+        explode_factor = kwargs.get('explode_factor', 1.0)
         maxiter = kwargs.get('maxiter', None)
         tol = kwargs.get('tol', 1e-07)
         if self._optimizer is None:
             raise RuntimeError('optimizer of the stitcher not initialized.')
         Lbls, N_conn = self._optimizer.connected_subsystems
         self._connected_subsystem = Lbls
         if N_conn <= 1:
@@ -840,29 +857,29 @@
         v = np.append(v, 1)
         A = sparse.csr_matrix((v, (idx0, idx1)), shape=(Neq+1, N_conn))
         overlaps_u, overlaps_inverse = np.unique(overlaps, return_inverse=True)
         overlaps_inverse = overlaps_inverse.reshape(overlaps.shape)
         txy = np.array([self.meshes[s].estimate_translation(gear=gear) for s in overlaps_u])
         offset1 = txy[overlaps_inverse[:,0]] - txy[overlaps_inverse[:,1]]
         offset0 = self._init_offset[overlaps[:,0]] - self._init_offset[overlaps[:,1]]
-        bxy = np.append(offset0 - offset1, [[0, 0]], axis=0)
+        bxy = np.append(explode_factor * offset0 - offset1, [[0, 0]], axis=0)
         Tx = sparse.linalg.lsqr(A, bxy[:,0], atol=tol, btol=tol, iter_lim=maxiter)[0]
         Ty = sparse.linalg.lsqr(A, bxy[:,1], atol=tol, btol=tol, iter_lim=maxiter)[0]
         if np.any(Tx != 0) or np.any(Ty != 0):
             for m, lbl in zip(self.meshes, Lbls):
                 tx = Tx[lbl]
                 ty = Ty[lbl]
                 m.unlock()
                 m.apply_translation((tx, ty), gear[-1])
         # if still not fully connected, align average point
         A_blk = sparse.csr_matrix((np.ones_like(L_ov[:,0]), (L_ov[:,0], L_ov[:,1])), shape=(N_conn, N_conn))
         N_blk, L_blk = csgraph.connected_components(A_blk, directed=False, return_labels=True)
         if N_blk > 1:
             offset1 = np.array([m.estimate_translation(gear=gear) for m in self.meshes])
-            dxy = self._init_offset - offset1
+            dxy = explode_factor * (self._init_offset) - offset1
             Ls = L_blk[Lbls]
             for lbl in range(N_blk):
                 txy = np.mean(dxy[Ls == lbl], axis = 0)
                 for m, l in zip(self.meshes, Ls):
                     if l != lbl:
                         continue
                     m.unlock()
@@ -919,15 +936,15 @@
     def clear_mesh_cache(self, gear=None, instant_gc=True):
         if self._default_mesh_cache is not None:
             if gear is None:
                 for g in const.MESH_GEARS:
                     self.clear_mesh_cache(gear=g)
             else:
                 cache = self._default_mesh_cache[gear]
-                if isinstance(cache, common.CacheNull):
+                if isinstance(cache, caching.CacheNull):
                     cache.clear()
                 elif isinstance(cache, dict):
                     for c in cache.values():
                         c.clear()
         if instant_gc:
             gc.collect()
 
@@ -1012,15 +1029,16 @@
     Kwargs:
         loader_settings(dict): settings to initialize the image loader, refer to
             feabas.dal.AbstractImageLoade
         root_dir(str): if set, the paths in filepaths are relative path to this
             root directory.
     """
     def __init__(self, imgpaths, mesh_info, tile_sizes, **kwargs):
-        self._loader_settings = kwargs.get('loader_settings', {})
+        self.resolution = kwargs.get('resolution', DEFAULT_RESOLUTION)
+        self._loader_settings = kwargs.get('loader_settings', {}).copy()
         self._connected_subsystem = kwargs.get('connected_subsystem', None)
         if bool(kwargs.get('root_dir', None)):
             self.imgrootdir = kwargs['root_dir']
             self.imgrelpaths = imgpaths
         else:
             self.imgrootdir = os.path.dirname(os.path.commonprefix(imgpaths))
             self.imgrelpaths = [os.path.relpath(s, self.imgrootdir) for s in imgpaths]
@@ -1036,23 +1054,24 @@
     def from_stitcher(cls, stitcher, gear=(const.MESH_GEAR_INITIAL, const.MESH_GEAR_MOVING), **kwargs):
         if stitcher.meshes is None:
             raise RuntimeError('stitcher meshes not initializad.')
         root_dir = stitcher.imgrootdir
         imgpaths = stitcher.imgrelpaths
         tile_sizes = stitcher.tile_sizes
         connected_subsystem = stitcher.connected_subsystem
+        resolution = stitcher.resolution
         mesh_info = []
         for M in stitcher.meshes:
             v0 = M.vertices_w_offset(gear=gear[0])
             v1 = M.vertices(gear=gear[1])
             offset = M.offset(gear=gear[1])
             T = M.triangles
             mesh_info.append(Mesh_Info(v1, offset, T, v0))
         return cls(imgpaths, mesh_info, tile_sizes, root_dir=root_dir,
-                   connected_subsystem=connected_subsystem, **kwargs)
+                   connected_subsystem=connected_subsystem, resolution=resolution, **kwargs)
 
 
     @classmethod
     def from_h5(cls, fname, selected=None, gear=(const.MESH_GEAR_INITIAL, const.MESH_GEAR_MOVING), **kwargs):
         stitcher = Stitcher.from_h5(fname, load_matches=False, load_meshes=True, selected=selected)
         return cls.from_stitcher(stitcher, gear=gear, **kwargs)
 
@@ -1069,14 +1088,15 @@
                 tile_size = self._tile_sizes[selected]
             else:
                 tile_size = self._tile_sizes[0]
             args = [imgpaths, mesh_info, tile_size]
             kwargs = {}
             kwargs['root_dir'] = self.imgrootdir
             kwargs['loader_settings'] = self._loader_settings
+            kwargs['resolution'] = self.resolution
         return args, kwargs
 
 
     def clear_cache(self, instant_gc=False):
         self._interpolants = None
         self._rtree = None
         if self._image_loader is not None:
@@ -1233,28 +1253,37 @@
         else:
             img_out = image_hp
         img_out[weight_sum <= weight_eps] = fillval
         if np.issubdtype(dtype_out, np.integer):
             iinfo = np.iinfo(dtype_out)
             img_out = img_out.clip(iinfo.min, iinfo.max)
         img_out = img_out.astype(dtype_out, copy=False)
+        if np.all(img_out == fillval, axis=None):
+            return None
         return img_out
 
 
     def render_series_to_file(self, bboxes, filenames, **kwargs):
         rendered = {}
+        scale = kwargs.get('scale', 1.0)
+        if scale > 0.33:
+            self.image_loader._preprocess = None
+        else:
+            ksz = round(0.5/scale) * 2 - 1
+            self.image_loader._preprocess = partial(cv2.blur, ksize=(ksz, ksz))
         for bbox, filename in zip(bboxes, filenames):
             if os.path.isfile(filename):
                 rendered[filename] = bbox
                 continue
             imgt = self.crop(bbox, **kwargs)
             if imgt is None:
                 continue
             common.imwrite(filename, imgt)
             rendered[filename] = bbox
+        self.image_loader.clear_cache()
         return rendered
 
 
     def plan_render_series(self, tile_size, prefix='', **kwargs):
         """
         Return the output filenames and bboxes that cover the entire montage in
         z-order. Set pattern to provide filename formatting appended to the
```

### Comparing `feabas-0.1.1/feabas/visualization.py` & `feabas-1.0.0/feabas/visualization.py`

 * *Files identical despite different names*

