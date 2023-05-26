# Comparing `tmp/Report-Ranger-1.0.tar.gz` & `tmp/Report-Ranger-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Report-Ranger-1.0.tar", max compression
+gzip compressed data, was "Report-Ranger-2.0.tar", max compression
```

## Comparing `Report-Ranger-1.0.tar` & `Report-Ranger-2.0.tar`

### file list

```diff
@@ -1,25 +1,32 @@
--rw-r--r--   0        0        0      387 2022-06-10 06:13:41.955374 Report-Ranger-1.0/pyproject.toml
--rw-r--r--   0        0        0       32 2022-02-15 04:42:40.568200 Report-Ranger-1.0/report_ranger/__init__.py
--rw-r--r--   0        0        0      636 2022-05-23 04:19:45.460680 Report-Ranger-1.0/report_ranger/config.py
--rw-r--r--   0        0        0     6263 2022-02-15 04:42:40.568200 Report-Ranger-1.0/report_ranger/contentassistant.py
--rw-r--r--   0        0        0     3668 2022-05-13 06:02:17.792202 Report-Ranger-1.0/report_ranger/csvformatter.py
--rw-r--r--   0        0        0     3104 2022-02-15 04:42:40.568200 Report-Ranger-1.0/report_ranger/csvrenderer.py
--rw-r--r--   0        0        0     3094 2022-02-15 04:42:40.568200 Report-Ranger-1.0/report_ranger/environment.py
--rw-r--r--   0        0        0      217 2022-02-15 04:42:40.568200 Report-Ranger-1.0/report_ranger/errors.py
--rw-r--r--   0        0        0    11380 2022-06-10 05:10:42.802660 Report-Ranger-1.0/report_ranger/helpers.py
--rw-r--r--   0        0        0     4362 2022-05-13 06:02:17.792202 Report-Ranger-1.0/report_ranger/htmlformatter.py
--rw-r--r--   0        0        0     2891 2022-06-10 05:10:42.802660 Report-Ranger-1.0/report_ranger/imports.py
--rw-r--r--   0        0        0    16947 2022-06-10 05:10:42.802660 Report-Ranger-1.0/report_ranger/latexformatter.py
--rw-r--r--   0        0        0     5841 2022-06-10 05:10:42.802660 Report-Ranger-1.0/report_ranger/latexrenderer.py
--rw-r--r--   0        0        0    12117 2022-05-13 06:02:17.792202 Report-Ranger-1.0/report_ranger/mdread.py
--rw-r--r--   0        0        0    30659 2022-06-10 05:10:42.802660 Report-Ranger-1.0/report_ranger/outputformatter.py
--rw-r--r--   0        0        0     4007 2022-05-23 04:19:45.484025 Report-Ranger-1.0/report_ranger/report_ranger.py
--rw-r--r--   0        0        0     8277 2022-02-15 04:42:40.568200 Report-Ranger-1.0/report_ranger/riskassessment.py
--rw-r--r--   0        0        0     3814 2022-05-13 06:02:17.792202 Report-Ranger-1.0/report_ranger/section.py
--rw-r--r--   0        0        0     2904 2022-06-10 05:10:42.802660 Report-Ranger-1.0/report_ranger/styles.py
--rw-r--r--   0        0        0    17483 2022-06-10 05:10:42.802660 Report-Ranger-1.0/report_ranger/table.py
--rw-r--r--   0        0        0    17094 2022-05-17 05:55:31.304798 Report-Ranger-1.0/report_ranger/template.py
--rw-r--r--   0        0        0     1138 2022-05-13 06:02:17.792202 Report-Ranger-1.0/report_ranger/validation.py
--rw-r--r--   0        0        0    18456 2022-05-13 06:02:17.792202 Report-Ranger-1.0/report_ranger/vulnerability.py
--rw-r--r--   0        0        0      722 2022-06-10 06:14:06.369396 Report-Ranger-1.0/setup.py
--rw-r--r--   0        0        0      536 2022-06-10 06:14:06.369620 Report-Ranger-1.0/PKG-INFO
+-rwxr-xr-x   0        0        0      463 2023-05-26 00:14:23.375274 Report-Ranger-2.0/pyproject.toml
+-rwxr-xr-x   0        0        0       33 2021-09-15 13:25:33.000000 Report-Ranger-2.0/report_ranger/__init__.py
+-rwxr-xr-x   0        0        0     1064 2023-04-24 00:31:02.414450 Report-Ranger-2.0/report_ranger/config.py
+-rwxr-xr-x   0        0        0     8812 2023-05-02 03:51:52.380891 Report-Ranger-2.0/report_ranger/contentassistant.py
+-rwxr-xr-x   0        0        0     3806 2023-05-02 06:44:16.057745 Report-Ranger-2.0/report_ranger/environment.py
+-rwxr-xr-x   0        0        0      217 2021-09-15 13:25:33.000000 Report-Ranger-2.0/report_ranger/errors.py
+-rwxr-xr-x   0        0        0    12991 2023-04-13 07:20:23.609912 Report-Ranger-2.0/report_ranger/helpers.py
+-rwxr-xr-x   0        0        0     3034 2023-03-23 05:17:42.138978 Report-Ranger-2.0/report_ranger/imports/imports.py
+-rwxr-xr-x   0        0        0     4473 2023-05-23 22:45:26.028951 Report-Ranger-2.0/report_ranger/imports/section.py
+-rwxr-xr-x   0        0        0    20287 2023-05-23 07:27:07.987448 Report-Ranger-2.0/report_ranger/imports/vulnerability.py
+-rwxr-xr-x   0        0        0     3210 2023-03-23 05:17:42.140109 Report-Ranger-2.0/report_ranger/markdown_renderer/csvrenderer.py
+-rwxr-xr-x   0        0        0     4266 2023-04-28 02:59:32.119136 Report-Ranger-2.0/report_ranger/markdown_renderer/latexrenderer.py
+-rwxr-xr-x   0        0        0     2682 2023-04-29 06:11:16.074523 Report-Ranger-2.0/report_ranger/markdown_renderer/typstrenderer.py
+-rwxr-xr-x   0        0        0     3810 2023-05-23 07:19:00.069356 Report-Ranger-2.0/report_ranger/output_formatter/csvformatter.py
+-rwxr-xr-x   0        0        0     1336 2023-05-23 07:18:57.380497 Report-Ranger-2.0/report_ranger/output_formatter/docxformatter.py
+-rwxr-xr-x   0        0        0     4519 2023-05-23 07:18:54.540800 Report-Ranger-2.0/report_ranger/output_formatter/htmlformatter.py
+-rwxr-xr-x   0        0        0    20061 2023-05-23 07:18:51.519431 Report-Ranger-2.0/report_ranger/output_formatter/latexformatter.py
+-rwxr-xr-x   0        0        0    32470 2023-05-24 01:30:53.846118 Report-Ranger-2.0/report_ranger/output_formatter/outputformatter.py
+-rwxr-xr-x   0        0        0     5764 2023-05-23 07:19:04.716847 Report-Ranger-2.0/report_ranger/output_formatter/typstformatter.py
+-rwxr-xr-x   0        0        0    11488 2023-05-24 01:37:48.702425 Report-Ranger-2.0/report_ranger/report.py
+-rwxr-xr-x   0        0        0     7227 2023-05-23 22:42:30.650688 Report-Ranger-2.0/report_ranger/report_ranger.py
+-rwxr-xr-x   0        0        0     8290 2023-03-23 05:17:42.147623 Report-Ranger-2.0/report_ranger/riskassessment.py
+-rwxr-xr-x   0        0        0     3019 2022-05-27 05:01:58.000000 Report-Ranger-2.0/report_ranger/styles.py
+-rwxr-xr-x   0        0        0    19313 2023-03-23 05:17:42.148620 Report-Ranger-2.0/report_ranger/table.py
+-rwxr-xr-x   0        0        0     1442 2023-05-02 06:37:25.929867 Report-Ranger-2.0/report_ranger/template.py
+-rwxr-xr-x   0        0        0     2119 2023-03-23 05:17:42.150976 Report-Ranger-2.0/report_ranger/templatemapper.py
+-rwxr-xr-x   0        0        0      555 2023-04-28 02:54:06.713280 Report-Ranger-2.0/report_ranger/utils/jinja_helpers.py
+-rwxr-xr-x   0        0        0    20774 2023-05-24 08:00:56.417779 Report-Ranger-2.0/report_ranger/utils/mdread.py
+-rwxr-xr-x   0        0        0     1138 2022-05-27 05:01:58.000000 Report-Ranger-2.0/report_ranger/validation.py
+-rwxr-xr-x   0        0        0     2833 2023-05-23 22:43:39.663890 Report-Ranger-2.0/report_ranger/watcher.py
+-rw-r--r--   0        0        0      893 2023-05-26 00:27:34.070409 Report-Ranger-2.0/setup.py
+-rw-r--r--   0        0        0      597 2023-05-26 00:27:34.070641 Report-Ranger-2.0/PKG-INFO
```

### Comparing `Report-Ranger-1.0/report_ranger/contentassistant.py` & `Report-Ranger-2.0/report_ranger/contentassistant.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,22 +3,26 @@
 import logging
 
 log = logging.getLogger(__name__)
 
 
 class ContentAssistant:
     def __init__(self):
+        self.defaulticounter = None
+        self.icounters = {}
         self.defaultcounter = 0
         self.counters = {}
         self.defaulttable = []
         self.tables = {}
         self._register = {}
+        self._string_register = {}
         self._table_register = {}  # For holding table formatting
+        self._function_register = {} # For holding simple function calls
 
-    def _display_table(self, of, tablename="", *args, **kwargs):
+    def _display_table(self, uuid, markdown, of, tablename="", *args, **kwargs):
         """ Display a table from
         """
         if tablename == "":
             table = self.defaulttable
         elif not isinstance(tablename, str):
             log.warn(
                 "CA table name you're trying to display to is not a string, skipping: {}".format(tablename))
@@ -26,15 +30,41 @@
         elif tablename not in self.tables:
             log.warning(
                 "Table {} has not had any rows added to it. Skipping the display of this table.".format(tablename))
             return ""
         else:
             table = self.tables[tablename]
 
-        return of.table(table, *args, **kwargs)
+        return markdown.replace(uuid, of.table(table, *args, **kwargs))
+
+    def _display_icounter(self, uuid, markdown, of):
+        """ Convert the counter UUIDs in the document to numbers.
+        """
+        searchre = re.compile("(x|y|z){}".format(uuid))
+        counter = 0
+        max = 10000
+        while max > 0:
+            max -= 1
+            match = searchre.search(markdown)
+            if match == None:
+                return markdown
+            if(match.group()[0]) == 'x':
+                counter += 1
+            if(match.group()[0]) == 'z':
+                counter = 0
+                markdown = searchre.sub("", markdown, 1)
+            else:
+                markdown = searchre.sub(str(counter), markdown, 1)
+        log.warn("Max counter size of 10000 reached.")
+        return markdown
+    
+    def _register_string(self, string):
+        newuuid = str(uuid4())
+        self._string_register[newuuid] = string
+        return newuuid
 
     def _register_ca(self, function, *args, **kwargs):
         """ Add a function to the register. This can be called later so that we can display content on the second pass
         """
         newuuid = str(uuid4())
         self._register[newuuid] = {
             'function': function, 'args': args, 'kwargs': kwargs}
@@ -50,20 +80,20 @@
     def parse_register(self, of, markdown):
         """ Go through the register and print out the results of the functions
         """
         log.info("Adding Content Assistant content")
 
         # CA register
         for uuid, f in self._register.items():
-            output = f['function'](
-                of, *f['args'], **f['kwargs'])
-            markdown = markdown.replace(uuid, output)
+            markdown = f['function'](
+                uuid, markdown, of, *f['args'], **f['kwargs'])
 
+        # Now to go through calls to ft(). The below code will replace the markdown table with a table() call.
         t_r_row = r'\|?([^\|\r\n]+\|)+[^\|\r\n]*'
-        t_r_header_sep = r'\|?(\:?\s+-+\s*\:?\s*\|)*\s*'
+        t_r_header_sep = r'\|?(\:?\s+-+\s*\:?\s*\|)*'
         table_regex = r'[\r\s\n]*((' + t_r_row + \
             r')?[\r\s\n]*(' + t_r_header_sep + \
             r')?([\r\s\n]*' + t_r_row + ')+)'
 
         # Table register
         for uuid, f in self._table_register.items():
             m = re.search(uuid + table_regex, markdown)
@@ -74,55 +104,86 @@
                 continue
             table_markdown = m.group(1)
             table_output = of.table(table_markdown, *f['args'], **f['kwargs'])
             start, end = m.span()
             markdown = markdown[:start] + \
                 table_output + markdown[end:]
 
+        # String register
+        if len(self._string_register) > 0:
+            regex = re.compile('|'.join(re.escape(str(key)) for key in sorted(
+                self._string_register.keys(), key=lambda item: - len(item))))
+            markdown = regex.sub(lambda match: self._string_register[match.group()], markdown)
+
         return markdown
 
-    def counter(self, countername=""):
+    def icounter(self, countername="", mode="x"):
         """ This function allows counters throughout the document. Multiple counters can be used by specifying counter names.
         """
+        if mode not in ['x', 'y', 'z']:
+            log.warn("Unknown mode for icounter {}".format(countername))
+            return ""
+
         if countername == "":
-            self.defaultcounter += 1
-            return self.defaultcounter
+            if self.defaulticounter == None:
+                self.defaulticounter = self._register_ca(
+                    self._display_icounter)
+            return "{}{}".format(mode, self.defaulticounter)
+
         elif not isinstance(countername, str):
             log.warn("Counter name not a string: {}".format(countername))
             return 0
         else:
-            if countername not in self.counters:
-                self.counters[countername] = 1
-                return 1
-            self.counters[countername] += 1
-            return self.counters[countername]
+            if countername not in self.icounters:
+                self.icounters[countername] = self._register_ca(
+                    self._display_icounter)
+            return "{}{}".format(mode, self.icounters[countername])
 
-    def get_counter(self, countername=""):
+    def get_icounter(self, countername=""):
         """ This function retrieves the value of the counter WITHOUT iterating it.
         """
+        return self.icounter(countername, "y")
+
+    def reset_icounter(self, countername=""):
+        return self.icounter(countername, "z")
+
+    def counter(self, countername="", iterate=True):
+        """ This function allows counters throughout the document. Multiple counters can be used by specifying counter names.
+        """
+
         if countername == "":
+            if iterate:
+                self.defaultcounter += 1
             return self.defaultcounter
         elif not isinstance(countername, str):
             log.warn("Counter name not a string: {}".format(countername))
             return 0
         else:
             if countername not in self.counters:
-                return 0
+                self.counters[countername] = 0
+            if iterate:
+                self.counters[countername] += 1
             return self.counters[countername]
 
+    def get_counter(self, countername=""):
+        """ This function retrieves the value of the counter WITHOUT iterating it.
+        """
+        return self.counter(countername, False)
+
     def reset_counter(self, countername=""):
         """ Reset a counter to 0
         """
         if countername == "":
             self.defaultcounter = 0
         elif not isinstance(countername, str):
             log.warn(
                 "Counter name you're trying to reset is not a string, skipping: {}".format(countername))
         else:
             self.counters[countername] = 0
+        return ""
 
     def table_row(self, tablename="", row=[]):
         """ Add a row to a content assistant table, which can then be displayed with display_table
         """
         if tablename == "":
             self.defaulttable.append(row)
         elif not isinstance(tablename, str):
