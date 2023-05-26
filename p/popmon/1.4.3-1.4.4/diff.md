# Comparing `tmp/popmon-1.4.3.tar.gz` & `tmp/popmon-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "popmon-1.4.3.tar", last modified: Thu May 25 16:40:55 2023, max compression
+gzip compressed data, was "popmon-1.4.4.tar", last modified: Fri May 26 09:00:56 2023, max compression
```

## Comparing `popmon-1.4.3.tar` & `popmon-1.4.4.tar`

### file list

```diff
@@ -1,124 +1,123 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:40:55.803537 popmon-1.4.3/
--rw-r--r--   0 root         (0) root         (0)     1071 2023-05-25 16:40:44.000000 popmon-1.4.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       75 2023-05-25 16:40:44.000000 popmon-1.4.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3792 2023-05-25 16:40:44.000000 popmon-1.4.3/NOTICE
--rw-r--r--   0 root         (0) root         (0)    23345 2023-05-25 16:40:55.803537 popmon-1.4.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    21523 2023-05-25 16:40:44.000000 popmon-1.4.3/README.rst
--rw-r--r--   0 root         (0) root         (0)       24 2023-05-25 16:40:44.000000 popmon-1.4.3/extras.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:40:55.775536 popmon-1.4.3/popmon/
--rw-r--r--   0 root         (0) root         (0)     1893 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:40:55.779537 popmon-1.4.3/popmon/alerting/
--rw-r--r--   0 root         (0) root         (0)     1627 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/alerting/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4197 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/alerting/alerts_summary.py
--rw-r--r--   0 root         (0) root         (0)    18616 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/alerting/compute_tl_bounds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:40:55.779537 popmon-1.4.3/popmon/analysis/
--rw-r--r--   0 root         (0) root         (0)     1280 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/analysis/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13883 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/analysis/apply_func.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:40:55.779537 popmon-1.4.3/popmon/analysis/comparison/
--rw-r--r--   0 root         (0) root         (0)     1589 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/analysis/comparison/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8815 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/analysis/comparison/comparisons.py
--rw-r--r--   0 root         (0) root         (0)    15490 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/analysis/comparison/hist_comparer.py
--rw-r--r--   0 root         (0) root         (0)    19311 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/analysis/functions.py
--rw-r--r--   0 root         (0) root         (0)    18578 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/analysis/hist_numpy.py
--rw-r--r--   0 root         (0) root         (0)     2484 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/analysis/merge_statistics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:40:55.779537 popmon-1.4.3/popmon/analysis/profiling/
--rw-r--r--   0 root         (0) root         (0)     1490 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/analysis/profiling/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8232 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/analysis/profiling/hist_profiler.py
--rw-r--r--   0 root         (0) root         (0)     6805 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/analysis/profiling/profiles.py
--rw-r--r--   0 root         (0) root         (0)    11323 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/analysis/profiling/pull_calculator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:40:55.779537 popmon-1.4.3/popmon/base/
--rw-r--r--   0 root         (0) root         (0)     1224 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/base/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6973 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/base/module.py
--rw-r--r--   0 root         (0) root         (0)     2987 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/base/pipeline.py
--rw-r--r--   0 root         (0) root         (0)     4730 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/base/registry.py
--rw-r--r--   0 root         (0) root         (0)    14500 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:40:55.779537 popmon-1.4.3/popmon/decorators/
--rw-r--r--   0 root         (0) root         (0)     1215 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1689 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/decorators/pandas.py
--rw-r--r--   0 root         (0) root         (0)     1728 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/decorators/spark.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:40:55.783537 popmon-1.4.3/popmon/extensions/
--rw-r--r--   0 root         (0) root         (0)     1241 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/extensions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2039 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/extensions/extension.py
--rw-r--r--   0 root         (0) root         (0)     2448 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/extensions/profile_diptest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:40:55.783537 popmon-1.4.3/popmon/hist/
--rw-r--r--   0 root         (0) root         (0)     1189 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/hist/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:40:55.783537 popmon-1.4.3/popmon/hist/filling/
--rw-r--r--   0 root         (0) root         (0)     1745 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/hist/filling/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6570 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/hist/hist_splitter.py
--rw-r--r--   0 root         (0) root         (0)    10908 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/hist/hist_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:40:55.783537 popmon-1.4.3/popmon/io/
--rw-r--r--   0 root         (0) root         (0)     1299 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/io/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2932 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/io/file_reader.py
--rw-r--r--   0 root         (0) root         (0)     3293 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/io/file_writer.py
--rw-r--r--   0 root         (0) root         (0)     1721 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/io/json_reader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:40:55.783537 popmon-1.4.3/popmon/notebooks/
--rw-r--r--   0 root         (0) root         (0)    19461 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/notebooks/popmon_tutorial_advanced.ipynb
--rw-r--r--   0 root         (0) root         (0)     5777 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/notebooks/popmon_tutorial_basic.ipynb
--rw-r--r--   0 root         (0) root         (0)    11902 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/notebooks/popmon_tutorial_incremental_data.ipynb
--rw-r--r--   0 root         (0) root         (0)    11762 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/notebooks/popmon_tutorial_reports.ipynb
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:40:55.787537 popmon-1.4.3/popmon/pipeline/
--rw-r--r--   0 root         (0) root         (0)     1108 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/pipeline/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2409 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/pipeline/amazing_pipeline.py
--rw-r--r--   0 root         (0) root         (0)     5208 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/pipeline/dataset_splitter.py
--rw-r--r--   0 root         (0) root         (0)     7102 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/pipeline/metrics.py
--rw-r--r--   0 root         (0) root         (0)    16465 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/pipeline/metrics_pipelines.py
--rw-r--r--   0 root         (0) root         (0)    11202 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/pipeline/report.py
--rw-r--r--   0 root         (0) root         (0)     9117 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/pipeline/report_pipelines.py
--rw-r--r--   0 root         (0) root         (0)     1752 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/pipeline/timing.py
--rw-r--r--   0 root         (0) root         (0)     4598 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:40:55.787537 popmon-1.4.3/popmon/stats/
--rw-r--r--   0 root         (0) root         (0)     1218 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/stats/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11198 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/stats/numpy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:40:55.787537 popmon-1.4.3/popmon/stitching/
--rw-r--r--   0 root         (0) root         (0)     1234 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/stitching/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20217 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/stitching/hist_stitcher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:40:55.791537 popmon-1.4.3/popmon/test_data/
--rw-r--r--   0 root         (0) root         (0)    73043 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/test_data/data_generator_hists.json.gz
--rw-r--r--   0 root         (0) root         (0)      128 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/test_data/example.json
--rw-r--r--   0 root         (0) root         (0)    15152 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/test_data/example_histogram.json
--rw-r--r--   0 root         (0) root         (0)   696816 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/test_data/flight_delays.csv.gz
--rw-r--r--   0 root         (0) root         (0)   692782 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/test_data/flight_delays_reference.csv.gz
--rw-r--r--   0 root         (0) root         (0)    79082 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/test_data/synthetic_histograms.json
--rw-r--r--   0 root         (0) root         (0)    64368 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/test_data/test.csv.gz
--rw-r--r--   0 root         (0) root         (0)     2705 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/utils.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-25 16:40:45.000000 popmon-1.4.3/popmon/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:40:55.795537 popmon-1.4.3/popmon/visualization/
--rw-r--r--   0 root         (0) root         (0)     1645 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/visualization/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6306 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/visualization/alert_section_generator.py
--rw-r--r--   0 root         (0) root         (0)    15429 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/visualization/histogram_section.py
--rw-r--r--   0 root         (0) root         (0)     8517 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/visualization/overview_section.py
--rw-r--r--   0 root         (0) root         (0)     3079 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/visualization/report_generator.py
--rw-r--r--   0 root         (0) root         (0)    10829 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/visualization/section_generator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:40:55.795537 popmon-1.4.3/popmon/visualization/templates/
--rw-r--r--   0 root         (0) root         (0)      835 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/visualization/templates/aggregated-overview.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:40:55.775536 popmon-1.4.3/popmon/visualization/templates/assets/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:40:55.799537 popmon-1.4.3/popmon/visualization/templates/assets/css/
--rw-r--r--   0 root         (0) root         (0)   155712 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/visualization/templates/assets/css/bootstrap.min.css
--rw-r--r--   0 root         (0) root         (0)     2090 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/visualization/templates/assets/css/custom-style.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:40:55.803537 popmon-1.4.3/popmon/visualization/templates/assets/js/
--rw-r--r--   0 root         (0) root         (0)    78586 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/visualization/templates/assets/js/bootstrap.bundle.min.js
--rw-r--r--   0 root         (0) root         (0)     2943 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/visualization/templates/assets/js/custom-script.js
--rwxr-xr-x   0 root         (0) root         (0)     2532 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/visualization/templates/assets/js/jquery.easing.min.js
--rw-r--r--   0 root         (0) root         (0)    88145 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/visualization/templates/assets/js/jquery.min.js
--rw-r--r--   0 root         (0) root         (0)  3682474 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/visualization/templates/assets/js/plotly.js
--rw-r--r--   0 root         (0) root         (0)      927 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/visualization/templates/assets/js/scrolling-nav.js
--rw-r--r--   0 root         (0) root         (0)     2453 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/visualization/templates/card.html
--rw-r--r--   0 root         (0) root         (0)     1003 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/visualization/templates/core.html
--rw-r--r--   0 root         (0) root         (0)      941 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/visualization/templates/footer.html
--rw-r--r--   0 root         (0) root         (0)      782 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/visualization/templates/header.html
--rw-r--r--   0 root         (0) root         (0)      988 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/visualization/templates/modal-popup.html
--rw-r--r--   0 root         (0) root         (0)      178 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/visualization/templates/notebook_iframe.html
--rw-r--r--   0 root         (0) root         (0)     2739 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/visualization/templates/section.html
--rw-r--r--   0 root         (0) root         (0)     1401 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/visualization/templates/table.html
--rw-r--r--   0 root         (0) root         (0)     7295 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/visualization/traffic_light_section_generator.py
--rw-r--r--   0 root         (0) root         (0)    26741 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/visualization/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:40:55.775536 popmon-1.4.3/popmon.egg-info/
--rw-r--r--   0 root         (0) root         (0)    23345 2023-05-25 16:40:55.000000 popmon-1.4.3/popmon.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3422 2023-05-25 16:40:55.000000 popmon-1.4.3/popmon.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 16:40:55.000000 popmon-1.4.3/popmon.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       68 2023-05-25 16:40:55.000000 popmon-1.4.3/popmon.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      309 2023-05-25 16:40:55.000000 popmon-1.4.3/popmon.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-25 16:40:55.000000 popmon-1.4.3/popmon.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     4619 2023-05-25 16:40:44.000000 popmon-1.4.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      144 2023-05-25 16:40:44.000000 popmon-1.4.3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-25 16:40:55.803537 popmon-1.4.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 09:00:56.061332 popmon-1.4.4/
+-rw-r--r--   0 root         (0) root         (0)     1071 2023-05-26 09:00:44.000000 popmon-1.4.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       75 2023-05-26 09:00:44.000000 popmon-1.4.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3792 2023-05-26 09:00:44.000000 popmon-1.4.4/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    23345 2023-05-26 09:00:56.057332 popmon-1.4.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    21523 2023-05-26 09:00:44.000000 popmon-1.4.4/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 09:00:56.037331 popmon-1.4.4/popmon/
+-rw-r--r--   0 root         (0) root         (0)     1893 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 09:00:56.037331 popmon-1.4.4/popmon/alerting/
+-rw-r--r--   0 root         (0) root         (0)     1627 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/alerting/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4197 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/alerting/alerts_summary.py
+-rw-r--r--   0 root         (0) root         (0)    18616 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/alerting/compute_tl_bounds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 09:00:56.041331 popmon-1.4.4/popmon/analysis/
+-rw-r--r--   0 root         (0) root         (0)     1280 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/analysis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13883 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/analysis/apply_func.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 09:00:56.041331 popmon-1.4.4/popmon/analysis/comparison/
+-rw-r--r--   0 root         (0) root         (0)     1589 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/analysis/comparison/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8815 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/analysis/comparison/comparisons.py
+-rw-r--r--   0 root         (0) root         (0)    15490 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/analysis/comparison/hist_comparer.py
+-rw-r--r--   0 root         (0) root         (0)    19311 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/analysis/functions.py
+-rw-r--r--   0 root         (0) root         (0)    18578 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/analysis/hist_numpy.py
+-rw-r--r--   0 root         (0) root         (0)     2484 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/analysis/merge_statistics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 09:00:56.041331 popmon-1.4.4/popmon/analysis/profiling/
+-rw-r--r--   0 root         (0) root         (0)     1490 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/analysis/profiling/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8232 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/analysis/profiling/hist_profiler.py
+-rw-r--r--   0 root         (0) root         (0)     6805 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/analysis/profiling/profiles.py
+-rw-r--r--   0 root         (0) root         (0)    11323 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/analysis/profiling/pull_calculator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 09:00:56.041331 popmon-1.4.4/popmon/base/
+-rw-r--r--   0 root         (0) root         (0)     1224 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/base/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6973 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/base/module.py
+-rw-r--r--   0 root         (0) root         (0)     2987 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/base/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     4730 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/base/registry.py
+-rw-r--r--   0 root         (0) root         (0)    14500 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 09:00:56.041331 popmon-1.4.4/popmon/decorators/
+-rw-r--r--   0 root         (0) root         (0)     1215 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/decorators/pandas.py
+-rw-r--r--   0 root         (0) root         (0)     1728 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/decorators/spark.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 09:00:56.041331 popmon-1.4.4/popmon/extensions/
+-rw-r--r--   0 root         (0) root         (0)     1241 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/extensions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1642 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/extensions/extension.py
+-rw-r--r--   0 root         (0) root         (0)     2479 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/extensions/profile_diptest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 09:00:56.041331 popmon-1.4.4/popmon/hist/
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/hist/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 09:00:56.041331 popmon-1.4.4/popmon/hist/filling/
+-rw-r--r--   0 root         (0) root         (0)     1745 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/hist/filling/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6570 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/hist/hist_splitter.py
+-rw-r--r--   0 root         (0) root         (0)    10908 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/hist/hist_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 09:00:56.045331 popmon-1.4.4/popmon/io/
+-rw-r--r--   0 root         (0) root         (0)     1299 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/io/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2932 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/io/file_reader.py
+-rw-r--r--   0 root         (0) root         (0)     3293 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/io/file_writer.py
+-rw-r--r--   0 root         (0) root         (0)     1721 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/io/json_reader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 09:00:56.045331 popmon-1.4.4/popmon/notebooks/
+-rw-r--r--   0 root         (0) root         (0)    19461 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/notebooks/popmon_tutorial_advanced.ipynb
+-rw-r--r--   0 root         (0) root         (0)     5777 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/notebooks/popmon_tutorial_basic.ipynb
+-rw-r--r--   0 root         (0) root         (0)    11902 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/notebooks/popmon_tutorial_incremental_data.ipynb
+-rw-r--r--   0 root         (0) root         (0)    11762 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/notebooks/popmon_tutorial_reports.ipynb
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 09:00:56.045331 popmon-1.4.4/popmon/pipeline/
+-rw-r--r--   0 root         (0) root         (0)     1108 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/pipeline/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2409 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/pipeline/amazing_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     5208 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/pipeline/dataset_splitter.py
+-rw-r--r--   0 root         (0) root         (0)     7102 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/pipeline/metrics.py
+-rw-r--r--   0 root         (0) root         (0)    16465 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/pipeline/metrics_pipelines.py
+-rw-r--r--   0 root         (0) root         (0)    11202 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/pipeline/report.py
+-rw-r--r--   0 root         (0) root         (0)     9117 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/pipeline/report_pipelines.py
+-rw-r--r--   0 root         (0) root         (0)     1752 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/pipeline/timing.py
+-rw-r--r--   0 root         (0) root         (0)     4598 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 09:00:56.045331 popmon-1.4.4/popmon/stats/
+-rw-r--r--   0 root         (0) root         (0)     1218 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/stats/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11198 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/stats/numpy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 09:00:56.045331 popmon-1.4.4/popmon/stitching/
+-rw-r--r--   0 root         (0) root         (0)     1234 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/stitching/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20217 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/stitching/hist_stitcher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 09:00:56.049332 popmon-1.4.4/popmon/test_data/
+-rw-r--r--   0 root         (0) root         (0)    73043 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/test_data/data_generator_hists.json.gz
+-rw-r--r--   0 root         (0) root         (0)      128 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/test_data/example.json
+-rw-r--r--   0 root         (0) root         (0)    15152 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/test_data/example_histogram.json
+-rw-r--r--   0 root         (0) root         (0)   696816 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/test_data/flight_delays.csv.gz
+-rw-r--r--   0 root         (0) root         (0)   692782 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/test_data/flight_delays_reference.csv.gz
+-rw-r--r--   0 root         (0) root         (0)    79082 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/test_data/synthetic_histograms.json
+-rw-r--r--   0 root         (0) root         (0)    64368 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/test_data/test.csv.gz
+-rw-r--r--   0 root         (0) root         (0)     2705 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/utils.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-26 09:00:45.000000 popmon-1.4.4/popmon/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 09:00:56.053332 popmon-1.4.4/popmon/visualization/
+-rw-r--r--   0 root         (0) root         (0)     1645 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/visualization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6306 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/visualization/alert_section_generator.py
+-rw-r--r--   0 root         (0) root         (0)    15429 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/visualization/histogram_section.py
+-rw-r--r--   0 root         (0) root         (0)     8517 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/visualization/overview_section.py
+-rw-r--r--   0 root         (0) root         (0)     3079 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/visualization/report_generator.py
+-rw-r--r--   0 root         (0) root         (0)    10829 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/visualization/section_generator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 09:00:56.053332 popmon-1.4.4/popmon/visualization/templates/
+-rw-r--r--   0 root         (0) root         (0)      835 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/visualization/templates/aggregated-overview.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 09:00:56.037331 popmon-1.4.4/popmon/visualization/templates/assets/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 09:00:56.053332 popmon-1.4.4/popmon/visualization/templates/assets/css/
+-rw-r--r--   0 root         (0) root         (0)   155712 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/visualization/templates/assets/css/bootstrap.min.css
+-rw-r--r--   0 root         (0) root         (0)     2090 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/visualization/templates/assets/css/custom-style.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 09:00:56.057332 popmon-1.4.4/popmon/visualization/templates/assets/js/
+-rw-r--r--   0 root         (0) root         (0)    78586 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/visualization/templates/assets/js/bootstrap.bundle.min.js
+-rw-r--r--   0 root         (0) root         (0)     2943 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/visualization/templates/assets/js/custom-script.js
+-rwxr-xr-x   0 root         (0) root         (0)     2532 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/visualization/templates/assets/js/jquery.easing.min.js
+-rw-r--r--   0 root         (0) root         (0)    88145 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/visualization/templates/assets/js/jquery.min.js
+-rw-r--r--   0 root         (0) root         (0)  3682474 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/visualization/templates/assets/js/plotly.js
+-rw-r--r--   0 root         (0) root         (0)      927 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/visualization/templates/assets/js/scrolling-nav.js
+-rw-r--r--   0 root         (0) root         (0)     2453 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/visualization/templates/card.html
+-rw-r--r--   0 root         (0) root         (0)     1003 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/visualization/templates/core.html
+-rw-r--r--   0 root         (0) root         (0)      941 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/visualization/templates/footer.html
+-rw-r--r--   0 root         (0) root         (0)      782 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/visualization/templates/header.html
+-rw-r--r--   0 root         (0) root         (0)      988 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/visualization/templates/modal-popup.html
+-rw-r--r--   0 root         (0) root         (0)      178 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/visualization/templates/notebook_iframe.html
+-rw-r--r--   0 root         (0) root         (0)     2739 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/visualization/templates/section.html
+-rw-r--r--   0 root         (0) root         (0)     1401 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/visualization/templates/table.html
+-rw-r--r--   0 root         (0) root         (0)     7295 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/visualization/traffic_light_section_generator.py
+-rw-r--r--   0 root         (0) root         (0)    26741 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/visualization/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 09:00:56.037331 popmon-1.4.4/popmon.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    23345 2023-05-26 09:00:56.000000 popmon-1.4.4/popmon.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3410 2023-05-26 09:00:56.000000 popmon-1.4.4/popmon.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 09:00:56.000000 popmon-1.4.4/popmon.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       68 2023-05-26 09:00:56.000000 popmon-1.4.4/popmon.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      268 2023-05-26 09:00:56.000000 popmon-1.4.4/popmon.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-26 09:00:56.000000 popmon-1.4.4/popmon.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     4571 2023-05-26 09:00:44.000000 popmon-1.4.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      144 2023-05-26 09:00:44.000000 popmon-1.4.4/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-26 09:00:56.061332 popmon-1.4.4/setup.cfg
```

### Comparing `popmon-1.4.3/LICENSE` & `popmon-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/NOTICE` & `popmon-1.4.4/NOTICE`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/PKG-INFO` & `popmon-1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: popmon
-Version: 1.4.3
+Version: 1.4.4
 Summary: Monitor the stability of a pandas or spark dataset
 Author-email: ING Analytics Wholesale Banking <wbaa@ing.com>
 License: Copyright 2023 ING Analytics Wholesale Banking
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
         documentation files (the "Software"), to deal in the Software without restriction, including without limitation
         the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and
```

