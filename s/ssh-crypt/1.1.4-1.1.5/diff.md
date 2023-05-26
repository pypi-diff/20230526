# Comparing `tmp/ssh-crypt-1.1.4.tar.gz` & `tmp/ssh-crypt-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssh-crypt-1.1.4.tar", last modified: Fri May 26 04:52:31 2023, max compression
+gzip compressed data, was "ssh-crypt-1.1.5.tar", last modified: Fri May 26 05:06:21 2023, max compression
```

## Comparing `ssh-crypt-1.1.4.tar` & `ssh-crypt-1.1.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-26 04:52:31.083265 ssh-crypt-1.1.4/
--rw-r--r--   0 user       (501) staff       (20)       45 2022-12-09 09:10:04.000000 ssh-crypt-1.1.4/MANIFEST.in
--rw-r--r--   0 user       (501) staff       (20)     7253 2023-05-26 04:52:31.083075 ssh-crypt-1.1.4/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)     6969 2023-05-25 14:53:13.000000 ssh-crypt-1.1.4/README.md
--rw-r--r--   0 user       (501) staff       (20)     1460 2022-12-09 09:10:04.000000 ssh-crypt-1.1.4/license.txt
--rw-r--r--   0 user       (501) staff       (20)       36 2021-03-30 07:40:28.000000 ssh-crypt-1.1.4/requirements.txt
--rw-r--r--   0 user       (501) staff       (20)       38 2023-05-26 04:52:31.083316 ssh-crypt-1.1.4/setup.cfg
--rw-r--r--   0 user       (501) staff       (20)      929 2023-05-26 04:52:08.000000 ssh-crypt-1.1.4/setup.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-26 04:52:31.081348 ssh-crypt-1.1.4/ssh_crypt/
--rw-r--r--   0 user       (501) staff       (20)       53 2021-03-30 12:27:03.000000 ssh-crypt-1.1.4/ssh_crypt/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     9661 2022-12-13 12:12:07.000000 ssh-crypt-1.1.4/ssh_crypt/ssh_crypt.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-26 04:52:31.082537 ssh-crypt-1.1.4/ssh_crypt.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     7253 2023-05-26 04:52:31.000000 ssh-crypt-1.1.4/ssh_crypt.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      358 2023-05-26 04:52:31.000000 ssh-crypt-1.1.4/ssh_crypt.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2023-05-26 04:52:31.000000 ssh-crypt-1.1.4/ssh_crypt.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)       45 2023-05-26 04:52:31.000000 ssh-crypt-1.1.4/ssh_crypt.egg-info/entry_points.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2023-05-26 04:52:30.000000 ssh-crypt-1.1.4/ssh_crypt.egg-info/not-zip-safe
--rw-r--r--   0 user       (501) staff       (20)       36 2023-05-26 04:52:31.000000 ssh-crypt-1.1.4/ssh_crypt.egg-info/requires.txt
--rw-r--r--   0 user       (501) staff       (20)       10 2023-05-26 04:52:31.000000 ssh-crypt-1.1.4/ssh_crypt.egg-info/top_level.txt
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-26 04:52:31.082675 ssh-crypt-1.1.4/tests/
--rw-r--r--   0 user       (501) staff       (20)     8973 2021-07-29 06:27:04.000000 ssh-crypt-1.1.4/tests/test_encrypt.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-26 05:06:21.652350 ssh-crypt-1.1.5/
+-rw-r--r--   0 user       (501) staff       (20)       45 2022-12-09 09:10:04.000000 ssh-crypt-1.1.5/MANIFEST.in
+-rw-r--r--   0 user       (501) staff       (20)     7253 2023-05-26 05:06:21.652118 ssh-crypt-1.1.5/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)     6969 2023-05-25 14:53:13.000000 ssh-crypt-1.1.5/README.md
+-rw-r--r--   0 user       (501) staff       (20)     1460 2022-12-09 09:10:04.000000 ssh-crypt-1.1.5/license.txt
+-rw-r--r--   0 user       (501) staff       (20)       37 2023-05-26 05:03:14.000000 ssh-crypt-1.1.5/requirements.txt
+-rw-r--r--   0 user       (501) staff       (20)       38 2023-05-26 05:06:21.652413 ssh-crypt-1.1.5/setup.cfg
+-rw-r--r--   0 user       (501) staff       (20)      929 2023-05-26 05:05:53.000000 ssh-crypt-1.1.5/setup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-26 05:06:21.650744 ssh-crypt-1.1.5/ssh_crypt/
+-rw-r--r--   0 user       (501) staff       (20)       53 2021-03-30 12:27:03.000000 ssh-crypt-1.1.5/ssh_crypt/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     9661 2022-12-13 12:12:07.000000 ssh-crypt-1.1.5/ssh_crypt/ssh_crypt.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-26 05:06:21.651745 ssh-crypt-1.1.5/ssh_crypt.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     7253 2023-05-26 05:06:21.000000 ssh-crypt-1.1.5/ssh_crypt.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      358 2023-05-26 05:06:21.000000 ssh-crypt-1.1.5/ssh_crypt.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2023-05-26 05:06:21.000000 ssh-crypt-1.1.5/ssh_crypt.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)       45 2023-05-26 05:06:21.000000 ssh-crypt-1.1.5/ssh_crypt.egg-info/entry_points.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2023-05-26 05:06:21.000000 ssh-crypt-1.1.5/ssh_crypt.egg-info/not-zip-safe
+-rw-r--r--   0 user       (501) staff       (20)       37 2023-05-26 05:06:21.000000 ssh-crypt-1.1.5/ssh_crypt.egg-info/requires.txt
+-rw-r--r--   0 user       (501) staff       (20)       10 2023-05-26 05:06:21.000000 ssh-crypt-1.1.5/ssh_crypt.egg-info/top_level.txt
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-26 05:06:21.651882 ssh-crypt-1.1.5/tests/
+-rw-r--r--   0 user       (501) staff       (20)     8973 2021-07-29 06:27:04.000000 ssh-crypt-1.1.5/tests/test_encrypt.py
```

### Comparing `ssh-crypt-1.1.4/PKG-INFO` & `ssh-crypt-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssh-crypt
-Version: 1.1.4
+Version: 1.1.5
 Summary: ssh-crypt is a tool to encrypt/decrypt data using your ssh key from ssh-agent
 Author: Maxim Nikitenko
 Author-email: iam@sets88.com
 License: BSD
 Platform: any
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

