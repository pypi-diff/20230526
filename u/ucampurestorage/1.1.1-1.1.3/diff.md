# Comparing `tmp/ucampurestorage-1.1.1.tar.gz` & `tmp/ucampurestorage-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ucampurestorage-1.1.1.tar", last modified: Thu May 25 16:38:06 2023, max compression
+gzip compressed data, was "ucampurestorage-1.1.3.tar", last modified: Fri May 26 11:07:24 2023, max compression
```

## Comparing `ucampurestorage-1.1.1.tar` & `ucampurestorage-1.1.3.tar`

### file list

```diff
@@ -1,189 +1,189 @@
-drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-25 16:38:06.797116 ucampurestorage-1.1.1/
--rw-rw-r--   0 im        (1000) im        (1000)       62 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/.coveragerc
--rw-rw-r--   0 im        (1000) im        (1000)       64 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/.flake8
--rw-rw-r--   0 im        (1000) im        (1000)      581 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/.gitignore
--rw-rw-r--   0 im        (1000) im        (1000)     1403 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/.gitlab-ci.yml
--rw-rw-r--   0 im        (1000) im        (1000)      107 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/Dockerfile
--rw-rw-r--   0 im        (1000) im        (1000)     1094 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/LICENSE
--rw-rw-r--   0 im        (1000) im        (1000)    20169 2023-05-25 16:38:06.785116 ucampurestorage-1.1.1/PKG-INFO
--rw-rw-r--   0 im        (1000) im        (1000)    19799 2023-05-25 16:27:48.000000 ucampurestorage-1.1.1/README.md
-drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-25 16:38:06.329117 ucampurestorage-1.1.1/compose/
--rw-rw-r--   0 im        (1000) im        (1000)      566 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/compose/docs.Dockerfile
--rw-rw-r--   0 im        (1000) im        (1000)      270 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/compose/docs.yml
--rw-rw-r--   0 im        (1000) im        (1000)       73 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/compose/docs_http.Dockerfile
--rw-rw-r--   0 im        (1000) im        (1000)      135 2023-05-22 13:17:56.000000 ucampurestorage-1.1.1/compose/docs_http.yml
--rw-rw-r--   0 im        (1000) im        (1000)      136 2023-05-22 13:17:56.000000 ucampurestorage-1.1.1/compose/document.Dockerfile
--rw-rw-r--   0 im        (1000) im        (1000)      174 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/compose/pytest.Dockerfile
--rw-rw-r--   0 im        (1000) im        (1000)      172 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/compose/tox.Dockerfile
--rw-rw-r--   0 im        (1000) im        (1000)      161 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/compose/tox.env
--rw-rw-r--   0 im        (1000) im        (1000)      367 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/compose/tox.yml
-drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-25 16:38:06.365117 ucampurestorage-1.1.1/docs/
--rw-rw-r--   0 im        (1000) im        (1000)      634 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/Makefile
--rw-rw-r--   0 im        (1000) im        (1000)    20369 2023-05-25 16:27:48.000000 ucampurestorage-1.1.1/docs/README.rst
-drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-25 16:38:06.253117 ucampurestorage-1.1.1/docs/_build/
-drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-25 16:38:06.389117 ucampurestorage-1.1.1/docs/_build/doctrees/
--rw-rw-r--   0 im        (1000) im        (1000)     9696 2023-05-22 13:17:56.000000 ucampurestorage-1.1.1/docs/_build/doctrees/access.doctree
--rw-rw-r--   0 im        (1000) im        (1000)     9138 2023-05-23 02:06:23.000000 ucampurestorage-1.1.1/docs/_build/doctrees/changelog.doctree
--rw-rw-r--   0 im        (1000) im        (1000)   224739 2023-05-25 16:27:48.000000 ucampurestorage-1.1.1/docs/_build/doctrees/environment.pickle
--rw-rw-r--   0 im        (1000) im        (1000)     5375 2023-05-22 13:17:56.000000 ucampurestorage-1.1.1/docs/_build/doctrees/index.doctree
--rw-rw-r--   0 im        (1000) im        (1000)     2774 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/doctrees/modules.doctree
--rw-rw-r--   0 im        (1000) im        (1000)    49098 2023-05-25 16:27:48.000000 ucampurestorage-1.1.1/docs/_build/doctrees/readme.doctree
--rw-rw-r--   0 im        (1000) im        (1000)     3364 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/doctrees/readme_link.doctree
--rw-rw-r--   0 im        (1000) im        (1000)     4245 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/doctrees/ucampurestorage.doctree
--rw-rw-r--   0 im        (1000) im        (1000)   401753 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/doctrees/ucampurestorage.lib.doctree
--rw-rw-r--   0 im        (1000) im        (1000)    82637 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/doctrees/ucampurestorage.tests.doctree
-drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-25 16:38:06.469117 ucampurestorage-1.1.1/docs/_build/html/
--rw-rw-r--   0 im        (1000) im        (1000)      230 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/.buildinfo
-drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-25 16:38:06.485117 ucampurestorage-1.1.1/docs/_build/html/_images/
--rw-rw-r--   0 im        (1000) im        (1000)    55850 2023-05-22 13:17:56.000000 ucampurestorage-1.1.1/docs/_build/html/_images/access1.jpg
--rw-rw-r--   0 im        (1000) im        (1000)    48072 2023-05-22 13:17:56.000000 ucampurestorage-1.1.1/docs/_build/html/_images/access2.jpg
--rw-rw-r--   0 im        (1000) im        (1000)    65210 2023-05-22 13:17:56.000000 ucampurestorage-1.1.1/docs/_build/html/_images/access3.jpg
--rw-rw-r--   0 im        (1000) im        (1000)    64548 2023-05-22 13:17:56.000000 ucampurestorage-1.1.1/docs/_build/html/_images/access4.jpg
--rw-rw-r--   0 im        (1000) im        (1000)    68756 2023-05-22 13:17:56.000000 ucampurestorage-1.1.1/docs/_build/html/_images/access5.jpg
--rw-rw-r--   0 im        (1000) im        (1000)    77722 2023-05-22 13:17:56.000000 ucampurestorage-1.1.1/docs/_build/html/_images/access6.jpg
--rw-rw-r--   0 im        (1000) im        (1000)   127824 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_images/pure_storage.jpg
--rw-rw-r--   0 im        (1000) im        (1000)   127824 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_images/pure_storage1.jpg
-drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-25 16:38:06.489117 ucampurestorage-1.1.1/docs/_build/html/_modules/
--rw-rw-r--   0 im        (1000) im        (1000)     4577 2023-05-22 13:17:56.000000 ucampurestorage-1.1.1/docs/_build/html/_modules/index.html
-drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-25 16:38:06.261117 ucampurestorage-1.1.1/docs/_build/html/_modules/ucampurestorage/
-drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-25 16:38:06.497117 ucampurestorage-1.1.1/docs/_build/html/_modules/ucampurestorage/lib/
--rw-rw-r--   0 im        (1000) im        (1000)    17027 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_modules/ucampurestorage/lib/httpclient.html
--rw-rw-r--   0 im        (1000) im        (1000)   171346 2023-05-22 13:17:56.000000 ucampurestorage-1.1.1/docs/_build/html/_modules/ucampurestorage/lib/options.html
--rw-rw-r--   0 im        (1000) im        (1000)   112303 2023-05-25 16:27:48.000000 ucampurestorage-1.1.1/docs/_build/html/_modules/ucampurestorage/lib/process.html
--rw-rw-r--   0 im        (1000) im        (1000)   239110 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_modules/ucampurestorage/lib/pureconnect.html
--rw-rw-r--   0 im        (1000) im        (1000)    27634 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_modules/ucampurestorage/lib/tokencreater.html
-drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-25 16:38:06.501117 ucampurestorage-1.1.1/docs/_build/html/_modules/ucampurestorage/tests/
--rw-rw-r--   0 im        (1000) im        (1000)     7825 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_modules/ucampurestorage/tests/test_httpclient.html
--rw-rw-r--   0 im        (1000) im        (1000)    39634 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_modules/ucampurestorage/tests/test_process.html
--rw-rw-r--   0 im        (1000) im        (1000)    20339 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_modules/ucampurestorage/tests/test_pureconnection.html
--rw-rw-r--   0 im        (1000) im        (1000)    13133 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_modules/ucampurestorage/tests/test_tokencreater.html
-drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-25 16:38:06.517117 ucampurestorage-1.1.1/docs/_build/html/_sources/
--rw-rw-r--   0 im        (1000) im        (1000)     1708 2023-05-22 13:17:56.000000 ucampurestorage-1.1.1/docs/_build/html/_sources/access.rst.txt
--rw-rw-r--   0 im        (1000) im        (1000)      632 2023-05-23 02:06:23.000000 ucampurestorage-1.1.1/docs/_build/html/_sources/changelog.rst.txt
--rw-rw-r--   0 im        (1000) im        (1000)      578 2023-05-22 13:17:56.000000 ucampurestorage-1.1.1/docs/_build/html/_sources/index.rst.txt
--rw-rw-r--   0 im        (1000) im        (1000)       82 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_sources/modules.rst.txt
--rw-rw-r--   0 im        (1000) im        (1000)    20369 2023-05-25 16:27:48.000000 ucampurestorage-1.1.1/docs/_build/html/_sources/readme.rst.txt
--rw-rw-r--   0 im        (1000) im        (1000)       52 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_sources/readme_link.rst.txt
--rw-rw-r--   0 im        (1000) im        (1000)     1089 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_sources/ucampurestorage.lib.rst.txt
--rw-rw-r--   0 im        (1000) im        (1000)      272 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_sources/ucampurestorage.rst.txt
--rw-rw-r--   0 im        (1000) im        (1000)     1213 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_sources/ucampurestorage.tests.rst.txt
-drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-25 16:38:06.561117 ucampurestorage-1.1.1/docs/_build/html/_static/
--rw-rw-r--   0 im        (1000) im        (1000)    14692 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_static/basic.css
-drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-25 16:38:06.561117 ucampurestorage-1.1.1/docs/_build/html/_static/css/
--rw-rw-r--   0 im        (1000) im        (1000)     3229 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_static/css/badge_only.css
-drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-25 16:38:06.625117 ucampurestorage-1.1.1/docs/_build/html/_static/css/fonts/
--rw-rw-r--   0 im        (1000) im        (1000)    87624 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-rw-r--   0 im        (1000) im        (1000)    67312 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-rw-r--   0 im        (1000) im        (1000)    86288 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-rw-r--   0 im        (1000) im        (1000)    66444 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-rw-r--   0 im        (1000) im        (1000)   165742 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot
--rw-rw-r--   0 im        (1000) im        (1000)   444379 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-rw-r--   0 im        (1000) im        (1000)   165548 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf
--rw-rw-r--   0 im        (1000) im        (1000)    98024 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff
--rw-rw-r--   0 im        (1000) im        (1000)    77160 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2
--rw-rw-r--   0 im        (1000) im        (1000)   323344 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_static/css/fonts/lato-bold-italic.woff
--rw-rw-r--   0 im        (1000) im        (1000)   193308 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2
--rw-rw-r--   0 im        (1000) im        (1000)   309728 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_static/css/fonts/lato-bold.woff
--rw-rw-r--   0 im        (1000) im        (1000)   184912 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_static/css/fonts/lato-bold.woff2
--rw-rw-r--   0 im        (1000) im        (1000)   328412 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_static/css/fonts/lato-normal-italic.woff
--rw-rw-r--   0 im        (1000) im        (1000)   195704 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2
--rw-rw-r--   0 im        (1000) im        (1000)   309192 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_static/css/fonts/lato-normal.woff
--rw-rw-r--   0 im        (1000) im        (1000)   182708 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_static/css/fonts/lato-normal.woff2
--rw-rw-r--   0 im        (1000) im        (1000)   135235 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_static/css/theme.css
--rw-rw-r--   0 im        (1000) im        (1000)    10766 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_static/doctools.js
--rw-rw-r--   0 im        (1000) im        (1000)      422 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_static/documentation_options.js
--rw-rw-r--   0 im        (1000) im        (1000)      286 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_static/file.png
--rw-rw-r--   0 im        (1000) im        (1000)   287630 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_static/jquery-3.5.1.js
--rw-rw-r--   0 im        (1000) im        (1000)    89476 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_static/jquery.js
-drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-25 16:38:06.657117 ucampurestorage-1.1.1/docs/_build/html/_static/js/
--rw-rw-r--   0 im        (1000) im        (1000)      934 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_static/js/badge_only.js
--rw-rw-r--   0 im        (1000) im        (1000)     4370 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_static/js/html5shiv-printshiv.min.js
--rw-rw-r--   0 im        (1000) im        (1000)     2734 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_static/js/html5shiv.min.js
--rw-rw-r--   0 im        (1000) im        (1000)     5023 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_static/js/theme.js
--rw-rw-r--   0 im        (1000) im        (1000)    10854 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_static/language_data.js
--rw-rw-r--   0 im        (1000) im        (1000)       90 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_static/minus.png
--rw-rw-r--   0 im        (1000) im        (1000)     4467 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_static/nbsphinx-broken-thumbnail.svg
--rw-rw-r--   0 im        (1000) im        (1000)     6625 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_static/nbsphinx-code-cells.css
--rw-rw-r--   0 im        (1000) im        (1000)      584 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_static/nbsphinx-gallery.css
--rw-rw-r--   0 im        (1000) im        (1000)     2871 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_static/nbsphinx-no-thumbnail.svg
--rw-rw-r--   0 im        (1000) im        (1000)       90 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_static/plus.png
--rw-rw-r--   0 im        (1000) im        (1000)     4819 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_static/pygments.css
--rw-rw-r--   0 im        (1000) im        (1000)    16634 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_static/searchtools.js
--rw-rw-r--   0 im        (1000) im        (1000)     4712 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_static/sphinx_highlight.js
--rw-rw-r--   0 im        (1000) im        (1000)    68420 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_static/underscore-1.13.1.js
--rw-rw-r--   0 im        (1000) im        (1000)    19530 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/_static/underscore.js
--rw-rw-r--   0 im        (1000) im        (1000)     7712 2023-05-22 13:17:56.000000 ucampurestorage-1.1.1/docs/_build/html/access.html
--rw-rw-r--   0 im        (1000) im        (1000)     5742 2023-05-23 02:06:23.000000 ucampurestorage-1.1.1/docs/_build/html/changelog.html
--rw-rw-r--   0 im        (1000) im        (1000)    40657 2023-05-22 13:17:56.000000 ucampurestorage-1.1.1/docs/_build/html/genindex.html
--rw-rw-r--   0 im        (1000) im        (1000)     6554 2023-05-25 16:27:48.000000 ucampurestorage-1.1.1/docs/_build/html/index.html
--rw-rw-r--   0 im        (1000) im        (1000)     7680 2023-05-22 13:17:56.000000 ucampurestorage-1.1.1/docs/_build/html/modules.html
--rw-rw-r--   0 im        (1000) im        (1000)     1696 2023-05-22 13:17:56.000000 ucampurestorage-1.1.1/docs/_build/html/objects.inv
--rw-rw-r--   0 im        (1000) im        (1000)     7208 2023-05-22 13:17:56.000000 ucampurestorage-1.1.1/docs/_build/html/py-modindex.html
--rw-rw-r--   0 im        (1000) im        (1000)    96668 2023-05-25 16:27:48.000000 ucampurestorage-1.1.1/docs/_build/html/readme.html
--rw-rw-r--   0 im        (1000) im        (1000)     3746 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/_build/html/readme_link.html
--rw-rw-r--   0 im        (1000) im        (1000)     4019 2023-05-22 13:17:56.000000 ucampurestorage-1.1.1/docs/_build/html/search.html
--rw-rw-r--   0 im        (1000) im        (1000)    17057 2023-05-25 16:27:48.000000 ucampurestorage-1.1.1/docs/_build/html/searchindex.js
--rw-rw-r--   0 im        (1000) im        (1000)     8344 2023-05-22 13:17:56.000000 ucampurestorage-1.1.1/docs/_build/html/ucampurestorage.html
--rw-rw-r--   0 im        (1000) im        (1000)   144181 2023-05-22 13:17:56.000000 ucampurestorage-1.1.1/docs/_build/html/ucampurestorage.lib.html
--rw-rw-r--   0 im        (1000) im        (1000)    44746 2023-05-22 13:17:56.000000 ucampurestorage-1.1.1/docs/_build/html/ucampurestorage.tests.html
--rw-rw-r--   0 im        (1000) im        (1000)     1708 2023-05-22 13:17:56.000000 ucampurestorage-1.1.1/docs/access.rst
--rw-rw-r--   0 im        (1000) im        (1000)    55850 2023-05-22 13:17:56.000000 ucampurestorage-1.1.1/docs/access1.JPG
--rw-rw-r--   0 im        (1000) im        (1000)    48072 2023-05-22 13:17:56.000000 ucampurestorage-1.1.1/docs/access2.JPG
--rw-rw-r--   0 im        (1000) im        (1000)    65210 2023-05-22 13:17:56.000000 ucampurestorage-1.1.1/docs/access3.JPG
--rw-rw-r--   0 im        (1000) im        (1000)    64548 2023-05-22 13:17:56.000000 ucampurestorage-1.1.1/docs/access4.JPG
--rw-rw-r--   0 im        (1000) im        (1000)    68756 2023-05-22 13:17:56.000000 ucampurestorage-1.1.1/docs/access5.JPG
--rw-rw-r--   0 im        (1000) im        (1000)    77722 2023-05-22 13:17:56.000000 ucampurestorage-1.1.1/docs/access6.JPG
--rw-rw-r--   0 im        (1000) im        (1000)      704 2023-05-25 16:30:14.000000 ucampurestorage-1.1.1/docs/changelog.rst
--rw-rw-r--   0 im        (1000) im        (1000)     1138 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/conf.py
--rw-rw-r--   0 im        (1000) im        (1000)      578 2023-05-22 13:17:56.000000 ucampurestorage-1.1.1/docs/index.rst
--rw-rw-r--   0 im        (1000) im        (1000)      765 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/make.bat
--rw-rw-r--   0 im        (1000) im        (1000)       82 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/modules.rst
--rw-rw-r--   0 im        (1000) im        (1000)   127824 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/pure_storage.jpg
--rw-rw-r--   0 im        (1000) im        (1000)     1089 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/ucampurestorage.lib.rst
--rw-rw-r--   0 im        (1000) im        (1000)      272 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/ucampurestorage.rst
--rw-rw-r--   0 im        (1000) im        (1000)     1213 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/docs/ucampurestorage.tests.rst
--rw-rw-r--   0 im        (1000) im        (1000)   127824 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/pure_storage.jpg
--rw-rw-r--   0 im        (1000) im        (1000)     1384 2023-05-25 16:27:48.000000 ucampurestorage-1.1.1/pyproject.toml
--rw-rw-r--   0 im        (1000) im        (1000)      119 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/requirements-dev.txt
--rw-rw-r--   0 im        (1000) im        (1000)       58 2023-05-22 13:17:56.000000 ucampurestorage-1.1.1/requirements-docs.txt
--rw-rw-r--   0 im        (1000) im        (1000)       60 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/requirements.txt
--rw-rw-r--   0 im        (1000) im        (1000)       38 2023-05-25 16:38:06.797116 ucampurestorage-1.1.1/setup.cfg
--rwxrwxr-x   0 im        (1000) im        (1000)     2672 2023-05-22 19:38:08.000000 ucampurestorage-1.1.1/test.sh
--rw-rw-r--   0 im        (1000) im        (1000)      666 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/tox.ini
-drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-25 16:38:06.709117 ucampurestorage-1.1.1/ucampurecli/
--rw-rw-r--   0 im        (1000) im        (1000)     2675 2023-05-22 22:55:51.000000 ucampurestorage-1.1.1/ucampurecli/README.md
--rwxrwxr-x   0 im        (1000) im        (1000)     2937 2023-05-25 16:27:48.000000 ucampurestorage-1.1.1/ucampurecli/pure_clone_volume
--rwxrwxr-x   0 im        (1000) im        (1000)     3241 2023-05-25 16:27:48.000000 ucampurestorage-1.1.1/ucampurecli/pure_create_snapshot
--rwxrwxr-x   0 im        (1000) im        (1000)     2824 2023-05-25 16:27:48.000000 ucampurestorage-1.1.1/ucampurecli/pure_create_volume
--rwxrwxr-x   0 im        (1000) im        (1000)     2455 2023-05-25 16:27:48.000000 ucampurestorage-1.1.1/ucampurecli/pure_delete_volume
--rwxrwxr-x   0 im        (1000) im        (1000)     5272 2023-05-25 16:27:48.000000 ucampurestorage-1.1.1/ucampurecli/pure_eradicate_destroyed_volume
--rwxrwxr-x   0 im        (1000) im        (1000)     2469 2023-05-25 16:27:48.000000 ucampurestorage-1.1.1/ucampurecli/pure_eradicate_volume
--rwxrwxr-x   0 im        (1000) im        (1000)     3208 2023-05-25 16:27:48.000000 ucampurestorage-1.1.1/ucampurecli/pure_map_volume
--rwxrwxr-x   0 im        (1000) im        (1000)     2401 2023-05-25 16:27:48.000000 ucampurestorage-1.1.1/ucampurecli/pure_record_destoyed_volume
--rwxrwxr-x   0 im        (1000) im        (1000)     3549 2023-05-25 16:27:48.000000 ucampurestorage-1.1.1/ucampurecli/pure_replace_volume
--rwxrwxr-x   0 im        (1000) im        (1000)     3207 2023-05-25 16:27:48.000000 ucampurestorage-1.1.1/ucampurecli/pure_unmap_volume
-drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-25 16:38:06.725116 ucampurestorage-1.1.1/ucampurestorage/
--rw-rw-r--   0 im        (1000) im        (1000)       77 2023-05-25 16:30:52.000000 ucampurestorage-1.1.1/ucampurestorage/__init__.py
--rw-rw-r--   0 im        (1000) im        (1000)     1384 2023-05-22 16:46:35.000000 ucampurestorage-1.1.1/ucampurestorage/__main__.py
-drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-25 16:38:06.777116 ucampurestorage-1.1.1/ucampurestorage/lib/
--rw-rw-r--   0 im        (1000) im        (1000)        0 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/ucampurestorage/lib/__init__.py
--rw-rw-r--   0 im        (1000) im        (1000)     2578 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/ucampurestorage/lib/httpclient.py
--rw-rw-r--   0 im        (1000) im        (1000)    43574 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/ucampurestorage/lib/options.py
--rw-rw-r--   0 im        (1000) im        (1000)    25225 2023-05-25 16:27:48.000000 ucampurestorage-1.1.1/ucampurestorage/lib/process.py
--rw-rw-r--   0 im        (1000) im        (1000)    52149 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/ucampurestorage/lib/pureconnect.py
--rw-rw-r--   0 im        (1000) im        (1000)        0 2023-05-22 13:17:56.000000 ucampurestorage-1.1.1/ucampurestorage/lib/tasks.py
--rw-rw-r--   0 im        (1000) im        (1000)     6044 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/ucampurestorage/lib/tokencreater.py
-drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-25 16:38:06.781116 ucampurestorage-1.1.1/ucampurestorage/tests/
--rw-rw-r--   0 im        (1000) im        (1000)        0 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/ucampurestorage/tests/__init__.py
--rw-rw-r--   0 im        (1000) im        (1000)      699 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/ucampurestorage/tests/test_httpclient.py
--rw-rw-r--   0 im        (1000) im        (1000)     6950 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/ucampurestorage/tests/test_process.py
--rw-rw-r--   0 im        (1000) im        (1000)     3321 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/ucampurestorage/tests/test_pureconnection.py
--rw-rw-r--   0 im        (1000) im        (1000)        0 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/ucampurestorage/tests/test_tasks.py
--rw-rw-r--   0 im        (1000) im        (1000)     2189 2023-05-22 00:08:34.000000 ucampurestorage-1.1.1/ucampurestorage/tests/test_tokencreater.py
-drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-25 16:38:06.757116 ucampurestorage-1.1.1/ucampurestorage.egg-info/
--rw-rw-r--   0 im        (1000) im        (1000)    20169 2023-05-25 16:38:05.000000 ucampurestorage-1.1.1/ucampurestorage.egg-info/PKG-INFO
--rw-rw-r--   0 im        (1000) im        (1000)     6058 2023-05-25 16:38:06.000000 ucampurestorage-1.1.1/ucampurestorage.egg-info/SOURCES.txt
--rw-rw-r--   0 im        (1000) im        (1000)        1 2023-05-25 16:38:05.000000 ucampurestorage-1.1.1/ucampurestorage.egg-info/dependency_links.txt
--rw-rw-r--   0 im        (1000) im        (1000)       66 2023-05-25 16:38:05.000000 ucampurestorage-1.1.1/ucampurestorage.egg-info/entry_points.txt
--rw-rw-r--   0 im        (1000) im        (1000)      109 2023-05-25 16:38:05.000000 ucampurestorage-1.1.1/ucampurestorage.egg-info/requires.txt
--rw-rw-r--   0 im        (1000) im        (1000)       16 2023-05-25 16:38:05.000000 ucampurestorage-1.1.1/ucampurestorage.egg-info/top_level.txt
+drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-26 11:07:24.560426 ucampurestorage-1.1.3/
+-rw-rw-r--   0 im        (1000) im        (1000)       62 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/.coveragerc
+-rw-rw-r--   0 im        (1000) im        (1000)       64 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/.flake8
+-rw-rw-r--   0 im        (1000) im        (1000)      581 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/.gitignore
+-rw-rw-r--   0 im        (1000) im        (1000)     1403 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/.gitlab-ci.yml
+-rw-rw-r--   0 im        (1000) im        (1000)      107 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/Dockerfile
+-rw-rw-r--   0 im        (1000) im        (1000)     1094 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/LICENSE
+-rw-rw-r--   0 im        (1000) im        (1000)    20169 2023-05-26 11:07:24.560426 ucampurestorage-1.1.3/PKG-INFO
+-rw-rw-r--   0 im        (1000) im        (1000)    19799 2023-05-25 16:27:48.000000 ucampurestorage-1.1.3/README.md
+drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-26 11:07:24.440425 ucampurestorage-1.1.3/compose/
+-rw-rw-r--   0 im        (1000) im        (1000)      566 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/compose/docs.Dockerfile
+-rw-rw-r--   0 im        (1000) im        (1000)      270 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/compose/docs.yml
+-rw-rw-r--   0 im        (1000) im        (1000)       73 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/compose/docs_http.Dockerfile
+-rw-rw-r--   0 im        (1000) im        (1000)      135 2023-05-22 13:17:56.000000 ucampurestorage-1.1.3/compose/docs_http.yml
+-rw-rw-r--   0 im        (1000) im        (1000)      136 2023-05-22 13:17:56.000000 ucampurestorage-1.1.3/compose/document.Dockerfile
+-rw-rw-r--   0 im        (1000) im        (1000)      174 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/compose/pytest.Dockerfile
+-rw-rw-r--   0 im        (1000) im        (1000)      172 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/compose/tox.Dockerfile
+-rw-rw-r--   0 im        (1000) im        (1000)      161 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/compose/tox.env
+-rw-rw-r--   0 im        (1000) im        (1000)      367 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/compose/tox.yml
+drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-26 11:07:24.452425 ucampurestorage-1.1.3/docs/
+-rw-rw-r--   0 im        (1000) im        (1000)      634 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/Makefile
+-rw-rw-r--   0 im        (1000) im        (1000)    20369 2023-05-25 16:27:48.000000 ucampurestorage-1.1.3/docs/README.rst
+drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-26 11:07:24.416425 ucampurestorage-1.1.3/docs/_build/
+drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-26 11:07:24.460425 ucampurestorage-1.1.3/docs/_build/doctrees/
+-rw-rw-r--   0 im        (1000) im        (1000)     9696 2023-05-22 13:17:56.000000 ucampurestorage-1.1.3/docs/_build/doctrees/access.doctree
+-rw-rw-r--   0 im        (1000) im        (1000)     9138 2023-05-23 02:06:23.000000 ucampurestorage-1.1.3/docs/_build/doctrees/changelog.doctree
+-rw-rw-r--   0 im        (1000) im        (1000)   224739 2023-05-25 16:27:48.000000 ucampurestorage-1.1.3/docs/_build/doctrees/environment.pickle
+-rw-rw-r--   0 im        (1000) im        (1000)     5375 2023-05-22 13:17:56.000000 ucampurestorage-1.1.3/docs/_build/doctrees/index.doctree
+-rw-rw-r--   0 im        (1000) im        (1000)     2774 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/doctrees/modules.doctree
+-rw-rw-r--   0 im        (1000) im        (1000)    49098 2023-05-25 16:27:48.000000 ucampurestorage-1.1.3/docs/_build/doctrees/readme.doctree
+-rw-rw-r--   0 im        (1000) im        (1000)     3364 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/doctrees/readme_link.doctree
+-rw-rw-r--   0 im        (1000) im        (1000)     4245 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/doctrees/ucampurestorage.doctree
+-rw-rw-r--   0 im        (1000) im        (1000)   401753 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/doctrees/ucampurestorage.lib.doctree
+-rw-rw-r--   0 im        (1000) im        (1000)    82637 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/doctrees/ucampurestorage.tests.doctree
+drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-26 11:07:24.468425 ucampurestorage-1.1.3/docs/_build/html/
+-rw-rw-r--   0 im        (1000) im        (1000)      230 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/.buildinfo
+drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-26 11:07:24.476426 ucampurestorage-1.1.3/docs/_build/html/_images/
+-rw-rw-r--   0 im        (1000) im        (1000)    55850 2023-05-22 13:17:56.000000 ucampurestorage-1.1.3/docs/_build/html/_images/access1.jpg
+-rw-rw-r--   0 im        (1000) im        (1000)    48072 2023-05-22 13:17:56.000000 ucampurestorage-1.1.3/docs/_build/html/_images/access2.jpg
+-rw-rw-r--   0 im        (1000) im        (1000)    65210 2023-05-22 13:17:56.000000 ucampurestorage-1.1.3/docs/_build/html/_images/access3.jpg
+-rw-rw-r--   0 im        (1000) im        (1000)    64548 2023-05-22 13:17:56.000000 ucampurestorage-1.1.3/docs/_build/html/_images/access4.jpg
+-rw-rw-r--   0 im        (1000) im        (1000)    68756 2023-05-22 13:17:56.000000 ucampurestorage-1.1.3/docs/_build/html/_images/access5.jpg
+-rw-rw-r--   0 im        (1000) im        (1000)    77722 2023-05-22 13:17:56.000000 ucampurestorage-1.1.3/docs/_build/html/_images/access6.jpg
+-rw-rw-r--   0 im        (1000) im        (1000)   127824 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_images/pure_storage.jpg
+-rw-rw-r--   0 im        (1000) im        (1000)   127824 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_images/pure_storage1.jpg
+drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-26 11:07:24.476426 ucampurestorage-1.1.3/docs/_build/html/_modules/
+-rw-rw-r--   0 im        (1000) im        (1000)     4577 2023-05-22 13:17:56.000000 ucampurestorage-1.1.3/docs/_build/html/_modules/index.html
+drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-26 11:07:24.420425 ucampurestorage-1.1.3/docs/_build/html/_modules/ucampurestorage/
+drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-26 11:07:24.484426 ucampurestorage-1.1.3/docs/_build/html/_modules/ucampurestorage/lib/
+-rw-rw-r--   0 im        (1000) im        (1000)    17027 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_modules/ucampurestorage/lib/httpclient.html
+-rw-rw-r--   0 im        (1000) im        (1000)   171346 2023-05-22 13:17:56.000000 ucampurestorage-1.1.3/docs/_build/html/_modules/ucampurestorage/lib/options.html
+-rw-rw-r--   0 im        (1000) im        (1000)   112303 2023-05-25 16:27:48.000000 ucampurestorage-1.1.3/docs/_build/html/_modules/ucampurestorage/lib/process.html
+-rw-rw-r--   0 im        (1000) im        (1000)   239110 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_modules/ucampurestorage/lib/pureconnect.html
+-rw-rw-r--   0 im        (1000) im        (1000)    27634 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_modules/ucampurestorage/lib/tokencreater.html
+drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-26 11:07:24.488426 ucampurestorage-1.1.3/docs/_build/html/_modules/ucampurestorage/tests/
+-rw-rw-r--   0 im        (1000) im        (1000)     7825 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_modules/ucampurestorage/tests/test_httpclient.html
+-rw-rw-r--   0 im        (1000) im        (1000)    39634 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_modules/ucampurestorage/tests/test_process.html
+-rw-rw-r--   0 im        (1000) im        (1000)    20339 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_modules/ucampurestorage/tests/test_pureconnection.html
+-rw-rw-r--   0 im        (1000) im        (1000)    13133 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_modules/ucampurestorage/tests/test_tokencreater.html
+drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-26 11:07:24.492426 ucampurestorage-1.1.3/docs/_build/html/_sources/
+-rw-rw-r--   0 im        (1000) im        (1000)     1708 2023-05-22 13:17:56.000000 ucampurestorage-1.1.3/docs/_build/html/_sources/access.rst.txt
+-rw-rw-r--   0 im        (1000) im        (1000)      632 2023-05-23 02:06:23.000000 ucampurestorage-1.1.3/docs/_build/html/_sources/changelog.rst.txt
+-rw-rw-r--   0 im        (1000) im        (1000)      578 2023-05-22 13:17:56.000000 ucampurestorage-1.1.3/docs/_build/html/_sources/index.rst.txt
+-rw-rw-r--   0 im        (1000) im        (1000)       82 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_sources/modules.rst.txt
+-rw-rw-r--   0 im        (1000) im        (1000)    20369 2023-05-25 16:27:48.000000 ucampurestorage-1.1.3/docs/_build/html/_sources/readme.rst.txt
+-rw-rw-r--   0 im        (1000) im        (1000)       52 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_sources/readme_link.rst.txt
+-rw-rw-r--   0 im        (1000) im        (1000)     1089 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_sources/ucampurestorage.lib.rst.txt
+-rw-rw-r--   0 im        (1000) im        (1000)      272 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_sources/ucampurestorage.rst.txt
+-rw-rw-r--   0 im        (1000) im        (1000)     1213 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_sources/ucampurestorage.tests.rst.txt
+drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-26 11:07:24.504426 ucampurestorage-1.1.3/docs/_build/html/_static/
+-rw-rw-r--   0 im        (1000) im        (1000)    14692 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_static/basic.css
+drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-26 11:07:24.508426 ucampurestorage-1.1.3/docs/_build/html/_static/css/
+-rw-rw-r--   0 im        (1000) im        (1000)     3229 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_static/css/badge_only.css
+drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-26 11:07:24.532426 ucampurestorage-1.1.3/docs/_build/html/_static/css/fonts/
+-rw-rw-r--   0 im        (1000) im        (1000)    87624 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-rw-r--   0 im        (1000) im        (1000)    67312 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-rw-r--   0 im        (1000) im        (1000)    86288 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-rw-r--   0 im        (1000) im        (1000)    66444 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-rw-r--   0 im        (1000) im        (1000)   165742 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-rw-r--   0 im        (1000) im        (1000)   444379 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-rw-r--   0 im        (1000) im        (1000)   165548 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-rw-r--   0 im        (1000) im        (1000)    98024 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-rw-r--   0 im        (1000) im        (1000)    77160 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-rw-r--   0 im        (1000) im        (1000)   323344 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_static/css/fonts/lato-bold-italic.woff
+-rw-rw-r--   0 im        (1000) im        (1000)   193308 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2
+-rw-rw-r--   0 im        (1000) im        (1000)   309728 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_static/css/fonts/lato-bold.woff
+-rw-rw-r--   0 im        (1000) im        (1000)   184912 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_static/css/fonts/lato-bold.woff2
+-rw-rw-r--   0 im        (1000) im        (1000)   328412 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_static/css/fonts/lato-normal-italic.woff
+-rw-rw-r--   0 im        (1000) im        (1000)   195704 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2
+-rw-rw-r--   0 im        (1000) im        (1000)   309192 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_static/css/fonts/lato-normal.woff
+-rw-rw-r--   0 im        (1000) im        (1000)   182708 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_static/css/fonts/lato-normal.woff2
+-rw-rw-r--   0 im        (1000) im        (1000)   135235 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_static/css/theme.css
+-rw-rw-r--   0 im        (1000) im        (1000)    10766 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_static/doctools.js
+-rw-rw-r--   0 im        (1000) im        (1000)      422 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_static/documentation_options.js
+-rw-rw-r--   0 im        (1000) im        (1000)      286 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_static/file.png
+-rw-rw-r--   0 im        (1000) im        (1000)   287630 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_static/jquery-3.5.1.js
+-rw-rw-r--   0 im        (1000) im        (1000)    89476 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_static/jquery.js
+drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-26 11:07:24.532426 ucampurestorage-1.1.3/docs/_build/html/_static/js/
+-rw-rw-r--   0 im        (1000) im        (1000)      934 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_static/js/badge_only.js
+-rw-rw-r--   0 im        (1000) im        (1000)     4370 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_static/js/html5shiv-printshiv.min.js
+-rw-rw-r--   0 im        (1000) im        (1000)     2734 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_static/js/html5shiv.min.js
+-rw-rw-r--   0 im        (1000) im        (1000)     5023 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_static/js/theme.js
+-rw-rw-r--   0 im        (1000) im        (1000)    10854 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_static/language_data.js
+-rw-rw-r--   0 im        (1000) im        (1000)       90 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 im        (1000) im        (1000)     4467 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_static/nbsphinx-broken-thumbnail.svg
+-rw-rw-r--   0 im        (1000) im        (1000)     6625 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_static/nbsphinx-code-cells.css
+-rw-rw-r--   0 im        (1000) im        (1000)      584 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_static/nbsphinx-gallery.css
+-rw-rw-r--   0 im        (1000) im        (1000)     2871 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_static/nbsphinx-no-thumbnail.svg
+-rw-rw-r--   0 im        (1000) im        (1000)       90 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 im        (1000) im        (1000)     4819 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_static/pygments.css
+-rw-rw-r--   0 im        (1000) im        (1000)    16634 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_static/searchtools.js
+-rw-rw-r--   0 im        (1000) im        (1000)     4712 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_static/sphinx_highlight.js
+-rw-rw-r--   0 im        (1000) im        (1000)    68420 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_static/underscore-1.13.1.js
+-rw-rw-r--   0 im        (1000) im        (1000)    19530 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/_static/underscore.js
+-rw-rw-r--   0 im        (1000) im        (1000)     7712 2023-05-22 13:17:56.000000 ucampurestorage-1.1.3/docs/_build/html/access.html
+-rw-rw-r--   0 im        (1000) im        (1000)     5742 2023-05-23 02:06:23.000000 ucampurestorage-1.1.3/docs/_build/html/changelog.html
+-rw-rw-r--   0 im        (1000) im        (1000)    40657 2023-05-22 13:17:56.000000 ucampurestorage-1.1.3/docs/_build/html/genindex.html
+-rw-rw-r--   0 im        (1000) im        (1000)     6554 2023-05-25 16:27:48.000000 ucampurestorage-1.1.3/docs/_build/html/index.html
+-rw-rw-r--   0 im        (1000) im        (1000)     7680 2023-05-22 13:17:56.000000 ucampurestorage-1.1.3/docs/_build/html/modules.html
+-rw-rw-r--   0 im        (1000) im        (1000)     1696 2023-05-22 13:17:56.000000 ucampurestorage-1.1.3/docs/_build/html/objects.inv
+-rw-rw-r--   0 im        (1000) im        (1000)     7208 2023-05-22 13:17:56.000000 ucampurestorage-1.1.3/docs/_build/html/py-modindex.html
+-rw-rw-r--   0 im        (1000) im        (1000)    96668 2023-05-25 16:27:48.000000 ucampurestorage-1.1.3/docs/_build/html/readme.html
+-rw-rw-r--   0 im        (1000) im        (1000)     3746 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/_build/html/readme_link.html
+-rw-rw-r--   0 im        (1000) im        (1000)     4019 2023-05-22 13:17:56.000000 ucampurestorage-1.1.3/docs/_build/html/search.html
+-rw-rw-r--   0 im        (1000) im        (1000)    17057 2023-05-25 16:27:48.000000 ucampurestorage-1.1.3/docs/_build/html/searchindex.js
+-rw-rw-r--   0 im        (1000) im        (1000)     8344 2023-05-22 13:17:56.000000 ucampurestorage-1.1.3/docs/_build/html/ucampurestorage.html
+-rw-rw-r--   0 im        (1000) im        (1000)   144181 2023-05-22 13:17:56.000000 ucampurestorage-1.1.3/docs/_build/html/ucampurestorage.lib.html
+-rw-rw-r--   0 im        (1000) im        (1000)    44746 2023-05-22 13:17:56.000000 ucampurestorage-1.1.3/docs/_build/html/ucampurestorage.tests.html
+-rw-rw-r--   0 im        (1000) im        (1000)     1708 2023-05-22 13:17:56.000000 ucampurestorage-1.1.3/docs/access.rst
+-rw-rw-r--   0 im        (1000) im        (1000)    55850 2023-05-22 13:17:56.000000 ucampurestorage-1.1.3/docs/access1.JPG
+-rw-rw-r--   0 im        (1000) im        (1000)    48072 2023-05-22 13:17:56.000000 ucampurestorage-1.1.3/docs/access2.JPG
+-rw-rw-r--   0 im        (1000) im        (1000)    65210 2023-05-22 13:17:56.000000 ucampurestorage-1.1.3/docs/access3.JPG
+-rw-rw-r--   0 im        (1000) im        (1000)    64548 2023-05-22 13:17:56.000000 ucampurestorage-1.1.3/docs/access4.JPG
+-rw-rw-r--   0 im        (1000) im        (1000)    68756 2023-05-22 13:17:56.000000 ucampurestorage-1.1.3/docs/access5.JPG
+-rw-rw-r--   0 im        (1000) im        (1000)    77722 2023-05-22 13:17:56.000000 ucampurestorage-1.1.3/docs/access6.JPG
+-rw-rw-r--   0 im        (1000) im        (1000)      704 2023-05-25 16:30:14.000000 ucampurestorage-1.1.3/docs/changelog.rst
+-rw-rw-r--   0 im        (1000) im        (1000)     1138 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/conf.py
+-rw-rw-r--   0 im        (1000) im        (1000)      578 2023-05-22 13:17:56.000000 ucampurestorage-1.1.3/docs/index.rst
+-rw-rw-r--   0 im        (1000) im        (1000)      765 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/make.bat
+-rw-rw-r--   0 im        (1000) im        (1000)       82 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/modules.rst
+-rw-rw-r--   0 im        (1000) im        (1000)   127824 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/pure_storage.jpg
+-rw-rw-r--   0 im        (1000) im        (1000)     1089 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/ucampurestorage.lib.rst
+-rw-rw-r--   0 im        (1000) im        (1000)      272 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/ucampurestorage.rst
+-rw-rw-r--   0 im        (1000) im        (1000)     1213 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/docs/ucampurestorage.tests.rst
+-rw-rw-r--   0 im        (1000) im        (1000)   127824 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/pure_storage.jpg
+-rw-rw-r--   0 im        (1000) im        (1000)     1384 2023-05-25 16:27:48.000000 ucampurestorage-1.1.3/pyproject.toml
+-rw-rw-r--   0 im        (1000) im        (1000)      134 2023-05-26 10:54:51.000000 ucampurestorage-1.1.3/requirements-dev.txt
+-rw-rw-r--   0 im        (1000) im        (1000)       58 2023-05-22 13:17:56.000000 ucampurestorage-1.1.3/requirements-docs.txt
+-rw-rw-r--   0 im        (1000) im        (1000)       68 2023-05-26 10:54:32.000000 ucampurestorage-1.1.3/requirements.txt
+-rw-rw-r--   0 im        (1000) im        (1000)       38 2023-05-26 11:07:24.560426 ucampurestorage-1.1.3/setup.cfg
+-rwxrwxr-x   0 im        (1000) im        (1000)     2672 2023-05-22 19:38:08.000000 ucampurestorage-1.1.3/test.sh
+-rw-rw-r--   0 im        (1000) im        (1000)      666 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/tox.ini
+drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-26 11:07:24.560426 ucampurestorage-1.1.3/ucampurecli/
+-rw-rw-r--   0 im        (1000) im        (1000)     2675 2023-05-22 22:55:51.000000 ucampurestorage-1.1.3/ucampurecli/README.md
+-rwxrwxr-x   0 im        (1000) im        (1000)     2933 2023-05-26 10:55:21.000000 ucampurestorage-1.1.3/ucampurecli/pure_clone_volume
+-rwxrwxr-x   0 im        (1000) im        (1000)     3237 2023-05-26 10:55:54.000000 ucampurestorage-1.1.3/ucampurecli/pure_create_snapshot
+-rwxrwxr-x   0 im        (1000) im        (1000)     2820 2023-05-26 10:56:11.000000 ucampurestorage-1.1.3/ucampurecli/pure_create_volume
+-rwxrwxr-x   0 im        (1000) im        (1000)     2451 2023-05-26 10:56:25.000000 ucampurestorage-1.1.3/ucampurecli/pure_delete_volume
+-rwxrwxr-x   0 im        (1000) im        (1000)     5268 2023-05-26 10:56:40.000000 ucampurestorage-1.1.3/ucampurecli/pure_eradicate_destroyed_volume
+-rwxrwxr-x   0 im        (1000) im        (1000)     2465 2023-05-26 10:56:53.000000 ucampurestorage-1.1.3/ucampurecli/pure_eradicate_volume
+-rwxrwxr-x   0 im        (1000) im        (1000)     3204 2023-05-26 10:57:11.000000 ucampurestorage-1.1.3/ucampurecli/pure_map_volume
+-rwxrwxr-x   0 im        (1000) im        (1000)     2397 2023-05-26 10:57:34.000000 ucampurestorage-1.1.3/ucampurecli/pure_record_destoyed_volume
+-rwxrwxr-x   0 im        (1000) im        (1000)     3545 2023-05-26 10:57:49.000000 ucampurestorage-1.1.3/ucampurecli/pure_replace_volume
+-rwxrwxr-x   0 im        (1000) im        (1000)     3203 2023-05-26 10:58:01.000000 ucampurestorage-1.1.3/ucampurecli/pure_unmap_volume
+drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-26 11:07:24.560426 ucampurestorage-1.1.3/ucampurestorage/
+-rw-rw-r--   0 im        (1000) im        (1000)       77 2023-05-26 10:58:54.000000 ucampurestorage-1.1.3/ucampurestorage/__init__.py
+-rw-rw-r--   0 im        (1000) im        (1000)     1384 2023-05-22 16:46:35.000000 ucampurestorage-1.1.3/ucampurestorage/__main__.py
+drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-26 11:07:24.560426 ucampurestorage-1.1.3/ucampurestorage/lib/
+-rw-rw-r--   0 im        (1000) im        (1000)        0 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/ucampurestorage/lib/__init__.py
+-rw-rw-r--   0 im        (1000) im        (1000)     2578 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/ucampurestorage/lib/httpclient.py
+-rw-rw-r--   0 im        (1000) im        (1000)    43574 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/ucampurestorage/lib/options.py
+-rw-rw-r--   0 im        (1000) im        (1000)    25225 2023-05-25 16:27:48.000000 ucampurestorage-1.1.3/ucampurestorage/lib/process.py
+-rw-rw-r--   0 im        (1000) im        (1000)    52149 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/ucampurestorage/lib/pureconnect.py
+-rw-rw-r--   0 im        (1000) im        (1000)        0 2023-05-22 13:17:56.000000 ucampurestorage-1.1.3/ucampurestorage/lib/tasks.py
+-rw-rw-r--   0 im        (1000) im        (1000)     6044 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/ucampurestorage/lib/tokencreater.py
+drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-26 11:07:24.560426 ucampurestorage-1.1.3/ucampurestorage/tests/
+-rw-rw-r--   0 im        (1000) im        (1000)        0 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/ucampurestorage/tests/__init__.py
+-rw-rw-r--   0 im        (1000) im        (1000)      699 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/ucampurestorage/tests/test_httpclient.py
+-rw-rw-r--   0 im        (1000) im        (1000)     6950 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/ucampurestorage/tests/test_process.py
+-rw-rw-r--   0 im        (1000) im        (1000)     3321 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/ucampurestorage/tests/test_pureconnection.py
+-rw-rw-r--   0 im        (1000) im        (1000)        0 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/ucampurestorage/tests/test_tasks.py
+-rw-rw-r--   0 im        (1000) im        (1000)     2189 2023-05-22 00:08:34.000000 ucampurestorage-1.1.3/ucampurestorage/tests/test_tokencreater.py
+drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-26 11:07:24.560426 ucampurestorage-1.1.3/ucampurestorage.egg-info/
+-rw-rw-r--   0 im        (1000) im        (1000)    20169 2023-05-26 11:07:24.000000 ucampurestorage-1.1.3/ucampurestorage.egg-info/PKG-INFO
+-rw-rw-r--   0 im        (1000) im        (1000)     6058 2023-05-26 11:07:24.000000 ucampurestorage-1.1.3/ucampurestorage.egg-info/SOURCES.txt
+-rw-rw-r--   0 im        (1000) im        (1000)        1 2023-05-26 11:07:24.000000 ucampurestorage-1.1.3/ucampurestorage.egg-info/dependency_links.txt
+-rw-rw-r--   0 im        (1000) im        (1000)       66 2023-05-26 11:07:24.000000 ucampurestorage-1.1.3/ucampurestorage.egg-info/entry_points.txt
+-rw-rw-r--   0 im        (1000) im        (1000)      109 2023-05-26 11:07:24.000000 ucampurestorage-1.1.3/ucampurestorage.egg-info/requires.txt
+-rw-rw-r--   0 im        (1000) im        (1000)       16 2023-05-26 11:07:24.000000 ucampurestorage-1.1.3/ucampurestorage.egg-info/top_level.txt
```

### Comparing `ucampurestorage-1.1.1/.gitignore` & `ucampurestorage-1.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/.gitlab-ci.yml` & `ucampurestorage-1.1.3/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/LICENSE` & `ucampurestorage-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/PKG-INFO` & `ucampurestorage-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ucampurestorage
-Version: 1.1.1
+Version: 1.1.3
 Summary: Pure Storage module for the utilization in Cambridge University
 Author-email: Ishan Mahajan <imahajan0007@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ucampurestorage-1.1.1/README.md` & `ucampurestorage-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/compose/docs.Dockerfile` & `ucampurestorage-1.1.3/compose/docs.Dockerfile`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/Makefile` & `ucampurestorage-1.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/README.rst` & `ucampurestorage-1.1.3/docs/README.rst`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/doctrees/access.doctree` & `ucampurestorage-1.1.3/docs/_build/doctrees/access.doctree`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/doctrees/changelog.doctree` & `ucampurestorage-1.1.3/docs/_build/doctrees/changelog.doctree`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/doctrees/environment.pickle` & `ucampurestorage-1.1.3/docs/_build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/doctrees/index.doctree` & `ucampurestorage-1.1.3/docs/_build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/doctrees/modules.doctree` & `ucampurestorage-1.1.3/docs/_build/doctrees/modules.doctree`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/doctrees/readme.doctree` & `ucampurestorage-1.1.3/docs/_build/doctrees/readme.doctree`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/doctrees/readme_link.doctree` & `ucampurestorage-1.1.3/docs/_build/doctrees/readme_link.doctree`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/doctrees/ucampurestorage.doctree` & `ucampurestorage-1.1.3/docs/_build/doctrees/ucampurestorage.doctree`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/doctrees/ucampurestorage.lib.doctree` & `ucampurestorage-1.1.3/docs/_build/doctrees/ucampurestorage.lib.doctree`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/doctrees/ucampurestorage.tests.doctree` & `ucampurestorage-1.1.3/docs/_build/doctrees/ucampurestorage.tests.doctree`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_images/access1.jpg` & `ucampurestorage-1.1.3/docs/_build/html/_images/access1.jpg`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_images/access2.jpg` & `ucampurestorage-1.1.3/docs/_build/html/_images/access2.jpg`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_images/access3.jpg` & `ucampurestorage-1.1.3/docs/_build/html/_images/access3.jpg`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_images/access4.jpg` & `ucampurestorage-1.1.3/docs/_build/html/_images/access4.jpg`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_images/access5.jpg` & `ucampurestorage-1.1.3/docs/_build/html/_images/access5.jpg`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_images/access6.jpg` & `ucampurestorage-1.1.3/docs/_build/html/_images/access6.jpg`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_images/pure_storage.jpg` & `ucampurestorage-1.1.3/docs/_build/html/_images/pure_storage.jpg`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_images/pure_storage1.jpg` & `ucampurestorage-1.1.3/docs/_build/html/_images/pure_storage1.jpg`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_modules/index.html` & `ucampurestorage-1.1.3/docs/_build/html/_modules/index.html`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_modules/ucampurestorage/lib/httpclient.html` & `ucampurestorage-1.1.3/docs/_build/html/_modules/ucampurestorage/lib/httpclient.html`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_modules/ucampurestorage/lib/options.html` & `ucampurestorage-1.1.3/docs/_build/html/_modules/ucampurestorage/lib/options.html`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_modules/ucampurestorage/lib/process.html` & `ucampurestorage-1.1.3/docs/_build/html/_modules/ucampurestorage/lib/process.html`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_modules/ucampurestorage/lib/pureconnect.html` & `ucampurestorage-1.1.3/docs/_build/html/_modules/ucampurestorage/lib/pureconnect.html`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_modules/ucampurestorage/lib/tokencreater.html` & `ucampurestorage-1.1.3/docs/_build/html/_modules/ucampurestorage/lib/tokencreater.html`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_modules/ucampurestorage/tests/test_httpclient.html` & `ucampurestorage-1.1.3/docs/_build/html/_modules/ucampurestorage/tests/test_httpclient.html`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_modules/ucampurestorage/tests/test_process.html` & `ucampurestorage-1.1.3/docs/_build/html/_modules/ucampurestorage/tests/test_process.html`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_modules/ucampurestorage/tests/test_pureconnection.html` & `ucampurestorage-1.1.3/docs/_build/html/_modules/ucampurestorage/tests/test_pureconnection.html`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_modules/ucampurestorage/tests/test_tokencreater.html` & `ucampurestorage-1.1.3/docs/_build/html/_modules/ucampurestorage/tests/test_tokencreater.html`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_sources/access.rst.txt` & `ucampurestorage-1.1.3/docs/_build/html/_sources/access.rst.txt`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_sources/changelog.rst.txt` & `ucampurestorage-1.1.3/docs/_build/html/_sources/changelog.rst.txt`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_sources/index.rst.txt` & `ucampurestorage-1.1.3/docs/_build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_sources/readme.rst.txt` & `ucampurestorage-1.1.3/docs/_build/html/_sources/readme.rst.txt`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_sources/ucampurestorage.lib.rst.txt` & `ucampurestorage-1.1.3/docs/_build/html/_sources/ucampurestorage.lib.rst.txt`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_sources/ucampurestorage.tests.rst.txt` & `ucampurestorage-1.1.3/docs/_build/html/_sources/ucampurestorage.tests.rst.txt`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_static/basic.css` & `ucampurestorage-1.1.3/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_static/css/badge_only.css` & `ucampurestorage-1.1.3/docs/_build/html/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff` & `ucampurestorage-1.1.3/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2` & `ucampurestorage-1.1.3/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff` & `ucampurestorage-1.1.3/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2` & `ucampurestorage-1.1.3/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot` & `ucampurestorage-1.1.3/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg` & `ucampurestorage-1.1.3/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf` & `ucampurestorage-1.1.3/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff` & `ucampurestorage-1.1.3/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2` & `ucampurestorage-1.1.3/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_static/css/fonts/lato-bold-italic.woff` & `ucampurestorage-1.1.3/docs/_build/html/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2` & `ucampurestorage-1.1.3/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_static/css/fonts/lato-bold.woff` & `ucampurestorage-1.1.3/docs/_build/html/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_static/css/fonts/lato-bold.woff2` & `ucampurestorage-1.1.3/docs/_build/html/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_static/css/fonts/lato-normal-italic.woff` & `ucampurestorage-1.1.3/docs/_build/html/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2` & `ucampurestorage-1.1.3/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_static/css/fonts/lato-normal.woff` & `ucampurestorage-1.1.3/docs/_build/html/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_static/css/fonts/lato-normal.woff2` & `ucampurestorage-1.1.3/docs/_build/html/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_static/css/theme.css` & `ucampurestorage-1.1.3/docs/_build/html/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_static/doctools.js` & `ucampurestorage-1.1.3/docs/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_static/jquery-3.5.1.js` & `ucampurestorage-1.1.3/docs/_build/html/_static/jquery-3.5.1.js`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_static/jquery.js` & `ucampurestorage-1.1.3/docs/_build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_static/js/badge_only.js` & `ucampurestorage-1.1.3/docs/_build/html/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_static/js/html5shiv-printshiv.min.js` & `ucampurestorage-1.1.3/docs/_build/html/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_static/js/html5shiv.min.js` & `ucampurestorage-1.1.3/docs/_build/html/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_static/js/theme.js` & `ucampurestorage-1.1.3/docs/_build/html/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_static/language_data.js` & `ucampurestorage-1.1.3/docs/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_static/nbsphinx-broken-thumbnail.svg` & `ucampurestorage-1.1.3/docs/_build/html/_static/nbsphinx-broken-thumbnail.svg`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_static/nbsphinx-code-cells.css` & `ucampurestorage-1.1.3/docs/_build/html/_static/nbsphinx-code-cells.css`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_static/nbsphinx-gallery.css` & `ucampurestorage-1.1.3/docs/_build/html/_static/nbsphinx-gallery.css`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_static/nbsphinx-no-thumbnail.svg` & `ucampurestorage-1.1.3/docs/_build/html/_static/nbsphinx-no-thumbnail.svg`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_static/pygments.css` & `ucampurestorage-1.1.3/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_static/searchtools.js` & `ucampurestorage-1.1.3/docs/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_static/sphinx_highlight.js` & `ucampurestorage-1.1.3/docs/_build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_static/underscore-1.13.1.js` & `ucampurestorage-1.1.3/docs/_build/html/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/_static/underscore.js` & `ucampurestorage-1.1.3/docs/_build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/access.html` & `ucampurestorage-1.1.3/docs/_build/html/access.html`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/changelog.html` & `ucampurestorage-1.1.3/docs/_build/html/changelog.html`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/genindex.html` & `ucampurestorage-1.1.3/docs/_build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/index.html` & `ucampurestorage-1.1.3/docs/_build/html/index.html`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/modules.html` & `ucampurestorage-1.1.3/docs/_build/html/modules.html`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/objects.inv` & `ucampurestorage-1.1.3/docs/_build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/py-modindex.html` & `ucampurestorage-1.1.3/docs/_build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/readme.html` & `ucampurestorage-1.1.3/docs/_build/html/readme.html`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/readme_link.html` & `ucampurestorage-1.1.3/docs/_build/html/readme_link.html`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/search.html` & `ucampurestorage-1.1.3/docs/_build/html/search.html`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/searchindex.js` & `ucampurestorage-1.1.3/docs/_build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/ucampurestorage.html` & `ucampurestorage-1.1.3/docs/_build/html/ucampurestorage.html`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/ucampurestorage.lib.html` & `ucampurestorage-1.1.3/docs/_build/html/ucampurestorage.lib.html`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/_build/html/ucampurestorage.tests.html` & `ucampurestorage-1.1.3/docs/_build/html/ucampurestorage.tests.html`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/access.rst` & `ucampurestorage-1.1.3/docs/access.rst`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/access1.JPG` & `ucampurestorage-1.1.3/docs/access1.JPG`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/access2.JPG` & `ucampurestorage-1.1.3/docs/access2.JPG`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/access3.JPG` & `ucampurestorage-1.1.3/docs/access3.JPG`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/access4.JPG` & `ucampurestorage-1.1.3/docs/access4.JPG`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/access5.JPG` & `ucampurestorage-1.1.3/docs/access5.JPG`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/access6.JPG` & `ucampurestorage-1.1.3/docs/access6.JPG`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/changelog.rst` & `ucampurestorage-1.1.3/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/conf.py` & `ucampurestorage-1.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/index.rst` & `ucampurestorage-1.1.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/make.bat` & `ucampurestorage-1.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/pure_storage.jpg` & `ucampurestorage-1.1.3/docs/pure_storage.jpg`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/ucampurestorage.lib.rst` & `ucampurestorage-1.1.3/docs/ucampurestorage.lib.rst`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/docs/ucampurestorage.tests.rst` & `ucampurestorage-1.1.3/docs/ucampurestorage.tests.rst`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/pure_storage.jpg` & `ucampurestorage-1.1.3/pure_storage.jpg`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/pyproject.toml` & `ucampurestorage-1.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/test.sh` & `ucampurestorage-1.1.3/test.sh`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/tox.ini` & `ucampurestorage-1.1.3/tox.ini`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/ucampurecli/README.md` & `ucampurestorage-1.1.3/ucampurecli/README.md`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/ucampurecli/pure_clone_volume` & `ucampurestorage-1.1.3/ucampurecli/pure_clone_volume`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/bin/bash
-os_level = `cat /etc/os-release |grep REDHAT_SUPPORT_PRODUCT_VERSION |awk -F= '{print $2}' |sed s/\"//g |awk -F. '{print $1}'`
-python38 = "/opt/rh/rh-python38"
+os_level=`cat /etc/os-release |grep REDHAT_SUPPORT_PRODUCT_VERSION |awk -F= '{print $2}' |sed s/\"//g |awk -F. '{print $1}'`
+python38="/opt/rh/rh-python38"
 if [[ "$os_level" == 7 ]]
 then
   if [[ -d  "$python38" ]]
   then
     ucampurestorage="/opt/rh/rh-python38/root/usr/local/bin/ucampurestorage"
   else
     echo "Python 3.8 is not installed as per the recommendatations"