```

### Comparing `Report-Ranger-1.0/report_ranger/csvrenderer.py` & `Report-Ranger-2.0/report_ranger/markdown_renderer/csvrenderer.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,106 +1,106 @@
-import mistune
-import re
-
-
-class CSVRenderer(mistune.HTMLRenderer):
-    NAME = 'csv'
-    IS_TREE = False
-
-    # This set of data structures is a bit 'special'.
-    #
-    # We want the template to be able to refer to headings and get all the text from under that header. Usually you could do this with a tree, but
-    # I chose a different way here. Instead of a tree, it has a dict and a list. The dict gives the headings from every level and the list gives the current
-    # headings in play. When the renderer gets a new piece of text, it adds it to all the headings currently in play. This means it's very easy to get
-    # and refer to all the text from the headings without having to traverse a tree.
-
-    def _add_text(self, text):
-
-        for heading in self.heading_levels:
-            if heading != '' and heading in self.heading_text:
-                self.heading_text[heading] += text
-
-    def heading(self, text, level):
-        # This is brought to the top as it relates to the above heading structures
-
-        if len(self.heading_levels) < level:
-            self.heading_levels += [''] * \
-                (level - len(self.heading_levels)) + [text]
-        else:
-            self.heading_levels = self.heading_levels[:level - 1] + [text]
-
-        for heading in self.heading_levels[-1:]:
-            if heading != '' and heading in self.heading_text:
-                self.heading_text[heading] += '#' * level + ' ' + text
-
-        self.heading_text[text] = ''
-
-        return '#' * level + ' ' + text
-
-    def __init__(self, escape=True):
-        self.heading_levels = []  # The current headings in play
-        self.heading_text = {}  # The current heading text
-        super(CSVRenderer, self).__init__()
-
-    def text(self, text):
-        return text
-
-    def link(self, link, text=None, title=None):
-        self._add_text(text)
-        return text
-
-    def image(self, src, alt="", title=None):
-        self._add_text(alt)
-        return alt
-
-    def emphasis(self, text):
-        self._add_text(text)
-        return text
-
-    def strong(self, text):
-        self._add_text(text)
-        return text
-
-    def codespan(self, text):
-        self._add_text(text)
-        return text
-
-    def linebreak(self):
-        self._add_text('\n\n')
-        return '\n\n'
-
-    def inline_html(self, html):
-        self._add_text(self._escape_csv(html))
-        return self._escape_csv(html)
-
-    def paragraph(self, text):
-        self._add_text(text + '\n\n')
-        return text + '\n\n'
-
-    def newline(self):
-        self._add_text('\n\n')
-        return '\n\n'
-
-    def thematic_break(self):
-        # TODO NO THEMATIC BREAK
-        return '\n\n'
-
-    def block_text(self, text):
-        return text
-
-    def block_code(self, code, info=None):
-        return code
-
-    def block_quote(self, text):
-        return text
-
-    def block_html(self, html):
-        return html
-
-    def block_error(self, html):
-        return html
-
-    def list(self, text, ordered, level, start=None):
-        return text
-
-    def list_item(self, text, level):
-        return '  ' * level + '- ' + text + '\n'
+import mistune
+import re
+
+
+class CSVRenderer(mistune.HTMLRenderer):
+    NAME = 'csv'
+    IS_TREE = False
+
+    # This set of data structures is a bit 'special'.
+    #
+    # We want the template to be able to refer to headings and get all the text from under that header. Usually you could do this with a tree, but
+    # I chose a different way here. Instead of a tree, it has a dict and a list. The dict gives the headings from every level and the list gives the current
+    # headings in play. When the renderer gets a new piece of text, it adds it to all the headings currently in play. This means it's very easy to get
+    # and refer to all the text from the headings without having to traverse a tree.
+
+    def _add_text(self, text):
+
+        for heading in self.heading_levels:
+            if heading != '' and heading in self.heading_text:
+                self.heading_text[heading] += text
+
+    def heading(self, text, level):
+        # This is brought to the top as it relates to the above heading structures
+
+        if len(self.heading_levels) < level:
+            self.heading_levels += [''] * \
+                (level - len(self.heading_levels)) + [text]
+        else:
+            self.heading_levels = self.heading_levels[:level - 1] + [text]
+
+        for heading in self.heading_levels[-1:]:
+            if heading != '' and heading in self.heading_text:
+                self.heading_text[heading] += '#' * level + ' ' + text
+
+        self.heading_text[text] = ''
+
+        return '#' * level + ' ' + text
+
+    def __init__(self, escape=True):
+        self.heading_levels = []  # The current headings in play
+        self.heading_text = {}  # The current heading text
+        super(CSVRenderer, self).__init__()
+
+    def text(self, text):
+        return text
+
+    def link(self, link, text=None, title=None):
+        self._add_text(text)
+        return text
+
+    def image(self, src, alt="", title=None):
+        self._add_text(alt)
+        return alt
+
+    def emphasis(self, text):
+        self._add_text(text)
+        return text
+
+    def strong(self, text):
+        self._add_text(text)
+        return text
+
+    def codespan(self, text):
+        self._add_text(text)
+        return text
+
+    def linebreak(self):
+        self._add_text('\n\n')
+        return '\n\n'
+
+    def inline_html(self, html):
+        self._add_text(self._escape_csv(html))
+        return self._escape_csv(html)
+
+    def paragraph(self, text):
+        self._add_text(text + '\n\n')
+        return text + '\n\n'
+
+    def newline(self):
+        self._add_text('\n\n')
+        return '\n\n'
+
+    def thematic_break(self):
+        # TODO NO THEMATIC BREAK
+        return '\n\n'
+
+    def block_text(self, text):
+        return text
+
+    def block_code(self, code, info=None):
+        return code
+
+    def block_quote(self, text):
+        return text
+
+    def block_html(self, html):
+        return html
+
+    def block_error(self, html):
+        return html
+
+    def list(self, text, ordered, level, start=None):
+        return text
+
+    def list_item(self, text, level):
+        return '  ' * level + '- ' + text + '\n'
```

### Comparing `Report-Ranger-1.0/report_ranger/imports.py` & `Report-Ranger-2.0/report_ranger/imports/imports.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,101 +1,102 @@
-import os
-from pathlib import Path
-import logging
-import csv
-import traceback
-import copy
-
-try:
-    from openpyxl import load_workbook
-    openpyxl_imported = True
-except ImportError:
-    openpyxl_imported = False
-
-log = logging.getLogger(__name__)
-
-
-def import_csv(csvfile, as_dict_list=False, index_col=None):
-    filepath = Path(csvfile)
-    cwdpath = Path(os.path.curdir)
-    if cwdpath not in filepath.parents:
-        log.warning(
-            "import_csv figure path {} doesn't seem to be in cwd".format(csvfile))
-        return ''
-
-    try:
-        with open(filepath) as csvfile:
-            reader = csv.reader(csvfile)
-            return make_structure(reader, as_dict_list, index_col)
-    except Exception as e:
-        log.warning(
-            "Error opening CSV file {}: {}".format(csvfile, e.args))
-        return ''
-
-
-def import_xlsx(fp, worksheet=None, min_row=None, max_row=None, min_col=None, max_col=None, as_dict_list=False, index_col=None):
-    if not openpyxl_imported:
-        log.warning(
-            "Unsuccessful loading of openpyxl, skipping import of XLSX file")
-        return []
-    filepath = Path(fp)
-    cwdpath = Path(os.path.curdir)
-    if cwdpath not in filepath.parents:
-        log.warning(
-            "import_xlsx path {} doesn't seem to be in cwd".format(fp))
-        return ''
-
-    try:
-        workbook = load_workbook(filename=fp)
-        if worksheet:
-            sheet = workbook[worksheet]
-        else:
-            sheet = workbook.active
-
-        row_iterator = sheet.iter_rows(
-            min_row, max_row, min_col, max_col, values_only=True)
-        return make_structure(row_iterator, as_dict_list, index_col)
-    except Exception as e:
-        log.warning(
-            "error importing XLSX file {}: {}".format(fp, e.args))
-        log.warn(traceback.format_exc())
-
-        return ''
-
-
-def make_structure(row_iterator, as_dict_list=False, index_col=None):
-    # Let's just make 0 and 1 the same thing for simplicity and less user errors
-    if index_col == 0:
-        index_col = 1
-
-    if index_col:
-        results = {}
-    else:
-        results = []
-
-    headings = []
-    for row in row_iterator:
-        # Make sure row is a list and not a tuple
-        row = copy.deepcopy(list(row))
-
-        # We need to store the headings to use as keys in our dicts.
-        if as_dict_list and len(headings) < 1:
-            headings = row
-            continue
-
-        # Turn this row into a dict, rather than a list.
-        if as_dict_list:
-            new_item = {}
-            i = 0
-            for key in headings:
-                new_item[key] = row[i]
-                i += 1
-        else:
-            new_item = row
-
-        # We either create a new key/value pair or add the item to the list
-        if index_col:
-            results[row[index_col-1]] = new_item
-        else:
-            results.append(new_item)
-
-    return results
+import os
+from pathlib import Path
+import logging
+import csv
+import traceback
+import copy
+
+try:
+    from openpyxl import load_workbook
+    openpyxl_imported = True
+except ImportError:
+    openpyxl_imported = False
+
+log = logging.getLogger(__name__)
+
+
+def import_csv(csvfile, as_dict_list=False, index_col=None):
+    filepath = Path(csvfile)
+    cwdpath = Path(os.path.curdir)
+    if cwdpath not in filepath.parents:
+        log.warning(
+            "import_csv figure path {} doesn't seem to be in cwd".format(csvfile))
+        return ''
+
+    try:
+        with open(filepath) as csvfileopen:
+            reader = csv.reader(csvfileopen)
+            return make_structure(reader, as_dict_list, index_col)
+    except Exception as e:
+        log.warning(
+            "Error opening CSV file {}: {}".format(filepath, e.args))
+        return ''
+
+
+def import_xlsx(fp, worksheet=None, min_row=None, max_row=None, min_col=None, max_col=None, as_dict_list=False, index_col=None):
+    log.info(f"Importing {fp}")
+    if not openpyxl_imported:
+        log.warning(
+            "Unsuccessful loading of openpyxl, skipping import of XLSX file")
+        return []
+    filepath = Path(fp)
+    cwdpath = Path(os.path.curdir)
+    if cwdpath not in filepath.parents:
+        log.warning(
+            "import_xlsx path {} doesn't seem to be in cwd".format(fp))
+        return ''
+
+    try:
+        workbook = load_workbook(filename=fp)
+        if worksheet:
+            sheet = workbook[worksheet]
+        else:
+            sheet = workbook.active
+
+        row_iterator = sheet.iter_rows(
+            min_row, max_row, min_col, max_col, values_only=True)
+        return make_structure(row_iterator, as_dict_list, index_col)
+    except Exception as e:
+        log.warning(
+            "error importing XLSX file {}: {}".format(fp, e.args))
+        log.warn(traceback.format_exc())
+
+        return ''
+
+
+def make_structure(row_iterator, as_dict_list=False, index_col=None):
+    # Let's just make 0 and 1 the same thing for simplicity and less user errors
+    if index_col == 0:
+        index_col = 1
+
+    if index_col:
+        results = {}
+    else:
+        results = []
+
+    headings = []
+    for row in row_iterator:
+        # Make sure row is a list and not a tuple
+        row = copy.deepcopy(list(row))
+
+        # We need to store the headings to use as keys in our dicts.
+        if as_dict_list and len(headings) < 1:
+            headings = row
+            continue
+
+        # Turn this row into a dict, rather than a list.
+        if as_dict_list:
+            new_item = {}
+            i = 0
+            for key in headings:
+                new_item[key] = row[i]
+                i += 1
+        else:
+            new_item = row
+
+        # We either create a new key/value pair or add the item to the list
+        if index_col:
+            results[row[index_col-1]] = new_item
+        else:
+            results.append(new_item)
+
+    return results
```

### Comparing `Report-Ranger-1.0/report_ranger/latexformatter.py` & `Report-Ranger-2.0/report_ranger/output_formatter/latexformatter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,26 @@
-from .outputformatter import OutputFormatter, headeralias
+from report_ranger.output_formatter.outputformatter import OutputFormatter, headeralias
 import re
 import os
 import yaml
+import jinja2
 import mistune
-from .latexrenderer import LatexTableRenderer
-from .table import Table
+from report_ranger.markdown_renderer.latexrenderer import LatexTableRenderer
+from report_ranger.table import Table
 import subprocess
 import logging
+from report_ranger.utils.mdread import process_template
+
 
 log = logging.getLogger(__name__)
 
 default_latex = {'title': '{{title}}',
                  'author': '[Author Name]',
                  'date': '{{date.strftime("%-d %B %Y")}}',
-                 'subtitle': 'Prepared for {{client}}',
+                 'subtitle': 'Prepared for {% if longclient %}{{longclient}}{% else %}{{client}}{% endif %}',
                  'template': '',
                  'lang': 'en',
                  'twoside': False,
                  'numbersections': False,
                  'titlepage': True,
                  'titlepage-text-color': '000000',
                  'titlepage-rule-height': 0,
@@ -82,48 +85,49 @@
     if text[-4:] == ' \\\\ ':
         return text[:-4]
     else:
         return text
 
 
 class LatexFormatter(OutputFormatter):
-    def __init__(self, format="latex", templatedir='', template=dict(), headers=dict()):
-        OutputFormatter.__init__(self, "latex", templatedir, template, headers)
+    def __init__(self, templateheaders=dict(), timer=None, watcher=None):
+        OutputFormatter.__init__(self, templateheaders, timer, watcher=watcher)
+        self.templatefile = self.templateheaders['latex_template']
         self.figformat = "pdf"
 
         # Set up latex file headers
         latexheaders = dict()
 
         # Put in the defaults for the latex template
         latexheaders.update(default_latex)
 
         # Update latex headers with what's in the template
-        if "latex" in self.template:
+        if "latex" in templateheaders:
             for header in header_aliases.keys():
-                if header in self.template['latex']:
-                    self.template['latex'][header_aliases[header]
-                                           ] = self.template['latex'][header]
-                    del self.template['latex'][header]
+                if header in templateheaders['latex']:
+                    templateheaders['latex'][header_aliases[header]
+                                           ] = templateheaders['latex'][header]
+                    del templateheaders['latex'][header]
 
-            latexheaders.update(self.template['latex'])
+            latexheaders.update(templateheaders['latex'])
 
         if ('header-left' in latexheaders and latexheaders['header-left'] != '') or ('header-center' in latexheaders and latexheaders['header-center'] != '') or ('header-right' in latexheaders and latexheaders['header-right'] != ''):
             latexheaders['has-header'] = 'true'
 
         # Add the toc-section if there's a section
         if latexheaders['toc-section']:
             latexheaders['toc-section'] = self.newsection()
         else:
             latexheaders['toc-section'] = False
 
         # Add over the headers that refer to local files
         for header in ['titlepage-background', 'page-background']:
             if header in latexheaders:
                 latexheaders[header] = os.path.join(
-                    self.templatedir, latexheaders[header])
+                    self.templateheaders['templatedir'], latexheaders[header])
 
         # Set the default table options
         self.default_table_options = latex_default_table_options
 
         colors = ''
         colorlist = self.colors.getcolors()
         for name, color in colorlist.items():
@@ -150,15 +154,14 @@
                         style['bgcolor'])
                 bold = ''
                 if style['bold'] == True:
                     bold = '\\bfseries '
 
                 if style['size']:
                     s = style['size']
-                    log.warn("setting size {}".format(s))
                     sizes = {
                         'tiny': '\\tiny',
                         'small': '\\small',
                         'normal': '',
                         'large': '\\large',
                         'Large': '\\Large',
                         'LARGE': '\\LARGE',
@@ -236,18 +239,25 @@
         opts = self.default_table_options.copy()
         opts.update(options)
 
         t = Table(table, env=self.env, **tableargs)
 
         toptions = []
         if opts['vlines']:
-            toptions.append("vlines")
+            if 'vlines-options' in opts:
+                toptions.append(f"vlines = {opts['vlines-options']}")
+            else:
+                toptions.append("vlines")
+                
         if opts['hlines']:
-            toptions.append("hlines")
-        if opts['rowhead'] > 0:
+            if 'hlines-options' in opts:
+                toptions.append(f"hlines = {opts['hlines-options']}")
+            else:
+                toptions.append("hlines")
+        if opts['rowhead'] > 0 and len(t.table) > 1:
             toptions.append("rowhead = {}".format(opts['rowhead']))
 
         # If there's no actual table, warn and exit
         if t.width == 0:
             log.warn("Table is now empty. Printing an empty string.")
             return ""
 
@@ -257,19 +267,25 @@
             toptions.append("row{{odd}} = {{bg={}}}".format(opts['color-1']))
             toptions.append("row{{even}} = {{bg={}}}".format(opts['color-2']))
 
         colspec = []
         for c in range(len(t.table[0])):
             col = ''
             if opts['fullwidth']:
-                col += 'X'
+
                 copts = []
 
                 if tableargs.get('colwidths'):
-                    copts.append(str(t.colwidths[int(c)]))
+                    if t.colwidths[int(c)] == 0:
+                        col += 'Q'
+                    else:
+                        col += 'X'
+                        copts.append(str(t.colwidths[int(c)]))
+                else:
+                    col += 'X'
                 if t.colalign[c] != "":
                     copts.append(t.colalign[c])
 
                 if len(copts) > 0:
                     col += "[{}]".format(",".join(copts))
             else:
                 if t.colalign[c] != "":
@@ -278,15 +294,17 @@
                     col = 'l'
 
             colspec.append(col)
 
         toptions.append("colspec={{{}}}".format("".join(colspec)))
         if opts['longtable']:
             # Hack to remove header caption
-            markdown += "\\vspace{{-1.5\\baselineskip}}\\SetTblrTemplate{{head}}{{empty}}".format()
+            if 'headerhack' in opts and opts['headerhack']:
+                markdown += "\\vspace{{-1.5\\baselineskip}}"
+            markdown += "\\SetTblrTemplate{{head}}{{empty}}".format()
             markdown += "\\begin{{longtblr}}{{ {} }} \n".format(
                 ",".join(toptions))
         else:
             markdown += "\\begin{{tblr}}{{ {} }} \n".format(",".join(toptions))
 
         for i in range(len(t.table)):
             for j in range(len(t.table[i])):
@@ -371,64 +389,106 @@
         if opts['longtable']:
             markdown += "\\end{longtblr}\n"
         else:
             markdown += "\\end{tblr}\n"
         return markdown
 
     def newsection(self):
+        if "newsection-content" in self.templateheaders['latex']:
+            output = process_template(
+                [], self.templateheaders['latex']['newsection-content'], env=self.env, name="section", filename="")
+            return output
         markdown = '\\newpage\n'
-        if "section-background" in self.template['latex']:
+        if "section-background" in self.templateheaders['latex']:
             markdown += '\\begin{tikzpicture}[remember picture,overlay]\n'
             markdown += '\\node[inner sep=0] at (current page.center)\n'
             markdown += '{\\includegraphics[width=\\paperwidth,height=\\paperheight]{' + os.path.join(
-                self.templatedir, self.template['latex']["section-background"]) + '}};\n'
+                self.templateheaders['templatedir'], self.templateheaders['latex']["section-background"]) + '}};\n'
             markdown += '\\end{tikzpicture}\n'
-            if "section-skip" in self.template['latex']:
+            if "section-skip" in self.templateheaders['latex']:
                 markdown += '\\vskip {}\n'.format(
-                    self.template['latex']['section-skip'])
+                    self.templateheaders['latex']['section-skip'])
             else:
                 markdown += '\\vskip 14em\n'
         return markdown
 
     def newpage(self):
         return "\\pagebreak"
+    
+    def _process_template_headers(self, header, headername, env):
+        if type(header) == str:
+            # Run a jinja template if it's a string
+            try:
+                j2template = jinja2.Template(header)
+                return j2template.render(env)
+            except jinja2.exceptions.TemplateSyntaxError as error:
+                log.error(f"Error in processing template header {headername}: {error.message}")
+                log.error(f"Header contents: {header}")
+                log.error(f"Returning unprocessed header")
+                return header
+            except jinja2.exceptions.TemplateError as error:
+                log.error(f"Error in processing template header {headername}: {error.message}")
+                log.error(f"Returning unprocessed header")
+                return header
+        if type(header) == list:
+            # If it's a list, rerun on each element of the list
+            return [self._process_template_headers(headervalue, headername, env) for headername, headervalue in enumerate(header)]
+        if type(header) == dict:
+            # If it's a dict, rerun on each element of the dict
+            return {headername: self._process_template_headers(headervalue, headername, env) for headername, headervalue in header.items()}
+        # If it's anything else (number, date, etc), just return it blank.
+        return header
+                
+
+
 
     def headers(self):
-        markdown = yaml.dump(self.latexheaders)
+        
+        env = self.env.get_env()
+
+        markdown = yaml.dump(self._process_template_headers(self.latexheaders, "headers", env))
         return markdown
 
     def end(self):
-        """ To be called at the end of the output - puts in the ending page/graphics """
-        markdown = ''
-        markdown += '\\pagebreak\n'
-        markdown += '\\thispagestyle{empty}\n'
-        markdown += '\\NoBgThispage\n'
-        markdown += '\\begin{tikzpicture}[remember picture,overlay]\n'
-        markdown += '\\node[inner sep=0] at (current page.center)\n'
-        markdown += '{\\includegraphics[width=\\paperwidth,height=\\paperheight]{' + os.path.join(
-            self.templatedir, self.template['latex']['titlepage-background']) + '}};\n'
-        markdown += '\\end{tikzpicture}\n'
-        markdown += '\\vskip 14em\n'
-        return markdown
+        if "endpage-content" in self.templateheaders['latex']:
+            output = process_template(
+                [], self.templateheaders['latex']['endpage-content'], env=self.env, name="endpage", filename="")
+            return output
+        else:
+            markdown = '\\newpage\n'
+            """ To be called at the end of the output - puts in the ending page/graphics """
+            markdown = ''
+            markdown += '\\pagebreak\n'
+            markdown += '\\thispagestyle{empty}\n'
+            markdown += '\\NoBgThispage\n'
+            markdown += '\\begin{tikzpicture}[remember picture,overlay]\n'
+            markdown += '\\node[inner sep=0] at (current page.center)\n'
+            markdown += '{\\includegraphics[width=\\paperwidth,height=\\paperheight]{' + os.path.join(
+                self.templateheaders['templatedir'], self.templateheaders['latex']['titlepage-background']) + '}};\n'
+            markdown += '\\end{tikzpicture}\n'
+            markdown += '\\vskip 14em\n'
+            return markdown
 
