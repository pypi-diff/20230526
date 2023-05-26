# Comparing `tmp/uquake-1.3.8.tar.gz` & `tmp/uquake-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uquake-1.3.8.tar", max compression
+gzip compressed data, was "uquake-1.4.0.tar", max compression
```

## Comparing `uquake-1.3.8.tar` & `uquake-1.4.0.tar`

### file list

```diff
@@ -1,74 +1,75 @@
--rw-r--r--   0        0        0     2399 2023-05-24 16:21:36.067271 uquake-1.3.8/pyproject.toml
--rw-r--r--   0        0        0      158 2023-01-25 01:11:29.666160 uquake-1.3.8/uquake/__init__.py
--rw-r--r--   0        0        0      191 2023-01-15 00:23:22.715786 uquake-1.3.8/uquake/core/__init__.py
--rw-r--r--   0        0        0      417 2023-01-24 21:43:18.390403 uquake-1.3.8/uquake/core/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      413 2023-01-15 02:11:42.951602 uquake-1.3.8/uquake/core/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    27829 2023-01-24 21:43:18.394404 uquake-1.3.8/uquake/core/__pycache__/event.cpython-310.pyc
--rw-r--r--   0        0        0    30935 2023-05-24 14:35:52.245262 uquake-1.3.8/uquake/core/__pycache__/event.cpython-39.pyc
--rw-r--r--   0        0        0    26446 2023-04-16 18:31:14.934875 uquake-1.3.8/uquake/core/__pycache__/inventory.cpython-39.pyc
--rw-r--r--   0        0        0      374 2023-01-15 02:11:43.043606 uquake-1.3.8/uquake/core/__pycache__/logging.cpython-39.pyc
--rw-r--r--   0        0        0    12711 2023-01-25 01:12:24.248712 uquake-1.3.8/uquake/core/__pycache__/stream.cpython-39.pyc
--rw-r--r--   0        0        0     4747 2023-01-15 02:11:43.051606 uquake-1.3.8/uquake/core/__pycache__/trace.cpython-39.pyc
--rw-r--r--   0        0        0      658 2023-01-15 00:23:22.715786 uquake-1.3.8/uquake/core/decorators.py
--rw-r--r--   0        0        0    35160 2023-05-24 16:21:25.074761 uquake-1.3.8/uquake/core/event.py
--rw-r--r--   0        0        0     6233 2023-01-15 00:23:22.715786 uquake-1.3.8/uquake/core/focal_mechanism.py
--rw-r--r--   0        0        0    38774 2023-04-16 18:22:31.094780 uquake-1.3.8/uquake/core/inventory.py
--rw-r--r--   0        0        0      239 2023-01-15 00:23:22.715786 uquake-1.3.8/uquake/core/logging.py
--rw-r--r--   0        0        0    13782 2023-01-25 01:08:23.561456 uquake-1.3.8/uquake/core/stream.py
--rw-r--r--   0        0        0     5308 2023-01-15 00:23:22.715786 uquake-1.3.8/uquake/core/trace.py
--rw-r--r--   0        0        0       67 2023-01-15 00:23:22.715786 uquake-1.3.8/uquake/core/util/__init__.py
--rw-r--r--   0        0        0      257 2023-01-15 02:11:43.051606 uquake-1.3.8/uquake/core/util/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     3018 2023-01-15 02:11:43.051606 uquake-1.3.8/uquake/core/util/__pycache__/base.cpython-39.pyc
--rw-r--r--   0        0        0      732 2023-04-16 18:19:59.471807 uquake-1.3.8/uquake/core/util/__pycache__/requests.cpython-39.pyc
--rw-r--r--   0        0        0    14853 2023-01-15 02:11:43.055606 uquake-1.3.8/uquake/core/util/__pycache__/tools.cpython-39.pyc
--rw-r--r--   0        0        0     4206 2023-01-15 00:23:22.715786 uquake-1.3.8/uquake/core/util/base.py
--rw-r--r--   0        0        0     5713 2023-01-15 00:23:22.715786 uquake-1.3.8/uquake/core/util/decorator.py
--rw-r--r--   0        0        0      620 2023-04-16 18:19:34.782672 uquake-1.3.8/uquake/core/util/requests.py
--rw-r--r--   0        0        0    13768 2023-01-15 00:23:22.715786 uquake-1.3.8/uquake/core/util/tools.py
--rw-r--r--   0        0        0       28 2023-01-15 00:23:22.715786 uquake-1.3.8/uquake/grid/__init__.py
--rw-r--r--   0        0        0      211 2023-03-01 00:04:36.193081 uquake-1.3.8/uquake/grid/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    20180 2023-04-27 19:46:01.284004 uquake-1.3.8/uquake/grid/__pycache__/base.cpython-39.pyc
--rw-r--r--   0        0        0     5136 2023-03-01 00:04:36.301086 uquake-1.3.8/uquake/grid/__pycache__/hdf5.cpython-39.pyc
--rw-r--r--   0        0        0    41279 2023-04-27 19:46:01.292004 uquake-1.3.8/uquake/grid/__pycache__/nlloc.cpython-39.pyc
--rw-r--r--   0        0        0    22173 2023-04-27 00:23:45.744173 uquake-1.3.8/uquake/grid/base.py
--rw-r--r--   0        0        0     4660 2023-05-06 10:03:22.429231 uquake-1.3.8/uquake/grid/hdf5.py
--rw-r--r--   0        0        0    47247 2023-04-27 00:26:03.338550 uquake-1.3.8/uquake/grid/nlloc.py
--rw-r--r--   0        0        0        0 2023-01-15 00:23:22.715786 uquake-1.3.8/uquake/imaging/__init__.py
--rw-r--r--   0        0        0      174 2023-01-15 15:41:46.597579 uquake-1.3.8/uquake/imaging/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     7674 2023-03-08 09:37:32.650116 uquake-1.3.8/uquake/imaging/__pycache__/plot.cpython-39.pyc
--rw-r--r--   0        0        0    34375 2023-01-15 15:41:46.605579 uquake-1.3.8/uquake/imaging/__pycache__/waveform.cpython-39.pyc
--rw-r--r--   0        0        0    10043 2023-03-08 09:37:25.089762 uquake-1.3.8/uquake/imaging/plot.py
--rw-r--r--   0        0        0     2474 2023-01-15 00:23:22.715786 uquake-1.3.8/uquake/imaging/stereonet.py
--rw-r--r--   0        0        0    59743 2023-01-15 00:23:22.719786 uquake-1.3.8/uquake/imaging/waveform.py
--rw-r--r--   0        0        0      423 2023-01-15 00:23:22.719786 uquake-1.3.8/uquake/io/__init__.py
--rw-r--r--   0        0        0      319 2023-03-01 00:09:16.246153 uquake-1.3.8/uquake/io/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0        0 2023-01-15 00:23:22.719786 uquake-1.3.8/uquake/io/event/__init__.py
--rw-r--r--   0        0        0     3417 2023-01-15 00:23:22.719786 uquake-1.3.8/uquake/io/event/core.py
--rw-r--r--   0        0        0       20 2023-01-15 00:23:22.719786 uquake-1.3.8/uquake/io/grid/__init__.py
--rw-r--r--   0        0        0      197 2023-03-01 00:09:16.250153 uquake-1.3.8/uquake/io/grid/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     6606 2023-03-01 00:09:16.250153 uquake-1.3.8/uquake/io/grid/__pycache__/core.cpython-39.pyc
--rw-r--r--   0        0        0     8496 2023-01-15 00:23:22.719786 uquake-1.3.8/uquake/io/grid/core.py
--rw-r--r--   0        0        0       21 2023-01-15 00:23:22.719786 uquake-1.3.8/uquake/io/inventory/__init__.py
--rw-r--r--   0        0        0     6531 2023-01-15 00:23:22.719786 uquake-1.3.8/uquake/io/inventory/core.py
--rw-r--r--   0        0        0       20 2023-01-15 00:23:22.719786 uquake-1.3.8/uquake/io/waveform/__init__.py
--rw-r--r--   0        0        0     9262 2023-01-15 00:23:22.719786 uquake-1.3.8/uquake/io/waveform/core.py
--rw-r--r--   0        0        0       21 2023-01-15 00:23:22.719786 uquake-1.3.8/uquake/nlloc/__init__.py
--rw-r--r--   0        0        0      196 2023-03-01 00:04:36.185081 uquake-1.3.8/uquake/nlloc/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    44596 2023-03-01 00:04:36.193081 uquake-1.3.8/uquake/nlloc/__pycache__/nlloc.cpython-39.pyc
--rw-r--r--   0        0        0    48293 2023-01-15 00:23:22.719786 uquake-1.3.8/uquake/nlloc/nlloc.py
--rw-r--r--   0        0        0        0 2023-01-15 00:23:22.719786 uquake-1.3.8/uquake/waveform/__init__.py
--rw-r--r--   0        0        0      175 2023-01-15 02:11:43.043606 uquake-1.3.8/uquake/waveform/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     4044 2023-01-15 02:11:43.043606 uquake-1.3.8/uquake/waveform/__pycache__/mag_utils.cpython-39.pyc
--rw-r--r--   0        0        0    17136 2023-04-13 09:29:34.130441 uquake-1.3.8/uquake/waveform/__pycache__/pick.cpython-39.pyc
--rw-r--r--   0        0        0    34650 2023-04-04 20:01:50.963657 uquake-1.3.8/uquake/waveform/__pycache__/simple_mag.cpython-39.pyc
--rw-r--r--   0        0        0    34528 2023-01-15 00:23:22.719786 uquake-1.3.8/uquake/waveform/amp_measures.py
--rw-r--r--   0        0        0    15799 2023-01-15 00:23:22.719786 uquake-1.3.8/uquake/waveform/mag.py
--rw-r--r--   0        0        0     5354 2023-01-15 00:23:22.719786 uquake-1.3.8/uquake/waveform/mag_utils.py
--rw-r--r--   0        0        0     2827 2023-01-15 00:23:22.719786 uquake-1.3.8/uquake/waveform/parseval_utils.py
--rw-r--r--   0        0        0    21331 2023-05-16 01:15:39.357070 uquake-1.3.8/uquake/waveform/pick.py
--rw-r--r--   0        0        0    45461 2023-04-04 17:02:48.691928 uquake-1.3.8/uquake/waveform/simple_mag.py
--rw-r--r--   0        0        0    32225 2023-01-15 00:23:22.719786 uquake-1.3.8/uquake/waveform/smom_measure.py
--rw-r--r--   0        0        0    33065 2023-01-15 00:23:22.719786 uquake-1.3.8/uquake/waveform/smom_measure_legacy.py
--rw-r--r--   0        0        0     4456 2023-01-15 00:23:22.719786 uquake-1.3.8/uquake/waveform/transforms.py
--rw-r--r--   0        0        0     2919 1970-01-01 00:00:00.000000 uquake-1.3.8/setup.py
--rw-r--r--   0        0        0     1152 1970-01-01 00:00:00.000000 uquake-1.3.8/PKG-INFO
+-rw-r--r--   0        0        0     2399 2023-05-26 12:31:02.938887 uquake-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0      158 2023-01-25 01:11:29.666160 uquake-1.4.0/uquake/__init__.py
+-rw-r--r--   0        0        0      191 2023-01-15 00:23:22.715786 uquake-1.4.0/uquake/core/__init__.py
+-rw-r--r--   0        0        0      417 2023-01-24 21:43:18.390403 uquake-1.4.0/uquake/core/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      413 2023-01-15 02:11:42.951602 uquake-1.4.0/uquake/core/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    27829 2023-01-24 21:43:18.394404 uquake-1.4.0/uquake/core/__pycache__/event.cpython-310.pyc
+-rw-r--r--   0        0        0    30935 2023-05-24 14:35:52.245262 uquake-1.4.0/uquake/core/__pycache__/event.cpython-39.pyc
+-rw-r--r--   0        0        0    26446 2023-04-16 18:31:14.934875 uquake-1.4.0/uquake/core/__pycache__/inventory.cpython-39.pyc
+-rw-r--r--   0        0        0      374 2023-01-15 02:11:43.043606 uquake-1.4.0/uquake/core/__pycache__/logging.cpython-39.pyc
+-rw-r--r--   0        0        0    12711 2023-01-25 01:12:24.248712 uquake-1.4.0/uquake/core/__pycache__/stream.cpython-39.pyc
+-rw-r--r--   0        0        0     4747 2023-01-15 02:11:43.051606 uquake-1.4.0/uquake/core/__pycache__/trace.cpython-39.pyc
+-rw-r--r--   0        0        0     5502 2023-05-26 12:26:44.678893 uquake-1.4.0/uquake/core/data_ensemble.py
+-rw-r--r--   0        0        0      658 2023-01-15 00:23:22.715786 uquake-1.4.0/uquake/core/decorators.py
+-rw-r--r--   0        0        0    35167 2023-05-26 12:28:53.460873 uquake-1.4.0/uquake/core/event.py
+-rw-r--r--   0        0        0     6233 2023-01-15 00:23:22.715786 uquake-1.4.0/uquake/core/focal_mechanism.py
+-rw-r--r--   0        0        0    38730 2023-05-26 12:30:49.530264 uquake-1.4.0/uquake/core/inventory.py
+-rw-r--r--   0        0        0      239 2023-01-15 00:23:22.715786 uquake-1.4.0/uquake/core/logging.py
+-rw-r--r--   0        0        0    13782 2023-01-25 01:08:23.561456 uquake-1.4.0/uquake/core/stream.py
+-rw-r--r--   0        0        0     5308 2023-01-15 00:23:22.715786 uquake-1.4.0/uquake/core/trace.py
+-rw-r--r--   0        0        0       67 2023-01-15 00:23:22.715786 uquake-1.4.0/uquake/core/util/__init__.py
+-rw-r--r--   0        0        0      257 2023-01-15 02:11:43.051606 uquake-1.4.0/uquake/core/util/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     3018 2023-01-15 02:11:43.051606 uquake-1.4.0/uquake/core/util/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0        0        0      732 2023-04-16 18:19:59.471807 uquake-1.4.0/uquake/core/util/__pycache__/requests.cpython-39.pyc
+-rw-r--r--   0        0        0    14853 2023-01-15 02:11:43.055606 uquake-1.4.0/uquake/core/util/__pycache__/tools.cpython-39.pyc
+-rw-r--r--   0        0        0     4206 2023-01-15 00:23:22.715786 uquake-1.4.0/uquake/core/util/base.py
+-rw-r--r--   0        0        0     5713 2023-01-15 00:23:22.715786 uquake-1.4.0/uquake/core/util/decorator.py
+-rw-r--r--   0        0        0      620 2023-04-16 18:19:34.782672 uquake-1.4.0/uquake/core/util/requests.py
+-rw-r--r--   0        0        0    13768 2023-01-15 00:23:22.715786 uquake-1.4.0/uquake/core/util/tools.py
+-rw-r--r--   0        0        0       28 2023-01-15 00:23:22.715786 uquake-1.4.0/uquake/grid/__init__.py
+-rw-r--r--   0        0        0      211 2023-03-01 00:04:36.193081 uquake-1.4.0/uquake/grid/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    20180 2023-04-27 19:46:01.284004 uquake-1.4.0/uquake/grid/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0        0        0     5136 2023-03-01 00:04:36.301086 uquake-1.4.0/uquake/grid/__pycache__/hdf5.cpython-39.pyc
+-rw-r--r--   0        0        0    41279 2023-04-27 19:46:01.292004 uquake-1.4.0/uquake/grid/__pycache__/nlloc.cpython-39.pyc
+-rw-r--r--   0        0        0    22173 2023-04-27 00:23:45.744173 uquake-1.4.0/uquake/grid/base.py
+-rw-r--r--   0        0        0     4660 2023-05-06 10:03:22.429231 uquake-1.4.0/uquake/grid/hdf5.py
+-rw-r--r--   0        0        0    47247 2023-04-27 00:26:03.338550 uquake-1.4.0/uquake/grid/nlloc.py
+-rw-r--r--   0        0        0        0 2023-01-15 00:23:22.715786 uquake-1.4.0/uquake/imaging/__init__.py
+-rw-r--r--   0        0        0      174 2023-01-15 15:41:46.597579 uquake-1.4.0/uquake/imaging/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     7674 2023-03-08 09:37:32.650116 uquake-1.4.0/uquake/imaging/__pycache__/plot.cpython-39.pyc
+-rw-r--r--   0        0        0    34375 2023-01-15 15:41:46.605579 uquake-1.4.0/uquake/imaging/__pycache__/waveform.cpython-39.pyc
+-rw-r--r--   0        0        0    10043 2023-03-08 09:37:25.089762 uquake-1.4.0/uquake/imaging/plot.py
+-rw-r--r--   0        0        0     2474 2023-01-15 00:23:22.715786 uquake-1.4.0/uquake/imaging/stereonet.py
+-rw-r--r--   0        0        0    59743 2023-01-15 00:23:22.719786 uquake-1.4.0/uquake/imaging/waveform.py
+-rw-r--r--   0        0        0      423 2023-01-15 00:23:22.719786 uquake-1.4.0/uquake/io/__init__.py
+-rw-r--r--   0        0        0      319 2023-03-01 00:09:16.246153 uquake-1.4.0/uquake/io/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0        0 2023-01-15 00:23:22.719786 uquake-1.4.0/uquake/io/event/__init__.py
+-rw-r--r--   0        0        0     3417 2023-01-15 00:23:22.719786 uquake-1.4.0/uquake/io/event/core.py
+-rw-r--r--   0        0        0       20 2023-01-15 00:23:22.719786 uquake-1.4.0/uquake/io/grid/__init__.py
+-rw-r--r--   0        0        0      197 2023-03-01 00:09:16.250153 uquake-1.4.0/uquake/io/grid/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     6606 2023-03-01 00:09:16.250153 uquake-1.4.0/uquake/io/grid/__pycache__/core.cpython-39.pyc
+-rw-r--r--   0        0        0     8496 2023-01-15 00:23:22.719786 uquake-1.4.0/uquake/io/grid/core.py
+-rw-r--r--   0        0        0       21 2023-01-15 00:23:22.719786 uquake-1.4.0/uquake/io/inventory/__init__.py
+-rw-r--r--   0        0        0     6531 2023-01-15 00:23:22.719786 uquake-1.4.0/uquake/io/inventory/core.py
+-rw-r--r--   0        0        0       20 2023-01-15 00:23:22.719786 uquake-1.4.0/uquake/io/waveform/__init__.py
+-rw-r--r--   0        0        0     9262 2023-01-15 00:23:22.719786 uquake-1.4.0/uquake/io/waveform/core.py
+-rw-r--r--   0        0        0       21 2023-01-15 00:23:22.719786 uquake-1.4.0/uquake/nlloc/__init__.py
+-rw-r--r--   0        0        0      196 2023-03-01 00:04:36.185081 uquake-1.4.0/uquake/nlloc/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    44596 2023-03-01 00:04:36.193081 uquake-1.4.0/uquake/nlloc/__pycache__/nlloc.cpython-39.pyc
+-rw-r--r--   0        0        0    48293 2023-01-15 00:23:22.719786 uquake-1.4.0/uquake/nlloc/nlloc.py
+-rw-r--r--   0        0        0        0 2023-01-15 00:23:22.719786 uquake-1.4.0/uquake/waveform/__init__.py
+-rw-r--r--   0        0        0      175 2023-01-15 02:11:43.043606 uquake-1.4.0/uquake/waveform/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     4044 2023-01-15 02:11:43.043606 uquake-1.4.0/uquake/waveform/__pycache__/mag_utils.cpython-39.pyc
+-rw-r--r--   0        0        0    17136 2023-04-13 09:29:34.130441 uquake-1.4.0/uquake/waveform/__pycache__/pick.cpython-39.pyc
+-rw-r--r--   0        0        0    34650 2023-04-04 20:01:50.963657 uquake-1.4.0/uquake/waveform/__pycache__/simple_mag.cpython-39.pyc
+-rw-r--r--   0        0        0    34528 2023-01-15 00:23:22.719786 uquake-1.4.0/uquake/waveform/amp_measures.py
+-rw-r--r--   0        0        0    15799 2023-01-15 00:23:22.719786 uquake-1.4.0/uquake/waveform/mag.py
+-rw-r--r--   0        0        0     5354 2023-01-15 00:23:22.719786 uquake-1.4.0/uquake/waveform/mag_utils.py
+-rw-r--r--   0        0        0     2827 2023-01-15 00:23:22.719786 uquake-1.4.0/uquake/waveform/parseval_utils.py
+-rw-r--r--   0        0        0    21331 2023-05-16 01:15:39.357070 uquake-1.4.0/uquake/waveform/pick.py
+-rw-r--r--   0        0        0    45461 2023-04-04 17:02:48.691928 uquake-1.4.0/uquake/waveform/simple_mag.py
+-rw-r--r--   0        0        0    32225 2023-01-15 00:23:22.719786 uquake-1.4.0/uquake/waveform/smom_measure.py
+-rw-r--r--   0        0        0    33065 2023-01-15 00:23:22.719786 uquake-1.4.0/uquake/waveform/smom_measure_legacy.py
+-rw-r--r--   0        0        0     4456 2023-01-15 00:23:22.719786 uquake-1.4.0/uquake/waveform/transforms.py
+-rw-r--r--   0        0        0     2919 1970-01-01 00:00:00.000000 uquake-1.4.0/setup.py
+-rw-r--r--   0        0        0     1152 1970-01-01 00:00:00.000000 uquake-1.4.0/PKG-INFO
```

### Comparing `uquake-1.3.8/pyproject.toml` & `uquake-1.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uquake"
-version = "1.3.8"
+version = "1.4.0"
 description = "extension of the ObsPy library for local seismicity"
 authors = ["uQuake development team <dev@uQuake.org>"]
 license = "MIT"
 
 # poetry config virtualenvs.create false; poetry env info
 
 [tool.poetry.dependencies]
