# Comparing `tmp/anonupload-1.1.3-py3-none-any.whl.zip` & `tmp/anonupload-1.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 6010 bytes, number of entries: 8
--rw-r--r--  2.0 unx       81 b- defN 23-May-24 14:03 anonupload/__init__.py
--rw-r--r--  2.0 unx     6764 b- defN 23-May-24 14:03 anonupload/main.py
--rwxr-xr-x  2.0 unx     1064 b- defN 23-May-24 14:03 anonupload-1.1.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     2442 b- defN 23-May-24 14:03 anonupload-1.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-24 14:03 anonupload-1.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       46 b- defN 23-May-24 14:03 anonupload-1.1.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 23-May-24 14:03 anonupload-1.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      651 b- defN 23-May-24 14:03 anonupload-1.1.3.dist-info/RECORD
-8 files, 11151 bytes uncompressed, 4866 bytes compressed:  56.4%
+Zip file size: 6040 bytes, number of entries: 8
+-rw-r--r--  2.0 unx       81 b- defN 23-May-26 11:47 anonupload/__init__.py
+-rw-r--r--  2.0 unx     6894 b- defN 23-May-26 11:47 anonupload/main.py
+-rwxr-xr-x  2.0 unx     1064 b- defN 23-May-26 11:47 anonupload-1.1.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2456 b- defN 23-May-26 11:47 anonupload-1.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-26 11:47 anonupload-1.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       46 b- defN 23-May-26 11:47 anonupload-1.1.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 23-May-26 11:47 anonupload-1.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      651 b- defN 23-May-26 11:47 anonupload-1.1.4.dist-info/RECORD
+8 files, 11295 bytes uncompressed, 4896 bytes compressed:  56.7%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: anonupload/__init__.py
 Comment: 
 
 Filename: anonupload/main.py
 Comment: 
 
-Filename: anonupload-1.1.3.dist-info/LICENSE
+Filename: anonupload-1.1.4.dist-info/LICENSE
 Comment: 
 
-Filename: anonupload-1.1.3.dist-info/METADATA
+Filename: anonupload-1.1.4.dist-info/METADATA
 Comment: 
 
-Filename: anonupload-1.1.3.dist-info/WHEEL
+Filename: anonupload-1.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: anonupload-1.1.3.dist-info/entry_points.txt
+Filename: anonupload-1.1.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: anonupload-1.1.3.dist-info/top_level.txt
+Filename: anonupload-1.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: anonupload-1.1.3.dist-info/RECORD
+Filename: anonupload-1.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## anonupload/__init__.py

```diff
@@ -1,3 +1,3 @@
-__version__ = "1.1.3"
+__version__ = "1.1.4"
 
 from .main import download, upload, changefile_and_upload
```

## anonupload/main.py

