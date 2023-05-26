# Comparing `tmp/prefect_postgres_sensors-0.1.0.tar.gz` & `tmp/prefect_postgres_sensors-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect_postgres_sensors-0.1.0.tar", last modified: Fri May 26 11:09:47 2023, max compression
+gzip compressed data, was "prefect_postgres_sensors-0.2.0.tar", last modified: Fri May 26 11:13:29 2023, max compression
```

## Comparing `prefect_postgres_sensors-0.1.0.tar` & `prefect_postgres_sensors-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0 james     (1000) james     (1000)        0 2023-05-26 11:09:47.951087 prefect_postgres_sensors-0.1.0/
--rwxrwxrwx   0 james     (1000) james     (1000)      249 2023-05-26 11:09:47.945084 prefect_postgres_sensors-0.1.0/PKG-INFO
--rwxrwxrwx   0 james     (1000) james     (1000)     3221 2023-05-26 11:08:30.000000 prefect_postgres_sensors-0.1.0/README.md
-drwxrwxrwx   0 james     (1000) james     (1000)        0 2023-05-26 11:09:47.617079 prefect_postgres_sensors-0.1.0/prefect_postgres_sensors/
--rwxrwxrwx   0 james     (1000) james     (1000)        0 2023-05-26 10:21:18.000000 prefect_postgres_sensors-0.1.0/prefect_postgres_sensors/__init__.py
--rwxrwxrwx   0 james     (1000) james     (1000)     1089 2023-05-26 10:22:22.000000 prefect_postgres_sensors-0.1.0/prefect_postgres_sensors/table_update_sensor.py
-drwxrwxrwx   0 james     (1000) james     (1000)        0 2023-05-26 11:09:47.882081 prefect_postgres_sensors-0.1.0/prefect_postgres_sensors.egg-info/
--rwxrwxrwx   0 james     (1000) james     (1000)      249 2023-05-26 11:09:47.000000 prefect_postgres_sensors-0.1.0/prefect_postgres_sensors.egg-info/PKG-INFO
--rwxrwxrwx   0 james     (1000) james     (1000)      342 2023-05-26 11:09:47.000000 prefect_postgres_sensors-0.1.0/prefect_postgres_sensors.egg-info/SOURCES.txt
--rwxrwxrwx   0 james     (1000) james     (1000)        1 2023-05-26 11:09:47.000000 prefect_postgres_sensors-0.1.0/prefect_postgres_sensors.egg-info/dependency_links.txt
--rwxrwxrwx   0 james     (1000) james     (1000)       26 2023-05-26 11:09:47.000000 prefect_postgres_sensors-0.1.0/prefect_postgres_sensors.egg-info/requires.txt
--rwxrwxrwx   0 james     (1000) james     (1000)       25 2023-05-26 11:09:47.000000 prefect_postgres_sensors-0.1.0/prefect_postgres_sensors.egg-info/top_level.txt
--rwxrwxrwx   0 james     (1000) james     (1000)       38 2023-05-26 11:09:47.954083 prefect_postgres_sensors-0.1.0/setup.cfg
--rwxrwxrwx   0 james     (1000) james     (1000)      356 2023-05-26 10:23:57.000000 prefect_postgres_sensors-0.1.0/setup.py
+drwxrwxrwx   0 james     (1000) james     (1000)        0 2023-05-26 11:13:29.638169 prefect_postgres_sensors-0.2.0/
+-rwxrwxrwx   0 james     (1000) james     (1000)      249 2023-05-26 11:13:29.627166 prefect_postgres_sensors-0.2.0/PKG-INFO
+-rwxrwxrwx   0 james     (1000) james     (1000)     3221 2023-05-26 11:08:30.000000 prefect_postgres_sensors-0.2.0/README.md
+drwxrwxrwx   0 james     (1000) james     (1000)        0 2023-05-26 11:13:29.362170 prefect_postgres_sensors-0.2.0/prefect_postgres_sensors/
+-rwxrwxrwx   0 james     (1000) james     (1000)        0 2023-05-26 10:21:18.000000 prefect_postgres_sensors-0.2.0/prefect_postgres_sensors/__init__.py
+-rwxrwxrwx   0 james     (1000) james     (1000)     1089 2023-05-26 10:22:22.000000 prefect_postgres_sensors-0.2.0/prefect_postgres_sensors/table_update_sensor.py
+drwxrwxrwx   0 james     (1000) james     (1000)        0 2023-05-26 11:13:29.575167 prefect_postgres_sensors-0.2.0/prefect_postgres_sensors.egg-info/
+-rwxrwxrwx   0 james     (1000) james     (1000)      249 2023-05-26 11:13:27.000000 prefect_postgres_sensors-0.2.0/prefect_postgres_sensors.egg-info/PKG-INFO
+-rwxrwxrwx   0 james     (1000) james     (1000)      342 2023-05-26 11:13:28.000000 prefect_postgres_sensors-0.2.0/prefect_postgres_sensors.egg-info/SOURCES.txt
+-rwxrwxrwx   0 james     (1000) james     (1000)        1 2023-05-26 11:13:27.000000 prefect_postgres_sensors-0.2.0/prefect_postgres_sensors.egg-info/dependency_links.txt
+-rwxrwxrwx   0 james     (1000) james     (1000)       26 2023-05-26 11:13:28.000000 prefect_postgres_sensors-0.2.0/prefect_postgres_sensors.egg-info/requires.txt
+-rwxrwxrwx   0 james     (1000) james     (1000)       25 2023-05-26 11:13:28.000000 prefect_postgres_sensors-0.2.0/prefect_postgres_sensors.egg-info/top_level.txt
+-rwxrwxrwx   0 james     (1000) james     (1000)       38 2023-05-26 11:13:29.640171 prefect_postgres_sensors-0.2.0/setup.cfg
+-rwxrwxrwx   0 james     (1000) james     (1000)      356 2023-05-26 11:12:56.000000 prefect_postgres_sensors-0.2.0/setup.py
```

### Comparing `prefect_postgres_sensors-0.1.0/README.md` & `prefect_postgres_sensors-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `prefect_postgres_sensors-0.1.0/prefect_postgres_sensors/table_update_sensor.py` & `prefect_postgres_sensors-0.2.0/prefect_postgres_sensors/table_update_sensor.py`

 * *Files identical despite different names*

