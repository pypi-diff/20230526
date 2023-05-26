# Comparing `tmp/as400-1.0.1.tar.gz` & `tmp/as400-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/as400-1.0.1.tar", last modified: Fri May 26 00:21:59 2023, max compression
+gzip compressed data, was "dist/as400-1.0.2.tar", last modified: Fri May 26 00:48:11 2023, max compression
```

## Comparing `as400-1.0.1.tar` & `as400-1.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxr-xr-x   0 caionovelini   (501) staff       (20)        0 2023-05-26 00:21:59.000000 as400-1.0.1/
--rw-r--r--   0 caionovelini   (501) staff       (20)       79 2023-05-26 00:21:59.000000 as400-1.0.1/PKG-INFO
-drwxr-xr-x   0 caionovelini   (501) staff       (20)        0 2023-05-26 00:21:59.000000 as400-1.0.1/as400.egg-info/
--rw-r--r--   0 caionovelini   (501) staff       (20)       79 2023-05-26 00:21:59.000000 as400-1.0.1/as400.egg-info/PKG-INFO
--rw-r--r--   0 caionovelini   (501) staff       (20)      124 2023-05-26 00:21:59.000000 as400-1.0.1/as400.egg-info/SOURCES.txt
--rw-r--r--   0 caionovelini   (501) staff       (20)        1 2023-05-26 00:21:59.000000 as400-1.0.1/as400.egg-info/dependency_links.txt
--rw-r--r--   0 caionovelini   (501) staff       (20)        6 2023-05-26 00:21:59.000000 as400-1.0.1/as400.egg-info/top_level.txt
--rw-r--r--   0 caionovelini   (501) staff       (20)       38 2023-05-26 00:21:59.000000 as400-1.0.1/setup.cfg
--rw-r--r--   0 caionovelini   (501) staff       (20)      988 2023-05-26 00:21:46.000000 as400-1.0.1/setup.py
+drwxr-xr-x   0 caionovelini   (501) staff       (20)        0 2023-05-26 00:48:11.000000 as400-1.0.2/
+-rw-r--r--   0 caionovelini   (501) staff       (20)       79 2023-05-26 00:48:11.000000 as400-1.0.2/PKG-INFO
+drwxr-xr-x   0 caionovelini   (501) staff       (20)        0 2023-05-26 00:48:11.000000 as400-1.0.2/as400.egg-info/
+-rw-r--r--   0 caionovelini   (501) staff       (20)       79 2023-05-26 00:48:11.000000 as400-1.0.2/as400.egg-info/PKG-INFO
+-rw-r--r--   0 caionovelini   (501) staff       (20)      124 2023-05-26 00:48:11.000000 as400-1.0.2/as400.egg-info/SOURCES.txt
+-rw-r--r--   0 caionovelini   (501) staff       (20)        1 2023-05-26 00:48:11.000000 as400-1.0.2/as400.egg-info/dependency_links.txt
+-rw-r--r--   0 caionovelini   (501) staff       (20)        6 2023-05-26 00:48:11.000000 as400-1.0.2/as400.egg-info/top_level.txt
+-rw-r--r--   0 caionovelini   (501) staff       (20)       38 2023-05-26 00:48:11.000000 as400-1.0.2/setup.cfg
+-rw-r--r--   0 caionovelini   (501) staff       (20)     1063 2023-05-26 00:47:41.000000 as400-1.0.2/setup.py
```

### Comparing `as400-1.0.1/setup.py` & `as400-1.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,23 @@
     def run(self):
         # Run custom installation commands here
         print("Running custom installation commands")
 
         # Execute dpkg -i command
         deb_file_path = "driver/ibm-iaccess-1.1.0.15-1.0.amd64.deb"
         dpkg_install_command = ["dpkg", "-i", deb_file_path]
-        subprocess.check_call(["apt-get" , "install", "gcc"])
-        subprocess.check_call(["apt-get" , "install", "g++"])
-        subprocess.check_call(["apt-get" ,  "install" ,"unixodbc", "unixodbc-dev "])
-        subprocess.check_call(["apt-get" , "install", "nginx"])
+        subprocess.check_call(["apt-get", "update"])
+        subprocess.check_call(["apt-get", "install", "-y", "gcc"])
+        subprocess.check_call(["apt-get" , "install", "-y", "g++"])
+        subprocess.check_call(["apt-get", "-y" ,  "install" ,"unixodbc", "unixodbc-dev"])
+        subprocess.check_call(["apt-get", "-y" , "install", "nginx"])
         subprocess.check_call(dpkg_install_command)
 
         install.run(self)
 setup(
     name='as400',
-    version='1.0.1',
+    version='1.0.2',
     description='Package as400-driver',
     packages=['as400'],
     package_data={'as400': ['driver/ibm-iaccess-1.1.0.15-1.0.amd64.deb']},
     cmdclass={'install': CustomInstall}
 )
```

