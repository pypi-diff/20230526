# Comparing `tmp/second_myload_project-1.0.tar.gz` & `tmp/second_myload_project-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\second_myload_project-1.0.tar", last modified: Fri May 26 09:55:42 2023, max compression
+gzip compressed data, was "dist\second_myload_project-1.1.tar", last modified: Fri May 26 11:42:02 2023, max compression
```

## Comparing `second_myload_project-1.0.tar` & `second_myload_project-1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 09:55:42.000000 second_myload_project-1.0/
--rw-rw-rw-   0        0        0      216 2023-05-26 09:55:42.000000 second_myload_project-1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-26 09:55:42.000000 second_myload_project-1.0/second_myload_project/
--rw-rw-rw-   0        0        0      174 2023-05-26 09:55:04.000000 second_myload_project-1.0/second_myload_project/Student.py
--rw-rw-rw-   0        0        0        0 2023-05-26 09:51:50.000000 second_myload_project-1.0/second_myload_project/__init__.py
--rw-rw-rw-   0        0        0      354 2023-05-26 09:55:21.000000 second_myload_project-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 11:42:02.000000 second_myload_project-1.1/
+-rw-rw-rw-   0        0        0      216 2023-05-26 11:42:02.000000 second_myload_project-1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-26 11:42:02.000000 second_myload_project-1.1/second_myload_project/
+-rw-rw-rw-   0        0        0      178 2023-05-26 10:02:46.000000 second_myload_project-1.1/second_myload_project/Student.py
+-rw-rw-rw-   0        0        0        0 2023-05-26 09:51:50.000000 second_myload_project-1.1/second_myload_project/__init__.py
+-rw-rw-rw-   0        0        0      354 2023-05-26 11:41:55.000000 second_myload_project-1.1/setup.py
```

