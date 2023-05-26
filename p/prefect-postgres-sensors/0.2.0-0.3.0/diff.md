# Comparing `tmp/prefect_postgres_sensors-0.2.0.tar.gz` & `tmp/prefect_postgres_sensors-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect_postgres_sensors-0.2.0.tar", last modified: Fri May 26 11:13:29 2023, max compression
+gzip compressed data, was "prefect_postgres_sensors-0.3.0.tar", last modified: Fri May 26 11:32:19 2023, max compression
```

## Comparing `prefect_postgres_sensors-0.2.0.tar` & `prefect_postgres_sensors-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0 james     (1000) james     (1000)        0 2023-05-26 11:13:29.638169 prefect_postgres_sensors-0.2.0/
--rwxrwxrwx   0 james     (1000) james     (1000)      249 2023-05-26 11:13:29.627166 prefect_postgres_sensors-0.2.0/PKG-INFO
--rwxrwxrwx   0 james     (1000) james     (1000)     3221 2023-05-26 11:08:30.000000 prefect_postgres_sensors-0.2.0/README.md
-drwxrwxrwx   0 james     (1000) james     (1000)        0 2023-05-26 11:13:29.362170 prefect_postgres_sensors-0.2.0/prefect_postgres_sensors/
--rwxrwxrwx   0 james     (1000) james     (1000)        0 2023-05-26 10:21:18.000000 prefect_postgres_sensors-0.2.0/prefect_postgres_sensors/__init__.py
--rwxrwxrwx   0 james     (1000) james     (1000)     1089 2023-05-26 10:22:22.000000 prefect_postgres_sensors-0.2.0/prefect_postgres_sensors/table_update_sensor.py
-drwxrwxrwx   0 james     (1000) james     (1000)        0 2023-05-26 11:13:29.575167 prefect_postgres_sensors-0.2.0/prefect_postgres_sensors.egg-info/
--rwxrwxrwx   0 james     (1000) james     (1000)      249 2023-05-26 11:13:27.000000 prefect_postgres_sensors-0.2.0/prefect_postgres_sensors.egg-info/PKG-INFO
--rwxrwxrwx   0 james     (1000) james     (1000)      342 2023-05-26 11:13:28.000000 prefect_postgres_sensors-0.2.0/prefect_postgres_sensors.egg-info/SOURCES.txt
--rwxrwxrwx   0 james     (1000) james     (1000)        1 2023-05-26 11:13:27.000000 prefect_postgres_sensors-0.2.0/prefect_postgres_sensors.egg-info/dependency_links.txt
--rwxrwxrwx   0 james     (1000) james     (1000)       26 2023-05-26 11:13:28.000000 prefect_postgres_sensors-0.2.0/prefect_postgres_sensors.egg-info/requires.txt
--rwxrwxrwx   0 james     (1000) james     (1000)       25 2023-05-26 11:13:28.000000 prefect_postgres_sensors-0.2.0/prefect_postgres_sensors.egg-info/top_level.txt
--rwxrwxrwx   0 james     (1000) james     (1000)       38 2023-05-26 11:13:29.640171 prefect_postgres_sensors-0.2.0/setup.cfg
--rwxrwxrwx   0 james     (1000) james     (1000)      356 2023-05-26 11:12:56.000000 prefect_postgres_sensors-0.2.0/setup.py
+drwxrwxrwx   0 james     (1000) james     (1000)        0 2023-05-26 11:32:19.194517 prefect_postgres_sensors-0.3.0/
+-rwxrwxrwx   0 james     (1000) james     (1000)     1074 2023-05-17 13:09:12.000000 prefect_postgres_sensors-0.3.0/LICENSE
+-rwxrwxrwx   0 james     (1000) james     (1000)      271 2023-05-26 11:32:19.183513 prefect_postgres_sensors-0.3.0/PKG-INFO
+-rwxrwxrwx   0 james     (1000) james     (1000)     3603 2023-05-26 11:26:27.000000 prefect_postgres_sensors-0.3.0/README.md
+drwxrwxrwx   0 james     (1000) james     (1000)        0 2023-05-26 11:32:18.888255 prefect_postgres_sensors-0.3.0/prefect_postgres_sensors/
+-rwxrwxrwx   0 james     (1000) james     (1000)      128 2023-05-26 11:30:24.000000 prefect_postgres_sensors-0.3.0/prefect_postgres_sensors/__init__.py
+-rwxrwxrwx   0 james     (1000) james     (1000)     1089 2023-05-26 10:22:22.000000 prefect_postgres_sensors-0.3.0/prefect_postgres_sensors/table_update_sensor.py
+drwxrwxrwx   0 james     (1000) james     (1000)        0 2023-05-26 11:32:19.139545 prefect_postgres_sensors-0.3.0/prefect_postgres_sensors.egg-info/
+-rwxrwxrwx   0 james     (1000) james     (1000)      271 2023-05-26 11:32:17.000000 prefect_postgres_sensors-0.3.0/prefect_postgres_sensors.egg-info/PKG-INFO
+-rwxrwxrwx   0 james     (1000) james     (1000)      350 2023-05-26 11:32:17.000000 prefect_postgres_sensors-0.3.0/prefect_postgres_sensors.egg-info/SOURCES.txt
+-rwxrwxrwx   0 james     (1000) james     (1000)        1 2023-05-26 11:32:17.000000 prefect_postgres_sensors-0.3.0/prefect_postgres_sensors.egg-info/dependency_links.txt
+-rwxrwxrwx   0 james     (1000) james     (1000)       26 2023-05-26 11:32:17.000000 prefect_postgres_sensors-0.3.0/prefect_postgres_sensors.egg-info/requires.txt
+-rwxrwxrwx   0 james     (1000) james     (1000)       25 2023-05-26 11:32:17.000000 prefect_postgres_sensors-0.3.0/prefect_postgres_sensors.egg-info/top_level.txt
+-rwxrwxrwx   0 james     (1000) james     (1000)       38 2023-05-26 11:32:19.196516 prefect_postgres_sensors-0.3.0/setup.cfg
+-rwxrwxrwx   0 james     (1000) james     (1000)      356 2023-05-26 11:31:51.000000 prefect_postgres_sensors-0.3.0/setup.py
```

### Comparing `prefect_postgres_sensors-0.2.0/README.md` & `prefect_postgres_sensors-0.3.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,30 @@
-Certainly! Here's an example of an elaborate GitHub README file for the "prefect_postgres_sensors" project:
-
 # Prefect PostgreSQL Sensors
 
