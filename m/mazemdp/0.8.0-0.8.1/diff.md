# Comparing `tmp/mazemdp-0.8.0.tar.gz` & `tmp/mazemdp-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mazemdp-0.8.0.tar", last modified: Thu Mar 23 08:00:18 2023, max compression
+gzip compressed data, was "mazemdp-0.8.1.tar", last modified: Fri May 26 13:46:01 2023, max compression
```

## Comparing `mazemdp-0.8.0.tar` & `mazemdp-0.8.1.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:00:18.124658 mazemdp-0.8.0/
--rwxr-xr-x   0 runner    (1001) docker     (123)      161 2023-03-23 08:00:03.000000 mazemdp-0.8.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:00:18.120658 mazemdp-0.8.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:00:18.120658 mazemdp-0.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-03-23 08:00:03.000000 mazemdp-0.8.0/.github/workflows/python-publish.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1862 2023-03-23 08:00:03.000000 mazemdp-0.8.0/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)     1071 2023-03-23 08:00:03.000000 mazemdp-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-23 08:00:03.000000 mazemdp-0.8.0/MANIFEST.in
--rwxr-xr-x   0 runner    (1001) docker     (123)     1366 2023-03-23 08:00:03.000000 mazemdp-0.8.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-03-23 08:00:18.124658 mazemdp-0.8.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     4212 2023-03-23 08:00:03.000000 mazemdp-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:00:18.124658 mazemdp-0.8.0/mazemdp/
--rwxr-xr-x   0 runner    (1001) docker     (123)      227 2023-03-23 08:00:03.000000 mazemdp-0.8.0/mazemdp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-23 08:00:18.000000 mazemdp-0.8.0/mazemdp/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-03-23 08:00:03.000000 mazemdp-0.8.0/mazemdp/chrono.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10837 2023-03-23 08:00:03.000000 mazemdp-0.8.0/mazemdp/maze.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16128 2023-03-23 08:00:03.000000 mazemdp-0.8.0/mazemdp/maze_plotter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4273 2023-03-23 08:00:03.000000 mazemdp-0.8.0/mazemdp/mdp.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-03-23 08:00:03.000000 mazemdp-0.8.0/mazemdp/simple_action_space.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3268 2023-03-23 08:00:03.000000 mazemdp-0.8.0/mazemdp/toolbox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:00:18.124658 mazemdp-0.8.0/mazemdp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-03-23 08:00:18.000000 mazemdp-0.8.0/mazemdp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-03-23 08:00:18.000000 mazemdp-0.8.0/mazemdp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 08:00:18.000000 mazemdp-0.8.0/mazemdp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-23 08:00:18.000000 mazemdp-0.8.0/mazemdp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-23 08:00:18.000000 mazemdp-0.8.0/mazemdp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-03-23 08:00:03.000000 mazemdp-0.8.0/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)       51 2023-03-23 08:00:03.000000 mazemdp-0.8.0/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      579 2023-03-23 08:00:18.124658 mazemdp-0.8.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      793 2023-03-23 08:00:03.000000 mazemdp-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:00:18.124658 mazemdp-0.8.0/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:00:03.000000 mazemdp-0.8.0/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1654 2023-03-23 08:00:03.000000 mazemdp-0.8.0/tests/test_mdp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:46:01.097167 mazemdp-0.8.1/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      161 2023-05-26 13:45:48.000000 mazemdp-0.8.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:46:01.097167 mazemdp-0.8.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:46:01.097167 mazemdp-0.8.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-26 13:45:48.000000 mazemdp-0.8.1/.github/workflows/python-publish.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1866 2023-05-26 13:45:48.000000 mazemdp-0.8.1/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1071 2023-05-26 13:45:48.000000 mazemdp-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-26 13:45:48.000000 mazemdp-0.8.1/MANIFEST.in
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1366 2023-05-26 13:45:48.000000 mazemdp-0.8.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-05-26 13:46:01.097167 mazemdp-0.8.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4212 2023-05-26 13:45:48.000000 mazemdp-0.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-26 13:45:48.000000 mazemdp-0.8.1/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       51 2023-05-26 13:45:48.000000 mazemdp-0.8.1/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      677 2023-05-26 13:46:01.101167 mazemdp-0.8.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-05-26 13:45:48.000000 mazemdp-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:46:01.097167 mazemdp-0.8.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:46:01.097167 mazemdp-0.8.1/src/mazemdp/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      227 2023-05-26 13:45:48.000000 mazemdp-0.8.1/src/mazemdp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-26 13:46:00.000000 mazemdp-0.8.1/src/mazemdp/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-05-26 13:45:48.000000 mazemdp-0.8.1/src/mazemdp/chrono.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10828 2023-05-26 13:45:48.000000 mazemdp-0.8.1/src/mazemdp/maze.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16128 2023-05-26 13:45:48.000000 mazemdp-0.8.1/src/mazemdp/maze_plotter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4482 2023-05-26 13:45:48.000000 mazemdp-0.8.1/src/mazemdp/mdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-26 13:45:48.000000 mazemdp-0.8.1/src/mazemdp/simple_action_space.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3268 2023-05-26 13:45:48.000000 mazemdp-0.8.1/src/mazemdp/toolbox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:46:01.097167 mazemdp-0.8.1/src/mazemdp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-05-26 13:46:01.000000 mazemdp-0.8.1/src/mazemdp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-26 13:46:01.000000 mazemdp-0.8.1/src/mazemdp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 13:46:01.000000 mazemdp-0.8.1/src/mazemdp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 13:46:01.000000 mazemdp-0.8.1/src/mazemdp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-26 13:46:01.000000 mazemdp-0.8.1/src/mazemdp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:46:01.097167 mazemdp-0.8.1/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:45:48.000000 mazemdp-0.8.1/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1654 2023-05-26 13:45:48.000000 mazemdp-0.8.1/tests/test_mdp.py
```

### Comparing `mazemdp-0.8.0/.github/workflows/python-publish.yml` & `mazemdp-0.8.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `mazemdp-0.8.0/.gitignore` & `mazemdp-0.8.1/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -129,8 +129,8 @@
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
 test.py
-mazemdp/_version.py
+src/mazemdp/_version.py
```