```

### Comparing `uquake-1.3.8/uquake/core/__pycache__/event.cpython-310.pyc` & `uquake-1.4.0/uquake/core/__pycache__/event.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `uquake-1.3.8/uquake/core/__pycache__/event.cpython-39.pyc` & `uquake-1.4.0/uquake/core/__pycache__/event.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `uquake-1.3.8/uquake/core/__pycache__/inventory.cpython-39.pyc` & `uquake-1.4.0/uquake/core/__pycache__/inventory.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `uquake-1.3.8/uquake/core/__pycache__/stream.cpython-39.pyc` & `uquake-1.4.0/uquake/core/__pycache__/stream.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `uquake-1.3.8/uquake/core/__pycache__/trace.cpython-39.pyc` & `uquake-1.4.0/uquake/core/__pycache__/trace.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `uquake-1.3.8/uquake/core/decorators.py` & `uquake-1.4.0/uquake/core/decorators.py`

 * *Files identical despite different names*

### Comparing `uquake-1.3.8/uquake/core/event.py` & `uquake-1.4.0/uquake/core/event.py`

 * *Files 1% similar despite different names*

```diff
@@ -541,16 +541,15 @@
     def get_sta(self):
         if self.waveform_id is not None:
             return self.waveform_id.station_code
 
     @property
     def site(self):
         if self.waveform_id is not None:
-            site = self.waveform_id.station_code + \
-                   self.waveform_id.location_code
+            site = f'{self.waveform_id.station_code}.{self.waveform_id.location_code}
             return site
 
     @property
     def site_code(self):
         return self.site
 
 
@@ -563,15 +562,15 @@
 
     @property
     def site_code(self):
         if self.station_code is not None:
             if self.location_code is None:
                 return self.station_code
             else:
-                return self.station_code + self.location_code
+                return f'{self.station_code}.{self.location_code}'
 
         return
 
     @property
     def site(self):
         return self.site_code
 
@@ -979,19 +978,19 @@
         if len(self.nodes) > 2:
             v = self.nodes[-2] - self.nodes[-1]
             baz = np.arctan2(v[0], v[1]) * 180 / np.pi
         return baz
 
     @property
     def station(self):
-        return self.site_code[0:4]
+        return self.site_code.split('.')[0]
 
     @property
     def location(self):
-        return self.site_code[4:]
+        return self.site_code.split('.')[1]
 
     @property
     def back_azimuth(self):
         self.baz
 
     @property
     def incidence_angle(self):
```

