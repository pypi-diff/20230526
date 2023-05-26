# Comparing `tmp/canvas-pilot-0.1.2.tar.gz` & `tmp/canvas-pilot-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "canvas-pilot-0.1.2.tar", last modified: Fri May 26 05:33:03 2023, max compression
+gzip compressed data, was "canvas-pilot-0.1.3.tar", last modified: Fri May 26 05:48:07 2023, max compression
```

## Comparing `canvas-pilot-0.1.2.tar` & `canvas-pilot-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ziang      (501) staff       (20)        0 2023-05-26 05:33:03.240525 canvas-pilot-0.1.2/
--rw-r--r--   0 ziang      (501) staff       (20)    35148 2023-05-05 00:58:23.000000 canvas-pilot-0.1.2/LICENSE
--rw-r--r--   0 ziang      (501) staff       (20)     3539 2023-05-26 05:33:03.240388 canvas-pilot-0.1.2/PKG-INFO
--rw-r--r--   0 ziang      (501) staff       (20)     2732 2023-05-26 05:17:16.000000 canvas-pilot-0.1.2/README.md
-drwxr-xr-x   0 ziang      (501) staff       (20)        0 2023-05-26 05:33:03.240001 canvas-pilot-0.1.2/canvas_pilot.egg-info/
--rw-r--r--   0 ziang      (501) staff       (20)     3539 2023-05-26 05:33:03.000000 canvas-pilot-0.1.2/canvas_pilot.egg-info/PKG-INFO
--rw-r--r--   0 ziang      (501) staff       (20)      292 2023-05-26 05:33:03.000000 canvas-pilot-0.1.2/canvas_pilot.egg-info/SOURCES.txt
--rw-r--r--   0 ziang      (501) staff       (20)        1 2023-05-26 05:33:03.000000 canvas-pilot-0.1.2/canvas_pilot.egg-info/dependency_links.txt
--rw-r--r--   0 ziang      (501) staff       (20)       52 2023-05-26 05:33:03.000000 canvas-pilot-0.1.2/canvas_pilot.egg-info/entry_points.txt
--rw-r--r--   0 ziang      (501) staff       (20)       34 2023-05-26 05:33:03.000000 canvas-pilot-0.1.2/canvas_pilot.egg-info/requires.txt
--rw-r--r--   0 ziang      (501) staff       (20)       13 2023-05-26 05:33:03.000000 canvas-pilot-0.1.2/canvas_pilot.egg-info/top_level.txt
-drwxr-xr-x   0 ziang      (501) staff       (20)        0 2023-05-26 05:33:03.240221 canvas-pilot-0.1.2/canvas_tools/
--rw-r--r--   0 ziang      (501) staff       (20)        0 2023-05-04 20:58:38.000000 canvas-pilot-0.1.2/canvas_tools/__init__.py
--rw-r--r--   0 ziang      (501) staff       (20)     7787 2023-05-26 05:32:54.000000 canvas-pilot-0.1.2/canvas_tools/canvas.py
--rw-r--r--   0 ziang      (501) staff       (20)       38 2023-05-26 05:33:03.240568 canvas-pilot-0.1.2/setup.cfg
--rw-r--r--   0 ziang      (501) staff       (20)     1345 2023-05-26 05:33:00.000000 canvas-pilot-0.1.2/setup.py
+drwxr-xr-x   0 ziang      (501) staff       (20)        0 2023-05-26 05:48:07.280339 canvas-pilot-0.1.3/
+-rw-r--r--   0 ziang      (501) staff       (20)    35148 2023-05-05 00:58:23.000000 canvas-pilot-0.1.3/LICENSE
+-rw-r--r--   0 ziang      (501) staff       (20)     3998 2023-05-26 05:48:07.280158 canvas-pilot-0.1.3/PKG-INFO
+-rw-r--r--   0 ziang      (501) staff       (20)     3191 2023-05-26 05:47:26.000000 canvas-pilot-0.1.3/README.md
+drwxr-xr-x   0 ziang      (501) staff       (20)        0 2023-05-26 05:48:07.279745 canvas-pilot-0.1.3/canvas_pilot.egg-info/
+-rw-r--r--   0 ziang      (501) staff       (20)     3998 2023-05-26 05:48:07.000000 canvas-pilot-0.1.3/canvas_pilot.egg-info/PKG-INFO
+-rw-r--r--   0 ziang      (501) staff       (20)      292 2023-05-26 05:48:07.000000 canvas-pilot-0.1.3/canvas_pilot.egg-info/SOURCES.txt
+-rw-r--r--   0 ziang      (501) staff       (20)        1 2023-05-26 05:48:07.000000 canvas-pilot-0.1.3/canvas_pilot.egg-info/dependency_links.txt
+-rw-r--r--   0 ziang      (501) staff       (20)       52 2023-05-26 05:48:07.000000 canvas-pilot-0.1.3/canvas_pilot.egg-info/entry_points.txt
+-rw-r--r--   0 ziang      (501) staff       (20)       34 2023-05-26 05:48:07.000000 canvas-pilot-0.1.3/canvas_pilot.egg-info/requires.txt
+-rw-r--r--   0 ziang      (501) staff       (20)       13 2023-05-26 05:48:07.000000 canvas-pilot-0.1.3/canvas_pilot.egg-info/top_level.txt
+drwxr-xr-x   0 ziang      (501) staff       (20)        0 2023-05-26 05:48:07.279974 canvas-pilot-0.1.3/canvas_tools/
+-rw-r--r--   0 ziang      (501) staff       (20)        0 2023-05-04 20:58:38.000000 canvas-pilot-0.1.3/canvas_tools/__init__.py
+-rw-r--r--   0 ziang      (501) staff       (20)     7873 2023-05-26 05:38:10.000000 canvas-pilot-0.1.3/canvas_tools/canvas.py
+-rw-r--r--   0 ziang      (501) staff       (20)       38 2023-05-26 05:48:07.280382 canvas-pilot-0.1.3/setup.cfg
+-rw-r--r--   0 ziang      (501) staff       (20)     1345 2023-05-26 05:47:47.000000 canvas-pilot-0.1.3/setup.py
```

### Comparing `canvas-pilot-0.1.2/LICENSE` & `canvas-pilot-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `canvas-pilot-0.1.2/PKG-INFO` & `canvas-pilot-0.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canvas-pilot
-Version: 0.1.2
+Version: 0.1.3
 Summary: A command-line tool for managing Canvas courses, fetching assignments, and grades.
 Home-page: https://github.com/realzza/canvas-cli
 Author: Ziang Zhou
 Author-email: ziang.zhou518@gmail.com
 License: GPLv3+
 Keywords: canvas api cli
 Classifier: Development Status :: 3 - Alpha
@@ -17,14 +17,18 @@
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Canvas Pilot
 
+![PyPI](https://img.shields.io/pypi/v/canvas_pilot?color=df)&nbsp;
+![GitHub](https://img.shields.io/github/license/realzza/canvas-pilot?color=%23FFB6C1)&nbsp;
+![GitHub last commit](https://img.shields.io/github/last-commit/realzza/canvas-pilot?color=orange)&nbsp;
+[![CodeFactor](https://www.codefactor.io/repository/github/realzza/canvas-pilot/badge)](https://www.codefactor.io/repository/github/realzza/canvas-pilot)&nbsp;
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/canvas-pilot)
 
 A command-line tool for managing your Canvas courses, fetching assignments, and grades.
 
 ## Installation
 
 To install the Canvas CLI, run the following command:
@@ -57,19 +61,15 @@
 
 Once you have your API key and domain, run the following command and follow the prompts to configure the Canvas CLI:
 
 ```bash
 canvas configure
 ```
 
-You can reconfigure the Canvas API key and domain at any time by running:
-
-```bash
-canvas reconfigure
-```
+You can reconfigure the Canvas API key and domain at any time by running `canvas configure` again. You will be prompted to update your keys.
 
 ## Usage
 
 ### Fetch Courses
 
 To fetch the list of your Canvas courses, run:
```