```

### Comparing `ucampurestorage-1.1.1/ucampurecli/pure_create_snapshot` & `ucampurestorage-1.1.3/ucampurecli/pure_create_snapshot`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 #
 #    Args: -s -> source volume name
 #          -l -> Label for replay
 #
 #  Output: Log of actions
 # Returns: TRUE for success, FALSE for failure
 ###################################################################
-os_level = `cat /etc/os-release |grep REDHAT_SUPPORT_PRODUCT_VERSION |awk -F= '{print $2}' |sed s/\"//g |awk -F. '{print $1}'`
-python38 = "/opt/rh/rh-python38"
+os_level=`cat /etc/os-release |grep REDHAT_SUPPORT_PRODUCT_VERSION |awk -F= '{print $2}' |sed s/\"//g |awk -F. '{print $1}'`
+python38="/opt/rh/rh-python38"
 if [[ "$os_level" == 7 ]]
 then
   if [[ -d  "$python38" ]]
   then
     ucampurestorage="/opt/rh/rh-python38/root/usr/local/bin/ucampurestorage"
   else
     echo "Python 3.8 is not installed as per the recommendatations"
```

### Comparing `ucampurestorage-1.1.1/ucampurecli/pure_create_volume` & `ucampurestorage-1.1.3/ucampurecli/pure_create_volume`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 #    Args: -m -> source mountpoint
 #          -l -> Label for replay
 #          -r -> retention (days)
 #
 #  Output: Log of actions
 # Returns: TRUE for success, FALSE for failure
 ###################################################################
-os_level = `cat /etc/os-release |grep REDHAT_SUPPORT_PRODUCT_VERSION |awk -F= '{print $2}' |sed s/\"//g |awk -F. '{print $1}'`
-python38 = "/opt/rh/rh-python38"
+os_level=`cat /etc/os-release |grep REDHAT_SUPPORT_PRODUCT_VERSION |awk -F= '{print $2}' |sed s/\"//g |awk -F. '{print $1}'`
+python38="/opt/rh/rh-python38"
 if [[ "$os_level" == 7 ]]
 then
   if [[ -d  "$python38" ]]
   then
     ucampurestorage="/opt/rh/rh-python38/root/usr/local/bin/ucampurestorage"
   else
     echo "Python 3.8 is not installed as per the recommendatations"
