# Comparing `tmp/py_gf_auto_doc-0.1.0.tar.gz` & `tmp/py_gf_auto_doc-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_gf_auto_doc-0.1.0.tar", last modified: Thu May 25 10:45:20 2023, max compression
+gzip compressed data, was "py_gf_auto_doc-0.1.1.tar", last modified: Fri May 26 07:20:10 2023, max compression
```

## Comparing `py_gf_auto_doc-0.1.0.tar` & `py_gf_auto_doc-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 10:45:20.244155 py_gf_auto_doc-0.1.0/
--rw-rw-rw-   0        0        0     1084 2023-05-25 10:38:48.000000 py_gf_auto_doc-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      736 2023-05-25 10:45:20.244155 py_gf_auto_doc-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      177 2023-05-25 10:38:48.000000 py_gf_auto_doc-0.1.0/README.md
--rw-rw-rw-   0        0        0      549 2023-05-25 10:44:12.000000 py_gf_auto_doc-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-25 10:45:20.245155 py_gf_auto_doc-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-25 10:45:20.217149 py_gf_auto_doc-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-25 10:45:20.233153 py_gf_auto_doc-0.1.0/src/py_gf_auto_doc/
--rw-rw-rw-   0        0        0      296 2023-05-23 08:31:59.000000 py_gf_auto_doc-0.1.0/src/py_gf_auto_doc/__main__.py
--rw-rw-rw-   0        0        0     6175 2023-05-24 07:21:14.000000 py_gf_auto_doc-0.1.0/src/py_gf_auto_doc/doc_gen.py
-drwxrwxrwx   0        0        0        0 2023-05-25 10:45:20.241154 py_gf_auto_doc-0.1.0/src/py_gf_auto_doc.egg-info/
--rw-rw-rw-   0        0        0      736 2023-05-25 10:45:20.000000 py_gf_auto_doc-0.1.0/src/py_gf_auto_doc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2023-05-25 10:45:20.000000 py_gf_auto_doc-0.1.0/src/py_gf_auto_doc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 10:45:20.000000 py_gf_auto_doc-0.1.0/src/py_gf_auto_doc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-25 10:45:20.000000 py_gf_auto_doc-0.1.0/src/py_gf_auto_doc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-26 07:20:10.350901 py_gf_auto_doc-0.1.1/
+-rw-rw-rw-   0        0        0     1084 2023-05-25 10:38:48.000000 py_gf_auto_doc-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1416 2023-05-26 07:20:10.349901 py_gf_auto_doc-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      857 2023-05-26 07:19:31.000000 py_gf_auto_doc-0.1.1/README.md
+-rw-rw-rw-   0        0        0      549 2023-05-26 07:16:19.000000 py_gf_auto_doc-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-26 07:20:10.350901 py_gf_auto_doc-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-26 07:20:10.308765 py_gf_auto_doc-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-26 07:20:10.339901 py_gf_auto_doc-0.1.1/src/py_gf_auto_doc/
+-rw-rw-rw-   0        0        0      468 2023-05-25 11:20:02.000000 py_gf_auto_doc-0.1.1/src/py_gf_auto_doc/__main__.py
+-rw-rw-rw-   0        0        0     6678 2023-05-26 07:13:09.000000 py_gf_auto_doc-0.1.1/src/py_gf_auto_doc/doc_gen.py
+drwxrwxrwx   0        0        0        0 2023-05-26 07:20:10.347901 py_gf_auto_doc-0.1.1/src/py_gf_auto_doc.egg-info/
+-rw-rw-rw-   0        0        0     1416 2023-05-26 07:20:10.000000 py_gf_auto_doc-0.1.1/src/py_gf_auto_doc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2023-05-26 07:20:10.000000 py_gf_auto_doc-0.1.1/src/py_gf_auto_doc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 07:20:10.000000 py_gf_auto_doc-0.1.1/src/py_gf_auto_doc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-26 07:20:10.000000 py_gf_auto_doc-0.1.1/src/py_gf_auto_doc.egg-info/top_level.txt
```

### Comparing `py_gf_auto_doc-0.1.0/LICENSE` & `py_gf_auto_doc-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py_gf_auto_doc-0.1.0/PKG-INFO` & `py_gf_auto_doc-0.1.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-Metadata-Version: 2.1
-Name: py_gf_auto_doc
-Version: 0.1.0
-Summary: Auto doc generator for GitFlic book
-Author-email: Vladimir Chistov <wchistow@yandex.ru>
-Project-URL: Homepage, https://gitflic.ru/project/wchistow/py_gf_auto_doc
-Project-URL: Bug Tracker, https://gitflic.ru/project/wchistow/py_gf_auto_doc/issue
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
+[project]
+name = "py_gf_auto_doc"
+version = "0.1.1"
+authors = [
+  { name="Vladimir Chistov", email="wchistow@yandex.ru" },
+]
+description = "Auto doc generator for GitFlic book"
+readme = "README.md"
+requires-python = ">=3.10"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
 
