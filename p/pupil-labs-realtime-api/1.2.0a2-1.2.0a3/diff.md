# Comparing `tmp/pupil_labs_realtime_api-1.2.0a2.tar.gz` & `tmp/pupil_labs_realtime_api-1.2.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pupil_labs_realtime_api-1.2.0a2.tar", last modified: Fri Oct  7 14:18:03 2022, max compression
+gzip compressed data, was "pupil_labs_realtime_api-1.2.0a3.tar", last modified: Mon Oct 10 12:04:41 2022, max compression
```

## Comparing `pupil_labs_realtime_api-1.2.0a2.tar` & `pupil_labs_realtime_api-1.2.0a3.tar`

### file list

```diff
@@ -1,90 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 14:18:03.723166 pupil_labs_realtime_api-1.2.0a2/
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)      216 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (121)      207 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 14:18:03.715166 pupil_labs_realtime_api-1.2.0a2/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 14:18:03.715166 pupil_labs_realtime_api-1.2.0a2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (121)     6134 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      901 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     5527 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1955 2022-10-07 14:18:03.723166 pupil_labs_realtime_api-1.2.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1033 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 14:18:03.715166 pupil_labs_realtime_api-1.2.0a2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 14:18:03.715166 pupil_labs_realtime_api-1.2.0a2/docs/api/
--rw-r--r--   0 runner    (1001) docker     (121)     1024 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/docs/api/async.rst
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/docs/api/base.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      133 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/docs/api/models.rst
--rw-r--r--   0 runner    (1001) docker     (121)      201 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/docs/api/simple.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2034 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 14:18:03.715166 pupil_labs_realtime_api-1.2.0a2/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     2422 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/docs/examples/async.rst
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/docs/examples/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2185 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/docs/examples/simple.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 14:18:03.715166 pupil_labs_realtime_api-1.2.0a2/docs/guides/
--rw-r--r--   0 runner    (1001) docker     (121)      308 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/docs/guides/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)    13663 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/docs/guides/under-the-hood.rst
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2008 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 14:18:03.711166 pupil_labs_realtime_api-1.2.0a2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 14:18:03.719166 pupil_labs_realtime_api-1.2.0a2/examples/async/
--rw-r--r--   0 runner    (1001) docker     (121)      667 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/examples/async/device_camera_controls.py
--rw-r--r--   0 runner    (1001) docker     (121)      965 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/examples/async/device_status_get_current.py
--rw-r--r--   0 runner    (1001) docker     (121)      855 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/examples/async/device_status_update_via_callback.py
--rw-r--r--   0 runner    (1001) docker     (121)      625 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/examples/async/device_status_update_wait.py
--rw-r--r--   0 runner    (1001) docker     (121)     1308 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/examples/async/device_time_offset.py
--rw-r--r--   0 runner    (1001) docker     (121)      799 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/examples/async/discover_devices.py
--rw-r--r--   0 runner    (1001) docker     (121)      700 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/examples/async/send_event.py
--rw-r--r--   0 runner    (1001) docker     (121)     1208 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/examples/async/start_stop_recordings.py
--rw-r--r--   0 runner    (1001) docker     (121)      887 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/examples/async/stream_gaze.py
--rw-r--r--   0 runner    (1001) docker     (121)     1544 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/examples/async/stream_scene_camera_video.py
--rw-r--r--   0 runner    (1001) docker     (121)     3300 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/examples/async/stream_video_with_overlayed_gaze.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 14:18:03.719166 pupil_labs_realtime_api-1.2.0a2/examples/simple/
--rw-r--r--   0 runner    (1001) docker     (121)      592 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/examples/simple/device_time_offset.py
--rw-r--r--   0 runner    (1001) docker     (121)      432 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/examples/simple/discover_devices.py
--rw-r--r--   0 runner    (1001) docker     (121)      934 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/examples/simple/get_status.py
--rw-r--r--   0 runner    (1001) docker     (121)      499 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/examples/simple/send_event.py
--rw-r--r--   0 runner    (1001) docker     (121)      612 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/examples/simple/start_stop_recordings.py
--rw-r--r--   0 runner    (1001) docker     (121)      691 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/examples/simple/status_auto_update.py
--rw-r--r--   0 runner    (1001) docker     (121)      667 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/examples/simple/stream_gaze.py
--rw-r--r--   0 runner    (1001) docker     (121)     1301 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/examples/simple/stream_scene_camera_video.py
--rw-r--r--   0 runner    (1001) docker     (121)     1041 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/examples/simple/stream_video_with_overlayed_gaze.py
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (121)      277 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)     1461 2022-10-07 14:18:03.723166 pupil_labs_realtime_api-1.2.0a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 14:18:03.711166 pupil_labs_realtime_api-1.2.0a2/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 14:18:03.711166 pupil_labs_realtime_api-1.2.0a2/src/pupil_labs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 14:18:03.719166 pupil_labs_realtime_api-1.2.0a2/src/pupil_labs/realtime_api/
--rw-r--r--   0 runner    (1001) docker     (121)     1097 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/src/pupil_labs/realtime_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2069 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/src/pupil_labs/realtime_api/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     9339 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/src/pupil_labs/realtime_api/device.py
--rw-r--r--   0 runner    (1001) docker     (121)     3798 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/src/pupil_labs/realtime_api/discovery.py
--rw-r--r--   0 runner    (1001) docker     (121)     8191 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/src/pupil_labs/realtime_api/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 14:18:03.719166 pupil_labs_realtime_api-1.2.0a2/src/pupil_labs/realtime_api/simple/
--rw-r--r--   0 runner    (1001) docker     (121)      261 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/src/pupil_labs/realtime_api/simple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7031 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/src/pupil_labs/realtime_api/simple/_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    13746 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/src/pupil_labs/realtime_api/simple/device.py
--rw-r--r--   0 runner    (1001) docker     (121)     1303 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/src/pupil_labs/realtime_api/simple/discovery.py
--rw-r--r--   0 runner    (1001) docker     (121)      729 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/src/pupil_labs/realtime_api/simple/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 14:18:03.719166 pupil_labs_realtime_api-1.2.0a2/src/pupil_labs/realtime_api/streaming/
--rw-r--r--   0 runner    (1001) docker     (121)      653 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/src/pupil_labs/realtime_api/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4087 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/src/pupil_labs/realtime_api/streaming/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2205 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/src/pupil_labs/realtime_api/streaming/gaze.py
--rw-r--r--   0 runner    (1001) docker     (121)     1877 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/src/pupil_labs/realtime_api/streaming/nal_unit.py
--rw-r--r--   0 runner    (1001) docker     (121)     3289 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/src/pupil_labs/realtime_api/streaming/video.py
--rw-r--r--   0 runner    (1001) docker     (121)     7361 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/src/pupil_labs/realtime_api/time_echo.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 14:18:03.723166 pupil_labs_realtime_api-1.2.0a2/src/pupil_labs_realtime_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1955 2022-10-07 14:18:03.000000 pupil_labs_realtime_api-1.2.0a2/src/pupil_labs_realtime_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2258 2022-10-07 14:18:03.000000 pupil_labs_realtime_api-1.2.0a2/src/pupil_labs_realtime_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-07 14:18:03.000000 pupil_labs_realtime_api-1.2.0a2/src/pupil_labs_realtime_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      348 2022-10-07 14:18:03.000000 pupil_labs_realtime_api-1.2.0a2/src/pupil_labs_realtime_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-10-07 14:18:03.000000 pupil_labs_realtime_api-1.2.0a2/src/pupil_labs_realtime_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 14:18:03.723166 pupil_labs_realtime_api-1.2.0a2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      303 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (121)      745 2022-10-07 14:17:33.000000 pupil_labs_realtime_api-1.2.0a2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 12:04:41.856255 pupil_labs_realtime_api-1.2.0a3/
+-rw-r--r--   0 runner    (1001) docker     (121)       99 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (121)      216 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (121)      207 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 12:04:41.848255 pupil_labs_realtime_api-1.2.0a3/.github/
+-rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 12:04:41.848255 pupil_labs_realtime_api-1.2.0a3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     6134 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      901 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      134 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     5527 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     1955 2022-10-10 12:04:41.856255 pupil_labs_realtime_api-1.2.0a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1033 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 12:04:41.848255 pupil_labs_realtime_api-1.2.0a3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 12:04:41.848255 pupil_labs_realtime_api-1.2.0a3/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (121)     1024 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/docs/api/async.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      129 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/docs/api/base.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      133 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/docs/api/models.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      201 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/docs/api/simple.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2034 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 12:04:41.848255 pupil_labs_realtime_api-1.2.0a3/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     2422 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/docs/examples/async.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       98 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/docs/examples/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2185 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/docs/examples/simple.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 12:04:41.848255 pupil_labs_realtime_api-1.2.0a3/docs/guides/
+-rw-r--r--   0 runner    (1001) docker     (121)      308 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/docs/guides/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    13663 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/docs/guides/under-the-hood.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2008 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 12:04:41.844255 pupil_labs_realtime_api-1.2.0a3/examples/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 12:04:41.848255 pupil_labs_realtime_api-1.2.0a3/examples/async/
+-rw-r--r--   0 runner    (1001) docker     (121)     1161 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/examples/async/device_camera_controls.py
+-rw-r--r--   0 runner    (1001) docker     (121)      965 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/examples/async/device_status_get_current.py
+-rw-r--r--   0 runner    (1001) docker     (121)      855 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/examples/async/device_status_update_via_callback.py
+-rw-r--r--   0 runner    (1001) docker     (121)      625 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/examples/async/device_status_update_wait.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1308 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/examples/async/device_time_offset.py
+-rw-r--r--   0 runner    (1001) docker     (121)      799 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/examples/async/discover_devices.py
+-rw-r--r--   0 runner    (1001) docker     (121)      700 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/examples/async/send_event.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1208 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/examples/async/start_stop_recordings.py
+-rw-r--r--   0 runner    (1001) docker     (121)      887 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/examples/async/stream_gaze.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1544 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/examples/async/stream_scene_camera_video.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3300 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/examples/async/stream_video_with_overlayed_gaze.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 12:04:41.852255 pupil_labs_realtime_api-1.2.0a3/examples/simple/
+-rw-r--r--   0 runner    (1001) docker     (121)      592 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/examples/simple/device_time_offset.py
+-rw-r--r--   0 runner    (1001) docker     (121)      432 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/examples/simple/discover_devices.py
+-rw-r--r--   0 runner    (1001) docker     (121)      934 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/examples/simple/get_status.py
+-rw-r--r--   0 runner    (1001) docker     (121)      499 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/examples/simple/send_event.py
+-rw-r--r--   0 runner    (1001) docker     (121)      612 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/examples/simple/start_stop_recordings.py
+-rw-r--r--   0 runner    (1001) docker     (121)      691 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/examples/simple/status_auto_update.py
+-rw-r--r--   0 runner    (1001) docker     (121)      667 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/examples/simple/stream_gaze.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1301 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/examples/simple/stream_scene_camera_video.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1041 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/examples/simple/stream_video_with_overlayed_gaze.py
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (121)      277 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (121)     1572 2022-10-10 12:04:41.856255 pupil_labs_realtime_api-1.2.0a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       92 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 12:04:41.844255 pupil_labs_realtime_api-1.2.0a3/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 12:04:41.844255 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 12:04:41.852255 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/
+-rw-r--r--   0 runner    (1001) docker     (121)     1097 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2069 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2035 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/camera_control.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13297 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/device.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4170 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8191 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/models.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 12:04:41.852255 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/simple/
+-rw-r--r--   0 runner    (1001) docker     (121)      261 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/simple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7031 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/simple/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13746 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/simple/device.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1303 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/simple/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (121)      729 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/simple/models.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 12:04:41.852255 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/streaming/
+-rw-r--r--   0 runner    (1001) docker     (121)      653 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4087 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/streaming/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2205 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/streaming/gaze.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1877 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/streaming/nal_unit.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3289 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/streaming/video.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7361 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/time_echo.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 12:04:41.856255 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs_realtime_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1955 2022-10-10 12:04:41.000000 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs_realtime_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2381 2022-10-10 12:04:41.000000 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs_realtime_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-10 12:04:41.000000 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs_realtime_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       70 2022-10-10 12:04:41.000000 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs_realtime_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-10-10 12:04:41.000000 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs_realtime_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2022-10-10 12:04:41.000000 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs_realtime_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 12:04:41.856255 pupil_labs_realtime_api-1.2.0a3/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      303 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)      675 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/tests/test_controls.py
+-rw-r--r--   0 runner    (1001) docker     (121)      745 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/tox.ini
```

### Comparing `pupil_labs_realtime_api-1.2.0a2/.github/workflows/main.yml` & `pupil_labs_realtime_api-1.2.0a3/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a2/.gitignore` & `pupil_labs_realtime_api-1.2.0a3/.gitignore`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a2/.pre-commit-config.yaml` & `pupil_labs_realtime_api-1.2.0a3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a2/CHANGES.rst` & `pupil_labs_realtime_api-1.2.0a3/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a2/LICENSE` & `pupil_labs_realtime_api-1.2.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a2/PKG-INFO` & `pupil_labs_realtime_api-1.2.0a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pupil_labs_realtime_api
-Version: 1.2.0a2
+Version: 1.2.0a3
 Summary: Python client for the Pupil Labs Realtime API
 Home-page: https://github.com/pupil-labs/realtime-python-api
 Author: Pupil Labs GmbH
 Author-email: info@pupil-labs.com
 License: MIT
 Project-URL: Documentation, https://pupil-labs-realtime-api.readthedocs.io/en/stable/
 Project-URL: History, https://pupil-labs-realtime-api.readthedocs.io/en/latest/history.html
```

