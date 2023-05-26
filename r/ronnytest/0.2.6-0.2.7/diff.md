# Comparing `tmp/ronnytest-0.2.6.tar.gz` & `tmp/ronnytest-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ronnytest-0.2.6.tar", last modified: Thu May 25 12:14:52 2023, max compression
+gzip compressed data, was "dist/ronnytest-0.2.7.tar", last modified: Fri May 26 08:54:05 2023, max compression
```

## Comparing `ronnytest-0.2.6.tar` & `ronnytest-0.2.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 12:14:52.000000 ronnytest-0.2.6/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 12:14:52.000000 ronnytest-0.2.6/ronnytest.egg-info/
--rw-r--r--   0 root         (0) root         (0)      220 2023-05-25 12:14:52.000000 ronnytest-0.2.6/ronnytest.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 12:14:52.000000 ronnytest-0.2.6/ronnytest.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      158 2023-05-25 12:14:52.000000 ronnytest-0.2.6/ronnytest.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 12:14:52.000000 ronnytest-0.2.6/ronnytest.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      122 2023-05-25 03:55:14.000000 ronnytest-0.2.6/README.md
--rw-r--r--   0 root         (0) root         (0)     1073 2023-05-25 03:55:14.000000 ronnytest-0.2.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)      220 2023-05-25 12:14:52.000000 ronnytest-0.2.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-25 12:14:52.000000 ronnytest-0.2.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1844 2023-05-25 12:14:34.000000 ronnytest-0.2.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 08:54:05.000000 ronnytest-0.2.7/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 08:54:05.000000 ronnytest-0.2.7/ronnytest.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      220 2023-05-26 08:54:05.000000 ronnytest-0.2.7/ronnytest.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 08:54:05.000000 ronnytest-0.2.7/ronnytest.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      158 2023-05-26 08:54:05.000000 ronnytest-0.2.7/ronnytest.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 08:54:05.000000 ronnytest-0.2.7/ronnytest.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      122 2023-05-25 03:55:14.000000 ronnytest-0.2.7/README.md
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-05-25 03:55:14.000000 ronnytest-0.2.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      220 2023-05-26 08:54:05.000000 ronnytest-0.2.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-26 08:54:05.000000 ronnytest-0.2.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1725 2023-05-26 08:49:20.000000 ronnytest-0.2.7/setup.py
```

### Comparing `ronnytest-0.2.6/LICENSE` & `ronnytest-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ronnytest-0.2.6/setup.py` & `ronnytest-0.2.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,24 +6,21 @@
         print('\033[91m*************************************************************************************************************************************\033[0m')
         print('\033[91m*************************************************************************************************************************************\033[0m')
         print("\033[91mWarning: Tencent security team found that you are currently trying to download the company's internal private package from the official source of pypi!!!\033[0m")
         print("\033[91mWarning: According to Tencent's security regulations, you are not allowed to download third-party private packages that have not been evaluated and confirmed for safety, and your downloading behavior has been blocked!!!\033[0m")
         print('\033[91mWarning: Please use company internal repo for private package downloads, For example : pip install your_package_name --index-url=https://mirrors.tencent.com/#/private/pypi.\033[0m')
         print('\033[91m*************************************************************************************************************************************\033[0m')
         print('\033[91m*************************************************************************************************************************************\033[0m')
-        try:
-          raise RuntimeError('do not install!')
-        except RuntimeError as e:
-           print('you have no permission to install this package!!!')
+        raise RuntimeError('do not install!')
     _post_actions()
     return setup
 
 setup(
     name = 'ronnytest',
-    version = '0.2.6',
+    version = '0.2.7',
     author = 'wxpay_sec_team',
     author_email = 'wxpay_sec_team@tencent.com',
     packages = find_packages(),
     install_requires=[""],
     tests_require=[],
 )
```

