# Comparing `tmp/tscratchapiget-0.2.7.tar.gz` & `tmp/tscratchapiget-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tscratchapiget-0.2.7.tar", last modified: Mon Sep 26 14:46:00 2022, max compression
+gzip compressed data, was "tscratchapiget-0.2.9.tar", last modified: Fri May 26 15:05:40 2023, max compression
```

## Comparing `tscratchapiget-0.2.7.tar` & `tscratchapiget-0.2.9.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-09-26 14:46:00.624042 tscratchapiget-0.2.7/
--rw-rw-rw-   0        0        0     1065 2022-09-10 14:01:46.000000 tscratchapiget-0.2.7/LICENSE
--rw-rw-rw-   0        0        0     3125 2022-09-26 14:46:00.623044 tscratchapiget-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0     1374 2022-09-26 14:45:21.000000 tscratchapiget-0.2.7/README.md
--rw-rw-rw-   0        0        0      639 2022-09-26 14:45:21.000000 tscratchapiget-0.2.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-09-26 14:46:00.625041 tscratchapiget-0.2.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-09-26 14:46:00.493890 tscratchapiget-0.2.7/src/
-drwxrwxrwx   0        0        0        0 2022-09-26 14:46:00.504883 tscratchapiget-0.2.7/src/tscratchapiget/
--rw-rw-rw-   0        0        0        0 2022-09-10 01:07:31.000000 tscratchapiget-0.2.7/src/tscratchapiget/_init_.py
--rw-rw-rw-   0        0        0     2106 2022-09-26 14:45:21.000000 tscratchapiget-0.2.7/src/tscratchapiget/user.py
-drwxrwxrwx   0        0        0        0 2022-09-26 14:46:00.621040 tscratchapiget-0.2.7/src/tscratchapiget.egg-info/
--rw-rw-rw-   0        0        0     3125 2022-09-26 14:46:00.000000 tscratchapiget-0.2.7/src/tscratchapiget.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      256 2022-09-26 14:46:00.000000 tscratchapiget-0.2.7/src/tscratchapiget.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-26 14:46:00.000000 tscratchapiget-0.2.7/src/tscratchapiget.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2022-09-26 14:46:00.000000 tscratchapiget-0.2.7/src/tscratchapiget.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-26 15:05:40.367826 tscratchapiget-0.2.9/
+-rw-rw-rw-   0        0        0     1075 2023-05-21 08:00:32.000000 tscratchapiget-0.2.9/LICENSE
+-rw-rw-rw-   0        0        0     3627 2023-05-26 15:05:40.366821 tscratchapiget-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1806 2023-05-26 14:21:43.000000 tscratchapiget-0.2.9/README.md
+-rw-rw-rw-   0        0        0      639 2023-05-26 15:04:41.000000 tscratchapiget-0.2.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-26 15:05:40.368822 tscratchapiget-0.2.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-26 15:05:40.300447 tscratchapiget-0.2.9/src/
+drwxrwxrwx   0        0        0        0 2023-05-26 15:05:40.335722 tscratchapiget-0.2.9/src/tscratchapiget/
+-rw-rw-rw-   0        0        0        0 2023-05-21 04:30:30.000000 tscratchapiget-0.2.9/src/tscratchapiget/__init__.py
+-rw-rw-rw-   0        0        0     2405 2023-05-26 14:21:43.000000 tscratchapiget-0.2.9/src/tscratchapiget/user.py
+drwxrwxrwx   0        0        0        0 2023-05-26 15:05:40.356739 tscratchapiget-0.2.9/src/tscratchapiget.egg-info/
+-rw-rw-rw-   0        0        0     3627 2023-05-26 15:05:40.000000 tscratchapiget-0.2.9/src/tscratchapiget.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-05-26 15:05:40.000000 tscratchapiget-0.2.9/src/tscratchapiget.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 15:05:40.000000 tscratchapiget-0.2.9/src/tscratchapiget.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-26 15:05:40.000000 tscratchapiget-0.2.9/src/tscratchapiget.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-26 15:05:40.364299 tscratchapiget-0.2.9/tests/
+-rw-rw-rw-   0        0        0       71 2023-05-26 14:54:28.000000 tscratchapiget-0.2.9/tests/test.py
```

### Comparing `tscratchapiget-0.2.7/LICENSE` & `tscratchapiget-0.2.9/LICENSE`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-Copyright (c) 2022 Tony
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 Scratch_Tony_14261
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `tscratchapiget-0.2.7/PKG-INFO` & `tscratchapiget-0.2.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: tscratchapiget
-Version: 0.2.7
+Version: 0.2.9
 Summary: A library can get scratch api
 Author-email: Tony <tonyvu4913@gmail.com>
