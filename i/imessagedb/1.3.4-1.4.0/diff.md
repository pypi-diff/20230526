# Comparing `tmp/imessagedb-1.3.4.tar.gz` & `tmp/imessagedb-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imessagedb-1.3.4.tar", max compression
+gzip compressed data, was "imessagedb-1.4.0.tar", max compression
```

## Comparing `imessagedb-1.3.4.tar` & `imessagedb-1.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rwxr-xr-x   0        0        0     1070 2023-05-25 14:27:25.168008 imessagedb-1.3.4/LICENSE
--rw-r--r--   0        0        0     9251 2023-05-25 14:27:25.168008 imessagedb-1.3.4/README.md
--rw-r--r--   0        0        0     1309 2023-05-25 14:27:58.251901 imessagedb-1.3.4/pyproject.toml
--rw-r--r--   0        0        0    12623 2023-05-25 14:27:25.180008 imessagedb-1.3.4/src/imessagedb/__init__.py
--rw-r--r--   0        0        0       71 2023-05-25 14:27:25.180008 imessagedb-1.3.4/src/imessagedb/__main__.py
--rw-r--r--   0        0        0     8476 2023-05-25 14:27:25.180008 imessagedb-1.3.4/src/imessagedb/attachment.py
--rw-r--r--   0        0        0     3186 2023-05-25 14:27:25.180008 imessagedb-1.3.4/src/imessagedb/attachments.py
--rw-r--r--   0        0        0     2365 2023-05-25 14:27:25.180008 imessagedb-1.3.4/src/imessagedb/chat.py
--rw-r--r--   0        0        0     4100 2023-05-25 14:27:25.180008 imessagedb-1.3.4/src/imessagedb/chats.py
--rw-r--r--   0        0        0     3300 2023-05-25 14:27:25.180008 imessagedb-1.3.4/src/imessagedb/db.py
--rw-r--r--   0        0        0     3357 2023-05-25 14:27:25.180008 imessagedb-1.3.4/src/imessagedb/default.ini
--rw-r--r--   0        0        0     1092 2023-05-25 14:27:25.180008 imessagedb-1.3.4/src/imessagedb/handle.py
--rw-r--r--   0        0        0     3760 2023-05-25 14:27:25.180008 imessagedb-1.3.4/src/imessagedb/handles.py
--rw-r--r--   0        0        0    24304 2023-05-25 14:27:25.180008 imessagedb-1.3.4/src/imessagedb/html.py
--rw-r--r--   0        0        0     4975 2023-05-25 14:27:25.180008 imessagedb-1.3.4/src/imessagedb/message.py
--rw-r--r--   0        0        0     6269 2023-05-25 14:27:25.180008 imessagedb-1.3.4/src/imessagedb/messages.py
--rw-r--r--   0        0        0     6655 2023-05-25 14:27:25.180008 imessagedb-1.3.4/src/imessagedb/text.py
--rw-r--r--   0        0        0      677 2023-05-25 14:27:25.180008 imessagedb-1.3.4/src/imessagedb/utils.py
--rw-r--r--   0        0        0     9957 1970-01-01 00:00:00.000000 imessagedb-1.3.4/PKG-INFO
+-rwxr-xr-x   0        0        0     1070 2023-05-26 03:49:14.716365 imessagedb-1.4.0/LICENSE
+-rw-r--r--   0        0        0     9445 2023-05-26 03:49:14.716365 imessagedb-1.4.0/README.md
+-rw-r--r--   0        0        0     1336 2023-05-26 03:49:59.784394 imessagedb-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0    13233 2023-05-26 03:49:14.732365 imessagedb-1.4.0/src/imessagedb/__init__.py
+-rw-r--r--   0        0        0       71 2023-05-26 03:49:14.732365 imessagedb-1.4.0/src/imessagedb/__main__.py
+-rw-r--r--   0        0        0     8476 2023-05-26 03:49:14.732365 imessagedb-1.4.0/src/imessagedb/attachment.py
+-rw-r--r--   0        0        0     3186 2023-05-26 03:49:14.732365 imessagedb-1.4.0/src/imessagedb/attachments.py
+-rw-r--r--   0        0        0     2365 2023-05-26 03:49:14.732365 imessagedb-1.4.0/src/imessagedb/chat.py
+-rw-r--r--   0        0        0     4100 2023-05-26 03:49:14.732365 imessagedb-1.4.0/src/imessagedb/chats.py
+-rw-r--r--   0        0        0     3300 2023-05-26 03:49:14.732365 imessagedb-1.4.0/src/imessagedb/db.py
+-rw-r--r--   0        0        0     3357 2023-05-26 03:49:14.732365 imessagedb-1.4.0/src/imessagedb/default.ini
+-rw-r--r--   0        0        0     1092 2023-05-26 03:49:14.732365 imessagedb-1.4.0/src/imessagedb/handle.py
+-rw-r--r--   0        0        0     3760 2023-05-26 03:49:14.732365 imessagedb-1.4.0/src/imessagedb/handles.py
+-rw-r--r--   0        0        0    29454 2023-05-26 03:49:14.732365 imessagedb-1.4.0/src/imessagedb/html.py
+-rw-r--r--   0        0        0     5037 2023-05-26 03:49:14.732365 imessagedb-1.4.0/src/imessagedb/message.py
+-rw-r--r--   0        0        0     6222 2023-05-26 03:49:14.732365 imessagedb-1.4.0/src/imessagedb/messages.py
+-rw-r--r--   0        0        0     6655 2023-05-26 03:49:14.732365 imessagedb-1.4.0/src/imessagedb/text.py
+-rw-r--r--   0        0        0      677 2023-05-26 03:49:14.732365 imessagedb-1.4.0/src/imessagedb/utils.py
+-rw-r--r--   0        0        0    10199 1970-01-01 00:00:00.000000 imessagedb-1.4.0/PKG-INFO
```

### Comparing `imessagedb-1.3.4/LICENSE` & `imessagedb-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `imessagedb-1.3.4/README.md` & `imessagedb-1.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -65,18 +65,18 @@
                         The type of output
   -i, --inline          Show the attachments inline
   -f, --force           Force a copy of the attachments
   --no_copy             Don't copy the attachments
   --no_attachments      Don't process attachments at all
   -v, --verbose         Turn on additional output
   --start_time START_TIME
-                        The start time of the messages in YYYY-MM-DD HH:MM:SS
-                        format
-  --end_time END_TIME   The end time of the messages in YYYY-MM-DD HH:MM:SS
-                        format
+                        The start time of the messages
+  --end_time END_TIME   The end time of the messages
+  --split_output SPLIT_OUTPUT
+                        Split the html output into files with this many messages per file
   --version             Show the version number and exit
   --get_handles         Display the list of handles in the database and exit
   --get_chats           Display the list of chats in the database and exit
 ```
 
 #### Command line options
 