```

### Comparing `ucampurestorage-1.1.1/ucampurecli/pure_delete_volume` & `ucampurestorage-1.1.3/ucampurecli/pure_delete_volume`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 # Purpose: Delete of PureStorage volume
 #
 #    Args: $1 -> name of volume to delete
 #
 #  Output: Log of actions
 # Returns: TRUE for success, FALSE for failure
 ###################################################################
-os_level = `cat /etc/os-release |grep REDHAT_SUPPORT_PRODUCT_VERSION |awk -F= '{print $2}' |sed s/\"//g |awk -F. '{print $1}'`
-python38 = "/opt/rh/rh-python38"
+os_level=`cat /etc/os-release |grep REDHAT_SUPPORT_PRODUCT_VERSION |awk -F= '{print $2}' |sed s/\"//g |awk -F. '{print $1}'`
+python38="/opt/rh/rh-python38"
 if [[ "$os_level" == 7 ]]
 then
   if [[ -d  "$python38" ]]
   then
     ucampurestorage="/opt/rh/rh-python38/root/usr/local/bin/ucampurestorage"
   else
     echo "Python 3.8 is not installed as per the recommendatations"
```

### Comparing `ucampurestorage-1.1.1/ucampurecli/pure_eradicate_destroyed_volume` & `ucampurestorage-1.1.3/ucampurecli/pure_eradicate_destroyed_volume`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/bin/bash
 
-os_level = `cat /etc/os-release |grep REDHAT_SUPPORT_PRODUCT_VERSION |awk -F= '{print $2}' |sed s/\"//g |awk -F. '{print $1}'`
-python38 = "/opt/rh/rh-python38"
+os_level=`cat /etc/os-release |grep REDHAT_SUPPORT_PRODUCT_VERSION |awk -F= '{print $2}' |sed s/\"//g |awk -F. '{print $1}'`
+python38="/opt/rh/rh-python38"
 if [[ "$os_level" == 7 ]]
 then
   if [[ -d  "$python38" ]]
   then
     ucampurestorage="/opt/rh/rh-python38/root/usr/local/bin/ucampurestorage"
   else
     echo "Python 3.8 is not installed as per the recommendatations"
