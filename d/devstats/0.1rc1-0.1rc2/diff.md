# Comparing `tmp/devstats-0.1rc1.tar.gz` & `tmp/devstats-0.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devstats-0.1rc1.tar", last modified: Wed May 24 17:35:32 2023, max compression
+gzip compressed data, was "devstats-0.1rc2.tar", last modified: Fri May 26 16:02:59 2023, max compression
```

## Comparing `devstats-0.1rc1.tar` & `devstats-0.1rc2.tar`

### file list

```diff
@@ -1,23 +1,34 @@
-drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-05-24 17:35:32.632254 devstats-0.1rc1/
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1504 2023-05-22 22:53:17.000000 devstats-0.1rc1/LICENSE
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)     2147 2023-05-24 17:35:32.632254 devstats-0.1rc1/PKG-INFO
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1203 2023-05-23 20:04:35.000000 devstats-0.1rc1/README.md
-drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-05-24 17:35:32.630254 devstats-0.1rc1/devstats/
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)        0 2023-05-24 00:27:42.000000 devstats-0.1rc1/devstats/__init__.py
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1764 2023-05-24 17:33:45.000000 devstats-0.1rc1/devstats/__main__.py
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)      494 2023-05-24 17:33:45.000000 devstats-0.1rc1/devstats/publish.py
-drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-05-24 17:35:32.631254 devstats-0.1rc1/devstats/queries/
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1453 2023-05-24 00:22:14.000000 devstats-0.1rc1/devstats/queries/issue_activity_since_date.gql
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)      582 2023-05-24 00:22:14.000000 devstats-0.1rc1/devstats/queries/pr_data_query.gql
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)     6364 2023-05-24 16:58:50.000000 devstats-0.1rc1/devstats/query.py
-drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-05-24 17:35:32.631254 devstats-0.1rc1/devstats/reports/
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)    17738 2023-05-24 17:33:45.000000 devstats-0.1rc1/devstats/reports/analysis_template.md
-drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-05-24 17:35:32.631254 devstats-0.1rc1/devstats.egg-info/
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)     2147 2023-05-24 17:35:32.000000 devstats-0.1rc1/devstats.egg-info/PKG-INFO
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)      426 2023-05-24 17:35:32.000000 devstats-0.1rc1/devstats.egg-info/SOURCES.txt
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)        1 2023-05-24 17:35:32.000000 devstats-0.1rc1/devstats.egg-info/dependency_links.txt
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)       51 2023-05-24 17:35:32.000000 devstats-0.1rc1/devstats.egg-info/entry_points.txt
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)       73 2023-05-24 17:35:32.000000 devstats-0.1rc1/devstats.egg-info/requires.txt
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)        9 2023-05-24 17:35:32.000000 devstats-0.1rc1/devstats.egg-info/top_level.txt
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)      848 2023-05-24 17:33:52.000000 devstats-0.1rc1/pyproject.toml
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)       38 2023-05-24 17:35:32.632254 devstats-0.1rc1/setup.cfg
+drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-05-26 16:02:59.910227 devstats-0.1rc2/
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1504 2023-05-22 22:53:17.000000 devstats-0.1rc2/LICENSE
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     2146 2023-05-26 16:02:59.910227 devstats-0.1rc2/PKG-INFO
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     2146 2023-05-24 23:45:39.000000 devstats-0.1rc2/README.md
+drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-05-26 16:02:59.906227 devstats-0.1rc2/devstats/
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)        0 2023-05-24 00:27:42.000000 devstats-0.1rc2/devstats/__init__.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1764 2023-05-26 15:53:46.000000 devstats-0.1rc2/devstats/__main__.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)      999 2023-05-26 15:58:53.000000 devstats-0.1rc2/devstats/publish.py
+drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-05-26 16:02:59.908228 devstats-0.1rc2/devstats/queries/
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1453 2023-05-24 00:22:14.000000 devstats-0.1rc2/devstats/queries/issue_activity_since_date.gql
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)      582 2023-05-24 00:22:14.000000 devstats-0.1rc2/devstats/queries/pr_data_query.gql
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     6364 2023-05-24 16:58:50.000000 devstats-0.1rc2/devstats/query.py
+drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-05-26 16:02:59.904228 devstats-0.1rc2/devstats/reports/
+drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-05-26 16:02:59.908228 devstats-0.1rc2/devstats/reports/issues/
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)      445 2023-05-26 15:58:53.000000 devstats-0.1rc2/devstats/reports/issues/first_responders.md
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1786 2023-05-26 15:58:53.000000 devstats-0.1rc2/devstats/reports/issues/new_issues.md
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     3079 2023-05-26 15:58:53.000000 devstats-0.1rc2/devstats/reports/issues/time_to_response.md
+drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-05-26 16:02:59.910227 devstats-0.1rc2/devstats/reports/pull_requests/
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1078 2023-05-26 15:58:53.000000 devstats-0.1rc2/devstats/reports/pull_requests/mergeability_of_open_prs.md
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     2080 2023-05-26 15:58:53.000000 devstats-0.1rc2/devstats/reports/pull_requests/merged_prs_over_time.md
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)      824 2023-05-26 15:58:53.000000 devstats-0.1rc2/devstats/reports/pull_requests/number_of_pr_participants.md
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1695 2023-05-26 15:58:53.000000 devstats-0.1rc2/devstats/reports/pull_requests/pony_factor.md
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     2424 2023-05-26 15:58:53.000000 devstats-0.1rc2/devstats/reports/pull_requests/pr_lifetime.md
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1669 2023-05-26 15:58:53.000000 devstats-0.1rc2/devstats/reports/pull_requests/where_contributions_come_from.md
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     2881 2023-05-26 15:58:53.000000 devstats-0.1rc2/devstats/template.md
+drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-05-26 16:02:59.907227 devstats-0.1rc2/devstats.egg-info/
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     2146 2023-05-26 16:02:59.000000 devstats-0.1rc2/devstats.egg-info/PKG-INFO
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)      865 2023-05-26 16:02:59.000000 devstats-0.1rc2/devstats.egg-info/SOURCES.txt
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)        1 2023-05-26 16:02:59.000000 devstats-0.1rc2/devstats.egg-info/dependency_links.txt
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)       51 2023-05-26 16:02:59.000000 devstats-0.1rc2/devstats.egg-info/entry_points.txt
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)       73 2023-05-26 16:02:59.000000 devstats-0.1rc2/devstats.egg-info/requires.txt
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)        9 2023-05-26 16:02:59.000000 devstats-0.1rc2/devstats.egg-info/top_level.txt
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)      847 2023-05-26 15:59:15.000000 devstats-0.1rc2/pyproject.toml
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)       38 2023-05-26 16:02:59.911228 devstats-0.1rc2/setup.cfg
```

### Comparing `devstats-0.1rc1/LICENSE` & `devstats-0.1rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `devstats-0.1rc1/PKG-INFO` & `devstats-0.1rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devstats
-Version: 0.1rc1
+Version: 0.1rc2
 Summary: Developer tool for scientific Python libraries
 Maintainer-email: Scientific Python <devstats@discuss.scientific-python.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Scientific Python
         
         Redistribution and use in source and binary forms, with or without
@@ -31,10 +31,10 @@
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
 Project-URL: homepage, https://github.com/scientific-python/devstats
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Provides-Extra: lint
 License-File: LICENSE
```

