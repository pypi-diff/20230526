# Comparing `tmp/jsonfmt-0.2.0.tar.gz` & `tmp/jsonfmt-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonfmt-0.2.0.tar", last modified: Wed May 24 03:53:33 2023, max compression
+gzip compressed data, was "jsonfmt-0.2.1.tar", last modified: Fri May 26 02:33:49 2023, max compression
```

## Comparing `jsonfmt-0.2.0.tar` & `jsonfmt-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:53:33.813517 jsonfmt-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-24 03:53:18.000000 jsonfmt-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-05-24 03:53:33.813517 jsonfmt-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-05-24 03:53:18.000000 jsonfmt-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:53:33.813517 jsonfmt-0.2.0/jsonfmt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-05-24 03:53:33.000000 jsonfmt-0.2.0/jsonfmt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-24 03:53:33.000000 jsonfmt-0.2.0/jsonfmt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 03:53:33.000000 jsonfmt-0.2.0/jsonfmt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-24 03:53:33.000000 jsonfmt-0.2.0/jsonfmt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-24 03:53:33.000000 jsonfmt-0.2.0/jsonfmt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-24 03:53:33.000000 jsonfmt-0.2.0/jsonfmt.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     6926 2023-05-24 03:53:18.000000 jsonfmt-0.2.0/jsonfmt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-24 03:53:18.000000 jsonfmt-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 03:53:33.813517 jsonfmt-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:53:33.813517 jsonfmt-0.2.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-05-24 03:53:18.000000 jsonfmt-0.2.0/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:33:49.118660 jsonfmt-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-26 02:33:30.000000 jsonfmt-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-05-26 02:33:49.118660 jsonfmt-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-05-26 02:33:30.000000 jsonfmt-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:33:49.118660 jsonfmt-0.2.1/jsonfmt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-05-26 02:33:49.000000 jsonfmt-0.2.1/jsonfmt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-26 02:33:49.000000 jsonfmt-0.2.1/jsonfmt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 02:33:49.000000 jsonfmt-0.2.1/jsonfmt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-26 02:33:49.000000 jsonfmt-0.2.1/jsonfmt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-26 02:33:49.000000 jsonfmt-0.2.1/jsonfmt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-26 02:33:49.000000 jsonfmt-0.2.1/jsonfmt.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7550 2023-05-26 02:33:30.000000 jsonfmt-0.2.1/jsonfmt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-26 02:33:30.000000 jsonfmt-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 02:33:49.118660 jsonfmt-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:33:49.118660 jsonfmt-0.2.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    11226 2023-05-26 02:33:30.000000 jsonfmt-0.2.1/test/test.py
```

### Comparing `jsonfmt-0.2.0/LICENSE` & `jsonfmt-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonfmt-0.2.0/PKG-INFO` & `jsonfmt-0.2.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,77 +1,51 @@
-Metadata-Version: 2.1
-Name: jsonfmt
-Version: 0.2.0
-Summary: A simple tool for formatting JSON object.
-Author-email: Seamile <lanhuermao@gmail.com>
-License: MIT License
-Project-URL: homepage, https://github.com/seamile/jsonfmt
-Project-URL: repository, https://github.com/seamile/jsonfmt
-Project-URL: documentation, https://seamile.github.io/jsonfmt/
-Keywords: json,formatter,pretty-print,highlight,jsonpath
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: File Formats :: JSON
-Classifier: Topic :: Printing
-Classifier: Topic :: Utilities
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # JSON Formator
 
 [![Build Status](https://github.com/seamile/jsonfmt/actions/workflows/python-package.yml/badge.svg)](https://github.com/seamile/jsonfmt/actions)
 [![PyPI Version](https://img.shields.io/pypi/v/jsonfmt?color=blue&label=Version&logo=python&logoColor=white)](https://pypi.org/project/jsonfmt/)
 [![Installs](https://static.pepy.tech/personalized-badge/jsonfmt?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Installs)](https://pepy.tech/project/jsonfmt)
 [![Code Grade](https://app.codacy.com/project/badge/Grade/1e12e3cd8c8342bca68db4caf5b6a31d)](https://app.codacy.com/gh/seamile/jsonfmt/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 [![Test Coverage](https://app.codacy.com/project/badge/Coverage/1e12e3cd8c8342bca68db4caf5b6a31d)](https://app.codacy.com/gh/seamile/jsonfmt/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage)
 
 **jsonfmt** is a CLI tool for pretty printing or compressing JSON objects.
 
 It has the following features:
 
-- [Print JSON with **hightlight** and **pretty format** from files or stdin.](#1-pretty-print-json-object)
-- [Minimize JSON to a single line.](#2-minimize-the-json-object)
-- [Output part of a large JSON via jsonpath.](#3-use-jsonpath-to-match-part-of-the-object)
-- [Format JSON to TOML or YAML](#4-format-json-to-toml-or-yaml)
-- [Convert between other formats](#5-convert-between-json-toml-and-yaml-formats)
+1. [Print JSON with **hightlight** and **pretty format** from files or stdin.](#1-pretty-print-json-object)
+2. [Minimize JSON to a single line.](#2-minimize-the-json-object)
+3. [Output part of a large JSON via jsonpath.](#3-use-jsonpath-to-match-part-of-the-object)
+4. [Format JSON to TOML or YAML.](#4-format-json-to-toml-or-yaml)
+5. [Convert between other formats.](#5-convert-between-json-toml-and-yaml-formats)
+6. [Copy the result to clipboard.](#6-copy-the-result-to-clipboard)
 
 
 ## Install
 
 ```shell
 $ pip install jsonfmt
 ```
 
 
 ## Usage
 
 ```shell
-$ jsonfmt [Options] [Files ...]
+$ jsonfmt [options] [files ...]
 ```
 
 - Positional arguments:
 
     - `files`: the files that will be processed
 
 - Options:
   - `-h, --help`: show this help message and exit
   - `-c`: compact the json object to a single line
+  - `-C`: copy the result to clipboard
   - `-e`: escape non-ASCII characters
   - `-f {json,toml,yaml}`: the format to output (default: json)
-  - `-i INDENT`: number of spaces to use for indentation (default: 2)
+  - `-i INDENT`: number of spaces for indentation (default: 2)
   - `-O`: overwrite the formated text to original file
   - `-p JSONPATH`: output part of the object via jsonpath
   - `-v`: show the version
 
 
 ## Example
 
@@ -84,54 +58,62 @@
 ```
 
 ### 1. Pretty print JSON object.
 
 - read from file
 
     ```shell
-    $ jsonfmt test/example.json
+    # format the json with 4-space indentaion
+    $ jsonfmt -i 4 test/example.json
     ```
 
-    Output:
+    *Output:*
     ```json
     {
         "actions": [
             {
-            "calorie": 294.9,
-            "date": "2021-03-02",
-            "name": "eat"
+                "calorie": 294.9,
+                "date": "2021-03-02",
+                "name": "eat"
             },
             {
-            "calorie": -375,
-            "date": "2023-04-27",
-            "name": "sport"
+                "calorie": -375,
+                "date": "2023-04-27",
+                "name": "sport"
             }
         ],
         "age": 23,
         "gender": "纯爷们",
         "money": 3.1415926,
         "name": "Bob"
     }
     ```
 
 - read from stdin
 
     ```shell
-    $ cat test/example.json | jsonfmt
+    $ cat test/example.json | jsonfmt -i 4
     ```
 
-    Output: Ditto.
+    *Output*: Ditto.
 
 ### 2. Minimize the JSON object.
 
 ```shell
-$ echo '{ "name": "alex", "age": 21, "items": ["pen", "phone"] }' | jsonfmt -c
+$ echo '{
+    "name": "alex",
+    "age": 21,
+    "items": [
+        "pen",
+        "phone"
+    ]
+}' | jsonfmt -c
 ```
 
-Output:
+*Output:*
 ```json
 {"age":21,"items":["pen","phone"],"name":"alex"}
 ```
 
 ### 3. Use jsonpath to match part of the object.
 
 **jsonfmt** uses a simplified jsonpath syntax.
@@ -140,44 +122,44 @@
 
 - You can use keys to match dictionaries and indexes to match lists, and use `/` to separate different levels.
 
     ```shell
     $ jsonfmt -p 'actions/0' test/example.json
     ```
 
-    Output:
+    *Output:*
     ```json
     {
         "calorie": 294.9,
         "date": "2021-03-02",
         "name": "eat"
     }
     ```
 
 - If you want to match all items in a list, just use `*` to match.
 
     ```shell
     $ jsonfmt -p 'actions/*/name' test/example.json
     ```
 
-    Output:
+    *Output:*
     ```json
     [
         "eat",
         "sport"
     ]
     ```
 
 ### 4. Format JSON to TOML or YAML.
 
 ```shell
-$ jsonfmt -f toml test/example.json
+$ jsonfmt test/example.json -f toml
 ```
 
-Output:
+*Output:*
 ```toml
 age = 23
 gender = "纯爷们"
 money = 3.1415926
 name = "Bob"
 [[actions]]
 calorie = 294.9
@@ -188,26 +170,43 @@
 calorie = -375
 date = "2023-04-27"
 name = "sport"
 ```
 
 ### 5. Convert between JSON, TOML and YAML formats.
 
+<div style="color: red"><strong>Note this!</strong></div>
+The `null` value is invalid in TOML.
+Therefore, any null values in JSON or YAML will be removed when converting to TOML.
+
 ```shell
 # json to yaml
-$ jsonfmt -f yaml test/example.json
+$ jsonfmt test/example.json -f yaml
 
 # yaml to toml
-$ jsonfmt -f toml test/example.yaml
+$ jsonfmt test/example.yaml -f toml
 
 # toml to json
-$ jsonfmt -f json test/example.toml
+$ jsonfmt test/example.toml -f json
+```
+
+### 6. Copy the result to clipboard.
+
+```shell
+$ jsonfmt -C test/example.json
+
+# Output
+jsonfmt: result copied to clipboard.
 ```
 
-### 6. Other usages
+You can then use <kbd>ctrl</kbd>+<kbd>v</kbd> or <kbd>cmd</kbd>+<kbd>v</kbd> to paste the result anywhere on your computer.
+
+But when you process multiple files, only the last result is kept in the clipboard.
+
+### 7. Other usages
 
 - use the `-O` parameter to overwrite the file with the result.
 
 ```shell
 $ jsonfmt -O test/example.json
 ```
```

### Comparing `jsonfmt-0.2.0/jsonfmt.py` & `jsonfmt-0.2.1/jsonfmt.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 #!/usr/bin/env python
 '''JSON Format Tool'''
 
 import json
+import pyperclip
 import toml
 import yaml
 from argparse import ArgumentParser
 from functools import partial
 from pygments import highlight
 from pygments.formatters import TerminalFormatter
 from pygments.lexers import JsonLexer, TOMLLexer, YamlLexer
 from sys import stdin, stdout, stderr, exit
 from typing import Any, List, IO, Optional, Sequence, Union
 
-__version__ = '0.2.0'
+__version__ = '0.2.1'
+
+
+def print_inf(msg: str):
+    print(f'\033[1;94mjsonfmt:\033[0m \033[0;94m{msg}\033[0m')
 
 
 def print_err(msg: str):
     print(f'\033[1;91mjsonfmt:\033[0m \033[0;91m{msg}\033[0m', file=stderr)
 
 
 class JSONPathError(Exception):
@@ -73,85 +78,93 @@
     try:
         return match_element(py_obj, jpath_components)
     except JSONPathError as err:
         print_err(f'{err}')
         raise ParseError from err
 
 
-def output_json(py_obj: Any, output_fp: IO, compact: bool,
+def output_json(py_obj: Any, output_fp: IO, *, cp2clip: bool, compact: bool,
                 escape: bool, indent: int):
     '''output formated json to file or stdout'''
-    if output_fp.fileno() > 2:
-        output_fp.seek(0)
-        output_fp.truncate()
-
     if compact:
         json_text = json.dumps(py_obj, ensure_ascii=escape, sort_keys=True,
                                separators=(',', ':'))
     else:
         json_text = json.dumps(py_obj, ensure_ascii=escape, sort_keys=True,
                                indent=indent)
 
+    # copy the result to clipboard
+    if cp2clip:
+        pyperclip.copy(json_text)
+        print_inf('result copied to clipboard.')
+        return
+
     # highlight the json code when output to TTY divice
     if output_fp.isatty():
         json_text = highlight(json_text, JsonLexer(), TerminalFormatter())
 
-    # append a blank line at the end of `fp``
+    # append a blank line at the end of `fp`
     if json_text[-1] != '\n':
         json_text += '\n'
 
     output_fp.write(json_text)
 
 
-def output_toml(py_obj: Any, output_fp: IO):
+def output_toml(py_obj: Any, output_fp: IO, *, cp2clip: bool):
     '''output formated toml to file or stdout'''
     if not isinstance(py_obj, dict):
         print_err('the pyobj must be a Mapping when format to toml')
         exit(3)
 
-    if output_fp.fileno() > 2:
-        output_fp.seek(0)
-        output_fp.truncate()
+    toml_text = toml.dumps(py_obj)
+
+    # copy the result to clipboard
+    if cp2clip:
+        pyperclip.copy(toml_text)
+        print_inf('result copied to clipboard.')
+        return
 
     # highlight the toml code when output to TTY divice
     if output_fp.isatty():
-        toml_text = toml.dumps(py_obj)
-        highlight_toml = highlight(toml_text, TOMLLexer(), TerminalFormatter())
-        output_fp.write(highlight_toml)
-    else:
-        toml.dump(py_obj, output_fp)
+        toml_text = highlight(toml_text, TOMLLexer(), TerminalFormatter())
 
+    output_fp.write(toml_text)
 
-def output_yaml(py_obj: Any, output_fp: IO, escape: bool, indent: int):
+
+def output_yaml(py_obj: Any, output_fp: IO, *, cp2clip: bool, escape: bool, indent: int):
     '''output formated yaml to file or stdout'''
-    if output_fp.fileno() > 2:
-        output_fp.seek(0)
-        output_fp.truncate()
+    yaml_text = yaml.safe_dump(py_obj, allow_unicode=not escape, indent=indent,
+                               sort_keys=True)
+
+    # copy the result to clipboard
+    if cp2clip:
+        pyperclip.copy(yaml_text)
+        print_inf('result copied to clipboard.')
+        return
 
     # highlight the yaml code when output to TTY divice
     if output_fp.isatty():
-        yaml_text = yaml.safe_dump(py_obj, allow_unicode=not escape,
-                                   indent=indent, sort_keys=True)
-        highlight_yaml = highlight(yaml_text, YamlLexer(), TerminalFormatter())
-        output_fp.write(highlight_yaml)
-    else:
-        yaml.safe_dump(py_obj, output_fp, allow_unicode=not escape,
-                       indent=indent, sort_keys=True)
+        yaml_text = highlight(yaml_text, YamlLexer(), TerminalFormatter())
+
+    output_fp.write(yaml_text)
 
 
 def parse_cmdline_args(args: Optional[Sequence[str]] = None):
     parser = ArgumentParser('jsonfmt')
     parser.add_argument('-c', dest='compact', action='store_true',
                         help='compact the json object to a single line')
+    parser.add_argument('-C', dest='cp2clip', action='store_true',
+                        help='copy the result to clipboard')
     parser.add_argument('-e', dest='escape', action='store_true',
                         help='escape non-ASCII characters')
-    parser.add_argument('-f', dest='format', choices=['json', 'toml', 'yaml'],
-                        default='json', help='the format to output (default: %(default)s)')
+    parser.add_argument('-f', dest='format', default='json',
+                        choices=['json', 'toml', 'yaml'],
+                        help='the format to output ''(default: %(default)s)')
     parser.add_argument('-i', dest='indent', type=int, default=2,
-                        help='number of spaces to use for indentation (default: %(default)s)')
+                        help='number of spaces for indentation (default: %(default)s)')
     parser.add_argument('-O', dest='overwrite', action='store_true',
                         help='overwrite the formated text to original file')
     parser.add_argument('-p', dest='jsonpath', type=str, default='',
                         help='output part of the object via jsonpath')
     parser.add_argument(dest='files', nargs='*',
                         help='the files that will be processed')
     parser.add_argument('-v', dest='version', action='version',
@@ -160,37 +173,44 @@
 
 
 def main():
     args = parse_cmdline_args()
 
     # match the specified output function
     fn_output = {
-        'json': partial(output_json, compact=args.compact,
+        'json': partial(output_json, cp2clip=args.cp2clip, compact=args.compact,
                         escape=args.escape, indent=args.indent),
-        'yaml': partial(output_yaml, escape=args.escape, indent=args.indent),
-        'toml': output_toml,
+        'yaml': partial(output_yaml, cp2clip=args.cp2clip, escape=args.escape, indent=args.indent),
+        'toml': partial(output_toml, cp2clip=args.cp2clip),
     }[args.format]
 
     if args.files:
         for file in args.files:
             try:
                 # read from file
                 with open(file, 'r+') as input_fp:
                     try:
                         py_obj = parse_to_pyobj(input_fp, args.jsonpath)
                     except ParseError:
                         exit(1)
                     else:
-                        output_fp = input_fp if args.overwrite else stdout
+                        if args.overwrite:
+                            # truncate file to zero length before overwrite
+                            input_fp.seek(0)
+                            input_fp.truncate()
+                            output_fp = input_fp
+                        else:
+                            output_fp = stdout
+
                         fn_output(py_obj, output_fp)
             except FileNotFoundError:
                 print_err(f'no such file `{file}`')
     else:
-        # read from stdin
         try:
+            # read from stdin
             py_obj = parse_to_pyobj(stdin, args.jsonpath)
         except ParseError:
             exit(2)
         else:
             fn_output(py_obj, stdout)
```

### Comparing `jsonfmt-0.2.0/pyproject.toml` & `jsonfmt-0.2.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 license = {text = "MIT License"}
 description = "A simple tool for formatting JSON object."
 readme = "README.md"
 keywords = ["json", "formatter", "pretty-print", "highlight", "jsonpath"]
 authors = [{name = "Seamile", email = "lanhuermao@gmail.com"}]
 dependencies = [
     "Pygments >= 2.13.0",
+    "pyperclip >= 1.8.2",
     "pyyaml >= 6.0",
     "toml >= 0.10.2"
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "License :: OSI Approved :: MIT License",
```

### Comparing `jsonfmt-0.2.0/test/test.py` & `jsonfmt-0.2.1/test/test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 import os
 import sys
 import tempfile
 import unittest
+import pyperclip
 from argparse import Namespace
 from functools import partial
 from io import StringIO
 from pygments import highlight
 from pygments.formatters import TerminalFormatter
 from pygments.lexers import JsonLexer, YamlLexer, TOMLLexer
 from unittest.mock import patch
@@ -130,89 +131,96 @@
     @patch('jsonfmt.stdout', FakeStdOut())
     def test_output_json(self):
         py_obj = {"name": "约翰", "age": 30}
 
         # test output json to file (temp file)
         with_indent_output = '{\n "age": 30,\n "name": "\\u7ea6\\u7ff0"\n}\n'
         with tempfile.NamedTemporaryFile(mode='r+') as tmpfile:
-            jsonfmt.output_json(py_obj, tmpfile, False, True, 1)
+            jsonfmt.output_json(py_obj, tmpfile, cp2clip=False,
+                                compact=False, escape=True, indent=1)
             tmpfile.seek(0)
             output_str = tmpfile.read()
             self.assertEqual(output_str, with_indent_output)
 
         # test output json to stdout (mock)
         compact_and_colored = color('{"age":30,"name":"约翰"}', 'json')
-        jsonfmt.output_json(py_obj, jsonfmt.stdout, True, False, 4)
+        jsonfmt.output_json(py_obj, jsonfmt.stdout, cp2clip=False,
+                            compact=True, escape=False, indent=4)
         self.assertEqual(jsonfmt.stdout.read(), compact_and_colored)
 
     @patch.multiple(jsonfmt, stdout=FakeStdOut(), stderr=FakeStdErr())
     def test_output_toml(self):
         py_obj = {"name": "约翰", "age": 30}
         expected_outputs = ['name = "约翰"\nage = 30\n',
                             'age = 30\nname = "约翰"\n']
 
         # test output toml to file (temp file)
         with tempfile.NamedTemporaryFile(mode='r+') as tmpfile:
-            jsonfmt.output_toml(py_obj, tmpfile)
+            jsonfmt.output_toml(py_obj, tmpfile, cp2clip=False)
             tmpfile.seek(0)
             self.assertIn(tmpfile.read(), expected_outputs)
 
         # test output toml to stdout (mock)
         colored_outputs = [color(o, 'toml') for o in expected_outputs]
-        jsonfmt.output_toml(py_obj, jsonfmt.stdout)
+        jsonfmt.output_toml(py_obj, jsonfmt.stdout, cp2clip=False)
         self.assertIn(jsonfmt.stdout.read(), colored_outputs)
 
         # test SystemExit when using non-mapping
         with self.assertRaises(SystemExit) as raise_ctx:
-            jsonfmt.output_toml(['foo', 'bar'], jsonfmt.stdout)
+            jsonfmt.output_toml(['foo', 'bar'], jsonfmt.stdout, cp2clip=False)
             self.assertEqual(raise_ctx.exception.code, 3)
 
     @patch('jsonfmt.stdout', FakeStdOut())
     def test_output_yaml(self):
         py_obj = {"name": "约翰", "age": 30}
 
         # test output yaml to file (temp file)
         expected_output = 'age: 30\nname: "\\u7EA6\\u7FF0"\n'
         with tempfile.NamedTemporaryFile(mode='r+') as tmpfile:
-            jsonfmt.output_yaml(py_obj, tmpfile, True, 2)
+            jsonfmt.output_yaml(py_obj, tmpfile, cp2clip=False,
+                                escape=True, indent=2)
             tmpfile.seek(0)
             self.assertEqual(tmpfile.read(), expected_output)
 
         # jsonfmt.output to stdout (mock)
         colored_output = color('age: 30\nname: 约翰\n', 'yaml')
-        jsonfmt.output_yaml(py_obj, jsonfmt.stdout, False, 2)
+        jsonfmt.output_yaml(py_obj, jsonfmt.stdout, cp2clip=False,
+                            escape=False, indent=2)
         self.assertEqual(jsonfmt.stdout.read(), colored_output)
 
     def test_parse_cmdline_args(self):
         # test default parameters
         default_args = Namespace(
             compact=False,
+            cp2clip=False,
             escape=False,
             format='json',
             indent=2,
             overwrite=False,
             jsonpath='',
             files=[]
         )
         actual_args = jsonfmt.parse_cmdline_args([])
         self.assertEqual(actual_args, default_args)
 
         # test specified parameters
         args = [
             '-c',
+            '-C',
             '-e',
             '-f', 'toml',
             '-i', '4',
             '-O',
             '-p', 'path/to/json',
             'file1.json',
             'file2.json'
         ]
         expected_args = Namespace(
             compact=True,
+            cp2clip=True,
             escape=True,
             format='toml',
             indent=4,
             overwrite=True,
             jsonpath='path/to/json',
             files=['file1.json', 'file2.json']
         )
@@ -265,10 +273,40 @@
     @patch.multiple(sys, argv=['jsonfmt', '-c', '-f', 'json'])
     @patch.multiple(jsonfmt, stdin=FakeStdIn(YAML_TEXT), stdout=FakeStdOut())
     def test_yaml_to_json(self):
         colored_output = color(JSON_TEXT, 'json')
         jsonfmt.main()
         self.assertEqual(jsonfmt.stdout.read(), colored_output)
 
+    @patch.multiple(sys, argv=['jsonfmt', '-cO', f'{BASE_DIR}/test/example.toml'])
+    def test_overwrite_to_original_file(self):
+        try:
+            jsonfmt.main()
+            with open(f'{BASE_DIR}/test/example.toml') as toml_fp:
+                new_content = toml_fp.read()
+            self.assertEqual(new_content, JSON_TEXT)
+        finally:
+            with open(f'{BASE_DIR}/test/example.toml', 'w') as toml_fp:
+                toml_fp.write(TOML_TEXT)
+
+    def test_copy_to_clipboard(self):
+        try:
+            with patch("sys.argv", ['jsonfmt', f'{BASE_DIR}/test/example.toml', '-Cc']):
+                jsonfmt.main()
+                copied_text = pyperclip.paste().strip()
+                self.assertEqual(copied_text, JSON_TEXT.strip())
+
+            with patch("sys.argv", ['jsonfmt', f'{BASE_DIR}/test/example.json', '-Cf', 'toml']):
+                jsonfmt.main()
+                copied_text = pyperclip.paste().strip()
+                self.assertEqual(copied_text, TOML_TEXT.strip())
+
+            with patch("sys.argv", ['jsonfmt', f'{BASE_DIR}/test/example.json', '-Cf', 'yaml']):
+                jsonfmt.main()
+                copied_text = pyperclip.paste().strip()
+                self.assertEqual(copied_text, YAML_TEXT.strip())
+        except pyperclip.PyperclipException as e:
+            jsonfmt.print_err(e)  # type: ignore
+
 
 if __name__ == '__main__':
     unittest.main()
```

