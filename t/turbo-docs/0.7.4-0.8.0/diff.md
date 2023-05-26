# Comparing `tmp/turbo_docs-0.7.4.tar.gz` & `tmp/turbo_docs-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\turbo_docs-0.7.4.tar", last modified: Sat Apr 29 00:24:12 2023, max compression
+gzip compressed data, was "dist\turbo_docs-0.8.0.tar", last modified: Fri May 26 14:19:42 2023, max compression
```

## Comparing `turbo_docs-0.7.4.tar` & `turbo_docs-0.8.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 00:24:12.801364 turbo_docs-0.7.4/
--rw-rw-rw-   0        0        0     1199 2023-04-29 00:24:12.801364 turbo_docs-0.7.4/PKG-INFO
--rw-rw-rw-   0        0        0      743 2023-04-29 00:23:36.000000 turbo_docs-0.7.4/README.md
--rw-rw-rw-   0        0        0       42 2023-04-29 00:24:12.802474 turbo_docs-0.7.4/setup.cfg
--rw-rw-rw-   0        0        0      757 2023-04-29 00:16:43.000000 turbo_docs-0.7.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-29 00:24:12.777153 turbo_docs-0.7.4/turbo_docs/
--rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.7.4/turbo_docs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 00:24:12.791747 turbo_docs-0.7.4/turbo_docs/commands/
--rw-rw-rw-   0        0        0        0 2023-04-22 22:02:08.000000 turbo_docs-0.7.4/turbo_docs/commands/__init__.py
--rw-rw-rw-   0        0        0     2163 2023-04-28 23:59:47.000000 turbo_docs-0.7.4/turbo_docs/commands/docstring.py
--rw-rw-rw-   0        0        0     1669 2023-04-29 00:14:51.000000 turbo_docs-0.7.4/turbo_docs/commands/readme.py
--rw-rw-rw-   0        0        0     1221 2023-04-29 00:15:18.000000 turbo_docs-0.7.4/turbo_docs/generate.py
-drwxrwxrwx   0        0        0        0 2023-04-29 00:24:12.799356 turbo_docs-0.7.4/turbo_docs/utils/
--rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.7.4/turbo_docs/utils/__init__.py
--rw-rw-rw-   0        0        0     1222 2023-04-29 00:15:09.000000 turbo_docs-0.7.4/turbo_docs/utils/cli_options.py
--rw-rw-rw-   0        0        0     1871 2023-04-29 00:15:05.000000 turbo_docs-0.7.4/turbo_docs/utils/directory.py
--rw-rw-rw-   0        0        0     1467 2023-04-29 00:08:47.000000 turbo_docs-0.7.4/turbo_docs/utils/openai_api.py
-drwxrwxrwx   0        0        0        0 2023-04-29 00:24:12.787229 turbo_docs-0.7.4/turbo_docs.egg-info/
--rw-rw-rw-   0        0        0     1199 2023-04-29 00:24:12.000000 turbo_docs-0.7.4/turbo_docs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      487 2023-04-29 00:24:12.000000 turbo_docs-0.7.4/turbo_docs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 00:24:12.000000 turbo_docs-0.7.4/turbo_docs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-04-29 00:24:12.000000 turbo_docs-0.7.4/turbo_docs.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       51 2023-04-29 00:24:12.000000 turbo_docs-0.7.4/turbo_docs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-29 00:24:12.000000 turbo_docs-0.7.4/turbo_docs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-26 14:19:42.635946 turbo_docs-0.8.0/
+-rw-rw-rw-   0        0        0     2080 2023-05-26 14:19:42.634953 turbo_docs-0.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1624 2023-05-26 14:19:21.000000 turbo_docs-0.8.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-26 14:19:42.635946 turbo_docs-0.8.0/setup.cfg
+-rw-rw-rw-   0        0        0      757 2023-05-26 13:43:40.000000 turbo_docs-0.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 14:19:42.607699 turbo_docs-0.8.0/turbo_docs/
+-rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.8.0/turbo_docs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 14:19:42.625803 turbo_docs-0.8.0/turbo_docs/commands/
+-rw-rw-rw-   0        0        0        0 2023-04-29 00:25:31.000000 turbo_docs-0.8.0/turbo_docs/commands/__init__.py
+-rw-rw-rw-   0        0        0     2163 2023-05-26 13:55:07.000000 turbo_docs-0.8.0/turbo_docs/commands/docstring.py
+-rw-rw-rw-   0        0        0      663 2023-05-26 14:15:07.000000 turbo_docs-0.8.0/turbo_docs/commands/readme.py
+-rw-rw-rw-   0        0        0     1036 2023-05-26 13:55:51.000000 turbo_docs-0.8.0/turbo_docs/generate.py
+drwxrwxrwx   0        0        0        0 2023-05-26 14:19:42.632948 turbo_docs-0.8.0/turbo_docs/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.8.0/turbo_docs/utils/__init__.py
+-rw-rw-rw-   0        0        0      653 2023-05-26 14:15:08.000000 turbo_docs-0.8.0/turbo_docs/utils/cli_options.py
+-rw-rw-rw-   0        0        0     1871 2023-04-29 00:25:31.000000 turbo_docs-0.8.0/turbo_docs/utils/directory.py
+-rw-rw-rw-   0        0        0     1581 2023-05-26 14:15:10.000000 turbo_docs-0.8.0/turbo_docs/utils/openai_api.py
+drwxrwxrwx   0        0        0        0 2023-05-26 14:19:42.618853 turbo_docs-0.8.0/turbo_docs.egg-info/
+-rw-rw-rw-   0        0        0     2080 2023-05-26 14:19:42.000000 turbo_docs-0.8.0/turbo_docs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      487 2023-05-26 14:19:42.000000 turbo_docs-0.8.0/turbo_docs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 14:19:42.000000 turbo_docs-0.8.0/turbo_docs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-05-26 14:19:42.000000 turbo_docs-0.8.0/turbo_docs.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       51 2023-05-26 14:19:42.000000 turbo_docs-0.8.0/turbo_docs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-26 14:19:42.000000 turbo_docs-0.8.0/turbo_docs.egg-info/top_level.txt
```

### Comparing `turbo_docs-0.7.4/setup.py` & `turbo_docs-0.8.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
 	name="turbo_docs",