### Comparing `uquake-1.3.8/uquake/core/focal_mechanism.py` & `uquake-1.4.0/uquake/core/focal_mechanism.py`

 * *Files identical despite different names*

### Comparing `uquake-1.3.8/uquake/core/inventory.py` & `uquake-1.4.0/uquake/core/inventory.py`

 * *Files 1% similar despite different names*

```diff
@@ -674,24 +674,23 @@
 
     @property
     def location_code(self):
         return self.channels[0].location_code
 
     @property
     def code(self):
-        return f'{self.station_code}{self.location_code}'
+        return f'{self.station_code}.{self.location_code}'
 
     @property
     def sensor_type_code(self):
         return self.channels[0].code[0:-1]
 
     @property
     def site_code(self):
-        return f'{self.station_code}.{self.location_code}.' \
-               f'{self.sensor_type_code}'
+        return f'{self.station_code}.{self.location_code}'
 
 
 class Channel(inventory.Channel):
     defaults = {}
     extra_keys = ['x', 'y', 'z', 'alternative_code', 'active', 'oriented']
 
     __doc__ = inventory.Channel.__doc__.replace('obspy', ns)
```

### Comparing `uquake-1.3.8/uquake/core/stream.py` & `uquake-1.4.0/uquake/core/stream.py`

 * *Files identical despite different names*

