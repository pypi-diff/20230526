# Comparing `tmp/mpbn-2.0.tar.gz` & `tmp/mpbn-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpbn-2.0.tar", last modified: Wed Nov 30 23:15:49 2022, max compression
+gzip compressed data, was "mpbn-3.0.tar", last modified: Thu May 25 22:04:40 2023, max compression
```

## Comparing `mpbn-2.0.tar` & `mpbn-3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 23:15:49.208446 mpbn-2.0/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2022-11-30 23:15:41.000000 mpbn-2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2022-11-30 23:15:49.208446 mpbn-2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2022-11-30 23:15:41.000000 mpbn-2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 23:15:49.204446 mpbn-2.0/mpbn/
--rw-r--r--   0 runner    (1001) docker     (123)    14282 2022-11-30 23:15:41.000000 mpbn-2.0/mpbn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 23:15:49.204446 mpbn-2.0/mpbn/asplib/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2022-11-30 23:15:41.000000 mpbn-2.0/mpbn/asplib/mp_attractor.asp
--rw-r--r--   0 runner    (1001) docker     (123)      535 2022-11-30 23:15:41.000000 mpbn-2.0/mpbn/asplib/mp_eval.asp
--rw-r--r--   0 runner    (1001) docker     (123)      453 2022-11-30 23:15:41.000000 mpbn-2.0/mpbn/asplib/mp_positivereach-np.asp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 23:15:49.204446 mpbn-2.0/mpbn/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2022-11-30 23:15:41.000000 mpbn-2.0/mpbn/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6086 2022-11-30 23:15:41.000000 mpbn-2.0/mpbn/cli/sim.py
--rw-r--r--   0 runner    (1001) docker     (123)     9093 2022-11-30 23:15:41.000000 mpbn-2.0/mpbn/simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 23:15:49.204446 mpbn-2.0/mpbn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2022-11-30 23:15:49.000000 mpbn-2.0/mpbn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      362 2022-11-30 23:15:49.000000 mpbn-2.0/mpbn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-30 23:15:49.000000 mpbn-2.0/mpbn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2022-11-30 23:15:49.000000 mpbn-2.0/mpbn.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2022-11-30 23:15:49.000000 mpbn-2.0/mpbn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2022-11-30 23:15:49.000000 mpbn-2.0/mpbn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-11-30 23:15:49.208446 mpbn-2.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1111 2022-11-30 23:15:41.000000 mpbn-2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 22:04:40.905704 mpbn-3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-25 22:04:29.000000 mpbn-3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-05-25 22:04:40.905704 mpbn-3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-25 22:04:29.000000 mpbn-3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 22:04:40.905704 mpbn-3.0/mpbn/
+-rw-r--r--   0 runner    (1001) docker     (123)    15838 2023-05-25 22:04:29.000000 mpbn-3.0/mpbn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 22:04:40.905704 mpbn-3.0/mpbn/asplib/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-25 22:04:29.000000 mpbn-3.0/mpbn/asplib/mp_attractor.asp
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-25 22:04:29.000000 mpbn-3.0/mpbn/asplib/mp_eval.asp
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-25 22:04:29.000000 mpbn-3.0/mpbn/asplib/mp_positivereach-np.asp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 22:04:40.905704 mpbn-3.0/mpbn/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-25 22:04:29.000000 mpbn-3.0/mpbn/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-05-25 22:04:29.000000 mpbn-3.0/mpbn/cli/sim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-05-25 22:04:29.000000 mpbn-3.0/mpbn/simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 22:04:40.905704 mpbn-3.0/mpbn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-05-25 22:04:40.000000 mpbn-3.0/mpbn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-25 22:04:40.000000 mpbn-3.0/mpbn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 22:04:40.000000 mpbn-3.0/mpbn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-25 22:04:40.000000 mpbn-3.0/mpbn.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-25 22:04:40.000000 mpbn-3.0/mpbn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-25 22:04:40.000000 mpbn-3.0/mpbn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 22:04:40.905704 mpbn-3.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1128 2023-05-25 22:04:29.000000 mpbn-3.0/setup.py
```

### Comparing `mpbn-2.0/PKG-INFO` & `mpbn-3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpbn
-Version: 2.0
+Version: 3.0
 Summary: Simple implementation of Most Permissive Boolean networks
 Home-page: https://github.com/bnediction/mpbn
 Author: Loïc Paulevé
 Author-email: loic.pauleve@labri.fr
 License: CeCILL
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `mpbn-2.0/README.md` & `mpbn-3.0/README.md`

 * *Files identical despite different names*

