# Comparing `tmp/sas-airflow-provider-0.0.1.tar.gz` & `tmp/sas-airflow-provider-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sas-airflow-provider-0.0.1.tar", last modified: Wed Jan 11 20:37:44 2023, max compression
+gzip compressed data, was "/home/runner/work/sas-airflow-provider/sas-airflow-provider/dist/.tmp-kibsn5oh/sas-airflow-provider-0.0.3.tar", last modified: Fri May 26 20:22:25 2023, max compression
```

## Comparing `sas-airflow-provider-0.0.1.tar` & `sas-airflow-provider-0.0.3.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 anshak     (501) staff       (20)        0 2023-01-11 20:37:44.397611 sas-airflow-provider-0.0.1/
--rw-r--r--   0 anshak     (501) staff       (20)    11358 2023-01-11 20:33:03.000000 sas-airflow-provider-0.0.1/LICENSE
--rw-r--r--   0 anshak     (501) staff       (20)     4045 2023-01-11 20:37:44.397797 sas-airflow-provider-0.0.1/PKG-INFO
--rw-r--r--   0 anshak     (501) staff       (20)     3499 2023-01-11 20:33:03.000000 sas-airflow-provider-0.0.1/README.md
--rw-r--r--   0 anshak     (501) staff       (20)      105 2023-01-11 20:33:03.000000 sas-airflow-provider-0.0.1/pyproject.toml
--rw-r--r--   0 anshak     (501) staff       (20)      785 2023-01-11 20:37:44.398555 sas-airflow-provider-0.0.1/setup.cfg
-drwxr-xr-x   0 anshak     (501) staff       (20)        0 2023-01-11 20:37:44.386840 sas-airflow-provider-0.0.1/src/
-drwxr-xr-x   0 anshak     (501) staff       (20)        0 2023-01-11 20:37:44.389396 sas-airflow-provider-0.0.1/src/sas_airflow_provider/
--rw-r--r--   0 anshak     (501) staff       (20)      388 2023-01-11 20:33:03.000000 sas-airflow-provider-0.0.1/src/sas_airflow_provider/__init__.py
-drwxr-xr-x   0 anshak     (501) staff       (20)        0 2023-01-11 20:37:44.393840 sas-airflow-provider-0.0.1/src/sas_airflow_provider/example_dags/
--rw-r--r--   0 anshak     (501) staff       (20)      785 2023-01-11 20:33:03.000000 sas-airflow-provider-0.0.1/src/sas_airflow_provider/example_dags/__init__.py
--rw-r--r--   0 anshak     (501) staff       (20)     1427 2023-01-11 20:33:03.000000 sas-airflow-provider-0.0.1/src/sas_airflow_provider/example_dags/example_sas_jobexecution.py
--rw-r--r--   0 anshak     (501) staff       (20)     1716 2023-01-11 20:33:03.000000 sas-airflow-provider-0.0.1/src/sas_airflow_provider/example_dags/example_sas_studioflow.py
-drwxr-xr-x   0 anshak     (501) staff       (20)        0 2023-01-11 20:37:44.395123 sas-airflow-provider-0.0.1/src/sas_airflow_provider/hooks/
--rw-r--r--   0 anshak     (501) staff       (20)      785 2023-01-11 20:33:03.000000 sas-airflow-provider-0.0.1/src/sas_airflow_provider/hooks/__init__.py
--rw-r--r--   0 anshak     (501) staff       (20)     3721 2023-01-11 20:33:03.000000 sas-airflow-provider-0.0.1/src/sas_airflow_provider/hooks/sas.py
-drwxr-xr-x   0 anshak     (501) staff       (20)        0 2023-01-11 20:37:44.397157 sas-airflow-provider-0.0.1/src/sas_airflow_provider/operators/
--rw-r--r--   0 anshak     (501) staff       (20)      787 2023-01-11 20:33:03.000000 sas-airflow-provider-0.0.1/src/sas_airflow_provider/operators/__init__.py
--rw-r--r--   0 anshak     (501) staff       (20)     2772 2023-01-11 20:33:03.000000 sas-airflow-provider-0.0.1/src/sas_airflow_provider/operators/sas_jobexecution.py
--rw-r--r--   0 anshak     (501) staff       (20)    10072 2023-01-11 20:33:03.000000 sas-airflow-provider-0.0.1/src/sas_airflow_provider/operators/sas_studioflow.py
-drwxr-xr-x   0 anshak     (501) staff       (20)        0 2023-01-11 20:37:44.391746 sas-airflow-provider-0.0.1/src/sas_airflow_provider.egg-info/
--rw-r--r--   0 anshak     (501) staff       (20)     4045 2023-01-11 20:37:44.000000 sas-airflow-provider-0.0.1/src/sas_airflow_provider.egg-info/PKG-INFO
--rw-r--r--   0 anshak     (501) staff       (20)      738 2023-01-11 20:37:44.000000 sas-airflow-provider-0.0.1/src/sas_airflow_provider.egg-info/SOURCES.txt
--rw-r--r--   0 anshak     (501) staff       (20)        1 2023-01-11 20:37:44.000000 sas-airflow-provider-0.0.1/src/sas_airflow_provider.egg-info/dependency_links.txt
--rw-r--r--   0 anshak     (501) staff       (20)       90 2023-01-11 20:37:44.000000 sas-airflow-provider-0.0.1/src/sas_airflow_provider.egg-info/entry_points.txt
--rw-r--r--   0 anshak     (501) staff       (20)       21 2023-01-11 20:37:44.000000 sas-airflow-provider-0.0.1/src/sas_airflow_provider.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:22:25.000000 sas-airflow-provider-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-26 20:22:12.000000 sas-airflow-provider-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-05-26 20:22:25.000000 sas-airflow-provider-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-05-26 20:22:12.000000 sas-airflow-provider-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 20:22:12.000000 sas-airflow-provider-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-26 20:22:25.000000 sas-airflow-provider-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:22:25.000000 sas-airflow-provider-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:22:25.000000 sas-airflow-provider-0.0.3/src/sas_airflow_provider/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 20:22:12.000000 sas-airflow-provider-0.0.3/src/sas_airflow_provider/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:22:25.000000 sas-airflow-provider-0.0.3/src/sas_airflow_provider/example_dags/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-26 20:22:12.000000 sas-airflow-provider-0.0.3/src/sas_airflow_provider/example_dags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-26 20:22:12.000000 sas-airflow-provider-0.0.3/src/sas_airflow_provider/example_dags/example_sas_jobexecution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-26 20:22:12.000000 sas-airflow-provider-0.0.3/src/sas_airflow_provider/example_dags/example_sas_studioflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-05-26 20:22:12.000000 sas-airflow-provider-0.0.3/src/sas_airflow_provider/example_dags/example_templating.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:22:25.000000 sas-airflow-provider-0.0.3/src/sas_airflow_provider/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-26 20:22:12.000000 sas-airflow-provider-0.0.3/src/sas_airflow_provider/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-05-26 20:22:12.000000 sas-airflow-provider-0.0.3/src/sas_airflow_provider/hooks/sas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:22:25.000000 sas-airflow-provider-0.0.3/src/sas_airflow_provider/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-26 20:22:12.000000 sas-airflow-provider-0.0.3/src/sas_airflow_provider/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-26 20:22:12.000000 sas-airflow-provider-0.0.3/src/sas_airflow_provider/operators/sas_jobexecution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11079 2023-05-26 20:22:12.000000 sas-airflow-provider-0.0.3/src/sas_airflow_provider/operators/sas_studioflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:22:25.000000 sas-airflow-provider-0.0.3/src/sas_airflow_provider.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-05-26 20:22:25.000000 sas-airflow-provider-0.0.3/src/sas_airflow_provider.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-26 20:22:25.000000 sas-airflow-provider-0.0.3/src/sas_airflow_provider.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 20:22:25.000000 sas-airflow-provider-0.0.3/src/sas_airflow_provider.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-26 20:22:25.000000 sas-airflow-provider-0.0.3/src/sas_airflow_provider.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-26 20:22:25.000000 sas-airflow-provider-0.0.3/src/sas_airflow_provider.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `sas-airflow-provider-0.0.1/LICENSE` & `sas-airflow-provider-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sas-airflow-provider-0.0.1/PKG-INFO` & `sas-airflow-provider-0.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,62 +1,71 @@
 Metadata-Version: 2.1
 Name: sas-airflow-provider
-Version: 0.0.1
+Version: 0.0.3
 Summary: Enables execution of Studio Flows and Jobs from Airflow
 Home-page: https://github.com/sassoftware/sas-airflow-provider
 Author: SAS
 Author-email: andrew.shakinovsky@sas.com
 Project-URL: Bug Tracker, https://github.com/sassoftware
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# SAS Airflow Provider
+# SAS&reg; Airflow Provider
 
-## Current major capabilities of SAS Studio Flow Operator
+## Current major capabilities of the SAS&reg; Studio Flow Operator
 
-* Execute Studio Flow stored either on File System or in SAS Content
-* Select Compute Context to be used for execution of Studio Flow
-* Specify whether SAS logs of Studio Flow execution should be returned and displayed in Airflow or not
+* Execute a SAS Studio Flow stored either on the File System or in SAS Content
+* Select the Compute Context to be used for execution of a SAS Studio Flow
+* Specify whether SAS logs of a SAS Studio Flow execution should be returned and displayed in Airflow
 * Specify parameters (init_code, wrap_code) to be used for code generation
-* Honor return code of SAS Studio Flow in Airflow. In particular, if SAS Studio Flow fails, Airflow raises exception as well and stop execution
-* Authentication via oauth token or via user/password (i.e. generation of oauth token prior to each call)
+* Honor return code of a SAS Studio Flow in Airflow. In particular, if a SAS Studio Flow fails, Airflow raises an exception as well and stops execution
+* Authenticate via oauth token or via user/password (i.e. generation of oauth token prior to each call)
 
 
 ## Getting started
 ### Install Airflow
 Follow instructions at https://airflow.apache.org/docs/apache-airflow/stable/installation/index.html to install Airflow.
-If you just want to evaluate the SAS providers, then the simplest path would be to intall via PYPI and run Airflow on the local machine in a virtual environment. 
+If you just want to evaluate the SAS providers, then the simplest path would be to install via PYPI and run Airflow on the local machine in a virtual environment. 
+
 ### Install the SAS provider
-The SAS provider will be made available as a package on PYPI. In the meantime if you want to build the package from these sources, run `python -m build` from the root of the repository which will create a wheel file in the dist subdirectory.
-To upload to a repository such as pypi, define the repository in ~/.pypirc then:
-`python -m twine upload --repository repos_name dist/*`
+If you want to build the package from these sources, install the build module using `pip install build` and then run `python -m build` from the root of the repository which will create a wheel file in the dist subdirectory. 
+
 #### Installing in a local virtual environment
-If you are running Airflow locally, switch to the Python environment where Airflow is installed, and run pip install dist/sas_airflow_provider_xxxxx.whl
+The SAS provider is available as a package published in PyPI. To install it, switch to the Python environment where Airflow is installed, and run the following command:
+
+`pip install sas-airflow-provider`
+
+If you would like to install the provider from a package you built locally, run:
+
+`pip install dist/sas_airflow_provider_xxxxx.whl`
+
 #### Installing in a container
 There are a few ways to provide the package:
 - Environment variable: ```_PIP_ADDITIONAL_REQUIREMENTS``` Set this variable to the command line that will be passed to ```pip install```
 - Create a dockerfile that adds the pip install command to the base image and edit the docker-compose file to use "build" (there is a comment in the docker compose file where you can change it)
 
 ### Create a connection to SAS
 In order to connect to SAS Viya from the Airflow operator, you will need to create a connection. The easiest way to do this is to go into the Airflow UI under Admin/Connections and create a new connection using the blue + button. Select SAS from the list of connection types, and enter sas_default as the name. The applicable fields are host (http or https url to your SAS Viya install), login and password. It is also possible to specify an OAuth token by creating a json body in the extra field. For example `{"token": "oauth_token_here"}`. If a token is found it is used instead of the user/password.
 
 ### Running a DAG with a SAS provider
-See example files in the src/example_dags directory. These dags can be modified and 
+See example files in the src/sas_airflow_provider/example_dags directory. These dags can be modified and 
 placed in your Airflow dags directory. 
 
 Mac note: If you are running Airflow standalone on a Mac, there is a known issue regarding how process forking works.
-This causes issues with the urllib which is used by the operator. To get around it set NO_PROXY=URL in your environment
+This causes issues with the urllib which is used by the operator. To get around it set NO_PROXY=* in your environment
 prior to running Airflow in standalone mode.
+Eg:
+`export NO_PROXY="*"`
 
 ### Prerequisites for running demo DAGs
-You will need to create a SAS Studio Flow or a Job Definition before you can reference it from a DAG. The easiest way is to use SAS Studio UI to do this.
+You will need to create a SAS Studio Flow or a Job Definition before you can reference it from a DAG. The easiest way is to use the SAS Studio UI to do this.
 
 
 ## Contributing
 We welcome your contributions! Please read [CONTRIBUTING.md](CONTRIBUTING.md) for
 details on how to submit contributions to this project.
 
 ## License
```

### Comparing `sas-airflow-provider-0.0.1/README.md` & `sas-airflow-provider-0.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,56 @@
-# SAS Airflow Provider
+# SAS&reg; Airflow Provider
 
-## Current major capabilities of SAS Studio Flow Operator
+## Current major capabilities of the SAS&reg; Studio Flow Operator
 
-* Execute Studio Flow stored either on File System or in SAS Content
-* Select Compute Context to be used for execution of Studio Flow
-* Specify whether SAS logs of Studio Flow execution should be returned and displayed in Airflow or not
+* Execute a SAS Studio Flow stored either on the File System or in SAS Content
+* Select the Compute Context to be used for execution of a SAS Studio Flow
+* Specify whether SAS logs of a SAS Studio Flow execution should be returned and displayed in Airflow
 * Specify parameters (init_code, wrap_code) to be used for code generation
-* Honor return code of SAS Studio Flow in Airflow. In particular, if SAS Studio Flow fails, Airflow raises exception as well and stop execution
-* Authentication via oauth token or via user/password (i.e. generation of oauth token prior to each call)
+* Honor return code of a SAS Studio Flow in Airflow. In particular, if a SAS Studio Flow fails, Airflow raises an exception as well and stops execution
+* Authenticate via oauth token or via user/password (i.e. generation of oauth token prior to each call)
 
 
 ## Getting started
 ### Install Airflow
 Follow instructions at https://airflow.apache.org/docs/apache-airflow/stable/installation/index.html to install Airflow.
-If you just want to evaluate the SAS providers, then the simplest path would be to intall via PYPI and run Airflow on the local machine in a virtual environment. 
+If you just want to evaluate the SAS providers, then the simplest path would be to install via PYPI and run Airflow on the local machine in a virtual environment. 
+
 ### Install the SAS provider
-The SAS provider will be made available as a package on PYPI. In the meantime if you want to build the package from these sources, run `python -m build` from the root of the repository which will create a wheel file in the dist subdirectory.
-To upload to a repository such as pypi, define the repository in ~/.pypirc then:
-`python -m twine upload --repository repos_name dist/*`
+If you want to build the package from these sources, install the build module using `pip install build` and then run `python -m build` from the root of the repository which will create a wheel file in the dist subdirectory. 
+
 #### Installing in a local virtual environment
-If you are running Airflow locally, switch to the Python environment where Airflow is installed, and run pip install dist/sas_airflow_provider_xxxxx.whl
+The SAS provider is available as a package published in PyPI. To install it, switch to the Python environment where Airflow is installed, and run the following command:
+
+`pip install sas-airflow-provider`
+
+If you would like to install the provider from a package you built locally, run:
+
+`pip install dist/sas_airflow_provider_xxxxx.whl`
+
 #### Installing in a container
 There are a few ways to provide the package:
 - Environment variable: ```_PIP_ADDITIONAL_REQUIREMENTS``` Set this variable to the command line that will be passed to ```pip install```
 - Create a dockerfile that adds the pip install command to the base image and edit the docker-compose file to use "build" (there is a comment in the docker compose file where you can change it)
 
 ### Create a connection to SAS
 In order to connect to SAS Viya from the Airflow operator, you will need to create a connection. The easiest way to do this is to go into the Airflow UI under Admin/Connections and create a new connection using the blue + button. Select SAS from the list of connection types, and enter sas_default as the name. The applicable fields are host (http or https url to your SAS Viya install), login and password. It is also possible to specify an OAuth token by creating a json body in the extra field. For example `{"token": "oauth_token_here"}`. If a token is found it is used instead of the user/password.
 
 ### Running a DAG with a SAS provider
-See example files in the src/example_dags directory. These dags can be modified and 
+See example files in the src/sas_airflow_provider/example_dags directory. These dags can be modified and 
 placed in your Airflow dags directory. 
 
 Mac note: If you are running Airflow standalone on a Mac, there is a known issue regarding how process forking works.
-This causes issues with the urllib which is used by the operator. To get around it set NO_PROXY=URL in your environment
+This causes issues with the urllib which is used by the operator. To get around it set NO_PROXY=* in your environment
 prior to running Airflow in standalone mode.
+Eg:
+`export NO_PROXY="*"`
 
 ### Prerequisites for running demo DAGs
-You will need to create a SAS Studio Flow or a Job Definition before you can reference it from a DAG. The easiest way is to use SAS Studio UI to do this.
+You will need to create a SAS Studio Flow or a Job Definition before you can reference it from a DAG. The easiest way is to use the SAS Studio UI to do this.
 
 
 ## Contributing
 We welcome your contributions! Please read [CONTRIBUTING.md](CONTRIBUTING.md) for
 details on how to submit contributions to this project.
 
 ## License
```

### Comparing `sas-airflow-provider-0.0.1/setup.cfg` & `sas-airflow-provider-0.0.3/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sas-airflow-provider
-version = 0.0.1
+version = 0.0.3
 author = SAS
 author_email = andrew.shakinovsky@sas.com
 description = Enables execution of Studio Flows and Jobs from Airflow
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/sassoftware/sas-airflow-provider
 project_urls =
```

### Comparing `sas-airflow-provider-0.0.1/src/sas_airflow_provider/example_dags/__init__.py` & `sas-airflow-provider-0.0.3/src/sas_airflow_provider/example_dags/__init__.py`

 * *Files identical despite different names*

### Comparing `sas-airflow-provider-0.0.1/src/sas_airflow_provider/example_dags/example_sas_jobexecution.py` & `sas-airflow-provider-0.0.3/src/sas_airflow_provider/example_dags/example_sas_jobexecution.py`

 * *Files identical despite different names*

### Comparing `sas-airflow-provider-0.0.1/src/sas_airflow_provider/example_dags/example_sas_studioflow.py` & `sas-airflow-provider-0.0.3/src/sas_airflow_provider/example_dags/example_sas_studioflow.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,9 +31,10 @@
 task1 = SASStudioFlowOperator(task_id='demo_studio_flow_1.flw',
                               flow_path_type='content',
                               flow_path='/Public/Airflow/demo_studio_flow_1.flw',
                               flow_exec_log=True,
                               compute_context="SAS Studio compute context",
                               flow_codegen_init_code=False,
                               flow_codegen_wrap_code=False,
+                              connection_name='sas_default',
                               env_vars=environment_vars,
                               dag=dag)
```

### Comparing `sas-airflow-provider-0.0.1/src/sas_airflow_provider/hooks/__init__.py` & `sas-airflow-provider-0.0.3/src/sas_airflow_provider/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `sas-airflow-provider-0.0.1/src/sas_airflow_provider/hooks/sas.py` & `sas-airflow-provider-0.0.3/src/sas_airflow_provider/hooks/sas.py`

 * *Files identical despite different names*

### Comparing `sas-airflow-provider-0.0.1/src/sas_airflow_provider/operators/__init__.py` & `sas-airflow-provider-0.0.3/src/sas_airflow_provider/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `sas-airflow-provider-0.0.1/src/sas_airflow_provider/operators/sas_jobexecution.py` & `sas-airflow-provider-0.0.3/src/sas_airflow_provider/operators/sas_jobexecution.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,16 @@
 
     :param connection_name: Name of the SAS Viya connection stored as an Airflow HTTP connection
     :param job_name: Name of the SAS Job to be run
     :param parameters Dictionary of all the parameters that should be passed to the
         SAS Job as SAS Macro variables
     """
 
+    template_fields: Sequence[str] = ("parameters",)
+
     def __init__(self, job_name: str, parameters: dict, connection_name: str = None,  **kwargs) -> None:
         super().__init__(**kwargs)
         self.connection_name = connection_name
         self.job_name = job_name
         self.parameters = parameters
 
     def execute(self, context):
@@ -67,11 +69,11 @@
             "_output_type": "html",
             "_debug": "log",
         }
 
         headers = {"Accept": "application/vnd.sas.job.execution.job+json"}
         response = session.post(url, headers=headers, data=payload, verify=False)
 
-        if response.status_code != 200:
+        if(response.status_code < 200 or response.status_code >= 300):
             raise AirflowFailException(f"SAS Job Execution HTTP status code {response.status_code}")
 
         return 1
```

### Comparing `sas-airflow-provider-0.0.1/src/sas_airflow_provider/operators/sas_studioflow.py` & `sas-airflow-provider-0.0.3/src/sas_airflow_provider/operators/sas_studioflow.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 import copy
 import json
 import time
 
 import requests
 
 from airflow.exceptions import AirflowFailException
+from airflow.exceptions import AirflowException
 from airflow.models import BaseOperator
 from sas_airflow_provider.hooks.sas import SasHook
 
 class SASStudioFlowOperator(BaseOperator):
     """
     Executes a SAS Studio flow
 
@@ -48,14 +49,16 @@
         suitable default is used.
     :param env_vars: (optional) Dictionary of environment variables to set before running the flow.
     """
 
     ui_color = "#CCE5FF"
     ui_fgcolor = "black"
 
+    template_fields: Sequence[str] = ("env_vars",)
+
     def __init__(
         self,
         flow_path_type: str,
         flow_path: str,
         flow_exec_log: bool,
         flow_codegen_init_code=False,
         flow_codegen_wrap_code=False,
@@ -74,61 +77,74 @@
         self.flow_codegen_initCode = flow_codegen_init_code
         self.flow_codegen_wrapCode = flow_codegen_wrap_code
         self.connection_name = connection_name
         self.compute_context = compute_context
         self.env_vars = env_vars
 
     def execute(self, context):
+        try:
+            self.log.info("Authenticate connection")
+            h = SasHook(self.connection_name)
+            session = h.get_conn()
+
+            self.log.info("Generate code for Studio Flow: %s", str(self.flow_path))
+            code = _generate_flow_code(
+                session,
+                self.flow_path_type,
+                self.flow_path,
+                self.flow_codegen_initCode,
+                self.flow_codegen_wrapCode,
+                None,
+                self.compute_context,
+            )
 
-        self.log.info("Authenticate connection")
-        h = SasHook(self.connection_name)
-        session = h.get_conn()
-
-        self.log.info("Generate code for Studio Flow: %s", str(self.flow_path))
-        code = _generate_flow_code(
-            session,
-            self.flow_path_type,
-            self.flow_path,
-            self.flow_codegen_initCode,
-            self.flow_codegen_wrapCode,
-            None,
-            self.compute_context,
-        )
-
-        if self.env_vars:
-            # Add environment variables to pre-code
-            self.log.info(f"Adding {len(self.env_vars)} environment variables to code")
-            pre_env_code = "/** Setting up environment variables **/\n"
-            for env_var in self.env_vars:
-                env_val = self.env_vars[env_var]
-                pre_env_code = pre_env_code + f"options set={env_var}='{env_val}';\n"
-            pre_env_code = pre_env_code + "/** Finished setting up environment variables **/\n\n"
-            code["code"] = pre_env_code + code["code"]
-
-        # Create the job request for JES
-        jr = {
-            "name": f"Airflow_{self.task_id}",
-            "jobDefinition": {"type": "Compute", "code": code["code"]},
-            "arguments": {"_contextName": self.compute_context},
-        }
-
-        # Kick off the JES job
-        job = _run_job_and_wait(session, jr, 1)
-        job_state = job["state"]
+            if self.env_vars:
+                # Add environment variables to pre-code
+                self.log.info(f"Adding {len(self.env_vars)} environment variables to code")
+                pre_env_code = "/** Setting up environment variables **/\n"
+                for env_var in self.env_vars:
+                    env_val = self.env_vars[env_var]
+                    pre_env_code = pre_env_code + f"options set={env_var}='{env_val}';\n"
+                pre_env_code = pre_env_code + "/** Finished setting up environment variables **/\n\n"
+                code["code"] = pre_env_code + code["code"]
+
+            # Create the job request for JES
+            jr = {
+                "name": f"Airflow_{self.task_id}",
+                "jobDefinition": {"type": "Compute", "code": code["code"]},
+                "arguments": {"_contextName": self.compute_context},
+            }
+
+            # Kick off the JES job
+            job = _run_job_and_wait(session, jr, 1)
+            job_state = job["state"]
+
+        # support retry if API-calls fails for whatever reason
+        except Exception as e:
+            raise AirflowException(f"SASStudioFlowOperator error: {str(e)}")
 
         # display logs if needed
         if self.flow_exec_log is True:
