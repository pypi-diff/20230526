# Comparing `tmp/faker_cli-0.0.4.tar.gz` & `tmp/faker_cli-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faker_cli-0.0.4.tar", max compression
+gzip compressed data, was "faker_cli-0.0.5.tar", max compression
```

## Comparing `faker_cli-0.0.4.tar` & `faker_cli-0.0.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2023-05-25 22:00:32.729052 faker_cli-0.0.4/LICENSE
--rw-r--r--   0        0        0     2852 2023-05-25 22:00:32.729052 faker_cli-0.0.4/README.md
--rw-r--r--   0        0        0        0 2023-05-25 22:00:32.729052 faker_cli-0.0.4/faker_cli/__init__.py
--rw-r--r--   0        0        0     2024 2023-05-25 22:00:32.729052 faker_cli-0.0.4/faker_cli/cli.py
--rw-r--r--   0        0        0    14139 2023-05-25 22:00:32.729052 faker_cli-0.0.4/faker_cli/templates.py
--rw-r--r--   0        0        0      809 2023-05-25 22:00:32.729052 faker_cli-0.0.4/faker_cli/writer.py
--rw-r--r--   0        0        0      461 2023-05-25 22:00:52.493226 faker_cli-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3325 1970-01-01 00:00:00.000000 faker_cli-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-26 04:27:59.656983 faker_cli-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2829 2023-05-26 04:27:59.656983 faker_cli-0.0.5/README.md
+-rw-r--r--   0        0        0        0 2023-05-26 04:27:59.656983 faker_cli-0.0.5/faker_cli/__init__.py
+-rw-r--r--   0        0        0     2074 2023-05-26 04:27:59.656983 faker_cli-0.0.5/faker_cli/cli.py
+-rw-r--r--   0        0        0    15114 2023-05-26 04:27:59.656983 faker_cli-0.0.5/faker_cli/templates.py
+-rw-r--r--   0        0        0      809 2023-05-26 04:27:59.656983 faker_cli-0.0.5/faker_cli/writer.py
+-rw-r--r--   0        0        0      461 2023-05-26 04:28:26.852784 faker_cli-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3302 1970-01-01 00:00:00.000000 faker_cli-0.0.5/PKG-INFO
```

### Comparing `faker_cli-0.0.4/LICENSE` & `faker_cli-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `faker_cli-0.0.4/README.md` & `faker_cli-0.0.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 
 With Faker CLI, you can easily generate CSV or JSON data with fields of your choosing.
 
 You can also utilize pre-built templates for common data formats!
 
 ## Usage
 
-By default, faker-cli will generate a CSV output for you. You just specify the number of rows you want and the column types.
+By default, `fake` will generate a CSV output for you. You just specify the number of rows you want and the column types.
 
 ```bash
-faker-cli -n 10 pyint,user_name,date_this_year
+fake -n 10 pyint,user_name,date_this_year
 ```
 
 BAM! You've got a CSV file with your data.
 
 ```
 pyint,user_name,date_this_year
 8649,fward,2023-03-08
@@ -31,15 +31,15 @@
 ```
 
 ### JSON
 
 Wnat a JSON file? Sweet, use `-f json`.
 
 ```bash
-faker-cli -n 10 pyint,user_name,date_this_year -f json
+fake -n 10 pyint,user_name,date_this_year -f json
 ```
 
 ```json
 {"pyint": 3854, "user_name": "cchavez", "date_this_year": "2023-01-20"}
 {"pyint": 2008, "user_name": "vnguyen", "date_this_year": "2023-04-03"}
 {"pyint": 1434, "user_name": "karen38", "date_this_year": "2023-03-02"}
 {"pyint": 4922, "user_name": "duncanellen", "date_this_year": "2023-04-22"}
@@ -50,15 +50,15 @@
 {"pyint": 3353, "user_name": "melissaatkinson", "date_this_year": "2023-02-10"}
 {"pyint": 5306, "user_name": "mark12", "date_this_year": "2023-04-16"}
 ```
 
 Default column names aren't good enough for you? Fine, use your own.
 
 ```bash
