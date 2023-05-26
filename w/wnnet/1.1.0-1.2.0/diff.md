# Comparing `tmp/wnnet-1.1.0.tar.gz` & `tmp/wnnet-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wnnet-1.1.0.tar", last modified: Sat Apr 29 20:39:34 2023, max compression
+gzip compressed data, was "wnnet-1.2.0.tar", last modified: Fri May 26 12:14:59 2023, max compression
```

## Comparing `wnnet-1.1.0.tar` & `wnnet-1.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-04-29 20:39:34.469135 wnnet-1.1.0/
--rw-r--r--   0 bradleymeyer   (501) staff       (20)    35147 2023-01-19 23:05:37.000000 wnnet-1.1.0/LICENSE.txt
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      188 2023-02-20 16:56:48.000000 wnnet-1.1.0/MANIFEST.in
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     1623 2023-04-29 20:39:34.469490 wnnet-1.1.0/PKG-INFO
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      837 2023-03-18 14:20:36.000000 wnnet-1.1.0/README.rst
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      107 2023-04-29 20:39:34.471778 wnnet-1.1.0/setup.cfg
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     6056 2023-03-18 14:18:12.000000 wnnet-1.1.0/setup.py
-drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-04-29 20:39:34.455627 wnnet-1.1.0/wnnet/
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      279 2023-04-29 20:37:57.000000 wnnet-1.1.0/wnnet/__about__.py
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      197 2023-03-18 14:18:12.000000 wnnet-1.1.0/wnnet/__init__.py
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      993 2023-02-20 16:43:35.000000 wnnet-1.1.0/wnnet/consts.py
--rw-r--r--   0 bradleymeyer   (501) staff       (20)    15337 2023-04-29 20:37:57.000000 wnnet-1.1.0/wnnet/flows.py
--rw-r--r--   0 bradleymeyer   (501) staff       (20)    47384 2023-04-29 20:37:57.000000 wnnet-1.1.0/wnnet/graph.py
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     7120 2023-04-29 20:37:57.000000 wnnet-1.1.0/wnnet/net.py
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     4155 2023-02-20 16:43:35.000000 wnnet-1.1.0/wnnet/nuc.py
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     3531 2023-02-20 16:43:35.000000 wnnet-1.1.0/wnnet/reac.py
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      864 2023-01-19 23:05:37.000000 wnnet-1.1.0/wnnet/zones.py
-drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-04-29 20:39:34.465451 wnnet-1.1.0/wnnet.egg-info/
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     1623 2023-04-29 20:39:34.000000 wnnet-1.1.0/wnnet.egg-info/PKG-INFO
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      335 2023-04-29 20:39:34.000000 wnnet-1.1.0/wnnet.egg-info/SOURCES.txt
--rw-r--r--   0 bradleymeyer   (501) staff       (20)        1 2023-04-29 20:39:34.000000 wnnet-1.1.0/wnnet.egg-info/dependency_links.txt
--rw-r--r--   0 bradleymeyer   (501) staff       (20)       66 2023-04-29 20:39:34.000000 wnnet-1.1.0/wnnet.egg-info/requires.txt
--rw-r--r--   0 bradleymeyer   (501) staff       (20)        6 2023-04-29 20:39:34.000000 wnnet-1.1.0/wnnet.egg-info/top_level.txt
+drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-05-26 12:14:59.281010 wnnet-1.2.0/
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)    35147 2023-01-19 23:05:37.000000 wnnet-1.2.0/LICENSE.txt
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      188 2023-02-20 16:56:48.000000 wnnet-1.2.0/MANIFEST.in
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     1623 2023-05-26 12:14:59.281218 wnnet-1.2.0/PKG-INFO
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      837 2023-03-18 14:20:36.000000 wnnet-1.2.0/README.rst
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      107 2023-05-26 12:14:59.282297 wnnet-1.2.0/setup.cfg
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     6056 2023-03-18 14:18:12.000000 wnnet-1.2.0/setup.py
+drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-05-26 12:14:59.258545 wnnet-1.2.0/wnnet/
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      279 2023-05-26 12:14:25.000000 wnnet-1.2.0/wnnet/__about__.py
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      197 2023-03-18 14:18:12.000000 wnnet-1.2.0/wnnet/__init__.py
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      993 2023-02-20 16:43:35.000000 wnnet-1.2.0/wnnet/consts.py
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)    15337 2023-04-29 20:37:57.000000 wnnet-1.2.0/wnnet/flows.py
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)    47384 2023-04-29 20:37:57.000000 wnnet-1.2.0/wnnet/graph.py
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     8618 2023-05-26 12:14:25.000000 wnnet-1.2.0/wnnet/net.py
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     4155 2023-02-20 16:43:35.000000 wnnet-1.2.0/wnnet/nuc.py
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     3531 2023-02-20 16:43:35.000000 wnnet-1.2.0/wnnet/reac.py
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      864 2023-01-19 23:05:37.000000 wnnet-1.2.0/wnnet/zones.py
+drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-05-26 12:14:59.280077 wnnet-1.2.0/wnnet.egg-info/
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     1623 2023-05-26 12:14:59.000000 wnnet-1.2.0/wnnet.egg-info/PKG-INFO
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      335 2023-05-26 12:14:59.000000 wnnet-1.2.0/wnnet.egg-info/SOURCES.txt
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)        1 2023-05-26 12:14:59.000000 wnnet-1.2.0/wnnet.egg-info/dependency_links.txt
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)       66 2023-05-26 12:14:59.000000 wnnet-1.2.0/wnnet.egg-info/requires.txt
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)        6 2023-05-26 12:14:59.000000 wnnet-1.2.0/wnnet.egg-info/top_level.txt
```

### Comparing `wnnet-1.1.0/LICENSE.txt` & `wnnet-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wnnet-1.1.0/PKG-INFO` & `wnnet-1.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wnnet
-Version: 1.1.0
+Version: 1.2.0
 Summary: Python project to handle webnucleo reaction networks
 Home-page: https://github.com/mbradle/wnnet
 Author: Clemson University
 Author-email: mbradle@g.clemson.edu
 License: GPLv3+
 Project-URL: Bug Reports, https://github.com/mbradle/wnnet/issues
 Project-URL: Source, https://github.com/mbradle/wnnet/
