# Comparing `tmp/jsonfmt-0.2.1.tar.gz` & `tmp/jsonfmt-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonfmt-0.2.1.tar", last modified: Fri May 26 02:33:49 2023, max compression
+gzip compressed data, was "jsonfmt-0.2.2.tar", last modified: Fri May 26 06:14:42 2023, max compression
```

## Comparing `jsonfmt-0.2.1.tar` & `jsonfmt-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:33:49.118660 jsonfmt-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-26 02:33:30.000000 jsonfmt-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-05-26 02:33:49.118660 jsonfmt-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-05-26 02:33:30.000000 jsonfmt-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:33:49.118660 jsonfmt-0.2.1/jsonfmt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-05-26 02:33:49.000000 jsonfmt-0.2.1/jsonfmt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-26 02:33:49.000000 jsonfmt-0.2.1/jsonfmt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 02:33:49.000000 jsonfmt-0.2.1/jsonfmt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-26 02:33:49.000000 jsonfmt-0.2.1/jsonfmt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-26 02:33:49.000000 jsonfmt-0.2.1/jsonfmt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-26 02:33:49.000000 jsonfmt-0.2.1/jsonfmt.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     7550 2023-05-26 02:33:30.000000 jsonfmt-0.2.1/jsonfmt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-26 02:33:30.000000 jsonfmt-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 02:33:49.118660 jsonfmt-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:33:49.118660 jsonfmt-0.2.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)    11226 2023-05-26 02:33:30.000000 jsonfmt-0.2.1/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:14:42.152842 jsonfmt-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-26 06:14:24.000000 jsonfmt-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-05-26 06:14:42.152842 jsonfmt-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-05-26 06:14:24.000000 jsonfmt-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:14:42.152842 jsonfmt-0.2.2/jsonfmt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-05-26 06:14:42.000000 jsonfmt-0.2.2/jsonfmt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-26 06:14:42.000000 jsonfmt-0.2.2/jsonfmt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 06:14:42.000000 jsonfmt-0.2.2/jsonfmt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-26 06:14:42.000000 jsonfmt-0.2.2/jsonfmt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-26 06:14:42.000000 jsonfmt-0.2.2/jsonfmt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-26 06:14:42.000000 jsonfmt-0.2.2/jsonfmt.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7955 2023-05-26 06:14:24.000000 jsonfmt-0.2.2/jsonfmt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-26 06:14:24.000000 jsonfmt-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 06:14:42.152842 jsonfmt-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:14:42.152842 jsonfmt-0.2.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    11398 2023-05-26 06:14:24.000000 jsonfmt-0.2.2/test/test.py
```

### Comparing `jsonfmt-0.2.1/LICENSE` & `jsonfmt-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonfmt-0.2.1/PKG-INFO` & `jsonfmt-0.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonfmt
-Version: 0.2.1
+Version: 0.2.2
 Summary: A simple tool for formatting JSON object.
 Author-email: Seamile <lanhuermao@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/seamile/jsonfmt
 Project-URL: repository, https://github.com/seamile/jsonfmt
 Project-URL: documentation, https://seamile.github.io/jsonfmt/
 Keywords: json,formatter,pretty-print,highlight,jsonpath
