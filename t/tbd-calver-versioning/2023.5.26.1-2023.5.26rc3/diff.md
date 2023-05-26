# Comparing `tmp/tbd-calver-versioning-2023.5.26.1.tar.gz` & `tmp/tbd-calver-versioning-2023.5.26rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tbd-calver-versioning-2023.5.26.1.tar", last modified: Fri May 26 18:33:48 2023, max compression
+gzip compressed data, was "tbd-calver-versioning-2023.5.26rc3.tar", last modified: Fri May 26 17:04:35 2023, max compression
```

## Comparing `tbd-calver-versioning-2023.5.26.1.tar` & `tbd-calver-versioning-2023.5.26rc3.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 18:33:48.037171 tbd-calver-versioning-2023.5.26.1/
--rw-r--r--   0 root         (0) root         (0)     4225 2023-05-26 18:33:48.037171 tbd-calver-versioning-2023.5.26.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3633 2023-05-26 16:53:29.000000 tbd-calver-versioning-2023.5.26.1/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-26 18:33:48.037171 tbd-calver-versioning-2023.5.26.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3641 2023-05-26 18:32:41.000000 tbd-calver-versioning-2023.5.26.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 18:33:48.033171 tbd-calver-versioning-2023.5.26.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 18:33:48.033171 tbd-calver-versioning-2023.5.26.1/src/bash/
--rw-r--r--   0 root         (0) root         (0)      292 2023-05-26 13:59:12.000000 tbd-calver-versioning-2023.5.26.1/src/bash/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 18:33:48.034170 tbd-calver-versioning-2023.5.26.1/src/bash/bin/
--rw-r--r--   0 root         (0) root         (0)     5763 2023-05-26 18:32:41.000000 tbd-calver-versioning-2023.5.26.1/src/bash/bin/determine_tbd_calver_version_number.sh
--rw-r--r--   0 root         (0) root         (0)      469 2023-05-26 13:59:12.000000 tbd-calver-versioning-2023.5.26.1/src/bash/bin/tag_repo_with_version_number.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 18:33:48.035171 tbd-calver-versioning-2023.5.26.1/src/bash/repo_inspection/
--rw-r--r--   0 root         (0) root         (0)      326 2023-05-26 13:59:12.000000 tbd-calver-versioning-2023.5.26.1/src/bash/repo_inspection/README.md
--rw-r--r--   0 root         (0) root         (0)     1404 2023-05-26 13:59:12.000000 tbd-calver-versioning-2023.5.26.1/src/bash/repo_inspection/checkout_git_repo_properly.sh
--rw-r--r--   0 root         (0) root         (0)     1773 2023-05-26 13:59:12.000000 tbd-calver-versioning-2023.5.26.1/src/bash/repo_inspection/configure_credential_helper.sh
--rw-r--r--   0 root         (0) root         (0)     1134 2023-05-26 18:32:41.000000 tbd-calver-versioning-2023.5.26.1/src/bash/repo_inspection/determine_commit_where_branch_created.sh
--rw-r--r--   0 root         (0) root         (0)     3297 2023-05-26 13:59:12.000000 tbd-calver-versioning-2023.5.26.1/src/bash/repo_inspection/determine_if_changed_files_match_triggers.sh
--rw-r--r--   0 root         (0) root         (0)      511 2023-05-26 13:59:12.000000 tbd-calver-versioning-2023.5.26.1/src/bash/repo_inspection/determine_if_commit_is_merge_commit.sh
--rw-r--r--   0 root         (0) root         (0)     1379 2023-05-26 13:59:12.000000 tbd-calver-versioning-2023.5.26.1/src/bash/repo_inspection/get_changed_files_on_branch.sh
--rw-r--r--   0 root         (0) root         (0)      576 2023-05-26 13:59:12.000000 tbd-calver-versioning-2023.5.26.1/src/bash/repo_inspection/get_changed_files_since_commit.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 18:33:48.035171 tbd-calver-versioning-2023.5.26.1/src/python/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 18:33:48.036171 tbd-calver-versioning-2023.5.26.1/src/python/tbd_calver_versioning.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4225 2023-05-26 18:33:47.000000 tbd-calver-versioning-2023.5.26.1/src/python/tbd_calver_versioning.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      910 2023-05-26 18:33:47.000000 tbd-calver-versioning-2023.5.26.1/src/python/tbd_calver_versioning.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 18:33:47.000000 tbd-calver-versioning-2023.5.26.1/src/python/tbd_calver_versioning.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 18:33:47.000000 tbd-calver-versioning-2023.5.26.1/src/python/tbd_calver_versioning.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 18:33:47.000000 tbd-calver-versioning-2023.5.26.1/src/python/tbd_calver_versioning.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     3083 2023-05-26 16:53:29.000000 tbd-calver-versioning-2023.5.26.1/src/python/tbd_calver_versioning.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:04:35.132287 tbd-calver-versioning-2023.5.26rc3/
+-rw-r--r--   0 root         (0) root         (0)     4226 2023-05-26 17:04:35.131287 tbd-calver-versioning-2023.5.26rc3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3633 2023-05-26 16:53:29.000000 tbd-calver-versioning-2023.5.26rc3/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-26 17:04:35.132287 tbd-calver-versioning-2023.5.26rc3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3250 2023-05-26 17:04:20.000000 tbd-calver-versioning-2023.5.26rc3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:04:35.127287 tbd-calver-versioning-2023.5.26rc3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:04:35.128287 tbd-calver-versioning-2023.5.26rc3/src/bash/
+-rw-r--r--   0 root         (0) root         (0)      292 2023-05-26 13:59:12.000000 tbd-calver-versioning-2023.5.26rc3/src/bash/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:04:35.128287 tbd-calver-versioning-2023.5.26rc3/src/bash/bin/
+-rw-r--r--   0 root         (0) root         (0)     4899 2023-05-26 13:59:12.000000 tbd-calver-versioning-2023.5.26rc3/src/bash/bin/determine_tbd_calver_version_number.sh
+-rw-r--r--   0 root         (0) root         (0)      469 2023-05-26 13:59:12.000000 tbd-calver-versioning-2023.5.26rc3/src/bash/bin/tag_repo_with_version_number.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:04:35.130287 tbd-calver-versioning-2023.5.26rc3/src/bash/repo_inspection/
+-rw-r--r--   0 root         (0) root         (0)      326 2023-05-26 13:59:12.000000 tbd-calver-versioning-2023.5.26rc3/src/bash/repo_inspection/README.md
+-rw-r--r--   0 root         (0) root         (0)     1404 2023-05-26 13:59:12.000000 tbd-calver-versioning-2023.5.26rc3/src/bash/repo_inspection/checkout_git_repo_properly.sh
+-rw-r--r--   0 root         (0) root         (0)     1773 2023-05-26 13:59:12.000000 tbd-calver-versioning-2023.5.26rc3/src/bash/repo_inspection/configure_credential_helper.sh
+-rw-r--r--   0 root         (0) root         (0)      941 2023-05-26 13:59:12.000000 tbd-calver-versioning-2023.5.26rc3/src/bash/repo_inspection/determine_commit_where_branch_created.sh
+-rw-r--r--   0 root         (0) root         (0)     1069 2023-05-26 13:59:12.000000 tbd-calver-versioning-2023.5.26rc3/src/bash/repo_inspection/determine_first_commit_on_branch.sh
+-rw-r--r--   0 root         (0) root         (0)     3297 2023-05-26 13:59:12.000000 tbd-calver-versioning-2023.5.26rc3/src/bash/repo_inspection/determine_if_changed_files_match_triggers.sh
+-rw-r--r--   0 root         (0) root         (0)      511 2023-05-26 13:59:12.000000 tbd-calver-versioning-2023.5.26rc3/src/bash/repo_inspection/determine_if_commit_is_merge_commit.sh
+-rw-r--r--   0 root         (0) root         (0)     1379 2023-05-26 13:59:12.000000 tbd-calver-versioning-2023.5.26rc3/src/bash/repo_inspection/get_changed_files_on_branch.sh
+-rw-r--r--   0 root         (0) root         (0)      576 2023-05-26 13:59:12.000000 tbd-calver-versioning-2023.5.26rc3/src/bash/repo_inspection/get_changed_files_since_commit.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:04:35.130287 tbd-calver-versioning-2023.5.26rc3/src/python/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:04:35.131287 tbd-calver-versioning-2023.5.26rc3/src/python/tbd_calver_versioning.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4226 2023-05-26 17:04:35.000000 tbd-calver-versioning-2023.5.26rc3/src/python/tbd_calver_versioning.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      971 2023-05-26 17:04:35.000000 tbd-calver-versioning-2023.5.26rc3/src/python/tbd_calver_versioning.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 17:04:35.000000 tbd-calver-versioning-2023.5.26rc3/src/python/tbd_calver_versioning.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 17:04:35.000000 tbd-calver-versioning-2023.5.26rc3/src/python/tbd_calver_versioning.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 17:04:35.000000 tbd-calver-versioning-2023.5.26rc3/src/python/tbd_calver_versioning.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     3083 2023-05-26 16:53:29.000000 tbd-calver-versioning-2023.5.26rc3/src/python/tbd_calver_versioning.py
```

### Comparing `tbd-calver-versioning-2023.5.26.1/PKG-INFO` & `tbd-calver-versioning-2023.5.26rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tbd-calver-versioning
-Version: 2023.5.26.1
+Version: 2023.5.26rc3
 Summary: A set of tools to manage a code repository using trunk based development and CalVer.
 Home-page: https://github.com/taylor-schneider/tbd-calver-versioning
 Author: tschneider
 Author-email: tschneider@live.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Unix Shell
