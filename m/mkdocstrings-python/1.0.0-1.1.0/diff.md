# Comparing `tmp/mkdocstrings_python-1.0.0.tar.gz` & `tmp/mkdocstrings_python-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocstrings_python-1.0.0.tar", last modified: Thu May 11 10:08:32 2023, max compression
+gzip compressed data, was "mkdocstrings_python-1.1.0.tar", last modified: Fri May 26 11:01:50 2023, max compression
```

## Comparing `mkdocstrings_python-1.0.0.tar` & `mkdocstrings_python-1.1.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0      754 2023-05-11 08:57:22.621862 mkdocstrings_python-1.0.0/LICENSE
--rw-r--r--   0        0        0     4243 2023-05-11 08:57:25.185137 mkdocstrings_python-1.0.0/README.md
--rw-r--r--   0        0        0     2606 2023-05-11 10:08:32.951065 mkdocstrings_python-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-11 08:57:22.365201 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/py.typed
--rw-r--r--   0        0        0      326 2023-05-01 15:54:09.233042 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/__init__.py
--rw-r--r--   0        0        0    17985 2023-05-11 09:46:36.018635 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/handler.py
--rw-r--r--   0        0        0     7542 2023-05-11 09:40:34.155577 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/rendering.py
--rw-r--r--   0        0        0     2532 2022-04-29 13:33:38.953329 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/attribute.html
--rw-r--r--   0        0        0     5053 2023-05-01 15:54:09.233042 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/children.html
--rw-r--r--   0        0        0     4078 2023-05-11 09:36:36.899109 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/class.html
--rw-r--r--   0        0        0     1740 2023-03-03 13:20:57.896481 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring.html
--rw-r--r--   0        0        0      274 2023-05-01 15:54:09.233042 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/admonition.html
--rw-r--r--   0        0        0     2465 2022-04-29 23:09:02.903315 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/attributes.html
--rw-r--r--   0        0        0      400 2022-03-01 18:29:05.585970 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/examples.html
--rw-r--r--   0        0        0     2475 2022-04-29 23:09:07.859915 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/other_parameters.html
--rw-r--r--   0        0        0     3134 2022-04-29 23:09:10.543213 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/parameters.html
--rw-r--r--   0        0        0     2132 2022-04-29 23:09:12.233190 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/raises.html
--rw-r--r--   0        0        0     3111 2022-04-29 23:09:14.279830 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/receives.html
--rw-r--r--   0        0        0     3081 2022-04-29 23:09:16.163138 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/returns.html
--rw-r--r--   0        0        0     2115 2022-04-29 23:09:18.059779 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/warns.html
--rw-r--r--   0        0        0     3051 2022-04-29 23:09:20.759743 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/yields.html
--rw-r--r--   0        0        0      674 2023-05-11 09:36:36.899109 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/expression.html
--rw-r--r--   0        0        0     2436 2023-05-11 09:36:36.899109 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/function.html
--rw-r--r--   0        0        0      245 2022-05-08 08:40:49.298304 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/labels.html
--rw-r--r--   0        0        0     1852 2022-04-29 17:36:56.831573 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/module.html
--rw-r--r--   0        0        0     2698 2023-05-11 09:36:36.899109 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/signature.html
--rw-r--r--   0        0        0       37 2021-11-03 19:53:40.146116 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/attribute.html
--rw-r--r--   0        0        0       36 2021-11-03 19:53:40.146116 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/children.html
--rw-r--r--   0        0        0       33 2021-11-03 19:53:40.146116 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/class.html
--rw-r--r--   0        0        0       37 2021-11-03 19:53:40.146116 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/docstring.html
--rw-r--r--   0        0        0       48 2022-02-01 20:48:46.512716 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/docstring/admonition.html
--rw-r--r--   0        0        0       48 2021-11-03 19:54:24.832142 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/docstring/attributes.html
--rw-r--r--   0        0        0       46 2021-11-03 19:54:24.832142 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/docstring/examples.html
--rw-r--r--   0        0        0       54 2021-11-03 19:54:24.832142 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/docstring/other_parameters.html
--rw-r--r--   0        0        0       48 2021-11-03 19:54:24.832142 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/docstring/parameters.html
--rw-r--r--   0        0        0       44 2021-11-22 18:41:47.281610 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/docstring/raises.html
--rw-r--r--   0        0        0       46 2021-11-22 18:41:51.551545 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/docstring/receives.html
--rw-r--r--   0        0        0       45 2021-11-03 19:54:24.832142 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/docstring/returns.html
--rw-r--r--   0        0        0       43 2021-11-22 18:41:56.598136 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/docstring/warns.html
--rw-r--r--   0        0        0       44 2021-11-03 19:54:24.832142 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/docstring/yields.html
--rw-r--r--   0        0        0       38 2021-11-08 00:26:56.388000 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/expression.html
--rw-r--r--   0        0        0       36 2021-11-03 19:53:40.146116 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/function.html
--rw-r--r--   0        0        0       34 2021-11-03 19:53:40.146116 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/labels.html
--rw-r--r--   0        0        0       34 2021-11-03 19:53:40.146116 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/module.html
--rw-r--r--   0        0        0       37 2021-11-03 19:53:40.146116 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/signature.html
--rw-r--r--   0        0        0      703 2022-03-03 18:21:59.514950 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/style.css
--rw-r--r--   0        0        0      224 2021-10-30 13:54:10.019274 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/mkdocs/exceptions.html
--rw-r--r--   0        0        0      277 2021-10-30 13:54:10.202605 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/mkdocs/keyword_args.html
--rw-r--r--   0        0        0      293 2021-10-30 13:54:10.019274 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/mkdocs/parameters.html
--rw-r--r--   0        0        0      200 2021-10-30 13:54:10.092606 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/mkdocs/return.html
--rw-r--r--   0        0        0      137 2021-10-30 13:54:10.199272 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/mkdocs/style.css
--rw-r--r--   0        0        0      196 2021-10-30 13:54:10.202605 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/mkdocs/yield.html
--rw-r--r--   0        0        0      545 2021-10-30 13:54:09.842609 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/readthedocs/exceptions.html
--rw-r--r--   0        0        0      601 2021-11-06 17:58:09.459000 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/readthedocs/other_parameters.html
--rw-r--r--   0        0        0      618 2021-11-06 17:59:12.206399 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/readthedocs/parameters.html
--rw-r--r--   0        0        0      494 2021-11-06 17:58:14.115000 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/readthedocs/returns.html
--rw-r--r--   0        0        0      600 2021-10-30 13:54:09.942608 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/readthedocs/style.css
--rw-r--r--   0        0        0      490 2021-11-06 17:58:20.568000 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/readthedocs/yields.html
--rw-r--r--   0        0        0      174 2023-05-11 08:57:22.358534 mkdocstrings_python-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0     3042 2023-05-11 08:57:25.185137 mkdocstrings_python-1.0.0/tests/conftest.py
--rw-r--r--   0        0        0     3222 2023-05-01 15:54:09.233042 mkdocstrings_python-1.0.0/tests/test_handler.py
--rw-r--r--   0        0        0     1975 2023-05-11 09:36:36.899109 mkdocstrings_python-1.0.0/tests/test_rendering.py
--rw-r--r--   0        0        0     1332 2023-05-01 15:54:09.233042 mkdocstrings_python-1.0.0/tests/test_themes.py
--rw-r--r--   0        0        0     5749 1970-01-01 00:00:00.000000 mkdocstrings_python-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      754 2023-05-16 10:40:20.986168 mkdocstrings_python-1.1.0/LICENSE
+-rw-r--r--   0        0        0     4243 2023-05-16 10:41:07.688645 mkdocstrings_python-1.1.0/README.md
+-rw-r--r--   0        0        0     2604 2023-05-26 11:01:50.845735 mkdocstrings_python-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-16 10:40:20.579508 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/py.typed
+-rw-r--r--   0        0        0      326 2023-05-01 15:54:09.233042 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/__init__.py
+-rw-r--r--   0        0        0    18098 2023-05-25 09:39:58.824275 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/handler.py
+-rw-r--r--   0        0        0     7871 2023-05-25 09:39:58.824275 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/rendering.py
+-rw-r--r--   0        0        0     2532 2022-04-29 13:33:38.953329 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/attribute.html
+-rw-r--r--   0        0        0     5036 2023-05-25 09:39:58.824275 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/children.html
+-rw-r--r--   0        0        0     4078 2023-05-11 09:36:36.899109 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/class.html
+-rw-r--r--   0        0        0     1740 2023-03-03 13:20:57.896481 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring.html
+-rw-r--r--   0        0        0      274 2023-05-01 15:54:09.233042 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/admonition.html
+-rw-r--r--   0        0        0     2465 2022-04-29 23:09:02.903315 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/attributes.html
+-rw-r--r--   0        0        0      400 2022-03-01 18:29:05.585970 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/examples.html
+-rw-r--r--   0        0        0     2475 2022-04-29 23:09:07.859915 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/other_parameters.html
+-rw-r--r--   0        0        0     3134 2022-04-29 23:09:10.543213 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/parameters.html
+-rw-r--r--   0        0        0     2132 2022-04-29 23:09:12.233190 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/raises.html
+-rw-r--r--   0        0        0     3111 2022-04-29 23:09:14.279830 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/receives.html
+-rw-r--r--   0        0        0     3081 2022-04-29 23:09:16.163138 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/returns.html
+-rw-r--r--   0        0        0     2115 2022-04-29 23:09:18.059779 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/warns.html
+-rw-r--r--   0        0        0     3051 2022-04-29 23:09:20.759743 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/yields.html
+-rw-r--r--   0        0        0      674 2023-05-11 09:36:36.899109 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/expression.html
+-rw-r--r--   0        0        0     2436 2023-05-11 09:36:36.899109 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/function.html
+-rw-r--r--   0        0        0      245 2022-05-08 08:40:49.298304 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/labels.html
+-rw-r--r--   0        0        0     1852 2022-04-29 17:36:56.831573 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/module.html
+-rw-r--r--   0        0        0     2698 2023-05-11 09:36:36.899109 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/signature.html
+-rw-r--r--   0        0        0       37 2021-11-03 19:53:40.146116 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/attribute.html
+-rw-r--r--   0        0        0       36 2021-11-03 19:53:40.146116 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/children.html
+-rw-r--r--   0        0        0       33 2021-11-03 19:53:40.146116 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/class.html
+-rw-r--r--   0        0        0       37 2021-11-03 19:53:40.146116 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/docstring.html
+-rw-r--r--   0        0        0       48 2022-02-01 20:48:46.512716 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/docstring/admonition.html
+-rw-r--r--   0        0        0       48 2021-11-03 19:54:24.832142 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/docstring/attributes.html
+-rw-r--r--   0        0        0       46 2021-11-03 19:54:24.832142 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/docstring/examples.html
+-rw-r--r--   0        0        0       54 2021-11-03 19:54:24.832142 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/docstring/other_parameters.html
+-rw-r--r--   0        0        0       48 2021-11-03 19:54:24.832142 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/docstring/parameters.html
+-rw-r--r--   0        0        0       44 2021-11-22 18:41:47.281610 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/docstring/raises.html
+-rw-r--r--   0        0        0       46 2021-11-22 18:41:51.551545 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/docstring/receives.html
+-rw-r--r--   0        0        0       45 2021-11-03 19:54:24.832142 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/docstring/returns.html
+-rw-r--r--   0        0        0       43 2021-11-22 18:41:56.598136 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/docstring/warns.html
+-rw-r--r--   0        0        0       44 2021-11-03 19:54:24.832142 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/docstring/yields.html
+-rw-r--r--   0        0        0       38 2021-11-08 00:26:56.388000 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/expression.html
+-rw-r--r--   0        0        0       36 2021-11-03 19:53:40.146116 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/function.html
+-rw-r--r--   0        0        0       34 2021-11-03 19:53:40.146116 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/labels.html
+-rw-r--r--   0        0        0       34 2021-11-03 19:53:40.146116 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/module.html
+-rw-r--r--   0        0        0       37 2021-11-03 19:53:40.146116 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/signature.html
+-rw-r--r--   0        0        0      703 2022-03-03 18:21:59.514950 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/style.css
+-rw-r--r--   0        0        0      224 2021-10-30 13:54:10.019274 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/mkdocs/exceptions.html
+-rw-r--r--   0        0        0      277 2021-10-30 13:54:10.202605 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/mkdocs/keyword_args.html
+-rw-r--r--   0        0        0      293 2021-10-30 13:54:10.019274 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/mkdocs/parameters.html
+-rw-r--r--   0        0        0      200 2021-10-30 13:54:10.092606 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/mkdocs/return.html
+-rw-r--r--   0        0        0      137 2021-10-30 13:54:10.199272 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/mkdocs/style.css
+-rw-r--r--   0        0        0      196 2021-10-30 13:54:10.202605 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/mkdocs/yield.html
+-rw-r--r--   0        0        0      545 2021-10-30 13:54:09.842609 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/readthedocs/exceptions.html
+-rw-r--r--   0        0        0      601 2021-11-06 17:58:09.459000 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/readthedocs/other_parameters.html
+-rw-r--r--   0        0        0      618 2021-11-06 17:59:12.206399 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/readthedocs/parameters.html
+-rw-r--r--   0        0        0      494 2021-11-06 17:58:14.115000 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/readthedocs/returns.html
+-rw-r--r--   0        0        0      600 2021-10-30 13:54:09.942608 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/readthedocs/style.css
+-rw-r--r--   0        0        0      490 2021-11-06 17:58:20.568000 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/readthedocs/yields.html
+-rw-r--r--   0        0        0      174 2023-05-16 10:40:20.572842 mkdocstrings_python-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     3042 2023-05-16 10:40:23.629451 mkdocstrings_python-1.1.0/tests/conftest.py
+-rw-r--r--   0        0        0     3222 2023-05-01 15:54:09.233042 mkdocstrings_python-1.1.0/tests/test_handler.py
+-rw-r--r--   0        0        0     1975 2023-05-11 09:36:36.899109 mkdocstrings_python-1.1.0/tests/test_rendering.py
+-rw-r--r--   0        0        0     1332 2023-05-01 15:54:09.233042 mkdocstrings_python-1.1.0/tests/test_themes.py
+-rw-r--r--   0        0        0     5747 1970-01-01 00:00:00.000000 mkdocstrings_python-1.1.0/PKG-INFO
```

### Comparing `mkdocstrings_python-1.0.0/LICENSE` & `mkdocstrings_python-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.0.0/README.md` & `mkdocstrings_python-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.0.0/pyproject.toml` & `mkdocstrings_python-1.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -31,28 +31,28 @@
     "Topic :: Utilities",
     "Typing :: Typed",
 ]
 dependencies = [
     "mkdocstrings>=0.20",
     "griffe>=0.24",
 ]