### Comparing `mpbn-2.0/mpbn/__init__.py` & `mpbn-3.0/mpbn/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,17 @@
 
 import os
 from colomoto import minibn
 
 from boolean import boolean
 import clingo
 
+from pyeda.boolalg import bdd
+from pyeda.boolalg.expr import expr
+
 __asplibdir__ = os.path.realpath(os.path.join(os.path.dirname(__file__), "asplib"))
 
 clingo_options = ["-W", "no-atom-undefined"]
 if hasattr(clingo, "version") and clingo.version() >= (5,5,0):
     clingo_options.append("--single-shot")
 
 def aspf(basename):
@@ -62,14 +65,79 @@
     return s
 
 def s2v(s):
     return 1 if s > 0 else -1
 def v2s(v):
     return 1 if v > 0 else 0
 
+def is_unate(ba, f):
+    pos_lits = set()
+    neg_lits = set()
+    def is_lit(f):
+        if isinstance(f, ba.Symbol):
+            pos_lits.add(f.obj)
+            return True
+        if isinstance(f, ba.NOT) \
+                and isinstance(f.args[0], ba.Symbol):
+            neg_lits.add(f.args[0].obj)
+            return True
+        return False
+
+    def is_clause(f):
+        if is_lit(f):
+            return True
+        if isinstance(f, ba.AND):
+            for g in f.args:
+                if not is_lit(g):
+                    return False
+            return True
+        return False
+
+    def test_monotonicity():
+        both = pos_lits.intersection(neg_lits)
+        return not both
+
+    if f in [ba.TRUE, ba.FALSE]:
+        return True
+    if is_clause(f):
+        return test_monotonicity()
+    if isinstance(f, ba.OR):
+        for g in f.args:
+            if not is_clause(g):
+                return False
+        return test_monotonicity()
+    return False
+
+def asp_of_bdd(bid, b):
+    _rules = dict()
+    def register(node, nid=None):
+        if node is bdd.BDDNODEONE:
+            if nid is not None:
+                _rules[bid] = f"bdd({clingo.String(nid)},1)"
+            return 1
+        elif node is bdd.BDDNODEZERO:
+            if nid is not None:
+                _rules[bid] = f"bdd({clingo.String(nid)},-1)"
+            return -1
+        nid = clingo.String(f"{bid}_n{id(node)}" if nid is None else nid)
+        if nid not in _rules:
+            var = clingo.String(bdd._VARS[node.root].qualname)
+            lo = register(node.lo)
+            hi = register(node.hi)
+            a = f"bdd({nid},{var},{lo},{hi})"
+            _rules[nid] = a
+        return nid
+    register(b.node, bid)
+    return _rules.values()
+
+def bddasp_of_boolfunc(f, i):
+    e = expr(str(f).replace("!","~"))
+    b = bdd.expr2bdd(e)
+    atoms = asp_of_bdd(i, b)
+    return "\n".join((f"{a}." for a in atoms))
 
 class MPBooleanNetwork(minibn.BooleanNetwork):
     """
     Most Permissive Boolean Network
 
     Extends ``colomoto.minibn.BooleanNetwork`` class by adding methods for
     computing reachable and attractor properties with the Most Permissive
@@ -77,15 +145,17 @@
     It requires that the Boolean network is *locally monotonic*.
 
     Ensures that the Boolean functions are monotonic and in disjunctive normal
     form (DNF).
     The local-monotonic checking requires that a literal never appears
     with both signs in a same Boolean function.
     """