-    def output(self, templatemarkdown, templatefile='', docformat='pdf', outputfile='', options={}):
-        output = self._build_markdown(templatemarkdown)
+    def output(self, markdown, outputfile=''):
+        output = self._build_markdown(markdown)
 
-        if(docformat != 'pdf'):
+        if self.docformat and self.docformat != 'pdf':
             log.info("Writing Markdown")
             with open(outputfile, 'w') as fh:
                 fh.write(output)
             log.info("Finished writing")
 
             return output
 
         log.info("Writing PDF")
+        log.info(f"Latex template file: {self.templatefile}")
+        log.info(f"Output file: {outputfile}")
         # Use Pandoc to print to PDF
         pandoc_arguments = ['pandoc', '--from', 'markdown', '--to', 'latex',
-                            '--template', templatefile, '--listings', '-o', outputfile]
-        if 'latex_numbered-headers' in options and options['latex_numbered-headers']:
+                            '--template', self.templatefile, '--listings', '-o', outputfile]
+        if self.options and 'latex_numbered-headers' in self.options and self.options['latex_numbered-headers']:
             pandoc_arguments.append('--number-sections')
         process = subprocess.run(pandoc_arguments,
                                  input=output,
                                  universal_newlines=True)
 
         return output
```

### Comparing `Report-Ranger-1.0/report_ranger/latexrenderer.py` & `Report-Ranger-2.0/report_ranger/markdown_renderer/latexrenderer.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,214 +1,142 @@
-import mistune
-import re
-import logging
-
-log = logging.getLogger(__name__)
-
-
-class LatexTableRenderer(mistune.HTMLRenderer):
-    NAME = 'latex'
-    IS_TREE = False
-
-    def _escape_latex(self, text):
-        ''' Escape the given text based on the format we're working with
-
-        :param text: a plain text message
-        :return: the message escaped to appear correctly in LaTeX
-        '''
-        conv = {
-            '&': r'\&',
-            '%': r'\%',
-            '$': r'\$',
-            '#': r'\#',
-            '_': r'\_',
-            '{': r'\{',
-            '}': r'\}',
-            '~': r'\textasciitilde{}',
-            '^': r'\^{}',
-            '\\': r'\textbackslash{}',
-            '<': r'\textless{}',
-            '>': r'\textgreater{}',
-        }
-        regex = re.compile('|'.join(re.escape(str(key)) for key in sorted(
-            conv.keys(), key=lambda item: - len(item))))
-        return regex.sub(lambda match: conv[match.group()], text)
-
-    def __init__(self, escape=True):
-        super(LatexTableRenderer, self).__init__()
-        self._escape = escape
-
-    def text(self, text):
-        return self._escape_latex(text)
-
-    def link(self, link, text=None, title=None):
-        if text is None or text == '':
-            return '\\url{{{}}}'.format(self._escape_latex(link))
-
-        s = '\\href{' + \
-            self._escape_latex(link) + '}{' + self._escape_latex(text) + '}'
-        return s
-
-    def image(self, src, alt="", title=None):
-        s = '\\begin{{figure}}'
-        s += '\\centering'
-        s += '\\includegraphics{{{}}}}'.format(self._escape_latex(src))
-        s += '\\caption{{{}}}'.format(self._escape_latex(alt))
-        s += '\\end{{figure}}'
-        return s
-
-    def emphasis(self, text):
-        return '\\emph{' + text + '}'
-
-    def strong(self, text):
-        return '\\textbf{' + text + '}'
-
-    def codespan(self, text):
-        return '\\passthrough{\\lstinline$' + self._escape_latex(text) + '$}'
-
-    def linebreak(self):
-        return ' \\\\ '
-
-    def inline_html(self, html):
-        return self._escape_latex(html)
-
-    def paragraph(self, text):
-        return text + ' \\\\ '
-
-    def heading(self, text, level):
-        # TODO DOES NOT PROPERLY DO HEADINGS
-        return text
-
-    def newline(self):
-        return ''
-
-    def thematic_break(self):
-        # TODO NO THEMATIC BREAK
-        return ''
-
-    def block_text(self, text):
-        return text
-
-    def block_code(self, code, info=None):
-        return code
-
-    def block_quote(self, text):
-        return text
-
-    def block_html(self, html):
-        return html
-
-    def block_error(self, html):
-        return html
-
-    def list(self, text, ordered, level, start=None):
-        if ordered:
-            return "\n\\begin{{enumerate}}\n{}\\end{{enumerate}}".format(text)
-        else:
-            return "\n\\begin{{varwidth}}[t]{{\\linewidth}}\n\\begin{{itemize}}[topsep = 0pt, parsep = 0pt]\n{}\\strut\\end{{itemize}}\end{{varwidth}}\n".format(text)
-
-    def list_item(self, text, level):
-        return " \item {}\n".format("text")
-
-
-class LatexRenderer(mistune.HTMLRenderer):
-    NAME = 'latex'
-    IS_TREE = False
-
-    def _escape_latex(self, text):
-        ''' Escape the given text based on the format we're working with
-
-        :param text: a plain text message
-        :return: the message escaped to appear correctly in LaTeX
-        '''
-        conv = {
-            '&': r'\&',
-            '%': r'\%',
-            '$': r'\$',
-            '#': r'\#',
-            '_': r'\_',
-            '{': r'\{',
-            '}': r'\}',
-            '~': r'\textasciitilde{}',
-            '^': r'\^{}',
-            '\\': r'\textbackslash{}',
-            '<': r'\textless{}',
-            '>': r'\textgreater{}',
-        }
-        regex = re.compile('|'.join(re.escape(str(key)) for key in sorted(
-            conv.keys(), key=lambda item: - len(item))))
-        return regex.sub(lambda match: conv[match.group()], text)
-
-    def __init__(self, escape=True):
-        super(LatexRenderer, self).__init__()
-        self._escape = escape
-
-    def text(self, text):
-        return self._escape_latex(text)
-
-    def link(self, link, text=None, title=None):
-        if text is None:
-            return '\\url{{{}}}'.format(self._escape_latex(link))
-
-        s = '\\href{' + \
-            self._escape_latex(link) + '}{' + self._escape_latex(text) + '}'
-        return s
-
-    def image(self, src, alt="", title=None):
-        s = '\\begin{{figure}}'
-        s += '\\centering'
-        s += '\\includegraphics{{{}}}}'.format(self._escape_latex(src))
-        s += '\\caption{{{}}}'.format(self._escape_latex(alt))
-        s += '\\end{{figure}}'
-        return s
-
-    def emphasis(self, text):
-        return '\\emph{' + self._escape_latex(text) + '}'
-
-    def strong(self, text):
-        return '\\textbf{' + self._escape_latex(text) + '}'
-
-    def codespan(self, text):
-        return '\\passthrough{\\lstinline$' + self._escape_latex(text) + '$}'
-
-    def linebreak(self):
-        return '\\\\\n'
-
-    def inline_html(self, html):
-        return self._escape_latex(html)
-
-    def paragraph(self, text):
-        return text + '\n\n'
-
-    def heading(self, text, level):
-        # TODO DOES NOT PROPERLY DO HEADINGS
-        return text
-
-    def newline(self):
-        return ' \\\n'
-
-    def thematic_break(self):
-        # TODO NO THEMATIC BREAK
-        return '\n'
-
-    def block_text(self, text):
-        return text
-
-    def block_code(self, code, info=None):
-        return code
-
-    def block_quote(self, text):
-        return text
-
-    def block_html(self, html):
-        return html
-
-    def block_error(self, html):
-        return html
-
-    def list(self, text, ordered, level, start=None):
-        # TODO LIST
-        return text
-
-    def list_item(self, text, level):
-        # TODO LIST_ITEM
-        return text
+import mistune
+import re
+import logging
+
+log = logging.getLogger(__name__)
+
+
+class LatexTableRenderer(mistune.HTMLRenderer):
+    NAME = 'latex'
+    IS_TREE = False
+
+    def _escape_latex(self, text):
+        ''' Escape the given text for display in Latex output
+
+        :param text: a plain text message
+        :return: the message escaped to appear correctly in LaTeX
+        '''
+        conv = {
+            '&': r'\&',
+            '%': r'\%',
+            '$': r'\$',
+            '#': r'\#',
+            '_': r'\_',
+            '{': r'\{',
+            '}': r'\}',
+            '~': r'{\textasciitilde}',
+            '^': r'\^',
+            '\\': r'{\textbackslash}',
+            '<': r'{\textless}',
+            '>': r'{\textgreater}',
+        }
+        regex = re.compile('|'.join(re.escape(str(key)) for key in sorted(
+            conv.keys(), key=lambda item: - len(item))))
+        return regex.sub(lambda match: conv[match.group()], text)
+
+    def _escape_latex_codespan(self, text):
+        ''' Escape the given text for codespans in latex. This has different rules to elsewhere.
+        '''
+        sepchar = None
+        for char in "!\"'()*,-./:;_":
+            if char not in text:
+                sepchar = char
+                break
+        if not sepchar:
+            return None
+        conv = {
+            '&': r'\&',
+            '%': r'\%',
+            '#': r'\#',
+            '_': r'\_',
+            '{': r'\{',
+            '}': r'\}',
+            '~': r'\~',
+            '\\': r'\\\\'
+        }
+        regex = re.compile('|'.join(re.escape(str(key)) for key in sorted(
+            conv.keys(), key=lambda item: - len(item))))
+        return sepchar + regex.sub(lambda match: conv[match.group()], text) + sepchar
+
+    def __init__(self, escape=True):
+        super(LatexTableRenderer, self).__init__()
+        self._escape = escape
+
+    def text(self, text):
+        return self._escape_latex(text)
+
+    def link(self, link, text=None, title=None):
+        if text is None or text == '':
+            return '\\url{{{}}}'.format(self._escape_latex(link))
+
+        s = '\\href{' + \
+            self._escape_latex(link) + '}{' + self._escape_latex(text) + '}'
+        return s
+
+    def image(self, src, alt="", title=None):
+        s = '\\begin{{figure}}'
+        s += '\\centering'
+        s += '\\includegraphics{{{}}}}'.format(self._escape_latex(src))
+        s += '\\caption{{{}}}'.format(self._escape_latex(alt))
+        s += '\\end{{figure}}'
+        return s
+
+    def emphasis(self, text):
+        return '\\emph{' + text + '}'
+
+    def strong(self, text):
+        return '\\textbf{' + text + '}'
+
+    def codespan(self, text):
+        code = '\\passthrough{\\lstinline' + \
+            self._escape_latex_codespan(text) + '}'
+        if code != None:
+            return code
+        return self.block_code(text)
+
+    def linebreak(self):
+        return ' \\\\ '
+
+    def inline_html(self, html):
+        return self._escape_latex(html)
+
+    def paragraph(self, text):
+        return text + ' \\\\ '
+
+    def heading(self, text, level):
+        # TODO DOES NOT PROPERLY DO HEADINGS
+        return text
+
+    def newline(self):
+        return ''
+
+    def thematic_break(self):
+        # TODO NO THEMATIC BREAK
+        return ''
+
+    def block_text(self, text):
+        return text
+
+    def block_code(self, code, info=None):
+        code = code.replace('\n', '^^J\n')
+        code = code.replace('{', '\{')
+        code = code.replace('}', '\}')
+        return f"""\\begin{{lstlisting}}^^J
+{code}^^J\\end{{lstlisting}}"""
+
+    def block_quote(self, text):
+        return text
+
+    def block_html(self, html):
+        return html
+
+    def block_error(self, html):
+        return html
+
+    def list(self, text, ordered, level, start=None):
+        if ordered:
+            return "\n\\begin{{enumerate}}\n{}\\end{{enumerate}}".format(text)
+        else:
+            return "\n\\begin{{varwidth}}[t]{{\\linewidth}}\n\\begin{{itemize}}[topsep = 0pt, parsep = 0pt]\n{}\\strut\\end{{itemize}}\end{{varwidth}}\n".format(text)
+
+    def list_item(self, text, level):
+        return " \item {}\n".format(text)
```

### Comparing `Report-Ranger-1.0/report_ranger/outputformatter.py` & `Report-Ranger-2.0/report_ranger/output_formatter/outputformatter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import os
 import jinja2
-from .mdread import markdown_from_file, process_template
-from .table import Table
-from .contentassistant import ContentAssistant
+from report_ranger.utils.jinja_helpers import log_jinja2_error
+from report_ranger.utils.mdread import markdown_from_file, process_template
+from report_ranger.table import Table
+from report_ranger.contentassistant import ContentAssistant
 from num2words import num2words
 import pandas as pd
 import plotly.express as px
 from pathlib import Path
-from .environment import Environment
+from report_ranger.environment import Environment
 from tabulate import tabulate
-from .imports import import_csv, import_xlsx
+from report_ranger.imports.imports import import_csv, import_xlsx
 import traceback
 import logging
-from .styles import TableStyles, ColorList, test_color
-from .section import Section
+from report_ranger.styles import TableStyles, ColorList, test_color
+from report_ranger.imports.section import Section
 import plotly.io as pio
 import plotly.graph_objects as go
-from .helpers import table_aggregate, table_aggregate_value, filter_rows, table_to_dict, tables_outer_join, table_separate_column, table_add_row, table_separate_column_groups
+from report_ranger.helpers import table_aggregate, table_aggregate_value, filter_rows, table_to_dict, tables_outer_join, table_separate_column, table_add_row, table_separate_column_groups, sort_table, separate_sequences
 
 # Mathjax fix for plotly
 pio.kaleido.scope.mathjax = None
 
 log = logging.getLogger(__name__)
 
 headeralias = {
@@ -35,46 +36,47 @@
     'c': 'tclosed',
     'cb': 'tclosedbold',
     'O': 'topenbold',
     'ob': 'topenbold',
     'b': 'bold'
 }
 
-# For sorting IP addresses
-
 
+# For sorting IP addresses
 def split_ip(ip):
     """Split a IP address given as string into a 4-tuple of integers."""
     return tuple(int(part) for part in ip.split('.'))
 
-
 def sort_ips(item):
     ''' Helper function for sorting IPs, used as key in sorted function. '''
     return split_ip(item)
 
-
 def oxfordcomma(listed):
     if len(listed) == 0:
         return ''
     if len(listed) == 1:
         return listed[0]
     if len(listed) == 2:
         return listed[0] + ' and ' + listed[1]
     return ', '.join(listed[:-1]) + ', and ' + listed[-1]
 
 
 class OutputFormatter:
-    def __init__(self, format="latex", templatedir='', template=dict(), headers=dict()):
-        self.format = format
-        self.templatedir = templatedir
-        self.template = template
+    def __init__(self, templateheaders=dict(), timer=None, watcher=None):
+        self.templateheaders = templateheaders
         self.figformat = "png"
+        self.watcher=watcher
+        log.info(f"watcher is {watcher}")
+
+        self.timer = timer
+
+        self.timer = timer
 
         # Initial filling in the environment
-        log.debug("Initialising new environment for output formatter")
+        log.info(f"{self.time()}: Initialising new environment for output formatter")
         env = Environment()
         env.set_static('file_exists', self.file_exists)
         env.set_static('include_file', self.include_file)
         env.set_static('escape', self.escape)
         env.set_static('stringescape', self.escape)
         env.set_static('pathjoin', os.path.join)
         env.set_static('range', range)
@@ -89,25 +91,30 @@
         env.set_static('nfig', 0)
         ca = ContentAssistant()
         env.set_static('ca', ca)
         env.set_static('ft', ca.format_table)
         env.set_static('format_table', ca.format_table)
         env.set_static('counter', ca.counter)
         env.set_static('get_counter', ca.get_counter)
+        env.set_static('reset_counter', ca.reset_counter)
+        env.set_static('icounter', ca.icounter)
+        env.set_static('get_icounter', ca.get_icounter)
+        env.set_static('reset_icounter', ca.reset_icounter)
         env.set_static('table_row', ca.table_row)
         env.set_static('table_rows', ca.table_rows)
         env.set_static('display_table', ca.display_table)
 
         env.set_static('newpage', self.newpage)
         env.set_static('new_page', self.newpage)
         env.set_static('import_csv', import_csv)
         env.set_static('csv', import_csv)
         env.set_static('import_xlsx', import_xlsx)
         env.set_static('xlsx', import_xlsx)
         env.set_static('import_section', self.import_section)
+        env.set_static('process_tags', self.process_tags)
         env.set_static('build_from_data', self.build_from_data)
         env.set_static('new_section', self.newsection)
         env.set_static('end_report', self.end)
         env.set_static('iplist', self.iplist)
         env.set_static('table', self.table)
         env.set_static('figure', self.fig)
         env.set_static('fig', self.fig)
@@ -115,20 +122,23 @@
         env.set_static('polar_bar_chart', self.polar_bar_chart)
         env.set_static('funnel_chart', self.funnel_chart)
         env.set_static('chart', self.chart)
         env.set_static('include', self.include_file)
         env.set_static('table_aggregate', table_aggregate)
         env.set_static('table_aggregate_value', table_aggregate_value)
         env.set_static('filter_rows', filter_rows)
+        env.set_static('sort_table', sort_table)
         env.set_static('table_to_dict', table_to_dict)
         env.set_static('tables_outer_join', tables_outer_join)
         env.set_static('table_separate_column', table_separate_column)
         env.set_static('table_add_row', table_add_row)
         env.set_static('table_separate_column_groups',
                        table_separate_column_groups)
+        env.set_static('separate_sequences',
+                       separate_sequences)
 
         # Legacy variables - these function names have changed, but can be referred to with the old function name
         env.set_static('include_file', self.include_file)  # Legacy
 
         # For legacy reasons, let's set a new "of" variable which contains pointers to functions in the output formatter
         of = type('of', (object,), {})()
         of.newpage = self.newpage
@@ -136,38 +146,41 @@
         of.end = self.end
         of.table = self.table
         of.iplist = self.iplist
         of.fig = self.fig
         of.include_file = self.include_file
         of.escape = self.escape
         env.set_static('of', of)
+        
+        log.info(f"{self.time()}: Finished basic setting up env")
 
         # Start with the defaults
-        if 'defaults' in template:
-            env.set_variables(template['defaults'])
-
-        env.set_variables(headers)
+        if 'defaults' in templateheaders:
+            env.set_variables(templateheaders['defaults'])
 
         # Get color list
         self.colors = ColorList()