-version = "1.0.0"
+version = "1.1.0"
 
 [project.license]
 text = "ISC"
 
 [project.urls]
 Homepage = "https://mkdocstrings.github.io/python"
 Documentation = "https://mkdocstrings.github.io/python"
 Changelog = "https://mkdocstrings.github.io/python/changelog"
 Repository = "https://github.com/mkdocstrings/python"
 Issues = "https://github.com/mkdocstrings/python/issues"
 Discussions = "https://github.com/mkdocstrings/python/discussions"
-Gitter = "https://gitter.im/python/community"
-Funding = "https://github.com/sponsors/mkdocstrings"
+Gitter = "https://gitter.im/mkdocstrings/python"
+Funding = "https://github.com/sponsors/pawamoy"
 
 [tool.pdm]
 plugins = [
     "pdm-multirun",
 ]
 
 [tool.pdm.version]
```

### Comparing `mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/handler.py` & `mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -293,15 +293,16 @@
         return doc_object
 
     def render(self, data: CollectorItem, config: Mapping[str, Any]) -> str:  # noqa: D102 (ignore missing docstring)
         # See https://github.com/python/typeshed/issues/8430
         mutabled_config = dict(copy.deepcopy(config))
         final_config = ChainMap(mutabled_config, self.default_config)
 