```

### Comparing `wnnet-1.1.0/README.rst` & `wnnet-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `wnnet-1.1.0/setup.py` & `wnnet-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `wnnet-1.1.0/wnnet/consts.py` & `wnnet-1.2.0/wnnet/consts.py`

 * *Files identical despite different names*

### Comparing `wnnet-1.1.0/wnnet/flows.py` & `wnnet-1.2.0/wnnet/flows.py`

 * *Files identical despite different names*

### Comparing `wnnet-1.1.0/wnnet/graph.py` & `wnnet-1.2.0/wnnet/graph.py`

 * *Files identical despite different names*

### Comparing `wnnet-1.1.0/wnnet/net.py` & `wnnet-1.2.0/wnnet/net.py`

 * *Files 18% similar despite different names*

```diff
@@ -110,14 +110,58 @@
             "positron" in reaction.nuclide_reactants
             and "anti-neutrino_e" in reaction_products
         ):
             result += 2.0 * wc.m_e_in_MeV
 
         return result
 
+    def _obeys_conservation_laws(self, nuclides, reaction):
+        ep = {"electron": -1, "positron": 1}
+        e_lepton = {
+            "electron": 1,
+            "positron": -1,
+            "neutrino_e": 1,
+            "anti-neutrino_e": -1,
+        }
+        mu_lepton = {"neutrino_mu": 1, "anti-neutrino_mu": -1}
+        tau_lepton = {"neutrino_tau": 1, "anti-neutrino_tau": -1}
+
+        d_z = 0
+        d_a = 0
+        d_l_e = 0
+        d_l_mu = 0
+        d_l_tau = 0
+
+        for sp in reaction.reactants:
+            if sp in nuclides:
+                d_a += nuclides[sp]["a"]
+                d_z += nuclides[sp]["z"]
+            if sp in ep:
+                d_z += ep[sp]
+            if sp in e_lepton:
+                d_l_e += e_lepton[sp]
+            if sp in mu_lepton:
+                d_l_mu += mu_lepton[sp]
+            if sp in tau_lepton:
+                d_l_tau += tau_lepton[sp]
+        for sp in reaction.products:
+            if sp in nuclides:
+                d_a -= nuclides[sp]["a"]
+                d_z -= nuclides[sp]["z"]
+            if sp in ep:
+                d_z -= ep[sp]
+            if sp in e_lepton:
+                d_l_e -= e_lepton[sp]
+            if sp in mu_lepton:
+                d_l_mu -= mu_lepton[sp]
+            if sp in tau_lepton:
+                d_l_tau -= tau_lepton[sp]
+
+        return d_a == 0 and d_z == 0 and d_l_e == 0 and d_l_mu == 0 and d_l_tau == 0
+
     def is_valid_reaction(self, name, nuc_xpath=""):
         """Method to determine a reaction is valid in the network.
 
         Args:
             ``name`` (:obj:`str`):  A string giving the reaction.
 
             ``nuclides`` (:obj:`str`, optional):  An XPath expression to select nuclides.  Default is all nuclides.
@@ -125,14 +169,18 @@
         Returns:
             A :obj:`bool` with value True if the reaction is valid and False if not.
 
         """
 
         nuclides = self.get_nuclides(nuc_xpath=nuc_xpath)
         reaction = self.get_reactions()[name]
+
+        if not self._obeys_conservation_laws(nuclides, reaction):
+            return False
+
         for sp in reaction.nuclide_reactants + reaction.nuclide_products:
             if sp not in nuclides:
                 return False
         return True
 
     def compute_rates_for_reaction(self, name, t9, user_funcs=""):
         """Method to compute the forward and reverse rates for a valid reaction.
```

### Comparing `wnnet-1.1.0/wnnet/nuc.py` & `wnnet-1.2.0/wnnet/nuc.py`

 * *Files identical despite different names*

### Comparing `wnnet-1.1.0/wnnet/reac.py` & `wnnet-1.2.0/wnnet/reac.py`

 * *Files identical despite different names*

### Comparing `wnnet-1.1.0/wnnet/zones.py` & `wnnet-1.2.0/wnnet/zones.py`

 * *Files identical despite different names*

### Comparing `wnnet-1.1.0/wnnet.egg-info/PKG-INFO` & `wnnet-1.2.0/wnnet.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wnnet
-Version: 1.1.0
+Version: 1.2.0
 Summary: Python project to handle webnucleo reaction networks
 Home-page: https://github.com/mbradle/wnnet
 Author: Clemson University
 Author-email: mbradle@g.clemson.edu
 License: GPLv3+
 Project-URL: Bug Reports, https://github.com/mbradle/wnnet/issues
 Project-URL: Source, https://github.com/mbradle/wnnet/
```

