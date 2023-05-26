# Comparing `tmp/macrometa-target-bigquery-0.0.7.tar.gz` & `tmp/macrometa-target-bigquery-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-bigquery-0.0.7.tar", last modified: Thu Apr 20 10:26:20 2023, max compression
+gzip compressed data, was "macrometa-target-bigquery-0.0.8.tar", last modified: Fri May 26 08:10:03 2023, max compression
```

## Comparing `macrometa-target-bigquery-0.0.7.tar` & `macrometa-target-bigquery-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:26:20.417810 macrometa-target-bigquery-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    10409 2023-04-20 10:26:00.000000 macrometa-target-bigquery-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21167 2023-04-20 10:26:20.417810 macrometa-target-bigquery-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20733 2023-04-20 10:26:00.000000 macrometa-target-bigquery-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:26:20.417810 macrometa-target-bigquery-0.0.7/macrometa_target_bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)    29847 2023-04-20 10:26:00.000000 macrometa-target-bigquery-0.0.7/macrometa_target_bigquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25667 2023-04-20 10:26:00.000000 macrometa-target-bigquery-0.0.7/macrometa_target_bigquery/db_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-20 10:26:00.000000 macrometa-target-bigquery-0.0.7/macrometa_target_bigquery/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-20 10:26:00.000000 macrometa-target-bigquery-0.0.7/macrometa_target_bigquery/flattening.py
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-04-20 10:26:00.000000 macrometa-target-bigquery-0.0.7/macrometa_target_bigquery/sql_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-20 10:26:00.000000 macrometa-target-bigquery-0.0.7/macrometa_target_bigquery/stream_ref_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-04-20 10:26:00.000000 macrometa-target-bigquery-0.0.7/macrometa_target_bigquery/stream_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:26:20.417810 macrometa-target-bigquery-0.0.7/macrometa_target_bigquery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21167 2023-04-20 10:26:20.000000 macrometa-target-bigquery-0.0.7/macrometa_target_bigquery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-20 10:26:20.000000 macrometa-target-bigquery-0.0.7/macrometa_target_bigquery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 10:26:20.000000 macrometa-target-bigquery-0.0.7/macrometa_target_bigquery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-20 10:26:20.000000 macrometa-target-bigquery-0.0.7/macrometa_target_bigquery.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-20 10:26:20.000000 macrometa-target-bigquery-0.0.7/macrometa_target_bigquery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-20 10:26:20.000000 macrometa-target-bigquery-0.0.7/macrometa_target_bigquery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 10:26:20.417810 macrometa-target-bigquery-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-20 10:26:00.000000 macrometa-target-bigquery-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:10:03.145582 macrometa-target-bigquery-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    10409 2023-05-26 08:09:46.000000 macrometa-target-bigquery-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21167 2023-05-26 08:10:03.145582 macrometa-target-bigquery-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20733 2023-05-26 08:09:46.000000 macrometa-target-bigquery-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:10:03.145582 macrometa-target-bigquery-0.0.8/macrometa_target_bigquery/
+-rw-r--r--   0 runner    (1001) docker     (123)    27638 2023-05-26 08:09:46.000000 macrometa-target-bigquery-0.0.8/macrometa_target_bigquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25010 2023-05-26 08:09:46.000000 macrometa-target-bigquery-0.0.8/macrometa_target_bigquery/db_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-26 08:09:46.000000 macrometa-target-bigquery-0.0.8/macrometa_target_bigquery/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-26 08:09:46.000000 macrometa-target-bigquery-0.0.8/macrometa_target_bigquery/flattening.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-26 08:09:46.000000 macrometa-target-bigquery-0.0.8/macrometa_target_bigquery/sql_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-26 08:09:46.000000 macrometa-target-bigquery-0.0.8/macrometa_target_bigquery/stream_ref_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-05-26 08:09:46.000000 macrometa-target-bigquery-0.0.8/macrometa_target_bigquery/stream_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:10:03.145582 macrometa-target-bigquery-0.0.8/macrometa_target_bigquery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21167 2023-05-26 08:10:03.000000 macrometa-target-bigquery-0.0.8/macrometa_target_bigquery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-26 08:10:03.000000 macrometa-target-bigquery-0.0.8/macrometa_target_bigquery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 08:10:03.000000 macrometa-target-bigquery-0.0.8/macrometa_target_bigquery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-26 08:10:03.000000 macrometa-target-bigquery-0.0.8/macrometa_target_bigquery.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-26 08:10:03.000000 macrometa-target-bigquery-0.0.8/macrometa_target_bigquery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-26 08:10:03.000000 macrometa-target-bigquery-0.0.8/macrometa_target_bigquery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 08:10:03.145582 macrometa-target-bigquery-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-26 08:09:46.000000 macrometa-target-bigquery-0.0.8/setup.py
```

### Comparing `macrometa-target-bigquery-0.0.7/LICENSE` & `macrometa-target-bigquery-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-bigquery-0.0.7/PKG-INFO` & `macrometa-target-bigquery-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-bigquery
-Version: 0.0.7
+Version: 0.0.8
 Summary: Macrometa target bigquery connector for loading data to BigQuery
 Home-page: https://github.com/Macrometacorp/macrometa-target-bigquery
 Author: Macrometa
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `macrometa-target-bigquery-0.0.7/README.md` & `macrometa-target-bigquery-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `macrometa-target-bigquery-0.0.7/macrometa_target_bigquery/__init__.py` & `macrometa-target-bigquery-0.0.8/macrometa_target_bigquery/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,22 +89,24 @@
     def config(self) -> list[ConfigProperty]:
         """Get configuration parameters for the connector."""
         return [
             ConfigProperty('project_id', 'Project ID', ConfigAttributeType.STRING, True, False,
                            description='BigQuery project ID.',
                            placeholder_value='my_project_id'),
             ConfigProperty('credentials_file', 'Credentials JSON file', ConfigAttributeType.FILE, True, False,
-                           description='Fully qualified path to client_secrets.json for your service account. See the '
+                           description='Content of the credentials.json file for your service account. See the '
                                        '"Activate the Google BigQuery API" section of the repository\'s README and '
                                        'https://cloud.google.com/docs/authentication/production.',
-                           placeholder_value='credentials.json contents'),
-            ConfigProperty('target_schema', 'Target Schema/Dataset', ConfigAttributeType.STRING, True, False,
-                           description='Name of the schema/dataset where the tables will be created.'),
-            ConfigProperty('target_table', 'Target Table', ConfigAttributeType.STRING, True, False,
-                           description='Name of the bigquery table. The table will be created if it does not exist'),
+                           placeholder_value='my_credentials'),
+            ConfigProperty('target_schema', 'Target Schema/Dataset', ConfigAttributeType.STRING, True, True,
+                           description='Name of the schema/dataset where the tables will be created.',
+                           placeholder_value='my_schema'),
+            ConfigProperty('target_table', 'Target Table', ConfigAttributeType.STRING, True, True,
+                           description='Name of the bigquery table. The table will be created if it does not exist.',
+                           placeholder_value='my_table'),
             ConfigProperty('location', 'Location', ConfigAttributeType.STRING, False, False,
                            description='Region where BigQuery stores your dataset.'),
             ConfigProperty('default_target_schema_select_permission', 'Target Schema privileges',
                            ConfigAttributeType.STRING, False, False,
                            description='Grant USAGE privilege on newly created schemas and grant SELECT privilege on '
                                        'newly created table.',
                            placeholder_value='SELECT'),
