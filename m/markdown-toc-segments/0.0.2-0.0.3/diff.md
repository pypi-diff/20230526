# Comparing `tmp/markdown_toc_segments-0.0.2.tar.gz` & `tmp/markdown_toc_segments-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown_toc_segments-0.0.2.tar", max compression
+gzip compressed data, was "markdown_toc_segments-0.0.3.tar", max compression
```

## Comparing `markdown_toc_segments-0.0.2.tar` & `markdown_toc_segments-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     6130 2023-05-26 12:30:25.668727 markdown_toc_segments-0.0.2/README.md
--rw-r--r--   0        0        0      138 2023-05-26 12:30:58.695157 markdown_toc_segments-0.0.2/markdown_toc_segments/__init__.py
--rw-r--r--   0        0        0      358 2023-05-26 10:26:27.753009 markdown_toc_segments-0.0.2/markdown_toc_segments/footnote.py
--rw-r--r--   0        0        0     1775 2023-05-26 12:24:30.304012 markdown_toc_segments-0.0.2/markdown_toc_segments/main.py
--rw-r--r--   0        0        0     3235 2023-05-26 12:24:28.869101 markdown_toc_segments-0.0.2/markdown_toc_segments/segment.py
--rw-r--r--   0        0        0      333 2023-05-26 11:19:36.097115 markdown_toc_segments-0.0.2/markdown_toc_segments/utils.py
--rw-r--r--   0        0        0     1100 2023-05-26 12:31:35.163154 markdown_toc_segments-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     6830 1970-01-01 00:00:00.000000 markdown_toc_segments-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     6131 2023-05-26 13:53:52.389529 markdown_toc_segments-0.0.3/README.md
+-rw-r--r--   0        0        0      138 2023-05-26 12:30:58.695157 markdown_toc_segments-0.0.3/markdown_toc_segments/__init__.py
+-rw-r--r--   0        0        0      358 2023-05-26 10:26:27.753009 markdown_toc_segments-0.0.3/markdown_toc_segments/footnote.py
+-rw-r--r--   0        0        0     3505 2023-05-26 13:57:59.627945 markdown_toc_segments-0.0.3/markdown_toc_segments/main.py
+-rw-r--r--   0        0        0     3235 2023-05-26 12:24:28.869101 markdown_toc_segments-0.0.3/markdown_toc_segments/segment.py
+-rw-r--r--   0        0        0      333 2023-05-26 11:19:36.097115 markdown_toc_segments-0.0.3/markdown_toc_segments/utils.py
+-rw-r--r--   0        0        0     1100 2023-05-26 13:58:34.582505 markdown_toc_segments-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6831 1970-01-01 00:00:00.000000 markdown_toc_segments-0.0.3/PKG-INFO
```

### Comparing `markdown_toc_segments-0.0.2/README.md` & `markdown_toc_segments-0.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  [Segment(id='ponencia', markup='<p>This is a sample decision written in markdown to illustrate the ability to compartamentalize text.<sup id="fnref:1"><a class="footnote-ref" href="#fn:1">1</a></sup></p>'),
  Segment(id='antecedents', markup='<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit,<sup id="fnref:2"><a class="footnote-ref" href="#fn:2">2</a></sup> sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat<sup id="fnref:3"><a class="footnote-ref" href="#fn:3">3</a></sup> nulla pariatur. Excepteur sint occaecat cupidatat non proident,<sup id="fnref:4"><a class="footnote-ref" href="#fn:4">4</a></sup> sunt in culpa qui officia deserunt mollit anim id est laborum.</p>'),
  Segment(id='version-of-the-defense', markup='<p>XXX</p>'),
 ...
  Segment(id='the-courts-ruling', markup='<p>The Court dismisses the appeal.</p>'),
  Segment(id='this-is-a-proper-headline', markup='<p>XXXX</p>'),
 ...]
->>> obj.toc
+>>> obj.tree
 [
   Item(
     id='ponencia',
     label='Ponencia',
     segment=Segment(id='ponencia', markup='<p>This is a sample decision written in markdown to illustrate the ability to compartamentalize text.<sup id="fnref:1"><a class="footnote-ref" href="#fn:1">1</a></sup></p>'),
     text='This is a sample decision written in markdown to illustrate the ability to compartamentalize text.%% I am no footnote %%',
     children=[
```

### Comparing `markdown_toc_segments-0.0.2/markdown_toc_segments/segment.py` & `markdown_toc_segments-0.0.3/markdown_toc_segments/segment.py`

 * *Files identical despite different names*

### Comparing `markdown_toc_segments-0.0.2/pyproject.toml` & `markdown_toc_segments-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "markdown-toc-segments"
 description = "Create markdown segments based on a table of contents"
-version = "0.0.2"
+version = "0.0.3"
 authors = ["Marcelino G. Veloso III <mars@veloso.one>"]
 readme = "README.md"
 homepage = "https://mv3.dev"
 repository = "https://github.com/justmars/markdown-toc-segments"
 classifiers = [
   "Programming Language :: Python :: 3.11",
   "Typing :: Typed",
```

### Comparing `markdown_toc_segments-0.0.2/PKG-INFO` & `markdown_toc_segments-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdown-toc-segments
-Version: 0.0.2
+Version: 0.0.3
 Summary: Create markdown segments based on a table of contents
 Home-page: https://mv3.dev
 Author: Marcelino G. Veloso III
 Author-email: mars@veloso.one
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
@@ -40,15 +40,15 @@
  [Segment(id='ponencia', markup='<p>This is a sample decision written in markdown to illustrate the ability to compartamentalize text.<sup id="fnref:1"><a class="footnote-ref" href="#fn:1">1</a></sup></p>'),
  Segment(id='antecedents', markup='<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit,<sup id="fnref:2"><a class="footnote-ref" href="#fn:2">2</a></sup> sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat<sup id="fnref:3"><a class="footnote-ref" href="#fn:3">3</a></sup> nulla pariatur. Excepteur sint occaecat cupidatat non proident,<sup id="fnref:4"><a class="footnote-ref" href="#fn:4">4</a></sup> sunt in culpa qui officia deserunt mollit anim id est laborum.</p>'),
  Segment(id='version-of-the-defense', markup='<p>XXX</p>'),
 ...
  Segment(id='the-courts-ruling', markup='<p>The Court dismisses the appeal.</p>'),
  Segment(id='this-is-a-proper-headline', markup='<p>XXXX</p>'),
 ...]
->>> obj.toc
+>>> obj.tree
 [
   Item(
     id='ponencia',
     label='Ponencia',
     segment=Segment(id='ponencia', markup='<p>This is a sample decision written in markdown to illustrate the ability to compartamentalize text.<sup id="fnref:1"><a class="footnote-ref" href="#fn:1">1</a></sup></p>'),
     text='This is a sample decision written in markdown to illustrate the ability to compartamentalize text.%% I am no footnote %%',
     children=[
```

