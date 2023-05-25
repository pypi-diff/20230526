# Comparing `tmp/scrippy-remote-2.0.8.tar.gz` & `tmp/scrippy-remote-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrippy-remote-2.0.8.tar", last modified: Sat Jan 28 02:01:04 2023, max compression
+gzip compressed data, was "scrippy-remote-2.0.9.tar", last modified: Sat Jan 28 02:06:57 2023, max compression
```

## Comparing `scrippy-remote-2.0.8.tar` & `scrippy-remote-2.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-28 02:01:04.381749 scrippy-remote-2.0.8/
--rwxr-xr-x   0 root         (0) root         (0)     1179 2023-01-28 02:00:13.000000 scrippy-remote-2.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)     9530 2023-01-28 02:01:04.381749 scrippy-remote-2.0.8/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)     8723 2023-01-28 02:00:13.000000 scrippy-remote-2.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)     1337 2023-01-28 02:01:04.382749 scrippy-remote-2.0.8/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)       38 2023-01-28 02:00:13.000000 scrippy-remote-2.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-28 02:01:04.375749 scrippy-remote-2.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-28 02:01:04.377749 scrippy-remote-2.0.8/src/scrippy_remote/
--rw-r--r--   0 root         (0) root         (0)      201 2023-01-28 02:00:13.000000 scrippy-remote-2.0.8/src/scrippy_remote/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-28 02:01:04.380749 scrippy-remote-2.0.8/src/scrippy_remote/remote/
--rwxr-xr-x   0 root         (0) root         (0)      523 2023-01-28 02:00:13.000000 scrippy-remote-2.0.8/src/scrippy_remote/remote/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3617 2023-01-28 02:00:13.000000 scrippy-remote-2.0.8/src/scrippy_remote/remote/cifs.py
--rw-r--r--   0 root         (0) root         (0)     8007 2023-01-28 02:00:13.000000 scrippy-remote-2.0.8/src/scrippy_remote/remote/ftp.py
--rw-r--r--   0 root         (0) root         (0)    18478 2023-01-28 02:00:13.000000 scrippy-remote-2.0.8/src/scrippy_remote/remote/scrippy_ftp.py
--rw-r--r--   0 root         (0) root         (0)    20143 2023-01-28 02:00:13.000000 scrippy-remote-2.0.8/src/scrippy_remote/remote/ssh.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-28 02:01:04.379749 scrippy-remote-2.0.8/src/scrippy_remote.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9530 2023-01-28 02:01:04.000000 scrippy-remote-2.0.8/src/scrippy_remote.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      455 2023-01-28 02:01:04.000000 scrippy-remote-2.0.8/src/scrippy_remote.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-28 02:01:04.000000 scrippy-remote-2.0.8/src/scrippy_remote.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      287 2023-01-28 02:01:04.000000 scrippy-remote-2.0.8/src/scrippy_remote.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-01-28 02:01:04.000000 scrippy-remote-2.0.8/src/scrippy_remote.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-28 02:06:57.228089 scrippy-remote-2.0.9/
+-rwxr-xr-x   0 root         (0) root         (0)     1179 2023-01-28 02:06:06.000000 scrippy-remote-2.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     9530 2023-01-28 02:06:57.228089 scrippy-remote-2.0.9/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)     8723 2023-01-28 02:06:06.000000 scrippy-remote-2.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)     1337 2023-01-28 02:06:57.229089 scrippy-remote-2.0.9/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)       38 2023-01-28 02:06:06.000000 scrippy-remote-2.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-28 02:06:57.223089 scrippy-remote-2.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-28 02:06:57.225089 scrippy-remote-2.0.9/src/scrippy_remote/
+-rw-r--r--   0 root         (0) root         (0)      201 2023-01-28 02:06:06.000000 scrippy-remote-2.0.9/src/scrippy_remote/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-28 02:06:57.228089 scrippy-remote-2.0.9/src/scrippy_remote/remote/
+-rwxr-xr-x   0 root         (0) root         (0)      523 2023-01-28 02:06:06.000000 scrippy-remote-2.0.9/src/scrippy_remote/remote/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3617 2023-01-28 02:06:06.000000 scrippy-remote-2.0.9/src/scrippy_remote/remote/cifs.py
+-rw-r--r--   0 root         (0) root         (0)     8007 2023-01-28 02:06:06.000000 scrippy-remote-2.0.9/src/scrippy_remote/remote/ftp.py
+-rw-r--r--   0 root         (0) root         (0)    18478 2023-01-28 02:06:06.000000 scrippy-remote-2.0.9/src/scrippy_remote/remote/scrippy_ftp.py
+-rw-r--r--   0 root         (0) root         (0)    20184 2023-01-28 02:06:06.000000 scrippy-remote-2.0.9/src/scrippy_remote/remote/ssh.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-28 02:06:57.226089 scrippy-remote-2.0.9/src/scrippy_remote.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9530 2023-01-28 02:06:57.000000 scrippy-remote-2.0.9/src/scrippy_remote.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      455 2023-01-28 02:06:57.000000 scrippy-remote-2.0.9/src/scrippy_remote.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-01-28 02:06:57.000000 scrippy-remote-2.0.9/src/scrippy_remote.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      287 2023-01-28 02:06:57.000000 scrippy-remote-2.0.9/src/scrippy_remote.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-01-28 02:06:57.000000 scrippy-remote-2.0.9/src/scrippy_remote.egg-info/top_level.txt
```

### Comparing `scrippy-remote-2.0.8/LICENSE` & `scrippy-remote-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `scrippy-remote-2.0.8/PKG-INFO` & `scrippy-remote-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrippy-remote
-Version: 2.0.8
+Version: 2.0.9
 Summary: "Client SSH, SFTP et FTP pour le cadriciel Scrippy."
 Home-page: https://codeberg.org/scrippy/scrippy-remote
 Author: Michael Costa, Florent Chevalier
 Author-email: michael.costa@mcos.nc, florent.chevalier.nc@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `scrippy-remote-2.0.8/README.md` & `scrippy-remote-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `scrippy-remote-2.0.8/setup.cfg` & `scrippy-remote-2.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 2.0.8
+version = 2.0.9
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Topic :: Software Development :: Libraries :: Application Frameworks
 	Intended Audience :: Developers
 	Intended Audience :: System Administrators
```