-        template = self.env.get_template(f"{data.kind.value}.html")
+        template_name = rendering.do_get_template(data)
+        template = self.env.get_template(template_name)
 
         # Heading level is a "state" variable, that will change at each step
         # of the rendering recursion. Therefore, it's easier to use it as a plain value
         # than as an item in a dictionary.
         heading_level = final_config["heading_level"]
         try:
             final_config["members_order"] = rendering.Order(final_config["members_order"])
@@ -331,14 +332,15 @@
         self.env.filters["crossref"] = rendering.do_crossref
         self.env.filters["multi_crossref"] = rendering.do_multi_crossref
         self.env.filters["order_members"] = rendering.do_order_members
         self.env.filters["format_code"] = rendering.do_format_code
         self.env.filters["format_signature"] = rendering.do_format_signature
         self.env.filters["filter_objects"] = rendering.do_filter_objects
         self.env.filters["stash_crossref"] = lambda ref, length: ref
+        self.env.filters["get_template"] = rendering.do_get_template
 
     def get_anchors(self, data: CollectorItem) -> set[str]:  # noqa: D102 (ignore missing docstring)
         try:
             return {data.path, data.canonical_path, *data.aliases}
         except AliasResolutionError:
             return {data.path}
```

### Comparing `mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/rendering.py` & `mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/rendering.py`

 * *Files 6% similar despite different names*

```diff
@@ -244,7 +244,20 @@
         return lambda text, _: text
 
     def formatter(code: str, line_length: int) -> str:
         mode = Mode(line_length=line_length)
         return format_str(code, mode=mode)
 
     return formatter
