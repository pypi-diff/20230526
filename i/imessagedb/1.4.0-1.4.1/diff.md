# Comparing `tmp/imessagedb-1.4.0.tar.gz` & `tmp/imessagedb-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imessagedb-1.4.0.tar", max compression
+gzip compressed data, was "imessagedb-1.4.1.tar", max compression
```

## Comparing `imessagedb-1.4.0.tar` & `imessagedb-1.4.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rwxr-xr-x   0        0        0     1070 2023-05-26 03:49:14.716365 imessagedb-1.4.0/LICENSE
--rw-r--r--   0        0        0     9445 2023-05-26 03:49:14.716365 imessagedb-1.4.0/README.md
--rw-r--r--   0        0        0     1336 2023-05-26 03:49:59.784394 imessagedb-1.4.0/pyproject.toml
--rw-r--r--   0        0        0    13233 2023-05-26 03:49:14.732365 imessagedb-1.4.0/src/imessagedb/__init__.py
--rw-r--r--   0        0        0       71 2023-05-26 03:49:14.732365 imessagedb-1.4.0/src/imessagedb/__main__.py
--rw-r--r--   0        0        0     8476 2023-05-26 03:49:14.732365 imessagedb-1.4.0/src/imessagedb/attachment.py
--rw-r--r--   0        0        0     3186 2023-05-26 03:49:14.732365 imessagedb-1.4.0/src/imessagedb/attachments.py
--rw-r--r--   0        0        0     2365 2023-05-26 03:49:14.732365 imessagedb-1.4.0/src/imessagedb/chat.py
--rw-r--r--   0        0        0     4100 2023-05-26 03:49:14.732365 imessagedb-1.4.0/src/imessagedb/chats.py
--rw-r--r--   0        0        0     3300 2023-05-26 03:49:14.732365 imessagedb-1.4.0/src/imessagedb/db.py
--rw-r--r--   0        0        0     3357 2023-05-26 03:49:14.732365 imessagedb-1.4.0/src/imessagedb/default.ini
--rw-r--r--   0        0        0     1092 2023-05-26 03:49:14.732365 imessagedb-1.4.0/src/imessagedb/handle.py
--rw-r--r--   0        0        0     3760 2023-05-26 03:49:14.732365 imessagedb-1.4.0/src/imessagedb/handles.py
--rw-r--r--   0        0        0    29454 2023-05-26 03:49:14.732365 imessagedb-1.4.0/src/imessagedb/html.py
--rw-r--r--   0        0        0     5037 2023-05-26 03:49:14.732365 imessagedb-1.4.0/src/imessagedb/message.py
--rw-r--r--   0        0        0     6222 2023-05-26 03:49:14.732365 imessagedb-1.4.0/src/imessagedb/messages.py
--rw-r--r--   0        0        0     6655 2023-05-26 03:49:14.732365 imessagedb-1.4.0/src/imessagedb/text.py
--rw-r--r--   0        0        0      677 2023-05-26 03:49:14.732365 imessagedb-1.4.0/src/imessagedb/utils.py
--rw-r--r--   0        0        0    10199 1970-01-01 00:00:00.000000 imessagedb-1.4.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1070 2023-05-26 04:18:46.971686 imessagedb-1.4.1/LICENSE
+-rw-r--r--   0        0        0     9445 2023-05-26 04:18:46.971686 imessagedb-1.4.1/README.md
+-rw-r--r--   0        0        0     1336 2023-05-26 04:19:27.055192 imessagedb-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0    13235 2023-05-26 04:18:46.983686 imessagedb-1.4.1/src/imessagedb/__init__.py
+-rw-r--r--   0        0        0       71 2023-05-26 04:18:46.983686 imessagedb-1.4.1/src/imessagedb/__main__.py
+-rw-r--r--   0        0        0     8476 2023-05-26 04:18:46.983686 imessagedb-1.4.1/src/imessagedb/attachment.py
+-rw-r--r--   0        0        0     3186 2023-05-26 04:18:46.983686 imessagedb-1.4.1/src/imessagedb/attachments.py
+-rw-r--r--   0        0        0     2365 2023-05-26 04:18:46.983686 imessagedb-1.4.1/src/imessagedb/chat.py
+-rw-r--r--   0        0        0     4100 2023-05-26 04:18:46.983686 imessagedb-1.4.1/src/imessagedb/chats.py
+-rw-r--r--   0        0        0     3300 2023-05-26 04:18:46.983686 imessagedb-1.4.1/src/imessagedb/db.py
+-rw-r--r--   0        0        0     3357 2023-05-26 04:18:46.983686 imessagedb-1.4.1/src/imessagedb/default.ini
+-rw-r--r--   0        0        0     1092 2023-05-26 04:18:46.983686 imessagedb-1.4.1/src/imessagedb/handle.py
+-rw-r--r--   0        0        0     3760 2023-05-26 04:18:46.983686 imessagedb-1.4.1/src/imessagedb/handles.py
+-rw-r--r--   0        0        0    30347 2023-05-26 04:18:46.983686 imessagedb-1.4.1/src/imessagedb/html.py
+-rw-r--r--   0        0        0     5037 2023-05-26 04:18:46.983686 imessagedb-1.4.1/src/imessagedb/message.py
+-rw-r--r--   0        0        0     6222 2023-05-26 04:18:46.983686 imessagedb-1.4.1/src/imessagedb/messages.py
+-rw-r--r--   0        0        0     6655 2023-05-26 04:18:46.983686 imessagedb-1.4.1/src/imessagedb/text.py
+-rw-r--r--   0        0        0      677 2023-05-26 04:18:46.983686 imessagedb-1.4.1/src/imessagedb/utils.py
+-rw-r--r--   0        0        0    10199 1970-01-01 00:00:00.000000 imessagedb-1.4.1/PKG-INFO
```

### Comparing `imessagedb-1.4.0/LICENSE` & `imessagedb-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `imessagedb-1.4.0/README.md` & `imessagedb-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `imessagedb-1.4.0/pyproject.toml` & `imessagedb-1.4.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "imessagedb"
-version = "1.4.0"
+version = "1.4.1"
 description = "Reads and displays the Apple iMessage database"
 authors = ["xev <git@schore.org>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `imessagedb-1.4.0/src/imessagedb/__init__.py` & `imessagedb-1.4.1/src/imessagedb/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,15 +204,15 @@
         config.set(CONTROL, 'output type', args.output_type)
     if args.force:
         config.set(CONTROL, 'force copy', 'True')
     if args.no_attachments:
         config.set(CONTROL, 'skip attachments', 'True')
     if args.inline:
         config.set(DISPLAY, 'inline attachments', 'True')
-    if args.split_line:
+    if args.split_output:
         config.set(DISPLAY, 'split output', args.split_output)
 
     start_date = None
     end_date = None
     if args.start_time:
         try:
             start_date = dateutil.parser.parse(args.start_time)
```

### Comparing `imessagedb-1.4.0/src/imessagedb/attachment.py` & `imessagedb-1.4.1/src/imessagedb/attachment.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.4.0/src/imessagedb/attachments.py` & `imessagedb-1.4.1/src/imessagedb/attachments.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.4.0/src/imessagedb/chat.py` & `imessagedb-1.4.1/src/imessagedb/chat.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.4.0/src/imessagedb/chats.py` & `imessagedb-1.4.1/src/imessagedb/chats.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.4.0/src/imessagedb/db.py` & `imessagedb-1.4.1/src/imessagedb/db.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.4.0/src/imessagedb/default.ini` & `imessagedb-1.4.1/src/imessagedb/default.ini`

 * *Files identical despite different names*

### Comparing `imessagedb-1.4.0/src/imessagedb/handle.py` & `imessagedb-1.4.1/src/imessagedb/handle.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.4.0/src/imessagedb/handles.py` & `imessagedb-1.4.1/src/imessagedb/handles.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.4.0/src/imessagedb/html.py` & `imessagedb-1.4.1/src/imessagedb/html.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,16 +113,15 @@
         if end_time:
             date_string = f"{date_string} until {end_time}"
 
         self._file_header_string = f'  <div id="file_summary">Exchanged {len(self._messages):,} total messages with ' \
                                    f'{self._messages.title}{date_string}.</div><p>\n'
 
         self._html_array.append(self._generate_table(self._messages))
-        self._print_and_save('</body>\n</html>\n',
-                             self._html_array)
+        self._print_and_save('</body>\n</html>\n', self._html_array, eof=True)
 
     def __repr__(self) -> str:
         return ''.join(self._html_array)
 
     def save(self, filename: str) -> None:
         """ Write the output to the output file"""
         file_handle = open(filename, "w")
@@ -131,46 +130,60 @@
         return
 
     def print(self) -> None:
         """ Print the output to stdout """
         print('\n'.join(self._html_array))
         return
 
-    def _print_and_save(self, message: str, array: list, new_day: bool = False) -> None:
+    def _print_and_save(self, message: str, array: list, new_day: bool = False, eof: bool = False) -> None:
         """ Save to the output file while it is processing """
 
         if self._current_messages_processed == 0:
             # If this is a new file, because it is either the first pass through, or if we need to create new file
 
             new_file_array = [self._generate_head(), "<body>\n", self._file_header_string,
                               f'{" ":2s}<div class="picboxframe"  id="picbox"> <img src="" /> </div>\n',
-                              f'{" ":2s}<table>\n{" ":4s}<tr>\n']
+                              f'{" ":2s}<table style="table-layout: fixed;">\n{" ":4s}<tr>\n']
             if self._previous_output_filename:
-                new_file_array.append(f'{" ":6s}<td style="text-align: left;">'
+                new_file_array.append(f'{" ":6s}<td style="text-align: left; width: 33%;">'
                                       f'<a href="file://{self._previous_output_filename}"> &lt </a> </td>\n'
-                                      f'{" ":6s}<td style="text-align: center;"><div class="next_file">' +
+                                      f'{" ":6s}<td style="text-align: center; width: 33%;"><div class="next_file">' +
                                       f'<a href="file://{self._previous_output_filename}">' +
                                       f' Previous Messages {self._previous_range}</a></div></td>\n')
             else:
-                new_file_array.append(f'{" ":6s}<td> </td>\n{" ":6s}<td> </td>\n')
+                new_file_array.append(f'{" ":6s}<td style="width: 33%;"> </td>\n'
+                                      f'{" ":6s}<td style="width: 33%;"> </td>\n')
 
-            new_file_array.append(f'{" ":6s}<td style="text-align: right;" id="next_page"> </td>\n'
+            new_file_array.append(f'{" ":6s}<td style="text-align: right; width: 33%;" id="next_page"> </td>\n'
                                   f'{" ":4s}</tr>\n{" ":2s}</table>\n\n')
             new_file_array.append(f'{" ":2s}<table class="main_table">\n{" ":2s}</table>\n')
 
             for i in new_file_array:
                 array.append(i)
                 if self._output_filename is not None:
                     print(i, end="", file=self._output_file_handle)
 
         array.append(message)
         self._current_messages_processed += 1
         if self._output_filename is None:  # We are not writing to a file
             return
 
+        if eof:
+            # Normally this gets done on the file split, but the eof indicates its last file, so do it
+            #  on the last write
+
+            description_string = f' This page contains {self._current_messages_processed:,} messages from ' \
+                                 f'{self._file_start_date.strftime("%A %Y-%m-%d")} to ' \
+                                 f'{self._file_end_date.strftime("%A %Y-%m-%d")}.'
+            print(f' <script>\n'
+                  f'  el = document.getElementById("file_summary")\n'
+                  f'  new_text = el.innerHTML.concat("{description_string}")\n'
+                  f'  el.innerHTML = new_text\n',
+                  f' </script>\n', file=self._output_file_handle)
+
         print(message, end="", file=self._output_file_handle)
 
         if new_day and 0 < self._split_output < self._current_messages_processed:
             total_processed = self._current_messages_processed
             self._current_messages_processed = 0
             self._current_messages_file += 1
             self._previous_output_filename = self._current_output_filename
@@ -185,15 +198,15 @@
                                    f'({self._file_start_date.strftime("%A %Y-%m-%d")} to ' \
                                    f'{self._file_end_date.strftime("%A %Y-%m-%d")})</div>'
             print(f' <script>\n'
                   f'  el = document.getElementById("file_summary")\n'
                   f'  new_text = el.innerHTML.concat("{description_string}")\n'
                   f'  el.innerHTML = new_text\n'
                   f'  document.getElementById("next_page").innerHTML = '
-                  f'   "<a href=\'file://{self._current_output_filename}\'> &gt </a>"\n'
+                  f'   "<a href=\'file://{self._current_output_filename}\'> Next Page &gt </a>"\n'
                   f' </script>', file=self._output_file_handle)
             print('</body>\n</html>\n', end="", file=self._output_file_handle)
             self._output_file_handle.close()
             print(f"Creating output file {self._current_output_filename}")
             self._output_file_handle = open(self._current_output_filename, "w")
 
     def _generate_thread_row(self, message: Message) -> str:
```

### Comparing `imessagedb-1.4.0/src/imessagedb/message.py` & `imessagedb-1.4.1/src/imessagedb/message.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.4.0/src/imessagedb/messages.py` & `imessagedb-1.4.1/src/imessagedb/messages.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.4.0/src/imessagedb/text.py` & `imessagedb-1.4.1/src/imessagedb/text.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.4.0/src/imessagedb/utils.py` & `imessagedb-1.4.1/src/imessagedb/utils.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.4.0/PKG-INFO` & `imessagedb-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imessagedb
-Version: 1.4.0
+Version: 1.4.1
 Summary: Reads and displays the Apple iMessage database
 License: MIT
 Author: xev
 Author-email: git@schore.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

