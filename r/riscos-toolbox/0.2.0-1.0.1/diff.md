# Comparing `tmp/riscos_toolbox-0.2.0.tar.gz` & `tmp/riscos_toolbox-1.0.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "riscos_toolbox-0.2.0.tar", last modified: Wed Nov  3 15:30:05 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