+
+
+def do_get_template(obj: Object) -> str:
+    """Get the template name used to render an object.
+
+    Parameters:
+        obj: A Griffe object.
+
+    Returns:
+        A template name.
+    """
+    extra_data = getattr(obj, "extra", {}).get("mkdocstrings", {})
+    return extra_data.get("template", "") or f"{obj.kind.value}.html"
```

### Comparing `mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/attribute.html` & `mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/attribute.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/children.html` & `mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/children.html`

 * *Files 8% similar despite different names*

```diff
@@ -23,30 +23,30 @@
           {% if attributes %}
             {% if config.show_category_heading %}
               {% filter heading(heading_level, id=html_id ~ "-attributes") %}Attributes{% endfilter %}
             {% endif %}
             {% with heading_level = heading_level + extra_level %}
               {% for attribute in attributes|order_members(config.members_order, members_list) %}
                 {% if not attribute.is_alias or attribute.is_explicitely_exported %}
-                  {% include "attribute.html" with context %}
+                  {% include attribute|get_template with context %}
                 {% endif %}
               {% endfor %}
             {% endwith %}
           {% endif %}
         {% endwith %}
 
         {% with classes = obj.classes|filter_objects(filters=config.filters, members_list=members_list, keep_no_docstrings=config.show_if_no_docstring) %}
           {% if classes %}
             {% if config.show_category_heading %}
               {% filter heading(heading_level, id=html_id ~ "-classes") %}Classes{% endfilter %}
             {% endif %}
             {% with heading_level = heading_level + extra_level %}
               {% for class in classes|order_members(config.members_order, members_list) %}
                 {% if not class.is_alias or class.is_explicitely_exported %}
