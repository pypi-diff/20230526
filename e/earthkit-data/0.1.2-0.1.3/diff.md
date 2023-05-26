# Comparing `tmp/earthkit-data-0.1.2.tar.gz` & `tmp/earthkit-data-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "earthkit-data-0.1.2.tar", last modified: Tue May 23 13:59:54 2023, max compression
+gzip compressed data, was "earthkit-data-0.1.3.tar", last modified: Fri May 26 11:14:12 2023, max compression
```

## Comparing `earthkit-data-0.1.2.tar` & `earthkit-data-0.1.3.tar`

### file list

```diff
@@ -1,229 +1,270 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:59:54.902288 earthkit-data-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:59:54.870288 earthkit-data-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:59:54.874288 earthkit-data-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/.github/workflows/label-public-pr.yml
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/.github/workflows/notify_new_issue.yml
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/.github/workflows/notify_new_pr.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7160 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11382 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-05-23 13:59:54.902288 earthkit-data-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:59:54.874288 earthkit-data-0.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:59:54.874288 earthkit-data-0.1.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/docs/_static/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/docs/_static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:59:54.874288 earthkit-data-0.1.2/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/docs/_templates/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/docs/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:59:54.878288 earthkit-data-0.1.2/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    11746 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/docs/examples/bufr.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    45108 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/docs/examples/grib_fdb_stream.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8457 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/docs/examples/grib_file_pattern.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    46028 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/docs/examples/grib_from_stream.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    13846 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/docs/examples/grib_indexing.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    76257 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/docs/examples/grib_metadata.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/docs/examples/grib_missing.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    16154 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/docs/examples/grib_multi.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   111937 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/docs/examples/grib_overview.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    45664 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/docs/examples/grib_selection.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9445 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/docs/examples/grib_tar.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/docs/examples/grib_to_netcdf.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    28136 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/docs/examples/grib_url.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    34095 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/docs/examples/list_of_dict.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/docs/examples/missing.grib
--rw-r--r--   0 runner    (1001) docker     (123)    39106 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/docs/examples/netcdf.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    13530 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/docs/examples/temp_10.bufr
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/docs/examples/test.grib
--rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/docs/examples/test.nc
--rw-r--r--   0 runner    (1001) docker     (123)   521712 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/docs/examples/test4.grib
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/docs/examples/test6.grib
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/docs/examples/tuv_pl.grib
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/docs/licence.rst
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:59:54.870288 earthkit-data-0.1.2/earthkit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:59:54.878288 earthkit-data-0.1.2/earthkit/data/
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:59:54.882288 earthkit-data-0.1.2/earthkit/data/arguments/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/arguments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/arguments/args_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/arguments/argument.py
--rw-r--r--   0 runner    (1001) docker     (123)    10134 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/arguments/earthkit_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/arguments/input_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/arguments/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:59:54.882288 earthkit-data-0.1.2/earthkit/data/core/
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22865 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/core/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    11921 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/core/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/core/ipython.py
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/core/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/core/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/core/select.py
--rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/core/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/core/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/core/temporary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/core/thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:59:54.870288 earthkit-data-0.1.2/earthkit/data/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:59:54.882288 earthkit-data-0.1.2/earthkit/data/data/css/
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/data/css/tab.css
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/data/css/table.css
--rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:59:54.882288 earthkit-data-0.1.2/earthkit/data/indexing/
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/indexing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:59:54.882288 earthkit-data-0.1.2/earthkit/data/indexing/database/
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/indexing/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/indexing/database/json.py
--rw-r--r--   0 runner    (1001) docker     (123)    19393 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/indexing/database/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/indexing/database/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/input_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:59:54.882288 earthkit-data-0.1.2/earthkit/data/mergers/
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/mergers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/mergers/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/mergers/xarray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:59:54.886288 earthkit-data-0.1.2/earthkit/data/mirrors/
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/mirrors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/mirrors/directory_mirror.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:59:54.886288 earthkit-data-0.1.2/earthkit/data/readers/
--rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/readers/archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/readers/bufr.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/readers/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/readers/directory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:59:54.886288 earthkit-data-0.1.2/earthkit/data/readers/grib/
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/readers/grib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15380 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/readers/grib/codes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7780 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/readers/grib/fieldset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:59:54.886288 earthkit-data-0.1.2/earthkit/data/readers/grib/index/
--rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/readers/grib/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/readers/grib/index/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/readers/grib/index/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/readers/grib/index/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/readers/grib/index/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/readers/grib/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/readers/grib/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/readers/grib/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/readers/grib/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/readers/grib/xarray.py
--rw-r--r--   0 runner    (1001) docker     (123)    11379 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/readers/netcdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/readers/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/readers/odb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/readers/tar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/readers/text.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/readers/unknown.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/readers/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:59:54.890288 earthkit-data-0.1.2/earthkit/data/sources/
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/sources/dummy.grib
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/sources/dummy_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/sources/empty.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/sources/fdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/sources/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/sources/file_indexed.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/sources/file_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/sources/indexed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/sources/list_of_dicts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/sources/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/sources/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/sources/multi_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/sources/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/sources/url.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/sources/url_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/sources/virtual.py
--rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/sources/virtual_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:59:54.894288 earthkit-data-0.1.2/earthkit/data/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/utils/availability.py
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/utils/bbox.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/utils/conventions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/utils/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)    19711 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/utils/factorise.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/utils/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/utils/humanize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/utils/kwargs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/utils/lazy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/utils/parts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/utils/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/utils/serialise.py
--rw-r--r--   0 runner    (1001) docker     (123)     5028 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/utils/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-23 13:59:54.000000 earthkit-data-0.1.2/earthkit/data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:59:54.894288 earthkit-data-0.1.2/earthkit/data/vocabularies/
--rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/vocabularies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/vocabularies/aliases.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/vocabularies/cf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/vocabularies/grib-paramid.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/vocabularies/grib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:59:54.894288 earthkit-data-0.1.2/earthkit/data/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/earthkit/data/wrappers/string.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:59:54.894288 earthkit-data-0.1.2/earthkit_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-05-23 13:59:54.000000 earthkit-data-0.1.2/earthkit_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-05-23 13:59:54.000000 earthkit-data-0.1.2/earthkit_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 13:59:54.000000 earthkit-data-0.1.2/earthkit_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-23 13:59:54.000000 earthkit-data-0.1.2/earthkit_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-23 13:59:54.000000 earthkit-data-0.1.2/earthkit_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-23 13:59:54.902288 earthkit-data-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:59:54.894288 earthkit-data-0.1.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:59:54.894288 earthkit-data-0.1.2/tests/bufr/
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/tests/bufr/test_bufr_summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:59:54.894288 earthkit-data-0.1.2/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/tests/core/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/tests/core/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:59:54.898288 earthkit-data-0.1.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    22138 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/tests/data/mercator.grib
--rw-r--r--   0 runner    (1001) docker     (123)    47520 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/tests/data/ml_data.grib
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/tests/data/rgg_small_subarea_cellarea_ref.grib
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/tests/data/t_pl.grib
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/tests/data/t_time_series.grib
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/tests/data/test_icon.grib
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/tests/data/test_single.grib
--rw-r--r--   0 runner    (1001) docker     (123)    21233 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/tests/data/test_single.nc
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/tests/data/test_single_with_missing.grib
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/tests/data/u_pl.grib
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/tests/data/v_pl.grib
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:59:54.898288 earthkit-data-0.1.2/tests/documentation/
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/tests/documentation/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/tests/documentation/test_notebooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:59:54.898288 earthkit-data-0.1.2/tests/grib/
--rw-r--r--   0 runner    (1001) docker     (123)    20450 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/tests/grib/test_grib_contents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/tests/grib/test_grib_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/tests/grib/test_grib_order_by.py
--rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/tests/grib/test_grib_sel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/tests/grib/test_grib_slice.py
--rw-r--r--   0 runner    (1001) docker     (123)    14358 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/tests/grib/test_grib_summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:59:54.898288 earthkit-data-0.1.2/tests/indexing/
--rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/tests/indexing/indexing_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/tests/indexing/test_indexing_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/tests/indexing/test_indexing_isel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/tests/indexing/test_indexing_order_by.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/tests/indexing/test_indexing_serialisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/tests/indexing/test_order_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/tests/indexing/test_selection_kwargs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:59:54.902288 earthkit-data-0.1.2/tests/readers/
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/tests/readers/test_csv_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/tests/readers/test_grib_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/tests/readers/test_netcdf_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/tests/readers/test_tar_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/tests/readers/test_unknown_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/tests/readers/test_zip_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/tests/readers/unknown_file.unknown_ext
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/tests/readers/unknown_text_file.unknown_ext
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:59:54.902288 earthkit-data-0.1.2/tests/sources/
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/tests/sources/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/tests/sources/test_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/tests/sources/test_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/tests/sources/test_url_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-23 13:59:36.000000 earthkit-data-0.1.2/tests/test_00_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.899907 earthkit-data-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.871907 earthkit-data-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.875907 earthkit-data-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/.github/workflows/label-public-pr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/.github/workflows/notify_new_issue.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/.github/workflows/notify_new_pr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7160 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11382 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-05-26 11:14:12.899907 earthkit-data-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.875907 earthkit-data-0.1.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.875907 earthkit-data-0.1.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/_static/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/_static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.875907 earthkit-data-0.1.3/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/_templates/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/development.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.879907 earthkit-data-0.1.3/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/Untitled.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11813 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/bufr.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/cds.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    48723 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/fdb.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/grib_file_pattern.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    46046 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/grib_from_stream.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    13863 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/grib_indexing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    76259 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/grib_metadata.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/grib_missing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    16588 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/grib_multi.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   100543 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/grib_overview.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    45612 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/grib_selection.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9452 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/grib_tar.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/grib_to_netcdf.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    28172 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/grib_url.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    34189 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/list_of_dict.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/mars.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/missing.grib
+-rw-r--r--   0 runner    (1001) docker     (123)    39112 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/netcdf.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10586 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/odb.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    13530 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/temp_10.bufr
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/test.grib
+-rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/test.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    13297 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/test.odb
+-rw-r--r--   0 runner    (1001) docker     (123)   521712 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/test4.grib
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/test6.grib
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/tuv_pl.grib
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.879907 earthkit-data-0.1.3/docs/guide/
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/guide/caching.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10512 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/guide/data.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.879907 earthkit-data-0.1.3/docs/guide/data_format/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/guide/data_format/bufr.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/guide/data_format/csv.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/guide/data_format/grib.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/guide/data_format/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/guide/data_format/netcdf.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/guide/data_format/odb.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.879907 earthkit-data-0.1.3/docs/guide/include/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/guide/include/settings-1-get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/guide/include/settings-2-set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/guide/include/settings-3-reset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/guide/settings.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/guide/sources.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/licence.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.871907 earthkit-data-0.1.3/earthkit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.879907 earthkit-data-0.1.3/earthkit/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.883907 earthkit-data-0.1.3/earthkit/data/arguments/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/arguments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/arguments/args_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/arguments/argument.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10134 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/arguments/earthkit_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/arguments/input_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/arguments/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.883907 earthkit-data-0.1.3/earthkit/data/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22865 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/core/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20857 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/core/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/core/ipython.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/core/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/core/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/core/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/core/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/core/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/core/temporary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/core/thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.871907 earthkit-data-0.1.3/earthkit/data/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.883907 earthkit-data-0.1.3/earthkit/data/data/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/data/css/tab.css
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/data/css/table.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.883907 earthkit-data-0.1.3/earthkit/data/indexing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/indexing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.883907 earthkit-data-0.1.3/earthkit/data/indexing/database/
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/indexing/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/indexing/database/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19393 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/indexing/database/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/indexing/database/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/input_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.883907 earthkit-data-0.1.3/earthkit/data/mergers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/mergers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/mergers/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/mergers/xarray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.883907 earthkit-data-0.1.3/earthkit/data/mirrors/
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/mirrors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/mirrors/directory_mirror.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.887907 earthkit-data-0.1.3/earthkit/data/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/readers/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/readers/bufr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/readers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/readers/directory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.887907 earthkit-data-0.1.3/earthkit/data/readers/grib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/readers/grib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27074 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/readers/grib/codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15965 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/readers/grib/fieldlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.887907 earthkit-data-0.1.3/earthkit/data/readers/grib/index/
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/readers/grib/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/readers/grib/index/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/readers/grib/index/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/readers/grib/index/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/readers/grib/index/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/readers/grib/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10324 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/readers/grib/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/readers/grib/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/readers/grib/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/readers/grib/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/readers/grib/xarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11380 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/readers/netcdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/readers/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/readers/odb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/readers/tar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/readers/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/readers/unknown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/readers/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.891907 earthkit-data-0.1.3/earthkit/data/sources/
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/sources/cds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/sources/dummy.grib
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/sources/dummy_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/sources/ecmwf_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/sources/empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/sources/fdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/sources/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/sources/file_indexed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/sources/file_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/sources/indexed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/sources/list_of_dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/sources/mars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/sources/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/sources/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/sources/multi_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/sources/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/sources/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/sources/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/sources/url_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/sources/virtual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6483 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/sources/virtual_directory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.891907 earthkit-data-0.1.3/earthkit/data/sphinxext/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/sphinxext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/sphinxext/generate_settings_rst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/sphinxext/module_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/sphinxext/xref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.891907 earthkit-data-0.1.3/earthkit/data/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/utils/availability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/utils/bbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/utils/conventions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/utils/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19711 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/utils/factorise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/utils/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/utils/humanize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/utils/kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/utils/lazy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/utils/parts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/utils/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/utils/serialise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5028 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/utils/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-26 11:14:12.000000 earthkit-data-0.1.3/earthkit/data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.891907 earthkit-data-0.1.3/earthkit/data/vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/vocabularies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/vocabularies/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/vocabularies/cf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/vocabularies/grib-paramid.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/vocabularies/grib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.891907 earthkit-data-0.1.3/earthkit/data/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/wrappers/integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/wrappers/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65385 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit-data.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.891907 earthkit-data-0.1.3/earthkit_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-05-26 11:14:12.000000 earthkit-data-0.1.3/earthkit_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-05-26 11:14:12.000000 earthkit-data-0.1.3/earthkit_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 11:14:12.000000 earthkit-data-0.1.3/earthkit_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-26 11:14:12.000000 earthkit-data-0.1.3/earthkit_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-26 11:14:12.000000 earthkit-data-0.1.3/earthkit_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-26 11:14:12.899907 earthkit-data-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.895907 earthkit-data-0.1.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.895907 earthkit-data-0.1.3/tests/bufr/
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/bufr/test_bufr_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.895907 earthkit-data-0.1.3/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/core/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/core/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.895907 earthkit-data-0.1.3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    22138 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/data/mercator.grib
+-rw-r--r--   0 runner    (1001) docker     (123)    47520 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/data/ml_data.grib
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/data/rgg_small_subarea_cellarea_ref.grib
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/data/t_pl.grib
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/data/t_time_series.grib
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/data/test_icon.grib
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/data/test_single.grib
+-rw-r--r--   0 runner    (1001) docker     (123)    21233 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/data/test_single.nc
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/data/test_single_with_missing.grib
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/data/u_pl.grib
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/data/v_pl.grib
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.895907 earthkit-data-0.1.3/tests/documentation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/documentation/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/documentation/test_notebooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.895907 earthkit-data-0.1.3/tests/grib/
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/grib/test_grib_concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21795 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/grib/test_grib_contents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/grib/test_grib_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/grib/test_grib_order_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5499 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/grib/test_grib_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/grib/test_grib_sel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/grib/test_grib_slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14358 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/grib/test_grib_summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.895907 earthkit-data-0.1.3/tests/indexing/
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/indexing/indexing_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/indexing/test_indexing_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/indexing/test_indexing_isel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/indexing/test_indexing_order_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/indexing/test_indexing_serialisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/indexing/test_order_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/indexing/test_selection_kwargs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.899907 earthkit-data-0.1.3/tests/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/readers/test_csv_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/readers/test_grib_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/readers/test_netcdf_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/readers/test_odb_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/readers/test_tar_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/readers/test_unknown_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/readers/test_zip_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/readers/unknown_file.unknown_ext
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/readers/unknown_text_file.unknown_ext
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.899907 earthkit-data-0.1.3/tests/sources/
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/sources/test_cds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/sources/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/sources/test_mars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/sources/test_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/sources/test_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/sources/test_url_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/test_00_version.py
```

### Comparing `earthkit-data-0.1.2/.github/workflows/ci.yml` & `earthkit-data-0.1.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/.gitignore` & `earthkit-data-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/.pre-commit-config.yaml` & `earthkit-data-0.1.3/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -15,18 +15,18 @@
   hooks:
   - id: isort
 - repo: https://github.com/psf/black
   rev: 23.3.0
   hooks:
   - id: black
 - repo: https://github.com/keewis/blackdoc
-  rev: v0.3.4
+  rev: v0.3.8
   hooks:
   - id: blackdoc
-    additional_dependencies: [black==22.3.0]
+    additional_dependencies: [black==23.3.0]
 - repo: https://github.com/PyCQA/flake8
   rev: 4.0.1
   hooks:
   - id: flake8
 - repo: https://github.com/executablebooks/mdformat
   rev: 0.7.14
   hooks:
```

### Comparing `earthkit-data-0.1.2/LICENSE` & `earthkit-data-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/Makefile` & `earthkit-data-0.1.3/Makefile`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/PKG-INFO` & `earthkit-data-0.1.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,62 @@
 Metadata-Version: 2.1
 Name: earthkit-data
-Version: 0.1.2
+Version: 0.1.3
 Summary: A format-agnostic Python interface for geospatial data
 License: Apache License 2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # earthkit-data
 
+![earthkit-data](https://raw.githubusercontent.com/ecmwf/earthkit-data/develop/earthkit-data.png)
+
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/earthkit-data.svg)](https://pypi.python.org/pypi/earthkit-data/)
 
 A format-agnostic interface for geospatial data with a focus on meteorology and
 climate science.
 
 **DISCLAIMER**
 This project is **BETA** and will be **Experimental** for the foreseeable future.
 Interfaces and functionality are likely to change, and the project itself may be scrapped.
 **DO NOT** use this software in any project/software that is operational.
 
+## Documentation
+
 The documentation can be found at https://earthkit-data.readthedocs.io/.
 
+## Install
+
+Install via `pip` with:
+
+```
+$ pip install earthkit-data
+```
+
+More details, such as how to install any necessary binaries, can be found  at https://earthkit-data.readthedocs.io/en/latest/install.html.
+
+Alternatively, install via `conda` with:
+
+```
+$ conda install earthkit-data -c conda-forge
+```
+
+This will bring in some necessary binary dependencies for you.
+
 ## License
 
 ```
 Copyright 2022, European Centre for Medium Range Weather Forecasts.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
```

### Comparing `earthkit-data-0.1.2/README.md` & `earthkit-data-0.1.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,43 @@
 # earthkit-data
 
+![earthkit-data](https://raw.githubusercontent.com/ecmwf/earthkit-data/develop/earthkit-data.png)
+
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/earthkit-data.svg)](https://pypi.python.org/pypi/earthkit-data/)
 
 A format-agnostic interface for geospatial data with a focus on meteorology and
 climate science.
 
 **DISCLAIMER**
 This project is **BETA** and will be **Experimental** for the foreseeable future.
 Interfaces and functionality are likely to change, and the project itself may be scrapped.
 **DO NOT** use this software in any project/software that is operational.
 
+## Documentation
+
 The documentation can be found at https://earthkit-data.readthedocs.io/.
 
+## Install
+
+Install via `pip` with:
+
+```
+$ pip install earthkit-data
+```
+
+More details, such as how to install any necessary binaries, can be found  at https://earthkit-data.readthedocs.io/en/latest/install.html.
+
+Alternatively, install via `conda` with:
+
+```
+$ conda install earthkit-data -c conda-forge
+```
+
+This will bring in some necessary binary dependencies for you.
+
 ## License
 
 ```
 Copyright 2022, European Centre for Medium Range Weather Forecasts.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
```

### Comparing `earthkit-data-0.1.2/docs/Makefile` & `earthkit-data-0.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/docs/examples/bufr.ipynb` & `earthkit-data-0.1.3/docs/examples/bufr.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9952083333333334%*

 * *Differences: {"'cells'": "{0: {'source': ['!test -f temp_10.bufr || wget "*

 * *            "https://get.ecmwf.int/repository/test-data/earthkit-data/examples/temp_10.bufr']}, 7: "*

 * *            "{'source': ['to_pandas() extracts data into a Pandas dataframe (uses "*

 * *            '[pdbufr]("https://github.com/ecmwf/pdbufr") under the hood). The following example '*

 * *            "shows how the get the temperature profile for a given station:'], 'attachments': "*

 * *            'OrderedDict()}}'}*

```diff
@@ -3,15 +3,15 @@
         {
             "cell_type": "code",
             "execution_count": 1,
             "id": "27c5ff09-4f9f-4eb0-947e-5e75b56a65ba",
             "metadata": {},
             "outputs": [],
             "source": [
-                "!test -f temp_10.bufr || wget https://get.ecmwf.int/repository/test-data/emohawk/examples/temp_10.bufr"
+                "!test -f temp_10.bufr || wget https://get.ecmwf.int/repository/test-data/earthkit-data/examples/temp_10.bufr"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "102b1cf9-33a5-4310-af4d-bcd17d598d29",
             "metadata": {},
             "source": [
@@ -216,19 +216,20 @@
                 }
             ],
             "source": [
                 "fs.head()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "07ca0ea4-cad9-4973-ac79-681f9140c116",
             "metadata": {},
             "source": [
-                "to_pandas() extracts data into a Pandas dataframe (uses pdbufr under the hood). The following example shows how the get the temperature profile for a given station:"
+                "to_pandas() extracts data into a Pandas dataframe (uses [pdbufr](\"https://github.com/ecmwf/pdbufr\") under the hood). The following example shows how the get the temperature profile for a given station:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "id": "53ac87d6-09b9-46c3-bc54-07fd2a175b05",
             "metadata": {},
```

### Comparing `earthkit-data-0.1.2/docs/examples/grib_fdb_stream.ipynb` & `earthkit-data-0.1.3/docs/examples/grib_from_stream.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9538026422453484%*

 * *Differences: {"'cells'": "{1: {'id': 'recovered-organizer', 'source': ['## Reading GRIB from a stream']}, 2: "*

 * *            "{'execution_count': 2, 'id': 'sticky-refrigerator', 'source': {delete: [0]}}, 3: "*

 * *            "{'id': 'german-simulation', 'source': ['earthkit-data can load GRIB data from a "*

 * *            '**stream**, which can be an FDB stream, a standard Python IO stream or any object '*

 * *            "implementing the necessary stream methods. \\n', '\\n', 'For simplicity, in this "*

 * *            "notebook we will  […]*

```diff
@@ -1,334 +1,275 @@
 {
     "cells": [
         {
+            "cell_type": "code",
+            "execution_count": 1,
+            "id": "collectible-accreditation",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "!test -f test6.grib || wget https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test6.grib"
+            ]
+        },
+        {
             "cell_type": "markdown",
-            "id": "fad5f9b6-c33a-4d57-b982-95f5e3d64eff",
+            "id": "recovered-organizer",
             "metadata": {},
             "source": [
-                "## Reading GRIB from FDB stream"
+                "## Reading GRIB from a stream"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 1,
-            "id": "sufficient-league",
+            "execution_count": 2,
+            "id": "sticky-refrigerator",
             "metadata": {},
             "outputs": [],
             "source": [
-                "import pyfdb \n",
                 "import earthkit.data"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "occasional-music",
+            "id": "german-simulation",
             "metadata": {},
             "source": [
-                "<div class=\"alert alert-block alert-warning\">\n",
-                "To run this scirpt FDB access is needed and the <b>FDB_HOME</b> environment variable has to be set correctly.\n",
-                "</div>"
+                "earthkit-data can load GRIB data from a **stream**, which can be an FDB stream, a standard Python IO stream or any object implementing the necessary stream methods. \n",
+                "\n",
+                "For simplicity, in this notebook we will use a **file stream** to demonstrate the usage of streams."
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": 2,
-            "id": "metric-machinery",
+            "cell_type": "markdown",
+            "id": "prescribed-giant",
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "env: FDB_HOME=/home/fdbprod\n"
-                    ]
-                }
-            ],
             "source": [
-                "# date must be adjusted since FDB only stores recent dates\n",
-                "request = {\n",
-                "    'class': 'od',\n",
-                "    'expver': '0001',\n",
-                "    'stream': 'oper',\n",
-                "    'date': '20230404',\n",
-                "    'time': [0, 12],\n",
-                "    'domain': 'g',\n",
-                "    'type': 'an',\n",
-                "    'levtype': 'sfc',\n",
-                "    'step': 0,\n",
-                "    'param': [151, 167]\n",
-                "}\n",
-                "\n",
-                "# Must be set correctly\n",
-                "%env FDB_HOME=/home/fdbprod\n",
-                "\n",
-                "fdb = pyfdb.FDB()"
+                "### Getting single items from the stream"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "streaming-poultry",
+            "id": "affiliated-joint",
             "metadata": {},
             "source": [
-                "#### Iteration with one field at a time in memory"
+                "We create a stream from a file containing 6 GRIB fields by simply calling *open()*. It returns an io.BufferedReader object (a file stream)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
-            "id": "printable-islam",
+            "id": "verbal-damage",
             "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": [
-                            "earthkit.data.sources.stream.StreamSource"
-                        ]
-                    },
-                    "execution_count": 3,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
+            "outputs": [],
             "source": [
-                "r = fdb.retrieve(request)\n",
-                "\n",
-                "fs = earthkit.data.from_source(\"stream\", r)\n",
-                "type(fs)"
+                "stream = open(\"test6.grib\", \"rb\")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "contemporary-liability",
+            "id": "covered-greensboro",
+            "metadata": {},
+            "source": [
+                "We load it into earthkit-data by using the **batch_size=1** (default) option. With this when we iterate through *fs* it will consume one message from the stream at a time:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 4,
+            "id": "durable-helicopter",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "Nothing is read at this moment."
+                "fs = earthkit.data.from_source(\"stream\", stream)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "extra-phenomenon",
+            "id": "resident-guard",
             "metadata": {},
             "source": [
-                "We can only use *fs* for iteration. Fields crerated in the iteration get deleted when going out of scope:"
+                "At this point nothing is read from the stream. As we progressing with the iteration GribField objects are created then get deleted when going out of scope. As a result there is only one GRIB message is kept in memory at a time."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
-            "id": "historic-panic",
+            "execution_count": 5,
+            "id": "animated-prayer",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "  param=msl shape=(6599680,) mean=101165.30143351648\n",
-                        "  param=2t shape=(6599680,) mean=288.471588476875\n",
-                        "  param=msl shape=(6599680,) mean=101158.70017015976\n",
-                        "  param=2t shape=(6599680,) mean=289.29876940588883\n"
+                        "GribField(t,1000,20180801,1200,0,0)\n",
+                        "GribField(u,1000,20180801,1200,0,0)\n",
+                        "GribField(v,1000,20180801,1200,0,0)\n",
+                        "GribField(t,850,20180801,1200,0,0)\n",
+                        "GribField(u,850,20180801,1200,0,0)\n",
+                        "GribField(v,850,20180801,1200,0,0)\n"
                     ]
                 }
             ],
             "source": [
                 "for f in fs:\n",
-                "    print(f\"  param={f['param']} shape={f.values.shape} mean={f.values.mean()}\")"
+                "    # f is GribField object. It gets deleted when going out of scope\n",
+                "    print(f)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "damaged-fever",
+            "id": "brilliant-struggle",
             "metadata": {},
             "source": [
-                "Once the iteration is completed, there is nothing left in fs."
+                "Having finished the iteration there is no data available any longer in *fs*.  We can close the stream:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
-            "id": "impressive-percentage",
+            "execution_count": 6,
+            "id": "unique-metadata",
             "metadata": {},
             "outputs": [],
             "source": [
-                "for f in fs:\n",
-                "    print(f\"type(f)={type(f)}\")"
+                "stream.close()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "spatial-driving",
+            "id": "judicial-backing",
             "metadata": {},
             "source": [
-                "#### Using group_by"
+                "### Using batch_size"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "suspected-sequence",
+            "id": "planned-weekly",
             "metadata": {},
             "source": [
-                "We can read multiple fields into memory from the stream at a time by using **group_by** in *from_source()*:"
+                "This time we create a stream and read 2 fields from it at a time by using **batch_size=2** in *from_source()*:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
-            "id": "located-quick",
+            "execution_count": 7,
+            "id": "placed-blues",
             "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": [
-                            "earthkit.data.sources.stream.StreamSource"
-                        ]
-                    },
-                    "execution_count": 6,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
+            "outputs": [],
             "source": [
-                "r = fdb.retrieve(request)\n",
-                "fs = earthkit.data.from_source(\"stream\", r, group_by=2)\n",
-                "type(fs)"
+                "stream = open(\"test6.grib\", \"rb\")\n",
+                "fs = earthkit.data.from_source(\"stream\", stream, batch_size=2)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
-            "id": "micro-noise",
+            "execution_count": 8,
+            "id": "outside-tennis",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "2\n",
-                        "['msl', '2t']\n",
+                        "['t', 'u']\n",
+                        "2\n",
+                        "['v', 't']\n",
                         "2\n",
-                        "['msl', '2t']\n"
+                        "['u', 'v']\n"
                     ]
                 }
             ],
             "source": [
                 "for f in fs:\n",
                 "    # f is a FieldList containing 2 fields. It gets deleted when going out of scope\n",
                 "    print(len(f))\n",
                 "    print(f.metadata(\"param\"))"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "greenhouse-decade",
+            "id": "unavailable-actress",
             "metadata": {},
             "source": [
-                "#### Storing all the fields in memory"
+                "Having finished the iteration there is no data available any longer in *fs*.  We can close the stream:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
-            "id": "coastal-irish",
+            "execution_count": 9,
+            "id": "jewish-season",
             "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": [
-                            "earthkit.data.sources.stream.StreamMemorySource"
-                        ]
-                    },
-                    "execution_count": 8,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
+            "outputs": [],
             "source": [
-                "r = fdb.retrieve(request)\n",
-                "\n",
-                "fs = earthkit.data.from_source(\"stream\", r, group_by=0)\n",
-                "type(fs)"
+                "stream.close()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "permanent-uncertainty",
+            "metadata": {},
+            "source": [
+                "### Storing each GRIB message in memory"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "skilled-floating",
+            "id": "blessed-paintball",
             "metadata": {},
             "source": [
-                "Nothing is read at this moment:"
+                "We can also set **batch_size=0** in *from_source()*:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
-            "id": "narrow-chocolate",
+            "execution_count": 10,
+            "id": "simple-london",
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "stored fields count=0\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
-                "print(f\"stored fields count={len(fs._reader._fields)}\")"
+                "stream = open(\"test6.grib\", \"rb\")\n",
+                "fs = earthkit.data.from_source(\"stream\", stream, batch_size=0)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "noted-fossil",
+            "id": "seeing-freight",
             "metadata": {},
             "source": [
-                "If we call any function on the fieldlist it reads the messages into memory"
+                "The resulting earthkit-data object is empty at this point. However, as soon as we call any method on it it will consume the whole stream and load all the GRIB messages into memory. They will be stored in memory as long as *fs* exists.\n",
+                "\n",
+                "We can call all the standard earthkit-data methods on *fs*:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
-            "id": "structural-cover",
+            "execution_count": 11,
+            "id": "meaning-oxide",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "4"
+                            "6"
                         ]
                     },
-                    "execution_count": 10,
+                    "execution_count": 11,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "len(fs)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
-            "id": "nearby-murray",
-            "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "stored fields count=4\n"
-                    ]
-                }
-            ],
-            "source": [
-                "print(f\"stored fields count={len(fs._reader._fields)}\")"
-            ]
-        },
-        {
-            "cell_type": "code",
             "execution_count": 12,
-            "id": "western-drawing",
+            "id": "copyrighted-walnut",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -360,113 +301,124 @@
                             "      <th>gridType</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
                             "      <td>ecmf</td>\n",
-                            "      <td>msl</td>\n",
-                            "      <td>surface</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>20230404</td>\n",
-                            "      <td>0</td>\n",
+                            "      <td>t</td>\n",
+                            "      <td>isobaricInhPa</td>\n",
+                            "      <td>1000</td>\n",
+                            "      <td>20180801</td>\n",
+                            "      <td>1200</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>reduced_gg</td>\n",
+                            "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
                             "      <td>ecmf</td>\n",
-                            "      <td>2t</td>\n",
-                            "      <td>surface</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>20230404</td>\n",
-                            "      <td>0</td>\n",
+                            "      <td>u</td>\n",
+                            "      <td>isobaricInhPa</td>\n",
+                            "      <td>1000</td>\n",
+                            "      <td>20180801</td>\n",
+                            "      <td>1200</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>reduced_gg</td>\n",
+                            "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
                             "      <td>ecmf</td>\n",
-                            "      <td>msl</td>\n",
-                            "      <td>surface</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>20230404</td>\n",
+                            "      <td>v</td>\n",
+                            "      <td>isobaricInhPa</td>\n",
+                            "      <td>1000</td>\n",
+                            "      <td>20180801</td>\n",
                             "      <td>1200</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>reduced_gg</td>\n",
+                            "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>3</th>\n",
                             "      <td>ecmf</td>\n",
-                            "      <td>2t</td>\n",
-                            "      <td>surface</td>\n",
+                            "      <td>t</td>\n",
+                            "      <td>isobaricInhPa</td>\n",
+                            "      <td>850</td>\n",
+                            "      <td>20180801</td>\n",
+                            "      <td>1200</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>an</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>20230404</td>\n",
+                            "      <td>regular_ll</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>4</th>\n",
+                            "      <td>ecmf</td>\n",
+                            "      <td>u</td>\n",
+                            "      <td>isobaricInhPa</td>\n",
+                            "      <td>850</td>\n",
+                            "      <td>20180801</td>\n",
                             "      <td>1200</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>reduced_gg</td>\n",
+                            "      <td>regular_ll</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>5</th>\n",
+                            "      <td>ecmf</td>\n",
+                            "      <td>v</td>\n",
+                            "      <td>isobaricInhPa</td>\n",
+                            "      <td>850</td>\n",
+                            "      <td>20180801</td>\n",
+                            "      <td>1200</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>an</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "  centre shortName typeOfLevel  level  dataDate  dataTime stepRange dataType  \\\n",
-                            "0   ecmf       msl     surface      0  20230404         0         0       an   \n",
-                            "1   ecmf        2t     surface      0  20230404         0         0       an   \n",
-                            "2   ecmf       msl     surface      0  20230404      1200         0       an   \n",
-                            "3   ecmf        2t     surface      0  20230404      1200         0       an   \n",
-                            "\n",
-                            "   number    gridType  \n",
-                            "0       0  reduced_gg  \n",
-                            "1       0  reduced_gg  \n",
-                            "2       0  reduced_gg  \n",
-                            "3       0  reduced_gg  "
+                            "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange  \\\n",
+                            "0   ecmf         t  isobaricInhPa   1000  20180801      1200         0   \n",
+                            "1   ecmf         u  isobaricInhPa   1000  20180801      1200         0   \n",
+                            "2   ecmf         v  isobaricInhPa   1000  20180801      1200         0   \n",
+                            "3   ecmf         t  isobaricInhPa    850  20180801      1200         0   \n",
+                            "4   ecmf         u  isobaricInhPa    850  20180801      1200         0   \n",
+                            "5   ecmf         v  isobaricInhPa    850  20180801      1200         0   \n",
+                            "\n",
+                            "  dataType  number    gridType  \n",
+                            "0       an       0  regular_ll  \n",
+                            "1       an       0  regular_ll  \n",
+                            "2       an       0  regular_ll  \n",
+                            "3       an       0  regular_ll  \n",
+                            "4       an       0  regular_ll  \n",
+                            "5       an       0  regular_ll  "
                         ]
                     },
                     "execution_count": 12,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "fs.ls()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 13,
-            "id": "mobile-dallas",
-            "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "<class 'earthkit.data.readers.grib.index.MaskFieldSet'>\n"
-                    ]
-                }
-            ],
-            "source": [
-                "a = fs.sel(param=\"2t\")\n",
-                "print(type(a))"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 14,
-            "id": "caring-memphis",
+            "id": "static-reasoning",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -498,64 +450,65 @@
                             "      <th>gridType</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
                             "      <td>ecmf</td>\n",
-                            "      <td>2t</td>\n",
-                            "      <td>surface</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>20230404</td>\n",
-                            "      <td>0</td>\n",
+                            "      <td>t</td>\n",
+                            "      <td>isobaricInhPa</td>\n",
+                            "      <td>1000</td>\n",
+                            "      <td>20180801</td>\n",
+                            "      <td>1200</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>reduced_gg</td>\n",
+                            "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
                             "      <td>ecmf</td>\n",
-                            "      <td>2t</td>\n",
-                            "      <td>surface</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>20230404</td>\n",
+                            "      <td>t</td>\n",
+                            "      <td>isobaricInhPa</td>\n",
+                            "      <td>850</td>\n",
+                            "      <td>20180801</td>\n",
                             "      <td>1200</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>reduced_gg</td>\n",
+                            "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "  centre shortName typeOfLevel  level  dataDate  dataTime stepRange dataType  \\\n",
-                            "0   ecmf        2t     surface      0  20230404         0         0       an   \n",
-                            "1   ecmf        2t     surface      0  20230404      1200         0       an   \n",
-                            "\n",
-                            "   number    gridType  \n",
-                            "0       0  reduced_gg  \n",
-                            "1       0  reduced_gg  "
+                            "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange  \\\n",
+                            "0   ecmf         t  isobaricInhPa   1000  20180801      1200         0   \n",
+                            "1   ecmf         t  isobaricInhPa    850  20180801      1200         0   \n",
+                            "\n",
+                            "  dataType  number    gridType  \n",
+                            "0       an       0  regular_ll  \n",
+                            "1       an       0  regular_ll  "
                         ]
                     },
-                    "execution_count": 14,
+                    "execution_count": 13,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
+                "a = fs.sel(param=\"t\")\n",
                 "a.ls()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
-            "id": "after-capability",
+            "execution_count": 14,
+            "id": "spanish-wagon",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
                             "<defs>\n",
@@ -917,75 +870,93 @@
                             "  width: 1em;\n",
                             "  height: 1.5em !important;\n",
                             "  stroke-width: 0;\n",
                             "  stroke: currentColor;\n",
                             "  fill: currentColor;\n",
                             "}\n",
                             "</style><pre class='xr-text-repr-fallback'>&lt;xarray.Dataset&gt;\n",
-                            "Dimensions:     (number: 1, time: 2, step: 1, surface: 1, values: 6599680)\n",
+                            "Dimensions:        (number: 1, time: 1, step: 1, isobaricInhPa: 2, latitude: 7,\n",
+                            "                    longitude: 12)\n",
                             "Coordinates:\n",
-                            "  * number      (number) int64 0\n",
-                            "  * time        (time) datetime64[ns] 2023-04-04 2023-04-04T12:00:00\n",
-                            "  * step        (step) timedelta64[ns] 00:00:00\n",
-                            "  * surface     (surface) float64 0.0\n",
-                            "    latitude    (values) float64 ...\n",
-                            "    longitude   (values) float64 ...\n",
-                            "    valid_time  (time, step) datetime64[ns] ...\n",
-                            "Dimensions without coordinates: values\n",
+                            "  * number         (number) int64 0\n",
+                            "  * time           (time) datetime64[ns] 2018-08-01T12:00:00\n",
+                            "  * step           (step) timedelta64[ns] 00:00:00\n",
+                            "  * isobaricInhPa  (isobaricInhPa) float64 1e+03 850.0\n",
+                            "  * latitude       (latitude) float64 90.0 60.0 30.0 0.0 -30.0 -60.0 -90.0\n",
+                            "  * longitude      (longitude) float64 0.0 30.0 60.0 90.0 ... 270.0 300.0 330.0\n",
+                            "    valid_time     (time, step) datetime64[ns] ...\n",
                             "Data variables:\n",
-                            "    msl         (number, time, step, surface, values) float32 ...\n",
-                            "    t2m         (number, time, step, surface, values) float32 ...\n",
+                            "    t              (number, time, step, isobaricInhPa, latitude, longitude) float32 ...\n",
                             "Attributes:\n",
                             "    GRIB_edition:            1\n",
                             "    GRIB_centre:             ecmf\n",
                             "    GRIB_centreDescription:  European Centre for Medium-Range Weather Forecasts\n",
                             "    GRIB_subCentre:          0\n",
                             "    Conventions:             CF-1.7\n",
                             "    institution:             European Centre for Medium-Range Weather Forecasts\n",
-                            "    history:                 2023-04-05T15:29 GRIB to CDM+CF via cfgrib-0.9.1...</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.Dataset</div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-c8fe408f-6032-4547-94b9-f678ffaa5433' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-c8fe408f-6032-4547-94b9-f678ffaa5433' class='xr-section-summary'  title='Expand/collapse section'>Dimensions:</label><div class='xr-section-inline-details'><ul class='xr-dim-list'><li><span class='xr-has-index'>number</span>: 1</li><li><span class='xr-has-index'>time</span>: 2</li><li><span class='xr-has-index'>step</span>: 1</li><li><span class='xr-has-index'>surface</span>: 1</li><li><span>values</span>: 6599680</li></ul></div><div class='xr-section-details'></div></li><li class='xr-section-item'><input id='section-8a6757e4-bd1b-4cb7-96ed-07311a9f9f2f' class='xr-section-summary-in' type='checkbox'  checked><label for='section-8a6757e4-bd1b-4cb7-96ed-07311a9f9f2f' class='xr-section-summary' >Coordinates: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>number</span></div><div class='xr-var-dims'>(number)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>0</div><input id='attrs-543aa304-a106-4eff-b821-6024c22ec370' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-543aa304-a106-4eff-b821-6024c22ec370' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-66cf2f36-24a9-4d5d-ae19-e69d5a2f4048' class='xr-var-data-in' type='checkbox'><label for='data-66cf2f36-24a9-4d5d-ae19-e69d5a2f4048' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>ensemble member numerical id</dd><dt><span>units :</span></dt><dd>1</dd><dt><span>standard_name :</span></dt><dd>realization</dd></dl></div><div class='xr-var-data'><pre>array([0])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>time</span></div><div class='xr-var-dims'>(time)</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>2023-04-04 2023-04-04T12:00:00</div><input id='attrs-2a2a64db-d2b6-4613-81db-7582e141d537' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-2a2a64db-d2b6-4613-81db-7582e141d537' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-2a211f79-cc71-4ced-9542-5eb6c476dbd0' class='xr-var-data-in' type='checkbox'><label for='data-2a211f79-cc71-4ced-9542-5eb6c476dbd0' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>initial time of forecast</dd><dt><span>standard_name :</span></dt><dd>forecast_reference_time</dd></dl></div><div class='xr-var-data'><pre>array([&#x27;2023-04-04T00:00:00.000000000&#x27;, &#x27;2023-04-04T12:00:00.000000000&#x27;],\n",
-                            "      dtype=&#x27;datetime64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>step</span></div><div class='xr-var-dims'>(step)</div><div class='xr-var-dtype'>timedelta64[ns]</div><div class='xr-var-preview xr-preview'>00:00:00</div><input id='attrs-e223c24d-2ad1-4c77-b369-808b46f6271b' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-e223c24d-2ad1-4c77-b369-808b46f6271b' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-ee5ec17d-4ecc-464e-b29d-85c9c1a9a3f4' class='xr-var-data-in' type='checkbox'><label for='data-ee5ec17d-4ecc-464e-b29d-85c9c1a9a3f4' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>time since forecast_reference_time</dd><dt><span>standard_name :</span></dt><dd>forecast_period</dd></dl></div><div class='xr-var-data'><pre>array([0], dtype=&#x27;timedelta64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>surface</span></div><div class='xr-var-dims'>(surface)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>0.0</div><input id='attrs-b1af5798-b16a-4189-b349-c55dc0423627' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-b1af5798-b16a-4189-b349-c55dc0423627' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-c89dc8c1-9232-4fab-a84e-636268079710' class='xr-var-data-in' type='checkbox'><label for='data-c89dc8c1-9232-4fab-a84e-636268079710' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>original GRIB coordinate for key: level(surface)</dd><dt><span>units :</span></dt><dd>1</dd></dl></div><div class='xr-var-data'><pre>array([0.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>latitude</span></div><div class='xr-var-dims'>(values)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-6e7b1fe8-d206-4a30-8444-011011a94352' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-6e7b1fe8-d206-4a30-8444-011011a94352' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-5554df06-d93f-4a74-9e12-267734875459' class='xr-var-data-in' type='checkbox'><label for='data-5554df06-d93f-4a74-9e12-267734875459' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_north</dd><dt><span>standard_name :</span></dt><dd>latitude</dd><dt><span>long_name :</span></dt><dd>latitude</dd></dl></div><div class='xr-var-data'><pre>[6599680 values with dtype=float64]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>longitude</span></div><div class='xr-var-dims'>(values)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-3aee9941-d7e6-4519-94ae-93dff9c0314d' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-3aee9941-d7e6-4519-94ae-93dff9c0314d' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-7bc72dc1-7041-4faa-9f5c-c9c8e584f478' class='xr-var-data-in' type='checkbox'><label for='data-7bc72dc1-7041-4faa-9f5c-c9c8e584f478' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_east</dd><dt><span>standard_name :</span></dt><dd>longitude</dd><dt><span>long_name :</span></dt><dd>longitude</dd></dl></div><div class='xr-var-data'><pre>[6599680 values with dtype=float64]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>valid_time</span></div><div class='xr-var-dims'>(time, step)</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-6d0517e6-bb35-4944-ab40-5405083eed83' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-6d0517e6-bb35-4944-ab40-5405083eed83' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-d5df4dcf-3401-44b6-848c-2a702b78c9e1' class='xr-var-data-in' type='checkbox'><label for='data-d5df4dcf-3401-44b6-848c-2a702b78c9e1' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>standard_name :</span></dt><dd>time</dd><dt><span>long_name :</span></dt><dd>time</dd></dl></div><div class='xr-var-data'><pre>[2 values with dtype=datetime64[ns]]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-2dfcc14a-27cf-4c40-9dc2-a84cbc360a77' class='xr-section-summary-in' type='checkbox'  checked><label for='section-2dfcc14a-27cf-4c40-9dc2-a84cbc360a77' class='xr-section-summary' >Data variables: <span>(2)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span>msl</span></div><div class='xr-var-dims'>(number, time, step, surface, values)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-4859e8e6-f60a-456e-8b41-75fb38c332a9' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-4859e8e6-f60a-456e-8b41-75fb38c332a9' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-9b8e25b4-5a01-47d1-935f-8ba842035354' class='xr-var-data-in' type='checkbox'><label for='data-9b8e25b4-5a01-47d1-935f-8ba842035354' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>151</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>6599680</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>surface</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>reduced_gg</dd><dt><span>GRIB_N :</span></dt><dd>1280</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_cfName :</span></dt><dd>air_pressure_at_mean_sea_level</dd><dt><span>GRIB_cfVarName :</span></dt><dd>msl</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Gaussian Latitude/Longitude Grid</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>Mean sea level pressure</dd><dt><span>GRIB_pl :</span></dt><dd>[20 24 28 ... 28 24 20]</dd><dt><span>GRIB_shortName :</span></dt><dd>msl</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>Pa</dd><dt><span>long_name :</span></dt><dd>Mean sea level pressure</dd><dt><span>units :</span></dt><dd>Pa</dd><dt><span>standard_name :</span></dt><dd>air_pressure_at_mean_sea_level</dd></dl></div><div class='xr-var-data'><pre>[13199360 values with dtype=float32]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>t2m</span></div><div class='xr-var-dims'>(number, time, step, surface, values)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-f2390690-8ad2-44d7-9afe-a8788576a800' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-f2390690-8ad2-44d7-9afe-a8788576a800' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-10ecdb84-fae0-4585-8c73-0f2816253198' class='xr-var-data-in' type='checkbox'><label for='data-10ecdb84-fae0-4585-8c73-0f2816253198' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>167</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>6599680</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>surface</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>reduced_gg</dd><dt><span>GRIB_N :</span></dt><dd>1280</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_cfName :</span></dt><dd>unknown</dd><dt><span>GRIB_cfVarName :</span></dt><dd>t2m</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Gaussian Latitude/Longitude Grid</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>2 metre temperature</dd><dt><span>GRIB_pl :</span></dt><dd>[20 24 28 ... 28 24 20]</dd><dt><span>GRIB_shortName :</span></dt><dd>2t</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>K</dd><dt><span>long_name :</span></dt><dd>2 metre temperature</dd><dt><span>units :</span></dt><dd>K</dd><dt><span>standard_name :</span></dt><dd>unknown</dd></dl></div><div class='xr-var-data'><pre>[13199360 values with dtype=float32]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-728aa772-ec0c-4341-a8e8-28e29312ee97' class='xr-section-summary-in' type='checkbox'  ><label for='section-728aa772-ec0c-4341-a8e8-28e29312ee97' class='xr-section-summary' >Indexes: <span>(4)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-index-name'><div>number</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-7c4b2414-e301-4e2e-b384-6364fe6cd012' class='xr-index-data-in' type='checkbox'/><label for='index-7c4b2414-e301-4e2e-b384-6364fe6cd012' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Int64Index([0], dtype=&#x27;int64&#x27;, name=&#x27;number&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>time</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-605d4045-46f6-4e36-b458-cad855d23f10' class='xr-index-data-in' type='checkbox'/><label for='index-605d4045-46f6-4e36-b458-cad855d23f10' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(DatetimeIndex([&#x27;2023-04-04 00:00:00&#x27;, &#x27;2023-04-04 12:00:00&#x27;], dtype=&#x27;datetime64[ns]&#x27;, name=&#x27;time&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>step</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-75b32e58-d8f9-4c33-accb-ec06c6b60e40' class='xr-index-data-in' type='checkbox'/><label for='index-75b32e58-d8f9-4c33-accb-ec06c6b60e40' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(TimedeltaIndex([&#x27;0 days&#x27;], dtype=&#x27;timedelta64[ns]&#x27;, name=&#x27;step&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>surface</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-e3e6446a-fc3f-48b9-9ca4-12a572117872' class='xr-index-data-in' type='checkbox'/><label for='index-e3e6446a-fc3f-48b9-9ca4-12a572117872' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Float64Index([0.0], dtype=&#x27;float64&#x27;, name=&#x27;surface&#x27;))</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-b06702bf-3be6-4fe1-80a1-7ec5e0b04095' class='xr-section-summary-in' type='checkbox'  checked><label for='section-b06702bf-3be6-4fe1-80a1-7ec5e0b04095' class='xr-section-summary' >Attributes: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>GRIB_edition :</span></dt><dd>1</dd><dt><span>GRIB_centre :</span></dt><dd>ecmf</dd><dt><span>GRIB_centreDescription :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>GRIB_subCentre :</span></dt><dd>0</dd><dt><span>Conventions :</span></dt><dd>CF-1.7</dd><dt><span>institution :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>history :</span></dt><dd>2023-04-05T15:29 GRIB to CDM+CF via cfgrib-0.9.10.3/ecCodes-2.28.0 with {&quot;source&quot;: &quot;N/A&quot;, &quot;filter_by_keys&quot;: {}, &quot;encode_cf&quot;: [&quot;parameter&quot;, &quot;time&quot;, &quot;geography&quot;, &quot;vertical&quot;]}</dd></dl></div></li></ul></div></div>"
+                            "    history:                 2023-04-05T15:29 GRIB to CDM+CF via cfgrib-0.9.1...</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.Dataset</div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-d1102122-03a0-4c94-a5d5-9aa6331891c6' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-d1102122-03a0-4c94-a5d5-9aa6331891c6' class='xr-section-summary'  title='Expand/collapse section'>Dimensions:</label><div class='xr-section-inline-details'><ul class='xr-dim-list'><li><span class='xr-has-index'>number</span>: 1</li><li><span class='xr-has-index'>time</span>: 1</li><li><span class='xr-has-index'>step</span>: 1</li><li><span class='xr-has-index'>isobaricInhPa</span>: 2</li><li><span class='xr-has-index'>latitude</span>: 7</li><li><span class='xr-has-index'>longitude</span>: 12</li></ul></div><div class='xr-section-details'></div></li><li class='xr-section-item'><input id='section-1bfad17d-489c-4bdc-a9be-2261201199c1' class='xr-section-summary-in' type='checkbox'  checked><label for='section-1bfad17d-489c-4bdc-a9be-2261201199c1' class='xr-section-summary' >Coordinates: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>number</span></div><div class='xr-var-dims'>(number)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>0</div><input id='attrs-74878baa-8b46-4268-843e-75b535349650' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-74878baa-8b46-4268-843e-75b535349650' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-fd1a2a80-a11b-4fb7-80b1-7df3425546d5' class='xr-var-data-in' type='checkbox'><label for='data-fd1a2a80-a11b-4fb7-80b1-7df3425546d5' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>ensemble member numerical id</dd><dt><span>units :</span></dt><dd>1</dd><dt><span>standard_name :</span></dt><dd>realization</dd></dl></div><div class='xr-var-data'><pre>array([0])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>time</span></div><div class='xr-var-dims'>(time)</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>2018-08-01T12:00:00</div><input id='attrs-459d7a98-f21d-43c4-8b7f-d7320623694e' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-459d7a98-f21d-43c4-8b7f-d7320623694e' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-62fed23c-60e2-42aa-9c50-c4e6c28bfcf9' class='xr-var-data-in' type='checkbox'><label for='data-62fed23c-60e2-42aa-9c50-c4e6c28bfcf9' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>initial time of forecast</dd><dt><span>standard_name :</span></dt><dd>forecast_reference_time</dd></dl></div><div class='xr-var-data'><pre>array([&#x27;2018-08-01T12:00:00.000000000&#x27;], dtype=&#x27;datetime64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>step</span></div><div class='xr-var-dims'>(step)</div><div class='xr-var-dtype'>timedelta64[ns]</div><div class='xr-var-preview xr-preview'>00:00:00</div><input id='attrs-e7dfcd39-0370-490d-8f4e-9e0a4c59e4a2' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-e7dfcd39-0370-490d-8f4e-9e0a4c59e4a2' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-cbe7237d-c31b-43cc-8622-40affcf8f8d4' class='xr-var-data-in' type='checkbox'><label for='data-cbe7237d-c31b-43cc-8622-40affcf8f8d4' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>time since forecast_reference_time</dd><dt><span>standard_name :</span></dt><dd>forecast_period</dd></dl></div><div class='xr-var-data'><pre>array([0], dtype=&#x27;timedelta64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>isobaricInhPa</span></div><div class='xr-var-dims'>(isobaricInhPa)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>1e+03 850.0</div><input id='attrs-674d75b1-141e-4018-94ed-9b461b091097' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-674d75b1-141e-4018-94ed-9b461b091097' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-cd99e54d-ce83-46f0-857c-a7871908233c' class='xr-var-data-in' type='checkbox'><label for='data-cd99e54d-ce83-46f0-857c-a7871908233c' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>pressure</dd><dt><span>units :</span></dt><dd>hPa</dd><dt><span>positive :</span></dt><dd>down</dd><dt><span>stored_direction :</span></dt><dd>decreasing</dd><dt><span>standard_name :</span></dt><dd>air_pressure</dd></dl></div><div class='xr-var-data'><pre>array([1000.,  850.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>latitude</span></div><div class='xr-var-dims'>(latitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>90.0 60.0 30.0 ... -60.0 -90.0</div><input id='attrs-76de01e4-646f-43fd-baeb-6cf24109b05b' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-76de01e4-646f-43fd-baeb-6cf24109b05b' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-26a9b8e8-322f-4292-a96a-b55fe11d1eb6' class='xr-var-data-in' type='checkbox'><label for='data-26a9b8e8-322f-4292-a96a-b55fe11d1eb6' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_north</dd><dt><span>standard_name :</span></dt><dd>latitude</dd><dt><span>long_name :</span></dt><dd>latitude</dd><dt><span>stored_direction :</span></dt><dd>decreasing</dd></dl></div><div class='xr-var-data'><pre>array([ 90.,  60.,  30.,   0., -30., -60., -90.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>longitude</span></div><div class='xr-var-dims'>(longitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>0.0 30.0 60.0 ... 270.0 300.0 330.0</div><input id='attrs-03e49b50-1a37-4301-8f2c-a587605e298c' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-03e49b50-1a37-4301-8f2c-a587605e298c' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-f4f250f5-ab5e-4052-acae-29f207b3c8d2' class='xr-var-data-in' type='checkbox'><label for='data-f4f250f5-ab5e-4052-acae-29f207b3c8d2' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_east</dd><dt><span>standard_name :</span></dt><dd>longitude</dd><dt><span>long_name :</span></dt><dd>longitude</dd></dl></div><div class='xr-var-data'><pre>array([  0.,  30.,  60.,  90., 120., 150., 180., 210., 240., 270., 300., 330.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>valid_time</span></div><div class='xr-var-dims'>(time, step)</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-fff6e7ad-b975-4ed4-b2db-c40deffcec45' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-fff6e7ad-b975-4ed4-b2db-c40deffcec45' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-8b1dd2a2-2317-494d-84eb-af2c90812d77' class='xr-var-data-in' type='checkbox'><label for='data-8b1dd2a2-2317-494d-84eb-af2c90812d77' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>standard_name :</span></dt><dd>time</dd><dt><span>long_name :</span></dt><dd>time</dd></dl></div><div class='xr-var-data'><pre>[1 values with dtype=datetime64[ns]]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-99e0fcc8-e571-4ca9-a56a-47a96b8f5fea' class='xr-section-summary-in' type='checkbox'  checked><label for='section-99e0fcc8-e571-4ca9-a56a-47a96b8f5fea' class='xr-section-summary' >Data variables: <span>(1)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span>t</span></div><div class='xr-var-dims'>(number, time, step, isobaricInhPa, latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-504787b9-5383-4000-8bee-eb57f345fdf0' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-504787b9-5383-4000-8bee-eb57f345fdf0' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-3a8b3c65-707e-4e21-ba20-21e44f7825eb' class='xr-var-data-in' type='checkbox'><label for='data-3a8b3c65-707e-4e21-ba20-21e44f7825eb' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>130</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>84</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>isobaricInhPa</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_Nx :</span></dt><dd>12</dd><dt><span>GRIB_Ny :</span></dt><dd>7</dd><dt><span>GRIB_cfName :</span></dt><dd>air_temperature</dd><dt><span>GRIB_cfVarName :</span></dt><dd>t</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>90.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>-90.0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>0.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>330.0</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>Temperature</dd><dt><span>GRIB_shortName :</span></dt><dd>t</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>K</dd><dt><span>long_name :</span></dt><dd>Temperature</dd><dt><span>units :</span></dt><dd>K</dd><dt><span>standard_name :</span></dt><dd>air_temperature</dd></dl></div><div class='xr-var-data'><pre>[168 values with dtype=float32]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-7bcee6c5-54d1-47be-ae6b-070a01f7a6b6' class='xr-section-summary-in' type='checkbox'  ><label for='section-7bcee6c5-54d1-47be-ae6b-070a01f7a6b6' class='xr-section-summary' >Indexes: <span>(6)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-index-name'><div>number</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-1e6aff8a-d34f-4523-a4d7-314f63ac9e46' class='xr-index-data-in' type='checkbox'/><label for='index-1e6aff8a-d34f-4523-a4d7-314f63ac9e46' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Int64Index([0], dtype=&#x27;int64&#x27;, name=&#x27;number&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>time</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-bc7283a6-3b42-44aa-a35d-3a856d8858b8' class='xr-index-data-in' type='checkbox'/><label for='index-bc7283a6-3b42-44aa-a35d-3a856d8858b8' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(DatetimeIndex([&#x27;2018-08-01 12:00:00&#x27;], dtype=&#x27;datetime64[ns]&#x27;, name=&#x27;time&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>step</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-8a23791c-655d-4519-ac04-91b406350ced' class='xr-index-data-in' type='checkbox'/><label for='index-8a23791c-655d-4519-ac04-91b406350ced' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(TimedeltaIndex([&#x27;0 days&#x27;], dtype=&#x27;timedelta64[ns]&#x27;, name=&#x27;step&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>isobaricInhPa</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-07d43a66-10e8-42e6-aff0-ea8158d8ca00' class='xr-index-data-in' type='checkbox'/><label for='index-07d43a66-10e8-42e6-aff0-ea8158d8ca00' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Float64Index([1000.0, 850.0], dtype=&#x27;float64&#x27;, name=&#x27;isobaricInhPa&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>latitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-0a7f772a-949e-4f4b-8fbc-ccb737da61f6' class='xr-index-data-in' type='checkbox'/><label for='index-0a7f772a-949e-4f4b-8fbc-ccb737da61f6' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Float64Index([90.0, 60.0, 30.0, 0.0, -30.0, -60.0, -90.0], dtype=&#x27;float64&#x27;, name=&#x27;latitude&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>longitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-9a50b678-4515-48e3-9f1b-335dca4a5adf' class='xr-index-data-in' type='checkbox'/><label for='index-9a50b678-4515-48e3-9f1b-335dca4a5adf' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Float64Index([0.0, 30.0, 60.0, 90.0, 120.0, 150.0, 180.0, 210.0, 240.0, 270.0,\n",
+                            "              300.0, 330.0],\n",
+                            "             dtype=&#x27;float64&#x27;, name=&#x27;longitude&#x27;))</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-a695af4e-6bf4-479c-827a-ec82c26c911b' class='xr-section-summary-in' type='checkbox'  checked><label for='section-a695af4e-6bf4-479c-827a-ec82c26c911b' class='xr-section-summary' >Attributes: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>GRIB_edition :</span></dt><dd>1</dd><dt><span>GRIB_centre :</span></dt><dd>ecmf</dd><dt><span>GRIB_centreDescription :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>GRIB_subCentre :</span></dt><dd>0</dd><dt><span>Conventions :</span></dt><dd>CF-1.7</dd><dt><span>institution :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>history :</span></dt><dd>2023-04-05T15:29 GRIB to CDM+CF via cfgrib-0.9.10.3/ecCodes-2.28.0 with {&quot;source&quot;: &quot;N/A&quot;, &quot;filter_by_keys&quot;: {}, &quot;encode_cf&quot;: [&quot;parameter&quot;, &quot;time&quot;, &quot;geography&quot;, &quot;vertical&quot;]}</dd></dl></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<xarray.Dataset>\n",
-                            "Dimensions:     (number: 1, time: 2, step: 1, surface: 1, values: 6599680)\n",
+                            "Dimensions:        (number: 1, time: 1, step: 1, isobaricInhPa: 2, latitude: 7,\n",
+                            "                    longitude: 12)\n",
                             "Coordinates:\n",
-                            "  * number      (number) int64 0\n",
-                            "  * time        (time) datetime64[ns] 2023-04-04 2023-04-04T12:00:00\n",
-                            "  * step        (step) timedelta64[ns] 00:00:00\n",
-                            "  * surface     (surface) float64 0.0\n",
-                            "    latitude    (values) float64 ...\n",
-                            "    longitude   (values) float64 ...\n",
-                            "    valid_time  (time, step) datetime64[ns] ...\n",
-                            "Dimensions without coordinates: values\n",
+                            "  * number         (number) int64 0\n",
+                            "  * time           (time) datetime64[ns] 2018-08-01T12:00:00\n",
+                            "  * step           (step) timedelta64[ns] 00:00:00\n",
+                            "  * isobaricInhPa  (isobaricInhPa) float64 1e+03 850.0\n",
+                            "  * latitude       (latitude) float64 90.0 60.0 30.0 0.0 -30.0 -60.0 -90.0\n",
+                            "  * longitude      (longitude) float64 0.0 30.0 60.0 90.0 ... 270.0 300.0 330.0\n",
+                            "    valid_time     (time, step) datetime64[ns] ...\n",
                             "Data variables:\n",
-                            "    msl         (number, time, step, surface, values) float32 ...\n",
-                            "    t2m         (number, time, step, surface, values) float32 ...\n",
+                            "    t              (number, time, step, isobaricInhPa, latitude, longitude) float32 ...\n",
                             "Attributes:\n",
                             "    GRIB_edition:            1\n",
                             "    GRIB_centre:             ecmf\n",
                             "    GRIB_centreDescription:  European Centre for Medium-Range Weather Forecasts\n",
                             "    GRIB_subCentre:          0\n",
                             "    Conventions:             CF-1.7\n",
                             "    institution:             European Centre for Medium-Range Weather Forecasts\n",
                             "    history:                 2023-04-05T15:29 GRIB to CDM+CF via cfgrib-0.9.1..."
                         ]
                     },
-                    "execution_count": 15,
+                    "execution_count": 14,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "fs.to_xarray()"
+                "a = a.to_xarray()\n",
+                "a"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "contained-jackson",
+            "metadata": {},
+            "source": [
+                "We close the stream:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 15,
+            "id": "through-mistress",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "stream.close()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "musical-learning",
+            "id": "shared-tournament",
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
```

### Comparing `earthkit-data-0.1.2/docs/examples/grib_file_pattern.ipynb` & `earthkit-data-0.1.3/docs/examples/grib_file_pattern.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9979166666666667%*

 * *Differences: {"'cells'": "{0: {'source': ['!test -f test4.grib || wget "*

 * *            "https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test4.grib\\n', "*

 * *            "'!test -f test6.grib || wget "*

 * *            "https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test6.grib']}}"}*

```diff
@@ -5,16 +5,16 @@
             "execution_count": 1,
             "id": "96e90730-5bc9-420e-b67a-d6c69044db33",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "!test -f test4.grib || wget https://get.ecmwf.int/repository/test-data/emohawk/examples/test4.grib\n",
-                "!test -f test6.grib || wget https://get.ecmwf.int/repository/test-data/emohawk/examples/test6.grib"
+                "!test -f test4.grib || wget https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test4.grib\n",
+                "!test -f test6.grib || wget https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test6.grib"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "id": "bc208232-02b2-4ce2-bfb8-34a480198f33",
             "metadata": {},
```

### Comparing `earthkit-data-0.1.2/docs/examples/grib_from_stream.ipynb` & `earthkit-data-0.1.3/docs/examples/fdb.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.933579876186544%*

 * *Differences: {"'cells'": "{1: {'id': 'behind-carry', 'source': ['import earthkit.data']}, 3: {'id': "*

 * *            "'concrete-wallet', 'source': ['The following request was  written to retrieve data "*

 * *            'from the operational FDB at ECMWF.  Please note that the **date** must be adjusted '*

 * *            "since FDB at ECMWF only stores the most recent dates.']}, 4: {'id': 'drawn-renewal', "*

 * *            '\'source\': [\'request = {\\n\', "    \'class\': \'od\',\\n", "    \'expver\': '*

 * *            '\'0001\',\\n", "     […]*

```diff
@@ -1,275 +1,290 @@
 {
     "cells": [
         {
-            "cell_type": "code",
-            "execution_count": 1,
-            "id": "collectible-accreditation",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "!test -f test6.grib || wget https://get.ecmwf.int/repository/test-data/emohawk/examples/test6.grib"
-            ]
-        },
-        {
+            "attachments": {},
             "cell_type": "markdown",
-            "id": "recovered-organizer",
+            "id": "hourly-multimedia",
             "metadata": {},
             "source": [
-                "## Reading GRIB from a stream"
+                "## Retrieving data from FDB"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
-            "id": "sticky-refrigerator",
+            "execution_count": 1,
+            "id": "behind-carry",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import earthkit.data"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
-            "id": "german-simulation",
+            "id": "numerous-france",
             "metadata": {},
             "source": [
-                "earthkit-data can load GRIB data from a **stream**, which can be an FDB stream, a standard Python IO stream or any object implementing the necessary stream methods. \n",
+                "FDB (Fields DataBase) is a domain-specific object store developed at ECMWF for storing, indexing and retrieving GRIB data. For more information on FBD please consult the following pages:\n",
+                "\n",
+                "- [FDB](https://fields-database.readthedocs.io/en/latest/)\n",
+                "- [pyfdb](https://pyfdb.readthedocs.io/en/latest/)\n",
                 "\n",
-                "For simplicity, in this notebook we will use a **file stream** to demonstrate the usage of streams."
+                "This example requires FDB access and the <b>FDB_HOME</b> environment variable has to be set correctly. "
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "prescribed-giant",
+            "id": "concrete-wallet",
             "metadata": {},
             "source": [
-                "### Getting single items from the stream"
+                "The following request was  written to retrieve data from the operational FDB at ECMWF.  Please note that the **date** must be adjusted since FDB at ECMWF only stores the most recent dates."
             ]
         },
         {
-            "cell_type": "markdown",
-            "id": "affiliated-joint",
+            "cell_type": "code",
+            "execution_count": 2,
+            "id": "drawn-renewal",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "We create a stream from a file containing 6 GRIB fields by simply calling *open()*. It returns an io.BufferedReader object (a file stream)."
+                "request = {\n",
+                "    'class': 'od',\n",
+                "    'expver': '0001',\n",
+                "    'stream': 'oper',\n",
+                "    'date': '20230524',\n",
+                "    'time': [0, 12],\n",
+                "    'domain': 'g',\n",
+                "    'type': 'an',\n",
+                "    'levtype': 'sfc',\n",
+                "    'step': 0,\n",
+                "    'param': [151, 167]\n",
+                "}"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": 3,
-            "id": "verbal-damage",
+            "cell_type": "markdown",
+            "id": "compound-pastor",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "stream = open(\"test6.grib\", \"rb\")"
+                "### Reading as a stream"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "covered-greensboro",
+            "id": "driving-delivery",
             "metadata": {},
             "source": [
-                "We load it into earthkit-data by using the **group_by=1** (default) option. With this when we iterate through *fs* it will consume one message from the stream at a time:"
+                "We can retrieve data from FDB as a stream."
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": 4,
-            "id": "durable-helicopter",
+            "attachments": {},
+            "cell_type": "markdown",
+            "id": "bizarre-threshold",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "fs = earthkit.data.from_source(\"stream\", stream)"
+                "#### Stream: iteration with one field at a time in memory"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "resident-guard",
+            "id": "considered-excellence",
             "metadata": {},
             "source": [
-                "At this point nothing is read from the stream. As we progressing with the iteration GribField objects are created then get deleted when going out of scope. As a result there is only one GRIB message is kept in memory at a time."
+                "When we use the default arguments the resulting object can only be used for iteration and only one field is kept in memory at a time. Fields created in the iteration get deleted when going out of scope."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
-            "id": "animated-prayer",
+            "execution_count": 3,
+            "id": "signal-rocket",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "GribField(t,1000,20180801,1200,0,0)\n",
-                        "GribField(u,1000,20180801,1200,0,0)\n",
-                        "GribField(v,1000,20180801,1200,0,0)\n",
-                        "GribField(t,850,20180801,1200,0,0)\n",
-                        "GribField(u,850,20180801,1200,0,0)\n",
-                        "GribField(v,850,20180801,1200,0,0)\n"
+                        "GribField(msl,None,20230524,0,0,0)\n",
+                        "GribField(2t,None,20230524,0,0,0)\n",
+                        "GribField(msl,None,20230524,1200,0,0)\n",
+                        "GribField(2t,None,20230524,1200,0,0)\n"
                     ]
                 }
             ],
             "source": [
-                "for f in fs:\n",
-                "    # f is GribField object. It gets deleted when going out of scope\n",
+                "ds = earthkit.data.from_source(\"fdb\", request)\n",
+                "for f in ds:\n",
                 "    print(f)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "brilliant-struggle",
+            "id": "white-lebanon",
             "metadata": {},
             "source": [
-                "Having finished the iteration there is no data available any longer in *fs*.  We can close the stream:"
+                "Once the iteration is completed, there is nothing left in *ds*."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
-            "id": "unique-metadata",
+            "execution_count": 4,
+            "id": "blank-affiliate",
             "metadata": {},
             "outputs": [],
             "source": [
-                "stream.close()"
+                "for f in ds:\n",
+                "    print(f)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "judicial-backing",
+            "id": "ethical-canyon",
             "metadata": {},
             "source": [
-                "### Using group_by"
+                "#### Stream: using batch_size"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "planned-weekly",
+            "id": "standard-soviet",
             "metadata": {},
             "source": [
-                "This time we create a stream and read 2 fields from it at a time by using **group_by=2** in *from_source()*:"
+                "We can read multiple fields into memory from the stream at a time by using **batch_size** in *from_source()*:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
-            "id": "placed-blues",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "stream = open(\"test6.grib\", \"rb\")\n",
-                "fs = earthkit.data.from_source(\"stream\", stream, group_by=2)"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 8,
-            "id": "outside-tennis",
+            "execution_count": 5,
+            "id": "precise-guyana",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "2\n",
-                        "['t', 'u']\n",
-                        "2\n",
-                        "['v', 't']\n",
+                        "['msl', '2t']\n",
                         "2\n",
-                        "['u', 'v']\n"
+                        "['msl', '2t']\n"
                     ]
                 }
             ],
             "source": [
-                "for f in fs:\n",
+                "ds = earthkit.data.from_source(\"fdb\", request, batch_size=2)\n",
+                "for f in ds:\n",
                 "    # f is a FieldList containing 2 fields. It gets deleted when going out of scope\n",
                 "    print(len(f))\n",
                 "    print(f.metadata(\"param\"))"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "unavailable-actress",
+            "id": "through-seven",
             "metadata": {},
             "source": [
-                "Having finished the iteration there is no data available any longer in *fs*.  We can close the stream:"
+                "#### Stream: storing all the fields in memory"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": 9,
-            "id": "jewish-season",
+            "cell_type": "markdown",
+            "id": "personal-sense",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "stream.close()"
+                "When we use **batch_size=0** all the fields are loaded into memory and the resulting object iswill behave like a FieldList"
             ]
         },
         {
-            "cell_type": "markdown",
-            "id": "permanent-uncertainty",
+            "cell_type": "code",
+            "execution_count": 6,
+            "id": "bizarre-basket",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "### Storing each GRIB message in memory"
+                "ds = earthkit.data.from_source(\"fdb\", request, batch_size=0)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "blessed-paintball",
+            "id": "concrete-filling",
             "metadata": {},
             "source": [
-                "We can also set **group_by=0** in *from_source()*:"
+                "Nothing is read at this moment:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
-            "id": "simple-london",
+            "execution_count": 7,
+            "id": "defensive-spell",
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "stored fields count=0\n"
+                    ]
+                }
+            ],
             "source": [
-                "stream = open(\"test6.grib\", \"rb\")\n",
-                "fs = earthkit.data.from_source(\"stream\", stream, group_by=0)"
+                "print(f\"stored fields count={len(ds._reader._fields)}\")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "seeing-freight",
+            "id": "blind-houston",
             "metadata": {},
             "source": [
-                "The resulting earthkit-data object is empty at this point. However, as soon as we call any method on it it will consume the whole stream and load all the GRIB messages into memory. They will be stored in memory as long as *fs* exists.\n",
-                "\n",
-                "We can call all the standard earthkit-data methods on *fs*:"
+                "If we call any function on the fieldlist it reads the messages into memory"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
-            "id": "meaning-oxide",
+            "execution_count": 8,
+            "id": "exciting-accused",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "6"
+                            "4"
                         ]
                     },
-                    "execution_count": 11,
+                    "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "len(fs)"
+                "len(ds)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
-            "id": "copyrighted-walnut",
+            "execution_count": 9,
+            "id": "efficient-submission",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "stored fields count=4\n"
+                    ]
+                }
+            ],
+            "source": [
+                "print(f\"stored fields count={len(ds._reader._fields)}\")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 10,
+            "id": "minus-horizon",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -301,127 +316,104 @@
                             "      <th>gridType</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
                             "      <td>ecmf</td>\n",
-                            "      <td>t</td>\n",
-                            "      <td>isobaricInhPa</td>\n",
-                            "      <td>1000</td>\n",
-                            "      <td>20180801</td>\n",
-                            "      <td>1200</td>\n",
+                            "      <td>msl</td>\n",
+                            "      <td>surface</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>an</td>\n",
+                            "      <td>20230524</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>regular_ll</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>1</th>\n",
-                            "      <td>ecmf</td>\n",
-                            "      <td>u</td>\n",
-                            "      <td>isobaricInhPa</td>\n",
-                            "      <td>1000</td>\n",
-                            "      <td>20180801</td>\n",
-                            "      <td>1200</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>regular_ll</td>\n",
+                            "      <td>reduced_gg</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>2</th>\n",
+                            "      <th>1</th>\n",
                             "      <td>ecmf</td>\n",
-                            "      <td>v</td>\n",
-                            "      <td>isobaricInhPa</td>\n",
-                            "      <td>1000</td>\n",
-                            "      <td>20180801</td>\n",
-                            "      <td>1200</td>\n",
+                            "      <td>2t</td>\n",
+                            "      <td>surface</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>an</td>\n",
+                            "      <td>20230524</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>regular_ll</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>3</th>\n",
-                            "      <td>ecmf</td>\n",
-                            "      <td>t</td>\n",
-                            "      <td>isobaricInhPa</td>\n",
-                            "      <td>850</td>\n",
-                            "      <td>20180801</td>\n",
-                            "      <td>1200</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>regular_ll</td>\n",
+                            "      <td>reduced_gg</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>4</th>\n",
+                            "      <th>2</th>\n",
                             "      <td>ecmf</td>\n",
-                            "      <td>u</td>\n",
-                            "      <td>isobaricInhPa</td>\n",
-                            "      <td>850</td>\n",
-                            "      <td>20180801</td>\n",
+                            "      <td>msl</td>\n",
+                            "      <td>surface</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>20230524</td>\n",
                             "      <td>1200</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>regular_ll</td>\n",
+                            "      <td>reduced_gg</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>5</th>\n",
+                            "      <th>3</th>\n",
                             "      <td>ecmf</td>\n",
-                            "      <td>v</td>\n",
-                            "      <td>isobaricInhPa</td>\n",
-                            "      <td>850</td>\n",
-                            "      <td>20180801</td>\n",
+                            "      <td>2t</td>\n",
+                            "      <td>surface</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>20230524</td>\n",
                             "      <td>1200</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>regular_ll</td>\n",
+                            "      <td>reduced_gg</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange  \\\n",
-                            "0   ecmf         t  isobaricInhPa   1000  20180801      1200         0   \n",
-                            "1   ecmf         u  isobaricInhPa   1000  20180801      1200         0   \n",
-                            "2   ecmf         v  isobaricInhPa   1000  20180801      1200         0   \n",
-                            "3   ecmf         t  isobaricInhPa    850  20180801      1200         0   \n",
-                            "4   ecmf         u  isobaricInhPa    850  20180801      1200         0   \n",
-                            "5   ecmf         v  isobaricInhPa    850  20180801      1200         0   \n",
-                            "\n",
-                            "  dataType  number    gridType  \n",
-                            "0       an       0  regular_ll  \n",
-                            "1       an       0  regular_ll  \n",
-                            "2       an       0  regular_ll  \n",
-                            "3       an       0  regular_ll  \n",
-                            "4       an       0  regular_ll  \n",
-                            "5       an       0  regular_ll  "
+                            "  centre shortName typeOfLevel  level  dataDate  dataTime stepRange dataType  \\\n",
+                            "0   ecmf       msl     surface      0  20230524         0         0       an   \n",
+                            "1   ecmf        2t     surface      0  20230524         0         0       an   \n",
+                            "2   ecmf       msl     surface      0  20230524      1200         0       an   \n",
+                            "3   ecmf        2t     surface      0  20230524      1200         0       an   \n",
+                            "\n",
+                            "   number    gridType  \n",
+                            "0       0  reduced_gg  \n",
+                            "1       0  reduced_gg  \n",
+                            "2       0  reduced_gg  \n",
+                            "3       0  reduced_gg  "
                         ]
                     },
-                    "execution_count": 12,
+                    "execution_count": 10,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "fs.ls()"
+                "ds.ls()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
-            "id": "static-reasoning",
+            "execution_count": 11,
+            "id": "tamil-tattoo",
             "metadata": {},
             "outputs": [
                 {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "remapping={}\n"
+                    ]
+                },
+                {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
                             "    .dataframe tbody tr th:only-of-type {\n",
                             "        vertical-align: middle;\n",
                             "    }\n",
@@ -450,65 +442,64 @@
                             "      <th>gridType</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
                             "      <td>ecmf</td>\n",
-                            "      <td>t</td>\n",
-                            "      <td>isobaricInhPa</td>\n",
-                            "      <td>1000</td>\n",
-                            "      <td>20180801</td>\n",
-                            "      <td>1200</td>\n",
+                            "      <td>2t</td>\n",
+                            "      <td>surface</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>20230524</td>\n",
+                            "      <td>0</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>regular_ll</td>\n",
+                            "      <td>reduced_gg</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
                             "      <td>ecmf</td>\n",
-                            "      <td>t</td>\n",
-                            "      <td>isobaricInhPa</td>\n",
-                            "      <td>850</td>\n",
-                            "      <td>20180801</td>\n",
+                            "      <td>2t</td>\n",
+                            "      <td>surface</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>20230524</td>\n",
                             "      <td>1200</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>regular_ll</td>\n",
+                            "      <td>reduced_gg</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange  \\\n",
-                            "0   ecmf         t  isobaricInhPa   1000  20180801      1200         0   \n",
-                            "1   ecmf         t  isobaricInhPa    850  20180801      1200         0   \n",
-                            "\n",
-                            "  dataType  number    gridType  \n",
-                            "0       an       0  regular_ll  \n",
-                            "1       an       0  regular_ll  "
+                            "  centre shortName typeOfLevel  level  dataDate  dataTime stepRange dataType  \\\n",
+                            "0   ecmf        2t     surface      0  20230524         0         0       an   \n",
+                            "1   ecmf        2t     surface      0  20230524      1200         0       an   \n",
+                            "\n",
+                            "   number    gridType  \n",
+                            "0       0  reduced_gg  \n",
+                            "1       0  reduced_gg  "
                         ]
                     },
-                    "execution_count": 13,
+                    "execution_count": 11,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "a = fs.sel(param=\"t\")\n",
-                "a.ls()"
+                "ds.sel(param=\"2t\").ls()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
-            "id": "spanish-wagon",
+            "execution_count": 12,
+            "id": "assumed-month",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
                             "<defs>\n",
@@ -870,113 +861,248 @@
                             "  width: 1em;\n",
                             "  height: 1.5em !important;\n",
                             "  stroke-width: 0;\n",
                             "  stroke: currentColor;\n",
                             "  fill: currentColor;\n",
                             "}\n",
                             "</style><pre class='xr-text-repr-fallback'>&lt;xarray.Dataset&gt;\n",
-                            "Dimensions:        (number: 1, time: 1, step: 1, isobaricInhPa: 2, latitude: 7,\n",
-                            "                    longitude: 12)\n",
+                            "Dimensions:     (number: 1, time: 2, step: 1, surface: 1, values: 6599680)\n",
                             "Coordinates:\n",
-                            "  * number         (number) int64 0\n",
-                            "  * time           (time) datetime64[ns] 2018-08-01T12:00:00\n",
-                            "  * step           (step) timedelta64[ns] 00:00:00\n",
-                            "  * isobaricInhPa  (isobaricInhPa) float64 1e+03 850.0\n",
-                            "  * latitude       (latitude) float64 90.0 60.0 30.0 0.0 -30.0 -60.0 -90.0\n",
-                            "  * longitude      (longitude) float64 0.0 30.0 60.0 90.0 ... 270.0 300.0 330.0\n",
-                            "    valid_time     (time, step) datetime64[ns] ...\n",
+                            "  * number      (number) int64 0\n",
+                            "  * time        (time) datetime64[ns] 2023-05-24 2023-05-24T12:00:00\n",
+                            "  * step        (step) timedelta64[ns] 00:00:00\n",
+                            "  * surface     (surface) int64 0\n",
+                            "    latitude    (values) float64 ...\n",
+                            "    longitude   (values) float64 ...\n",
+                            "    valid_time  (time, step) datetime64[ns] ...\n",
+                            "Dimensions without coordinates: values\n",
                             "Data variables:\n",
-                            "    t              (number, time, step, isobaricInhPa, latitude, longitude) float32 ...\n",
+                            "    msl         (number, time, step, surface, values) float32 ...\n",
+                            "    t2m         (number, time, step, surface, values) float32 ...\n",
                             "Attributes:\n",
                             "    GRIB_edition:            1\n",
                             "    GRIB_centre:             ecmf\n",
                             "    GRIB_centreDescription:  European Centre for Medium-Range Weather Forecasts\n",
                             "    GRIB_subCentre:          0\n",
                             "    Conventions:             CF-1.7\n",
                             "    institution:             European Centre for Medium-Range Weather Forecasts\n",
-                            "    history:                 2023-04-05T15:29 GRIB to CDM+CF via cfgrib-0.9.1...</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.Dataset</div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-d1102122-03a0-4c94-a5d5-9aa6331891c6' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-d1102122-03a0-4c94-a5d5-9aa6331891c6' class='xr-section-summary'  title='Expand/collapse section'>Dimensions:</label><div class='xr-section-inline-details'><ul class='xr-dim-list'><li><span class='xr-has-index'>number</span>: 1</li><li><span class='xr-has-index'>time</span>: 1</li><li><span class='xr-has-index'>step</span>: 1</li><li><span class='xr-has-index'>isobaricInhPa</span>: 2</li><li><span class='xr-has-index'>latitude</span>: 7</li><li><span class='xr-has-index'>longitude</span>: 12</li></ul></div><div class='xr-section-details'></div></li><li class='xr-section-item'><input id='section-1bfad17d-489c-4bdc-a9be-2261201199c1' class='xr-section-summary-in' type='checkbox'  checked><label for='section-1bfad17d-489c-4bdc-a9be-2261201199c1' class='xr-section-summary' >Coordinates: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>number</span></div><div class='xr-var-dims'>(number)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>0</div><input id='attrs-74878baa-8b46-4268-843e-75b535349650' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-74878baa-8b46-4268-843e-75b535349650' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-fd1a2a80-a11b-4fb7-80b1-7df3425546d5' class='xr-var-data-in' type='checkbox'><label for='data-fd1a2a80-a11b-4fb7-80b1-7df3425546d5' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>ensemble member numerical id</dd><dt><span>units :</span></dt><dd>1</dd><dt><span>standard_name :</span></dt><dd>realization</dd></dl></div><div class='xr-var-data'><pre>array([0])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>time</span></div><div class='xr-var-dims'>(time)</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>2018-08-01T12:00:00</div><input id='attrs-459d7a98-f21d-43c4-8b7f-d7320623694e' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-459d7a98-f21d-43c4-8b7f-d7320623694e' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-62fed23c-60e2-42aa-9c50-c4e6c28bfcf9' class='xr-var-data-in' type='checkbox'><label for='data-62fed23c-60e2-42aa-9c50-c4e6c28bfcf9' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>initial time of forecast</dd><dt><span>standard_name :</span></dt><dd>forecast_reference_time</dd></dl></div><div class='xr-var-data'><pre>array([&#x27;2018-08-01T12:00:00.000000000&#x27;], dtype=&#x27;datetime64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>step</span></div><div class='xr-var-dims'>(step)</div><div class='xr-var-dtype'>timedelta64[ns]</div><div class='xr-var-preview xr-preview'>00:00:00</div><input id='attrs-e7dfcd39-0370-490d-8f4e-9e0a4c59e4a2' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-e7dfcd39-0370-490d-8f4e-9e0a4c59e4a2' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-cbe7237d-c31b-43cc-8622-40affcf8f8d4' class='xr-var-data-in' type='checkbox'><label for='data-cbe7237d-c31b-43cc-8622-40affcf8f8d4' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>time since forecast_reference_time</dd><dt><span>standard_name :</span></dt><dd>forecast_period</dd></dl></div><div class='xr-var-data'><pre>array([0], dtype=&#x27;timedelta64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>isobaricInhPa</span></div><div class='xr-var-dims'>(isobaricInhPa)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>1e+03 850.0</div><input id='attrs-674d75b1-141e-4018-94ed-9b461b091097' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-674d75b1-141e-4018-94ed-9b461b091097' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-cd99e54d-ce83-46f0-857c-a7871908233c' class='xr-var-data-in' type='checkbox'><label for='data-cd99e54d-ce83-46f0-857c-a7871908233c' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>pressure</dd><dt><span>units :</span></dt><dd>hPa</dd><dt><span>positive :</span></dt><dd>down</dd><dt><span>stored_direction :</span></dt><dd>decreasing</dd><dt><span>standard_name :</span></dt><dd>air_pressure</dd></dl></div><div class='xr-var-data'><pre>array([1000.,  850.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>latitude</span></div><div class='xr-var-dims'>(latitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>90.0 60.0 30.0 ... -60.0 -90.0</div><input id='attrs-76de01e4-646f-43fd-baeb-6cf24109b05b' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-76de01e4-646f-43fd-baeb-6cf24109b05b' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-26a9b8e8-322f-4292-a96a-b55fe11d1eb6' class='xr-var-data-in' type='checkbox'><label for='data-26a9b8e8-322f-4292-a96a-b55fe11d1eb6' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_north</dd><dt><span>standard_name :</span></dt><dd>latitude</dd><dt><span>long_name :</span></dt><dd>latitude</dd><dt><span>stored_direction :</span></dt><dd>decreasing</dd></dl></div><div class='xr-var-data'><pre>array([ 90.,  60.,  30.,   0., -30., -60., -90.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>longitude</span></div><div class='xr-var-dims'>(longitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>0.0 30.0 60.0 ... 270.0 300.0 330.0</div><input id='attrs-03e49b50-1a37-4301-8f2c-a587605e298c' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-03e49b50-1a37-4301-8f2c-a587605e298c' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-f4f250f5-ab5e-4052-acae-29f207b3c8d2' class='xr-var-data-in' type='checkbox'><label for='data-f4f250f5-ab5e-4052-acae-29f207b3c8d2' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_east</dd><dt><span>standard_name :</span></dt><dd>longitude</dd><dt><span>long_name :</span></dt><dd>longitude</dd></dl></div><div class='xr-var-data'><pre>array([  0.,  30.,  60.,  90., 120., 150., 180., 210., 240., 270., 300., 330.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>valid_time</span></div><div class='xr-var-dims'>(time, step)</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-fff6e7ad-b975-4ed4-b2db-c40deffcec45' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-fff6e7ad-b975-4ed4-b2db-c40deffcec45' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-8b1dd2a2-2317-494d-84eb-af2c90812d77' class='xr-var-data-in' type='checkbox'><label for='data-8b1dd2a2-2317-494d-84eb-af2c90812d77' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>standard_name :</span></dt><dd>time</dd><dt><span>long_name :</span></dt><dd>time</dd></dl></div><div class='xr-var-data'><pre>[1 values with dtype=datetime64[ns]]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-99e0fcc8-e571-4ca9-a56a-47a96b8f5fea' class='xr-section-summary-in' type='checkbox'  checked><label for='section-99e0fcc8-e571-4ca9-a56a-47a96b8f5fea' class='xr-section-summary' >Data variables: <span>(1)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span>t</span></div><div class='xr-var-dims'>(number, time, step, isobaricInhPa, latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-504787b9-5383-4000-8bee-eb57f345fdf0' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-504787b9-5383-4000-8bee-eb57f345fdf0' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-3a8b3c65-707e-4e21-ba20-21e44f7825eb' class='xr-var-data-in' type='checkbox'><label for='data-3a8b3c65-707e-4e21-ba20-21e44f7825eb' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>130</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>84</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>isobaricInhPa</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_Nx :</span></dt><dd>12</dd><dt><span>GRIB_Ny :</span></dt><dd>7</dd><dt><span>GRIB_cfName :</span></dt><dd>air_temperature</dd><dt><span>GRIB_cfVarName :</span></dt><dd>t</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>90.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>-90.0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>0.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>330.0</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>Temperature</dd><dt><span>GRIB_shortName :</span></dt><dd>t</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>K</dd><dt><span>long_name :</span></dt><dd>Temperature</dd><dt><span>units :</span></dt><dd>K</dd><dt><span>standard_name :</span></dt><dd>air_temperature</dd></dl></div><div class='xr-var-data'><pre>[168 values with dtype=float32]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-7bcee6c5-54d1-47be-ae6b-070a01f7a6b6' class='xr-section-summary-in' type='checkbox'  ><label for='section-7bcee6c5-54d1-47be-ae6b-070a01f7a6b6' class='xr-section-summary' >Indexes: <span>(6)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-index-name'><div>number</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-1e6aff8a-d34f-4523-a4d7-314f63ac9e46' class='xr-index-data-in' type='checkbox'/><label for='index-1e6aff8a-d34f-4523-a4d7-314f63ac9e46' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Int64Index([0], dtype=&#x27;int64&#x27;, name=&#x27;number&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>time</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-bc7283a6-3b42-44aa-a35d-3a856d8858b8' class='xr-index-data-in' type='checkbox'/><label for='index-bc7283a6-3b42-44aa-a35d-3a856d8858b8' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(DatetimeIndex([&#x27;2018-08-01 12:00:00&#x27;], dtype=&#x27;datetime64[ns]&#x27;, name=&#x27;time&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>step</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-8a23791c-655d-4519-ac04-91b406350ced' class='xr-index-data-in' type='checkbox'/><label for='index-8a23791c-655d-4519-ac04-91b406350ced' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(TimedeltaIndex([&#x27;0 days&#x27;], dtype=&#x27;timedelta64[ns]&#x27;, name=&#x27;step&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>isobaricInhPa</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-07d43a66-10e8-42e6-aff0-ea8158d8ca00' class='xr-index-data-in' type='checkbox'/><label for='index-07d43a66-10e8-42e6-aff0-ea8158d8ca00' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Float64Index([1000.0, 850.0], dtype=&#x27;float64&#x27;, name=&#x27;isobaricInhPa&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>latitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-0a7f772a-949e-4f4b-8fbc-ccb737da61f6' class='xr-index-data-in' type='checkbox'/><label for='index-0a7f772a-949e-4f4b-8fbc-ccb737da61f6' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Float64Index([90.0, 60.0, 30.0, 0.0, -30.0, -60.0, -90.0], dtype=&#x27;float64&#x27;, name=&#x27;latitude&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>longitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-9a50b678-4515-48e3-9f1b-335dca4a5adf' class='xr-index-data-in' type='checkbox'/><label for='index-9a50b678-4515-48e3-9f1b-335dca4a5adf' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Float64Index([0.0, 30.0, 60.0, 90.0, 120.0, 150.0, 180.0, 210.0, 240.0, 270.0,\n",
-                            "              300.0, 330.0],\n",
-                            "             dtype=&#x27;float64&#x27;, name=&#x27;longitude&#x27;))</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-a695af4e-6bf4-479c-827a-ec82c26c911b' class='xr-section-summary-in' type='checkbox'  checked><label for='section-a695af4e-6bf4-479c-827a-ec82c26c911b' class='xr-section-summary' >Attributes: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>GRIB_edition :</span></dt><dd>1</dd><dt><span>GRIB_centre :</span></dt><dd>ecmf</dd><dt><span>GRIB_centreDescription :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>GRIB_subCentre :</span></dt><dd>0</dd><dt><span>Conventions :</span></dt><dd>CF-1.7</dd><dt><span>institution :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>history :</span></dt><dd>2023-04-05T15:29 GRIB to CDM+CF via cfgrib-0.9.10.3/ecCodes-2.28.0 with {&quot;source&quot;: &quot;N/A&quot;, &quot;filter_by_keys&quot;: {}, &quot;encode_cf&quot;: [&quot;parameter&quot;, &quot;time&quot;, &quot;geography&quot;, &quot;vertical&quot;]}</dd></dl></div></li></ul></div></div>"
+                            "    history:                 2023-05-26T07:07 GRIB to CDM+CF via cfgrib-0.9.1...</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.Dataset</div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-fa78a10f-d9db-4c7e-bd3e-80361e7356d9' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-fa78a10f-d9db-4c7e-bd3e-80361e7356d9' class='xr-section-summary'  title='Expand/collapse section'>Dimensions:</label><div class='xr-section-inline-details'><ul class='xr-dim-list'><li><span class='xr-has-index'>number</span>: 1</li><li><span class='xr-has-index'>time</span>: 2</li><li><span class='xr-has-index'>step</span>: 1</li><li><span class='xr-has-index'>surface</span>: 1</li><li><span>values</span>: 6599680</li></ul></div><div class='xr-section-details'></div></li><li class='xr-section-item'><input id='section-4586cc93-b6ba-4c38-8347-116a80f84a86' class='xr-section-summary-in' type='checkbox'  checked><label for='section-4586cc93-b6ba-4c38-8347-116a80f84a86' class='xr-section-summary' >Coordinates: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>number</span></div><div class='xr-var-dims'>(number)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>0</div><input id='attrs-b1c514bb-c70e-4420-83fb-49ee40e7b9a6' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-b1c514bb-c70e-4420-83fb-49ee40e7b9a6' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-333ec79b-0849-456b-a125-292e586846c9' class='xr-var-data-in' type='checkbox'><label for='data-333ec79b-0849-456b-a125-292e586846c9' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>ensemble member numerical id</dd><dt><span>units :</span></dt><dd>1</dd><dt><span>standard_name :</span></dt><dd>realization</dd></dl></div><div class='xr-var-data'><pre>array([0])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>time</span></div><div class='xr-var-dims'>(time)</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>2023-05-24 2023-05-24T12:00:00</div><input id='attrs-b7221341-a7a1-4da6-8680-6946fcb11ef0' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-b7221341-a7a1-4da6-8680-6946fcb11ef0' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-86f69536-4962-4a01-b74e-9c846ad9294b' class='xr-var-data-in' type='checkbox'><label for='data-86f69536-4962-4a01-b74e-9c846ad9294b' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>initial time of forecast</dd><dt><span>standard_name :</span></dt><dd>forecast_reference_time</dd></dl></div><div class='xr-var-data'><pre>array([&#x27;2023-05-24T00:00:00.000000000&#x27;, &#x27;2023-05-24T12:00:00.000000000&#x27;],\n",
+                            "      dtype=&#x27;datetime64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>step</span></div><div class='xr-var-dims'>(step)</div><div class='xr-var-dtype'>timedelta64[ns]</div><div class='xr-var-preview xr-preview'>00:00:00</div><input id='attrs-2366611c-92f3-4e80-954b-904efbf7de2b' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-2366611c-92f3-4e80-954b-904efbf7de2b' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-2facf33b-36eb-4262-8db4-083480031731' class='xr-var-data-in' type='checkbox'><label for='data-2facf33b-36eb-4262-8db4-083480031731' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>time since forecast_reference_time</dd><dt><span>standard_name :</span></dt><dd>forecast_period</dd></dl></div><div class='xr-var-data'><pre>array([0], dtype=&#x27;timedelta64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>surface</span></div><div class='xr-var-dims'>(surface)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>0</div><input id='attrs-a420068a-d7b2-4676-9fca-618cd8a8ae2c' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-a420068a-d7b2-4676-9fca-618cd8a8ae2c' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-f8edc595-7f3e-4c6e-a774-6dc73666374f' class='xr-var-data-in' type='checkbox'><label for='data-f8edc595-7f3e-4c6e-a774-6dc73666374f' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>original GRIB coordinate for key: level(surface)</dd><dt><span>units :</span></dt><dd>1</dd></dl></div><div class='xr-var-data'><pre>array([0])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>latitude</span></div><div class='xr-var-dims'>(values)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-21c15ca7-c6e2-4dec-9919-b1c8e7ae246f' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-21c15ca7-c6e2-4dec-9919-b1c8e7ae246f' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-d082669a-873b-4b72-97e6-8a89385204fc' class='xr-var-data-in' type='checkbox'><label for='data-d082669a-873b-4b72-97e6-8a89385204fc' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_north</dd><dt><span>standard_name :</span></dt><dd>latitude</dd><dt><span>long_name :</span></dt><dd>latitude</dd></dl></div><div class='xr-var-data'><pre>[6599680 values with dtype=float64]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>longitude</span></div><div class='xr-var-dims'>(values)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-175be16b-a5e9-43d3-bc9b-b14ce97084f0' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-175be16b-a5e9-43d3-bc9b-b14ce97084f0' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-c2c965ef-055a-45a7-aedc-0c4545cc0280' class='xr-var-data-in' type='checkbox'><label for='data-c2c965ef-055a-45a7-aedc-0c4545cc0280' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_east</dd><dt><span>standard_name :</span></dt><dd>longitude</dd><dt><span>long_name :</span></dt><dd>longitude</dd></dl></div><div class='xr-var-data'><pre>[6599680 values with dtype=float64]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>valid_time</span></div><div class='xr-var-dims'>(time, step)</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-646dd9a0-aecb-463c-80a0-2780f98100ca' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-646dd9a0-aecb-463c-80a0-2780f98100ca' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-c07c156f-2019-410c-b5a2-b67eb202664b' class='xr-var-data-in' type='checkbox'><label for='data-c07c156f-2019-410c-b5a2-b67eb202664b' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>standard_name :</span></dt><dd>time</dd><dt><span>long_name :</span></dt><dd>time</dd></dl></div><div class='xr-var-data'><pre>[2 values with dtype=datetime64[ns]]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-54c2e21f-1909-4e94-be1d-26e1d3b82ddc' class='xr-section-summary-in' type='checkbox'  checked><label for='section-54c2e21f-1909-4e94-be1d-26e1d3b82ddc' class='xr-section-summary' >Data variables: <span>(2)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span>msl</span></div><div class='xr-var-dims'>(number, time, step, surface, values)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-ec5ae1e7-fe00-4070-8148-912b95b6bae6' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-ec5ae1e7-fe00-4070-8148-912b95b6bae6' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-829fc772-2027-4df3-8abb-4404cd506bbf' class='xr-var-data-in' type='checkbox'><label for='data-829fc772-2027-4df3-8abb-4404cd506bbf' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>151</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>6599680</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>surface</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>reduced_gg</dd><dt><span>GRIB_N :</span></dt><dd>1280</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_cfName :</span></dt><dd>air_pressure_at_mean_sea_level</dd><dt><span>GRIB_cfVarName :</span></dt><dd>msl</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Gaussian Latitude/Longitude Grid</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>Mean sea level pressure</dd><dt><span>GRIB_pl :</span></dt><dd>[20 24 28 ... 28 24 20]</dd><dt><span>GRIB_shortName :</span></dt><dd>msl</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>Pa</dd><dt><span>long_name :</span></dt><dd>Mean sea level pressure</dd><dt><span>units :</span></dt><dd>Pa</dd><dt><span>standard_name :</span></dt><dd>air_pressure_at_mean_sea_level</dd></dl></div><div class='xr-var-data'><pre>[13199360 values with dtype=float32]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>t2m</span></div><div class='xr-var-dims'>(number, time, step, surface, values)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-18359663-687c-4ee6-a919-2a739ed1460f' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-18359663-687c-4ee6-a919-2a739ed1460f' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-59cced59-1037-4e94-9082-18250deac157' class='xr-var-data-in' type='checkbox'><label for='data-59cced59-1037-4e94-9082-18250deac157' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>167</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>6599680</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>surface</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>reduced_gg</dd><dt><span>GRIB_N :</span></dt><dd>1280</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_cfName :</span></dt><dd>unknown</dd><dt><span>GRIB_cfVarName :</span></dt><dd>t2m</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Gaussian Latitude/Longitude Grid</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>2 metre temperature</dd><dt><span>GRIB_pl :</span></dt><dd>[20 24 28 ... 28 24 20]</dd><dt><span>GRIB_shortName :</span></dt><dd>2t</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>K</dd><dt><span>long_name :</span></dt><dd>2 metre temperature</dd><dt><span>units :</span></dt><dd>K</dd><dt><span>standard_name :</span></dt><dd>unknown</dd></dl></div><div class='xr-var-data'><pre>[13199360 values with dtype=float32]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-c7353cab-a0a7-4206-adc0-f5f06d1ede8c' class='xr-section-summary-in' type='checkbox'  ><label for='section-c7353cab-a0a7-4206-adc0-f5f06d1ede8c' class='xr-section-summary' >Indexes: <span>(4)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-index-name'><div>number</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-e5f4101a-e60c-447d-92f0-99c01b927616' class='xr-index-data-in' type='checkbox'/><label for='index-e5f4101a-e60c-447d-92f0-99c01b927616' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Int64Index([0], dtype=&#x27;int64&#x27;, name=&#x27;number&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>time</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-0ffe7750-3f7f-4739-90d6-bada21420101' class='xr-index-data-in' type='checkbox'/><label for='index-0ffe7750-3f7f-4739-90d6-bada21420101' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(DatetimeIndex([&#x27;2023-05-24 00:00:00&#x27;, &#x27;2023-05-24 12:00:00&#x27;], dtype=&#x27;datetime64[ns]&#x27;, name=&#x27;time&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>step</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-350d14ec-5453-4813-b52b-b48de373bc23' class='xr-index-data-in' type='checkbox'/><label for='index-350d14ec-5453-4813-b52b-b48de373bc23' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(TimedeltaIndex([&#x27;0 days&#x27;], dtype=&#x27;timedelta64[ns]&#x27;, name=&#x27;step&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>surface</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-79f62cb5-d16d-48f1-a6dd-8e9b7083bcc0' class='xr-index-data-in' type='checkbox'/><label for='index-79f62cb5-d16d-48f1-a6dd-8e9b7083bcc0' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Int64Index([0], dtype=&#x27;int64&#x27;, name=&#x27;surface&#x27;))</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-95e25296-ccc0-4b92-bb44-1885c151bfb1' class='xr-section-summary-in' type='checkbox'  checked><label for='section-95e25296-ccc0-4b92-bb44-1885c151bfb1' class='xr-section-summary' >Attributes: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>GRIB_edition :</span></dt><dd>1</dd><dt><span>GRIB_centre :</span></dt><dd>ecmf</dd><dt><span>GRIB_centreDescription :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>GRIB_subCentre :</span></dt><dd>0</dd><dt><span>Conventions :</span></dt><dd>CF-1.7</dd><dt><span>institution :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>history :</span></dt><dd>2023-05-26T07:07 GRIB to CDM+CF via cfgrib-0.9.10.3/ecCodes-2.30.0 with {&quot;source&quot;: &quot;N/A&quot;, &quot;filter_by_keys&quot;: {}, &quot;encode_cf&quot;: [&quot;parameter&quot;, &quot;time&quot;, &quot;geography&quot;, &quot;vertical&quot;]}</dd></dl></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<xarray.Dataset>\n",
-                            "Dimensions:        (number: 1, time: 1, step: 1, isobaricInhPa: 2, latitude: 7,\n",
-                            "                    longitude: 12)\n",
+                            "Dimensions:     (number: 1, time: 2, step: 1, surface: 1, values: 6599680)\n",
                             "Coordinates:\n",
-                            "  * number         (number) int64 0\n",
-                            "  * time           (time) datetime64[ns] 2018-08-01T12:00:00\n",
-                            "  * step           (step) timedelta64[ns] 00:00:00\n",
-                            "  * isobaricInhPa  (isobaricInhPa) float64 1e+03 850.0\n",
-                            "  * latitude       (latitude) float64 90.0 60.0 30.0 0.0 -30.0 -60.0 -90.0\n",
-                            "  * longitude      (longitude) float64 0.0 30.0 60.0 90.0 ... 270.0 300.0 330.0\n",
-                            "    valid_time     (time, step) datetime64[ns] ...\n",
+                            "  * number      (number) int64 0\n",
+                            "  * time        (time) datetime64[ns] 2023-05-24 2023-05-24T12:00:00\n",
+                            "  * step        (step) timedelta64[ns] 00:00:00\n",
+                            "  * surface     (surface) int64 0\n",
+                            "    latitude    (values) float64 ...\n",
+                            "    longitude   (values) float64 ...\n",
+                            "    valid_time  (time, step) datetime64[ns] ...\n",
+                            "Dimensions without coordinates: values\n",
                             "Data variables:\n",
-                            "    t              (number, time, step, isobaricInhPa, latitude, longitude) float32 ...\n",
+                            "    msl         (number, time, step, surface, values) float32 ...\n",
+                            "    t2m         (number, time, step, surface, values) float32 ...\n",
                             "Attributes:\n",
                             "    GRIB_edition:            1\n",
                             "    GRIB_centre:             ecmf\n",
                             "    GRIB_centreDescription:  European Centre for Medium-Range Weather Forecasts\n",
                             "    GRIB_subCentre:          0\n",
                             "    Conventions:             CF-1.7\n",
                             "    institution:             European Centre for Medium-Range Weather Forecasts\n",
-                            "    history:                 2023-04-05T15:29 GRIB to CDM+CF via cfgrib-0.9.1..."
+                            "    history:                 2023-05-26T07:07 GRIB to CDM+CF via cfgrib-0.9.1..."
                         ]
                     },
-                    "execution_count": 14,
+                    "execution_count": 12,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "a = a.to_xarray()\n",
-                "a"
+                "ds.to_xarray()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "decent-algeria",
+            "metadata": {},
+            "source": [
+                "### Reading into a file"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "contained-jackson",
+            "id": "exact-interstate",
             "metadata": {},
             "source": [
-                "We close the stream:"
+                "We can retrieve data from FDB into a file, which is located in the cache: "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
-            "id": "through-mistress",
+            "execution_count": 13,
+            "id": "passing-georgia",
             "metadata": {},
             "outputs": [],
             "source": [
-                "stream.close()"
+                "ds = earthkit.data.from_source(\"fdb\", request, stream=False)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 14,
+            "id": "foster-profile",
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/html": [
+                            "<div>\n",
+                            "<style scoped>\n",
+                            "    .dataframe tbody tr th:only-of-type {\n",
+                            "        vertical-align: middle;\n",
+                            "    }\n",
+                            "\n",
+                            "    .dataframe tbody tr th {\n",
+                            "        vertical-align: top;\n",
+                            "    }\n",
+                            "\n",
+                            "    .dataframe thead th {\n",
+                            "        text-align: right;\n",
+                            "    }\n",
+                            "</style>\n",
+                            "<table border=\"1\" class=\"dataframe\">\n",
+                            "  <thead>\n",
+                            "    <tr style=\"text-align: right;\">\n",
+                            "      <th></th>\n",
+                            "      <th>centre</th>\n",
+                            "      <th>shortName</th>\n",
+                            "      <th>typeOfLevel</th>\n",
+                            "      <th>level</th>\n",
+                            "      <th>dataDate</th>\n",
+                            "      <th>dataTime</th>\n",
+                            "      <th>stepRange</th>\n",
+                            "      <th>dataType</th>\n",
+                            "      <th>number</th>\n",
+                            "      <th>gridType</th>\n",
+                            "    </tr>\n",
+                            "  </thead>\n",
+                            "  <tbody>\n",
+                            "    <tr>\n",
+                            "      <th>0</th>\n",
+                            "      <td>ecmf</td>\n",
+                            "      <td>msl</td>\n",
+                            "      <td>surface</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>20230524</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>an</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>reduced_gg</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>1</th>\n",
+                            "      <td>ecmf</td>\n",
+                            "      <td>2t</td>\n",
+                            "      <td>surface</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>20230524</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>an</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>reduced_gg</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2</th>\n",
+                            "      <td>ecmf</td>\n",
+                            "      <td>msl</td>\n",
+                            "      <td>surface</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>20230524</td>\n",
+                            "      <td>1200</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>an</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>reduced_gg</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>3</th>\n",
+                            "      <td>ecmf</td>\n",
+                            "      <td>2t</td>\n",
+                            "      <td>surface</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>20230524</td>\n",
+                            "      <td>1200</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>an</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>reduced_gg</td>\n",
+                            "    </tr>\n",
+                            "  </tbody>\n",
+                            "</table>\n",
+                            "</div>"
+                        ],
+                        "text/plain": [
+                            "  centre shortName typeOfLevel  level  dataDate  dataTime stepRange dataType  \\\n",
+                            "0   ecmf       msl     surface      0  20230524         0         0       an   \n",
+                            "1   ecmf        2t     surface      0  20230524         0         0       an   \n",
+                            "2   ecmf       msl     surface      0  20230524      1200         0       an   \n",
+                            "3   ecmf        2t     surface      0  20230524      1200         0       an   \n",
+                            "\n",
+                            "   number    gridType  \n",
+                            "0       0  reduced_gg  \n",
+                            "1       0  reduced_gg  \n",
+                            "2       0  reduced_gg  \n",
+                            "3       0  reduced_gg  "
+                        ]
+                    },
+                    "execution_count": 14,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "ds.ls()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "successful-collins",
+            "metadata": {},
+            "source": [
+                "The data is now cached. Subsequent retrievals will used the cached file directly."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "shared-tournament",
+            "id": "outer-accommodation",
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "mpy38",
+            "display_name": "pyfdb",
             "language": "python",
-            "name": "mpy38"
+            "name": "pyfdb"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.16"
+            "version": "3.8.12"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `earthkit-data-0.1.2/docs/examples/grib_indexing.ipynb` & `earthkit-data-0.1.3/docs/examples/grib_indexing.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995833333333333%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '!test -f test.grib || wget "*

 * *            "https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test.grib\\n'), (1, "*

 * *            "'!test -f tuv_pl.grib || wget "*

 * *            "https://get.ecmwf.int/repository/test-data/earthkit-data/examples/tuv_pl.grib\\n')], "*

 * *            'delete: [1, 0]}}}'}*

```diff
@@ -2,16 +2,16 @@
     "cells": [
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
-                "!test -f test.grib || https://get.ecmwf.int/repository/test-data/emohawk/examples/test.grib\n",
-                "!test -f tuv_pl.grib || wget https://get.ecmwf.int/repository/test-data/emohawk/examples/tuv_pl.grib\n",
+                "!test -f test.grib || wget https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test.grib\n",
+                "!test -f tuv_pl.grib || wget https://get.ecmwf.int/repository/test-data/earthkit-data/examples/tuv_pl.grib\n",
                 "!test -d _grib_dir_with_sql || (mkdir -p _grib_dir_with_sql; cp -f test.grib tuv_pl.grib _grib_dir_with_sql/)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
```

### Comparing `earthkit-data-0.1.2/docs/examples/grib_metadata.ipynb` & `earthkit-data-0.1.3/docs/examples/grib_metadata.ipynb`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9974043721722277%*

 * *Differences: {"'cells'": "{0: {'source': ['!test -f test6.grib || wget "*

 * *            "https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test6.grib']}, 8: "*

 * *            "{'outputs': {0: {'data': {'text/plain': {insert: [(0, '  centre shortName    "*

 * *            "typeOfLevel  level  dataDate  dataTime stepRange  \\\\\\n'), (1, '0   ecmf         t  "*

 * *            "isobaricInhPa   1000  20180801      1200         0   \\n')], delete: [1, 0]}}}}}, 10: "*

 * *            "{'outputs': {0: {'data': {'text/plain': {inser […]*

```diff
@@ -4,15 +4,15 @@
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "!test -f test6.grib || wget https://get.ecmwf.int/repository/test-data/emohawk/examples/test6.grib"
+                "!test -f test6.grib || wget https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test6.grib"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Inspecting GRIB contents"
@@ -177,16 +177,16 @@
                             "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange   \n",
-                            "0   ecmf         t  isobaricInhPa   1000  20180801      1200         0  \\\n",
+                            "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange  \\\n",
+                            "0   ecmf         t  isobaricInhPa   1000  20180801      1200         0   \n",
                             "1   ecmf         u  isobaricInhPa   1000  20180801      1200         0   \n",
                             "2   ecmf         v  isobaricInhPa   1000  20180801      1200         0   \n",
                             "3   ecmf         t  isobaricInhPa    850  20180801      1200         0   \n",
                             "4   ecmf         u  isobaricInhPa    850  20180801      1200         0   \n",
                             "\n",
                             "  dataType  number    gridType  \n",
                             "0       an       0  regular_ll  \n",
@@ -280,16 +280,16 @@
                             "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange   \n",
-                            "0   ecmf         t  isobaricInhPa   1000  20180801      1200         0  \\\n",
+                            "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange  \\\n",
+                            "0   ecmf         t  isobaricInhPa   1000  20180801      1200         0   \n",
                             "1   ecmf         u  isobaricInhPa   1000  20180801      1200         0   \n",
                             "\n",
                             "  dataType  number    gridType  \n",
                             "0       an       0  regular_ll  \n",
                             "1       an       0  regular_ll  "
                         ]
                     },
@@ -370,16 +370,16 @@
                             "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange   \n",
-                            "0   ecmf         t  isobaricInhPa   1000  20180801      1200         0  \\\n",
+                            "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange  \\\n",
+                            "0   ecmf         t  isobaricInhPa   1000  20180801      1200         0   \n",
                             "1   ecmf         u  isobaricInhPa   1000  20180801      1200         0   \n",
                             "\n",
                             "  dataType  number    gridType  \n",
                             "0       an       0  regular_ll  \n",
                             "1       an       0  regular_ll  "
                         ]
                     },
@@ -790,16 +790,16 @@
                             "      <td>131</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange   \n",
-                            "0   ecmf         t  isobaricInhPa   1000  20180801      1200         0  \\\n",
+                            "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange  \\\n",
+                            "0   ecmf         t  isobaricInhPa   1000  20180801      1200         0   \n",
                             "1   ecmf         u  isobaricInhPa   1000  20180801      1200         0   \n",
                             "2   ecmf         v  isobaricInhPa   1000  20180801      1200         0   \n",
                             "3   ecmf         t  isobaricInhPa    850  20180801      1200         0   \n",
                             "4   ecmf         u  isobaricInhPa    850  20180801      1200         0   \n",
                             "\n",
                             "  dataType  number    gridType  paramId  \n",
                             "0       an       0  regular_ll      130  \n",
@@ -937,16 +937,16 @@
                             "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange   \n",
-                            "0   ecmf         u  isobaricInhPa   1000  20180801      1200         0  \\\n",
+                            "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange  \\\n",
+                            "0   ecmf         u  isobaricInhPa   1000  20180801      1200         0   \n",
                             "1   ecmf         v  isobaricInhPa   1000  20180801      1200         0   \n",
                             "2   ecmf         t  isobaricInhPa    850  20180801      1200         0   \n",
                             "3   ecmf         u  isobaricInhPa    850  20180801      1200         0   \n",
                             "4   ecmf         v  isobaricInhPa    850  20180801      1200         0   \n",
                             "\n",
                             "  dataType  number    gridType  \n",
                             "0       an       0  regular_ll  \n",
@@ -1097,16 +1097,16 @@
                             "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange   \n",
-                            "0   ecmf         t  isobaricInhPa   1000  20180801      1200         0  \\\n",
+                            "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange  \\\n",
+                            "0   ecmf         t  isobaricInhPa   1000  20180801      1200         0   \n",
                             "1   ecmf         u  isobaricInhPa   1000  20180801      1200         0   \n",
                             "2   ecmf         v  isobaricInhPa   1000  20180801      1200         0   \n",
                             "3   ecmf         t  isobaricInhPa    850  20180801      1200         0   \n",
                             "4   ecmf         u  isobaricInhPa    850  20180801      1200         0   \n",
                             "5   ecmf         v  isobaricInhPa    850  20180801      1200         0   \n",
                             "\n",
                             "  dataType  number    gridType  \n",
@@ -1200,16 +1200,16 @@
                             "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange   \n",
-                            "0   ecmf         t  isobaricInhPa   1000  20180801      1200         0  \\\n",
+                            "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange  \\\n",
+                            "0   ecmf         t  isobaricInhPa   1000  20180801      1200         0   \n",
                             "1   ecmf         u  isobaricInhPa   1000  20180801      1200         0   \n",
                             "\n",
                             "  dataType  number    gridType  \n",
                             "0       an       0  regular_ll  \n",
                             "1       an       0  regular_ll  "
                         ]
                     },
@@ -1288,16 +1288,16 @@
                             "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange   \n",
-                            "0   ecmf         u  isobaricInhPa    850  20180801      1200         0  \\\n",
+                            "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange  \\\n",
+                            "0   ecmf         u  isobaricInhPa    850  20180801      1200         0   \n",
                             "1   ecmf         v  isobaricInhPa    850  20180801      1200         0   \n",
                             "\n",
                             "  dataType  number    gridType  \n",
                             "0       an       0  regular_ll  \n",
                             "1       an       0  regular_ll  "
                         ]
                     },
@@ -1329,35 +1329,35 @@
             "execution_count": 14,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<style type=\"text/css\">\n",
-                            "#T_8ae4e th {\n",
+                            "#T_c83aa th {\n",
                             "  text-align: left;\n",
                             "}\n",
-                            "#T_8ae4e_row0_col0, #T_8ae4e_row0_col1, #T_8ae4e_row0_col2, #T_8ae4e_row0_col3, #T_8ae4e_row0_col4, #T_8ae4e_row0_col5, #T_8ae4e_row0_col6, #T_8ae4e_row0_col7, #T_8ae4e_row0_col8, #T_8ae4e_row1_col0, #T_8ae4e_row1_col1, #T_8ae4e_row1_col2, #T_8ae4e_row1_col3, #T_8ae4e_row1_col4, #T_8ae4e_row1_col5, #T_8ae4e_row1_col6, #T_8ae4e_row1_col7, #T_8ae4e_row1_col8, #T_8ae4e_row2_col0, #T_8ae4e_row2_col1, #T_8ae4e_row2_col2, #T_8ae4e_row2_col3, #T_8ae4e_row2_col4, #T_8ae4e_row2_col5, #T_8ae4e_row2_col6, #T_8ae4e_row2_col7, #T_8ae4e_row2_col8 {\n",
+                            "#T_c83aa_row0_col0, #T_c83aa_row0_col1, #T_c83aa_row0_col2, #T_c83aa_row0_col3, #T_c83aa_row0_col4, #T_c83aa_row0_col5, #T_c83aa_row0_col6, #T_c83aa_row0_col7, #T_c83aa_row0_col8, #T_c83aa_row1_col0, #T_c83aa_row1_col1, #T_c83aa_row1_col2, #T_c83aa_row1_col3, #T_c83aa_row1_col4, #T_c83aa_row1_col5, #T_c83aa_row1_col6, #T_c83aa_row1_col7, #T_c83aa_row1_col8, #T_c83aa_row2_col0, #T_c83aa_row2_col1, #T_c83aa_row2_col2, #T_c83aa_row2_col3, #T_c83aa_row2_col4, #T_c83aa_row2_col5, #T_c83aa_row2_col6, #T_c83aa_row2_col7, #T_c83aa_row2_col8 {\n",
                             "  text-align: left;\n",
                             "}\n",
                             "</style>\n",
-                            "<table id=\"T_8ae4e\">\n",
+                            "<table id=\"T_c83aa\">\n",
                             "  <thead>\n",
                             "    <tr>\n",
                             "      <th class=\"blank\" >&nbsp;</th>\n",
                             "      <th class=\"blank level0\" >&nbsp;</th>\n",
-                            "      <th id=\"T_8ae4e_level0_col0\" class=\"col_heading level0 col0\" >level</th>\n",
-                            "      <th id=\"T_8ae4e_level0_col1\" class=\"col_heading level0 col1\" >date</th>\n",
-                            "      <th id=\"T_8ae4e_level0_col2\" class=\"col_heading level0 col2\" >time</th>\n",
-                            "      <th id=\"T_8ae4e_level0_col3\" class=\"col_heading level0 col3\" >step</th>\n",
-                            "      <th id=\"T_8ae4e_level0_col4\" class=\"col_heading level0 col4\" >paramId</th>\n",
-                            "      <th id=\"T_8ae4e_level0_col5\" class=\"col_heading level0 col5\" >class</th>\n",
-                            "      <th id=\"T_8ae4e_level0_col6\" class=\"col_heading level0 col6\" >stream</th>\n",
-                            "      <th id=\"T_8ae4e_level0_col7\" class=\"col_heading level0 col7\" >type</th>\n",
-                            "      <th id=\"T_8ae4e_level0_col8\" class=\"col_heading level0 col8\" >experimentVersionNumber</th>\n",
+                            "      <th id=\"T_c83aa_level0_col0\" class=\"col_heading level0 col0\" >level</th>\n",
+                            "      <th id=\"T_c83aa_level0_col1\" class=\"col_heading level0 col1\" >date</th>\n",
+                            "      <th id=\"T_c83aa_level0_col2\" class=\"col_heading level0 col2\" >time</th>\n",
+                            "      <th id=\"T_c83aa_level0_col3\" class=\"col_heading level0 col3\" >step</th>\n",
+                            "      <th id=\"T_c83aa_level0_col4\" class=\"col_heading level0 col4\" >paramId</th>\n",
+                            "      <th id=\"T_c83aa_level0_col5\" class=\"col_heading level0 col5\" >class</th>\n",
+                            "      <th id=\"T_c83aa_level0_col6\" class=\"col_heading level0 col6\" >stream</th>\n",
+                            "      <th id=\"T_c83aa_level0_col7\" class=\"col_heading level0 col7\" >type</th>\n",
+                            "      <th id=\"T_c83aa_level0_col8\" class=\"col_heading level0 col8\" >experimentVersionNumber</th>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th class=\"index_name level0\" >shortName</th>\n",
                             "      <th class=\"index_name level1\" >typeOfLevel</th>\n",
                             "      <th class=\"blank col0\" >&nbsp;</th>\n",
                             "      <th class=\"blank col1\" >&nbsp;</th>\n",
                             "      <th class=\"blank col2\" >&nbsp;</th>\n",
@@ -1367,57 +1367,57 @@
                             "      <th class=\"blank col6\" >&nbsp;</th>\n",
                             "      <th class=\"blank col7\" >&nbsp;</th>\n",
                             "      <th class=\"blank col8\" >&nbsp;</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_8ae4e_level0_row0\" class=\"row_heading level0 row0\" >t</th>\n",
-                            "      <th id=\"T_8ae4e_level1_row0\" class=\"row_heading level1 row0\" >isobaricInhPa</th>\n",
-                            "      <td id=\"T_8ae4e_row0_col0\" class=\"data row0 col0\" >1000,850</td>\n",
-                            "      <td id=\"T_8ae4e_row0_col1\" class=\"data row0 col1\" >20180801</td>\n",
-                            "      <td id=\"T_8ae4e_row0_col2\" class=\"data row0 col2\" >1200</td>\n",
-                            "      <td id=\"T_8ae4e_row0_col3\" class=\"data row0 col3\" >0</td>\n",
-                            "      <td id=\"T_8ae4e_row0_col4\" class=\"data row0 col4\" >130</td>\n",
-                            "      <td id=\"T_8ae4e_row0_col5\" class=\"data row0 col5\" >od</td>\n",
-                            "      <td id=\"T_8ae4e_row0_col6\" class=\"data row0 col6\" >oper</td>\n",
-                            "      <td id=\"T_8ae4e_row0_col7\" class=\"data row0 col7\" >an</td>\n",
-                            "      <td id=\"T_8ae4e_row0_col8\" class=\"data row0 col8\" >0001</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th id=\"T_8ae4e_level0_row1\" class=\"row_heading level0 row1\" >u</th>\n",
-                            "      <th id=\"T_8ae4e_level1_row1\" class=\"row_heading level1 row1\" >isobaricInhPa</th>\n",
-                            "      <td id=\"T_8ae4e_row1_col0\" class=\"data row1 col0\" >1000,850</td>\n",
-                            "      <td id=\"T_8ae4e_row1_col1\" class=\"data row1 col1\" >20180801</td>\n",
-                            "      <td id=\"T_8ae4e_row1_col2\" class=\"data row1 col2\" >1200</td>\n",
-                            "      <td id=\"T_8ae4e_row1_col3\" class=\"data row1 col3\" >0</td>\n",
-                            "      <td id=\"T_8ae4e_row1_col4\" class=\"data row1 col4\" >131</td>\n",
-                            "      <td id=\"T_8ae4e_row1_col5\" class=\"data row1 col5\" >od</td>\n",
-                            "      <td id=\"T_8ae4e_row1_col6\" class=\"data row1 col6\" >oper</td>\n",
-                            "      <td id=\"T_8ae4e_row1_col7\" class=\"data row1 col7\" >an</td>\n",
-                            "      <td id=\"T_8ae4e_row1_col8\" class=\"data row1 col8\" >0001</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th id=\"T_8ae4e_level0_row2\" class=\"row_heading level0 row2\" >v</th>\n",
-                            "      <th id=\"T_8ae4e_level1_row2\" class=\"row_heading level1 row2\" >isobaricInhPa</th>\n",
-                            "      <td id=\"T_8ae4e_row2_col0\" class=\"data row2 col0\" >1000,850</td>\n",
-                            "      <td id=\"T_8ae4e_row2_col1\" class=\"data row2 col1\" >20180801</td>\n",
-                            "      <td id=\"T_8ae4e_row2_col2\" class=\"data row2 col2\" >1200</td>\n",
-                            "      <td id=\"T_8ae4e_row2_col3\" class=\"data row2 col3\" >0</td>\n",
-                            "      <td id=\"T_8ae4e_row2_col4\" class=\"data row2 col4\" >132</td>\n",
-                            "      <td id=\"T_8ae4e_row2_col5\" class=\"data row2 col5\" >od</td>\n",
-                            "      <td id=\"T_8ae4e_row2_col6\" class=\"data row2 col6\" >oper</td>\n",
-                            "      <td id=\"T_8ae4e_row2_col7\" class=\"data row2 col7\" >an</td>\n",
-                            "      <td id=\"T_8ae4e_row2_col8\" class=\"data row2 col8\" >0001</td>\n",
+                            "      <th id=\"T_c83aa_level0_row0\" class=\"row_heading level0 row0\" >t</th>\n",
+                            "      <th id=\"T_c83aa_level1_row0\" class=\"row_heading level1 row0\" >isobaricInhPa</th>\n",
+                            "      <td id=\"T_c83aa_row0_col0\" class=\"data row0 col0\" >1000,850</td>\n",
+                            "      <td id=\"T_c83aa_row0_col1\" class=\"data row0 col1\" >20180801</td>\n",
+                            "      <td id=\"T_c83aa_row0_col2\" class=\"data row0 col2\" >1200</td>\n",
+                            "      <td id=\"T_c83aa_row0_col3\" class=\"data row0 col3\" >0</td>\n",
+                            "      <td id=\"T_c83aa_row0_col4\" class=\"data row0 col4\" >130</td>\n",
+                            "      <td id=\"T_c83aa_row0_col5\" class=\"data row0 col5\" >od</td>\n",
+                            "      <td id=\"T_c83aa_row0_col6\" class=\"data row0 col6\" >oper</td>\n",
+                            "      <td id=\"T_c83aa_row0_col7\" class=\"data row0 col7\" >an</td>\n",
+                            "      <td id=\"T_c83aa_row0_col8\" class=\"data row0 col8\" >0001</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th id=\"T_c83aa_level0_row1\" class=\"row_heading level0 row1\" >u</th>\n",
+                            "      <th id=\"T_c83aa_level1_row1\" class=\"row_heading level1 row1\" >isobaricInhPa</th>\n",
+                            "      <td id=\"T_c83aa_row1_col0\" class=\"data row1 col0\" >1000,850</td>\n",
+                            "      <td id=\"T_c83aa_row1_col1\" class=\"data row1 col1\" >20180801</td>\n",
+                            "      <td id=\"T_c83aa_row1_col2\" class=\"data row1 col2\" >1200</td>\n",
+                            "      <td id=\"T_c83aa_row1_col3\" class=\"data row1 col3\" >0</td>\n",
+                            "      <td id=\"T_c83aa_row1_col4\" class=\"data row1 col4\" >131</td>\n",
+                            "      <td id=\"T_c83aa_row1_col5\" class=\"data row1 col5\" >od</td>\n",
+                            "      <td id=\"T_c83aa_row1_col6\" class=\"data row1 col6\" >oper</td>\n",
+                            "      <td id=\"T_c83aa_row1_col7\" class=\"data row1 col7\" >an</td>\n",
+                            "      <td id=\"T_c83aa_row1_col8\" class=\"data row1 col8\" >0001</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th id=\"T_c83aa_level0_row2\" class=\"row_heading level0 row2\" >v</th>\n",
+                            "      <th id=\"T_c83aa_level1_row2\" class=\"row_heading level1 row2\" >isobaricInhPa</th>\n",
+                            "      <td id=\"T_c83aa_row2_col0\" class=\"data row2 col0\" >1000,850</td>\n",
+                            "      <td id=\"T_c83aa_row2_col1\" class=\"data row2 col1\" >20180801</td>\n",
+                            "      <td id=\"T_c83aa_row2_col2\" class=\"data row2 col2\" >1200</td>\n",
+                            "      <td id=\"T_c83aa_row2_col3\" class=\"data row2 col3\" >0</td>\n",
+                            "      <td id=\"T_c83aa_row2_col4\" class=\"data row2 col4\" >132</td>\n",
+                            "      <td id=\"T_c83aa_row2_col5\" class=\"data row2 col5\" >od</td>\n",
+                            "      <td id=\"T_c83aa_row2_col6\" class=\"data row2 col6\" >oper</td>\n",
+                            "      <td id=\"T_c83aa_row2_col7\" class=\"data row2 col7\" >an</td>\n",
+                            "      <td id=\"T_c83aa_row2_col8\" class=\"data row2 col8\" >0001</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n"
                         ],
                         "text/plain": [
-                            "<pandas.io.formats.style.Styler at 0x1412bdb10>"
+                            "<pandas.io.formats.style.Styler at 0x12d88fdc0>"
                         ]
                     },
                     "execution_count": 14,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -1437,74 +1437,74 @@
             "execution_count": 15,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<style type=\"text/css\">\n",
-                            "#T_ed832 th {\n",
+                            "#T_1c6d0 th {\n",
                             "  text-align: left;\n",
                             "}\n",
-                            "#T_ed832_row0_col0, #T_ed832_row1_col0, #T_ed832_row2_col0, #T_ed832_row3_col0, #T_ed832_row4_col0, #T_ed832_row5_col0, #T_ed832_row6_col0, #T_ed832_row7_col0, #T_ed832_row8_col0, #T_ed832_row9_col0, #T_ed832_row10_col0 {\n",
+                            "#T_1c6d0_row0_col0, #T_1c6d0_row1_col0, #T_1c6d0_row2_col0, #T_1c6d0_row3_col0, #T_1c6d0_row4_col0, #T_1c6d0_row5_col0, #T_1c6d0_row6_col0, #T_1c6d0_row7_col0, #T_1c6d0_row8_col0, #T_1c6d0_row9_col0, #T_1c6d0_row10_col0 {\n",
                             "  text-align: left;\n",
                             "}\n",
                             "</style>\n",
-                            "<table id=\"T_ed832\">\n",
+                            "<table id=\"T_1c6d0\">\n",
                             "  <thead>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_ed832_level0_row0\" class=\"row_heading level0 row0\" >shortName</th>\n",
-                            "      <td id=\"T_ed832_row0_col0\" class=\"data row0 col0\" >t</td>\n",
+                            "      <th id=\"T_1c6d0_level0_row0\" class=\"row_heading level0 row0\" >shortName</th>\n",
+                            "      <td id=\"T_1c6d0_row0_col0\" class=\"data row0 col0\" >t</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_ed832_level0_row1\" class=\"row_heading level0 row1\" >typeOfLevel</th>\n",
-                            "      <td id=\"T_ed832_row1_col0\" class=\"data row1 col0\" >isobaricInhPa</td>\n",
+                            "      <th id=\"T_1c6d0_level0_row1\" class=\"row_heading level0 row1\" >typeOfLevel</th>\n",
+                            "      <td id=\"T_1c6d0_row1_col0\" class=\"data row1 col0\" >isobaricInhPa</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_ed832_level0_row2\" class=\"row_heading level0 row2\" >level</th>\n",
-                            "      <td id=\"T_ed832_row2_col0\" class=\"data row2 col0\" >1000,850</td>\n",
+                            "      <th id=\"T_1c6d0_level0_row2\" class=\"row_heading level0 row2\" >level</th>\n",
+                            "      <td id=\"T_1c6d0_row2_col0\" class=\"data row2 col0\" >1000,850</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_ed832_level0_row3\" class=\"row_heading level0 row3\" >date</th>\n",
-                            "      <td id=\"T_ed832_row3_col0\" class=\"data row3 col0\" >20180801</td>\n",
+                            "      <th id=\"T_1c6d0_level0_row3\" class=\"row_heading level0 row3\" >date</th>\n",
+                            "      <td id=\"T_1c6d0_row3_col0\" class=\"data row3 col0\" >20180801</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_ed832_level0_row4\" class=\"row_heading level0 row4\" >time</th>\n",
-                            "      <td id=\"T_ed832_row4_col0\" class=\"data row4 col0\" >1200</td>\n",
+                            "      <th id=\"T_1c6d0_level0_row4\" class=\"row_heading level0 row4\" >time</th>\n",
+                            "      <td id=\"T_1c6d0_row4_col0\" class=\"data row4 col0\" >1200</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_ed832_level0_row5\" class=\"row_heading level0 row5\" >step</th>\n",
-                            "      <td id=\"T_ed832_row5_col0\" class=\"data row5 col0\" >0</td>\n",
+                            "      <th id=\"T_1c6d0_level0_row5\" class=\"row_heading level0 row5\" >step</th>\n",
+                            "      <td id=\"T_1c6d0_row5_col0\" class=\"data row5 col0\" >0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_ed832_level0_row6\" class=\"row_heading level0 row6\" >paramId</th>\n",
-                            "      <td id=\"T_ed832_row6_col0\" class=\"data row6 col0\" >130</td>\n",
+                            "      <th id=\"T_1c6d0_level0_row6\" class=\"row_heading level0 row6\" >paramId</th>\n",
+                            "      <td id=\"T_1c6d0_row6_col0\" class=\"data row6 col0\" >130</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_ed832_level0_row7\" class=\"row_heading level0 row7\" >class</th>\n",
-                            "      <td id=\"T_ed832_row7_col0\" class=\"data row7 col0\" >od</td>\n",
+                            "      <th id=\"T_1c6d0_level0_row7\" class=\"row_heading level0 row7\" >class</th>\n",
+                            "      <td id=\"T_1c6d0_row7_col0\" class=\"data row7 col0\" >od</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_ed832_level0_row8\" class=\"row_heading level0 row8\" >stream</th>\n",
-                            "      <td id=\"T_ed832_row8_col0\" class=\"data row8 col0\" >oper</td>\n",
+                            "      <th id=\"T_1c6d0_level0_row8\" class=\"row_heading level0 row8\" >stream</th>\n",
+                            "      <td id=\"T_1c6d0_row8_col0\" class=\"data row8 col0\" >oper</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_ed832_level0_row9\" class=\"row_heading level0 row9\" >type</th>\n",
-                            "      <td id=\"T_ed832_row9_col0\" class=\"data row9 col0\" >an</td>\n",
+                            "      <th id=\"T_1c6d0_level0_row9\" class=\"row_heading level0 row9\" >type</th>\n",
+                            "      <td id=\"T_1c6d0_row9_col0\" class=\"data row9 col0\" >an</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_ed832_level0_row10\" class=\"row_heading level0 row10\" >experimentVersionNumber</th>\n",
-                            "      <td id=\"T_ed832_row10_col0\" class=\"data row10 col0\" >0001</td>\n",
+                            "      <th id=\"T_1c6d0_level0_row10\" class=\"row_heading level0 row10\" >experimentVersionNumber</th>\n",
+                            "      <td id=\"T_1c6d0_row10_col0\" class=\"data row10 col0\" >0001</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n"
                         ],
                         "text/plain": [
-                            "<pandas.io.formats.style.Styler at 0x155bf6d50>"
+                            "<pandas.io.formats.style.Styler at 0x12d8998e0>"
                         ]
                     },
                     "execution_count": 15,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -1517,74 +1517,74 @@
             "execution_count": 16,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<style type=\"text/css\">\n",
-                            "#T_f5ed5 th {\n",
+                            "#T_7aaba th {\n",
                             "  text-align: left;\n",
                             "}\n",
-                            "#T_f5ed5_row0_col0, #T_f5ed5_row1_col0, #T_f5ed5_row2_col0, #T_f5ed5_row3_col0, #T_f5ed5_row4_col0, #T_f5ed5_row5_col0, #T_f5ed5_row6_col0, #T_f5ed5_row7_col0, #T_f5ed5_row8_col0, #T_f5ed5_row9_col0, #T_f5ed5_row10_col0 {\n",
+                            "#T_7aaba_row0_col0, #T_7aaba_row1_col0, #T_7aaba_row2_col0, #T_7aaba_row3_col0, #T_7aaba_row4_col0, #T_7aaba_row5_col0, #T_7aaba_row6_col0, #T_7aaba_row7_col0, #T_7aaba_row8_col0, #T_7aaba_row9_col0, #T_7aaba_row10_col0 {\n",
                             "  text-align: left;\n",
                             "}\n",
                             "</style>\n",
-                            "<table id=\"T_f5ed5\">\n",
+                            "<table id=\"T_7aaba\">\n",
                             "  <thead>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_f5ed5_level0_row0\" class=\"row_heading level0 row0\" >shortName</th>\n",
-                            "      <td id=\"T_f5ed5_row0_col0\" class=\"data row0 col0\" >u</td>\n",
+                            "      <th id=\"T_7aaba_level0_row0\" class=\"row_heading level0 row0\" >shortName</th>\n",
+                            "      <td id=\"T_7aaba_row0_col0\" class=\"data row0 col0\" >u</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_f5ed5_level0_row1\" class=\"row_heading level0 row1\" >typeOfLevel</th>\n",
-                            "      <td id=\"T_f5ed5_row1_col0\" class=\"data row1 col0\" >isobaricInhPa</td>\n",
+                            "      <th id=\"T_7aaba_level0_row1\" class=\"row_heading level0 row1\" >typeOfLevel</th>\n",
+                            "      <td id=\"T_7aaba_row1_col0\" class=\"data row1 col0\" >isobaricInhPa</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_f5ed5_level0_row2\" class=\"row_heading level0 row2\" >level</th>\n",
-                            "      <td id=\"T_f5ed5_row2_col0\" class=\"data row2 col0\" >1000,850</td>\n",
+                            "      <th id=\"T_7aaba_level0_row2\" class=\"row_heading level0 row2\" >level</th>\n",
+                            "      <td id=\"T_7aaba_row2_col0\" class=\"data row2 col0\" >1000,850</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_f5ed5_level0_row3\" class=\"row_heading level0 row3\" >date</th>\n",
-                            "      <td id=\"T_f5ed5_row3_col0\" class=\"data row3 col0\" >20180801</td>\n",
+                            "      <th id=\"T_7aaba_level0_row3\" class=\"row_heading level0 row3\" >date</th>\n",
+                            "      <td id=\"T_7aaba_row3_col0\" class=\"data row3 col0\" >20180801</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_f5ed5_level0_row4\" class=\"row_heading level0 row4\" >time</th>\n",
-                            "      <td id=\"T_f5ed5_row4_col0\" class=\"data row4 col0\" >1200</td>\n",
+                            "      <th id=\"T_7aaba_level0_row4\" class=\"row_heading level0 row4\" >time</th>\n",
+                            "      <td id=\"T_7aaba_row4_col0\" class=\"data row4 col0\" >1200</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_f5ed5_level0_row5\" class=\"row_heading level0 row5\" >step</th>\n",
-                            "      <td id=\"T_f5ed5_row5_col0\" class=\"data row5 col0\" >0</td>\n",
+                            "      <th id=\"T_7aaba_level0_row5\" class=\"row_heading level0 row5\" >step</th>\n",
+                            "      <td id=\"T_7aaba_row5_col0\" class=\"data row5 col0\" >0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_f5ed5_level0_row6\" class=\"row_heading level0 row6\" >paramId</th>\n",
-                            "      <td id=\"T_f5ed5_row6_col0\" class=\"data row6 col0\" >131</td>\n",
+                            "      <th id=\"T_7aaba_level0_row6\" class=\"row_heading level0 row6\" >paramId</th>\n",
+                            "      <td id=\"T_7aaba_row6_col0\" class=\"data row6 col0\" >131</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_f5ed5_level0_row7\" class=\"row_heading level0 row7\" >class</th>\n",
-                            "      <td id=\"T_f5ed5_row7_col0\" class=\"data row7 col0\" >od</td>\n",
+                            "      <th id=\"T_7aaba_level0_row7\" class=\"row_heading level0 row7\" >class</th>\n",
+                            "      <td id=\"T_7aaba_row7_col0\" class=\"data row7 col0\" >od</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_f5ed5_level0_row8\" class=\"row_heading level0 row8\" >stream</th>\n",
-                            "      <td id=\"T_f5ed5_row8_col0\" class=\"data row8 col0\" >oper</td>\n",
+                            "      <th id=\"T_7aaba_level0_row8\" class=\"row_heading level0 row8\" >stream</th>\n",
+                            "      <td id=\"T_7aaba_row8_col0\" class=\"data row8 col0\" >oper</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_f5ed5_level0_row9\" class=\"row_heading level0 row9\" >type</th>\n",
-                            "      <td id=\"T_f5ed5_row9_col0\" class=\"data row9 col0\" >an</td>\n",
+                            "      <th id=\"T_7aaba_level0_row9\" class=\"row_heading level0 row9\" >type</th>\n",
+                            "      <td id=\"T_7aaba_row9_col0\" class=\"data row9 col0\" >an</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_f5ed5_level0_row10\" class=\"row_heading level0 row10\" >experimentVersionNumber</th>\n",
-                            "      <td id=\"T_f5ed5_row10_col0\" class=\"data row10 col0\" >0001</td>\n",
+                            "      <th id=\"T_7aaba_level0_row10\" class=\"row_heading level0 row10\" >experimentVersionNumber</th>\n",
+                            "      <td id=\"T_7aaba_row10_col0\" class=\"data row10 col0\" >0001</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n"
                         ],
                         "text/plain": [
-                            "<pandas.io.formats.style.Styler at 0x1558ef190>"
+                            "<pandas.io.formats.style.Styler at 0x12d909a90>"
                         ]
                     },
                     "execution_count": 16,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -1635,15 +1635,15 @@
             "cell_type": "code",
             "execution_count": 18,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "('isobaricInhPa', 1000, 'ecmf', 98)"
+                            "['isobaricInhPa', 1000, 'ecmf', 98]"
                         ]
                     },
                     "execution_count": 18,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -1864,107 +1864,107 @@
                             "</style><div class=\"eh-description\">GribField</div>\n",
                             "<div>\n",
                             "<section class=\"eh-section>\n",
                             "<div class=\"eh-tabs-container\">\n",
                             "<div class=\"eh-tabs-block\">\n",
                             "<div class=\"eh-tabs\">\n",
                             "\n",
-                            "<input type=\"radio\" name=\"eh-tabs\" id=\"bd2ba442-d557-48ff-b3a1-ba0971c1f9e7\"  />\n",
-                            "<label for=\"bd2ba442-d557-48ff-b3a1-ba0971c1f9e7\" title=\"Keys in the ecCodes None namespace\">default</label>\n",
+                            "<input type=\"radio\" name=\"eh-tabs\" id=\"74688028-9b3d-4994-ae66-f9af3ffea504\"  />\n",
+                            "<label for=\"74688028-9b3d-4994-ae66-f9af3ffea504\" title=\"Keys in the ecCodes default namespace\">default</label>\n",
                             "<div class=\"tab\">\n",
                             "<style type=\"text/css\">table.eh td {\n",
                             "    vertical-align: top;\n",
                             "    text-align: left !important;\n",
                             "}\n",
                             "</style>\n",
                             "<table class=\"eh-table\">\n",
-                            "<tr><td><b>globalDomain</b></td><td>g</td></tr> <tr><td><b>GRIBEditionNumber</b></td><td>1</td></tr> <tr><td><b>eps</b></td><td>0</td></tr> <tr><td><b>offsetSection0</b></td><td>0</td></tr> <tr><td><b>section0Length</b></td><td>8</td></tr> <tr><td><b>totalLength</b></td><td>150</td></tr> <tr><td><b>editionNumber</b></td><td>1</td></tr> <tr><td><b>WMO</b></td><td>0</td></tr> <tr><td><b>productionStatusOfProcessedData</b></td><td>0</td></tr> <tr><td><b>section1Length</b></td><td>52</td></tr> <tr><td><b>wrongPadding</b></td><td>0</td></tr> <tr><td><b>table2Version</b></td><td>128</td></tr> <tr><td><b>centre</b></td><td>ecmf</td></tr> <tr><td><b>centreDescription</b></td><td>European Centre for Medium-Range Weather Forecasts</td></tr> <tr><td><b>generatingProcessIdentifier</b></td><td>254</td></tr> <tr><td><b>gridDefinition</b></td><td>255</td></tr> <tr><td><b>indicatorOfParameter</b></td><td>130</td></tr> <tr><td><b>parameterName</b></td><td>Temperature</td></tr> <tr><td><b>parameterUnits</b></td><td>K</td></tr> <tr><td><b>indicatorOfTypeOfLevel</b></td><td>pl</td></tr> <tr><td><b>pressureUnits</b></td><td>hPa</td></tr> <tr><td><b>typeOfLevelECMF</b></td><td>isobaricInhPa</td></tr> <tr><td><b>typeOfLevel</b></td><td>isobaricInhPa</td></tr> <tr><td><b>level</b></td><td>1000</td></tr> <tr><td><b>yearOfCentury</b></td><td>18</td></tr> <tr><td><b>month</b></td><td>8</td></tr> <tr><td><b>day</b></td><td>1</td></tr> <tr><td><b>hour</b></td><td>12</td></tr> <tr><td><b>minute</b></td><td>0</td></tr> <tr><td><b>second</b></td><td>0</td></tr> <tr><td><b>unitOfTimeRange</b></td><td>1</td></tr> <tr><td><b>P1</b></td><td>0</td></tr> <tr><td><b>P2</b></td><td>0</td></tr> <tr><td><b>timeRangeIndicator</b></td><td>0</td></tr> <tr><td><b>numberIncludedInAverage</b></td><td>0</td></tr> <tr><td><b>numberMissingFromAveragesOrAccumulations</b></td><td>0</td></tr> <tr><td><b>centuryOfReferenceTimeOfData</b></td><td>21</td></tr> <tr><td><b>subCentre</b></td><td>0</td></tr> <tr><td><b>paramIdECMF</b></td><td>130</td></tr> <tr><td><b>paramId</b></td><td>130</td></tr> <tr><td><b>cfNameECMF</b></td><td>air_temperature</td></tr> <tr><td><b>cfName</b></td><td>air_temperature</td></tr> <tr><td><b>cfVarNameECMF</b></td><td>t</td></tr> <tr><td><b>cfVarName</b></td><td>t</td></tr> <tr><td><b>unitsECMF</b></td><td>K</td></tr> <tr><td><b>units</b></td><td>K</td></tr> <tr><td><b>nameECMF</b></td><td>Temperature</td></tr> <tr><td><b>name</b></td><td>Temperature</td></tr> <tr><td><b>decimalScaleFactor</b></td><td>0</td></tr> <tr><td><b>setLocalDefinition</b></td><td>0</td></tr> <tr><td><b>optimizeScaleFactor</b></td><td>0</td></tr> <tr><td><b>dataDate</b></td><td>20180801</td></tr> <tr><td><b>year</b></td><td>2018</td></tr> <tr><td><b>dataTime</b></td><td>1200</td></tr> <tr><td><b>julianDay</b></td><td>2458332.0</td></tr> <tr><td><b>stepUnits</b></td><td>1</td></tr> <tr><td><b>stepType</b></td><td>instant</td></tr> <tr><td><b>stepRange</b></td><td>0</td></tr> <tr><td><b>startStep</b></td><td>0</td></tr> <tr><td><b>endStep</b></td><td>0</td></tr> <tr><td><b>marsParam</b></td><td>130.128</td></tr> <tr><td><b>validityDate</b></td><td>20180801</td></tr> <tr><td><b>validityTime</b></td><td>1200</td></tr> <tr><td><b>deleteLocalDefinition</b></td><td>0</td></tr> <tr><td><b>localUsePresent</b></td><td>1</td></tr> <tr><td><b>reservedNeedNotBePresent</b></td><td>None</td></tr> <tr><td><b>localDefinitionNumber</b></td><td>1</td></tr> <tr><td><b>GRIBEXSection1Problem</b></td><td>0</td></tr> <tr><td><b>marsClass</b></td><td>od</td></tr> <tr><td><b>marsType</b></td><td>an</td></tr> <tr><td><b>marsStream</b></td><td>oper</td></tr> <tr><td><b>experimentVersionNumber</b></td><td>0001</td></tr> <tr><td><b>perturbationNumber</b></td><td>0</td></tr> <tr><td><b>numberOfForecastsInEnsemble</b></td><td>0</td></tr> <tr><td><b>padding_local1_1</b></td><td>None</td></tr> <tr><td><b>grib2LocalSectionNumber</b></td><td>1</td></tr> <tr><td><b>localExtensionPadding</b></td><td>None</td></tr> <tr><td><b>_x</b></td><td>None</td></tr> <tr><td><b>section1Padding</b></td><td>None</td></tr> <tr><td><b>shortNameECMF</b></td><td>t</td></tr> <tr><td><b>shortName</b></td><td>t</td></tr> <tr><td><b>ifsParam</b></td><td>130</td></tr> <tr><td><b>stepTypeForConversion</b></td><td>unknown</td></tr> <tr><td><b>md5Section1</b></td><td>3ae6b1f6f34f431c6134c40ec42f27fa</td></tr> <tr><td><b>md5Product</b></td><td>54697e1d910c88b76a8759b67e5c7a9c</td></tr> <tr><td><b>gridDescriptionSectionPresent</b></td><td>1</td></tr> <tr><td><b>bitmapPresent</b></td><td>0</td></tr> <tr><td><b>angleSubdivisions</b></td><td>1000</td></tr> <tr><td><b>section2Length</b></td><td>32</td></tr> <tr><td><b>radius</b></td><td>6367470</td></tr> <tr><td><b>numberOfVerticalCoordinateValues</b></td><td>0</td></tr> <tr><td><b>neitherPresent</b></td><td>255</td></tr> <tr><td><b>pvlLocation</b></td><td>255</td></tr> <tr><td><b>dataRepresentationType</b></td><td>0</td></tr> <tr><td><b>gridDefinitionDescription</b></td><td>Latitude/Longitude Grid</td></tr> <tr><td><b>gridDefinitionTemplateNumber</b></td><td>0</td></tr> <tr><td><b>Ni</b></td><td>12</td></tr> <tr><td><b>Nj</b></td><td>7</td></tr> <tr><td><b>latitudeOfFirstGridPoint</b></td><td>90000</td></tr> <tr><td><b>latitudeOfFirstGridPointInDegrees</b></td><td>90.0</td></tr> <tr><td><b>longitudeOfFirstGridPoint</b></td><td>0</td></tr> <tr><td><b>longitudeOfFirstGridPointInDegrees</b></td><td>0.0</td></tr> <tr><td><b>resolutionAndComponentFlags</b></td><td>128</td></tr> <tr><td><b>ijDirectionIncrementGiven</b></td><td>1</td></tr> <tr><td><b>earthIsOblate</b></td><td>0</td></tr> <tr><td><b>resolutionAndComponentFlags3</b></td><td>0</td></tr> <tr><td><b>resolutionAndComponentFlags4</b></td><td>0</td></tr> <tr><td><b>uvRelativeToGrid</b></td><td>0</td></tr> <tr><td><b>resolutionAndComponentFlags6</b></td><td>0</td></tr> <tr><td><b>resolutionAndComponentFlags7</b></td><td>0</td></tr> <tr><td><b>resolutionAndComponentFlags8</b></td><td>0</td></tr> <tr><td><b>latitudeOfLastGridPoint</b></td><td>-90000</td></tr> <tr><td><b>latitudeOfLastGridPointInDegrees</b></td><td>-90.0</td></tr> <tr><td><b>longitudeOfLastGridPoint</b></td><td>330000</td></tr> <tr><td><b>longitudeOfLastGridPointInDegrees</b></td><td>330.0</td></tr> <tr><td><b>iDirectionIncrement</b></td><td>30000</td></tr> <tr><td><b>jDirectionIncrement</b></td><td>30000</td></tr> <tr><td><b>scanningMode</b></td><td>0</td></tr> <tr><td><b>iScansNegatively</b></td><td>0</td></tr> <tr><td><b>jScansPositively</b></td><td>0</td></tr> <tr><td><b>jPointsAreConsecutive</b></td><td>0</td></tr> <tr><td><b>alternativeRowScanning</b></td><td>0</td></tr> <tr><td><b>iScansPositively</b></td><td>1</td></tr> <tr><td><b>jScansNegatively</b></td><td>1</td></tr> <tr><td><b>scanningMode4</b></td><td>0</td></tr> <tr><td><b>scanningMode5</b></td><td>0</td></tr> <tr><td><b>scanningMode6</b></td><td>0</td></tr> <tr><td><b>scanningMode7</b></td><td>0</td></tr> <tr><td><b>scanningMode8</b></td><td>0</td></tr> <tr><td><b>swapScanningAlternativeRows</b></td><td>0</td></tr> <tr><td><b>jDirectionIncrementInDegrees</b></td><td>30.0</td></tr> <tr><td><b>iDirectionIncrementInDegrees</b></td><td>30.0</td></tr> <tr><td><b>numberOfDataPoints</b></td><td>84</td></tr> <tr><td><b>numberOfValues</b></td><td>84</td></tr> <tr><td><b>zeros</b></td><td></td></tr> <tr><td><b>PVPresent</b></td><td>0</td></tr> <tr><td><b>padding_sec2_2</b></td><td>None</td></tr> <tr><td><b>PLPresent</b></td><td>0</td></tr> <tr><td><b>padding_sec2_1</b></td><td>None</td></tr> <tr><td><b>deletePV</b></td><td>1</td></tr> <tr><td><b>padding_sec2_3</b></td><td>None</td></tr> <tr><td><b>md5Section2</b></td><td>e09e4d6171c0ac85da1d256b2f8acf88</td></tr> <tr><td><b>lengthOfHeaders</b></td><td>85</td></tr> <tr><td><b>md5Headers</b></td><td>9160fb809a9d7b1efc95163bf36e6b51</td></tr> <tr><td><b>missingValue</b></td><td>9999</td></tr> <tr><td><b>tableReference</b></td><td>0</td></tr> <tr><td><b>section4Length</b></td><td>54</td></tr> <tr><td><b>halfByte</b></td><td>8</td></tr> <tr><td><b>dataFlag</b></td><td>8</td></tr> <tr><td><b>binaryScaleFactor</b></td><td>3</td></tr> <tr><td><b>referenceValue</b></td><td>240.56417846679688</td></tr> <tr><td><b>referenceValueError</b></td><td>1.52587890625e-05</td></tr> <tr><td><b>sphericalHarmonics</b></td><td>0</td></tr> <tr><td><b>complexPacking</b></td><td>0</td></tr> <tr><td><b>integerPointValues</b></td><td>0</td></tr> <tr><td><b>additionalFlagPresent</b></td><td>0</td></tr> <tr><td><b>orderOfSPD</b></td><td>2</td></tr> <tr><td><b>boustrophedonic</b></td><td>0</td></tr> <tr><td><b>hideThis</b></td><td>0</td></tr> <tr><td><b>packingType</b></td><td>grid_simple</td></tr> <tr><td><b>bitsPerValue</b></td><td>4</td></tr> <tr><td><b>constantFieldHalfByte</b></td><td>8</td></tr> <tr><td><b>bitMapIndicator</b></td><td>255</td></tr> <tr><td><b>numberOfCodedValues</b></td><td>84</td></tr> <tr><td><b>packingError</b></td><td>4.000007629394531</td></tr> <tr><td><b>unpackedError</b></td><td>1.52587890625e-05</td></tr> <tr><td><b>maximum</b></td><td>320.5641784667969</td></tr> <tr><td><b>minimum</b></td><td>240.56417846679688</td></tr> <tr><td><b>average</b></td><td>279.70703560965404</td></tr> <tr><td><b>standardDeviation</b></td><td>19.67421739058438</td></tr> <tr><td><b>skewness</b></td><td>-0.7312302105044429</td></tr> <tr><td><b>kurtosis</b></td><td>-0.16904561574741717</td></tr> <tr><td><b>isConstant</b></td><td>0.0</td></tr> <tr><td><b>numberOfMissing</b></td><td>0</td></tr> <tr><td><b>dataLength</b></td><td>5</td></tr> <tr><td><b>changeDecimalPrecision</b></td><td>0</td></tr> <tr><td><b>decimalPrecision</b></td><td>0</td></tr> <tr><td><b>bitsPerValueAndRepack</b></td><td>4</td></tr> <tr><td><b>scaleValuesBy</b></td><td>1.0</td></tr> <tr><td><b>offsetValuesBy</b></td><td>0.0</td></tr> <tr><td><b>gridType</b></td><td>regular_ll</td></tr> <tr><td><b>getNumberOfValues</b></td><td>84</td></tr> <tr><td><b>padding_sec4_1</b></td><td>None</td></tr> <tr><td><b>md5Section4</b></td><td>7ea3331d80a962b5dc99276b76451eac</td></tr> <tr><td><b>section5Length</b></td><td>4</td></tr> <tr><td><b>7777</b></td><td>7777</td></tr>\n",
+                            "<tr><td><b>globalDomain</b></td><td>g</td></tr> <tr><td><b>GRIBEditionNumber</b></td><td>1</td></tr> <tr><td><b>eps</b></td><td>0</td></tr> <tr><td><b>offsetSection0</b></td><td>0</td></tr> <tr><td><b>section0Length</b></td><td>8</td></tr> <tr><td><b>totalLength</b></td><td>150</td></tr> <tr><td><b>editionNumber</b></td><td>1</td></tr> <tr><td><b>WMO</b></td><td>0</td></tr> <tr><td><b>productionStatusOfProcessedData</b></td><td>0</td></tr> <tr><td><b>section1Length</b></td><td>52</td></tr> <tr><td><b>wrongPadding</b></td><td>0</td></tr> <tr><td><b>table2Version</b></td><td>128</td></tr> <tr><td><b>centre</b></td><td>ecmf</td></tr> <tr><td><b>centreDescription</b></td><td>European Centre for Medium-Range Weather Forecasts</td></tr> <tr><td><b>generatingProcessIdentifier</b></td><td>254</td></tr> <tr><td><b>gridDefinition</b></td><td>255</td></tr> <tr><td><b>indicatorOfParameter</b></td><td>130</td></tr> <tr><td><b>parameterName</b></td><td>Temperature</td></tr> <tr><td><b>parameterUnits</b></td><td>K</td></tr> <tr><td><b>indicatorOfTypeOfLevel</b></td><td>pl</td></tr> <tr><td><b>pressureUnits</b></td><td>hPa</td></tr> <tr><td><b>typeOfLevelECMF</b></td><td>isobaricInhPa</td></tr> <tr><td><b>typeOfLevel</b></td><td>isobaricInhPa</td></tr> <tr><td><b>level</b></td><td>1000</td></tr> <tr><td><b>yearOfCentury</b></td><td>18</td></tr> <tr><td><b>month</b></td><td>8</td></tr> <tr><td><b>day</b></td><td>1</td></tr> <tr><td><b>hour</b></td><td>12</td></tr> <tr><td><b>minute</b></td><td>0</td></tr> <tr><td><b>second</b></td><td>0</td></tr> <tr><td><b>unitOfTimeRange</b></td><td>1</td></tr> <tr><td><b>P1</b></td><td>0</td></tr> <tr><td><b>P2</b></td><td>0</td></tr> <tr><td><b>timeRangeIndicator</b></td><td>0</td></tr> <tr><td><b>numberIncludedInAverage</b></td><td>0</td></tr> <tr><td><b>mybits</b></td><td>None</td></tr> <tr><td><b>numberMissingFromAveragesOrAccumulations</b></td><td>0</td></tr> <tr><td><b>centuryOfReferenceTimeOfData</b></td><td>21</td></tr> <tr><td><b>subCentre</b></td><td>0</td></tr> <tr><td><b>paramIdECMF</b></td><td>130</td></tr> <tr><td><b>paramId</b></td><td>130</td></tr> <tr><td><b>cfNameECMF</b></td><td>air_temperature</td></tr> <tr><td><b>cfName</b></td><td>air_temperature</td></tr> <tr><td><b>cfVarNameECMF</b></td><td>t</td></tr> <tr><td><b>cfVarName</b></td><td>t</td></tr> <tr><td><b>unitsECMF</b></td><td>K</td></tr> <tr><td><b>units</b></td><td>K</td></tr> <tr><td><b>nameECMF</b></td><td>Temperature</td></tr> <tr><td><b>name</b></td><td>Temperature</td></tr> <tr><td><b>decimalScaleFactor</b></td><td>0</td></tr> <tr><td><b>setLocalDefinition</b></td><td>0</td></tr> <tr><td><b>optimizeScaleFactor</b></td><td>0</td></tr> <tr><td><b>dataDate</b></td><td>20180801</td></tr> <tr><td><b>year</b></td><td>2018</td></tr> <tr><td><b>dataTime</b></td><td>1200</td></tr> <tr><td><b>julianDay</b></td><td>2458332.0</td></tr> <tr><td><b>stepUnits</b></td><td>1</td></tr> <tr><td><b>stepType</b></td><td>instant</td></tr> <tr><td><b>stepRange</b></td><td>0</td></tr> <tr><td><b>startStep</b></td><td>0</td></tr> <tr><td><b>endStep</b></td><td>0</td></tr> <tr><td><b>marsParam</b></td><td>130.128</td></tr> <tr><td><b>validityDate</b></td><td>20180801</td></tr> <tr><td><b>validityTime</b></td><td>1200</td></tr> <tr><td><b>deleteLocalDefinition</b></td><td>0</td></tr> <tr><td><b>localUsePresent</b></td><td>1</td></tr> <tr><td><b>reservedNeedNotBePresent</b></td><td>None</td></tr> <tr><td><b>localDefinitionNumber</b></td><td>1</td></tr> <tr><td><b>GRIBEXSection1Problem</b></td><td>0</td></tr> <tr><td><b>marsClass</b></td><td>od</td></tr> <tr><td><b>marsType</b></td><td>an</td></tr> <tr><td><b>marsStream</b></td><td>oper</td></tr> <tr><td><b>experimentVersionNumber</b></td><td>0001</td></tr> <tr><td><b>perturbationNumber</b></td><td>0</td></tr> <tr><td><b>numberOfForecastsInEnsemble</b></td><td>0</td></tr> <tr><td><b>padding_local1_1</b></td><td>None</td></tr> <tr><td><b>grib2LocalSectionNumber</b></td><td>1</td></tr> <tr><td><b>localExtensionPadding</b></td><td>None</td></tr> <tr><td><b>_x</b></td><td>None</td></tr> <tr><td><b>section1Padding</b></td><td>None</td></tr> <tr><td><b>shortNameECMF</b></td><td>t</td></tr> <tr><td><b>shortName</b></td><td>t</td></tr> <tr><td><b>ifsParam</b></td><td>130</td></tr> <tr><td><b>stepTypeForConversion</b></td><td>unknown</td></tr> <tr><td><b>md5Section1</b></td><td>3ae6b1f6f34f431c6134c40ec42f27fa</td></tr> <tr><td><b>md5Product</b></td><td>54697e1d910c88b76a8759b67e5c7a9c</td></tr> <tr><td><b>gridDescriptionSectionPresent</b></td><td>1</td></tr> <tr><td><b>bitmapPresent</b></td><td>0</td></tr> <tr><td><b>angleSubdivisions</b></td><td>1000</td></tr> <tr><td><b>section2Length</b></td><td>32</td></tr> <tr><td><b>radius</b></td><td>6367470</td></tr> <tr><td><b>numberOfVerticalCoordinateValues</b></td><td>0</td></tr> <tr><td><b>neitherPresent</b></td><td>255</td></tr> <tr><td><b>pvlLocation</b></td><td>255</td></tr> <tr><td><b>dataRepresentationType</b></td><td>0</td></tr> <tr><td><b>gridDefinitionDescription</b></td><td>Latitude/Longitude Grid</td></tr> <tr><td><b>gridDefinitionTemplateNumber</b></td><td>0</td></tr> <tr><td><b>Ni</b></td><td>12</td></tr> <tr><td><b>Nj</b></td><td>7</td></tr> <tr><td><b>latitudeOfFirstGridPoint</b></td><td>90000</td></tr> <tr><td><b>latitudeOfFirstGridPointInDegrees</b></td><td>90.0</td></tr> <tr><td><b>longitudeOfFirstGridPoint</b></td><td>0</td></tr> <tr><td><b>longitudeOfFirstGridPointInDegrees</b></td><td>0.0</td></tr> <tr><td><b>resolutionAndComponentFlags</b></td><td>128</td></tr> <tr><td><b>ijDirectionIncrementGiven</b></td><td>1</td></tr> <tr><td><b>earthIsOblate</b></td><td>0</td></tr> <tr><td><b>resolutionAndComponentFlags3</b></td><td>0</td></tr> <tr><td><b>resolutionAndComponentFlags4</b></td><td>0</td></tr> <tr><td><b>uvRelativeToGrid</b></td><td>0</td></tr> <tr><td><b>resolutionAndComponentFlags6</b></td><td>0</td></tr> <tr><td><b>resolutionAndComponentFlags7</b></td><td>0</td></tr> <tr><td><b>resolutionAndComponentFlags8</b></td><td>0</td></tr> <tr><td><b>latitudeOfLastGridPoint</b></td><td>-90000</td></tr> <tr><td><b>latitudeOfLastGridPointInDegrees</b></td><td>-90.0</td></tr> <tr><td><b>longitudeOfLastGridPoint</b></td><td>330000</td></tr> <tr><td><b>longitudeOfLastGridPointInDegrees</b></td><td>330.0</td></tr> <tr><td><b>iDirectionIncrement</b></td><td>30000</td></tr> <tr><td><b>jDirectionIncrement</b></td><td>30000</td></tr> <tr><td><b>scanningMode</b></td><td>0</td></tr> <tr><td><b>iScansNegatively</b></td><td>0</td></tr> <tr><td><b>jScansPositively</b></td><td>0</td></tr> <tr><td><b>jPointsAreConsecutive</b></td><td>0</td></tr> <tr><td><b>alternativeRowScanning</b></td><td>0</td></tr> <tr><td><b>iScansPositively</b></td><td>1</td></tr> <tr><td><b>scanningMode4</b></td><td>0</td></tr> <tr><td><b>scanningMode5</b></td><td>0</td></tr> <tr><td><b>scanningMode6</b></td><td>0</td></tr> <tr><td><b>scanningMode7</b></td><td>0</td></tr> <tr><td><b>scanningMode8</b></td><td>0</td></tr> <tr><td><b>swapScanningAlternativeRows</b></td><td>0</td></tr> <tr><td><b>jDirectionIncrementInDegrees</b></td><td>30.0</td></tr> <tr><td><b>iDirectionIncrementInDegrees</b></td><td>30.0</td></tr> <tr><td><b>numberOfDataPoints</b></td><td>84</td></tr> <tr><td><b>numberOfValues</b></td><td>84</td></tr> <tr><td><b>zeros</b></td><td></td></tr> <tr><td><b>PVPresent</b></td><td>0</td></tr> <tr><td><b>padding_sec2_2</b></td><td>None</td></tr> <tr><td><b>PLPresent</b></td><td>0</td></tr> <tr><td><b>padding_sec2_1</b></td><td>None</td></tr> <tr><td><b>deletePV</b></td><td>1</td></tr> <tr><td><b>padding_sec2_3</b></td><td>None</td></tr> <tr><td><b>md5Section2</b></td><td>e09e4d6171c0ac85da1d256b2f8acf88</td></tr> <tr><td><b>lengthOfHeaders</b></td><td>85</td></tr> <tr><td><b>md5Headers</b></td><td>9160fb809a9d7b1efc95163bf36e6b51</td></tr> <tr><td><b>missingValue</b></td><td>9999</td></tr> <tr><td><b>tableReference</b></td><td>0</td></tr> <tr><td><b>section4Length</b></td><td>54</td></tr> <tr><td><b>halfByte</b></td><td>8</td></tr> <tr><td><b>dataFlag</b></td><td>8</td></tr> <tr><td><b>binaryScaleFactor</b></td><td>3</td></tr> <tr><td><b>referenceValue</b></td><td>240.56417846679688</td></tr> <tr><td><b>referenceValueError</b></td><td>1.52587890625e-05</td></tr> <tr><td><b>sphericalHarmonics</b></td><td>0</td></tr> <tr><td><b>complexPacking</b></td><td>0</td></tr> <tr><td><b>integerPointValues</b></td><td>0</td></tr> <tr><td><b>additionalFlagPresent</b></td><td>0</td></tr> <tr><td><b>orderOfSPD</b></td><td>2</td></tr> <tr><td><b>boustrophedonic</b></td><td>0</td></tr> <tr><td><b>hideThis</b></td><td>0</td></tr> <tr><td><b>packingType</b></td><td>grid_simple</td></tr> <tr><td><b>bitsPerValue</b></td><td>4</td></tr> <tr><td><b>constantFieldHalfByte</b></td><td>8</td></tr> <tr><td><b>bitMapIndicator</b></td><td>255</td></tr> <tr><td><b>numberOfCodedValues</b></td><td>84</td></tr> <tr><td><b>packingError</b></td><td>4.000007629394531</td></tr> <tr><td><b>unpackedError</b></td><td>1.52587890625e-05</td></tr> <tr><td><b>maximum</b></td><td>320.5641784667969</td></tr> <tr><td><b>minimum</b></td><td>240.56417846679688</td></tr> <tr><td><b>average</b></td><td>279.70703560965404</td></tr> <tr><td><b>numberOfMissing</b></td><td>0</td></tr> <tr><td><b>standardDeviation</b></td><td>19.67421739058438</td></tr> <tr><td><b>skewness</b></td><td>-0.7312302105044429</td></tr> <tr><td><b>kurtosis</b></td><td>-0.16904561574741717</td></tr> <tr><td><b>isConstant</b></td><td>0.0</td></tr> <tr><td><b>dataLength</b></td><td>5</td></tr> <tr><td><b>changeDecimalPrecision</b></td><td>0</td></tr> <tr><td><b>decimalPrecision</b></td><td>0</td></tr> <tr><td><b>bitsPerValueAndRepack</b></td><td>4</td></tr> <tr><td><b>scaleValuesBy</b></td><td>1.0</td></tr> <tr><td><b>offsetValuesBy</b></td><td>0.0</td></tr> <tr><td><b>gridType</b></td><td>regular_ll</td></tr> <tr><td><b>getNumberOfValues</b></td><td>84</td></tr> <tr><td><b>padding_sec4_1</b></td><td>None</td></tr> <tr><td><b>md5Section4</b></td><td>7ea3331d80a962b5dc99276b76451eac</td></tr> <tr><td><b>section5Length</b></td><td>4</td></tr> <tr><td><b>7777</b></td><td>7777</td></tr>\n",
                             "</table>\n",
                             "</div>\n",
                             "     \n",
-                            "<input type=\"radio\" name=\"eh-tabs\" id=\"1f32e53f-cf32-467f-99a1-34f536fe3df2\"  />\n",
-                            "<label for=\"1f32e53f-cf32-467f-99a1-34f536fe3df2\" title=\"Keys in the ecCodes ls namespace\">ls</label>\n",
+                            "<input type=\"radio\" name=\"eh-tabs\" id=\"339cb5be-05ae-40c9-a395-23c0530e2284\"  />\n",
+                            "<label for=\"339cb5be-05ae-40c9-a395-23c0530e2284\" title=\"Keys in the ecCodes ls namespace\">ls</label>\n",
                             "<div class=\"tab\">\n",
                             "<style type=\"text/css\">table.eh td {\n",
                             "    vertical-align: top;\n",
                             "    text-align: left !important;\n",
                             "}\n",
                             "</style>\n",
                             "<table class=\"eh-table\">\n",
                             "<tr><td><b>edition</b></td><td>1</td></tr> <tr><td><b>centre</b></td><td>ecmf</td></tr> <tr><td><b>typeOfLevel</b></td><td>isobaricInhPa</td></tr> <tr><td><b>level</b></td><td>1000</td></tr> <tr><td><b>dataDate</b></td><td>20180801</td></tr> <tr><td><b>stepRange</b></td><td>0</td></tr> <tr><td><b>dataType</b></td><td>an</td></tr> <tr><td><b>shortName</b></td><td>t</td></tr> <tr><td><b>packingType</b></td><td>grid_simple</td></tr> <tr><td><b>gridType</b></td><td>regular_ll</td></tr>\n",
                             "</table>\n",
                             "</div>\n",
                             "     \n",
-                            "<input type=\"radio\" name=\"eh-tabs\" id=\"d41e79c9-324b-40e8-8afa-e91b3790f5e6\"  />\n",
-                            "<label for=\"d41e79c9-324b-40e8-8afa-e91b3790f5e6\" title=\"Keys in the ecCodes geography namespace\">geography</label>\n",
+                            "<input type=\"radio\" name=\"eh-tabs\" id=\"e2750566-42bb-4618-af6b-be16d22b6274\"  />\n",
+                            "<label for=\"e2750566-42bb-4618-af6b-be16d22b6274\" title=\"Keys in the ecCodes geography namespace\">geography</label>\n",
                             "<div class=\"tab\">\n",
                             "<style type=\"text/css\">table.eh td {\n",
                             "    vertical-align: top;\n",
                             "    text-align: left !important;\n",
                             "}\n",
                             "</style>\n",
                             "<table class=\"eh-table\">\n",
                             "<tr><td><b>bitmapPresent</b></td><td>0</td></tr> <tr><td><b>latitudeOfFirstGridPointInDegrees</b></td><td>90.0</td></tr> <tr><td><b>longitudeOfFirstGridPointInDegrees</b></td><td>0.0</td></tr> <tr><td><b>latitudeOfLastGridPointInDegrees</b></td><td>-90.0</td></tr> <tr><td><b>longitudeOfLastGridPointInDegrees</b></td><td>330.0</td></tr> <tr><td><b>iScansNegatively</b></td><td>0</td></tr> <tr><td><b>jScansPositively</b></td><td>0</td></tr> <tr><td><b>jPointsAreConsecutive</b></td><td>0</td></tr> <tr><td><b>jDirectionIncrementInDegrees</b></td><td>30.0</td></tr> <tr><td><b>iDirectionIncrementInDegrees</b></td><td>30.0</td></tr> <tr><td><b>gridType</b></td><td>regular_ll</td></tr>\n",
                             "</table>\n",
                             "</div>\n",
                             "     \n",
-                            "<input type=\"radio\" name=\"eh-tabs\" id=\"5a953ecd-f4b9-44ac-a7b2-c7cabd0aeb46\"  />\n",
-                            "<label for=\"5a953ecd-f4b9-44ac-a7b2-c7cabd0aeb46\" title=\"Keys in the ecCodes mars namespace\">mars</label>\n",
+                            "<input type=\"radio\" name=\"eh-tabs\" id=\"694e962e-4d1f-42ab-a7b8-b34fb25a04c8\"  />\n",
+                            "<label for=\"694e962e-4d1f-42ab-a7b8-b34fb25a04c8\" title=\"Keys in the ecCodes mars namespace\">mars</label>\n",
                             "<div class=\"tab\">\n",
                             "<style type=\"text/css\">table.eh td {\n",
                             "    vertical-align: top;\n",
                             "    text-align: left !important;\n",
                             "}\n",
                             "</style>\n",
                             "<table class=\"eh-table\">\n",
                             "<tr><td><b>domain</b></td><td>g</td></tr> <tr><td><b>levtype</b></td><td>pl</td></tr> <tr><td><b>levelist</b></td><td>1000</td></tr> <tr><td><b>date</b></td><td>20180801</td></tr> <tr><td><b>time</b></td><td>1200</td></tr> <tr><td><b>step</b></td><td>0</td></tr> <tr><td><b>param</b></td><td>t</td></tr> <tr><td><b>class</b></td><td>od</td></tr> <tr><td><b>type</b></td><td>an</td></tr> <tr><td><b>stream</b></td><td>oper</td></tr> <tr><td><b>expver</b></td><td>0001</td></tr>\n",
                             "</table>\n",
                             "</div>\n",
                             "     \n",
-                            "<input type=\"radio\" name=\"eh-tabs\" id=\"db581bab-d814-40b0-ac67-d295c1615db9\" checked />\n",
-                            "<label for=\"db581bab-d814-40b0-ac67-d295c1615db9\" title=\"Keys in the ecCodes parameter namespace\">parameter</label>\n",
+                            "<input type=\"radio\" name=\"eh-tabs\" id=\"96d0fd35-c0af-4330-8b3d-efe22671f74b\" checked />\n",
+                            "<label for=\"96d0fd35-c0af-4330-8b3d-efe22671f74b\" title=\"Keys in the ecCodes parameter namespace\">parameter</label>\n",
                             "<div class=\"tab\">\n",
                             "<style type=\"text/css\">table.eh td {\n",
                             "    vertical-align: top;\n",
                             "    text-align: left !important;\n",
                             "}\n",
                             "</style>\n",
                             "<table class=\"eh-table\">\n",
                             "<tr><td><b>centre</b></td><td>ecmf</td></tr> <tr><td><b>paramId</b></td><td>130</td></tr> <tr><td><b>units</b></td><td>K</td></tr> <tr><td><b>name</b></td><td>Temperature</td></tr> <tr><td><b>shortName</b></td><td>t</td></tr>\n",
                             "</table>\n",
                             "</div>\n",
                             "     \n",
-                            "<input type=\"radio\" name=\"eh-tabs\" id=\"88d9241a-8e94-4df4-b0b6-955f6655e1cb\"  />\n",
-                            "<label for=\"88d9241a-8e94-4df4-b0b6-955f6655e1cb\" title=\"Keys in the ecCodes statistics namespace\">statistics</label>\n",
+                            "<input type=\"radio\" name=\"eh-tabs\" id=\"ebb99973-46d6-41d2-aaec-338624f06c33\"  />\n",
+                            "<label for=\"ebb99973-46d6-41d2-aaec-338624f06c33\" title=\"Keys in the ecCodes statistics namespace\">statistics</label>\n",
                             "<div class=\"tab\">\n",
                             "<style type=\"text/css\">table.eh td {\n",
                             "    vertical-align: top;\n",
                             "    text-align: left !important;\n",
                             "}\n",
                             "</style>\n",
                             "<table class=\"eh-table\">\n",
                             "<tr><td><b>max</b></td><td>320.5641784667969</td></tr> <tr><td><b>min</b></td><td>240.56417846679688</td></tr> <tr><td><b>avg</b></td><td>279.70703560965404</td></tr> <tr><td><b>sd</b></td><td>19.67421739058438</td></tr> <tr><td><b>skew</b></td><td>-0.7312302105044429</td></tr> <tr><td><b>kurt</b></td><td>-0.16904561574741717</td></tr> <tr><td><b>const</b></td><td>0.0</td></tr>\n",
                             "</table>\n",
                             "</div>\n",
                             "     \n",
-                            "<input type=\"radio\" name=\"eh-tabs\" id=\"58056fef-26ca-44cf-a0d2-4a497af48c15\"  />\n",
-                            "<label for=\"58056fef-26ca-44cf-a0d2-4a497af48c15\" title=\"Keys in the ecCodes time namespace\">time</label>\n",
+                            "<input type=\"radio\" name=\"eh-tabs\" id=\"6a4e876c-1996-4579-83d3-498dc6fce73d\"  />\n",
+                            "<label for=\"6a4e876c-1996-4579-83d3-498dc6fce73d\" title=\"Keys in the ecCodes time namespace\">time</label>\n",
                             "<div class=\"tab\">\n",
                             "<style type=\"text/css\">table.eh td {\n",
                             "    vertical-align: top;\n",
                             "    text-align: left !important;\n",
                             "}\n",
                             "</style>\n",
                             "<table class=\"eh-table\">\n",
                             "<tr><td><b>dataDate</b></td><td>20180801</td></tr> <tr><td><b>dataTime</b></td><td>1200</td></tr> <tr><td><b>stepUnits</b></td><td>1</td></tr> <tr><td><b>stepType</b></td><td>instant</td></tr> <tr><td><b>stepRange</b></td><td>0</td></tr> <tr><td><b>startStep</b></td><td>0</td></tr> <tr><td><b>endStep</b></td><td>0</td></tr> <tr><td><b>validityDate</b></td><td>20180801</td></tr> <tr><td><b>validityTime</b></td><td>1200</td></tr>\n",
                             "</table>\n",
                             "</div>\n",
                             "     \n",
-                            "<input type=\"radio\" name=\"eh-tabs\" id=\"3da2eefa-f60c-4b5a-a82c-067e2e1b367e\"  />\n",
-                            "<label for=\"3da2eefa-f60c-4b5a-a82c-067e2e1b367e\" title=\"Keys in the ecCodes vertical namespace\">vertical</label>\n",
+                            "<input type=\"radio\" name=\"eh-tabs\" id=\"92b144c0-bde3-474e-bfbf-9b982af5efe0\"  />\n",
+                            "<label for=\"92b144c0-bde3-474e-bfbf-9b982af5efe0\" title=\"Keys in the ecCodes vertical namespace\">vertical</label>\n",
                             "<div class=\"tab\">\n",
                             "<style type=\"text/css\">table.eh td {\n",
                             "    vertical-align: top;\n",
                             "    text-align: left !important;\n",
                             "}\n",
                             "</style>\n",
                             "<table class=\"eh-table\">\n",
@@ -2005,13 +2005,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.3"
+            "version": "3.8.16"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `earthkit-data-0.1.2/docs/examples/grib_missing.ipynb` & `earthkit-data-0.1.3/docs/examples/grib_missing.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99875%*

 * *Differences: {"'cells'": "{0: {'source': ['!test -f missing.grib || wget "*

 * *            "https://get.ecmwf.int/repository/test-data/earthkit-data/examples/missing.grib']}}"}*

```diff
@@ -2,15 +2,15 @@
     "cells": [
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
-                "!test -f missing.grib || wget https://get.ecmwf.int/repository/test-data/emohawk/examples/missing.grib"
+                "!test -f missing.grib || wget https://get.ecmwf.int/repository/test-data/earthkit-data/examples/missing.grib"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## GRIB missing values"
```

### Comparing `earthkit-data-0.1.2/docs/examples/grib_multi.ipynb` & `earthkit-data-0.1.3/docs/examples/grib_multi.ipynb`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9962784090909091%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '!test -f test.grib || wget "*

 * *            "https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test.grib\\n'), (1, "*

 * *            "'!test -f test4.grib || wget "*

 * *            "https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test4.grib\\n')], "*

 * *            "delete: [1, 0]}}, 7: {'outputs': {0: {'output_type': 'execute_result', 'data': "*

 * *            "OrderedDict([('text/html', "*

 * *            "['MultiFieldList(GRIBReader(test.grib),GRIBRead […]*

```diff
@@ -2,16 +2,16 @@
     "cells": [
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
-                "!test -f test.grib || wget https://get.ecmwf.int/repository/test-data/emohawk/examples/test.grib\n",
-                "!test -f test4.grib || wget https://get.ecmwf.int/repository/test-data/emohawk/examples/test4.grib\n",
+                "!test -f test.grib || wget https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test.grib\n",
+                "!test -f test4.grib || wget https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test4.grib\n",
                 "!test -d _grib_dir_no_sql || (mkdir -p _grib_dir_no_sql; cp -f test.grib test4.grib _grib_dir_no_sql/)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -72,26 +72,29 @@
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {},
             "outputs": [
                 {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        " MultiFieldSet\n",
-                        "    GRIBReader(test.grib)\n",
-                        "    GRIBReader(test4.grib)\n",
-                        "    GRIBReader(test6.grib)\n"
-                    ]
+                    "data": {
+                        "text/html": [
+                            "MultiFieldList(GRIBReader(test.grib),GRIBReader(test4.grib),GRIBReader(test6.grib))"
+                        ],
+                        "text/plain": [
+                            "MultiFieldList(GRIBReader(test.grib),GRIBReader(test4.grib),GRIBReader(test6.grib))"
+                        ]
+                    },
+                    "execution_count": 5,
+                    "metadata": {},
+                    "output_type": "execute_result"
                 }
             ],
             "source": [
-                "fs.graph()"
+                "fs"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Option 2: using a list"
@@ -128,25 +131,29 @@
         },
         {
             "cell_type": "code",
             "execution_count": 8,
             "metadata": {},
             "outputs": [
                 {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        " MultiFieldSet\n",
-                        "    GRIBReader(test.grib)\n",
-                        "    GRIBReader(test4.grib)\n"
-                    ]
+                    "data": {
+                        "text/html": [
+                            "MultiFieldList(GRIBReader(test.grib),GRIBReader(test4.grib))"
+                        ],
+                        "text/plain": [
+                            "MultiFieldList(GRIBReader(test.grib),GRIBReader(test4.grib))"
+                        ]
+                    },
+                    "execution_count": 8,
+                    "metadata": {},
+                    "output_type": "execute_result"
                 }
             ],
             "source": [
-                "fs.graph()"
+                "fs"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Option 3: reading all files in a directory"
@@ -183,25 +190,29 @@
         },
         {
             "cell_type": "code",
             "execution_count": 11,
             "metadata": {},
             "outputs": [
                 {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        " MultiFieldSet\n",
-                        "    GRIBReader(./_grib_dir_no_sql/test.grib)\n",
-                        "    GRIBReader(./_grib_dir_no_sql/test4.grib)\n"
-                    ]
+                    "data": {
+                        "text/html": [
+                            "MultiFieldList(GRIBReader(./_grib_dir_no_sql/test.grib),GRIBReader(./_grib_dir_no_sql/test4.grib))"
+                        ],
+                        "text/plain": [
+                            "MultiFieldList(GRIBReader(./_grib_dir_no_sql/test.grib),GRIBReader(./_grib_dir_no_sql/test4.grib))"
+                        ]
+                    },
+                    "execution_count": 11,
+                    "metadata": {},
+                    "output_type": "execute_result"
                 }
             ],
             "source": [
-                "fs.graph()"
+                "fs"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Working with the object"
```

### Comparing `earthkit-data-0.1.2/docs/examples/grib_overview.ipynb` & `earthkit-data-0.1.3/docs/examples/grib_overview.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999675157588759%*

 * *Differences: {"'cells'": "{0: {'source': ['!test -f test6.grib || wget "*

 * *            "https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test6.grib']}, 11: "*

 * *            "{'outputs': {0: {'data': {'text/html': {insert: [(1, '#T_41673 th {\\n'), (4, "*

 * *            "'#T_41673_row0_col0, #T_41673_row0_col1, #T_41673_row0_col2, #T_41673_row0_col3, "*

 * *            '#T_41673_row0_col4, #T_41673_row0_col5, #T_41673_row0_col6, #T_41673_row0_col7, '*

 * *            '#T_41673_row0_col8, #T_41673_row1_col0, #T_41673_row1_c […]*

```diff
@@ -2,15 +2,15 @@
     "cells": [
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
-                "!test -f test6.grib || wget https://get.ecmwf.int/repository/test-data/emohawk/examples/test6.grib"
+                "!test -f test6.grib || wget https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test6.grib"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Using GRIB data overview"
@@ -258,35 +258,35 @@
             "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<style type=\"text/css\">\n",
-                            "#T_cfd90 th {\n",
+                            "#T_41673 th {\n",
                             "  text-align: left;\n",
                             "}\n",
-                            "#T_cfd90_row0_col0, #T_cfd90_row0_col1, #T_cfd90_row0_col2, #T_cfd90_row0_col3, #T_cfd90_row0_col4, #T_cfd90_row0_col5, #T_cfd90_row0_col6, #T_cfd90_row0_col7, #T_cfd90_row0_col8, #T_cfd90_row1_col0, #T_cfd90_row1_col1, #T_cfd90_row1_col2, #T_cfd90_row1_col3, #T_cfd90_row1_col4, #T_cfd90_row1_col5, #T_cfd90_row1_col6, #T_cfd90_row1_col7, #T_cfd90_row1_col8, #T_cfd90_row2_col0, #T_cfd90_row2_col1, #T_cfd90_row2_col2, #T_cfd90_row2_col3, #T_cfd90_row2_col4, #T_cfd90_row2_col5, #T_cfd90_row2_col6, #T_cfd90_row2_col7, #T_cfd90_row2_col8 {\n",
+                            "#T_41673_row0_col0, #T_41673_row0_col1, #T_41673_row0_col2, #T_41673_row0_col3, #T_41673_row0_col4, #T_41673_row0_col5, #T_41673_row0_col6, #T_41673_row0_col7, #T_41673_row0_col8, #T_41673_row1_col0, #T_41673_row1_col1, #T_41673_row1_col2, #T_41673_row1_col3, #T_41673_row1_col4, #T_41673_row1_col5, #T_41673_row1_col6, #T_41673_row1_col7, #T_41673_row1_col8, #T_41673_row2_col0, #T_41673_row2_col1, #T_41673_row2_col2, #T_41673_row2_col3, #T_41673_row2_col4, #T_41673_row2_col5, #T_41673_row2_col6, #T_41673_row2_col7, #T_41673_row2_col8 {\n",
                             "  text-align: left;\n",
                             "}\n",
                             "</style>\n",
-                            "<table id=\"T_cfd90\">\n",
+                            "<table id=\"T_41673\">\n",
                             "  <thead>\n",
                             "    <tr>\n",
                             "      <th class=\"blank\" >&nbsp;</th>\n",
                             "      <th class=\"blank level0\" >&nbsp;</th>\n",
-                            "      <th id=\"T_cfd90_level0_col0\" class=\"col_heading level0 col0\" >level</th>\n",
-                            "      <th id=\"T_cfd90_level0_col1\" class=\"col_heading level0 col1\" >date</th>\n",
-                            "      <th id=\"T_cfd90_level0_col2\" class=\"col_heading level0 col2\" >time</th>\n",
-                            "      <th id=\"T_cfd90_level0_col3\" class=\"col_heading level0 col3\" >step</th>\n",
-                            "      <th id=\"T_cfd90_level0_col4\" class=\"col_heading level0 col4\" >paramId</th>\n",
-                            "      <th id=\"T_cfd90_level0_col5\" class=\"col_heading level0 col5\" >class</th>\n",
-                            "      <th id=\"T_cfd90_level0_col6\" class=\"col_heading level0 col6\" >stream</th>\n",
-                            "      <th id=\"T_cfd90_level0_col7\" class=\"col_heading level0 col7\" >type</th>\n",
-                            "      <th id=\"T_cfd90_level0_col8\" class=\"col_heading level0 col8\" >experimentVersionNumber</th>\n",
+                            "      <th id=\"T_41673_level0_col0\" class=\"col_heading level0 col0\" >level</th>\n",
+                            "      <th id=\"T_41673_level0_col1\" class=\"col_heading level0 col1\" >date</th>\n",
+                            "      <th id=\"T_41673_level0_col2\" class=\"col_heading level0 col2\" >time</th>\n",
+                            "      <th id=\"T_41673_level0_col3\" class=\"col_heading level0 col3\" >step</th>\n",
+                            "      <th id=\"T_41673_level0_col4\" class=\"col_heading level0 col4\" >paramId</th>\n",
+                            "      <th id=\"T_41673_level0_col5\" class=\"col_heading level0 col5\" >class</th>\n",
+                            "      <th id=\"T_41673_level0_col6\" class=\"col_heading level0 col6\" >stream</th>\n",
+                            "      <th id=\"T_41673_level0_col7\" class=\"col_heading level0 col7\" >type</th>\n",
+                            "      <th id=\"T_41673_level0_col8\" class=\"col_heading level0 col8\" >experimentVersionNumber</th>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th class=\"index_name level0\" >shortName</th>\n",
                             "      <th class=\"index_name level1\" >typeOfLevel</th>\n",
                             "      <th class=\"blank col0\" >&nbsp;</th>\n",
                             "      <th class=\"blank col1\" >&nbsp;</th>\n",
                             "      <th class=\"blank col2\" >&nbsp;</th>\n",
@@ -296,57 +296,57 @@
                             "      <th class=\"blank col6\" >&nbsp;</th>\n",
                             "      <th class=\"blank col7\" >&nbsp;</th>\n",
                             "      <th class=\"blank col8\" >&nbsp;</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_cfd90_level0_row0\" class=\"row_heading level0 row0\" >t</th>\n",
-                            "      <th id=\"T_cfd90_level1_row0\" class=\"row_heading level1 row0\" >isobaricInhPa</th>\n",
-                            "      <td id=\"T_cfd90_row0_col0\" class=\"data row0 col0\" >1000,850</td>\n",
-                            "      <td id=\"T_cfd90_row0_col1\" class=\"data row0 col1\" >20180801</td>\n",
-                            "      <td id=\"T_cfd90_row0_col2\" class=\"data row0 col2\" >1200</td>\n",
-                            "      <td id=\"T_cfd90_row0_col3\" class=\"data row0 col3\" >0</td>\n",
-                            "      <td id=\"T_cfd90_row0_col4\" class=\"data row0 col4\" >130</td>\n",
-                            "      <td id=\"T_cfd90_row0_col5\" class=\"data row0 col5\" >od</td>\n",
-                            "      <td id=\"T_cfd90_row0_col6\" class=\"data row0 col6\" >oper</td>\n",
-                            "      <td id=\"T_cfd90_row0_col7\" class=\"data row0 col7\" >an</td>\n",
-                            "      <td id=\"T_cfd90_row0_col8\" class=\"data row0 col8\" >0001</td>\n",
+                            "      <th id=\"T_41673_level0_row0\" class=\"row_heading level0 row0\" >t</th>\n",
+                            "      <th id=\"T_41673_level1_row0\" class=\"row_heading level1 row0\" >isobaricInhPa</th>\n",
+                            "      <td id=\"T_41673_row0_col0\" class=\"data row0 col0\" >1000,850</td>\n",
+                            "      <td id=\"T_41673_row0_col1\" class=\"data row0 col1\" >20180801</td>\n",
+                            "      <td id=\"T_41673_row0_col2\" class=\"data row0 col2\" >1200</td>\n",
+                            "      <td id=\"T_41673_row0_col3\" class=\"data row0 col3\" >0</td>\n",
+                            "      <td id=\"T_41673_row0_col4\" class=\"data row0 col4\" >130</td>\n",
+                            "      <td id=\"T_41673_row0_col5\" class=\"data row0 col5\" >od</td>\n",
+                            "      <td id=\"T_41673_row0_col6\" class=\"data row0 col6\" >oper</td>\n",
+                            "      <td id=\"T_41673_row0_col7\" class=\"data row0 col7\" >an</td>\n",
+                            "      <td id=\"T_41673_row0_col8\" class=\"data row0 col8\" >0001</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_cfd90_level0_row1\" class=\"row_heading level0 row1\" >u</th>\n",
-                            "      <th id=\"T_cfd90_level1_row1\" class=\"row_heading level1 row1\" >isobaricInhPa</th>\n",
-                            "      <td id=\"T_cfd90_row1_col0\" class=\"data row1 col0\" >1000,850</td>\n",
-                            "      <td id=\"T_cfd90_row1_col1\" class=\"data row1 col1\" >20180801</td>\n",
-                            "      <td id=\"T_cfd90_row1_col2\" class=\"data row1 col2\" >1200</td>\n",
-                            "      <td id=\"T_cfd90_row1_col3\" class=\"data row1 col3\" >0</td>\n",
-                            "      <td id=\"T_cfd90_row1_col4\" class=\"data row1 col4\" >131</td>\n",
-                            "      <td id=\"T_cfd90_row1_col5\" class=\"data row1 col5\" >od</td>\n",
-                            "      <td id=\"T_cfd90_row1_col6\" class=\"data row1 col6\" >oper</td>\n",
-                            "      <td id=\"T_cfd90_row1_col7\" class=\"data row1 col7\" >an</td>\n",
-                            "      <td id=\"T_cfd90_row1_col8\" class=\"data row1 col8\" >0001</td>\n",
+                            "      <th id=\"T_41673_level0_row1\" class=\"row_heading level0 row1\" >u</th>\n",
+                            "      <th id=\"T_41673_level1_row1\" class=\"row_heading level1 row1\" >isobaricInhPa</th>\n",
+                            "      <td id=\"T_41673_row1_col0\" class=\"data row1 col0\" >1000,850</td>\n",
+                            "      <td id=\"T_41673_row1_col1\" class=\"data row1 col1\" >20180801</td>\n",
+                            "      <td id=\"T_41673_row1_col2\" class=\"data row1 col2\" >1200</td>\n",
+                            "      <td id=\"T_41673_row1_col3\" class=\"data row1 col3\" >0</td>\n",
+                            "      <td id=\"T_41673_row1_col4\" class=\"data row1 col4\" >131</td>\n",
+                            "      <td id=\"T_41673_row1_col5\" class=\"data row1 col5\" >od</td>\n",
+                            "      <td id=\"T_41673_row1_col6\" class=\"data row1 col6\" >oper</td>\n",
+                            "      <td id=\"T_41673_row1_col7\" class=\"data row1 col7\" >an</td>\n",
+                            "      <td id=\"T_41673_row1_col8\" class=\"data row1 col8\" >0001</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_cfd90_level0_row2\" class=\"row_heading level0 row2\" >v</th>\n",
-                            "      <th id=\"T_cfd90_level1_row2\" class=\"row_heading level1 row2\" >isobaricInhPa</th>\n",
-                            "      <td id=\"T_cfd90_row2_col0\" class=\"data row2 col0\" >1000,850</td>\n",
-                            "      <td id=\"T_cfd90_row2_col1\" class=\"data row2 col1\" >20180801</td>\n",
-                            "      <td id=\"T_cfd90_row2_col2\" class=\"data row2 col2\" >1200</td>\n",
-                            "      <td id=\"T_cfd90_row2_col3\" class=\"data row2 col3\" >0</td>\n",
-                            "      <td id=\"T_cfd90_row2_col4\" class=\"data row2 col4\" >132</td>\n",
-                            "      <td id=\"T_cfd90_row2_col5\" class=\"data row2 col5\" >od</td>\n",
-                            "      <td id=\"T_cfd90_row2_col6\" class=\"data row2 col6\" >oper</td>\n",
-                            "      <td id=\"T_cfd90_row2_col7\" class=\"data row2 col7\" >an</td>\n",
-                            "      <td id=\"T_cfd90_row2_col8\" class=\"data row2 col8\" >0001</td>\n",
+                            "      <th id=\"T_41673_level0_row2\" class=\"row_heading level0 row2\" >v</th>\n",
+                            "      <th id=\"T_41673_level1_row2\" class=\"row_heading level1 row2\" >isobaricInhPa</th>\n",
+                            "      <td id=\"T_41673_row2_col0\" class=\"data row2 col0\" >1000,850</td>\n",
+                            "      <td id=\"T_41673_row2_col1\" class=\"data row2 col1\" >20180801</td>\n",
+                            "      <td id=\"T_41673_row2_col2\" class=\"data row2 col2\" >1200</td>\n",
+                            "      <td id=\"T_41673_row2_col3\" class=\"data row2 col3\" >0</td>\n",
+                            "      <td id=\"T_41673_row2_col4\" class=\"data row2 col4\" >132</td>\n",
+                            "      <td id=\"T_41673_row2_col5\" class=\"data row2 col5\" >od</td>\n",
+                            "      <td id=\"T_41673_row2_col6\" class=\"data row2 col6\" >oper</td>\n",
+                            "      <td id=\"T_41673_row2_col7\" class=\"data row2 col7\" >an</td>\n",
+                            "      <td id=\"T_41673_row2_col8\" class=\"data row2 col8\" >0001</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n"
                         ],
                         "text/plain": [
-                            "<pandas.io.formats.style.Styler at 0x12cf4b220>"
+                            "<pandas.io.formats.style.Styler at 0x130267b50>"
                         ]
                     },
                     "execution_count": 6,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -675,15 +675,15 @@
             "cell_type": "code",
             "execution_count": 16,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "[(1000, 130), (1000, 131)]"
+                            "[[1000, 130], [1000, 131]]"
                         ]
                     },
                     "execution_count": 16,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -722,15 +722,15 @@
             "cell_type": "code",
             "execution_count": 18,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "[(1000, 130), (1000, 131), (1000, 132), (850, 130), (850, 131), (850, 132)]"
+                            "[[1000, 130], [1000, 131], [1000, 132], [850, 130], [850, 131], [850, 132]]"
                         ]
                     },
                     "execution_count": 18,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -749,15 +749,15 @@
             "cell_type": "code",
             "execution_count": 19,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "('ecmf', 98, 'ecmf')"
+                            "['ecmf', 98, 'ecmf']"
                         ]
                     },
                     "execution_count": 19,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -1387,17 +1387,17 @@
                             "Attributes:\n",
                             "    GRIB_edition:            1\n",
                             "    GRIB_centre:             ecmf\n",
                             "    GRIB_centreDescription:  European Centre for Medium-Range Weather Forecasts\n",
                             "    GRIB_subCentre:          0\n",
                             "    Conventions:             CF-1.7\n",
                             "    institution:             European Centre for Medium-Range Weather Forecasts\n",
-                            "    history:                 2023-05-04T16:43 GRIB to CDM+CF via cfgrib-0.9.1...</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.Dataset</div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-db0e39c7-3033-4a18-81e8-84a3cf647fb7' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-db0e39c7-3033-4a18-81e8-84a3cf647fb7' class='xr-section-summary'  title='Expand/collapse section'>Dimensions:</label><div class='xr-section-inline-details'><ul class='xr-dim-list'><li><span class='xr-has-index'>number</span>: 1</li><li><span class='xr-has-index'>time</span>: 1</li><li><span class='xr-has-index'>step</span>: 1</li><li><span class='xr-has-index'>isobaricInhPa</span>: 2</li><li><span class='xr-has-index'>latitude</span>: 7</li><li><span class='xr-has-index'>longitude</span>: 12</li></ul></div><div class='xr-section-details'></div></li><li class='xr-section-item'><input id='section-17a6c222-0bdf-49e9-9a37-605c01177cb1' class='xr-section-summary-in' type='checkbox'  checked><label for='section-17a6c222-0bdf-49e9-9a37-605c01177cb1' class='xr-section-summary' >Coordinates: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>number</span></div><div class='xr-var-dims'>(number)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>0</div><input id='attrs-e5e8bc26-bf87-4870-98f3-324cce0f9bb7' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-e5e8bc26-bf87-4870-98f3-324cce0f9bb7' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-c0b95ce9-7659-44f5-92f8-db8b99bb6f6c' class='xr-var-data-in' type='checkbox'><label for='data-c0b95ce9-7659-44f5-92f8-db8b99bb6f6c' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>ensemble member numerical id</dd><dt><span>units :</span></dt><dd>1</dd><dt><span>standard_name :</span></dt><dd>realization</dd></dl></div><div class='xr-var-data'><pre>array([0])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>time</span></div><div class='xr-var-dims'>(time)</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>2018-08-01T12:00:00</div><input id='attrs-9ec6920a-7583-43e5-ad4b-1c9e44c48f05' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-9ec6920a-7583-43e5-ad4b-1c9e44c48f05' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-0574eef0-17fb-44b0-8ba2-30b1880d17e5' class='xr-var-data-in' type='checkbox'><label for='data-0574eef0-17fb-44b0-8ba2-30b1880d17e5' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>initial time of forecast</dd><dt><span>standard_name :</span></dt><dd>forecast_reference_time</dd></dl></div><div class='xr-var-data'><pre>array([&#x27;2018-08-01T12:00:00.000000000&#x27;], dtype=&#x27;datetime64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>step</span></div><div class='xr-var-dims'>(step)</div><div class='xr-var-dtype'>timedelta64[ns]</div><div class='xr-var-preview xr-preview'>00:00:00</div><input id='attrs-0cfdd62d-907e-4e67-ae58-2258e25bf9da' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-0cfdd62d-907e-4e67-ae58-2258e25bf9da' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-0dd74b66-c447-4bb7-959c-174f2b902c29' class='xr-var-data-in' type='checkbox'><label for='data-0dd74b66-c447-4bb7-959c-174f2b902c29' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>time since forecast_reference_time</dd><dt><span>standard_name :</span></dt><dd>forecast_period</dd></dl></div><div class='xr-var-data'><pre>array([0], dtype=&#x27;timedelta64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>isobaricInhPa</span></div><div class='xr-var-dims'>(isobaricInhPa)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>1000 850</div><input id='attrs-ab07721d-24f3-4fe5-837d-e0721ea5df7c' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-ab07721d-24f3-4fe5-837d-e0721ea5df7c' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-ee0c53ac-74f5-4d93-a30d-a3ac42c373ae' class='xr-var-data-in' type='checkbox'><label for='data-ee0c53ac-74f5-4d93-a30d-a3ac42c373ae' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>pressure</dd><dt><span>units :</span></dt><dd>hPa</dd><dt><span>positive :</span></dt><dd>down</dd><dt><span>stored_direction :</span></dt><dd>decreasing</dd><dt><span>standard_name :</span></dt><dd>air_pressure</dd></dl></div><div class='xr-var-data'><pre>array([1000,  850])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>latitude</span></div><div class='xr-var-dims'>(latitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>90.0 60.0 30.0 ... -60.0 -90.0</div><input id='attrs-980e035e-f00e-43f4-8137-f38a11fd54c0' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-980e035e-f00e-43f4-8137-f38a11fd54c0' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-c32a02da-ed8d-4e78-a546-f15b4d8f4b03' class='xr-var-data-in' type='checkbox'><label for='data-c32a02da-ed8d-4e78-a546-f15b4d8f4b03' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_north</dd><dt><span>standard_name :</span></dt><dd>latitude</dd><dt><span>long_name :</span></dt><dd>latitude</dd><dt><span>stored_direction :</span></dt><dd>decreasing</dd></dl></div><div class='xr-var-data'><pre>array([ 90.,  60.,  30.,   0., -30., -60., -90.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>longitude</span></div><div class='xr-var-dims'>(longitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>0.0 30.0 60.0 ... 270.0 300.0 330.0</div><input id='attrs-0bc9e819-b627-4b6d-b829-087606a5813e' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-0bc9e819-b627-4b6d-b829-087606a5813e' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-ea7797bf-d267-4e4b-ab98-ae55b5479e15' class='xr-var-data-in' type='checkbox'><label for='data-ea7797bf-d267-4e4b-ab98-ae55b5479e15' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_east</dd><dt><span>standard_name :</span></dt><dd>longitude</dd><dt><span>long_name :</span></dt><dd>longitude</dd></dl></div><div class='xr-var-data'><pre>array([  0.,  30.,  60.,  90., 120., 150., 180., 210., 240., 270., 300., 330.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>valid_time</span></div><div class='xr-var-dims'>(time, step)</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-b79add36-e2a0-40ff-9bf1-d8abbfb88711' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-b79add36-e2a0-40ff-9bf1-d8abbfb88711' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-da901062-7f72-49d6-b95a-022578735e7f' class='xr-var-data-in' type='checkbox'><label for='data-da901062-7f72-49d6-b95a-022578735e7f' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>standard_name :</span></dt><dd>time</dd><dt><span>long_name :</span></dt><dd>time</dd></dl></div><div class='xr-var-data'><pre>[1 values with dtype=datetime64[ns]]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-48c313e7-a24a-4465-a5a8-00cce3c434b3' class='xr-section-summary-in' type='checkbox'  checked><label for='section-48c313e7-a24a-4465-a5a8-00cce3c434b3' class='xr-section-summary' >Data variables: <span>(3)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span>t</span></div><div class='xr-var-dims'>(number, time, step, isobaricInhPa, latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-235ab54e-b4b8-45bc-99c7-e3cad3a9d680' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-235ab54e-b4b8-45bc-99c7-e3cad3a9d680' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-8c7d4c21-9061-4241-97c6-514072d4bcf4' class='xr-var-data-in' type='checkbox'><label for='data-8c7d4c21-9061-4241-97c6-514072d4bcf4' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>130</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>84</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>isobaricInhPa</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_Nx :</span></dt><dd>12</dd><dt><span>GRIB_Ny :</span></dt><dd>7</dd><dt><span>GRIB_cfName :</span></dt><dd>air_temperature</dd><dt><span>GRIB_cfVarName :</span></dt><dd>t</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>90.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>-90.0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>0.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>330.0</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>Temperature</dd><dt><span>GRIB_shortName :</span></dt><dd>t</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>K</dd><dt><span>long_name :</span></dt><dd>Temperature</dd><dt><span>units :</span></dt><dd>K</dd><dt><span>standard_name :</span></dt><dd>air_temperature</dd></dl></div><div class='xr-var-data'><pre>[168 values with dtype=float32]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>u</span></div><div class='xr-var-dims'>(number, time, step, isobaricInhPa, latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-1ee7e1bd-50cf-4435-bd35-179936089503' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-1ee7e1bd-50cf-4435-bd35-179936089503' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-5404aa18-18e5-483a-85d1-c08862c97d28' class='xr-var-data-in' type='checkbox'><label for='data-5404aa18-18e5-483a-85d1-c08862c97d28' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>131</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>84</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>isobaricInhPa</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_Nx :</span></dt><dd>12</dd><dt><span>GRIB_Ny :</span></dt><dd>7</dd><dt><span>GRIB_cfName :</span></dt><dd>eastward_wind</dd><dt><span>GRIB_cfVarName :</span></dt><dd>u</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>90.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>-90.0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>0.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>330.0</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>U component of wind</dd><dt><span>GRIB_shortName :</span></dt><dd>u</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>m s**-1</dd><dt><span>long_name :</span></dt><dd>U component of wind</dd><dt><span>units :</span></dt><dd>m s**-1</dd><dt><span>standard_name :</span></dt><dd>eastward_wind</dd></dl></div><div class='xr-var-data'><pre>[168 values with dtype=float32]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>v</span></div><div class='xr-var-dims'>(number, time, step, isobaricInhPa, latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-2f3867f5-2027-4148-8264-841598cfbed4' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-2f3867f5-2027-4148-8264-841598cfbed4' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-eae0a5e1-a556-49e7-9d20-47939c94ff4b' class='xr-var-data-in' type='checkbox'><label for='data-eae0a5e1-a556-49e7-9d20-47939c94ff4b' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>132</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>84</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>isobaricInhPa</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_Nx :</span></dt><dd>12</dd><dt><span>GRIB_Ny :</span></dt><dd>7</dd><dt><span>GRIB_cfName :</span></dt><dd>northward_wind</dd><dt><span>GRIB_cfVarName :</span></dt><dd>v</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>90.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>-90.0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>0.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>330.0</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>V component of wind</dd><dt><span>GRIB_shortName :</span></dt><dd>v</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>m s**-1</dd><dt><span>long_name :</span></dt><dd>V component of wind</dd><dt><span>units :</span></dt><dd>m s**-1</dd><dt><span>standard_name :</span></dt><dd>northward_wind</dd></dl></div><div class='xr-var-data'><pre>[168 values with dtype=float32]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-a10d0606-54a1-4c97-93af-ed914118ddbe' class='xr-section-summary-in' type='checkbox'  ><label for='section-a10d0606-54a1-4c97-93af-ed914118ddbe' class='xr-section-summary' >Indexes: <span>(6)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-index-name'><div>number</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-97013f57-9e3b-4a78-a3b5-599b61df78df' class='xr-index-data-in' type='checkbox'/><label for='index-97013f57-9e3b-4a78-a3b5-599b61df78df' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Int64Index([0], dtype=&#x27;int64&#x27;, name=&#x27;number&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>time</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-282d7849-c5a4-4d6c-abb1-f4e44748c9ea' class='xr-index-data-in' type='checkbox'/><label for='index-282d7849-c5a4-4d6c-abb1-f4e44748c9ea' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(DatetimeIndex([&#x27;2018-08-01 12:00:00&#x27;], dtype=&#x27;datetime64[ns]&#x27;, name=&#x27;time&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>step</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-8bd8f5d1-d944-4f5a-a8f2-421508190093' class='xr-index-data-in' type='checkbox'/><label for='index-8bd8f5d1-d944-4f5a-a8f2-421508190093' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(TimedeltaIndex([&#x27;0 days&#x27;], dtype=&#x27;timedelta64[ns]&#x27;, name=&#x27;step&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>isobaricInhPa</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-747c0b6a-059b-4945-8789-1aa78050112a' class='xr-index-data-in' type='checkbox'/><label for='index-747c0b6a-059b-4945-8789-1aa78050112a' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Int64Index([1000, 850], dtype=&#x27;int64&#x27;, name=&#x27;isobaricInhPa&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>latitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-003455f9-a696-4c08-a808-8a6e8e54ff74' class='xr-index-data-in' type='checkbox'/><label for='index-003455f9-a696-4c08-a808-8a6e8e54ff74' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Float64Index([90.0, 60.0, 30.0, 0.0, -30.0, -60.0, -90.0], dtype=&#x27;float64&#x27;, name=&#x27;latitude&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>longitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-91e9a977-13b1-4de2-8030-47618eebdc76' class='xr-index-data-in' type='checkbox'/><label for='index-91e9a977-13b1-4de2-8030-47618eebdc76' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Float64Index([0.0, 30.0, 60.0, 90.0, 120.0, 150.0, 180.0, 210.0, 240.0, 270.0,\n",
+                            "    history:                 2023-05-17T17:40 GRIB to CDM+CF via cfgrib-0.9.1...</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.Dataset</div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-1841cade-985f-43dd-8a97-34c5f7f9d70c' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-1841cade-985f-43dd-8a97-34c5f7f9d70c' class='xr-section-summary'  title='Expand/collapse section'>Dimensions:</label><div class='xr-section-inline-details'><ul class='xr-dim-list'><li><span class='xr-has-index'>number</span>: 1</li><li><span class='xr-has-index'>time</span>: 1</li><li><span class='xr-has-index'>step</span>: 1</li><li><span class='xr-has-index'>isobaricInhPa</span>: 2</li><li><span class='xr-has-index'>latitude</span>: 7</li><li><span class='xr-has-index'>longitude</span>: 12</li></ul></div><div class='xr-section-details'></div></li><li class='xr-section-item'><input id='section-cfe0690a-a41a-4517-a72c-864269dbb782' class='xr-section-summary-in' type='checkbox'  checked><label for='section-cfe0690a-a41a-4517-a72c-864269dbb782' class='xr-section-summary' >Coordinates: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>number</span></div><div class='xr-var-dims'>(number)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>0</div><input id='attrs-ba2b4ce4-83c6-49ac-a83b-165d26807394' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-ba2b4ce4-83c6-49ac-a83b-165d26807394' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-399b1d7a-e45a-428f-a7e5-bdaabb4379ef' class='xr-var-data-in' type='checkbox'><label for='data-399b1d7a-e45a-428f-a7e5-bdaabb4379ef' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>ensemble member numerical id</dd><dt><span>units :</span></dt><dd>1</dd><dt><span>standard_name :</span></dt><dd>realization</dd></dl></div><div class='xr-var-data'><pre>array([0])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>time</span></div><div class='xr-var-dims'>(time)</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>2018-08-01T12:00:00</div><input id='attrs-afd247a7-4b1f-41dc-a882-f589aef2012a' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-afd247a7-4b1f-41dc-a882-f589aef2012a' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-1fdf56ad-c6ad-4b12-a201-f50338684570' class='xr-var-data-in' type='checkbox'><label for='data-1fdf56ad-c6ad-4b12-a201-f50338684570' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>initial time of forecast</dd><dt><span>standard_name :</span></dt><dd>forecast_reference_time</dd></dl></div><div class='xr-var-data'><pre>array([&#x27;2018-08-01T12:00:00.000000000&#x27;], dtype=&#x27;datetime64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>step</span></div><div class='xr-var-dims'>(step)</div><div class='xr-var-dtype'>timedelta64[ns]</div><div class='xr-var-preview xr-preview'>00:00:00</div><input id='attrs-018b7074-b540-4741-83ae-5d691efb8e02' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-018b7074-b540-4741-83ae-5d691efb8e02' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-3b483e70-a6c5-4445-a3a6-a646fb299d13' class='xr-var-data-in' type='checkbox'><label for='data-3b483e70-a6c5-4445-a3a6-a646fb299d13' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>time since forecast_reference_time</dd><dt><span>standard_name :</span></dt><dd>forecast_period</dd></dl></div><div class='xr-var-data'><pre>array([0], dtype=&#x27;timedelta64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>isobaricInhPa</span></div><div class='xr-var-dims'>(isobaricInhPa)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>1000 850</div><input id='attrs-1a866171-d371-47b6-8df7-ccdeaeedf474' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-1a866171-d371-47b6-8df7-ccdeaeedf474' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-f5d0a1cf-9fce-4ab2-bb81-f331dbf7f36f' class='xr-var-data-in' type='checkbox'><label for='data-f5d0a1cf-9fce-4ab2-bb81-f331dbf7f36f' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>pressure</dd><dt><span>units :</span></dt><dd>hPa</dd><dt><span>positive :</span></dt><dd>down</dd><dt><span>stored_direction :</span></dt><dd>decreasing</dd><dt><span>standard_name :</span></dt><dd>air_pressure</dd></dl></div><div class='xr-var-data'><pre>array([1000,  850])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>latitude</span></div><div class='xr-var-dims'>(latitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>90.0 60.0 30.0 ... -60.0 -90.0</div><input id='attrs-54ae76ec-da6d-410d-acff-e5f9a14365f0' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-54ae76ec-da6d-410d-acff-e5f9a14365f0' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-050c3b54-85df-4872-b060-c7e08224b0b4' class='xr-var-data-in' type='checkbox'><label for='data-050c3b54-85df-4872-b060-c7e08224b0b4' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_north</dd><dt><span>standard_name :</span></dt><dd>latitude</dd><dt><span>long_name :</span></dt><dd>latitude</dd><dt><span>stored_direction :</span></dt><dd>decreasing</dd></dl></div><div class='xr-var-data'><pre>array([ 90.,  60.,  30.,   0., -30., -60., -90.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>longitude</span></div><div class='xr-var-dims'>(longitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>0.0 30.0 60.0 ... 270.0 300.0 330.0</div><input id='attrs-28f28bd1-cb3b-4631-acc7-10151f301e31' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-28f28bd1-cb3b-4631-acc7-10151f301e31' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-d26aa714-604e-4228-8048-9739843a04c0' class='xr-var-data-in' type='checkbox'><label for='data-d26aa714-604e-4228-8048-9739843a04c0' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_east</dd><dt><span>standard_name :</span></dt><dd>longitude</dd><dt><span>long_name :</span></dt><dd>longitude</dd></dl></div><div class='xr-var-data'><pre>array([  0.,  30.,  60.,  90., 120., 150., 180., 210., 240., 270., 300., 330.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>valid_time</span></div><div class='xr-var-dims'>(time, step)</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-cd26a69c-bfa8-426c-b4dc-e9f256df319a' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-cd26a69c-bfa8-426c-b4dc-e9f256df319a' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-ebc34426-222a-41f1-b713-e2917c492493' class='xr-var-data-in' type='checkbox'><label for='data-ebc34426-222a-41f1-b713-e2917c492493' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>standard_name :</span></dt><dd>time</dd><dt><span>long_name :</span></dt><dd>time</dd></dl></div><div class='xr-var-data'><pre>[1 values with dtype=datetime64[ns]]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-d9bb2937-7fdf-4343-94ad-ab5c88c3f407' class='xr-section-summary-in' type='checkbox'  checked><label for='section-d9bb2937-7fdf-4343-94ad-ab5c88c3f407' class='xr-section-summary' >Data variables: <span>(3)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span>t</span></div><div class='xr-var-dims'>(number, time, step, isobaricInhPa, latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-d074b3f7-d50c-4582-a481-f61e454eae9b' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-d074b3f7-d50c-4582-a481-f61e454eae9b' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-e2925141-2cff-4610-8919-64c2e0a5444e' class='xr-var-data-in' type='checkbox'><label for='data-e2925141-2cff-4610-8919-64c2e0a5444e' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>130</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>84</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>isobaricInhPa</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_Nx :</span></dt><dd>12</dd><dt><span>GRIB_Ny :</span></dt><dd>7</dd><dt><span>GRIB_cfName :</span></dt><dd>air_temperature</dd><dt><span>GRIB_cfVarName :</span></dt><dd>t</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>90.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>-90.0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>0.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>330.0</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>Temperature</dd><dt><span>GRIB_shortName :</span></dt><dd>t</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>K</dd><dt><span>long_name :</span></dt><dd>Temperature</dd><dt><span>units :</span></dt><dd>K</dd><dt><span>standard_name :</span></dt><dd>air_temperature</dd></dl></div><div class='xr-var-data'><pre>[168 values with dtype=float32]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>u</span></div><div class='xr-var-dims'>(number, time, step, isobaricInhPa, latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-17b65f4b-4e2d-4e00-81f6-e1ccd38b3b69' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-17b65f4b-4e2d-4e00-81f6-e1ccd38b3b69' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-53ac77b9-e5af-4940-904e-8a52848c41e0' class='xr-var-data-in' type='checkbox'><label for='data-53ac77b9-e5af-4940-904e-8a52848c41e0' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>131</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>84</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>isobaricInhPa</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_Nx :</span></dt><dd>12</dd><dt><span>GRIB_Ny :</span></dt><dd>7</dd><dt><span>GRIB_cfName :</span></dt><dd>eastward_wind</dd><dt><span>GRIB_cfVarName :</span></dt><dd>u</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>90.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>-90.0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>0.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>330.0</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>U component of wind</dd><dt><span>GRIB_shortName :</span></dt><dd>u</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>m s**-1</dd><dt><span>long_name :</span></dt><dd>U component of wind</dd><dt><span>units :</span></dt><dd>m s**-1</dd><dt><span>standard_name :</span></dt><dd>eastward_wind</dd></dl></div><div class='xr-var-data'><pre>[168 values with dtype=float32]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>v</span></div><div class='xr-var-dims'>(number, time, step, isobaricInhPa, latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-6742e27d-da1e-4940-97b3-24a079a190d5' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-6742e27d-da1e-4940-97b3-24a079a190d5' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-ee3b3cb2-a6cf-4304-9d63-e257cfa9c57a' class='xr-var-data-in' type='checkbox'><label for='data-ee3b3cb2-a6cf-4304-9d63-e257cfa9c57a' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>132</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>84</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>isobaricInhPa</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_Nx :</span></dt><dd>12</dd><dt><span>GRIB_Ny :</span></dt><dd>7</dd><dt><span>GRIB_cfName :</span></dt><dd>northward_wind</dd><dt><span>GRIB_cfVarName :</span></dt><dd>v</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>90.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>-90.0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>0.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>330.0</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>V component of wind</dd><dt><span>GRIB_shortName :</span></dt><dd>v</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>m s**-1</dd><dt><span>long_name :</span></dt><dd>V component of wind</dd><dt><span>units :</span></dt><dd>m s**-1</dd><dt><span>standard_name :</span></dt><dd>northward_wind</dd></dl></div><div class='xr-var-data'><pre>[168 values with dtype=float32]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-5f527475-7d93-4024-b24d-8d2079da693a' class='xr-section-summary-in' type='checkbox'  ><label for='section-5f527475-7d93-4024-b24d-8d2079da693a' class='xr-section-summary' >Indexes: <span>(6)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-index-name'><div>number</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-b4ce9783-836b-4a43-a112-bd3eb1d7da22' class='xr-index-data-in' type='checkbox'/><label for='index-b4ce9783-836b-4a43-a112-bd3eb1d7da22' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Int64Index([0], dtype=&#x27;int64&#x27;, name=&#x27;number&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>time</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-9b0c78d8-18f6-426f-856c-179e063f2eda' class='xr-index-data-in' type='checkbox'/><label for='index-9b0c78d8-18f6-426f-856c-179e063f2eda' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(DatetimeIndex([&#x27;2018-08-01 12:00:00&#x27;], dtype=&#x27;datetime64[ns]&#x27;, name=&#x27;time&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>step</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-72655b31-4cb6-4864-a315-58a3fdd41b46' class='xr-index-data-in' type='checkbox'/><label for='index-72655b31-4cb6-4864-a315-58a3fdd41b46' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(TimedeltaIndex([&#x27;0 days&#x27;], dtype=&#x27;timedelta64[ns]&#x27;, name=&#x27;step&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>isobaricInhPa</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-e76203c4-6ed3-4aaa-874c-79b878955b73' class='xr-index-data-in' type='checkbox'/><label for='index-e76203c4-6ed3-4aaa-874c-79b878955b73' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Int64Index([1000, 850], dtype=&#x27;int64&#x27;, name=&#x27;isobaricInhPa&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>latitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-9e80af1f-890c-4106-91bc-3bd5b8fa27b6' class='xr-index-data-in' type='checkbox'/><label for='index-9e80af1f-890c-4106-91bc-3bd5b8fa27b6' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Float64Index([90.0, 60.0, 30.0, 0.0, -30.0, -60.0, -90.0], dtype=&#x27;float64&#x27;, name=&#x27;latitude&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>longitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-fca27e0e-aeca-4529-a62a-38214239ca2f' class='xr-index-data-in' type='checkbox'/><label for='index-fca27e0e-aeca-4529-a62a-38214239ca2f' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Float64Index([0.0, 30.0, 60.0, 90.0, 120.0, 150.0, 180.0, 210.0, 240.0, 270.0,\n",
                             "              300.0, 330.0],\n",
-                            "             dtype=&#x27;float64&#x27;, name=&#x27;longitude&#x27;))</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-4120d9a5-4080-4ca8-b5ab-b0835e3f38eb' class='xr-section-summary-in' type='checkbox'  checked><label for='section-4120d9a5-4080-4ca8-b5ab-b0835e3f38eb' class='xr-section-summary' >Attributes: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>GRIB_edition :</span></dt><dd>1</dd><dt><span>GRIB_centre :</span></dt><dd>ecmf</dd><dt><span>GRIB_centreDescription :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>GRIB_subCentre :</span></dt><dd>0</dd><dt><span>Conventions :</span></dt><dd>CF-1.7</dd><dt><span>institution :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>history :</span></dt><dd>2023-05-04T16:43 GRIB to CDM+CF via cfgrib-0.9.10.3/ecCodes-2.27.1 with {&quot;source&quot;: &quot;N/A&quot;, &quot;filter_by_keys&quot;: {}, &quot;encode_cf&quot;: [&quot;parameter&quot;, &quot;time&quot;, &quot;geography&quot;, &quot;vertical&quot;]}</dd></dl></div></li></ul></div></div>"
+                            "             dtype=&#x27;float64&#x27;, name=&#x27;longitude&#x27;))</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-927c801a-a45e-42c2-bde0-154985e63192' class='xr-section-summary-in' type='checkbox'  checked><label for='section-927c801a-a45e-42c2-bde0-154985e63192' class='xr-section-summary' >Attributes: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>GRIB_edition :</span></dt><dd>1</dd><dt><span>GRIB_centre :</span></dt><dd>ecmf</dd><dt><span>GRIB_centreDescription :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>GRIB_subCentre :</span></dt><dd>0</dd><dt><span>Conventions :</span></dt><dd>CF-1.7</dd><dt><span>institution :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>history :</span></dt><dd>2023-05-17T17:40 GRIB to CDM+CF via cfgrib-0.9.10.3/ecCodes-2.27.1 with {&quot;source&quot;: &quot;N/A&quot;, &quot;filter_by_keys&quot;: {}, &quot;encode_cf&quot;: [&quot;parameter&quot;, &quot;time&quot;, &quot;geography&quot;, &quot;vertical&quot;]}</dd></dl></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<xarray.Dataset>\n",
                             "Dimensions:        (number: 1, time: 1, step: 1, isobaricInhPa: 2, latitude: 7,\n",
                             "                    longitude: 12)\n",
                             "Coordinates:\n",
                             "  * number         (number) int64 0\n",
@@ -1414,15 +1414,15 @@
                             "Attributes:\n",
                             "    GRIB_edition:            1\n",
                             "    GRIB_centre:             ecmf\n",
                             "    GRIB_centreDescription:  European Centre for Medium-Range Weather Forecasts\n",
                             "    GRIB_subCentre:          0\n",
                             "    Conventions:             CF-1.7\n",
                             "    institution:             European Centre for Medium-Range Weather Forecasts\n",
-                            "    history:                 2023-05-04T16:43 GRIB to CDM+CF via cfgrib-0.9.1..."
+                            "    history:                 2023-05-17T17:40 GRIB to CDM+CF via cfgrib-0.9.1..."
                         ]
                     },
                     "execution_count": 23,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -1826,17 +1826,17 @@
                             "Attributes:\n",
                             "    GRIB_edition:            1\n",
                             "    GRIB_centre:             ecmf\n",
                             "    GRIB_centreDescription:  European Centre for Medium-Range Weather Forecasts\n",
                             "    GRIB_subCentre:          0\n",
                             "    Conventions:             CF-1.7\n",
                             "    institution:             European Centre for Medium-Range Weather Forecasts\n",
-                            "    history:                 2023-05-04T16:43 GRIB to CDM+CF via cfgrib-0.9.1...</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.Dataset</div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-01bdfa88-a320-4eb9-87ff-92f9ca26cc9f' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-01bdfa88-a320-4eb9-87ff-92f9ca26cc9f' class='xr-section-summary'  title='Expand/collapse section'>Dimensions:</label><div class='xr-section-inline-details'><ul class='xr-dim-list'><li><span class='xr-has-index'>time</span>: 1</li><li><span class='xr-has-index'>step</span>: 1</li><li><span class='xr-has-index'>isobaricInhPa</span>: 2</li><li><span class='xr-has-index'>latitude</span>: 7</li><li><span class='xr-has-index'>longitude</span>: 12</li></ul></div><div class='xr-section-details'></div></li><li class='xr-section-item'><input id='section-c55677d6-e1b1-4a75-b66f-a5bf09978944' class='xr-section-summary-in' type='checkbox'  checked><label for='section-c55677d6-e1b1-4a75-b66f-a5bf09978944' class='xr-section-summary' >Coordinates: <span>(6)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>time</span></div><div class='xr-var-dims'>(time)</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>2018-08-01T12:00:00</div><input id='attrs-0936b6a3-0026-4755-83f7-c22657d1d3f1' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-0936b6a3-0026-4755-83f7-c22657d1d3f1' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-b2d736eb-bdc3-44aa-9602-72a08cf7bb03' class='xr-var-data-in' type='checkbox'><label for='data-b2d736eb-bdc3-44aa-9602-72a08cf7bb03' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>initial time of forecast</dd><dt><span>standard_name :</span></dt><dd>forecast_reference_time</dd></dl></div><div class='xr-var-data'><pre>array([&#x27;2018-08-01T12:00:00.000000000&#x27;], dtype=&#x27;datetime64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>step</span></div><div class='xr-var-dims'>(step)</div><div class='xr-var-dtype'>timedelta64[ns]</div><div class='xr-var-preview xr-preview'>00:00:00</div><input id='attrs-0e8f705c-fb3e-4976-95a5-db37685f4384' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-0e8f705c-fb3e-4976-95a5-db37685f4384' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-e913d1ae-f4fd-4a36-bd8c-68f36e742abe' class='xr-var-data-in' type='checkbox'><label for='data-e913d1ae-f4fd-4a36-bd8c-68f36e742abe' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>time since forecast_reference_time</dd><dt><span>standard_name :</span></dt><dd>forecast_period</dd></dl></div><div class='xr-var-data'><pre>array([0], dtype=&#x27;timedelta64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>isobaricInhPa</span></div><div class='xr-var-dims'>(isobaricInhPa)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>1000 850</div><input id='attrs-0e43754b-54a9-4d7c-834a-37bb40160a60' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-0e43754b-54a9-4d7c-834a-37bb40160a60' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-b1223a41-0cc1-4abb-8444-a9e024db1732' class='xr-var-data-in' type='checkbox'><label for='data-b1223a41-0cc1-4abb-8444-a9e024db1732' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>pressure</dd><dt><span>units :</span></dt><dd>hPa</dd><dt><span>positive :</span></dt><dd>down</dd><dt><span>stored_direction :</span></dt><dd>decreasing</dd><dt><span>standard_name :</span></dt><dd>air_pressure</dd></dl></div><div class='xr-var-data'><pre>array([1000,  850])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>latitude</span></div><div class='xr-var-dims'>(latitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>90.0 60.0 30.0 ... -60.0 -90.0</div><input id='attrs-d56113cd-12c4-412e-852c-f0af3f949732' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-d56113cd-12c4-412e-852c-f0af3f949732' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-1a55ff7a-c6a0-4a81-9613-a4acfc299586' class='xr-var-data-in' type='checkbox'><label for='data-1a55ff7a-c6a0-4a81-9613-a4acfc299586' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_north</dd><dt><span>standard_name :</span></dt><dd>latitude</dd><dt><span>long_name :</span></dt><dd>latitude</dd><dt><span>stored_direction :</span></dt><dd>decreasing</dd></dl></div><div class='xr-var-data'><pre>array([ 90.,  60.,  30.,   0., -30., -60., -90.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>longitude</span></div><div class='xr-var-dims'>(longitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>0.0 30.0 60.0 ... 270.0 300.0 330.0</div><input id='attrs-7f5a7bac-6972-49e4-9aa7-989e8529e899' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-7f5a7bac-6972-49e4-9aa7-989e8529e899' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-84f0b041-be5d-4580-8129-64f2dff39ef8' class='xr-var-data-in' type='checkbox'><label for='data-84f0b041-be5d-4580-8129-64f2dff39ef8' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_east</dd><dt><span>standard_name :</span></dt><dd>longitude</dd><dt><span>long_name :</span></dt><dd>longitude</dd></dl></div><div class='xr-var-data'><pre>array([  0.,  30.,  60.,  90., 120., 150., 180., 210., 240., 270., 300., 330.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>valid_time</span></div><div class='xr-var-dims'>(time, step)</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-28f336d8-f2a9-4d1b-b3b4-d9651a62ef8c' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-28f336d8-f2a9-4d1b-b3b4-d9651a62ef8c' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-11112970-9d92-4a0a-8610-d6e0df39b351' class='xr-var-data-in' type='checkbox'><label for='data-11112970-9d92-4a0a-8610-d6e0df39b351' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>standard_name :</span></dt><dd>time</dd><dt><span>long_name :</span></dt><dd>time</dd></dl></div><div class='xr-var-data'><pre>[1 values with dtype=datetime64[ns]]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-3b511f7a-b7ca-4be7-864f-86a2ec84c129' class='xr-section-summary-in' type='checkbox'  checked><label for='section-3b511f7a-b7ca-4be7-864f-86a2ec84c129' class='xr-section-summary' >Data variables: <span>(3)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span>t</span></div><div class='xr-var-dims'>(time, step, isobaricInhPa, latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-e59deb93-7f80-4370-997f-d2c929dd4d07' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-e59deb93-7f80-4370-997f-d2c929dd4d07' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-d07b2021-a342-4a53-84dd-124e9f8ccbfe' class='xr-var-data-in' type='checkbox'><label for='data-d07b2021-a342-4a53-84dd-124e9f8ccbfe' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>130</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>84</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>isobaricInhPa</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_Nx :</span></dt><dd>12</dd><dt><span>GRIB_Ny :</span></dt><dd>7</dd><dt><span>GRIB_cfName :</span></dt><dd>air_temperature</dd><dt><span>GRIB_cfVarName :</span></dt><dd>t</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>90.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>-90.0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>0.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>330.0</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>Temperature</dd><dt><span>GRIB_shortName :</span></dt><dd>t</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>K</dd><dt><span>long_name :</span></dt><dd>Temperature</dd><dt><span>units :</span></dt><dd>K</dd><dt><span>standard_name :</span></dt><dd>air_temperature</dd></dl></div><div class='xr-var-data'><pre>[168 values with dtype=float32]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>u</span></div><div class='xr-var-dims'>(time, step, isobaricInhPa, latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-acab4bb0-f031-4972-a89e-d572861d9e44' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-acab4bb0-f031-4972-a89e-d572861d9e44' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-d243c247-5cbd-4b84-8f29-ffb5855a1a0b' class='xr-var-data-in' type='checkbox'><label for='data-d243c247-5cbd-4b84-8f29-ffb5855a1a0b' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>131</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>84</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>isobaricInhPa</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_Nx :</span></dt><dd>12</dd><dt><span>GRIB_Ny :</span></dt><dd>7</dd><dt><span>GRIB_cfName :</span></dt><dd>eastward_wind</dd><dt><span>GRIB_cfVarName :</span></dt><dd>u</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>90.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>-90.0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>0.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>330.0</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>U component of wind</dd><dt><span>GRIB_shortName :</span></dt><dd>u</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>m s**-1</dd><dt><span>long_name :</span></dt><dd>U component of wind</dd><dt><span>units :</span></dt><dd>m s**-1</dd><dt><span>standard_name :</span></dt><dd>eastward_wind</dd></dl></div><div class='xr-var-data'><pre>[168 values with dtype=float32]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>v</span></div><div class='xr-var-dims'>(time, step, isobaricInhPa, latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-5372495d-a466-428d-9f52-1ef8962f3c07' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-5372495d-a466-428d-9f52-1ef8962f3c07' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-bf420c93-6bc8-44c4-bd66-fd370e989d7d' class='xr-var-data-in' type='checkbox'><label for='data-bf420c93-6bc8-44c4-bd66-fd370e989d7d' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>132</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>84</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>isobaricInhPa</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_Nx :</span></dt><dd>12</dd><dt><span>GRIB_Ny :</span></dt><dd>7</dd><dt><span>GRIB_cfName :</span></dt><dd>northward_wind</dd><dt><span>GRIB_cfVarName :</span></dt><dd>v</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>90.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>-90.0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>0.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>330.0</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>V component of wind</dd><dt><span>GRIB_shortName :</span></dt><dd>v</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>m s**-1</dd><dt><span>long_name :</span></dt><dd>V component of wind</dd><dt><span>units :</span></dt><dd>m s**-1</dd><dt><span>standard_name :</span></dt><dd>northward_wind</dd></dl></div><div class='xr-var-data'><pre>[168 values with dtype=float32]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-2bb630e1-fa26-4967-b59c-f354837a9dcb' class='xr-section-summary-in' type='checkbox'  ><label for='section-2bb630e1-fa26-4967-b59c-f354837a9dcb' class='xr-section-summary' >Indexes: <span>(5)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-index-name'><div>time</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-66fc280d-528b-49e0-bffe-ecf179b1ab77' class='xr-index-data-in' type='checkbox'/><label for='index-66fc280d-528b-49e0-bffe-ecf179b1ab77' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(DatetimeIndex([&#x27;2018-08-01 12:00:00&#x27;], dtype=&#x27;datetime64[ns]&#x27;, name=&#x27;time&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>step</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-fdbbb6f3-73b8-4562-a322-f8edec410372' class='xr-index-data-in' type='checkbox'/><label for='index-fdbbb6f3-73b8-4562-a322-f8edec410372' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(TimedeltaIndex([&#x27;0 days&#x27;], dtype=&#x27;timedelta64[ns]&#x27;, name=&#x27;step&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>isobaricInhPa</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-a7784232-1a71-48d0-a148-b26a01343085' class='xr-index-data-in' type='checkbox'/><label for='index-a7784232-1a71-48d0-a148-b26a01343085' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Int64Index([1000, 850], dtype=&#x27;int64&#x27;, name=&#x27;isobaricInhPa&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>latitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-04c848f0-27a2-4a0d-9c0e-349cc5dc8b2a' class='xr-index-data-in' type='checkbox'/><label for='index-04c848f0-27a2-4a0d-9c0e-349cc5dc8b2a' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Float64Index([90.0, 60.0, 30.0, 0.0, -30.0, -60.0, -90.0], dtype=&#x27;float64&#x27;, name=&#x27;latitude&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>longitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-9c5ca668-c309-410f-94f3-5695f06974e3' class='xr-index-data-in' type='checkbox'/><label for='index-9c5ca668-c309-410f-94f3-5695f06974e3' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Float64Index([0.0, 30.0, 60.0, 90.0, 120.0, 150.0, 180.0, 210.0, 240.0, 270.0,\n",
+                            "    history:                 2023-05-17T17:40 GRIB to CDM+CF via cfgrib-0.9.1...</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.Dataset</div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-342df797-d354-4636-bbe4-b6970390c297' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-342df797-d354-4636-bbe4-b6970390c297' class='xr-section-summary'  title='Expand/collapse section'>Dimensions:</label><div class='xr-section-inline-details'><ul class='xr-dim-list'><li><span class='xr-has-index'>time</span>: 1</li><li><span class='xr-has-index'>step</span>: 1</li><li><span class='xr-has-index'>isobaricInhPa</span>: 2</li><li><span class='xr-has-index'>latitude</span>: 7</li><li><span class='xr-has-index'>longitude</span>: 12</li></ul></div><div class='xr-section-details'></div></li><li class='xr-section-item'><input id='section-53776147-d34c-4c72-9035-4d3afecf75a1' class='xr-section-summary-in' type='checkbox'  checked><label for='section-53776147-d34c-4c72-9035-4d3afecf75a1' class='xr-section-summary' >Coordinates: <span>(6)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>time</span></div><div class='xr-var-dims'>(time)</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>2018-08-01T12:00:00</div><input id='attrs-99135cb9-9abb-4f75-808e-a67469aaf52c' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-99135cb9-9abb-4f75-808e-a67469aaf52c' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-5471c338-dca7-4591-8562-00ff93ecd8e1' class='xr-var-data-in' type='checkbox'><label for='data-5471c338-dca7-4591-8562-00ff93ecd8e1' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>initial time of forecast</dd><dt><span>standard_name :</span></dt><dd>forecast_reference_time</dd></dl></div><div class='xr-var-data'><pre>array([&#x27;2018-08-01T12:00:00.000000000&#x27;], dtype=&#x27;datetime64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>step</span></div><div class='xr-var-dims'>(step)</div><div class='xr-var-dtype'>timedelta64[ns]</div><div class='xr-var-preview xr-preview'>00:00:00</div><input id='attrs-b658ad58-1a96-48b1-b6d8-6ea7bf206063' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-b658ad58-1a96-48b1-b6d8-6ea7bf206063' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-0d277e90-cc0a-42ce-930b-da3dfdd1df25' class='xr-var-data-in' type='checkbox'><label for='data-0d277e90-cc0a-42ce-930b-da3dfdd1df25' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>time since forecast_reference_time</dd><dt><span>standard_name :</span></dt><dd>forecast_period</dd></dl></div><div class='xr-var-data'><pre>array([0], dtype=&#x27;timedelta64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>isobaricInhPa</span></div><div class='xr-var-dims'>(isobaricInhPa)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>1000 850</div><input id='attrs-5f846d80-0858-45a9-8581-9e4f6da5cab7' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-5f846d80-0858-45a9-8581-9e4f6da5cab7' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-00396e82-f5de-4366-83d2-c7fad5844fa1' class='xr-var-data-in' type='checkbox'><label for='data-00396e82-f5de-4366-83d2-c7fad5844fa1' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>pressure</dd><dt><span>units :</span></dt><dd>hPa</dd><dt><span>positive :</span></dt><dd>down</dd><dt><span>stored_direction :</span></dt><dd>decreasing</dd><dt><span>standard_name :</span></dt><dd>air_pressure</dd></dl></div><div class='xr-var-data'><pre>array([1000,  850])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>latitude</span></div><div class='xr-var-dims'>(latitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>90.0 60.0 30.0 ... -60.0 -90.0</div><input id='attrs-74096228-e9e1-49b2-b87a-262484acac9b' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-74096228-e9e1-49b2-b87a-262484acac9b' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-bdc03411-ab02-4bf1-9040-cf9cfa1c4134' class='xr-var-data-in' type='checkbox'><label for='data-bdc03411-ab02-4bf1-9040-cf9cfa1c4134' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_north</dd><dt><span>standard_name :</span></dt><dd>latitude</dd><dt><span>long_name :</span></dt><dd>latitude</dd><dt><span>stored_direction :</span></dt><dd>decreasing</dd></dl></div><div class='xr-var-data'><pre>array([ 90.,  60.,  30.,   0., -30., -60., -90.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>longitude</span></div><div class='xr-var-dims'>(longitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>0.0 30.0 60.0 ... 270.0 300.0 330.0</div><input id='attrs-27ff62a2-0295-4bf7-b7cb-e1f3957adf49' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-27ff62a2-0295-4bf7-b7cb-e1f3957adf49' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-4d29d1c4-8fca-4788-9e2d-3a1fe0bfa67e' class='xr-var-data-in' type='checkbox'><label for='data-4d29d1c4-8fca-4788-9e2d-3a1fe0bfa67e' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_east</dd><dt><span>standard_name :</span></dt><dd>longitude</dd><dt><span>long_name :</span></dt><dd>longitude</dd></dl></div><div class='xr-var-data'><pre>array([  0.,  30.,  60.,  90., 120., 150., 180., 210., 240., 270., 300., 330.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>valid_time</span></div><div class='xr-var-dims'>(time, step)</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-a74262ed-3a3a-4e73-88ba-1feba25ac1e5' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-a74262ed-3a3a-4e73-88ba-1feba25ac1e5' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-674e840c-4345-4f99-9388-77018d20f746' class='xr-var-data-in' type='checkbox'><label for='data-674e840c-4345-4f99-9388-77018d20f746' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>standard_name :</span></dt><dd>time</dd><dt><span>long_name :</span></dt><dd>time</dd></dl></div><div class='xr-var-data'><pre>[1 values with dtype=datetime64[ns]]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-28f2dc4a-e075-4692-a759-e85dab58084a' class='xr-section-summary-in' type='checkbox'  checked><label for='section-28f2dc4a-e075-4692-a759-e85dab58084a' class='xr-section-summary' >Data variables: <span>(3)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span>t</span></div><div class='xr-var-dims'>(time, step, isobaricInhPa, latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-5f814b44-c347-4dd0-981f-252c11b03adf' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-5f814b44-c347-4dd0-981f-252c11b03adf' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-dce1ac10-96d8-4706-a3ec-c8e8c1ecd55e' class='xr-var-data-in' type='checkbox'><label for='data-dce1ac10-96d8-4706-a3ec-c8e8c1ecd55e' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>130</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>84</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>isobaricInhPa</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_Nx :</span></dt><dd>12</dd><dt><span>GRIB_Ny :</span></dt><dd>7</dd><dt><span>GRIB_cfName :</span></dt><dd>air_temperature</dd><dt><span>GRIB_cfVarName :</span></dt><dd>t</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>90.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>-90.0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>0.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>330.0</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>Temperature</dd><dt><span>GRIB_shortName :</span></dt><dd>t</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>K</dd><dt><span>long_name :</span></dt><dd>Temperature</dd><dt><span>units :</span></dt><dd>K</dd><dt><span>standard_name :</span></dt><dd>air_temperature</dd></dl></div><div class='xr-var-data'><pre>[168 values with dtype=float32]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>u</span></div><div class='xr-var-dims'>(time, step, isobaricInhPa, latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-5a628772-171c-429e-ba44-b34b43eaad2e' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-5a628772-171c-429e-ba44-b34b43eaad2e' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-7c018c72-4456-4e0c-a5b8-2ae67f445768' class='xr-var-data-in' type='checkbox'><label for='data-7c018c72-4456-4e0c-a5b8-2ae67f445768' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>131</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>84</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>isobaricInhPa</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_Nx :</span></dt><dd>12</dd><dt><span>GRIB_Ny :</span></dt><dd>7</dd><dt><span>GRIB_cfName :</span></dt><dd>eastward_wind</dd><dt><span>GRIB_cfVarName :</span></dt><dd>u</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>90.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>-90.0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>0.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>330.0</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>U component of wind</dd><dt><span>GRIB_shortName :</span></dt><dd>u</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>m s**-1</dd><dt><span>long_name :</span></dt><dd>U component of wind</dd><dt><span>units :</span></dt><dd>m s**-1</dd><dt><span>standard_name :</span></dt><dd>eastward_wind</dd></dl></div><div class='xr-var-data'><pre>[168 values with dtype=float32]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>v</span></div><div class='xr-var-dims'>(time, step, isobaricInhPa, latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-64df24d5-74a4-405d-9552-b8a412f40ab0' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-64df24d5-74a4-405d-9552-b8a412f40ab0' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-c2f1f3d5-458f-4fb1-9383-9a6f27aca991' class='xr-var-data-in' type='checkbox'><label for='data-c2f1f3d5-458f-4fb1-9383-9a6f27aca991' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>132</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>84</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>isobaricInhPa</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_Nx :</span></dt><dd>12</dd><dt><span>GRIB_Ny :</span></dt><dd>7</dd><dt><span>GRIB_cfName :</span></dt><dd>northward_wind</dd><dt><span>GRIB_cfVarName :</span></dt><dd>v</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>90.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>-90.0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>0.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>330.0</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>V component of wind</dd><dt><span>GRIB_shortName :</span></dt><dd>v</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>m s**-1</dd><dt><span>long_name :</span></dt><dd>V component of wind</dd><dt><span>units :</span></dt><dd>m s**-1</dd><dt><span>standard_name :</span></dt><dd>northward_wind</dd></dl></div><div class='xr-var-data'><pre>[168 values with dtype=float32]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-4213f844-5c41-47e1-a95f-8ebfc797a7f5' class='xr-section-summary-in' type='checkbox'  ><label for='section-4213f844-5c41-47e1-a95f-8ebfc797a7f5' class='xr-section-summary' >Indexes: <span>(5)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-index-name'><div>time</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-f21370f2-2d99-47de-aa94-368321ce64b6' class='xr-index-data-in' type='checkbox'/><label for='index-f21370f2-2d99-47de-aa94-368321ce64b6' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(DatetimeIndex([&#x27;2018-08-01 12:00:00&#x27;], dtype=&#x27;datetime64[ns]&#x27;, name=&#x27;time&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>step</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-c6502882-1a79-41fd-8007-84de45639ef4' class='xr-index-data-in' type='checkbox'/><label for='index-c6502882-1a79-41fd-8007-84de45639ef4' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(TimedeltaIndex([&#x27;0 days&#x27;], dtype=&#x27;timedelta64[ns]&#x27;, name=&#x27;step&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>isobaricInhPa</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-077ae806-6cd7-46f0-842a-24c560289233' class='xr-index-data-in' type='checkbox'/><label for='index-077ae806-6cd7-46f0-842a-24c560289233' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Int64Index([1000, 850], dtype=&#x27;int64&#x27;, name=&#x27;isobaricInhPa&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>latitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-c9510b7a-bddf-4e3f-b124-be6b0dcc2a0e' class='xr-index-data-in' type='checkbox'/><label for='index-c9510b7a-bddf-4e3f-b124-be6b0dcc2a0e' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Float64Index([90.0, 60.0, 30.0, 0.0, -30.0, -60.0, -90.0], dtype=&#x27;float64&#x27;, name=&#x27;latitude&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>longitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-7f71d23e-8f3a-4a57-baf1-ece1a13759cb' class='xr-index-data-in' type='checkbox'/><label for='index-7f71d23e-8f3a-4a57-baf1-ece1a13759cb' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Float64Index([0.0, 30.0, 60.0, 90.0, 120.0, 150.0, 180.0, 210.0, 240.0, 270.0,\n",
                             "              300.0, 330.0],\n",
-                            "             dtype=&#x27;float64&#x27;, name=&#x27;longitude&#x27;))</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-a4dfbfb4-d7ff-4c8e-a1f9-32f4e74a6649' class='xr-section-summary-in' type='checkbox'  checked><label for='section-a4dfbfb4-d7ff-4c8e-a1f9-32f4e74a6649' class='xr-section-summary' >Attributes: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>GRIB_edition :</span></dt><dd>1</dd><dt><span>GRIB_centre :</span></dt><dd>ecmf</dd><dt><span>GRIB_centreDescription :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>GRIB_subCentre :</span></dt><dd>0</dd><dt><span>Conventions :</span></dt><dd>CF-1.7</dd><dt><span>institution :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>history :</span></dt><dd>2023-05-04T16:43 GRIB to CDM+CF via cfgrib-0.9.10.3/ecCodes-2.27.1 with {&quot;source&quot;: &quot;N/A&quot;, &quot;filter_by_keys&quot;: {}, &quot;encode_cf&quot;: [&quot;parameter&quot;, &quot;time&quot;, &quot;geography&quot;, &quot;vertical&quot;]}</dd></dl></div></li></ul></div></div>"
+                            "             dtype=&#x27;float64&#x27;, name=&#x27;longitude&#x27;))</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-0bab1f97-9927-421d-b0ab-92692c0a212f' class='xr-section-summary-in' type='checkbox'  checked><label for='section-0bab1f97-9927-421d-b0ab-92692c0a212f' class='xr-section-summary' >Attributes: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>GRIB_edition :</span></dt><dd>1</dd><dt><span>GRIB_centre :</span></dt><dd>ecmf</dd><dt><span>GRIB_centreDescription :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>GRIB_subCentre :</span></dt><dd>0</dd><dt><span>Conventions :</span></dt><dd>CF-1.7</dd><dt><span>institution :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>history :</span></dt><dd>2023-05-17T17:40 GRIB to CDM+CF via cfgrib-0.9.10.3/ecCodes-2.27.1 with {&quot;source&quot;: &quot;N/A&quot;, &quot;filter_by_keys&quot;: {}, &quot;encode_cf&quot;: [&quot;parameter&quot;, &quot;time&quot;, &quot;geography&quot;, &quot;vertical&quot;]}</dd></dl></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<xarray.Dataset>\n",
                             "Dimensions:        (time: 1, step: 1, isobaricInhPa: 2, latitude: 7,\n",
                             "                    longitude: 12)\n",
                             "Coordinates:\n",
                             "  * time           (time) datetime64[ns] 2018-08-01T12:00:00\n",
@@ -1852,15 +1852,15 @@
                             "Attributes:\n",
                             "    GRIB_edition:            1\n",
                             "    GRIB_centre:             ecmf\n",
                             "    GRIB_centreDescription:  European Centre for Medium-Range Weather Forecasts\n",
                             "    GRIB_subCentre:          0\n",
                             "    Conventions:             CF-1.7\n",
                             "    institution:             European Centre for Medium-Range Weather Forecasts\n",
-                            "    history:                 2023-05-04T16:43 GRIB to CDM+CF via cfgrib-0.9.1..."
+                            "    history:                 2023-05-17T17:40 GRIB to CDM+CF via cfgrib-0.9.1..."
                         ]
                     },
                     "execution_count": 24,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
```

### Comparing `earthkit-data-0.1.2/docs/examples/grib_selection.ipynb` & `earthkit-data-0.1.3/docs/examples/grib_selection.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9865757275132275%*

 * *Differences: {"'cells'": "{0: {'source': ['!test -f tuv_pl.grib || wget "*

 * *            "https://get.ecmwf.int/repository/test-data/earthkit-data/examples/tuv_pl.grib']}, 8: "*

 * *            "{'outputs': {0: {'data': {'text/plain': "*

 * *            "['earthkit.data.readers.grib.index.MaskFieldList']}}}}, 16: {'source': ['isel() works "*

 * *            'similarly to sel() but takes indices instead of values. Please note that the index '*

 * *            "values are sorted for isel().']}, 24: {'outputs': {0: {'data': {'text/plain': "*

 * *     […]*

```diff
@@ -2,15 +2,15 @@
     "cells": [
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
-                "!test -f tuv_pl.grib || https://get.ecmwf.int/repository/test-data/emohawk/examples/tuv_pl.grib"
+                "!test -f tuv_pl.grib || wget https://get.ecmwf.int/repository/test-data/earthkit-data/examples/tuv_pl.grib"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "tags": []
             },
@@ -178,15 +178,15 @@
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "earthkit.data.readers.grib.index.MaskFieldSet"
+                            "earthkit.data.readers.grib.index.MaskFieldList"
                         ]
                     },
                     "execution_count": 5,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -549,15 +549,15 @@
                 "### Using isel"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "isel() works similarly to sel() but takes indices instead of values. Please note that the coordinate values are not sorted for isel() but used in their order of appearance in the input data."
+                "isel() works similarly to sel() but takes indices instead of values. Please note that the index values are sorted for isel()."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 9,
             "metadata": {},
             "outputs": [
@@ -952,15 +952,15 @@
             "cell_type": "code",
             "execution_count": 13,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "earthkit.data.readers.grib.index.MaskFieldSet"
+                            "earthkit.data.readers.grib.index.MaskFieldList"
                         ]
                     },
                     "execution_count": 13,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -1634,27 +1634,27 @@
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "mpy38",
+            "display_name": "dev",
             "language": "python",
-            "name": "mpy38"
+            "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.16"
+            "version": "3.10.9"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `earthkit-data-0.1.2/docs/examples/grib_tar.ipynb` & `earthkit-data-0.1.3/docs/examples/grib_tar.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9984953703703703%*

 * *Differences: {"'cells'": "{0: {'source': ['!test -f test_gribs.tar || wget "*

 * *            "https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test_gribs.tar']}, "*

 * *            "5: {'outputs': {0: {'text': {insert: [(0, ' MultiFieldList\\n')], delete: [0]}}}}}"}*

```diff
@@ -2,15 +2,15 @@
     "cells": [
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
-                "!test -f test_gribs.tar || wget https://get.ecmwf.int/repository/test-data/emohawk/examples/test_gribs.tar"
+                "!test -f test_gribs.tar || wget https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test_gribs.tar"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Reading GRIB in tar or zip archive"
@@ -46,15 +46,15 @@
             "execution_count": 3,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        " MultiFieldSet\n",
+                        " MultiFieldList\n",
                         "    GRIBReader(/var/folders/ng/g0zkhc2s42xbslpsywwp_26m0000gn/T/earthkit-data-cgr/file-461599e4bea1fe52b7dfd30afff92448fce511fe6e8c41fba0893c7822ab2f30.d/test.grib)\n",
                         "    GRIBReader(/var/folders/ng/g0zkhc2s42xbslpsywwp_26m0000gn/T/earthkit-data-cgr/file-461599e4bea1fe52b7dfd30afff92448fce511fe6e8c41fba0893c7822ab2f30.d/test4.grib)\n"
                     ]
                 }
             ],
             "source": [
                 "fs.graph()"
```

### Comparing `earthkit-data-0.1.2/docs/examples/grib_to_netcdf.ipynb` & `earthkit-data-0.1.3/docs/examples/grib_to_netcdf.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9985119047619048%*

 * *Differences: {"'cells'": "{0: {'source': ['!test -f tuv_pl.grib || wget "*

 * *            "https://get.ecmwf.int/repository/test-data/earthkit-data/examples/tuv_pl.grib']}}"}*

```diff
@@ -3,15 +3,15 @@
         {
             "cell_type": "code",
             "execution_count": 1,
             "id": "bea7a770-c42d-488f-a533-d8fe9202a38f",
             "metadata": {},
             "outputs": [],
             "source": [
-                "!test -f tuv_pl.grib || https://get.ecmwf.int/repository/test-data/emohawk/examples/tuv_pl.grib"
+                "!test -f tuv_pl.grib || wget https://get.ecmwf.int/repository/test-data/earthkit-data/examples/tuv_pl.grib"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "9c53d7c8-7f38-4a5f-93d0-e05919408b6e",
             "metadata": {},
             "source": [
```

### Comparing `earthkit-data-0.1.2/docs/examples/grib_url.ipynb` & `earthkit-data-0.1.3/docs/examples/grib_url.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9985396241830065%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(3, '                       "*

 * *            '"https://get.ecmwf.int/repository/test-data/earthkit-data/test-data/t_pl.grib")\')], '*

 * *            "delete: [3]}}, 6: {'source': {insert: [(1, '                       "*

 * *            '"https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test_gribs.tar")\')], '*

 * *            "delete: [1]}}, 10: {'source': {insert: [(1, '                       "*

 * *            '["https://get.ecmwf.int/repository/test-data/earthkit-data/exa […]*

```diff
@@ -32,15 +32,15 @@
             "id": "9e07cfc0-6a41-4865-aefc-1d352d70fe4a",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import earthkit.data\n",
                 "\n",
                 "fs = earthkit.data.from_source(\"url\", \n",
-                "                       \"https://get.ecmwf.int/repository/test-data/emohawk/test-data/t_pl.grib\")"
+                "                       \"https://get.ecmwf.int/repository/test-data/earthkit-data/test-data/t_pl.grib\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "id": "df2a80a3-05a7-4385-947b-7c383f453929",
             "metadata": {},
@@ -200,15 +200,15 @@
             "cell_type": "code",
             "execution_count": 3,
             "id": "f1a423ae-7003-4185-b0c4-292f01cebb70",
             "metadata": {},
             "outputs": [],
             "source": [
                 "fs = earthkit.data.from_source(\"url\", \n",
-                "                       \"https://get.ecmwf.int/repository/test-data/emohawk/examples/test_gribs.tar\")"
+                "                       \"https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test_gribs.tar\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "id": "e44b8784-51e9-4529-b9c7-4cfa03aa0f21",
             "metadata": {},
@@ -515,16 +515,16 @@
                     "execution_count": 5,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "fs = earthkit.data.from_source(\"url\", \n",
-                "                       [\"https://get.ecmwf.int/repository/test-data/emohawk/examples/test.grib\",\n",
-                "                        \"https://get.ecmwf.int/repository/test-data/emohawk/examples/test4.grib\"])\n",
+                "                       [\"https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test.grib\",\n",
+                "                        \"https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test4.grib\"])\n",
                 "fs.ls()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "585e7e29-9e50-49cb-96af-13d4d725de6a",
             "metadata": {},
@@ -757,15 +757,15 @@
                     "execution_count": 6,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "fs = earthkit.data.from_source(\"url-pattern\",                        \n",
-                "                        \"https://get.ecmwf.int/repository/test-data/emohawk/examples/test{id}.grib\",\n",
+                "                        \"https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test{id}.grib\",\n",
                 "                        {\"id\": [4, 6]})\n",
                 "fs.ls()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "a0420b9d-3d9a-4357-9044-3dec40951b80",
@@ -874,15 +874,15 @@
                 }
             ],
             "source": [
                 "import datetime \n",
                 "\n",
                 "fs = earthkit.data.from_source(\n",
                 "    \"url-pattern\",                        \n",
-                "    \"https://get.ecmwf.int/repository/test-data/emohawk/test-data/test_{my_date:date(%Y-%m-%d)}_{name}.grib\",\n",
+                "    \"https://get.ecmwf.int/repository/test-data/earthkit-data/test-data/test_{my_date:date(%Y-%m-%d)}_{name}.grib\",\n",
                 "    {\"my_date\": datetime.datetime(2020,5,13), \"name\": [\"t2\",\"msl\"]})\n",
                 "fs.ls()\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
```

### Comparing `earthkit-data-0.1.2/docs/examples/list_of_dict.ipynb` & `earthkit-data-0.1.3/docs/examples/list_of_dict.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.984375%*

 * *Differences: {"'cells'": "{1: {'source': ['The following object is created from a list of dicts:'], "*

 * *            "'attachments': OrderedDict()}, insert: [(10, OrderedDict([('cell_type', 'markdown'), "*

 * *            "('metadata', OrderedDict()), ('source', [])]))]}"}*

```diff
@@ -4,18 +4,19 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Using list of dictionaries as input"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "The following object is created form a list of dicts:"
+                "The following object is created from a list of dicts:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
@@ -763,14 +764,19 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": []
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "mpy38",
             "language": "python",
             "name": "mpy38"
```

### Comparing `earthkit-data-0.1.2/docs/examples/missing.grib` & `earthkit-data-0.1.3/docs/examples/missing.grib`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/docs/examples/netcdf.ipynb` & `earthkit-data-0.1.3/docs/examples/netcdf.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9984375%*

 * *Differences: {"'cells'": "{0: {'source': ['!test -f test.nc || wget "*

 * *            "https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test.nc']}}"}*

```diff
@@ -2,15 +2,15 @@
     "cells": [
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
-                "!test -f test.nc || wget https://get.ecmwf.int/repository/test-data/emohawk/examples/test.nc"
+                "!test -f test.nc || wget https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test.nc"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Using NetCDF data"
```

### Comparing `earthkit-data-0.1.2/docs/examples/temp_10.bufr` & `earthkit-data-0.1.3/docs/examples/temp_10.bufr`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/docs/examples/test.grib` & `earthkit-data-0.1.3/docs/examples/test.grib`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/docs/examples/test.nc` & `earthkit-data-0.1.3/docs/examples/test.nc`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/docs/examples/test4.grib` & `earthkit-data-0.1.3/docs/examples/test4.grib`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/docs/examples/test6.grib` & `earthkit-data-0.1.3/docs/examples/test6.grib`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/docs/examples/tuv_pl.grib` & `earthkit-data-0.1.3/docs/examples/tuv_pl.grib`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/docs/examples.rst` & `earthkit-data-0.1.3/docs/examples.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,34 @@
 .. _examples:
 
 Examples
 ============
 
 Here is a list of example notebooks to illustrate how to use earthkit-data.
 
+
+.. toctree::
+    :maxdepth: 1
+    :caption: Retrieve
+
+    examples/mars.ipynb
+    examples/cds.ipynb
+    examples/fdb.ipynb
+
+
 .. toctree::
     :maxdepth: 1
     :caption: GRIB
 
     examples/grib_overview.ipynb
-    examples/grib_indexing.ipynb
     examples/grib_metadata.ipynb
-    examples/grib_missing.ipynb
     examples/grib_selection.ipynb
+    examples/grib_indexing.ipynb
+    examples/grib_missing.ipynb
     examples/grib_multi.ipynb
-    examples/grib_fdb_stream.ipynb
     examples/grib_from_stream.ipynb
     examples/grib_file_pattern.ipynb
     examples/grib_tar.ipynb
     examples/grib_url.ipynb
     examples/grib_to_netcdf.ipynb
 
 .. toctree::
@@ -34,11 +43,18 @@
     :caption: BUFR
     :glob:
 
     examples/bufr*
 
 .. toctree::
     :maxdepth: 1
+    :caption: ODB
+    :glob:
+
+    examples/odb*
+
+.. toctree::
+    :maxdepth: 1
     :caption: List of dicts
     :glob:
 
     examples/list_of_dict*
```

### Comparing `earthkit-data-0.1.2/docs/index.rst` & `earthkit-data-0.1.3/docs/index.rst`

 * *Files 11% similar despite different names*

```diff
@@ -10,20 +10,20 @@
     This documentation is still work in progress and can only be regarded as a **DRAFT**.
 
 
 **earthkit-data** is a format-agnostic Python interface for geospatial data with a focus on meteorology and
 climate science.
 
 **earthkit-data** makes it simple to read, inspect and slice data from a wide range of
-geospatial input types (GRIB, netCDF and more) and transform them into
+geospatial input types (:ref:`grib`, :ref:`netcdf` and more) and transform them into
 familiar scientific Python objects (including numpy arrays, pandas dataframes, xarray datasets).
 
 .. code-block:: python
 
-    data = earthkit.data.from_source("my-data.nc")
+    data = earthkit.data.from_source("file", "my-data.nc")
     arr = data.to_numpy()
     df = data.to_pandas()
     dataset = data.to_xarray()
 
 
 **earthkit-data** provides additional convenient methods for quickly inspecting certain
 features of your input data, such as data dimensionality, axes, coordinate
@@ -32,21 +32,27 @@
 .. toctree::
    :maxdepth: 1
    :caption: Examples
    :titlesonly:
 
    examples
 
+.. toctree::
+   :maxdepth: 1
+   :caption: Documentation
+
+   guide/index
+   api
 
 .. toctree::
    :maxdepth: 1
    :caption: Installation
 
    install
-   contributing
+   development
    licence
 
 
 Indices and tables
 ==================
 
 * :ref:`genindex`
```

### Comparing `earthkit-data-0.1.2/docs/install.rst` & `earthkit-data-0.1.3/docs/install.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Installation
 ============
 
 Installing earthkit-data
 ----------------------------
 
-**earthkit-data** can be installed from PyPI with:
+Install **earthkit-data** with python3 (>= 3.8) and **pip** as follows:
 
 .. code-block:: bash
 
-    pip install earthkit-data
+    python3 -m pip install earthkit-data
 
 
 Installing the binary dependencies
 --------------------------------------
 
+eccCodes
++++++++++++
+
 **earthkit-data** depends on the ECMWF *ecCodes* library
 that must be installed on the system and accessible as a shared library. The easiest way to install it is to use Conda:
 
 .. code-block:: bash
 
     conda install eccodes -c conda-forge
 
@@ -27,7 +30,12 @@
 .. code-block:: bash
 
     brew install eccodes
 
 As an alternative you may install the official source distribution
 by following the instructions at
 https://software.ecmwf.int/wiki/display/ECC/ecCodes+installation
+
+FDB
++++++
+
+For FDB (Fields DataBase) access FDB5 must be installed in the system. See the `FDB documentation <https://fields-database.readthedocs.io/en/latest/>`_ for details.
```

### Comparing `earthkit-data-0.1.2/docs/licence.rst` & `earthkit-data-0.1.3/docs/licence.rst`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/docs/make.bat` & `earthkit-data-0.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/__init__.py` & `earthkit-data-0.1.3/earthkit/data/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,17 +14,19 @@
 except ImportError:  # pragma: no cover
     # Local copy or not installed with setuptools
     __version__ = "999"
 
 from .arguments.transformers import ALL
 from .core.caching import CACHE as cache
 from .core.settings import SETTINGS as settings
+from .readers.grib.output import new_grib_output
 from .sources import from_source, from_source_lazily
 
 __all__ = [
     "ALL",
     "cache",
     "from_source",
     "from_source_lazily",
+    "new_grib_output",
     "settings",
     "__version__",
 ]
```

### Comparing `earthkit-data-0.1.2/earthkit/data/arguments/__init__.py` & `earthkit-data-0.1.3/earthkit/data/arguments/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/arguments/args_kwargs.py` & `earthkit-data-0.1.3/earthkit/data/arguments/args_kwargs.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/arguments/argument.py` & `earthkit-data-0.1.3/earthkit/data/arguments/argument.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/arguments/earthkit_types.py` & `earthkit-data-0.1.3/earthkit/data/arguments/earthkit_types.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/arguments/input_manager.py` & `earthkit-data-0.1.3/earthkit/data/arguments/input_manager.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/arguments/transformers.py` & `earthkit-data-0.1.3/earthkit/data/arguments/transformers.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/core/__init__.py` & `earthkit-data-0.1.3/earthkit/data/core/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -31,72 +31,86 @@
 
         return args, kwargs
 
 
 class Base(metaclass=MetaBase):
     # Convertors
     def to_numpy(self, **kwargs):
+        """Converts into a numpy array"""
         self._not_implemented()
 
     @abstractmethod
     def to_xarray(self, **kwargs):
+        """Converts into an xarray dataset"""
         self._not_implemented()
 
     @abstractmethod
     def to_pandas(self, **kwargs):
+        """Converts into a pandas dataframe"""
         self._not_implemented()
 
     # Change class
     def mutate(self):
         return self
 
     @classmethod
     def merge(cls, *args, **kwargs):
+        """Merges the object with other ones."""
         return None
 
     @abstractmethod
-    def metadata(self):
+    def metadata(self, *args, **kwargs):
+        """Returns metadata."""
         self._not_implemented()
 
     # I/O
     @abstractmethod
     def save(self, path):
+        """Writes data into the specified ``path``."""
         self._not_implemented()
 
     @abstractmethod
     def write(self, f):
+        """Writes data to the ``f`` file object."""
         self._not_implemented()
 
     @abstractmethod
     def datetime(self):
+        """Returns datetime."""
         self._not_implemented()
 
     @abstractmethod
     def bounding_box(self):
+        """Returns the bounding box."""
         self._not_implemented()
 
     # For machine learning
     @abstractmethod
     def statistics(self):
         self._not_implemented()
 
     @abstractmethod
     def scaled(self, args, kwargs):
         self._not_implemented()
 
     @abstractmethod
     def sel(self, *args, **kwargs):
+        """Filters the object based on metadata."""
         self._not_implemented()
 
     @abstractmethod
     def isel(self, *args, **kwargs):
         self._not_implemented()
 
     @abstractmethod
     def order_by(self, *args, **kwargs):
+        """Reorder the elements of the object."""
+        self._not_implemented()
+
+    def __add__(self, other):
         self._not_implemented()
 
     #
     def _not_implemented(self):
         import inspect
 
         func = inspect.stack()[1][3]
```

### Comparing `earthkit-data-0.1.2/earthkit/data/core/caching.py` & `earthkit-data-0.1.3/earthkit/data/core/caching.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/core/ipython.py` & `earthkit-data-0.1.3/earthkit/data/core/ipython.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/core/order.py` & `earthkit-data-0.1.3/earthkit/data/core/order.py`

 * *Files 21% similar despite different names*

```diff
@@ -22,44 +22,44 @@
             self.remapping[k] = m
 
     def __call__(self, func):
         if self.remapping is None or not self.remapping:
             return func
 
         class CustomJoiner:
-            def format_name(self, x):
-                return func(x)
+            def format_name(self, x, **kwargs):
+                return func(x, **kwargs)
 
             def format_string(self, x):
                 return str(x)
 
             def join(self, args):
                 return "".join(str(x) for x in args)
 
         joiner = CustomJoiner()
 
-        def wrapped(name):
-            return self.substitute(name, joiner)
+        def wrapped(name, **kwargs):
+            return self.substitute(name, joiner, **kwargs)
 
         return wrapped
 
-    def substitute(self, name, joiner):
+    def substitute(self, name, joiner, **kwargs):
         if name in self.remapping:
             lst = []
             for i, bit in enumerate(self.remapping[name]):
                 if i % 2:
-                    p = joiner.format_name(bit)
+                    p = joiner.format_name(bit, **kwargs)
                     if p is not None:
                         lst.append(p)
                     else:
                         lst = lst[:-1]
                 else:
                     lst.append(joiner.format_string(bit))
             return joiner.join(lst)
-        return joiner.format_name(name)
+        return joiner.format_name(name, **kwargs)
 
     def as_dict(self):
         return self.remapping
 
 
 def build_remapping(mapping):
     if mapping is None:
```

### Comparing `earthkit-data-0.1.2/earthkit/data/core/plugins.py` & `earthkit-data-0.1.3/earthkit/data/core/plugins.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/core/select.py` & `earthkit-data-0.1.3/earthkit/data/core/select.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/core/settings.py` & `earthkit-data-0.1.3/earthkit/data/core/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,20 +23,29 @@
 
 LOG = logging.getLogger(__name__)
 
 DOT_EARTHKIT_DATA = os.path.expanduser("~/.earthkit_data")
 
 
 class Setting:
-    def __init__(self, default, description, getter=None, none_ok=False, kind=None):
+    def __init__(
+        self,
+        default,
+        description,
+        getter=None,
+        none_ok=False,
+        kind=None,
+        docs_default=None,
+    ):
         self.default = default
         self.description = description
         self.getter = getter
         self.none_ok = none_ok
         self.kind = kind if kind is not None else type(default)
+        self.docs_default = docs_default if docs_default is not None else self.default
 
     def kind(self):
         return type(self.default)
 
     def save(self, name, value, f):
         for n in self.description.split("\n"):
             print(f"# {n.strip()}", file=f)
@@ -54,14 +63,15 @@
 
 
 SETTINGS_AND_HELP = {
     "cache-directory": _(
         os.path.join(tempfile.gettempdir(), "earthkit-data-%s" % (getpass.getuser(),)),
         """Directory of where the dowloaded files are cached, with ``${USER}`` is the user id.
         See :doc:`/guide/caching` for more information.""",
+        docs_default=os.path.join("TMP", "earthkit-data-%s" % (getpass.getuser(),)),
     ),
     "dask-directories": _(
         [os.path.join(DOT_EARTHKIT_DATA, "dask")],
         """List of directories where to search for dask cluster definitions.
         See :ref:`dask` for more information.""",
     ),
     "datasets-directories": _(
@@ -76,21 +86,21 @@
     ),
     "number-of-download-threads": _(
         5,
         """Number of threads used to download data.""",
     ),
     "maximum-cache-size": _(
         None,
-        """Maximum disk space used by the CliMetLab cache (ex: 100G or 2T).""",
+        """Maximum disk space used by the earthkit-data cache (ex: 100G or 2T).""",
         getter="_as_bytes",
         none_ok=True,
     ),
     "maximum-cache-disk-usage": _(
         "95%",
-        """Disk usage threshold after which CliMetLab expires older cached
+        """Disk usage threshold after which earthkit-data expires older cached
         entries (% of the full disk capacity).
         See :doc:`/guide/caching` for more information.""",
         getter="_as_percent",
     ),
     "url-download-timeout": _(
         "30s",
         """Timeout when downloading from an url.""",
@@ -100,14 +110,18 @@
         True,
         "Perform a HTTP request to check if the remote version of a cache file has changed",
     ),
     "download-out-of-date-urls": _(
         False,
         "Re-download URLs when the remote version of a cached file as been changed",
     ),
+    "use-standalone-mars-client-when-available": _(
+        True,
+        "Use the standalone mars client when available instead of using the web API.",
+    ),
 }
 
 
 NONE = object()
 DEFAULTS = {}
 for k, v in SETTINGS_AND_HELP.items():
     DEFAULTS[k] = v.default
```

### Comparing `earthkit-data-0.1.2/earthkit/data/core/statistics.py` & `earthkit-data-0.1.3/earthkit/data/core/statistics.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/core/temporary.py` & `earthkit-data-0.1.3/earthkit/data/core/temporary.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/core/thread.py` & `earthkit-data-0.1.3/earthkit/data/core/thread.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/data/css/tab.css` & `earthkit-data-0.1.3/earthkit/data/data/css/tab.css`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/decorators.py` & `earthkit-data-0.1.3/earthkit/data/decorators.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/indexing/__init__.py` & `earthkit-data-0.1.3/earthkit/data/indexing/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/indexing/database/__init__.py` & `earthkit-data-0.1.3/earthkit/data/indexing/database/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/indexing/database/json.py` & `earthkit-data-0.1.3/earthkit/data/indexing/database/json.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/indexing/database/sql.py` & `earthkit-data-0.1.3/earthkit/data/indexing/database/sql.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/indexing/database/stdout.py` & `earthkit-data-0.1.3/earthkit/data/indexing/database/stdout.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/input_manager.py` & `earthkit-data-0.1.3/earthkit/data/input_manager.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/mergers/__init__.py` & `earthkit-data-0.1.3/earthkit/data/mergers/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/mergers/pandas.py` & `earthkit-data-0.1.3/earthkit/data/mergers/pandas.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/mergers/xarray.py` & `earthkit-data-0.1.3/earthkit/data/mergers/xarray.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/mirrors/__init__.py` & `earthkit-data-0.1.3/earthkit/data/mirrors/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/mirrors/directory_mirror.py` & `earthkit-data-0.1.3/earthkit/data/mirrors/directory_mirror.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/readers/__init__.py` & `earthkit-data-0.1.3/earthkit/data/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/readers/archive.py` & `earthkit-data-0.1.3/earthkit/data/readers/archive.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/readers/bufr.py` & `earthkit-data-0.1.3/earthkit/data/readers/bufr.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,19 +27,43 @@
     "ident": "ident",
     "lat": "localLatitude",
     "lon": "localLongitude",
 }
 
 
 class BUFRReader(Reader):
+    """Represents a BUFR file"""
+
     def __init__(self, source, path):
         super().__init__(source, path)
         self._num = None
 
     def to_pandas(self, columns=COLUMNS, filters=None, **kwargs):
+        """Extracts BUFR data into an pandas DataFranme using :xref:`pdbufr`.
+
+        Parameters
+        ----------
+        columns: str, sequence[str]
+            List of ecCodes BUFR keys to extract for each BUFR message/subset.
+            See: :xref:`read_bufr` for details.
+        filters: dict
+            Defines the conditions when to extract the specified ``columns``. See:
+            :xref:`read_bufr` for details.
+        **kwargs: dict, optional
+            Other keyword arguments:
+
+        Returns
+        -------
+        Pandas DataFrame
+
+        Examples
+        --------
+        :ref:`/examples/bufr.ipynb`
+
+        """
         import pdbufr
 
         return pdbufr.read_bufr(self.path, columns=columns, filters=filters)
 
     def __len__(self):
         if self._num is None:
             import eccodes
```

### Comparing `earthkit-data-0.1.2/earthkit/data/readers/csv.py` & `earthkit-data-0.1.3/earthkit/data/readers/csv.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/readers/directory.py` & `earthkit-data-0.1.3/earthkit/data/readers/directory.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/readers/grib/__init__.py` & `earthkit-data-0.1.3/earthkit/data/readers/grib/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,20 +20,20 @@
         from .reader import GRIBReader
 
         return GRIBReader(source, path)
 
 
 def memory_reader(source, buf, magic=None, deeper_check=False):
     if _match_magic(magic):
-        from .memory import FieldSetInMemory, GribMessageMemoryReader
+        from .memory import FieldListInMemory, GribMessageMemoryReader
 
-        return FieldSetInMemory(source, GribMessageMemoryReader(buf))
+        return FieldListInMemory(source, GribMessageMemoryReader(buf))
 
 
 def stream_reader(source, stream, magic=None, deeper_check=False):
     if _match_magic(magic):
-        from .memory import FieldSetInMemory, GribStreamReader
+        from .memory import FieldListInMemory, GribStreamReader
 
         r = GribStreamReader(stream)
-        if source.group_by == 0:
-            r = FieldSetInMemory(source, r)
+        if source.batch_size == 0:
+            r = FieldListInMemory(source, r)
         return r
```

### Comparing `earthkit-data-0.1.2/earthkit/data/readers/grib/index/db.py` & `earthkit-data-0.1.3/earthkit/data/readers/grib/index/db.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,25 +8,22 @@
 #
 
 import json
 import logging
 import os
 from urllib.parse import urljoin
 
-import requests
-from multiurl import robust
-
 from earthkit.data.core.caching import cache_file
-from earthkit.data.readers.grib.index import FieldSetInFiles
+from earthkit.data.readers.grib.index import FieldListInFiles
 from earthkit.data.utils import progress_bar
 
 LOG = logging.getLogger(__name__)
 
 
-class FieldsetInFilesWithDBIndex(FieldSetInFiles):
+class FieldListInFilesWithDBIndex(FieldListInFiles):
     def __init__(self, db, **kwargs):
         """Should not be instantiated directly.
         The public API are the constructors "_from*()" class methods.
         """
         self.db = db
 
         # self._cache is a tuple : (first, length, result). It holds one chunk of the db.
@@ -72,14 +69,17 @@
         new = new.sel(selection)
         new = new.order_by(order_by)
         return new
 
     @classmethod
     def from_url(cls, url, patch_entry=None, **kwargs):
         """Create a database from a given url"""
+        import requests
+        from multiurl import robust
+
         # If this is a file, open it without download
         if os.path.exists(url):
             return cls.from_file(path=url, **kwargs)
         if url.startswith("file://") and os.path.exists(url[7:]):
             return cls.from_file(path=url[7:], **kwargs)
 
         # Request to download the data
```

### Comparing `earthkit-data-0.1.2/earthkit/data/readers/grib/index/file.py` & `earthkit-data-0.1.3/earthkit/data/readers/grib/index/file.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,21 +10,21 @@
 
 import json
 import logging
 import os
 
 from earthkit.data.core.caching import auxiliary_cache_file
 from earthkit.data.readers.grib.codes import get_messages_positions
-from earthkit.data.readers.grib.index import FieldSetInFiles
+from earthkit.data.readers.grib.index import FieldListInFiles
 from earthkit.data.utils.parts import Part
 
 LOG = logging.getLogger(__name__)
 
 
-class FieldSetInOneFile(FieldSetInFiles):
+class FieldListInOneFile(FieldListInFiles):
     VERSION = 1
 
     @property
     def availability_path(self):
         return os.path.join(self.path, ".availability.pickle")
 
     def __init__(self, path, **kwargs):
```

### Comparing `earthkit-data-0.1.2/earthkit/data/readers/grib/index/json.py` & `earthkit-data-0.1.3/earthkit/data/readers/grib/index/json.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 #
 
 
 from earthkit.data.decorators import cached_method
 from earthkit.data.indexing.database.json import JsonFileDatabase
-from earthkit.data.readers.grib.index.db import FieldsetInFilesWithDBIndex
+from earthkit.data.readers.grib.index.db import FieldListInFilesWithDBIndex
 
 
-class FieldsetInFilesWithJsonIndex(FieldsetInFilesWithDBIndex):
+class FieldListInFilesWithJsonIndex(FieldListInFilesWithDBIndex):
     DBCLASS = JsonFileDatabase
 
     @cached_method
     def _lookup_parts(self):
         return self.db.lookup_parts()
 
     def part(self, n):
```

### Comparing `earthkit-data-0.1.2/earthkit/data/readers/grib/index/sql.py` & `earthkit-data-0.1.3/earthkit/data/readers/grib/index/sql.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,28 +16,28 @@
 from earthkit.data.decorators import cached_method, normalize
 from earthkit.data.indexing.database.sql import (
     SqlDatabase,
     SqlOrder,
     SqlRemapping,
     SqlSelection,
 )
-from earthkit.data.readers.grib.index.db import FieldsetInFilesWithDBIndex
+from earthkit.data.readers.grib.index.db import FieldListInFilesWithDBIndex
 from earthkit.data.utils.serialise import register_serialisation
 
 LOG = logging.getLogger(__name__)
 
 SqlResultCache = namedtuple("SqlResultCache", ["first", "length", "result"])
 
 
 @normalize(DATETIME, "date-list", format="%Y-%m-%d %H:%M:%S")
 def _normalize_grib_kwargs_values(**kwargs):
     return kwargs
 
 
-class FieldsetInFilesWithSqlIndex(FieldsetInFilesWithDBIndex):
+class FieldListInFilesWithSqlIndex(FieldListInFilesWithDBIndex):
     DBCLASS = SqlDatabase
     DB_CACHE_SIZE = 100_000
     DB_DICT_CACHE_SIZE = 100_000
 
     def apply_filters(self, filters):
         obj = self
         for f in filters:
@@ -137,13 +137,13 @@
 
     @cached_method
     def number_of_parts(self):
         return self.db.count()
 
 
 register_serialisation(
-    FieldsetInFilesWithSqlIndex,
+    FieldListInFilesWithSqlIndex,
     lambda x: [x.db.db_path, x.db._filters],
-    lambda x: FieldsetInFilesWithSqlIndex(db=SqlDatabase(x[0])).apply_filters(
+    lambda x: FieldListInFilesWithSqlIndex(db=SqlDatabase(x[0])).apply_filters(
         filters=x[1]
     ),
 )
```

### Comparing `earthkit-data-0.1.2/earthkit/data/readers/grib/memory.py` & `earthkit-data-0.1.3/earthkit/data/readers/grib/memory.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 import logging
 
 import eccodes
 
 from earthkit.data.readers import Reader
 from earthkit.data.readers.grib.codes import CodesHandle, GribField
-from earthkit.data.readers.grib.index import FieldSet
+from earthkit.data.readers.grib.index import FieldList
 
 LOG = logging.getLogger(__name__)
 
 
 class GribMemoryReader(Reader):
     def __iter__(self):
         return self
@@ -28,17 +28,17 @@
         if handle is not None:
             return GribFieldInMemory(CodesHandle(handle, None, None))
         raise StopIteration
 
     def _next_handle(self):
         raise NotImplementedError
 
-    def read_group(self, n):
+    def read_batch(self, n):
         fields = [self.__next__() for _ in range(n)]
-        return FieldSetInMemory.from_fields(fields)
+        return FieldListInMemory.from_fields(fields)
 
 
 class GribFileMemoryReader(GribMemoryReader):
     def __init__(self, path):
         self.fp = open(path, "rb")
 
     def __del__(self):
@@ -95,31 +95,31 @@
         return self._handle
 
     @GribField.handle.getter
     def offset(self):
         return None
 
 
-class FieldSetInMemory(FieldSet, Reader):
+class FieldListInMemory(FieldList, Reader):
     """Represent a GRIB field list in memory"""
 
     @staticmethod
     def from_fields(fields):
-        fs = FieldSetInMemory(None, None)
+        fs = FieldListInMemory(None, None)
         fs._fields = fields
         fs._loaded = True
         return fs
 
     def __init__(self, source, reader, *args, **kwargs):
         """
         The reader must support __next__.
         """
         if source is not None:
             Reader.__init__(self, source, None)
-        FieldSet.__init__(self, *args, **kwargs)
+        FieldList.__init__(self, *args, **kwargs)
 
         self._reader = reader
         self._loaded = False
         self._fields = []
 
     def __len__(self):
         self._load()
```

### Comparing `earthkit-data-0.1.2/earthkit/data/readers/grib/pandas.py` & `earthkit-data-0.1.3/earthkit/data/readers/grib/pandas.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,14 @@
         if latitude is not None or longitude is not None:
             filter = select_point
 
         columns = ("lat", "lon", "value")
         frames = []
         for s in self:
             df = pd.DataFrame.from_dict(
-                filter(dict(zip(columns, s.data("lat", "lon", "value", flatten=True))))
+                filter(dict(zip(columns, s.data(columns, flatten=True))))
             )
             df["datetime"] = s.datetime()["valid_time"]
             for k, v in s.metadata(namespace="mars").items():
                 df[k] = v
             frames.append(df)
         return pd.concat(frames)
```

### Comparing `earthkit-data-0.1.2/earthkit/data/readers/grib/parsing.py` & `earthkit-data-0.1.3/earthkit/data/readers/grib/parsing.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/readers/grib/reader.py` & `earthkit-data-0.1.3/earthkit/data/readers/grib/reader.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,33 +6,33 @@
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 #
 
 import logging
 
 from earthkit.data.readers import Reader
-from earthkit.data.readers.grib.index import MultiFieldSet
-from earthkit.data.readers.grib.index.file import FieldSetInOneFile
+from earthkit.data.readers.grib.index import MultiFieldList
+from earthkit.data.readers.grib.index.file import FieldListInOneFile
 
 LOG = logging.getLogger(__name__)
 
 
-class GRIBReader(FieldSetInOneFile, Reader):
+class GRIBReader(FieldListInOneFile, Reader):
     appendable = True  # GRIB messages can be added to the same file
 
     def __init__(self, source, path):
         Reader.__init__(self, source, path)
-        FieldSetInOneFile.__init__(self, path)
+        FieldListInOneFile.__init__(self, path)
 
     def __repr__(self):
         return "GRIBReader(%s)" % (self.path,)
 
     @classmethod
     def merge(cls, readers):
         assert all(isinstance(s, GRIBReader) for s in readers), readers
         assert len(readers) > 1
 
-        return MultiFieldSet(readers)
+        return MultiFieldList(readers)
 
     def mutate_source(self):
         # A GRIBReader is a source itself
         return self
```

### Comparing `earthkit-data-0.1.2/earthkit/data/readers/grib/xarray.py` & `earthkit-data-0.1.3/earthkit/data/readers/grib/xarray.py`

 * *Files 14% similar despite different names*

```diff
@@ -56,14 +56,47 @@
     def xarray_open_dataset_kwargs(self):
         return dict(
             cache=True,  # Set to false to prevent loading the whole dataset
             chunks=None,  # Set to 'auto' for lazy loading
         )
 
     def to_xarray(self, **kwargs):
+        """
+        Converts the fieldset into an xarray DataSet using :xref:`cfgrib`.
+
+        Parameters
+        ----------
+        **kwargs: dict, optional
+            Other keyword arguments:
+
+            xarray_open_dataset_kwargs: dict, optional
+                Keyword arguments passed to ``xarray.open_dataset()``. Default value is::
+
+                    {"backend_kwargs": {"errors": "raise"},
+                    "squeeze": False, "cache": True, "chunks": None,
+                    "errors": "raise", "engine": "cfgrib"}
+
+                Please note that the settings ``errors="raise"`` and ``engine="cfgrib"`` are always
+                enforced and cannot be changed.
+
+        Returns
+        -------
+        xarray DataSet
+
+        Examples
+        --------
+        >>> import earthkit.data
+        >>> fs = earthkit.data.from_source("file", "test6.grib")
+        >>> ds = fs.to_xarray(
+        ...     xarray_open_dataset_kwargs={
+        ...         "backend_kwargs": {"ignore_keys": ["number"]}
+        ...     }
+        ... )
+
+        """
         import xarray as xr
 
         xarray_open_dataset_kwargs = {}
 
         if "xarray_open_mfdataset_kwargs" in kwargs:
             warnings.warn(
                 "xarray_open_mfdataset_kwargs is deprecated, please use xarray_open_dataset_kwargs instead."
```

### Comparing `earthkit-data-0.1.2/earthkit/data/readers/netcdf.py` & `earthkit-data-0.1.3/earthkit/data/readers/netcdf.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,15 +207,15 @@
             )
 
         # Simply assume a WGS 84 target projection for CF-compliant netCDF
         proj_target = "+proj=eqc +datum=WGS84 +units=m +no_defs"
 
         return proj_source, proj_target
 
-    def to_points(self, flatten=True):
+    def to_points(self, flatten=False):
         points = dict()
         for axis in ("x", "y"):
             for coord in self._da.coords:
                 if self._da.coords[coord].attrs.get("axis", "").lower() == axis:
                     break
             else:
                 candidates = GEOGRAPHIC_COORDS.get(axis, [])
```

### Comparing `earthkit-data-0.1.2/earthkit/data/readers/numpy.py` & `earthkit-data-0.1.3/earthkit/data/readers/numpy.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/readers/odb.py` & `earthkit-data-0.1.3/earthkit/data/readers/odb.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,13 +20,13 @@
             import codc as odc
         except Exception:
             import pyodc as odc
 
             LOG.debug("Using pure Python odc decoder.")
 
         odc_read_odb_kwargs = kwargs.get("odc_read_odb_kwargs", {})
-        return odc.read_odb(self.path, single=True, *odc_read_odb_kwargs)
+        return odc.read_odb(self.path, single=True, **odc_read_odb_kwargs)
 
 
 def reader(source, path, magic=None, deeper_check=False):
     if magic is None or magic[:5] == b"\xff\xffODA":
         return ODBReader(source, path)
```

### Comparing `earthkit-data-0.1.2/earthkit/data/readers/tar.py` & `earthkit-data-0.1.3/earthkit/data/readers/tar.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/readers/text.py` & `earthkit-data-0.1.3/earthkit/data/readers/text.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/readers/unknown.py` & `earthkit-data-0.1.3/earthkit/data/readers/unknown.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/readers/zip.py` & `earthkit-data-0.1.3/earthkit/data/readers/zip.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/sources/__init__.py` & `earthkit-data-0.1.3/earthkit/data/sources/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 from importlib import import_module
 
 from earthkit.data.core import Base
 from earthkit.data.core.caching import cache_file
 from earthkit.data.core.plugins import find_plugin
 from earthkit.data.core.plugins import register as register_plugin
 from earthkit.data.core.settings import SETTINGS
-from earthkit.data.utils.html import table
 
 
 class Source(Base):
     """
     Doc
     """
 
@@ -44,14 +43,19 @@
         # Give a chance to `multi` to change source
         return self
 
     def ignore(self):
         # Used by multi-source
         return False
 
+    def __add__(self, other):
+        from earthkit.data.sources import from_source
+
+        return from_source("multi", self, other)
+
     def cache_file(self, create, args, **kwargs):
         owner = self.name
         if self.dataset:
             owner = self.dataset.name
         if owner is None:
             owner = re.sub(r"(?!^)([A-Z]+)", r"-\1", self.__class__.__name__).lower()
 
@@ -80,15 +84,15 @@
     def parent(self, parent):
         self._set_parent(weakref.ref(parent))
 
     def _set_parent(self, parent):
         self._parent = parent
 
     def _repr_html_(self):
-        return table(self)
+        return self.__repr__()
 
     def graph(self, depth=0):
         print(" " * depth, self)
 
 
 class SourceLoader:
     kind = "source"
```

### Comparing `earthkit-data-0.1.2/earthkit/data/sources/dummy_source.py` & `earthkit-data-0.1.3/earthkit/data/sources/dummy_source.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/sources/empty.py` & `earthkit-data-0.1.3/earthkit/data/sources/empty.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/sources/file.py` & `earthkit-data-0.1.3/earthkit/data/sources/file.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/sources/file_indexed.py` & `earthkit-data-0.1.3/earthkit/data/sources/file_indexed.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # In applying this licence, ECMWF does not waive the privileges and immunities
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 #
 import logging
 import os
 
-from earthkit.data.readers.grib.index.sql import FieldsetInFilesWithSqlIndex
+from earthkit.data.readers.grib.index.sql import FieldListInFilesWithSqlIndex
 from earthkit.data.readers.grib.parsing import GribIndexingPathParserIterator
 from earthkit.data.sources.indexed import IndexedSource
 
 LOG = logging.getLogger(__name__)
 
 
 def make_absolute(filename, root_dir, default):
@@ -27,15 +27,15 @@
     LOG.debug(f"Transforming {filename} into absolute path {absolute}")
     return absolute
 
 
 class FileIndexedSource(IndexedSource):
     DEFAULT_JSON_FILE = "earthkit.index"
     DEFAULT_DB_FILE = "earthkit.db"
-    INDEX_CLASS = FieldsetInFilesWithSqlIndex
+    INDEX_CLASS = FieldListInFilesWithSqlIndex
 
     def __init__(
         self,
         path,
         db_path=None,
         index_file=None,
         _index=None,
```

### Comparing `earthkit-data-0.1.2/earthkit/data/sources/file_pattern.py` & `earthkit-data-0.1.3/earthkit/data/sources/file_pattern.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/sources/indexed.py` & `earthkit-data-0.1.3/earthkit/data/sources/indexed.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/sources/list_of_dicts.py` & `earthkit-data-0.1.3/earthkit/data/sources/list_of_dicts.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 #
 
 import datetime
 import logging
 
-from earthkit.data.readers.grib.index import FieldSet
+from earthkit.data.readers.grib.index import FieldList
 
 LOG = logging.getLogger(__name__)
 
 
 class VirtualGribField(dict):
     KEY_TYPES = {
         "s": str,
@@ -119,15 +119,15 @@
     def _attributes(self, names):
         result = {}
         for name in names:
             result[name] = self._get(name)
         return result
 
 
-class GribFromDicts(FieldSet):
+class GribFromDicts(FieldList):
     def __init__(self, list_of_dicts, *args, **kwargs):
         self.list_of_dicts = list_of_dicts
         super().__init__(*args, **kwargs)
 
     def __getitem__(self, n):
         return VirtualGribField(self.list_of_dicts[n])
```

### Comparing `earthkit-data-0.1.2/earthkit/data/sources/memory.py` & `earthkit-data-0.1.3/earthkit/data/sources/memory.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/sources/multi.py` & `earthkit-data-0.1.3/earthkit/data/sources/multi.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/sources/multi_url.py` & `earthkit-data-0.1.3/earthkit/data/sources/multi_url.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/sources/stream.py` & `earthkit-data-0.1.3/earthkit/data/sources/stream.py`

 * *Files 24% similar despite different names*

```diff
@@ -23,40 +23,40 @@
         self._reader = reader
 
     def __iter__(self):
         return iter(self._reader)
 
 
 class StreamSource(Source):
-    def __init__(self, stream, group_by=1, **kwargs):
+    def __init__(self, stream, batch_size=1, **kwargs):
         super().__init__(**kwargs)
         self._stream = stream
         self._reader_ = None
-        self._group_by = group_by
+        self._batch_size = batch_size
 
     @property
-    def group_by(self):
-        return self._group_by
+    def batch_size(self):
+        return self._batch_size
 
     def mutate(self):
-        if self.group_by == 0:
+        if self.batch_size == 0:
             source = StreamMemorySource(self._reader)
             return source
         else:
             return self
 
     def __iter__(self):
         return self
 
     def __next__(self):
-        assert self.group_by > 0
-        if self.group_by == 1:
+        assert self.batch_size > 0
+        if self.batch_size == 1:
             return self._reader.__next__()
         else:
-            return self._reader.read_group(self.group_by)
+            return self._reader.read_batch(self.batch_size)
 
     @property
     def _reader(self):
         if self._reader_ is None:
             self._reader_ = stream_reader(self, self._stream)
             self._stream = None
         return self._reader_
```

### Comparing `earthkit-data-0.1.2/earthkit/data/sources/url.py` & `earthkit-data-0.1.3/earthkit/data/sources/url.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/sources/url_pattern.py` & `earthkit-data-0.1.3/earthkit/data/sources/url_pattern.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/sources/virtual.py` & `earthkit-data-0.1.3/earthkit/data/sources/virtual.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import calendar
 import datetime
 import logging
 import threading
 
 import earthkit.data as cml
-from earthkit.data.readers.grib.index import FieldSet
+from earthkit.data.readers.grib.index import FieldList
 from earthkit.data.utils.serialise import register_serialisation
 
 LOG = logging.getLogger(__name__)
 
 
 class NoLock:
     def __enter__(self):
@@ -67,15 +67,15 @@
         try:
             return super().__getitem__(key)
         except KeyError:
             self[key] = self.field[key]
             return self[key]
 
 
-class Virtual(FieldSet):
+class Virtual(FieldList):
     SIZE = int(365.25 * 24 * (2022 - 1959))
     # SIZE = 100
 
     def __init__(self, **kwargs):
         super().__init__()
         self.request = dict(
             dataset="reanalysis-era5-single-levels",
```

### Comparing `earthkit-data-0.1.2/earthkit/data/sources/virtual_directory.py` & `earthkit-data-0.1.3/earthkit/data/sources/virtual_directory.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 #
 import logging
 import warnings
 from collections import defaultdict
 
-from earthkit.data.readers.grib.index import FieldsetInFilesWithSqlIndex
+from earthkit.data.readers.grib.index import FieldListInFilesWithSqlIndex
 from earthkit.data.sources.directory import DirectorySource
 from earthkit.data.utils import progress_bar
 
 LOG = logging.getLogger(__name__)
 
 USE_REFERENCE = [
     "distinctLatitudes",
@@ -133,15 +133,15 @@
     def shape(self):
         return self.owner.reference[0].shape
 
     def __str__(self):
         return "Virt" + str(self.real_item)
 
 
-class VirtualFieldsetInFilesWithSqlIndex(FieldsetInFilesWithSqlIndex):
+class VirtualFieldListInFilesWithSqlIndex(FieldListInFilesWithSqlIndex):
     # DEBUG = True
     DEBUG = False
 
     def __init__(self, *args, **kwargs):
         self._reference = None
         self.pbar = None
         super().__init__(*args, **kwargs)
@@ -222,11 +222,11 @@
         if r != i:
             raise Exception(
                 f"Error for field={item.i}, key={key}: reference={r}, item={i}"
             )
 
 
 class VirtualDirectorySource(DirectorySource):
-    INDEX_CLASS = VirtualFieldsetInFilesWithSqlIndex
+    INDEX_CLASS = VirtualFieldListInFilesWithSqlIndex
 
 
 source = VirtualDirectorySource
```

### Comparing `earthkit-data-0.1.2/earthkit/data/testing.py` & `earthkit-data-0.1.3/earthkit/data/testing.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 class OfflineError(Exception):
     pass
 
 
 _NETWORK_PATCHER = patch("socket.socket", side_effect=OfflineError)
 
-_REMOTE_TEST_DATA_URL = "https://get.ecmwf.int/repository/test-data/emohawk/"
+_REMOTE_TEST_DATA_URL = "https://get.ecmwf.int/repository/test-data/earthkit-data/"
 
 _ROOT_DIR = top = os.path.dirname(os.path.dirname(os.path.dirname(__file__)))
 
 
 @contextmanager
 def network_off():
     try:
```

### Comparing `earthkit-data-0.1.2/earthkit/data/utils/__init__.py` & `earthkit-data-0.1.3/earthkit/data/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/utils/availability.py` & `earthkit-data-0.1.3/earthkit/data/utils/availability.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/utils/bbox.py` & `earthkit-data-0.1.3/earthkit/data/utils/bbox.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/utils/conventions.py` & `earthkit-data-0.1.3/earthkit/data/utils/conventions.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/utils/dates.py` & `earthkit-data-0.1.3/earthkit/data/utils/dates.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/utils/factorise.py` & `earthkit-data-0.1.3/earthkit/data/utils/factorise.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/utils/html.py` & `earthkit-data-0.1.3/earthkit/data/utils/html.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/utils/humanize.py` & `earthkit-data-0.1.3/earthkit/data/utils/humanize.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/utils/kwargs.py` & `earthkit-data-0.1.3/earthkit/data/utils/kwargs.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/utils/lazy.py` & `earthkit-data-0.1.3/earthkit/data/utils/lazy.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/utils/parts.py` & `earthkit-data-0.1.3/earthkit/data/utils/parts.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/utils/patterns.py` & `earthkit-data-0.1.3/earthkit/data/utils/patterns.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/utils/serialise.py` & `earthkit-data-0.1.3/earthkit/data/utils/serialise.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/utils/summary.py` & `earthkit-data-0.1.3/earthkit/data/utils/summary.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/vocabularies/__init__.py` & `earthkit-data-0.1.3/earthkit/data/vocabularies/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 import itertools
 import logging
 
 from earthkit.data.utils.humanize import did_you_mean
 
 LOG = logging.getLogger(__name__)
 
-
 SYNONYMS = (
     (("mars", "2t"), ("cf", "t2m")),
     (("mars", "ci"), ("cf", "siconc")),
 )
 
 VOCABULARIES = {}
 
@@ -83,16 +82,16 @@
             word,
             itertools.chain(
                 self.words,
                 self.aliases.keys(),
             ),
         )
         if correction is not None:
-            LOG.warning(
-                "Cannot find '%s' in %s vocabulary, did you mean '%s'?",
+            LOG.debug(
+                "This warning can be safely ignored: Cannot find '%s' in %s vocabulary, did you mean '%s'?",
                 word,
                 self.name,
                 correction,
             )
 
         return word
```

### Comparing `earthkit-data-0.1.2/earthkit/data/vocabularies/aliases.py` & `earthkit-data-0.1.3/earthkit/data/vocabularies/aliases.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/vocabularies/cf.py` & `earthkit-data-0.1.3/earthkit/data/vocabularies/cf.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/vocabularies/grib-paramid.csv` & `earthkit-data-0.1.3/earthkit/data/vocabularies/grib-paramid.csv`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/vocabularies/grib.py` & `earthkit-data-0.1.3/earthkit/data/vocabularies/grib.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/wrappers/__init__.py` & `earthkit-data-0.1.3/earthkit/data/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit/data/wrappers/string.py` & `earthkit-data-0.1.3/earthkit/data/wrappers/string.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/earthkit_data.egg-info/PKG-INFO` & `earthkit-data-0.1.3/earthkit_data.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,62 @@
 Metadata-Version: 2.1
 Name: earthkit-data
-Version: 0.1.2
+Version: 0.1.3
 Summary: A format-agnostic Python interface for geospatial data
 License: Apache License 2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # earthkit-data
 
+![earthkit-data](https://raw.githubusercontent.com/ecmwf/earthkit-data/develop/earthkit-data.png)
+
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/earthkit-data.svg)](https://pypi.python.org/pypi/earthkit-data/)
 
 A format-agnostic interface for geospatial data with a focus on meteorology and
 climate science.
 
 **DISCLAIMER**
 This project is **BETA** and will be **Experimental** for the foreseeable future.
 Interfaces and functionality are likely to change, and the project itself may be scrapped.
 **DO NOT** use this software in any project/software that is operational.
 
+## Documentation
+
 The documentation can be found at https://earthkit-data.readthedocs.io/.
 
+## Install
+
+Install via `pip` with:
+
+```
+$ pip install earthkit-data
+```
+
+More details, such as how to install any necessary binaries, can be found  at https://earthkit-data.readthedocs.io/en/latest/install.html.
+
+Alternatively, install via `conda` with:
+
+```
+$ conda install earthkit-data -c conda-forge
+```
+
+This will bring in some necessary binary dependencies for you.
+
 ## License
 
 ```
 Copyright 2022, European Centre for Medium Range Weather Forecasts.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
```

### Comparing `earthkit-data-0.1.2/earthkit_data.egg-info/SOURCES.txt` & `earthkit-data-0.1.3/earthkit_data.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,55 +1,76 @@
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yml
 LICENSE
 Makefile
 README.md
+earthkit-data.png
 environment.yml
 pyproject.toml
 pytest.ini
 setup.cfg
 .github/workflows/ci.yml
 .github/workflows/label-public-pr.yml
 .github/workflows/notify_new_issue.yml
 .github/workflows/notify_new_pr.yml
 docs/Makefile
+docs/api.rst
 docs/conf.py
-docs/contributing.rst
+docs/development.rst
 docs/examples.rst
 docs/index.rst
 docs/install.rst
 docs/licence.rst
 docs/make.bat
 docs/requirements.txt
 docs/_static/.gitkeep
 docs/_static/style.css
 docs/_templates/.gitkeep
+docs/examples/Untitled.ipynb
 docs/examples/bufr.ipynb
-docs/examples/grib_fdb_stream.ipynb
+docs/examples/cds.ipynb
+docs/examples/fdb.ipynb
 docs/examples/grib_file_pattern.ipynb
 docs/examples/grib_from_stream.ipynb
 docs/examples/grib_indexing.ipynb
 docs/examples/grib_metadata.ipynb
 docs/examples/grib_missing.ipynb
 docs/examples/grib_multi.ipynb
 docs/examples/grib_overview.ipynb
 docs/examples/grib_selection.ipynb
 docs/examples/grib_tar.ipynb
 docs/examples/grib_to_netcdf.ipynb
 docs/examples/grib_url.ipynb
 docs/examples/list_of_dict.ipynb
+docs/examples/mars.ipynb
 docs/examples/missing.grib
 docs/examples/netcdf.ipynb
+docs/examples/odb.ipynb
 docs/examples/temp_10.bufr
 docs/examples/test.grib
 docs/examples/test.nc
+docs/examples/test.odb
 docs/examples/test4.grib
 docs/examples/test6.grib
 docs/examples/tuv_pl.grib
+docs/guide/caching.rst
+docs/guide/data.rst
+docs/guide/index.rst
+docs/guide/settings.rst
+docs/guide/sources.rst
+docs/guide/data_format/bufr.rst
+docs/guide/data_format/csv.rst
+docs/guide/data_format/grib.rst
+docs/guide/data_format/index.rst
+docs/guide/data_format/netcdf.rst
+docs/guide/data_format/odb.rst
+docs/guide/include/settings-1-get.py
+docs/guide/include/settings-2-set.py
+docs/guide/include/settings-3-reset.py
 earthkit/data/__init__.py
 earthkit/data/decorators.py
 earthkit/data/input_manager.py
 earthkit/data/testing.py
 earthkit/data/version.py
 earthkit/data/arguments/__init__.py
 earthkit/data/arguments/args_kwargs.py
@@ -91,43 +112,52 @@
 earthkit/data/readers/odb.py
 earthkit/data/readers/tar.py
 earthkit/data/readers/text.py
 earthkit/data/readers/unknown.py
 earthkit/data/readers/zip.py
 earthkit/data/readers/grib/__init__.py
 earthkit/data/readers/grib/codes.py
-earthkit/data/readers/grib/fieldset.py
+earthkit/data/readers/grib/fieldlist.py
 earthkit/data/readers/grib/memory.py
+earthkit/data/readers/grib/output.py
 earthkit/data/readers/grib/pandas.py
 earthkit/data/readers/grib/parsing.py
 earthkit/data/readers/grib/reader.py
 earthkit/data/readers/grib/xarray.py
 earthkit/data/readers/grib/index/__init__.py
 earthkit/data/readers/grib/index/db.py
 earthkit/data/readers/grib/index/file.py
 earthkit/data/readers/grib/index/json.py
 earthkit/data/readers/grib/index/sql.py
 earthkit/data/sources/__init__.py
+earthkit/data/sources/cds.py
 earthkit/data/sources/dummy.grib
 earthkit/data/sources/dummy_source.py
+earthkit/data/sources/ecmwf_api.py
 earthkit/data/sources/empty.py
 earthkit/data/sources/fdb.py
 earthkit/data/sources/file.py
 earthkit/data/sources/file_indexed.py
 earthkit/data/sources/file_pattern.py
 earthkit/data/sources/indexed.py
 earthkit/data/sources/list_of_dicts.py
+earthkit/data/sources/mars.py
 earthkit/data/sources/memory.py
 earthkit/data/sources/multi.py
 earthkit/data/sources/multi_url.py
+earthkit/data/sources/prompt.py
 earthkit/data/sources/stream.py
 earthkit/data/sources/url.py
 earthkit/data/sources/url_pattern.py
 earthkit/data/sources/virtual.py
 earthkit/data/sources/virtual_directory.py
+earthkit/data/sphinxext/__init__.py
+earthkit/data/sphinxext/generate_settings_rst.py
+earthkit/data/sphinxext/module_output.py
+earthkit/data/sphinxext/xref.py
 earthkit/data/utils/__init__.py
 earthkit/data/utils/availability.py
 earthkit/data/utils/bbox.py
 earthkit/data/utils/conventions.py
 earthkit/data/utils/dates.py
 earthkit/data/utils/factorise.py
 earthkit/data/utils/html.py
@@ -140,20 +170,22 @@
 earthkit/data/utils/summary.py
 earthkit/data/vocabularies/__init__.py
 earthkit/data/vocabularies/aliases.py
 earthkit/data/vocabularies/cf.py
 earthkit/data/vocabularies/grib-paramid.csv
 earthkit/data/vocabularies/grib.py
 earthkit/data/wrappers/__init__.py
+earthkit/data/wrappers/integer.py
 earthkit/data/wrappers/string.py
 earthkit_data.egg-info/PKG-INFO
 earthkit_data.egg-info/SOURCES.txt
 earthkit_data.egg-info/dependency_links.txt
 earthkit_data.egg-info/requires.txt
 earthkit_data.egg-info/top_level.txt
+tests/conftest.py
 tests/test_00_version.py
 tests/bufr/test_bufr_summary.py
 tests/core/test_cache.py
 tests/core/test_version.py
 tests/data/mercator.grib
 tests/data/ml_data.grib
 tests/data/rgg_small_subarea_cellarea_ref.grib
@@ -163,32 +195,37 @@
 tests/data/test_single.grib
 tests/data/test_single.nc
 tests/data/test_single_with_missing.grib
 tests/data/u_pl.grib
 tests/data/v_pl.grib
 tests/documentation/test_examples.py
 tests/documentation/test_notebooks.py
+tests/grib/test_grib_concat.py
 tests/grib/test_grib_contents.py
 tests/grib/test_grib_convert.py
 tests/grib/test_grib_order_by.py
+tests/grib/test_grib_output.py
 tests/grib/test_grib_sel.py
 tests/grib/test_grib_slice.py
 tests/grib/test_grib_summary.py
 tests/indexing/indexing_fixtures.py
 tests/indexing/test_indexing_db.py
 tests/indexing/test_indexing_isel.py
 tests/indexing/test_indexing_order_by.py
 tests/indexing/test_indexing_serialisation.py
 tests/indexing/test_order_kwargs.py
 tests/indexing/test_selection_kwargs.py
 tests/readers/test_csv_reader.py
 tests/readers/test_grib_reader.py
 tests/readers/test_netcdf_reader.py
+tests/readers/test_odb_reader.py
 tests/readers/test_tar_reader.py
 tests/readers/test_unknown_reader.py
 tests/readers/test_zip_reader.py
 tests/readers/unknown_file.unknown_ext
 tests/readers/unknown_text_file.unknown_ext
+tests/sources/test_cds.py
 tests/sources/test_file.py
+tests/sources/test_mars.py
 tests/sources/test_multi.py
 tests/sources/test_url.py
 tests/sources/test_url_pattern.py
```

### Comparing `earthkit-data-0.1.2/setup.cfg` & `earthkit-data-0.1.3/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Scientific/Engineering
 long_description_content_type = text/markdown
 long_description = file: README.md
 test_suite = tests
 
 [options]
 packages = find_namespace:
@@ -24,14 +25,15 @@
 	dask
 	entrypoints
 	filelock
 	jinja2
 	multiurl
 	netcdf4
 	pdbufr
+	pyfdb
 	pyodc
 	pyyaml
 	tqdm
 	xarray>=0.19.0
 
 [options.packages.find]
 include = earthkit.*
```

### Comparing `earthkit-data-0.1.2/tests/bufr/test_bufr_summary.py` & `earthkit-data-0.1.3/tests/bufr/test_bufr_summary.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/tests/core/test_cache.py` & `earthkit-data-0.1.3/tests/core/test_cache.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/tests/core/test_version.py` & `earthkit-data-0.1.3/tests/core/test_version.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/tests/data/mercator.grib` & `earthkit-data-0.1.3/tests/data/mercator.grib`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/tests/data/ml_data.grib` & `earthkit-data-0.1.3/tests/data/ml_data.grib`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/tests/data/rgg_small_subarea_cellarea_ref.grib` & `earthkit-data-0.1.3/tests/data/rgg_small_subarea_cellarea_ref.grib`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/tests/data/t_pl.grib` & `earthkit-data-0.1.3/tests/data/t_pl.grib`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/tests/data/t_time_series.grib` & `earthkit-data-0.1.3/tests/data/t_time_series.grib`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/tests/data/test_icon.grib` & `earthkit-data-0.1.3/tests/data/test_icon.grib`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/tests/data/test_single.nc` & `earthkit-data-0.1.3/tests/data/test_single.nc`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/tests/data/u_pl.grib` & `earthkit-data-0.1.3/tests/data/u_pl.grib`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/tests/data/v_pl.grib` & `earthkit-data-0.1.3/tests/data/v_pl.grib`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/tests/documentation/test_examples.py` & `earthkit-data-0.1.3/tests/documentation/test_examples.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 IGNORE = [
     "conf.py",
     "xml2rst.py",
     "actions.py",
     "generate-examples-maps.py",
     "settings-2-set.py",
+    "xref.py",
 ]
 
 EXAMPLES = earthkit_file("docs")
 
 
 def example_list():
     examples = []
```

### Comparing `earthkit-data-0.1.2/tests/documentation/test_notebooks.py` & `earthkit-data-0.1.3/tests/documentation/test_notebooks.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from earthkit.data.testing import MISSING, earthkit_file
 
 # See https://www.blog.pythonlibrary.org/2018/10/16/testing-jupyter-notebooks/
 
 
 EXAMPLES = earthkit_file("docs", "examples")
 
-SKIP = "grib_fdb_stream.ipynb"
+SKIP = ["fdb.ipynb", "mars.ipynb", "cds.ipynb"]
 
 
 def notebooks_list():
     notebooks = []
     for path in os.listdir(EXAMPLES):
         if re.match(r".+\.ipynb$", path):
             # if re.match(r"^\d\d-.*\.ipynb$", path):
```

### Comparing `earthkit-data-0.1.2/tests/grib/test_grib_contents.py` & `earthkit-data-0.1.3/tests/grib/test_grib_contents.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,17 +37,21 @@
         ("shortName:s", "2t"),
         ("shortName:str", "2t"),
         ("centre", "ecmf"),
         ("centre:l", 98),
         ("level", 0),
         ("level:l", 0),
         ("level:int", 0),
+        (["shortName"], ["2t"]),
+        (["shortName", "level"], ["2t", 0]),
+        (("shortName"), "2t"),
+        (("shortName", "level"), ("2t", 0)),
     ],
 )
-def test_metadata_get_1(key, expected_value):
+def test_grib_metadata_grib(key, expected_value):
     f = from_source("file", earthkit_test_data_file("test_single.grib"))
     sn = f.metadata(key)
     assert sn == [expected_value]
     sn = f[0].metadata(key)
     assert sn == expected_value
 
 
@@ -285,59 +289,80 @@
     assert np.isclose(v[0][1], 2.0003650188446045, eps)
     assert np.isclose(v[0][20], 316.4207458496094, eps)
     assert np.isclose(v[17][1], 2.0003650188446045, eps)
     assert np.isclose(v[17][20], 316.4207458496094, eps)
 
 
 def test_grib_metadata_generic():
-    f = from_source("file", earthkit_examples_file("tuv_pl.grib"))
-    f = f.sel(count=[1, 2, 3, 4])
+    f = from_source("file", earthkit_examples_file("tuv_pl.grib"))[0:4]
 
-    sn = f.metadata(["shortName"])
+    sn = f.metadata("shortName")
     assert sn == ["t", "u", "v", "t"]
-    cs = f.metadata(["centre:s"])
+    sn = f.metadata(["shortName"])
+    assert sn == [["t"], ["u"], ["v"], ["t"]]
+    cs = f.metadata("centre:s")
     assert cs == ["ecmf", "ecmf", "ecmf", "ecmf"]
-    cl = f.metadata(["centre:l"])
+    cl = f.metadata("centre:l")
     assert cl == [98, 98, 98, 98]
     lg = f.metadata(["level:d", "cfVarName"])
-    assert lg == [(1000, "t"), (1000, "u"), (1000, "v"), (850, "t")]
+    assert lg == [[1000, "t"], [1000, "u"], [1000, "v"], [850, "t"]]
     lg = f.metadata("level", "cfVarName")
     assert lg == [(1000, "t"), (1000, "u"), (1000, "v"), (850, "t")]
 
     # astype
     cs = f.metadata("centre", astype=None)
     assert cs == ["ecmf", "ecmf", "ecmf", "ecmf"]
     cs = f.metadata("centre", astype=str)
     assert cs == ["ecmf", "ecmf", "ecmf", "ecmf"]
     cl = f.metadata("centre", astype=int)
     assert cl == [98, 98, 98, 98]
     lg = f.metadata(["level", "cfVarName"], astype=(int, None))
-    assert lg == [(1000, "t"), (1000, "u"), (1000, "v"), (850, "t")]
+    assert lg == [[1000, "t"], [1000, "u"], [1000, "v"], [850, "t"]]
     lg = f.metadata(["level", "cfVarName"], astype=str)
-    assert lg == [("1000", "t"), ("1000", "u"), ("1000", "v"), ("850", "t")]
+    assert lg == [["1000", "t"], ["1000", "u"], ["1000", "v"], ["850", "t"]]
 
     # non matching astype
     with pytest.raises(ValueError):
         f.metadata(["level", "cfVarName", "centre"], astype=(int, None))
 
     # lgk = f.metadata(["level:d", "cfVarName"], "key")
     # assert lgk == [[1000, 1000, 1000, 850], ["t", "u", "v", "t"]]
     # with pytest.raises(ValueError):
     #     lgk = f.metadata(["level:d", "cfVarName"], "invalid")
 
     # single fieldlist
     f = from_source("file", earthkit_examples_file("tuv_pl.grib"))
     f = f.sel(count=[1])
     lg = f.metadata(["level", "cfVarName"])
-    assert lg == [(1000, "t")]
+    assert lg == [[1000, "t"]]
 
     # single field
     f = from_source("file", earthkit_examples_file("tuv_pl.grib"))[0]
     lg = f.metadata(["level", "cfVarName"])
-    assert lg == (1000, "t")
+    assert lg == [1000, "t"]
+
+
+def test_grib_metadata_missing_value():
+    f = from_source("file", earthkit_test_data_file("ml_data.grib"))
+
+    with pytest.raises(KeyError):
+        f[0].metadata("scaleFactorOfSecondFixedSurface")
+
+    v = f[0].metadata("scaleFactorOfSecondFixedSurface", default=None)
+    assert v is None
+
+
+def test_grib_metadata_missing_key():
+    f = from_source("file", earthkit_examples_file("test.grib"))
+
+    with pytest.raises(KeyError):
+        f[0].metadata("_badkey_")
+
+    v = f[0].metadata("__badkey__", default=0)
+    assert v == 0
 
 
 def test_grib_metadata_namespace():
     f = from_source("file", earthkit_examples_file("test6.grib"))
 
     r = f[0].metadata(namespace="vertical")
     ref = {"level": 1000, "typeOfLevel": "isobaricInhPa"}
@@ -358,15 +383,15 @@
             "validityTime": 1200,
         },
     }
     assert r == ref
 
     r = f[0].metadata()
     assert isinstance(r, dict)
-    for ns in ["", "vertical", "time"]:
+    for ns in ["default", "vertical", "time"]:
         assert ns in r, ns
 
 
 def test_grib_values_1():
     f = from_source("file", earthkit_test_data_file("test_single.grib"))
 
     eps = 1e-5
@@ -534,14 +559,36 @@
     assert v1.shape == expected_shape
     vr = v1[0].flatten()
     assert np.allclose(vf0, vr, eps)
     vr = v1[15].flatten()
     assert np.allclose(vf15, vr, eps)
 
 
+@pytest.mark.parametrize("dtype", [np.float32, np.float64])
+def test_grib_to_numpy_1_dtype(dtype):
+    f = from_source("file", earthkit_test_data_file("test_single.grib"))
+
+    v = f[0].to_numpy(dtype=dtype)
+    assert v.dtype == dtype
+
+    v = f.to_numpy(dtype=dtype)
+    assert v.dtype == dtype
+
+
+@pytest.mark.parametrize("dtype", [np.float32, np.float64])
+def test_grib_to_numpy_18_dtype(dtype):
+    f = from_source("file", earthkit_examples_file("tuv_pl.grib"))
+
+    v = f[0].to_numpy(dtype=dtype)
+    assert v.dtype == dtype
+
+    v = f.to_numpy(dtype=dtype)
+    assert v.dtype == dtype
+
+
 def test_grib_values_with_missing():
     f = from_source("file", earthkit_test_data_file("test_single_with_missing.grib"))
 
     v = f[0].values
     assert isinstance(v, np.ndarray)
     assert v.shape == (84,)
     eps = 0.001
@@ -555,15 +602,15 @@
     assert np.count_nonzero(np.isnan(m)) == 38
 
 
 def test_grib_to_points_1():
     f = from_source("file", earthkit_test_data_file("test_single.grib"))
 
     eps = 1e-5
-    v = f[0].to_points()
+    v = f[0].to_points(flatten=True)
     assert isinstance(v, dict)
     assert isinstance(v["lon"], np.ndarray)
     assert isinstance(v["lat"], np.ndarray)
     check_array(
         v["lon"],
         (84,),
         first=0.0,
@@ -580,15 +627,15 @@
         eps=eps,
     )
 
 
 def test_grib_to_points_1_shape():
     f = from_source("file", earthkit_test_data_file("test_single.grib"))
 
-    v = f[0].to_points(flatten=False)
+    v = f[0].to_points()
     assert isinstance(v, dict)
     assert isinstance(v["lon"], np.ndarray)
     assert isinstance(v["lat"], np.ndarray)
 
     # x
     assert v["lon"].shape == (7, 12)
     for x in v["lon"]:
@@ -697,15 +744,15 @@
         for f in fs:
             i += 1
         assert i == 0
 
 
 def test_grib_from_stream_multi_group():
     with open(earthkit_examples_file("test6.grib"), "rb") as stream:
-        fs = from_source("stream", stream, group_by=2)
+        fs = from_source("stream", stream, batch_size=2)
 
         # no methods are available
         with pytest.raises(TypeError):
             len(fs)
 
         ref = [["t", "u"], ["v", "t"], ["u", "v"]]
         for i, f in enumerate(fs):
@@ -717,15 +764,15 @@
         for f in fs:
             i += 1
         assert i == 0
 
 
 def test_grib_from_stream_in_memory():
     with open(earthkit_examples_file("test6.grib"), "rb") as stream:
-        fs = from_source("stream", stream, group_by=0)
+        fs = from_source("stream", stream, batch_size=0)
 
         assert len(fs) == 6
 
         ref = ["t", "u", "v", "t", "u", "v"]
         val = []
 
         # iteration
@@ -758,15 +805,15 @@
             fs.save(tmp)
             fs_saved = from_source("file", tmp)
             assert len(fs) == len(fs_saved)
 
 
 def test_grib_save_when_loaded_from_stream():
     with open(earthkit_examples_file("test6.grib"), "rb") as stream:
-        fs = from_source("stream", stream, group_by=0)
+        fs = from_source("stream", stream, batch_size=0)
         assert len(fs) == 6
         with temp_file() as tmp:
             fs.save(tmp)
             fs_saved = from_source("file", tmp)
             assert len(fs) == len(fs_saved)
```

### Comparing `earthkit-data-0.1.2/tests/grib/test_grib_convert.py` & `earthkit-data-0.1.3/tests/grib/test_grib_convert.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/tests/grib/test_grib_order_by.py` & `earthkit-data-0.1.3/tests/grib/test_grib_order_by.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/tests/grib/test_grib_sel.py` & `earthkit-data-0.1.3/tests/grib/test_grib_sel.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,33 +24,33 @@
     assert len(r) == 1
     assert r[0].metadata("shortName") == "2t"
 
 
 @pytest.mark.parametrize(
     "params,expected_meta,metadata_keys",
     [
-        (dict(shortName="u", level=700), [("u", 700)], []),
-        (dict(paramId=131, level=700), [(131, 700)], []),
+        (dict(shortName="u", level=700), [["u", 700]], []),
+        (dict(paramId=131, level=700), [[131, 700]], []),
         (
             dict(shortName=["t", "u"], level=[700, 500]),
             [
-                ("t", 700),
-                ("u", 700),
-                ("t", 500),
-                ("u", 500),
+                ["t", 700],
+                ["u", 700],
+                ["t", 500],
+                ["u", 500],
             ],
             ["shortName", "level:l"],
         ),
         (dict(shortName="w"), [], []),
         (dict(INVALIDKEY="w"), [], []),
         (
             dict(shortName=["t"], level=[500, 700], marsType="an"),
             [
-                ("t", 700, "an"),
-                ("t", 500, "an"),
+                ["t", 700, "an"],
+                ["t", 500, "an"],
             ],
             ["shortName", "level:l", "marsType"],
         ),
     ],
 )
 def test_grib_sel_single_file_1(params, expected_meta, metadata_keys):
     f = from_source("file", earthkit_file("docs/examples/tuv_pl.grib"))
@@ -68,46 +68,46 @@
 
 def test_grib_sel_single_file_2():
     f = from_source("file", earthkit_file("tests/data/t_time_series.grib"))
 
     g = f.sel(shortName=["t"], step=[3, 6])
     assert len(g) == 2
     assert g.metadata(["shortName", "level:l", "step:l"]) == [
-        ("t", 1000, 3),
-        ("t", 1000, 6),
+        ["t", 1000, 3],
+        ["t", 1000, 6],
     ]
 
     # repeated use
     g = f.sel(shortName=["t"], step=[3, 6])
     # g = f.sel(shortName=["t"], step=["3", "06"])
     assert len(g) == 2
     assert g.metadata(["shortName", "level:l", "step:l"]) == [
-        ("t", 1000, 3),
-        ("t", 1000, 6),
+        ["t", 1000, 3],
+        ["t", 1000, 6],
     ]
 
 
 def test_grib_sel_single_file_as_dict():
     f = from_source("file", earthkit_file("docs/examples/tuv_pl.grib"))
     g = f.sel({"shortName": "t", "level": [500, 700], "mars.type": "an"})
     assert len(g) == 2
     assert g.metadata(["shortName", "level:l", "mars.type"]) == [
-        ("t", 700, "an"),
-        ("t", 500, "an"),
+        ["t", 700, "an"],
+        ["t", 500, "an"],
     ]
 
 
 @pytest.mark.parametrize(
     "param_id,level,expected_meta",
     [
-        (131, (slice(600, 700)), [(131, 700)]),
-        (131, (slice(650, 750)), [(131, 700)]),
-        (131, (slice(1000, None)), [(131, 1000)]),
-        (131, (slice(None, 300)), [(131, 300)]),
-        (131, (slice(500, 700)), [(131, 700), (131, 500)]),
+        (131, (slice(600, 700)), [[131, 700]]),
+        (131, (slice(650, 750)), [[131, 700]]),
+        (131, (slice(1000, None)), [[131, 1000]]),
+        (131, (slice(None, 300)), [[131, 300]]),
+        (131, (slice(500, 700)), [[131, 700], [131, 500]]),
         (131, (slice(510, 520)), []),
     ],
 )
 def test_grib_sel_slice_single_file(param_id, level, expected_meta):
     f = from_source("file", earthkit_file("docs/examples/tuv_pl.grib"))
 
     g = f.sel(paramId=param_id, level=level)
@@ -120,46 +120,46 @@
     f1 = from_source("file", earthkit_file("docs/examples/tuv_pl.grib"))
     f2 = from_source("file", earthkit_file("tests/data/ml_data.grib"))
     f = from_source("multi", [f1, f2])
 
     # single resulting field
     g = f.sel(shortName="t", level=61)
     assert len(g) == 1
-    assert g.metadata(["shortName", "level:l", "typeOfLevel"]) == [("t", 61, "hybrid")]
+    assert g.metadata(["shortName", "level:l", "typeOfLevel"]) == [["t", 61, "hybrid"]]
 
     g1 = f[34]
     d = g.to_numpy() - g1.to_numpy()
     assert np.allclose(d, np.zeros(len(d)))
 
 
 def test_grib_sel_slice_multi_file():
     f1 = from_source("file", earthkit_file("docs/examples/tuv_pl.grib"))
     f2 = from_source("file", earthkit_file("tests/data/ml_data.grib"))
     f = from_source("multi", [f1, f2])
 
     g = f.sel(shortName="t", level=slice(56, 62))
     assert len(g) == 2
     assert g.metadata(["shortName", "level:l", "typeOfLevel"]) == [
-        ("t", 57, "hybrid"),
-        ("t", 61, "hybrid"),
+        ["t", 57, "hybrid"],
+        ["t", 61, "hybrid"],
     ]
 
 
 def test_grib_sel_date():
     # date and time
     f = from_source("file", earthkit_file("tests/data/t_time_series.grib"))
 
     g = f.sel(date=20201221, time=1200, step=9)
     # g = f.sel(date="20201221", time="12", step="9")
     assert len(g) == 2
 
     ref_keys = ["shortName", "date", "time", "step"]
     ref = [
-        ("t", 20201221, 1200, 9),
-        ("z", 20201221, 1200, 9),
+        ["t", 20201221, 1200, 9],
+        ["z", 20201221, 1200, 9],
     ]
 
     assert g.metadata(ref_keys) == ref
 
 
 def test_grib_isel_single_message():
     s = from_source("file", earthkit_file("tests/data/test_single.grib"))
@@ -168,42 +168,42 @@
     assert len(r) == 1
     assert r[0].metadata("shortName") == "2t"
 
 
 @pytest.mark.parametrize(
     "params,expected_meta,metadata_keys",
     [
-        (dict(shortName=1, level=2), [("u", 500)], []),
-        (dict(paramId=1, level=2), [(131, 500)], []),
+        (dict(shortName=1, level=2), [["u", 500]], []),
+        (dict(paramId=1, level=2), [[131, 500]], []),
         (
             dict(shortName=[0, 1], level=[2, 3]),
             [
-                ("t", 700),
-                ("u", 700),
-                ("t", 500),
-                ("u", 500),
+                ["t", 700],
+                ["u", 700],
+                ["t", 500],
+                ["u", 500],
             ],
             ["shortName", "level:l"],
         ),
         # (dict(shortName="w"), [], []),
         (dict(INVALIDKEY=0), [], []),
         (
             dict(shortName=[0], level=[3, 2], marsType=0),
             [
-                ("t", 700, "an"),
-                ("t", 500, "an"),
+                ["t", 700, "an"],
+                ["t", 500, "an"],
             ],
             ["shortName", "level:l", "marsType"],
         ),
         (
             dict(level=-1),
             [
-                ("t", 1000),
-                ("u", 1000),
-                ("v", 1000),
+                ["t", 1000],
+                ["u", 1000],
+                ["v", 1000],
             ],
             ["shortName", "level:l"],
         ),
     ],
 )
 def test_grib_isel_single_file(params, expected_meta, metadata_keys):
     f = from_source("file", earthkit_file("docs/examples/tuv_pl.grib"))
@@ -217,20 +217,20 @@
 
         assert g.metadata(keys) == expected_meta
 
 
 @pytest.mark.parametrize(
     "param_id,level,expected_meta",
     [
-        (1, (slice(2)), [(131, 400), (131, 300)]),
-        (1, (slice(None, 2)), [(131, 400), (131, 300)]),
-        (1, (slice(2, 3)), [(131, 500)]),
-        (1, (slice(2, 4)), [(131, 700), (131, 500)]),
-        (1, (slice(4, None)), [(131, 1000), (131, 850)]),
-        (1, (slice(None, None, 2)), [(131, 850), (131, 500), (131, 300)]),
+        (1, (slice(2)), [[131, 400], [131, 300]]),
+        (1, (slice(None, 2)), [[131, 400], [131, 300]]),
+        (1, (slice(2, 3)), [[131, 500]]),
+        (1, (slice(2, 4)), [[131, 700], [131, 500]]),
+        (1, (slice(4, None)), [[131, 1000], [131, 850]]),
+        (1, (slice(None, None, 2)), [[131, 850], [131, 500], [131, 300]]),
     ],
 )
 def test_grib_isel_slice_single_file(param_id, level, expected_meta):
     f = from_source("file", earthkit_file("docs/examples/tuv_pl.grib"))
 
     g = f.isel(paramId=param_id, level=level)
     assert len(g) == len(expected_meta)
@@ -252,31 +252,31 @@
     f1 = from_source("file", earthkit_file("docs/examples/tuv_pl.grib"))
     f2 = from_source("file", earthkit_file("tests/data/ml_data.grib"))
     f = from_source("multi", [f1, f2])
 
     # single resulting field
     g = f.isel(shortName=1, level=21)
     assert len(g) == 1
-    assert g.metadata(["shortName", "level:l", "typeOfLevel"]) == [("t", 85, "hybrid")]
+    assert g.metadata(["shortName", "level:l", "typeOfLevel"]) == [["t", 85, "hybrid"]]
 
     g1 = f[40]
     d = g.to_numpy() - g1.to_numpy()
     assert np.allclose(d, np.zeros(len(d)))
 
 
 def test_grib_isel_slice_multi_file():
     f1 = from_source("file", earthkit_file("docs/examples/tuv_pl.grib"))
     f2 = from_source("file", earthkit_file("tests/data/ml_data.grib"))
     f = from_source("multi", [f1, f2])
 
     g = f.isel(shortName=1, level=slice(20, 22))
     assert len(g) == 2
     assert g.metadata(["shortName", "level:l", "typeOfLevel"]) == [
-        ("t", 81, "hybrid"),
-        ("t", 85, "hybrid"),
+        ["t", 81, "hybrid"],
+        ["t", 85, "hybrid"],
     ]
 
 
 if __name__ == "__main__":
     from earthkit.data.testing import main
 
     main()
```

### Comparing `earthkit-data-0.1.2/tests/grib/test_grib_slice.py` & `earthkit-data-0.1.3/tests/grib/test_grib_slice.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 from earthkit.data import from_source
 from earthkit.data.testing import earthkit_examples_file
 
 
 @pytest.mark.parametrize(
     "index,expected_meta",
     [
-        (0, ("t", 1000)),
-        (2, ("v", 1000)),
-        (17, ("v", 300)),
-        (-1, ("v", 300)),
-        (-5, ("u", 400)),
+        (0, ["t", 1000]),
+        (2, ["v", 1000]),
+        (17, ["v", 300]),
+        (-1, ["v", 300]),
+        (-5, ["u", 400]),
     ],
 )
 def test_grib_single_index(index, expected_meta):
     f = from_source("file", earthkit_examples_file("tuv_pl.grib"))
 
     r = f[index]
     assert r.metadata(["shortName", "level"]) == expected_meta
@@ -43,54 +43,54 @@
     with pytest.raises(IndexError):
         f[27]
 
 
 @pytest.mark.parametrize(
     "indexes,expected_meta",
     [
-        (slice(0, 4), [("t", 1000), ("u", 1000), ("v", 1000), ("t", 850)]),
-        (slice(None, 4), [("t", 1000), ("u", 1000), ("v", 1000), ("t", 850)]),
-        (slice(2, 9, 2), [("v", 1000), ("u", 850), ("t", 700), ("v", 700)]),
-        (slice(8, 1, -2), [("v", 700), ("t", 700), ("u", 850), ("v", 1000)]),
-        (slice(14, 18), [("v", 400), ("t", 300), ("u", 300), ("v", 300)]),
-        (slice(14, None), [("v", 400), ("t", 300), ("u", 300), ("v", 300)]),
+        (slice(0, 4), [["t", 1000], ["u", 1000], ["v", 1000], ["t", 850]]),
+        (slice(None, 4), [["t", 1000], ["u", 1000], ["v", 1000], ["t", 850]]),
+        (slice(2, 9, 2), [["v", 1000], ["u", 850], ["t", 700], ["v", 700]]),
+        (slice(8, 1, -2), [["v", 700], ["t", 700], ["u", 850], ["v", 1000]]),
+        (slice(14, 18), [["v", 400], ["t", 300], ["u", 300], ["v", 300]]),
+        (slice(14, None), [["v", 400], ["t", 300], ["u", 300], ["v", 300]]),
     ],
 )
 def test_grib_slice_single_file(indexes, expected_meta):
     f = from_source("file", earthkit_examples_file("tuv_pl.grib"))
     r = f[indexes]
     assert len(r) == 4
     assert r.metadata(["shortName", "level"]) == expected_meta
     v = r.values
     assert v.shape == (4, 84)
-    # check the original fieldset
+    # check the original fieldlist
     assert len(f) == 18
     assert f.metadata("shortName") == ["t", "u", "v"] * 6
 
 
 @pytest.mark.parametrize(
     "indexes,expected_meta",
     [
-        (slice(1, 4), [("msl", 0), ("t", 500), ("z", 500)]),
-        (slice(1, 6, 2), [("msl", 0), ("z", 500), ("z", 850)]),
-        (slice(5, 0, -2), [("z", 850), ("z", 500), ("msl", 0)]),
-        (slice(3, 6), [("z", 500), ("t", 850), ("z", 850)]),
+        (slice(1, 4), [["msl", 0], ["t", 500], ["z", 500]]),
+        (slice(1, 6, 2), [["msl", 0], ["z", 500], ["z", 850]]),
+        (slice(5, 0, -2), [["z", 850], ["z", 500], ["msl", 0]]),
+        (slice(3, 6), [["z", 500], ["t", 850], ["z", 850]]),
     ],
 )
 def test_grib_slice_multi_file(indexes, expected_meta):
     f = from_source(
         "file",
         [earthkit_examples_file("test.grib"), earthkit_examples_file("test4.grib")],
     )
     r = f[indexes]
     assert len(r) == 3
     assert r.metadata(["shortName", "level"]) == expected_meta
     # v = r.values
     # assert v.shape == (3, 84)
-    # check the original fieldset
+    # check the original fieldlist
     assert len(f) == 6
     assert f.metadata("shortName") == ["2t", "msl", "t", "z", "t", "z"]
 
 
 @pytest.mark.parametrize(
     "indexes1,indexes2",
     [(np.array([1, 16, 5, 9]), np.array([1, 3])), ([1, 16, 5, 9], [1, 3])],
@@ -109,57 +109,57 @@
 @pytest.mark.parametrize("indexes", [(np.array([1, 19, 5, 9])), ([1, 19, 5, 9])])
 def test_grib_array_indexing_bad(indexes):
     f = from_source("file", earthkit_examples_file("tuv_pl.grib"))
     with pytest.raises(IndexError):
         f[indexes]
 
 
-def test_grib_fieldset_iterator():
+def test_grib_fieldlist_iterator():
     g = from_source("file", earthkit_examples_file("tuv_pl.grib"))
     sn = g.metadata("shortName")
     assert len(sn) == 18
     iter_sn = [f["shortName"] for f in g]
     assert iter_sn == sn
     # repeated iteration
     iter_sn = [f["shortName"] for f in g]
     assert iter_sn == sn
 
 
-def test_fieldset_iterator_with_zip():
+def test_fieldlist_iterator_with_zip():
     # this tests something different with the iterator - this does not try to
-    # 'go off the edge' of the fieldset, because the length is determined by
+    # 'go off the edge' of the fieldlist, because the length is determined by
     # the list of levels
     g = from_source("file", earthkit_examples_file("tuv_pl.grib"))
     ref_levs = g.metadata("level")
     assert len(ref_levs) == 18
     levs1 = []
     levs2 = []
     for k, f in zip(g.metadata("level"), g):
         levs1.append(k)
         levs2.append(f.metadata("level"))
     assert levs1 == ref_levs
     assert levs2 == ref_levs
 
 
-def test_fieldset_iterator_with_zip_multiple():
-    # same as test_fieldset_iterator_with_zip() but multiple times
+def test_fieldlist_iterator_with_zip_multiple():
+    # same as test_fieldlist_iterator_with_zip() but multiple times
     g = from_source("file", earthkit_examples_file("tuv_pl.grib"))
     ref_levs = g.metadata("level")
     assert len(ref_levs) == 18
     for i in range(2):
         levs1 = []
         levs2 = []
         for k, f in zip(g.metadata("level"), g):
             levs1.append(k)
             levs2.append(f.metadata("level"))
         assert levs1 == ref_levs, i
         assert levs2 == ref_levs, i
 
 
-def test_fieldset_reverse_iterator():
+def test_fieldlist_reverse_iterator():
     g = from_source("file", earthkit_examples_file("tuv_pl.grib"))
     sn = g.metadata("shortName")
     sn_reversed = list(reversed(sn))
     assert sn_reversed[0] == "v"
     assert sn_reversed[17] == "t"
     gr = reversed(g)
     iter_sn = [f.metadata("shortName") for f in gr]
```

### Comparing `earthkit-data-0.1.2/tests/grib/test_grib_summary.py` & `earthkit-data-0.1.3/tests/grib/test_grib_summary.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/tests/indexing/indexing_fixtures.py` & `earthkit-data-0.1.3/tests/indexing/indexing_fixtures.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #
 
 import os
 import shutil
 import warnings
 
 from earthkit.data.core.temporary import temp_directory, temp_file
-from earthkit.data.readers.grib.index import FieldSet
+from earthkit.data.readers.grib.index import FieldList
 from earthkit.data.testing import (
     earthkit_examples_file,
     earthkit_file,
     earthkit_test_data_file,
 )
 
 TEST_GRIB_FILES = [
@@ -74,15 +74,15 @@
         {"param": "u", "levelist": 500, **prototype},
         {"param": "u", "levelist": 850, **prototype},
         {"param": "d", "levelist": 850, **prototype},
         {"param": "d", "levelist": 600, **prototype},
     ]
 
 
-class GribIndexFromDicts(FieldSet):
+class GribIndexFromDicts(FieldList):
     def __init__(self, list_of_dicts, *args, **kwargs):
         self.list_of_dicts = list_of_dicts
         print(f"KWARGS={kwargs}")
         super().__init__(*args, **kwargs)
 
     def __getitem__(self, n):
         class _VirtualGribField(dict):
```

### Comparing `earthkit-data-0.1.2/tests/indexing/test_indexing_db.py` & `earthkit-data-0.1.3/tests/indexing/test_indexing_db.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/tests/indexing/test_indexing_isel.py` & `earthkit-data-0.1.3/tests/indexing/test_indexing_isel.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,40 +21,40 @@
 from indexing_fixtures import get_tmp_fixture  # noqa
 
 
 @pytest.mark.parametrize("mode", ["file", "multi", "directory"])
 @pytest.mark.parametrize(
     "params,expected_meta,metadata_keys",
     [
-        (dict(param=1, level=2), [("u", 500)], ["shortName", "level:l"]),
-        (dict(param=1, level=2), [(131, 500)], ["paramId", "level:l"]),
+        (dict(param=1, level=2), [["u", 500]], ["shortName", "level:l"]),
+        (dict(param=1, level=2), [[131, 500]], ["paramId", "level:l"]),
         (
             dict(param=[0, 1], level=[2, 3]),
             [
-                ("t", 500),
-                ("t", 700),
-                ("u", 500),
-                ("u", 700),
+                ["t", 500],
+                ["t", 700],
+                ["u", 500],
+                ["u", 700],
             ],
             ["shortName", "level:l"],
         ),
         (
             dict(param=[0], level=[3, 2], type=0),
             [
-                ("t", 500, "an"),
-                ("t", 700, "an"),
+                ["t", 500, "an"],
+                ["t", 700, "an"],
             ],
             ["shortName", "level:l", "marsType"],
         ),
         (
             dict(level=-1),
             [
-                ("t", 1000),
-                ("u", 1000),
-                ("v", 1000),
+                ["t", 1000],
+                ["u", 1000],
+                ["v", 1000],
             ],
             ["shortName", "level:l"],
         ),
     ],
 )
 def test_indexing_isel_grib_file(mode, params, expected_meta, metadata_keys):
     tmp, path = get_tmp_fixture(mode)
```

### Comparing `earthkit-data-0.1.2/tests/indexing/test_indexing_order_by.py` & `earthkit-data-0.1.3/tests/indexing/test_indexing_order_by.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/tests/indexing/test_indexing_serialisation.py` & `earthkit-data-0.1.3/tests/indexing/test_indexing_serialisation.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/tests/indexing/test_order_kwargs.py` & `earthkit-data-0.1.3/tests/indexing/test_order_kwargs.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/tests/indexing/test_selection_kwargs.py` & `earthkit-data-0.1.3/tests/indexing/test_selection_kwargs.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/tests/readers/test_csv_reader.py` & `earthkit-data-0.1.3/tests/readers/test_csv_reader.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/tests/readers/test_grib_reader.py` & `earthkit-data-0.1.3/tests/readers/test_grib_reader.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/tests/readers/test_netcdf_reader.py` & `earthkit-data-0.1.3/tests/readers/test_netcdf_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,15 +168,15 @@
     assert s.datetime() == ref
 
 
 def test_netcdf_to_points_1():
     f = from_source("file", earthkit_test_data_file("test_single.nc"))
 
     eps = 1e-5
-    v = f[0].to_points()
+    v = f[0].to_points(flatten=True)
     assert isinstance(v, dict)
     assert isinstance(v["x"], np.ndarray)
     assert isinstance(v["y"], np.ndarray)
     check_array(
         v["x"],
         (84,),
         first=0.0,
```

### Comparing `earthkit-data-0.1.2/tests/readers/test_tar_reader.py` & `earthkit-data-0.1.3/tests/readers/test_tar_reader.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/tests/readers/test_unknown_reader.py` & `earthkit-data-0.1.3/tests/readers/test_unknown_reader.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/tests/readers/test_zip_reader.py` & `earthkit-data-0.1.3/tests/readers/test_zip_reader.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/tests/sources/test_file.py` & `earthkit-data-0.1.3/tests/sources/test_file.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,37 +9,39 @@
 # nor does it submit to any jurisdiction.
 #
 
 
 import logging
 import os
 
-import pytest
-
 from earthkit.data import from_source
 from earthkit.data.core.temporary import temp_directory
-from earthkit.data.testing import earthkit_file
+from earthkit.data.testing import earthkit_examples_file
 
 LOG = logging.getLogger(__name__)
 
 
-@pytest.mark.long_test
 def test_file_source_grib():
-    s = from_source("file", earthkit_file("docs/examples/test.grib"))
+    s = from_source("file", earthkit_examples_file("test.grib"))
     from earthkit.data.readers.grib.reader import GRIBReader
 
     assert isinstance(s, GRIBReader), s
     assert len(s) == 2
 
 
 def test_file_source_netcdf():
-    s = from_source("file", earthkit_file("docs/examples/test.nc"))
+    s = from_source("file", earthkit_examples_file("test.nc"))
     assert len(s) == 2
 
 
+def test_file_source_odb():
+    s = from_source("file", earthkit_examples_file("test.odb"))
+    assert s.path == earthkit_examples_file("test.odb")
+
+
 # def test_user_1():
 #     s = from_source("file", earthkit_file("docs/examples/test.grib"))
 #     home_file = os.path.expanduser("~/.earthkit_data/test.grib")
 #     try:
 #         s.save(home_file)
 #         # Test expand user
 #         s = from_source("file", "~/.earthkit_data/test.grib")
@@ -66,15 +68,15 @@
 #         try:
 #             os.unlink(home_file)
 #         except OSError:
 #             LOG.exception("unlink(%s)", home_file)
 
 
 def test_glob():
-    s = from_source("file", earthkit_file("docs/examples/test.grib"))
+    s = from_source("file", earthkit_examples_file("test.grib"))
     with temp_directory() as tmpdir:
         s.save(os.path.join(tmpdir, "a.grib"))
         s.save(os.path.join(tmpdir, "b.grib"))
 
         s = from_source("file", os.path.join(tmpdir, "*.grib"))
         assert len(s) == 4, len(s)
```

### Comparing `earthkit-data-0.1.2/tests/sources/test_multi.py` & `earthkit-data-0.1.3/tests/sources/test_multi.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.2/tests/sources/test_url.py` & `earthkit-data-0.1.3/tests/sources/test_url.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,23 +27,24 @@
     filename = os.path.abspath(earthkit_file("docs/examples/test.nc"))
     s = from_source("url", f"file://{filename}")
     assert len(s) == 2
 
 
 def test_url_source_1():
     from_source(
-        "url", "https://get.ecmwf.int/repository/test-data/emohawk/examples/test.grib"
+        "url",
+        "https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test.grib",
     )
 
 
 def test_url_source_check_out_of_date():
     def load():
         from_source(
             "url",
-            "https://get.ecmwf.int/repository/test-data/emohawk/examples/test.grib",
+            "https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test.grib",
         )
 
     with temp_directory() as tmpdir:
         with settings.temporary():
             settings.set("cache-directory", tmpdir)
             load()
 
@@ -51,53 +52,53 @@
             with network_off():
                 load()
 
 
 def test_url_source_2():
     from_source(
         "url",
-        "https://get.ecmwf.int/repository/test-data/emohawk/test-data/temp.bufr",
+        "https://get.ecmwf.int/repository/test-data/earthkit-data/test-data/temp.bufr",
     )
 
 
 def test_url_source_3():
     from_source(
         "url",
-        "https://get.ecmwf.int/repository/test-data/emohawk/examples/test.nc",
+        "https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test.nc",
     )
 
 
 def test_url_source_tar():
     ds = from_source(
         "url",
-        "https://get.ecmwf.int/repository/test-data/emohawk/examples/test_gribs.tar",
+        "https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test_gribs.tar",
     )
     assert len(ds) == 6
 
 
 def test_part_url():
     ds = from_source(
         "url",
-        "https://get.ecmwf.int/repository/test-data/emohawk/test-data/temp.bufr",
+        "https://get.ecmwf.int/repository/test-data/earthkit-data/test-data/temp.bufr",
     )
 
     ds = from_source(
         "url",
-        "https://get.ecmwf.int/repository/test-data/emohawk/test-data/temp.bufr",
+        "https://get.ecmwf.int/repository/test-data/earthkit-data/test-data/temp.bufr",
         parts=((0, 4),),
     )
 
     assert os.path.getsize(ds.path) == 4
 
     with open(ds.path, "rb") as f:
         assert f.read() == b"BUFR"
 
     ds = from_source(
         "url",
-        "https://get.ecmwf.int/repository/test-data/emohawk/test-data/temp.bufr",
+        "https://get.ecmwf.int/repository/test-data/earthkit-data/test-data/temp.bufr",
         parts=((0, 10), (50, 10), (60, 10)),
     )
 
     print(ds.path)
 
     assert os.path.getsize(ds.path) == 30
```

### Comparing `earthkit-data-0.1.2/tests/sources/test_url_pattern.py` & `earthkit-data-0.1.3/tests/sources/test_url_pattern.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,34 +13,34 @@
 
 from earthkit.data import from_source
 
 
 def test_url_pattern_source_1():
     from_source(
         "url-pattern",
-        "https://get.ecmwf.int/repository/test-data/emohawk/examples/test.{format}",
+        "https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test.{format}",
         {"format": ["nc", "grib"]},
     )
     # source.to_xarray()
 
 
 def test_url_pattern_int():
     fs = from_source(
         "url-pattern",
-        "https://get.ecmwf.int/repository/test-data/emohawk/examples/test{id}.grib",
+        "https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test{id}.grib",
         {"id": [4, 6]},
     )
 
     assert len(fs) == 10
 
 
 def test_url_pattern_date():
     fs = from_source(
         "url-pattern",
-        "https://get.ecmwf.int/repository/test-data/emohawk/test-data/"
+        "https://get.ecmwf.int/repository/test-data/earthkit-data/test-data/"
         "test_{my_date:date(%Y-%m-%d)}_{name}.grib",
         {"my_date": datetime.datetime(2020, 5, 13), "name": ["t2", "msl"]},
     )
 
     assert len(fs) == 2
```

