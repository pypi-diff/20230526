# Comparing `tmp/canvas-pilot-0.1.1.tar.gz` & `tmp/canvas-pilot-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "canvas-pilot-0.1.1.tar", last modified: Fri May  5 00:59:31 2023, max compression
+gzip compressed data, was "canvas-pilot-0.1.2.tar", last modified: Fri May 26 05:33:03 2023, max compression
```

## Comparing `canvas-pilot-0.1.1.tar` & `canvas-pilot-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ziang      (501) staff       (20)        0 2023-05-05 00:59:31.102842 canvas-pilot-0.1.1/
--rw-r--r--   0 ziang      (501) staff       (20)    35148 2023-05-05 00:58:23.000000 canvas-pilot-0.1.1/LICENSE
--rw-r--r--   0 ziang      (501) staff       (20)     2447 2023-05-05 00:59:31.102714 canvas-pilot-0.1.1/PKG-INFO
--rw-r--r--   0 ziang      (501) staff       (20)     1640 2023-05-05 00:56:46.000000 canvas-pilot-0.1.1/README.md
-drwxr-xr-x   0 ziang      (501) staff       (20)        0 2023-05-05 00:59:31.102181 canvas-pilot-0.1.1/canvas_pilot.egg-info/
--rw-r--r--   0 ziang      (501) staff       (20)     2447 2023-05-05 00:59:31.000000 canvas-pilot-0.1.1/canvas_pilot.egg-info/PKG-INFO
--rw-r--r--   0 ziang      (501) staff       (20)      292 2023-05-05 00:59:31.000000 canvas-pilot-0.1.1/canvas_pilot.egg-info/SOURCES.txt
--rw-r--r--   0 ziang      (501) staff       (20)        1 2023-05-05 00:59:31.000000 canvas-pilot-0.1.1/canvas_pilot.egg-info/dependency_links.txt
--rw-r--r--   0 ziang      (501) staff       (20)       52 2023-05-05 00:59:31.000000 canvas-pilot-0.1.1/canvas_pilot.egg-info/entry_points.txt
--rw-r--r--   0 ziang      (501) staff       (20)       25 2023-05-05 00:59:31.000000 canvas-pilot-0.1.1/canvas_pilot.egg-info/requires.txt
--rw-r--r--   0 ziang      (501) staff       (20)       13 2023-05-05 00:59:31.000000 canvas-pilot-0.1.1/canvas_pilot.egg-info/top_level.txt
-drwxr-xr-x   0 ziang      (501) staff       (20)        0 2023-05-05 00:59:31.102415 canvas-pilot-0.1.1/canvas_tools/
--rw-r--r--   0 ziang      (501) staff       (20)        0 2023-05-04 20:58:38.000000 canvas-pilot-0.1.1/canvas_tools/__init__.py
--rw-r--r--   0 ziang      (501) staff       (20)     5958 2023-05-05 00:40:42.000000 canvas-pilot-0.1.1/canvas_tools/canvas.py
--rw-r--r--   0 ziang      (501) staff       (20)       38 2023-05-05 00:59:31.102881 canvas-pilot-0.1.1/setup.cfg
--rw-r--r--   0 ziang      (501) staff       (20)     1326 2023-05-05 00:57:02.000000 canvas-pilot-0.1.1/setup.py
+drwxr-xr-x   0 ziang      (501) staff       (20)        0 2023-05-26 05:33:03.240525 canvas-pilot-0.1.2/
+-rw-r--r--   0 ziang      (501) staff       (20)    35148 2023-05-05 00:58:23.000000 canvas-pilot-0.1.2/LICENSE
+-rw-r--r--   0 ziang      (501) staff       (20)     3539 2023-05-26 05:33:03.240388 canvas-pilot-0.1.2/PKG-INFO
+-rw-r--r--   0 ziang      (501) staff       (20)     2732 2023-05-26 05:17:16.000000 canvas-pilot-0.1.2/README.md
+drwxr-xr-x   0 ziang      (501) staff       (20)        0 2023-05-26 05:33:03.240001 canvas-pilot-0.1.2/canvas_pilot.egg-info/
+-rw-r--r--   0 ziang      (501) staff       (20)     3539 2023-05-26 05:33:03.000000 canvas-pilot-0.1.2/canvas_pilot.egg-info/PKG-INFO
+-rw-r--r--   0 ziang      (501) staff       (20)      292 2023-05-26 05:33:03.000000 canvas-pilot-0.1.2/canvas_pilot.egg-info/SOURCES.txt
+-rw-r--r--   0 ziang      (501) staff       (20)        1 2023-05-26 05:33:03.000000 canvas-pilot-0.1.2/canvas_pilot.egg-info/dependency_links.txt
+-rw-r--r--   0 ziang      (501) staff       (20)       52 2023-05-26 05:33:03.000000 canvas-pilot-0.1.2/canvas_pilot.egg-info/entry_points.txt
+-rw-r--r--   0 ziang      (501) staff       (20)       34 2023-05-26 05:33:03.000000 canvas-pilot-0.1.2/canvas_pilot.egg-info/requires.txt
+-rw-r--r--   0 ziang      (501) staff       (20)       13 2023-05-26 05:33:03.000000 canvas-pilot-0.1.2/canvas_pilot.egg-info/top_level.txt
+drwxr-xr-x   0 ziang      (501) staff       (20)        0 2023-05-26 05:33:03.240221 canvas-pilot-0.1.2/canvas_tools/
+-rw-r--r--   0 ziang      (501) staff       (20)        0 2023-05-04 20:58:38.000000 canvas-pilot-0.1.2/canvas_tools/__init__.py
+-rw-r--r--   0 ziang      (501) staff       (20)     7787 2023-05-26 05:32:54.000000 canvas-pilot-0.1.2/canvas_tools/canvas.py
+-rw-r--r--   0 ziang      (501) staff       (20)       38 2023-05-26 05:33:03.240568 canvas-pilot-0.1.2/setup.cfg
+-rw-r--r--   0 ziang      (501) staff       (20)     1345 2023-05-26 05:33:00.000000 canvas-pilot-0.1.2/setup.py
```

### Comparing `canvas-pilot-0.1.1/LICENSE` & `canvas-pilot-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `canvas-pilot-0.1.1/PKG-INFO` & `canvas-pilot-0.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canvas-pilot
-Version: 0.1.1
+Version: 0.1.2
 Summary: A command-line tool for managing Canvas courses, fetching assignments, and grades.
 Home-page: https://github.com/realzza/canvas-cli
 Author: Ziang Zhou
 Author-email: ziang.zhou518@gmail.com
 License: GPLv3+
 Keywords: canvas api cli
 Classifier: Development Status :: 3 - Alpha
@@ -17,40 +17,70 @@
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Canvas Pilot
 
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/canvas-pilot)
+
 A command-line tool for managing your Canvas courses, fetching assignments, and grades.
 
 ## Installation
 
 To install the Canvas CLI, run the following command:
 
 ```bash
 pip install canvas-pilot
 ```
 
 ## Configuration
 
-Before using the Canvas CLI, you'll need to configure it with your Canvas API key and domain. To do this, run the following command and follow the prompts:
+Before using the Canvas CLI, you'll need to configure it with your Canvas API key and domain.
+
+### Retrieving your Canvas API Key
+
+To retrieve your Canvas API key, follow these steps:
+
+1. Log in to your Canvas account.
+2. Click on "Account" in the left-hand side menu.
+3. Click on "Settings" from the dropdown.
+4. Scroll down to the "Approved Integrations" section and click on "+ New Access Token".
+5. In the pop-up window, optionally enter a purpose for the token and set its expiry date.
+6. Click on "Generate Token".
+7. Copy the token displayed in the "Token" field. This is your Canvas API key.
+
+**Important:** Keep your API key safe and secure, like you would with a password. Don't share it with anyone.
+
+### Getting your Canvas Domain
+
+Your Canvas domain is the URL you use to access Canvas. For example, if you access Canvas by navigating to `https://canvas.<yourinstitution>.com`, then your Canvas domain is `canvas.<yourinstitution>.com`.
+
+Once you have your API key and domain, run the following command and follow the prompts to configure the Canvas CLI:
 
 ```bash
 canvas configure
 ```
 
 You can reconfigure the Canvas API key and domain at any time by running:
 
 ```bash
 canvas reconfigure
 ```
 
 ## Usage
 