```

### Comparing `ucampurestorage-1.1.1/ucampurecli/pure_eradicate_volume` & `ucampurestorage-1.1.3/ucampurecli/pure_eradicate_volume`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 # Purpose: Eradication of PureStorage volume
 #
 #    Args: $1 -> name of volume to delete
 #
 #  Output: Log of actions
 # Returns: TRUE for success, FALSE for failure
 ###################################################################
-os_level = `cat /etc/os-release |grep REDHAT_SUPPORT_PRODUCT_VERSION |awk -F= '{print $2}' |sed s/\"//g |awk -F. '{print $1}'`
-python38 = "/opt/rh/rh-python38"
+os_level=`cat /etc/os-release |grep REDHAT_SUPPORT_PRODUCT_VERSION |awk -F= '{print $2}' |sed s/\"//g |awk -F. '{print $1}'`
+python38="/opt/rh/rh-python38"
 if [[ "$os_level" == 7 ]]
 then
   if [[ -d  "$python38" ]]
   then
     ucampurestorage="/opt/rh/rh-python38/root/usr/local/bin/ucampurestorage"
   else
     echo "Python 3.8 is not installed as per the recommendatations"
```

### Comparing `ucampurestorage-1.1.1/ucampurecli/pure_map_volume` & `ucampurestorage-1.1.3/ucampurecli/pure_map_volume`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 #
 #    Args: $1 -> name of volume to delete
 #          $2 -> mount point to mount the volume
 #
 #  Output: Log of actions
 # Returns: TRUE for success, FALSE for failure
 ###################################################################
-os_level = `cat /etc/os-release |grep REDHAT_SUPPORT_PRODUCT_VERSION |awk -F= '{print $2}' |sed s/\"//g |awk -F. '{print $1}'`
-python38 = "/opt/rh/rh-python38"
+os_level=`cat /etc/os-release |grep REDHAT_SUPPORT_PRODUCT_VERSION |awk -F= '{print $2}' |sed s/\"//g |awk -F. '{print $1}'`
+python38="/opt/rh/rh-python38"
 if [[ "$os_level" == 7 ]]
 then
   if [[ -d  "$python38" ]]
   then
     ucampurestorage="/opt/rh/rh-python38/root/usr/local/bin/ucampurestorage"
   else
     echo "Python 3.8 is not installed as per the recommendatations"