-        if 'colors' in self.template:
-            self.colors.addcolors(self.template['colors'])
-        if 'colors' in self.template['riskassessment']:
-            self.colors.addcolors(self.template['riskassessment']['colors'])
+        if 'colors' in self.templateheaders:
+            self.colors.addcolors(self.templateheaders['colors'])
+        if 'colors' in self.templateheaders['riskassessment']:
+            self.colors.addcolors(self.templateheaders['riskassessment']['colors'])
+
+
+        log.info(f"{self.time()}: Setting up table styles")
 
         # Get table styles
         self.tablestyles = TableStyles()
 
         temp_ts = dict()
 
-        if 'table_styles' in self.template:
-            temp_ts = self.template['table_styles']
+        if 'table_styles' in self.templateheaders:
+            temp_ts = self.templateheaders['table_styles']
 
-        if 'table_styles' in self.template['riskassessment']:
-            temp_ts.update(self.template['riskassessment']['table_styles'])
+        if 'table_styles' in self.templateheaders['riskassessment']:
+            temp_ts.update(self.templateheaders['riskassessment']['table_styles'])
 
         for name, style in temp_ts.items():
             # We need to make sure the colors are in the colorlist otherwise
             # latex won't be able to refer to the color
             if 'color' in style and not self.colors.getcolor(style['color']):
                 style['color'] = self.colors.addcolor(None, style['color'])
                 log.info("added new color {}".format(style['color']))
@@ -175,26 +188,35 @@
                 style['bgcolor'] = self.colors.addcolor(
                     None, style['bgcolor'])
                 log.info("added new color {}".format(style['bgcolor']))
 
             self.tablestyles.addstyle(name, style)
 
         self.env = env
+        
+        log.info(f"{self.time()}: Setting up plotly template")
 
-        self.setup_plotly_template(self.template, self.colors)
+        self.setup_plotly_template(self.templateheaders, self.colors)
+
+        log.info(f"{self.time()}: Finished output formatter initialisation")
+
+    def time(self):
+        if self.timer:
+            return self.timer.time()
+        return ""
 
     def stringescape(self, text):
         return text.replace("\\", "\\\\")
 
     def escape(self, text):
         return text
 
     def import_section(self, directory, ordinal='1'):
-        newsection = Section(directory, ordinal)
-        return newsection.get_chapters(self)
+        newsection = Section(directory, ordinal, watcher=self.watcher)
+        return newsection.get_chapters(self.env)
 
     def iplist(self, listofips, heading="IP list", columns=4):
         '''Build a table from a list of IPs. Automatically format based on number of columns and sort IPs into order.'''
 
         log.debug("iplist(): Building IP list")
 
         try:
@@ -257,14 +279,24 @@
 
     def file_exists(self, file_loc):
         fn, ext = os.path.splitext(file_loc)
         if ext != ".md" and ext != ".rr":
             return False
         return os.path.isfile(file_loc)
 
