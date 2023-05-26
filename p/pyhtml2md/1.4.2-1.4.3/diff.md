# Comparing `tmp/pyhtml2md-1.4.2.tar.gz` & `tmp/pyhtml2md-1.4.3-cp310-cp310-win32.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhtml2md-1.4.2.tar", last modified: Thu Mar 23 15:09:57 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