```

### Comparing `ucampurestorage-1.1.1/ucampurecli/pure_record_destoyed_volume` & `ucampurestorage-1.1.3/ucampurecli/pure_record_destoyed_volume`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/bin/bash
 
-os_level = `cat /etc/os-release |grep REDHAT_SUPPORT_PRODUCT_VERSION |awk -F= '{print $2}' |sed s/\"//g |awk -F. '{print $1}'`
-python38 = "/opt/rh/rh-python38"
+os_level=`cat /etc/os-release |grep REDHAT_SUPPORT_PRODUCT_VERSION |awk -F= '{print $2}' |sed s/\"//g |awk -F. '{print $1}'`
+python38="/opt/rh/rh-python38"
 if [[ "$os_level" == 7 ]]
 then
   if [[ -d  "$python38" ]]
   then
     ucampurestorage="/opt/rh/rh-python38/root/usr/local/bin/ucampurestorage"
   else
     echo "Python 3.8 is not installed as per the recommendatations"
```

### Comparing `ucampurestorage-1.1.1/ucampurecli/pure_replace_volume` & `ucampurestorage-1.1.3/ucampurecli/pure_replace_volume`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 #
 #    Args: -g -> Gold Image (source) mountpoint
 #          -t -> Target (dest) dest mountpoint
 #
 #  Output: Log of actions
 # Returns: TRUE for success, FALSE for failure
 ###################################################################
-os_level = `cat /etc/os-release |grep REDHAT_SUPPORT_PRODUCT_VERSION |awk -F= '{print $2}' |sed s/\"//g |awk -F. '{print $1}'`
-python38 = "/opt/rh/rh-python38"
+os_level=`cat /etc/os-release |grep REDHAT_SUPPORT_PRODUCT_VERSION |awk -F= '{print $2}' |sed s/\"//g |awk -F. '{print $1}'`
+python38="/opt/rh/rh-python38"
 if [[ "$os_level" == 7 ]]
 then
   if [[ -d  "$python38" ]]
   then
     ucampurestorage="/opt/rh/rh-python38/root/usr/local/bin/ucampurestorage"
   else
     echo "Python 3.8 is not installed as per the recommendatations"
