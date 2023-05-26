# Comparing `tmp/anonupload-1.1.4-py3-none-any.whl.zip` & `tmp/anonupload-1.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 6040 bytes, number of entries: 8
--rw-r--r--  2.0 unx       81 b- defN 23-May-26 11:47 anonupload/__init__.py
--rw-r--r--  2.0 unx     6894 b- defN 23-May-26 11:47 anonupload/main.py
--rwxr-xr-x  2.0 unx     1064 b- defN 23-May-26 11:47 anonupload-1.1.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     2456 b- defN 23-May-26 11:47 anonupload-1.1.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-26 11:47 anonupload-1.1.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       46 b- defN 23-May-26 11:47 anonupload-1.1.4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 23-May-26 11:47 anonupload-1.1.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      651 b- defN 23-May-26 11:47 anonupload-1.1.4.dist-info/RECORD
-8 files, 11295 bytes uncompressed, 4896 bytes compressed:  56.7%
+Zip file size: 6078 bytes, number of entries: 8
+-rw-r--r--  2.0 unx       92 b- defN 23-May-26 12:14 anonupload/__init__.py
+-rw-r--r--  2.0 unx     6986 b- defN 23-May-26 12:14 anonupload/main.py
+-rwxr-xr-x  2.0 unx     1064 b- defN 23-May-26 12:14 anonupload-1.1.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2529 b- defN 23-May-26 12:14 anonupload-1.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-26 12:14 anonupload-1.1.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       46 b- defN 23-May-26 12:14 anonupload-1.1.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 23-May-26 12:14 anonupload-1.1.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      651 b- defN 23-May-26 12:14 anonupload-1.1.5.dist-info/RECORD
+8 files, 11471 bytes uncompressed, 4934 bytes compressed:  57.0%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: anonupload/__init__.py
 Comment: 
 
 Filename: anonupload/main.py
 Comment: 
 
-Filename: anonupload-1.1.4.dist-info/LICENSE
+Filename: anonupload-1.1.5.dist-info/LICENSE
 Comment: 
 
-Filename: anonupload-1.1.4.dist-info/METADATA
+Filename: anonupload-1.1.5.dist-info/METADATA
 Comment: 
 
-Filename: anonupload-1.1.4.dist-info/WHEEL
+Filename: anonupload-1.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: anonupload-1.1.4.dist-info/entry_points.txt
+Filename: anonupload-1.1.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: anonupload-1.1.4.dist-info/top_level.txt
+Filename: anonupload-1.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: anonupload-1.1.4.dist-info/RECORD
+Filename: anonupload-1.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## anonupload/__init__.py

```diff
@@ -1,3 +1,3 @@
-__version__ = "1.1.4"
+__version__ = "1.1.5"
 
-from .main import download, upload, changefile_and_upload
+from .main import download, downloads, upload, changefile_and_upload
```

## anonupload/main.py

```diff
@@ -145,26 +145,29 @@
 
 def remove_file(filename: Path):
 	try:
 		os.remove(filename)
 	except FileNotFoundError:
 		print(f'[ERROR]: The file "{filename}" doesn\'t exist!')
 
-def download(url: str, path: Path=Path.cwd(), delete: bool=False):
+def download(url: str, custom_filename: str=None, path: Path=Path.cwd(), delete: bool=False):
 	try:
 		filesize = int(head(url).headers["Content-Length"])
 	except ConnectionError:
 		print("[Error]: No internet")
 		return 1
 	except MissingSchema as e:
 		sys.exit(str(e))
 	except KeyError:
 		filesize = None
-		
-	filename = detect_filename(url, head(url).headers)
+	
+	if custom_filename == None:
+		filename = detect_filename(url, head(url).headers)
+	else:
+		filename = custom_filename
 	
 	chunk_size = 1024
 
 	try:
 		with get(url, stream=True) as r, open(filename, "wb") as f, tqdm(
 				unit="B",  # unit string to be displayed.
 				unit_scale=True,  # let tqdm to determine the scale in kilo, mega..etc.
```

## Comparing `anonupload-1.1.4.dist-info/LICENSE` & `anonupload-1.1.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `anonupload-1.1.4.dist-info/METADATA` & `anonupload-1.1.5.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anonupload
-Version: 1.1.4
+Version: 1.1.5
 Summary: upload and download to anonfiles server
 Home-page: https://github.com/jakbin/anonupload
 Author: Jak Bin
 Author-email: jakbin4747@gmail.com
 Project-URL: Bug Tracker, https://github.com/jakbin/anonupload/issues
 Keywords: anonfile,anonfile-api,anonfile-cli,anonymous,upload
 Classifier: Programming Language :: Python :: 3.6
@@ -62,16 +62,22 @@
 ```
 
 ```py
 from anonupload import changefile_and_upload
 changefile_and_upload([file1, file2])
 ```
 
-### anonupload.download([url1, url2])
+### anonupload.download(url)
 
 ```py
 from anonupload import download
 
 download(url)
+```
+
+### anonupload.download([url1, url2])
+
+```py
+from anonupload import download
 
 downloads([url1, url2])
 ```
```

