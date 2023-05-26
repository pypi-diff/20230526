# Comparing `tmp/faker_cli-0.0.5.tar.gz` & `tmp/faker_cli-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faker_cli-0.0.5.tar", max compression
+gzip compressed data, was "faker_cli-0.1.0.tar", max compression
```

## Comparing `faker_cli-0.0.5.tar` & `faker_cli-0.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2023-05-26 04:27:59.656983 faker_cli-0.0.5/LICENSE
--rw-r--r--   0        0        0     2829 2023-05-26 04:27:59.656983 faker_cli-0.0.5/README.md
--rw-r--r--   0        0        0        0 2023-05-26 04:27:59.656983 faker_cli-0.0.5/faker_cli/__init__.py
--rw-r--r--   0        0        0     2074 2023-05-26 04:27:59.656983 faker_cli-0.0.5/faker_cli/cli.py
--rw-r--r--   0        0        0    15114 2023-05-26 04:27:59.656983 faker_cli-0.0.5/faker_cli/templates.py
--rw-r--r--   0        0        0      809 2023-05-26 04:27:59.656983 faker_cli-0.0.5/faker_cli/writer.py
--rw-r--r--   0        0        0      461 2023-05-26 04:28:26.852784 faker_cli-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3302 1970-01-01 00:00:00.000000 faker_cli-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-26 07:16:29.115396 faker_cli-0.1.0/LICENSE
+-rw-r--r--   0        0        0     2829 2023-05-26 07:16:29.115396 faker_cli-0.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-26 07:16:29.115396 faker_cli-0.1.0/faker_cli/__init__.py
+-rw-r--r--   0        0        0     2343 2023-05-26 07:16:29.119396 faker_cli-0.1.0/faker_cli/cli.py
+-rw-r--r--   0        0        0    26455 2023-05-26 07:16:29.119396 faker_cli-0.1.0/faker_cli/templates.py
+-rw-r--r--   0        0        0      809 2023-05-26 07:16:29.119396 faker_cli-0.1.0/faker_cli/writer.py
+-rw-r--r--   0        0        0      461 2023-05-26 07:16:53.423462 faker_cli-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3302 1970-01-01 00:00:00.000000 faker_cli-0.1.0/PKG-INFO
```

### Comparing `faker_cli-0.0.5/LICENSE` & `faker_cli-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `faker_cli-0.0.5/README.md` & `faker_cli-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `faker_cli-0.0.5/faker_cli/cli.py` & `faker_cli-0.1.0/faker_cli/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from faker import Faker
 import click
 import sys
-from faker_cli.templates import S3AccessLogs, S3AccessWriter, CloudTrailLogs
+from faker_cli.templates import CloudFrontWriter, S3AccessLogs, S3AccessWriter, CloudTrailLogs, CloudFrontLogs
 
 from faker_cli.writer import CSVWriter, JSONWriter
 from typing import List
 
 def infer_column_names(col_names, col_types: str) -> List[str]:
     """
     Infer column names from column types
@@ -17,29 +17,36 @@
     return col_types.split(",")
 
 KLAS_MAPPER = {
     "csv": CSVWriter,
     "json": JSONWriter
 }
 
+TEMPLATE_MAPPER = {
+    "s3access": [S3AccessWriter, "s3_access_log"],
+    "cloudfront": [CloudFrontWriter, "cloudfront_log"],
+}
+
 fake = Faker()
 fake.add_provider(S3AccessLogs)
 fake.add_provider(CloudTrailLogs)
+fake.add_provider(CloudFrontLogs)
 
 @click.command()
 @click.option("--num-rows", "-n", default=1, help="Number of rows")
 @click.option("--format", "-f", type=click.Choice(["csv", "json"]), default="csv", help="Format of the output")
 @click.option("--columns", "-c", help="Column names", default=None, required=False)
-@click.option("--template", "-t", help="Template to use", type=click.Choice(["s3access"]), default=None)
+@click.option("--template", "-t", help="Template to use", type=click.Choice(["s3access", "cloudfront"]), default=None)
 @click.argument("column_types", required=False)
 def main(num_rows, format, columns, template, column_types):
     if template:
-        writer = S3AccessWriter(sys.stdout, None)
+        writer = TEMPLATE_MAPPER[template][0](sys.stdout, None)
+        log_entry = TEMPLATE_MAPPER[template][1]
         for i in range(num_rows):
-            row = fake.format("s3_access_log")
+            row = fake.format(log_entry)
             writer.write(row)
         return
         
     col_types = column_types.split(",")
     headers = infer_column_names(columns, column_types)
     writer = KLAS_MAPPER.get(format)(sys.stdout, headers)
     for i in range(num_rows):
```

### Comparing `faker_cli-0.0.5/faker_cli/writer.py` & `faker_cli-0.1.0/faker_cli/writer.py`

 * *Files identical despite different names*

### Comparing `faker_cli-0.0.5/PKG-INFO` & `faker_cli-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faker-cli
-Version: 0.0.5
+Version: 0.1.0
 Summary: 
 Author: Damon P. Cortesi
 Author-email: d.lifehacker@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