```

### Comparing `tbd-calver-versioning-2023.5.26.1/README.md` & `tbd-calver-versioning-2023.5.26rc3/README.md`

 * *Files identical despite different names*

### Comparing `tbd-calver-versioning-2023.5.26.1/setup.py` & `tbd-calver-versioning-2023.5.26rc3/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,15 @@
 import sys
 import setuptools
 import os
 import logging
-
-# Do some magic to import the module from the src/python dir
-import importlib.util
-current_dir = os.path.abspath(os.path.dirname(__file__))
-module_path = os.path.join(current_dir, "src", "python", "tbd_calver_versioning.py")
-spec = importlib.util.spec_from_file_location("tbd_calver_versioning", module_path)
-tbd_calver_versioning = importlib.util.module_from_spec(spec)
-spec.loader.exec_module(tbd_calver_versioning)
+import tbd_calver_versioning
 
 logging.basicConfig(level=logging.DEBUG, filename="/tmp/foobar.log")
 
-
 # Read the text from the README
 with open('README.md', "r") as fh:
     long_description = fh.read()
 
 # Read the text from the requirements file
 with open('requirements.txt') as file:
     lines = file.readlines()
@@ -48,21 +40,21 @@
     bash_files = [(key, value) for key,value in bash_files.items()]    
     return bash_files  
 import json
 bash_files = get_data_paths_for_bash_files("src/bash")
 logging.debug(json.dumps(bash_files, indent=4))
 
 # Determine which versioning scheme to use
