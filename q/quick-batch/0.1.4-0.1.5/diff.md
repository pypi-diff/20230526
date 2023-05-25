# Comparing `tmp/quick_batch-0.1.4.tar.gz` & `tmp/quick_batch-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quick_batch-0.1.4.tar", max compression
+gzip compressed data, was "quick_batch-0.1.5.tar", max compression
```

## Comparing `quick_batch-0.1.4.tar` & `quick_batch-0.1.5.tar`

### file list

```diff
@@ -1,31 +1,29 @@
--rw-r--r--   0        0        0     3112 2023-05-25 04:16:03.689066 quick_batch-0.1.4/README.md
--rw-r--r--   0        0        0      658 2023-05-25 04:16:03.689066 quick_batch-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-25 04:16:03.689066 quick_batch-0.1.4/quick_batch/README.md
--rw-r--r--   0        0        0      120 2023-05-25 04:16:03.689066 quick_batch-0.1.4/quick_batch/__init__.py
--rw-r--r--   0        0        0      906 2023-05-25 04:16:03.689066 quick_batch-0.1.4/quick_batch/main.py
--rw-r--r--   0        0        0      368 2023-05-25 04:16:03.689066 quick_batch-0.1.4/quick_batch/processor_app/Dockerfile
--rwxr-xr-x   0        0        0     1215 2023-05-25 04:16:03.689066 quick_batch-0.1.4/quick_batch/processor_app/processor_app/__init__.py
--rwxr-xr-x   0        0        0     1594 2023-05-25 04:16:03.689066 quick_batch-0.1.4/quick_batch/processor_app/processor_app/activate_process.py
--rwxr-xr-x   0        0        0     2234 2023-05-25 04:16:03.689066 quick_batch-0.1.4/quick_batch/processor_app/processor_app/api_connects.py
--rwxr-xr-x   0        0        0      409 2023-05-25 04:16:03.689066 quick_batch-0.1.4/quick_batch/processor_app/processor_app/run.py
--rwxr-xr-x   0        0        0       21 2023-05-25 04:16:03.689066 quick_batch-0.1.4/quick_batch/processor_app/requirements.txt
--rwxr-xr-x   0        0        0     5224 2023-05-25 04:16:03.689066 quick_batch-0.1.4/quick_batch/processor_app/wait-for-it.sh
--rw-r--r--   0        0        0      241 2023-05-25 04:16:03.689066 quick_batch-0.1.4/quick_batch/queue_app/Dockerfile
--rw-r--r--   0        0        0     1220 2023-05-25 04:16:03.689066 quick_batch-0.1.4/quick_batch/queue_app/queue_app/__init__.py
--rw-r--r--   0        0        0     2312 2023-05-25 04:16:03.693066 quick_batch-0.1.4/quick_batch/queue_app/queue_app/apis.py
--rw-r--r--   0        0        0     3250 2023-05-25 04:16:03.693066 quick_batch-0.1.4/quick_batch/queue_app/queue_app/queues_init.py
--rw-r--r--   0        0        0      424 2023-05-25 04:16:03.693066 quick_batch-0.1.4/quick_batch/queue_app/queue_app/run.py
--rwxr-xr-x   0        0        0       21 2023-05-25 04:16:03.693066 quick_batch-0.1.4/quick_batch/queue_app/requirements.txt
--rwxr-xr-x   0        0        0     5224 2023-05-25 04:16:03.693066 quick_batch-0.1.4/quick_batch/queue_app/wait-for-it.sh
--rw-r--r--   0        0        0      551 2023-05-25 04:16:03.693066 quick_batch-0.1.4/quick_batch/utilities/__init__.py
--rw-r--r--   0        0        0     2088 2023-05-25 04:16:03.693066 quick_batch-0.1.4/quick_batch/utilities/manage_containers.py
--rw-r--r--   0        0        0     3959 2023-05-25 04:16:03.693066 quick_batch-0.1.4/quick_batch/utilities/manage_images.py
--rw-r--r--   0        0        0     1788 2023-05-25 04:16:03.693066 quick_batch-0.1.4/quick_batch/utilities/manage_loggers.py
--rw-r--r--   0        0        0      551 2023-05-25 04:16:03.693066 quick_batch-0.1.4/quick_batch/utilities/manage_networks.py
--rw-r--r--   0        0        0     2487 2023-05-25 04:16:03.693066 quick_batch-0.1.4/quick_batch/utilities/manage_queue.py
--rw-r--r--   0        0        0     1394 2023-05-25 04:16:03.693066 quick_batch-0.1.4/quick_batch/utilities/manage_requirements.py
--rw-r--r--   0        0        0     4687 2023-05-25 04:16:03.693066 quick_batch-0.1.4/quick_batch/utilities/manage_services.py
--rw-r--r--   0        0        0     2395 2023-05-25 04:16:03.693066 quick_batch-0.1.4/quick_batch/utilities/manage_setup.py
--rw-r--r--   0        0        0      229 2023-05-25 04:16:03.693066 quick_batch-0.1.4/quick_batch/utilities/manage_swarm.py
--rw-r--r--   0        0        0     3720 2023-05-25 04:16:03.693066 quick_batch-0.1.4/quick_batch/utilities/param_checks.py
--rw-r--r--   0        0        0     3786 1970-01-01 00:00:00.000000 quick_batch-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     3843 2023-05-25 23:05:55.292224 quick_batch-0.1.5/README.md
+-rw-r--r--   0        0        0      686 2023-05-25 23:05:55.292224 quick_batch-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      120 2023-05-25 23:05:55.292224 quick_batch-0.1.5/quick_batch/__init__.py
+-rw-r--r--   0        0        0      906 2023-05-25 23:05:55.292224 quick_batch-0.1.5/quick_batch/main.py
+-rwxr-xr-x   0        0        0     1215 2023-05-25 23:05:55.296224 quick_batch-0.1.5/quick_batch/processor_app/processor_app/__init__.py
+-rwxr-xr-x   0        0        0     1747 2023-05-25 23:05:55.296224 quick_batch-0.1.5/quick_batch/processor_app/processor_app/activate_process.py
+-rwxr-xr-x   0        0        0     2234 2023-05-25 23:05:55.296224 quick_batch-0.1.5/quick_batch/processor_app/processor_app/api_connects.py
+-rwxr-xr-x   0        0        0      409 2023-05-25 23:05:55.296224 quick_batch-0.1.5/quick_batch/processor_app/processor_app/run.py
+-rwxr-xr-x   0        0        0     5224 2023-05-25 23:05:55.296224 quick_batch-0.1.5/quick_batch/processor_app/wait-for-it.sh
+-rw-r--r--   0        0        0      241 2023-05-25 23:05:55.296224 quick_batch-0.1.5/quick_batch/queue_app/Dockerfile
+-rw-r--r--   0        0        0     1220 2023-05-25 23:05:55.296224 quick_batch-0.1.5/quick_batch/queue_app/queue_app/__init__.py
+-rw-r--r--   0        0        0     2312 2023-05-25 23:05:55.296224 quick_batch-0.1.5/quick_batch/queue_app/queue_app/apis.py
+-rw-r--r--   0        0        0     3250 2023-05-25 23:05:55.296224 quick_batch-0.1.5/quick_batch/queue_app/queue_app/queues_init.py
+-rw-r--r--   0        0        0      424 2023-05-25 23:05:55.296224 quick_batch-0.1.5/quick_batch/queue_app/queue_app/run.py
+-rwxr-xr-x   0        0        0       21 2023-05-25 23:05:55.296224 quick_batch-0.1.5/quick_batch/queue_app/requirements.txt
+-rwxr-xr-x   0        0        0     5224 2023-05-25 23:05:55.296224 quick_batch-0.1.5/quick_batch/queue_app/wait-for-it.sh
+-rw-r--r--   0        0        0      551 2023-05-25 23:05:55.296224 quick_batch-0.1.5/quick_batch/utilities/__init__.py
+-rw-r--r--   0        0        0     2088 2023-05-25 23:05:55.296224 quick_batch-0.1.5/quick_batch/utilities/manage_containers.py
+-rw-r--r--   0        0        0     1244 2023-05-25 23:05:55.296224 quick_batch-0.1.5/quick_batch/utilities/manage_dockerfile.py
+-rw-r--r--   0        0        0     4624 2023-05-25 23:05:55.296224 quick_batch-0.1.5/quick_batch/utilities/manage_images.py
+-rw-r--r--   0        0        0     1951 2023-05-25 23:05:55.296224 quick_batch-0.1.5/quick_batch/utilities/manage_loggers.py
+-rw-r--r--   0        0        0      551 2023-05-25 23:05:55.296224 quick_batch-0.1.5/quick_batch/utilities/manage_networks.py
+-rw-r--r--   0        0        0     2487 2023-05-25 23:05:55.296224 quick_batch-0.1.5/quick_batch/utilities/manage_queue.py
+-rw-r--r--   0        0        0     2033 2023-05-25 23:05:55.296224 quick_batch-0.1.5/quick_batch/utilities/manage_requirements.py
+-rw-r--r--   0        0        0     4722 2023-05-25 23:05:55.296224 quick_batch-0.1.5/quick_batch/utilities/manage_services.py
+-rw-r--r--   0        0        0     3201 2023-05-25 23:05:55.296224 quick_batch-0.1.5/quick_batch/utilities/manage_setup.py
+-rw-r--r--   0        0        0      229 2023-05-25 23:05:55.296224 quick_batch-0.1.5/quick_batch/utilities/manage_swarm.py
+-rw-r--r--   0        0        0     4429 2023-05-25 23:05:55.296224 quick_batch-0.1.5/quick_batch/utilities/param_checks.py
+-rw-r--r--   0        0        0     4566 1970-01-01 00:00:00.000000 quick_batch-0.1.5/PKG-INFO
```

### Comparing `quick_batch-0.1.4/pyproject.toml` & `quick_batch-0.1.5/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "quick_batch"
-version = "0.1.4"
+version = "0.1.5"
 description = "ultra simple command line tool for docker-scaling batch processing"
 authors = ["Jeremy Watt <jermwatt@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/jermwatt/quick_batch"
 license = "MIT"
 
 [tool.poetry.scripts]
@@ -12,14 +12,15 @@
 
 
 [tool.poetry.dependencies]
 python = "^3.9"
 docker = "^6.1.2"
 fire = "^0.5.0"
 pyyaml = "<5.5"
+dockerfile-parse = "^2.0.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
 flake8 = "^4.0.1"
 mypy = "^0.910"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `quick_batch-0.1.4/quick_batch/main.py` & `quick_batch-0.1.5/quick_batch/main.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.4/quick_batch/processor_app/processor_app/__init__.py` & `quick_batch-0.1.5/quick_batch/processor_app/processor_app/__init__.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.4/quick_batch/processor_app/processor_app/activate_process.py` & `quick_batch-0.1.5/quick_batch/processor_app/processor_app/activate_process.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,17 +37,21 @@
 
         # update lifetime
         lifetime -= 1
 
         # print progress
         print('FINISHED: with', str(app.file_paths_to_process), flush=True)
 
-        if app.success:
-            # send report to queue_app
-            api_connects.send_done_report(app)
+        # send report to queue_app
+        api_connects.send_done_report(app)
 
-            # reset success flag
-            app.success = False
+        # WIP: send different report based on processor success
+        # if app.success:
+        #     # send report to queue_app
+        #     api_connects.send_done_report(app)
+
+        #     # reset success flag
+        #     app.success = False
 
     # if reaching the lifetime end signal to orchestator
     # that a new container be built
     sys.exit(1)
```

### Comparing `quick_batch-0.1.4/quick_batch/processor_app/processor_app/api_connects.py` & `quick_batch-0.1.5/quick_batch/processor_app/processor_app/api_connects.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.4/quick_batch/processor_app/wait-for-it.sh` & `quick_batch-0.1.5/quick_batch/processor_app/wait-for-it.sh`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.4/quick_batch/queue_app/queue_app/__init__.py` & `quick_batch-0.1.5/quick_batch/queue_app/queue_app/__init__.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.4/quick_batch/queue_app/queue_app/apis.py` & `quick_batch-0.1.5/quick_batch/queue_app/queue_app/apis.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
             object_paths.append(next_path)
 
             # update wip queue
             app.wip_queue.append(next_path)
 
             # update counters
             app.wip_queue_length += 1
+            app.feed_queue_length -= 1
 
         return jsonify({'object_paths': object_paths,
                         'queue_message': f"{app.feed_queue_length} objects "
                                          f"remaining in feeder queue"
                         })
     else:
         if app.empty_trigger == 0:
@@ -55,15 +56,14 @@
         data = request.get_data()
 
         # get datapoint from request
         data = json.loads(data)["paths_complete"]
 
         # update counters
         for d in data:
-            app.feed_queue_length -= 1
             app.done_queue_length += 1
             app.wip_queue_length -= 1
             app.done_queue.append(d)
 
         # update wip queue
         app.wip_queue = list(set(app.wip_queue) - set(data))
         app.wip_queue_length = len(app.wip_queue)
```

### Comparing `quick_batch-0.1.4/quick_batch/queue_app/queue_app/queues_init.py` & `quick_batch-0.1.5/quick_batch/queue_app/queue_app/queues_init.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.4/quick_batch/queue_app/wait-for-it.sh` & `quick_batch-0.1.5/quick_batch/queue_app/wait-for-it.sh`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.4/quick_batch/utilities/__init__.py` & `quick_batch-0.1.5/quick_batch/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.4/quick_batch/utilities/manage_containers.py` & `quick_batch-0.1.5/quick_batch/utilities/manage_containers.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.4/quick_batch/utilities/manage_images.py` & `quick_batch-0.1.5/quick_batch/utilities/manage_images.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,50 +1,96 @@
 import shutil
 import os
-import sys
 import docker
 from utilities import queue_path, processor_path
 from .manage_requirements import make_requirements
+from .manage_requirements import infer_requirements
+from .manage_dockerfile import check_requirements_copy_and_install
 from utilities import log_exceptions
 import subprocess
 
 
 # create client for docker
 @log_exceptions
 def create_client():
     return docker.from_env()
 
 
+@log_exceptions
+def pull_and_tag_image(client, image_name, new_tag):
+    try:
+        print('INFO: Pulling and tagging image...')
+
+        # Try tagging local image
+        try: 
+            image = client.images.get(image_name)
+            tag_success = image.tag(new_tag)
+            
+            if tag_success:
+                print('SUCCESS: Tagging local image successful!')
+                return True
+        except docker.errors.ImageNotFound:
+            pass
+
+        # Pull the image
+        pulled_image = client.images.pull(image_name)
+
+        # Tag the pulled image with a new name
+        tagged_image = pulled_image.tag(new_tag)
+        
+        print('SUCCESS: Pulling and tagging image complete!')
+        return True
+
+    except docker.errors.APIError as e:
+        print(f"FAILURE: Error occurred while pulling and tagging the image: {e}")
+        return False
+
+
 def check_requirements_file(requirements_path):
     if not os.path.isfile(requirements_path):
         return False  # The path is not a file
 
     if os.path.getsize(requirements_path) == 0:
         return False  # The file is empty
 
     return True  # The file exists and is not empty
 
 
 # build processor_app docker image
 @log_exceptions
-def build_processor_image(client, requirements_path, processor):
+def build_processor_image(client,
+                          dockerfile_path,
+                          requirements_path,
+                          processor):
+
+    # create container path for dockerfile
+    container_dockerfile_path = os.path.join(processor_path, 'Dockerfile')
+
+    # copy dockerfile to processor_path directory
+    shutil.copy(dockerfile_path, container_dockerfile_path)
+
+    # check if requirements.txt is being copied and installed in dockerfile
+    check_requirements_copy_and_install(container_dockerfile_path)
+
     # create container path for requirements
-    container_path = os.path.join(processor_path, 'processor_requirements.txt')
+    container_requirements_path = os.path.join(processor_path,
+                                               'requirements.txt')
 
     # check if requirements_path is valid and not empty,
     # if so copy to container path
     if check_requirements_file(requirements_path):
         print('INFO: valid requirements file')
-        shutil.copyfile(os.path.join(requirements_path), container_path)
+        make_requirements(requirements_path, container_requirements_path)
     else:
         # create requirements file from processor
-        print('INFO: no valid requirements file, creating from processor')
-        make_requirements(processor, container_path)
+        print('INFO: no valid requirements file, attempting to create '
+              'from processor')
+        infer_requirements(processor, container_requirements_path)
 
-    # create docker image for processor app - including user defined    
+    # create docker image for processor app - including user defined
     def stream_build_logs(path, tag):
         command = ["docker", "build", "-t", tag, path]
         process = subprocess.Popen(
             command,
             stdout=subprocess.PIPE,
             stderr=subprocess.STDOUT,
             universal_newlines=True
@@ -67,51 +113,22 @@
     print('INFO: building processor image...')
     print('===============================')
     print('===============================')
     stream_build_logs(processor_path, 'quick_batch_processor_app')
     print('===============================')
     print('===============================')
 
-    
-    # try:
-    #     # Set quiet=False to print the build output
-    #     build_output = client.images.build(path=processor_path, tag='quick_batch_processor_app',
-    #                     quiet=False)
-            
-    #     # Print the build output
-    #     for line in build_output[1]:
-    #         if 'stream' in line:
-    #             print(line['stream'], end='')
-    #             sys.stdout.flush() 
-
-    #     # Build completed successfully
-    #     print("Image build completed!")
-        
-    # except docker.errors.BuildError as e:
-    #     # Handle build errors
-    #     print("Build failed!")
-    #     print("Error message:", e.msg)
-        
-    # except docker.errors.APIError as e:
-    #     # Handle API errors
-    #     print("API error occurred during build!")
-    #     print("Error message:", e)
-
-    # except Exception as e:
-    #     # Handle other exceptions
-    #     print("An unexpected error occurred during build:", str(e))
-        
-        
-        
-        
     # Build completed
     print("INFO: ... processor image build completed!")
 
+    # remove dockerfile from the processor_path directory
+    os.remove(container_dockerfile_path)
+
     # remove processor_requirements.txt from the processor_path directory
-    os.remove(container_path)
+    os.remove(container_requirements_path)
 
 
 @log_exceptions
 def build_queue_image(client):
     # create docker image for queue app - including user defined requirements
     client.images.build(path=queue_path, tag='quick_batch_queue_app',
                         quiet=False)
```

### Comparing `quick_batch-0.1.4/quick_batch/utilities/manage_loggers.py` & `quick_batch-0.1.5/quick_batch/utilities/manage_loggers.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,15 +48,19 @@
 
     def open_log(self):
         self.log = open(self.log_file, "a")
 
     def write(self, message):
         self.terminal.write(message)
         self.terminal.flush()  # Flush the terminal output
-        self.log.write(message)
-        self.log.flush()  # Flush the log file output
+        if self.log is not None:
+            self.log.write(message)
+            self.log.flush()  # Flush the log file output
 
     def flush(self):
         pass
 
     def close_log(self):
-        self.log.close()
+        if self.log is not None:
+            self.log.close()
+            self.log = None  # Set log attribute to None to prevent further writing
+
```

### Comparing `quick_batch-0.1.4/quick_batch/utilities/manage_networks.py` & `quick_batch-0.1.5/quick_batch/utilities/manage_networks.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.4/quick_batch/utilities/manage_queue.py` & `quick_batch-0.1.5/quick_batch/utilities/manage_queue.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.4/quick_batch/utilities/manage_requirements.py` & `quick_batch-0.1.5/quick_batch/utilities/manage_requirements.py`

 * *Files 22% similar despite different names*

```diff
@@ -26,19 +26,37 @@
     # Get the required external modules
     installed_modules = sorted(imported_modules.difference(excluded_modules))
 
     return installed_modules
 
 
 def write_requirements(required_modules, file_path):
+    base_requirements = ['flask', 'requests', 'pyyaml']
     with open(file_path, 'w') as file:
-        for module in required_modules:
+        for module in base_requirements:
             file.write(module + '\n')
 
+        for module in set(required_modules) - set(base_requirements):
+            file.write(module + '\n')
+
+
+@log_exceptions
+def make_requirements(requirements_path, container_requirements_path):
+    # read contents of the requirements file
+    with open(requirements_path, 'r') as file:
+        contents = file.readlines()
+
+    # Clean up the contents by removing leading/trailing
+    # whitespace and newlines
+    modules_to_install = [line.strip() for line in contents]
+
+    # write requirements to file
+    write_requirements(modules_to_install, container_requirements_path)
+
 
 @log_exceptions
-def make_requirements(processor, container_path):
+def infer_requirements(processor, container_path):
     # get requirements for processor.py
     installed_modules = get_processor_requirements(processor)
 
     # write requirements to file
     write_requirements(installed_modules, container_path)
```

### Comparing `quick_batch-0.1.4/quick_batch/utilities/manage_services.py` & `quick_batch-0.1.5/quick_batch/utilities/manage_services.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,15 +143,18 @@
     ]
 
     # Define the service configuration
     service_config = {
         'image': 'quick_batch_processor_app',
         'name': 'processor_app',
         'log_driver': 'json-file',
-        'log_driver_options': {'max-size': '10m', 'max-file': '3'},
+        'log_driver_options': {
+            'max-size': '10m', 
+            'max-file': '3'
+        },
         'restart_policy': {'Condition': 'none', 'MaxAttempts': 0},
         'mounts': mounts,
         'user': 'root',
         'networks': ['quick_batch_network'],
         'command': ['python', '/processor_app/run.py'],
         # 'command': ['tail', '-f', '/dev/null'],
     }
