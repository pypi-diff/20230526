# Comparing `tmp/alive-progress-3.1.2.tar.gz` & `tmp/alive-progress-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alive-progress-3.1.2.tar", last modified: Tue May  9 01:09:06 2023, max compression
+gzip compressed data, was "dist/alive-progress-3.1.3.tar", last modified: Fri May 26 03:44:59 2023, max compression
```

## Comparing `alive-progress-3.1.2.tar` & `alive-progress-3.1.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-05-09 01:09:06.000000 alive-progress-3.1.2/
--rw-r--r--   0 rogerio    (501) staff       (20)     1084 2019-08-05 05:55:53.000000 alive-progress-3.1.2/LICENSE
--rw-r--r--   0 rogerio    (501) staff       (20)    75898 2023-05-09 01:09:06.000000 alive-progress-3.1.2/PKG-INFO
--rw-r--r--   0 rogerio    (501) staff       (20)    67100 2023-04-19 02:55:54.000000 alive-progress-3.1.2/README.md
-drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-05-09 01:09:06.000000 alive-progress-3.1.2/alive_progress/
--rw-r--r--   0 rogerio    (501) staff       (20)      417 2023-05-09 01:08:53.000000 alive-progress-3.1.2/alive_progress/__init__.py
-drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-05-09 01:09:06.000000 alive-progress-3.1.2/alive_progress/animations/
--rw-r--r--   0 rogerio    (501) staff       (20)      481 2021-08-26 23:38:44.000000 alive-progress-3.1.2/alive_progress/animations/__init__.py
--rw-r--r--   0 rogerio    (501) staff       (20)     9721 2023-03-24 02:50:30.000000 alive-progress-3.1.2/alive_progress/animations/bars.py
--rw-r--r--   0 rogerio    (501) staff       (20)    13834 2023-03-24 02:50:30.000000 alive-progress-3.1.2/alive_progress/animations/spinner_compiler.py
--rw-r--r--   0 rogerio    (501) staff       (20)    11443 2023-03-24 02:50:30.000000 alive-progress-3.1.2/alive_progress/animations/spinners.py
--rw-r--r--   0 rogerio    (501) staff       (20)     4723 2021-08-26 23:38:44.000000 alive-progress-3.1.2/alive_progress/animations/utils.py
-drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-05-09 01:09:06.000000 alive-progress-3.1.2/alive_progress/core/
--rw-r--r--   0 rogerio    (501) staff       (20)        0 2020-07-28 14:16:28.000000 alive-progress-3.1.2/alive_progress/core/__init__.py
--rw-r--r--   0 rogerio    (501) staff       (20)     1351 2022-02-02 06:03:46.000000 alive-progress-3.1.2/alive_progress/core/calibration.py
--rw-r--r--   0 rogerio    (501) staff       (20)     8876 2023-03-24 02:50:30.000000 alive-progress-3.1.2/alive_progress/core/configuration.py
--rw-r--r--   0 rogerio    (501) staff       (20)     5488 2023-05-09 01:08:53.000000 alive-progress-3.1.2/alive_progress/core/hook_manager.py
--rw-r--r--   0 rogerio    (501) staff       (20)    23500 2023-04-24 17:28:20.000000 alive-progress-3.1.2/alive_progress/core/progress.py
-drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-05-09 01:09:06.000000 alive-progress-3.1.2/alive_progress/styles/
--rw-r--r--   0 rogerio    (501) staff       (20)      614 2021-08-26 23:38:44.000000 alive-progress-3.1.2/alive_progress/styles/__init__.py
--rw-r--r--   0 rogerio    (501) staff       (20)    11233 2023-03-24 02:50:30.000000 alive-progress-3.1.2/alive_progress/styles/exhibit.py
--rw-r--r--   0 rogerio    (501) staff       (20)     8454 2023-03-24 02:50:30.000000 alive-progress-3.1.2/alive_progress/styles/internal.py
-drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-05-09 01:09:06.000000 alive-progress-3.1.2/alive_progress/tools/
--rw-r--r--   0 rogerio    (501) staff       (20)       58 2021-08-26 23:38:44.000000 alive-progress-3.1.2/alive_progress/tools/__init__.py
--rw-r--r--   0 rogerio    (501) staff       (20)     3002 2022-03-22 04:49:57.000000 alive-progress-3.1.2/alive_progress/tools/demo.py
--rw-r--r--   0 rogerio    (501) staff       (20)     1024 2021-08-26 23:38:44.000000 alive-progress-3.1.2/alive_progress/tools/repl.py
--rw-r--r--   0 rogerio    (501) staff       (20)     2717 2022-12-22 05:23:53.000000 alive-progress-3.1.2/alive_progress/tools/sampling.py
--rw-r--r--   0 rogerio    (501) staff       (20)     6634 2021-08-26 23:38:44.000000 alive-progress-3.1.2/alive_progress/tools/unicode_breaks.py
--rw-r--r--   0 rogerio    (501) staff       (20)      399 2021-08-26 23:38:44.000000 alive-progress-3.1.2/alive_progress/tools/utils.py
-drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-05-09 01:09:06.000000 alive-progress-3.1.2/alive_progress/utils/
--rw-r--r--   0 rogerio    (501) staff       (20)        0 2022-10-31 01:30:29.000000 alive-progress-3.1.2/alive_progress/utils/__init__.py
--rw-r--r--   0 rogerio    (501) staff       (20)     8811 2022-12-22 05:23:53.000000 alive-progress-3.1.2/alive_progress/utils/cells.py
--rw-r--r--   0 rogerio    (501) staff       (20)     2308 2022-02-11 05:29:12.000000 alive-progress-3.1.2/alive_progress/utils/colors.py
-drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-05-09 01:09:06.000000 alive-progress-3.1.2/alive_progress/utils/terminal/
--rw-r--r--   0 rogerio    (501) staff       (20)     2100 2023-03-24 02:50:30.000000 alive-progress-3.1.2/alive_progress/utils/terminal/__init__.py
--rw-r--r--   0 rogerio    (501) staff       (20)      747 2023-03-24 02:50:30.000000 alive-progress-3.1.2/alive_progress/utils/terminal/jupyter.py
--rw-r--r--   0 rogerio    (501) staff       (20)      418 2022-12-22 05:23:53.000000 alive-progress-3.1.2/alive_progress/utils/terminal/non_tty.py
--rw-r--r--   0 rogerio    (501) staff       (20)     1284 2023-03-24 02:50:30.000000 alive-progress-3.1.2/alive_progress/utils/terminal/tty.py
--rw-r--r--   0 rogerio    (501) staff       (20)      550 2023-03-24 02:50:30.000000 alive-progress-3.1.2/alive_progress/utils/terminal/void.py
--rw-r--r--   0 rogerio    (501) staff       (20)     1411 2022-12-22 05:23:53.000000 alive-progress-3.1.2/alive_progress/utils/timing.py
-drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-05-09 01:09:06.000000 alive-progress-3.1.2/alive_progress.egg-info/
--rw-r--r--   0 rogerio    (501) staff       (20)    75898 2023-05-09 01:09:06.000000 alive-progress-3.1.2/alive_progress.egg-info/PKG-INFO
--rw-r--r--   0 rogerio    (501) staff       (20)     1223 2023-05-09 01:09:06.000000 alive-progress-3.1.2/alive_progress.egg-info/SOURCES.txt
--rw-r--r--   0 rogerio    (501) staff       (20)        1 2023-05-09 01:09:06.000000 alive-progress-3.1.2/alive_progress.egg-info/dependency_links.txt
--rw-r--r--   0 rogerio    (501) staff       (20)       34 2023-05-09 01:09:06.000000 alive-progress-3.1.2/alive_progress.egg-info/requires.txt
--rw-r--r--   0 rogerio    (501) staff       (20)       15 2023-05-09 01:09:06.000000 alive-progress-3.1.2/alive_progress.egg-info/top_level.txt
--rw-r--r--   0 rogerio    (501) staff       (20)       38 2023-05-09 01:09:06.000000 alive-progress-3.1.2/setup.cfg
--rw-r--r--   0 rogerio    (501) staff       (20)     2306 2022-12-22 05:23:53.000000 alive-progress-3.1.2/setup.py
+drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-05-26 03:44:59.000000 alive-progress-3.1.3/
+-rw-r--r--   0 rogerio    (501) staff       (20)     1084 2019-08-05 05:55:53.000000 alive-progress-3.1.3/LICENSE
+-rw-r--r--   0 rogerio    (501) staff       (20)    75919 2023-05-26 03:44:59.000000 alive-progress-3.1.3/PKG-INFO
+-rw-r--r--   0 rogerio    (501) staff       (20)    67113 2023-05-26 03:41:18.000000 alive-progress-3.1.3/README.md
+drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-05-26 03:44:59.000000 alive-progress-3.1.3/alive_progress/
+-rw-r--r--   0 rogerio    (501) staff       (20)      417 2023-05-26 03:40:31.000000 alive-progress-3.1.3/alive_progress/__init__.py
+drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-05-26 03:44:59.000000 alive-progress-3.1.3/alive_progress/animations/
+-rw-r--r--   0 rogerio    (501) staff       (20)      481 2021-08-26 23:38:44.000000 alive-progress-3.1.3/alive_progress/animations/__init__.py
+-rw-r--r--   0 rogerio    (501) staff       (20)     9721 2023-03-24 02:50:30.000000 alive-progress-3.1.3/alive_progress/animations/bars.py
+-rw-r--r--   0 rogerio    (501) staff       (20)    13834 2023-03-24 02:50:30.000000 alive-progress-3.1.3/alive_progress/animations/spinner_compiler.py
+-rw-r--r--   0 rogerio    (501) staff       (20)    11443 2023-03-24 02:50:30.000000 alive-progress-3.1.3/alive_progress/animations/spinners.py
+-rw-r--r--   0 rogerio    (501) staff       (20)     4723 2021-08-26 23:38:44.000000 alive-progress-3.1.3/alive_progress/animations/utils.py
+drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-05-26 03:44:59.000000 alive-progress-3.1.3/alive_progress/core/
+-rw-r--r--   0 rogerio    (501) staff       (20)        0 2020-07-28 14:16:28.000000 alive-progress-3.1.3/alive_progress/core/__init__.py
+-rw-r--r--   0 rogerio    (501) staff       (20)     1351 2022-02-02 06:03:46.000000 alive-progress-3.1.3/alive_progress/core/calibration.py
+-rw-r--r--   0 rogerio    (501) staff       (20)     8876 2023-03-24 02:50:30.000000 alive-progress-3.1.3/alive_progress/core/configuration.py
+-rw-r--r--   0 rogerio    (501) staff       (20)     5627 2023-05-26 03:43:17.000000 alive-progress-3.1.3/alive_progress/core/hook_manager.py
+-rw-r--r--   0 rogerio    (501) staff       (20)    23674 2023-05-26 03:42:11.000000 alive-progress-3.1.3/alive_progress/core/progress.py
+drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-05-26 03:44:59.000000 alive-progress-3.1.3/alive_progress/styles/
+-rw-r--r--   0 rogerio    (501) staff       (20)      614 2021-08-26 23:38:44.000000 alive-progress-3.1.3/alive_progress/styles/__init__.py
+-rw-r--r--   0 rogerio    (501) staff       (20)    11233 2023-03-24 02:50:30.000000 alive-progress-3.1.3/alive_progress/styles/exhibit.py
+-rw-r--r--   0 rogerio    (501) staff       (20)     8454 2023-03-24 02:50:30.000000 alive-progress-3.1.3/alive_progress/styles/internal.py
+drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-05-26 03:44:59.000000 alive-progress-3.1.3/alive_progress/tools/
+-rw-r--r--   0 rogerio    (501) staff       (20)       58 2021-08-26 23:38:44.000000 alive-progress-3.1.3/alive_progress/tools/__init__.py
+-rw-r--r--   0 rogerio    (501) staff       (20)     3002 2022-03-22 04:49:57.000000 alive-progress-3.1.3/alive_progress/tools/demo.py
+-rw-r--r--   0 rogerio    (501) staff       (20)     1024 2021-08-26 23:38:44.000000 alive-progress-3.1.3/alive_progress/tools/repl.py
+-rw-r--r--   0 rogerio    (501) staff       (20)     2717 2022-12-22 05:23:53.000000 alive-progress-3.1.3/alive_progress/tools/sampling.py
+-rw-r--r--   0 rogerio    (501) staff       (20)     6634 2021-08-26 23:38:44.000000 alive-progress-3.1.3/alive_progress/tools/unicode_breaks.py
+-rw-r--r--   0 rogerio    (501) staff       (20)      399 2021-08-26 23:38:44.000000 alive-progress-3.1.3/alive_progress/tools/utils.py
+drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-05-26 03:44:59.000000 alive-progress-3.1.3/alive_progress/utils/
+-rw-r--r--   0 rogerio    (501) staff       (20)        0 2022-10-31 01:30:29.000000 alive-progress-3.1.3/alive_progress/utils/__init__.py
+-rw-r--r--   0 rogerio    (501) staff       (20)     8811 2022-12-22 05:23:53.000000 alive-progress-3.1.3/alive_progress/utils/cells.py
+-rw-r--r--   0 rogerio    (501) staff       (20)     2308 2022-02-11 05:29:12.000000 alive-progress-3.1.3/alive_progress/utils/colors.py
+drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-05-26 03:44:59.000000 alive-progress-3.1.3/alive_progress/utils/terminal/
+-rw-r--r--   0 rogerio    (501) staff       (20)     2100 2023-03-24 02:50:30.000000 alive-progress-3.1.3/alive_progress/utils/terminal/__init__.py
+-rw-r--r--   0 rogerio    (501) staff       (20)      747 2023-03-24 02:50:30.000000 alive-progress-3.1.3/alive_progress/utils/terminal/jupyter.py
+-rw-r--r--   0 rogerio    (501) staff       (20)      418 2022-12-22 05:23:53.000000 alive-progress-3.1.3/alive_progress/utils/terminal/non_tty.py
+-rw-r--r--   0 rogerio    (501) staff       (20)     1284 2023-03-24 02:50:30.000000 alive-progress-3.1.3/alive_progress/utils/terminal/tty.py
+-rw-r--r--   0 rogerio    (501) staff       (20)      550 2023-03-24 02:50:30.000000 alive-progress-3.1.3/alive_progress/utils/terminal/void.py
+-rw-r--r--   0 rogerio    (501) staff       (20)     1411 2022-12-22 05:23:53.000000 alive-progress-3.1.3/alive_progress/utils/timing.py
+drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-05-26 03:44:59.000000 alive-progress-3.1.3/alive_progress.egg-info/
+-rw-r--r--   0 rogerio    (501) staff       (20)    75919 2023-05-26 03:44:59.000000 alive-progress-3.1.3/alive_progress.egg-info/PKG-INFO
+-rw-r--r--   0 rogerio    (501) staff       (20)     1223 2023-05-26 03:44:59.000000 alive-progress-3.1.3/alive_progress.egg-info/SOURCES.txt
+-rw-r--r--   0 rogerio    (501) staff       (20)        1 2023-05-26 03:44:59.000000 alive-progress-3.1.3/alive_progress.egg-info/dependency_links.txt
+-rw-r--r--   0 rogerio    (501) staff       (20)       34 2023-05-26 03:44:59.000000 alive-progress-3.1.3/alive_progress.egg-info/requires.txt
+-rw-r--r--   0 rogerio    (501) staff       (20)       15 2023-05-26 03:44:59.000000 alive-progress-3.1.3/alive_progress.egg-info/top_level.txt
+-rw-r--r--   0 rogerio    (501) staff       (20)       38 2023-05-26 03:44:59.000000 alive-progress-3.1.3/setup.cfg
+-rw-r--r--   0 rogerio    (501) staff       (20)     2306 2022-12-22 05:23:53.000000 alive-progress-3.1.3/setup.py
```

### Comparing `alive-progress-3.1.2/LICENSE` & `alive-progress-3.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.2/PKG-INFO` & `alive-progress-3.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alive-progress
-Version: 3.1.2
+Version: 3.1.3
 Summary: A new kind of Progress Bar, with real-time throughput, ETA, and very cool animations!
 Home-page: https://github.com/rsalmei/alive-progress
 Author: Rogério Sampaio de Almeida
 Author-email: rsalmei@gmail.com
 License: MIT
 Description: [<img align="right" src="https://cdn.buymeacoffee.com/buttons/default-orange.png" width="217px" height="51x">](https://www.buymeacoffee.com/rsalmei)
         [<img align="right" alt="Donate with PayPal button" src="https://www.paypalobjects.com/en_US/i/btn/btn_donate_LG.gif">](https://www.paypal.com/donate?business=6SWSHEB5ZNS5N&no_recurring=0&item_name=I%27m+the+author+of+alive-progress%2C+clearly+and+about-time.+Thank+you+for+appreciating+my+work%21&currency_code=USD)
@@ -12,17 +12,16 @@
         ![alive-progress logo](https://raw.githubusercontent.com/rsalmei/alive-progress/main/img/alive-logo.gif)
         
         # alive-progress
         
         [![Maintenance](https://img.shields.io/badge/maintained-yes-brightgreen.svg)](https://gitHub.com/rsalmei/alive-progress/graphs/commit-activity)
         [![PyPI version](https://img.shields.io/pypi/v/alive-progress.svg)](https://pypi.python.org/pypi/alive-progress/)
         [![PyPI pyversions](https://img.shields.io/pypi/pyversions/alive-progress.svg)](https://pypi.python.org/pypi/alive-progress/)
-        [![Downloads](https://static.pepy.tech/personalized-badge/alive-progress?period=week&units=international_system&left_color=grey&right_color=orange&left_text=downloads/week)](https://pepy.tech/project/alive-progress)
-        [![Downloads](https://static.pepy.tech/personalized-badge/alive-progress?period=month&units=international_system&left_color=grey&right_color=orange&left_text=/month)](https://pepy.tech/project/alive-progress)
-        [![Downloads](https://static.pepy.tech/personalized-badge/alive-progress?period=total&units=international_system&left_color=grey&right_color=orange&left_text=total)](https://pepy.tech/project/alive-progress)
+        [![Downloads](https://static.pepy.tech/personalized-badge/alive-progress?period=month&units=international_system&left_color=grey&right_color=orange&left_text=downloads/month)](https://pepy.tech/project/alive-progress)
+        [![Downloads](https://static.pepy.tech/personalized-badge/alive-progress?period=total&units=international_system&left_color=grey&right_color=orange&left_text=downloads)](https://pepy.tech/project/alive-progress)
         ![GitHub Sponsors](https://img.shields.io/github/sponsors/rsalmei)
         
         
         Have you ever wondered where your lengthy processing was at, and when would it finish? Do you usually hit `RETURN` several times to make sure it didn't crash, or the SSH connection didn't freeze? Have you ever thought it'd be awesome to be able to _pause some processing_ without hassle, return to the Python prompt to manually fix some items, then _seamlessly resume_ it? I did...
         
         I've started this new progress bar thinking about all that, behold the **alive-progress**! 😃
         
@@ -897,15 +896,17 @@
         </details>
         
         <details>
         <summary>Changelog highlights</summary>
         
         <br>Complete [here](https://github.com/rsalmei/alive-progress/blob/main/CHANGELOG.md).
         
-        - 3.1.1: print hook support for ANSI Escape Codes, typing support in `alive_it`
+        - 3.1.3: better error handling of invalid alive_it calls, better error message when detecting nested uses of alive_progress
+        - 3.1.2: fix some exotic ANSI Escape Codes not being printed (OSC)
+        - 3.1.1: support for printing ANSI Escape Codes like set console title, typing annotations in `alive_it`
         - 3.1.0: new resuming computations support with `skipped` items, new `max_cols` config setting for jupyter, fix fetching the size of the terminal when using stderr, officially supports Python 3.11
         - 3.0.1: fix for logging streams that extend StreamHandler but doesn't allow changing streams
         - 3.0.0: units support with automatic and configurable scaling and precision, automatic stats scaling for slow throughputs, support for using `sys.stderr` and other files instead of `sys.stdout`, smoothed out the rate estimation, more queries into the currently running widgets' data, help system in configuration errors
         - 2.4.1: fix a crash when dual-line and disabled are set
         - 2.4.0: support dual line text mode; finalize function parameter in alive_it; improve logging support, detecting customized ones
         - 2.3.1: introduce ctrl_c config param; print the final receipt even when interrupted
         - 2.3.0: customizable `monitor`, `elapsed`, and `stats` core widgets, new `monitor_end`, `elapsed_end`, and `stats_end` core widgets, better support for CTRL+C, which makes `alive_bar` stop prematurely
```

### Comparing `alive-progress-3.1.2/README.md` & `alive-progress-3.1.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 ![alive-progress logo](https://raw.githubusercontent.com/rsalmei/alive-progress/main/img/alive-logo.gif)
 
 # alive-progress
 
 [![Maintenance](https://img.shields.io/badge/maintained-yes-brightgreen.svg)](https://gitHub.com/rsalmei/alive-progress/graphs/commit-activity)
 [![PyPI version](https://img.shields.io/pypi/v/alive-progress.svg)](https://pypi.python.org/pypi/alive-progress/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/alive-progress.svg)](https://pypi.python.org/pypi/alive-progress/)
-[![Downloads](https://static.pepy.tech/personalized-badge/alive-progress?period=week&units=international_system&left_color=grey&right_color=orange&left_text=downloads/week)](https://pepy.tech/project/alive-progress)
-[![Downloads](https://static.pepy.tech/personalized-badge/alive-progress?period=month&units=international_system&left_color=grey&right_color=orange&left_text=/month)](https://pepy.tech/project/alive-progress)
-[![Downloads](https://static.pepy.tech/personalized-badge/alive-progress?period=total&units=international_system&left_color=grey&right_color=orange&left_text=total)](https://pepy.tech/project/alive-progress)
+[![Downloads](https://static.pepy.tech/personalized-badge/alive-progress?period=month&units=international_system&left_color=grey&right_color=orange&left_text=downloads/month)](https://pepy.tech/project/alive-progress)
+[![Downloads](https://static.pepy.tech/personalized-badge/alive-progress?period=total&units=international_system&left_color=grey&right_color=orange&left_text=downloads)](https://pepy.tech/project/alive-progress)
 ![GitHub Sponsors](https://img.shields.io/github/sponsors/rsalmei)
 
 
 Have you ever wondered where your lengthy processing was at, and when would it finish? Do you usually hit `RETURN` several times to make sure it didn't crash, or the SSH connection didn't freeze? Have you ever thought it'd be awesome to be able to _pause some processing_ without hassle, return to the Python prompt to manually fix some items, then _seamlessly resume_ it? I did...
 
 I've started this new progress bar thinking about all that, behold the **alive-progress**! 😃
 
@@ -889,15 +888,17 @@
 </details>
 
 <details>
 <summary>Changelog highlights</summary>
 
 <br>Complete [here](https://github.com/rsalmei/alive-progress/blob/main/CHANGELOG.md).
 
-- 3.1.1: print hook support for ANSI Escape Codes, typing support in `alive_it`
+- 3.1.3: better error handling of invalid alive_it calls, better error message when detecting nested uses of alive_progress
+- 3.1.2: fix some exotic ANSI Escape Codes not being printed (OSC)
+- 3.1.1: support for printing ANSI Escape Codes like set console title, typing annotations in `alive_it`
 - 3.1.0: new resuming computations support with `skipped` items, new `max_cols` config setting for jupyter, fix fetching the size of the terminal when using stderr, officially supports Python 3.11
 - 3.0.1: fix for logging streams that extend StreamHandler but doesn't allow changing streams
 - 3.0.0: units support with automatic and configurable scaling and precision, automatic stats scaling for slow throughputs, support for using `sys.stderr` and other files instead of `sys.stdout`, smoothed out the rate estimation, more queries into the currently running widgets' data, help system in configuration errors
 - 2.4.1: fix a crash when dual-line and disabled are set
 - 2.4.0: support dual line text mode; finalize function parameter in alive_it; improve logging support, detecting customized ones
 - 2.3.1: introduce ctrl_c config param; print the final receipt even when interrupted
 - 2.3.0: customizable `monitor`, `elapsed`, and `stats` core widgets, new `monitor_end`, `elapsed_end`, and `stats_end` core widgets, better support for CTRL+C, which makes `alive_bar` stop prematurely
```

### Comparing `alive-progress-3.1.2/alive_progress/animations/bars.py` & `alive-progress-3.1.3/alive_progress/animations/bars.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.2/alive_progress/animations/spinner_compiler.py` & `alive-progress-3.1.3/alive_progress/animations/spinner_compiler.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.2/alive_progress/animations/spinners.py` & `alive-progress-3.1.3/alive_progress/animations/spinners.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.2/alive_progress/animations/utils.py` & `alive-progress-3.1.3/alive_progress/animations/utils.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.2/alive_progress/core/calibration.py` & `alive-progress-3.1.3/alive_progress/core/calibration.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.2/alive_progress/core/configuration.py` & `alive-progress-3.1.3/alive_progress/core/configuration.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.2/alive_progress/core/hook_manager.py` & `alive-progress-3.1.3/alive_progress/core/hook_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,26 +66,20 @@
                     term.clear_end_screen()
                 stream.write(text)
                 stream.flush()
                 cond_refresh.notify()
                 buffer[:] = []
 
     # better hook impl, which works even when nested, since __hash__ will be forwarded.
-    class Hook:
-        def __init__(self, stream):
-            self.__stream = stream
-
+    class Hook(BaseHook):
         def write(self, part):
-            return write(self.__stream, part)
+            return write(self._stream, part)
 
         def flush(self):
-            return flush(self.__stream)
-
-        def __getattr__(self, item):
-            return getattr(self.__stream, item)
+            return flush(self._stream)
 
     def get_hook_for(handler):
         if handler.stream:  # supports FileHandlers with delay=true.
             handler.stream.flush()
         return Hook(handler.stream)
 
     def install():
@@ -116,14 +110,17 @@
 
         # did the number of logging handlers change??
         # if yes, it probably means logging was initialized within alive_bar context,
         # and thus there can be an instrumented stdout or stderr within handlers,
         # which causes a TypeError: unhashable type: 'types.SimpleNamespace'...
         # or simply a logger **reuses** a handler...
 
+    if issubclass(sys.stdout.__class__, BaseHook):
+        raise UserWarning('Nested use of alive_progress is not yet supported.')
+
     # internal data.
     buffers = defaultdict(list)
     get_header = gen_header(header_template, get_pos) if header_template else null_header
     base = sys.stdout, sys.stderr  # needed for tests.
     before_handlers = {}
 
     # external interface.
@@ -132,14 +129,22 @@
         install=install,
         uninstall=uninstall,
     )
 
     return hook_manager
 
 
+class BaseHook:
+    def __init__(self, stream):
+        self._stream = stream
+
+    def __getattr__(self, item):
+        return getattr(self._stream, item)
+
+
 def passthrough_hook_manager():  # pragma: no cover
     passthrough_hook_manager.flush_buffers = __noop
     passthrough_hook_manager.install = __noop
     passthrough_hook_manager.uninstall = __noop
     return passthrough_hook_manager
```

### Comparing `alive-progress-3.1.2/alive_progress/core/progress.py` & `alive-progress-3.1.3/alive_progress/core/progress.py`

 * *Files 2% similar despite different names*

```diff
@@ -565,18 +565,20 @@
             for item in self._it:
                 yield item
                 self._bar()
             if self._finalize:
                 self._finalize(self._bar)
 
     def __call__(self, *args, **kwargs):
-        raise UserWarning('The bar position is controlled automatically with `alive_it`.')
+        raise UserWarning('The bar position is controlled automatically by `alive_it`.')
 
     def __getattr__(self, item):
         # makes this adapter work as the real bar.
-        return getattr(self._bar, item)
+        if '_bar' in self.__dict__: # detects not yet started bar instances.
+            return getattr(self._bar, item)
+        raise UserWarning('Configure this bar either via `alive_it()` or after iterating it.')
 
     def __setattr__(self, key, value):
         # makes this adapter work as the real bar.
         if '_bar' in self.__dict__:
             return setattr(self._bar, key, value)
         return super().__setattr__(key, value)
```

### Comparing `alive-progress-3.1.2/alive_progress/styles/__init__.py` & `alive-progress-3.1.3/alive_progress/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.2/alive_progress/styles/exhibit.py` & `alive-progress-3.1.3/alive_progress/styles/exhibit.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.2/alive_progress/styles/internal.py` & `alive-progress-3.1.3/alive_progress/styles/internal.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.2/alive_progress/tools/demo.py` & `alive-progress-3.1.3/alive_progress/tools/demo.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.2/alive_progress/tools/repl.py` & `alive-progress-3.1.3/alive_progress/tools/repl.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.2/alive_progress/tools/sampling.py` & `alive-progress-3.1.3/alive_progress/tools/sampling.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.2/alive_progress/tools/unicode_breaks.py` & `alive-progress-3.1.3/alive_progress/tools/unicode_breaks.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.2/alive_progress/utils/cells.py` & `alive-progress-3.1.3/alive_progress/utils/cells.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.2/alive_progress/utils/colors.py` & `alive-progress-3.1.3/alive_progress/utils/colors.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.2/alive_progress/utils/terminal/__init__.py` & `alive-progress-3.1.3/alive_progress/utils/terminal/__init__.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.2/alive_progress/utils/terminal/jupyter.py` & `alive-progress-3.1.3/alive_progress/utils/terminal/jupyter.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.2/alive_progress/utils/terminal/tty.py` & `alive-progress-3.1.3/alive_progress/utils/terminal/tty.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.2/alive_progress/utils/terminal/void.py` & `alive-progress-3.1.3/alive_progress/utils/terminal/void.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.2/alive_progress/utils/timing.py` & `alive-progress-3.1.3/alive_progress/utils/timing.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.2/alive_progress.egg-info/PKG-INFO` & `alive-progress-3.1.3/alive_progress.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alive-progress
-Version: 3.1.2
+Version: 3.1.3
 Summary: A new kind of Progress Bar, with real-time throughput, ETA, and very cool animations!
 Home-page: https://github.com/rsalmei/alive-progress
 Author: Rogério Sampaio de Almeida
 Author-email: rsalmei@gmail.com
 License: MIT
 Description: [<img align="right" src="https://cdn.buymeacoffee.com/buttons/default-orange.png" width="217px" height="51x">](https://www.buymeacoffee.com/rsalmei)
         [<img align="right" alt="Donate with PayPal button" src="https://www.paypalobjects.com/en_US/i/btn/btn_donate_LG.gif">](https://www.paypal.com/donate?business=6SWSHEB5ZNS5N&no_recurring=0&item_name=I%27m+the+author+of+alive-progress%2C+clearly+and+about-time.+Thank+you+for+appreciating+my+work%21&currency_code=USD)
@@ -12,17 +12,16 @@
         ![alive-progress logo](https://raw.githubusercontent.com/rsalmei/alive-progress/main/img/alive-logo.gif)
         
         # alive-progress
         
         [![Maintenance](https://img.shields.io/badge/maintained-yes-brightgreen.svg)](https://gitHub.com/rsalmei/alive-progress/graphs/commit-activity)
         [![PyPI version](https://img.shields.io/pypi/v/alive-progress.svg)](https://pypi.python.org/pypi/alive-progress/)
         [![PyPI pyversions](https://img.shields.io/pypi/pyversions/alive-progress.svg)](https://pypi.python.org/pypi/alive-progress/)
-        [![Downloads](https://static.pepy.tech/personalized-badge/alive-progress?period=week&units=international_system&left_color=grey&right_color=orange&left_text=downloads/week)](https://pepy.tech/project/alive-progress)
-        [![Downloads](https://static.pepy.tech/personalized-badge/alive-progress?period=month&units=international_system&left_color=grey&right_color=orange&left_text=/month)](https://pepy.tech/project/alive-progress)
-        [![Downloads](https://static.pepy.tech/personalized-badge/alive-progress?period=total&units=international_system&left_color=grey&right_color=orange&left_text=total)](https://pepy.tech/project/alive-progress)
+        [![Downloads](https://static.pepy.tech/personalized-badge/alive-progress?period=month&units=international_system&left_color=grey&right_color=orange&left_text=downloads/month)](https://pepy.tech/project/alive-progress)
+        [![Downloads](https://static.pepy.tech/personalized-badge/alive-progress?period=total&units=international_system&left_color=grey&right_color=orange&left_text=downloads)](https://pepy.tech/project/alive-progress)
         ![GitHub Sponsors](https://img.shields.io/github/sponsors/rsalmei)
         
         
         Have you ever wondered where your lengthy processing was at, and when would it finish? Do you usually hit `RETURN` several times to make sure it didn't crash, or the SSH connection didn't freeze? Have you ever thought it'd be awesome to be able to _pause some processing_ without hassle, return to the Python prompt to manually fix some items, then _seamlessly resume_ it? I did...
         
         I've started this new progress bar thinking about all that, behold the **alive-progress**! 😃
         
@@ -897,15 +896,17 @@
         </details>
         
         <details>
         <summary>Changelog highlights</summary>
         
         <br>Complete [here](https://github.com/rsalmei/alive-progress/blob/main/CHANGELOG.md).
         
-        - 3.1.1: print hook support for ANSI Escape Codes, typing support in `alive_it`
+        - 3.1.3: better error handling of invalid alive_it calls, better error message when detecting nested uses of alive_progress
+        - 3.1.2: fix some exotic ANSI Escape Codes not being printed (OSC)
+        - 3.1.1: support for printing ANSI Escape Codes like set console title, typing annotations in `alive_it`
         - 3.1.0: new resuming computations support with `skipped` items, new `max_cols` config setting for jupyter, fix fetching the size of the terminal when using stderr, officially supports Python 3.11
         - 3.0.1: fix for logging streams that extend StreamHandler but doesn't allow changing streams
         - 3.0.0: units support with automatic and configurable scaling and precision, automatic stats scaling for slow throughputs, support for using `sys.stderr` and other files instead of `sys.stdout`, smoothed out the rate estimation, more queries into the currently running widgets' data, help system in configuration errors
         - 2.4.1: fix a crash when dual-line and disabled are set
         - 2.4.0: support dual line text mode; finalize function parameter in alive_it; improve logging support, detecting customized ones
         - 2.3.1: introduce ctrl_c config param; print the final receipt even when interrupted
         - 2.3.0: customizable `monitor`, `elapsed`, and `stats` core widgets, new `monitor_end`, `elapsed_end`, and `stats_end` core widgets, better support for CTRL+C, which makes `alive_bar` stop prematurely
```

### Comparing `alive-progress-3.1.2/alive_progress.egg-info/SOURCES.txt` & `alive-progress-3.1.3/alive_progress.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.2/setup.py` & `alive-progress-3.1.3/setup.py`

 * *Files identical despite different names*

