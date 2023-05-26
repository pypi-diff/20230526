# Comparing `tmp/xemc3-0.2.4.tar.gz` & `tmp/xemc3-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xemc3-0.2.4.tar", last modified: Fri Apr 21 06:56:10 2023, max compression
+gzip compressed data, was "xemc3-0.2.5.tar", last modified: Fri May 26 13:00:01 2023, max compression
```

## Comparing `xemc3-0.2.4.tar` & `xemc3-0.2.5.tar`

### file list

```diff
@@ -1,87 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:56:10.568656 xemc3-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-21 06:55:53.000000 xemc3-0.2.4/.codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:56:10.556656 xemc3-0.2.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:56:10.560656 xemc3-0.2.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-21 06:55:53.000000 xemc3-0.2.4/.github/workflows/black-fix.yml
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-21 06:55:53.000000 xemc3-0.2.4/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-21 06:55:53.000000 xemc3-0.2.4/.github/workflows/python_publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-21 06:55:53.000000 xemc3-0.2.4/.github/workflows/test-python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-21 06:55:53.000000 xemc3-0.2.4/.github/workflows/zenodo.yml
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-21 06:55:53.000000 xemc3-0.2.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-21 06:55:53.000000 xemc3-0.2.4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-21 06:55:53.000000 xemc3-0.2.4/.zenodo.json
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-21 06:55:53.000000 xemc3-0.2.4/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-21 06:55:53.000000 xemc3-0.2.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-04-21 06:56:10.568656 xemc3-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-21 06:55:53.000000 xemc3-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:56:10.560656 xemc3-0.2.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-21 06:55:53.000000 xemc3-0.2.4/docs/citing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-21 06:55:53.000000 xemc3-0.2.4/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-21 06:55:53.000000 xemc3-0.2.4/docs/cli.rst.in.py
--rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-04-21 06:55:53.000000 xemc3-0.2.4/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:56:10.560656 xemc3-0.2.4/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-04-21 06:55:53.000000 xemc3-0.2.4/docs/examples/evaluate_at.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-21 06:55:53.000000 xemc3-0.2.4/docs/examples/get_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-21 06:55:53.000000 xemc3-0.2.4/docs/examples/heatflux.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-04-21 06:55:53.000000 xemc3-0.2.4/docs/examples/info.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12317 2023-04-21 06:55:53.000000 xemc3-0.2.4/docs/examples/introduction.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-21 06:55:53.000000 xemc3-0.2.4/docs/examples/load1.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-04-21 06:55:53.000000 xemc3-0.2.4/docs/examples/load2.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-21 06:55:53.000000 xemc3-0.2.4/docs/examples/setup_plt.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-21 06:55:53.000000 xemc3-0.2.4/docs/examples.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:56:10.560656 xemc3-0.2.4/docs/exercises/
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-21 06:55:53.000000 xemc3-0.2.4/docs/exercises/get_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8773 2023-04-21 06:55:53.000000 xemc3-0.2.4/docs/exercises/introduction.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-21 06:55:53.000000 xemc3-0.2.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-04-21 06:55:53.000000 xemc3-0.2.4/docs/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-21 06:55:53.000000 xemc3-0.2.4/docs/xarray.rst
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-21 06:55:53.000000 xemc3-0.2.4/docs/xemc3.rst
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-21 06:55:53.000000 xemc3-0.2.4/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-21 06:55:53.000000 xemc3-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-21 06:55:53.000000 xemc3-0.2.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-04-21 06:56:10.568656 xemc3-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-21 06:55:53.000000 xemc3-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:56:10.560656 xemc3-0.2.4/xemc3/
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-21 06:56:10.000000 xemc3-0.2.4/xemc3/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:56:10.564656 xemc3-0.2.4/xemc3/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/cli/_common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1465 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/cli/append_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/cli/to_archive.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      887 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/cli/to_netcdf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3698 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/cli/xdivertor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:56:10.564656 xemc3-0.2.4/xemc3/core/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20437 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/core/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/core/depo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/core/evaluate_at.py
--rw-r--r--   0 runner    (1001) docker     (123)    66317 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/core/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/core/plot_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    10401 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/core/plot_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:56:10.564656 xemc3-0.2.4/xemc3/load/
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/load/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:56:10.564656 xemc3-0.2.4/xemc3/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9446 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/test/gen_ds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/test/test_average.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/test/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/test/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    15461 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/test/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/test/test_load_real.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/test/test_write_load.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:56:10.564656 xemc3-0.2.4/xemc3/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     9653 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/tools/run_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:56:10.568656 xemc3-0.2.4/xemc3/write/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/write/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/write/fortran.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/write/nc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:56:10.564656 xemc3-0.2.4/xemc3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-04-21 06:56:10.000000 xemc3-0.2.4/xemc3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-04-21 06:56:10.000000 xemc3-0.2.4/xemc3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 06:56:10.000000 xemc3-0.2.4/xemc3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-21 06:56:10.000000 xemc3-0.2.4/xemc3.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-21 06:56:10.000000 xemc3-0.2.4/xemc3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-21 06:56:10.000000 xemc3-0.2.4/xemc3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:00:01.296853 xemc3-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 12:59:40.000000 xemc3-0.2.5/.codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:00:01.288853 xemc3-0.2.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:00:01.288853 xemc3-0.2.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-26 12:59:40.000000 xemc3-0.2.5/.github/workflows/black-fix.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-26 12:59:40.000000 xemc3-0.2.5/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-26 12:59:40.000000 xemc3-0.2.5/.github/workflows/python_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-26 12:59:40.000000 xemc3-0.2.5/.github/workflows/test-python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-26 12:59:40.000000 xemc3-0.2.5/.github/workflows/version-yaml.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-26 12:59:40.000000 xemc3-0.2.5/.github/workflows/zenodo.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-26 12:59:40.000000 xemc3-0.2.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-26 12:59:40.000000 xemc3-0.2.5/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-26 12:59:40.000000 xemc3-0.2.5/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-26 12:59:40.000000 xemc3-0.2.5/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-26 12:59:40.000000 xemc3-0.2.5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-05-26 13:00:01.296853 xemc3-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-26 12:59:40.000000 xemc3-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:00:01.288853 xemc3-0.2.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-26 12:59:40.000000 xemc3-0.2.5/docs/citing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-26 12:59:40.000000 xemc3-0.2.5/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-26 12:59:40.000000 xemc3-0.2.5/docs/cli.rst.in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-05-26 12:59:40.000000 xemc3-0.2.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-05-26 12:59:40.000000 xemc3-0.2.5/docs/config.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:00:01.292853 xemc3-0.2.5/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-05-26 12:59:40.000000 xemc3-0.2.5/docs/examples/evaluate_at.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-26 12:59:40.000000 xemc3-0.2.5/docs/examples/get_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-05-26 12:59:40.000000 xemc3-0.2.5/docs/examples/heatflux.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-05-26 12:59:40.000000 xemc3-0.2.5/docs/examples/info.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12317 2023-05-26 12:59:40.000000 xemc3-0.2.5/docs/examples/introduction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-26 12:59:40.000000 xemc3-0.2.5/docs/examples/load1.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-05-26 12:59:40.000000 xemc3-0.2.5/docs/examples/load2.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-26 12:59:40.000000 xemc3-0.2.5/docs/examples/setup_plt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-26 12:59:40.000000 xemc3-0.2.5/docs/examples.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:00:01.292853 xemc3-0.2.5/docs/exercises/
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-26 12:59:40.000000 xemc3-0.2.5/docs/exercises/get_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8773 2023-05-26 12:59:40.000000 xemc3-0.2.5/docs/exercises/introduction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-05-26 12:59:40.000000 xemc3-0.2.5/docs/filenames.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-26 12:59:40.000000 xemc3-0.2.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-05-26 12:59:40.000000 xemc3-0.2.5/docs/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-26 12:59:40.000000 xemc3-0.2.5/docs/xarray.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-26 12:59:40.000000 xemc3-0.2.5/docs/xemc3.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-26 12:59:40.000000 xemc3-0.2.5/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-26 12:59:40.000000 xemc3-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-26 12:59:40.000000 xemc3-0.2.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-26 13:00:01.296853 xemc3-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-26 12:59:40.000000 xemc3-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:00:01.292853 xemc3-0.2.5/xemc3/
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-26 13:00:00.000000 xemc3-0.2.5/xemc3/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:00:01.292853 xemc3-0.2.5/xemc3/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/cli/_common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1465 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/cli/append_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/cli/to_archive.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      887 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/cli/to_netcdf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3698 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/cli/xdivertor.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:00:01.292853 xemc3-0.2.5/xemc3/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21282 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/core/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/core/depo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/core/evaluate_at.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56312 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/core/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/core/plot_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10401 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/core/plot_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:00:01.292853 xemc3-0.2.5/xemc3/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/data/default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/data/v0.2.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/data/v0.2.1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/data/v0.2.2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/data/v0.2.3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/data/v0.2.4.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/data/v0.2.5.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:00:01.292853 xemc3-0.2.5/xemc3/load/
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/load/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:00:01.296853 xemc3-0.2.5/xemc3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9446 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/test/gen_ds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/test/test_average.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/test/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/test/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15461 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/test/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/test/test_load_real.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/test/test_write_load.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:00:01.296853 xemc3-0.2.5/xemc3/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     9653 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/tools/run_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:00:01.296853 xemc3-0.2.5/xemc3/write/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/write/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/write/fortran.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/write/nc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:00:01.292853 xemc3-0.2.5/xemc3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-05-26 13:00:01.000000 xemc3-0.2.5/xemc3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-26 13:00:01.000000 xemc3-0.2.5/xemc3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 13:00:01.000000 xemc3-0.2.5/xemc3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-26 13:00:01.000000 xemc3-0.2.5/xemc3.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-26 13:00:01.000000 xemc3-0.2.5/xemc3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-26 13:00:01.000000 xemc3-0.2.5/xemc3.egg-info/top_level.txt
```

### Comparing `xemc3-0.2.4/.github/workflows/black-fix.yml` & `xemc3-0.2.5/.github/workflows/black-fix.yml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     shell: bash
 
 jobs:
   black:
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
       with:
         ref: ${{ github.head_ref }}
 
     - name: Installing black
       run: |
         sudo apt update -y
         sudo apt -y install python3-pip python3-setuptools python3-wheel
