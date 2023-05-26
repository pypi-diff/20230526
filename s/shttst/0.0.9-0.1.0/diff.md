# Comparing `tmp/shttst-0.0.9.tar.gz` & `tmp/shttst-0.1.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shttst-0.0.9.tar", last modified: Mon May  8 09:38:24 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