-faker-cli -n 10 pyint,user_name,date_this_year -f json -c id,awesome_name,last_attention_at
+fake -n 10 pyint,user_name,date_this_year -f json -c id,awesome_name,last_attention_at
 ```
 
 ```
 {"id": 6048, "awesome_name": "jtran", "last_attention_at": "2023-04-24"}
 {"id": 4310, "awesome_name": "stacey99", "last_attention_at": "2023-04-27"}
 {"id": 1839, "awesome_name": "jho", "last_attention_at": "2023-03-07"}
 {"id": 236, "awesome_name": "melissamassey", "last_attention_at": "2023-04-17"}
@@ -73,9 +73,9 @@
 ## Templates
 
 As of now,the only amazing best template supported ever is `s3access`.
 
 Want to generate 1 MILLION S3 Access logs in ~2 minutes? Now you can.
 
 ```bash
-faker-cli -t s3access -n 10
+fake -t s3access -n 10
 ```
```

### Comparing `faker_cli-0.0.4/faker_cli/cli.py` & `faker_cli-0.0.5/faker_cli/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from faker import Faker
 import click
 import sys
-from faker_cli.templates import S3AccessLogs, S3AccessWriter
+from faker_cli.templates import S3AccessLogs, S3AccessWriter, CloudTrailLogs
 
 from faker_cli.writer import CSVWriter, JSONWriter
 from typing import List
 
 def infer_column_names(col_names, col_types: str) -> List[str]:
     """
     Infer column names from column types
@@ -19,14 +19,15 @@
 KLAS_MAPPER = {
     "csv": CSVWriter,
     "json": JSONWriter
 }
 
 fake = Faker()
 fake.add_provider(S3AccessLogs)
+fake.add_provider(CloudTrailLogs)
 
 @click.command()
 @click.option("--num-rows", "-n", default=1, help="Number of rows")
 @click.option("--format", "-f", type=click.Choice(["csv", "json"]), default="csv", help="Format of the output")
 @click.option("--columns", "-c", help="Column names", default=None, required=False)
 @click.option("--template", "-t", help="Template to use", type=click.Choice(["s3access"]), default=None)
 @click.argument("column_types", required=False)
```

### Comparing `faker_cli-0.0.4/faker_cli/templates.py` & `faker_cli-0.0.5/faker_cli/templates.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,14 +85,16 @@
         "me-south-1",
         "me-central-1",
         "sa-east-1",
         "us-gov-east-1",
         "us-gov-west-1",
     ]
 
+    _services: List[str] = ["ec2", "cloudtrail", "s3"]
+
 
 class S3AccessWriter(Writer):
     def __init__(self, output, headers):
         super().__init__(output, headers)
 
     def write(self, row):
         self.output.write(" ".join(map(str, row)) + "\n")
@@ -117,14 +119,15 @@
             service = self.generator.random_element(elements=["s3", "ec2", "iam", "sts"])
         if not region and service not in ["iam"]:
             region = self.generator.random_element(elements=AWSConstants._regions)
         if not account_id:
             account_id = self.aws_account_id()
 
         # TODO: There are a WHOLE bunch more rules here to take care of
+        # Also figure out how to handle if resource-type is specificed
         if resource_id is None:
             if service == "iam":
                 resource_id = self.generator.random_element(elements=["root", f"user/{self.generator.user_name()}"])
             else:
                 resource_id = self.generator.user_name()
 
         resource_part = resource_id
@@ -302,15 +305,15 @@
         )
         return f'"{method} {key} HTTP/{http_version}"'
 
     def http_status(self) -> str:
         return str(self._http_status_code())
 
     def error_code(self) -> str:
-        return self.generator.random_element(elements=("NoSuchBucket", "NoSuchLifecycleConfiguration" "-"))
+        return self.generator.random_element(elements=("NoSuchBucket", "NoSuchLifecycleConfiguration", "-"))
 
     def bytes_sent(self, total_object_size: Optional[int] = None) -> str:
         return self.generator.random_element(
             elements=(
                 "-",
                 self.generator.pyint(min_value=1, max_value=total_object_size or (1024 * 1024 * 1024)),
             )
@@ -404,7 +407,36 @@
             status_codes = [num for sublist in AWSConstants._http_status_codes.values() for num in sublist]
 
         return self.generator.random_element(elements=status_codes)
 
 
 # then add new provider to faker instance
 # fake.add_provider(S3AccessLogs)
+
+
+class CloudTrailLogs(AWSProvider):
+    def event_version(self) -> str:
+        return "1.0"
+
+    def event_time(self) -> str:
+        return self.generator.iso8601()
+
+    def event_source(self) -> str:
+        return self.generator.random_element(AWSConstants._services) + ".amazonaws.com"
+
+    def user_id_with_iam_user(self) -> str:
+        """
+        "userIdentity": {
+        "type": "IAMUser",
+        "principalId": "AIDAJ45Q7YFFAREXAMPLE",
+        "arn": "arn:aws:iam::123456789012:user/Alice",
+        "accountId": "123456789012",
+        "accessKeyId": "",
+        "userName": "Alice"
+        }
+        """
+        return {
+            "type": "IAMUser",
+            "principalId": "AIDAJ45Q7YFFAREXAMPLE",
+            "arn": self.aws_arn(service="iam", resource_type="user"),
+            "accountId": self.aws_account_id(),
+        }
```

### Comparing `faker_cli-0.0.4/faker_cli/writer.py` & `faker_cli-0.0.5/faker_cli/writer.py`

 * *Files identical despite different names*

### Comparing `faker_cli-0.0.4/PKG-INFO` & `faker_cli-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faker-cli
-Version: 0.0.4
+Version: 0.0.5
 Summary: 
 Author: Damon P. Cortesi
 Author-email: d.lifehacker@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -19,18 +19,18 @@
 
 With Faker CLI, you can easily generate CSV or JSON data with fields of your choosing.
 
 You can also utilize pre-built templates for common data formats!
 
 ## Usage
 
-By default, faker-cli will generate a CSV output for you. You just specify the number of rows you want and the column types.
+By default, `fake` will generate a CSV output for you. You just specify the number of rows you want and the column types.
 
 ```bash
-faker-cli -n 10 pyint,user_name,date_this_year
+fake -n 10 pyint,user_name,date_this_year
 ```
 
 BAM! You've got a CSV file with your data.
 
 ```
 pyint,user_name,date_this_year
 8649,fward,2023-03-08
@@ -46,15 +46,15 @@
 ```
 
 ### JSON
 
 Wnat a JSON file? Sweet, use `-f json`.
 
 ```bash
-faker-cli -n 10 pyint,user_name,date_this_year -f json
+fake -n 10 pyint,user_name,date_this_year -f json
 ```
 
 ```json
 {"pyint": 3854, "user_name": "cchavez", "date_this_year": "2023-01-20"}
 {"pyint": 2008, "user_name": "vnguyen", "date_this_year": "2023-04-03"}
 {"pyint": 1434, "user_name": "karen38", "date_this_year": "2023-03-02"}
 {"pyint": 4922, "user_name": "duncanellen", "date_this_year": "2023-04-22"}
@@ -65,15 +65,15 @@
 {"pyint": 3353, "user_name": "melissaatkinson", "date_this_year": "2023-02-10"}
 {"pyint": 5306, "user_name": "mark12", "date_this_year": "2023-04-16"}
 ```
 
 Default column names aren't good enough for you? Fine, use your own.
 
 ```bash
-faker-cli -n 10 pyint,user_name,date_this_year -f json -c id,awesome_name,last_attention_at
+fake -n 10 pyint,user_name,date_this_year -f json -c id,awesome_name,last_attention_at
 ```
 
 ```
 {"id": 6048, "awesome_name": "jtran", "last_attention_at": "2023-04-24"}
 {"id": 4310, "awesome_name": "stacey99", "last_attention_at": "2023-04-27"}
 {"id": 1839, "awesome_name": "jho", "last_attention_at": "2023-03-07"}
 {"id": 236, "awesome_name": "melissamassey", "last_attention_at": "2023-04-17"}
@@ -88,9 +88,9 @@
 ## Templates
 
 As of now,the only amazing best template supported ever is `s3access`.
 
 Want to generate 1 MILLION S3 Access logs in ~2 minutes? Now you can.
 
 ```bash
-faker-cli -t s3access -n 10
+fake -t s3access -n 10
 ```
```

