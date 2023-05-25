# Comparing `tmp/skeleton_plot-0.0.3.tar.gz` & `tmp/skeleton_plot-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/skeleton_plot-0.0.3.tar", last modified: Mon Apr 24 18:52:50 2023, max compression
+gzip compressed data, was "dist/skeleton_plot-0.0.5.tar", last modified: Thu May 25 22:09:31 2023, max compression
```

## Comparing `skeleton_plot-0.0.3.tar` & `skeleton_plot-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 emily.joyce   (502) staff       (20)        0 2023-04-24 18:52:50.671012 skeleton_plot-0.0.3/
--rw-r--r--   0 emily.joyce   (502) staff       (20)      394 2023-04-24 18:52:50.670531 skeleton_plot-0.0.3/PKG-INFO
--rw-r--r--   0 emily.joyce   (502) staff       (20)     1906 2023-04-04 22:53:25.000000 skeleton_plot-0.0.3/README.md
--rw-r--r--   0 emily.joyce   (502) staff       (20)       38 2023-04-24 18:52:50.671161 skeleton_plot-0.0.3/setup.cfg
--rw-r--r--   0 emily.joyce   (502) staff       (20)     1146 2023-03-24 18:48:35.000000 skeleton_plot-0.0.3/setup.py
-drwxr-xr-x   0 emily.joyce   (502) staff       (20)        0 2023-04-24 18:52:50.662082 skeleton_plot-0.0.3/skeleton_plot/
--rw-r--r--   0 emily.joyce   (502) staff       (20)       46 2023-02-17 18:19:45.000000 skeleton_plot-0.0.3/skeleton_plot/__init__.py
--rw-r--r--   0 emily.joyce   (502) staff       (20)    11096 2023-03-28 23:42:02.000000 skeleton_plot-0.0.3/skeleton_plot/plot_tools.py
--rw-r--r--   0 emily.joyce   (502) staff       (20)     4309 2023-03-30 18:17:26.000000 skeleton_plot-0.0.3/skeleton_plot/skel_io.py
--rw-r--r--   0 emily.joyce   (502) staff       (20)      998 2023-04-04 17:59:44.000000 skeleton_plot-0.0.3/skeleton_plot/utils.py
-drwxr-xr-x   0 emily.joyce   (502) staff       (20)        0 2023-04-24 18:52:50.669522 skeleton_plot-0.0.3/skeleton_plot.egg-info/
--rw-r--r--   0 emily.joyce   (502) staff       (20)      394 2023-04-24 18:52:50.000000 skeleton_plot-0.0.3/skeleton_plot.egg-info/PKG-INFO
--rw-r--r--   0 emily.joyce   (502) staff       (20)      304 2023-04-24 18:52:50.000000 skeleton_plot-0.0.3/skeleton_plot.egg-info/SOURCES.txt
--rw-r--r--   0 emily.joyce   (502) staff       (20)        1 2023-04-24 18:52:50.000000 skeleton_plot-0.0.3/skeleton_plot.egg-info/dependency_links.txt
--rw-r--r--   0 emily.joyce   (502) staff       (20)       67 2023-04-24 18:52:50.000000 skeleton_plot-0.0.3/skeleton_plot.egg-info/requires.txt
--rw-r--r--   0 emily.joyce   (502) staff       (20)       14 2023-04-24 18:52:50.000000 skeleton_plot-0.0.3/skeleton_plot.egg-info/top_level.txt
+drwxr-xr-x   0 emily.joyce   (502) staff       (20)        0 2023-05-25 22:09:31.458110 skeleton_plot-0.0.5/
+-rw-r--r--   0 emily.joyce   (502) staff       (20)      394 2023-05-25 22:09:31.455377 skeleton_plot-0.0.5/PKG-INFO
+-rw-r--r--   0 emily.joyce   (502) staff       (20)     1934 2023-05-11 20:53:34.000000 skeleton_plot-0.0.5/README.md
+-rw-r--r--   0 emily.joyce   (502) staff       (20)       38 2023-05-25 22:09:31.458479 skeleton_plot-0.0.5/setup.cfg
+-rw-r--r--   0 emily.joyce   (502) staff       (20)     1146 2023-05-11 20:53:50.000000 skeleton_plot-0.0.5/setup.py
+drwxr-xr-x   0 emily.joyce   (502) staff       (20)        0 2023-05-25 22:09:31.398989 skeleton_plot-0.0.5/skeleton_plot/
+-rw-r--r--   0 emily.joyce   (502) staff       (20)       46 2023-02-17 18:19:45.000000 skeleton_plot-0.0.5/skeleton_plot/__init__.py
+-rw-r--r--   0 emily.joyce   (502) staff       (20)    15606 2023-05-18 18:04:06.000000 skeleton_plot-0.0.5/skeleton_plot/plot_tools.py
+-rw-r--r--   0 emily.joyce   (502) staff       (20)     4295 2023-04-24 19:54:40.000000 skeleton_plot-0.0.5/skeleton_plot/skel_io.py
+-rw-r--r--   0 emily.joyce   (502) staff       (20)     1724 2023-05-18 16:53:22.000000 skeleton_plot-0.0.5/skeleton_plot/utils.py
+drwxr-xr-x   0 emily.joyce   (502) staff       (20)        0 2023-05-25 22:09:31.439164 skeleton_plot-0.0.5/skeleton_plot.egg-info/
+-rw-r--r--   0 emily.joyce   (502) staff       (20)      394 2023-05-25 22:09:29.000000 skeleton_plot-0.0.5/skeleton_plot.egg-info/PKG-INFO
+-rw-r--r--   0 emily.joyce   (502) staff       (20)      304 2023-05-25 22:09:30.000000 skeleton_plot-0.0.5/skeleton_plot.egg-info/SOURCES.txt
+-rw-r--r--   0 emily.joyce   (502) staff       (20)        1 2023-05-25 22:09:29.000000 skeleton_plot-0.0.5/skeleton_plot.egg-info/dependency_links.txt
+-rw-r--r--   0 emily.joyce   (502) staff       (20)       67 2023-05-25 22:09:29.000000 skeleton_plot-0.0.5/skeleton_plot.egg-info/requires.txt
+-rw-r--r--   0 emily.joyce   (502) staff       (20)       14 2023-05-25 22:09:29.000000 skeleton_plot-0.0.5/skeleton_plot.egg-info/top_level.txt
```

### Comparing `skeleton_plot-0.0.3/README.md` & `skeleton_plot-0.0.5/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -4,37 +4,37 @@
 
 Skeleton keys is a plotting tool for neuronal skeletons. 
 
 ## If you have an object with vertices and edges, or vertices and edges:
 use skeleton_plot.plot_tools.plot_verts. This is how the leftmost skeleton plot above was plotted:
 
 ```
-skelskeleton_plotplot.plot_tools.plot_verts(ax[0], vertices, edges,  
+skeleton_plot.plot_tools.plot_verts(vertices, edges,  ax = ax[0], 
     invert_y=True, line_width = 2.2, color = 'maroon', plot_soma = True)
 ```
 note: more arguments are available to be used with this function such as color and radius maps 
 
