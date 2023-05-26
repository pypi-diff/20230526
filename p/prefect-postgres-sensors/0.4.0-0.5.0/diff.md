# Comparing `tmp/prefect_postgres_sensors-0.4.0.tar.gz` & `tmp/prefect_postgres_sensors-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect_postgres_sensors-0.4.0.tar", last modified: Fri May 26 11:59:39 2023, max compression
+gzip compressed data, was "prefect_postgres_sensors-0.5.0.tar", last modified: Fri May 26 12:13:33 2023, max compression
```

## Comparing `prefect_postgres_sensors-0.4.0.tar` & `prefect_postgres_sensors-0.5.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0 james     (1000) james     (1000)        0 2023-05-26 11:59:39.112535 prefect_postgres_sensors-0.4.0/
--rwxrwxrwx   0 james     (1000) james     (1000)     1074 2023-05-17 13:09:12.000000 prefect_postgres_sensors-0.4.0/LICENSE
--rwxrwxrwx   0 james     (1000) james     (1000)      271 2023-05-26 11:59:39.103538 prefect_postgres_sensors-0.4.0/PKG-INFO
--rwxrwxrwx   0 james     (1000) james     (1000)     3607 2023-05-26 11:40:57.000000 prefect_postgres_sensors-0.4.0/README.md
-drwxrwxrwx   0 james     (1000) james     (1000)        0 2023-05-26 11:59:38.802098 prefect_postgres_sensors-0.4.0/prefect_postgres_sensors/
--rwxrwxrwx   0 james     (1000) james     (1000)      129 2023-05-26 11:56:29.000000 prefect_postgres_sensors-0.4.0/prefect_postgres_sensors/__init__.py
-drwxrwxrwx   0 james     (1000) james     (1000)        0 2023-05-26 11:59:39.057244 prefect_postgres_sensors-0.4.0/prefect_postgres_sensors.egg-info/
--rwxrwxrwx   0 james     (1000) james     (1000)      271 2023-05-26 11:59:37.000000 prefect_postgres_sensors-0.4.0/prefect_postgres_sensors.egg-info/PKG-INFO
--rwxrwxrwx   0 james     (1000) james     (1000)      302 2023-05-26 11:59:37.000000 prefect_postgres_sensors-0.4.0/prefect_postgres_sensors.egg-info/SOURCES.txt
--rwxrwxrwx   0 james     (1000) james     (1000)        1 2023-05-26 11:59:37.000000 prefect_postgres_sensors-0.4.0/prefect_postgres_sensors.egg-info/dependency_links.txt
--rwxrwxrwx   0 james     (1000) james     (1000)       26 2023-05-26 11:59:37.000000 prefect_postgres_sensors-0.4.0/prefect_postgres_sensors.egg-info/requires.txt
--rwxrwxrwx   0 james     (1000) james     (1000)       25 2023-05-26 11:59:37.000000 prefect_postgres_sensors-0.4.0/prefect_postgres_sensors.egg-info/top_level.txt
--rwxrwxrwx   0 james     (1000) james     (1000)       38 2023-05-26 11:59:39.117536 prefect_postgres_sensors-0.4.0/setup.cfg
--rwxrwxrwx   0 james     (1000) james     (1000)      356 2023-05-26 11:56:12.000000 prefect_postgres_sensors-0.4.0/setup.py
+drwxrwxrwx   0 james     (1000) james     (1000)        0 2023-05-26 12:13:33.642224 prefect_postgres_sensors-0.5.0/
+-rwxrwxrwx   0 james     (1000) james     (1000)     1074 2023-05-17 13:09:12.000000 prefect_postgres_sensors-0.5.0/LICENSE
+-rwxrwxrwx   0 james     (1000) james     (1000)      271 2023-05-26 12:13:33.628236 prefect_postgres_sensors-0.5.0/PKG-INFO
+-rwxrwxrwx   0 james     (1000) james     (1000)     3607 2023-05-26 11:40:57.000000 prefect_postgres_sensors-0.5.0/README.md
+drwxrwxrwx   0 james     (1000) james     (1000)        0 2023-05-26 12:13:33.290262 prefect_postgres_sensors-0.5.0/prefect_postgres_sensors/
+-rwxrwxrwx   0 james     (1000) james     (1000)      129 2023-05-26 11:56:29.000000 prefect_postgres_sensors-0.5.0/prefect_postgres_sensors/__init__.py
+drwxrwxrwx   0 james     (1000) james     (1000)        0 2023-05-26 12:13:33.570248 prefect_postgres_sensors-0.5.0/prefect_postgres_sensors.egg-info/
+-rwxrwxrwx   0 james     (1000) james     (1000)      271 2023-05-26 12:13:31.000000 prefect_postgres_sensors-0.5.0/prefect_postgres_sensors.egg-info/PKG-INFO
+-rwxrwxrwx   0 james     (1000) james     (1000)      302 2023-05-26 12:13:31.000000 prefect_postgres_sensors-0.5.0/prefect_postgres_sensors.egg-info/SOURCES.txt
+-rwxrwxrwx   0 james     (1000) james     (1000)        1 2023-05-26 12:13:31.000000 prefect_postgres_sensors-0.5.0/prefect_postgres_sensors.egg-info/dependency_links.txt
+-rwxrwxrwx   0 james     (1000) james     (1000)       26 2023-05-26 12:13:31.000000 prefect_postgres_sensors-0.5.0/prefect_postgres_sensors.egg-info/requires.txt
+-rwxrwxrwx   0 james     (1000) james     (1000)       25 2023-05-26 12:13:31.000000 prefect_postgres_sensors-0.5.0/prefect_postgres_sensors.egg-info/top_level.txt
+-rwxrwxrwx   0 james     (1000) james     (1000)       38 2023-05-26 12:13:33.646222 prefect_postgres_sensors-0.5.0/setup.cfg
+-rwxrwxrwx   0 james     (1000) james     (1000)      356 2023-05-26 12:12:43.000000 prefect_postgres_sensors-0.5.0/setup.py
```

### Comparing `prefect_postgres_sensors-0.4.0/LICENSE` & `prefect_postgres_sensors-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect_postgres_sensors-0.4.0/README.md` & `prefect_postgres_sensors-0.5.0/README.md`

 * *Files identical despite different names*