### Comparing `popmon-1.4.3/README.rst` & `popmon-1.4.4/README.rst`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/__init__.py` & `popmon-1.4.4/popmon/__init__.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/alerting/__init__.py` & `popmon-1.4.4/popmon/alerting/__init__.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/alerting/alerts_summary.py` & `popmon-1.4.4/popmon/alerting/alerts_summary.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/alerting/compute_tl_bounds.py` & `popmon-1.4.4/popmon/alerting/compute_tl_bounds.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/analysis/__init__.py` & `popmon-1.4.4/popmon/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/analysis/apply_func.py` & `popmon-1.4.4/popmon/analysis/apply_func.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/analysis/comparison/__init__.py` & `popmon-1.4.4/popmon/analysis/comparison/__init__.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/analysis/comparison/comparisons.py` & `popmon-1.4.4/popmon/analysis/comparison/comparisons.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/analysis/comparison/hist_comparer.py` & `popmon-1.4.4/popmon/analysis/comparison/hist_comparer.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/analysis/functions.py` & `popmon-1.4.4/popmon/analysis/functions.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/analysis/hist_numpy.py` & `popmon-1.4.4/popmon/analysis/hist_numpy.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/analysis/merge_statistics.py` & `popmon-1.4.4/popmon/analysis/merge_statistics.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/analysis/profiling/__init__.py` & `popmon-1.4.4/popmon/analysis/profiling/__init__.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/analysis/profiling/hist_profiler.py` & `popmon-1.4.4/popmon/analysis/profiling/hist_profiler.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/analysis/profiling/profiles.py` & `popmon-1.4.4/popmon/analysis/profiling/profiles.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/analysis/profiling/pull_calculator.py` & `popmon-1.4.4/popmon/analysis/profiling/pull_calculator.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/base/__init__.py` & `popmon-1.4.4/popmon/base/__init__.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/base/module.py` & `popmon-1.4.4/popmon/base/module.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/base/pipeline.py` & `popmon-1.4.4/popmon/base/pipeline.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/base/registry.py` & `popmon-1.4.4/popmon/base/registry.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/config.py` & `popmon-1.4.4/popmon/config.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/decorators/__init__.py` & `popmon-1.4.4/popmon/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/decorators/pandas.py` & `popmon-1.4.4/popmon/decorators/pandas.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/decorators/spark.py` & `popmon-1.4.4/popmon/decorators/spark.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/extensions/__init__.py` & `popmon-1.4.4/popmon/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/extensions/extension.py` & `popmon-1.4.4/popmon/extensions/extension.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,43 +15,26 @@
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 from __future__ import annotations
 
 import importlib.util
