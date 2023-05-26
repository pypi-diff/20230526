# Comparing `tmp/std_daq_client-1.1.1.tar.gz` & `tmp/std_daq_client-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "std_daq_client-1.1.1.tar", last modified: Fri May 26 10:11:29 2023, max compression
+gzip compressed data, was "std_daq_client-1.2.0.tar", last modified: Fri May 26 17:29:09 2023, max compression
```

## Comparing `std_daq_client-1.1.1.tar` & `std_daq_client-1.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 babic_a    (501) staff       (20)        0 2023-05-26 10:11:29.137218 std_daq_client-1.1.1/
--rw-r--r--   0 babic_a    (501) staff       (20)      693 2023-05-26 10:11:29.136505 std_daq_client-1.1.1/PKG-INFO
--rw-r--r--   0 babic_a    (501) staff       (20)    11059 2023-05-12 12:51:12.000000 std_daq_client-1.1.1/README.md
--rw-r--r--   0 babic_a    (501) staff       (20)       38 2023-05-26 10:11:29.137367 std_daq_client-1.1.1/setup.cfg
--rw-r--r--   0 babic_a    (501) staff       (20)     1317 2023-05-16 08:33:36.000000 std_daq_client-1.1.1/setup.py
--rw-r--r--   0 babic_a    (501) staff       (20)     1131 2023-05-26 10:11:20.000000 std_daq_client-1.1.1/setup_client.py
-drwxr-xr-x   0 babic_a    (501) staff       (20)        0 2023-05-26 10:11:29.131187 std_daq_client-1.1.1/std_daq_client/
--rw-r--r--   0 babic_a    (501) staff       (20)       68 2023-05-24 09:15:21.000000 std_daq_client-1.1.1/std_daq_client/__init__.py
-drwxr-xr-x   0 babic_a    (501) staff       (20)        0 2023-05-26 10:11:29.135958 std_daq_client-1.1.1/std_daq_client/cli/
--rw-r--r--   0 babic_a    (501) staff       (20)        0 2023-05-24 09:17:15.000000 std_daq_client-1.1.1/std_daq_client/cli/__init__.py
--rw-r--r--   0 babic_a    (501) staff       (20)      448 2023-05-24 09:55:36.000000 std_daq_client-1.1.1/std_daq_client/cli/get_config.py
--rw-r--r--   0 babic_a    (501) staff       (20)      470 2023-05-24 09:55:47.000000 std_daq_client-1.1.1/std_daq_client/cli/get_deploy_status.py
--rw-r--r--   0 babic_a    (501) staff       (20)      550 2023-05-24 09:55:59.000000 std_daq_client-1.1.1/std_daq_client/cli/get_logs.py
--rw-r--r--   0 babic_a    (501) staff       (20)      446 2023-05-24 09:56:12.000000 std_daq_client-1.1.1/std_daq_client/cli/get_stats.py
--rw-r--r--   0 babic_a    (501) staff       (20)      448 2023-05-24 09:56:17.000000 std_daq_client-1.1.1/std_daq_client/cli/get_status.py
--rw-r--r--   0 babic_a    (501) staff       (20)     1149 2023-05-26 10:03:12.000000 std_daq_client-1.1.1/std_daq_client/cli/write.py
--rw-r--r--   0 babic_a    (501) staff       (20)    12087 2023-05-26 09:52:04.000000 std_daq_client-1.1.1/std_daq_client/client.py
-drwxr-xr-x   0 babic_a    (501) staff       (20)        0 2023-05-26 10:11:29.133592 std_daq_client-1.1.1/std_daq_client.egg-info/
--rw-r--r--   0 babic_a    (501) staff       (20)      693 2023-05-26 10:11:29.000000 std_daq_client-1.1.1/std_daq_client.egg-info/PKG-INFO
--rw-r--r--   0 babic_a    (501) staff       (20)      544 2023-05-26 10:11:29.000000 std_daq_client-1.1.1/std_daq_client.egg-info/SOURCES.txt
--rw-r--r--   0 babic_a    (501) staff       (20)        1 2023-05-26 10:11:29.000000 std_daq_client-1.1.1/std_daq_client.egg-info/dependency_links.txt
--rw-r--r--   0 babic_a    (501) staff       (20)      422 2023-05-26 10:11:29.000000 std_daq_client-1.1.1/std_daq_client.egg-info/entry_points.txt
--rw-r--r--   0 babic_a    (501) staff       (20)        9 2023-05-26 10:11:29.000000 std_daq_client-1.1.1/std_daq_client.egg-info/requires.txt
--rw-r--r--   0 babic_a    (501) staff       (20)       15 2023-05-26 10:11:29.000000 std_daq_client-1.1.1/std_daq_client.egg-info/top_level.txt
+drwxr-xr-x   0 babic_a   (1000) babic_a   (1000)        0 2023-05-26 17:29:09.504797 std_daq_client-1.2.0/
+-rw-r--r--   0 babic_a   (1000) babic_a   (1000)     9495 2023-05-26 17:29:09.504797 std_daq_client-1.2.0/PKG-INFO
+-rw-r--r--   0 babic_a   (1000) babic_a   (1000)    11059 2023-05-16 16:53:29.000000 std_daq_client-1.2.0/README.md
+-rw-r--r--   0 babic_a   (1000) babic_a   (1000)       38 2023-05-26 17:29:09.504797 std_daq_client-1.2.0/setup.cfg
+-rw-r--r--   0 babic_a   (1000) babic_a   (1000)     1317 2023-05-16 16:53:29.000000 std_daq_client-1.2.0/setup.py
+-rw-r--r--   0 babic_a   (1000) babic_a   (1000)     1194 2023-05-26 17:19:20.000000 std_daq_client-1.2.0/setup_client.py
+drwxr-xr-x   0 babic_a   (1000) babic_a   (1000)        0 2023-05-26 17:29:09.501797 std_daq_client-1.2.0/std_daq_client/
+-rw-r--r--   0 babic_a   (1000) babic_a   (1000)       68 2023-05-24 00:18:58.000000 std_daq_client-1.2.0/std_daq_client/__init__.py
+drwxr-xr-x   0 babic_a   (1000) babic_a   (1000)        0 2023-05-26 17:29:09.503797 std_daq_client-1.2.0/std_daq_client/cli/
+-rw-r--r--   0 babic_a   (1000) babic_a   (1000)        0 2023-05-25 18:06:27.000000 std_daq_client-1.2.0/std_daq_client/cli/__init__.py
+-rw-r--r--   0 babic_a   (1000) babic_a   (1000)      448 2023-05-25 18:06:27.000000 std_daq_client-1.2.0/std_daq_client/cli/get_config.py
+-rw-r--r--   0 babic_a   (1000) babic_a   (1000)      470 2023-05-25 18:06:27.000000 std_daq_client-1.2.0/std_daq_client/cli/get_deploy_status.py
+-rw-r--r--   0 babic_a   (1000) babic_a   (1000)      550 2023-05-25 18:06:27.000000 std_daq_client-1.2.0/std_daq_client/cli/get_logs.py
+-rw-r--r--   0 babic_a   (1000) babic_a   (1000)      446 2023-05-25 18:06:27.000000 std_daq_client-1.2.0/std_daq_client/cli/get_stats.py
+-rw-r--r--   0 babic_a   (1000) babic_a   (1000)      448 2023-05-25 18:06:27.000000 std_daq_client-1.2.0/std_daq_client/cli/get_status.py
+-rw-r--r--   0 babic_a   (1000) babic_a   (1000)     1518 2023-05-26 17:19:45.000000 std_daq_client-1.2.0/std_daq_client/cli/write.py
+-rw-r--r--   0 babic_a   (1000) babic_a   (1000)    12094 2023-05-26 16:40:32.000000 std_daq_client-1.2.0/std_daq_client/client.py
+drwxr-xr-x   0 babic_a   (1000) babic_a   (1000)        0 2023-05-26 17:29:09.502797 std_daq_client-1.2.0/std_daq_client.egg-info/
+-rw-r--r--   0 babic_a   (1000) babic_a   (1000)     9495 2023-05-26 17:29:09.000000 std_daq_client-1.2.0/std_daq_client.egg-info/PKG-INFO
+-rw-r--r--   0 babic_a   (1000) babic_a   (1000)      544 2023-05-26 17:29:09.000000 std_daq_client-1.2.0/std_daq_client.egg-info/SOURCES.txt
+-rw-r--r--   0 babic_a   (1000) babic_a   (1000)        1 2023-05-26 17:29:09.000000 std_daq_client-1.2.0/std_daq_client.egg-info/dependency_links.txt
+-rw-r--r--   0 babic_a   (1000) babic_a   (1000)      479 2023-05-26 17:29:09.000000 std_daq_client-1.2.0/std_daq_client.egg-info/entry_points.txt
+-rw-r--r--   0 babic_a   (1000) babic_a   (1000)        9 2023-05-26 17:29:09.000000 std_daq_client-1.2.0/std_daq_client.egg-info/requires.txt
+-rw-r--r--   0 babic_a   (1000) babic_a   (1000)       15 2023-05-26 17:29:09.000000 std_daq_client-1.2.0/std_daq_client.egg-info/top_level.txt
```

### Comparing `std_daq_client-1.1.1/README.md` & `std_daq_client-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `std_daq_client-1.1.1/setup.py` & `std_daq_client-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `std_daq_client-1.1.1/setup_client.py` & `std_daq_client-1.2.0/setup_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 from setuptools import setup
 