### Comparing `ssh-crypt-1.1.4/README.md` & `ssh-crypt-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `ssh-crypt-1.1.4/license.txt` & `ssh-crypt-1.1.5/license.txt`

 * *Files identical despite different names*

### Comparing `ssh-crypt-1.1.4/setup.py` & `ssh-crypt-1.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
             return f.readlines()
     except FileNotFoundError:
         raise RuntimeError('No requirements info found.')
 
 
 setup(
     name='ssh-crypt',
-    version='1.1.4',
+    version='1.1.5',
     license='BSD',
     author='Maxim Nikitenko',
     author_email='iam@sets88.com',
     packages=find_packages(),
     description='ssh-crypt is a tool to encrypt/decrypt data using your ssh key from ssh-agent',\
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

### Comparing `ssh-crypt-1.1.4/ssh_crypt/ssh_crypt.py` & `ssh-crypt-1.1.5/ssh_crypt/ssh_crypt.py`

 * *Files identical despite different names*

### Comparing `ssh-crypt-1.1.4/ssh_crypt.egg-info/PKG-INFO` & `ssh-crypt-1.1.5/ssh_crypt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssh-crypt
-Version: 1.1.4
+Version: 1.1.5
 Summary: ssh-crypt is a tool to encrypt/decrypt data using your ssh key from ssh-agent
 Author: Maxim Nikitenko
 Author-email: iam@sets88.com
 License: BSD
 Platform: any
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

### Comparing `ssh-crypt-1.1.4/tests/test_encrypt.py` & `ssh-crypt-1.1.5/tests/test_encrypt.py`

 * *Files identical despite different names*

