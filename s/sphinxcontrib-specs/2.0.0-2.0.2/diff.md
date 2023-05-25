# Comparing `tmp/sphinxcontrib_specs-2.0.0.tar.gz` & `tmp/sphinxcontrib_specs-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxcontrib_specs-2.0.0.tar", max compression
+gzip compressed data, was "sphinxcontrib_specs-2.0.2.tar", max compression
```

## Comparing `sphinxcontrib_specs-2.0.0.tar` & `sphinxcontrib_specs-2.0.2.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0    15921 2023-01-10 21:23:41.840193 sphinxcontrib_specs-2.0.0/LICENSE
--rw-r--r--   0        0        0      655 2023-01-10 21:23:41.840193 sphinxcontrib_specs-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      866 2023-01-10 21:23:41.840193 sphinxcontrib_specs-2.0.0/src/sphinxcontrib/specs/__init__.py
--rw-r--r--   0        0        0     5740 2023-01-10 21:23:41.840193 sphinxcontrib_specs-2.0.0/src/sphinxcontrib/specs/admonitions/__init__.py
--rw-r--r--   0        0        0      452 2023-01-10 21:23:41.840193 sphinxcontrib_specs-2.0.0/src/sphinxcontrib/specs/builder.py
--rw-r--r--   0        0        0     6089 2023-01-10 21:23:41.840193 sphinxcontrib_specs-2.0.0/src/sphinxcontrib/specs/content.py
--rw-r--r--   0        0        0     4728 2023-01-10 21:23:41.840193 sphinxcontrib_specs-2.0.0/src/sphinxcontrib/specs/objectives.py
--rw-r--r--   0        0        0     2384 2023-01-10 21:23:41.840193 sphinxcontrib_specs-2.0.0/src/sphinxcontrib/specs/overridenodes.py
--rw-r--r--   0        0        0     4010 2023-01-10 21:23:41.840193 sphinxcontrib_specs-2.0.0/src/sphinxcontrib/specs/steps.py
--rw-r--r--   0        0        0     1610 2023-01-10 21:23:41.840193 sphinxcontrib_specs-2.0.0/src/sphinxcontrib/specs/theme/layout.html
--rw-r--r--   0        0        0      378 2023-01-10 21:23:41.840193 sphinxcontrib_specs-2.0.0/src/sphinxcontrib/specs/theme/page.html
--rw-r--r--   0        0        0     1496 2023-01-10 21:23:41.840193 sphinxcontrib_specs-2.0.0/src/sphinxcontrib/specs/theme/static/components.css
--rw-r--r--   0        0        0      992 2023-01-10 21:23:41.840193 sphinxcontrib_specs-2.0.0/src/sphinxcontrib/specs/theme/static/content.css
--rw-r--r--   0        0        0     5269 2023-01-10 21:23:41.840193 sphinxcontrib_specs-2.0.0/src/sphinxcontrib/specs/theme/static/layout.css
--rw-r--r--   0        0        0      903 2023-01-10 21:23:41.840193 sphinxcontrib_specs-2.0.0/src/sphinxcontrib/specs/theme/static/styles.css
--rw-r--r--   0        0        0       74 2023-01-10 21:23:41.840193 sphinxcontrib_specs-2.0.0/src/sphinxcontrib/specs/theme/theme.conf
--rw-r--r--   0        0        0      751 1970-01-01 00:00:00.000000 sphinxcontrib_specs-2.0.0/setup.py
--rw-r--r--   0        0        0      417 1970-01-01 00:00:00.000000 sphinxcontrib_specs-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0    15921 2023-05-25 23:16:16.877239 sphinxcontrib_specs-2.0.2/LICENSE
+-rw-r--r--   0        0        0      654 2023-05-25 23:16:16.881239 sphinxcontrib_specs-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0      866 2023-05-25 23:16:16.881239 sphinxcontrib_specs-2.0.2/src/sphinxcontrib/specs/__init__.py
+-rw-r--r--   0        0        0     5711 2023-05-25 23:16:16.881239 sphinxcontrib_specs-2.0.2/src/sphinxcontrib/specs/admonitions/__init__.py
+-rw-r--r--   0        0        0      452 2023-05-25 23:16:16.881239 sphinxcontrib_specs-2.0.2/src/sphinxcontrib/specs/builder.py
+-rw-r--r--   0        0        0     6089 2023-05-25 23:16:16.881239 sphinxcontrib_specs-2.0.2/src/sphinxcontrib/specs/content.py
+-rw-r--r--   0        0        0     4728 2023-05-25 23:16:16.881239 sphinxcontrib_specs-2.0.2/src/sphinxcontrib/specs/objectives.py
+-rw-r--r--   0        0        0     2384 2023-05-25 23:16:16.881239 sphinxcontrib_specs-2.0.2/src/sphinxcontrib/specs/overridenodes.py
+-rw-r--r--   0        0        0     4010 2023-05-25 23:16:16.881239 sphinxcontrib_specs-2.0.2/src/sphinxcontrib/specs/steps.py
+-rw-r--r--   0        0        0     1610 2023-05-25 23:16:16.881239 sphinxcontrib_specs-2.0.2/src/sphinxcontrib/specs/theme/layout.html
+-rw-r--r--   0        0        0      378 2023-05-25 23:16:16.881239 sphinxcontrib_specs-2.0.2/src/sphinxcontrib/specs/theme/page.html
+-rw-r--r--   0        0        0     1496 2023-05-25 23:16:16.881239 sphinxcontrib_specs-2.0.2/src/sphinxcontrib/specs/theme/static/components.css
+-rw-r--r--   0        0        0      992 2023-05-25 23:16:16.881239 sphinxcontrib_specs-2.0.2/src/sphinxcontrib/specs/theme/static/content.css
+-rw-r--r--   0        0        0     5269 2023-05-25 23:16:16.881239 sphinxcontrib_specs-2.0.2/src/sphinxcontrib/specs/theme/static/layout.css
+-rw-r--r--   0        0        0      903 2023-05-25 23:16:16.881239 sphinxcontrib_specs-2.0.2/src/sphinxcontrib/specs/theme/static/styles.css
+-rw-r--r--   0        0        0       74 2023-05-25 23:16:16.881239 sphinxcontrib_specs-2.0.2/src/sphinxcontrib/specs/theme/theme.conf
+-rw-r--r--   0        0        0      466 1970-01-01 00:00:00.000000 sphinxcontrib_specs-2.0.2/PKG-INFO
```

### Comparing `sphinxcontrib_specs-2.0.0/LICENSE` & `sphinxcontrib_specs-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_specs-2.0.0/pyproject.toml` & `sphinxcontrib_specs-2.0.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "sphinxcontrib-specs"
-version = "2.0.0"
+version = "2.0.2"
 description = "Extensions for building Specializations content."
 authors = ["Ashley Trinh <ashley@hackbrightacademy.com>"]
 license = "MPL-2.0"
 packages = [{ include = "sphinxcontrib", from = "src" }]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.9"
 
 [tool.poetry.dev-dependencies]
 black = "^22.6.0"
 pytest = "^7.1.2"
 mypy = "^0.961"
 html5lib = "^1.1"
 Sphinx = "^5.3"