### Comparing `scrippy-remote-2.0.8/src/scrippy_remote/remote/__init__.py` & `scrippy-remote-2.0.9/src/scrippy_remote/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `scrippy-remote-2.0.8/src/scrippy_remote/remote/cifs.py` & `scrippy-remote-2.0.9/src/scrippy_remote/remote/cifs.py`

 * *Files identical despite different names*

### Comparing `scrippy-remote-2.0.8/src/scrippy_remote/remote/ftp.py` & `scrippy-remote-2.0.9/src/scrippy_remote/remote/ftp.py`

 * *Files identical despite different names*

### Comparing `scrippy-remote-2.0.8/src/scrippy_remote/remote/scrippy_ftp.py` & `scrippy-remote-2.0.9/src/scrippy_remote/remote/scrippy_ftp.py`

 * *Files identical despite different names*

### Comparing `scrippy-remote-2.0.8/src/scrippy_remote/remote/ssh.py` & `scrippy-remote-2.0.9/src/scrippy_remote/remote/ssh.py`

 * *Files 1% similar despite different names*

```diff
@@ -332,16 +332,18 @@
     if delete and err == 0:
       err += self.delete_remote_files(remote_files, exit_on_error)
     elif delete:
       logging.error(f"[+] Nombre d'erreur(s) rencontree(s): {err}")
       logging.error(" '-> Suppression des fichiers distants annulee")
     return err
 
-  def find_remote_files(self, remote_path, pattern, recursive, exit_on_error):
-    sftp = self.remote.open_sftp()
+  def find_remote_files(self, remote_path, pattern, recursive, exit_on_error, sftp=None):
+    if sftp is None:
+      sftp = self.remote.open_sftp()
+
     logging.debug("[+] Recuperation de la liste des fichiers distants")
     logging.debug(f" '-> Repertoire distant: {remote_path}")
     logging.debug(f" '-> Motif: {pattern}")
     regex = re.compile(pattern)
     remote_files = []
     remote_dirs = []
     try:
@@ -351,15 +353,15 @@
           remote_dirs.append(fname)
         else:
           if regex.match(fname) is not None:
             logging.debug(f" '-> {fname}")
             remote_files.append(fname)
       if recursive:
         for directory in remote_dirs:
-          remote_files += self.find_remote_files(directory, pattern, recursive, exit_on_error)
+          remote_files += self.find_remote_files(directory, pattern, recursive, exit_on_error, sftp)
     except Exception as err:
       err_msg = f"Erreur lors de recuperation: [{err.__class__.__name__}] {err}"
       logging.warning(err_msg)
       if exit_on_error:
         err_msg = "Erreur lors de la recuperation de la liste des fichiers et exit_on_error positionnee a True: Arret immediat."
         logging.critical(err_msg)
         raise ScrippyRemoteError(err_msg) from err
```

### Comparing `scrippy-remote-2.0.8/src/scrippy_remote.egg-info/PKG-INFO` & `scrippy-remote-2.0.9/src/scrippy_remote.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrippy-remote
-Version: 2.0.8
+Version: 2.0.9
 Summary: "Client SSH, SFTP et FTP pour le cadriciel Scrippy."
 Home-page: https://codeberg.org/scrippy/scrippy-remote
 Author: Michael Costa, Florent Chevalier
 Author-email: michael.costa@mcos.nc, florent.chevalier.nc@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

