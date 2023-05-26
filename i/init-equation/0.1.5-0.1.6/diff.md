# Comparing `tmp/init_equation-0.1.5.tar.gz` & `tmp/init_equation-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "init_equation-0.1.5.tar", max compression
+gzip compressed data, was "init_equation-0.1.6.tar", max compression
```

## Comparing `init_equation-0.1.5.tar` & `init_equation-0.1.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1081 2023-03-22 15:09:01.820624 init_equation-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-03-10 05:56:08.778276 init_equation-0.1.5/init_equation/__init__.py
--rw-r--r--   0        0        0       55 2023-03-10 06:42:17.894790 init_equation-0.1.5/init_equation/__main__.py
--rw-r--r--   0        0        0     1263 2023-03-13 13:12:21.163423 init_equation-0.1.5/init_equation/chapters.py
--rw-r--r--   0        0        0     1236 2023-03-10 06:10:03.992578 init_equation-0.1.5/init_equation/choice_option.py
--rw-r--r--   0        0        0     2791 2023-03-13 13:13:34.587451 init_equation-0.1.5/init_equation/equation.py
--rw-r--r--   0        0        0     3711 2023-04-01 11:48:22.978771 init_equation-0.1.5/init_equation/main.py
--rw-r--r--   0        0        0      488 2023-04-01 11:48:37.803376 init_equation-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1481 1970-01-01 00:00:00.000000 init_equation-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-03-22 15:09:01.820624 init_equation-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-03-10 05:56:08.778276 init_equation-0.1.6/init_equation/__init__.py
+-rw-r--r--   0        0        0       55 2023-03-10 06:42:17.894790 init_equation-0.1.6/init_equation/__main__.py
+-rw-r--r--   0        0        0     1263 2023-03-13 13:12:21.163423 init_equation-0.1.6/init_equation/chapters.py
+-rw-r--r--   0        0        0     1236 2023-03-10 06:10:03.992578 init_equation-0.1.6/init_equation/choice_option.py
+-rw-r--r--   0        0        0     2791 2023-03-13 13:13:34.587451 init_equation-0.1.6/init_equation/equation.py
+-rw-r--r--   0        0        0     3936 2023-05-26 08:31:31.447016 init_equation-0.1.6/init_equation/main.py
+-rw-r--r--   0        0        0      427 2023-05-26 08:33:09.777248 init_equation-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1420 1970-01-01 00:00:00.000000 init_equation-0.1.6/PKG-INFO
```

### Comparing `init_equation-0.1.5/README.md` & `init_equation-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `init_equation-0.1.5/init_equation/chapters.py` & `init_equation-0.1.6/init_equation/chapters.py`

 * *Files identical despite different names*

### Comparing `init_equation-0.1.5/init_equation/choice_option.py` & `init_equation-0.1.6/init_equation/choice_option.py`

 * *Files identical despite different names*

### Comparing `init_equation-0.1.5/init_equation/equation.py` & `init_equation-0.1.6/init_equation/equation.py`

 * *Files identical despite different names*

### Comparing `init_equation-0.1.5/init_equation/main.py` & `init_equation-0.1.6/init_equation/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,27 @@
 from .equation import Equation
 from .choice_option import ChoiceOption
 
 path_parent = os.environ["TEX_PARENT_PATH"] 
 
 eqn_number_without_database = f'{int(time.strftime("%H%M%S%d%m%Y")):14}'
 
+link = r"""
+\def\gdrive{Link}
+"""
+
+qrcode = r"""
+\pagebreak
+
+\vspace*{\fill}
+\begin{center}
+    \fbox{\qrcode[height=2cm]{\gdrive}}
+\end{center}
+\vspace*{\fill}
+"""
 
 size_square = f'\\vgeometry\n\n'
 size_h_rectangle = f'\\vgeometry[8][4.5][15][15][10][10]\n\n'
 size_v_rectangle = f'\\vgeometry[4.5][8][15][15][10][10]\n\n'
 
 CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help'])
 
@@ -100,25 +113,27 @@
                 file.write(size_square)
             elif size == 'h-rectangle':
                 file.write(size_h_rectangle)
             elif size == 'v-rectangle':
                 file.write(size_v_rectangle)
 
             file.write(f'\\begin{{document}}\n')
+            file.write(link)
             file.write(f'\\vtitle[title]\n')
             file.write(f'\\begin{{center}}\n')
             file.write(f'\\begin{{tikzpicture}}\n')
             file.write(f'\\tzdot*(0, 0)\n')
             file.write(f'\\end{{tikzpicture}}\n')
             file.write(f'\\end{{center}}\n')
             file.write(f'\\vspace*{{\\fill}}\n')
             file.write(f'\\begin{{align*}}\n')
             file.write(f'\\int x dx\n')
             file.write(f'\\end{{align*}}\n')
             file.write(f'\\vspace*{{\\fill}}\n')
+            file.write(qrcode)
             file.write(f'\\end{{document}}\n')
 
 
 
     os.system(f'bat {main_tex}')
     time.sleep(1)
     os.system(f'open -a texmaker {main_tex}')
```

### Comparing `init_equation-0.1.5/PKG-INFO` & `init_equation-0.1.6/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: init-equation
-Version: 0.1.5
-Summary: Added a copy option as flag if true the main.tex file will be copied from the previous equation number.
+Version: 0.1.6
+Summary: Added qrcode lines in main.py for main.tex
 Author: vaibhavblayer
 Author-email: vaibhavblayer@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