### Comparing `uquake-1.3.8/uquake/core/trace.py` & `uquake-1.4.0/uquake/core/trace.py`

 * *Files identical despite different names*

### Comparing `uquake-1.3.8/uquake/core/util/__pycache__/base.cpython-39.pyc` & `uquake-1.4.0/uquake/core/util/__pycache__/base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `uquake-1.3.8/uquake/core/util/__pycache__/requests.cpython-39.pyc` & `uquake-1.4.0/uquake/core/util/__pycache__/requests.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `uquake-1.3.8/uquake/core/util/__pycache__/tools.cpython-39.pyc` & `uquake-1.4.0/uquake/core/util/__pycache__/tools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `uquake-1.3.8/uquake/core/util/base.py` & `uquake-1.4.0/uquake/core/util/base.py`

 * *Files identical despite different names*

### Comparing `uquake-1.3.8/uquake/core/util/decorator.py` & `uquake-1.4.0/uquake/core/util/decorator.py`

 * *Files identical despite different names*

### Comparing `uquake-1.3.8/uquake/core/util/requests.py` & `uquake-1.4.0/uquake/core/util/requests.py`

 * *Files identical despite different names*

### Comparing `uquake-1.3.8/uquake/core/util/tools.py` & `uquake-1.4.0/uquake/core/util/tools.py`

 * *Files identical despite different names*