-CLIENT_VERSION = "1.1.1"
+CLIENT_VERSION = "1.2.0"
 
 with open(os.path.join(os.path.dirname(__file__), 'std_daq_client/', 'README.md')) as readme:
     long_description = readme.read()
 
 setup(
     version=CLIENT_VERSION,
     name='std_daq_client',
@@ -20,14 +20,15 @@
         std_cli_get_config=std_daq_client.cli.get_config:main
         std_cli_get_deploy_status=std_daq_client.cli.get_deploy_status:main
         std_cli_get_logs=std_daq_client.cli.get_logs:main
         std_cli_get_stats=std_daq_client.cli.get_stats:main
         std_cli_get_status=std_daq_client.cli.get_status:main
         std_cli_write_async=std_daq_client.cli.write:write_sync
         std_cli_write_sync=std_daq_client.cli.write:write_async
+        std_cli_write_stop=std_daq_client.cli.write:write_stop
     ''',
 
     author="Paul Scherrer Institute",
     url='https://github.com/paulscherrerinstitute/std_daq_service',
     description='Python client for standard-daq',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

### Comparing `std_daq_client-1.1.1/std_daq_client/cli/get_logs.py` & `std_daq_client-1.2.0/std_daq_client/cli/get_logs.py`

 * *Files identical despite different names*

### Comparing `std_daq_client-1.1.1/std_daq_client/cli/write.py` & `std_daq_client-1.2.0/std_daq_client/cli/write.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,10 +30,21 @@
     url_base, write_request = _process_arguments()
     client = StdDaqClient(url_base)
     response = client.start_writer_async(write_request)
 
     print(json.dumps(response, indent=2))
 
 
+def write_stop():
+    parser = argparse.ArgumentParser(description='Get std_daq stats')
+    parser.add_argument("--url_base", type=str, default='http://localhost:5000', help="Base URL of the REST Endpoint")
+    url_base = parser.parse_args().url_base
+
+    client = StdDaqClient(url_base)
+    response = client.stop_writer()
+
+    print(json.dumps(response, indent=2))
+
+
 if __name__ == "__main__":
     # The default is sync, for no real reason.
     write_sync()
```

### Comparing `std_daq_client-1.1.1/std_daq_client/client.py` & `std_daq_client-1.2.0/std_daq_client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,17 +57,17 @@
         Return dictionary format:
         {
           "bit_depth": 16,                   # Bit depth of the image. Supported values are dependent on the detector.
           "detector_name": "EG9M",           # Name of the detector. Must be unique, used as internal DAQ identifier.
           "detector_type": "eiger",          # Type of detector. Currently supported: eiger, jungfrau, gigafrost, bsread
           "image_pixel_height": 3264,        # Assembled image height in pixels.
           "image_pixel_width": 3106,         # Assembled image width in pixels.
-          "n_modules: 2,                     # Number of modules to assemble.
+          "n_modules": 2,                    # Number of modules to assemble.
           "start_udp_port": 50000,           # Start UDP port where the detector is streaming modules.
-          "writer_user_id": 12345,           # User_id under which the writer will create and write the file.
+          "writer_user_id": 12345,           # User_id under which the writer will create and write files.
           "module_positions": {              # Dictionary with mapping between module number -> image position.
             "0": [0, 3263, 513, 3008 ],      #     Format: [start_x, start_y, end_x, end_y]
             "1": [516, 3263, 1029, 3008 ],
         }
 
         :return: Dictionary with current configuration.
         """
@@ -142,15 +142,15 @@
         Also used to reset the driver in case the writer crushed and restarted in the background.
 
         When the writer process dies due to an error, it gets restarted after a couple of seconds. The driver might
         recover from this event, but it might also not be able to. This is the case when the status of the writer
         is 'UNKNOWN'. When this happens call the 'stop_writer' function to re-establish the connection between the
         driver and the writer.
         """
-        return self._post_url(WRITER_STOP_ENDPOINT, {})
+        return self._post_url(WRITER_STOP_ENDPOINT, {})['writer']
 
     def get_status(self):
         """
         Return the current DAQ status.
 
         Return dictionary format:
         {
```

### Comparing `std_daq_client-1.1.1/std_daq_client.egg-info/SOURCES.txt` & `std_daq_client-1.2.0/std_daq_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

