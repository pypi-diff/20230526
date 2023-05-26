# Comparing `tmp/pyrsm-0.8.3.tar.gz` & `tmp/pyrsm-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrsm-0.8.3.tar", last modified: Tue May 23 07:26:20 2023, max compression
+gzip compressed data, was "pyrsm-0.8.4.tar", last modified: Fri May 26 01:12:48 2023, max compression
```

## Comparing `pyrsm-0.8.3.tar` & `pyrsm-0.8.4.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-23 07:26:20.193928 pyrsm-0.8.3/
--rw-r--r--   0 root         (0) staff       (20)    34523 2022-03-19 20:23:12.000000 pyrsm-0.8.3/LICENSE
--rw-r--r--   0 root         (0) staff       (20)      243 2023-05-16 06:57:58.000000 pyrsm-0.8.3/MANIFEST.in
--rw-r--r--   0 root         (0) staff       (20)      592 2023-05-23 07:26:20.194016 pyrsm-0.8.3/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     2625 2023-05-16 19:42:31.000000 pyrsm-0.8.3/README.md
--rw-r--r--   0 root         (0) staff       (20)       80 2022-02-19 01:02:39.000000 pyrsm-0.8.3/pyproject.toml
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-23 07:26:20.180406 pyrsm-0.8.3/pyrsm/
--rw-r--r--   0 root         (0) staff       (20)      312 2023-05-23 07:25:55.000000 pyrsm-0.8.3/pyrsm/__init__.py
--rw-r--r--   0 root         (0) staff       (20)    54279 2023-05-15 06:31:28.000000 pyrsm-0.8.3/pyrsm/basics.py
--rw-r--r--   0 root         (0) staff       (20)     2843 2023-01-31 17:36:18.000000 pyrsm-0.8.3/pyrsm/bins.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-23 07:26:20.181347 pyrsm-0.8.3/pyrsm/data/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-23 07:26:20.182220 pyrsm-0.8.3/pyrsm/data/basics/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/basics/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     6996 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/basics/consider.pkl
--rw-r--r--   0 root         (0) staff       (20)    13754 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/basics/demand_uk.pkl
--rw-r--r--   0 root         (0) staff       (20)     5508 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/basics/newspaper.pkl
--rw-r--r--   0 root         (0) staff       (20)     8545 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/basics/salary.pkl
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-23 07:26:20.183857 pyrsm-0.8.3/pyrsm/data/data/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/data/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     1620 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/data/avengers.pkl
--rw-r--r--   0 root         (0) staff       (20)   207435 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/data/diamonds.pkl
--rw-r--r--   0 root         (0) staff       (20)     1557 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/data/publishers.pkl
--rw-r--r--   0 root         (0) staff       (20)     1660 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/data/superheroes.pkl
--rw-r--r--   0 root         (0) staff       (20)    69129 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/data/titanic.pkl
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-23 07:26:20.184304 pyrsm-0.8.3/pyrsm/data/design/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/design/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     3414 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/design/rndnames.pkl
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-23 07:26:20.187716 pyrsm-0.8.3/pyrsm/data/model/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/model/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     8197 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/model/catalog.pkl
--rw-r--r--   0 root         (0) staff       (20)    41039 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/model/direct_marketing.pkl
--rw-r--r--   0 root         (0) staff       (20)   342723 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/model/dvd.pkl
--rw-r--r--   0 root         (0) staff       (20)     4468 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/model/houseprices.pkl
--rw-r--r--   0 root         (0) staff       (20)    33206 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/model/ideal.pkl
--rw-r--r--   0 root         (0) staff       (20)   126402 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/model/ketchup.pkl
--rw-r--r--   0 root         (0) staff       (20)      315 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/model/movie_contract.pkl
--rw-r--r--   0 root         (0) staff       (20)     3123 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/model/ratings.pkl
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-23 07:26:20.189531 pyrsm-0.8.3/pyrsm/data/multivariate/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/multivariate/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     3125 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/multivariate/carpet.pkl
--rw-r--r--   0 root         (0) staff       (20)     2423 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/multivariate/city.pkl
--rw-r--r--   0 root         (0) staff       (20)     3923 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/multivariate/city2.pkl
--rw-r--r--   0 root         (0) staff       (20)     2625 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/multivariate/computer.pkl
--rw-r--r--   0 root         (0) staff       (20)     3442 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/multivariate/movie.pkl
--rw-r--r--   0 root         (0) staff       (20)     2994 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/multivariate/mp3.pkl
--rw-r--r--   0 root         (0) staff       (20)     3278 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/multivariate/retailers.pkl
--rw-r--r--   0 root         (0) staff       (20)     2357 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/multivariate/shopping.pkl
--rw-r--r--   0 root         (0) staff       (20)     4872 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/multivariate/toothpaste.pkl
--rw-r--r--   0 root         (0) staff       (20)     3678 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/multivariate/tpbrands.pkl
--rw-r--r--   0 root         (0) staff       (20)     1966 2023-01-26 08:23:23.000000 pyrsm-0.8.3/pyrsm/example_data.py
--rw-r--r--   0 root         (0) staff       (20)     5271 2023-05-07 05:21:24.000000 pyrsm-0.8.3/pyrsm/logit.py
--rw-r--r--   0 root         (0) staff       (20)    25270 2023-05-21 21:48:34.000000 pyrsm-0.8.3/pyrsm/model.py
--rw-r--r--   0 root         (0) staff       (20)     2214 2023-05-15 20:48:14.000000 pyrsm-0.8.3/pyrsm/notebook.py
--rw-r--r--   0 root         (0) staff       (20)    37519 2023-04-16 05:51:16.000000 pyrsm-0.8.3/pyrsm/perf.py
--rw-r--r--   0 root         (0) staff       (20)     1835 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/props.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-23 07:26:20.190646 pyrsm-0.8.3/pyrsm/radiant/
--rw-r--r--   0 root         (0) staff       (20)       23 2023-05-18 03:04:58.000000 pyrsm-0.8.3/pyrsm/radiant/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     9489 2023-05-15 05:18:12.000000 pyrsm-0.8.3/pyrsm/radiant/logit.py
--rw-r--r--   0 root         (0) staff       (20)    19960 2023-05-23 03:13:46.000000 pyrsm-0.8.3/pyrsm/radiant/regress.py
--rw-r--r--   0 root         (0) staff       (20)     1200 2023-05-23 03:10:54.000000 pyrsm-0.8.3/pyrsm/radiant/utils.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-23 07:26:20.191551 pyrsm-0.8.3/pyrsm/radiant/www/
--rw-r--r--   0 root         (0) staff       (20)      230 2023-05-11 03:12:37.000000 pyrsm-0.8.3/pyrsm/radiant/www/copy.js
--rw-r--r--   0 root         (0) staff       (20)     1964 2023-05-23 02:45:36.000000 pyrsm-0.8.3/pyrsm/radiant/www/returnTextAreaBinding.js
--rw-r--r--   0 root         (0) staff       (20)     3597 2023-05-11 03:12:22.000000 pyrsm-0.8.3/pyrsm/radiant/www/style.css
--rw-r--r--   0 root         (0) staff       (20)     7564 2023-05-23 03:00:47.000000 pyrsm-0.8.3/pyrsm/regress.py
--rw-r--r--   0 root         (0) staff       (20)     5411 2023-03-27 22:17:11.000000 pyrsm-0.8.3/pyrsm/stats.py
--rw-r--r--   0 root         (0) staff       (20)    10313 2023-05-14 21:06:56.000000 pyrsm-0.8.3/pyrsm/utils.py
--rw-r--r--   0 root         (0) staff       (20)    22603 2023-05-22 00:34:13.000000 pyrsm-0.8.3/pyrsm/visualize.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-23 07:26:20.181227 pyrsm-0.8.3/pyrsm.egg-info/
--rw-r--r--   0 root         (0) staff       (20)      592 2023-05-23 07:26:20.000000 pyrsm-0.8.3/pyrsm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     1838 2023-05-23 07:26:20.000000 pyrsm-0.8.3/pyrsm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-05-23 07:26:20.000000 pyrsm-0.8.3/pyrsm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)      193 2023-05-23 07:26:20.000000 pyrsm-0.8.3/pyrsm.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)        6 2023-05-23 07:26:20.000000 pyrsm-0.8.3/pyrsm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)     1003 2023-05-23 07:26:20.194387 pyrsm-0.8.3/setup.cfg
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-23 07:26:20.193681 pyrsm-0.8.3/tests/
--rw-r--r--   0 root         (0) staff       (20)      722 2023-05-16 05:24:37.000000 pyrsm-0.8.3/tests/test_basics.py
--rw-r--r--   0 root         (0) staff       (20)     1072 2023-03-05 06:28:28.000000 pyrsm-0.8.3/tests/test_bins.py
--rw-r--r--   0 root         (0) staff       (20)      794 2023-05-16 05:39:55.000000 pyrsm-0.8.3/tests/test_example_data.py
--rw-r--r--   0 root         (0) staff       (20)     2756 2023-01-21 01:15:24.000000 pyrsm-0.8.3/tests/test_perf.py
--rw-r--r--   0 root         (0) staff       (20)      615 2023-05-16 05:41:07.000000 pyrsm-0.8.3/tests/test_regression.py
--rw-r--r--   0 root         (0) staff       (20)     2036 2023-03-05 06:38:03.000000 pyrsm-0.8.3/tests/test_stats.py
--rw-r--r--   0 root         (0) staff       (20)     1979 2022-02-13 01:24:09.000000 pyrsm-0.8.3/tests/test_utils.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-26 01:12:48.103767 pyrsm-0.8.4/
+-rw-r--r--   0 root         (0) staff       (20)    34523 2022-03-19 20:23:12.000000 pyrsm-0.8.4/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)      243 2023-05-16 06:57:58.000000 pyrsm-0.8.4/MANIFEST.in
+-rw-r--r--   0 root         (0) staff       (20)      592 2023-05-26 01:12:48.103839 pyrsm-0.8.4/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     2625 2023-05-16 19:42:31.000000 pyrsm-0.8.4/README.md
+-rw-r--r--   0 root         (0) staff       (20)       80 2022-02-19 01:02:39.000000 pyrsm-0.8.4/pyproject.toml
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-26 01:12:48.091590 pyrsm-0.8.4/pyrsm/
+-rw-r--r--   0 root         (0) staff       (20)      312 2023-05-26 01:12:13.000000 pyrsm-0.8.4/pyrsm/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)    54279 2023-05-15 06:31:28.000000 pyrsm-0.8.4/pyrsm/basics.py
+-rw-r--r--   0 root         (0) staff       (20)     2843 2023-01-31 17:36:18.000000 pyrsm-0.8.4/pyrsm/bins.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-26 01:12:48.092500 pyrsm-0.8.4/pyrsm/data/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.4/pyrsm/data/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-26 01:12:48.093525 pyrsm-0.8.4/pyrsm/data/basics/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.4/pyrsm/data/basics/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     6996 2022-02-13 01:24:09.000000 pyrsm-0.8.4/pyrsm/data/basics/consider.pkl
+-rw-r--r--   0 root         (0) staff       (20)    13754 2022-02-13 01:24:09.000000 pyrsm-0.8.4/pyrsm/data/basics/demand_uk.pkl
+-rw-r--r--   0 root         (0) staff       (20)     5508 2022-02-13 01:24:09.000000 pyrsm-0.8.4/pyrsm/data/basics/newspaper.pkl
+-rw-r--r--   0 root         (0) staff       (20)     8545 2022-02-13 01:24:09.000000 pyrsm-0.8.4/pyrsm/data/basics/salary.pkl
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-26 01:12:48.094756 pyrsm-0.8.4/pyrsm/data/data/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.4/pyrsm/data/data/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     1620 2022-02-13 01:24:09.000000 pyrsm-0.8.4/pyrsm/data/data/avengers.pkl
+-rw-r--r--   0 root         (0) staff       (20)   207435 2022-02-13 01:24:09.000000 pyrsm-0.8.4/pyrsm/data/data/diamonds.pkl
+-rw-r--r--   0 root         (0) staff       (20)     1557 2022-02-13 01:24:09.000000 pyrsm-0.8.4/pyrsm/data/data/publishers.pkl
+-rw-r--r--   0 root         (0) staff       (20)     1660 2022-02-13 01:24:09.000000 pyrsm-0.8.4/pyrsm/data/data/superheroes.pkl
+-rw-r--r--   0 root         (0) staff       (20)    69129 2022-02-13 01:24:09.000000 pyrsm-0.8.4/pyrsm/data/data/titanic.pkl
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-26 01:12:48.095106 pyrsm-0.8.4/pyrsm/data/design/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.4/pyrsm/data/design/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     3414 2022-02-13 01:24:09.000000 pyrsm-0.8.4/pyrsm/data/design/rndnames.pkl
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-26 01:12:48.097796 pyrsm-0.8.4/pyrsm/data/model/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.4/pyrsm/data/model/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     8197 2022-02-13 01:24:09.000000 pyrsm-0.8.4/pyrsm/data/model/catalog.pkl
+-rw-r--r--   0 root         (0) staff       (20)    41039 2022-02-13 01:24:09.000000 pyrsm-0.8.4/pyrsm/data/model/direct_marketing.pkl
+-rw-r--r--   0 root         (0) staff       (20)   342723 2022-02-13 01:24:09.000000 pyrsm-0.8.4/pyrsm/data/model/dvd.pkl
+-rw-r--r--   0 root         (0) staff       (20)     4468 2022-02-13 01:24:09.000000 pyrsm-0.8.4/pyrsm/data/model/houseprices.pkl
+-rw-r--r--   0 root         (0) staff       (20)    33206 2022-02-13 01:24:09.000000 pyrsm-0.8.4/pyrsm/data/model/ideal.pkl
+-rw-r--r--   0 root         (0) staff       (20)   126402 2022-02-13 01:24:09.000000 pyrsm-0.8.4/pyrsm/data/model/ketchup.pkl
+-rw-r--r--   0 root         (0) staff       (20)      315 2022-02-13 01:24:09.000000 pyrsm-0.8.4/pyrsm/data/model/movie_contract.pkl
+-rw-r--r--   0 root         (0) staff       (20)     3123 2022-02-13 01:24:09.000000 pyrsm-0.8.4/pyrsm/data/model/ratings.pkl
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-26 01:12:48.099609 pyrsm-0.8.4/pyrsm/data/multivariate/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.4/pyrsm/data/multivariate/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     3125 2022-02-13 01:24:09.000000 pyrsm-0.8.4/pyrsm/data/multivariate/carpet.pkl
+-rw-r--r--   0 root         (0) staff       (20)     2423 2022-02-13 01:24:09.000000 pyrsm-0.8.4/pyrsm/data/multivariate/city.pkl
+-rw-r--r--   0 root         (0) staff       (20)     3923 2022-02-13 01:24:09.000000 pyrsm-0.8.4/pyrsm/data/multivariate/city2.pkl
+-rw-r--r--   0 root         (0) staff       (20)     2625 2022-02-13 01:24:09.000000 pyrsm-0.8.4/pyrsm/data/multivariate/computer.pkl
+-rw-r--r--   0 root         (0) staff       (20)     3442 2022-02-13 01:24:09.000000 pyrsm-0.8.4/pyrsm/data/multivariate/movie.pkl
+-rw-r--r--   0 root         (0) staff       (20)     2994 2022-02-13 01:24:09.000000 pyrsm-0.8.4/pyrsm/data/multivariate/mp3.pkl
+-rw-r--r--   0 root         (0) staff       (20)     3278 2022-02-13 01:24:09.000000 pyrsm-0.8.4/pyrsm/data/multivariate/retailers.pkl
+-rw-r--r--   0 root         (0) staff       (20)     2357 2022-02-13 01:24:09.000000 pyrsm-0.8.4/pyrsm/data/multivariate/shopping.pkl
+-rw-r--r--   0 root         (0) staff       (20)     4872 2022-02-13 01:24:09.000000 pyrsm-0.8.4/pyrsm/data/multivariate/toothpaste.pkl
+-rw-r--r--   0 root         (0) staff       (20)     3678 2022-02-13 01:24:09.000000 pyrsm-0.8.4/pyrsm/data/multivariate/tpbrands.pkl
+-rw-r--r--   0 root         (0) staff       (20)     1966 2023-01-26 08:23:23.000000 pyrsm-0.8.4/pyrsm/example_data.py
+-rw-r--r--   0 root         (0) staff       (20)     5271 2023-05-07 05:21:24.000000 pyrsm-0.8.4/pyrsm/logit.py
+-rw-r--r--   0 root         (0) staff       (20)    25270 2023-05-21 21:48:34.000000 pyrsm-0.8.4/pyrsm/model.py
+-rw-r--r--   0 root         (0) staff       (20)     2214 2023-05-15 20:48:14.000000 pyrsm-0.8.4/pyrsm/notebook.py
+-rw-r--r--   0 root         (0) staff       (20)    37519 2023-04-16 05:51:16.000000 pyrsm-0.8.4/pyrsm/perf.py
+-rw-r--r--   0 root         (0) staff       (20)     1835 2022-02-13 01:24:09.000000 pyrsm-0.8.4/pyrsm/props.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-26 01:12:48.100557 pyrsm-0.8.4/pyrsm/radiant/
+-rw-r--r--   0 root         (0) staff       (20)       23 2023-05-18 03:04:58.000000 pyrsm-0.8.4/pyrsm/radiant/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     9489 2023-05-15 05:18:12.000000 pyrsm-0.8.4/pyrsm/radiant/logit.py
+-rw-r--r--   0 root         (0) staff       (20)    20280 2023-05-24 04:40:42.000000 pyrsm-0.8.4/pyrsm/radiant/regress.py
+-rw-r--r--   0 root         (0) staff       (20)     1200 2023-05-23 03:10:54.000000 pyrsm-0.8.4/pyrsm/radiant/utils.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-26 01:12:48.101091 pyrsm-0.8.4/pyrsm/radiant/www/
+-rw-r--r--   0 root         (0) staff       (20)      230 2023-05-11 03:12:37.000000 pyrsm-0.8.4/pyrsm/radiant/www/copy.js
+-rw-r--r--   0 root         (0) staff       (20)     1964 2023-05-23 02:45:36.000000 pyrsm-0.8.4/pyrsm/radiant/www/returnTextAreaBinding.js
+-rw-r--r--   0 root         (0) staff       (20)     3597 2023-05-11 03:12:22.000000 pyrsm-0.8.4/pyrsm/radiant/www/style.css
+-rw-r--r--   0 root         (0) staff       (20)     9296 2023-05-24 09:09:52.000000 pyrsm-0.8.4/pyrsm/regress.py
+-rw-r--r--   0 root         (0) staff       (20)     5411 2023-03-27 22:17:11.000000 pyrsm-0.8.4/pyrsm/stats.py
+-rw-r--r--   0 root         (0) staff       (20)    10313 2023-05-14 21:06:56.000000 pyrsm-0.8.4/pyrsm/utils.py
+-rw-r--r--   0 root         (0) staff       (20)    22603 2023-05-22 00:34:13.000000 pyrsm-0.8.4/pyrsm/visualize.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-26 01:12:48.092366 pyrsm-0.8.4/pyrsm.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)      592 2023-05-26 01:12:48.000000 pyrsm-0.8.4/pyrsm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     1838 2023-05-26 01:12:48.000000 pyrsm-0.8.4/pyrsm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-05-26 01:12:48.000000 pyrsm-0.8.4/pyrsm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)      208 2023-05-26 01:12:48.000000 pyrsm-0.8.4/pyrsm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)        6 2023-05-26 01:12:48.000000 pyrsm-0.8.4/pyrsm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)     1019 2023-05-26 01:12:48.104154 pyrsm-0.8.4/setup.cfg
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-26 01:12:48.103514 pyrsm-0.8.4/tests/
+-rw-r--r--   0 root         (0) staff       (20)      722 2023-05-16 05:24:37.000000 pyrsm-0.8.4/tests/test_basics.py
+-rw-r--r--   0 root         (0) staff       (20)     1072 2023-03-05 06:28:28.000000 pyrsm-0.8.4/tests/test_bins.py
+-rw-r--r--   0 root         (0) staff       (20)      794 2023-05-16 05:39:55.000000 pyrsm-0.8.4/tests/test_example_data.py
+-rw-r--r--   0 root         (0) staff       (20)     2756 2023-01-21 01:15:24.000000 pyrsm-0.8.4/tests/test_perf.py
+-rw-r--r--   0 root         (0) staff       (20)      615 2023-05-16 05:41:07.000000 pyrsm-0.8.4/tests/test_regression.py
+-rw-r--r--   0 root         (0) staff       (20)     2036 2023-03-05 06:38:03.000000 pyrsm-0.8.4/tests/test_stats.py
+-rw-r--r--   0 root         (0) staff       (20)     1979 2022-02-13 01:24:09.000000 pyrsm-0.8.4/tests/test_utils.py
```

### Comparing `pyrsm-0.8.3/LICENSE` & `pyrsm-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.3/PKG-INFO` & `pyrsm-0.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrsm
-Version: 0.8.3
+Version: 0.8.4
 Summary: Python functions for Customer Analytics at the Rady School of Management (RSM)
 Author: Vincent Nijs <vnijs@ucsd.edu>, Vikram Jambulapati <vikjam@ucsd.edu>, Suhas Goutham <sgoutham@ucsd.edu>, Raghav Prasad <rprasad@ucsd.edu>
 Author-email: vnijs@ucsd.edu
 License: AGPL-3.0-only
 Project-URL: Bug Reports, https://github.com/vnijs/pyrsm/issues
 Project-URL: Source, https://github.com/vnijs/pyrsm
 Description-Content-Type: text/markdown