-            _dump_logs(session, job)
-
-        # raise exception in Airflow if SAS Studio Flow ended execution with "failed" state
+            # Safeguard if we are unable to retreive the log. We will NOT throw any exceptions
+            try:
+                _dump_logs(session, job)
+            except Exception as e:
+                self.log.info("Unable to retrieve log. Maybe the log is too large.")
+
+        # raise exception in Airflow if SAS Studio Flow ended execution with "failed" "canceled" or "timed out" state
+        # support retry for 'failed' (typically there is an ERROR in the log) and 'timed out'
+        # do NOT support retry for 'canceled' (typically the SAS Job called ABORT ABEND)
         if job_state == "failed":
-            raise AirflowFailException(
-                "SAS Studio Flow Execution completed with an error. See log for details "
-                "(set flow_exec_log to True in the operator to turn on logging)"
-            )
+            raise AirflowException("SAS Studio Flow Execution completed with an error.")
+
+        if job_state == "canceled":
+            raise AirflowFailException("SAS Studio Flow Execution was cancelled or aborted. See log for details ")
+
+        if job_state == "timed out":
+            raise AirflowException("SAS Studio Flow Execution has timed out. See log for details ")
 
         return 1
 
 
 def _generate_flow_code(
     session,
     artifact_type: str,
```

### Comparing `sas-airflow-provider-0.0.1/src/sas_airflow_provider.egg-info/PKG-INFO` & `sas-airflow-provider-0.0.3/src/sas_airflow_provider.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,62 +1,71 @@
 Metadata-Version: 2.1
 Name: sas-airflow-provider
-Version: 0.0.1
+Version: 0.0.3
 Summary: Enables execution of Studio Flows and Jobs from Airflow
 Home-page: https://github.com/sassoftware/sas-airflow-provider
 Author: SAS
 Author-email: andrew.shakinovsky@sas.com
 Project-URL: Bug Tracker, https://github.com/sassoftware
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# SAS Airflow Provider
+# SAS&reg; Airflow Provider
 
-## Current major capabilities of SAS Studio Flow Operator
+## Current major capabilities of the SAS&reg; Studio Flow Operator
 
-* Execute Studio Flow stored either on File System or in SAS Content
-* Select Compute Context to be used for execution of Studio Flow
-* Specify whether SAS logs of Studio Flow execution should be returned and displayed in Airflow or not
+* Execute a SAS Studio Flow stored either on the File System or in SAS Content
+* Select the Compute Context to be used for execution of a SAS Studio Flow
+* Specify whether SAS logs of a SAS Studio Flow execution should be returned and displayed in Airflow
 * Specify parameters (init_code, wrap_code) to be used for code generation
-* Honor return code of SAS Studio Flow in Airflow. In particular, if SAS Studio Flow fails, Airflow raises exception as well and stop execution
-* Authentication via oauth token or via user/password (i.e. generation of oauth token prior to each call)
+* Honor return code of a SAS Studio Flow in Airflow. In particular, if a SAS Studio Flow fails, Airflow raises an exception as well and stops execution
+* Authenticate via oauth token or via user/password (i.e. generation of oauth token prior to each call)
 
 
 ## Getting started
 ### Install Airflow
 Follow instructions at https://airflow.apache.org/docs/apache-airflow/stable/installation/index.html to install Airflow.
-If you just want to evaluate the SAS providers, then the simplest path would be to intall via PYPI and run Airflow on the local machine in a virtual environment. 
+If you just want to evaluate the SAS providers, then the simplest path would be to install via PYPI and run Airflow on the local machine in a virtual environment. 
+
 ### Install the SAS provider
-The SAS provider will be made available as a package on PYPI. In the meantime if you want to build the package from these sources, run `python -m build` from the root of the repository which will create a wheel file in the dist subdirectory.
-To upload to a repository such as pypi, define the repository in ~/.pypirc then:
-`python -m twine upload --repository repos_name dist/*`
+If you want to build the package from these sources, install the build module using `pip install build` and then run `python -m build` from the root of the repository which will create a wheel file in the dist subdirectory. 
+
 #### Installing in a local virtual environment
-If you are running Airflow locally, switch to the Python environment where Airflow is installed, and run pip install dist/sas_airflow_provider_xxxxx.whl
+The SAS provider is available as a package published in PyPI. To install it, switch to the Python environment where Airflow is installed, and run the following command:
+
+`pip install sas-airflow-provider`
+
+If you would like to install the provider from a package you built locally, run:
+
+`pip install dist/sas_airflow_provider_xxxxx.whl`
+
 #### Installing in a container
 There are a few ways to provide the package:
 - Environment variable: ```_PIP_ADDITIONAL_REQUIREMENTS``` Set this variable to the command line that will be passed to ```pip install```
 - Create a dockerfile that adds the pip install command to the base image and edit the docker-compose file to use "build" (there is a comment in the docker compose file where you can change it)
 
 ### Create a connection to SAS
 In order to connect to SAS Viya from the Airflow operator, you will need to create a connection. The easiest way to do this is to go into the Airflow UI under Admin/Connections and create a new connection using the blue + button. Select SAS from the list of connection types, and enter sas_default as the name. The applicable fields are host (http or https url to your SAS Viya install), login and password. It is also possible to specify an OAuth token by creating a json body in the extra field. For example `{"token": "oauth_token_here"}`. If a token is found it is used instead of the user/password.
 
 ### Running a DAG with a SAS provider
-See example files in the src/example_dags directory. These dags can be modified and 
+See example files in the src/sas_airflow_provider/example_dags directory. These dags can be modified and 
 placed in your Airflow dags directory. 
 
 Mac note: If you are running Airflow standalone on a Mac, there is a known issue regarding how process forking works.
-This causes issues with the urllib which is used by the operator. To get around it set NO_PROXY=URL in your environment
+This causes issues with the urllib which is used by the operator. To get around it set NO_PROXY=* in your environment
 prior to running Airflow in standalone mode.
+Eg:
+`export NO_PROXY="*"`
 
 ### Prerequisites for running demo DAGs
-You will need to create a SAS Studio Flow or a Job Definition before you can reference it from a DAG. The easiest way is to use SAS Studio UI to do this.
+You will need to create a SAS Studio Flow or a Job Definition before you can reference it from a DAG. The easiest way is to use the SAS Studio UI to do this.
 
 
 ## Contributing
 We welcome your contributions! Please read [CONTRIBUTING.md](CONTRIBUTING.md) for
 details on how to submit contributions to this project.
 
 ## License
```

### Comparing `sas-airflow-provider-0.0.1/src/sas_airflow_provider.egg-info/SOURCES.txt` & `sas-airflow-provider-0.0.3/src/sas_airflow_provider.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -7,12 +7,13 @@
 src/sas_airflow_provider.egg-info/SOURCES.txt
 src/sas_airflow_provider.egg-info/dependency_links.txt
 src/sas_airflow_provider.egg-info/entry_points.txt
 src/sas_airflow_provider.egg-info/top_level.txt
 src/sas_airflow_provider/example_dags/__init__.py
 src/sas_airflow_provider/example_dags/example_sas_jobexecution.py
 src/sas_airflow_provider/example_dags/example_sas_studioflow.py
+src/sas_airflow_provider/example_dags/example_templating.py
 src/sas_airflow_provider/hooks/__init__.py
 src/sas_airflow_provider/hooks/sas.py
 src/sas_airflow_provider/operators/__init__.py
 src/sas_airflow_provider/operators/sas_jobexecution.py
 src/sas_airflow_provider/operators/sas_studioflow.py
```