```

### Comparing `xemc3-0.2.4/.github/workflows/python_publish.yml` & `xemc3-0.2.5/.github/workflows/python_publish.yml`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,17 @@
   release:
     types: [created]
 
 jobs:
   deploy:
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v1
+    - uses: actions/checkout@v3
     - name: Set up Python
-      uses: actions/setup-python@v1
+      uses: actions/setup-python@v2
       with:
         python-version: '3.x'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install setuptools wheel twine
     - name: Build and publish
```

### Comparing `xemc3-0.2.4/.github/workflows/test-python-package.yml` & `xemc3-0.2.5/.github/workflows/test-python-package.yml`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         extra-install: ["", "numba"]
         exclude:
           - python-version: '3.11'
             extra-install: 'numba'
       fail-fast: false
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Get Remote SHA
       id: get-sha
       run: |
         echo "sha=$(git ls-remote https://oauth2:uQ7_vw_m5fo4UFQrenUs@gitlab.mpcdf.mpg.de/dave/xemc3-data.git HEAD|cut -c -20)" >> $GITHUB_OUTPUT
     - name: Cache example data
       id: cache-example
       uses: actions/cache@v2
```

### Comparing `xemc3-0.2.4/COPYING` & `xemc3-0.2.5/COPYING`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.4/Makefile` & `xemc3-0.2.5/Makefile`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.4/PKG-INFO` & `xemc3-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xemc3
-Version: 0.2.4
+Version: 0.2.5
 Summary: Collect data from EMC3 runs in python using xarray
 Home-page: https://github.com/dschwoerer/xemc3
 Author: David Bold
 Author-email: dave@ipp.mpg.de
 License: GPL
 Project-URL: Tracker, https://github.com/dschwoerer/xemc3/issues
 Project-URL: Documentation, https://xemc3.rtfd.io
