# Comparing `tmp/as400-1.0.2.tar.gz` & `tmp/as400-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/as400-1.0.2.tar", last modified: Fri May 26 00:48:11 2023, max compression
+gzip compressed data, was "dist/as400-1.0.3.tar", last modified: Fri May 26 01:27:59 2023, max compression
```

## Comparing `as400-1.0.2.tar` & `as400-1.0.3.tar`

### file list

```diff
@@ -1,9 +1,12 @@
-drwxr-xr-x   0 caionovelini   (501) staff       (20)        0 2023-05-26 00:48:11.000000 as400-1.0.2/
--rw-r--r--   0 caionovelini   (501) staff       (20)       79 2023-05-26 00:48:11.000000 as400-1.0.2/PKG-INFO
-drwxr-xr-x   0 caionovelini   (501) staff       (20)        0 2023-05-26 00:48:11.000000 as400-1.0.2/as400.egg-info/
--rw-r--r--   0 caionovelini   (501) staff       (20)       79 2023-05-26 00:48:11.000000 as400-1.0.2/as400.egg-info/PKG-INFO
--rw-r--r--   0 caionovelini   (501) staff       (20)      124 2023-05-26 00:48:11.000000 as400-1.0.2/as400.egg-info/SOURCES.txt
--rw-r--r--   0 caionovelini   (501) staff       (20)        1 2023-05-26 00:48:11.000000 as400-1.0.2/as400.egg-info/dependency_links.txt
--rw-r--r--   0 caionovelini   (501) staff       (20)        6 2023-05-26 00:48:11.000000 as400-1.0.2/as400.egg-info/top_level.txt
--rw-r--r--   0 caionovelini   (501) staff       (20)       38 2023-05-26 00:48:11.000000 as400-1.0.2/setup.cfg
--rw-r--r--   0 caionovelini   (501) staff       (20)     1063 2023-05-26 00:47:41.000000 as400-1.0.2/setup.py
+drwxr-xr-x   0 caionovelini   (501) staff       (20)        0 2023-05-26 01:27:59.000000 as400-1.0.3/
+-rw-r--r--   0 caionovelini   (501) staff       (20)       79 2023-05-26 01:27:59.000000 as400-1.0.3/PKG-INFO
+drwxr-xr-x   0 caionovelini   (501) staff       (20)        0 2023-05-26 01:27:59.000000 as400-1.0.3/as400/
+-rw-r--r--   0 caionovelini   (501) staff       (20)        0 2023-05-09 11:46:22.000000 as400-1.0.3/as400/__init__.py
+-rw-r--r--   0 caionovelini   (501) staff       (20)       25 2023-05-26 01:26:51.000000 as400-1.0.3/as400/as400.py
+drwxr-xr-x   0 caionovelini   (501) staff       (20)        0 2023-05-26 01:27:59.000000 as400-1.0.3/as400.egg-info/
+-rw-r--r--   0 caionovelini   (501) staff       (20)       79 2023-05-26 01:27:59.000000 as400-1.0.3/as400.egg-info/PKG-INFO
+-rw-r--r--   0 caionovelini   (501) staff       (20)      157 2023-05-26 01:27:59.000000 as400-1.0.3/as400.egg-info/SOURCES.txt
+-rw-r--r--   0 caionovelini   (501) staff       (20)        1 2023-05-26 01:27:59.000000 as400-1.0.3/as400.egg-info/dependency_links.txt
+-rw-r--r--   0 caionovelini   (501) staff       (20)        6 2023-05-26 01:27:59.000000 as400-1.0.3/as400.egg-info/top_level.txt
+-rw-r--r--   0 caionovelini   (501) staff       (20)       38 2023-05-26 01:27:59.000000 as400-1.0.3/setup.cfg
+-rw-r--r--   0 caionovelini   (501) staff       (20)     1063 2023-05-26 01:27:42.000000 as400-1.0.3/setup.py
```

### Comparing `as400-1.0.2/setup.py` & `as400-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,13 +16,13 @@
         subprocess.check_call(["apt-get", "-y" ,  "install" ,"unixodbc", "unixodbc-dev"])
         subprocess.check_call(["apt-get", "-y" , "install", "nginx"])
         subprocess.check_call(dpkg_install_command)
 
         install.run(self)
 setup(
     name='as400',
-    version='1.0.2',
+    version='1.0.3',
     description='Package as400-driver',
     packages=['as400'],
     package_data={'as400': ['driver/ibm-iaccess-1.1.0.15-1.0.amd64.deb']},
     cmdclass={'install': CustomInstall}
 )
```

