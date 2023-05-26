# Comparing `tmp/ssind-0.1.3.tar.gz` & `tmp/ssind-0.1.3b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssind-0.1.3.tar", last modified: Fri May 26 02:44:08 2023, max compression
+gzip compressed data, was "ssind-0.1.3b1.tar", last modified: Fri May 26 08:37:03 2023, max compression
```

## Comparing `ssind-0.1.3.tar` & `ssind-0.1.3b1.tar`

### file list

```diff
@@ -1,36 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:44:08.984204 ssind-0.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:44:08.980204 ssind-0.1.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-26 02:43:52.000000 ssind-0.1.3/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:44:08.980204 ssind-0.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-26 02:43:52.000000 ssind-0.1.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-05-26 02:43:52.000000 ssind-0.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 02:43:52.000000 ssind-0.1.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    34590 2023-05-26 02:43:52.000000 ssind-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-26 02:44:08.984204 ssind-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-26 02:43:52.000000 ssind-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-05-26 02:43:52.000000 ssind-0.1.3/ceritaind.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:44:08.980204 ssind-0.1.3/config/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-26 02:43:52.000000 ssind-0.1.3/config/aceh.json
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-26 02:43:52.000000 ssind-0.1.3/config/websites.json
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-26 02:43:52.000000 ssind-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 02:44:08.984204 ssind-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-05-26 02:43:52.000000 ssind-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:44:08.984204 ssind-0.1.3/ssind/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 02:43:52.000000 ssind-0.1.3/ssind/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-26 02:43:52.000000 ssind-0.1.3/ssind/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-26 02:43:52.000000 ssind-0.1.3/ssind/lighthouse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:44:08.984204 ssind-0.1.3/ssind/mockups/
--rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-05-26 02:43:52.000000 ssind-0.1.3/ssind/mockups/devices.json
--rw-r--r--   0 runner    (1001) docker     (123)    25443 2023-05-26 02:43:52.000000 ssind-0.1.3/ssind/mockups/mockup.png
--rw-r--r--   0 runner    (1001) docker     (123)    13633 2023-05-26 02:43:52.000000 ssind-0.1.3/ssind/ssind.py
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-05-26 02:43:52.000000 ssind-0.1.3/ssind/ssind_0.bak
--rw-r--r--   0 runner    (1001) docker     (123)     8919 2023-05-26 02:43:52.000000 ssind-0.1.3/ssind/ssind_2.bak
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:44:08.984204 ssind-0.1.3/ssind/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-26 02:43:52.000000 ssind-0.1.3/ssind/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:44:08.984204 ssind-0.1.3/ssind.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-26 02:44:08.000000 ssind-0.1.3/ssind.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-26 02:44:08.000000 ssind-0.1.3/ssind.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 02:44:08.000000 ssind-0.1.3/ssind.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 02:44:08.000000 ssind-0.1.3/ssind.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-26 02:44:08.000000 ssind-0.1.3/ssind.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-26 02:44:08.000000 ssind-0.1.3/ssind.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:03.646017 ssind-0.1.3b1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:03.642017 ssind-0.1.3b1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-26 08:36:50.000000 ssind-0.1.3b1/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:03.642017 ssind-0.1.3b1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-26 08:36:50.000000 ssind-0.1.3b1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-05-26 08:36:50.000000 ssind-0.1.3b1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 08:36:50.000000 ssind-0.1.3b1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34590 2023-05-26 08:36:50.000000 ssind-0.1.3b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-26 08:37:03.646017 ssind-0.1.3b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-26 08:36:50.000000 ssind-0.1.3b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-05-26 08:36:50.000000 ssind-0.1.3b1/ceritaind.md
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-26 08:36:50.000000 ssind-0.1.3b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 08:37:03.646017 ssind-0.1.3b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-05-26 08:36:50.000000 ssind-0.1.3b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:03.642017 ssind-0.1.3b1/ssind/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:36:50.000000 ssind-0.1.3b1/ssind/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-26 08:36:50.000000 ssind-0.1.3b1/ssind/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:03.646017 ssind-0.1.3b1/ssind/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-26 08:36:50.000000 ssind-0.1.3b1/ssind/config/aceh.json
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-26 08:36:50.000000 ssind-0.1.3b1/ssind/config/websites.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-26 08:36:50.000000 ssind-0.1.3b1/ssind/lighthouse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:03.646017 ssind-0.1.3b1/ssind/mockups/
+-rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-05-26 08:36:50.000000 ssind-0.1.3b1/ssind/mockups/devices.json
+-rw-r--r--   0 runner    (1001) docker     (123)    25443 2023-05-26 08:36:50.000000 ssind-0.1.3b1/ssind/mockups/mockup.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13637 2023-05-26 08:36:50.000000 ssind-0.1.3b1/ssind/ssind.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:03.646017 ssind-0.1.3b1/ssind/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-26 08:36:50.000000 ssind-0.1.3b1/ssind/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:03.642017 ssind-0.1.3b1/ssind.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-26 08:37:03.000000 ssind-0.1.3b1/ssind.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-26 08:37:03.000000 ssind-0.1.3b1/ssind.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 08:37:03.000000 ssind-0.1.3b1/ssind.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 08:37:03.000000 ssind-0.1.3b1/ssind.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-26 08:37:03.000000 ssind-0.1.3b1/ssind.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-26 08:37:03.000000 ssind-0.1.3b1/ssind.egg-info/top_level.txt
```

### Comparing `ssind-0.1.3/.github/FUNDING.yml` & `ssind-0.1.3b1/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `ssind-0.1.3/.github/workflows/python-publish.yml` & `ssind-0.1.3b1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ssind-0.1.3/.gitignore` & `ssind-0.1.3b1/.gitignore`

 * *Files identical despite different names*