+### Fetch Courses
+
+To fetch the list of your Canvas courses, run:
+
+```bash
+canvas fetch courses
+```
+
 ### Fetch Assignments
 
 To fetch assignments for all your Canvas courses, run:
 
 ```bash
 canvas fetch assignments
 ```
```

### Comparing `canvas-pilot-0.1.1/README.md` & `canvas-pilot-0.1.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,65 @@
 # Canvas Pilot
 
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/canvas-pilot)
+
 A command-line tool for managing your Canvas courses, fetching assignments, and grades.
 
 ## Installation
 
 To install the Canvas CLI, run the following command:
 
 ```bash
 pip install canvas-pilot
 ```
 
 ## Configuration
 
-Before using the Canvas CLI, you'll need to configure it with your Canvas API key and domain. To do this, run the following command and follow the prompts:
+Before using the Canvas CLI, you'll need to configure it with your Canvas API key and domain.
+
+### Retrieving your Canvas API Key
+
+To retrieve your Canvas API key, follow these steps:
+
+1. Log in to your Canvas account.
+2. Click on "Account" in the left-hand side menu.
+3. Click on "Settings" from the dropdown.
+4. Scroll down to the "Approved Integrations" section and click on "+ New Access Token".
+5. In the pop-up window, optionally enter a purpose for the token and set its expiry date.
+6. Click on "Generate Token".
+7. Copy the token displayed in the "Token" field. This is your Canvas API key.
+
+**Important:** Keep your API key safe and secure, like you would with a password. Don't share it with anyone.
+
+### Getting your Canvas Domain
+
+Your Canvas domain is the URL you use to access Canvas. For example, if you access Canvas by navigating to `https://canvas.<yourinstitution>.com`, then your Canvas domain is `canvas.<yourinstitution>.com`.
+
+Once you have your API key and domain, run the following command and follow the prompts to configure the Canvas CLI:
 
 ```bash
 canvas configure
 ```
 
 You can reconfigure the Canvas API key and domain at any time by running:
 
 ```bash
 canvas reconfigure
 ```
 
 ## Usage
 