-    def __init__(self, bn=minibn.BooleanNetwork(), auto_dnf=True):
+    def __init__(self, bn=minibn.BooleanNetwork(), auto_dnf=True,
+                        try_unate_hard=True,
+                        encoding="auto"):
         """
         Constructor for :py:class:`.MPBoooleanNetwork`.
 
         :param bn: Boolean network to copy from
         :type bn: :py:class:`colomoto.minibn.BooleanNetwork` or any type accepted by
             :py:class:`colomoto.minibn.BooleanNetwork` constructor
         :param bool auto_dnf: if ``False``, turns off automatic DNF
@@ -94,104 +164,81 @@
         Examples:
 
         >>> mbn = MPBooleanNetwork("network.bnet")
         >>> bn = BooleanNetwork()
         >>> bn["a"] = ".."; ...
         >>> mbn = MPBooleanNetwork(bn)
         """
-        self.auto_dnf = auto_dnf
+        assert encoding in ["auto", "unate-dnf", "bdd"]
+        self.auto_dnf = auto_dnf and encoding != "bdd"
+        self.encoding = encoding
+        self.try_unate_hard = try_unate_hard
+        self._is_unate = dict()
         super(MPBooleanNetwork, self).__init__(bn)
 
-    def formula_well_formed(self, f):
-        pos_lits = set()
-        neg_lits = set()
-        def is_lit(f):
-            if isinstance(f, self.ba.Symbol):
-                pos_lits.add(f.obj)
-                return True
-            if isinstance(f, self.ba.NOT) \
-                    and isinstance(f.args[0], self.ba.Symbol):
-                neg_lits.add(f.args[0].obj)
-                return True
-            return False
-
-        def is_clause(f):
-            if is_lit(f):
-                return True
-            if isinstance(f, self.ba.AND):
-                for g in f.args:
-                    if not is_lit(g):
-                        return False
-                return True
-            return False
-
-        def assert_monotonicity():
-            both = pos_lits.intersection(neg_lits)
-            assert not both, \
-                f"expression '{f}' contains literals with both signs ({both}). Try .simplify()?"
-
-        if f in [self.ba.TRUE, self.ba.FALSE]:
-            return True
-        if is_clause(f):
-            assert_monotonicity()
-            return True
-        if isinstance(f, self.ba.OR):
-            for g in f.args:
-                if not is_clause(g):
-                    return False
-            assert_monotonicity()
-            return True
-        return False
-
     def __setitem__(self, a, f):
         """
         Assigns the Boolean function ``f`` to component ``a``.
         Unless :py:attr:`.auto_dnf` is ``False``, ``f`` is converted into DNF
         form first.
         """
         if isinstance(f, str):
             f = self.ba.parse(f)
         f = self._autobool(f)
         if self.auto_dnf:
             f = self.ba.dnf(f).simplify()
-            f = minibn.simplify_dnf(self.ba, f)
-        assert self.formula_well_formed(f)
-        return super().__setitem__(self._autokey(a), f)
+            if self.try_unate_hard:
+                f = minibn.simplify_dnf(self.ba, f)
+        a = self._autokey(a)
+        if self.encoding != "bdd":
+            self._is_unate[a] = is_unate(self.ba, f)
+            if self.encoding == "unate-dnf":
+                assert self._is_unate[a], f"'{f}' seems not unate. Try simplify()?"
+        return super().__setitem__(a, f)
 
     def asp_of_bn(self):
         def clauses_of_dnf(f):
-            if f == self.ba.FALSE:
-                return [False]
-            if f == self.ba.TRUE:
-                return [True]
             if isinstance(f, boolean.OR):
                 return f.args
             else:
                 return [f]
-
         def literals_of_clause(c):
             def make_literal(l):
                 if isinstance(l, boolean.NOT):
                     return (l.args[0].obj, -1)
                 else:
                     return (l.obj, 1)
             lits = c.args if isinstance(c, boolean.AND) else [c]
             return map(make_literal, lits)
+        def encode_dnf(f):
+            facts = []
+            for cid, c in enumerate(clauses_of_dnf(f)):
+                for m, v in literals_of_clause(c):
+                    facts.append(" clause(\"{}\",{},\"{}\",{}).".format(n, cid, m, v))
+            return facts
 
         facts = []
         for n, f in self.items():
             facts.append("node(\"{}\").".format(n))
