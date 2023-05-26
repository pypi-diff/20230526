# Comparing `tmp/mazemdp-0.7.3.tar.gz` & `tmp/mazemdp-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mazemdp-0.7.3.tar", last modified: Sat Nov 12 09:53:57 2022, max compression
+gzip compressed data, was "mazemdp-0.8.0.tar", last modified: Thu Mar 23 08:00:18 2023, max compression
```

## Comparing `mazemdp-0.7.3.tar` & `mazemdp-0.8.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 09:53:57.491585 mazemdp-0.7.3/
--rwxr-xr-x   0 runner    (1001) docker     (121)      161 2022-11-12 09:53:45.000000 mazemdp-0.7.3/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 09:53:57.483585 mazemdp-0.7.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 09:53:57.487585 mazemdp-0.7.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1091 2022-11-12 09:53:45.000000 mazemdp-0.7.3/.github/workflows/python-publish.yml
--rwxr-xr-x   0 runner    (1001) docker     (121)     1862 2022-11-12 09:53:45.000000 mazemdp-0.7.3/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (121)     1071 2022-11-12 09:53:45.000000 mazemdp-0.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-11-12 09:53:45.000000 mazemdp-0.7.3/MANIFEST.in
--rwxr-xr-x   0 runner    (1001) docker     (121)     1366 2022-11-12 09:53:45.000000 mazemdp-0.7.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     4514 2022-11-12 09:53:57.491585 mazemdp-0.7.3/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (121)     4212 2022-11-12 09:53:45.000000 mazemdp-0.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 09:53:57.487585 mazemdp-0.7.3/mazemdp/
--rwxr-xr-x   0 runner    (1001) docker     (121)      181 2022-11-12 09:53:45.000000 mazemdp-0.7.3/mazemdp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-11-12 09:53:57.000000 mazemdp-0.7.3/mazemdp/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      865 2022-11-12 09:53:45.000000 mazemdp-0.7.3/mazemdp/chrono.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    10582 2022-11-12 09:53:45.000000 mazemdp-0.7.3/mazemdp/maze.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    16141 2022-11-12 09:53:45.000000 mazemdp-0.7.3/mazemdp/maze_plotter.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4273 2022-11-12 09:53:45.000000 mazemdp-0.7.3/mazemdp/mdp.py
--rw-r--r--   0 runner    (1001) docker     (121)      764 2022-11-12 09:53:45.000000 mazemdp-0.7.3/mazemdp/simple_action_space.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3268 2022-11-12 09:53:45.000000 mazemdp-0.7.3/mazemdp/toolbox.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 09:53:57.491585 mazemdp-0.7.3/mazemdp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4514 2022-11-12 09:53:57.000000 mazemdp-0.7.3/mazemdp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      485 2022-11-12 09:53:57.000000 mazemdp-0.7.3/mazemdp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-12 09:53:57.000000 mazemdp-0.7.3/mazemdp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-11-12 09:53:57.000000 mazemdp-0.7.3/mazemdp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-11-12 09:53:57.000000 mazemdp-0.7.3/mazemdp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-11-12 09:53:45.000000 mazemdp-0.7.3/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (121)      477 2022-11-12 09:53:57.491585 mazemdp-0.7.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)      793 2022-11-12 09:53:45.000000 mazemdp-0.7.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 09:53:57.491585 mazemdp-0.7.3/tests/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 09:53:45.000000 mazemdp-0.7.3/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1627 2022-11-12 09:53:45.000000 mazemdp-0.7.3/tests/test_mdp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:00:18.124658 mazemdp-0.8.0/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      161 2023-03-23 08:00:03.000000 mazemdp-0.8.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:00:18.120658 mazemdp-0.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:00:18.120658 mazemdp-0.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-03-23 08:00:03.000000 mazemdp-0.8.0/.github/workflows/python-publish.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1862 2023-03-23 08:00:03.000000 mazemdp-0.8.0/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1071 2023-03-23 08:00:03.000000 mazemdp-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-23 08:00:03.000000 mazemdp-0.8.0/MANIFEST.in
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1366 2023-03-23 08:00:03.000000 mazemdp-0.8.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-03-23 08:00:18.124658 mazemdp-0.8.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4212 2023-03-23 08:00:03.000000 mazemdp-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:00:18.124658 mazemdp-0.8.0/mazemdp/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      227 2023-03-23 08:00:03.000000 mazemdp-0.8.0/mazemdp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-23 08:00:18.000000 mazemdp-0.8.0/mazemdp/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-03-23 08:00:03.000000 mazemdp-0.8.0/mazemdp/chrono.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10837 2023-03-23 08:00:03.000000 mazemdp-0.8.0/mazemdp/maze.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16128 2023-03-23 08:00:03.000000 mazemdp-0.8.0/mazemdp/maze_plotter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4273 2023-03-23 08:00:03.000000 mazemdp-0.8.0/mazemdp/mdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-03-23 08:00:03.000000 mazemdp-0.8.0/mazemdp/simple_action_space.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3268 2023-03-23 08:00:03.000000 mazemdp-0.8.0/mazemdp/toolbox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:00:18.124658 mazemdp-0.8.0/mazemdp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-03-23 08:00:18.000000 mazemdp-0.8.0/mazemdp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-03-23 08:00:18.000000 mazemdp-0.8.0/mazemdp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 08:00:18.000000 mazemdp-0.8.0/mazemdp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-23 08:00:18.000000 mazemdp-0.8.0/mazemdp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-23 08:00:18.000000 mazemdp-0.8.0/mazemdp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-03-23 08:00:03.000000 mazemdp-0.8.0/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       51 2023-03-23 08:00:03.000000 mazemdp-0.8.0/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      579 2023-03-23 08:00:18.124658 mazemdp-0.8.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      793 2023-03-23 08:00:03.000000 mazemdp-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:00:18.124658 mazemdp-0.8.0/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:00:03.000000 mazemdp-0.8.0/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1654 2023-03-23 08:00:03.000000 mazemdp-0.8.0/tests/test_mdp.py
```

### Comparing `mazemdp-0.7.3/.github/workflows/python-publish.yml` & `mazemdp-0.8.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `mazemdp-0.7.3/.gitignore` & `mazemdp-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mazemdp-0.7.3/LICENSE` & `mazemdp-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mazemdp-0.7.3/Makefile` & `mazemdp-0.8.0/Makefile`

 * *Files identical despite different names*