```

### Comparing `xemc3-0.2.4/README.md` & `xemc3-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.4/docs/cli.rst.in.py` & `xemc3-0.2.5/docs/cli.rst.in.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.4/docs/conf.py` & `xemc3-0.2.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.4/docs/examples/evaluate_at.ipynb` & `xemc3-0.2.5/docs/examples/evaluate_at.ipynb`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.4/docs/examples/get_data.py` & `xemc3-0.2.5/docs/examples/get_data.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.4/docs/examples/heatflux.ipynb` & `xemc3-0.2.5/docs/examples/heatflux.ipynb`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.4/docs/examples/info.ipynb` & `xemc3-0.2.5/docs/examples/info.ipynb`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.4/docs/examples/introduction.ipynb` & `xemc3-0.2.5/docs/examples/introduction.ipynb`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.4/docs/examples/load1.ipynb` & `xemc3-0.2.5/docs/examples/load1.ipynb`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.4/docs/examples/load2.ipynb` & `xemc3-0.2.5/docs/examples/load2.ipynb`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.4/docs/exercises/get_data.py` & `xemc3-0.2.5/docs/exercises/get_data.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.4/docs/exercises/introduction.ipynb` & `xemc3-0.2.5/docs/exercises/introduction.ipynb`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.4/docs/index.rst` & `xemc3-0.2.5/docs/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,16 @@
    :maxdepth: 2
    :caption: Contents:
 
    introduction
    examples
    xemc3
    xarray
+   config
+   filenames
    cli
    citing
 
 Installation
 ------------
 
 With ``pip``:
```

### Comparing `xemc3-0.2.4/docs/introduction.rst` & `xemc3-0.2.5/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.4/docs/xarray.rst` & `xemc3-0.2.5/docs/xarray.rst`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.4/docs/xemc3.rst` & `xemc3-0.2.5/docs/xemc3.rst`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.4/requirements.txt` & `xemc3-0.2.5/requirements.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 xarray>=0.16.0
 
 netcdf4>=1.4.0
 importlib-metadata<4.3,>=1.1.0; python_version < "3.8"
 numpy >= 1.13.0
 eudist
+pyyaml
 
 # for version number in non-installed package:
 setuptools>=42
 setuptools_scm[toml]>=3.4
 
 # for tests
 pytest>=3.3.0
```

### Comparing `xemc3-0.2.4/setup.cfg` & `xemc3-0.2.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 [options]
 setup_requires = 
 	setuptools>=42
 	setuptools_scm[toml]>=3.4
 	setuptools_scm_git_archive
 install_requires = 
 	xarray>=0.16.0
-	matplotlib>=3.1.1,!=3.3.0,!=3.3.1,!=3.3.2
 	netcdf4>=1.4.0
 	importlib-metadata; python_version < "3.8"
 	numpy >= 1.13.0
 	eudist
+	pyyaml
 tests_require = 
 	pytest >= 3.3.0
 	mayavi
 	vtk !=9.0.3, !=9.0.2
 	matplotlib
 	coverage
 include_package_data = True
```

### Comparing `xemc3-0.2.4/xemc3/__init__.py` & `xemc3-0.2.5/xemc3/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 A python library for reading EMC3 simulation as xarray data.
 
 Additionally also provides some basic routines for plotting and
 analysing the data. The data is mostly in SI units, with the exception
 of temperatures that are in eV.
 """
 
-__all__ = ["load", "utils", "write"]
+__all__ = ["load", "write", "config"]
 
-from . import load, write
+from . import load, write, config
 from .core.dataset import EMC3DatasetAccessor
 
 
 try:
     from importlib.metadata import (  # type: ignore
         PackageNotFoundError as _PackageNotFoundError,
         version as _version,
```

### Comparing `xemc3-0.2.4/xemc3/cli/_common.py` & `xemc3-0.2.5/xemc3/cli/_common.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.4/xemc3/cli/append_time.py` & `xemc3-0.2.5/xemc3/cli/append_time.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.4/xemc3/cli/to_archive.py` & `xemc3-0.2.5/xemc3/cli/to_archive.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.4/xemc3/cli/to_netcdf.py` & `xemc3-0.2.5/xemc3/cli/to_netcdf.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.4/xemc3/cli/xdivertor.py` & `xemc3-0.2.5/xemc3/cli/xdivertor.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.4/xemc3/core/dataset.py` & `xemc3-0.2.5/xemc3/core/dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,31 +57,54 @@
                     if getDA:
                         yield self.data[f"{d}_dims"]
                     else:
                         yield self.data[f"{d}_dims"].data
                 except KeyError:
                     yield None
 
-    def _get(self, var):
-        """Load a single var."""
+    def _get(self, var, crop=True, resolve=True):
+        """
+        Load a single var.
+
+        crop : bool
+            Remove nan data
+        resolve : bool
+            Check alternative names to get data
+        """
+        docrop = crop
         transform = identity
         try:
             dims = self.data[var].dims
         except KeyError as e:
+            if not resolve:
+                raise e
             if var.endswith("_corners"):
                 var_ = var[: -len("_corners")] + "_bounds"
                 try:
                     dims = self.data[var_].dims
                 except KeyError:
                     raise e
                 var = var_
                 transform = from_interval_no_checks
+            elif var.endswith("_bounds"):
+                var = var[: -len("_bounds")]
+                try:
+                    dims = self.data[var + "_corners"].dims
+                    var = var + "_corners"
+                except KeyError:
+                    try:
+                        dims = self.data[var].dims
+                    except KeyError:
+                        raise e
+                if not any(["_plus1" in x for x in dims]):
+                    raise e
+                transform = utils.to_interval
             else:
                 raise
-        if "plate_ind" in dims:
+        if docrop and "plate_ind" in dims:
             crop = list(self._get_crop(dims, skip=["plate_ind"]))
             ret = []
             for i in range(len(self.data["plate_ind"])):
                 slcr = tuple(
                     [slice(None) if j is None else slice(None, j[i]) for j in crop]
                 )
                 data = self.data.isel(plate_ind=i)
@@ -95,16 +118,19 @@
                     data[var].data[slcr],
                     dims=data[var].dims,
                     attrs=data[var].attrs,
                     # coords=coords,
                 )
                 ret.append(transform(data))
             return ret
-        crop = [slice(None, x) for x in self._get_crop(dims)]
-        data = self.data[var][tuple(crop)]
+        if docrop:
+            crop = [slice(None, x) for x in self._get_crop(dims)]
+            data = self.data[var][tuple(crop)]
+        else:
+            data = self.data[var]
         return transform(data)
 
     def _set(self, var, data):
         """Set a single variable."""
         transform = identity
         if var.endswith("_corners"):
             var = var[: -len("_corners")] + "_bounds"
@@ -173,16 +199,16 @@
             is accepted.
         """
         return self._set(var, data)
 
     def _get_alt_name(self, var_name, suffix=""):
         var_suffix = ["_bounds", "", "_plus1"]
         var_prefix = ["plate_", "_plate_", ""]