@@ -104,19 +104,21 @@
 
 **-m ME, --me ME** The name to use to refer to you in the output. If this option is not 
 provided it will default to `Me`.
 
 **-t {text,html}, --output_type {text,html}** The type of output, either *text* or *html*. 
 If this option is not provided it will default to `html`.
 
-
 **--start_time START_TIME** <br>
 **--end_time END_TIME** By default, the program will process all messages. If you want
 to restrict that to particular timeframe, you can specify the `--start-time` and/or `--end_time`
-options in the  YYYY-MM-DD HH:MM:SS  format
+options
+
+**--split_output SPLIT_OUTPUT** Split the html output into files with this many messages 
+per file
 
 **-i, --inline**   Show the attachments inline. By default, the attachments will show as links
 that you can hover over and it will pop up the attachment. With this option, it will put them
 inline, which will make your output much busier and take a lot more memory in your browser.
 
 **-f, --force**  Force a copy of the attachments. By default, if the attachment already exists
 in the destination directory, it will not re-copy the file, but this will force it to re-copy it.
@@ -126,15 +128,14 @@
 
 **--no_attachments**      Do not show the attachments at all
 
 **-v, --verbose**         Turn on additional output
 
 **--version**  Shows the version number and exits
 
-
 **--get_handles** Display the list of handles in the database and exit
 
 **--get_chats** Display the list of chats in the database and exit
 ### Configuration File
 
 The configuration file is in configparser format. Here is the template that is created
 by default:
@@ -174,14 +175,18 @@
 
 [DISPLAY]
 
 # Output type, either html or text
 
 output_type = html
 
+# Number of messages in each html file. If this is 0 or not specified, it will be one large file.
+
+output split = 1000
+
 # Inline attachments mean that the images are in the HTML instead of loaded when hovered over
 
 inline attachments = False
 
 # Popup location is where the attachment popup window shows up, and is either 'upper right', 'upper left' or 'floating'
 
 popup location = upper right