### Comparing `canvas-pilot-0.1.2/canvas_pilot.egg-info/PKG-INFO` & `canvas-pilot-0.1.3/canvas_pilot.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canvas-pilot
-Version: 0.1.2
+Version: 0.1.3
 Summary: A command-line tool for managing Canvas courses, fetching assignments, and grades.
 Home-page: https://github.com/realzza/canvas-cli
 Author: Ziang Zhou
 Author-email: ziang.zhou518@gmail.com
 License: GPLv3+
 Keywords: canvas api cli
 Classifier: Development Status :: 3 - Alpha
@@ -17,14 +17,18 @@
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Canvas Pilot
 
+![PyPI](https://img.shields.io/pypi/v/canvas_pilot?color=df)&nbsp;
+![GitHub](https://img.shields.io/github/license/realzza/canvas-pilot?color=%23FFB6C1)&nbsp;
+![GitHub last commit](https://img.shields.io/github/last-commit/realzza/canvas-pilot?color=orange)&nbsp;
+[![CodeFactor](https://www.codefactor.io/repository/github/realzza/canvas-pilot/badge)](https://www.codefactor.io/repository/github/realzza/canvas-pilot)&nbsp;
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/canvas-pilot)
 
 A command-line tool for managing your Canvas courses, fetching assignments, and grades.
 
 ## Installation
 
 To install the Canvas CLI, run the following command:
@@ -57,19 +61,15 @@
 
 Once you have your API key and domain, run the following command and follow the prompts to configure the Canvas CLI:
 
 ```bash
 canvas configure
 ```
 
-You can reconfigure the Canvas API key and domain at any time by running:
-
-```bash
-canvas reconfigure
-```
+You can reconfigure the Canvas API key and domain at any time by running `canvas configure` again. You will be prompted to update your keys.
 
 ## Usage
 
 ### Fetch Courses
 
 To fetch the list of your Canvas courses, run:
```

### Comparing `canvas-pilot-0.1.2/canvas_tools/canvas.py` & `canvas-pilot-0.1.3/canvas_tools/canvas.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-import getpass4
 import json
+import operator
 import os
+from collections import defaultdict
 from datetime import datetime
 
-import operator
-from collections import defaultdict
 import click
+import getpass4
 import requests
 from icalendar import Calendar, Event
 
 CONFIG_FILE = "canvas_config.json"
 
 
 def load_config():
@@ -45,34 +45,36 @@
             break
 
         all_results.extend(results)
         page += 1
 
     return all_results
 
+
 def parse_semester(start_date, end_date):
-    start_date = datetime.strptime(start_date, '%Y-%m-%dT%H:%M:%SZ')
-    end_date = datetime.strptime(end_date, '%Y-%m-%dT%H:%M:%SZ')
-    
+    start_date = datetime.strptime(start_date, "%Y-%m-%dT%H:%M:%SZ")
+    end_date = datetime.strptime(end_date, "%Y-%m-%dT%H:%M:%SZ")
+
     if start_date.month <= 5 and end_date.month <= 5:
-        return f'Spring {start_date.year}'
+        return f"Spring {start_date.year}"
     elif start_date.month >= 8 and end_date.month >= 8:
-        return f'Fall {start_date.year}'
+        return f"Fall {start_date.year}"
     else:
-        return f'Summer {start_date.year}'
+        return f"Summer {start_date.year}"
+
 
 @click.group()
 def main():
     pass
 
 
 @main.command("configure")
 def configure():
     if os.path.exists(CONFIG_FILE):
-        if click.confirm('Configuration already exists. Do you want to overwrite it?'):
+        if click.confirm("Configuration already exists. Do you want to overwrite it?"):
             api_key = getpass4.getpass("Canvas API key: ")
             domain = click.prompt("Canvas domain (e.g., canvas.<yourinstitution>.com)")
             config = {"api_key": api_key, "domain": domain}
             save_config(config)
             click.echo("Configuration saved.")
     else:
         api_key = getpass4.getpass("Canvas API key: ")
@@ -135,37 +137,46 @@
                     cal.add_component(event)
 
     if export:
         with open("canvas_assignments.ics", "wb") as f:
             f.write(cal.to_ical())
         click.echo("Assignments exported to canvas_assignments.ics")
 
+
 @fetch.command("courses")
 def fetch_courses():
     config = load_config()
 
     headers = {"Authorization": f"Bearer {config['api_key']}"}
 
     url_courses = f"{config['domain']}/api/v1/courses?enrollment_type=student&enrollment_state=active"
     courses = fetch_all_pages(url_courses, headers)
-    
+
     semester_courses = defaultdict(list)
     for course in courses:
         if "name" in course:
-            if "start_at" in course and "end_at" in course and course['start_at'] and course['end_at']:
-                semester = parse_semester(course['start_at'], course['end_at'])
+            if (
+                "start_at" in course
+                and "end_at" in course
+                and course["start_at"]
+                and course["end_at"]
+            ):
+                semester = parse_semester(course["start_at"], course["end_at"])
             else:
                 semester = "No Semester"
-            semester_courses[semester].append((course['id'], course['name']))
-    
-    for semester, courses in sorted(semester_courses.items(), key=operator.itemgetter(0), reverse=True):
+            semester_courses[semester].append((course["id"], course["name"]))
+
+    for semester, courses in sorted(
+        semester_courses.items(), key=operator.itemgetter(0), reverse=True
+    ):
         click.echo(f"\n{semester}:")
         for course_id, course_name in courses:
             click.echo(f"- Course ID: {course_id}, Course Name: {course_name}")
 
+
 @fetch.command("grades")
 @click.argument("course_id", nargs=-1, type=str)
 @click.option("-e", "--export", is_flag=True, help="Export grades to a .csv file")
 def fetch_grades(course_id, export):
     config = load_config()
     headers = {"Authorization": f"Bearer {config['api_key']}"}
```

### Comparing `canvas-pilot-0.1.2/setup.py` & `canvas-pilot-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Get the README.md content
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="canvas-pilot",
-    version="0.1.2",
+    version="0.1.3",
     packages=find_packages(),
     install_requires=[
         "requests",
         "icalendar",
         "click",
         "getpass4",
     ],
```