-                  {% include "class.html" with context %}
+                  {% include class|get_template with context %}
                 {% endif %}
               {% endfor %}
             {% endwith %}
           {% endif %}
         {% endwith %}
 
         {% with functions = obj.functions|filter_objects(filters=config.filters, members_list=members_list, keep_no_docstrings=config.show_if_no_docstring) %}
@@ -54,15 +54,15 @@
             {% if config.show_category_heading %}
               {% filter heading(heading_level, id=html_id ~ "-functions") %}Functions{% endfilter %}
             {% endif %}
             {% with heading_level = heading_level + extra_level %}
               {% for function in functions|order_members(config.members_order, members_list) %}
                 {% if not (obj.kind.value == "class" and function.name == "__init__" and config.merge_init_into_class) %}
                   {% if not function.is_alias or function.is_explicitely_exported %}
-                    {% include "function.html" with context %}
+                    {% include function|get_template with context %}
                   {% endif %}
                 {% endif %}
               {% endfor %}
             {% endwith %}
           {% endif %}
         {% endwith %}
 
@@ -71,15 +71,15 @@
             {% if modules %}
               {% if config.show_category_heading %}
                 {% filter heading(heading_level, id=html_id ~ "-modules") %}Modules{% endfilter %}
               {% endif %}
               {% with heading_level = heading_level + extra_level %}
                 {% for module in modules|order_members(config.members_order, members_list) %}
                   {% if not module.is_alias or module.is_explicitely_exported %}
