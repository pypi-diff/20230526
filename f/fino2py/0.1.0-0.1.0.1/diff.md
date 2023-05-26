# Comparing `tmp/fino2py-0.1.0.tar.gz` & `tmp/fino2py-0.1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fino2py-0.1.0.tar", max compression
+gzip compressed data, was "fino2py-0.1.0.1.tar", max compression
```

## Comparing `fino2py-0.1.0.tar` & `fino2py-0.1.0.1.tar`

### file list

```diff
@@ -1,58 +1,38 @@
--rw-r--r--   0        0        0     1205 2023-05-26 10:57:57.957020 fino2py-0.1.0/fino2py/__init__.py
--rw-r--r--   0        0        0        0 2023-05-26 09:46:12.264080 fino2py-0.1.0/fino2py/cleaning/__init__.py
--rw-r--r--   0        0        0      219 2023-05-26 11:22:20.691985 fino2py-0.1.0/fino2py/cleaning/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3630 2023-05-26 11:22:20.708939 fino2py-0.1.0/fino2py/cleaning/__pycache__/merge_split_data.cpython-311.pyc
--rw-r--r--   0        0        0     2873 2023-05-26 10:57:59.234613 fino2py-0.1.0/fino2py/cleaning/merge_split_data.py
--rw-r--r--   0        0        0      379 2023-05-24 20:26:54.190484 fino2py-0.1.0/fino2py/dependencies.py
--rw-r--r--   0        0        0        0 2023-05-26 08:09:59.137334 fino2py-0.1.0/fino2py/ingesting/__init__.py
--rw-r--r--   0        0        0      220 2023-05-26 11:22:18.422075 fino2py-0.1.0/fino2py/ingesting/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3184 2023-05-26 11:22:20.688993 fino2py-0.1.0/fino2py/ingesting/__pycache__/read_raw_demographics.cpython-311.pyc
--rw-r--r--   0        0        0     6538 2023-05-26 11:22:18.437034 fino2py-0.1.0/fino2py/ingesting/__pycache__/read_raw_finometer_data.cpython-311.pyc
--rw-r--r--   0        0        0     2273 2023-05-26 09:09:06.117721 fino2py-0.1.0/fino2py/ingesting/read_raw_demographics.py
--rw-r--r--   0        0        0     4540 2023-05-26 10:57:53.921759 fino2py-0.1.0/fino2py/ingesting/read_raw_finometer_data.py
--rw-r--r--   0        0        0       84 2023-04-21 11:48:58.242633 fino2py-0.1.0/fino2py/reshaping/__init__.py
--rw-r--r--   0        0        0      310 2023-05-24 12:29:07.642726 fino2py-0.1.0/fino2py/reshaping/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2777 2023-05-25 15:51:59.195216 fino2py-0.1.0/fino2py/reshaping/__pycache__/append_cardio_data.cpython-311.pyc
--rw-r--r--   0        0        0     3872 2023-05-26 11:22:20.755814 fino2py-0.1.0/fino2py/reshaping/__pycache__/create_chunk.cpython-311.pyc
--rw-r--r--   0        0        0     5299 2023-05-26 11:22:20.784737 fino2py-0.1.0/fino2py/reshaping/__pycache__/generate_protocol_averages.cpython-311.pyc
--rw-r--r--   0        0        0     2403 2023-05-25 15:51:59.145349 fino2py-0.1.0/fino2py/reshaping/__pycache__/import_demographics.cpython-311.pyc
--rw-r--r--   0        0        0     3934 2023-05-25 15:51:59.160314 fino2py-0.1.0/fino2py/reshaping/__pycache__/import_protocol_averages.cpython-311.pyc
--rw-r--r--   0        0        0     4522 2023-05-26 11:22:20.723900 fino2py-0.1.0/fino2py/reshaping/__pycache__/minute_by_minute.cpython-311.pyc
--rw-r--r--   0        0        0     4028 2023-05-26 11:22:20.736877 fino2py-0.1.0/fino2py/reshaping/__pycache__/minute_by_minute_from_folder.cpython-311.pyc
--rw-r--r--   0        0        0     5252 2023-05-25 15:51:56.868035 fino2py-0.1.0/fino2py/reshaping/__pycache__/read_raw_finometer_data.cpython-311.pyc
--rw-r--r--   0        0        0     3034 2023-05-26 08:58:54.430499 fino2py-0.1.0/fino2py/reshaping/create_chunk.py
--rw-r--r--   0        0        0     4140 2023-05-26 09:43:26.401381 fino2py-0.1.0/fino2py/reshaping/generate_protocol_averages.py
--rw-r--r--   0        0        0     3377 2023-05-26 08:20:44.263887 fino2py-0.1.0/fino2py/reshaping/minute_by_minute.py
--rw-r--r--   0        0        0     3483 2023-05-26 10:57:55.994223 fino2py-0.1.0/fino2py/reshaping/minute_by_minute_from_folder.py
--rw-r--r--   0        0        0   143953 2023-05-12 18:26:28.613384 fino2py-0.1.0/fino2py/tests/current.html
--rw-r--r--   0        0        0   151209 2023-05-16 11:14:34.755093 fino2py-0.1.0/fino2py/tests/current.ipynb
--rw-r--r--   0        0        0    31265 2023-05-16 10:09:11.841529 fino2py-0.1.0/fino2py/tests/current.qmd
--rw-r--r--   0        0        0    80418 2022-11-08 19:32:36.000000 fino2py-0.1.0/fino2py/tests/current_files/libs/bootstrap/bootstrap-icons.css
--rw-r--r--   0        0        0   137124 2022-11-08 19:32:36.000000 fino2py-0.1.0/fino2py/tests/current_files/libs/bootstrap/bootstrap-icons.woff
--rw-r--r--   0        0        0   247908 2023-05-12 18:26:27.479000 fino2py-0.1.0/fino2py/tests/current_files/libs/bootstrap/bootstrap.min.css
--rw-r--r--   0        0        0    78129 2022-11-08 19:32:36.000000 fino2py-0.1.0/fino2py/tests/current_files/libs/bootstrap/bootstrap.min.js
--rw-r--r--   0        0        0     9034 2022-11-08 19:32:36.000000 fino2py-0.1.0/fino2py/tests/current_files/libs/clipboard/clipboard.min.js
--rw-r--r--   0        0        0     6008 2022-11-08 19:32:36.000000 fino2py-0.1.0/fino2py/tests/current_files/libs/quarto-html/anchor.min.js
--rw-r--r--   0        0        0    19728 2022-11-08 19:32:36.000000 fino2py-0.1.0/fino2py/tests/current_files/libs/quarto-html/popper.min.js
--rw-r--r--   0        0        0     2501 2023-04-05 11:21:17.414000 fino2py-0.1.0/fino2py/tests/current_files/libs/quarto-html/quarto-syntax-highlighting.css
--rw-r--r--   0        0        0    24192 2022-11-08 19:32:36.000000 fino2py-0.1.0/fino2py/tests/current_files/libs/quarto-html/quarto.js
--rw-r--r--   0        0        0     1409 2022-11-08 19:32:36.000000 fino2py-0.1.0/fino2py/tests/current_files/libs/quarto-html/tippy.css
--rw-r--r--   0        0        0    24033 2022-11-08 19:32:36.000000 fino2py-0.1.0/fino2py/tests/current_files/libs/quarto-html/tippy.umd.min.js
--rw-r--r--   0        0        0   176240 2023-05-26 10:57:54.924081 fino2py-0.1.0/fino2py/tests/making minute by minutes.ipynb
--rw-r--r--   0        0        0    80230 2023-03-14 13:39:19.929360 fino2py-0.1.0/fino2py/tests/scratch.ipynb
--rw-r--r--   0        0        0     7231 2023-05-24 13:25:45.539597 fino2py-0.1.0/fino2py/tests/test_env.ipynb
--rw-r--r--   0        0        0        0 2023-04-28 09:21:25.682384 fino2py-0.1.0/fino2py/times/__init__.py
--rw-r--r--   0        0        0      220 2023-05-22 18:35:47.591319 fino2py-0.1.0/fino2py/times/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1505 2023-05-25 15:51:59.222144 fino2py-0.1.0/fino2py/times/__pycache__/convert_fino_time.cpython-311.pyc
--rw-r--r--   0        0        0     1514 2023-05-25 15:51:59.184245 fino2py-0.1.0/fino2py/times/__pycache__/convert_partial_time.cpython-311.pyc
--rw-r--r--   0        0        0     1266 2023-05-24 10:37:24.502461 fino2py-0.1.0/fino2py/times/__pycache__/convert_time.cpython-311.pyc
--rw-r--r--   0        0        0     1212 2023-05-26 11:22:20.769777 fino2py-0.1.0/fino2py/times/__pycache__/convert_timestamp_time.cpython-311.pyc
--rw-r--r--   0        0        0     6346 2023-05-25 15:51:59.241093 fino2py-0.1.0/fino2py/times/__pycache__/import_protocol_times.cpython-311.pyc
--rw-r--r--   0        0        0      787 2023-05-24 20:12:35.532955 fino2py-0.1.0/fino2py/times/convert_fino_time.py
--rw-r--r--   0        0        0      779 2023-05-24 20:12:35.532955 fino2py-0.1.0/fino2py/times/convert_partial_time.py
--rw-r--r--   0        0        0      636 2023-05-26 08:40:49.279999 fino2py-0.1.0/fino2py/times/convert_timestamp_time.py
--rw-r--r--   0        0        0     4176 2023-05-24 20:12:35.532955 fino2py-0.1.0/fino2py/times/import_protocol_times.py
--rw-r--r--   0        0        0     1089 2023-05-26 12:14:46.143861 fino2py-0.1.0/LICENSE
--rw-r--r--   0        0        0      509 2023-05-26 11:01:42.197242 fino2py-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1436 2023-05-26 12:01:10.892257 fino2py-0.1.0/README.md
--rw-r--r--   0        0        0     1822 1970-01-01 00:00:00.000000 fino2py-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1205 2023-05-26 10:57:57.957020 fino2py-0.1.0.1/fino2py/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-26 09:46:12.264080 fino2py-0.1.0.1/fino2py/cleaning/__init__.py
+-rw-r--r--   0        0        0     2873 2023-05-26 10:57:59.234613 fino2py-0.1.0.1/fino2py/cleaning/merge_split_data.py
+-rw-r--r--   0        0        0      379 2023-05-24 20:26:54.190484 fino2py-0.1.0.1/fino2py/dependencies.py
+-rw-r--r--   0        0        0        0 2023-05-26 08:09:59.137334 fino2py-0.1.0.1/fino2py/ingesting/__init__.py
+-rw-r--r--   0        0        0     2273 2023-05-26 09:09:06.117721 fino2py-0.1.0.1/fino2py/ingesting/read_raw_demographics.py
+-rw-r--r--   0        0        0     4540 2023-05-26 10:57:53.921759 fino2py-0.1.0.1/fino2py/ingesting/read_raw_finometer_data.py
+-rw-r--r--   0        0        0       84 2023-04-21 11:48:58.242633 fino2py-0.1.0.1/fino2py/reshaping/__init__.py
+-rw-r--r--   0        0        0     3034 2023-05-26 08:58:54.430499 fino2py-0.1.0.1/fino2py/reshaping/create_chunk.py
+-rw-r--r--   0        0        0     4140 2023-05-26 09:43:26.401381 fino2py-0.1.0.1/fino2py/reshaping/generate_protocol_averages.py
+-rw-r--r--   0        0        0     3377 2023-05-26 08:20:44.263887 fino2py-0.1.0.1/fino2py/reshaping/minute_by_minute.py
+-rw-r--r--   0        0        0     3483 2023-05-26 10:57:55.994223 fino2py-0.1.0.1/fino2py/reshaping/minute_by_minute_from_folder.py
+-rw-r--r--   0        0        0   143953 2023-05-12 18:26:28.613384 fino2py-0.1.0.1/fino2py/tests/current.html
+-rw-r--r--   0        0        0   151209 2023-05-16 11:14:34.755093 fino2py-0.1.0.1/fino2py/tests/current.ipynb
+-rw-r--r--   0        0        0    31265 2023-05-16 10:09:11.841529 fino2py-0.1.0.1/fino2py/tests/current.qmd
+-rw-r--r--   0        0        0    80418 2022-11-08 19:32:36.000000 fino2py-0.1.0.1/fino2py/tests/current_files/libs/bootstrap/bootstrap-icons.css
+-rw-r--r--   0        0        0   137124 2022-11-08 19:32:36.000000 fino2py-0.1.0.1/fino2py/tests/current_files/libs/bootstrap/bootstrap-icons.woff
+-rw-r--r--   0        0        0   247908 2023-05-12 18:26:27.479000 fino2py-0.1.0.1/fino2py/tests/current_files/libs/bootstrap/bootstrap.min.css
+-rw-r--r--   0        0        0    78129 2022-11-08 19:32:36.000000 fino2py-0.1.0.1/fino2py/tests/current_files/libs/bootstrap/bootstrap.min.js
+-rw-r--r--   0        0        0     9034 2022-11-08 19:32:36.000000 fino2py-0.1.0.1/fino2py/tests/current_files/libs/clipboard/clipboard.min.js
+-rw-r--r--   0        0        0     6008 2022-11-08 19:32:36.000000 fino2py-0.1.0.1/fino2py/tests/current_files/libs/quarto-html/anchor.min.js
+-rw-r--r--   0        0        0    19728 2022-11-08 19:32:36.000000 fino2py-0.1.0.1/fino2py/tests/current_files/libs/quarto-html/popper.min.js
+-rw-r--r--   0        0        0     2501 2023-04-05 11:21:17.414000 fino2py-0.1.0.1/fino2py/tests/current_files/libs/quarto-html/quarto-syntax-highlighting.css
+-rw-r--r--   0        0        0    24192 2022-11-08 19:32:36.000000 fino2py-0.1.0.1/fino2py/tests/current_files/libs/quarto-html/quarto.js
+-rw-r--r--   0        0        0     1409 2022-11-08 19:32:36.000000 fino2py-0.1.0.1/fino2py/tests/current_files/libs/quarto-html/tippy.css
+-rw-r--r--   0        0        0    24033 2022-11-08 19:32:36.000000 fino2py-0.1.0.1/fino2py/tests/current_files/libs/quarto-html/tippy.umd.min.js
+-rw-r--r--   0        0        0   176240 2023-05-26 10:57:54.924081 fino2py-0.1.0.1/fino2py/tests/making minute by minutes.ipynb
+-rw-r--r--   0        0        0    80230 2023-03-14 13:39:19.929360 fino2py-0.1.0.1/fino2py/tests/scratch.ipynb
+-rw-r--r--   0        0        0     7231 2023-05-24 13:25:45.539597 fino2py-0.1.0.1/fino2py/tests/test_env.ipynb
+-rw-r--r--   0        0        0        0 2023-04-28 09:21:25.682384 fino2py-0.1.0.1/fino2py/times/__init__.py
+-rw-r--r--   0        0        0      787 2023-05-24 20:12:35.532955 fino2py-0.1.0.1/fino2py/times/convert_fino_time.py
+-rw-r--r--   0        0        0      779 2023-05-24 20:12:35.532955 fino2py-0.1.0.1/fino2py/times/convert_partial_time.py
+-rw-r--r--   0        0        0      636 2023-05-26 08:40:49.279999 fino2py-0.1.0.1/fino2py/times/convert_timestamp_time.py
+-rw-r--r--   0        0        0     4176 2023-05-24 20:12:35.532955 fino2py-0.1.0.1/fino2py/times/import_protocol_times.py
+-rw-r--r--   0        0        0     1089 2023-05-26 12:40:23.455047 fino2py-0.1.0.1/LICENSE
+-rw-r--r--   0        0        0      511 2023-05-26 13:10:16.740002 fino2py-0.1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2028 2023-05-26 12:54:17.403360 fino2py-0.1.0.1/README.md
+-rw-r--r--   0        0        0     2416 1970-01-01 00:00:00.000000 fino2py-0.1.0.1/PKG-INFO
```

### Comparing `fino2py-0.1.0/fino2py/__init__.py` & `fino2py-0.1.0.1/fino2py/__init__.py`

 * *Files identical despite different names*

### Comparing `fino2py-0.1.0/fino2py/cleaning/merge_split_data.py` & `fino2py-0.1.0.1/fino2py/cleaning/merge_split_data.py`

 * *Files identical despite different names*

### Comparing `fino2py-0.1.0/fino2py/ingesting/read_raw_demographics.py` & `fino2py-0.1.0.1/fino2py/ingesting/read_raw_demographics.py`

 * *Files identical despite different names*

### Comparing `fino2py-0.1.0/fino2py/ingesting/read_raw_finometer_data.py` & `fino2py-0.1.0.1/fino2py/ingesting/read_raw_finometer_data.py`

 * *Files identical despite different names*

### Comparing `fino2py-0.1.0/fino2py/reshaping/create_chunk.py` & `fino2py-0.1.0.1/fino2py/reshaping/create_chunk.py`

 * *Files identical despite different names*

### Comparing `fino2py-0.1.0/fino2py/reshaping/generate_protocol_averages.py` & `fino2py-0.1.0.1/fino2py/reshaping/generate_protocol_averages.py`

 * *Files identical despite different names*

### Comparing `fino2py-0.1.0/fino2py/reshaping/minute_by_minute.py` & `fino2py-0.1.0.1/fino2py/reshaping/minute_by_minute.py`

 * *Files identical despite different names*

### Comparing `fino2py-0.1.0/fino2py/reshaping/minute_by_minute_from_folder.py` & `fino2py-0.1.0.1/fino2py/reshaping/minute_by_minute_from_folder.py`

 * *Files identical despite different names*

### Comparing `fino2py-0.1.0/fino2py/tests/current.html` & `fino2py-0.1.0.1/fino2py/tests/current.html`

 * *Files identical despite different names*

### Comparing `fino2py-0.1.0/fino2py/tests/current.ipynb` & `fino2py-0.1.0.1/fino2py/tests/current.ipynb`

 * *Files identical despite different names*

### Comparing `fino2py-0.1.0/fino2py/tests/current.qmd` & `fino2py-0.1.0.1/fino2py/tests/current.qmd`

 * *Files identical despite different names*

### Comparing `fino2py-0.1.0/fino2py/tests/current_files/libs/bootstrap/bootstrap-icons.css` & `fino2py-0.1.0.1/fino2py/tests/current_files/libs/bootstrap/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `fino2py-0.1.0/fino2py/tests/current_files/libs/bootstrap/bootstrap-icons.woff` & `fino2py-0.1.0.1/fino2py/tests/current_files/libs/bootstrap/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `fino2py-0.1.0/fino2py/tests/current_files/libs/bootstrap/bootstrap.min.css` & `fino2py-0.1.0.1/fino2py/tests/current_files/libs/bootstrap/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `fino2py-0.1.0/fino2py/tests/current_files/libs/bootstrap/bootstrap.min.js` & `fino2py-0.1.0.1/fino2py/tests/current_files/libs/bootstrap/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `fino2py-0.1.0/fino2py/tests/current_files/libs/clipboard/clipboard.min.js` & `fino2py-0.1.0.1/fino2py/tests/current_files/libs/clipboard/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `fino2py-0.1.0/fino2py/tests/current_files/libs/quarto-html/anchor.min.js` & `fino2py-0.1.0.1/fino2py/tests/current_files/libs/quarto-html/anchor.min.js`

 * *Files identical despite different names*