```

### Comparing `quick_batch-0.1.4/quick_batch/utilities/manage_setup.py` & `quick_batch-0.1.5/quick_batch/utilities/manage_setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,65 @@
 import time
 from utilities import log_exceptions
 from utilities import manage_images
 from utilities.param_checks import setup_logger
 from utilities.param_checks import check_config
 from utilities.param_checks import check_config_data_paths
 from utilities.param_checks import check_processor
+from utilities.param_checks import check_dockerfile
 from utilities.manage_containers import remove_all_containers
 from utilities.manage_networks import remove_network
 from utilities.manage_services import remove_all_services
 from utilities.manage_swarm import leave_swarm
 from utilities.manage_swarm import create_swarm
 from utilities.manage_networks import create_network
 from utilities.manage_services import create_queue_service
 from utilities.manage_services import create_processor_service
 from utilities.manage_queue import monitor_queue_app_containers
+from utilities.manage_images import pull_and_tag_image
 
 
 @log_exceptions
 def setup_client(config):
     # setup logger
     logger = setup_logger(config)
 
     # check that input files exist
     check_config(config)
 
     # check config data paths
     input_path, output_path, processor, num_processors, \
-        requirements_path = check_config_data_paths(config)
+        dockerfile_path, requirements_path, image_name = check_config_data_paths(config)
 
     # check processor
     check_processor(processor)