+### Fetch Courses
+
+To fetch the list of your Canvas courses, run:
+
+```bash
+canvas fetch courses
+```
+
 ### Fetch Assignments
 
 To fetch assignments for all your Canvas courses, run:
 
 ```bash
 canvas fetch assignments
 ```
```

### Comparing `canvas-pilot-0.1.1/canvas_pilot.egg-info/PKG-INFO` & `canvas-pilot-0.1.2/canvas_pilot.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canvas-pilot
-Version: 0.1.1
+Version: 0.1.2
 Summary: A command-line tool for managing Canvas courses, fetching assignments, and grades.
 Home-page: https://github.com/realzza/canvas-cli
 Author: Ziang Zhou
 Author-email: ziang.zhou518@gmail.com
 License: GPLv3+
 Keywords: canvas api cli
 Classifier: Development Status :: 3 - Alpha
@@ -17,40 +17,70 @@
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Canvas Pilot
 
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/canvas-pilot)
+
 A command-line tool for managing your Canvas courses, fetching assignments, and grades.
 
 ## Installation
 
 To install the Canvas CLI, run the following command:
 
 ```bash
 pip install canvas-pilot
 ```
 
 ## Configuration
 
-Before using the Canvas CLI, you'll need to configure it with your Canvas API key and domain. To do this, run the following command and follow the prompts:
+Before using the Canvas CLI, you'll need to configure it with your Canvas API key and domain.
+
+### Retrieving your Canvas API Key
+
+To retrieve your Canvas API key, follow these steps:
+
+1. Log in to your Canvas account.
+2. Click on "Account" in the left-hand side menu.
+3. Click on "Settings" from the dropdown.
+4. Scroll down to the "Approved Integrations" section and click on "+ New Access Token".
+5. In the pop-up window, optionally enter a purpose for the token and set its expiry date.
+6. Click on "Generate Token".
+7. Copy the token displayed in the "Token" field. This is your Canvas API key.
+
+**Important:** Keep your API key safe and secure, like you would with a password. Don't share it with anyone.
+
+### Getting your Canvas Domain
+
+Your Canvas domain is the URL you use to access Canvas. For example, if you access Canvas by navigating to `https://canvas.<yourinstitution>.com`, then your Canvas domain is `canvas.<yourinstitution>.com`.
+
+Once you have your API key and domain, run the following command and follow the prompts to configure the Canvas CLI:
 
 ```bash
 canvas configure
 ```
 
 You can reconfigure the Canvas API key and domain at any time by running:
 
 ```bash
 canvas reconfigure
 ```
 
 ## Usage
 
+### Fetch Courses
+
+To fetch the list of your Canvas courses, run:
+
+```bash
+canvas fetch courses
+```
+
 ### Fetch Assignments
 
 To fetch assignments for all your Canvas courses, run:
 
 ```bash
 canvas fetch assignments
 ```