### Comparing `fino2py-0.1.0/fino2py/tests/current_files/libs/quarto-html/popper.min.js` & `fino2py-0.1.0.1/fino2py/tests/current_files/libs/quarto-html/popper.min.js`

 * *Files identical despite different names*

### Comparing `fino2py-0.1.0/fino2py/tests/current_files/libs/quarto-html/quarto-syntax-highlighting.css` & `fino2py-0.1.0.1/fino2py/tests/current_files/libs/quarto-html/quarto-syntax-highlighting.css`

 * *Files identical despite different names*

### Comparing `fino2py-0.1.0/fino2py/tests/current_files/libs/quarto-html/quarto.js` & `fino2py-0.1.0.1/fino2py/tests/current_files/libs/quarto-html/quarto.js`

 * *Files identical despite different names*

### Comparing `fino2py-0.1.0/fino2py/tests/current_files/libs/quarto-html/tippy.css` & `fino2py-0.1.0.1/fino2py/tests/current_files/libs/quarto-html/tippy.css`

 * *Files identical despite different names*

### Comparing `fino2py-0.1.0/fino2py/tests/current_files/libs/quarto-html/tippy.umd.min.js` & `fino2py-0.1.0.1/fino2py/tests/current_files/libs/quarto-html/tippy.umd.min.js`

 * *Files identical despite different names*

