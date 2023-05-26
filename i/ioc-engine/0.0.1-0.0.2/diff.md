# Comparing `tmp/ioc_engine-0.0.1.tar.gz` & `tmp/ioc_engine-0.0.2-py3.8.egg`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ioc_engine-0.0.1.tar", last modified: Fri May 26 10:31:22 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