```

### Comparing `canvas-pilot-0.1.1/canvas_tools/canvas.py` & `canvas-pilot-0.1.2/canvas_tools/canvas.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+import getpass4
 import json
 import os
 from datetime import datetime
 
+import operator
+from collections import defaultdict
 import click
 import requests
 from icalendar import Calendar, Event
 
 CONFIG_FILE = "canvas_config.json"
 
 
@@ -42,34 +45,45 @@
             break
 
         all_results.extend(results)
         page += 1
 
     return all_results
 
+def parse_semester(start_date, end_date):
+    start_date = datetime.strptime(start_date, '%Y-%m-%dT%H:%M:%SZ')
+    end_date = datetime.strptime(end_date, '%Y-%m-%dT%H:%M:%SZ')
+    
+    if start_date.month <= 5 and end_date.month <= 5:
+        return f'Spring {start_date.year}'
+    elif start_date.month >= 8 and end_date.month >= 8:
+        return f'Fall {start_date.year}'
+    else:
+        return f'Summer {start_date.year}'
 
 @click.group()
 def main():
     pass
 
 
 @main.command("configure")
-@click.option("--api_key", prompt="Canvas API key")
-@click.option(
-    "--domain", prompt="Canvas domain (e.g., yourinstitution.instructure.com)"
-)
-def configure(api_key, domain):
-    config = {"api_key": api_key, "domain": domain}
-    save_config(config)
-    click.echo("Configuration saved.")
-
-
-@main.command("reconfigure")
-def reconfigure():
-    configure()
+def configure():
+    if os.path.exists(CONFIG_FILE):
+        if click.confirm('Configuration already exists. Do you want to overwrite it?'):
+            api_key = getpass4.getpass("Canvas API key: ")
+            domain = click.prompt("Canvas domain (e.g., canvas.<yourinstitution>.com)")
+            config = {"api_key": api_key, "domain": domain}
+            save_config(config)
+            click.echo("Configuration saved.")
+    else:
+        api_key = getpass4.getpass("Canvas API key: ")
+        domain = click.prompt("Canvas domain (e.g., canvas.<yourinstitution>.com)")
+        config = {"api_key": api_key, "domain": domain}
+        save_config(config)
+        click.echo("Configuration saved.")
 
 
 @main.group("fetch")
 def fetch():
     pass
 
 
@@ -121,14 +135,36 @@
                     cal.add_component(event)
 
     if export:
         with open("canvas_assignments.ics", "wb") as f:
             f.write(cal.to_ical())
         click.echo("Assignments exported to canvas_assignments.ics")
 
+@fetch.command("courses")
+def fetch_courses():
+    config = load_config()
+
+    headers = {"Authorization": f"Bearer {config['api_key']}"}
+
+    url_courses = f"{config['domain']}/api/v1/courses?enrollment_type=student&enrollment_state=active"
+    courses = fetch_all_pages(url_courses, headers)
+    
+    semester_courses = defaultdict(list)
+    for course in courses:
+        if "name" in course:
+            if "start_at" in course and "end_at" in course and course['start_at'] and course['end_at']:
+                semester = parse_semester(course['start_at'], course['end_at'])
+            else:
+                semester = "No Semester"
+            semester_courses[semester].append((course['id'], course['name']))
+    
+    for semester, courses in sorted(semester_courses.items(), key=operator.itemgetter(0), reverse=True):
+        click.echo(f"\n{semester}:")
+        for course_id, course_name in courses:
+            click.echo(f"- Course ID: {course_id}, Course Name: {course_name}")
 
 @fetch.command("grades")
 @click.argument("course_id", nargs=-1, type=str)
 @click.option("-e", "--export", is_flag=True, help="Export grades to a .csv file")
 def fetch_grades(course_id, export):
     config = load_config()
     headers = {"Authorization": f"Bearer {config['api_key']}"}
```

### Comparing `canvas-pilot-0.1.1/setup.py` & `canvas-pilot-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 
 # Get the README.md content
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="canvas-pilot",
-    version="0.1.1",
+    version="0.1.2",
     packages=find_packages(),
     install_requires=[
         "requests",
         "icalendar",
         "click",
+        "getpass4",
     ],
     entry_points={
         "console_scripts": [
             "canvas=canvas_tools.canvas:main",
         ],
     },
     author="Ziang Zhou",
@@ -35,8 +36,7 @@
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
     ],
     python_requires=">=3.6, <4",
 )
-
```