```

### Comparing `pyrsm-0.8.3/README.md` & `pyrsm-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.3/pyrsm/basics.py` & `pyrsm-0.8.4/pyrsm/basics.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.3/pyrsm/bins.py` & `pyrsm-0.8.4/pyrsm/bins.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.3/pyrsm/data/basics/consider.pkl` & `pyrsm-0.8.4/pyrsm/data/basics/consider.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.3/pyrsm/data/basics/demand_uk.pkl` & `pyrsm-0.8.4/pyrsm/data/basics/demand_uk.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.3/pyrsm/data/basics/newspaper.pkl` & `pyrsm-0.8.4/pyrsm/data/basics/newspaper.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.3/pyrsm/data/basics/salary.pkl` & `pyrsm-0.8.4/pyrsm/data/basics/salary.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.3/pyrsm/data/data/avengers.pkl` & `pyrsm-0.8.4/pyrsm/data/data/avengers.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.3/pyrsm/data/data/diamonds.pkl` & `pyrsm-0.8.4/pyrsm/data/data/diamonds.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.3/pyrsm/data/data/publishers.pkl` & `pyrsm-0.8.4/pyrsm/data/data/publishers.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.3/pyrsm/data/data/superheroes.pkl` & `pyrsm-0.8.4/pyrsm/data/data/superheroes.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.3/pyrsm/data/data/titanic.pkl` & `pyrsm-0.8.4/pyrsm/data/data/titanic.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.3/pyrsm/data/design/rndnames.pkl` & `pyrsm-0.8.4/pyrsm/data/design/rndnames.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.3/pyrsm/data/model/catalog.pkl` & `pyrsm-0.8.4/pyrsm/data/model/catalog.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.3/pyrsm/data/model/direct_marketing.pkl` & `pyrsm-0.8.4/pyrsm/data/model/direct_marketing.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.3/pyrsm/data/model/dvd.pkl` & `pyrsm-0.8.4/pyrsm/data/model/dvd.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.3/pyrsm/data/model/houseprices.pkl` & `pyrsm-0.8.4/pyrsm/data/model/houseprices.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.3/pyrsm/data/model/ideal.pkl` & `pyrsm-0.8.4/pyrsm/data/model/ideal.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.3/pyrsm/data/model/ketchup.pkl` & `pyrsm-0.8.4/pyrsm/data/model/ketchup.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.3/pyrsm/data/model/ratings.pkl` & `pyrsm-0.8.4/pyrsm/data/model/ratings.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.3/pyrsm/data/multivariate/carpet.pkl` & `pyrsm-0.8.4/pyrsm/data/multivariate/carpet.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.3/pyrsm/data/multivariate/city.pkl` & `pyrsm-0.8.4/pyrsm/data/multivariate/city.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.3/pyrsm/data/multivariate/city2.pkl` & `pyrsm-0.8.4/pyrsm/data/multivariate/city2.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.3/pyrsm/data/multivariate/computer.pkl` & `pyrsm-0.8.4/pyrsm/data/multivariate/computer.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.3/pyrsm/data/multivariate/movie.pkl` & `pyrsm-0.8.4/pyrsm/data/multivariate/movie.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.3/pyrsm/data/multivariate/mp3.pkl` & `pyrsm-0.8.4/pyrsm/data/multivariate/mp3.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.3/pyrsm/data/multivariate/retailers.pkl` & `pyrsm-0.8.4/pyrsm/data/multivariate/retailers.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.3/pyrsm/data/multivariate/shopping.pkl` & `pyrsm-0.8.4/pyrsm/data/multivariate/shopping.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.3/pyrsm/data/multivariate/toothpaste.pkl` & `pyrsm-0.8.4/pyrsm/data/multivariate/toothpaste.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.3/pyrsm/data/multivariate/tpbrands.pkl` & `pyrsm-0.8.4/pyrsm/data/multivariate/tpbrands.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.3/pyrsm/example_data.py` & `pyrsm-0.8.4/pyrsm/example_data.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.3/pyrsm/logit.py` & `pyrsm-0.8.4/pyrsm/logit.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.3/pyrsm/model.py` & `pyrsm-0.8.4/pyrsm/model.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.3/pyrsm/notebook.py` & `pyrsm-0.8.4/pyrsm/notebook.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.3/pyrsm/perf.py` & `pyrsm-0.8.4/pyrsm/perf.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.3/pyrsm/props.py` & `pyrsm-0.8.4/pyrsm/props.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.3/pyrsm/radiant/logit.py` & `pyrsm-0.8.4/pyrsm/radiant/logit.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.3/pyrsm/radiant/regress.py` & `pyrsm-0.8.4/pyrsm/radiant/regress.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 from shiny import App, render, ui, reactive, Inputs, Outputs, Session
-
-# from htmltools import TagList, tags, div, css
 from faicons import icon_svg
 import webbrowser, nest_asyncio, uvicorn
 import io, os, signal, black
 from pathlib import Path
 import pyrsm as rsm
 import pandas as pd
 from contextlib import redirect_stdout