### Comparing `fino2py-0.1.0/fino2py/tests/making minute by minutes.ipynb` & `fino2py-0.1.0.1/fino2py/tests/making minute by minutes.ipynb`

 * *Files identical despite different names*

### Comparing `fino2py-0.1.0/fino2py/tests/scratch.ipynb` & `fino2py-0.1.0.1/fino2py/tests/scratch.ipynb`

 * *Files identical despite different names*

### Comparing `fino2py-0.1.0/fino2py/tests/test_env.ipynb` & `fino2py-0.1.0.1/fino2py/tests/test_env.ipynb`

 * *Files identical despite different names*

### Comparing `fino2py-0.1.0/fino2py/times/convert_fino_time.py` & `fino2py-0.1.0.1/fino2py/times/convert_fino_time.py`

 * *Files identical despite different names*

### Comparing `fino2py-0.1.0/fino2py/times/convert_partial_time.py` & `fino2py-0.1.0.1/fino2py/times/convert_partial_time.py`

 * *Files identical despite different names*

### Comparing `fino2py-0.1.0/fino2py/times/convert_timestamp_time.py` & `fino2py-0.1.0.1/fino2py/times/convert_timestamp_time.py`

 * *Files identical despite different names*

### Comparing `fino2py-0.1.0/fino2py/times/import_protocol_times.py` & `fino2py-0.1.0.1/fino2py/times/import_protocol_times.py`

 * *Files identical despite different names*

### Comparing `fino2py-0.1.0/LICENSE` & `fino2py-0.1.0.1/LICENSE`

 * *Files identical despite different names*

