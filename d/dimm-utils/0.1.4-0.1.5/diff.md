# Comparing `tmp/dimm_utils-0.1.4.tar.gz` & `tmp/dimm_utils-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dimm_utils-0.1.4.tar", max compression
+gzip compressed data, was "dimm_utils-0.1.5.tar", max compression
```

## Comparing `dimm_utils-0.1.4.tar` & `dimm_utils-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0       91 2023-05-23 14:36:01.477822 dimm_utils-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-05-23 14:04:10.404588 dimm_utils-0.1.4/dimm_utils/__init__.py
--rw-r--r--   0        0        0       21 2023-05-23 14:08:51.294332 dimm_utils-0.1.4/dimm_utils/constants.py
--rw-r--r--   0        0        0     5036 2023-05-23 15:23:35.159779 dimm_utils-0.1.4/dimm_utils/core.py
--rw-r--r--   0        0        0      323 2023-05-23 15:23:38.415346 dimm_utils-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      506 1970-01-01 00:00:00.000000 dimm_utils-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       91 2023-05-23 16:55:29.569693 dimm_utils-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-05-23 16:55:29.569800 dimm_utils-0.1.5/dimm_utils/__init__.py
+-rw-r--r--   0        0        0       21 2023-05-23 16:55:29.570921 dimm_utils-0.1.5/dimm_utils/constants.py
+-rw-r--r--   0        0        0     5398 2023-05-26 16:28:39.541752 dimm_utils-0.1.5/dimm_utils/core.py
+-rw-r--r--   0        0        0      323 2023-05-26 16:28:48.812245 dimm_utils-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      727 1970-01-01 00:00:00.000000 dimm_utils-0.1.5/setup.py
+-rw-r--r--   0        0        0      506 1970-01-01 00:00:00.000000 dimm_utils-0.1.5/PKG-INFO
```

### Comparing `dimm_utils-0.1.4/dimm_utils/core.py` & `dimm_utils-0.1.5/dimm_utils/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -148,10 +148,24 @@
     except botocore_exceptions.ClientError as e:
         error_code = e.response["Error"]["Code"]
         error_message = e.response["Error"]["Message"]
         print(f"Error uploading file to S3: {error_code} - {error_message}")
         return None
 
 
+def get_dynamodb_client(session_name: str):
+    if os.environ.get("aws_region") is None:
+        authenticate_local()
+
+    credentials = authenticate(session_name)
+    dynamodb = boto3.resource("dynamodb", **credentials)
+    return dynamodb
+
+
+def get_dynamodb_table(dynamodb, table_name="telegram-bot"):
+    table = dynamodb.Table(table_name)
+    return table
+
+
 def main():
     print("This is a module, not a script.")
     pass
```