@@ -60,28 +60,30 @@
 ```
 
 - Positional arguments:
 
     - `files`: the files that will be processed
 
 - Options:
-  - `-h, --help`: show this help message and exit
-  - `-c`: compact the json object to a single line
-  - `-C`: copy the result to clipboard
-  - `-e`: escape non-ASCII characters
-  - `-f {json,toml,yaml}`: the format to output (default: json)
-  - `-i INDENT`: number of spaces for indentation (default: 2)
-  - `-O`: overwrite the formated text to original file
-  - `-p JSONPATH`: output part of the object via jsonpath
-  - `-v`: show the version
+
+    - `-h, --help`: show this help message and exit
+    - `-c`: compact the json object to a single line
+    - `-C`: copy the result to clipboard
+    - `-e`: escape non-ASCII characters
+    - `-f {json,toml,yaml}`: the format to output (default: json)
+    - `-i INDENT`: number of spaces for indentation (default: 2)
+    - `-O`: overwrite the formated text to original file
+    - `-p JSONPATH`: output part of the object via jsonpath
+    - `-v`: show the version
 
 
 ## Example
 
 There are some test data in folder `test`:
+
 ```
 test/
 |- example.json
 |- example.toml
 |- example.yaml
 ```
 
@@ -91,14 +93,15 @@
 
     ```shell
     # format the json with 4-space indentaion
     $ jsonfmt -i 4 test/example.json
     ```
 
     *Output:*
+
     ```json
     {
         "actions": [
             {
                 "calorie": 294.9,
                 "date": "2021-03-02",
                 "name": "eat"
@@ -134,14 +137,15 @@
         "pen",
         "phone"
     ]
 }' | jsonfmt -c
 ```
 
 *Output:*
+
 ```json
 {"age":21,"items":["pen","phone"],"name":"alex"}
 ```
 
 ### 3. Use jsonpath to match part of the object.
 
 **jsonfmt** uses a simplified jsonpath syntax.
@@ -151,14 +155,15 @@
 - You can use keys to match dictionaries and indexes to match lists, and use `/` to separate different levels.
 
     ```shell
     $ jsonfmt -p 'actions/0' test/example.json
     ```
 
     *Output:*
+
     ```json
     {
         "calorie": 294.9,
         "date": "2021-03-02",
         "name": "eat"
     }
     ```
@@ -166,28 +171,30 @@
 - If you want to match all items in a list, just use `*` to match.
 
     ```shell
     $ jsonfmt -p 'actions/*/name' test/example.json
     ```
 
     *Output:*
+
     ```json
     [
         "eat",
         "sport"
     ]
     ```
 
 ### 4. Format JSON to TOML or YAML.
 
 ```shell
 $ jsonfmt test/example.json -f toml
 ```
 
 *Output:*
+
 ```toml
 age = 23
 gender = "纯爷们"
 money = 3.1415926
 name = "Bob"
 [[actions]]
 calorie = 294.9
@@ -198,17 +205,16 @@
 calorie = -375
 date = "2023-04-27"
 name = "sport"
 ```
 
 ### 5. Convert between JSON, TOML and YAML formats.
 
-<div style="color: red"><strong>Note this!</strong></div>
-The `null` value is invalid in TOML.
-Therefore, any null values in JSON or YAML will be removed when converting to TOML.
+<div style="color: orange"><strong>Note this:</strong></div>
+The `null` value is invalid in TOML. Therefore, any null values in JSON or YAML will be removed when converting to TOML.
 
 ```shell
 # json to yaml
 $ jsonfmt test/example.json -f yaml
 
 # yaml to toml
 $ jsonfmt test/example.yaml -f toml
@@ -222,17 +228,20 @@
 ```shell
 $ jsonfmt -C test/example.json
 
 # Output
 jsonfmt: result copied to clipboard.
 ```
 
-You can then use <kbd>ctrl</kbd>+<kbd>v</kbd> or <kbd>cmd</kbd>+<kbd>v</kbd> to paste the result anywhere on your computer.
+Once you've done the above, you can then use <kbd>ctrl</kbd>+<kbd>v</kbd> or <kbd>cmd</kbd>+<kbd>v</kbd> to paste the result anywhere on your computer.
+
+<div style="color: orange"><strong>Note these:</strong></div>
 
-But when you process multiple files, only the last result is kept in the clipboard.
+- When you specify the `-C` option, any output destination other than the clipboard will be ignored.
+- When you process multiple files, only the last result will be preserved in the clipboard.
 
 ### 7. Other usages
 
 - use the `-O` parameter to overwrite the file with the result.
 
 ```shell
 $ jsonfmt -O test/example.json
```

### Comparing `jsonfmt-0.2.1/README.md` & `jsonfmt-0.2.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -32,28 +32,30 @@
 ```
 
 - Positional arguments:
 
     - `files`: the files that will be processed
 
 - Options:
-  - `-h, --help`: show this help message and exit
-  - `-c`: compact the json object to a single line
-  - `-C`: copy the result to clipboard
-  - `-e`: escape non-ASCII characters
-  - `-f {json,toml,yaml}`: the format to output (default: json)
-  - `-i INDENT`: number of spaces for indentation (default: 2)
-  - `-O`: overwrite the formated text to original file
-  - `-p JSONPATH`: output part of the object via jsonpath
-  - `-v`: show the version
+
+    - `-h, --help`: show this help message and exit
+    - `-c`: compact the json object to a single line
+    - `-C`: copy the result to clipboard
+    - `-e`: escape non-ASCII characters
+    - `-f {json,toml,yaml}`: the format to output (default: json)
+    - `-i INDENT`: number of spaces for indentation (default: 2)
+    - `-O`: overwrite the formated text to original file
+    - `-p JSONPATH`: output part of the object via jsonpath
+    - `-v`: show the version
 
 
 ## Example
 
 There are some test data in folder `test`:
+
 ```
 test/
 |- example.json
 |- example.toml
 |- example.yaml
 ```
 
@@ -63,14 +65,15 @@
 
     ```shell
     # format the json with 4-space indentaion
     $ jsonfmt -i 4 test/example.json
     ```
 
     *Output:*
+
     ```json
     {
         "actions": [
             {
                 "calorie": 294.9,
                 "date": "2021-03-02",
                 "name": "eat"
@@ -106,14 +109,15 @@
         "pen",
         "phone"
     ]
 }' | jsonfmt -c
 ```
 
 *Output:*
+
 ```json
 {"age":21,"items":["pen","phone"],"name":"alex"}
 ```
 
 ### 3. Use jsonpath to match part of the object.
 
 **jsonfmt** uses a simplified jsonpath syntax.
@@ -123,14 +127,15 @@
 - You can use keys to match dictionaries and indexes to match lists, and use `/` to separate different levels.
 
     ```shell
     $ jsonfmt -p 'actions/0' test/example.json
     ```
 
     *Output:*
+
     ```json
     {
         "calorie": 294.9,
         "date": "2021-03-02",
         "name": "eat"
     }
     ```
@@ -138,28 +143,30 @@
 - If you want to match all items in a list, just use `*` to match.
 
     ```shell
     $ jsonfmt -p 'actions/*/name' test/example.json
     ```
 
     *Output:*
+
     ```json
     [
         "eat",
         "sport"
     ]
     ```
 
 ### 4. Format JSON to TOML or YAML.
 
 ```shell
 $ jsonfmt test/example.json -f toml
 ```
 
 *Output:*
+
 ```toml
 age = 23
 gender = "纯爷们"
 money = 3.1415926
 name = "Bob"
 [[actions]]
 calorie = 294.9
@@ -170,17 +177,16 @@
 calorie = -375
 date = "2023-04-27"
 name = "sport"
 ```
 
 ### 5. Convert between JSON, TOML and YAML formats.
 
-<div style="color: red"><strong>Note this!</strong></div>
-The `null` value is invalid in TOML.
-Therefore, any null values in JSON or YAML will be removed when converting to TOML.
+<div style="color: orange"><strong>Note this:</strong></div>
+The `null` value is invalid in TOML. Therefore, any null values in JSON or YAML will be removed when converting to TOML.
 
 ```shell
 # json to yaml
 $ jsonfmt test/example.json -f yaml
 
 # yaml to toml
 $ jsonfmt test/example.yaml -f toml
@@ -194,17 +200,20 @@
 ```shell
 $ jsonfmt -C test/example.json
 
 # Output
 jsonfmt: result copied to clipboard.
 ```
 
-You can then use <kbd>ctrl</kbd>+<kbd>v</kbd> or <kbd>cmd</kbd>+<kbd>v</kbd> to paste the result anywhere on your computer.
+Once you've done the above, you can then use <kbd>ctrl</kbd>+<kbd>v</kbd> or <kbd>cmd</kbd>+<kbd>v</kbd> to paste the result anywhere on your computer.
+
+<div style="color: orange"><strong>Note these:</strong></div>
 
-But when you process multiple files, only the last result is kept in the clipboard.
+- When you specify the `-C` option, any output destination other than the clipboard will be ignored.
+- When you process multiple files, only the last result will be preserved in the clipboard.
 
 ### 7. Other usages
 
 - use the `-O` parameter to overwrite the file with the result.
 
 ```shell
 $ jsonfmt -O test/example.json
```

### Comparing `jsonfmt-0.2.1/jsonfmt.egg-info/PKG-INFO` & `jsonfmt-0.2.2/jsonfmt.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonfmt
-Version: 0.2.1
+Version: 0.2.2
 Summary: A simple tool for formatting JSON object.
 Author-email: Seamile <lanhuermao@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/seamile/jsonfmt
 Project-URL: repository, https://github.com/seamile/jsonfmt
 Project-URL: documentation, https://seamile.github.io/jsonfmt/
 Keywords: json,formatter,pretty-print,highlight,jsonpath
@@ -60,28 +60,30 @@
 ```
 
 - Positional arguments:
 
     - `files`: the files that will be processed
 
 - Options:
-  - `-h, --help`: show this help message and exit
-  - `-c`: compact the json object to a single line
-  - `-C`: copy the result to clipboard
-  - `-e`: escape non-ASCII characters
-  - `-f {json,toml,yaml}`: the format to output (default: json)
-  - `-i INDENT`: number of spaces for indentation (default: 2)
-  - `-O`: overwrite the formated text to original file
-  - `-p JSONPATH`: output part of the object via jsonpath
-  - `-v`: show the version
+
+    - `-h, --help`: show this help message and exit
+    - `-c`: compact the json object to a single line
+    - `-C`: copy the result to clipboard
+    - `-e`: escape non-ASCII characters
+    - `-f {json,toml,yaml}`: the format to output (default: json)
+    - `-i INDENT`: number of spaces for indentation (default: 2)
+    - `-O`: overwrite the formated text to original file
+    - `-p JSONPATH`: output part of the object via jsonpath
+    - `-v`: show the version
 
 
 ## Example
 
 There are some test data in folder `test`:
+
 ```
 test/
 |- example.json
 |- example.toml
 |- example.yaml
 ```
 
@@ -91,14 +93,15 @@
 
     ```shell
     # format the json with 4-space indentaion
     $ jsonfmt -i 4 test/example.json
     ```
 
     *Output:*
+
     ```json
     {
         "actions": [
             {
                 "calorie": 294.9,
                 "date": "2021-03-02",
                 "name": "eat"
@@ -134,14 +137,15 @@
         "pen",
         "phone"
     ]
 }' | jsonfmt -c
 ```
 
 *Output:*
+
 ```json
 {"age":21,"items":["pen","phone"],"name":"alex"}
 ```
 
 ### 3. Use jsonpath to match part of the object.
 
 **jsonfmt** uses a simplified jsonpath syntax.
@@ -151,14 +155,15 @@
 - You can use keys to match dictionaries and indexes to match lists, and use `/` to separate different levels.
 
     ```shell
     $ jsonfmt -p 'actions/0' test/example.json
     ```
 
     *Output:*
+
     ```json
     {
         "calorie": 294.9,
         "date": "2021-03-02",
         "name": "eat"
     }
     ```
@@ -166,28 +171,30 @@
 - If you want to match all items in a list, just use `*` to match.
 
     ```shell
     $ jsonfmt -p 'actions/*/name' test/example.json
     ```
 
     *Output:*
+
     ```json
     [
         "eat",
         "sport"
     ]
     ```
 
 ### 4. Format JSON to TOML or YAML.
 
 ```shell
 $ jsonfmt test/example.json -f toml
 ```
 
 *Output:*
+
 ```toml
 age = 23
 gender = "纯爷们"
 money = 3.1415926
 name = "Bob"
 [[actions]]
 calorie = 294.9
@@ -198,17 +205,16 @@
 calorie = -375
 date = "2023-04-27"
 name = "sport"
 ```
 
 ### 5. Convert between JSON, TOML and YAML formats.
 
-<div style="color: red"><strong>Note this!</strong></div>
-The `null` value is invalid in TOML.
-Therefore, any null values in JSON or YAML will be removed when converting to TOML.
+<div style="color: orange"><strong>Note this:</strong></div>
+The `null` value is invalid in TOML. Therefore, any null values in JSON or YAML will be removed when converting to TOML.
 
 ```shell
 # json to yaml
 $ jsonfmt test/example.json -f yaml
 
 # yaml to toml
 $ jsonfmt test/example.yaml -f toml
@@ -222,17 +228,20 @@
 ```shell
 $ jsonfmt -C test/example.json
 
 # Output
 jsonfmt: result copied to clipboard.
 ```
 
-You can then use <kbd>ctrl</kbd>+<kbd>v</kbd> or <kbd>cmd</kbd>+<kbd>v</kbd> to paste the result anywhere on your computer.
+Once you've done the above, you can then use <kbd>ctrl</kbd>+<kbd>v</kbd> or <kbd>cmd</kbd>+<kbd>v</kbd> to paste the result anywhere on your computer.
+
+<div style="color: orange"><strong>Note these:</strong></div>
 
-But when you process multiple files, only the last result is kept in the clipboard.
+- When you specify the `-C` option, any output destination other than the clipboard will be ignored.
+- When you process multiple files, only the last result will be preserved in the clipboard.
 
 ### 7. Other usages
 
 - use the `-O` parameter to overwrite the file with the result.
 
 ```shell
 $ jsonfmt -O test/example.json
```

### Comparing `jsonfmt-0.2.1/jsonfmt.py` & `jsonfmt-0.2.2/jsonfmt.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,33 +9,39 @@
 from functools import partial
 from pygments import highlight
 from pygments.formatters import TerminalFormatter
 from pygments.lexers import JsonLexer, TOMLLexer, YamlLexer
 from sys import stdin, stdout, stderr, exit
 from typing import Any, List, IO, Optional, Sequence, Union
 
-__version__ = '0.2.1'
+__version__ = '0.2.2'
 
 
 def print_inf(msg: str):
-    print(f'\033[1;94mjsonfmt:\033[0m \033[0;94m{msg}\033[0m')
+    print(f'\033[1;94mjsonfmt:\033[0m \033[0;94m{msg}\033[0m', file=stdout)
 
 
 def print_err(msg: str):
     print(f'\033[1;91mjsonfmt:\033[0m \033[0;91m{msg}\033[0m', file=stderr)
 
 
 class JSONPathError(Exception):
     pass
 
 
 class ParseError(Exception):
     pass
 
 
+def is_clipboard_available() -> bool:
+    copy_fn, paste_fn = pyperclip.determine_clipboard()
+    return copy_fn.__class__.__name__ != 'ClipboardUnavailable' \
+        and paste_fn.__class__.__name__ != 'ClipboardUnavailable'
+
+
 def parse_jsonpath(jsonpath: str) -> List[Union[str, int]]:
     '''parse the jsonpath into a list of pathname components'''
     if jsonpath := jsonpath.strip().strip('/'):
         components = jsonpath.split('/')
         for i, component in enumerate(components):
             if component.isdecimal():
                 components[i] = int(component)  # type: ignore
@@ -171,20 +177,25 @@
                         version=__version__, help="show the version")
     return parser.parse_args(args)
 
 
 def main():
     args = parse_cmdline_args()
 
+    # check if the clipboard is available
+    cp2clip = args.cp2clip and is_clipboard_available()
+    if args.cp2clip and not cp2clip:
+        print_err('clipboard unavailable')
+
     # match the specified output function
     fn_output = {
-        'json': partial(output_json, cp2clip=args.cp2clip, compact=args.compact,
+        'json': partial(output_json, cp2clip=cp2clip, compact=args.compact,
                         escape=args.escape, indent=args.indent),
-        'yaml': partial(output_yaml, cp2clip=args.cp2clip, escape=args.escape, indent=args.indent),
-        'toml': partial(output_toml, cp2clip=args.cp2clip),
+        'yaml': partial(output_yaml, cp2clip=cp2clip, escape=args.escape, indent=args.indent),
+        'toml': partial(output_toml, cp2clip=cp2clip),
     }[args.format]
 
     if args.files:
         for file in args.files:
             try:
                 # read from file
                 with open(file, 'r+') as input_fp:
```

### Comparing `jsonfmt-0.2.1/pyproject.toml` & `jsonfmt-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jsonfmt-0.2.1/test/test.py` & `jsonfmt-0.2.2/test/test.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,46 +38,33 @@
         'yaml': partial(highlight,
                         lexer=YamlLexer(),
                         formatter=TerminalFormatter()),
     }[format]
     return fn(text)
 
 
-class FakeStdIn(StringIO):
-    name = '<stdin>'
-
+class FakeStdStream(StringIO):
     def isatty(self):
         return True
 
-    def fileno(self):
-        return 0
-
-
-class FakeStdOut(StringIO):
-    name = '<stdout>'
-
-    def isatty(self):
-        return True
-
-    def fileno(self):
-        return 1
-
     def read(self):
         self.seek(0)
         return super().read()
 
 
-class FakeStdErr(StringIO):
-    name = '<stderr>'
+class FakeStdIn(FakeStdStream):
+    name = '<stdin>'
 
-    def isatty(self):
-        return True
 
-    def fileno(self):
-        return 2
+class FakeStdOut(FakeStdStream):
+    name = '<stdout>'
+
+
+class FakeStdErr(FakeStdStream):
+    name = '<stderr>'
 
 
 class JSONFormatToolTestCase(unittest.TestCase):
     def setUp(self):
         self.py_obj = json.loads(JSON_TEXT)
 
     def test_parse_jsonpath(self):
@@ -163,15 +150,15 @@
         colored_outputs = [color(o, 'toml') for o in expected_outputs]
         jsonfmt.output_toml(py_obj, jsonfmt.stdout, cp2clip=False)
         self.assertIn(jsonfmt.stdout.read(), colored_outputs)
 
         # test SystemExit when using non-mapping
         with self.assertRaises(SystemExit) as raise_ctx:
             jsonfmt.output_toml(['foo', 'bar'], jsonfmt.stdout, cp2clip=False)
-            self.assertEqual(raise_ctx.exception.code, 3)
+        self.assertEqual(raise_ctx.exception.code, 3)
 
     @patch('jsonfmt.stdout', FakeStdOut())
     def test_output_yaml(self):
         py_obj = {"name": "约翰", "age": 30}
 
         # test output yaml to file (temp file)
         expected_output = 'age: 30\nname: "\\u7EA6\\u7FF0"\n'
@@ -243,22 +230,22 @@
         self.assertEqual(jsonfmt.stdout.read(), expected_output)
 
     @patch.multiple(sys, argv=['jsonfmt', 'foo.bar', __file__])
     @patch.multiple(jsonfmt, stderr=FakeStdErr())
     def test_main_invalid_file(self):
         with self.assertRaises(SystemExit) as raise_ctx:
             jsonfmt.main()
-            self.assertEqual(raise_ctx.exception.code, 1)
+        self.assertEqual(raise_ctx.exception.code, 1)
 
     @patch.multiple(sys, argv=['jsonfmt', '-f', 'json'])
     @patch.multiple(jsonfmt, stdin=FakeStdIn(']a, b, c]'), stderr=FakeStdErr())
     def test_main_invalid_input(self):
         with self.assertRaises(SystemExit) as raise_ctx:
             jsonfmt.main()
-            self.assertEqual(raise_ctx.exception.code, 2)
+        self.assertEqual(raise_ctx.exception.code, 2)
 
     @patch.multiple(sys, argv=['jsonfmt', '-f', 'toml'])
     @patch.multiple(jsonfmt, stdin=FakeStdIn(JSON_TEXT), stdout=FakeStdOut())
     def test_json_to_toml(self):
         colored_output = color(TOML_TEXT, 'toml')
         jsonfmt.main()
         self.assertEqual(jsonfmt.stdout.read(), colored_output)
@@ -284,29 +271,34 @@
             with open(f'{BASE_DIR}/test/example.toml') as toml_fp:
                 new_content = toml_fp.read()
             self.assertEqual(new_content, JSON_TEXT)
         finally:
             with open(f'{BASE_DIR}/test/example.toml', 'w') as toml_fp:
                 toml_fp.write(TOML_TEXT)
 
+    @patch.multiple(jsonfmt, stdout=FakeStdOut(), stderr=FakeStdErr())
     def test_copy_to_clipboard(self):
-        try:
+        if jsonfmt.is_clipboard_available():
             with patch("sys.argv", ['jsonfmt', f'{BASE_DIR}/test/example.toml', '-Cc']):
                 jsonfmt.main()
                 copied_text = pyperclip.paste().strip()
                 self.assertEqual(copied_text, JSON_TEXT.strip())
 
             with patch("sys.argv", ['jsonfmt', f'{BASE_DIR}/test/example.json', '-Cf', 'toml']):
                 jsonfmt.main()
                 copied_text = pyperclip.paste().strip()
                 self.assertEqual(copied_text, TOML_TEXT.strip())
 
             with patch("sys.argv", ['jsonfmt', f'{BASE_DIR}/test/example.json', '-Cf', 'yaml']):
                 jsonfmt.main()
                 copied_text = pyperclip.paste().strip()
                 self.assertEqual(copied_text, YAML_TEXT.strip())
-        except pyperclip.PyperclipException as e:
-            jsonfmt.print_err(e)  # type: ignore
+        else:
+            errmsg = '\033[1;91mjsonfmt:\033[0m \033[0;91mclipboard unavailable\033[0m\n'
+            with patch.multiple(sys, argv=['jsonfmt', '-C']), \
+                    patch.multiple(jsonfmt, stdin=FakeStdIn('["a", "b"]')):
+                jsonfmt.main()
+                self.assertEqual(jsonfmt.stderr.read(), errmsg)
 
 
 if __name__ == '__main__':
     unittest.main()
```