### Comparing `uquake-1.3.8/uquake/grid/__pycache__/base.cpython-39.pyc` & `uquake-1.4.0/uquake/grid/__pycache__/base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `uquake-1.3.8/uquake/grid/__pycache__/hdf5.cpython-39.pyc` & `uquake-1.4.0/uquake/grid/__pycache__/hdf5.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `uquake-1.3.8/uquake/grid/__pycache__/nlloc.cpython-39.pyc` & `uquake-1.4.0/uquake/grid/__pycache__/nlloc.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `uquake-1.3.8/uquake/grid/base.py` & `uquake-1.4.0/uquake/grid/base.py`

 * *Files identical despite different names*

### Comparing `uquake-1.3.8/uquake/grid/hdf5.py` & `uquake-1.4.0/uquake/grid/hdf5.py`

 * *Files identical despite different names*

### Comparing `uquake-1.3.8/uquake/grid/nlloc.py` & `uquake-1.4.0/uquake/grid/nlloc.py`

 * *Files identical despite different names*

### Comparing `uquake-1.3.8/uquake/imaging/__pycache__/plot.cpython-39.pyc` & `uquake-1.4.0/uquake/imaging/__pycache__/plot.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `uquake-1.3.8/uquake/imaging/__pycache__/waveform.cpython-39.pyc` & `uquake-1.4.0/uquake/imaging/__pycache__/waveform.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `uquake-1.3.8/uquake/imaging/plot.py` & `uquake-1.4.0/uquake/imaging/plot.py`

 * *Files identical despite different names*