```

### Comparing `sphinxcontrib_specs-2.0.0/src/sphinxcontrib/specs/__init__.py` & `sphinxcontrib_specs-2.0.2/src/sphinxcontrib/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_specs-2.0.0/src/sphinxcontrib/specs/admonitions/__init__.py` & `sphinxcontrib_specs-2.0.2/src/sphinxcontrib/specs/admonitions/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from typing import TYPE_CHECKING
 
+from docutils import nodes
 from docutils.parsers.rst.directives.admonitions import BaseAdmonition
 from docutils.parsers.rst.roles import set_classes
-from docutils import nodes
-
 from sphinx.writers.html5 import HTML5Translator
 
 if TYPE_CHECKING:
     from sphinx.application import Sphinx
 
 
 class OverrideAdmonition(BaseAdmonition):
@@ -39,55 +38,46 @@
 
         self.state.nested_parse(self.content, self.content_offset, admonition_node)
 
         return [admonition_node]
 
 
 class Attention(OverrideAdmonition):
-
     node_class = nodes.attention
 
 
 class Caution(OverrideAdmonition):
-
     node_class = nodes.caution
 
 
 class Danger(OverrideAdmonition):
-
     node_class = nodes.danger
 
 
 class Error(OverrideAdmonition):
-
     node_class = nodes.error
 
 
 class Hint(OverrideAdmonition):