-            for cid, c in enumerate(clauses_of_dnf(f)):
-                facts.append("\n")
-                if isinstance(c, bool):
-                    facts.append(" constant(\"{}\",{}).".format(n, s2v(c)))
-                else:
-                    for m, v in literals_of_clause(c):
-                        facts.append(" clause(\"{}\",{},\"{}\",{}).".format(n, cid, m, v))
-            facts.append("\n")
+            if self.encoding == "bdd":
+                f_encoding = "bdd"
+            elif self.encoding == "unate-dnf":
+                f_encoding = "dnf"
+            else:
+                f_encoding = "dnf" if self._is_unate[n] else "bdd"
+            if f == self.ba.FALSE:
+                f = False
+            elif f == self.ba.TRUE:
+                f = True
+            if isinstance(f, bool):
+                facts.append(" constant(\"{}\",{}).".format(n, s2v(f)))
+            elif f_encoding == "dnf":
+                facts.extend(encode_dnf(f))
+            elif f_encoding == "bdd":
+                facts.append(bddasp_of_boolfunc(f, n))
         return "".join(facts)
 
     def asp_of_cfg(self, e, t, c):
         facts = ["timepoint({},{}).".format(e,t)]
         facts += [" mp_state({},{},\"{}\",{}).".format(e,t,n,s2v(s))
                     for (n,s) in c.items()]
         facts += [" 1 {{mp_state({},{},\"{}\",(-1;1))}} 1.".format(e,t,n)
```

### Comparing `mpbn-2.0/mpbn/cli/__init__.py` & `mpbn-3.0/mpbn/cli/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 import sys
 from argparse import ArgumentParser
 
 def main():
     ap = ArgumentParser(prog=sys.argv[0])
     ap.add_argument("bnet_file")
     ap.add_argument("method", choices=["attractors", "fixedpoints", "bn2asp"])
+    ap.add_argument("--encoding", default="auto", choices=["auto", "bdd", "unate-dnf"])
     ap.add_argument("--limit", type=int, default=0,
                     help="limit the number of results")
     args = ap.parse_args()
-    mbn = mpbn.MPBooleanNetwork(args.bnet_file)
+    mbn = mpbn.MPBooleanNetwork(args.bnet_file, encoding=args.encoding)
     if args.method == "attractors":
         for attractor in mbn.attractors(limit=args.limit):
             print(attractor)
     elif args.method == "fixedpoints":
         for attractor in mbn.fixedpoints(limit=args.limit):
             print(attractor)
     elif args.method == "bn2asp":
```

### Comparing `mpbn-2.0/mpbn/cli/sim.py` & `mpbn-3.0/mpbn/cli/sim.py`

 * *Files identical despite different names*

### Comparing `mpbn-2.0/mpbn/simulation.py` & `mpbn-3.0/mpbn/simulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import re
 
 BNET_SYMBOL_PAT = re.compile(r"[\w\.:]+")
 
 class MPBNSim(MPBooleanNetwork):
     def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs, encoding="unate-dnf")
         g = self.influence_graph()
         self.deps = {}
         for i in g:
             self.deps[i] = {1: [], -1: []}
         for (j, i, d) in g.edges(data=True):
             self.deps[i][d["sign"]].append(j)
         for i in g:
```

### Comparing `mpbn-2.0/mpbn.egg-info/PKG-INFO` & `mpbn-3.0/mpbn.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpbn
-Version: 2.0
+Version: 3.0
 Summary: Simple implementation of Most Permissive Boolean networks
 Home-page: https://github.com/bnediction/mpbn
 Author: Loïc Paulevé
 Author-email: loic.pauleve@labri.fr
 License: CeCILL
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `mpbn-2.0/setup.py` & `mpbn-3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 # -*- coding: utf-8
 
 from setuptools import setup, find_packages
 
 NAME = "mpbn"
-VERSION = "2.0"
+VERSION = "3.0"
 
 setup(name=NAME,
     version=VERSION,
     author="Loïc Paulevé",
     author_email="loic.pauleve@labri.fr",
     url="https://github.com/bnediction/mpbn",
     license="CeCILL",
@@ -23,14 +23,15 @@
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     install_requires=[
         "boolean.py",
         "clingo",
         "colomoto_jupyter>=0.8.0",
         "numpy",
+        "pyeda",
         "scipy",
         "tqdm"
     ],
     entry_points={
         "console_scripts": [
             "mpbn=mpbn.cli:main",
             "mpbn-sim=mpbn.cli.sim:main",
```