+    
+    # check dockerfile - seems to save a copy local to the project - not using for now
+    # check_dockerfile(dockerfile_path)
 
     # create docker client
     client = manage_images.create_client()
 
-    # build images
-    manage_images.build_processor_image(client, requirements_path, processor)
+    # # try to pull and tag image
+    # pull_success = pull_and_tag_image(client, 'jermwatt/quick_batch_queue_app', 'quick_batch_queue_app')
+    
+    # # if not successful, build image
+    # if not pull_success:
+        
     manage_images.build_queue_image(client)
+    
+    # # try to pull and tag image
+    # pull_success = pull_and_tag_image(client, image_name, 'quick_batch_processor_app')
+    
+    # # if not successful, build image
+    # if not pull_success:
+    manage_images.build_processor_image(client,
+                                        dockerfile_path,
+                                        requirements_path,
+                                        processor)
 
     return client, input_path, output_path, processor, num_processors, logger
 
 
 @log_exceptions
 def reset_workspace(client):
     try:
```

### Comparing `quick_batch-0.1.4/quick_batch/utilities/param_checks.py` & `quick_batch-0.1.5/quick_batch/utilities/param_checks.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import sys
 import os
 import ast
 import yaml
+from dockerfile_parse import DockerfileParser
 from utilities import log_exceptions
 from utilities.manage_loggers import Logger
 
 
 def setup_logger(config):
     # import log path
     with open(config, "r") as yaml_file:
@@ -33,18 +34,21 @@
     # import config variables
     with open(config_path, "r") as yaml_file:
         config = yaml.safe_load(yaml_file)
 
     # check that data paths in config file entries are valid
     input_path = config["data"]["input_path"]
     output_path = config["data"]["output_path"]
+    dockerfile_path = config["processor"]["dockerfile_path"]
     processor_path = config["processor"]["processor_path"]
     num_processors = config["processor"]["num_processors"]
     requirements_path = config.get("processor", {}). \
         get("requirements_path", "")
+    image_name = config.get("processor", {}). \
+        get("image_name", "")
 
     # if requirements_path is not empty, check that it exists
     if not os.path.isfile(requirements_path):
         requirements_path = ""
 
     # check that processor_path is file and exists
     if not os.path.isfile(processor_path):
@@ -83,15 +87,15 @@
     elif num_processors <= 0:
         print("FAILURE: num_processors is not greater than 0")
         sys.exit(1)
     else:
         print("SUCCESS: num_processors is an integer greater than 0")
 
     return input_path, output_path, processor_path, num_processors, \
-        requirements_path
+        dockerfile_path, requirements_path, image_name
 
 
 @log_exceptions
 def check_config(config_path):
     # check if file exists
     if not os.path.isfile(config_path):
         print("FAILURE: config_path file does not exist")