### Comparing `pupil_labs_realtime_api-1.2.0a2/README.rst` & `pupil_labs_realtime_api-1.2.0a3/README.rst`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a2/docs/api/async.rst` & `pupil_labs_realtime_api-1.2.0a3/docs/api/async.rst`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a2/docs/conf.py` & `pupil_labs_realtime_api-1.2.0a3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a2/docs/examples/async.rst` & `pupil_labs_realtime_api-1.2.0a3/docs/examples/async.rst`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a2/docs/examples/simple.rst` & `pupil_labs_realtime_api-1.2.0a3/docs/examples/simple.rst`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a2/docs/guides/under-the-hood.rst` & `pupil_labs_realtime_api-1.2.0a3/docs/guides/under-the-hood.rst`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a2/docs/index.rst` & `pupil_labs_realtime_api-1.2.0a3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a2/examples/async/device_camera_controls.py` & `pupil_labs_realtime_api-1.2.0a3/examples/async/send_event.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import asyncio
-import logging
+import time
 
-from pupil_labs.realtime_api import Device, Network, discover_devices
+from pupil_labs.realtime_api import Device, Network
 
 
 async def main():
-    dev_info = None
-    async for dev_info in discover_devices():
-        if "9865e04c385bcb59" in dev_info.name:
-            break
-
+    async with Network() as network:
+        dev_info = await network.wait_for_new_device(timeout_seconds=5)
     if dev_info is None:
         print("No device could be found! Abort")
         return
 
     async with Device.from_discovered_device(dev_info) as device:
-        status = await device._camera_control(
-            ae_mode="auto", man_exp=50, gain=50, brightness=0, contrast=70, gamma=300
+        # send event without timestamp
+        print(await device.send_event("test event"))
+
+        # send event with current timestamp
+        print(
+            await device.send_event(
+                "test event", event_timestamp_unix_ns=time.time_ns()
+            )
         )
-        print(status)
 
 
 if __name__ == "__main__":
-    logging.basicConfig(level="DEBUG")
     asyncio.run(main())
```

### Comparing `pupil_labs_realtime_api-1.2.0a2/examples/async/device_status_get_current.py` & `pupil_labs_realtime_api-1.2.0a3/examples/async/device_status_get_current.py`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a2/examples/async/device_status_update_via_callback.py` & `pupil_labs_realtime_api-1.2.0a3/examples/async/device_status_update_via_callback.py`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a2/examples/async/device_status_update_wait.py` & `pupil_labs_realtime_api-1.2.0a3/examples/async/device_status_update_wait.py`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a2/examples/async/device_time_offset.py` & `pupil_labs_realtime_api-1.2.0a3/examples/async/device_time_offset.py`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a2/examples/async/discover_devices.py` & `pupil_labs_realtime_api-1.2.0a3/examples/async/discover_devices.py`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a2/examples/async/start_stop_recordings.py` & `pupil_labs_realtime_api-1.2.0a3/examples/async/start_stop_recordings.py`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a2/examples/async/stream_gaze.py` & `pupil_labs_realtime_api-1.2.0a3/examples/async/stream_gaze.py`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a2/examples/async/stream_scene_camera_video.py` & `pupil_labs_realtime_api-1.2.0a3/examples/async/stream_scene_camera_video.py`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a2/examples/async/stream_video_with_overlayed_gaze.py` & `pupil_labs_realtime_api-1.2.0a3/examples/async/stream_video_with_overlayed_gaze.py`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a2/examples/simple/device_time_offset.py` & `pupil_labs_realtime_api-1.2.0a3/examples/simple/device_time_offset.py`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a2/examples/simple/get_status.py` & `pupil_labs_realtime_api-1.2.0a3/examples/simple/get_status.py`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a2/examples/simple/start_stop_recordings.py` & `pupil_labs_realtime_api-1.2.0a3/examples/simple/start_stop_recordings.py`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a2/examples/simple/status_auto_update.py` & `pupil_labs_realtime_api-1.2.0a3/examples/simple/status_auto_update.py`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a2/examples/simple/stream_gaze.py` & `pupil_labs_realtime_api-1.2.0a3/examples/simple/stream_gaze.py`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a2/examples/simple/stream_scene_camera_video.py` & `pupil_labs_realtime_api-1.2.0a3/examples/simple/stream_scene_camera_video.py`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a2/examples/simple/stream_video_with_overlayed_gaze.py` & `pupil_labs_realtime_api-1.2.0a3/examples/simple/stream_video_with_overlayed_gaze.py`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a2/setup.cfg` & `pupil_labs_realtime_api-1.2.0a3/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -21,32 +21,38 @@
 
 [options]
 packages = find_namespace:
 install_requires = 
 	aiohttp[speedups]
 	aiortsp
 	av
+	click
 	nptyping<2  # TODO: Support nptyping>=2
+	rich
 	websockets
 	zeroconf
 	importlib-metadata;python_version<"3.8"
-	typing-extensions;python_version<"3.8"
+	typing-extensions;python_version<="3.10"
 python_requires = >=3.7
 include_package_data = true
 package_dir = 
 	=src
 
 [options.packages.find]
 where = src
 exclude = 
 	build*
 	dist*
 	docs*
 	tests*
 
+[options.entry_points]
+console_scripts = 
+	pl-discover = pupil_labs.realtime_api.discovery:cli
+
 [options.extras_require]
 docs = 
 	furo
 	jaraco.packaging>=8.2
 	rst.linker>=1.9
 	sphinx<4.4
 	importlib-metadata;python_version<"3.8"
```

### Comparing `pupil_labs_realtime_api-1.2.0a2/src/pupil_labs/realtime_api/__init__.py` & `pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/__init__.py`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a2/src/pupil_labs/realtime_api/base.py` & `pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/base.py`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a2/src/pupil_labs/realtime_api/discovery.py` & `pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/discovery.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import asyncio
 import logging
 import time
 import types
 import typing as T
 
+import click
 from zeroconf import ServiceStateChange
 from zeroconf.asyncio import AsyncServiceBrowser, AsyncServiceInfo, AsyncZeroconf
 
 from .models import DiscoveredDeviceInfo
 
 logger = logging.getLogger(__name__)
 
@@ -110,7 +111,23 @@
                 yield device
             if timeout_seconds is not None:
                 timeout_seconds -= time.perf_counter() - t0
 
 
 def is_valid_service_name(name: str) -> bool:
     return name.split(":")[0] == "PI monitor"
+
+
+@click.command()
+@click.option("-t", "--search-duration", type=float)
+def cli(search_duration: T.Optional[float] = None):
+    async def print_devices():
+        from rich import print
+
+        async for dev in discover_devices(timeout_seconds=search_duration):
+            print(dev)
+
+    asyncio.run(print_devices())
+
+
+if __name__ == "__main__":
+    cli()
```

### Comparing `pupil_labs_realtime_api-1.2.0a2/src/pupil_labs/realtime_api/models.py` & `pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/models.py`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a2/src/pupil_labs/realtime_api/simple/_utils.py` & `pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/simple/_utils.py`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a2/src/pupil_labs/realtime_api/simple/device.py` & `pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/simple/device.py`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a2/src/pupil_labs/realtime_api/simple/discovery.py` & `pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/simple/discovery.py`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a2/src/pupil_labs/realtime_api/simple/models.py` & `pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/simple/models.py`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a2/src/pupil_labs/realtime_api/streaming/__init__.py` & `pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/streaming/__init__.py`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a2/src/pupil_labs/realtime_api/streaming/base.py` & `pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/streaming/base.py`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a2/src/pupil_labs/realtime_api/streaming/gaze.py` & `pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/streaming/gaze.py`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a2/src/pupil_labs/realtime_api/streaming/nal_unit.py` & `pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/streaming/nal_unit.py`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a2/src/pupil_labs/realtime_api/streaming/video.py` & `pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/streaming/video.py`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a2/src/pupil_labs/realtime_api/time_echo.py` & `pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/time_echo.py`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a2/src/pupil_labs_realtime_api.egg-info/PKG-INFO` & `pupil_labs_realtime_api-1.2.0a3/src/pupil_labs_realtime_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pupil-labs-realtime-api
-Version: 1.2.0a2
+Version: 1.2.0a3
 Summary: Python client for the Pupil Labs Realtime API
 Home-page: https://github.com/pupil-labs/realtime-python-api
 Author: Pupil Labs GmbH
 Author-email: info@pupil-labs.com
 License: MIT
 Project-URL: Documentation, https://pupil-labs-realtime-api.readthedocs.io/en/stable/
 Project-URL: History, https://pupil-labs-realtime-api.readthedocs.io/en/latest/history.html
```

### Comparing `pupil_labs_realtime_api-1.2.0a2/src/pupil_labs_realtime_api.egg-info/SOURCES.txt` & `pupil_labs_realtime_api-1.2.0a3/src/pupil_labs_realtime_api.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 examples/simple/start_stop_recordings.py
 examples/simple/status_auto_update.py
 examples/simple/stream_gaze.py
 examples/simple/stream_scene_camera_video.py
 examples/simple/stream_video_with_overlayed_gaze.py
 src/pupil_labs/realtime_api/__init__.py
 src/pupil_labs/realtime_api/base.py
+src/pupil_labs/realtime_api/camera_control.py
 src/pupil_labs/realtime_api/device.py
 src/pupil_labs/realtime_api/discovery.py
 src/pupil_labs/realtime_api/models.py
 src/pupil_labs/realtime_api/time_echo.py
 src/pupil_labs/realtime_api/simple/__init__.py
 src/pupil_labs/realtime_api/simple/_utils.py
 src/pupil_labs/realtime_api/simple/device.py
@@ -63,10 +64,12 @@
 src/pupil_labs/realtime_api/streaming/base.py
 src/pupil_labs/realtime_api/streaming/gaze.py
 src/pupil_labs/realtime_api/streaming/nal_unit.py
 src/pupil_labs/realtime_api/streaming/video.py
 src/pupil_labs_realtime_api.egg-info/PKG-INFO
 src/pupil_labs_realtime_api.egg-info/SOURCES.txt
 src/pupil_labs_realtime_api.egg-info/dependency_links.txt
+src/pupil_labs_realtime_api.egg-info/entry_points.txt
 src/pupil_labs_realtime_api.egg-info/requires.txt
 src/pupil_labs_realtime_api.egg-info/top_level.txt
-tests/test_api.py
+tests/test_api.py
+tests/test_controls.py
```

### Comparing `pupil_labs_realtime_api-1.2.0a2/tox.ini` & `pupil_labs_realtime_api-1.2.0a3/tox.ini`

 * *Files identical despite different names*