### Comparing `mazemdp-0.8.0/LICENSE` & `mazemdp-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mazemdp-0.8.0/Makefile` & `mazemdp-0.8.1/Makefile`

 * *Files identical despite different names*

### Comparing `mazemdp-0.8.0/PKG-INFO` & `mazemdp-0.8.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: mazemdp
-Version: 0.8.0
+Version: 0.8.1
 Summary: An simple maze to test dynamic programming and tabular reinforcement learning algorithms
-Home-page: https://github.com/osigaud/SimpleMazeMDP
-Author: Olivier Sigaud
-Author-email: Olivier.Sigaud@isir.upmc.fr
-License: MIT
-Description-Content-Type: text/markdown; charset=UTF-8
+Author-email: Olivier Sigaud <Olivier.Sigaud@isir.upmc.fr>
+Project-URL: homepage, https://github.com/osigaud/SimpleMazeMDP
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SimpleMazeMDP: 
 
 This repository contains code to provide a simple Maze environment used as example MDP for tabular dynamic programming and reinforcement learning labs.
 
 If you want to do the corresponding labs, you need a Google account. Then you can copy-paste the [dynamic programming colab](https://colab.research.google.com/drive/1FpI-h_q-Iq3hBnmRjRUUwhDDK7TtQEVz) and the [reinforcement learning colab](https://colab.research.google.com/drive/1o4TnFGwgeN1e1DBrLRANj7Rj1_MTIkDJ).
```

### Comparing `mazemdp-0.8.0/README.md` & `mazemdp-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `mazemdp-0.8.0/mazemdp/chrono.py` & `mazemdp-0.8.1/src/mazemdp/chrono.py`

 * *Files identical despite different names*

### Comparing `mazemdp-0.8.0/mazemdp/maze.py` & `mazemdp-0.8.1/src/mazemdp/maze.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,26 +8,26 @@
 import numpy as np
 
 from mazemdp.maze_plotter import MazePlotter  # used to plot the maze
 from mazemdp.mdp import Mdp
 from mazemdp.toolbox import E, N, S, W
 
 
-def check_navigability(mdp):
+def check_navigability(mdp: Mdp):
     v = np.zeros(mdp.nb_states)  # initial state values are set to 0
     stop = False
 
     while not stop:
         v_old = v.copy()
 
         for x in range(mdp.nb_states):  # for each state x
             # Compute the value of state x for each action u of the MDP action space
             if x not in mdp.terminal_states:
                 v_temp = []
-                for u in range(mdp.action_space.n):
+                for u in range(mdp.nb_actions):
                     # Process sum of the values of the neighbouring states
                     summ = 0
                     for y in range(mdp.nb_states):
                         summ = summ + mdp.P[x, u, y] * v_old[y]
                     v_temp.append(mdp.r[x, u] + summ)
 
                 # Select the highest state value among those computed
@@ -142,15 +142,15 @@
         else:
             reward_matrix = self.simple_reward(transition_matrix)
 
         plotter = MazePlotter(self)  # renders the environment
 
         self.mdp = Mdp(
             self.nb_states + 1,
-            self.action_space,
+            self.nb_actions,
             start_distribution,
             transition_matrix,
             reward_matrix,
             plotter,
             gamma=self.gamma,
             terminal_states=[self.nb_states],
             timeout=timeout,
@@ -183,15 +183,15 @@
     def init_transitions(self, hit):
         """
         Init the transition matrix
         a "well" state is added that only the terminal states can get into
         """
 
         transition_matrix = np.empty(
-            (self.nb_states + 1, self.action_space.n, self.nb_states + 1)
+            (self.nb_states + 1, self.nb_actions, self.nb_states + 1)
         )
 
         transition_matrix[:, N, :] = np.zeros((self.nb_states + 1, self.nb_states + 1))
         transition_matrix[:, S, :] = np.zeros((self.nb_states + 1, self.nb_states + 1))
         transition_matrix[:, E, :] = np.zeros((self.nb_states + 1, self.nb_states + 1))
         transition_matrix[:, W, :] = np.zeros((self.nb_states + 1, self.nb_states + 1))
 
@@ -232,15 +232,15 @@
         return transition_matrix
 
         # self.mdp = MyMdp(self.nb_states, self.action_space, start_distribution, transition_matrix, reward_matrix,
         #                plotter, proba_action=0.5, gamma=gamma, terminal_states=terminal_states, timeout=timeout)
 
     # --------------------------------- Reward Matrix ---------------------------------
     def simple_reward(self, transition_matrix: np.array):
-        reward_matrix = np.zeros((self.nb_states, self.action_space.n))
+        reward_matrix = np.zeros((self.nb_states, self.nb_actions))
         for from_state, action in zip(*np.nonzero(transition_matrix[:, :, self.well])):
             reward_matrix[from_state, action] = 1.0
         return reward_matrix
 
     # --------------------------------- Reward Matrix ---------------------------------
     def reward_hit_walls(self, transition_matrix: np.array):
         # Get the for reaching a final state
```

### Comparing `mazemdp-0.8.0/mazemdp/maze_plotter.py` & `mazemdp-0.8.1/src/mazemdp/maze_plotter.py`

 * *Files identical despite different names*

### Comparing `mazemdp-0.8.0/mazemdp/mdp.py` & `mazemdp-0.8.1/src/mazemdp/mdp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,57 @@
 """
 Author: Olivier Sigaud
 """
 
+from functools import cached_property
 import numpy as np
 
 from mazemdp.toolbox import sample_categorical
 
 
 class Mdp:
     """
     defines a Markov Decision Process
     """
 
     def __init__(
         self,
         nb_states,
-        action_space,
+        nb_actions,
         start_distribution,
         transition_matrix,
         reward_matrix,
         plotter,
         gamma=0.9,
         terminal_states=None,
         timeout=50,
         has_state=True,
     ):
         assert timeout > 10, "timeout too short:" + timeout
         self.nb_states = nb_states
+        self.nb_actions = nb_actions
         if terminal_states is None:
             terminal_states = []
         self.terminal_states = terminal_states
-        self.action_space = action_space
         self.has_state = has_state
         self.timeout = timeout  # maximum length of an episode
         self.timestep = 0
         self.P0 = start_distribution  # distribution used to draw the first state of the agent, used in method reset()
         self.P = transition_matrix
         self.r = reward_matrix
         self.plotter = plotter  # used to plot the maze
         self.gamma = gamma  # discount factor
         self.current_state = None
 
+    @cached_property
+    def action_space(self):
+        """Legacy method to get the action space"""
+        import gym
+        return gym.spaces.Discrete(self.nb_actions)
+    
     def reset(
         self, uniform=False
     ):  # initializes an episode and returns the state of the agent
         # if uniform is set to False, the first state is drawn according to the P0 distribution,
         # else it is drawn from a uniform distribution over all the states except for walls
 
         if uniform:
```

### Comparing `mazemdp-0.8.0/mazemdp/simple_action_space.py` & `mazemdp-0.8.1/src/mazemdp/simple_action_space.py`

 * *Files identical despite different names*

### Comparing `mazemdp-0.8.0/mazemdp/toolbox.py` & `mazemdp-0.8.1/src/mazemdp/toolbox.py`

 * *Files identical despite different names*

### Comparing `mazemdp-0.8.0/mazemdp.egg-info/PKG-INFO` & `mazemdp-0.8.1/src/mazemdp.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: mazemdp
-Version: 0.8.0
+Version: 0.8.1
 Summary: An simple maze to test dynamic programming and tabular reinforcement learning algorithms
-Home-page: https://github.com/osigaud/SimpleMazeMDP
-Author: Olivier Sigaud
-Author-email: Olivier.Sigaud@isir.upmc.fr
-License: MIT
-Description-Content-Type: text/markdown; charset=UTF-8
+Author-email: Olivier Sigaud <Olivier.Sigaud@isir.upmc.fr>
+Project-URL: homepage, https://github.com/osigaud/SimpleMazeMDP
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SimpleMazeMDP: 
 
 This repository contains code to provide a simple Maze environment used as example MDP for tabular dynamic programming and reinforcement learning labs.
 
 If you want to do the corresponding labs, you need a Google account. Then you can copy-paste the [dynamic programming colab](https://colab.research.google.com/drive/1FpI-h_q-Iq3hBnmRjRUUwhDDK7TtQEVz) and the [reinforcement learning colab](https://colab.research.google.com/drive/1o4TnFGwgeN1e1DBrLRANj7Rj1_MTIkDJ).
```

### Comparing `mazemdp-0.8.0/setup.cfg` & `mazemdp-0.8.1/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 [metadata]
+name = mazemdp
 license_file = LICENSE
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8
 
-[pytype]
-inputs = mazemdp
-
 [options]
 include_package_data = True
+package_dir = 
+	=src
+packages = find:
+
+[options.packages.find]
+where = src
+
+[pytype]
+inputs = mazemdp
 
 [flake8]
 ignore = W503,W504,E203,E231  # line breaks before and after binary operators
 per-file-ignores = 
-	./mazemdp/__init__.py:F401
-	./mazemdp/maze_plotter.py:E402, F821
+	./src/mazemdp/__init__.py:F401
+	./src/mazemdp/maze_plotter.py:E402, F821
 exclude = 
 	.git,
 	__pycache__,
 	docs/
 	build,
 	dist
 	*.egg-info
```

### Comparing `mazemdp-0.8.0/tests/test_mdp.py` & `mazemdp-0.8.1/tests/test_mdp.py`

 * *Files identical despite different names*