-License: Copyright (c) 2022 Tony
+License: MIT License
+        
+        Copyright (c) 2022 Scratch_Tony_14261
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -18,30 +20,34 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
+        
 Project-URL: Homepage, https://github.com/Tony14261/tscratchapiget
 Project-URL: Bug Tracker, https://github.com/Tony14261/tscratchapiget/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-This project gets the scratch api. Everything in this project code by me (except some needed library). Big credit to TimMcCool(Scratcher) for example codes.
+This project gets the scratch api. Everything in this project code by me (except some needed library). Big credit to TimMcCool(Scratcher) for example codes. (This project is not related to TimMcCool)<br>
+Install: `pip install tscratchapiget`
+Change log: https://github.com/Tony14261/tscratchapiget/blob/main/change.log
 
-This can do:
-    User features(v0.2.5 to v0.2.7):
-        - Get a user unread-message-count ```message_count('[user]')```     EX: ```user.message_count('TimMcCool')```
-        - Get a user id ```id('[user]')```     EX: ```user.id('griffpatch')```
-        - Get if a user is a scratchteam ```scratchteam('[user]')```     EX: ```user.scratchteam('ScratchCat')``` #Return 'True'
-        - Get user join date ```join('[user]')```     EX: ```user.join('Will_Wam')```#Return '2013-11-25T19:52:29.000Z'
-        - Get a user pfp(link) ```pfp_link('[user]')```     EX: ```user.pfp_link('Scratch_Tony_14261')```          +Bonus Feature: Open that pfp link in browser. Change that to ```pfp_link_open('[Username]')```
-        - Get user About-Me section ```aboutme('[user]')``` EX: ```user.aboutme('WazzoTV')```
-        - Get user What-I'm-Working-On section ```wiwo('[username]')```     EX: ```user.wiwo('ceebee')```
-        - Get user country ```country(['user]')```     EX: ```user.country(['')```
-        - Get user follower count ```followers('[user]')```     Ex: ```user.followers('sharkyshar')```
-        - Get user following count ```following('[user]')```     EX: ```user.followers('atomicmagicnumber')```
+**This can do**<br>
+    **User features(v0.2.7)(Updated commands in v0.3.0)** (New commands are at the top):<br>
+        - Get if a username exists  ```exists([username])```     EX: ```user.exists('Scratch_Tony_14261')``` if yes: Return 'User exists'     if not: Return 'User does not exist'
+        - Get a user unread-message-count ```message_count('[user]')```     EX: ```user.message_count('TimMcCool')```<br>
+        - Get a user id ```id('[user]')```     EX: ```user.id('griffpatch')```<br>
+        - Get if a user is a scratchteam ```scratchteam('[user]')```     EX: ```user.scratchteam('ScratchCat')``` #Return 'True'<br>
+        - Get user join date ```join('[user]')```     EX: ```user.join('Will_Wam')```#Return '2013-11-25T19:52:29.000Z'<br>
+        - Get a user pfp(link) ```pfp_link('[user]')```     EX: ```user.pfp_link('Scratch_Tony_14261')```          +Bonus Feature: Open that pfp link in browser. Change that to ```pfp_link_open('[Username]')```<br>
+        - Get user About-Me section ```aboutme('[user]')``` EX: ```user.aboutme('WazzoTV')```<br>
+        - Get user What-I'm-Working-On section ```wiwo('[username]')```     EX: ```user.wiwo('ceebee')```<br>
+        - Get user country ```country(['user]')```     EX: ```user.country(['')```<br>
+        - Get user follower count ```followers('[user]')```     Ex: ```user.followers('sharkyshar')```<br>
+        - Get user following count ```following('[user]')```     EX: ```user.followers('atomicmagicnumber')```<br>
```

### Comparing `tscratchapiget-0.2.7/README.md` & `tscratchapiget-0.2.9/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,17 @@
-This project gets the scratch api. Everything in this project code by me (except some needed library). Big credit to TimMcCool(Scratcher) for example codes.
-
-This can do:
-    User features(v0.2.5 to v0.2.7):
-        - Get a user unread-message-count ```message_count('[user]')```     EX: ```user.message_count('TimMcCool')```
-        - Get a user id ```id('[user]')```     EX: ```user.id('griffpatch')```
-        - Get if a user is a scratchteam ```scratchteam('[user]')```     EX: ```user.scratchteam('ScratchCat')``` #Return 'True'
-        - Get user join date ```join('[user]')```     EX: ```user.join('Will_Wam')```#Return '2013-11-25T19:52:29.000Z'
-        - Get a user pfp(link) ```pfp_link('[user]')```     EX: ```user.pfp_link('Scratch_Tony_14261')```          +Bonus Feature: Open that pfp link in browser. Change that to ```pfp_link_open('[Username]')```
-        - Get user About-Me section ```aboutme('[user]')``` EX: ```user.aboutme('WazzoTV')```
-        - Get user What-I'm-Working-On section ```wiwo('[username]')```     EX: ```user.wiwo('ceebee')```
-        - Get user country ```country(['user]')```     EX: ```user.country(['')```
-        - Get user follower count ```followers('[user]')```     Ex: ```user.followers('sharkyshar')```
-        - Get user following count ```following('[user]')```     EX: ```user.followers('atomicmagicnumber')```
+This project gets the scratch api. Everything in this project code by me (except some needed library). Big credit to TimMcCool(Scratcher) for example codes. (This project is not related to TimMcCool)<br>
+Install: `pip install tscratchapiget`
+Change log: https://github.com/Tony14261/tscratchapiget/blob/main/change.log
+
+**This can do**<br>
+    **User features(v0.2.7)(Updated commands in v0.3.0)** (New commands are at the top):<br>
+        - Get if a username exists  ```exists([username])```     EX: ```user.exists('Scratch_Tony_14261')``` if yes: Return 'User exists'     if not: Return 'User does not exist'
+        - Get a user unread-message-count ```message_count('[user]')```     EX: ```user.message_count('TimMcCool')```<br>
+        - Get a user id ```id('[user]')```     EX: ```user.id('griffpatch')```<br>
+        - Get if a user is a scratchteam ```scratchteam('[user]')```     EX: ```user.scratchteam('ScratchCat')``` #Return 'True'<br>
+        - Get user join date ```join('[user]')```     EX: ```user.join('Will_Wam')```#Return '2013-11-25T19:52:29.000Z'<br>
+        - Get a user pfp(link) ```pfp_link('[user]')```     EX: ```user.pfp_link('Scratch_Tony_14261')```          +Bonus Feature: Open that pfp link in browser. Change that to ```pfp_link_open('[Username]')```<br>
+        - Get user About-Me section ```aboutme('[user]')``` EX: ```user.aboutme('WazzoTV')```<br>
+        - Get user What-I'm-Working-On section ```wiwo('[username]')```     EX: ```user.wiwo('ceebee')```<br>
+        - Get user country ```country(['user]')```     EX: ```user.country(['')```<br>
+        - Get user follower count ```followers('[user]')```     Ex: ```user.followers('sharkyshar')```<br>
+        - Get user following count ```following('[user]')```     EX: ```user.followers('atomicmagicnumber')```<br>
```

### Comparing `tscratchapiget-0.2.7/pyproject.toml` & `tscratchapiget-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tscratchapiget"
-version = "0.2.7"
+version = "0.2.9"
 authors = [
   { name="Tony", email="tonyvu4913@gmail.com" },
 ]
 description = "A library can get scratch api"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9"