-        for extra_suffix in var_suffix:
-            for prefix in var_prefix:
+        for prefix in var_prefix:
+            for extra_suffix in var_suffix:
                 cur = prefix + var_name + extra_suffix + suffix
                 if cur in self.data:
                     return cur
         assert False, f"Didn't find variable for {var_name} coordinate!"
 
     def iter_plates(self, *, symmetry=False, segments=1):
         """
```

### Comparing `xemc3-0.2.4/xemc3/core/depo.py` & `xemc3-0.2.5/xemc3/core/depo.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.4/xemc3/core/evaluate_at.py` & `xemc3-0.2.5/xemc3/core/evaluate_at.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.4/xemc3/core/load.py` & `xemc3-0.2.5/xemc3/core/load.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import uuid
 
 import numpy as np
 import xarray as xr
 
 from .utils import from_interval, open, prod, rrange, timeit, to_interval, raise_issue
 from .depo import read_depo_raw, write_depo_raw
+from .config import files
 
 try:
     from numba import jit  # type: ignore
 except ImportError:
 
     def jit(x):
         return x
@@ -382,15 +383,15 @@
     -------
     xr.Dataset
         A dataset with the coordinates set
     """
     if ds is None:
         ds = xr.Dataset()
     assert isinstance(ds, xr.Dataset)
-    phi, r, z = read_locations_raw(path + "/GRID_3D_DATA")
+    phi, r, z = read_locations_raw(get_file_name(path, "geom"))
     ds = ds.assign_coords(
         {
             "R_bounds": to_interval(("r", "theta", "phi"), r),
             "z_bounds": to_interval(("r", "theta", "phi"), z),
             "phi_bounds": to_interval(("phi",), phi),
         }
     )
@@ -744,15 +745,15 @@
                 plate_prefix + "phi_bounds": corrs_da[2],
             }
             ds = xr.Dataset(coords=coords)  # type: ignore
             ds.coords[plate_prefix + "R_bounds"].attrs["units"] = "m"
             ds.coords[plate_prefix + "z_bounds"].attrs["units"] = "m"
             ds.coords[plate_prefix + "phi_bounds"].attrs["units"] = "radian"
 
-            vars = files["TARGET_PROFILES"]["vars"].copy()
+            vars = files[get_file_name(None, "target_flux")]["vars"].copy()
             for i, (l, meta) in enumerate(vars.items()):
                 ds[l] = (plate_prefix + "phi", plate_prefix + "x"), data[i] * meta.get(
                     "scale", 1
                 )
                 for k in meta:
                     ds[l].attrs[k] = meta[k]
             for i, l in enumerate(["tot_n", "tot_P"]):
@@ -821,15 +822,15 @@
     for var in dss[0]:
         ds[var] = merge(var)
         ds[var].attrs = dss[0][var].attrs
 
     return ds
 
 
-def load_plates(dir: str, fn: str = "TARGET_PROFILES") -> xr.Dataset:
+def load_plates(dir: str, fn: typing.Optional[str] = None) -> xr.Dataset:
     """
     Read the target heatflux mapping from EMC3 Postprocessing routine.
 
     Parameters
     ----------
     dir : str
         The location of the directory in which the files are to be read
@@ -838,14 +839,16 @@
         The name of the deposition file
 
     Returns
     -------
     xr.Dataset
         The read data
     """
+    if fn is None:
+        fn = get_file_name(None, "target_flux")
     if dir[-1] != "/":
         dir += "/"
     plates = read_plates_raw(dir, fn)
     return merge_blocks(plates)
 
 
 def write_plates(dir: str, plates: xr.Dataset) -> None:
@@ -894,15 +897,15 @@
         The target profiles
     """
     dir = _dir_of(dir)
 
     if cache:
         try:
             if os.path.getmtime(dir + "/TARGET_PROFILES.nc") > os.path.getmtime(
-                dir + "/TARGET_PROFILES"
+                get_file_name(dir, "target_flux")
             ):
                 return read_plates(dir)
         except OSError:
             pass
         data = load_plates(dir)
         write_plates(dir, data)
         return data
@@ -1052,15 +1055,15 @@
 
     """
 
     if isinstance(mapping, xr.Dataset):
         mapping = ensure_mapping(_dir_of(fn), mapping, fn=fn)
         mapping = mapping["_plasma_map"]
     if kinetic:
-        assert unmapped == False
+        assert unmapped is False
         max = np.max(mapping.data) + 1
     elif unmapped:
         max = mapping.attrs["numcells"]
     else:
         max = mapping.attrs["plasmacells"]
     firsts = []
     with open(fn) as f:
@@ -1098,15 +1101,17 @@
         for ijk in rrange(mapping.shape):
             mapid = mapdat[ijk]
             if mapid < max:
                 out[ijk] = raw[mapid]
         return xr.DataArray(data=out, dims=mapping.dims)
 
     def to_da_unmapped(raw):
-        return xr.DataArray(data=raw.reshape(mapping.shape), dims=mapping.dims)
+        return xr.DataArray(
+            data=raw.reshape(mapping.shape[::-1]).transpose(2, 1, 0), dims=mapping.dims
+        )
 
     to_da = to_da_unmapped if unmapped else to_da_mapped
     das = [to_da(raw) for raw in raws]
     if skip_first:
         for first, da in zip(firsts, das):
             da.attrs["print_before"] = first
     if squeeze and len(das) == 1:
@@ -1326,16 +1331,16 @@
                 assert d.attrs["print_before"] != ""
             else:
                 if "print_before" in d.attrs:
                     assert d.attrs["print_before"] == ""
     if not isinstance(datas, (list, tuple)):
         datas = [datas]
     if unmapped:
-        assert kinetic == False
-        out = [np.ravel(x) for x in datas]
+        assert kinetic is False
+        out = [np.ravel(x, order="F") for x in datas]
     else:
         out = [to_mapped(x, mapping, kinetic, dtype) for x in datas]
     with open(fn, "w") as f:
         for i, da in zip(out, datas):
             if "print_before" in da.attrs:
                 f.write(da.attrs["print_before"])
             if fmt is None:
@@ -1394,336 +1399,14 @@
     valid_entries = np.sum(np.isfinite(dat), axis=1)
     assert len(valid_entries) == fmtc
     with open(fn, "w") as f:
         for d in dat.T[-np.max(valid_entries) :]:
             f.write(fmt % tuple(d) + "\n")
 
 