+    def process_tags(self, text, add_to_env={}):
+        if type(text) is not str:
+            log.warn("Text passed to process_tags is not a string")
+            return ""
+        if text == "":
+            log.warn("Empty string passed to process_tags")
+            return ""
+        return process_template(
+            add_to_env, text, env=self.env, name="Call to process")
+
     def build_from_data(self, data, headings={}, heading_text={}, text={}, pre_text={}):
         """
         Build a hierarchy of report headings and text based on the entries in data.
 
         This function is commonly used to "reportise" a spreadsheet and so the expected data structures match
         the csv and xslx functions. Data should be in the format of dicts/lists of dicts/lists, like what the
         csv and xslx functions return.
@@ -432,15 +464,15 @@
             return ''
 
     def include_file(self, file_loc, include_headers=True, custom_headers=None):
         """ Process the file, template it, and return just the markdown """
         fn, ext = os.path.splitext(file_loc)
         if ext != ".md" and ext != ".rr":
             return ""
-        headers, markdown = markdown_from_file(file_loc)
+        headers, markdown = markdown_from_file(file_loc, env=self.env, watcher=self.watcher)
         headers['cwd'] = os.path.dirname(
             os.path.join(os.path.curdir, file_loc))
 
         if not include_headers:
             headers = {}
 
         if custom_headers != None:
@@ -450,42 +482,47 @@
             output = process_template(
                 headers, markdown, env=self.env, name="included file", filename=file_loc)
             return output
         except jinja2.exceptions.TemplateSyntaxError as error:
             log.error("Jinja2 error processing included file {}: {} at lineno {} for file {}".format(
                 file_loc, error.message, error.lineno, filename=error.filename))
             log.error("Removing markdown for included file {}".format(file_loc))
+            log_jinja2_error(markdown, error)
+            log.error(traceback.format_exc())
             return ""
         except Exception as e:
             log.error(
                 "Received exception when processing markdown for included file {}: {}".format(file_loc, e.args))
             log.error(
                 "Removing markdown for included file {}".format(file_loc))
+            log.error(traceback.format_exc())
             return ""
 
     def setup_plotly_template(self, template, colors):
         """ Setup the plotly template based on the table_styles template header
         """
         if 'charts' in template:
-            log.info("Customising chart template")
+            log.info(f"{self.time()}: Customising chart template")
             charts = template['charts']
             # Translate colours for the template
             for l in ['colorway']:
                 if l in charts:
                     for i in range(len(charts[l])):
                         if colors.getcolor(charts[l][i]):
                             charts[l][i] = '#' + colors.getcolor(charts[l][i])
                         elif test_color(charts[l][i]):
                             charts[l][i] = '#' + charts[l][i]
 
+
             plotly_template = dict(
                 layout=go.Layout(template['charts'])
             )
             pio.templates["reportranger"] = plotly_template
 
+            log.info(f"{self.time()}: Before set static plotly template")
             pio.templates.default = 'plotly_white+reportranger'
         else:
             plotly_template = 'plotly_white'
             pio.templates.default = 'plotly_white'
 
         self.env.set_static("plotly_template", plotly_template)
 
@@ -501,15 +538,15 @@
             )
             df[labels[2]] = i
             frames.append(df)
 
         dataframe = pd.concat(frames, axis=0)
         return dataframe
 
-    def bar_chart(self, description, data, *args, **kwargs):
+    def bar_chart(self, description, data, update_layout=None, update_traces=None, *args, **kwargs):
         """ Simple vertical bar chart that is {column: value}
         """
         multi = False
         # See if we have multiple categories
         for i in data:
             if type(data[i]) is dict:
                 multi = True
@@ -521,15 +558,15 @@
             figure = px.bar(dataframe, x="index", y="value",
                             color="category", *args, **kwargs)
         else:
             dataframe = pd.Series(data=data)
 
             figure = px.bar(dataframe, *args, **kwargs)
             figure.update_layout(showlegend=False)
-        return self.fig(description, figure)
+        return self.fig(description, figure, update_layout, update_traces)
 
     def funnel_chart(self, description, data, *args, **kwargs):
 
         multi = False
         # See if we have multiple categories
         for i in data:
             if type(data[i]) is dict:
@@ -592,15 +629,17 @@
             kwargs['color_discrete_map'] = colors
             kwargs['color'] = 'maturity'
 
         figure = px.bar_polar(dataframe, r='value',
                               theta='direction', *args, **kwargs)
 
         update_layout = {'showlegend': False, 'polar_radialaxis_dtick': 1,
-                         'polar_radialaxis_showticklabels': True}
+                         'polar_radialaxis_showticklabels': False,
+                         'polar_radialaxis_showline': False
+                         }
 
         if range:
             update_layout['polar_radialaxis_range'] = range
 
         figure.update_layout(**update_layout)
 
         return self.fig(description, figure)
@@ -646,96 +685,93 @@
             figure.update_layout(**update_layout)
         if update_traces:
             figure.update_traces(**update_traces)
 
         figure.write_image(filename)
         return '![{}]({})'.format(description, filename)
 
-    def _build_markdown(self, templatemarkdown):
-        # A giant string to put all the output markdown into
-        markdown = ""
+    def _build_markdown_headers(self, headers):
+        # Headers. This is a separate function because it might be modified or taken away by specific formatters.
+        markdown = '''---\n'''
+        markdown += headers
+        markdown += "\n...\n\n"
+        return markdown
 
-        log.info("Outputting markdown")
-        # Headers
-        markdown += '''---\n'''
+    def _warn_in_text(self, templateheaders, env, text):
+        ''' Throw a log warning if the warn list in templateheaders or env is in the text
+        '''
+        warn = []
+
+        # Generate the warning list. This combines the lists in the template as well as the report (if it's there)
+
+        # Get the list from the template
+        if 'warn' in templateheaders:
+            log.info("Warning on {}".format(templateheaders['warn']))
 
-        markdown += self.headers()
+            if isinstance(templateheaders['warn'], list):
+                warn = templateheaders['warn']
+            else:
+                log.warn(
+                    "Warn header in the template front matter is not a list. Warning function won't work.")
 
-        markdown += "\n...\n\n"  # End the headers
+        # Get the list from the report headers
+        if 'warn' in env:
+            if isinstance(env['warn'], list):
+                warn = [*warn, *env['warn']]
+            else:
+                log.warn(
+                    "Warn header in the report front matter is not a list. Warning function won't work.")
 
-        env = self.env.get_env()
+        # Go through the final output and warn on the line if the warning text is found
+        for warntext in warn:
+            if text.find(warntext):
+                matched_lines = [line for line in text.split(
+                    '\n') if warntext.lower() in line.lower()]
+                for line in matched_lines:
+                    log.warn(
+                        "Found '{}' in the following line: {}".format(warntext, line))
 
-        markdown += templatemarkdown
 
-        try:
-            j2template = jinja2.Template(markdown)
-            output = j2template.render(env)
+    def _build_markdown(self, templatemarkdown):
+        # A giant string to put all the output markdown into
+        markdown = ""
 
-            # Content assistant parsing
-            output = self.env.get('ca').parse_register(self, output)
+        log.info(f"{self.time()}: Outputting markdown")
+        markdown += self._build_markdown_headers(self.headers())
 
-            warn = []
+        env = self.env.get_env()
 
-            # Generate the warning list. This combines the lists in the template as well as the report (if it's there)
 
-            # Get the list from the template
-            if 'warn' in self.template:
-                log.info("Warning on {}".format(self.template['warn']))
+        try:
+            j2template = jinja2.Template(templatemarkdown)
+            processedtemplate = j2template.render(env)
+            markdown += processedtemplate
 
-                if isinstance(self.template['warn'], list):
-                    warn = self.template['warn']
-                else:
-                    log.warn(
-                        "Warn header in the template front matter is not a list. Warning function won't work.")
+            # Content assistant parsing
+            output = self.env.get('ca').parse_register(self, markdown)
 
-            # Get the list from the report headers
-            if 'warn' in env:
-                if isinstance(env['warn'], list):
-                    warn = [*warn, *env['warn']]
-                else:
-                    log.warn(
-                        "Warn header in the report front matter is not a list. Warning function won't work.")
+            self._warn_in_text(self.templateheaders, env, output)
 
-            # Go through the final output and warn on the line if the warning text is found
-            for warntext in warn:
-                if output.find(warntext):
-                    matched_lines = [line for line in output.split(
-                        '\n') if warntext.lower() in line.lower()]
-                    for line in matched_lines:
-                        log.warn(
-                            "Found '{}' in the following line: {}".format(warntext, line))
 
         except jinja2.exceptions.TemplateSyntaxError as error:
             log.error(
                 "Error in processing the final template: {}".format(error.message))
-            log.error("Affected lines:")
-            mdlines = markdown.splitlines()
-            for i in range(5):
-                el = error.lineno - 5 + i
-                if el < 0:
-                    continue
-                log.error("{}: {}".format(el, mdlines[el]))
-            log.error("+ {}: {}".format(error.lineno, mdlines[error.lineno]))
-            for i in range(5):
-                el = error.lineno + 1 + i
-                if el >= len(mdlines):
-                    continue
-                log.error("{}: {}".format(el, mdlines[el]))
+            log_jinja2_error(markdown, error)
             raise Exception("Error reading the final template: {} at lineno {} for file {}".format(
                 error.message, error.lineno, error.filename))
         except jinja2.exceptions.TemplateError as error:
             log.error(
                 "Error in processing the final template: {}".format(error.message))
             raise Exception("Error reading the final template: {}".format(
                 error.message))
 
         return output
 
-    def output(self, templatemarkdown, templatefile='', docformat='md', outputfile='', options={}):
-        output = self._build_markdown(templatemarkdown)
+    def output(self, markdown, outputfile=''):
+        output = self._build_markdown(markdown)
 
         log.info("Writing Markdown")
 
         with open(outputfile, 'w') as fh:
             fh.write(output)
         log.info("Finished writing")
```

### Comparing `Report-Ranger-1.0/report_ranger/report_ranger.py` & `Report-Ranger-2.0/report_ranger/report_ranger.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,21 @@
-from . import vulnerability
-from . import config  # Configuration settings within report ranger
-from .errors import InputError
-from .template import Template
+import time
+from report_ranger.imports import vulnerability
+from report_ranger import config  # Configuration settings within report ranger
+from report_ranger.errors import InputError
+from report_ranger.report import Report
+from report_ranger.template import Template
+from report_ranger.templatemapper import process_templatemapper
 import os
 import jinja2
 import logging
+from watchdog.observers import Observer
+from report_ranger.watcher import Watcher
+
+from report_ranger.utils.jinja_helpers import log_jinja2_error
 
 log = logging.getLogger(__name__)
 
 
 def main(args):
     # Turn on verbose mode
     if args.verbose:
@@ -20,42 +27,57 @@
 
     parentdir = os.path.dirname(os.path.join(os.path.curdir, args.input))
 
     # We need to change the current working directory to the directory of the template otherwise relative
     # paths inside the template won't work. For instance you won't be able to include executivesummary.md
     rr_parent_folder = os.path.abspath(os.path.curdir)
 
-    # Get the absolute location of the template so it survives the change of directory
+    ctm = config.config['templatemapper'] if 'templatemapper' in config.config else {}        
+    ctms = config.config['templatemappers'] if 'templatemappers' in config.config else []
+
+    templatemapper = process_templatemapper(args.templatemapper, ctm, ctms)
 
     if args.template:
-        if args.template in config.config['templatemapper']:
-            templatefile = config.config['templatemapper'][args.template]
+        if args.template in templatemapper:
+            templatefile = templatemapper[args.template]
         else:
             templatefile = os.path.abspath(args.template)
     else:
         templatefile = ''
 
     os.chdir(parentdir)
     parentdir = '.'
     mdfile = os.path.basename(args.input)
 
     # Get the template
-    template = Template(
-        templatefile, config.config['templatemapper'], config.config['defaulttemplate'])
+    report = Report(
+        mdfile,
+        templatefile=templatefile,
+        templatemapper=templatemapper,
+        default_template=config.config['defaulttemplate'])
 
     # Get the extension of the output file
-    fn, ext = os.path.splitext(args.output)
+    if args.output:
+        fn, ext = os.path.splitext(args.output)
+    else:
+        ext = 'md'
 
     # Figure out what target we have
     if args.format == "pdf":
         target = "latex"
         docformat = "pdf"
-    elif args.format == "latex":
+    if args.format == "pdf-latex":
+        target = "latex"
+        docformat = "pdf"
+    elif args.format == "markdown-latex":
         target = "latex"
         docformat = "markdown"
+    elif args.format == "typst":
+        target = "typst"
+        docformat = "typst"
     elif args.format == "markdown":
         target = "markdown"
         docformat = "markdown"
     elif args.format == "docx":
         target = "docx"
         docformat = "docx"
     elif args.format == "html":
@@ -69,14 +91,18 @@
             target = "docx"
             docformat = "docx"
             log.info("Setting target and format to docx")
         elif ext == ".md" or ext == ".rr":
             target = "markdown"
             docformat = "md"
             log.info("Setting target to markdown and format to md")
+        elif ext == ".typ":
+            target = "typst"
+            docformat = "typst"
+            log.info("Setting target to markdown and format to md")
         elif ext == ".html":
             target = "html"
             docformat = "html"
             log.info("Setting target and format to html")
         elif ext == ".csv":
             target = "csv"
             docformat = "csv"
@@ -91,23 +117,66 @@
     stdout_link = None
     if docformat.lower() == 'pdf' and args.output == '-':
         stdout_link = '/tmp/stdout.pdf'
         os.symlink('/dev/stdout', stdout_link)
         args.output = stdout_link
 
     # Convert output file path into full path if relative path is given
-    if args.output[0] != '/':
+    if args.output and args.output[0] != '/':
         args.output = os.path.join(rr_parent_folder, args.output)
 
-    try:
-        output = template.process_file(mdfile, target, docformat, args.output)
-    except InputError as ie:
-        log.error("Input Error: {}".format(ie.message))
-        exit()
-    except jinja2.exceptions.TemplateSyntaxError as error:
-        log.error("Jinja2 error: {} at lineno {} for file {}".format(
-            error.message, error.lineno, error.filename))
-        exit()
-
-    # If we're outputting to stdout, remove the link
-    if stdout_link and os.path.exists(stdout_link):
-        os.remove(stdout_link)
+
+    if args.watch:
+        log.info("Starting watch")
+        try:
+            watcher = Watcher(log.info, "Callback")
+            watcher.set_callback(report.process_file, mdfile, target, docformat, args.output, default_output_file=config.config.get('default_output_file'), watcher=watcher)
+            watcher.set_watch_mode(args.watch_mode)
+            output = report.process_file(mdfile, target, docformat, args.output, default_output_file=config.config.get('default_output_file'), watcher=watcher)
+            if args.watch_mode != "modified":
+                log.info("Setting watch mode to os")
+                observer = Observer()
+                observer.schedule(watcher, parentdir, recursive=True)
+                observer.start()
+                try:
+                    while True:
+                        time.sleep(5)
+                        watcher.run()
+                finally:
+                    observer.stop()
+                    observer.join()
+            else:
+                log.info("Setting watch mode to modification time")
+                while True:
+                    try:
+                        time.sleep(5)
+                        watcher.run()
+                    except InputError as ie:
+                        log.error("Input Error: {}".format(ie.message))
+                        exit()
+                    except jinja2.exceptions.TemplateSyntaxError as error:
+                        log.error("Final report processing Jinja2 error: {} at lineno {} for file {}".format(
+                            error.message, error.lineno, error.filename))
+                        log_jinja2_error(mdfile, error)
+                        exit()
+
+        except InputError as ie:
+            log.error("Input Error: {}".format(ie.message))
+        except jinja2.exceptions.TemplateSyntaxError as error:
+            log.error("Final report processing Jinja2 error: {} at lineno {} for file {}".format(
+                error.message, error.lineno, error.filename))
+            log_jinja2_error(mdfile, error)
+    else:
+        try:
+            output = report.process_file(mdfile, target, docformat, args.output, default_output_file=config.config.get('default_output_file'))
+        except InputError as ie:
+            log.error("Input Error: {}".format(ie.message))
+            exit()
+        except jinja2.exceptions.TemplateSyntaxError as error:
+            log.error("Final report processing Jinja2 error: {} at lineno {} for file {}".format(
+                error.message, error.lineno, error.filename))
+            log_jinja2_error(mdfile, error)
+            exit()
+
+        # If we're outputting to stdout, remove the link
+        if stdout_link and os.path.exists(stdout_link):
+            os.remove(stdout_link)
```

### Comparing `Report-Ranger-1.0/report_ranger/riskassessment.py` & `Report-Ranger-2.0/report_ranger/riskassessment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .errors import InputError
+from report_ranger.errors import InputError
 import logging
 
 log = logging.getLogger(__name__)
 
 
 def combine_matrix(matrix, next_matrix):
     """ Combine two risk matrices where the final risk in one is fed into the next. It is called recursively """
```

### Comparing `Report-Ranger-1.0/report_ranger/section.py` & `Report-Ranger-2.0/report_ranger/imports/section.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,115 +1,126 @@
-# from .mdread import markdown_from_directory, process_template
-from . import mdread
-import logging
-import traceback
-import jinja2
-
-log = logging.getLogger(__name__)
-
-
-def int_to_rn(num, uppercase=True):
-    val = [1000, 900, 500, 400, 100, 90, 50, 40, 10, 9, 5, 4, 1]
-    uppercase = ["M", "CM", "D", "CD", "C", "XC",
-                 "L", "XL", "X", "IX", "V", "IV", "I"]
-    lowercase = ["m", "cm", "d", "cd", "c", "xc",
-                 "l", "xl", "x", "ix", "v", "iv", "i"]
-    numeral = ''
-    i = 0
-    while num > 0:
-        for _ in range(num // val[i]):
-            if uppercase:
-                numeral += uppercase[i]
-            else:
-                numeral += lowercase[i]
-            num -= val[i]
-        i += 1
-    return numeral
-
-
-class Section:
-    def __init__(self, directory, ordinal='1'):
-        try:
-            chaptersmd = mdread.markdown_from_directory(directory)
-        except Exception as e:
-            log.error(
-                "Received exception when processing directory {}: {}".format(directory, e.args))
-            # log.error(traceback.format_exc()) Not displaying traceback because it's usually just a missing directory
-            self.chapters = []
-            return
-
-        # Sort the chapters by weight
-        for i in chaptersmd:
-            if 'weight' not in i[0]:
-                i[0]['weight'] = 1
-        chaptersmd = sorted(
-            chaptersmd, key=lambda x: float(x[0]['weight']) * -1)
-
-        nchapter = 0
-        chapters = []
-
-        for i in range(len(chaptersmd)):
-            if ordinal == 'a':
-                ref = chr(ord('a') + nchapter)
-            elif ordinal == 'A':
-                ref = chr(ord('A') + nchapter)
-            elif ordinal == 'I':
-                ref = int_to_rn(nchapter + 1)
-            elif ordinal == 'i':
-                ref = int_to_rn(nchapter + 1, False)
-            else:
-                ref = nchapter + 1
-
-            chapters.append(
-                Chapter(ref, chaptersmd[i]))
-            nchapter += 1
-
-        self.chapters = chapters
-
-    def get_chapters(self, of):
-        chapters = []
-        for chapter in self.chapters:
-            chapters.append(chapter.get_chapter(of))
-        return chapters
-
-
-class Chapter:
-    def __init__(self, ref, chaptermd):
-        self.headers = chaptermd[0]
-        self.headers['ref'] = ref
-        self.chapter_markdown = chaptermd[1]
-        self.ref = ref
-
-        if 'name' not in self.headers:
-            if 'Name' in self.headers:
-                self.headers['name'] = self.headers['Name']
-            else:
-                log.warn("Chapter does not have a name. Setting it to 'Chapter''")
-                self.headers['name'] = 'Chapter'
-
-        self.name = self.headers['name']
-
-    def markdown(self, of):
-        try:
-            output = mdread.process_template(
-                self.headers, self.chapter_markdown, of.env)
-            return output
-        except jinja2.exceptions.TemplateSyntaxError as error:
-            log.error("Jinja2 error processing chapter {}: {} at lineno {} for file {}".format(
-                self.name, error.message, error.lineno, filename=error.filename))
-            log.error("Removing markdown for chapter {}".format(self.name))
-            return ""
-        except Exception as e:
-            log.error(
-                "Received exception when processing markdown for section {}: {}".format(self.name, e.args))
-            log.error(traceback.format_exc())
-            log.error(
-                "Removing markdown for chapter {}".format(self.name))
-            return ""
-
-    def get_chapter(self, of):
-        chapter = {}
-        chapter['name'] = self.name
-        chapter['headers'] = self.headers
-        chapter['ref'] = self.ref
-        chapter['markdown'] = self.markdown(of)
-        return chapter
+# from .mdread import markdown_from_directory, process_template
+from report_ranger.utils import mdread
+import logging
+import traceback
+import jinja2
+
+from report_ranger.utils.jinja_helpers import log_jinja2_error
+
+log = logging.getLogger(__name__)
+
+
+def int_to_rn(num, uppercase=True):
+    val = [1000, 900, 500, 400, 100, 90, 50, 40, 10, 9, 5, 4, 1]
+    uppercase = ["M", "CM", "D", "CD", "C", "XC",
+                 "L", "XL", "X", "IX", "V", "IV", "I"]
+    lowercase = ["m", "cm", "d", "cd", "c", "xc",
+                 "l", "xl", "x", "ix", "v", "iv", "i"]
+    numeral = ''
+    i = 0
+    while num > 0:
+        for _ in range(num // val[i]):
+            if uppercase:
+                numeral += uppercase[i]
+            else:
+                numeral += lowercase[i]
+            num -= val[i]
+        i += 1
+    return numeral
+
+
+class Section:
+    def __init__(self, directory, ordinal='1', watcher=None):
+        try:
+            chaptersmd = mdread.markdown_from_directory(directory, watcher=watcher)
+            if watcher:
+                watcher.add_path(directory)
+        except FileNotFoundError as e:
+            log.warn(e.args[0])
+            self.chapters = []
+            return
+        except Exception as e:
+            log.error(
+                "Received exception when processing directory {}: {}".format(directory, e.args))
+            # log.error(traceback.format_exc()) Not displaying traceback because it's usually just a missing directory
+            self.chapters = []
+            return
+
+        # Sort the chapters by weight
+        for i in chaptersmd:
+            if 'weight' not in i[0]:
+                i[0]['weight'] = 1
+        chaptersmd = sorted(
+            chaptersmd, key=lambda x: float(x[0]['weight']) * -1)
+
+        nchapter = 0
+        chapters = []
+
+        for i in range(len(chaptersmd)):
+            if ordinal == 'a':
+                ref = chr(ord('a') + nchapter)
+            elif ordinal == 'A':
+                ref = chr(ord('A') + nchapter)
+            elif ordinal == 'I':
+                ref = int_to_rn(nchapter + 1)
+            elif ordinal == 'i':
+                ref = int_to_rn(nchapter + 1, False)
+            else:
+                ref = nchapter + 1
+
+            chapters.append(
+                Chapter(ref, chaptersmd[i]))
+            nchapter += 1
+
+        self.chapters = chapters
+
+    def get_chapters(self, env):
+        chapters = []
+        for chapter in self.chapters:
+            chapters.append(chapter.get_chapter(env))
+        return chapters
+
+
+class Chapter:
+    def __init__(self, ref, chaptermd, filename="name"):
+        self.headers = chaptermd[0]
+        self.headers['ref'] = ref
+        self.chapter_markdown = chaptermd[1]
+        self.ref = ref
+        self.filename = self.headers['filename']
+        self.filename_noext = self.headers['filename_noext']
+
+        if 'name' not in self.headers:
+            if 'Name' in self.headers:
+                self.headers['name'] = self.headers['Name']
+            else:
+                log.warn(f"Chapter from file '{self.filename}' does not have a name. Setting it to '{self.filename_noext}''")
+                self.headers['name'] = 'Chapter'
+
+        self.name = self.headers['name']
+
+    def markdown(self, env):
+        try:
+            output = mdread.process_template(
+                self.headers, self.chapter_markdown, env)
+            return output
+        except jinja2.exceptions.TemplateSyntaxError as error:
+            log.error("Jinja2 error processing chapter {}: {} at lineno {} for file {}".format(
+                self.name, error.message, error.lineno, filename=error.filename))
+            log.error("Removing markdown for chapter {}".format(self.name))
+            log_jinja2_error(self.chapter_markdown, error)
+            return ""
+        except Exception as e:
+            log.error(
+                "Received exception when processing markdown for section {}: {}".format(self.name, e.args))
+            log.error(traceback.format_exc())
+            log.error(
+                "Removing markdown for chapter {}".format(self.name))
+            return ""
+
+    def get_chapter(self, env):
+        chapter = {}
+        chapter['name'] = self.name
+        chapter['headers'] = self.headers
+        chapter['ref'] = self.ref
+        chapter['markdown'] = self.markdown(env)
+        return chapter
```

### Comparing `Report-Ranger-1.0/report_ranger/table.py` & `Report-Ranger-2.0/report_ranger/table.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,420 +1,454 @@
-import re
-import logging
-from .mdread import process_template
-from .helpers import filter_rows
-
-
-log = logging.getLogger(__name__)
-
-
-def style_text_match(style_text, text, regexlist=None):
-    ''' See if the text is in the style_text dict and match it to stylelist '''
-    if type(text) is not str:
-        return None
-    if not regexlist:
-        regexlist = [(re.compile(ts), cf)
-                     for (ts, cf) in style_text.items()]
-
-    # We have to go through each regex to see if it matches
-    for ts in regexlist:
-        # Regexes are in a tuple (regex, cf)
-        if ts[0].match(text):
-            return ts[1]
-
-
-class Table:
-    """ This class holds a table to be used in output formatters. It will hold things like table contents, headings, alignment, widths
-
-    The table has the following state:
-    table: A list of lists containing the content of each cell, always guaranteed to be square. Table will pad if necessary.
-    cellstyles: A list of lists containing a string with the style of each square, always guaranteed be the same size of table.
-    colalign: A list of strings, either 'l', 'c', 'r', 'j' or an empty string. Guaranteed to be the width of the table.
-    cellalign: A list of lists of strings,  either 'l', 'c', 'r', 'j' or an empty string, always guaranteed be the same size of table.
-    colspan: A list of lists containing numbers where each number >= 1 or -1 if the cell is overwritten, always guaranteed be the same size of table. This is for when you would like a cell to overwrite the next column.
-    rowspan: A list of lists containing numbers where each number >= 1 or -1 if the cell is overwritten, always guaranteed be the same size of table. This is for when you would like a cell to overwrite the next row.
-    colwidths: A single list of numbers. Guaranteed to be the width of the table. This corresponds to the width of each cell.
-    """
-
-    def _pad_matrix(self, m, width=0, height=0, pad_value=''):
-        """ Pad the matrix m (a list of lists) to the set width and height with the pad_value.
-
-        If the width and height is not set, make sure that the matrix m is rectangular, with each row being the same length by padding them with pad_value.
-        """
-        if m == None:
-            m = []
-            for i in range(height):
-                m += [[pad_value]*width]
-            return m
-
-        if height == 0:
-            height = len(m)
-
-        if width == 0:
-            for i in m:
-                mw = len(i)
-                if mw > width:
-                    width = mw
-
-        for row in m:
-            if len(row) < width:
-                row += [pad_value]*(width-len(row))
-            if len(row) > width:
-                row = row[:width]
-
-        if len(m) < height:
-            for i in range(height-len(m)):
-                m += [[pad_value]*width]
-        elif len(m) > height:
-            m = m[:height]
-
-        return m
-
-    def _pad_list(self, l, width, pad_value=''):
-        """ Pad the list l to the required width with pad_value """
-        if l == None:
-            l = []
-
-        if len(l) < width:
-            l += [pad_value]*(width-len(l))
-
-        return l
-
-    def __init__(self, table, env=None, filter_rows=None, header=[], headings=None, cellstyles=None, colalign=None, cellalign=None, colspan=None, rowspan=None, colwidths=None, append_column=None, colpicker=None, rowpicker=None, style_text={}):
-        # Is it just a markdown table?
-        if isinstance(table, str):
-            re_tablecells = re.compile(r'(\||^)([^\|]*)(?=(\||$))')
-            re_isheaderline = re.compile(r'^\|?( *:?-+:? *\|?)*$')
-            re_hastablecells = re.compile(r'\|')
-            lines = table.splitlines()
-            matrixtable = []
-            newcolalign = []
-            for line in lines:
-                if not re_hastablecells.match(line):
-                    continue
-                cells = re_tablecells.findall(line)
-                # Is it the heading line?
-                if re_isheaderline.match(line):
-                    if headings == None:
-                        headings = 'top'
-                    newcolalign = []
-                    for cell in cells:
-                        ic = cell[1].strip()
-                        if len(ic) == 0:
-                            continue
-                        if ic[0] == ':':
-                            if ic[-1] == ':':
-                                newcolalign.append('c')
-                            else:
-                                newcolalign.append('l')
-                        elif ic[-1] == ':':
-                            newcolalign.append('r')
-                        else:
-                            newcolalign.append('l')
-                else:
-                    row = []
-                    # Check to see if the first line has a |, if so skip the last one
-                    if cells[0][0] == '|':
-                        endpipe = True
-                    for cell in cells:
-                        row.append(cell[1].strip())
-                    if endpipe:  # Kill last empty cell
-                        if row[-1] == '':
-                            row = row[:-1]
-                    matrixtable.append(row)
-
-            # Append colalign if it's not complete
-            if colalign == None:
-                colalign = []
-            colalign += newcolalign[len(colalign):]
-            table = matrixtable
-
-        if not isinstance(table, list):
-            log.warn(
-                "Table not a list. Trying to make a table out of {}.".format(table))
-            self.table = [[]]
-            self.width = 0
-            self.height = 0
-            self.cellstyles = []
-            self.colalign = []
-            self.cellalign = []
-            self.colspan = []
-            self.rowspan = []
-            self.colwidths = []
-            return
-
-        # We perform validation now, after converting a blank markdown table and before converting list of dicts to list of lists
-        if filter_rows:
-            table = filter_rows(filter_rows)
-
-        # We are representing the table in a dict form and we need to translate that into a table. For instance:
-        # affected_hosts:
-        # - hostname: host.com
-        #   port: 80
-        # - hostname: host2.com
-        #   port: 80
-        tableheadings = None
-        append_column_done = False
-        if isinstance(table[0], dict):
-
-            for r in range(len(table)):
-                if not isinstance(table[r], dict):
-                    log.warn(
-                        "Table defined as dicts has something which is not a dict, replacing with empty row: {}".format(table[r]))
-                    table[r] = dict()
-
-                # Process append row
-                if isinstance(append_column, dict):
-                    append_column_done = True
-                    newcols = {}
-                    for key in append_column:
-                        newcols[key] = process_template(
-                            table[r], append_column[key], env=env, name="append_column")
-                    table[r].update(newcols)
-
-            tableheadings = []
-            # Get the headings from the dicts
-            for row in table:
-                for h in row.keys():
-                    if h not in tableheadings:
-                        tableheadings.append(h)
-
-            newtable = []
-
-            # Headings will always be the first row of the new table
-            newtable.append(tableheadings)
-            for row in table:
-                newrow = []
-                for h in tableheadings:
-                    if h in row.keys():
-                        newrow.append(row[h])
-                    else:
-                        # This heading isn't in this row, add a blank
-                        newrow.append("")
-                newtable.append(newrow)
-            table = newtable
-
-        # We should now have a list of lists. Let's just make sure!
-        newtable = []
-        for row in table:
-            if not isinstance(row, list):
-                log.warn("Table row not a list: {}".format(row))
-            else:
-                newtable.append(row)
-        table = newtable
-
-        if append_column and not append_column_done:
-            if isinstance(append_column, list):
-                for row in range(len(table)):
-                    rowdict = {}
-                    # We need to index for each column
-                    for col in range(len(row)):
-                        rowdict['col' + str(col)] = table[row][col]
-                    for key in range(len(append_column)):
-                        table[row].append(process_template(
-                            rowdict, append_column[key], env=env, name="append_column"))
-            elif isinstance(append_column, dict):
-                log.warning(
-                    "append_column a dict for a table of lists: {}".format(append_column))
-            else:
-                log.warning(
-                    "append_column not a list: {}".format(append_column))
-
-        # Pad everything
-        self.table = self._pad_matrix(table, pad_value='')
-        width = len(table[0])
-        height = len(table)
-
-        self.height = height
-        self.width = width
-
-        # Handle rowpicker and colpicker
-        # Rowpicker first, since filtering rows is easier and quicker than filtering columns
-        if rowpicker != None and rowpicker != []:
-            if not isinstance(rowpicker, list):
-                log.warn("Rowpicker variable not a list, ignoring.")
-            else:
-                newtable = []
-                for row in rowpicker:
-                    if not isinstance(row, int):
-                        log.warn(
-                            "Entry in rowpicker was not int. Found: {}".format(row))
-                    elif row < 0 or row >= len(self.table):
-                        log.warn("Entry in rowpicker outside the range of the table length {}. Found: {}".format(
-                            len(self.table), row))
-                    else:
-                        newtable.append(self.table[row])
-                self.table = newtable
-                self.height = len(self.table)
-
-        if colpicker != None and colpicker != []:
-            if not isinstance(colpicker, list):
-                log.warn("Colpicker variable not a list, ignoring.")
-            else:
-                newtable = []
-                for i in range(len(self.table)):
-                    newtable.append([])
-                for col in colpicker:
-                    if isinstance(col, str):
-                        # Check to see if we're referring to a column heading
-                        if col in self.table[0]:
-                            col = self.table[0].index(col)
-                        else:
-                            log.warn(
-                                "Entry in colpicker is a string but not a column heading. Found: {}".format(col))
-                            continue
-                    elif not isinstance(col, int):
-                        log.warn(
-                            "Entry in colpicker was not int. Found: {}".format(col))
-                        continue
-
-                    if col < 0 or col >= len(self.table[0]):
-                        log.warn("Entry in colpicker outside the range of the table length {}. Found: {}".format(
-                            len(self.table[0]), col))
-                        continue
-
-                    for trow in range(len(self.table)):
-                        newtable[trow].append(self.table[trow][col])
-                self.table = newtable
-
-                if len(self.table) > 0:  # Do we actually still have a table?
-                    self.width = len(self.table[0])
-                else:
-                    self.width = 0
-
-        # If there's no table anymore due to rowpicker or colpicker then get rid of the rest, just cancel it out
-        if self.width == 0:
-            log.warn("rowpicker and colpicker resulted in an empty table.")
-            self.table = [[]]
-            self.width = 0
-            self.height = 0
-            self.cellstyles = []
-            self.colalign = []
-            self.cellalign = []
-            self.colspan = []
-            self.rowspan = []
-            self.colwidths = []
-            return
-
-        # Put in the header if it's been supplied
-        if header != []:
-            if isinstance(header, list):
-                # If there's tableheadings from a dict already, remove them
-                if tableheadings:
-                    self.table = [header] + self.table[1:]
-
-                else:
-                    self.table = [header] + self.table
-
-                # Do we need to repad?
-                if width != len(header):
-                    self.table = self._pad_matrix(self.table, pad_value='')
-                    self.width = len(self.table[0])
-
-                self.height = len(self.table)
-            else:
-                log.warn(
-                    "Header of the table is not a list. Trying to add {}.".format(header))
-
-        # colalign must be one of 'l' 'c' 'r' or 'j' or an empty string
-        colalign = self._pad_list(colalign, self.width, '')
-        for i in range(self.width):
-            if colalign[i] not in 'lcrj':
-                colalign[i] = ''
-
-        cellalign = self._pad_matrix(cellalign, self.width, self.height, '')
-        for i in range(self.height):
-            for j in range(self.width):
-                if cellalign[i][j] not in 'lcrj':
-                    cellalign[i][j] = ''
-        self.colalign = colalign
-        self.cellalign = cellalign
-
-        # Handle colspan and rowspan
-        colspan = self._pad_matrix(
-            colspan, self.width, self.height, 1)  # Pad to size of table
-        rowspan = self._pad_matrix(
-            rowspan, self.width, self.height, 1)  # Pad to size of table
-
-        # Handle colspan
-        for i in range(self.height):
-            for j in range(self.width):
-                if not int(colspan[i][j]):  # Validate it's an int
-                    colspan[i][j] = 1
-                if colspan[i][j] >= 1:  # We have a colspan!
-                    # Does it go over the side of the table?
-                    if j + colspan[i][j] > self.width:
-                        colspan[i][j] = self.width - j  # Snip it off
-                    # We blank out the rest of the span
-                    for span in range(1, colspan[i][j]):
-                        colspan[i][j+span] = -1
-
-        # Handle rowspan. This is equivalent of the above, just swapping row and column
-        for i in range(self.height):
-            for j in range(self.width):
-                if not int(rowspan[i][j]):
-                    rowspan[i][j] = 1
-                if rowspan[i][j] >= 1:
-                    if i + rowspan[i][j] > self.height:
-                        rowspan[i][j] = self.height - i
-                    for span in range(1, rowspan[i][j]):
-                        rowspan[i+span][j] = -1
-        self.colspan = colspan
-        self.rowspan = rowspan
-
-        self.colwidths = self._pad_list(colwidths, self.width, 0)
-
-        cellstyles = self._pad_matrix(cellstyles, self.width, self.height, '')
-
-        # Allow the 'left', 'top', and 'left-top' headings settings
-        if not isinstance(headings, list) and not headings == None:
-            headingslist = headings.split('-')
-            if 'left' in headingslist:
-                for row in cellstyles:
-                    if row[0] == '':
-                        row[0] = 'h'
-            if 'right' in headingslist:
-                for row in cellstyles:
-                    if row[-1] == '':
-                        row[-1] = 'h'
-            if 'top' in headingslist:
-                for i in range(len(cellstyles[0])):
-                    if cellstyles[0][i] == '':
-                        cellstyles[0][i] = 'h'
-            if 'bottom' in headingslist:
-                for i in range(len(cellstyles[-1])):
-                    if cellstyles[-1][i] == '':
-                        cellstyles[-1][i] = 'h'
-        else:
-            cellstyles = self._pad_matrix(
-                cellstyles, self.width, self.height, '')
-
-        # If there's headings text sync then add them
-        if style_text:
-            # Get all the regexes
-            stregexlist = [(re.compile(ts), cf)
-                           for (ts, cf) in style_text.items()]
-
-        for r in range(self.height):
-            for c in range(self.width):
-                # First check to see if there's a style in cellstyles
-                if type(cellstyles[r][c]) is dict:
-                    # If it's a dict, treat it as a style text dict
-                    st_return = style_text_match(
-                        cellstyles[r][c], self.table[r][c])
-                    if st_return:
-                        cellstyles[r][c] = st_return
-                    else:
-                        cellstyles[r][c] = ''
-                elif type(cellstyles[r][c]) is str and cellstyles[r][c] != '':
-                    # Leave it as is if there's something filled in
-                    continue
-                elif style_text:
-                    # Now check master style_text
-                    cellstyle = style_text_match(
-                        style_text, self.table[r][c], stregexlist)
-                    if cellstyle:
-                        cellstyles[r][c] = cellstyle
-                else:
-                    cellstyles[r][c] = ''
-
-        self.cellstyles = cellstyles
+import re
+import logging
+from report_ranger.utils.mdread import process_template
+from report_ranger.helpers import filter_rows as fr
+
+
+log = logging.getLogger(__name__)
+
+
+def style_text_match(style_text, text, regexlist=None):
+    ''' See if the text is in the style_text dict and match it to stylelist '''
+    if type(text) is not str:
+        return None
+    if not regexlist:
+        regexlist = [(re.compile(ts), cf)
+                     for (ts, cf) in style_text.items()]
+
+    # We have to go through each regex to see if it matches
+    for ts in regexlist:
+        # Regexes are in a tuple (regex, cf)
+        if ts[0].match(text):
+            return ts[1]
+
+
+class Table:
+    """ This class holds a table to be used in output formatters. It will hold things like table contents, headings, alignment, widths
+
+    The table has the following state:
+    table: A list of lists containing the content of each cell, always guaranteed to be square. Table will pad if necessary.
+    cellstyles: A list of lists containing a string with the style of each square, always guaranteed be the same size of table.
+    colalign: A list of strings, either 'l', 'c', 'r', 'j' or an empty string. Guaranteed to be the width of the table.
+    cellalign: A list of lists of strings,  either 'l', 'c', 'r', 'j' or an empty string, always guaranteed be the same size of table.
+    colspan: A list of lists containing numbers where each number >= 1 or -1 if the cell is overwritten, always guaranteed be the same size of table. This is for when you would like a cell to overwrite the next column.
+    rowspan: A list of lists containing numbers where each number >= 1 or -1 if the cell is overwritten, always guaranteed be the same size of table. This is for when you would like a cell to overwrite the next row.
+    colwidths: A single list of numbers. Guaranteed to be the width of the table. This corresponds to the width of each cell.
+    """
+
+    def _pad_matrix(self, m, width=0, height=0, pad_value=''):
+        """ Pad the matrix m (a list of lists) to the set width and height with the pad_value.
+
+        If the width and height is not set, make sure that the matrix m is rectangular, with each row being the same length by padding them with pad_value.
+        """
+        if m == None:
+            m = []
+            for i in range(height):
+                m += [[pad_value]*width]
+            return m
+
+        if height == 0:
+            height = len(m)
+
+        if width == 0:
+            for i in m:
+                mw = len(i)
+                if mw > width:
+                    width = mw
+
+        for row in m:
+            if len(row) < width:
+                row += [pad_value]*(width-len(row))
+            if len(row) > width:
+                row = row[:width]
+
+        if len(m) < height:
+            for i in range(height-len(m)):
+                m += [[pad_value]*width]
+        elif len(m) > height:
+            m = m[:height]
+
+        return m
+
+    def _pad_list(self, l, width, pad_value=''):
+        """ Pad the list l to the required width with pad_value """
+        if l == None:
+            l = []
+
+        if len(l) < width:
+            l += [pad_value]*(width-len(l))
+
+        return l
+    
+    def _clear_table(self):
+        self.table = [[]]
+        self.width = 0
+        self.height = 0
+        self.cellstyles = []
+        self.colalign = []
+        self.cellalign = []
+        self.colspan = []
+        self.rowspan = []
+        self.colwidths = []
+    
+    def _markdown_to_matrix(self, markdown):
+        """ Convert the markdown string into a table.
+        
+        Returns """
+        re_tablecells = re.compile(r'(\||^)([^\|]*)(?=(\||$))')
+        re_isheaderline = re.compile(r'^\|?(\s*:?-+:?\s*\|?)*\s*$')
+        re_hastablecells = re.compile(r'\|')
+        lines = markdown.splitlines()
+        matrixtable = []
+        colalign = []
+        has_heading = False
+        for line in lines:
+            if not re_hastablecells.match(line):
+                continue
+            cells = re_tablecells.findall(line)
+            # Is it the heading line?
+            if re_isheaderline.match(line):
+                has_heading = True
+                for cell in cells:
+                    ic = cell[1].strip()
+                    if len(ic) == 0:
+                        continue
+                    if ic[0] == ':':
+                        if ic[-1] == ':':
+                            colalign.append('c')
+                        else:
+                            colalign.append('l')
+                    elif ic[-1] == ':':
+                        colalign.append('r')
+                    else:
+                        colalign.append('l')
+            else:
+                row = []
+                # Check to see if the first line has a |, if so skip the last one
+                if cells[0][0] == '|':
+                    endpipe = True
+                for cell in cells:
+                    row.append(cell[1].strip())
+                if endpipe:  # Kill last empty cell
+                    if row[-1] == '':
+                        row = row[:-1]
+                matrixtable.append(row)
+
+        return matrixtable, colalign, has_heading
+
+    def _process_list_of_dicts(self, table, append_column, env):
+        """Convert a list of dicts to a matrix with a header line
+        
+        append_column will be appended to the end of each row.
+        """
+        
+        tableheadings = None
+
+        for r in range(len(table)):
+            if not isinstance(table[r], dict):
+                log.warn(
+                    f"Table defined as dicts has something which is not a dict, replacing with empty row: {table[r]}")
+                table[r] = dict()
+
+            # Process append_column
+            if isinstance(append_column, dict):
+                append_column_done = True
+                newcols = {}
+                for key in append_column:
+                    newcols[key] = process_template(
+                        table[r], append_column[key], env=env, name="append_column")
+                table[r].update(newcols)
+
+        tableheadings = []
+
+        # Get the headings from the dicts
+        for row in table:
+            for h in row.keys():
+                if h not in tableheadings:
+                    tableheadings.append(h)
+
+        newtable = []
+
+        # Headings will always be the first row of the new table
+        newtable.append(tableheadings)
+        for row in table:
+            newrow = []
+            for h in tableheadings:
+                if h in row.keys():
+                    newrow.append(row[h])
+                else:
+                    # This heading isn't in this row, add a blank
+                    newrow.append("")
+            newtable.append(newrow)
+        return newtable, tableheadings
+        
+
+    def __init__(self, table, env=None, filter_rows=None, header=[], headings=None, cellstyles=None, colstyles=None, colalign=None, cellalign=None, colspan=None, rowspan=None, colwidths=None, append_column=None, colpicker=None, rowpicker=None, style_text={}):
+        # Is it just a markdown table?
+        if isinstance(table, str):
+            table, newcolalign, has_heading = self._markdown_to_matrix(table)
+
+            # Append colalign if it's not complete
+            if colalign == None:
+                colalign = []
+            colalign += newcolalign[len(colalign):]
+            
+            # Set a heading row if it has one
+            if has_heading == True and headings == None:
+                headings = 'top'
+
+        # The table now has to be a list. If it is not a list, warn and skip
+        if not isinstance(table, list):
+            log.warn(f"Table not a list. Trying to make a table out of {table}.")
+            self._clear_table()
+            return
+        
+        # If there's no rows there's nothing to display
+        if len(table) == 0:
+            log.warn("Table has no rows, skipping table.")
+            self._clear_table()
+            return
+
+        # We perform validation now, after converting a blank markdown table and before converting list of dicts to list of lists
+        if filter_rows:
+            table = fr(table, filter_rows)
+            if len(table) == 0:
+                log.warning("Table has no rows after filtering")
+                self._clear_table()
+                return
+            
+        append_column_done = False
+
+        # We are representing the table in a dict form and we need to translate that into a table. For instance:
+        # affected_hosts:
+        # - hostname: host.com
+        #   port: 80
+        # - hostname: host2.com
+        #   port: 80
+        tableheadings = None
+        if isinstance(table[0], dict):
+            table, tableheadings = self._process_list_of_dicts(table, append_column, env)
+            append_column_done = True
+
+        # We should now have a list of lists. Let's just make sure!
+        newtable = []
+        for row in table:
+            if not isinstance(row, list):
+                log.warn(f"Table row not a list. Skipping table row: {row}")
+            else:
+                newtable.append(row)
+        table = newtable
+
+        # If we have a list of lists, then append_column won't be done yet. Let's do that.
+        if append_column and not append_column_done:
+            if isinstance(append_column, list):
+                for row in range(len(table)):
+                    rowdict = {}
+                    # We need to index for each column
+                    for col in range(len(row)):
+                        rowdict['col' + str(col)] = table[row][col]
+                    for key in range(len(append_column)):
+                        table[row].append(process_template(
+                            rowdict, append_column[key], env=env, name="append_column"))
+            elif isinstance(append_column, dict):
+                log.warning(f"append_column a dict for a table of lists, skipping: {append_column}")
+            else:
+                log.warning(f"append_column not a list, skipping: {append_column}")
+
+        # Pad everything
+        self.table = self._pad_matrix(table, pad_value='')
+        width, height = len(table[0]), len(table)
+        
+        self.width, self.height = width, height
+
+        # Handle rowpicker and colpicker
+        # Rowpicker first, since filtering rows is easier and quicker than filtering columns
+        if rowpicker != None and rowpicker != []:
+            if not isinstance(rowpicker, list):
+                log.warn("Rowpicker variable not a list, ignoring.")
+            else:
+                newtable = []
+                for row in rowpicker:
+                    if not isinstance(row, int):
+                        log.warn(
+                            "Entry in rowpicker was not int. Found: {}".format(row))
+                    elif row < 0 or row >= len(self.table):
+                        log.warn("Entry in rowpicker outside the range of the table length {}. Found: {}".format(
+                            len(self.table), row))
+                    else:
+                        newtable.append(self.table[row])
+                self.table = newtable
+                self.height = len(self.table)
+
+        if colpicker != None and colpicker != []:
+            if not isinstance(colpicker, list):
+                log.warn("Colpicker variable not a list, ignoring.")
+            else:
+                newtable = []
+                for i in range(len(self.table)):
+                    newtable.append([])
+                for col in colpicker:
+                    if isinstance(col, str):
+                        # Check to see if we're referring to a column heading
+                        if col in self.table[0]:
+                            col = self.table[0].index(col)
+                        else:
+                            log.warn(
+                                "Entry in colpicker is a string but not a column heading. Found: {}".format(col))
+                            continue
+                    elif not isinstance(col, int):
+                        log.warn(
+                            "Entry in colpicker was not int. Found: {}".format(col))
+                        continue
+
+                    if col < 0 or col >= len(self.table[0]):
+                        log.warn("Entry in colpicker outside the range of the table length {}. Found: {}".format(
+                            len(self.table[0]), col))
+                        continue
+
+                    for trow in range(len(self.table)):
+                        newtable[trow].append(self.table[trow][col])
+                self.table = newtable
+
+                if len(self.table) > 0:  # Do we actually still have a table?
+                    self.width = len(self.table[0])
+                else:
+                    self.width = 0
+
+        # If there's no table anymore due to rowpicker or colpicker then get rid of the rest, just cancel it out
+        if self.width == 0:
+            log.warn("rowpicker and colpicker resulted in an empty table.")
+            self._clear_table()
+            return
+
+        # Put in the header if it's been supplied
+        if header != []:
+            if isinstance(header, list):
+                # If there's tableheadings from a dict already, remove them
+                if tableheadings:
+                    self.table = [header] + self.table[1:]
+
+                else:
+                    self.table = [header] + self.table
+
+                # Do we need to repad?
+                if width != len(header):
+                    self.table = self._pad_matrix(self.table, pad_value='')
+                    self.width = len(self.table[0])
+
+                self.height = len(self.table)
+            else:
+                log.warn(
+                    "Header of the table is not a list. Trying to add {}.".format(header))
+
+        # colalign must be one of 'l' 'c' 'r' or 'j' or an empty string
+        colalign = self._pad_list(colalign, self.width, '')
+        for i in range(self.width):
+            if colalign[i] not in 'lcrj':
+                colalign[i] = ''
+
+        cellalign = self._pad_matrix(cellalign, self.width, self.height, '')
+        for i in range(self.height):
+            for j in range(self.width):
+                if cellalign[i][j] not in 'lcrj':
+                    cellalign[i][j] = ''
+        self.colalign = colalign
+        self.cellalign = cellalign
+
+        # Handle colspan and rowspan
+        colspan = self._pad_matrix(
+            colspan, self.width, self.height, 1)  # Pad to size of table
+        rowspan = self._pad_matrix(
+            rowspan, self.width, self.height, 1)  # Pad to size of table
+
+        # Handle colspan
+        for i in range(self.height):
+            for j in range(self.width):
+                if not int(colspan[i][j]):  # Validate it's an int
+                    colspan[i][j] = 1
+                if colspan[i][j] >= 1:  # We have a colspan!
+                    # Does it go over the side of the table?
+                    if j + colspan[i][j] > self.width:
+                        colspan[i][j] = self.width - j  # Snip it off
+                    # We blank out the rest of the span
+                    for span in range(1, colspan[i][j]):
+                        colspan[i][j+span] = -1
+
+        # Handle rowspan. This is equivalent of the above, just swapping row and column
+        for i in range(self.height):
+            for j in range(self.width):
+                if not int(rowspan[i][j]):
+                    rowspan[i][j] = 1
+                if rowspan[i][j] >= 1:
+                    if i + rowspan[i][j] > self.height:
+                        rowspan[i][j] = self.height - i
+                    for span in range(1, rowspan[i][j]):
+                        rowspan[i+span][j] = -1
+        self.colspan = colspan
+        self.rowspan = rowspan
+
+        self.colwidths = self._pad_list(colwidths, self.width, 0)
+
+        cellstyles = self._pad_matrix(cellstyles, self.width, self.height, '')
+
+        # Allow the 'left', 'top', and 'left-top' headings settings
+        if not isinstance(headings, list) and not headings == None:
+            headingslist = headings.split('-')
+            if 'left' in headingslist:
+                for row in cellstyles:
+                    if row[0] == '':
+                        row[0] = 'h'
+            if 'right' in headingslist:
+                for row in cellstyles:
+                    if row[-1] == '':
+                        row[-1] = 'h'
+            if 'top' in headingslist:
+                for i in range(len(cellstyles[0])):
+                    if cellstyles[0][i] == '':
+                        cellstyles[0][i] = 'h'
+            if 'bottom' in headingslist:
+                for i in range(len(cellstyles[-1])):
+                    if cellstyles[-1][i] == '':
+                        cellstyles[-1][i] = 'h'
+        else:
+            cellstyles = self._pad_matrix(
+                cellstyles, self.width, self.height, '')
+
+        # Do the col styles if set. Go through and set each entire column in cellstyles as per what is set by the user in colstyles.
+        # Note that this won't overwrite headers
+        if colstyles:
+            for row in range(len(cellstyles)):
+                for col in range(len(cellstyles[row])):
+                    # Don't overwrite existing cellstyles, only fill in if it's blank
+                    if (cellstyles[row][col] == '' or cellstyles[row][col] == None) and col < len(colstyles) and colstyles[col] and colstyles[col] != '':
+                        cellstyles[row][col] = colstyles[col]
+
+        # If there's headings text sync then add them
+        if style_text:
+            # Get all the regexes
+            stregexlist = [(re.compile(ts), cf)
+                           for (ts, cf) in style_text.items()]
+
+        for r in range(self.height):
+            for c in range(self.width):
+                # First check to see if there's a style in cellstyles
+                if type(cellstyles[r][c]) is dict:
+                    # If it's a dict, treat it as a style text dict
+                    st_return = style_text_match(
+                        cellstyles[r][c], self.table[r][c])
+                    if st_return:
+                        cellstyles[r][c] = st_return
+                    else:
+                        cellstyles[r][c] = ''
+                elif type(cellstyles[r][c]) is str and cellstyles[r][c] != '':
+                    # Leave it as is if there's something filled in
+                    continue
+                elif style_text:
+                    # Now check master style_text
+                    cellstyle = style_text_match(
+                        style_text, self.table[r][c], stregexlist)
+                    if cellstyle:
+                        cellstyles[r][c] = cellstyle
+                else:
+                    cellstyles[r][c] = ''
+
+        self.cellstyles = cellstyles
```

### Comparing `Report-Ranger-1.0/report_ranger/validation.py` & `Report-Ranger-2.0/report_ranger/validation.py`

 * *Files identical despite different names*

### Comparing `Report-Ranger-1.0/report_ranger/vulnerability.py` & `Report-Ranger-2.0/report_ranger/imports/vulnerability.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,447 +1,464 @@
-from . import validation
-from .mdread import markdown_from_file, process_template
-from .outputformatter import oxfordcomma
-import os
-import logging
-import copy
-import datetime
-from collections import Counter
-from num2words import num2words
-import jinja2
-import traceback
-import cerberus
-
-log = logging.getLogger(__name__)
-
-
-def vuln_from_file(file_loc, riskassessment, env=dict(), vulnerability_validation={}, scope=None):
-    ''' Get the vulnerability markdown from a file, process the headers and make sure they're there. Return a Vulnerability object.'''
-    log.debug("Loading vulnerability file {}".format(file_loc))
-
-    headers, vulnmarkdown = markdown_from_file(file_loc)
-
-    if 'name' in headers:
-        if not isinstance(headers['name'], str):
-            log.warn("Vulnerability name not a string for file {}".format(file_loc))
-            name = file_loc
-            headers['name'] = file_loc
-        else:
-            name = headers['name']
-    elif 'Name' in headers:  # This is for legacy reasons, it used to be case insensitive so we still accept "Name"
-        name = headers['Name']
-        headers['name'] = headers['Name']
-    else:
-        log.warn("Vulnerability name not in headers for file {}".format(file_loc))
-        name = file_loc
-        headers['name'] = file_loc
-
-    if scope != None:
-        headers['scope'] = scope
-
-    validation.validate_headers(
-        vulnerability_validation, headers, validation.default_vulnerability_validation, name=name)
-
-    # Generate the new env variables they can play with
-    headers['cwd'] = os.path.dirname(os.path.join(
-        os.path.curdir, file_loc))  # for including screenshots
-
-    return Vulnerability(name, headers=headers, markdown=vulnmarkdown, riskassessment=riskassessment, filename=file_loc)
-
-
-class VulnerabilityList:
-    """Reads a directory for vulnerability definition files, arranges them, and stores the vulnerabilities as objects.
-
-    The class is usually referenced inside the markdown file itself to display the vulnerability information. It keeps the following attributes:
-
-    - scopes : a List of Scope objects corresponding to the vulnerability scopes
-    """
-
-    def __init__(self):
-        self.scopes = []
-
-    def add_from_dir(self, vulndir, of, riskassessment, vulnerability_validation={}):
-        # Make sure it's a directory
-        if not os.path.isdir(vulndir):
-            raise Exception("Vulnerabilities directory:{0} is not a valid path".format(
-                vulndir))
-
-        log.info("Reading vulnerabilities")
-        vulnerabilities = []
-
-        scopeintroductions = {}
-
-        # Get the vulnerability writeups from the vulndir
-        for f in os.listdir(vulndir):
-            # Scopes can be split into directories within the vulndir
-            if os.path.isdir(os.path.join(vulndir, f)):
-                log.info(
-                    "* New vulnerability scope in directory '{}'".format((os.path.join(vulndir, f))))
-                vdir = os.path.join(vulndir, f)
-                for v in os.listdir(vdir):
-                    if v == "template.md" or v == "template.md.rr":
-                        continue
-                    if v == "introduction.md" or v == "introduction.md.rr":
-                        scopeintroductions[f] = markdown_from_file(
-                            os.path.join(vdir, v))
-                        continue
-                    fn, ext = os.path.splitext(v)
-                    if ext == ".md" or ext == ".rr":  # Only process markdown files
-                        filename = os.path.join(vdir, v)
-                        log.info(
-                            "  - Reading vulnerability file '{}'".format(filename))
-                        try:
-                            vuln = vuln_from_file(
-                                filename, riskassessment=riskassessment, env=of.env, vulnerability_validation=vulnerability_validation, scope=f)
-                            vulnerabilities += [vuln]
-                        except validation.ValidationError as e:
-                            pass  # ValidationError already raises logs
-                        except Exception as e:
-                            log.error(
-                                "Received exception when processing markdown for vulnerability {}: {}".format(filename, e.args))
-                            log.error(
-                                "Removing markdown for vulnerability {}".format(self.name))
-                            self.markdown = ""
-            else:  # It's a file
-                if f == "template.md" or f == "template.md.rr":
-                    continue
-                if f == "introduction.md" or f == "introduction.md.rr":
-                    scopeintroduction = markdown_from_file(
-                        os.path.join(vulndir, f))
-                    if "scope" in scopeintroduction[0]:
-                        # There's a scope defined in the headers of the introduction
-                        scopeintroductions[f] = scopeintroduction
-                    else:
-                        scopeintroductions[''] = scopeintroduction
-                    continue
-                log.info(
-                    "* Reading vulnerability file '{}'".format(os.path.join(vulndir, f)))
-                fn, ext = os.path.splitext(f)
-                if ext == ".md" or ext == ".rr":  # Only process markdown files
-                    try:
-                        vulnerabilities += [vuln_from_file(
-                            os.path.join(vulndir, f), riskassessment=riskassessment, env=of.env)]
-                    except validation.ValidationError as e:
-                        pass  # ValidationError already raises logs
-                    except Exception as e:
-                        log.error(
-                            "Received exception when processing markdown for vulnerability {}: {}".format(filename, e.args))
-                        log.error(
-                            "Removing markdown for vulnerability {}".format(self.name))
-                        self.markdown = ""
-
-        # Sort the vulnerabilities into scopes
-        scopes = {}
-
-        # This is a marker for the highest risk
-        highestrisk = riskassessment.risks[0]
-        nhighestrisk = 0
-
-        suggest_rc = set()
-        suggest_ar = set()
-
-        # Suggest high level findings
-        for vuln in vulnerabilities:
-            if 'suggest_rc' in vuln.headers:
-                suggest_rc.update(vuln.headers['suggest_rc'])
-            if 'suggest_ar' in vuln.headers:
-                suggest_ar.update(vuln.headers['suggest_ar'])
-
-        for rc in suggest_rc:
-            log.info("Suggested root cause: {}".format(rc))
-        for ar in suggest_ar:
-            log.info("Suggested additional recommendation: {}".format(ar))
-
-        for i in vulnerabilities:
-            if i.nrisk > nhighestrisk:  # We have a new highest risk!
-                nhighestrisk = i.nrisk
-                highestrisk = i.risk
-            if not i.scope in scopes:  # New scope
-                scopes[i.scope] = Scope(i.scope)
-            scopes[i.scope].add_vulnerability(i)
-
-        for scope, introduction in scopeintroductions.items():
-            if scope not in scopes:
-                scopes[scope] = Scope(scope)
-            scopes[scope].introduction_headers = introduction[0]
-            scopes[scope].introduction = introduction[1]
-
-        # Add the highest risk to the variables
-        self.highestrisk = highestrisk
-        of.env.set_variable('highestrisk', highestrisk)
-        log.info("Highest risk of any vuln is {}".format(highestrisk))
-
-        self.scopes = list(scopes.values())
-        self.scopes.sort()
-
-        # Assign references
-        ref = 1
-        for scope in self.scopes:
-            for vulnerability in scope.vulnerabilities:
-                vulnerability.ref = ref
-                ref += 1
-
-    def get_scope_list(self, validation=None, date=None):
-        scopelist = {}
-        if date:
-            updatedvlist = self.updated(date)
-            scopes = updatedvlist.scopes
-        else:
-            scopes = self.scopes
-        for scope in scopes:
-            scopelist[scope.name] = scope.get_list(validation)
-        return scopelist
-
-    def get_ref(self, vulnerability_name):
-        """ Get the reference of a vulnerability by name. Usually called from a markdown file. """
-        for scope in self.scopes:
-            ref = scope.get_ref(vulnerability_name)
-            if ref:
-                return ref
-        return ""
-
-    def updated(self, date=datetime.date.today()):
-        # Alias for string today
-        if date == "today" or date == "now":
-            date = datetime.date.today()
-
-        newlist = VulnerabilityList()
-        for scope in self.scopes:
-            newlist.scopes.append(scope.updated(date))
-        newlist.scopes.sort()
-        return newlist
-
-    def nvulns(self, riskrating=""):
-        """ Get the number of vulnerabilities with the given risk rating """
-        return sum(scope.nvulns(riskrating) for scope in self.scopes)
-
-    def nriskdict(self):
-        """ Get a dictionary with risk:nrisks for all vulnerabilities """
-        nvulnlist = {}
-        for scope in self.scopes:
-            nvulnlist.update(scope.nriskdict())
-        return nvulnlist
-
-    def nrisklist(self):
-        return oxfordcomma(["{} ({}) {} risk".format(num2words(nrisk), nrisk, risk)
-                            for risk, nrisk in self.nriskdict().items()])
-
-    def generate_markdown(self, env):
-        for scope in self.scopes:
-            scope.generate_markdown(env)
-
-
-class Scope:
-    """ Holds a vulnerability scope, a container for vulnerabilities.
-
-    Has the following attributes:
-
-    name : The name of the scope as a string
-    vulnerabilities : A List of Vulnerability objects, corresponding to the vulnerabilities in this scope.
-                      Should always be sorted by severity and weight.
-    highestrisk : The highest risk in this scope as a string
-    sectionweight : The weight as a number used for ordering the scopes in a VulnerabilityList (highest weight first).
-                    Called sectionweight to have consistency with sections.
-    introduction_headers : The environment headers of an introduction, used for Jinja templating the markdown
-    introduction : The introduction markdown
-    """
-
-    def __init__(self, name, sectionweight=0):
-        self.name = name
-        self.vulnerabilities = []
-        self.highestrisk = 0
-        self.sectionweight = sectionweight
-        self.introduction_headers = {}
-        self.introduction = ""
-
-    def __lt__(self, other):
-        if other.sectionweight == self.sectionweight:
-            return other.highestrisk < self.highestrisk
-        else:
-            return other.sectionweight < self.sectionweight
-
-    def add_vulnerability(self, vulnerability):
-        """ Add a vulnerability to the scope. Automatically sort the vulnerabilities after adding. """
-        self.vulnerabilities.append(vulnerability)
-        if vulnerability.nrisk > self.highestrisk:
-            self.highestrisk = vulnerability.nrisk
-        if vulnerability.sectionweight > self.sectionweight:
-            self.sectionweight = vulnerability.sectionweight
-
-        self.vulnerabilities.sort()
-
-    def get_list(self, validation=None):
-        vulnlist = []
-        for vuln in self.vulnerabilities:
-            if validation == None:
-                vulnlist.append(vuln.get_list())
-            else:
-                vl = vuln.get_list()
-                validator = cerberus.Validator()
-                validator.allow_unknown = True
-                if vuln.validate(vl):
-                    vulnlist.append(vuln.get_list())
-        return vulnlist
-
-    def get_introduction(self, of):
-        """ Get the vulnerability introduction (usually put in the introduction.md file). Usually called from a markdown file. """
-        return process_template(self.introduction_headers, self.introduction, of.env)
-
-    def get_ref(self, vulnerability_name):
-        """ Get the reference of a vulnerability by name. Usually called from a markdown file. """
-        for vulnerability in self.vulnerabilities:
-            if vulnerability_name.lower() in vulnerability.name.lower():
-                return vulnerability.ref
-
-        return None
-
-    def nvulns(self, riskrating=""):
-        """ Get the number of vulnerabilities with the given risk rating """
-        return sum(riskrating in vuln.risk for vuln in self.vulnerabilities)
-
-    def nriskdict(self):
-        """ Get a dictionary with risk:nrisks for all vulnerabilities """
-        return Counter(vulnerability.risk for vulnerability in self.vulnerabilities)
-
-    def updated(self, date=datetime.date.today()):
-        """ Process the 'updates' header """
-        newscope = copy.copy(self)
-
-        # Regenerate with the added vulnerabilities
-        newscope.vulnerabilities = []
-        for vuln in self.vulnerabilities:
-            newscope.add_vulnerability(vuln.updated(date))
-
-        return newscope
-
-    def generate_markdown(self, env):
-        for vuln in self.vulnerabilities:
-            vuln.generate_markdown(env)
-
-
-class Vulnerability:
-    """A class for vulnerability markdown.
-
-    Has the following attributes:
-
-     - name : The name of the vulnerability as a string
-     - vulnerability_markdown : The markdown of the vulnerability as a tuple (headers, markdown)
-     - scope : The name of the scope as a string. Used by VulnerabilityList for sorting a bucket of vulnerabilities into scopes,
-                 taken from the headers, but this may be overwritten if it's in a scope bucket already.
-     - weight : A number, used for sorting vulnerabilities. Taken from the headers.
-     - sectionweight : A number, used for increasing the weight of a scope for sorting them. Set for particularly bad vulns. Taken from the headers.
-     - risk : The risk of the vuln as a string.
-     - nrisk : The risk of the vuln as a number. Used for sorting vulnerabilities.
-     - headers : The headers of the markdown.
-    """
-
-    def __init__(self, name, riskassessment, headers=dict(), markdown='', scope='', weight=0, sectionweight=0, filename=''):
-
-        self.name = name
-        self.vulnerability_markdown = markdown
-        self.scope = scope
-        self.ref = 0  # ref will be set by VulnerabilityList
-        self.filename = filename
-        self.riskassessment = riskassessment
-
-        if "riskassessment" in headers:
-            if riskassessment.id not in headers['riskassessment']:
-                raise Exception("Risk assessment {} not in the risk assessment for vulnerability {}".format(
-                    riskassessment.name, name))
-            headers.update(headers['riskassessment'][riskassessment.id])
-
-        if "scope" in headers:
-            self.scope = headers["scope"]
-        else:
-            self.scope = ''
-
-        if "weight" in headers:
-            self.weight = float(headers["weight"])
-        else:
-            self.weight = 0
-
-        if "sectionweight" in headers:
-            self.sectionweight = float(headers["sectionweight"])
-        else:
-            self.sectionweight = 0
-
-        self.risk = riskassessment.get_risk(headers)
-        self.nrisk = next((i for i, x in enumerate(
-            riskassessment.risks) if x == self.risk), 0)
-        headers['risk'] = self.risk
-
-        if "status" not in headers:
-            headers['status'] = "Open"
-
-        self.status = headers['status']
-        self.originalstatus = self.status
-        self.originalrisk = self.risk
-
-        self.headers = headers
-
-    def __lt__(self, other):
-        if other.nrisk == self.nrisk:
-            return other.weight < self.weight
-        else:
-            return other.nrisk < self.nrisk
-
-    def get_list(self):
-        vulnlist = {
-            'name': self.name,
-            'ref': self.ref,
-            'status': self.status,
-            'risk': self.risk,
-            'nrisk': self.nrisk,
-            'originalstatus': self.originalstatus,
-            'originalrisk': self.originalrisk,
-            'filename': self.filename,
-            'headers': self.headers
-        }
-        for stage in self.riskassessment.stages:
-            if stage['name'] in self.headers:
-                vulnlist[stage['name']] = self.headers[stage['name']]
-        return vulnlist
-
-    def updated(self, date=datetime.date.today()):
-        # Get a new vulnerability
-        newvuln = copy.copy(self)
-
-        # Deep headers needs a deep copy otherwise the updates will change the original vuln
-        newvuln.headers = copy.deepcopy(self.headers)
-
-        if 'updates' in self.headers:
-            for update in self.headers['updates']:
-                if 'date' not in update or update['date'] <= date or date == "all":
-                    for newvar in update.keys():
-                        if newvar == 'date':
-                            continue
-                        newvuln.headers[newvar] = update[newvar]
-
-        # We need to re-evaluate the risk just in case the likelihood or consequence changed
-        newvuln.risk = newvuln.riskassessment.get_risk(newvuln.headers)
-        newvuln.headers['risk'] = newvuln.risk
-        newvuln.status = newvuln.headers['status']
-
-        return newvuln
-
-    def generate_markdown(self, env):
-        """ Get the markdown of the vulnerability, processing the template with the current of.env.
-
-        Usually called from a markdown file. """
-        # First update the ref
-        self.headers['ref'] = self.ref
-        self.headers['scope'] = self.scope
-
-        try:
-            self.markdown = process_template(self.headers, self.vulnerability_markdown,
-                                             env, name="vulnerability {}".format(self.name), filename=self.filename)
-        except jinja2.exceptions.TemplateSyntaxError as error:
-            log.error("Jinja2 error processing vulnerability {}: {} at lineno {} for file {}".format(
-                self.name, error.message, error.lineno, filename=self.filename))
-            log.error("Removing markdown for vulnerability {}".format(self.name))
-            self.markdown = ""
-        except Exception as e:
-            log.error(
-                "Received exception when processing markdown for vulnerability {}: {}".format(self.name, e.args))
-            log.error(traceback.format_exc())
-            log.error("Removing markdown for vulnerability {}".format(self.name))
-            self.markdown = ""
+from report_ranger import validation
+from report_ranger.utils.jinja_helpers import log_jinja2_error
+from report_ranger.utils.mdread import markdown_from_file, process_template
+from report_ranger.output_formatter.outputformatter import oxfordcomma
+import os
+import logging
+import copy
+import datetime
+from collections import Counter
+from num2words import num2words
+import jinja2
+import traceback
+import cerberus
+from report_ranger.helpers import make_list
+
+log = logging.getLogger(__name__)
+
+
+def vuln_from_file(file_loc, riskassessment, env=None, vulnerability_validation={}, scope=None, watcher=None):
+    ''' Get the vulnerability markdown from a file, process the headers and make sure they're there. Return a Vulnerability object.'''
+    log.debug("Loading vulnerability file {}".format(file_loc))
+
+    headers, vulnmarkdown = markdown_from_file(file_loc, env=env, watcher=watcher)
+
+    if 'name' in headers:
+        if not isinstance(headers['name'], str):
+            log.warn("Vulnerability name not a string for file {}".format(file_loc))
+            name = file_loc
+            headers['name'] = file_loc
+        else:
+            name = headers['name']
+    elif 'Name' in headers:  # This is for legacy reasons, it used to be case insensitive so we still accept "Name"
+        name = headers['Name']
+        headers['name'] = headers['Name']
+    else:
+        log.warn("Vulnerability name not in headers for file {}".format(file_loc))
+        name = file_loc
+        headers['name'] = file_loc
+
+    if scope != None:
+        headers['scope'] = scope
+
+    validation.validate_headers(
+        vulnerability_validation, headers, validation.default_vulnerability_validation, name=name)
+
+    # Generate the new env variables they can play with
+    headers['cwd'] = os.path.dirname(os.path.join(
+        os.path.curdir, file_loc))  # for including screenshots
+
+    return Vulnerability(name, headers=headers, markdown=vulnmarkdown, riskassessment=riskassessment, filename=file_loc)
+
+
+class VulnerabilityList:
+    """Reads a directory for vulnerability definition files, arranges them, and stores the vulnerabilities as objects.
+
+    The class is usually referenced inside the markdown file itself to display the vulnerability information. It keeps the following attributes:
+
+    - scopes : a List of Scope objects corresponding to the vulnerability scopes
+    """
+
+    def __init__(self):
+        self.scopes = []
+
+    def add_from_dir(self, vulndir, env, riskassessment, vulnerability_validation={}, watcher=None):
+        # Make sure it's a directory
+        if not os.path.isdir(vulndir):
+            raise FileNotFoundError("Directory '{0}' doesn't exist. Skipping import of vulnerabilities.".format(
+                vulndir))
+
+        log.info("Reading vulnerabilities")
+        vulnerabilities = []
+
+        scopeintroductions = {}
+
+        # Get the vulnerability writeups from the vulndir
+        for f in os.listdir(vulndir):
+            if watcher:
+                watcher.add_path(vulndir)
+            # Scopes can be split into directories within the vulndir
+            if os.path.isdir(os.path.join(vulndir, f)):
+                if watcher:
+                    watcher.add_path(os.path.join(vulndir, f))
+                log.info(
+                    "* New vulnerability scope in directory '{}'".format((os.path.join(vulndir, f))))
+                vdir = os.path.join(vulndir, f)
+                for v in os.listdir(vdir):
+                    if v == "template.md" or v == "template.md.rr":
+                        continue
+                    if v == "introduction.md" or v == "introduction.md.rr":
+                        scopeintroductions[f] = markdown_from_file(
+                            os.path.join(vdir, v), env=env, watcher=watcher)
+                        continue
+                    fn, ext = os.path.splitext(v)
+                    if ext == ".md" or ext == ".rr":  # Only process markdown files
+                        filename = os.path.join(vdir, v)
+                        log.info(
+                            "  - Reading vulnerability file '{}'".format(filename))
+                        try:
+                            vuln = vuln_from_file(
+                                filename, riskassessment=riskassessment, env=env, vulnerability_validation=vulnerability_validation, scope=f, watcher=watcher)
+                            vulnerabilities += [vuln]
+                        except validation.ValidationError as e:
+                            pass  # ValidationError already raises logs
+                        except Exception as e:
+                            log.error(
+                                "Received exception when processing markdown for vulnerability {}: {}".format(filename, e.args))
+                            log.error(
+                                "Removing markdown for vulnerability {}".format(self.name))
+                            self.markdown = ""
+            else:  # It's a file
+                if f == "template.md" or f == "template.md.rr":
+                    continue
+                if f == "introduction.md" or f == "introduction.md.rr":
+                    scopeintroduction = markdown_from_file(
+                        os.path.join(vulndir, f), env=env, watcher=watcher)
+                    if "scope" in scopeintroduction[0]:
+                        # There's a scope defined in the headers of the introduction
+                        scopeintroductions[f] = scopeintroduction
+                    else:
+                        scopeintroductions[''] = scopeintroduction
+                    continue
+                log.info(
+                    "* Reading vulnerability file '{}'".format(os.path.join(vulndir, f)))
+                fn, ext = os.path.splitext(f)
+                if ext == ".md" or ext == ".rr":  # Only process markdown files
+                    try:
+                        vulnerabilities += [vuln_from_file(
+                            os.path.join(vulndir, f), riskassessment=riskassessment, env=env, watcher=watcher)]
+                    except validation.ValidationError as e:
+                        pass  # ValidationError already raises logs
+                    except Exception as e:
+                        log.error(
+                            "Received exception when processing markdown for vulnerability {}: {}".format(filename, e.args))
+                        log.error(
+                            "Removing markdown for vulnerability {}".format(self.name))
+                        self.markdown = ""
+
+        # Sort the vulnerabilities into scopes
+        scopes = {}
+
+        # This is a marker for the highest risk
+        highestrisk = riskassessment.risks[0]
+        nhighestrisk = 0
+
+        suggest_rc = set()
+        suggest_ar = set()
+
+        # Suggest high level findings
+        for vuln in vulnerabilities:
+            if 'suggest_rc' in vuln.headers:
+                suggest_rc.update(vuln.headers['suggest_rc'])
+            if 'suggest_ar' in vuln.headers:
+                suggest_ar.update(vuln.headers['suggest_ar'])
+
+        for rc in suggest_rc:
+            log.info("Suggested root cause: {}".format(rc))
+        for ar in suggest_ar:
+            log.info("Suggested additional recommendation: {}".format(ar))
+
+        for i in vulnerabilities:
+            if i.nrisk > nhighestrisk:  # We have a new highest risk!
+                nhighestrisk = i.nrisk
+                highestrisk = i.risk
+            if not i.scope in scopes:  # New scope
+                scopes[i.scope] = Scope(i.scope)
+            scopes[i.scope].add_vulnerability(i)
+
+        for scope, introduction in scopeintroductions.items():
+            if scope not in scopes:
+                scopes[scope] = Scope(scope)
+            scopes[scope].set_introduction(introduction[0], introduction[1])
+
+        # Add the highest risk to the variables
+        self.highestrisk = highestrisk
+        env.set_variable('highestrisk', highestrisk)
+        log.info("Highest risk of any vuln is {}".format(highestrisk))
+
+        self.scopes = list(scopes.values())
+        self.scopes.sort()
+
+        # Assign references
+        ref = 1
+        for scope in self.scopes:
+            for vulnerability in scope.vulnerabilities:
+                vulnerability.ref = ref
+                ref += 1
+
+    def get_scope_list(self, validation=None, date=None):
+        scopelist = {}
+        if date:
+            updatedvlist = self.updated(date)
+            scopes = updatedvlist.scopes
+        else:
+            scopes = self.scopes
+        for scope in scopes:
+            scopelist[scope.name] = scope.get_list(validation)
+        return scopelist
+
+    def get_ref(self, vulnerability_name):
+        """ Get the reference of a vulnerability by name. Usually called from a markdown file. """
+        for scope in self.scopes:
+            ref = scope.get_ref(vulnerability_name)
+            if ref:
+                return ref
+        return ""
+
+    def updated(self, date=datetime.date.today()):
+        # Alias for string today
+        if date == "today" or date == "now":
+            date = datetime.date.today()
+
+        newlist = VulnerabilityList()
+        for scope in self.scopes:
+            newlist.scopes.append(scope.updated(date))
+        newlist.scopes.sort()
+        return newlist
+
+    def nvulns(self, riskrating=""):
+        """ Get the number of vulnerabilities with the given risk rating """
+        return sum(scope.nvulns(riskrating) for scope in self.scopes)
+
+    def nriskdict(self):
+        """ Get a dictionary with risk:nrisks for all vulnerabilities """
+        nvulnlist = {}
+        for scope in self.scopes:
+            nvulnlist.update(scope.nriskdict())
+        return nvulnlist
+
+    def nrisklist(self):
+        return oxfordcomma(["{} ({}) {} risk".format(num2words(nrisk), nrisk, risk)
+                            for risk, nrisk in self.nriskdict().items()])
+
+    def generate_markdown(self, env):
+        for scope in self.scopes:
+            scope.generate_markdown(env)
+
+
+class Scope:
+    """ Holds a vulnerability scope, a container for vulnerabilities.
+
+    Has the following attributes:
+
+    name : The name of the scope as a string
+    vulnerabilities : A List of Vulnerability objects, corresponding to the vulnerabilities in this scope.
+                      Should always be sorted by severity and weight.
+    highestrisk : The highest risk in this scope as a string
+    sectionweight : The weight as a number used for ordering the scopes in a VulnerabilityList (highest weight first).
+                    Called sectionweight to have consistency with sections.
+    introduction_headers : The environment headers of an introduction, used for Jinja templating the markdown
+    introduction : The introduction markdown
+    """
+
+    def __init__(self, name, sectionweight=0):
+        self.name = name
+        self.vulnerabilities = []
+        self.highestrisk = 0
+        self.sectionweight = sectionweight
+        self.introduction_headers = {}
+        self.introduction = ""
+
+        # Process the introduction section weight if it's there
+        if "sectionweight" in self.introduction_headers and self.introduction_headers["sectionweight"] > self.sectionweight:
+            log.info(f"Setting sectionweight for {name} to {self.introduction_headers['sectionweight']} based on introduction header")
+            self.sectionweight = self.introduction_headers["sectionweight"]
+
+    def __lt__(self, other):
+        if other.sectionweight == self.sectionweight:
+            return other.highestrisk < self.highestrisk
+        else:
+            return other.sectionweight < self.sectionweight
+
+    def add_vulnerability(self, vulnerability):
+        """ Add a vulnerability to the scope. Automatically sort the vulnerabilities after adding. """
+        self.vulnerabilities.append(vulnerability)
+        if vulnerability.nrisk > self.highestrisk:
+            self.highestrisk = vulnerability.nrisk
+        if vulnerability.sectionweight > self.sectionweight:
+            self.sectionweight = vulnerability.sectionweight
+
+        self.vulnerabilities.sort()
+    
+    def set_introduction(self, introduction_headers, introduction):
+        self.introduction_headers = introduction_headers
+        self.introduction = introduction
+        # Process the introduction section weight if it's there
+        if "sectionweight" in self.introduction_headers and self.introduction_headers["sectionweight"] > self.sectionweight:
+            log.info(f"Setting sectionweight for {self.name} to {self.introduction_headers['sectionweight']} based on introduction header")
+            self.sectionweight = self.introduction_headers["sectionweight"]
+
+    def get_list(self, validation=None):
+        vulnlist = []
+        for vuln in self.vulnerabilities:
+            if validation == None:
+                vulnlist.append(vuln.get_list())
+            else:
+                vl = vuln.get_list()
+                validator = cerberus.Validator()
+                validator.allow_unknown = True
+                if vuln.validate(vl):
+                    vulnlist.append(vuln.get_list())
+        return vulnlist
+
+    def get_ref(self, vulnerability_name):
+        """ Get the reference of a vulnerability by name. Usually called from a markdown file. """
+        for vulnerability in self.vulnerabilities:
+            if vulnerability_name.lower() in vulnerability.name.lower():
+                return vulnerability.ref
+
+        return None
+
+    def nvulns(self, riskrating=""):
+        """ Get the number of vulnerabilities with the given risk rating """
+        return sum(riskrating in vuln.risk for vuln in self.vulnerabilities)
+
+    def nriskdict(self):
+        """ Get a dictionary with risk:nrisks for all vulnerabilities """
+        return Counter(vulnerability.risk for vulnerability in self.vulnerabilities)
+
+    def updated(self, date=datetime.date.today()):
+        """ Process the 'updates' header """
+        newscope = copy.copy(self)
+
+        # Regenerate with the added vulnerabilities
+        newscope.vulnerabilities = []
+        for vuln in self.vulnerabilities:
+            newscope.add_vulnerability(vuln.updated(date))
+
+        return newscope
+
+    def generate_markdown(self, env):
+        for vuln in self.vulnerabilities:
+            vuln.generate_markdown(env)
+        if self.introduction != "":
+            self.introduction = process_template(self.introduction_headers, self.introduction, env)
+
+
+class Vulnerability:
+    """A class for vulnerability markdown.
+
+    Has the following attributes:
+
+     - name : The name of the vulnerability as a string
+     - vulnerability_markdown : The markdown of the vulnerability as a tuple (headers, markdown)
+     - scope : The name of the scope as a string. Used by VulnerabilityList for sorting a bucket of vulnerabilities into scopes,
+                 taken from the headers, but this may be overwritten if it's in a scope bucket already.
+     - weight : A number, used for sorting vulnerabilities. Taken from the headers.
+     - sectionweight : A number, used for increasing the weight of a scope for sorting them. Set for particularly bad vulns. Taken from the headers.
+     - risk : The risk of the vuln as a string.
+     - nrisk : The risk of the vuln as a number. Used for sorting vulnerabilities.
+     - headers : The headers of the markdown.
+    """
+
+    def __init__(self, name, riskassessment, headers=dict(), markdown='', scope='', weight=0, sectionweight=0, filename=''):
+
+        self.name = name
+        self.vulnerability_markdown = markdown
+        self.scope = scope
+        self.ref = 0  # ref will be set by VulnerabilityList
+        self.filename = filename
+        self.riskassessment = riskassessment
+
+        if "riskassessment" in headers:
+            if riskassessment.id not in headers['riskassessment']:
+                raise Exception("Risk assessment {} not in the risk assessment for vulnerability {}".format(
+                    riskassessment.name, name))
+            headers.update(headers['riskassessment'][riskassessment.id])
+
+        if "scope" in headers:
+            self.scope = headers["scope"]
+        else:
+            self.scope = ''
+
+        if "weight" in headers:
+            self.weight = float(headers["weight"])
+        else:
+            self.weight = 0
+
+        if "sectionweight" in headers:
+            self.sectionweight = float(headers["sectionweight"])
+        else:
+            self.sectionweight = 0
+
+        self.risk = riskassessment.get_risk(headers)
+        self.nrisk = next((i for i, x in enumerate(
+            riskassessment.risks) if x == self.risk), 0)
+        headers['risk'] = self.risk
+
+        if "status" not in headers:
+            headers['status'] = "Open"
+
+        self.status = headers['status']
+        self.originalstatus = self.status
+        self.originalrisk = self.risk
+
+        self.headers = headers
+
+    def __lt__(self, other):
+        if other.nrisk == self.nrisk:
+            return other.weight < self.weight
+        else:
+            return other.nrisk < self.nrisk
+
+    def get_list(self):
+        vulnlist = {
+            'name': self.name,
+            'ref': self.ref,
+            'status': self.status,
+            'risk': self.risk,
+            'nrisk': self.nrisk,
+            'originalstatus': self.originalstatus,
+            'originalrisk': self.originalrisk,
+            'filename': self.filename,
+            'headers': self.headers
+        }
+        for stage in self.riskassessment.stages:
+            if stage['name'] in self.headers:
+                vulnlist[stage['name']] = self.headers[stage['name']]
+        return vulnlist
+
+    def updated(self, date=datetime.date.today()):
+        # Get a new vulnerability
+        newvuln = copy.copy(self)
+
+        # Deep headers needs a deep copy otherwise the updates will change the original vuln
+        newvuln.headers = copy.deepcopy(self.headers)
+
+        if 'updates' in self.headers:
+            for update in make_list(self.headers['updates']):
+                if 'date' not in update or update['date'] <= date or date == "all":
+                    for newvar in update.keys():
+                        if newvar == 'date':
+                            continue
+                        newvuln.headers[newvar] = update[newvar]
+
+        # We need to re-evaluate the risk just in case the likelihood or consequence changed
+        newvuln.risk = newvuln.riskassessment.get_risk(newvuln.headers)
+        newvuln.headers['risk'] = newvuln.risk
+        newvuln.status = newvuln.headers['status']
+
+        return newvuln
+
+    def generate_markdown(self, env):
+        """ Get the markdown of the vulnerability, processing the template with the current env.
+
+        Usually called from a markdown file. """
+        # First update the ref
+        self.headers['ref'] = self.ref
+        self.headers['scope'] = self.scope
+
+        try:
+            self.markdown = process_template(self.headers, self.vulnerability_markdown,
+                                             env, name="vulnerability {}".format(self.name), filename=self.filename)
+        except jinja2.exceptions.TemplateSyntaxError as error:
+            log.error("Jinja2 error processing vulnerability {}: {} at lineno {} for file {}".format(
+                self.name, error.message, error.lineno, filename=self.filename))
+            log.error("Removing markdown for vulnerability {}".format(self.name))
+            log_jinja2_error(self.vulnerability_markdown, error)
+            self.markdown = ""
+        except Exception as e:
+            log.error(
+                "Received exception when processing markdown for vulnerability {}: {}".format(self.name, e.args))
+            log.error(traceback.format_exc())
+            log.error("Removing markdown for vulnerability {}".format(self.name))
+            self.markdown = ""
```

### Comparing `Report-Ranger-1.0/setup.py` & `Report-Ranger-2.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['report_ranger']
+['report_ranger',
+ 'report_ranger.imports',
+ 'report_ranger.markdown_renderer',
+ 'report_ranger.output_formatter',
+ 'report_ranger.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['argparse',
  'cerberus',
@@ -15,20 +19,21 @@
  'mistune',
  'num2words',
  'numpy',
  'openpyxl',
  'pandas',
  'plotly',
  'pyyaml',
- 'tabulate']
+ 'tabulate',
+ 'watchdog']
 
 setup_kwargs = {
     'name': 'report-ranger',
-    'version': '1.0',
-    'description': '',
+    'version': '2.0',
+    'description': 'Create a report using markdown files.',
     'long_description': None,
     'author': 'Matthew Strahan',
     'author_email': 'matt@volkis.com.au',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
```

### Comparing `Report-Ranger-1.0/PKG-INFO` & `Report-Ranger-2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: report-ranger
-Version: 1.0
-Summary: 
+Version: 2.0
+Summary: Create a report using markdown files.
 Author: Matthew Strahan
 Author-email: matt@volkis.com.au
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: argparse
 Requires-Dist: cerberus
@@ -15,7 +15,8 @@
 Requires-Dist: num2words
 Requires-Dist: numpy
 Requires-Dist: openpyxl
 Requires-Dist: pandas
 Requires-Dist: plotly
 Requires-Dist: pyyaml
 Requires-Dist: tabulate
+Requires-Dist: watchdog
```