```

### Comparing `ucampurestorage-1.1.1/ucampurecli/pure_unmap_volume` & `ucampurestorage-1.1.3/ucampurecli/pure_unmap_volume`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 # Purpose: Unmap of PureStorage volume
 #
 #    Args: $1 -> name of volume to delete
 #
 #  Output: Log of actions
 # Returns: TRUE for success, FALSE for failure
 ###################################################################
-os_level = `cat /etc/os-release |grep REDHAT_SUPPORT_PRODUCT_VERSION |awk -F= '{print $2}' |sed s/\"//g |awk -F. '{print $1}'`
-python38 = "/opt/rh/rh-python38"
+os_level=`cat /etc/os-release |grep REDHAT_SUPPORT_PRODUCT_VERSION |awk -F= '{print $2}' |sed s/\"//g |awk -F. '{print $1}'`
+python38="/opt/rh/rh-python38"
 if [[ "$os_level" == 7 ]]
 then
   if [[ -d  "$python38" ]]
   then
     ucampurestorage="/opt/rh/rh-python38/root/usr/local/bin/ucampurestorage"
   else
     echo "Python 3.8 is not installed as per the recommendatations"
```

### Comparing `ucampurestorage-1.1.1/ucampurestorage/__main__.py` & `ucampurestorage-1.1.3/ucampurestorage/__main__.py`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/ucampurestorage/lib/httpclient.py` & `ucampurestorage-1.1.3/ucampurestorage/lib/httpclient.py`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/ucampurestorage/lib/options.py` & `ucampurestorage-1.1.3/ucampurestorage/lib/options.py`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/ucampurestorage/lib/process.py` & `ucampurestorage-1.1.3/ucampurestorage/lib/process.py`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/ucampurestorage/lib/pureconnect.py` & `ucampurestorage-1.1.3/ucampurestorage/lib/pureconnect.py`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/ucampurestorage/lib/tokencreater.py` & `ucampurestorage-1.1.3/ucampurestorage/lib/tokencreater.py`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/ucampurestorage/tests/test_httpclient.py` & `ucampurestorage-1.1.3/ucampurestorage/tests/test_httpclient.py`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/ucampurestorage/tests/test_process.py` & `ucampurestorage-1.1.3/ucampurestorage/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/ucampurestorage/tests/test_pureconnection.py` & `ucampurestorage-1.1.3/ucampurestorage/tests/test_pureconnection.py`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/ucampurestorage/tests/test_tokencreater.py` & `ucampurestorage-1.1.3/ucampurestorage/tests/test_tokencreater.py`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.1.1/ucampurestorage.egg-info/PKG-INFO` & `ucampurestorage-1.1.3/ucampurestorage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ucampurestorage
-Version: 1.1.1
+Version: 1.1.3
 Summary: Pure Storage module for the utilization in Cambridge University
 Author-email: Ishan Mahajan <imahajan0007@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ucampurestorage-1.1.1/ucampurestorage.egg-info/SOURCES.txt` & `ucampurestorage-1.1.3/ucampurestorage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

