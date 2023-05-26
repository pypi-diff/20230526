# Comparing `tmp/simple_sharepoint-0.1.0-py3-none-any.whl.zip` & `tmp/simple_sharepoint-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,10 @@
-Zip file size: 7788 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat       21 b- defN 23-Apr-13 09:57 simple_sharepoint/__init__.py
--rw-rw-rw-  2.0 fat     2900 b- defN 23-Apr-12 07:49 simple_sharepoint/api.py
--rw-rw-rw-  2.0 fat     2807 b- defN 23-Apr-13 09:53 simple_sharepoint/client.py
--rw-rw-rw-  2.0 fat     3269 b- defN 23-Apr-13 06:33 simple_sharepoint/sharepoint.py
--rw-rw-rw-  2.0 fat      684 b- defN 23-Apr-13 04:00 simple_sharepoint/test.py
--rw-rw-rw-  2.0 fat     1412 b- defN 23-Apr-05 09:21 simple_sharepoint/upload.py
+Zip file size: 5007 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat       21 b- defN 23-May-26 07:26 simple_sharepoint/__init__.py
+-rw-rw-rw-  2.0 fat     3292 b- defN 23-May-26 07:24 simple_sharepoint/client.py
 -rw-rw-rw-  2.0 fat      698 b- defN 23-Apr-13 09:54 simple_sharepoint/utils.py
--rw-rw-rw-  2.0 fat     3948 b- defN 23-Apr-13 09:57 simple_sharepoint-0.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-13 09:57 simple_sharepoint-0.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       18 b- defN 23-Apr-13 09:57 simple_sharepoint-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      922 b- defN 23-Apr-13 09:57 simple_sharepoint-0.1.0.dist-info/RECORD
-11 files, 16771 bytes uncompressed, 6216 bytes compressed:  62.9%
+-rw-rw-rw-  2.0 fat     1089 b- defN 23-May-26 07:26 simple_sharepoint-0.1.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     4280 b- defN 23-May-26 07:26 simple_sharepoint-0.1.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-26 07:26 simple_sharepoint-0.1.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       18 b- defN 23-May-26 07:26 simple_sharepoint-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      686 b- defN 23-May-26 07:26 simple_sharepoint-0.1.1.dist-info/RECORD
+8 files, 10176 bytes uncompressed, 3795 bytes compressed:  62.7%
```

## zipnote {}

```diff
@@ -1,34 +1,25 @@
 Filename: simple_sharepoint/__init__.py
 Comment: 
 
-Filename: simple_sharepoint/api.py
-Comment: 
-
 Filename: simple_sharepoint/client.py
 Comment: 
 
-Filename: simple_sharepoint/sharepoint.py
-Comment: 
-
-Filename: simple_sharepoint/test.py
-Comment: 
-
-Filename: simple_sharepoint/upload.py
+Filename: simple_sharepoint/utils.py
 Comment: 
 
-Filename: simple_sharepoint/utils.py
+Filename: simple_sharepoint-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: simple_sharepoint-0.1.0.dist-info/METADATA
+Filename: simple_sharepoint-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: simple_sharepoint-0.1.0.dist-info/WHEEL
+Filename: simple_sharepoint-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: simple_sharepoint-0.1.0.dist-info/top_level.txt
+Filename: simple_sharepoint-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: simple_sharepoint-0.1.0.dist-info/RECORD
+Filename: simple_sharepoint-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## simple_sharepoint/__init__.py

```diff
@@ -1 +1 @@
-__version__ = '0.1.0'
+__version__ = '0.1.1'
```

## simple_sharepoint/client.py

```diff
@@ -86,8 +86,31 @@
 			for item in files:
 				self.download_file(item.properties["ServerRelativeUrl"], os.path.join(dst, item.properties["Name"]))
 			
 			for item in folders:
 				self.download_dir(item.properties["ServerRelativeUrl"], os.path.join(dst, item.properties["Name"]))
 		except Exception as e:
 			print(f"[ERROR] Donwload failed")
-			print(e)
+			print(e)
+	
+	def list_dir(self, src: str):
+		try:
+			result = []
+
+			folder = self.ctx.web.get_folder_by_server_relative_url(src)
+			files = folder.files
+			folders = folder.folders
+
+			self.ctx.load(files)
+			self.ctx.load(folders)
+			self.ctx.execute_query()
+
+			for item in folders:
+				result.append((item.properties["Name"], True))
+			
+			for item in files:
+				result.append((item.properties["Name"], False))
+
+		except Exception as e:
+			print(e)
+		
+		return result
```

## Comparing `simple_sharepoint-0.1.0.dist-info/METADATA` & `simple_sharepoint-0.1.1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: simple-sharepoint
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simple way to handle sharepoint with python
 Home-page: UNKNOWN
 Author: sprumin
 Author-email: sprumin@wellbia.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: Office365-REST-Python-Client
 
 Simple way to handle sharepoint with python.
 Provides the ability to upload files and directories. 
 
 ## Installation
 
@@ -101,15 +102,15 @@
 default_path = < SHAREPOINT_BASE_PATH >
 src = default_path + < SHAREPOINT_TARGET_PATH >
 dst = < LOCAL_FILE_PATH >
 
 download_file(src, dst)
 ```
 
-- <b><i>SHAREPOINT_BASE_PATH</i></b>, <b><i>SHAREPIONT_TARGET_PATH</i></b>, <b><i>LOCAL_FILE_PATH</i></b> See item upload_file
+- <b><i>SHAREPOINT_BASE_PATH</i></b>, <b><i>SHAREPIONT_TARGET_PATH</i></b> See item upload_file
 
 - The download_file function requires you to specify the file name to be stored in <b><i>LOCAL_FILE_PATH</i></b>.
 ( ex ) `/home/ubuntu/files/test.txt`
 
 
 ### download_dir
 
@@ -122,11 +123,25 @@
 
 download_dir(src, dst)
 ```
 
 - <b><i>SHAREPOINT_BASE_PATH</i></b>, <b><i>SHAREPIONT_TARGET_PATH</i></b>, <b><i>LOCAL_DIR_PATH</i></b> See item upload_dir
 
 
+### list_dir
+
+A function that listing a particular directory in the sharepoint and all the contents under it.
+
+```python
+default_path = < SHAREPOINT_BASE_PATH >
+src = default_path + < SHAREPOINT_TARGET_PATH >
+
+list_dir(src)
+```
+
+- <b><i>SHAREPOINT_BASE_PATH</i></b>, <b><i>SHAREPIONT_TARGET_PATH</i></b> See item upload_dir
+
+
 ## Third Party Libraries and Dependencies
 
 - [Office365-REST-Python-Client](https://pypi.org/project/Office365-REST-Python-Client/)
```