-files: typing.Dict[str, typing.Dict[str, typing.Any]] = {
-    "fort.70": dict(type="mapping", vars={"_plasma_map": dict()}),
-    "fort.31": dict(
-        type="mapped",
-        skip_first=1,
-        kinetic=False,
-        vars={
-            "ne": dict(scale=1e6, units="m$^{-3}$", long_name="Electron density"),
-            "nZ%d": dict(scale=1e6, units="m$^{-3}$"),
-        },
-    ),
-    "fort.33": dict(type="mapped", vars={"M": dict(long_name="Mach number")}),
-    "fort.30": dict(
-        type="mapped",
-        vars={
-            "Te": dict(units="eV", long_name="Electron temperature"),
-            "Ti": dict(units="eV", long_name="Ion temperature"),
-        },
-    ),
-    "CONNECTION_LENGTH": dict(
-        type="mapped",
-        vars={"Lc": dict(scale=1e-2, units="m", long_name="Connection length")},
-    ),
-    "DENSITY_A": dict(
-        type="mapped",
-        kinetic=True,
-        vars=dict(
-            nH=dict(scale=1e6, units="m$^{-3}$", long_name="Atomic deuterium density")
-        ),
-    ),
-    "DENSITY_M": dict(
-        kinetic=True,
-        vars=dict(nH2=dict(scale=1e6, units="m$^{-3}$", long_name="D_2 density")),
-    ),
-    "DENSITY_I": dict(
-        kinetic=True,
-        vars={"nH2+": dict(scale=1e6, units="m$^{-3}$", long_name="D_2^+ density")},
-    ),
-    "TEMPERATURE_A": dict(
-        kinetic=True,
-        vars={"TH": dict(units="eV", long_name="Atomic hydrogen temperature")},
-    ),
-    "TEMPERATURE_M": dict(
-        kinetic=True,
-        vars={"TH": dict(units="eV", long_name="Atomic hydrogen temperature")},
-    ),
-    "BFIELD_STRENGTH": dict(
-        type="full",
-        vars={"bf_bounds": dict(units="T", long_name="Magnetic field strength")},
-    ),
-    "PLATES_MAG": dict(
-        type="plates_mag",
-        vars={"PLATES_MAG": dict(long_name="Cells that are within or behind plates")},
-    ),
-    # Some files - but don't know what they are
-    "TEMPERATURE_I": dict(
-        type="mapped",
-        kinetic=True,
-        vars={"TEMPERATURE_I_%d": dict()},
-    ),
-    "DENSITY_E_A": dict(
-        type="mapped",
-        kinetic=True,
-        vars={"DENSITY_E_A_%d": dict()},
-    ),
-    "DENSITY_E_I": dict(
-        type="mapped",
-        kinetic=True,
-        vars={"DENSITY_E_I_%d": dict()},
-    ),
-    "DENSITY_E_M": dict(
-        type="mapped",
-        kinetic=True,
-        vars={"DENSITY_E_M_%d": dict()},
-    ),
-    "NEUTRAL_DENSITY": dict(
-        type="mapped",
-        skip_first=[3, 2],
-        unmapped=True,
-        vars={"NEUTRAL_DENSITY_%d": dict()},
-    ),
-    "fort.1": dict(
-        type="raw",
-        vars={"fort.1": dict(long_name="Geometry input file")},
-    ),
-    "fort.2": dict(
-        type="raw",
-        vars={
-            "fort.2": dict(
-                long_name="Plasma parameters, boundary and initial conditions input file"
-            )
-        },
-    ),
-    "fort.3": dict(
-        type="raw",
-        vars={"fort.3": dict(long_name="Control flow input file")},
-    ),
-    "fort.4": dict(
-        type="raw",
-        vars={"fort.4": dict(long_name="Neutrals input file for EIRENE")},
-    ),
-    "fort.40": dict(
-        type="mapped",
-        vars={"fort.40_%d": dict()},
-    ),
-    "fort.42": dict(
-        type="mapped",
-        vars={"fort.42_%d": dict()},
-    ),
-    "fort.43": dict(
-        type="mapped",
-        vars={"fort.43_%d": dict()},
-    ),
-    "fort.46": dict(
-        type="mapped",
-        vars={"fort.46_%d": dict()},
-    ),
-    "fort.47": dict(
-        type="mapped",
-        vars={"fort.47_%d": dict()},
-    ),
-    "IMPURITY_IONIZATION_SOURCE": dict(
-        type="mapped",
-        vars={"IMPURITY_IONIZATION_SOURCE_%d": dict()},
-    ),
-    "IMPURITY_NEUTRAL": dict(
-        type="mapped",
-        vars={"IMPURITY_NEUTRAL_%d": dict()},
-    ),
-    "IMP_RADIATION": dict(
-        type="mapped",
-        vars={"IMP_RADIATION_%d": dict()},
-    ),
-    "FLUX_CONSERVATION": dict(
-        type="mapped",
-        vars={"FLUX_CONSERVATION_%d": dict()},
-    ),
-    "LG_CELL": dict(
-        type="mapped",
-        dtype=int,
-        vars={"LG_CELL_%d": dict()},
-    ),
-    "STREAMING_INFO": dict(
-        type="info",
-        fmt="%6.2f %5.3f %10.3E %10.3E %10.3E %10.3E %10.3E",
-        vars={
-            "dens_change": dict(
-                long_name="Relative change in density",
-                scale=1e-2,
-                units="",
-                notes="Unlike in EMC3/pymc3 this is not percent.",
-            ),
-            "flow_change": dict(
-                long_name="Change in Flow",
-                notes="Not scaled",
-            ),
-            "part_balance": dict(
-                long_name="Global particle balance",
-                units="A",
-            ),
-            "dens_upstream": dict(
-                long_name="Upstream Density",
-                scale=1e6,
-                units="m$^{-3}$",
-            ),
-            "dens_down_back": dict(
-                long_name="Downstream Density (backward direction)",
-                scale=1e6,
-                units="m$^{-3}$",
-            ),
-            "dens_down_mean": dict(
-                long_name="Downstream Density (averaged)",
-                scale=1e6,
-                units="m$^{-3}$",
-            ),
-            "dens_down_fwd": dict(
-                long_name="Downstream Density (forward direction)",
-                scale=1e6,
-                units="m$^{-3}$",
-            ),
-        },
-    ),
-    "ENERGY_INFO": dict(
-        type="info",
-        fmt=("%6.1f" + " %11.4E" * 4 + "\n") * 2 + " " * 18 + 3 * " %11.4E",
-        vars={
-            "Te_change": dict(
-                long_name="Relative change in el. temperature",
-                scale=1e-2,
-                units="",
-                notes="Unlike in EMC3/pymc3 this is not percent.",
-            ),
-            "Te_upstream": dict(
-                long_name="Upstream el. temperature",
-                units="eV",
-            ),
-            "Te_down_back": dict(
-                long_name="Downstream el. temperature (backward direction)", units="eV"
-            ),
-            "Te_down_mean": dict(
-                long_name="Downstream el. temperature (averaged)", units="eV"
-            ),
-            "Te_down_fwd": dict(
-                long_name="Downstream el. temperature (forward direction)",
-                units="eV",
-            ),
-            "Ti_change": dict(
-                long_name="Change in ion temperature",
-                scale=1e-2,
-                units="",
-                notes="Unlike in EMC3/pymc3 this is not percent.",
-            ),
-            "Ti_upstream": dict(
-                long_name="Upstream ion temperature",
-                units="eV",
-            ),
-            "Ti_down_back": dict(
-                long_name="Downstream ion temperature (backward direction)", units="eV"
-            ),
-            "Ti_down_mean": dict(
-                long_name="Downstream ion temperature (averaged)", units="eV"
-            ),
-            "Ti_down_fwd": dict(
-                long_name="Downstream ion temperature (forward direction)",
-                units="eV",
-            ),
-            "P_loss_gas": dict(long_name="Power losses (neutral gas)", units="W"),
-            "P_loss_imp": dict(long_name="Power losses (impurities)", units="W"),
-            "P_loss_target": dict(long_name="Power losses (target)", units="W"),
-        },
-    ),
-    "NEUTRAL_INFO": dict(
-        type="info",
-        fmt="%12.4E" + (" %11.4E" * 5),
-        vars={
-            "ionization_core": dict(long_name="Core ionization"),
-            "ionization_edge": dict(long_name="Edge ionization"),
-            "ionization_electron": dict(
-                long_name="Electron energy source / ionization",
-                units="eV",
-            ),
-            "ionization_ion": dict(
-                long_name="Ion energy source / ionization",
-                units="eV",
-            ),
-            "ionization_moment_fwd": dict(
-                long_name="Forward momentum source/ ionization"
-            ),
-            "ionization_moment_bwk": dict(
-                long_name="Backward momentum source/ ionization"
-            ),
-        },
-    ),
-    "IMPURITY_INFO": dict(
-        type="info",
-        fmt="%12.4E %11.4E",
-        vars={
-            "TOTAL_FLX": dict(long_name="Total impurity flux"),
-            "TOTAL_RAD": dict(long_name="Total radiation", units="W"),
-        },
-    ),
-    "ADD_SF_N0": dict(
-        type="surfaces",
-        vars={
-            plate_prefix + "phi": dict(units="radian"),
-            plate_prefix + "R": dict(units="m"),
-            plate_prefix + "z": dict(units="m"),
-        },
-    ),
-    "GRID_3D_DATA": dict(
-        type="geom",
-        vars={
-            "R_bounds": dict(units="m"),
-            "z_bounds": dict(units="m"),
-            "phi_bounds": dict(units="radian"),
-        },
-    ),
-    "PARTICLE_DEPO": dict(
-        type="depo",
-        vars={
-            "surftype_ne": dict(description="True means +1, False means -1"),
-            "flux_ne": dict(long_name="Outflux of particles", units="s^-1"),
-            "PARTICLE_DEPO_%d": dict(),
-        },
-    ),
-    "ENERGY_DEPO": dict(
-        type="depo",
-        vars={
-            "surftype_Te": dict(description="True means +1, False means -1"),
-            "flux_P": dict(long_name="Outflux of energy", units="W"),
-            "ENERGY_DEPO_%d": dict(),
-        },
-    ),
-    "TARGET_PROFILES": dict(
-        type="target_flux",
-        vars={
-            "f_n": dict(long_name="Particle flux"),
-            "f_E": dict(units="W/m²", scale=1e4, long_name="Energy flux"),
-            "avg_n": dict(units="m^-3", scale=1e6, long_name="Averge density"),
-            "avg_Te": dict(units="eV", long_name="Average electron temperature"),
-            "avg_Ti": dict(units="eV", long_name="Average ion temperature"),
-        },
-    ),
-}
-
-if False:
-    _files_bak = files.copy()
-    for k in files:
-        _files_bak[k] = files[k].copy()
-        if isinstance(files[k], dict):
-            for l in files[k]:
-                try:
-                    _files_bak[k][l] = files[k][l].copy()
-                except:  # noqa: E722
-                    try:
-                        _files_bak[k][l] = files[k][l][:]
-                    except:  # noqa: E722
-                        pass
-else:
-    _files_bak = files
-
-
 def read_fort_file_pub(
     fn: str, ds: typing.Union[None, xr.Dataset, xr.DataArray] = None, **opts
 ) -> xr.Dataset:
     """
     Read a EMC3 simulation file. The expected content is derived from
     the filename.
 
@@ -1758,15 +1441,14 @@
 
 
 def read_fort_file(ds: xr.Dataset, fn: str, type: str = "mapped", **opts) -> xr.Dataset:
     """
     Read an EMC3 simulation file and add to a dataset.
 
     """
-    assert files == _files_bak
     datas = None
     vars = opts.pop("vars")
     if type == "mapping":
         ds["_plasma_map"] = read_mappings(
             fn, tuple([len(ds[k]) for k in ("r", "theta", "phi")])
         )
     elif type == "mapped":
@@ -1807,35 +1489,30 @@
         datas = None
     elif type == "raw":
         datas = [read_raw(fn)]
     elif type == "depo":
         datas = read_depo_raw(ds, fn)
     else:
         raise RuntimeError(f"Unexpected type {type}")
-    assert files == _files_bak
     assert opts == {}, "Unexpected arguments: " + ", ".join(
         [f"{k}={v}" for k, v in opts.items()]
     )
     if datas is None:
         return ds
     vars = vars.copy()
-    assert files == _files_bak
     assert opts == {}
     keys = [k for k in vars]
     if "%" in keys[-1]:
         key = keys[-1]
         flexi = vars.pop(key)
         for i in range(len(vars), len(datas)):
             vars[key % i] = flexi
-
-    assert files == _files_bak
     assert len(vars) == len(
         datas
     ), f"in file {fn} we found {len(datas)} fields but only {len(vars)} vars are given!"
-    assert files == _files_bak
     for (var, varopts), data in zip(vars.items(), datas):
         ds[var] = data
         varopts = varopts.copy()
         scale = varopts.pop("scale", 1)
         if scale != 1:
             ds[var].data *= scale
 
@@ -1845,15 +1522,14 @@
             if k in varopts:
                 attrs[k] = varopts.pop(k)
 
         ds[var].attrs.update(attrs)
         assert (
             varopts == {}
         ), f"variable {var} has options {varopts} but didn't expect anything"
-    assert files == _files_bak
     return ds
 
 
 def guess_type(ds: xr.Dataset, key: typing.Hashable) -> str:
     data = ds[key]
     assert isinstance(key, str)
     try:
@@ -2006,15 +1682,14 @@
     elif type == "plates_mag":
         vars = opts.pop("vars")
         assert list(vars.keys()) == ["PLATES_MAG"]
         write_plates_mag(f"{dir}/{fn}", ds)
     elif type == "info":
         write_info_file(f"{dir}/{fn}", ds)
     elif type == "geom":
-        assert fn == "GRID_3D_DATA"
         write_locations(ds, f"{dir}/{fn}")
     elif type == "raw":
         vars = opts.pop("vars")
         assert len(vars) == 1
         write_raw(ds[list(vars.keys())[0]], f"{dir}/{fn}")
     elif type == "depo":
         vars = get_vars_for_file(ds, opts.pop("vars"))
@@ -2033,23 +1708,33 @@
     Parameters
     ----------
     ds : xr.Dataset
         The xemc3 dataset
     dir : str
         The directory to write the files to
     """
