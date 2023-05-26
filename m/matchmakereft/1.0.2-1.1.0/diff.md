# Comparing `tmp/matchmakereft-1.0.2.tar.gz` & `tmp/matchmakereft-1.1.0-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matchmakereft-1.0.2.tar", last modified: Wed Jan 12 14:57:52 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