### Comparing `mazemdp-0.7.3/PKG-INFO` & `mazemdp-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: mazemdp
-Version: 0.7.3
+Version: 0.8.0
 Summary: An simple maze to test dynamic programming and tabular reinforcement learning algorithms
 Home-page: https://github.com/osigaud/SimpleMazeMDP
 Author: Olivier Sigaud
 Author-email: Olivier.Sigaud@isir.upmc.fr
 License: MIT
+Description-Content-Type: text/markdown; charset=UTF-8
 License-File: LICENSE
 
 # SimpleMazeMDP: 
 
 This repository contains code to provide a simple Maze environment used as example MDP for tabular dynamic programming and reinforcement learning labs.
 
 If you want to do the corresponding labs, you need a Google account. Then you can copy-paste the [dynamic programming colab](https://colab.research.google.com/drive/1FpI-h_q-Iq3hBnmRjRUUwhDDK7TtQEVz) and the [reinforcement learning colab](https://colab.research.google.com/drive/1o4TnFGwgeN1e1DBrLRANj7Rj1_MTIkDJ).
```

### Comparing `mazemdp-0.7.3/README.md` & `mazemdp-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `mazemdp-0.7.3/mazemdp/chrono.py` & `mazemdp-0.8.0/mazemdp/chrono.py`

 * *Files identical despite different names*

### Comparing `mazemdp-0.7.3/mazemdp/maze.py` & `mazemdp-0.8.0/mazemdp/maze.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Author: Olivier Sigaud
 """
 
+from functools import cached_property
 import random
-import gym
 
 import numpy as np
 
 from mazemdp.maze_plotter import MazePlotter  # used to plot the maze
 from mazemdp.mdp import Mdp
 from mazemdp.toolbox import E, N, S, W
 
@@ -43,17 +43,16 @@
 
 
 def build_maze(width, height, walls, hit=False):
     ts = height * width - 1 - len(walls)
     maze = Maze(
         width, height, hit, walls=walls, last_states=[ts]
     )  # Markov Decision Process definition
-
-    # The MDP has one state more than the Maze (the final state
-    # outside of the maze)
+    # The MDP has one state more than the Maze
+    # (the final state is outside of the maze)
     return maze.mdp, maze.nb_states + 1, maze.coord_x, maze.coord_y
 
 
 def create_random_maze(width, height, ratio, hit=False):
     size = width * height
     n_walls = round(ratio * size)
 
@@ -119,15 +118,15 @@
         self.state_height = []
         self.coord_x = np.zeros(height * width - len(walls) + 1)
         self.coord_y = np.zeros(height * width - len(walls) + 1)
         # ##################### State Space ######################
         self.init_states(width, height, walls)
 
         # ##################### Action Space ######################
-        self.action_space = gym.spaces.Discrete(4)
+        self.nb_actions = nb_actions
 
         # ##################### Distribution Over Initial States ######################
 
         start_distribution = np.zeros(
             self.nb_states
         )  # distribution over initial states
 
@@ -153,14 +152,20 @@
             reward_matrix,
             plotter,
             gamma=self.gamma,
             terminal_states=[self.nb_states],
             timeout=timeout,
         )
 
+    @cached_property
+    def action_space(self):
+        """Legacy method to get the action space"""
+        import gym
+        return gym.spaces.Discrete(self.nb_actions)
+
     def init_states(self, width, height, walls):
         state = 0
         cell = 0
         for i in range(width):
             for j in range(height):
                 if cell not in walls:
                     self.cells[i][j] = state
@@ -268,7 +273,11 @@
                     # Reward Matrix when going west
                     if (
                         i == 0 or self.cells[i - 1][j] == -1
                     ):  # cells on the right + right side of a wall
                         reward_matrix[state, W] = -0.5
 
         return reward_matrix
+
+
+if __name__ == "__main__":
+    m = create_random_maze(3, 3, 0.0)
```

### Comparing `mazemdp-0.7.3/mazemdp/maze_plotter.py` & `mazemdp-0.8.0/mazemdp/maze_plotter.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,35 +10,37 @@
 
 try:
     import cv2
 except ImportError:
     cv2 = None
 import matplotlib
 
-# Force backend
-if os.environ.get("PLOT_BACKEND"):
-    matplotlib.use(os.environ.get("PLOT_BACKEND"))
-print(f"Matplotlib backend: {matplotlib.get_backend()}")
 import base64
 from pathlib import Path
 
 import matplotlib.patches as mpatches
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib.table import Table
 
 from mazemdp.toolbox import E, N, S, W
 
 try:
     shell = get_ipython().__class__.__module__  # noqa: F401
-    if shell is not None and shell in ['ipykernel.zmqshell', 'google.colab._shell']:
+    if shell is not None and shell in ["ipykernel.zmqshell", "google.colab._shell"]:
         os.environ["WEB_NOTEBOOK"] = shell
 except NameError:
     pass
 
+
+# Force backend
+if os.environ.get("PLOT_BACKEND"):
+    matplotlib.use(os.environ.get("PLOT_BACKEND"))
+print(f"Matplotlib backend: {matplotlib.get_backend()}")
+
 # ------------------- plot functions for a maze like environment ----------------#
 
 
 def show_videos(video_path: str = "", prefix: str = "") -> None:
     """
     Taken from https://github.com/eleurent/highway-env
 
@@ -48,15 +50,17 @@
     from IPython import display as ipythondisplay
 
     html = []
 
     for avi in Path(video_path).glob(f"{prefix}*.avi"):
         mp4_video = str(avi).replace("avi", "mp4")
         # Convert
-        if not os.path.isfile(mp4_video) or os.path.getmtime(mp4_video) < os.path.getmtime(avi):
+        if not os.path.isfile(mp4_video) or os.path.getmtime(
+            mp4_video
+        ) < os.path.getmtime(avi):
             print(f"Converting {avi}")
             os.system(f"ffmpeg -y -i {avi} -c:v libx264 -crf 19 {mp4_video}")
 
     for mp4 in Path(video_path).glob(f"{prefix}*.mp4"):
         video_b64 = base64.b64encode(mp4.read_bytes())
         html.append(
             """<video alt="{}" autoplay
@@ -112,40 +116,38 @@
     else:
         return [x, y]
 
 
 # -------------------------------------------------------------------------------#
 
 
-
 @dataclass
 class Plot:
     canvas: FigureCanvasAgg
     fig: Figure
     axes: Axes
     table: Table
     patch: Any
 
 
-
 class MazePlotter:
     """
     maze_mdp plot, used to plot the agent in its environment while processing the V/Q function and policy
     it can also create videos given a list of V/Q values and a list of policies
     """
 
     def __init__(
         self, maze, using_notebook=bool(os.environ.get("WEB_NOTEBOOK", False))
     ):  # maze defined in the mdp notebook
         self.maze_attr = maze
         self.terminal_states = maze.last_states
         self.using_notebook = using_notebook
         self.figW = self.maze_attr.width
         self.figH = self.maze_attr.height
-        
+
         self.plot_history: List[Plot] = []
 
         self.image_idx = 0
         self.video_writer = None
         self.video_name = ""
         self.video_folder = "videos"
 
@@ -161,50 +163,51 @@
         for i in range(self.maze_attr.width):
             for j in range(self.maze_attr.height):
                 color = np.zeros(3)
                 if self.maze_attr.cells[i][j] == -1:
                     color[0] = color[1] = color[2] = 0
                 else:
                     color[0] = color[1] = color[2] = 1
-                table.add_cell(
-                    j, i, 0.1, 0.2, facecolor=color, text="", loc="center"
-                )
+                table.add_cell(j, i, 0.1, 0.2, facecolor=color, text="", loc="center")
 
     def display(self, rgba, mode):
         if mode == "human" or mode == "legacy":
             if self.using_notebook:
-                import IPython.display as display 
+                import IPython.display as display
                 from PIL import Image
                 import io
                 import ipywidgets as widgets
 
                 # Creates a new widget if needed
                 # (1) no widget
                 # (2) widget in another cell
-                if self.widget_out is None or self.widget_execution_count != get_ipython().execution_count:
+                if (
+                    self.widget_out is None
+                    or self.widget_execution_count != get_ipython().execution_count
+                ):
                     self.widget_out = widgets.Output()
                     self.widget_execution_count = get_ipython().execution_count
                     display.display(self.widget_out)
 
                 self.widget_out.clear_output(True)
                 with self.widget_out:
-                    image = Image.fromarray(rgba, 'RGBA')
+                    image = Image.fromarray(rgba, "RGBA")
                     output = io.BytesIO()
-                    image.save(output, format='png')
+                    image.save(output, format="png")
                     display.display(display.Image(data=output.getvalue(), format="png"))
             else:
                 fig = plt.gcf()
                 fig.clear()
                 ax = fig.add_subplot()
-                ax.axis('off')
+                ax.axis("off")
                 ax.imshow(rgba)
                 plt.show(block=False)
 
         elif mode == "rgb_array":
-            return rgba
+            return rgba.copy()
         else:
             raise NotImplementedError(f"Mode {mode} is not implemented")
 
     def render_base(self, title):
         fig = Figure(figsize=(self.figW, self.figH))
         canvas = FigureCanvasAgg(fig)
         axes = fig.add_subplot(111)
@@ -216,16 +219,14 @@
 
         self.plot_history.append(Plot(canvas, fig, axes, table, patch))
         axes.add_patch(patch)
 
         self.init_table(table)
         axes.add_table(table)
 
-
-
     def new_render(self, title, mode="human"):
         """
         initializes the plot by creating its basic components (figure, axis, agent patch and table)
         a trace of these components is stored so that the old outputs will last on the notebook
         when a new rendering is performed
         """
 
@@ -247,15 +248,15 @@
     def render(
         self,
         v=None,
         policy=None,
         agent_state=None,
         stochastic=False,
         title="No title",
-        mode="legacy"
+        mode="legacy",
     ):
         """
         updates the values of the table
         and the agent position and current policy
         some of these components may not show depending on the parameters given when calling this function
         the agent state is set to None if we do not want to plot the agent
 
@@ -266,19 +267,18 @@
 
         if v is None:
             v = np.array([])
 
         if policy is None:
             policy = np.array([])
 
-
         if len(self.plot_history) == 0:
             self.render_base(title)
         plot = self.plot_history[-1]
-        
+
         plot.axes.clear()
         plot.axes.add_table(plot.table)
 
         # Table values and policy update
         for i in range(self.maze_attr.width):
             for j in range(self.maze_attr.height):
                 state = self.maze_attr.cells[i][j]
@@ -299,15 +299,14 @@
                 self.maze_attr.height,
                 self.maze_attr.state_width[agent_state],
                 self.maze_attr.state_height[agent_state],
             )
             plot.patch.center = x, y
             plot.axes.add_patch(plot.patch)
 
-
         plot.fig.subplots_adjust(left=0.2, bottom=0.2)
         # plot.axes.xticks([])
         # plot.axes.yticks([])
         plot.fig.tight_layout()
 
         plot.canvas.draw()
         plot.canvas.flush_events()
@@ -350,17 +349,15 @@
             color[0] = color[1] = color[2] = 0
         else:
             color[0] = color[1] = color[2] = np.min(
                 [1 - np.max(q[state]) / (np.max(q) + 1), 1]
             )
 
         plot.table._cells[(j, i)].set_facecolor(color)
-        plot.table._cells[(j, i)]._text.set_text(
-            np.round(np.max(q[state]), 2)
-        )
+        plot.table._cells[(j, i)]._text.set_text(np.round(np.max(q[state]), 2))
 
         if not (state == -1 or state in self.terminal_states):
             qmin = np.min(q[state])
             if qmin < 0:
                 qmin *= -1  # TODO: should deal better with negative Q values
             pos_q = q[state] + qmin
             qmax = np.max(pos_q)
@@ -429,17 +426,15 @@
             color[0] = color[1] = color[2] = 0
         else:
             color[0] = color[1] = color[2] = np.min(
                 [1 - np.max(q[state]) / (np.max(q) + 1), 1]
             )
 
         plot.table._cells[(j, i)].set_facecolor(color)
-        plot.table._cells[(j, i)]._text.set_text(
-            np.round(np.max(q[state]), 2)
-        )
+        plot.table._cells[(j, i)]._text.set_text(np.round(np.max(q[state]), 2))
 
         if not (state == -1 or state in self.terminal_states):
             qmin = np.min(q[state])
             if qmin < 0:
                 qmin *= -1  # TODO: should deal better with negative Q values
             pos__q = q[state] + qmin
             qmax = np.max(pos__q)
```

### Comparing `mazemdp-0.7.3/mazemdp/mdp.py` & `mazemdp-0.8.0/mazemdp/mdp.py`

 * *Files identical despite different names*

### Comparing `mazemdp-0.7.3/mazemdp/simple_action_space.py` & `mazemdp-0.8.0/mazemdp/simple_action_space.py`

 * *Files identical despite different names*

### Comparing `mazemdp-0.7.3/mazemdp/toolbox.py` & `mazemdp-0.8.0/mazemdp/toolbox.py`

 * *Files identical despite different names*

### Comparing `mazemdp-0.7.3/mazemdp.egg-info/PKG-INFO` & `mazemdp-0.8.0/mazemdp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: mazemdp
-Version: 0.7.3
+Version: 0.8.0
 Summary: An simple maze to test dynamic programming and tabular reinforcement learning algorithms
 Home-page: https://github.com/osigaud/SimpleMazeMDP
 Author: Olivier Sigaud
 Author-email: Olivier.Sigaud@isir.upmc.fr
 License: MIT
+Description-Content-Type: text/markdown; charset=UTF-8
 License-File: LICENSE
 
 # SimpleMazeMDP: 
 
 This repository contains code to provide a simple Maze environment used as example MDP for tabular dynamic programming and reinforcement learning labs.
 
 If you want to do the corresponding labs, you need a Google account. Then you can copy-paste the [dynamic programming colab](https://colab.research.google.com/drive/1FpI-h_q-Iq3hBnmRjRUUwhDDK7TtQEVz) and the [reinforcement learning colab](https://colab.research.google.com/drive/1o4TnFGwgeN1e1DBrLRANj7Rj1_MTIkDJ).
```

### Comparing `mazemdp-0.7.3/setup.py` & `mazemdp-0.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `mazemdp-0.7.3/tests/test_mdp.py` & `mazemdp-0.8.0/tests/test_mdp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import numpy as np
 
 from mazemdp import create_random_maze
 from mazemdp.chrono import Chrono
 from mazemdp.toolbox import egreedy_loc
 
-
 import matplotlib
 
 matplotlib.use("TkAgg")
 
 np.random.seed(0)
 
 
 def test_create():
     chrono = Chrono()
     mdp, *args = create_random_maze(5, 5, 0.2, hit=True)
     mdp.new_render("Test visu maze")
+    print(mdp.action_space)
     chrono.stop()
 
 
 def test_maze_visu():
     mdp, *args = create_random_maze(4, 5, 0.2)
     mdp.new_render("Test visu value")
     for _ in range(3):
```