-    write_locations(ds, f"{dir}/GRID_3D_DATA")
+    write_locations(ds, get_file_name(dir, "geom"))
     for fn, opts in files.items():
         try:
             get_vars_for_file(ds, fn)
         except KeyError:
             pass
         else:
             write_fort_file(ds, dir, fn, **opts)
 
+
+def get_file_name(dir: typing.Optional[str], type: str) -> str:
+    found: typing.List[str] = []
+    for file, data in files.items():
+        if data.get("type", "mapped") == type:
+            found.append(file)
+    assert len(found) == 1
+    if dir:
+        return f"{dir}/{found[0]}"
+    return found[0]
     # if False:
     #     ds["phi"] = read_mapped(path + "/POTENTIAL", map, skip_first=0, kinetic=False)[
     #         0
     #     ]
     #     ds["phi"].attrs["units"] = "V"
     #     ds["phi"].attrs["long_name"] = "Potential"
 
@@ -2091,9 +1776,7 @@
     #     ds["flux_conservation"].attrs["units"] = "flux []"
     #     ds["flux_conservation"].attrs["long_name"] = "flux []"
 
     # # R                              RECOMBINATION                  0 1.6021765699999998e-13 R [s$^{-1}$ m$^{-3}$]
     #     ds["R"]=read_mapped(path + "/RECOMBINATION", map, skip_first=0, kinetic=False)[0]*1.6021765699999998e-13
     #     ds["R"].attrs["units"] = "R [s$^{-1}$ m$^{-3}$]"
     #     ds["R"].attrs["long_name"] = "R [s$^{-1}$ m$^{-3}$]"
