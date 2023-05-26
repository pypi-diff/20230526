# Comparing `tmp/pmx_biobb-2.0.0.tar.gz` & `tmp/pmx_biobb-3.0.0-cp37-cp37m-macosx_10_9_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pmx_biobb-2.0.0.tar", last modified: Wed Apr 26 11:39:39 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