@@ -13,15 +11,14 @@
 from .utils import *
 
 # from itables import to_html_datatable as DT
 
 
 ## next steps
 ## try qgrid for interactive data table
-## shown description as markdown https://shinylive.io/py/examples/#extra-packages
 
 
 class model_regress:
     def __init__(self, datasets) -> None:
         self.datasets = rsm.ifelse(
             isinstance(datasets, dict), datasets, {"dataset": datasets}
         )
@@ -46,29 +43,26 @@
                     ),
                     ui.panel_conditional(
                         "input.tabs_regress == 'Data'",
                         ui.panel_well(
                             ui.input_checkbox("show_filter", "Show data filter"),
                             ui.panel_conditional(
                                 "input.show_filter == true",
-                                # ui.input_text_area(
                                 input_return_text_area(
                                     "data_filter",
                                     "Data Filter:",
                                     rows=2,
                                     placeholder="Provide a filter (e.g., price >  5000) and press return",
                                 ),
-                                # ui.input_text_area(
                                 input_return_text_area(
                                     "data_arrange",
                                     "Data arrange (sort):",
                                     rows=2,
                                     placeholder="Arrange (e.g., ['color', 'price'], ascending=[True, False])) and press return",
                                 ),
-                                # ui.input_text_area(
                                 input_return_text_area(
                                     "data_slice",
                                     "Data slice (rows):",
                                     rows=1,
                                     placeholder="e.g., 1:50 and press return",
                                 ),
                             ),
@@ -94,26 +88,25 @@
                                 choices={0: "None", 2: "2-way", 3: "3-way"},
                                 inline=True,
                             ),
                             ui.panel_conditional(
                                 "input.show_interactions > 0",
                                 ui.output_ui("ui_interactions"),
                             ),
-                            width=3,
-                        ),
-                        ui.panel_well(
+                            ui.output_ui("ui_evar_test"),
                             ui.input_checkbox_group(
                                 "controls",
-                                "Controls:",
+                                "Additional output:",
                                 {
                                     "ci": "Confidence intervals",
                                     "ssq": "Sum of Squares",
                                     "vif": "VIF",
                                 },
-                            )
+                            ),
+                            width=3,
                         ),
                     ),
                     ui.panel_conditional(
                         "input.tabs_regress == 'Predict'",
                         ui.panel_well(
                             ui.input_select(
                                 "pred_datasets", "Prediction data:", self.dataset_list
@@ -237,15 +230,15 @@
                 "isCat": isCat,
             }
 
             return (
                 data,
                 data_name,
                 var_types,
-                f"# {data_name} = pd.read_pickle('{data_name}.pkl')",
+                f"import pyrsm as rsm\n# {data_name} = pd.read_pickle('{data_name}.pkl')",
             )
 
         @output(id="show_data_code")
         @render.ui
         def show_data_code():
             fname, _, code = get_data()[1:]
             if input.show_filter():
@@ -326,21 +319,31 @@
                     selected=None,
                     choices=choices,
                     multiple=True,
                     size=min(8, len(choices)),
                     selectize=False,
                 )
 
+        @output(id="ui_evar_test")
+        @render.ui
+        def ui_evar_test():
+            return ui.input_select(
+                id="ui_evar_test",
+                label="Variables to test:",
+                placeholder="Select variables to test",
+                choices=[None, input.evar()],
+            )
+
         @output(id="ui_incl_evar")
         @render.ui
         def ui_incl_evar():
             if len(input.evar()) > 1:
                 return ui.input_select(
                     id="incl_evar",
-                    label="Explanatory variables to include",
+                    label="Explanatory variables to include:",
                     selected=None,
                     choices=input.evar(),
                     multiple=True,
                     size=min(8, len(input.evar())),
                     selectize=False,
                 )
 
@@ -348,15 +351,15 @@
         @render.ui
         def ui_incl_interactions():
             if len(input.evar()) > 1:
                 nway = int(input.show_interactions())
                 choices = iterms(input.evar(), nway=nway)
                 return ui.input_select(
                     id="incl_interactions",
-                    label="Interactions to include",
+                    label="Interactions to include:",
                     selected=None,
                     choices=choices,
                     multiple=True,
                     size=min(8, len(choices)),
                     selectize=False,
                 )
 
@@ -500,13 +503,16 @@
     """
     Launch a Shiny-for-Python app for regression analysis
     """
     mr = model_regress(data_dct)
     nest_asyncio.apply()
     webbrowser.open(f"http://{host}:{port}")
     print(f"Listening on http://{host}:{port}")
+    print(
+        "Pyrsm and Radiant are opensource tools and free to use. If you\nare a student or instructor using pyrsm or Radiant for a class,\nas a favor to the developers, please send an email to\n<radiant@rady.ucsd.edu> with the name of the school and class."
+    )
     uvicorn.run(
         App(mr.shiny_ui(), mr.shiny_server),
         host=host,
         port=port,
         log_level=log_level,
     )
```

### Comparing `pyrsm-0.8.3/pyrsm/radiant/utils.py` & `pyrsm-0.8.4/pyrsm/radiant/utils.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.3/pyrsm/radiant/www/returnTextAreaBinding.js` & `pyrsm-0.8.4/pyrsm/radiant/www/returnTextAreaBinding.js`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.3/pyrsm/radiant/www/style.css` & `pyrsm-0.8.4/pyrsm/radiant/www/style.css`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.3/pyrsm/regress.py` & `pyrsm-0.8.4/pyrsm/regress.py`

 * *Files 10% similar despite different names*

```diff
@@ -52,26 +52,33 @@
         if self.form:
             self.fitted = smf.ols(formula=self.form, data=self.dataset).fit()
             self.evar = extract_evars(self.fitted.model, self.dataset.columns)
             self.rvar = extract_rvar(self.fitted.model, self.dataset.columns)
         else:
             self.form = f"{self.rvar} ~ {' + '.join(self.evar)}"
             if self.int:
-                self.form += f"+ {' + '.join(self.int)}"
+                self.form += f" + {' + '.join(self.int)}"
             self.fitted = smf.ols(self.form, data=self.dataset).fit()
 
         df = pd.DataFrame(self.fitted.params, columns=["coefficient"]).dropna()
         df["std.error"] = self.fitted.params / self.fitted.tvalues
         df["t.value"] = self.fitted.tvalues
         df["p.value"] = self.fitted.pvalues
         df["  "] = sig_stars(self.fitted.pvalues)
         self.coef = df.reset_index()
 
     def summary(
-        self, ssq=False, vif=False, ci=False, dec=3, name="Not provided", shiny=False
+        self,
+        ssq=False,
+        vif=False,
+        ci=False,
+        test=None,
+        dec=3,
+        name="Not provided",
+        shiny=False,
     ) -> None:
         """
         Summarize output from a linear regression model
 
         parameters
         ----------
         ssq: Boolean; if True, include sum of squares
@@ -122,14 +129,57 @@
             )
             print(f"\n{sum_of_squares.to_string()}")
 
         if vif:
             print("\nVariance inflation factors:")
             print(f"\n{calc_vif(self.fitted).to_string()}")
 
+        if test is not None and len(test) > 0:
+            evar = setdiff(self.evar, test)
+            if self.int is not None and len(self.int) > 0:
+                sint = [
+                    s for s in self.int for t in test if f"I({t}" in s or t not in s
+                ]
+            else:
+                sint = []
+
+            form = f"{self.rvar} ~ "
+            if len(evar) == 0 and len(sint) == 0:
+                form += "1"
+            else:
+                # if len(evar) > 0:
+                # form += f"{' + '.join(evar)}"
+                # if len(sint) > 0:
+                form += f"{' + '.join(evar + sint)}"
+
+                ###### need to keep I(carat**2) in the formula even if carat is in test ######
+
+                # if self.int is not None and len(self.int) > 0:
+                #     sint = [
+                #         s for s in self.int for t in test if f"I({t}" in s or t not in s
+                #     ]
+                #     if len(sint) > 0:
+                #         form += f" + {' + '.join(sint)}"
+
+            hypothesis = [
+                f"({c} = 0)"
+                for c in self.fitted.model.exog_names
+                for v in test
+                if f"{v}:" in c or f":{v}" in c or f"{v}[T." in c or v == c
+            ]
+            print(hypothesis)
+
+            print(f"\nModel 1: {form}")
+            print(f"Model 2: {self.form}")
+            out = self.fitted.f_test(hypothesis)
+            pvalue = ifelse(out.pvalue < 0.001, "< .001", round(out.pvalue, dec))
+            print(
+                f"F-statistic: {round(out.fvalue, dec)} df ({out.df_num:.0f}, {out.df_denom:.0f}), p.value {pvalue}"
+            )
+
     def predict(self, df=None, ci=False, alpha=0.05) -> pd.DataFrame:
         """
         Predict values for a linear regression model
         """
         if df is None:
             df = self.dataset
         df = df.loc[:, self.evar].copy()
```

### Comparing `pyrsm-0.8.3/pyrsm/stats.py` & `pyrsm-0.8.4/pyrsm/stats.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.3/pyrsm/utils.py` & `pyrsm-0.8.4/pyrsm/utils.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.3/pyrsm/visualize.py` & `pyrsm-0.8.4/pyrsm/visualize.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.3/pyrsm.egg-info/PKG-INFO` & `pyrsm-0.8.4/pyrsm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrsm
-Version: 0.8.3
+Version: 0.8.4
 Summary: Python functions for Customer Analytics at the Rady School of Management (RSM)
 Author: Vincent Nijs <vnijs@ucsd.edu>, Vikram Jambulapati <vikjam@ucsd.edu>, Suhas Goutham <sgoutham@ucsd.edu>, Raghav Prasad <rprasad@ucsd.edu>
 Author-email: vnijs@ucsd.edu
 License: AGPL-3.0-only
 Project-URL: Bug Reports, https://github.com/vnijs/pyrsm/issues
 Project-URL: Source, https://github.com/vnijs/pyrsm
 Description-Content-Type: text/markdown
```

### Comparing `pyrsm-0.8.3/pyrsm.egg-info/SOURCES.txt` & `pyrsm-0.8.4/pyrsm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.3/setup.cfg` & `pyrsm-0.8.4/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 	Source=https://github.com/vnijs/pyrsm
 
 [options]
 include_package_data = True
 packages = find:
 install_requires = 
 	shiny>=0.3.3
+	faicons>=0.2.1
 	numpy>=1.17.3
 	pandas>=0.25.2
 	polars>=0.17.14
 	seaborn>=0.9.0
 	matplotlib>=3.1.1
 	statsmodels>=0.10.1
 	scipy>=1.4.1
```

### Comparing `pyrsm-0.8.3/tests/test_basics.py` & `pyrsm-0.8.4/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.3/tests/test_bins.py` & `pyrsm-0.8.4/tests/test_bins.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.3/tests/test_example_data.py` & `pyrsm-0.8.4/tests/test_example_data.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.3/tests/test_perf.py` & `pyrsm-0.8.4/tests/test_perf.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.3/tests/test_regression.py` & `pyrsm-0.8.4/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.3/tests/test_stats.py` & `pyrsm-0.8.4/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.3/tests/test_utils.py` & `pyrsm-0.8.4/tests/test_utils.py`

 * *Files identical despite different names*