```

### Comparing `tscratchapiget-0.2.7/src/tscratchapiget/user.py` & `tscratchapiget-0.2.9/src/tscratchapiget/user.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-import json
 import requests
+import json
 import webbrowser
 
 global message_count
 global id
 global scratchteam
 global join
 global pfp_link
 global pfp_link_open
 global aboutme
 global wiwo
 global country
 global followers
 global following
+global exist
 
 def message_count(username):
     return (json.loads(requests.get(f"https://api.scratch.mit.edu/users/{username}/messages/count/", headers = {'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.3c6 (KHTML, like Gecko) Chrome/75.0.3770.142 Safari/537.36',}).text)["count"])
 
 def id(username):
     data = json.loads(requests.get(f"https://api.scratch.mit.edu/users/{username}/").text)
     return (data["id"])
@@ -37,22 +38,30 @@
     data = json.loads(requests.get(f"https://api.scratch.mit.edu/users/{username}/").text)
     webbrowser.open_new(data['profile']['images']['90x90'])
 
 def aboutme(username):
     data = json.loads(requests.get(f"https://api.scratch.mit.edu/users/{username}/").text)
     return (data['status'])
 
-def wiwo(username):
+def wiwo(username): #What im working on
     data = json.loads(requests.get(f"https://api.scratch.mit.edu/users/{username}/").text)
     return (data['bio'])
 
 def country(username):
     data = json.loads(requests.get(f"https://api.scratch.mit.edu/users/{username}/").text)
     return (data['country'])
 
 def followers(username):
     data = json.loads(requests.get(f"https://scratchdb.lefty.one/v3/user/info/{username}/").text)
     return (data['statistics']['followers'])
 
 def following(username):
     data = json.loads(requests.get(f"https://scratchdb.lefty.one/v3/user/info/{username}/").text)
