# Comparing `tmp/anonupload-1.1.5-py3-none-any.whl.zip` & `tmp/anonupload-1.1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 6078 bytes, number of entries: 8
--rw-r--r--  2.0 unx       92 b- defN 23-May-26 12:14 anonupload/__init__.py
--rw-r--r--  2.0 unx     6986 b- defN 23-May-26 12:14 anonupload/main.py
--rwxr-xr-x  2.0 unx     1064 b- defN 23-May-26 12:14 anonupload-1.1.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     2529 b- defN 23-May-26 12:14 anonupload-1.1.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-26 12:14 anonupload-1.1.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       46 b- defN 23-May-26 12:14 anonupload-1.1.5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 23-May-26 12:14 anonupload-1.1.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      651 b- defN 23-May-26 12:14 anonupload-1.1.5.dist-info/RECORD
-8 files, 11471 bytes uncompressed, 4934 bytes compressed:  57.0%
+Zip file size: 6105 bytes, number of entries: 8
+-rw-r--r--  2.0 unx       92 b- defN 23-May-26 14:27 anonupload/__init__.py
+-rw-r--r--  2.0 unx     7091 b- defN 23-May-26 14:27 anonupload/main.py
+-rwxr-xr-x  2.0 unx     1064 b- defN 23-May-26 14:28 anonupload-1.1.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2529 b- defN 23-May-26 14:28 anonupload-1.1.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-26 14:28 anonupload-1.1.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       46 b- defN 23-May-26 14:28 anonupload-1.1.6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 23-May-26 14:28 anonupload-1.1.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      651 b- defN 23-May-26 14:28 anonupload-1.1.6.dist-info/RECORD
+8 files, 11576 bytes uncompressed, 4961 bytes compressed:  57.1%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: anonupload/__init__.py
 Comment: 
 
 Filename: anonupload/main.py
 Comment: 
 
-Filename: anonupload-1.1.5.dist-info/LICENSE
+Filename: anonupload-1.1.6.dist-info/LICENSE
 Comment: 
 
-Filename: anonupload-1.1.5.dist-info/METADATA
+Filename: anonupload-1.1.6.dist-info/METADATA
 Comment: 
 
-Filename: anonupload-1.1.5.dist-info/WHEEL
+Filename: anonupload-1.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: anonupload-1.1.5.dist-info/entry_points.txt
+Filename: anonupload-1.1.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: anonupload-1.1.5.dist-info/top_level.txt
+Filename: anonupload-1.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: anonupload-1.1.5.dist-info/RECORD
+Filename: anonupload-1.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## anonupload/__init__.py

```diff
@@ -1,3 +1,3 @@
-__version__ = "1.1.5"
+__version__ = "1.1.6"
 
 from .main import download, downloads, upload, changefile_and_upload
```

## anonupload/main.py

```diff
@@ -155,41 +155,45 @@
 	except ConnectionError:
 		print("[Error]: No internet")
 		return 1
 	except MissingSchema as e:
 		sys.exit(str(e))
 	except KeyError:
 		filesize = None
+
+	if not os.path.isdir(path):
+		os.mkdir(path)
 	
 	if custom_filename == None:
 		filename = detect_filename(url, head(url).headers)
+		full_filename = os.path.join(path, filename)
 	else:
 		filename = custom_filename
+		full_filename = os.path.join(path, filename)
 	
 	chunk_size = 1024
 
 	try:
-		with get(url, stream=True) as r, open(filename, "wb") as f, tqdm(
+		with get(url, stream=True) as r, open(full_filename, "wb") as f, tqdm(
 				unit="B",  # unit string to be displayed.
 				unit_scale=True,  # let tqdm to determine the scale in kilo, mega..etc.
 				unit_divisor=1024,  # is used when unit_scale is true
 				total=filesize,  # the total iteration.
 				file=sys.stdout,  # default goes to stderr, this is the display on console.
 				desc=filename  # prefix to be displayed on progress bar.
 		) as progress:
 			for chunk in r.iter_content(chunk_size=chunk_size):
 				datasize = f.write(chunk)
 				progress.update(datasize)
 	except ConnectionError:
 		return 1
 
-	full_filename = os.path.join(path, filename)
 	first_msg, second_msg = upload(full_filename)
 	if delete:
-		remove_file(filename)
+		remove_file(full_filename)
 	return first_msg, second_msg
 
 def downloads(urls: List[str], path: Path=Path.cwd(), delete: bool=False):
 	for url in urls:
 		download(url, path, delete)
 	
 example_uses = '''example:
```

## Comparing `anonupload-1.1.5.dist-info/LICENSE` & `anonupload-1.1.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `anonupload-1.1.5.dist-info/METADATA` & `anonupload-1.1.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anonupload
-Version: 1.1.5
+Version: 1.1.6
 Summary: upload and download to anonfiles server
 Home-page: https://github.com/jakbin/anonupload
 Author: Jak Bin
 Author-email: jakbin4747@gmail.com
 Project-URL: Bug Tracker, https://github.com/jakbin/anonupload/issues
 Keywords: anonfile,anonfile-api,anonfile-cli,anonymous,upload
 Classifier: Programming Language :: Python :: 3.6
```