### Comparing `ssind-0.1.3/LICENSE` & `ssind-0.1.3b1/LICENSE`

 * *Files identical despite different names*

### Comparing `ssind-0.1.3/PKG-INFO` & `ssind-0.1.3b1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssind
-Version: 0.1.3
+Version: 0.1.3b1
 Summary: Take Unlimited ScreenShot Automation and make a report
 Home-page: https://github.com/irfnrdh/ssind/issues
 Author: Irfannur Diah
 Author-email: irfnrdh@gmail.com
 License: AGPLv3
 Project-URL: Documentation, https://github.com/irfnrdh/ssind/wiki
 Project-URL: Source Code, https://github.com/irfnrdh/ssind
@@ -14,16 +14,14 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Upload Python Package](https://github.com/irfnrdh/ssind/actions/workflows/python-publish.yml/badge.svg)](https://github.com/irfnrdh/ssind/actions/workflows/python-publish.yml)
-
 ![image](https://github.com/irfnrdh/ssind/assets/7637012/f34a13ed-805f-47de-9671-8e2f63a66fcd)
 
 
 ```
 $ ssind_
 
     ssind adalah sebuah alat untuk menangkap layar
```

### Comparing `ssind-0.1.3/ceritaind.md` & `ssind-0.1.3b1/ceritaind.md`

 * *Files identical despite different names*

### Comparing `ssind-0.1.3/config/websites.json` & `ssind-0.1.3b1/ssind/config/websites.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333334%*

 * *Differences: {'0': "{'screenshot': "*

 * *      "'export/screenshots/google/20230526152539/screenshot_mockup_18_desktop_1600×900_1600x900_2023-05-26 "*

 * *      "15:25:41.png'}",*

 * * '1': "{'screenshot': "*

 * *      "'export/screenshots/retasin/20230526152612/screenshot_mockup_18_desktop_1600×900_1600x900_2023-05-26 "*

 * *      "15:26:14.png'}",*

 * * '2': "{'screenshot': "*

 * *      "'export/screenshots/kodekeras/20230526152656/screenshot_mockup_18_desktop_1600×900_1600x900_2023-05-26 "*

 * *      "15:26:58.png'}"}*

```diff
@@ -1,17 +1,17 @@
 [
     {
         "name": "google",
-        "screenshot": "../export/screenshots/google/20230525232204/screenshot_mockup_18_desktop_1600\u00d7900_1600x900_2023-05-25 23:22:05.png",
+        "screenshot": "export/screenshots/google/20230526152539/screenshot_mockup_18_desktop_1600\u00d7900_1600x900_2023-05-26 15:25:41.png",
         "url": "https://www.google.com"
     },
     {
         "name": "retasin",
-        "screenshot": "../export/screenshots/retasin/20230525232236/screenshot_mockup_18_desktop_1600\u00d7900_1600x900_2023-05-25 23:22:38.png",
+        "screenshot": "export/screenshots/retasin/20230526152612/screenshot_mockup_18_desktop_1600\u00d7900_1600x900_2023-05-26 15:26:14.png",
         "url": "https://www.retasin.com"
     },
     {
         "name": "kodekeras",
-        "screenshot": "../export/screenshots/kodekeras/20230525232319/screenshot_mockup_18_desktop_1600\u00d7900_1600x900_2023-05-25 23:23:20.png",
+        "screenshot": "export/screenshots/kodekeras/20230526152656/screenshot_mockup_18_desktop_1600\u00d7900_1600x900_2023-05-26 15:26:58.png",
         "url": "https://kodekeras.my.id"
     }
 ]
```

### Comparing `ssind-0.1.3/setup.py` & `ssind-0.1.3b1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of README file
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='ssind',
-    version='0.1.3',
+    version='0.1.4',
     description='Take Unlimited ScreenShot Automation and make a report',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/irfnrdh/ssind/issues',
     author='Irfannur Diah',
     author_email='irfnrdh@gmail.com',
     license='AGPLv3',
```

### Comparing `ssind-0.1.3/ssind/app.py` & `ssind-0.1.3b1/ssind/app.py`

 * *Files identical despite different names*

### Comparing `ssind-0.1.3/ssind/lighthouse.py` & `ssind-0.1.3b1/ssind/lighthouse.py`

 * *Files identical despite different names*

### Comparing `ssind-0.1.3/ssind/mockups/devices.json` & `ssind-0.1.3b1/ssind/mockups/devices.json`

 * *Files identical despite different names*

### Comparing `ssind-0.1.3/ssind/mockups/mockup.png` & `ssind-0.1.3b1/ssind/mockups/mockup.png`

 * *Files identical despite different names*

### Comparing `ssind-0.1.3/ssind/ssind.py` & `ssind-0.1.3b1/ssind/ssind.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,17 +25,18 @@
 ███████║███████║██║██║ ╚████║██████╔╝
 ╚══════╝╚══════╝╚═╝╚═╝  ╚═══╝╚═════╝ 
 
 Ambil Unlimited ScreenShoot Sambil Ngopi 
 v.0.1.1 - by irfnrdh                      
 """
 
-base_directory = '../export/screenshots'
-resized_directory = '../export/resized_screenshots'
-report_directory = "../export/report"
+base_directory = 'export/screenshots'
+resized_directory = 'export/resized_screenshots'
+report_directory = 'export/report'
+config_folder = 'config'
 
 @click.command()
 @click.option('--clear', is_flag=True, help='Clear screenshots folder')
 @click.option('--report', is_flag=True, help='Generate PDF Report')
 @click.option('--config', default='websites.json', help='Specify the path to the JSON config list of website file')
 def capture_screenshots(clear, config, report):
 
@@ -47,26 +48,26 @@
 
     # Create base directory to store the screenshots
     os.makedirs(base_directory, exist_ok=True)
     os.makedirs(resized_directory, exist_ok=True)
 
 
     # Create a log file
-    log_file = open('../export/website_status.log', 'w')
+    log_file = open('export/website_status.log', 'w')
 
     # Set up Chrome options
     chrome_options = Options()
     chrome_options.add_argument("--headless")  # Run Chrome in headless mode
 
     # Set up the path to your ChromeDriver executable
     chrome_driver_path = '/usr/bin/chromedriver'
 
     # Get the absolute path to the 'config' folder
-    config_folder = os.path.abspath(os.path.join(os.path.dirname(__file__), '..', 'config'))
-    websites = load_websites_from_json(os.path.join(config_folder, config))
+    # config_folder = os.path.abspath(os.path.join(os.path.dirname(__file__), '..', 'config'))
+    websites = load_websites_from_json(os.path.join('config', config))
 
     if config == "websites.json":
         click.echo(f'Config menggunakan data : "{config}" \n')
 
     # Iterate through the websites
     for website in tqdm(websites, desc="Capturing Screenshots"):
         name = website['name']
@@ -156,15 +157,15 @@
                 # Resize the captured screenshots
                 for screenshot_path in screenshot_paths:
                 
                     # Resize the image to the effective resolution
                     resized_screenshot = screenshot.resize((int(effective_width), int(effective_height)))
 
                     # Save the resized image
-                    resized_screenshot.save(f"../export/resized_screenshots/{index}_{platform}_{name}_resized.png")
+                    resized_screenshot.save(f"export/resized_screenshots/{index}_{platform}_{name}_resized.png")
 
                 
 
                 # screenshot = screenshot_paths[-1] if screenshot_paths else ""  # Update the 'screenshot' field with the last screenshot path or empty string
 
             # Update the 'screenshot' field in the 'websites' list with the screenshot paths
             website['screenshot'] = screenshot_paths[-1] if screenshot_paths else ""
@@ -240,15 +241,15 @@
             os.remove(os.path.join(root, file))
         for dir in dirs:
             os.rmdir(os.path.join(root, dir))
     print("Report folder cleared.")
 
 def clear_log_file():
     # Clear the content of the log file
-    # open('../export/website_status.log', 'w').close()
+    # open('export/website_status.log', 'w').close()
     print("Log file deative to clear.")
 
 def generate_pdf_report(base_directory):
 
     pdfkit_options = {
         'page-size': 'A4',
         'margin-top': '0mm',
```

### Comparing `ssind-0.1.3/ssind.egg-info/PKG-INFO` & `ssind-0.1.3b1/ssind.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssind
-Version: 0.1.3
+Version: 0.1.3b1
 Summary: Take Unlimited ScreenShot Automation and make a report
 Home-page: https://github.com/irfnrdh/ssind/issues
 Author: Irfannur Diah
 Author-email: irfnrdh@gmail.com
 License: AGPLv3
 Project-URL: Documentation, https://github.com/irfnrdh/ssind/wiki
 Project-URL: Source Code, https://github.com/irfnrdh/ssind
@@ -14,16 +14,14 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Upload Python Package](https://github.com/irfnrdh/ssind/actions/workflows/python-publish.yml/badge.svg)](https://github.com/irfnrdh/ssind/actions/workflows/python-publish.yml)
-
 ![image](https://github.com/irfnrdh/ssind/assets/7637012/f34a13ed-805f-47de-9671-8e2f63a66fcd)
 
 
 ```
 $ ssind_
 
     ssind adalah sebuah alat untuk menangkap layar
```