@@ -112,66 +114,48 @@
                            description='Maximum number of rows in each batch. At the end of each batch, '
                                        'the rows in the batch are loaded into BigQuery.',
                            default_value='10000'),
             ConfigProperty('batch_wait_limit_seconds', 'Batch Wait Limit (Seconds)',
                            ConfigAttributeType.INT, False, False,
                            description='Maximum time to wait for batch to reach batch_size_rows.',
                            placeholder_value='60'),
-            ConfigProperty('flush_all_streams', 'Flush All Streams', ConfigAttributeType.BOOLEAN, False, False,
-                           description='Flush and load every stream into BigQuery when one batch is full. Warning: '
-                                       'This may trigger transfer of data with low number of records, '
-                                       'and may cause performance problems.',
-                           default_value='false'),
-            ConfigProperty('parallelism', 'Parallelism', ConfigAttributeType.INT, False, False,
-                           description='The number of threads used to flush tables. 0 will create a thread for each '
-                                       'stream, up to parallelism_max. -1 will create a thread for each CPU core. '
-                                       'Any other positive number will create that number of threads, up to '
-                                       'parallelism_max.',
-                           default_value='0'),
-            ConfigProperty('max_parallelism', 'Maximum Parallelism', ConfigAttributeType.INT, False, False,
-                           description='Max number of parallel threads to use when flushing tables.',
-                           default_value='16'),
             ConfigProperty('add_metadata_columns', 'Add Metadata Columns', ConfigAttributeType.BOOLEAN, False, False,
                            description='Metadata columns add extra row level information about data ingestions, '
-                                       '(i.e. when was the row read in source, when was inserted or deleted in bigquery'
-                                       'etc.) Metadata columns are creating automatically by adding extra columns to '
+                                       '(i.e. when was the row read in source, when was inserted or deleted in bigquery, '
+                                       'etc.) Metadata columns are created automatically by adding extra columns to '
                                        'the tables with a column prefix _sdc_. The column names are following the '
                                        'stitch naming conventions documented at '
-                                       'https://www.stitchdata.com/docs/data-structure/integration-schemas#sdc-columns.'
-                                       'Enabling metadata columns will flag the deleted rows by setting the _'
-                                       'sdc_deleted_at metadata column. Without the add_metadata_columns option the '
-                                       'deleted rows from singer taps will not be recognisable in BigQuery.',
+                                       'https://www.stitchdata.com/docs/data-structure/integration-schemas#sdc-columns.',
                            default_value='false'),
             ConfigProperty('hard_delete', 'Hard Delete', ConfigAttributeType.BOOLEAN, False, False,
                            description='When hard_delete option is true then DELETE SQL commands will be performed in'
-                                       'BigQuery to delete rows in tables. It\'s achieved by continuously checking the'
-                                       'sdc_deleted_at metadata column sent by the singer tap. Due to deleting rows '
+                                       ' BigQuery to delete rows in tables. It\'s achieved by continuously checking the'
+                                       ' _sdc_deleted_at metadata column sent by the data source. Due to deleting rows '
                                        'requires metadata columns, hard_delete option automatically enables the '
                                        'add_metadata_columns option as well.',
                            default_value='false'),
             ConfigProperty('data_flattening_max_level', 'Data Flattening Max Level',
                            ConfigAttributeType.INT, False, False,
                            description='Object type RECORD items from data source can be loaded into VARIANT columns as JSON '
                                        '(default) or we can flatten the schema by creating columns automatically.'
-                                       'When value is 0 (default) then flattening functionality is turned off.',
+                                       ' When value is 0 (default) then flattening functionality is turned off.',
                            default_value='0'),
             ConfigProperty('primary_key_required', 'Primary Key Required', ConfigAttributeType.BOOLEAN, False, False,
-                           description='Log based and Incremental replications on tables with no Primary Key cause '
-                                       'duplicates when merging UPDATE events. When set to true, stop loading data if '
-                                       'no Primary Key is defined.',
+                           description='Tables with no Primary Key cause duplicates when merging UPDATE events. '
+                                       'When set to true, stop loading data if no Primary Key is defined.',
                            default_value='true'),
             ConfigProperty('validate_records', 'Validate Records', ConfigAttributeType.BOOLEAN, False, False,
                            description='Validate every single record message to the corresponding JSON schema. '
                                        'This option is disabled by default and invalid RECORD messages will fail only '
                                        'at load time by BigQuery. Enabling this option will detect invalid records '
                                        'earlier but could cause performance degradation.',
                            default_value='false'),
             ConfigProperty('temp_schema', 'Temporary Schema', ConfigAttributeType.STRING, False, False,
                            description='Name of the schema where the temporary tables will be created. Will default to '
-                                       'the same schema as the target tables',
+                                       'the same schema as the target tables.',
                            placeholder_value='my_temp_schema'),
             ConfigProperty('use_partition_pruning', 'Use Partition Pruning', ConfigAttributeType.BOOLEAN, False, False,
                            description='If true then BigQuery table partition pruning will be used for tables which '
                                        'have partitioning enabled. This partitioning should be on a column which is '
                                        'immutable such as an integer primary key or a created_at column. The '
                                        'partitioning should be set up manually by the user. This feature can '
                                        'dramatically reduce the cost of each MERGE for large tables.',
@@ -194,15 +178,14 @@
     extended_schema_message = schema_message
     extended_schema_message['schema']['properties']['_sdc_extracted_at'] = {'type': ['null', 'string'],
                                                                             'format': 'date-time'}
     extended_schema_message['schema']['properties']['_sdc_batched_at'] = {'type': ['null', 'string'],
                                                                           'format': 'date-time'}
     extended_schema_message['schema']['properties']['_sdc_deleted_at'] = {'type': ['null', 'string'],
                                                                           'format': 'date-time'}
-    extended_schema_message['schema']['properties']['_sdc_table_version'] = {'type': ['null', 'integer']}
 
     return extended_schema_message
 
 
 def emit_state(state):
     if state is not None:
         line = json.dumps(state)
@@ -368,24 +351,15 @@
 
             records_to_load[stream] = {}
             row_count[stream] = 0
             total_row_count[stream] = 0
 
         elif t == 'ACTIVATE_VERSION':
             stream = o['stream']
-            version = o['version']
-
-            if hard_delete_mapping.get(stream, default_hard_delete):
-                if stream in stream_to_sync:
-                    LOGGER.debug('ACTIVATE_VERSION message, clearing records with versions other than {}'.format(version))
-                    stream_to_sync[stream].activate_table_version(stream, version)
-                else:
-                    LOGGER.warn('ACTIVATE_VERSION message, unknown stream {}'.format(stream))
-            else:
-                LOGGER.debug('ACTIVATE_VERSION message - ignoring due hard_delete not set')
+            LOGGER.debug('ACTIVATE_VERSION message - ignoring')
 
         elif t == 'STATE':
             LOGGER.debug('Setting state to {}'.format(o['value']))
             state = o['value']
 
             # Initially set flushed state
             if not flushed_state:
```

### Comparing `macrometa-target-bigquery-0.0.7/macrometa_target_bigquery/db_sync.py` & `macrometa-target-bigquery-0.0.8/macrometa_target_bigquery/db_sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -424,27 +424,14 @@
         table_ref = self.ref_helper.get_table_ref(self.connection_config['target_table'], is_temporary=False)
         table_id = table_ref.table_id
         query = "DELETE FROM {} WHERE _sdc_deleted_at IS NOT NULL".format(
                     sql_utils.safe_table_ref(table_ref))
         logger.info("Deleting rows from '{}' table... {}".format(table_id, query))
         logger.info("DELETE {}".format(self.query(query).result().total_rows))
 
-    def activate_table_version(self, stream, version):
-        stream_schema_message = self.stream_schema_message
-        stream = stream_schema_message['stream']
-
-        table_ref = self.ref_helper.get_table_ref(self.connection_config['target_table'], is_temporary=False)
-        table_id = table_ref.table_id
-
-        query = "DELETE FROM {} WHERE _sdc_table_version != {}".format(
-                    sql_utils.safe_table_ref(table_ref),
-                    version)
-        logger.info("Removing rows from previous versions from '{}' table... {}".format(table_id, query))
-        logger.info("DELETE {}".format(self.query(query).result().total_rows))
-
     def create_schema_if_not_exists(self):
         schema_name = self.schema_name
         temp_schema = self.connection_config.get('temp_schema', self.schema_name)
         project_id = self.connection_config['project_id']
 
         for schema in set([schema_name, temp_schema]):
             try:
```

### Comparing `macrometa-target-bigquery-0.0.7/macrometa_target_bigquery/exceptions.py` & `macrometa-target-bigquery-0.0.8/macrometa_target_bigquery/exceptions.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-bigquery-0.0.7/macrometa_target_bigquery/flattening.py` & `macrometa-target-bigquery-0.0.8/macrometa_target_bigquery/flattening.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-bigquery-0.0.7/macrometa_target_bigquery/sql_utils.py` & `macrometa-target-bigquery-0.0.8/macrometa_target_bigquery/sql_utils.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-bigquery-0.0.7/macrometa_target_bigquery/stream_ref_helper.py` & `macrometa-target-bigquery-0.0.8/macrometa_target_bigquery/stream_ref_helper.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-bigquery-0.0.7/macrometa_target_bigquery/stream_utils.py` & `macrometa-target-bigquery-0.0.8/macrometa_target_bigquery/stream_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,10 +97,9 @@
         except TypeError:
             return None
 
     extended_record = record_message['record']
     extended_record['_sdc_extracted_at'] = parse_datetime(record_message.get('time_extracted', datetime.now()))
     extended_record['_sdc_batched_at'] = datetime.now()
     extended_record['_sdc_deleted_at'] = parse_datetime(record_message.get('record', {}).get('_sdc_deleted_at'))
-    extended_record['_sdc_table_version'] = record_message.get('version')
 
     return extended_record
```

### Comparing `macrometa-target-bigquery-0.0.7/macrometa_target_bigquery.egg-info/PKG-INFO` & `macrometa-target-bigquery-0.0.8/macrometa_target_bigquery.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-bigquery
-Version: 0.0.7
+Version: 0.0.8
 Summary: Macrometa target bigquery connector for loading data to BigQuery
 Home-page: https://github.com/Macrometacorp/macrometa-target-bigquery
 Author: Macrometa
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `macrometa-target-bigquery-0.0.7/macrometa_target_bigquery.egg-info/SOURCES.txt` & `macrometa-target-bigquery-0.0.8/macrometa_target_bigquery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `macrometa-target-bigquery-0.0.7/setup.py` & `macrometa-target-bigquery-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(name="macrometa-target-bigquery",
-      version='0.0.7',
+      version='0.0.8',
       description="Macrometa target bigquery connector for loading data to BigQuery",
       long_description=long_description,
       long_description_content_type='text/markdown',
       author="Macrometa",
       url='https://github.com/Macrometacorp/macrometa-target-bigquery',
       classifiers=[
           'License :: OSI Approved :: Apache Software License',
```