-# PyGFAutoDoc
-## v0.1.0
-
-Автоматический генератор документации
-в формате GitFlic-книги для проектов на Python.
+[project.urls]
+"Homepage" = "https://gitflic.ru/project/wchistow/py_gf_auto_doc"
+"Bug Tracker" = "https://gitflic.ru/project/wchistow/py_gf_auto_doc/issue"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `py_gf_auto_doc-0.1.0/src/py_gf_auto_doc/doc_gen.py` & `py_gf_auto_doc-0.1.1/src/py_gf_auto_doc/doc_gen.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,73 +6,81 @@
 import os
 
 FuncT: TypeAlias = tuple[str, str, str, str | None]
 ClassT: TypeAlias = tuple[str, str, str | None, list[FuncT]]
 
 BASE_PATH = os.path.dirname(__file__)
 
-FILE_TEMPLATE = open(f'{BASE_PATH}/templates/file.txt', encoding='utf-8').read()
-FUNC_TEMPLATE = open(f'{BASE_PATH}/templates/func.txt', encoding='utf-8').read()
-CLASS_TEMPLATE = open(f'{BASE_PATH}/templates/class.txt', encoding='utf-8').read()
+with open(f'{BASE_PATH}/templates/file.txt', encoding='utf-8') as f:
+    FILE_TEMPLATE = f.read()
+with open(f'{BASE_PATH}/templates/func.txt', encoding='utf-8') as f:
+    FUNC_TEMPLATE = f.read()
+with open(f'{BASE_PATH}/templates/class.txt', encoding='utf-8') as f:
+    CLASS_TEMPLATE = f.read()
 
 
 def generate_doc(path: str, out_dir: str) -> None:
     """Главная функция генерирования документации."""
     if not os.path.exists(out_dir):
         raise FileNotFoundError(f'Каталог {out_dir} не существует.')
     path = os.path.abspath(path)
 
     summary = '\n'.join(_generate_doc(path, out_dir))
 
-    with open(os.path.join(out_dir, 'README.md'), 'w', encoding='utf-8') as f:
-        f.write('> Эта документация сгенерирована утилитой `py_gf_auto_doc`.\n')
+    with open(os.path.join(out_dir, 'README.md'), 'w', encoding='utf-8') as readme:
+        readme.write('> Эта документация сгенерирована утилитой `py_gf_auto_doc`.\n')
 
-    with open(os.path.join(out_dir, 'SUMMARY.md'), 'w', encoding='utf-8') as f:
-        f.write(summary)
+    with open(os.path.join(out_dir, 'SUMMARY.md'), 'w', encoding='utf-8') as summ:
+        summ.write(summary)
 
 
 def _generate_doc(path: str, out_dir: str, inner_dir: str = '') -> list[str]:
     """Основная логика генерирования документации."""
     summary: list[str] = []
     indent = ' ' * (4 * len(Path(inner_dir).parents))
 
     if inner_dir and not os.path.exists(os.path.join(out_dir, inner_dir)):
         os.mkdir(os.path.join(out_dir, inner_dir))
 
     for py_file in get_py_files(os.path.join(path, inner_dir)):
-        py_objs = get_prog_elems(open(os.path.join(path, inner_dir, py_file),
-                                      encoding='utf-8').read())
+        with open(os.path.join(path, inner_dir, py_file), encoding='utf-8') as py_f:
+            py_objs = get_prog_elems(py_f.read())
 
-        classes = _get_classes_templates(filter(lambda elem: elem[0] == 'class', py_objs))  # type: ignore[arg-type]
-        funcs = _get_funcs_templates(filter(lambda elem: elem[0] == 'func', py_objs))  # type: ignore[arg-type]
+        classes = '\n'.join(_get_classes_templates(
+            filter(lambda elem: elem[0] == 'class', py_objs)))  # type: ignore[arg-type]
+        funcs = '\n'.join(_get_funcs_templates(
+            filter(lambda elem: elem[0] == 'func', py_objs)))  # type: ignore[arg-type]
 
         out_text = FILE_TEMPLATE.format(filename=py_file,
-                                        classes='\n'.join(classes),
-                                        funcs='\n'.join(funcs))
+                                        classes=classes or '*Нет классов*',
+                                        funcs=funcs or '*Нет функций*'
+                                        )
 
         filename = '.'.join(py_file.split('.')[:-1])
 
-        with open(os.path.join(out_dir, inner_dir, filename + '.md'), 'w', encoding='utf-8') as f:
-            f.write(out_text)
+        with open(os.path.join(out_dir, inner_dir, filename + '.md'),
+                  'w', encoding='utf-8') as result:
+            result.write(out_text)
 
         summary.append(f'{indent}* [{filename}]({os.path.join(inner_dir, filename + ".md")})')
 
     for directory in (item for item in os.listdir(path)
                       if os.path.isdir(os.path.join(path, inner_dir, item))
                       and item != '.'):
         if len(get_py_files(os.path.join(path, inner_dir, directory))) != 0:
             summary.append(f'{indent}* [{directory}]()')
             summary.extend(_generate_doc(path, out_dir, os.path.join(inner_dir, directory)))
 
     return summary
 
 
 def _get_classes_templates(classes: Iterable[ClassT]) -> list[str]:
+    """Возвращает список шаблонов `CLASS_TEMPLATE` отформатированных данными из `classes`."""
     result = []
-    for typ, signature, docstring, meths in classes:
+    for _, signature, docstring, meths in classes:
         meths_templates = []
         for _, meth_name, meth_signature, meth_docstring in meths:
             meths_templates.append(FUNC_TEMPLATE.format(name=meth_name,
                                                         signature=meth_signature,
                                                         docstring=meth_docstring or ''
                                                         )
                                    )
@@ -80,16 +88,17 @@
                                                docstring=docstring or '',
                                                meths='\n'.join(meths_templates))
         result.append(class_template)
     return result
 
 
 def _get_funcs_templates(funcs: Iterable[FuncT]) -> list[str]:
+    """Возвращает список шаблонов `FUNC_TEMPLATE` отформатированных данными из `funcs`."""
     result = []
-    for typ, name, signature, docstring in funcs:
+    for _, name, signature, docstring in funcs:
         func_template = FUNC_TEMPLATE.format(name=name,
                                              signature=signature,
                                              docstring=docstring or '')
         result.append(func_template)
     return result
```

