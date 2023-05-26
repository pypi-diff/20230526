# Comparing `tmp/as400-1.0.3.tar.gz` & `tmp/as400-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/as400-1.0.3.tar", last modified: Fri May 26 01:27:59 2023, max compression
+gzip compressed data, was "dist/as400-1.0.4.tar", last modified: Fri May 26 01:46:19 2023, max compression
```

## Comparing `as400-1.0.3.tar` & `as400-1.0.4.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxr-xr-x   0 caionovelini   (501) staff       (20)        0 2023-05-26 01:27:59.000000 as400-1.0.3/
--rw-r--r--   0 caionovelini   (501) staff       (20)       79 2023-05-26 01:27:59.000000 as400-1.0.3/PKG-INFO
-drwxr-xr-x   0 caionovelini   (501) staff       (20)        0 2023-05-26 01:27:59.000000 as400-1.0.3/as400/
--rw-r--r--   0 caionovelini   (501) staff       (20)        0 2023-05-09 11:46:22.000000 as400-1.0.3/as400/__init__.py
--rw-r--r--   0 caionovelini   (501) staff       (20)       25 2023-05-26 01:26:51.000000 as400-1.0.3/as400/as400.py
-drwxr-xr-x   0 caionovelini   (501) staff       (20)        0 2023-05-26 01:27:59.000000 as400-1.0.3/as400.egg-info/
--rw-r--r--   0 caionovelini   (501) staff       (20)       79 2023-05-26 01:27:59.000000 as400-1.0.3/as400.egg-info/PKG-INFO
--rw-r--r--   0 caionovelini   (501) staff       (20)      157 2023-05-26 01:27:59.000000 as400-1.0.3/as400.egg-info/SOURCES.txt
--rw-r--r--   0 caionovelini   (501) staff       (20)        1 2023-05-26 01:27:59.000000 as400-1.0.3/as400.egg-info/dependency_links.txt
--rw-r--r--   0 caionovelini   (501) staff       (20)        6 2023-05-26 01:27:59.000000 as400-1.0.3/as400.egg-info/top_level.txt
--rw-r--r--   0 caionovelini   (501) staff       (20)       38 2023-05-26 01:27:59.000000 as400-1.0.3/setup.cfg
--rw-r--r--   0 caionovelini   (501) staff       (20)     1063 2023-05-26 01:27:42.000000 as400-1.0.3/setup.py
+drwxr-xr-x   0 caionovelini   (501) staff       (20)        0 2023-05-26 01:46:19.000000 as400-1.0.4/
+-rw-r--r--   0 caionovelini   (501) staff       (20)       79 2023-05-26 01:46:19.000000 as400-1.0.4/PKG-INFO
+drwxr-xr-x   0 caionovelini   (501) staff       (20)        0 2023-05-26 01:46:19.000000 as400-1.0.4/as400/
+-rw-r--r--   0 caionovelini   (501) staff       (20)        0 2023-05-09 11:46:22.000000 as400-1.0.4/as400/__init__.py
+-rw-r--r--   0 caionovelini   (501) staff       (20)       25 2023-05-26 01:26:51.000000 as400-1.0.4/as400/as400.py
+drwxr-xr-x   0 caionovelini   (501) staff       (20)        0 2023-05-26 01:46:19.000000 as400-1.0.4/as400/driver/
+-rwxr-xr-x   0 caionovelini   (501) staff       (20)  5171342 2022-05-19 19:23:07.000000 as400-1.0.4/as400/driver/ibm-iaccess-1.1.0.15-1.0.amd64.deb
+drwxr-xr-x   0 caionovelini   (501) staff       (20)        0 2023-05-26 01:46:19.000000 as400-1.0.4/as400.egg-info/
+-rw-r--r--   0 caionovelini   (501) staff       (20)       79 2023-05-26 01:46:19.000000 as400-1.0.4/as400.egg-info/PKG-INFO
+-rw-r--r--   0 caionovelini   (501) staff       (20)      205 2023-05-26 01:46:19.000000 as400-1.0.4/as400.egg-info/SOURCES.txt
+-rw-r--r--   0 caionovelini   (501) staff       (20)        1 2023-05-26 01:46:19.000000 as400-1.0.4/as400.egg-info/dependency_links.txt
+-rw-r--r--   0 caionovelini   (501) staff       (20)        6 2023-05-26 01:46:19.000000 as400-1.0.4/as400.egg-info/top_level.txt
+-rw-r--r--   0 caionovelini   (501) staff       (20)       38 2023-05-26 01:46:19.000000 as400-1.0.4/setup.cfg
+-rw-r--r--   0 caionovelini   (501) staff       (20)     1069 2023-05-26 01:43:56.000000 as400-1.0.4/setup.py
```

### Comparing `as400-1.0.3/setup.py` & `as400-1.0.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 
 class CustomInstall(install):
     def run(self):
         # Run custom installation commands here
         print("Running custom installation commands")
 
         # Execute dpkg -i command
-        deb_file_path = "driver/ibm-iaccess-1.1.0.15-1.0.amd64.deb"
+        deb_file_path = "as400/driver/ibm-iaccess-1.1.0.15-1.0.amd64.deb"
         dpkg_install_command = ["dpkg", "-i", deb_file_path]
         subprocess.check_call(["apt-get", "update"])
         subprocess.check_call(["apt-get", "install", "-y", "gcc"])
         subprocess.check_call(["apt-get" , "install", "-y", "g++"])
         subprocess.check_call(["apt-get", "-y" ,  "install" ,"unixodbc", "unixodbc-dev"])
         subprocess.check_call(["apt-get", "-y" , "install", "nginx"])
         subprocess.check_call(dpkg_install_command)
 
         install.run(self)
 setup(
     name='as400',
-    version='1.0.3',
+    version='1.0.4',
     description='Package as400-driver',
     packages=['as400'],
     package_data={'as400': ['driver/ibm-iaccess-1.1.0.15-1.0.amd64.deb']},
     cmdclass={'install': CustomInstall}
 )
```

