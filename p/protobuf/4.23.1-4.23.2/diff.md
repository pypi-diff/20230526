# Comparing `tmp/protobuf-4.23.1.tar.gz` & `tmp/protobuf-4.23.2-cp39-cp39-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/protobuf-4.23.1.tar", last modified: Tue May 16 23:35:35 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