-from pathlib import Path
 from typing import Callable
 
-try:
-    import tomllib
-except ModuleNotFoundError:
-    import tomli as tomllib
-
 
 def is_installed(package):
     is_present = importlib.util.find_spec(package)
     return is_present is not None
 
 
 class Extension:
     name: str
     extension: Callable
-
-    @property
-    def requirements(self):
-        pyproject_path = Path(__file__).parent.parent.parent / "pyproject.toml"
-        with pyproject_path.open("rb") as f:
-            data = tomllib.load(f)
-
-        project = data["project"]
-        extras = project.get("optional-dependencies", {})
-        if self.name not in extras:
-            return []
-
-        return extras[self.name]
+    # should also be added to `pyproject.toml` optional-dependencies
+    requirements: list[str]
 
     def check(self):
         if all(is_installed(package) for package in self.requirements):
             func = self.extension
             func = func.__func__
             func()
```

### Comparing `popmon-1.4.3/popmon/extensions/profile_diptest.py` & `popmon-1.4.4/popmon/extensions/profile_diptest.py`

 * *Files 7% similar despite different names*

```diff
@@ -64,7 +64,8 @@
         dip, pval = diptest(sample_noise)
         return dip, pval
 
 
 class Diptest(Extension):
     name = "diptest"
     extension = extension