-
     node_class = nodes.hint
 
 
 class Important(OverrideAdmonition):
-
     node_class = nodes.important
 
 
 class Note(OverrideAdmonition):
-
     node_class = nodes.note
 
 
 class Tip(OverrideAdmonition):
-
     node_class = nodes.tip
 
 
 class Warning(OverrideAdmonition):
-
     node_class = nodes.warning
 
 
 def visit_title(self, node: nodes.title):
     # Skip node if this is a title for a hint
     if isinstance(node.parent, nodes.hint) and node.parent.index(node) == 0:
         raise nodes.SkipNode
@@ -145,25 +135,24 @@
 
 def visit_note(self, node: nodes.note):
     visit_admonition(self, node, "note")
 
 
 def depart_hint(self, node: nodes.hint):
     self.body.append("</details>")
-
-    super(HTML5Translator, self).depart_hint(node)
+    depart_admonition(self, node)
 
 
 def visit_paragraph(self, node: nodes.paragraph):
     # For handling hints
     self.body.append(self.starttag(node, "p", CLASS=" ".join(node["classes"])))
 
 
 def depart_paragraph(self, node: nodes.paragraph):
-    super(HTML5Translator, self).depart_paragraph(node)
+    super(self.__class__, self).depart_paragraph(node)
 
     # For handling hints
     if "admonition-title" in node["classes"] and isinstance(node.parent, nodes.hint):
         self.body.append("<details>")
         self.body.append("<summary></summary>")
```

### Comparing `sphinxcontrib_specs-2.0.0/src/sphinxcontrib/specs/content.py` & `sphinxcontrib_specs-2.0.2/src/sphinxcontrib/specs/content.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_specs-2.0.0/src/sphinxcontrib/specs/objectives.py` & `sphinxcontrib_specs-2.0.2/src/sphinxcontrib/specs/objectives.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_specs-2.0.0/src/sphinxcontrib/specs/overridenodes.py` & `sphinxcontrib_specs-2.0.2/src/sphinxcontrib/specs/overridenodes.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_specs-2.0.0/src/sphinxcontrib/specs/steps.py` & `sphinxcontrib_specs-2.0.2/src/sphinxcontrib/specs/steps.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_specs-2.0.0/src/sphinxcontrib/specs/theme/layout.html` & `sphinxcontrib_specs-2.0.2/src/sphinxcontrib/specs/theme/layout.html`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_specs-2.0.0/src/sphinxcontrib/specs/theme/static/components.css` & `sphinxcontrib_specs-2.0.2/src/sphinxcontrib/specs/theme/static/components.css`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_specs-2.0.0/src/sphinxcontrib/specs/theme/static/content.css` & `sphinxcontrib_specs-2.0.2/src/sphinxcontrib/specs/theme/static/content.css`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_specs-2.0.0/src/sphinxcontrib/specs/theme/static/layout.css` & `sphinxcontrib_specs-2.0.2/src/sphinxcontrib/specs/theme/static/layout.css`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_specs-2.0.0/src/sphinxcontrib/specs/theme/static/styles.css` & `sphinxcontrib_specs-2.0.2/src/sphinxcontrib/specs/theme/static/styles.css`

 * *Files identical despite different names*