-
-    return ds
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `xemc3-0.2.4/xemc3/core/plot_2d.py` & `xemc3-0.2.5/xemc3/core/plot_2d.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.4/xemc3/core/plot_3d.py` & `xemc3-0.2.5/xemc3/core/plot_3d.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.4/xemc3/core/utils.py` & `xemc3-0.2.5/xemc3/core/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -123,14 +123,16 @@
     else:
         in_dims = dims
         attrs = {}
     dims = len(data.shape)
     assert dims == len(
         in_dims
     ), f"Data mismatch - {in_dims} as dimensions given, but data is shape {data.shape} (len{len(data.shape)})"
+    # Once we drop python3.8, replace by removesuffix
+    in_dims = [x[: -len("_plus1")] if x.endswith("_plus1") else x for x in in_dims]
     out_dims = [d for d in in_dims] + ["delta_" + d for d in in_dims]
     ret = np.empty([i - 1 for i in data.shape] + [2] * dims, dtype=data.dtype)
     for ijk in itertools.product(*[range(a - 1) for a in data.shape]):
         tmp = np.array(data[tuple([slice(i, i + 2) for i in ijk])])
         ret[ijk] = tmp
     return xr.DataArray(data=ret, dims=out_dims, attrs=attrs)
```

### Comparing `xemc3-0.2.4/xemc3/load/__init__.py` & `xemc3-0.2.5/xemc3/load/__init__.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.4/xemc3/test/gen_ds.py` & `xemc3-0.2.5/xemc3/test/gen_ds.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.4/xemc3/test/test_average.py` & `xemc3-0.2.5/xemc3/test/test_average.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.4/xemc3/test/test_cli.py` & `xemc3-0.2.5/xemc3/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.4/xemc3/test/test_dataset.py` & `xemc3-0.2.5/xemc3/test/test_dataset.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.4/xemc3/test/test_load_real.py` & `xemc3-0.2.5/xemc3/test/test_load_real.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.4/xemc3/test/test_utils.py` & `xemc3-0.2.5/xemc3/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.4/xemc3/test/test_write_load.py` & `xemc3-0.2.5/xemc3/test/test_write_load.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.4/xemc3/tools/run_wrapper.py` & `xemc3-0.2.5/xemc3/tools/run_wrapper.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.4/xemc3/write/fortran.py` & `xemc3-0.2.5/xemc3/write/fortran.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.4/xemc3.egg-info/PKG-INFO` & `xemc3-0.2.5/xemc3.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xemc3
-Version: 0.2.4
+Version: 0.2.5
 Summary: Collect data from EMC3 runs in python using xarray
 Home-page: https://github.com/dschwoerer/xemc3
 Author: David Bold
 Author-email: dave@ipp.mpg.de
 License: GPL
 Project-URL: Tracker, https://github.com/dschwoerer/xemc3/issues
 Project-URL: Documentation, https://xemc3.rtfd.io
```

### Comparing `xemc3-0.2.4/xemc3.egg-info/SOURCES.txt` & `xemc3-0.2.5/xemc3.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -10,20 +10,23 @@
 requirements.txt
 setup.cfg
 setup.py
 .github/workflows/black-fix.yml
 .github/workflows/build.yml
 .github/workflows/python_publish.yml
 .github/workflows/test-python-package.yml
+.github/workflows/version-yaml.yml
 .github/workflows/zenodo.yml
 docs/citing.rst
 docs/cli.rst
 docs/cli.rst.in.py
 docs/conf.py
+docs/config.ipynb
 docs/examples.rst
+docs/filenames.ipynb
 docs/index.rst
 docs/introduction.rst
 docs/xarray.rst
 docs/xemc3.rst
 docs/examples/evaluate_at.ipynb
 docs/examples/get_data.py
 docs/examples/heatflux.ipynb
@@ -32,34 +35,43 @@
 docs/examples/load1.ipynb
 docs/examples/load2.ipynb
 docs/examples/setup_plt.py
 docs/exercises/get_data.py
 docs/exercises/introduction.ipynb
 xemc3/__init__.py
 xemc3/_version.py
+xemc3/config.py
 xemc3.egg-info/PKG-INFO
 xemc3.egg-info/SOURCES.txt
 xemc3.egg-info/dependency_links.txt
 xemc3.egg-info/entry_points.txt
 xemc3.egg-info/requires.txt
 xemc3.egg-info/top_level.txt
 xemc3/cli/__init__.py
 xemc3/cli/_common.py
 xemc3/cli/append_time.py
 xemc3/cli/to_archive.py
 xemc3/cli/to_netcdf.py
 xemc3/cli/xdivertor.py
 xemc3/core/__init__.py
+xemc3/core/config.py
 xemc3/core/dataset.py
 xemc3/core/depo.py
 xemc3/core/evaluate_at.py
 xemc3/core/load.py
 xemc3/core/plot_2d.py
 xemc3/core/plot_3d.py
 xemc3/core/utils.py
+xemc3/data/default.yaml
+xemc3/data/v0.2.0.yaml
+xemc3/data/v0.2.1.yaml
+xemc3/data/v0.2.2.yaml
+xemc3/data/v0.2.3.yaml
+xemc3/data/v0.2.4.yaml
+xemc3/data/v0.2.5.yaml
 xemc3/load/__init__.py
 xemc3/test/__init__.py
 xemc3/test/gen_ds.py
 xemc3/test/test_average.py
 xemc3/test/test_basic.py
 xemc3/test/test_cli.py
 xemc3/test/test_dataset.py
```