+[![PyPI version](https://badge.fury.io/py/prefect-postgres-sensors.svg)](https://badge.fury.io/py/prefect-postgres-sensors)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
-[![PyPI](https://img.shields.io/pypi/v/prefect_postgres_sensors.svg)](https://pypi.org/project/prefect_postgres_sensors/)
+[![Build Status](https://travis-ci.com/James-Wachuka/prefect-postgres-sensors.svg?branch=main)](https://travis-ci.com/James-Wachuka/prefect-postgres-sensors)
+[![Coverage Status](https://coveralls.io/repos/github/James-Wachuka/prefect-postgres-sensors/badge.svg?branch=main)](https://coveralls.io/github/James-Wachuka/prefect-postgres-sensors?branch=main)
+[![Downloads](https://img.shields.io/pypi/dm/prefect-postgres-sensors.svg)](https://pypi.org/project/prefect-postgres-sensors/)
+[![Stars](https://img.shields.io/github/stars/James-Wachuka/prefect-postgres-sensors.svg?style=social)](https://github.com/James-Wachuka/prefect-postgres-sensors/stargazers)
+
 
 The `prefect_postgres_sensors` package provides Prefect sensors for monitoring changes or conditions within a PostgreSQL database.
 
 ## Features
 
 - **TableUpdateSensor**: Monitors the last update timestamp of a table in a PostgreSQL database.
 - **monitor_table_row_count**: Retrieves the row count of a table in a PostgreSQL database.
 - **monitor_column_changes**: Detects changes in specific columns of a table in a PostgreSQL database.
 
 ## Installation
 
 Install the package via pip:
 
-```shell
+```
 pip install prefect_postgres_sensors
 ```
 
 ## Usage
 
 Here's an example of how you can use the `prefect_postgres_sensors` package:
 
@@ -29,31 +32,31 @@
 from prefect import Flow
 from prefect_postgres_sensors import TableUpdateSensor, monitor_table_row_count, monitor_column_changes
 
 # Define your PostgreSQL connection details
 postgres_config = {
     "host": "localhost",
     "port": 5432,
-    "database": "my_database",
-    "user": "my_user",
-    "password": "my_password"
+    "database": "database",
+    "user": "user",
+    "password": "password"
 }
 
 # Create a TableUpdateSensor to monitor the last update timestamp of a table
 table_update_sensor = TableUpdateSensor(
-    table_name="my_table",
-    last_updated_column="updated_at",
+    table_name="table",
+    last_updated_column="last_updated",
     **postgres_config
 )
 
 # Create a task to monitor the row count of a table
-row_count_task = monitor_table_row_count("my_table", **postgres_config)
+row_count_task = monitor_table_row_count("table, **postgres_config)
 
 # Create a task to monitor changes in a specific column of a table
-column_changes_task = monitor_column_changes("my_table", "my_column", "last_value", **postgres_config)
+column_changes_task = monitor_column_changes("table", "column", "last_value", **postgres_config)
 
 # Define a Prefect flow
 with Flow("PostgreSQL Monitoring") as flow:
     last_updated = table_update_sensor()
     row_count = row_count_task()
     changed_rows = column_changes_task()
 
@@ -63,31 +66,31 @@
     print(f"Row count: {row_count}")
     print(f"Changed rows: {changed_rows}")
 
 # Run the Prefect flow
 flow.run()
 ```
 
-Make sure to replace the placeholder values (`my_table`, `updated_at`, `my_column`, `last_value`, etc.) with the actual table name, column name, and values you want to monitor in your PostgreSQL database.
+Make sure to replace the placeholder values (`table`, `last_update`, `name`, `Mwangi`, etc.) with the actual table name, column name, and values you want to monitor in your PostgreSQL database.
 
 ## License
 
 This project is licensed under the [MIT License](LICENSE).
 
 ## Contributing
 
-Contributions are welcome! Please see the [Contributing Guidelines](CONTRIBUTING.md) for more details.
+Contributions are welcome!
 
 ## Acknowledgments
 
-This package was inspired by the need to monitor PostgreSQL databases using Prefect. Special thanks to the contributors and the Prefect team.
+This package was inspired by the need to monitor PostgreSQL databases using Prefect.
 
 ## Support
 
-For any questions or issues, please open an [issue](https://github.com/your_username/prefect_postgres_sensors/issues) on GitHub.
+For any questions or issues, please open an [issue](https://github.com/James-Wachuka/prefect-postgres-sensors/issues) on GitHub.
 
 ## Related Projects
 
 - [Prefect](https://github.com/PrefectHQ/prefect): The core Prefect library for building, scheduling, and monitoring workflows.
 
 ## Release Notes
```

### Comparing `prefect_postgres_sensors-0.2.0/prefect_postgres_sensors/table_update_sensor.py` & `prefect_postgres_sensors-0.3.0/prefect_postgres_sensors/table_update_sensor.py`

 * *Files identical despite different names*