```diff
@@ -56,15 +56,15 @@
 
 	resp = json.loads(r.text)
 	if resp['status']:
 		urlshort = resp['data']['file']['url']['short']
 		urllong = resp['data']['file']['url']['full']
 		print(f'[SUCCESS]: Your file has been succesfully uploaded:\nFull URL: {urllong}\nShort URL: {urlshort}')
 		with open('urls.txt', 'a+') as f:
-			f.write(urllong)
+			f.write(f"{urllong}\n")
 		print('url saved in urls.txt file')
 		return urlshort, urllong
 	else:
 		message = resp['error']['message']
 		errtype = resp['error']['type']
 		print(f'[ERROR]: {message}\n{errtype}')
 		return message, errtype
@@ -145,49 +145,53 @@
 
 def remove_file(filename: Path):
 	try:
 		os.remove(filename)
 	except FileNotFoundError:
 		print(f'[ERROR]: The file "{filename}" doesn\'t exist!')
 
-def download(urls: List[str], path: Path=Path.cwd(), delete: bool=False):
-	for url in urls:
-		try:
-			filesize = int(head(url).headers["Content-Length"])
-		except ConnectionError:
-			print("[Error]: No internet")
-			return 1
-		except MissingSchema as e:
-			sys.exit(str(e))
-		except KeyError:
-			filesize = None
-			
-		filename = detect_filename(url, head(url).headers)
+def download(url: str, path: Path=Path.cwd(), delete: bool=False):
+	try:
+		filesize = int(head(url).headers["Content-Length"])
+	except ConnectionError:
+		print("[Error]: No internet")
+		return 1
+	except MissingSchema as e:
+		sys.exit(str(e))
+	except KeyError:
+		filesize = None
 		
-		chunk_size = 1024
+	filename = detect_filename(url, head(url).headers)
+	
+	chunk_size = 1024
 
-		try:
-			with get(url, stream=True) as r, open(filename, "wb") as f, tqdm(
-					unit="B",  # unit string to be displayed.
-					unit_scale=True,  # let tqdm to determine the scale in kilo, mega..etc.
-					unit_divisor=1024,  # is used when unit_scale is true
-					total=filesize,  # the total iteration.
-					file=sys.stdout,  # default goes to stderr, this is the display on console.
-					desc=filename  # prefix to be displayed on progress bar.
-			) as progress:
-				for chunk in r.iter_content(chunk_size=chunk_size):
-					datasize = f.write(chunk)
-					progress.update(datasize)
-		except ConnectionError:
-			return 1
-
-		full_filename = os.path.join(path, filename)
-		upload(full_filename)
-		if delete:
-			remove_file(filename)
+	try:
+		with get(url, stream=True) as r, open(filename, "wb") as f, tqdm(
+				unit="B",  # unit string to be displayed.
+				unit_scale=True,  # let tqdm to determine the scale in kilo, mega..etc.
+				unit_divisor=1024,  # is used when unit_scale is true
+				total=filesize,  # the total iteration.
+				file=sys.stdout,  # default goes to stderr, this is the display on console.
+				desc=filename  # prefix to be displayed on progress bar.
+		) as progress:
+			for chunk in r.iter_content(chunk_size=chunk_size):
+				datasize = f.write(chunk)
+				progress.update(datasize)
+	except ConnectionError:
+		return 1
+
+	full_filename = os.path.join(path, filename)
+	first_msg, second_msg = upload(full_filename)
+	if delete:
+		remove_file(filename)
+	return first_msg, second_msg
+
+def downloads(urls: List[str], path: Path=Path.cwd(), delete: bool=False):
+	for url in urls:
+		download(url, path, delete)
 	
 example_uses = '''example:
    anon up {files_name}
    anon d {urls}'''
 
 def main(argv = None):
 	parser = argparse.ArgumentParser(prog=package_name, description="upload your files on anonfile server", epilog=example_uses, formatter_class=argparse.RawDescriptionHelpFormatter)
@@ -204,15 +208,15 @@
 	parser.add_argument('-v',"--version", action="store_true", dest="version", help="check version of anonupload")
 
 	args = parser.parse_args(argv)
 
 	if args.command == "up":
 		return changefile_and_upload(args.filename)
 	elif args.command == "d":
-		return download(args.filename, args.path, args.delete)
+		return downloads(args.filename, args.path, args.delete)
 	elif args.version:
 		return print(__version__)
 	else:
 		parser.print_help()
 
 if __name__ == '__main__':
 	raise SystemExit(main())
```

## Comparing `anonupload-1.1.3.dist-info/LICENSE` & `anonupload-1.1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `anonupload-1.1.3.dist-info/METADATA` & `anonupload-1.1.4.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: anonupload
-Version: 1.1.3
+Version: 1.1.4
 Summary: upload and download to anonfiles server
-Home-page: https://github.com/redevil1/anonfiles
+Home-page: https://github.com/jakbin/anonupload
 Author: Jak Bin
 Author-email: jakbin4747@gmail.com
-Project-URL: Bug Tracker, https://github.com/redevil1/anonfiles/issues
+Project-URL: Bug Tracker, https://github.com/jakbin/anonupload/issues
 Keywords: anonfile,anonfile-api,anonfile-cli,anonymous,upload
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
@@ -67,9 +67,11 @@
 ```
 
 ### anonupload.download([url1, url2])
 
 ```py
 from anonupload import download
 
-download([url1, url2])
+download(url)
+
+downloads([url1, url2])
 ```
```