@@ -119,7 +123,25 @@
             break
 
     if processor_found:
         print("SUCCESS: module contains a function named 'processor'")
     else:
         print("FAILURE: module does not contain a function named 'processor'")
         sys.exit(1)
+
+
+# check dockerfile validity
+@log_exceptions
+def check_dockerfile(dockerfile):
+    def validate_dockerfile(dockerfile_path):
+        try:
+            parser = DockerfileParser()
+            with open(dockerfile_path, 'r') as file:
+                parser.content = file.read()
+            return True
+        except Exception:
+            return False
+
+    if validate_dockerfile(dockerfile):
+        print("INFO: Dockerfile is valid!")
+    else:
+        print("INFO: Dockerfile is NOT valid.")
```

### Comparing `quick_batch-0.1.4/PKG-INFO` & `quick_batch-0.1.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,102 +1,121 @@
 Metadata-Version: 2.1
 Name: quick-batch
-Version: 0.1.4
+Version: 0.1.5
 Summary: ultra simple command line tool for docker-scaling batch processing
 Home-page: https://github.com/jermwatt/quick_batch
 License: MIT
 Author: Jeremy Watt
 Author-email: jermwatt@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: docker (>=6.1.2,<7.0.0)
+Requires-Dist: dockerfile-parse (>=2.0.0,<3.0.0)
 Requires-Dist: fire (>=0.5.0,<0.6.0)
 Requires-Dist: pyyaml (<5.5)
 Description-Content-Type: text/markdown
 
 [![Python application](https://github.com/jermwatt/quick_batch/actions/workflows/python-app.yml/badge.svg)](https://github.com/jermwatt/quick_batch/actions/workflows/python-app.yml)
 [![Upload Python Package](https://github.com/jermwatt/quick_batch/actions/workflows/python-publish.yml/badge.svg)](https://github.com/jermwatt/quick_batch/actions/workflows/python-publish.yml)
 
 # quick_batch
 
-quick_batch is an ultra-simple command-line tool for large batch processing and transformation. It allows you to scale any `processor` function that needs to be run over a large set of input data, enabling batch/parallel processing of the input with minimal setup and teardown.
+`quick_batch` is an ultra-simple command-line tool for large batch python-driven processing and transformation.  It was designed to be fast to deploy, transparent, and portable.  This allows you to scale any `processor` function that needs to be run over a large set of input data, enabling batch/parallel processing of the input with minimal setup and teardown.
+
 
 - [quick\_batch](#quick_batch)
-  - [Why use quick\_batch](#why-use-quick_batch)
-  - [Installation](#installation)
+- [Getting started](#getting-started)
   - [Usage](#usage)
-    - [`processor.py`](#processorpy)
-    - [`config.yaml`](#configyaml)
-    - [Running quick\_batch](#running-quick_batch)
+  - [Installation](#installation)
+  - [The `processor.py` file](#the-processorpy-file)
+- [Why use quick\_batch](#why-use-quick_batch)
 
+# Getting started
 
-## Why use quick_batch
+All you need to scale batch transformations with `quick_batch` is a
 
-quick_batch aims to be
+- transformation function(s) in a `processor.py` file
+- `Dockerfile` containing a container build appropriate to y our processor
+- an optional `requirements.txt` file containing required python modules
+  - custom `requirements.txt` require `flask`, `requests`, and `pyyaml`
 
-- **dead simple to use:** versus standard cloud service batch transformation services that require significant configuration / service understanding
+Document paths to these objects as well as other parameters in a `config.yaml` config file of the form below
 
-- **ultra fast setup:** versus setup of heavier orchestration tools like `airflow` or `mlflow`, which may be a hinderance due to time / familiarity / organisational constraints
 
-- **100% portable:** - use quick_batch on any machine, anywhere
+```yaml
+data:
+  input_path: /path/to/your/input/data
+  output_path: /path/to/your/output/data
+  log_path: /path/to/your/log/file
 
-- **processor-invariant:** quick_batch works with arbitrary processes, not just machine learning or deep learning tasks.
+queue:
+  feed_rate: <int - number of examples processed per processor instance>
+  order_files: <boolean - whether or not to order input files by size>
 
-- **transparent and open source:** quick_batch uses Docker under the hood and only abstracts away the not-so-fun stuff - including instantiation, scaling, and teardown.  you can still monitor your processing using familiar Docker command-line arguments (like `docker service ls`, `docker service logs`, etc.).
+processor:
+  image_name: <pre-built-image-name>
+  dockerfile_path: /path/to/your/Dockerfile
+  requirements_path: /path/to/your/requirements.txt
+  processor_path: /path/to/your/processor/processor.py
+  num_processors: <int - instances of processor to run in parallel>
+
+```
+
+`quick_batch` will point your `processor.py` at the `input_path` defined in this `config.yaml` and process the files listed in it in parallel at a scale given by your choice of `num_processors`.  
+
+Output will be written to the `output_path` specified in the configuration file.
+
+You can see `tests/config_files` for examples of valid configs.
+
+
+## Usage
+
+With your `config.yaml` defined you can use `quick_batch` at the terminal by typing
 
+```bash
+quick_batch /path/to/your/config.yaml
+```
 
 ## Installation
 
 To install quick_batch, simply use `pip`:
 
 ```bash
 pip install quick-batch
 ```
 
-## Usage
-
-To use quick_batch, you need to define a `processor.py` file and a `config.yaml` file containing the necessary paths and parameters.
-
-### `processor.py`
+## The `processor.py` file
 
-Create a `processor.py` file with the following pattern:
+Create a `processor.py` file with the following basic pattern:
 
 ```python
 import ...
 
 def processor(todos):
-    # Processor code
+  for file_name in todos.file_paths_to_process:
+    # processing code
 ```
 
-quick_batch will essentially point your `processor.py` at the `input_path` defined in your `config.yaml` and process this input in parallel at a scale given by your choice of `num_processors`.  Output will be written to the `output_path` specified in the configuration file.
+The `todos` object will carry in `feed_rate` number of file names to process in `.file_paths_to_process`.  
 
-### `config.yaml`
+Note: the function name `processor` is mandatory.
 
-Create a `config.yaml` file with the following structure:
 
-```yaml
-data:
-  input_path: /path/to/your/input/data
-  output_path: /path/to/your/output/data
-  log_path: /path/to/your/log/file
+# Why use quick_batch
 
-queue:
-  feed_rate: <int - number of examples processed per processor instance>
-  order_files: <boolean - whether or not to order input files by size>
+quick_batch aims to be
 
-processor:
-  processor_path: /path/to/your/processor/processor.py
-  num_processors: <int - instances of processor to run in parallel>
-```
+- **dead simple to use:** versus standard cloud service batch transformation services that require significant configuration / service understanding
+
+- **ultra fast setup:** versus setup of heavier orchestration tools like `airflow` or `mlflow`, which may be a hinderance due to time / familiarity / organisational constraints
 
-### Running quick_batch
+- **100% portable:** - use quick_batch on any machine, anywhere
 
-To run quick_batch, execute the following command in your terminal:
+- **processor-invariant:** quick_batch works with arbitrary processes, not just machine learning or deep learning tasks.
+
+- **transparent and open source:** quick_batch uses Docker under the hood and only abstracts away the not-so-fun stuff - including instantiation, scaling, and teardown.  you can still monitor your processing using familiar Docker command-line arguments (like `docker service ls`, `docker service logs`, etc.).
 
-```bash
-quick_batch /path/to/your/config.yaml
-```
```