-VERSION_FOR_PYPI = None
+VERSION_FOR_PYPY = None
 try:
-    VERSION_FOR_PYPI = os.environ['VERSION_FOR_PYPI']
+    VERSION_FOR_PYPY = os.environ['VERSION_FOR_PYPY']
 except Exception as e:
-    raise Exception("The environment variable VERSION_FOR_PYPI must be set to ensure the package is versioned correctly.")
+    raise Exception("The environment variable VERSION_FOR_PYPY must be set to ensure the package is versioned correctly.")
 
-if VERSION_FOR_PYPI == "true":
+if VERSION_FOR_PYPY == "true":
     version_number = tbd_calver_versioning.determine_version_number(adjust_for_pypi=True)
 else:
     version_number = tbd_calver_versioning.determine_version_number()
     
 # Run the setuptools setup function to install our code
 package_name = "tbd-calver-versioning"
 setuptools.setup(
```

### Comparing `tbd-calver-versioning-2023.5.26.1/src/bash/bin/determine_tbd_calver_version_number.sh` & `tbd-calver-versioning-2023.5.26rc3/src/bash/bin/determine_tbd_calver_version_number.sh`

 * *Files 12% similar despite different names*

```diff
@@ -76,32 +76,17 @@
 
 	# When a commit is made, the commit has parents marking the branches involved
 	# Typically, first perent represents the branch where the commit was originally made
 	# The first-parent flag allows us to filter out commit/merges which occurred on our branch
 	# as opposed to another branch
 	
 	FIRST_COMMIT=$(git log --pretty=tformat:"%h" --first-parent | tail -n 1)
-
-	# If we are on an integration branch we will consider all merges and commits
-	# but if we are on a non-integration branch we will only consider merges and commits
-	# that occur after the commit that created the branch. This means we need special logic 
-	# for the release branch and master branch.
-
-	if [[ "${BRANCH_TYPE}" == "release" ]]; then
-		COMMIT_WHERE_BRANCH_CREATED=$(bash "${ROOT_DIR}/repo_inspection/determine_commit_where_branch_created.sh")	
-		MERGES_COUNT=$(git rev-list --first-parent --count ${COMMIT_WHERE_BRANCH_CREATED}..HEAD --merges)
-		COMMIT_COUNT=$(git rev-list --first-parent --count ${COMMIT_WHERE_BRANCH_CREATED}..HEAD --no-merges)
-		VERSION_COUNT=$((MERGES_COUNT + COMMIT_COUNT + 1)) 
-		# Note: We add one because the revlist command above does not include the commit in question
-	elif [[ "${BRANCH_TYPE}" == "master" ]]; then
-		MERGES_COUNT=$(git rev-list --first-parent --count HEAD --since=${PREVIOUS_DATE} --merges)
-		COMMIT_COUNT=$(git rev-list --first-parent --count HEAD --since=${PREVIOUS_DATE} --no-merges)
-		VERSION_COUNT=$((MERGES_COUNT + COMMIT_COUNT))
-	fi
-
+	MERGES_COUNT=$(git rev-list --first-parent --count HEAD --since=${PREVIOUS_DATE} --merges)
+	COMMIT_COUNT=$(git rev-list --first-parent --count HEAD --since=${PREVIOUS_DATE} --no-merges)
+	VERSION_COUNT=$((MERGES_COUNT + COMMIT_COUNT))
 
 	# =========================================================
 	# Special case #1: Committing directly to mainline or release
 	# =========================================================
 	# Normally we should not be committing directly to the integration branches (master/release)
 	# However there is a special case when we are allowed to have commits appear without merges
 	# For master, the initial commit on the branch
```

### Comparing `tbd-calver-versioning-2023.5.26.1/src/bash/repo_inspection/checkout_git_repo_properly.sh` & `tbd-calver-versioning-2023.5.26rc3/src/bash/repo_inspection/checkout_git_repo_properly.sh`

 * *Files identical despite different names*

### Comparing `tbd-calver-versioning-2023.5.26.1/src/bash/repo_inspection/configure_credential_helper.sh` & `tbd-calver-versioning-2023.5.26rc3/src/bash/repo_inspection/configure_credential_helper.sh`

 * *Files identical despite different names*

### Comparing `tbd-calver-versioning-2023.5.26.1/src/bash/repo_inspection/determine_commit_where_branch_created.sh` & `tbd-calver-versioning-2023.5.26rc3/src/bash/repo_inspection/determine_first_commit_on_branch.sh`

 * *Files 7% similar despite different names*

```diff
@@ -23,13 +23,10 @@
 	if [ -z "${MAINLINE_BRANCH}" ]; then
 		echo "The mainline branch name was not set."
 		exit 1
 	fi
 
 # Do some magic to diff the two revision lists
 
-	FISRT_COMMIT_ON_BRANCH=$( diff --old-line-format='' --new-line-format='' \
+	diff --old-line-format='' --new-line-format='' \
 		<(git rev-list --first-parent "${1:-${MAINLINE_BRANCH}}") \
-	        <(git rev-list --first-parent "${2:-HEAD}") | head -1)
-
-	echo "${FISRT_COMMIT_ON_BRANCH=$}"
-
+	        <(git rev-list --first-parent "${2:-HEAD}") | head -1
```

### Comparing `tbd-calver-versioning-2023.5.26.1/src/bash/repo_inspection/determine_if_changed_files_match_triggers.sh` & `tbd-calver-versioning-2023.5.26rc3/src/bash/repo_inspection/determine_if_changed_files_match_triggers.sh`

 * *Files identical despite different names*

### Comparing `tbd-calver-versioning-2023.5.26.1/src/bash/repo_inspection/get_changed_files_on_branch.sh` & `tbd-calver-versioning-2023.5.26rc3/src/bash/repo_inspection/get_changed_files_on_branch.sh`

 * *Files identical despite different names*

### Comparing `tbd-calver-versioning-2023.5.26.1/src/bash/repo_inspection/get_changed_files_since_commit.sh` & `tbd-calver-versioning-2023.5.26rc3/src/bash/repo_inspection/get_changed_files_since_commit.sh`

 * *Files identical despite different names*

### Comparing `tbd-calver-versioning-2023.5.26.1/src/python/tbd_calver_versioning.egg-info/PKG-INFO` & `tbd-calver-versioning-2023.5.26rc3/src/python/tbd_calver_versioning.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tbd-calver-versioning
-Version: 2023.5.26.1
+Version: 2023.5.26rc3
 Summary: A set of tools to manage a code repository using trunk based development and CalVer.
 Home-page: https://github.com/taylor-schneider/tbd-calver-versioning
 Author: tschneider
 Author-email: tschneider@live.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Unix Shell
```

### Comparing `tbd-calver-versioning-2023.5.26.1/src/python/tbd_calver_versioning.egg-info/SOURCES.txt` & `tbd-calver-versioning-2023.5.26rc3/src/python/tbd_calver_versioning.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 src/bash/README.md
 src/bash/bin/determine_tbd_calver_version_number.sh
 src/bash/bin/tag_repo_with_version_number.sh
 src/bash/repo_inspection/README.md
 src/bash/repo_inspection/checkout_git_repo_properly.sh
 src/bash/repo_inspection/configure_credential_helper.sh
 src/bash/repo_inspection/determine_commit_where_branch_created.sh
+src/bash/repo_inspection/determine_first_commit_on_branch.sh
 src/bash/repo_inspection/determine_if_changed_files_match_triggers.sh
 src/bash/repo_inspection/determine_if_commit_is_merge_commit.sh
 src/bash/repo_inspection/get_changed_files_on_branch.sh
 src/bash/repo_inspection/get_changed_files_since_commit.sh
 src/python/tbd_calver_versioning.py
 src/python/tbd_calver_versioning.egg-info/PKG-INFO
 src/python/tbd_calver_versioning.egg-info/SOURCES.txt
```

### Comparing `tbd-calver-versioning-2023.5.26.1/src/python/tbd_calver_versioning.py` & `tbd-calver-versioning-2023.5.26rc3/src/python/tbd_calver_versioning.py`

 * *Files identical despite different names*

