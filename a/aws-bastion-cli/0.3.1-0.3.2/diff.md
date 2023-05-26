# Comparing `tmp/aws-bastion-cli-0.3.1.tar.gz` & `tmp/aws-bastion-cli-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-bastion-cli-0.3.1.tar", last modified: Tue May 23 07:34:28 2023, max compression
+gzip compressed data, was "aws-bastion-cli-0.3.2.tar", last modified: Fri May 26 05:50:31 2023, max compression
```

## Comparing `aws-bastion-cli-0.3.1.tar` & `aws-bastion-cli-0.3.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:34:28.789281 aws-bastion-cli-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-23 07:34:13.000000 aws-bastion-cli-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-23 07:34:28.789281 aws-bastion-cli-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-23 07:34:13.000000 aws-bastion-cli-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:34:28.789281 aws-bastion-cli-0.3.1/aws_bastion_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-23 07:34:28.000000 aws-bastion-cli-0.3.1/aws_bastion_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-23 07:34:28.000000 aws-bastion-cli-0.3.1/aws_bastion_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 07:34:28.000000 aws-bastion-cli-0.3.1/aws_bastion_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-23 07:34:28.000000 aws-bastion-cli-0.3.1/aws_bastion_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-23 07:34:28.000000 aws-bastion-cli-0.3.1/aws_bastion_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-23 07:34:28.000000 aws-bastion-cli-0.3.1/aws_bastion_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:34:28.789281 aws-bastion-cli-0.3.1/bastion_cli/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-23 07:34:13.000000 aws-bastion-cli-0.3.1/bastion_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13931 2023-05-23 07:34:13.000000 aws-bastion-cli-0.3.1/bastion_cli/command.py
--rw-r--r--   0 runner    (1001) docker     (123)    11131 2023-05-23 07:34:13.000000 aws-bastion-cli-0.3.1/bastion_cli/create_yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-05-23 07:34:13.000000 aws-bastion-cli-0.3.1/bastion_cli/deploy_cfn.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-23 07:34:13.000000 aws-bastion-cli-0.3.1/bastion_cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-23 07:34:13.000000 aws-bastion-cli-0.3.1/bastion_cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-23 07:34:13.000000 aws-bastion-cli-0.3.1/bastion_cli/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-23 07:34:28.789281 aws-bastion-cli-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-23 07:34:13.000000 aws-bastion-cli-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:50:31.748432 aws-bastion-cli-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-26 05:50:09.000000 aws-bastion-cli-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-26 05:50:31.748432 aws-bastion-cli-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-26 05:50:09.000000 aws-bastion-cli-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:50:31.748432 aws-bastion-cli-0.3.2/aws_bastion_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-26 05:50:31.000000 aws-bastion-cli-0.3.2/aws_bastion_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-26 05:50:31.000000 aws-bastion-cli-0.3.2/aws_bastion_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 05:50:31.000000 aws-bastion-cli-0.3.2/aws_bastion_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-26 05:50:31.000000 aws-bastion-cli-0.3.2/aws_bastion_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-26 05:50:31.000000 aws-bastion-cli-0.3.2/aws_bastion_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 05:50:31.000000 aws-bastion-cli-0.3.2/aws_bastion_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:50:31.748432 aws-bastion-cli-0.3.2/bastion_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-26 05:50:09.000000 aws-bastion-cli-0.3.2/bastion_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13931 2023-05-26 05:50:09.000000 aws-bastion-cli-0.3.2/bastion_cli/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11131 2023-05-26 05:50:09.000000 aws-bastion-cli-0.3.2/bastion_cli/create_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-05-26 05:50:09.000000 aws-bastion-cli-0.3.2/bastion_cli/deploy_cfn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-26 05:50:09.000000 aws-bastion-cli-0.3.2/bastion_cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-26 05:50:09.000000 aws-bastion-cli-0.3.2/bastion_cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-26 05:50:09.000000 aws-bastion-cli-0.3.2/bastion_cli/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-26 05:50:31.748432 aws-bastion-cli-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-26 05:50:09.000000 aws-bastion-cli-0.3.2/setup.py
```

### Comparing `aws-bastion-cli-0.3.1/LICENSE` & `aws-bastion-cli-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-bastion-cli-0.3.1/README.md` & `aws-bastion-cli-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `aws-bastion-cli-0.3.1/bastion_cli/command.py` & `aws-bastion-cli-0.3.2/bastion_cli/command.py`

 * *Files identical despite different names*

### Comparing `aws-bastion-cli-0.3.1/bastion_cli/create_yaml.py` & `aws-bastion-cli-0.3.2/bastion_cli/create_yaml.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
             }
 
             self.instance_profile = {
                 'Ref': 'InstanceProfile'
             }
 
         elif role['name'] is not None:
-            self.instance_profile = role['Name']
+            self.instance_profile = role['name']
 
         else:
             self.instance_profile = {
                 'Ref': 'AWS::NoValue'
             }
 
     def create_sg(self, vpc, sg, host, port):
```

### Comparing `aws-bastion-cli-0.3.1/bastion_cli/deploy_cfn.py` & `aws-bastion-cli-0.3.2/bastion_cli/deploy_cfn.py`

 * *Files identical despite different names*

### Comparing `aws-bastion-cli-0.3.1/bastion_cli/main.py` & `aws-bastion-cli-0.3.2/bastion_cli/main.py`

 * *Files identical despite different names*

### Comparing `aws-bastion-cli-0.3.1/bastion_cli/utils.py` & `aws-bastion-cli-0.3.2/bastion_cli/utils.py`

 * *Files identical despite different names*

### Comparing `aws-bastion-cli-0.3.1/bastion_cli/validators.py` & `aws-bastion-cli-0.3.2/bastion_cli/validators.py`

 * *Files identical despite different names*

### Comparing `aws-bastion-cli-0.3.1/setup.py` & `aws-bastion-cli-0.3.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     'six>=1.16.0',
     'urllib3>=1.26.14',
     'wcwidth>=0.2.6',
 ]
 
 setup(
     name='aws-bastion-cli',
-    version='0.3.1',
+    version='0.3.2',
     author='marcus16-kang',
     description='AWS Bastion EC2 Server Stack Generator',
     author_email='marcus16-kang@outlook.com',
     license='MIT',
     entry_points={
         'console_scripts': [
             'bastion-cli=bastion_cli.main:main'
```

