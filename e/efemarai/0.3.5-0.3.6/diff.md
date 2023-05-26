# Comparing `tmp/efemarai-0.3.5.tar.gz` & `tmp/efemarai-0.3.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efemarai-0.3.5.tar", last modified: Thu May 11 12:22:38 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