-                    {% include "module.html" with context %}
+                    {% include module|get_template with context %}
                   {% endif %}
                 {% endfor %}
               {% endwith %}
             {% endif %}
           {% endwith %}
         {% endif %}
 
@@ -87,34 +87,34 @@
 
     {% else %}
 
       {% for child in obj.members|
           filter_objects(filters=config.filters, members_list=members_list, keep_no_docstrings=config.show_if_no_docstring)|
           order_members(config.members_order, members_list) %}
 
-        {% if not (obj.kind.value == "class" and child.name == "__init__" and config.merge_init_into_class) %}
+        {% if not (obj.is_class and child.name == "__init__" and config.merge_init_into_class) %}
 
-          {% if child.kind.value == "attribute" %}
+          {% if child.is_attribute %}
             {% with attribute = child %}
-              {% include "attribute.html" with context %}
+              {% include attribute|get_template with context %}
             {% endwith %}
 
-          {% elif child.kind.value == "class" %}
+          {% elif child.is_class %}
             {% with class = child %}
-              {% include "class.html" with context %}
+              {% include class|get_template with context %}
             {% endwith %}
 
-          {% elif child.kind.value == "function" %}
+          {% elif child.is_function %}
             {% with function = child %}
-              {% include "function.html" with context %}
+              {% include function|get_template with context %}
             {% endwith %}
 
-          {% elif child.kind.value == "module" and config.show_submodules %}
+          {% elif child.is_module and config.show_submodules %}
             {% with module = child %}
-              {% include "module.html" with context %}
+              {% include module|get_template with context %}
             {% endwith %}
 
           {% endif %}
 
         {% endif %}
 
       {% endfor %}
