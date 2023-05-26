# Comparing `tmp/crewmate-0.0.0.3.tar.gz` & `tmp/crewmate-0.0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crewmate-0.0.0.3.tar", last modified: Thu May 25 10:37:33 2023, max compression
+gzip compressed data, was "crewmate-0.0.0.4.tar", last modified: Fri May 26 04:33:37 2023, max compression
```

## Comparing `crewmate-0.0.0.3.tar` & `crewmate-0.0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 10:37:33.069123 crewmate-0.0.0.3/
--rw-rw-rw-   0        0        0      178 2023-05-25 10:37:33.068114 crewmate-0.0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      434 2023-05-25 09:23:08.000000 crewmate-0.0.0.3/README.md
--rw-rw-rw-   0        0        0      108 2023-05-25 06:50:37.000000 crewmate-0.0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-25 10:37:33.069123 crewmate-0.0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      476 2023-05-25 10:37:28.000000 crewmate-0.0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-25 10:37:33.059218 crewmate-0.0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-25 10:37:33.063857 crewmate-0.0.0.3/src/crewmate/
--rw-rw-rw-   0        0        0        0 2023-05-25 09:10:04.000000 crewmate-0.0.0.3/src/crewmate/__init__.py
--rw-rw-rw-   0        0        0     1891 2023-05-25 04:31:44.000000 crewmate-0.0.0.3/src/crewmate/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-25 10:37:33.066997 crewmate-0.0.0.3/src/crewmate.egg-info/
--rw-rw-rw-   0        0        0      178 2023-05-25 10:37:32.000000 crewmate-0.0.0.3/src/crewmate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-05-25 10:37:32.000000 crewmate-0.0.0.3/src/crewmate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 10:37:32.000000 crewmate-0.0.0.3/src/crewmate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-25 10:37:32.000000 crewmate-0.0.0.3/src/crewmate.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-25 10:37:32.000000 crewmate-0.0.0.3/src/crewmate.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-26 04:33:37.597859 crewmate-0.0.0.4/
+-rw-rw-rw-   0        0        0      178 2023-05-26 04:33:37.597859 crewmate-0.0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      428 2023-05-26 04:28:27.000000 crewmate-0.0.0.4/README.md
+-rw-rw-rw-   0        0        0      108 2023-05-25 06:50:37.000000 crewmate-0.0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-26 04:33:37.599103 crewmate-0.0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      476 2023-05-26 04:33:34.000000 crewmate-0.0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 04:33:37.589186 crewmate-0.0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-26 04:33:37.592888 crewmate-0.0.0.4/src/crewmate/
+-rw-rw-rw-   0        0        0        0 2023-05-25 09:10:04.000000 crewmate-0.0.0.4/src/crewmate/__init__.py
+-rw-rw-rw-   0        0        0     3527 2023-05-26 04:31:10.000000 crewmate-0.0.0.4/src/crewmate/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-26 04:33:37.596852 crewmate-0.0.0.4/src/crewmate.egg-info/
+-rw-rw-rw-   0        0        0      178 2023-05-26 04:33:37.000000 crewmate-0.0.0.4/src/crewmate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-05-26 04:33:37.000000 crewmate-0.0.0.4/src/crewmate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 04:33:37.000000 crewmate-0.0.0.4/src/crewmate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-26 04:33:37.000000 crewmate-0.0.0.4/src/crewmate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-26 04:33:37.000000 crewmate-0.0.0.4/src/crewmate.egg-info/top_level.txt
```

### Comparing `crewmate-0.0.0.3/src/crewmate/utils.py` & `crewmate-0.0.0.4/src/crewmate/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,63 @@
 import numpy as np
+import qctrl
+import qctrlvisualizer
+import matplotlib.pyplot as plt
+
+
+def quick_wigner_qctrl(qctrl: qctrl.Qctrl, psi: np.array, c_dim: int, q_dim: int, title="Wigner"):
+    """Plot the Wigner function of the state in the cavity starting from the full state (qubit x cavity).
+
+    Parameters
+    ----------
+    qctrl : qctrl.Qctrl
+        qctrl session reference
+    psi : np.array
+        state in the form qubit x cavity
+    c_dim : int
+        dimension of the cavity Hilbert space
+    q_dim : int
+        dimension of the qubit Hilbert space
+    title : str, optional
+        plot title, by default "Wigner"
+
+    Examples
+    --------
+    Consider psi = |cavity> x |qubit> = [1,0,0,0,0,0]
+    >>> quick_wigner_qctrl(qctrl, [1,0,0,0,0,0], 3, 2)
+    """
+
+    graph = qctrl.create_graph()
+
+    # Cavity state
+    final_cavity_state = graph.partial_trace(
+        graph.outer_product(psi, psi),
+        [c_dim, q_dim],
+        1,
+    )
+    # Wigner
+    wigner_range = 3
+    wigner_density = 128
+    # Axes for wigner plot
+    position = np.linspace(-wigner_range, wigner_range, wigner_density)
+    momentum = np.linspace(-wigner_range, wigner_range, wigner_density)
+    # Wigner transform
+    graph.wigner_transform(
+        final_cavity_state, position, momentum, name="wigner")
+
+    # Simulate system
+    simulation = qctrl.functions.calculate_graph(
+        graph=graph,
+        output_node_names=["wigner"]
+    )
+
+    qctrlvisualizer.plot_wigner_function(
+        simulation.output["wigner"]["value"], position, momentum)
+    plt.suptitle(title)
+    plt.show()
 
 
 def find_highest_populated_state(state: np.array, tolerance: float = 1e-6) -> int:
     """Find the highest Fock state that is populated for more than the specified tolerance.
 
     Parameters
     ----------
@@ -19,21 +74,21 @@
     Raises
     ------
     Exception
         If couldn't find a populated-enough state.
 
     Examples
     --------
+    In this case state |1> is the highest populated state, considering the default tolerance of 1e-6.
     >>> find_highest_populated_state([0.99, 0.01, 0])
     1
-    State |1> is the highest populated state, considering the default tolerance of 1e-6.
 
+    Now state |0> is the highest populated state, considering a tolerance of 0.1.
     >>> find_highest_populated_state([0.99, 0.01, 0], tolerance=0.1)
     0
-    State |0> is the highest populated state, considering a tolerance of 0.1.
     """
     # Highest occupied state above tolerance
     highest = -1
     state_abs = np.abs(state) ** 2
     for n in range(len(state)-1, -1, -1):
         if state_abs[n] > tolerance:
             highest = n
```