```

### Comparing `imessagedb-1.3.4/pyproject.toml` & `imessagedb-1.4.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "imessagedb"
-version = "1.3.4"
+version = "1.4.0"
 description = "Reads and displays the Apple iMessage database"
 authors = ["xev <git@schore.org>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 alive-progress = "^3.1.2"
 ffmpeg-python = "^0.2.0"
 heic2png = "^1.0.0"
 configparser = "^5.3.0"
 termcolor = "^2.3.0"
+python-dateutil = "^2.8.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
 myst-nb = {version = "^0.17.2", python = "^3.9"}
 sphinx-autoapi = "^2.1.0"
 sphinx-rtd-theme = "^1.2.0"
```

### Comparing `imessagedb-1.3.4/src/imessagedb/__init__.py` & `imessagedb-1.4.0/src/imessagedb/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 __version__ = version("imessagedb")
 
 import os
 import configparser
 import logging
 import argparse
 import sys
-from datetime import datetime
+import dateutil.parser
 from imessagedb.db import DB
 from imessagedb.utils import *
 
 DEFAULT_CONFIGURATION = '''
 [CONTROL]
 
 # Whether or not to copy the attachments into a different directory. This is needed for two reasons:
@@ -50,15 +50,21 @@
 
 verbose = True
 
 [DISPLAY]
 
 # Output type, either html or text
 
-output_type = html
+output type = html
+
+# Number of messages in each html file. If this is 0 or not specified, it will be one large file.
+#  There may be more messages than this per file, as it splits at the next date change after that number 
+#  of messages. 
+
+split output = 1000
 
 # Inline attachments mean that the images are in the HTML instead of loaded when hovered over
 
 inline attachments = False
 
 # Popup location is where the attachment popup window shows up, and is either 'upper right', 'upper left' or 'floating'
 
@@ -157,21 +163,25 @@
     argument_parser.add_argument("-t", "--output_type", help="The type of output", choices=["text", "html"])
     argument_parser.add_argument("-i", "--inline", help="Show the attachments inline", action="store_true")
     copy_mutex_group = argument_parser.add_mutually_exclusive_group()
     copy_mutex_group.add_argument("-f", "--force", help="Force a copy of the attachments", action="store_true")
     copy_mutex_group.add_argument("--no_copy", help="Don't copy the attachments", action="store_true")
     argument_parser.add_argument("--no_attachments", help="Don't process attachments at all", action="store_true")
     argument_parser.add_argument("-v", "--verbose", help="Turn on additional output", action="store_true")
-    argument_parser.add_argument('--start_time', help="The start time of the messages in YYYY-MM-DD HH:MM:SS format")
-    argument_parser.add_argument('--end_time', help="The end time of the messages in YYYY-MM-DD HH:MM:SS format")
-    argument_parser.add_argument('--version', help="Prints the version number", action="store_true")
+    argument_parser.add_argument('--start_time', '--start-time',
+                                 help="The start date/time of the messages")
+    argument_parser.add_argument('--end_time', '--end-time',
+                                 help="The end date/time of the messages")
+    argument_parser.add_argument('--split_output', '--split-output',
+                                 help="Split the html output into files with this many messages per file")
     argument_parser.add_argument('--get_handles', '--get-handles',
                                  help="Display the list of handles in the database and exit", action="store_true")
     argument_parser.add_argument('--get_chats', '--get-chats',
                                  help="Display the list of chats in the database and exit", action="store_true")
+    argument_parser.add_argument('--version', help="Prints the version number", action="store_true")
 
     args = argument_parser.parse_args()
 
     if args.version:
         print(f"imessagedb {__version__}", file=sys.stderr)
         exit(0)
 
@@ -194,28 +204,30 @@
         config.set(CONTROL, 'output type', args.output_type)
     if args.force:
         config.set(CONTROL, 'force copy', 'True')
     if args.no_attachments:
         config.set(CONTROL, 'skip attachments', 'True')
     if args.inline:
         config.set(DISPLAY, 'inline attachments', 'True')
+    if args.split_line:
+        config.set(DISPLAY, 'split output', args.split_output)
 
     start_date = None
     end_date = None
     if args.start_time:
         try:
-            start_date = datetime.strptime(args.start_time, '%Y-%m-%d %H:%M:%S')
+            start_date = dateutil.parser.parse(args.start_time)
         except ValueError as exp:
             argument_parser.print_help(sys.stderr)
             print(f"\n **Start time not correct: {exp}", file=sys.stderr)
             exit(1)
         config.set(CONTROL, 'start time', str(start_date))
     if args.end_time:
         try:
-            end_date = datetime.strptime(args.end_time, '%Y-%m-%d %H:%M:%S')
+            end_date = dateutil.parser.parse(args.end_time)
         except ValueError as exp:
             argument_parser.print_help(sys.stderr)
             print(f"\n** End time not correct: {exp}", file=sys.stderr)
             exit(1)
         config.set(CONTROL, 'end time', str(end_date))
     if start_date and end_date and start_date >= end_date:
         argument_parser.print_help(sys.stderr)
@@ -229,14 +241,16 @@
 
     person = None
     numbers = None
 
     if not generic_database_request:
         if args.chat:
             person = f"chat_{args.chat}"
+            if args.name:
+                person = args.name
         else:
             if args.handle:
                 numbers = args.handle
                 if args.name:
                     person = args.name
                 else:
                     person = ', '.join(numbers)
@@ -258,16 +272,14 @@
 
         copy_directory = config[CONTROL].get('copy directory', fallback=os.environ['HOME'])
         if copy_directory == "HOME":
             copy_directory = os.environ['HOME']
         attachment_directory = f"{copy_directory}/{safe_filename(person)}_attachments"
         config[CONTROL]['attachment directory'] = attachment_directory
 
-        filename = f'{safe_filename(person)}.html'
-        out = open(f"{copy_directory}/{filename}", 'w')
         try:
             os.mkdir(attachment_directory)
         except FileExistsError:
             pass
 
     # Connect to the database
 
@@ -290,35 +302,39 @@
                 error_string = f"You have {len(chats)} chats named {args.chat}, " \
                                f"but this program can only handle the case where there is one. " \
                                f"Rename your group and try again."
                 logger.error(error_string)
                 exit(1)
             chat_id = chats[0].rowid
             title = args.chat
-        elif args.chat in database.chats.chat_list:
-            chat_id = args.chat
+        elif int(args.chat) in database.chats.chat_list:
+            chat_id = int(args.chat)
             if database.chats.chat_list[chat_id].chat_name:
                 title = database.chats.chat_list[chat_id].chat_name
+            elif args.name:
+                title = args.name
             else:
                 title = chat_id
         else:
             logger.error(f"{args.chat} not recognized as a chat. Run 'imessagedb --get_chats' to get the list of chats")
             argument_parser.print_help()
             exit(1)
 
         message_list = database.Messages('chat', title, chat_id=chat_id)
     else:
 
         message_list = database.Messages('person', person, numbers=numbers)
 
     me = config.get('DISPLAY', 'me', fallback='Me')
+
+    filename = os.path.join(copy_directory, safe_filename(person))
     output_type = config[CONTROL].get('output type', fallback='html')
     if output_type == 'text':
         database.TextOutput(me, message_list, output_file=out).print()
     else:
-        database.HTMLOutput(me, message_list, output_file=out)
+        database.HTMLOutput(me, message_list, output_file=filename)
 
     database.disconnect()
 
 
 if __name__ == '__main__':
     run()
```

### Comparing `imessagedb-1.3.4/src/imessagedb/attachment.py` & `imessagedb-1.4.0/src/imessagedb/attachment.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.3.4/src/imessagedb/attachments.py` & `imessagedb-1.4.0/src/imessagedb/attachments.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.3.4/src/imessagedb/chat.py` & `imessagedb-1.4.0/src/imessagedb/chat.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.3.4/src/imessagedb/chats.py` & `imessagedb-1.4.0/src/imessagedb/chats.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.3.4/src/imessagedb/db.py` & `imessagedb-1.4.0/src/imessagedb/db.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.3.4/src/imessagedb/default.ini` & `imessagedb-1.4.0/src/imessagedb/default.ini`

 * *Files identical despite different names*

### Comparing `imessagedb-1.3.4/src/imessagedb/handle.py` & `imessagedb-1.4.0/src/imessagedb/handle.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.3.4/src/imessagedb/handles.py` & `imessagedb-1.4.0/src/imessagedb/handles.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.3.4/src/imessagedb/html.py` & `imessagedb-1.4.0/src/imessagedb/html.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,17 +2,16 @@
 import re
 import string
 import imessagedb
 from imessagedb.message import Message
 from imessagedb.messages import Messages
 from alive_progress import alive_bar
 
-
-url_pattern = re.compile(r"((https?):((//)|(\\\\))+[\w\d:#@%/;$()~_?\+-=\\\.&]*)", re.MULTILINE | re.UNICODE)
-mailto_pattern = re.compile(r"([\w\-\.]+@(\w[\w\-]+\.)+[\w\-]+)", re.MULTILINE | re.UNICODE)
+url_pattern = re.compile(r'((https?):((//)|(\\\\))+[\w\d:#@%/;$()~_?+-=\\.&]*)', re.MULTILINE | re.UNICODE)
+mailto_pattern = re.compile(r'([\w\-.]+@(\w[\w\-]+\.)+[\w\-]+)', re.MULTILINE | re.UNICODE)
 
 
 def _replace_url_to_link(value: str) -> str:
     """ From https://gist.github.com/guillaumepiot/4539986 """
 
     # Replace url to link
     value = url_pattern.sub(r'<a href="\1" target="_blank">\1</a>', value)
@@ -28,15 +27,15 @@
 
     There are a number of options in the configuration file that affect how the HTML is created.
     In the CONTROL section, the following impact the output:
 
     copy = True :
                 If the attachments are not copied, they are not available on the HTML output.
                 There are two reasons for that. 1) The web browser does not have access to the directory
-                that the attachments are stored, so it cannot display them 2) Some of the attachments need
+                that the attachments are stored, so it cannot display them 2) Some attachments need
                 to be converted in order to be viewed in the browser, and need a place to live.
 
     skip attachments = False :
                 If true, attachments will not be available in the HTML output
 
     In the DISPLAY section, the following impact the output:
 
@@ -57,15 +56,15 @@
         first person in the conversation, the second for the second, third for the third, etc. If there are more
         participants than colors, it will wrap around to the first color.
 
     thread background = HoneyDew :
         The background color of the thread in replies
     """
 
-    def __init__(self, database, me: str, messages: Messages, inline=False, output_file=None) -> None:
+    def __init__(self, database, me: str, messages: Messages, inline: bool = False, output_file: str = None) -> None:
         """
             Parameters
             ----------
             database : imessagedb.DB
                 An instance of a connected database
 
             me : str
@@ -73,71 +72,139 @@
 
             messages: imessagedb.DB.Messages
                  The messages
 
             inline : bool
                 Display attachments inline or not
 
-            output_filename : str
+            output_file : str
                 The name of the output file"""
 
         self._database = database
         self._me = me
         self._messages = messages
         self._attachment_list = self._database.attachment_list
         self._inline = inline
-        self._output_file = output_file
 
         self._name_map = {}
         self._color_list = self._get_next_color()
         self._day = 'UNK'
         self._html_array = []
-        self._print_and_save(self._generate_head(), self._html_array)
-        self._print_and_save("<body>\n", self._html_array)
+        self._current_messages_processed = 0
+        self._current_messages_file = 0
+        self._file_start_date: datetime = None
+        self._file_end_date: datetime = None
+        self._previous_range: str = None
+        self._last_row_had_conversion = False
+
+        if output_file is not None:
+            self._output_filename = output_file
+            self._split_output = self._database.config.getint('DISPLAY', 'split output', fallback=0)
+            self._previous_output_filename = None
+            self._current_output_filename = f"{self._output_filename}.html"
+            self._output_file_handle = open(self._current_output_filename, "w")
+        else:
+            self._output_filename = None
 
         start_time = self._database.control.get('start time', fallback=None)
         end_time = self._database.control.get('end time', fallback=None)
         date_string = ""
         if start_time:
-            date_string = f"from {start_time} "
+            date_string = f" from {start_time}"
         if end_time:
             date_string = f"{date_string} until {end_time}"
 
-        self._print_and_save(f"Exchanged {len(self._messages):,} messages with " +
-                             f"{self._messages.title} {date_string}<p>\n",
-                             self._html_array)
-        self._print_and_save(f'{" ":2s}<div class="picboxframe"  id="picbox"> <img src="" /> </div>\n',
-                             self._html_array)
+        self._file_header_string = f'  <div id="file_summary">Exchanged {len(self._messages):,} total messages with ' \
+                                   f'{self._messages.title}{date_string}.</div><p>\n'
 
         self._html_array.append(self._generate_table(self._messages))
         self._print_and_save('</body>\n</html>\n',
                              self._html_array)
 
     def __repr__(self) -> str:
         return ''.join(self._html_array)
 
-    def save(self) -> None:
+    def save(self, filename: str) -> None:
         """ Write the output to the output file"""
-        print('\n'.join(self._html_array), file=self._output_file)
+        file_handle = open(filename, "w")
+        print('\n'.join(self._html_array), file=file_handle)
+        file_handle.close()
         return
 
     def print(self) -> None:
         """ Print the output to stdout """
         print('\n'.join(self._html_array))
         return
 
-    def _print_and_save(self, message: str, array: list) -> None:
+    def _print_and_save(self, message: str, array: list, new_day: bool = False) -> None:
         """ Save to the output file while it is processing """
+
+        if self._current_messages_processed == 0:
+            # If this is a new file, because it is either the first pass through, or if we need to create new file
+
+            new_file_array = [self._generate_head(), "<body>\n", self._file_header_string,
+                              f'{" ":2s}<div class="picboxframe"  id="picbox"> <img src="" /> </div>\n',
+                              f'{" ":2s}<table>\n{" ":4s}<tr>\n']
+            if self._previous_output_filename:
+                new_file_array.append(f'{" ":6s}<td style="text-align: left;">'
+                                      f'<a href="file://{self._previous_output_filename}"> &lt </a> </td>\n'
+                                      f'{" ":6s}<td style="text-align: center;"><div class="next_file">' +
+                                      f'<a href="file://{self._previous_output_filename}">' +
+                                      f' Previous Messages {self._previous_range}</a></div></td>\n')
+            else:
+                new_file_array.append(f'{" ":6s}<td> </td>\n{" ":6s}<td> </td>\n')
+
+            new_file_array.append(f'{" ":6s}<td style="text-align: right;" id="next_page"> </td>\n'
+                                  f'{" ":4s}</tr>\n{" ":2s}</table>\n\n')
+            new_file_array.append(f'{" ":2s}<table class="main_table">\n{" ":2s}</table>\n')
+
+            for i in new_file_array:
+                array.append(i)
+                if self._output_filename is not None:
+                    print(i, end="", file=self._output_file_handle)
+
         array.append(message)
-        if self._output_file:
-            print(message, end="", file=self._output_file)
+        self._current_messages_processed += 1
+        if self._output_filename is None:  # We are not writing to a file
+            return
+
+        print(message, end="", file=self._output_file_handle)
+
+        if new_day and 0 < self._split_output < self._current_messages_processed:
+            total_processed = self._current_messages_processed
+            self._current_messages_processed = 0
+            self._current_messages_file += 1
+            self._previous_output_filename = self._current_output_filename
+            self._current_output_filename = f"{self._output_filename}_{self._current_messages_file:02d}.html"
+
+            print(f'    <p><div class="next_file"><a href="file://{self._current_output_filename}">'
+                  f' Next Messages </a></div>\n', end="", file=self._output_file_handle)
+            description_string = f' This page contains {total_processed:,} messages from ' \
+                                 f'{self._file_start_date.strftime("%A %Y-%m-%d")} to ' \
+                                 f'{self._file_end_date.strftime("%A %Y-%m-%d")}.'
+            self._previous_range = f'<br><div style="font-size: 50%;">' \
+                                   f'({self._file_start_date.strftime("%A %Y-%m-%d")} to ' \
+                                   f'{self._file_end_date.strftime("%A %Y-%m-%d")})</div>'
+            print(f' <script>\n'
+                  f'  el = document.getElementById("file_summary")\n'
+                  f'  new_text = el.innerHTML.concat("{description_string}")\n'
+                  f'  el.innerHTML = new_text\n'
+                  f'  document.getElementById("next_page").innerHTML = '
+                  f'   "<a href=\'file://{self._current_output_filename}\'> &gt </a>"\n'
+                  f' </script>', file=self._output_file_handle)
+            print('</body>\n</html>\n', end="", file=self._output_file_handle)
+            self._output_file_handle.close()
+            print(f"Creating output file {self._current_output_filename}")
+            self._output_file_handle = open(self._current_output_filename, "w")
 
     def _generate_thread_row(self, message: Message) -> str:
-        who_data = self._get_name(message.handle_id)
-        who = who_data['name']
+        if message.is_from_me:
+            who_data = self._get_name(0)
+        else:
+            who_data = self._get_name(message.handle_id)
         style = who_data['style']
 
         text = message.text
         row_string = f'{" ":16s}<tr>\n' \
                      f'{" ":18s}<td class="reply_name" style="color: {who_data["name_color"]};"> ' \
                      f'{who_data["name"]}: </td>\n' \
                      f'{" ":18s}<td class="reply_text_thread">\n' \
@@ -170,22 +237,30 @@
             for message in message_list:
                 message_count = message_count + 1
 
                 today = message.date[:10]
                 if today != previous_day:
                     previous_day = today
 
+                    message_date = datetime(int(message.date[0:4]), int(message.date[5:7]), int(message.date[8:10]),
+                                            int(message.date[11:13]), int(message.date[14:16]),
+                                            int(message.date[17:19]))
+
+                    if self._file_start_date is None:
+                        self._file_start_date = message_date
+                    self._file_end_date = message_date
+
                     # If it's a new day, end the table, and start a new one
-                    self._print_and_save(f'{" ":2s}</table>\n\n{" ":2s}<table class="main_table">\n', table_array)
+                    self._print_and_save(f'{" ":2s}</table>\n\n', table_array, new_day=True)
+                    self._print_and_save(f'{" ":2s}<table class="main_table">\n', table_array)
 
-                    self._day = datetime(int(message.date[0:4]), int(message.date[5:7]), int(message.date[8:10]),
-                                         int(message.date[11:13]), int(message.date[14:16]),
-                                         int(message.date[17:19])).strftime('%a')
+                    self._day = message_date.strftime('%a')
+                self._last_row_had_conversion = False
                 self._print_and_save(self._generate_row(message), table_array)
-                if message.attachments:
+                if self._last_row_had_conversion:
                     bar()
                 else:
                     bar(skipped=True)
 
         self._print_and_save(f'{" ":2s}</table>\n', table_array)
         return ''.join(table_array)
 
@@ -225,15 +300,18 @@
                 self._name_map[handle_id] = {'name': handle_id, 'background_color': background_color,
                                              'name_color': name_color, 'style': 'them'}
 
         return self._name_map[handle_id]
 
     def _generate_row(self, message: Message) -> str:
         # Specify if the message is from me, or the other person
-        who_data = self._get_name(message.handle_id)
+        if message.is_from_me:
+            who_data = self._get_name(0)
+        else:
+            who_data = self._get_name(message.handle_id)
         who = who_data['name']
         style = who_data['style']
 
         # Check to see if we want the media box floating or fixed
         floating_option = self._database.config['DISPLAY'].get('popup location', fallback='floating')
         floating = floating_option == 'floating'
 
@@ -252,32 +330,40 @@
                     print_thread.append(i)
                 thread_table = self._generate_thread_table(print_thread, style)
 
         # Generate the attachment string
         attachments_string = ""
         if message.attachments:
             for attachment_key in message.attachments:
+                # If the attachment listed does not exist, then just list is as missing and continue to the next one
                 if attachment_key not in self._attachment_list.attachment_list:
                     attachments_string = f'{attachments_string} <span class="missing"> Attachment missing </span> '
                     continue
 
                 attachment = self._attachment_list.attachment_list[attachment_key]
-                attachment_string = ""
+                # If the attachment exists, but we have it marked to skip, skip it
                 if attachment.skip:
                     continue
+
+                # If the attachment exists, but is marked as missing, list it as missing and continue
                 if attachment.missing:
-                    attachment_string = f'{attachments_string} <span class="missing"> Attachment missing </span> '
+                    attachments_string = f'{attachments_string} <span class="missing"> Attachment missing </span> '
                     continue
+
+                # If we should copy the attachment, copy it or convert it
                 if attachment.copy:
                     if attachment.conversion_type == 'HEIC':
                         attachment.convert_heic_image(attachment.original_path, attachment.destination_path)
+                        self._last_row_had_conversion = True
                     elif attachment.conversion_type == 'Audio' or attachment.conversion_type == 'Video':
                         attachment.convert_audio_video(attachment.original_path, attachment.destination_path)
+                        self._last_row_had_conversion = True
                     else:
                         attachment.copy_attachment()
+                        self._last_row_had_conversion = True
 
                 if floating:
                     box_name = f'PopUp{attachment.rowid}'
                     image_box = f'<div class="imageBox" id="PopUp{attachment.rowid}">  <img src="" /> </div>'
                 else:
                     box_name = 'picbox'
                     image_box = ''
@@ -477,23 +563,23 @@
     padding: 15px;
     border-spacing: 40px;
 ''' + ''' }
 
 .edits_me {''' + f'''
     display: none;
     font-size: 70%;
-    font-style: italics;
+    font-style: italic;
     text-align: right;
     border-radius: 30px;
 ''' + ''' }  
 
 .edits_them {''' + f'''
     display: none;
     font-size: 70%;
-    font-style: italics;
+    font-style: italic;
     text-align: left;
     border-radius: 30px;
 ''' + ''' }    
 
 .infocell {''' + f'''
     margin-right: 0px;
     margin-left: auto;
@@ -608,14 +694,23 @@
     ''' + f'{popup_location}: 2%;' \
           '''
     background: Blue;
     transition: all .5s ease;
 
 ''' + ''' }
 
+.next_file {
+    text-align: center;
+    font-size: 150%;
+}
+
+#file_summary {
+    font-style: italic;
+}
+
     </style>'''
         script = '''  <script>
     
     function ToggleDisplay(id) {
       if (document.getElementById(id).style.display == "none") {
           document.getElementById(id).style.display = "inline";
       }
```

### Comparing `imessagedb-1.3.4/src/imessagedb/message.py` & `imessagedb-1.4.0/src/imessagedb/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 
     text = encoded.split(b'NSNumber')[0]
     text = text.split(b'NSString')[1]
     text = text.split(b'NSDictionary')[0]
     text = text[6:-12]
     if b'\x01' in text:
         text = text.split(b'\x01')[1]
+    if b'\x02' in text:
+        text = text.split(b'\x02')[1]
     if b'\x00' in text:
         text = text.split(b'\x00')[1]
     if b'\x86' in text:
         text = text.split(b'\x86')[0]
     return text.decode('utf-8', errors='replace')
```

### Comparing `imessagedb-1.3.4/src/imessagedb/messages.py` & `imessagedb-1.4.0/src/imessagedb/messages.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,27 +99,25 @@
                 message_count = message_count + 1
 
                 attachment_list = None
                 if not skip_attachment:
                     if rowid in self._database.attachment_list.message_join:
                         attachment_list = self._database.attachment_list.message_join[rowid]
 
-                skipped = True
-
                 new_message = Message(self._database, rowid, guid, date, is_from_me, handle_id, attributed_body,
                                       message_summary_info, text, reply_to_guid, thread_originator_guid,
                                       thread_originator_part, chat_id, attachment_list)
                 self._guids[guid] = new_message
                 self._message_list[rowid] = new_message
 
                 # Manage the thread
                 if thread_originator_guid:
                     self._guids[thread_originator_guid].thread[rowid] = new_message
 
-                bar(skipped=skipped)
+                bar()
                 i = self._database.connection.fetchone()
 
         self._sorted_message_list = sorted(self._message_list.values(), key=lambda x: x.date)
 
     @property
     def message_list(self) -> list:
         """ Returns a list of messages sorted by the date of the message"""
```

### Comparing `imessagedb-1.3.4/src/imessagedb/text.py` & `imessagedb-1.4.0/src/imessagedb/text.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.3.4/src/imessagedb/utils.py` & `imessagedb-1.4.0/src/imessagedb/utils.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.3.4/PKG-INFO` & `imessagedb-1.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: imessagedb
-Version: 1.3.4
+Version: 1.4.0
 Summary: Reads and displays the Apple iMessage database
 License: MIT
 Author: xev
 Author-email: git@schore.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: alive-progress (>=3.1.2,<4.0.0)
 Requires-Dist: configparser (>=5.3.0,<6.0.0)
 Requires-Dist: ffmpeg-python (>=0.2.0,<0.3.0)
 Requires-Dist: heic2png (>=1.0.0,<2.0.0)
+Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: termcolor (>=2.3.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # imessagedb
 
 Reads and displays the Apple iMessage database
 
@@ -85,18 +86,18 @@
                         The type of output
   -i, --inline          Show the attachments inline
   -f, --force           Force a copy of the attachments
   --no_copy             Don't copy the attachments
   --no_attachments      Don't process attachments at all
   -v, --verbose         Turn on additional output
   --start_time START_TIME
-                        The start time of the messages in YYYY-MM-DD HH:MM:SS
-                        format
-  --end_time END_TIME   The end time of the messages in YYYY-MM-DD HH:MM:SS
-                        format
+                        The start time of the messages
+  --end_time END_TIME   The end time of the messages
+  --split_output SPLIT_OUTPUT
+                        Split the html output into files with this many messages per file
   --version             Show the version number and exit
   --get_handles         Display the list of handles in the database and exit
   --get_chats           Display the list of chats in the database and exit
 ```
 
 #### Command line options
 
@@ -124,19 +125,21 @@
 
 **-m ME, --me ME** The name to use to refer to you in the output. If this option is not 
 provided it will default to `Me`.
 
 **-t {text,html}, --output_type {text,html}** The type of output, either *text* or *html*. 
 If this option is not provided it will default to `html`.
 
-
 **--start_time START_TIME** <br>
 **--end_time END_TIME** By default, the program will process all messages. If you want
 to restrict that to particular timeframe, you can specify the `--start-time` and/or `--end_time`
-options in the  YYYY-MM-DD HH:MM:SS  format
+options
+
+**--split_output SPLIT_OUTPUT** Split the html output into files with this many messages 
+per file
 
 **-i, --inline**   Show the attachments inline. By default, the attachments will show as links
 that you can hover over and it will pop up the attachment. With this option, it will put them
 inline, which will make your output much busier and take a lot more memory in your browser.
 
 **-f, --force**  Force a copy of the attachments. By default, if the attachment already exists
 in the destination directory, it will not re-copy the file, but this will force it to re-copy it.
@@ -146,15 +149,14 @@
 
 **--no_attachments**      Do not show the attachments at all
 
 **-v, --verbose**         Turn on additional output
 
 **--version**  Shows the version number and exits
 
-
 **--get_handles** Display the list of handles in the database and exit
 
 **--get_chats** Display the list of chats in the database and exit
 ### Configuration File
 
 The configuration file is in configparser format. Here is the template that is created
 by default:
@@ -194,14 +196,18 @@
 
 [DISPLAY]
 
 # Output type, either html or text
 
 output_type = html
 
+# Number of messages in each html file. If this is 0 or not specified, it will be one large file.
+
+output split = 1000
+
 # Inline attachments mean that the images are in the HTML instead of loaded when hovered over
 
 inline attachments = False
 
 # Popup location is where the attachment popup window shows up, and is either 'upper right', 'upper left' or 'floating'
 
 popup location = upper right
```