```

### Comparing `mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/class.html` & `mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/class.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring.html` & `mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/attributes.html` & `mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/attributes.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/other_parameters.html` & `mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/other_parameters.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/parameters.html` & `mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/parameters.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/raises.html` & `mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/raises.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/receives.html` & `mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/receives.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/returns.html` & `mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/returns.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/warns.html` & `mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/warns.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/yields.html` & `mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/yields.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/expression.html` & `mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/expression.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/function.html` & `mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/function.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/module.html` & `mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/module.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/signature.html` & `mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/signature.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/style.css` & `mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/style.css`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/readthedocs/exceptions.html` & `mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/readthedocs/exceptions.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/readthedocs/other_parameters.html` & `mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/readthedocs/other_parameters.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/readthedocs/parameters.html` & `mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/readthedocs/parameters.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/readthedocs/style.css` & `mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/readthedocs/style.css`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.0.0/tests/conftest.py` & `mkdocstrings_python-1.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.0.0/tests/test_handler.py` & `mkdocstrings_python-1.1.0/tests/test_handler.py`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.0.0/tests/test_rendering.py` & `mkdocstrings_python-1.1.0/tests/test_rendering.py`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.0.0/tests/test_themes.py` & `mkdocstrings_python-1.1.0/tests/test_themes.py`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.0.0/PKG-INFO` & `mkdocstrings_python-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocstrings-python
-Version: 1.0.0
+Version: 1.1.0
 Summary: A Python handler for mkdocstrings.
 Author-Email: Timothée Mazzucotelli <pawamoy@pm.me>
 License: ISC
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -21,16 +21,16 @@
 Classifier: Typing :: Typed
 Project-URL: Homepage, https://mkdocstrings.github.io/python
 Project-URL: Documentation, https://mkdocstrings.github.io/python
 Project-URL: Changelog, https://mkdocstrings.github.io/python/changelog
 Project-URL: Repository, https://github.com/mkdocstrings/python
 Project-URL: Issues, https://github.com/mkdocstrings/python/issues
 Project-URL: Discussions, https://github.com/mkdocstrings/python/discussions
-Project-URL: Gitter, https://gitter.im/python/community
-Project-URL: Funding, https://github.com/sponsors/mkdocstrings
+Project-URL: Gitter, https://gitter.im/mkdocstrings/python
+Project-URL: Funding, https://github.com/sponsors/pawamoy
 Requires-Python: >=3.7
 Requires-Dist: mkdocstrings>=0.20
 Requires-Dist: griffe>=0.24
 Description-Content-Type: text/markdown
 
 <h1 align="center">mkdocstrings-python</h1>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mkdocstrings-python Version: 1.0.0 Summary: A
+Metadata-Version: 2.1 Name: mkdocstrings-python Version: 1.1.0 Summary: A
 Python handler for mkdocstrings. Author-Email: TimothÃ©e Mazzucotelli
 pm.me> License: ISC Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
@@ -11,16 +11,16 @@
 Software Development :: Documentation Classifier: Topic :: Utilities
 Classifier: Typing :: Typed Project-URL: Homepage, https://
 mkdocstrings.github.io/python Project-URL: Documentation, https://
 mkdocstrings.github.io/python Project-URL: Changelog, https://
 mkdocstrings.github.io/python/changelog Project-URL: Repository, https://
 github.com/mkdocstrings/python Project-URL: Issues, https://github.com/
 mkdocstrings/python/issues Project-URL: Discussions, https://github.com/
-mkdocstrings/python/discussions Project-URL: Gitter, https://gitter.im/python/
-community Project-URL: Funding, https://github.com/sponsors/mkdocstrings
+mkdocstrings/python/discussions Project-URL: Gitter, https://gitter.im/
+mkdocstrings/python Project-URL: Funding, https://github.com/sponsors/pawamoy
 Requires-Python: >=3.7 Requires-Dist: mkdocstrings>=0.20 Requires-Dist:
 griffe>=0.24 Description-Content-Type: text/markdown
                        ****** mkdocstrings-python ******
                       A Python handler for mkdocstrings.
              [ci] [documentation] [pypi_version] [gitpod] [gitter]
 ---
                                   [logo.png]
```

