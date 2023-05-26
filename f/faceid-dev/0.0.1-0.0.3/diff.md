# Comparing `tmp/faceid-dev-0.0.1.tar.gz` & `tmp/faceid_dev-0.0.3-cp38-cp38-macosx_10_15_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faceid-dev-0.0.1.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