### Comparing `uquake-1.3.8/uquake/imaging/stereonet.py` & `uquake-1.4.0/uquake/imaging/stereonet.py`

 * *Files identical despite different names*

### Comparing `uquake-1.3.8/uquake/imaging/waveform.py` & `uquake-1.4.0/uquake/imaging/waveform.py`

 * *Files identical despite different names*

### Comparing `uquake-1.3.8/uquake/io/event/core.py` & `uquake-1.4.0/uquake/io/event/core.py`

 * *Files identical despite different names*

### Comparing `uquake-1.3.8/uquake/io/grid/__pycache__/core.cpython-39.pyc` & `uquake-1.4.0/uquake/io/grid/__pycache__/core.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `uquake-1.3.8/uquake/io/grid/core.py` & `uquake-1.4.0/uquake/io/grid/core.py`

 * *Files identical despite different names*

### Comparing `uquake-1.3.8/uquake/io/inventory/core.py` & `uquake-1.4.0/uquake/io/inventory/core.py`

 * *Files identical despite different names*

### Comparing `uquake-1.3.8/uquake/io/waveform/core.py` & `uquake-1.4.0/uquake/io/waveform/core.py`

 * *Files identical despite different names*

### Comparing `uquake-1.3.8/uquake/nlloc/__pycache__/nlloc.cpython-39.pyc` & `uquake-1.4.0/uquake/nlloc/__pycache__/nlloc.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `uquake-1.3.8/uquake/nlloc/nlloc.py` & `uquake-1.4.0/uquake/nlloc/nlloc.py`

 * *Files identical despite different names*