-## If you have an swc file that you want to plot:
+## If you have an meshparty skeleton that you want to plot:
 use skeleton_plot.plot_tools.plot_skel. This is how the skeleton plot above in the middle was generated:
 
 ```
-skeleton_plot.plot_tools.plot_skel(ax[1], sk,  pull_radius = True, 
+skeleton_plot.plot_tools.plot_skel(sk,  ax = ax[1], pull_radius = True, 
     pull_compartment_colors = True, invert_y=True, plot_soma = True, 
-    line_width = 3, color = 'darkslategray')
+    line_width = 3, color = 'darkslategray') 
 ``` 
 note: in order to use pull_radius argument, store the radius information in sk.vertex_properties['radius'] via 
 ```
 sk.vertex_properties['radius'] = **series with radius of each node of same length as sk.vertices**
 ```
 
-## If you have a meshwork:
+## If you have a meshparty meshwork:
 use skeleton_plot.plot_tools.plot_mw_skel. This is how the skeleton plot on the right was generated:
 
 ```
-skeleton_plot.plot_tools.plot_mw_skel(ax[2], mw, pull_radius = True,
+skeleton_plot.plot_tools.plot_mw_skel(mw, ax = ax[2], pull_radius = True,
     invert_y=True, line_width = 5, plot_soma = True,
     pull_compartment_colors = True, plot_presyn = True,
     plot_postsyn = True)
 ```
 note: in order to use pull_radius argument, you should have:
 - the appropriate root/soma location stored in mw.skeleton.root
 - basal dendrite labels stored in mw.anno[basal_table]