### Comparing `devstats-0.1rc1/devstats/__main__.py` & `devstats-0.1rc2/devstats/__main__.py`

 * *Files identical despite different names*

### Comparing `devstats-0.1rc1/devstats/queries/issue_activity_since_date.gql` & `devstats-0.1rc2/devstats/queries/issue_activity_since_date.gql`

 * *Files identical despite different names*

### Comparing `devstats-0.1rc1/devstats/queries/pr_data_query.gql` & `devstats-0.1rc2/devstats/queries/pr_data_query.gql`

 * *Files identical despite different names*

### Comparing `devstats-0.1rc1/devstats/query.py` & `devstats-0.1rc2/devstats/query.py`

 * *Files identical despite different names*

### Comparing `devstats-0.1rc1/devstats.egg-info/PKG-INFO` & `devstats-0.1rc2/devstats.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devstats
-Version: 0.1rc1
+Version: 0.1rc2
 Summary: Developer tool for scientific Python libraries
 Maintainer-email: Scientific Python <devstats@discuss.scientific-python.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Scientific Python
         
         Redistribution and use in source and binary forms, with or without
@@ -31,10 +31,10 @@
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
 Project-URL: homepage, https://github.com/scientific-python/devstats
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Provides-Extra: lint
 License-File: LICENSE
```

### Comparing `devstats-0.1rc1/pyproject.toml` & `devstats-0.1rc2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "devstats"
-version = "0.1rc1"
-requires-python = ">=3.10"
+version = "0.1rc2"
+requires-python = ">=3.8"
 description = "Developer tool for scientific Python libraries"
 license = {file = "LICENSE"}
 maintainers = [
   {name = "Scientific Python", email = "devstats@discuss.scientific-python.org"}
 ]
 classifiers = [
   "Development Status :: 3 - Alpha",
```