### Comparing `uquake-1.3.8/uquake/waveform/__pycache__/mag_utils.cpython-39.pyc` & `uquake-1.4.0/uquake/waveform/__pycache__/mag_utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `uquake-1.3.8/uquake/waveform/__pycache__/pick.cpython-39.pyc` & `uquake-1.4.0/uquake/waveform/__pycache__/pick.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `uquake-1.3.8/uquake/waveform/__pycache__/simple_mag.cpython-39.pyc` & `uquake-1.4.0/uquake/waveform/__pycache__/simple_mag.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `uquake-1.3.8/uquake/waveform/amp_measures.py` & `uquake-1.4.0/uquake/waveform/amp_measures.py`

 * *Files identical despite different names*

### Comparing `uquake-1.3.8/uquake/waveform/mag.py` & `uquake-1.4.0/uquake/waveform/mag.py`

 * *Files identical despite different names*

### Comparing `uquake-1.3.8/uquake/waveform/mag_utils.py` & `uquake-1.4.0/uquake/waveform/mag_utils.py`

 * *Files identical despite different names*

### Comparing `uquake-1.3.8/uquake/waveform/parseval_utils.py` & `uquake-1.4.0/uquake/waveform/parseval_utils.py`

 * *Files identical despite different names*

### Comparing `uquake-1.3.8/uquake/waveform/pick.py` & `uquake-1.4.0/uquake/waveform/pick.py`

 * *Files identical despite different names*