-	version="0.7.4",
+	version="0.8.0",
 	packages=find_packages(),
 	install_requires=[
 		"requests",
 		"openai",
 		"click",
 		"pyperclip",
 		"redbaron",
```

### Comparing `turbo_docs-0.7.4/turbo_docs/commands/docstring.py` & `turbo_docs-0.8.0/turbo_docs/commands/docstring.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-0.7.4/turbo_docs/generate.py` & `turbo_docs-0.8.0/turbo_docs/generate.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,24 +4,22 @@
 from turbo_docs.commands import readme as readme_module
 from turbo_docs.utils import directory, cli_options
 
 
 @click.command()
 @cli_options.copy
 @cli_options.readme
-@cli_options.readme_large_repo
 @cli_options.docstring
 def driver(
         copy: bool,
         readme: bool,
-        readme_large_repo: bool,
         docstring: bool,
 ) -> None:
     """
-    Generate a README or docs.md for the current directory.
+    Generate a README or docstring for the current directory.
     """
     files = directory.get_files()
     dir_text = "\n\n".join(
         [f"{name}:\n\n{content}" for name, content in files.items()])
 
     # Copy directory text to clipboard if specified
     if copy:
@@ -32,15 +30,10 @@
     if docstring:
         docstring_module.docstring(files)
 
     # Generate README.md file if specified
     if readme:
         readme_module.readme(dir_text)
 
-    # Generate docs.md file if specified
-    if readme_large_repo:
-        readme_module.readme_large_repo(files)
-
-
 
 if __name__ == '__main__':
     driver()
```

### Comparing `turbo_docs-0.7.4/turbo_docs/utils/cli_options.py` & `turbo_docs-0.8.0/turbo_docs/utils/cli_options.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,26 @@
 import click
 from typing import Callable
 
 def copy(func: Callable) -> Callable:
-    """
-    Copy the directory text to clipboard.
-    """
     return click.option(
         '--copy',
         default=False,
         is_flag=True,
         help='Copy the directory text to clipboard'
     )(func)
 
 def readme(func: Callable) -> Callable:
-    """
-    Add --readme option to a click command to generate a README.md file.
-    """
     return click.option(
         '--readme',
         default=False,
         is_flag=True,
         help='Generate README.md file'
     )(func)
 
-def readme_large_repo(func: Callable) -> Callable:
-    """
-    Decorate a given callable to add an option to generate readme for larger
-    repositories.
-    """
-    return click.option(
-        '--readme_large_repo',
-        default=False,
-        is_flag=True,
-        help='Generate readme for larger repositories'
-    )(func)
-
 def docstring(func: Callable) -> Callable:
-    """
-    Generate and insert docstrings for each function.
-    """
     return click.option(
         '--docstring',
         default=False,
         is_flag=True,
         help='Generate and insert docstrings for each function'
     )(func)
```

### Comparing `turbo_docs-0.7.4/turbo_docs/utils/directory.py` & `turbo_docs-0.8.0/turbo_docs/utils/directory.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-0.7.4/turbo_docs/utils/openai_api.py` & `turbo_docs-0.8.0/turbo_docs/utils/openai_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,29 +13,29 @@
     if not openai.api_key:
         print("OpenAI API key is not set. Please set it as an environment variable (export OPENAI_API_KEY=<your_api_key>) or enter it below.")
         print("If you have not done so already, create an OpenAI account at https://platform.openai.com/overview.")
         openai.api_key = input("Secret key:")
     return openai
 
 
-def gpt_completion_wrapper(prompt, openai_package=None):
+def gpt_completion_wrapper(prompt, openai_package=None, gpt_engine="gpt-4"):
     """
     Provide GPT-3 completions for a given prompt and optional OpenAI package.
     """
     if not openai_package:
         openai_package = openai_init()
 
-    completions = openai_package.Completion.create(
-        engine="text-davinci-003",
-        prompt=prompt,
-        max_tokens=2048,
-        n=1,
-        stop=None,
-    )
-    return completions.choices[0]['text'].strip()
+    resp = openai_package.ChatCompletion.create(
+        model=gpt_engine,
+        messages=[
+                {"role": "system", "content": "You are a helpful coding assistant."},
+                {"role": "user", "content": prompt},
+            ]
+        )
+    return resp['choices'][0]['message']['content'].strip()
 
 
 def gpt_completion_error_handler(prompt):
     """
     Handle errors raised by OpenAI GPT completion API.
     """
     text = None
```