+    requirements = ["diptest"]
```

### Comparing `popmon-1.4.3/popmon/hist/__init__.py` & `popmon-1.4.4/popmon/hist/__init__.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/hist/filling/__init__.py` & `popmon-1.4.4/popmon/hist/filling/__init__.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/hist/hist_splitter.py` & `popmon-1.4.4/popmon/hist/hist_splitter.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/hist/hist_utils.py` & `popmon-1.4.4/popmon/hist/hist_utils.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/io/__init__.py` & `popmon-1.4.4/popmon/io/__init__.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/io/file_reader.py` & `popmon-1.4.4/popmon/io/file_reader.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/io/file_writer.py` & `popmon-1.4.4/popmon/io/file_writer.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/io/json_reader.py` & `popmon-1.4.4/popmon/io/json_reader.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/notebooks/popmon_tutorial_advanced.ipynb` & `popmon-1.4.4/popmon/notebooks/popmon_tutorial_advanced.ipynb`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/notebooks/popmon_tutorial_basic.ipynb` & `popmon-1.4.4/popmon/notebooks/popmon_tutorial_basic.ipynb`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/notebooks/popmon_tutorial_incremental_data.ipynb` & `popmon-1.4.4/popmon/notebooks/popmon_tutorial_incremental_data.ipynb`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/notebooks/popmon_tutorial_reports.ipynb` & `popmon-1.4.4/popmon/notebooks/popmon_tutorial_reports.ipynb`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/pipeline/__init__.py` & `popmon-1.4.4/popmon/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/pipeline/amazing_pipeline.py` & `popmon-1.4.4/popmon/pipeline/amazing_pipeline.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/pipeline/dataset_splitter.py` & `popmon-1.4.4/popmon/pipeline/dataset_splitter.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/pipeline/metrics.py` & `popmon-1.4.4/popmon/pipeline/metrics.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/pipeline/metrics_pipelines.py` & `popmon-1.4.4/popmon/pipeline/metrics_pipelines.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/pipeline/report.py` & `popmon-1.4.4/popmon/pipeline/report.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/pipeline/report_pipelines.py` & `popmon-1.4.4/popmon/pipeline/report_pipelines.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/pipeline/timing.py` & `popmon-1.4.4/popmon/pipeline/timing.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/resources.py` & `popmon-1.4.4/popmon/resources.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/stats/__init__.py` & `popmon-1.4.4/popmon/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/stats/numpy.py` & `popmon-1.4.4/popmon/stats/numpy.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/stitching/__init__.py` & `popmon-1.4.4/popmon/stitching/__init__.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/stitching/hist_stitcher.py` & `popmon-1.4.4/popmon/stitching/hist_stitcher.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/test_data/data_generator_hists.json.gz` & `popmon-1.4.4/popmon/test_data/data_generator_hists.json.gz`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/test_data/example_histogram.json` & `popmon-1.4.4/popmon/test_data/example_histogram.json`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/test_data/flight_delays.csv.gz` & `popmon-1.4.4/popmon/test_data/flight_delays.csv.gz`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/test_data/flight_delays_reference.csv.gz` & `popmon-1.4.4/popmon/test_data/flight_delays_reference.csv.gz`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/test_data/synthetic_histograms.json` & `popmon-1.4.4/popmon/test_data/synthetic_histograms.json`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/test_data/test.csv.gz` & `popmon-1.4.4/popmon/test_data/test.csv.gz`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/utils.py` & `popmon-1.4.4/popmon/utils.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/visualization/__init__.py` & `popmon-1.4.4/popmon/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/visualization/alert_section_generator.py` & `popmon-1.4.4/popmon/visualization/alert_section_generator.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/visualization/histogram_section.py` & `popmon-1.4.4/popmon/visualization/histogram_section.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/visualization/overview_section.py` & `popmon-1.4.4/popmon/visualization/overview_section.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/visualization/report_generator.py` & `popmon-1.4.4/popmon/visualization/report_generator.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/visualization/section_generator.py` & `popmon-1.4.4/popmon/visualization/section_generator.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/visualization/templates/aggregated-overview.html` & `popmon-1.4.4/popmon/visualization/templates/aggregated-overview.html`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/visualization/templates/assets/css/bootstrap.min.css` & `popmon-1.4.4/popmon/visualization/templates/assets/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/visualization/templates/assets/css/custom-style.css` & `popmon-1.4.4/popmon/visualization/templates/assets/css/custom-style.css`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/visualization/templates/assets/js/bootstrap.bundle.min.js` & `popmon-1.4.4/popmon/visualization/templates/assets/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/visualization/templates/assets/js/custom-script.js` & `popmon-1.4.4/popmon/visualization/templates/assets/js/custom-script.js`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/visualization/templates/assets/js/jquery.easing.min.js` & `popmon-1.4.4/popmon/visualization/templates/assets/js/jquery.easing.min.js`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/visualization/templates/assets/js/jquery.min.js` & `popmon-1.4.4/popmon/visualization/templates/assets/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/visualization/templates/assets/js/plotly.js` & `popmon-1.4.4/popmon/visualization/templates/assets/js/plotly.js`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/visualization/templates/assets/js/scrolling-nav.js` & `popmon-1.4.4/popmon/visualization/templates/assets/js/scrolling-nav.js`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/visualization/templates/card.html` & `popmon-1.4.4/popmon/visualization/templates/card.html`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/visualization/templates/core.html` & `popmon-1.4.4/popmon/visualization/templates/core.html`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/visualization/templates/footer.html` & `popmon-1.4.4/popmon/visualization/templates/footer.html`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/visualization/templates/header.html` & `popmon-1.4.4/popmon/visualization/templates/header.html`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/visualization/templates/modal-popup.html` & `popmon-1.4.4/popmon/visualization/templates/modal-popup.html`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/visualization/templates/section.html` & `popmon-1.4.4/popmon/visualization/templates/section.html`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/visualization/templates/table.html` & `popmon-1.4.4/popmon/visualization/templates/table.html`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/visualization/traffic_light_section_generator.py` & `popmon-1.4.4/popmon/visualization/traffic_light_section_generator.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon/visualization/utils.py` & `popmon-1.4.4/popmon/visualization/utils.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.3/popmon.egg-info/PKG-INFO` & `popmon-1.4.4/popmon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: popmon
-Version: 1.4.3
+Version: 1.4.4
 Summary: Monitor the stability of a pandas or spark dataset
 Author-email: ING Analytics Wholesale Banking <wbaa@ing.com>
 License: Copyright 2023 ING Analytics Wholesale Banking
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
         documentation files (the "Software"), to deal in the Software without restriction, including without limitation
         the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and
```

### Comparing `popmon-1.4.3/popmon.egg-info/SOURCES.txt` & `popmon-1.4.4/popmon.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 LICENSE
 MANIFEST.in
 NOTICE
 README.rst
-extras.json
 pyproject.toml
 requirements.txt
 popmon/__init__.py
 popmon/config.py
 popmon/resources.py
 popmon/utils.py
 popmon/version.py
```

### Comparing `popmon-1.4.3/pyproject.toml` & `popmon-1.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -28,16 +28,15 @@
     "phik",
     "jinja2",
     "tqdm",
     "plotly>=5.8.0",
     "joblib>=0.14.0",
     "htmlmin",
     "pydantic",
-    "typing_extensions",
-    "tomli >= 1.1.0 ; python_version < '3.11'"
+    "typing_extensions"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dynamic = ["version"]
```