### Comparing `uquake-1.3.8/uquake/waveform/simple_mag.py` & `uquake-1.4.0/uquake/waveform/simple_mag.py`

 * *Files identical despite different names*

### Comparing `uquake-1.3.8/uquake/waveform/smom_measure.py` & `uquake-1.4.0/uquake/waveform/smom_measure.py`

 * *Files identical despite different names*

### Comparing `uquake-1.3.8/uquake/waveform/smom_measure_legacy.py` & `uquake-1.4.0/uquake/waveform/smom_measure_legacy.py`

 * *Files identical despite different names*

### Comparing `uquake-1.3.8/uquake/waveform/transforms.py` & `uquake-1.4.0/uquake/waveform/transforms.py`

 * *Files identical despite different names*

### Comparing `uquake-1.3.8/setup.py` & `uquake-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
  'uquake.io.waveform.IMS_ASCII': ['readFormat = '
                                   'uquake.io.waveform:read_IMS_ASCII'],
  'uquake.io.waveform.TEXCEL_CSV': ['readFormat = '
                                    'uquake.io.waveform:read_TEXCEL_CSV']}
 
 setup_kwargs = {
     'name': 'uquake',
-    'version': '1.3.8',
+    'version': '1.4.0',
     'description': 'extension of the ObsPy library for local seismicity',
     'long_description': 'None',
     'author': 'uQuake development team',
     'author_email': 'dev@uQuake.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `uquake-1.3.8/PKG-INFO` & `uquake-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uquake
-Version: 1.3.8
+Version: 1.4.0
 Summary: extension of the ObsPy library for local seismicity
 License: MIT
 Author: uQuake development team
 Author-email: dev@uQuake.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