-    return (data['statistics']['following'])
+    return (data['statistics']['following'])
+
+def exist(username):
+    data = json.loads(requests.get(f"https://api.scratch.mit.edu/users/{username}/").text)
+    try:
+        if data['code'] == 'NotFound':
+            return 'User does not exist'
+    except Exception:
+            return 'User exists'
```

### Comparing `tscratchapiget-0.2.7/src/tscratchapiget.egg-info/PKG-INFO` & `tscratchapiget-0.2.9/src/tscratchapiget.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: tscratchapiget
-Version: 0.2.7
+Version: 0.2.9
 Summary: A library can get scratch api
 Author-email: Tony <tonyvu4913@gmail.com>
-License: Copyright (c) 2022 Tony
+License: MIT License
+        
+        Copyright (c) 2022 Scratch_Tony_14261
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -18,30 +20,34 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
+        
 Project-URL: Homepage, https://github.com/Tony14261/tscratchapiget
 Project-URL: Bug Tracker, https://github.com/Tony14261/tscratchapiget/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-This project gets the scratch api. Everything in this project code by me (except some needed library). Big credit to TimMcCool(Scratcher) for example codes.
+This project gets the scratch api. Everything in this project code by me (except some needed library). Big credit to TimMcCool(Scratcher) for example codes. (This project is not related to TimMcCool)<br>
+Install: `pip install tscratchapiget`
+Change log: https://github.com/Tony14261/tscratchapiget/blob/main/change.log
 
-This can do:
-    User features(v0.2.5 to v0.2.7):
-        - Get a user unread-message-count ```message_count('[user]')```     EX: ```user.message_count('TimMcCool')```
-        - Get a user id ```id('[user]')```     EX: ```user.id('griffpatch')```
-        - Get if a user is a scratchteam ```scratchteam('[user]')```     EX: ```user.scratchteam('ScratchCat')``` #Return 'True'
-        - Get user join date ```join('[user]')```     EX: ```user.join('Will_Wam')```#Return '2013-11-25T19:52:29.000Z'
-        - Get a user pfp(link) ```pfp_link('[user]')```     EX: ```user.pfp_link('Scratch_Tony_14261')```          +Bonus Feature: Open that pfp link in browser. Change that to ```pfp_link_open('[Username]')```
-        - Get user About-Me section ```aboutme('[user]')``` EX: ```user.aboutme('WazzoTV')```
-        - Get user What-I'm-Working-On section ```wiwo('[username]')```     EX: ```user.wiwo('ceebee')```
-        - Get user country ```country(['user]')```     EX: ```user.country(['')```
-        - Get user follower count ```followers('[user]')```     Ex: ```user.followers('sharkyshar')```
-        - Get user following count ```following('[user]')```     EX: ```user.followers('atomicmagicnumber')```
+**This can do**<br>
+    **User features(v0.2.7)(Updated commands in v0.3.0)** (New commands are at the top):<br>
+        - Get if a username exists  ```exists([username])```     EX: ```user.exists('Scratch_Tony_14261')``` if yes: Return 'User exists'     if not: Return 'User does not exist'
+        - Get a user unread-message-count ```message_count('[user]')```     EX: ```user.message_count('TimMcCool')```<br>
+        - Get a user id ```id('[user]')```     EX: ```user.id('griffpatch')```<br>
+        - Get if a user is a scratchteam ```scratchteam('[user]')```     EX: ```user.scratchteam('ScratchCat')``` #Return 'True'<br>
+        - Get user join date ```join('[user]')```     EX: ```user.join('Will_Wam')```#Return '2013-11-25T19:52:29.000Z'<br>
+        - Get a user pfp(link) ```pfp_link('[user]')```     EX: ```user.pfp_link('Scratch_Tony_14261')```          +Bonus Feature: Open that pfp link in browser. Change that to ```pfp_link_open('[Username]')```<br>
+        - Get user About-Me section ```aboutme('[user]')``` EX: ```user.aboutme('WazzoTV')```<br>
+        - Get user What-I'm-Working-On section ```wiwo('[username]')```     EX: ```user.wiwo('ceebee')```<br>
+        - Get user country ```country(['user]')```     EX: ```user.country(['')```<br>
+        - Get user follower count ```followers('[user]')```     Ex: ```user.followers('sharkyshar')```<br>
+        - Get user following count ```following('[user]')```     EX: ```user.followers('atomicmagicnumber')```<br>
```

