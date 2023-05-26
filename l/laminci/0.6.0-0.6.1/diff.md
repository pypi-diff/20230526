# Comparing `tmp/laminci-0.6.0.tar.gz` & `tmp/laminci-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laminci-0.6.0.tar", last modified: Fri May 26 16:19:43 2023, max compression
+gzip compressed data, was "laminci-0.6.1.tar", last modified: Fri May 26 16:34:09 2023, max compression
```

## Comparing `laminci-0.6.0.tar` & `laminci-0.6.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1371 2023-02-23 21:08:15.192204 laminci-0.6.0/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-02-23 20:36:15.651723 laminci-0.6.0/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-02-23 20:36:15.652253 laminci-0.6.0/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1194 2023-02-23 20:36:15.627521 laminci-0.6.0/.gitignore
--rw-r--r--   0        0        0     1770 2023-02-23 20:36:15.623232 laminci-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       29 2023-02-23 21:02:08.741159 laminci-0.6.0/README.md
--rw-r--r--   0        0        0     3052 2023-05-26 16:19:25.148581 laminci-0.6.0/docs/changelog.md
--rw-r--r--   0        0        0      339 2023-02-23 20:36:15.640096 laminci-0.6.0/docs/guide/index.md
--rw-r--r--   0        0        0     1415 2023-05-26 15:57:31.631988 laminci-0.6.0/docs/guide/quickstart.ipynb
--rw-r--r--   0        0        0        0 2023-02-23 21:02:08.741423 laminci-0.6.0/docs/index.md
--rw-r--r--   0        0        0      805 2023-02-23 20:36:15.648759 laminci-0.6.0/docs/notes/YYYY-MM-DD-my-design-choice.ipynb
--rw-r--r--   0        0        0      223 2023-02-23 20:36:15.647572 laminci-0.6.0/docs/notes/index.md
--rw-r--r--   0        0        0      122 2023-02-23 20:36:15.618482 laminci-0.6.0/lamin-project.yaml
--rw-r--r--   0        0        0      378 2023-05-26 16:18:33.421862 laminci-0.6.0/laminci/__init__.py
--rw-r--r--   0        0        0     2122 2023-05-26 16:17:30.304228 laminci-0.6.0/laminci/_artifacts.py
--rw-r--r--   0        0        0     1358 2023-05-26 16:17:30.304517 laminci-0.6.0/laminci/_db.py
--rw-r--r--   0        0        0      380 2023-02-23 22:56:58.478640 laminci-0.6.0/laminci/_docs.py
--rw-r--r--   0        0        0      737 2023-02-23 22:56:58.478807 laminci-0.6.0/laminci/_env.py
--rw-r--r--   0        0        0     2423 2023-04-10 13:41:42.840205 laminci-0.6.0/laminci/_nox.py
--rw-r--r--   0        0        0       81 2023-05-26 16:17:30.304774 laminci-0.6.0/laminci/db.py
--rw-r--r--   0        0        0      167 2023-02-23 21:55:02.625861 laminci-0.6.0/laminci/nox.py
--rw-r--r--   0        0        0      497 2023-02-23 21:02:08.742361 laminci-0.6.0/noxfile.py
--rw-r--r--   0        0        0      694 2023-03-09 14:11:55.514326 laminci-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      126 2023-05-26 16:17:30.304991 laminci-0.6.0/tests/test_artifacts.py
--rw-r--r--   0        0        0      473 1970-01-01 00:00:00.000000 laminci-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1371 2023-02-23 21:08:15.192204 laminci-0.6.1/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-02-23 20:36:15.651723 laminci-0.6.1/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-02-23 20:36:15.652253 laminci-0.6.1/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1194 2023-02-23 20:36:15.627521 laminci-0.6.1/.gitignore
+-rw-r--r--   0        0        0     1770 2023-02-23 20:36:15.623232 laminci-0.6.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       29 2023-02-23 21:02:08.741159 laminci-0.6.1/README.md
+-rw-r--r--   0        0        0     3052 2023-05-26 16:19:25.148581 laminci-0.6.1/docs/changelog.md
+-rw-r--r--   0        0        0      339 2023-02-23 20:36:15.640096 laminci-0.6.1/docs/guide/index.md
+-rw-r--r--   0        0        0     1415 2023-05-26 15:57:31.631988 laminci-0.6.1/docs/guide/quickstart.ipynb
+-rw-r--r--   0        0        0        0 2023-02-23 21:02:08.741423 laminci-0.6.1/docs/index.md
+-rw-r--r--   0        0        0      805 2023-02-23 20:36:15.648759 laminci-0.6.1/docs/notes/YYYY-MM-DD-my-design-choice.ipynb
+-rw-r--r--   0        0        0      223 2023-02-23 20:36:15.647572 laminci-0.6.1/docs/notes/index.md
+-rw-r--r--   0        0        0      122 2023-02-23 20:36:15.618482 laminci-0.6.1/lamin-project.yaml
+-rw-r--r--   0        0        0      378 2023-05-26 16:33:54.518019 laminci-0.6.1/laminci/__init__.py
+-rw-r--r--   0        0        0     2122 2023-05-26 16:17:30.304228 laminci-0.6.1/laminci/_artifacts.py
+-rw-r--r--   0        0        0     1358 2023-05-26 16:17:30.304517 laminci-0.6.1/laminci/_db.py
+-rw-r--r--   0        0        0      380 2023-02-23 22:56:58.478640 laminci-0.6.1/laminci/_docs.py
+-rw-r--r--   0        0        0      737 2023-02-23 22:56:58.478807 laminci-0.6.1/laminci/_env.py
+-rw-r--r--   0        0        0     2423 2023-04-10 13:41:42.840205 laminci-0.6.1/laminci/_nox.py
+-rw-r--r--   0        0        0      148 2023-05-26 16:33:21.362381 laminci-0.6.1/laminci/db.py
+-rw-r--r--   0        0        0      167 2023-02-23 21:55:02.625861 laminci-0.6.1/laminci/nox.py
+-rw-r--r--   0        0        0      497 2023-02-23 21:02:08.742361 laminci-0.6.1/noxfile.py
+-rw-r--r--   0        0        0      694 2023-03-09 14:11:55.514326 laminci-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      126 2023-05-26 16:17:30.304991 laminci-0.6.1/tests/test_artifacts.py
+-rw-r--r--   0        0        0      473 1970-01-01 00:00:00.000000 laminci-0.6.1/PKG-INFO
```

### Comparing `laminci-0.6.0/.github/workflows/build.yml` & `laminci-0.6.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `laminci-0.6.0/.github/workflows/latest-changes.yml` & `laminci-0.6.1/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `laminci-0.6.0/.gitignore` & `laminci-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `laminci-0.6.0/.pre-commit-config.yaml` & `laminci-0.6.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `laminci-0.6.0/docs/changelog.md` & `laminci-0.6.1/docs/changelog.md`

 * *Files identical despite different names*

### Comparing `laminci-0.6.0/docs/guide/quickstart.ipynb` & `laminci-0.6.1/docs/guide/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `laminci-0.6.0/docs/notes/YYYY-MM-DD-my-design-choice.ipynb` & `laminci-0.6.1/docs/notes/YYYY-MM-DD-my-design-choice.ipynb`

 * *Files identical despite different names*

### Comparing `laminci-0.6.0/laminci/_artifacts.py` & `laminci-0.6.1/laminci/_artifacts.py`

 * *Files identical despite different names*

### Comparing `laminci-0.6.0/laminci/_db.py` & `laminci-0.6.1/laminci/_db.py`

 * *Files identical despite different names*

### Comparing `laminci-0.6.0/laminci/_env.py` & `laminci-0.6.1/laminci/_env.py`

 * *Files identical despite different names*

### Comparing `laminci-0.6.0/laminci/_nox.py` & `laminci-0.6.1/laminci/_nox.py`

 * *Files identical despite different names*

### Comparing `laminci-0.6.0/pyproject.toml` & `laminci-0.6.1/pyproject.toml`

 * *Files identical despite different names*