```

### Comparing `skeleton_plot-0.0.3/setup.py` & `skeleton_plot-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #     raise RuntimeError("Unable to find version string.")
 
 
 with open("requirements.txt", "r") as f:
     required = f.read().splitlines()
 
 setup(
-    version='0.0.3',
+    version='0.0.5',
     name="skeleton_plot",
     description="package for plotting skeletons",
     author="Emily Joyce, Forrest Collman, Casey Schneider-Mizell",
     author_email="emily.joyce@alleninstitute.org, forrestc@alleninstute.org,caseys@alleninstitute.org,",
     url="https://github.com/AllenInstitute/skeleton_plot",
     packages=find_packages(where="."),
     extras_require={"cloud": ["caveclient>=4.0.0", "cloudfiles"]},
```

### Comparing `skeleton_plot-0.0.3/skeleton_plot/plot_tools.py` & `skeleton_plot-0.0.5/skeleton_plot/plot_tools.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 import pandas as pd
 import numpy as np
 from meshparty import skeleton, meshwork
 from . import utils
+import matplotlib.pyplot as plt
 
 from matplotlib.collections import LineCollection
 
+axis_dict = {'x': 0, 'y': 1, 'z': 2}
 
-
-def plot_verts(ax, vertices, edges, radii = None, skeleton_colors = None, 
+def plot_verts(vertices, edges, radius = None, skel_colors = None, 
                 color = 'darkslategray', title = '', line_width = 1,
                 x = 'x', y = 'y',  plot_soma = False, soma_node = 0,
-                soma_size = 120, invert_y = False, 
+                soma_size = 120, skel_alpha = 1, invert_y = False, 
                 skel_color_map = {3: "firebrick", 4: "salmon", 2: "steelblue", 1: "olive"},
-                x_min_max = None, y_min_max = None, capstyle = 'round', joinstyle = 'round'
-                ):
+                x_min_max = None, y_min_max = None, capstyle = 'round', joinstyle = 'round',
+                ax = None):
     """plots skeleton vertices and edges with various options 
 
     Args:
-        ax (matplotlib.axes._subplots.AxesSubplot): axis on which to plot the skeleton
         vertices (np.array, nx2+): vertices to plot. nx2+. If nx3, possible to specify 
             which of the three axes are plotted in x and y arguments.
         edges (np.array, nx2): edges between specified vertices
-        radii (iterable, optional): radius of each vertex. Defaults to None.
-        line_width (int, optional): if no radii passed, line_width will be the width 
-            of every node in the plot. if radii are passed, those values will be 
+        radius (iterable, optional): radius of each vertex. Defaults to None.
+        line_width (int, optional): if no radius passed, line_width will be the width 
+            of every node in the plot. if radius are passed, those values will be 
             multiplied by line_width. Defaults to 1.
-        skeleton_colors (iterable, optional): map of numbers that indicate 
+        skel_colors (iterable, optional): map of numbers that indicate 
             color for each vertex recorded in skel_color_map. 
             Overwrites color argument. Defaults to None.
-        skel_color_map (dict, optional): map of skeleton_colors values->colors. 
+        skel_color_map (dict, optional): map of skel_colors values->colors. 
             Defaults to {3: "firebrick", 4: "salmon", 2: "steelblue", 1: "olive"}.
         color (str, optional): color of all vertices. Defaults to 'darkslategray'.
         title (str, optional): title to display on plot. Defaults to ''.
         x (str, optional): which dimension to plot in x. x y or z. Defaults to 'x'.
         y (str, optional): which dimension to plot in y. x y or z. Defaults to 'y'.
         plot_soma (bool, optional): whether or not to plot the soma. Defaults to False.
         soma_node (int, optional): which node in the skeleton represents the soma. 
@@ -44,180 +44,266 @@
         x_min_max (tuple, optional): manually specified x min and x max. 
             Defaults to None, which will set x min and max to the limits of the vertices.
         y_min_max (tuple, optional): manually specified y min and x max. 
             Defaults to None, which will set y min and max to the limits of the vertices.
         capstyle (str, optional): shape of the endpoints. Defaults to 'round'.
         joinstyle (str, optional): shape of the points between linecollection pieces. 
             Defaults to 'round'.
+        ax (matplotlib.axes._subplots.AxesSubplot, optional): axis on which to plot the skeleton.
+            If none is given, will find current axis with plt.gca()
 
     """    
     
-    
+    if ax is None:
+        ax = plt.gca()
 
 
-    sk=skeleton.Skeleton(vertices, edges, vertex_properties={'radius':pd.Series(radii), 
-                                            'compartment':pd.Series(skeleton_colors)}, root=soma_node,
+    sk=skeleton.Skeleton(vertices, edges, vertex_properties={'radius':pd.Series(radius), 
+                                            'compartment':pd.Series(skel_colors)}, root=soma_node,
                                             remove_zero_length_edges=False)
 
-    if skeleton_colors is not None: 
-        if len(skeleton_colors) != len(vertices):
-            raise ValueError('length of skeleton_colors must match len of vertices')
-    if radii is not None:
-        if len(radii) != len(vertices):
-            raise ValueError('length of radii must match len of vertices')
-
-    if invert_y:    
-        ax.invert_yaxis()
+    if skel_colors is not None: 
+        if len(skel_colors) != len(vertices):
+            raise ValueError('length of skel_colors must match len of vertices')
+    if radius is not None:
+        if len(radius) != len(vertices):
+            raise ValueError('length of radius must match len of vertices')
 
-    axis_dict = {'x': 0, 'y': 1, 'z': 2}
     x, y = axis_dict[x], axis_dict[y]
 
     for cover_path in sk.cover_paths_with_parent():
         
-        if skeleton_colors is None:
+        if skel_colors is None:
             colors = [color]*len(cover_path)
         else:
             colors = [skel_color_map[x] for x in sk.vertex_properties['compartment'][cover_path].values]
-        if radii is None:
+        if radius is None:
             linewidths  = pd.Series([line_width]*len(cover_path))
         else:
             linewidths = (sk.vertex_properties['radius'][cover_path])*line_width
 
         path_verts = sk.vertices[cover_path][:,[x, y]]
 
         segments = np.concatenate([path_verts[:-1], path_verts[0:-1], path_verts[1:]], axis=1).reshape(len(path_verts)-1,3,2)
-        lc = LineCollection(segments, linewidths=linewidths, color=colors, capstyle = capstyle, joinstyle = joinstyle)
+        lc = LineCollection(segments, linewidths=linewidths, color=colors, capstyle = capstyle, joinstyle = joinstyle, 
+                                    alpha = skel_alpha)
         ax.add_collection(lc)
 
     ax.set_aspect("equal")
 
     if plot_soma:
-        if skeleton_colors is not None:
+        if skel_colors is not None:
             soma_color = skel_color_map[1]
         else:
             soma_color = color
-        print(sk.root_position[x], sk.root_position[y])
         ax.scatter(sk.root_position[x], sk.root_position[y], s = soma_size, c = soma_color, zorder = 2)
 
-    if x_min_max:
-        ax.set_xlim(x_min_max[0], x_min_max[1])
-    if x_min_max and invert_y:
-        ax.set_ylim(y_min_max[1], y_min_max[0])
-    elif x_min_max:
-        ax.set_ylim(y_min_max[0], y_min_max[1])
-    elif x_min_max is None and y_min_max is None:
-        verts = sk.vertices
-        if invert_y:
-            ax.set_ylim(max(verts[:,y]), min(verts[:,y]))
-        else:
-            ax.set_ylim(min(verts[:,y]), max(verts[:,y]))
-        ax.set_xlim(min(verts[:,x]), max(verts[:,x]))
-
+    
+    utils.set_xy_lims(ax, verts = sk.vertices, invert_y = invert_y, 
+                x_min_max = x_min_max, y_min_max = y_min_max, x = x, y = y)
     
     ax.set_title(title)
+
+
         
 
-def plot_skel(ax, sk: skeleton, title='', x = 'x', y = 'y', pull_radius = False, radii = None, 
-                    line_width = 1, plot_soma = False, soma_size = 120, soma_node = 0, 
-                    invert_y = False, skeleton_colors = None, 
+def plot_skel(sk: skeleton, title='', x = 'x', y = 'y', pull_radius = False, radius = None, 
+                    line_width = 1, plot_soma = False, soma_size = 120, soma_node = None, 
+                    invert_y = False, skel_colors = None, skel_alpha = 1,
                     pull_compartment_colors = False, color = 'darkslategray',
                     skel_color_map = {3: "firebrick", 4: "salmon", 2: "steelblue", 1: "olive"},
-                    x_min_max = None, y_min_max = None, capstyle = 'round', joinstyle = 'round'):
+                    x_min_max = None, y_min_max = None, capstyle = 'round', joinstyle = 'round',
+                    ax = None):
     """plots a skeleton object. attempts to pull out arguments from skeleton and plot with plot_verts
 
     Args:
-        ax (matplotlib.axes): axis on which to plot the skeleton
         sk (skeleton): (meshparty.skeleton.Skeleton): skeleton to be plotted 
         title (str, optional): title to display on plot. Defaults to ''.
         x (str, optional): which dimension to plot in x. x y or z. Defaults to 'x'.
         y (str, optional): which dimension to plot in y. x y or z. Defaults to 'y'.
         pull_radius (bool, optional): whether or not to pull and plot the radius from 
             sk.vertex_properties['radius']. Defaults to False.
-        radii (iterable, optional): radius of each vertex. overwritten if pull_radius.
+        radius (iterable, optional): radius of each vertex. overwritten if pull_radius.
             Defaults to None.
         plot_soma (bool, optional): whether or not to plot the soma. Defaults to False.
         soma_size (int, optional): size of soma node to display. Defaults to 120.
         soma_node (int, optional): the index of the soma node in sk.vertices. Defaults to 0.
         invert_y (bool, optional): whether or not to invert the y axis. Defaults to False.
         pull_compartment_colors (bool, optional): whether to pull and plot the compartments in 
             sk.vertex_properties['compartment']. Defaults to False.
-        skeleton_colors (iterable, optional): map of numbers that indicate 
+        skel_colors (iterable, optional): map of numbers that indicate 
             color for each vertex recorded in skel_color_map. 
             Overwrites color argument. Defaults to None.
-        skel_color_map (dict, optional): map of skeleton_colors values->colors. 
+        skel_color_map (dict, optional): map of skel_colors values->colors. 
             Defaults to {3: "firebrick", 4: "salmon", 2: "steelblue", 1: "olive"}.
         color (str, optional): color of all vertices. Defaults to 'darkslategray'.
         x_min_max (tuple, optional): manually specified x min and x max. 
             Defaults to None, which will set x min and max to the limits of the vertices.
         y_min_max (tuple, optional): manually specified y min and x max. 
             Defaults to None, which will set y min and max to the limits of the vertices.
         capstyle (str, optional): shape of the endpoints. Defaults to 'round'.
         joinstyle (str, optional): shape of the points between linecollection pieces. 
             Defaults to 'round'.
+        ax (matplotlib.axes, optional): axis on which to plot the skeleton
+            If none is given, will find current axis with plt.gca()
     """    
-    
+    if ax is None:
+        ax = plt.gca()
 
-    if skeleton_colors is None:
+    if skel_colors is None:
         if pull_compartment_colors:
-            skeleton_colors = sk.vertex_properties['compartment']
+            skel_colors = sk.vertex_properties['compartment']
 
     if pull_radius:
-        radii = sk.vertex_properties['radius']
+        radius = sk.vertex_properties['radius']
     else:
-        radii = None
+        radius = None
+    
+    if soma_node is None:
+        soma_node = int(sk.root)
 
-    plot_verts(ax, sk.vertices, sk.edges, radii = radii, 
-                skeleton_colors = skeleton_colors, title = title, 
+    plot_verts(sk.vertices, sk.edges, ax = ax, radius = radius, 
+                skel_colors = skel_colors, title = title, skel_alpha = skel_alpha,
                 line_width = line_width, x = x, y = y,  plot_soma = plot_soma, soma_node = soma_node,
                 color = color, soma_size = soma_size, invert_y = invert_y, 
                 skel_color_map = skel_color_map, x_min_max = x_min_max, 
                 y_min_max = y_min_max, capstyle = capstyle, joinstyle = joinstyle
                 )
 
-def plot_mw_skel(ax, mw: meshwork, plot_presyn = False, plot_postsyn = False, presyn_color = 'deepskyblue', 
-                    postsyn_color = 'violet', presyn_size = 5, postsyn_size = 5, presyn_alpha = 1, postsyn_alpha = 1,
-                    title='', line_width = 1, x = 'x', y = 'y', radii = None, pull_radius = False, 
+def plot_mw_skel(mw: meshwork, plot_presyn = False, plot_postsyn = False, presyn_color = 'deepskyblue', 
+                    postsyn_color = 'violet', presyn_size = 5, postsyn_size = 5, syn_res = [4,4,40],
+                    presyn_alpha = 1, postsyn_alpha = 1, skel_alpha = 1,
+                    title='', line_width = 1, x = 'x', y = 'y', radius = None, pull_radius = False, 
                     radius_anno = 'segment_properties', basal_anno = 'basal_mesh_labels', apical_anno = 'apical_mesh_labels', 
                     axon_anno = 'is_axon', plot_soma = False, soma_node = None, soma_size = 120, 
                     invert_y = False, skel_colors = None, pull_compartment_colors = False,  color = 'darkslategray',
                     skel_color_map = {3: "firebrick", 4: "salmon", 2: "steelblue", 1: "olive"},
                     x_min_max = None, y_min_max = None, capstyle = 'round', joinstyle = 'round',
-                    ):
+                    pre_anno = {'pre_syn': 'pre_pt_position'}, post_anno = {'post_syn': 'post_pt_position'},
+                    ax = None):
+
+    if ax is None:
+        ax = plt.gca()
 
     # pull out radius, compartments, soma node
     if skel_colors is None:
         if pull_compartment_colors:
             skel_colors = utils.pull_mw_skel_colors(mw, basal_anno, apical_anno, axon_anno)
 
     
-    if radii is None:
+    if radius is None:
         if pull_radius:
-            radii = utils.pull_mw_rad(mw, radius_anno)
+            radius = utils.pull_mw_rad(mw, radius_anno)
 
 
     sk = mw.skeleton
 
-    if plot_soma and soma_node is None:
+    if soma_node is None:
         soma_node = sk.root
 
+    # add synapses
+
+    if plot_presyn:
+        pre_anno_table = list(pre_anno.keys())[0]
+        pre_column = list(pre_anno.values())[0]
+        presyn_verts = np.array([np.array(x) for x in (mw.anno[pre_anno_table][pre_column]).values])*syn_res
+
+    if plot_postsyn:
+        post_anno_table = list(post_anno.keys())[0]
+        post_column = list(post_anno.values())[0]
+        postsyn_verts = np.array([np.array(x) for x in (mw.anno[post_anno_table][post_column]).values])*syn_res
+
+    plot_synapses(presyn_verts = presyn_verts, postsyn_verts = postsyn_verts, x = x, y = y, presyn_size = presyn_size, 
+                    postsyn_size = postsyn_size, presyn_color = presyn_color, postsyn_color = postsyn_color, 
+                    presyn_alpha = presyn_alpha, postsyn_alpha = postsyn_alpha, ax = ax)
     
-    # use that information to plot verts 
-    plot_verts(ax, sk.vertices, sk.edges, radii = radii,
-                skeleton_colors = skel_colors, title = title, 
+    # plot verts 
+    plot_verts(sk.vertices, sk.edges, ax = ax, radius = radius,
+                skel_colors = skel_colors, title = title, skel_alpha = skel_alpha,
                 line_width = line_width, x = x, y = y,  plot_soma = plot_soma, soma_node = soma_node,
                 color = color, soma_size = soma_size, invert_y = invert_y, 
                 skel_color_map = skel_color_map, x_min_max = x_min_max, 
-                y_min_max = y_min_max, capstyle = capstyle, joinstyle = joinstyle
+                y_min_max = y_min_max, capstyle = capstyle, joinstyle = joinstyle,
                 )
 
-    # add synapses
-    if plot_presyn:
-        presyns = np.array([np.array(x) for x in (mw.anno.pre_syn['pre_pt_position']).values])
-        ax.scatter(presyns[:,0]*4, presyns[:,1]*4, s = presyn_size, c = presyn_color, alpha = presyn_alpha)
-    if plot_postsyn:
-        postsyns = np.array([np.array(x) for x in (mw.anno.post_syn['post_pt_position']).values])
-        ax.scatter(postsyns[:,0]*4, postsyns[:,1]*4, s = postsyn_size, c = postsyn_color, alpha = postsyn_alpha)
+def plot_synapses(presyn_verts = None, postsyn_verts = None, x = 'x', y = 'y', 
+                    presyn_size = 5, postsyn_size = 5, presyn_color = 'deepskyblue', 
+                    postsyn_color = 'violet', presyn_alpha = 1, postsyn_alpha = 1,
+                    x_min_max = None, y_min_max = None, title=None, invert_y = False, 
+                    ax = None
+                    ):
+    """plots presynaptic and postsynaptic sites on ax
 
+    Args:
+        presyn_verts (array, optional): vertices for each presyn point to be plotted. 
+            Defaults to None.
+        postsyn_verts (array, optional): vertices for each presyn point to be plotted. 
+            Defaults to None.
+        x (str, optional): which dimension to plot in x. x y or z. Defaults to 'x'.
+        y (str, optional): which dimension to plot in y. x y or z. Defaults to 'y'.
+        presyn_size (int or array, optional): size(s) for presynaptic points. 
+            Defaults to 5.
+        postsyn_size (int or array, optional): size(s) for postsynaptic points.  
+            Defaults to 5.
+        presyn_color (str, optional): color for presynaptic points. 
+            Defaults to 'deepskyblue'.
+        postsyn_color (str, optional): color for postsynaptic points. 
+            Defaults to 'violet'.
+        presyn_alpha (int, optional): opacity for presynaptic points. 
+            between 0(transparent) and 1(opaque). Defaults to 1.
+        postsyn_alpha (int, optional): opacity for presynaptic points. 
+            between 0(transparent) and 1(opaque). Defaults to 1.
+        x_min_max (tuple, optional): manually specified x min and x max. 
+            Defaults to None, which will set x min and max to the limits of the vertices.
+        y_min_max (tuple, optional): manually specified y min and x max. 
+            Defaults to None, which will set y min and max to the limits of the vertices.
+        title (str, optional): title to display on plot. Defaults to ''.
+        ax (matplotlib.axes, optional): axis on which to plot the skeleton
+            If none is given, will find current axis with plt.gca()
+    """   
+    x, y = axis_dict[x], axis_dict[y]
+
+    if presyn_verts is not None:
+        ax.scatter(presyn_verts[:,x], presyn_verts[:,y], s = presyn_size, c = presyn_color, alpha = presyn_alpha)
+    if postsyn_verts is not None:
+        ax.scatter(postsyn_verts[:,x], postsyn_verts[:,y], s = postsyn_size, c = postsyn_color, alpha = postsyn_alpha)
+
+    utils.set_xy_lims(ax, verts = np.vstack((presyn_verts, postsyn_verts)), invert_y = invert_y, 
+            x_min_max = x_min_max, y_min_max = y_min_max, x = x, y = y)
 
 
+def plot_layer_lines(y_vals, ax = None, labels = None, buffer_space = .01, line_styles = None):
+    """    
+    takes a list of y values on which to plot horizontal line across the current x ax.
+    Optionally, labels can be provided to label each line.
+
+    Args:
+        y_vals (list): y value for each line you wish to plot 
+        ax (matplotlib.axes, optional): axis on which to plot the skeleton
+            If none is given, will find current axis with plt.gca()
+        labels (list, optional): list of str labels for each line. Defaults to None.
+        buffer_space (float, optional): percentage of the x range of the plot to  
+            have as a buffer between the edge of the plot to the layer labels.
+            Defaults to .01.
+    """
+    
+    if ax is None:
+        plt.gca()
+    # get x vals
+    x_vals = ax.get_xlim()
+
+    if labels is None:
+        labels = ['']*len(y_vals)
+
+    if line_styles is None:
+        line_styles = [{}]*len(y_vals)
+    elif isinstance(line_styles, dict):
+        line_styles = [line_styles] * len(y_vals)
+
+    for y_val, label, style in zip(y_vals, labels, line_styles):
+        ax.plot([x_vals[0], x_vals[1]], [y_val, y_val], **style)
+        # add a buffer space between plot and labels
+        buffer = buffer_space * (x_vals[1] - x_vals[0])
+        ax.text(x_vals[1] + buffer, y_val, label, verticalalignment='center')
+
```

### Comparing `skeleton_plot-0.0.3/skeleton_plot/skel_io.py` & `skeleton_plot-0.0.5/skeleton_plot/skel_io.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,40 +12,40 @@
 SWC_COLUMNS = ('id', 'type', 'x', 'y', 'z', 'radius', 'parent',)
 COLUMN_CASTS = {
     'id': int,
     'parent': int,
     'type': int
 }
 
-def read_depths(directory, filename):
+def read_json(directory, filename):
     '''
-    enter cloudpath location of layer depths .json file, returns dict
+    enter cloudpath location of json file(i.e. layer depths .json file), returns dict
     of that layer containing vertices
     
     Parameters
     ----------
-    directory (str): directory location of layer file. in cloudpath format as seen in https://github.com/seung-lab/cloud-files
+    directory (str): directory location of json file. in cloudpath format as seen in https://github.com/seung-lab/cloud-files
     filename (str): full json filename 
 
     Returns:
     layer_bounds (list(dict)): list of dicts with values being the layer name, values containing the (x,y) vertices of the layer (among other things)
     ''' 
     if cf_imported == False:
         raise ImportError('cannot use read_depths without cloudfiles.Install https://github.com/seung-lab/cloud-files to continue')
 
     cf = CloudFiles(directory)
-    depths = cf.get_json(filename)
+    js = cf.get_json(filename)
 
-    if depths is None:
+    if js is None:
         if filename not in list(cf):
             raise FileNotFoundError(f"filename '{filename}' not found in '{directory}'")
         else:
             raise ValueError('unable to retrieve file')
 
-    return cf.get_json(filename)
+    return js
 
 # will be moved to meshparty?
 def read_skeleton(directory, filename):
     """reads skeleton file from cloudfiles style path
 
     Args:
     directory (str): directory location of swc skeleton file. in cloudpath format as seen in https://github.com/seung-lab/cloud-files
```

