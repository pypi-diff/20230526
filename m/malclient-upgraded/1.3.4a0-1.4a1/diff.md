# Comparing `tmp/malclient-upgraded-1.3.4a0.tar.gz` & `tmp/malclient-upgraded-1.4a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "malclient-upgraded-1.3.4a0.tar", last modified: Tue Mar 28 11:10:42 2023, max compression
+gzip compressed data, was "malclient-upgraded-1.4a1.tar", last modified: Thu May 25 23:50:41 2023, max compression
```

## Comparing `malclient-upgraded-1.3.4a0.tar` & `malclient-upgraded-1.4a1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 gruzin    (1000) gruzin    (1000)        0 2023-03-28 11:10:42.021728 malclient-upgraded-1.3.4a0/
--rw-r--r--   0 gruzin    (1000) gruzin    (1000)     1066 2022-10-25 07:20:09.000000 malclient-upgraded-1.3.4a0/LICENSE
--rw-r--r--   0 gruzin    (1000) gruzin    (1000)     4749 2023-03-28 11:10:42.021728 malclient-upgraded-1.3.4a0/PKG-INFO
--rw-r--r--   0 gruzin    (1000) gruzin    (1000)     4150 2022-10-25 07:20:09.000000 malclient-upgraded-1.3.4a0/README.md
-drwxr-xr-x   0 gruzin    (1000) gruzin    (1000)        0 2023-03-28 11:10:42.021728 malclient-upgraded-1.3.4a0/malclient/
-drwxr-xr-x   0 gruzin    (1000) gruzin    (1000)        0 2023-03-28 11:10:42.021728 malclient-upgraded-1.3.4a0/malclient/Datamodels/
--rw-r--r--   0 gruzin    (1000) gruzin    (1000)      101 2022-10-25 07:20:09.000000 malclient-upgraded-1.3.4a0/malclient/Datamodels/__init__.py
--rw-r--r--   0 gruzin    (1000) gruzin    (1000)     7120 2023-01-23 14:39:28.000000 malclient-upgraded-1.3.4a0/malclient/Datamodels/enums.py
--rw-r--r--   0 gruzin    (1000) gruzin    (1000)    14683 2023-01-23 14:39:28.000000 malclient-upgraded-1.3.4a0/malclient/Datamodels/fields.py
--rw-r--r--   0 gruzin    (1000) gruzin    (1000)    12191 2023-01-24 08:26:33.000000 malclient-upgraded-1.3.4a0/malclient/Datamodels/models.py
--rw-r--r--   0 gruzin    (1000) gruzin    (1000)     1244 2022-10-25 07:20:09.000000 malclient-upgraded-1.3.4a0/malclient/Datamodels/pagination.py
--rw-r--r--   0 gruzin    (1000) gruzin    (1000)       74 2022-11-21 08:17:04.000000 malclient-upgraded-1.3.4a0/malclient/__init__.py
--rw-r--r--   0 gruzin    (1000) gruzin    (1000)     7017 2022-11-04 12:07:01.000000 malclient-upgraded-1.3.4a0/malclient/anime.py
--rw-r--r--   0 gruzin    (1000) gruzin    (1000)     3261 2022-10-28 15:19:53.000000 malclient-upgraded-1.3.4a0/malclient/boards.py
--rw-r--r--   0 gruzin    (1000) gruzin    (1000)     7629 2023-01-23 14:39:28.000000 malclient-upgraded-1.3.4a0/malclient/client.py
--rw-r--r--   0 gruzin    (1000) gruzin    (1000)     2009 2023-01-23 14:39:28.000000 malclient-upgraded-1.3.4a0/malclient/exceptions.py
--rw-r--r--   0 gruzin    (1000) gruzin    (1000)     3749 2023-01-23 14:39:28.000000 malclient-upgraded-1.3.4a0/malclient/manga.py
--rw-r--r--   0 gruzin    (1000) gruzin    (1000)    11985 2023-01-23 14:39:28.000000 malclient-upgraded-1.3.4a0/malclient/my_list.py
--rw-r--r--   0 gruzin    (1000) gruzin    (1000)     3504 2023-01-23 14:39:28.000000 malclient-upgraded-1.3.4a0/malclient/request_handler.py
-drwxr-xr-x   0 gruzin    (1000) gruzin    (1000)        0 2023-03-28 11:10:42.021728 malclient-upgraded-1.3.4a0/malclient_upgraded.egg-info/
--rw-r--r--   0 gruzin    (1000) gruzin    (1000)     4749 2023-03-28 11:10:42.000000 malclient-upgraded-1.3.4a0/malclient_upgraded.egg-info/PKG-INFO
--rw-r--r--   0 gruzin    (1000) gruzin    (1000)      594 2023-03-28 11:10:42.000000 malclient-upgraded-1.3.4a0/malclient_upgraded.egg-info/SOURCES.txt
--rw-r--r--   0 gruzin    (1000) gruzin    (1000)        1 2023-03-28 11:10:42.000000 malclient-upgraded-1.3.4a0/malclient_upgraded.egg-info/dependency_links.txt
--rw-r--r--   0 gruzin    (1000) gruzin    (1000)       18 2023-03-28 11:10:42.000000 malclient-upgraded-1.3.4a0/malclient_upgraded.egg-info/requires.txt
--rw-r--r--   0 gruzin    (1000) gruzin    (1000)       10 2023-03-28 11:10:42.000000 malclient-upgraded-1.3.4a0/malclient_upgraded.egg-info/top_level.txt
--rw-r--r--   0 gruzin    (1000) gruzin    (1000)      142 2022-10-25 07:20:09.000000 malclient-upgraded-1.3.4a0/pyproject.toml
--rw-r--r--   0 gruzin    (1000) gruzin    (1000)       79 2023-03-28 11:10:42.021728 malclient-upgraded-1.3.4a0/setup.cfg
--rw-r--r--   0 gruzin    (1000) gruzin    (1000)      865 2023-03-28 11:07:06.000000 malclient-upgraded-1.3.4a0/setup.py
+drwxrwxrwx   0 gruzin    (1000) gruzin    (1000)        0 2023-05-25 23:50:41.894634 malclient-upgraded-1.4a1/
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     1087 2022-11-08 15:30:53.000000 malclient-upgraded-1.4a1/LICENSE
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     4655 2023-05-25 23:50:41.894634 malclient-upgraded-1.4a1/PKG-INFO
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     4165 2023-05-25 23:49:17.000000 malclient-upgraded-1.4a1/README.md
+drwxrwxrwx   0 gruzin    (1000) gruzin    (1000)        0 2023-05-25 23:50:41.861095 malclient-upgraded-1.4a1/malclient/
+drwxrwxrwx   0 gruzin    (1000) gruzin    (1000)        0 2023-05-25 23:50:41.884628 malclient-upgraded-1.4a1/malclient/Datamodels/
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)      105 2022-11-08 19:51:57.000000 malclient-upgraded-1.4a1/malclient/Datamodels/__init__.py
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     7420 2022-11-22 17:28:58.000000 malclient-upgraded-1.4a1/malclient/Datamodels/enums.py
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)    15784 2023-05-25 23:44:42.000000 malclient-upgraded-1.4a1/malclient/Datamodels/fields.py
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)    13014 2023-05-25 23:02:33.000000 malclient-upgraded-1.4a1/malclient/Datamodels/models.py
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     1275 2022-11-08 19:51:57.000000 malclient-upgraded-1.4a1/malclient/Datamodels/pagination.py
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)       77 2022-11-08 19:51:57.000000 malclient-upgraded-1.4a1/malclient/__init__.py
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     8757 2023-05-25 23:44:42.000000 malclient-upgraded-1.4a1/malclient/anime.py
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     3336 2022-11-08 19:51:57.000000 malclient-upgraded-1.4a1/malclient/boards.py
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     7808 2023-05-25 22:05:50.000000 malclient-upgraded-1.4a1/malclient/client.py
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     2068 2023-01-22 22:26:02.000000 malclient-upgraded-1.4a1/malclient/exceptions.py
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     3849 2022-11-22 20:46:54.000000 malclient-upgraded-1.4a1/malclient/manga.py
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)    12218 2022-11-22 20:47:13.000000 malclient-upgraded-1.4a1/malclient/my_list.py
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     3581 2023-01-22 22:26:40.000000 malclient-upgraded-1.4a1/malclient/request_handler.py
+drwxrwxrwx   0 gruzin    (1000) gruzin    (1000)        0 2023-05-25 23:50:41.893636 malclient-upgraded-1.4a1/malclient_upgraded.egg-info/
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     4655 2023-05-25 23:50:41.000000 malclient-upgraded-1.4a1/malclient_upgraded.egg-info/PKG-INFO
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)      594 2023-05-25 23:50:41.000000 malclient-upgraded-1.4a1/malclient_upgraded.egg-info/SOURCES.txt
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)        1 2023-05-25 23:50:41.000000 malclient-upgraded-1.4a1/malclient_upgraded.egg-info/dependency_links.txt
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)       18 2023-05-25 23:50:41.000000 malclient-upgraded-1.4a1/malclient_upgraded.egg-info/requires.txt
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)       10 2023-05-25 23:50:41.000000 malclient-upgraded-1.4a1/malclient_upgraded.egg-info/top_level.txt
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)      148 2022-11-08 15:30:53.000000 malclient-upgraded-1.4a1/pyproject.toml
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)       79 2023-05-25 23:50:41.895674 malclient-upgraded-1.4a1/setup.cfg
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)      889 2023-05-25 23:46:38.000000 malclient-upgraded-1.4a1/setup.py
```

### Comparing `malclient-upgraded-1.3.4a0/LICENSE` & `malclient-upgraded-1.4a1/LICENSE`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2021 ModerNews
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
+Copyright (c) 2021 ModerNews
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

### Comparing `malclient-upgraded-1.3.4a0/PKG-INFO` & `malclient-upgraded-1.4a1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: malclient-upgraded
-Version: 1.3.4a0
+Version: 1.4a1
 Summary: Modified and rewritten using modern models version of James Fotherby malclient
 Home-page: https://github.com/ModerNews/MAL-API-Client-Upgraded
 Author: ModerNews
 Author-email: polski.gruzin.biz@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://mal-api-client-upgraded.readthedocs.io
 Platform: UNKNOWN
@@ -22,15 +22,14 @@
 ![Read the Docs](https://img.shields.io/readthedocs/mal-api-client-upgraded?style=for-the-badge&color=3EB049)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/malclient-upgraded?style=for-the-badge&color=3EB049) </br>
 A third party object-oriented python3 client library for MyAnimeList's official REST API.
 Originally created by [@JFryy](https://github.com/JFryy/MAL-API-Client), dropped around 2 years ago, picked up and rewritten by ModerNews to fit more modern standards and new REST API functions.
 
 ## Documentation
 Unsure what to do? [Check out our documentation](https://mal-api-client-upgraded.readthedocs.io) </br>
-There will be quick guide coming up soon as well!
 
 ## Installation
 **Python 3.9 or newer required**, this is due to changes in type hinting guidelines, for more info regarding this issue read [PEP 585](https://peps.python.org/pep-0585/)  
 Install the latest stable version from [PyPI](https://pypi.org/project/malclient-upgraded/)  
 `pip install malclient-upgraded`  
 
 Or current unstable version directly from GitHub:  
@@ -109,15 +108,14 @@
 print(repr(anime))
 
 # Update anime List based off of search results
 anime = client.search_anime("Monogatari", limit=1)
 ```
 
 ### Most Imoprtant To-Do's
-- [ ] Rewrite boards (currently disabled)
 - [ ] Implement additional search endpoint
 
 ### Useful resources
 - [MAL auth guide](https://myanimelist.net/blog.php?eid=835707)
 - [Unofficial API Discord](https://discord.gg/XqzqDkzuFx)
 - [Official MAL API Club](https://myanimelist.net/clubs.php?cid=13727)
```

### Comparing `malclient-upgraded-1.3.4a0/README.md` & `malclient-upgraded-1.4a1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,109 +1,107 @@
-# MAL-API-Client-Upgraded
-
-![PyPI](https://img.shields.io/pypi/v/malclient-upgraded?logo=myanimelist&style=for-the-badge)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/malclient-upgraded?logo=python&logoColor=%23ffd43b&style=for-the-badge)
-![PyPI - License](https://img.shields.io/pypi/l/malclient-upgraded?style=for-the-badge&color=3EB049) </br>
-![Read the Docs](https://img.shields.io/readthedocs/mal-api-client-upgraded?style=for-the-badge&color=3EB049)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/malclient-upgraded?style=for-the-badge&color=3EB049) </br>
-A third party object-oriented python3 client library for MyAnimeList's official REST API.
-Originally created by [@JFryy](https://github.com/JFryy/MAL-API-Client), dropped around 2 years ago, picked up and rewritten by ModerNews to fit more modern standards and new REST API functions.
-
-## Documentation
-Unsure what to do? [Check out our documentation](https://mal-api-client-upgraded.readthedocs.io) </br>
-There will be quick guide coming up soon as well!
-
-## Installation
-**Python 3.9 or newer required**, this is due to changes in type hinting guidelines, for more info regarding this issue read [PEP 585](https://peps.python.org/pep-0585/)  
-Install the latest stable version from [PyPI](https://pypi.org/project/malclient-upgraded/)  
-`pip install malclient-upgraded`  
-
-Or current unstable version directly from GitHub:  
-`pip install git+https://github.com/ModerNews/MAL-API-Client-Upgraded`
-
-
-## Authentication
-Client library uses OAuth2 authorization, all you need to do is register your app [here](https://myanimelist.net/apiconfig).
-Main auth requires access token:
-
-```python
-import malclient
-
-malclient.client(access_token=token)
-```
-
-Alternatively can authenticate using your client ID
-
-```python
-import malclient
-
-malclient.client(client_id=id)
-```
-
-You can generate token old-fashioned way using [this tutorial](https://myanimelist.net/blog.php?eid=835707)  
-Or you can use function implemented in API
-
-```python
-import malclient
-
-print(malclient.generate_token("<YOUR_CLIENT_ID>", "<YOUR_CLIENT_SECRET>"))
-```
-
-Although remember to call it only once and, then use the token generated this way, optionally with `Client.refresh_bearer_token` method  
-
-As mentioned previously, if you're scared that your token will time out you can also utilize `Client.refresh_bearer_token` function
-
-```python
-client.refresh_bearer_token(
-          client_id="<your-client-id>",
-          client_secret="<your-client-secret>",
-          refresh_token="<your-refresh-token>")
-```
-
-For any other issues regarding authentication, [please refer to the following guide](https://myanimelist.net/blog.php?eid=835707).
-
-## Quick Start Examples
-I contained some examples of usage of this wrapper, note that all responses are converted to python objects using pydantic
-
-```python
-import malclient
-
-# nsfw filter is enabled by default, although it's recommended to disable it if your results are missing titles, 
-#  you can also enable/disable it for every query individually 
-client = malclient.Client(access_token="<your-access-token>", nsfw=True)
-
-# search anime, returns list
-anime = client.search_anime("cowboy", limit=20)
-for item in anime:
-    # prints only titles
-    print(item)
-    # prints all attributes of object
-    print(repr(item))
-    
-# search anime, returns list
-manga = client.search_manga("Monogatari", limit=20)
-for item in manga:
-    # prints only titles
-    print(manga)
-    # prints all attributes of object
-    print(repr(manga))
-
-# Get individual anime by ID
-anime = client.get_anime_details(1)
-print(anime)
-print(repr(anime))
-
-# Update anime List based off of search results
-anime = client.search_anime("Monogatari", limit=1)
-```
-
-### Most Imoprtant To-Do's
-- [ ] Rewrite boards (currently disabled)
-- [ ] Implement additional search endpoint
-
-### Useful resources
-- [MAL auth guide](https://myanimelist.net/blog.php?eid=835707)
-- [Unofficial API Discord](https://discord.gg/XqzqDkzuFx)
-- [Official MAL API Club](https://myanimelist.net/clubs.php?cid=13727)
-
-## P.S. 
-If anything bugs you, you can always reach me out at discord Gruzin#0911 as well
+# MAL-API-Client-Upgraded
+
+![PyPI](https://img.shields.io/pypi/v/malclient-upgraded?logo=myanimelist&style=for-the-badge)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/malclient-upgraded?logo=python&logoColor=%23ffd43b&style=for-the-badge)
+![PyPI - License](https://img.shields.io/pypi/l/malclient-upgraded?style=for-the-badge&color=3EB049) </br>
+![Read the Docs](https://img.shields.io/readthedocs/mal-api-client-upgraded?style=for-the-badge&color=3EB049)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/malclient-upgraded?style=for-the-badge&color=3EB049) </br>
+A third party object-oriented python3 client library for MyAnimeList's official REST API.
+Originally created by [@JFryy](https://github.com/JFryy/MAL-API-Client), dropped around 2 years ago, picked up and rewritten by ModerNews to fit more modern standards and new REST API functions.
+
+## Documentation
+Unsure what to do? [Check out our documentation](https://mal-api-client-upgraded.readthedocs.io) </br>
+
+## Installation
+**Python 3.9 or newer required**, this is due to changes in type hinting guidelines, for more info regarding this issue read [PEP 585](https://peps.python.org/pep-0585/)  
+Install the latest stable version from [PyPI](https://pypi.org/project/malclient-upgraded/)  
+`pip install malclient-upgraded`  
+
+Or current unstable version directly from GitHub:  
+`pip install git+https://github.com/ModerNews/MAL-API-Client-Upgraded`
+
+
+## Authentication
+Client library uses OAuth2 authorization, all you need to do is register your app [here](https://myanimelist.net/apiconfig).
+Main auth requires access token:
+
+```python
+import malclient
+
+malclient.client(access_token=token)
+```
+
+Alternatively can authenticate using your client ID
+
+```python
+import malclient
+
+malclient.client(client_id=id)
+```
+
+You can generate token old-fashioned way using [this tutorial](https://myanimelist.net/blog.php?eid=835707)  
+Or you can use function implemented in API
+
+```python
+import malclient
+
+print(malclient.generate_token("<YOUR_CLIENT_ID>", "<YOUR_CLIENT_SECRET>"))
+```
+
+Although remember to call it only once and, then use the token generated this way, optionally with `Client.refresh_bearer_token` method  
+
+As mentioned previously, if you're scared that your token will time out you can also utilize `Client.refresh_bearer_token` function
+
+```python
+client.refresh_bearer_token(
+          client_id="<your-client-id>",
+          client_secret="<your-client-secret>",
+          refresh_token="<your-refresh-token>")
+```
+
+For any other issues regarding authentication, [please refer to the following guide](https://myanimelist.net/blog.php?eid=835707).
+
+## Quick Start Examples
+I contained some examples of usage of this wrapper, note that all responses are converted to python objects using pydantic
+
+```python
+import malclient
+
+# nsfw filter is enabled by default, although it's recommended to disable it if your results are missing titles, 
+#  you can also enable/disable it for every query individually 
+client = malclient.Client(access_token="<your-access-token>", nsfw=True)
+
+# search anime, returns list
+anime = client.search_anime("cowboy", limit=20)
+for item in anime:
+    # prints only titles
+    print(item)
+    # prints all attributes of object
+    print(repr(item))
+    
+# search anime, returns list
+manga = client.search_manga("Monogatari", limit=20)
+for item in manga:
+    # prints only titles
+    print(manga)
+    # prints all attributes of object
+    print(repr(manga))
+
+# Get individual anime by ID
+anime = client.get_anime_details(1)
+print(anime)
+print(repr(anime))
+
+# Update anime List based off of search results
+anime = client.search_anime("Monogatari", limit=1)
+```
+
+### Most Imoprtant To-Do's
+- [ ] Implement additional search endpoint
+
+### Useful resources
+- [MAL auth guide](https://myanimelist.net/blog.php?eid=835707)
+- [Unofficial API Discord](https://discord.gg/XqzqDkzuFx)
+- [Official MAL API Club](https://myanimelist.net/clubs.php?cid=13727)
+
+## P.S. 
+If anything bugs you, you can always reach me out at discord Gruzin#0911 as well
```

### Comparing `malclient-upgraded-1.3.4a0/malclient/Datamodels/enums.py` & `malclient-upgraded-1.4a1/malclient/Datamodels/enums.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,300 +1,300 @@
-from __future__ import annotations
-from enum import Enum
-
-__all__ = ['Nsfw', 'RelationType', 'Rating', 'Season', 'AnimeType', 'AnimeStatus', 'AnimeSource', 'MangaType',
-           'MangaStatus', 'MangaRankingType', 'AnimeRankingType', 'SeasonalAnimeSorting', "MyAnimeListSorting",
-           "MyMangaListSorting"]
-
-
-class Nsfw(Enum):
-    """
-
-    Enumerator representing nsfw stages:
-
-    * **WHITE** - White
-    * **GRAY** - Gray
-    * **BLACK** - Black
-    """
-    WHITE = 'white'
-    GRAY = 'gray'
-    BLACK = 'black'
-
-
-class RelationType(Enum):
-    """
-
-    Enumerator representing possible relation types between anime and/or manga:
-
-    * **SEQUEL** - Sequel
-    * **PREQUEL** - Prequel
-    * **ALT_SETTING** - Alternative Setting
-    * **ALT_VERSION** - Alternative Version
-    * **SIDE_STORY** - Side Story
-    * **PARENT_STORY** - Parent Story
-    * **SUMMARY** - Summary
-    * **FULL_STORY** - Full Story
-    * **SPIN_OFF** - Spin-Off
-    * **CHARACTER** - Character
-    * **OTHER** - Other
-    """
-    SEQUEL = "sequel"
-    PREQUEL = "prequel"
-    ALT_SETTING = "alternative_setting"
-    ALT_VERSION = "alternative_version"
-    SIDE_STORY = "side_story"
-    PARENT_STORY = "parent_story"
-    SUMMARY = "summary"
-    FULL_STORY = "full_story"
-    SPIN_OFF = 'spin_off'
-    CHARACTER = 'character'
-    OTHER = 'other'
-
-
-class AnimeRankingType(Enum):
-    """
-
-    Representation of possible values for anime ranking type
-
-    * **ALL** - Top Anime Series
-    * **AIRING** - Top Airing Anime
-    * **UPCOMING** - Top Upcoming Anime
-    * **TV** - Top TV Anime Series
-    * **OVA** - Top OVA Anime Series
-    * **MOVIE** - Top Anime Movies
-    * **SPECIAL** - Top Anime Specials
-    * **POPULAR** - Top Anime by Popularity
-    * **FAVORITE** - Top Favorite Anime
-    """
-    ALL = 'all'
-    AIRING = 'airing'
-    UPCOMING = 'upcoming'
-    TV = 'tv'
-    OVA = 'ova'
-    MOVIE = 'movie'
-    SPECIAL = 'special'
-    POPULAR = 'bypopularity'
-    FAVORITE = 'favorite'
-
-
-class MangaRankingType(Enum):
-    """
-
-    Representation of possible values for manga ranking type
-
-    * **ALL** - All
-    * **MANGA** - Top Manga
-    * **NOVELS** - Top Novels
-    * **ONE_SHOTS** - Top One Shot Manga
-    * **DOUJIN** - Top Doujinshi
-    * **MANHWA** - Top Manhwa
-    * **MANHUA** - Top Manhua
-    * **POPULAR** - Most popular
-    * **FAVORITE** - Most Favorited
-    """
-    ALL = 'all'
-    MANGA = 'manga'
-    NOVELS = 'novels'
-    ONE_SHOTS = 'oneshots'
-    DOUJIN = 'doujin'
-    MANHWA = 'manhwa'
-    MANHUA = 'manhua'
-    POPULAR = 'bypopularity'
-    FAVORITE = 'favorite'
-
-
-class SeasonalAnimeSorting(Enum):
-    """
-
-    Representation of seasonal anime sorting
-
-    * **SCORE** - Sorted by score
-    * **USER_NUM** - Sorted by number of users in list
-    """
-    SCORE = "anime_score"
-    USER_NUM = "anime_num_list_users"
-
-
-class MyAnimeListSorting(Enum):
-    """
-
-    Sorting options for User Anime List
-
-    * **LIST_SCORE** - Sorted by score given by user
-    * **LAST_UPDATE** - Sorted by most recently updated
-    * **TITLE** - Sorted by title
-    * **START_DATE** - Sorted by broadcast start date
-    * **ID** - Sorted by ID
-    """
-    LIST_SCORE = 'list_score'
-    LAST_UPDATE = 'list_updated_at'
-    TITLE = "anime_title"
-    START_DATE = "anime_start_date"
-    # ID = "anime_id"
-
-
-class MyMangaListSorting(Enum):
-    """
-
-    Sorting options for User Manga List
-
-    * **LIST_SCORE** - Sorted by score given by user
-    * **LAST_UPDATE** - Sorted by most recently updated
-    * **TITLE** - Sorted by title
-    * **START_DATE** - Sorted by series start date
-    * **ID** - Sorted by manga ID
-    """
-    LIST_SCORE = 'list_score'
-    LAST_UPDATE = 'list_updated_at'
-    TITLE = "manga_title"
-    START_DATE = "manga_start_date"
-    # ID = "manga_id"
-
-
-class Rating(Enum):
-    """
-
-    Rating of shows provided by myanimelist:
-
-    * **G** - All Ages
-    * **PG** - Children
-    * **PG_13** - Teens 13 and Older
-    * **R** - 17+ (violence & profanity)
-    * **RR** - Profanity & Mild Nudity
-    * **Rx** - Hentai
-    """
-    G = 'g'
-    PG = 'pg'
-    PG_13 = 'pg_13'
-    R = 'r'
-    RR = 'r+'
-    Rx = 'rx'
-
-
-class Season(Enum):
-    WINTER = 'winter'
-    SPRING = 'spring'
-    SUMMER = 'summer'
-    FALL = 'fall'
-
-
-class AnimeStatus(Enum):
-    """
-
-    Enumerating representing current anime status
-
-    * **FINISHED** - Finished Airing
-    * **AIRING** - Currently Airing
-    * **NOT_AIRED** - Not Yet Aired
-    """
-    FINISHED = 'finished_airing'
-    AIRING = 'currently_airing'
-    NOT_AIRED = 'not_yet_aired'
-
-
-class MangaStatus(Enum):
-    """
-
-    Enumerating representing current manga status
-
-    * **FINISHED** - Finished
-    * **PUBLISHING** - Currently Publishing
-    * **NOT_PUBLISHED** - Not Yet Published
-    * **ON_HIATUS** - On Break
-    * **DISCONTINUED** - Discontinued
-    """
-    FINISHED = 'finished'
-    PUBLISHING = 'currently_publishing'
-    NOT_PUBLISHED = 'not_yet_published'
-    ON_HIATUS = 'on_hiatus'
-    DISCONTINUED = 'discontinued'
-
-
-class AnimeType(Enum):
-    """
-
-    Enumerator representing anime type:
-
-    * **Unknown**
-    * **TV** - Streamed in Japanese TV
-    * **OVA** - Original Video Animation
-    * **Movie** - Animated Movie
-    * **Special** - Special for an anime
-    * **ONA** - Original Net Anime (f.e. Netflix Originals)
-    * **Music** - Music Anime
-    """
-    UNKNOWN = "unknown"
-    TV = "tv"
-    OVA = 'ova'
-    MOVIE = 'movie'
-    SPECIAL = 'special'
-    ONA = 'ona'
-    MUSIC = 'music'
-
-
-class MangaType(Enum):
-    """
-
-    Enumerator representing type of manga
-
-    * **UNKNOWN** - Unknown
-    * **MANGA** - Manga
-    * **NOVEL** - Novel
-    * **ONE_SHOT** = One-Shot
-    * **DOUJIN** - Self-published Manga
-    * **MANHWA** - Korean comic
-    * **MANHUA** - Chinese comic
-    * **LIGHT_NOVEL** - Light Novel
-    * **OEL** - Original English-Language Manga
-    """
-    UNKNOWN = "unknown"
-    MANGA = "manga"
-    NOVEL = "novel"
-    ONE_SHOT = "one_shot"
-    DOUJIN = "doujinshi"
-    MANHWA = "manhwa"
-    MANHUA = "manhua"
-    OEL = "oel"
-    LIGHT_NOVEL = 'light_novel'
-
-
-class AnimeSource(Enum):
-    """
-
-    Enumerator representing source of anime
-    
-    * **OTHER** - Other
-    * **ORIGINAL** - Original
-    * **MANGA** - Manga
-    * **MANGA_4_KOMA** - 4-Koma, comedic manga format
-    * **WEB_MANGA** - Web Manga
-    * **WEB_NOVEL** - Web Novel
-    * **DIGITAL_MANGA** - Digital Manga
-    * **NOVEL** - Novel
-    * **LIGHT_NOVEL** - Light Novel
-    * **VISUAL_NOVEL** - Text-based video game
-    * **GAME** - Game
-    * **CARD_GAME** - Card Game
-    * **BOOK** - Book
-    * **PICTURE_BOOK** - Picture Book
-    * **RADIO** - Radio
-    * **MUSIC** - Music
-    * **MIXED_MEDIA** - Mixed Media
-
-    """
-    OTHER = "other"
-    ORIGINAL = "original"
-    MANGA = "manga"
-    MANGA_4_KOMA = "4_koma_manga"
-    WEB_MANGA = "web_manga"
-    WEB_NOVEL = "web_novel"
-    DIGITAL_MANGA = "digital_manga"
-    NOVEL = "novel"
-    LIGHT_NOVEL = "light_novel"
-    VISUAL_NOVEL = "visual_novel"
-    GAME = "game"
-    CARD_GAME = "card_game"
-    BOOK = "book"
-    PICTURE_BOOK = "picture_book"
-    RADIO = "radio"
-    MUSIC = "music"
-    MIXED_MEDIA = "mixed_media"
+from __future__ import annotations
+from enum import Enum
+
+__all__ = ['Nsfw', 'RelationType', 'Rating', 'Season', 'AnimeType', 'AnimeStatus', 'AnimeSource', 'MangaType',
+           'MangaStatus', 'MangaRankingType', 'AnimeRankingType', 'SeasonalAnimeSorting', "MyAnimeListSorting",
+           "MyMangaListSorting"]
+
+
+class Nsfw(Enum):
+    """
+
+    Enumerator representing nsfw stages:
+
+    * **WHITE** - White
+    * **GRAY** - Gray
+    * **BLACK** - Black
+    """
+    WHITE = 'white'
+    GRAY = 'gray'
+    BLACK = 'black'
+
+
+class RelationType(Enum):
+    """
+
+    Enumerator representing possible relation types between anime and/or manga:
+
+    * **SEQUEL** - Sequel
+    * **PREQUEL** - Prequel
+    * **ALT_SETTING** - Alternative Setting
+    * **ALT_VERSION** - Alternative Version
+    * **SIDE_STORY** - Side Story
+    * **PARENT_STORY** - Parent Story
+    * **SUMMARY** - Summary
+    * **FULL_STORY** - Full Story
+    * **SPIN_OFF** - Spin-Off
+    * **CHARACTER** - Character
+    * **OTHER** - Other
+    """
+    SEQUEL = "sequel"
+    PREQUEL = "prequel"
+    ALT_SETTING = "alternative_setting"
+    ALT_VERSION = "alternative_version"
+    SIDE_STORY = "side_story"
+    PARENT_STORY = "parent_story"
+    SUMMARY = "summary"
+    FULL_STORY = "full_story"
+    SPIN_OFF = 'spin_off'
+    CHARACTER = 'character'
+    OTHER = 'other'
+
+
+class AnimeRankingType(Enum):
+    """
+
+    Representation of possible values for anime ranking type
+
+    * **ALL** - Top Anime Series
+    * **AIRING** - Top Airing Anime
+    * **UPCOMING** - Top Upcoming Anime
+    * **TV** - Top TV Anime Series
+    * **OVA** - Top OVA Anime Series
+    * **MOVIE** - Top Anime Movies
+    * **SPECIAL** - Top Anime Specials
+    * **POPULAR** - Top Anime by Popularity
+    * **FAVORITE** - Top Favorite Anime
+    """
+    ALL = 'all'
+    AIRING = 'airing'
+    UPCOMING = 'upcoming'
+    TV = 'tv'
+    OVA = 'ova'
+    MOVIE = 'movie'
+    SPECIAL = 'special'
+    POPULAR = 'bypopularity'
+    FAVORITE = 'favorite'
+
+
+class MangaRankingType(Enum):
+    """
+
+    Representation of possible values for manga ranking type
+
+    * **ALL** - All
+    * **MANGA** - Top Manga
+    * **NOVELS** - Top Novels
+    * **ONE_SHOTS** - Top One Shot Manga
+    * **DOUJIN** - Top Doujinshi
+    * **MANHWA** - Top Manhwa
+    * **MANHUA** - Top Manhua
+    * **POPULAR** - Most popular
+    * **FAVORITE** - Most Favorited
+    """
+    ALL = 'all'
+    MANGA = 'manga'
+    NOVELS = 'novels'
+    ONE_SHOTS = 'oneshots'
+    DOUJIN = 'doujin'
+    MANHWA = 'manhwa'
+    MANHUA = 'manhua'
+    POPULAR = 'bypopularity'
+    FAVORITE = 'favorite'
+
+
+class SeasonalAnimeSorting(Enum):
+    """
+
+    Representation of seasonal anime sorting
+
+    * **SCORE** - Sorted by score
+    * **USER_NUM** - Sorted by number of users in list
+    """
+    SCORE = "anime_score"
+    USER_NUM = "anime_num_list_users"
+
+
+class MyAnimeListSorting(Enum):
+    """
+
+    Sorting options for User Anime List
+
+    * **LIST_SCORE** - Sorted by score given by user
+    * **LAST_UPDATE** - Sorted by most recently updated
+    * **TITLE** - Sorted by title
+    * **START_DATE** - Sorted by broadcast start date
+    * **ID** - Sorted by ID
+    """
+    LIST_SCORE = 'list_score'
+    LAST_UPDATE = 'list_updated_at'
+    TITLE = "anime_title"
+    START_DATE = "anime_start_date"
+    # ID = "anime_id"
+
+
+class MyMangaListSorting(Enum):
+    """
+
+    Sorting options for User Manga List
+
+    * **LIST_SCORE** - Sorted by score given by user
+    * **LAST_UPDATE** - Sorted by most recently updated
+    * **TITLE** - Sorted by title
+    * **START_DATE** - Sorted by series start date
+    * **ID** - Sorted by manga ID
+    """
+    LIST_SCORE = 'list_score'
+    LAST_UPDATE = 'list_updated_at'
+    TITLE = "manga_title"
+    START_DATE = "manga_start_date"
+    # ID = "manga_id"
+
+
+class Rating(Enum):
+    """
+
+    Rating of shows provided by myanimelist:
+
+    * **G** - All Ages
+    * **PG** - Children
+    * **PG_13** - Teens 13 and Older
+    * **R** - 17+ (violence & profanity)
+    * **RR** - Profanity & Mild Nudity
+    * **Rx** - Hentai
+    """
+    G = 'g'
+    PG = 'pg'
+    PG_13 = 'pg_13'
+    R = 'r'
+    RR = 'r+'
+    Rx = 'rx'
+
+
+class Season(Enum):
+    WINTER = 'winter'
+    SPRING = 'spring'
+    SUMMER = 'summer'
+    FALL = 'fall'
+
+
+class AnimeStatus(Enum):
+    """
+
+    Enumerating representing current anime status
+
+    * **FINISHED** - Finished Airing
+    * **AIRING** - Currently Airing
+    * **NOT_AIRED** - Not Yet Aired
+    """
+    FINISHED = 'finished_airing'
+    AIRING = 'currently_airing'
+    NOT_AIRED = 'not_yet_aired'
+
+
+class MangaStatus(Enum):
+    """
+
+    Enumerating representing current manga status
+
+    * **FINISHED** - Finished
+    * **PUBLISHING** - Currently Publishing
+    * **NOT_PUBLISHED** - Not Yet Published
+    * **ON_HIATUS** - On Break
+    * **DISCONTINUED** - Discontinued
+    """
+    FINISHED = 'finished'
+    PUBLISHING = 'currently_publishing'
+    NOT_PUBLISHED = 'not_yet_published'
+    ON_HIATUS = 'on_hiatus'
+    DISCONTINUED = 'discontinued'
+
+
+class AnimeType(Enum):
+    """
+
+    Enumerator representing anime type:
+
+    * **Unknown**
+    * **TV** - Streamed in Japanese TV
+    * **OVA** - Original Video Animation
+    * **Movie** - Animated Movie
+    * **Special** - Special for an anime
+    * **ONA** - Original Net Anime (f.e. Netflix Originals)
+    * **Music** - Music Anime
+    """
+    UNKNOWN = "unknown"
+    TV = "tv"
+    OVA = 'ova'
+    MOVIE = 'movie'
+    SPECIAL = 'special'
+    ONA = 'ona'
+    MUSIC = 'music'
+
+
+class MangaType(Enum):
+    """
+
+    Enumerator representing type of manga
+
+    * **UNKNOWN** - Unknown
+    * **MANGA** - Manga
+    * **NOVEL** - Novel
+    * **ONE_SHOT** = One-Shot
+    * **DOUJIN** - Self-published Manga
+    * **MANHWA** - Korean comic
+    * **MANHUA** - Chinese comic
+    * **LIGHT_NOVEL** - Light Novel
+    * **OEL** - Original English-Language Manga
+    """
+    UNKNOWN = "unknown"
+    MANGA = "manga"
+    NOVEL = "novel"
+    ONE_SHOT = "one_shot"
+    DOUJIN = "doujinshi"
+    MANHWA = "manhwa"
+    MANHUA = "manhua"
+    OEL = "oel"
+    LIGHT_NOVEL = 'light_novel'
+
+
+class AnimeSource(Enum):
+    """
+
+    Enumerator representing source of anime
+    
+    * **OTHER** - Other
+    * **ORIGINAL** - Original
+    * **MANGA** - Manga
+    * **MANGA_4_KOMA** - 4-Koma, comedic manga format
+    * **WEB_MANGA** - Web Manga
+    * **WEB_NOVEL** - Web Novel
+    * **DIGITAL_MANGA** - Digital Manga
+    * **NOVEL** - Novel
+    * **LIGHT_NOVEL** - Light Novel
+    * **VISUAL_NOVEL** - Text-based video game
+    * **GAME** - Game
+    * **CARD_GAME** - Card Game
+    * **BOOK** - Book
+    * **PICTURE_BOOK** - Picture Book
+    * **RADIO** - Radio
+    * **MUSIC** - Music
+    * **MIXED_MEDIA** - Mixed Media
+
+    """
+    OTHER = "other"
+    ORIGINAL = "original"
+    MANGA = "manga"
+    MANGA_4_KOMA = "4_koma_manga"
+    WEB_MANGA = "web_manga"
+    WEB_NOVEL = "web_novel"
+    DIGITAL_MANGA = "digital_manga"
+    NOVEL = "novel"
+    LIGHT_NOVEL = "light_novel"
+    VISUAL_NOVEL = "visual_novel"
+    GAME = "game"
+    CARD_GAME = "card_game"
+    BOOK = "book"
+    PICTURE_BOOK = "picture_book"
+    RADIO = "radio"
+    MUSIC = "music"
+    MIXED_MEDIA = "mixed_media"
```

### Comparing `malclient-upgraded-1.3.4a0/malclient/Datamodels/fields.py` & `malclient-upgraded-1.4a1/malclient/Datamodels/fields.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,367 +1,388 @@
-from types import MethodType, MethodWrapperType, BuiltinFunctionType
-from typing import Union
-
-__all__ = ['Fields', 'AuthorFields', 'ListStatusFields', 'UserFields']
-
-
-class FieldsBase(object):
-    """
-    Base class for all Field classes
-    """
-    def __init__(self, **kwargs):
-        pass
-
-    def __eq__(self, other):
-        if type(self) != type(other):
-            return False
-        else:
-            for field in dir(self):
-                if type(self.__getattribute__(field)) not in (MethodType, MethodWrapperType, BuiltinFunctionType):
-                    if self.__getattribute__(field) != other.__getattribute__(field):
-                        return False
-                else:
-                    continue
-        return True
-
-    def __repr__(self):
-        """
-        Returns string representation of dictionary containing all Fields
-        """
-        return str(self.__dict__)
-
-    def to_payload(self):
-        """
-        Generates query string for fields parameter
-        """
-        fields = []
-        for field, value in self.__dict__.items():
-            if isinstance(value, FieldsBase):
-                if value == value.empty():
-                    continue
-                else:
-                    fields.append(field[1:] + '{' + str(",".join([key for key, state in value.__dict__.items() if state])) + '}')
-            elif value is True:
-                fields.append(field)
-        return ','.join(fields)
-
-    def _generate_subclass(self, r_type, kwargs, key):
-        return r_type(**kwargs.get(key)) if isinstance(kwargs.get(key), dict) else kwargs.get(key) if isinstance(
-            kwargs.get(key), r_type) else False if kwargs.get(key) is not True else r_type()
-
-    @classmethod
-    def from_list(cls, field_list: list[str]):
-        """
-        Generates fields object based of list of fields
-        """
-        return cls(**{field: True for field in field_list})
-
-    @classmethod
-    def all(cls):
-        """
-        Generates fields object containing all fields possible
-        """
-        return cls.from_list(dir(cls()))
-
-    @classmethod
-    def empty(cls):
-        """
-        Generates empty fields object
-        Might be overridden by some classes, which have parameters set to True by default
-        """
-        return cls()
-
-
-class Fields(FieldsBase):
-    """
-    Object containing all fields possible for anime and manga
-    num_favorites, opening_themes, ending_themes are not documented by MAL
-    """
-    def __init__(self, **kwargs):
-        # general
-        self.id: bool = kwargs.get('id', True)
-        self.title: bool = kwargs.get('title', True)
-        self.main_picture: bool = kwargs.get('main_picture', True)
-        self.alternative_titles: bool = kwargs.get('alternative_titles', False)
-        self.start_date: bool = kwargs.get('start_date', False)
-        self.end_date: bool = kwargs.get('end_date', False)
-        self.synopsis: bool = kwargs.get('synopsis', False)
-        self.mean: bool = kwargs.get('mean', False)
-        self.rank: bool = kwargs.get('rank', False)
-        self.popularity: bool = kwargs.get('popularity', False)
-        self.num_list_users: bool = kwargs.get('num_list_users', False)
-        self.num_scoring_users: bool = kwargs.get('num_scoring_users', False)
-        self.updated_at: bool = kwargs.get('updated_at', False)
-        self.genres: bool = kwargs.get('genres', False)
-        # self.my_list_status: bool = kwargs.get('my_list_status', False)
-        self._my_list_status: ListStatusFields = self._generate_subclass(ListStatusFields, kwargs, 'my_list_status')
-        self.pictures: bool = kwargs.get('pictures', False)
-        self.background: bool = kwargs.get('background', False)
-        self._related_anime: bool = self._generate_subclass(Fields, kwargs, 'related_anime')
-        self._related_manga: bool = self._generate_subclass(Fields, kwargs, 'related_manga')
-        self._recommendations: bool = self._generate_subclass(Fields, kwargs, 'recommendations')
-        self.nsfw: bool = kwargs.get('nsfw', False)
-        self.created_at: bool = kwargs.get('created_at', False)
-        self.media_type: bool = kwargs.get('media_type', False)
-        self.status: bool = kwargs.get('status', False)
-        self.num_favorites: bool = kwargs.get('num_favorites', False)
-
-        # anime related
-        self.num_episodes: bool = kwargs.get('num_episodes', False)
-        self.start_season: bool = kwargs.get('start_season', False)
-        self.broadcast: bool = kwargs.get('broadcast', False)
-        self.source: bool = kwargs.get('source', False)
-        self.average_episode_duration: bool = kwargs.get('average_episode_duration', False)
-        self.rating: bool = kwargs.get('rating', False)
-        self.studios: bool = kwargs.get('studios', False)
-        self.opening_themes: bool = kwargs.get('opening_themes', False)
-        self.ending_themes: bool = kwargs.get('ending_themes', False)
-        self.statistics: bool = kwargs.get('statistics', False)
-        self.videos: bool = kwargs.get('videos', False)
-
-        # manga related
-        self.num_volumes: bool = kwargs.get('num_volumes', False)
-        self.num_chapters: bool = kwargs.get('num_chapters', False)
-        self._authors: Union[AuthorFields, bool] = self._generate_subclass(AuthorFields, kwargs, 'authors')
-        self.serialization: bool = kwargs.get('serialization', False)
-
-        # endpoint specific
-        self._list_status: Union[ListStatusFields, bool] = self._generate_subclass(ListStatusFields, kwargs, 'list_status')
-        # self._list_status: bool = kwargs.get('ranking', False)
-
-    @property
-    def authors(self):
-        return self._authors
-
-    @authors.setter
-    def authors(self, value):
-        self._authors = self._generate_subclass(AuthorFields, {'authors': value}, 'authors')
-
-    @property
-    def list_status(self):
-        return self._list_status
-
-    @list_status.setter
-    def list_status(self, value):
-        self._list_status = self._generate_subclass(ListStatusFields, {'list_status': value}, 'list_status')
-
-    @property
-    def related_anime(self):
-        return self._related_anime
-
-    @related_anime.setter
-    def related_anime(self, value):
-        self._related_anime = self._generate_subclass(Fields, {'related_anime': value}, 'related_anime')
-
-    @property
-    def related_manga(self):
-        return self._related_manga
-
-    @related_manga.setter
-    def related_manga(self, value):
-        self._related_manga = self._generate_subclass(Fields, {'related_manga': value}, 'related_manga')
-
-    @property
-    def recommendations(self):
-        return self._recommendations
-
-    @recommendations.setter
-    def recommendations(self, value):
-        self._recommendations = self._generate_subclass(Fields, {'recommendations': value}, 'recommendations')
-
-    @property
-    def my_list_status(self):
-        return self._my_list_status
-
-    @my_list_status.setter
-    def my_list_status(self, value):
-        self._my_list_status: ListStatusFields = self._generate_subclass(ListStatusFields, {'my_list_status': value}, 'my_list_status')
-
-    @classmethod
-    def empty(cls):
-        return cls(id=False, title=False, main_picture=False)
-
-    @classmethod
-    def node(cls):
-        """
-        Generates Fields object containing only parameters taken by node
-        """
-        return cls().from_list(['id', 'title', 'main_picture'])
-
-    @classmethod
-    def anime(cls):
-        """
-        Generates Fields object containing all parameters taken by anime
-        """
-        return cls().from_list(["id",
-                                "title",
-                                "main_picture",
-                                "alternative_titles",
-                                "start_date",
-                                "end_date",
-                                "synopsis",
-                                "mean",
-                                "rank",
-                                "popularity",
-                                "num_list_users",
-                                "num_scoring_users",
-                                "nsfw",
-                                "created_at",
-                                "updated_at",
-                                "media_type",
-                                "status",
-                                "genres",
-                                "my_list_status",
-                                "num_episodes",
-                                "start_season",
-                                "broadcast",
-                                "source",
-                                "average_episode_duration",
-                                "rating",
-                                "pictures",
-                                "background",
-                                "related_anime",
-                                "related_manga",
-                                "recommendations",
-                                "studios",
-                                "opening_theme",
-                                'ending_theme',
-                                'videos',])
-
-    @classmethod
-    def manga(cls):
-        """
-        Generates Fields object containing all parameters taken by manga
-        """
-        return cls(id=True,
-                   title=True,
-                   main_picture=True,
-                   alternative_titles=True,
-                   start_date=True,
-                   end_date=True,
-                   synopsis=True,
-                   mean=True,
-                   rank=True,
-                   popularity=True,
-                   num_list_users=True,
-                   num_scoring_users=True,
-                   nsfw=True,
-                   created_at=True,
-                   updated_at=True,
-                   media_type=True,
-                   status=True,
-                   genres=True,
-                   my_list_status=True,
-                   num_volumes=True,
-                   num_chapters=True,
-                   authors=True,
-                   pictures=True,
-                   background=True,
-                   related_anime=True,
-                   related_manga=True,
-                   recommendations=True,
-                   serialization=True)
-
-
-# class RecursiveFieldFields(Fields):
-#
-#
-#
-class AuthorFields(FieldsBase):
-    """
-    Helper fields class containing info about manga author
-    """
-    def __init__(self, **kwargs):
-        self.first_name: bool = kwargs.get('first_name', True)
-        self.last_name: bool = kwargs.get('last_name', True)
-
-    @classmethod
-    def empty(cls):
-        return cls(first_name=False, last_name=False)
-
-
-class ListStatusFields(FieldsBase):
-    """
-    Helper fields class containing precise data for my_list_status
-    """
-    def __init__(self, **kwargs):
-        self.priority: bool = kwargs.get('priority', False)
-        self.tags: bool = kwargs.get('tags', False)
-        self.comments: bool = kwargs.get('comments', False)
-
-        self.num_times_reread: bool = kwargs.get('num_times_reread', False)
-        self.reread_value: bool = kwargs.get('reread_value', False)
-
-        self.num_times_rewatched: bool = kwargs.get('num_times_rewatched', False)
-        self.rewatch_value: bool = kwargs.get('rewatch_value', False)
-
-        # DEPRECATED FIELDS - Always present in request
-        # self.score: bool = kwargs.get('score', True)
-        # self.status: bool = kwargs.get('status', True)
-        # self.updated_at: bool = kwargs.get('updated_at', True)
-        # self.start_date: bool = kwargs.get('start_date', False)
-        # self.finish_date: bool = kwargs.get('finish_date', False)
-        # self.is_rereading: bool = kwargs.get('is_rereading', False)
-        # self.num_chapters_read: bool = kwargs.get('num_chapters_read', False)
-        # self.num_volumes_read: bool = kwargs.get('num_volumes_read', False)
-        # self.num_episodes_watched: bool = kwargs.get('num_episodes_watched', False)
-        # self.is_rewatching: bool = kwargs.get('is_rewatching', False)
-
-    @classmethod
-    def empty(cls):
-        return cls(score=False, status=False, updated_at=False)
-
-
-    @classmethod
-    def manga_full(cls):
-        """
-        All fields for manga list status
-        """
-        return cls.from_list(['priority', 'tags', 'comments', 'num_times_reread', 'reread_value'])
-
-    @classmethod
-    def anime_full(cls):
-        """
-        All fields for anime list status
-        """
-        return cls.from_list(['priority', 'tags', 'comments', 'num_times_rewatched', 'rewatch_value'])
-
-
-class UserFields(FieldsBase):
-    def __init__(self, **kwargs):
-        self.id: bool = kwargs.get("id", True)
-        self.name: bool = kwargs.get("name", True)
-        self.picture: bool = kwargs.get("picture", True)
-        self.gender: bool = kwargs.get("gender", True)
-        self.birthday: bool = kwargs.get("birthday", False)
-        self.location: bool = kwargs.get("location", True)
-        self.joined_at: bool = kwargs.get("joined_at", True)
-        self.anime_statistics: bool = kwargs.get("anime_statistics", True)
-        self.time_zone: bool = kwargs.get("time_zone", False)
-        self.is_supporter: bool = kwargs.get("is_supporter", False)
-
-    @classmethod
-    def basic(cls):
-        return cls(id=True,
-                   name=True,
-                   picture=True,
-                   anime_statistics=True)
-
-
-# Deprecated - This serves no purpose, you can't specify fields for this parameter
-# class AnimeStatisticsFields(FieldsBase):
-#     def __init__(self, **kwargs):
-#         self.num_items_watching: bool = kwargs.get("num_items_watching", False)
-#         self.num_items_completed: bool = kwargs.get("num_items_completed", False)
-#         self.num_items_on_hold: bool = kwargs.get("num_items_on_hold", False)
-#         self.num_items_dropped: bool = kwargs.get("num_items_dropped", False)
-#         self.num_items_plan_to_watch: bool = kwargs.get("num_items_plan_to_watch", False)
-#         self.num_items: bool = kwargs.get("num_items", False)
-#         self.num_days_watched: bool = kwargs.get("num_days_watched", False)
-#         self.num_days_watching: bool = kwargs.get("num_days_watching", False)
-#         self.num_days_completed: bool = kwargs.get("num_days_completed", False)
-#         self.num_days_on_hold: bool = kwargs.get("num_days_on_hold", False)
-#         self.num_days_dropped: bool = kwargs.get("num_days_dropped", False)
-#         self.num_days: bool = kwargs.get("num_days", False)
-#         self.num_episodes: bool = kwargs.get("num_episodes", False)
-#         self.num_times_rewatched: bool = kwargs.get("num_times_rewatched", False)
-#         self.mean_score: bool = kwargs.get("mean_score", False)
+from types import MethodType, MethodWrapperType, BuiltinFunctionType
+from typing import Union
+
+__all__ = ['Fields', 'AuthorFields', 'ListStatusFields', 'UserFields', "CharacterFields"]
+
+
+class FieldsBase(object):
+    """
+    Base class for all Field classes
+    """
+    def __init__(self, **kwargs):
+        pass
+
+    def __eq__(self, other):
+        if type(self) != type(other):
+            return False
+        else:
+            for field in dir(self):
+                if type(self.__getattribute__(field)) not in (MethodType, MethodWrapperType, BuiltinFunctionType):
+                    if self.__getattribute__(field) != other.__getattribute__(field):
+                        return False
+                else:
+                    continue
+        return True
+
+    def __repr__(self):
+        """
+        Returns string representation of dictionary containing all Fields
+        """
+        return str(self.__dict__)
+
+    def to_payload(self):
+        """
+        Generates query string for fields parameter
+        """
+        fields = []
+        for field, value in self.__dict__.items():
+            if isinstance(value, FieldsBase):
+                if value == value.empty():
+                    continue
+                else:
+                    fields.append(field[1:] + '{' + str(",".join([key for key, state in value.__dict__.items() if state])) + '}')
+            elif value is True:
+                fields.append(field)
+        return ','.join(fields)
+
+    def _generate_subclass(self, r_type, value):
+        return r_type(**value) if isinstance(value, dict) else value if isinstance(
+            value, r_type) else False if value is not True else r_type()
+
+    @classmethod
+    def from_list(cls, field_list: list[str]):
+        """
+        Generates fields object based of list of fields
+        """
+        return cls(**{field: True for field in field_list})
+
+    @classmethod
+    def all(cls):
+        """
+        Generates fields object containing all fields possible
+        """
+        return cls.from_list(dir(cls()))
+
+    @classmethod
+    def empty(cls):
+        """
+        Generates empty fields object
+        Might be overridden by some classes, which have parameters set to True by default
+        """
+        return cls()
+
+
+class Fields(FieldsBase):
+    """
+    Object containing all fields possible for anime and manga
+    num_favorites, opening_themes, ending_themes are not documented by MAL
+    """
+    def __init__(self, **kwargs):
+        # general
+        self.id: bool = kwargs.get('id', True)
+        self.title: bool = kwargs.get('title', True)
+        self.main_picture: bool = kwargs.get('main_picture', True)
+        self.alternative_titles: bool = kwargs.get('alternative_titles', False)
+        self.start_date: bool = kwargs.get('start_date', False)
+        self.end_date: bool = kwargs.get('end_date', False)
+        self.synopsis: bool = kwargs.get('synopsis', False)
+        self.mean: bool = kwargs.get('mean', False)
+        self.rank: bool = kwargs.get('rank', False)
+        self.popularity: bool = kwargs.get('popularity', False)
+        self.num_list_users: bool = kwargs.get('num_list_users', False)
+        self.num_scoring_users: bool = kwargs.get('num_scoring_users', False)
+        self.updated_at: bool = kwargs.get('updated_at', False)
+        self.genres: bool = kwargs.get('genres', False)
+        # self.my_list_status: bool = kwargs.get('my_list_status', False)
+        self._my_list_status: ListStatusFields = self._generate_subclass(ListStatusFields, kwargs.get('my_list_status', False))
+        self.pictures: bool = kwargs.get('pictures', False)
+        self.background: bool = kwargs.get('background', False)
+        self._related_anime: bool = self._generate_subclass(Fields, kwargs.get('related_anime', False))
+        self._related_manga: bool = self._generate_subclass(Fields, kwargs.get('related_manga', False))
+        self._recommendations: bool = self._generate_subclass(Fields, kwargs.get('recommendations', False))
+        self.nsfw: bool = kwargs.get('nsfw', False)
+        self.created_at: bool = kwargs.get('created_at', False)
+        self.media_type: bool = kwargs.get('media_type', False)
+        self.status: bool = kwargs.get('status', False)
+        self.num_favorites: bool = kwargs.get('num_favorites', False)
+
+        # anime related
+        self.num_episodes: bool = kwargs.get('num_episodes', False)
+        self.start_season: bool = kwargs.get('start_season', False)
+        self.broadcast: bool = kwargs.get('broadcast', False)
+        self.source: bool = kwargs.get('source', False)
+        self.average_episode_duration: bool = kwargs.get('average_episode_duration', False)
+        self.rating: bool = kwargs.get('rating', False)
+        self.studios: bool = kwargs.get('studios', False)
+        self.opening_themes: bool = kwargs.get('opening_themes', False)
+        self.ending_themes: bool = kwargs.get('ending_themes', False)
+        self.statistics: bool = kwargs.get('statistics', False)
+        self.videos: bool = kwargs.get('videos', False)
+
+        # manga related
+        self.num_volumes: bool = kwargs.get('num_volumes', False)
+        self.num_chapters: bool = kwargs.get('num_chapters', False)
+        self._authors: Union[AuthorFields, bool] = self._generate_subclass(AuthorFields, kwargs.get('authors', False))
+        self.serialization: bool = kwargs.get('serialization', False)
+
+        # endpoint specific
+        self._list_status: Union[ListStatusFields, bool] = self._generate_subclass(ListStatusFields, kwargs.get('list_status'))
+        # self._list_status: bool = kwargs.get('ranking', False)
+
+    @property
+    def authors(self):
+        return self._authors
+
+    @authors.setter
+    def authors(self, value):
+        self._authors = self._generate_subclass(AuthorFields, value)
+
+    @property
+    def list_status(self):
+        return self._list_status
+
+    @list_status.setter
+    def list_status(self, value):
+        self._list_status = self._generate_subclass(ListStatusFields, value)
+
+    @property
+    def related_anime(self):
+        return self._related_anime
+
+    @related_anime.setter
+    def related_anime(self, value):
+        self._related_anime = self._generate_subclass(Fields, value)
+
+    @property
+    def related_manga(self):
+        return self._related_manga
+
+    @related_manga.setter
+    def related_manga(self, value):
+        self._related_manga = self._generate_subclass(Fields, value)
+
+    @property
+    def recommendations(self):
+        return self._recommendations
+
+    @recommendations.setter
+    def recommendations(self, value):
+        self._recommendations = self._generate_subclass(Fields, value)
+
+    @property
+    def my_list_status(self):
+        return self._my_list_status
+
+    @my_list_status.setter
+    def my_list_status(self, value):
+        self._my_list_status: ListStatusFields = self._generate_subclass(ListStatusFields, value)
+
+    @classmethod
+    def empty(cls):
+        return cls(id=False, title=False, main_picture=False)
+
+    @classmethod
+    def node(cls):
+        """
+        Generates Fields object containing only parameters taken by node
+        """
+        return cls().from_list(['id', 'title', 'main_picture'])
+
+    @classmethod
+    def anime(cls):
+        """
+        Generates Fields object containing all parameters taken by anime
+        """
+        return cls().from_list(["id",
+                                "title",
+                                "main_picture",
+                                "alternative_titles",
+                                "start_date",
+                                "end_date",
+                                "synopsis",
+                                "mean",
+                                "rank",
+                                "popularity",
+                                "num_list_users",
+                                "num_scoring_users",
+                                "nsfw",
+                                "created_at",
+                                "updated_at",
+                                "media_type",
+                                "status",
+                                "genres",
+                                "my_list_status",
+                                "num_episodes",
+                                "start_season",
+                                "broadcast",
+                                "source",
+                                "average_episode_duration",
+                                "rating",
+                                "pictures",
+                                "background",
+                                "related_anime",
+                                "related_manga",
+                                "recommendations",
+                                "studios",
+                                "opening_theme",
+                                'ending_theme',
+                                'videos',])
+
+    @classmethod
+    def manga(cls):
+        """
+        Generates Fields object containing all parameters taken by manga
+        """
+        return cls(id=True,
+                   title=True,
+                   main_picture=True,
+                   alternative_titles=True,
+                   start_date=True,
+                   end_date=True,
+                   synopsis=True,
+                   mean=True,
+                   rank=True,
+                   popularity=True,
+                   num_list_users=True,
+                   num_scoring_users=True,
+                   nsfw=True,
+                   created_at=True,
+                   updated_at=True,
+                   media_type=True,
+                   status=True,
+                   genres=True,
+                   my_list_status=True,
+                   num_volumes=True,
+                   num_chapters=True,
+                   authors=True,
+                   pictures=True,
+                   background=True,
+                   related_anime=True,
+                   related_manga=True,
+                   recommendations=True,
+                   serialization=True)
+
+
+# class RecursiveFieldFields(Fields):
+#
+#
+#
+class AuthorFields(FieldsBase):
+    """
+    Helper fields class containing info about manga author
+    """
+    def __init__(self, **kwargs):
+        self.first_name: bool = kwargs.get('first_name', True)
+        self.last_name: bool = kwargs.get('last_name', True)
+
+    @classmethod
+    def empty(cls):
+        return cls(first_name=False, last_name=False)
+
+
+class ListStatusFields(FieldsBase):
+    """
+    Helper fields class containing precise data for my_list_status
+    """
+    def __init__(self, **kwargs):
+        self.priority: bool = kwargs.get('priority', False)
+        self.tags: bool = kwargs.get('tags', False)
+        self.comments: bool = kwargs.get('comments', False)
+
+        self.num_times_reread: bool = kwargs.get('num_times_reread', False)
+        self.reread_value: bool = kwargs.get('reread_value', False)
+
+        self.num_times_rewatched: bool = kwargs.get('num_times_rewatched', False)
+        self.rewatch_value: bool = kwargs.get('rewatch_value', False)
+
+        # DEPRECATED FIELDS - Always present in request
+        # self.score: bool = kwargs.get('score', True)
+        # self.status: bool = kwargs.get('status', True)
+        # self.updated_at: bool = kwargs.get('updated_at', True)
+        # self.start_date: bool = kwargs.get('start_date', False)
+        # self.finish_date: bool = kwargs.get('finish_date', False)
+        # self.is_rereading: bool = kwargs.get('is_rereading', False)
+        # self.num_chapters_read: bool = kwargs.get('num_chapters_read', False)
+        # self.num_volumes_read: bool = kwargs.get('num_volumes_read', False)
+        # self.num_episodes_watched: bool = kwargs.get('num_episodes_watched', False)
+        # self.is_rewatching: bool = kwargs.get('is_rewatching', False)
+
+    @classmethod
+    def empty(cls):
+        return cls(score=False, status=False, updated_at=False)
+
+
+    @classmethod
+    def manga_full(cls):
+        """
+        All fields for manga list status
+        """
+        return cls.from_list(['priority', 'tags', 'comments', 'num_times_reread', 'reread_value'])
+
+    @classmethod
+    def anime_full(cls):
+        """
+        All fields for anime list status
+        """
+        return cls.from_list(['priority', 'tags', 'comments', 'num_times_rewatched', 'rewatch_value'])
+
+
+class UserFields(FieldsBase):
+    def __init__(self, **kwargs):
+        self.id: bool = kwargs.get("id", True)
+        self.name: bool = kwargs.get("name", True)
+        self.picture: bool = kwargs.get("picture", True)
+        self.gender: bool = kwargs.get("gender", True)
+        self.birthday: bool = kwargs.get("birthday", False)
+        self.location: bool = kwargs.get("location", True)
+        self.joined_at: bool = kwargs.get("joined_at", True)
+        self.anime_statistics: bool = kwargs.get("anime_statistics", True)
+        self.time_zone: bool = kwargs.get("time_zone", False)
+        self.is_supporter: bool = kwargs.get("is_supporter", False)
+
+    @classmethod
+    def basic(cls):
+        return cls(id=True,
+                   name=True,
+                   picture=True,
+                   anime_statistics=True)
+
+
+class CharacterFields(FieldsBase):
+    def __init__(self, **kwargs):
+        self.id: bool = kwargs.get("id", True)
+        self.role: bool = kwargs.get("role", True)
+        self.first_name: bool = kwargs.get("first_name", False)
+        self.last_name: bool = kwargs.get("last_name", False)
+        self.alternative_name: bool = kwargs.get("alternative_name", False)
+        self.main_picture: bool = kwargs.get("main_picture", False)
+        self.biography: bool = kwargs.get("biography", False)
+        self.pictures: bool = kwargs.get("pictures", False)
+        self._animeography: Fields = self._generate_subclass(Fields, kwargs.get("animeography", False))
+
+    @property
+    def animeography(self) -> Fields:
+        return self._animeography
+
+    @animeography.setter
+    def animeography(self, value: Fields):
+        self._animeography: Fields = self._generate_subclass(Fields, value)
+
+
+# Deprecated - This serves no purpose, you can't specify fields for this parameter
+# class AnimeStatisticsFields(FieldsBase):
+#     def __init__(self, **kwargs):
+#         self.num_items_watching: bool = kwargs.get("num_items_watching", False)
+#         self.num_items_completed: bool = kwargs.get("num_items_completed", False)
+#         self.num_items_on_hold: bool = kwargs.get("num_items_on_hold", False)
+#         self.num_items_dropped: bool = kwargs.get("num_items_dropped", False)
+#         self.num_items_plan_to_watch: bool = kwargs.get("num_items_plan_to_watch", False)
+#         self.num_items: bool = kwargs.get("num_items", False)
+#         self.num_days_watched: bool = kwargs.get("num_days_watched", False)
+#         self.num_days_watching: bool = kwargs.get("num_days_watching", False)
+#         self.num_days_completed: bool = kwargs.get("num_days_completed", False)
+#         self.num_days_on_hold: bool = kwargs.get("num_days_on_hold", False)
+#         self.num_days_dropped: bool = kwargs.get("num_days_dropped", False)
+#         self.num_days: bool = kwargs.get("num_days", False)
+#         self.num_episodes: bool = kwargs.get("num_episodes", False)
+#         self.num_times_rewatched: bool = kwargs.get("num_times_rewatched", False)
+#         self.mean_score: bool = kwargs.get("mean_score", False)
```

### Comparing `malclient-upgraded-1.3.4a0/malclient/anime.py` & `malclient-upgraded-1.4a1/malclient/anime.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,162 +1,197 @@
-from __future__ import annotations
-from typing import Optional, Literal, Union
-
-from .Datamodels import Fields, AnimeObject, Node, Season, PagedResult, AnimeRankingType, SeasonalAnimeSorting
-from .exceptions import MainAuthRequiredError
-
-__all__ = ["Anime"]
-
-
-class Anime:
-    def __init__(self):
-        return
-
-    def get_anime_details(self, anime_id: int) -> AnimeObject:
-        """
-
-        Get full info about anime with provided id
-
-        :param int anime_id: id on https://myanimelist.net
-
-        :returns: AnimeObject for requested id
-        :rtype: AnimeObject
-        """
-        uri = f'anime/{str(anime_id)}'
-        params = {'fields': Fields.anime().to_payload()}
-        data = self._api_handler.call(uri, params=params)
-        return AnimeObject(**data)
-
-    def get_anime_fields(self, anime_id: int, fields: Fields) -> AnimeObject:
-        """
-
-        Get specific fields from MAL anime entry with provided id
-
-        :param int anime_id: id on https://myanimelist.net
-        :param Fields fields: Fields returned alongside results
-
-        :returns: AnimeObject for requested id
-        :rtype: AnimeObject
-        """
-        uri = f'anime/{anime_id}'
-        params = {'fields': fields.to_payload()}
-        data = self._api_handler.call(uri, params=params)
-        return AnimeObject(**data)
-
-    def search_anime(self, keyword: str, *, limit: int = 20, nsfw: Optional[bool] = None, fields: Fields = Fields.node()) -> Union[PagedResult[Node], PagedResult[AnimeObject]]:
-        """
-        Lookup anime with keyword phrase on https://myanimelist.net
-
-        :param str keyword: string to look by
-        :param Fields fields: Fields returned alongside results
-        :param int limit: number of queries returned
-        :param bool nsfw: boolean enabling/disabling nsfw filter
-
-        :returns: list of lookup results with pagination support
-        :rtype: PagedResult
-        """
-        if nsfw is None:
-            nsfw = self.nsfw
-        uri = 'anime'
-        params = {
-            "q": keyword,
-            'limit': limit,
-            'fields': fields.to_payload(),
-            'nsfw': nsfw
-        }
-        temp = self._api_handler.call(uri=uri, params=params)
-        r_class = Node if fields == Fields.node() else AnimeObject
-        return PagedResult([r_class(**anime) for anime in temp["data"]], temp['paging'])
-
-    def get_anime_ranking(self, *, ranking_type: Union[AnimeRankingType, str] = AnimeRankingType.ALL, fields: Fields = Fields.node(), limit: int = 50, offset: int = 0) -> Union[PagedResult[Node], PagedResult[AnimeObject]]:
-        """
-        Gets list of anime from MyAnimeList rankings
-
-        :param AnimeRankingType ranking_type: [Optional] Name of ranking from which you want list to be fetched, default to Top Anime
-        :param Fields fields: Fields returned alongside results
-        :param int limit: [Optional] Number of ranking entries to fetch, 50 by default
-        :param int offset: [Optional] Position from which ranking fetch will start
-
-        :return: List of entries fetched from MyAnimeList with paging support
-        :rtype: PagedResult
-        """
-        if isinstance(ranking_type, str):
-            try:
-                ranking_type = AnimeRankingType(ranking_type.lower())
-            except ValueError:
-                raise ValueError(f"ranking_type can't be '{ranking_type}'")
-        uri = 'anime/ranking'
-        params = {
-            "ranking_type": ranking_type.value,
-            "fields": fields.to_payload(),
-            "limit": limit,
-            'offset': offset,
-        }
-        temp = self._api_handler.call(uri=uri, params=params)
-        r_class = Node if fields == Fields.node() else AnimeObject
-        return PagedResult([r_class(**anime) for anime in temp["data"]], temp['paging'])
-
-    SeasonT = Union[Season, Literal['winter', 'spring', 'summer', 'autumn']]
-
-    def get_seasonal_anime(self, season: SeasonT, year: int, *, sort: Union[SeasonalAnimeSorting, str] = SeasonalAnimeSorting.SCORE, fields: Fields = Fields.anime(), limit: int = 50, offset: int = 0, nsfw: bool = None) -> Union[PagedResult[Node], PagedResult[AnimeObject]]:
-        """
-        Gets list of anime from specified season
-
-        :param SeasonT season: Season of year to fetch
-        :param Fields fields: Fields returned alongside results
-        :param int year: Year to fetch
-        :param SeasonalAnimeSorting sort: Sorting method for query, default to Score
-        :param int limit: Number of series to fetch, 50 by default
-        :param int offset: Position from which search results will be presented
-        :param bool nsfw: If set to True results with nsfw grade 'gray' and 'black' will also be fetched, if omitted it will be inherited from Client class
-
-        :return: List of entries fetched from MyAnimeList with paging support
-        :rtype: PagedResult
-        """
-        if isinstance(sort, str):
-            try:
-                sort = SeasonalAnimeSorting(sort.lower())
-            except ValueError:
-                raise ValueError(f"sort can't be '{sort}'")
-
-        if isinstance(season, str):
-            try:
-                season = Season(season.lower())
-            except ValueError:
-                raise ValueError(f"season can't be '{season}'")
-
-        uri = f'anime/season/{year}/{season.value}'
-
-        params = {
-            "sort": sort.value.lower(),
-            "limit": limit,
-            "fields": fields.to_payload(),
-            'offset': offset,
-            "nsfw": nsfw if nsfw is not None else self.nsfw
-        }
-        temp = self._api_handler.call(uri=uri, params=params)
-        r_class = Node if fields == Fields.node() else AnimeObject
-        return PagedResult([r_class(**anime) for anime in temp["data"]], temp['paging'])
-
-    def get_suggested_anime(self, *, fields: Fields = Fields.node(), limit: int = 20, offset: int = 0, nsfw: bool = None) -> Union[PagedResult[Node], PagedResult[AnimeObject]]:
-        """
-        Gets list of suggested anime suggested for user
-
-        :param Fields fields: Fields returned alongside results
-        :param int limit: number of queries returned
-        :param int offset: Position from which search results will be presented
-        :param bool nsfw: If set to True results with nsfw grade 'gray' and 'black' will also be fetched, if omitted it will be inherited from Client class
-
-        :return: List of entries fetched from MyAnimeList with paging support
-        :rtype: PagedResult[None]
-        """
-        if not self.authorized:
-            raise MainAuthRequiredError()
-        uri = 'anime/suggestions'
-        params = {"limit": limit,
-                  "offset": offset,
-                  "fields": fields.to_payload(),
-                  "nsfw": nsfw if nsfw is not None else self.nsfw}
-
-        temp = self._api_handler.call(uri=uri, params=params)
-        r_class = Node if fields == Fields.node() else AnimeObject
-        return PagedResult([r_class(**anime) for anime in temp["data"]], temp['paging'])
+from __future__ import annotations
+from typing import Optional, Literal, Union
+
+from .Datamodels import Fields, AnimeObject, Node, Season, PagedResult, AnimeRankingType, SeasonalAnimeSorting, Character, CharacterFields
+from .exceptions import MainAuthRequiredError
+
+__all__ = ["Anime"]
+
+
+class Anime:
+    def __init__(self):
+        return
+
+    def get_anime_details(self, anime_id: int) -> AnimeObject:
+        """
+
+        Get full info about anime with provided id
+
+        :param int anime_id: id on https://myanimelist.net
+
+        :returns: AnimeObject for requested id
+        :rtype: AnimeObject
+        """
+        uri = f'anime/{str(anime_id)}'
+        params = {'fields': Fields.anime().to_payload()}
+        data = self._api_handler.call(uri, params=params)
+        return AnimeObject(**data)
+
+    def get_anime_fields(self, anime_id: int, fields: Fields) -> AnimeObject:
+        """
+
+        Get specific fields from MAL anime entry with provided id
+
+        :param int anime_id: id on https://myanimelist.net
+        :param Fields fields: Fields returned alongside results
+
+        :returns: AnimeObject for requested id
+        :rtype: AnimeObject
+        """
+        uri = f'anime/{anime_id}'
+        params = {'fields': fields.to_payload()}
+        data = self._api_handler.call(uri, params=params)
+        return AnimeObject(**data)
+
+    def search_anime(self, keyword: str, *, limit: int = 20, nsfw: Optional[bool] = None, fields: Fields = Fields.node()) -> Union[PagedResult[Node], PagedResult[AnimeObject]]:
+        """
+        Lookup anime with keyword phrase on https://myanimelist.net
+
+        :param str keyword: string to look by
+        :param Fields fields: Fields returned alongside results
+        :param int limit: number of queries returned
+        :param bool nsfw: boolean enabling/disabling nsfw filter
+
+        :returns: list of lookup results with pagination support
+        :rtype: PagedResult
+        """
+        if nsfw is None:
+            nsfw = self.nsfw
+        uri = 'anime'
+        params = {
+            "q": keyword,
+            'limit': limit,
+            'fields': fields.to_payload(),
+            'nsfw': nsfw
+        }
+        temp = self._api_handler.call(uri=uri, params=params)
+        r_class = Node if fields == Fields.node() else AnimeObject
+        return PagedResult([r_class(**anime) for anime in temp["data"]], temp['paging'])
+
+    def get_anime_ranking(self, *, ranking_type: Union[AnimeRankingType, str] = AnimeRankingType.ALL, fields: Fields = Fields.node(), limit: int = 50, offset: int = 0) -> Union[PagedResult[Node], PagedResult[AnimeObject]]:
+        """
+        Gets list of anime from MyAnimeList rankings
+
+        :param AnimeRankingType ranking_type: [Optional] Name of ranking from which you want list to be fetched, default to Top Anime
+        :param Fields fields: Fields returned alongside results
+        :param int limit: [Optional] Number of ranking entries to fetch, 50 by default
+        :param int offset: [Optional] Position from which ranking fetch will start
+
+        :return: List of entries fetched from MyAnimeList with paging support
+        :rtype: PagedResult
+        """
+        if isinstance(ranking_type, str):
+            try:
+                ranking_type = AnimeRankingType(ranking_type.lower())
+            except ValueError:
+                raise ValueError(f"ranking_type can't be '{ranking_type}'")
+        uri = 'anime/ranking'
+        params = {
+            "ranking_type": ranking_type.value,
+            "fields": fields.to_payload(),
+            "limit": limit,
+            'offset': offset,
+        }
+        temp = self._api_handler.call(uri=uri, params=params)
+        r_class = Node if fields == Fields.node() else AnimeObject
+        return PagedResult([r_class(**anime) for anime in temp["data"]], temp['paging'])
+
+    SeasonT = Union[Season, Literal['winter', 'spring', 'summer', 'autumn']]
+
+    def get_seasonal_anime(self, season: SeasonT, year: int, *, sort: Union[SeasonalAnimeSorting, str] = SeasonalAnimeSorting.SCORE, fields: Fields = Fields.anime(), limit: int = 50, offset: int = 0, nsfw: bool = None) -> Union[PagedResult[Node], PagedResult[AnimeObject]]:
+        """
+        Gets list of anime from specified season
+
+        :param SeasonT season: Season of year to fetch
+        :param Fields fields: Fields returned alongside results
+        :param int year: Year to fetch
+        :param SeasonalAnimeSorting sort: Sorting method for query, default to Score
+        :param int limit: Number of series to fetch, 50 by default
+        :param int offset: Position from which search results will be presented
+        :param bool nsfw: If set to True results with nsfw grade 'gray' and 'black' will also be fetched, if omitted it will be inherited from Client class
+
+        :return: List of entries fetched from MyAnimeList with paging support
+        :rtype: PagedResult
+        """
+        if isinstance(sort, str):
+            try:
+                sort = SeasonalAnimeSorting(sort.lower())
+            except ValueError:
+                raise ValueError(f"sort can't be '{sort}'")
+
+        if isinstance(season, str):
+            try:
+                season = Season(season.lower())
+            except ValueError:
+                raise ValueError(f"season can't be '{season}'")
+
+        uri = f'anime/season/{year}/{season.value}'
+
+        params = {
+            "sort": sort.value.lower(),
+            "limit": limit,
+            "fields": fields.to_payload(),
+            'offset': offset,
+            "nsfw": nsfw if nsfw is not None else self.nsfw
+        }
+        temp = self._api_handler.call(uri=uri, params=params)
+        r_class = Node if fields == Fields.node() else AnimeObject
+        return PagedResult([r_class(**anime) for anime in temp["data"]], temp['paging'])
+
+    def get_suggested_anime(self, *, fields: Fields = Fields.node(), limit: int = 20, offset: int = 0, nsfw: bool = None) -> Union[PagedResult[Node], PagedResult[AnimeObject]]:
+        """
+        Gets list of suggested anime suggested for user
+
+        :param Fields fields: Fields returned alongside results
+        :param int limit: number of queries returned
+        :param int offset: Position from which search results will be presented
+        :param bool nsfw: If set to True results with nsfw grade 'gray' and 'black' will also be fetched, if omitted it will be inherited from Client class
+
+        :return: List of entries fetched from MyAnimeList with paging support
+        :rtype: PagedResult[None]
+        """
+        if not self.authorized:
+            raise MainAuthRequiredError()
+        uri = 'anime/suggestions'
+        params = {"limit": limit,
+                  "offset": offset,
+                  "fields": fields.to_payload(),
+                  "nsfw": nsfw if nsfw is not None else self.nsfw}
+
+        temp = self._api_handler.call(uri=uri, params=params)
+        r_class = Node if fields == Fields.node() else AnimeObject
+        return PagedResult([r_class(**anime) for anime in temp["data"]], temp['paging'])
+
+    def get_anime_characters(self, anime_id: int, *, fields: CharacterFields = CharacterFields, limit: int = 500, offset: int = 0) -> PagedResult[Character]:
+        """
+        Gets list of characters from specified anime
+
+        :param int anime_id: Id of anime to fetch characters from
+        :param Fields fields: Fields returned alongside results
+        :param int limit: number of queries returned
+        :param int offset: Position from which search results will be presented
+
+        :return: List of entries fetched from MyAnimeList with paging support
+        :rtype: PagedResult[Character]
+        """
+        uri = f'anime/{anime_id}/characters'
+        params = {"limit": limit,
+                  "offset": offset,
+                  "fields": fields}
+
+        temp = self._api_handler.call(uri=uri, params=params)
+        return PagedResult([Character(**character) for character in temp["data"]], temp['paging'])
+
+    def get_character_details(self, character_id: int, *, fields: CharacterFields = CharacterFields.all()) -> Character:
+        """
+        Gets details of specified character
+
+        :param int character_id: Id of character to fetch
+        :param Fields fields: Fields returned alongside results
+
+        :return: List of entries fetched from MyAnimeList with paging support
+        :rtype: PagedResult[Character]
+        """
+        uri = f'characters/{character_id}'
+        params = {"fields": fields}
+
+        return Character(**self._api_handler.call(uri=uri, params=params))
```

### Comparing `malclient-upgraded-1.3.4a0/malclient/boards.py` & `malclient-upgraded-1.4a1/malclient/boards.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-from typing import Literal
-
-from .Datamodels import ForumCategory, ForumTopicDetail, ForumTopic
-from .Datamodels import PagedResult
-
-
-class Boards:
-    def __init__(self):
-        return
-
-    def get_forum_boards(self):
-        """
-
-        Get list of forum boards from MAL
-
-        :returns: List containing all forum boards on MAL
-        :rtype: list[ForumCategory]
-        """
-        uri = 'forum/boards'
-        return [ForumCategory(**data) for data in self._api_handler.call(uri)['categories']]
-        # return self._api_handler.call(uri)
-
-    def get_forum_topic_detail(self, topic_id: int, *, limit: int = 100, offset: int = 0):
-        """
-        Get details about forum topic from MAL
-
-        :param int topic_id: id of topic for which data will be fetched
-        :param int limit: number of posts in topic to fetch
-        :param int offset: number of posts in topic from start to be skipped
-        :returns: Details about forum topic
-        :rtype: ForumTopicDetail
-        """
-        uri = f'forum/topic/{topic_id}'
-        params = {'limit': limit,
-                  'offstet': offset}
-        temp = self._api_handler.call(uri, params=params)
-        return ForumTopicDetail(paging_data=temp['paging'], **temp["data"])
-
-    def get_forum_topics(self, *,
-                         board_id: int = None,
-                         subboard_id: int = None,
-                         limit: int = 100,
-                         offset: int = 0,
-                         sort: Literal["recent"] = "recent",
-                         query: str = None,
-                         topic_user_name: str = None,
-                         user_name: str = None):
-        """
-
-        Get list of topics available on MAL, by board_id, subboard_id, query, topic_user_name or user_name
-        Descriptions of parameters are uncertain as they're missing in official API documentation
-
-        :param int board_id: id of board wanted topics are on
-        :param int subboard_id: id of subboard wanted topics are on
-        :param str query: query by which forum topics will be filtered by
-        :param str topic_user_name: topics created by user with this name
-        :param str user_name: topic in which user with this username took part
-        :param int limit: number of topics to fetch
-        :param int offset: number of topics from start to be skipped
-        :param str sort: sorting method, currently only `recent` is available
-        :returns: List of forum topics matching provided parameters
-        :rtype: PagedResult[ForumTopic]
-        """
-        if not(query or board_id or subboard_id or topic_user_name or user_name):
-            raise AttributeError("You need to provide one of those: q, board_id, subboard_id, topic_user_name, user_name")
-        uri = 'forum/topics'
-        params = {'board_id': board_id,
-                  'subboard_id': subboard_id,
-                  'limit': limit,
-                  'offset': offset,
-                  'sort': sort,
-                  'q': query,
-                  'topic_user_name': topic_user_name,
-                  'user_name': user_name}
-        temp = self._api_handler.call(uri, params=params)
+from typing import Literal
+
+from .Datamodels import ForumCategory, ForumTopicDetail, ForumTopic
+from .Datamodels import PagedResult
+
+
+class Boards:
+    def __init__(self):
+        return
+
+    def get_forum_boards(self):
+        """
+
+        Get list of forum boards from MAL
+
+        :returns: List containing all forum boards on MAL
+        :rtype: list[ForumCategory]
+        """
+        uri = 'forum/boards'
+        return [ForumCategory(**data) for data in self._api_handler.call(uri)['categories']]
+        # return self._api_handler.call(uri)
+
+    def get_forum_topic_detail(self, topic_id: int, *, limit: int = 100, offset: int = 0):
+        """
+        Get details about forum topic from MAL
+
+        :param int topic_id: id of topic for which data will be fetched
+        :param int limit: number of posts in topic to fetch
+        :param int offset: number of posts in topic from start to be skipped
+        :returns: Details about forum topic
+        :rtype: ForumTopicDetail
+        """
+        uri = f'forum/topic/{topic_id}'
+        params = {'limit': limit,
+                  'offstet': offset}
+        temp = self._api_handler.call(uri, params=params)
+        return ForumTopicDetail(paging_data=temp['paging'], **temp["data"])
+
+    def get_forum_topics(self, *,
+                         board_id: int = None,
+                         subboard_id: int = None,
+                         limit: int = 100,
+                         offset: int = 0,
+                         sort: Literal["recent"] = "recent",
+                         query: str = None,
+                         topic_user_name: str = None,
+                         user_name: str = None):
+        """
+
+        Get list of topics available on MAL, by board_id, subboard_id, query, topic_user_name or user_name
+        Descriptions of parameters are uncertain as they're missing in official API documentation
+
+        :param int board_id: id of board wanted topics are on
+        :param int subboard_id: id of subboard wanted topics are on
+        :param str query: query by which forum topics will be filtered by
+        :param str topic_user_name: topics created by user with this name
+        :param str user_name: topic in which user with this username took part
+        :param int limit: number of topics to fetch
+        :param int offset: number of topics from start to be skipped
+        :param str sort: sorting method, currently only `recent` is available
+        :returns: List of forum topics matching provided parameters
+        :rtype: PagedResult[ForumTopic]
+        """
+        if not(query or board_id or subboard_id or topic_user_name or user_name):
+            raise AttributeError("You need to provide one of those: q, board_id, subboard_id, topic_user_name, user_name")
+        uri = 'forum/topics'
+        params = {'board_id': board_id,
+                  'subboard_id': subboard_id,
+                  'limit': limit,
+                  'offset': offset,
+                  'sort': sort,
+                  'q': query,
+                  'topic_user_name': topic_user_name,
+                  'user_name': user_name}
+        temp = self._api_handler.call(uri, params=params)
         return PagedResult([ForumTopic(**topic) for topic in temp['data']], temp['paging'])
```

### Comparing `malclient-upgraded-1.3.4a0/malclient/client.py` & `malclient-upgraded-1.4a1/malclient/client.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,179 +1,179 @@
-import re
-import secrets
-import os
-import datetime
-import logging
-from typing import Optional
-import platform
-
-from .request_handler import APICaller
-from .anime import Anime
-from .my_list import MyList
-from .manga import Manga
-from .exceptions import AuthorizationError
-from .boards import Boards
-
-__all__ = ['Client', 'setup_logging', 'generate_authorization_url', 'fetch_token_schema_2']
-
-
-def generate_authorization_url(client_id: str, *,
-                               code_verifier: Optional[str] = None,
-                               redirect_uri: Optional[str] = None) -> [str, str]:
-    if code_verifier is None:
-        token = secrets.token_urlsafe(100)
-        code_verifier = code_challenge = token[:128]
-
-    assert 48 <= len(code_verifier) <= 128
-
-    authorization_url = f"https://myanimelist.net/v1/oauth2/authorize?response_type=code&client_id={client_id}&state=RequestID42&code_challenge={code_verifier}&code_challenge_method=plain&redirect_uri={redirect_uri}"
-    return authorization_url, code_verifier
-
-
-def fetch_token_schema_2(client_id: str,
-                        client_secret: str,
-                        code_verifier: str,
-                        code: str,
-                        redirect_uri : Optional[str] = None) -> dict[str, str]:
-    """
-
-    Helper function to generate access token **do not use this to refresh token**
-    Function follows MAL auth schema 2
-
-    :ivar str client_id: your client id (available on myanimelist developer page)
-    :ivar str client_secret: your client secret (available on myanimelist developer page)
-    :return: Freshly generated Access Token for your client
-    :rtype: dict[str, str]
-    """
-
-    base_url = "https://myanimelist.net/v1/"
-    uri = "oauth2/token"
-    headers = {'Content-Type': 'application/x-www-form-urlencoded'}
-    api_handler = APICaller(base_url=base_url, headers=headers)
-    data = {
-        "client_id": client_id,
-        "client_secret": client_secret,
-        "code": code,
-        "code_verifier": code_verifier,
-        "grant_type": "authorization_code",
-        'redirect_uri': redirect_uri,
-    }
-    return api_handler.call(uri=uri, method="post", data=data)
-
-# TODO Scheme 1 (Is it even possible)
-# def fetch_token_schema_1(client_id: str,
-#                          )
-
-def setup_logging(*, format: str = None, filename: str = None, log_level: logging = logging.INFO):
-    """
-    This is helper function for setting up request logging, all parameters are optional and function may be executed as is
-    :param str format: Python Logging library format in which each event will be logged
-    :param str filename: filename under which log will be saved, default if malclient_log_{date}.log
-    :param log_level: Messages which are less severe than log-level will be ignored, most request have level INFO
-    """
-    if format is None:
-        format = "%(levelname)s | %(asctime)s | %(message)s"
-    now = datetime.datetime.now()
-    if filename is None:
-        filename = f"malclient_log_{now.strftime('%Y-%m-%d_%H-%M')}.log"
-    logging.basicConfig(filename=filename, level=log_level, format=format)
-
-
-class Client(Anime, Manga, MyList, Boards):
-    """
-
-    Base class for interacting with MyAnimeList REST API
-
-    :ivar client_id: string containing client_id obtained from [client configuration on MAL](https://myanimelist.net/apiconfig)
-    :ivar access_token: string containing access token obtained through OAuth2
-    :ivar refresh_token: string containing refresh token obtained through OAuth2
-    """
-    def __init__(self, *, client_id: str = None, access_token: str = None, refresh_token: str = None, nsfw: bool = False):
-        self.nsfw = nsfw
-        self._base_url = "https://api.myanimelist.net/"
-        self._version = "v2"
-        self._base_url = self._base_url + f'{self._version}/'
-        self._bearer_token = access_token
-        self._client_id = client_id
-        self.refresh_token = refresh_token
-        self.authorized = False
-        self._api_handler = None
-        self.headers = {}
-        self._connect_to_api()
-
-    @classmethod
-    def generate_new_token(cls, client_id: str, client_secret: str, *, code_verifier: str = None, redirect_uri: Optional[str] = None):
-        auth_url, code_verifier = generate_authorization_url(client_id, code_verifier=code_verifier, redirect_uri=redirect_uri)
-        if 'windows' in platform.system().lower():
-            os.system(f"explorer \"{auth_url}\"")
-        elif 'darwin' in platform.system().lower():
-            os.system(f"open \"{auth_url}\"")
-        elif 'linux' in platform.system().lower():
-            os.system(f"xdg-open \"{auth_url}\"")
-        print(f"If opening url failed enter it manually into your browser:\n{auth_url}")
-        code_url = input("Paste url you were redirected to\n")
-        code = re.search(r"(?<=code=)(\w+)", code_url).group()
-
-        data = fetch_token_schema_2(client_id, client_secret, code_verifier, code, redirect_uri)
-        return cls(access_token=data['access_token'], refresh_token=data['refresh_token'])
-
-    def _connect_to_api(self):
-        self.headers = {
-            'Content-Type': 'application/x-www-form-urlencoded',
-        }
-        if self._bearer_token is not None:
-            self.headers['Authorization'] = f'Bearer {self._bearer_token}'
-            self._api_handler = APICaller(base_url=self._base_url,
-                                          headers=self.headers)
-            self.authorized = True
-        elif self._client_id is not None:
-            self.headers['X-MAL-CLIENT-ID'] = self._client_id
-        else:
-            raise AuthorizationError()
-
-        self._api_handler = APICaller(base_url=self._base_url,
-                                      headers=self.headers)
-
-    def refresh_bearer_token(self,
-                             client_id: str,
-                             client_secret: str,
-                             refresh_token: str,
-                             print_response: bool = True) -> None:
-        """
-
-        Function to automatically refresh your clients bearer token (as for now there is no such thing as lifetime token)
-
-        :param str client_id: Your client id number
-        :param str client_secret: Your client secret
-        :param str refresh_token: Your refresh token
-        :param bool print_response: Should the response json be printed or not
-        """
-        base_url = "https://myanimelist.net/v1/"
-        uri = "oauth2/token"
-        headers = {
-            'Authorization': f'Bearer {self._bearer_token}',
-            'Content-Type': 'application/x-www-form-urlencoded',
-            'Authorization': 'basic {}'
-        }
-        api_handler = APICaller(base_url=base_url, headers=headers)
-        data = {
-            "grant_type": "refresh_token",
-            "refresh_token": refresh_token,
-            "client_id": client_id,
-            "client_secret": client_secret
-        }
-
-        # print response json of authentication, reinstantiate caller method.
-        response = api_handler.call(uri=uri, method="post", data=data)
-        if print_response:
-            print("Refreshing token with client id and secret:")
-            print(response)
-        self._bearer_token = response["access_token"]
-        self.refresh_token = response["refresh_token"]
-        self.headers = {
-            'Content-Type': 'application/x-www-form-urlencoded',
-            'Authorization': f'Bearer {response["access_token"]}',
-            'X-MAL-Client-ID': '{}'
-        }
-        self._api_handler = APICaller(base_url=self._base_url,
-                                      headers=self.headers)
-        return
+import re
+import secrets
+import os
+import datetime
+import logging
+from typing import Optional
+import platform
+
+from .request_handler import APICaller
+from .anime import Anime
+from .my_list import MyList
+from .manga import Manga
+from .exceptions import AuthorizationError
+from .boards import Boards
+
+__all__ = ['Client', 'setup_logging', 'generate_authorization_url', 'fetch_token_schema_2']
+
+
+def generate_authorization_url(client_id: str, *,
+                               code_verifier: Optional[str] = None,
+                               redirect_uri: Optional[str] = None) -> [str, str]:
+    if code_verifier is None:
+        token = secrets.token_urlsafe(100)
+        code_verifier = code_challenge = token[:128]
+
+    assert 48 <= len(code_verifier) <= 128
+
+    authorization_url = f"https://myanimelist.net/v1/oauth2/authorize?response_type=code&client_id={client_id}&state=RequestID42&code_challenge={code_verifier}&code_challenge_method=plain&redirect_uri={redirect_uri}"
+    return authorization_url, code_verifier
+
+
+def fetch_token_schema_2(client_id: str,
+                        client_secret: str,
+                        code_verifier: str,
+                        code: str,
+                        redirect_uri : Optional[str] = None) -> dict[str, str]:
+    """
+
+    Helper function to generate access token **do not use this to refresh token**
+    Function follows MAL auth schema 2
+
+    :ivar str client_id: your client id (available on myanimelist developer page)
+    :ivar str client_secret: your client secret (available on myanimelist developer page)
+    :return: Freshly generated Access Token for your client
+    :rtype: dict[str, str]
+    """
+
+    base_url = "https://myanimelist.net/v1/"
+    uri = "oauth2/token"
+    headers = {'Content-Type': 'application/x-www-form-urlencoded'}
+    api_handler = APICaller(base_url=base_url, headers=headers)
+    data = {
+        "client_id": client_id,
+        "client_secret": client_secret,
+        "code": code,
+        "code_verifier": code_verifier,
+        "grant_type": "authorization_code",
+        'redirect_uri': redirect_uri,
+    }
+    return api_handler.call(uri=uri, method="post", data=data)
+
+# TODO Scheme 1 (Is it even possible)
+# def fetch_token_schema_1(client_id: str,
+#                          )
+
+def setup_logging(*, format: str = None, filename: str = None, log_level: logging = logging.INFO):
+    """
+    This is helper function for setting up request logging, all parameters are optional and function may be executed as is
+    :param str format: Python Logging library format in which each event will be logged
+    :param str filename: filename under which log will be saved, default if malclient_log_{date}.log
+    :param log_level: Messages which are less severe than log-level will be ignored, most request have level INFO
+    """
+    if format is None:
+        format = "%(levelname)s | %(asctime)s | %(message)s"
+    now = datetime.datetime.now()
+    if filename is None:
+        filename = f"malclient_log_{now.strftime('%Y-%m-%d_%H-%M')}.log"
+    logging.basicConfig(filename=filename, level=log_level, format=format)
+
+
+class Client(Anime, Manga, MyList, Boards):
+    """
+
+    Base class for interacting with MyAnimeList REST API
+
+    :ivar client_id: string containing client_id obtained from [client configuration on MAL](https://myanimelist.net/apiconfig)
+    :ivar access_token: string containing access token obtained through OAuth2
+    :ivar refresh_token: string containing refresh token obtained through OAuth2
+    """
+    def __init__(self, *, client_id: str = None, access_token: str = None, refresh_token: str = None, nsfw: bool = False):
+        self.nsfw = nsfw
+        self._base_url = "https://api.myanimelist.net/"
+        self._version = "v2"
+        self._base_url = self._base_url + f'{self._version}/'
+        self._bearer_token = access_token
+        self._client_id = client_id
+        self.refresh_token = refresh_token
+        self.authorized = False
+        self._api_handler = None
+        self.headers = {}
+        self._connect_to_api()
+
+    @classmethod
+    def generate_new_token(cls, client_id: str, client_secret: str, *, code_verifier: str = None, redirect_uri: Optional[str] = None):
+        auth_url, code_verifier = generate_authorization_url(client_id, code_verifier=code_verifier, redirect_uri=redirect_uri)
+        if 'windows' in platform.system().lower():
+            os.system(f"explorer \"{auth_url}\"")
+        elif 'darwin' in platform.system().lower():
+            os.system(f"open \"{auth_url}\"")
+        elif 'linux' in platform.system().lower():
+            os.system(f"xdg-open \"{auth_url}\"")
+        print(f"If opening url failed enter it manually into your browser:\n{auth_url}")
+        code_url = input("Paste url you were redirected to\n")
+        code = re.search(r"(?<=code=)(\w+)", code_url).group()
+
+        data = fetch_token_schema_2(client_id, client_secret, code_verifier, code, redirect_uri)
+        return cls(access_token=data['access_token'], refresh_token=data['refresh_token'])
+
+    def _connect_to_api(self):
+        self.headers = {
+            'Content-Type': 'application/x-www-form-urlencoded',
+        }
+        if self._bearer_token is not None:
+            self.headers['Authorization'] = f'Bearer {self._bearer_token}'
+            self._api_handler = APICaller(base_url=self._base_url,
+                                          headers=self.headers)
+            self.authorized = True
+        elif self._client_id is not None:
+            self.headers['X-MAL-CLIENT-ID'] = self._client_id
+        else:
+            raise AuthorizationError()
+
+        self._api_handler = APICaller(base_url=self._base_url,
+                                      headers=self.headers)
+
+    def refresh_bearer_token(self,
+                             client_id: str,
+                             client_secret: str,
+                             refresh_token: str,
+                             print_response: bool = True) -> None:
+        """
+
+        Function to automatically refresh your clients bearer token (as for now there is no such thing as lifetime token)
+
+        :param str client_id: Your client id number
+        :param str client_secret: Your client secret
+        :param str refresh_token: Your refresh token
+        :param bool print_response: Should the response json be printed or not
+        """
+        base_url = "https://myanimelist.net/v1/"
+        uri = "oauth2/token"
+        headers = {
+            'Authorization': f'Bearer {self._bearer_token}',
+            'Content-Type': 'application/x-www-form-urlencoded',
+            'Authorization': 'basic {}'
+        }
+        api_handler = APICaller(base_url=base_url, headers=headers)
+        data = {
+            "grant_type": "refresh_token",
+            "refresh_token": refresh_token,
+            "client_id": client_id,
+            "client_secret": client_secret
+        }
+
+        # print response json of authentication, reinstantiate caller method.
+        response = api_handler.call(uri=uri, method="post", data=data)
+        if print_response:
+            print("Refreshing token with client id and secret:")
+            print(response)
+        self._bearer_token = response["access_token"]
+        self.refresh_token = response["refresh_token"]
+        self.headers = {
+            'Content-Type': 'application/x-www-form-urlencoded',
+            'Authorization': f'Bearer {response["access_token"]}',
+            'X-MAL-Client-ID': '{}'
+        }
+        self._api_handler = APICaller(base_url=self._base_url,
+                                      headers=self.headers)
+        return
```

### Comparing `malclient-upgraded-1.3.4a0/malclient/exceptions.py` & `malclient-upgraded-1.4a1/malclient/exceptions.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-import json
-from typing import Optional
-
-
-class APIException(Exception):
-    """Base exception for API"""
-    def __init__(self, status_code, message, response):
-        self.status_code = status_code
-        self.message = message
-        self.response = response
-
-    def __repr__(self):
-        return self.__str__()
-
-    def __str__(self):
-        return f"{self.status_code} - {self.message}"
-
-
-class AuthorizationError(Exception):
-    """
-    Base for all exceptions raised because of auth problems
-    More info: https://myanimelist.net/apiconfig/references/api/v2#section/Authentication
-    """
-    def __init__(self, message: Optional[str] = None):
-        super().__init__("No valid authorization method, use OAuth2 or Client ID" if message is None else message)
-
-
-class MainAuthRequiredError(AuthorizationError):
-    """
-    Exception indicates that for action you were trying to perform you need main_auth
-    More info: https://myanimelist.net/apiconfig/references/api/v2#section/Authentication
-    """
-    def __init__(self):
-        super().__init__("This endpoint is available only using OAuth2")
-
-
-# Those are helper classes to simplify catching exceptions
-class BadRequest(APIException):
-    """HTTP 400 Bad Request exception"""
-    def __init__(self, response):
-        super().__init__("400 Bad Request", json.loads(response.text).get('message', None), response)
-
-
-class Unauthorized(APIException):
-    """HTTP 401 Unauthorized exception"""
-    def __init__(self, response):
-        super().__init__("401 Unauthorized", json.loads(response.text).get('message', None), response)
-
-
-class Forbidden(APIException):
-    """HTTP 403 Forbidden exception"""
-    def __init__(self, response):
-        super().__init__("403 Forbidden", json.loads(response.text).get('message', None), response)
-
-
-class NotFound(APIException):
-    """HTTP 404 Not Found exception"""
-    def __init__(self, response):
-        super().__init__("404 Not Found", json.loads(response.text).get('message', None), response)
+import json
+from typing import Optional
+
+
+class APIException(Exception):
+    """Base exception for API"""
+    def __init__(self, status_code, message, response):
+        self.status_code = status_code
+        self.message = message
+        self.response = response
+
+    def __repr__(self):
+        return self.__str__()
+
+    def __str__(self):
+        return f"{self.status_code} - {self.message}"
+
+
+class AuthorizationError(Exception):
+    """
+    Base for all exceptions raised because of auth problems
+    More info: https://myanimelist.net/apiconfig/references/api/v2#section/Authentication
+    """
+    def __init__(self, message: Optional[str] = None):
+        super().__init__("No valid authorization method, use OAuth2 or Client ID" if message is None else message)
+
+
+class MainAuthRequiredError(AuthorizationError):
+    """
+    Exception indicates that for action you were trying to perform you need main_auth
+    More info: https://myanimelist.net/apiconfig/references/api/v2#section/Authentication
+    """
+    def __init__(self):
+        super().__init__("This endpoint is available only using OAuth2")
+
+
+# Those are helper classes to simplify catching exceptions
+class BadRequest(APIException):
+    """HTTP 400 Bad Request exception"""
+    def __init__(self, response):
+        super().__init__("400 Bad Request", json.loads(response.text).get('message', None), response)
+
+
+class Unauthorized(APIException):
+    """HTTP 401 Unauthorized exception"""
+    def __init__(self, response):
+        super().__init__("401 Unauthorized", json.loads(response.text).get('message', None), response)
+
+
+class Forbidden(APIException):
+    """HTTP 403 Forbidden exception"""
+    def __init__(self, response):
+        super().__init__("403 Forbidden", json.loads(response.text).get('message', None), response)
+
+
+class NotFound(APIException):
+    """HTTP 404 Not Found exception"""
+    def __init__(self, response):
+        super().__init__("404 Not Found", json.loads(response.text).get('message', None), response)
```

### Comparing `malclient-upgraded-1.3.4a0/malclient/manga.py` & `malclient-upgraded-1.4a1/malclient/manga.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,100 +1,100 @@
-from __future__ import annotations
-
-from typing import Union
-
-from .Datamodels import MangaObject, Node, Fields, PagedResult, MangaRankingType
-
-__all__ = ["Manga"]
-
-
-class Manga:
-    def __init__(self):
-        return
-
-    def search_manga(self, keyword: str, fields: Fields = Fields.node(), limit: int = 20, offset: int = 0, nsfw: bool = None) -> list[Node]:
-        """
-        Lookup manga with keyword phrase on https://myanimelist.net
-
-        :param str keyword: string to look by
-        :param Fields fields: fields that will be returned by API in addition to default ones
-        :param int limit: number of queries returned
-        :param int offset: Position from which search results will be presented
-        :param nsfw: boolean enabling/disabling nsfw filter
-
-        :returns: list of queries matching search keyword
-        :rtype: PagedResult
-        """
-        if nsfw is None:
-            nsfw = self.nsfw
-        uri = 'manga'
-        params = {
-            "q": keyword,
-            "limit": limit,
-            'offset': offset,
-            "fields": fields.to_payload(),
-            'nsfw': nsfw
-        }
-        temp = self._api_handler.call(uri, params=params)
-        r_class = Node if fields == Fields.node() else MangaObject
-        return PagedResult([r_class(**manga) for manga in temp["data"]], temp['paging'])
-
-    def get_manga_details(self, manga_id: int):
-        """
-        Get full info about manga with provided id
-
-        :param int manga_id: id on https://myanimelist.net
-
-        :returns: MangaObject for requested id
-        :rtype: MangaObject
-        """
-        uri = f'manga/{manga_id}'
-        params = {"fields": Fields.manga().to_payload()}
-        data = self._api_handler.call(uri, params=params)
-        return MangaObject(**data)
-
-    def get_manga_fields(self, manga_id: int, fields: Fields) -> MangaObject:
-        """
-
-        Get specific fields from MAL manga entry with provided id
-
-        :param int manga_id: id on https://myanimelist.net
-        :param Fields fields: Fields that will be returned with manga object
-
-        :returns: MangaObject for requested id
-        :rtype: MangaObject
-        """
-        uri = f'anime/{manga_id}'
-        params = {'fields': fields.to_payload()}
-        data = self._api_handler.call(uri, params=params)
-        return MangaObject(**data)
-
-    def get_manga_ranking(self, ranking_type: Union[str, MangaRankingType] = MangaRankingType.MANGA, fields: Fields = Fields.manga(), limit: int = 20, offset: int = 0) -> Union[PagedResult[Node], PagedResult[MangaObject]]:
-        """
-
-        Get current manga ranking from MAL
-
-        :param MangaRankingType ranking_type: type of manga ranking that will be fetched from API, refer to MangaRankingType dataclass for more info
-        :param Fields fields: Fields that will be returned additionally with manga data
-        :param int limit: number of queries returned
-        :param int offset: Position from which search results will be presented
-
-        :returns: List of queries with pagination support
-        :rtype: PagedResult
-        """
-        uri = 'manga/ranking'
-
-        if isinstance(ranking_type, str):
-            try:
-                ranking_type = MangaRankingType(ranking_type)
-            except ValueError:
-                raise ValueError(f"ranking_type can't be '{ranking_type}'")
-
-        params = {
-            "ranking_type": ranking_type.value,
-            "limit": limit,
-            "fields": fields.to_payload(),
-            'offset': offset,
-        }
-        temp = self._api_handler.call(uri, params=params)
-        r_class = Node if fields == Fields.node() else MangaObject
-        return PagedResult([r_class(**manga) for manga in temp["data"]], temp['paging'])
+from __future__ import annotations
+
+from typing import Union
+
+from .Datamodels import MangaObject, Node, Fields, PagedResult, MangaRankingType
+
+__all__ = ["Manga"]
+
+
+class Manga:
+    def __init__(self):
+        return
+
+    def search_manga(self, keyword: str, fields: Fields = Fields.node(), limit: int = 20, offset: int = 0, nsfw: bool = None) -> list[Node]:
+        """
+        Lookup manga with keyword phrase on https://myanimelist.net
+
+        :param str keyword: string to look by
+        :param Fields fields: fields that will be returned by API in addition to default ones
+        :param int limit: number of queries returned
+        :param int offset: Position from which search results will be presented
+        :param nsfw: boolean enabling/disabling nsfw filter
+
+        :returns: list of queries matching search keyword
+        :rtype: PagedResult
+        """
+        if nsfw is None:
+            nsfw = self.nsfw
+        uri = 'manga'
+        params = {
+            "q": keyword,
+            "limit": limit,
+            'offset': offset,
+            "fields": fields.to_payload(),
+            'nsfw': nsfw
+        }
+        temp = self._api_handler.call(uri, params=params)
+        r_class = Node if fields == Fields.node() else MangaObject
+        return PagedResult([r_class(**manga) for manga in temp["data"]], temp['paging'])
+
+    def get_manga_details(self, manga_id: int):
+        """
+        Get full info about manga with provided id
+
+        :param int manga_id: id on https://myanimelist.net
+
+        :returns: MangaObject for requested id
+        :rtype: MangaObject
+        """
+        uri = f'manga/{manga_id}'
+        params = {"fields": Fields.manga().to_payload()}
+        data = self._api_handler.call(uri, params=params)
+        return MangaObject(**data)
+
+    def get_manga_fields(self, manga_id: int, fields: Fields) -> MangaObject:
+        """
+
+        Get specific fields from MAL manga entry with provided id
+
+        :param int manga_id: id on https://myanimelist.net
+        :param Fields fields: Fields that will be returned with manga object
+
+        :returns: MangaObject for requested id
+        :rtype: MangaObject
+        """
+        uri = f'anime/{manga_id}'
+        params = {'fields': fields.to_payload()}
+        data = self._api_handler.call(uri, params=params)
+        return MangaObject(**data)
+
+    def get_manga_ranking(self, ranking_type: Union[str, MangaRankingType] = MangaRankingType.MANGA, fields: Fields = Fields.manga(), limit: int = 20, offset: int = 0) -> Union[PagedResult[Node], PagedResult[MangaObject]]:
+        """
+
+        Get current manga ranking from MAL
+
+        :param MangaRankingType ranking_type: type of manga ranking that will be fetched from API, refer to MangaRankingType dataclass for more info
+        :param Fields fields: Fields that will be returned additionally with manga data
+        :param int limit: number of queries returned
+        :param int offset: Position from which search results will be presented
+
+        :returns: List of queries with pagination support
+        :rtype: PagedResult
+        """
+        uri = 'manga/ranking'
+
+        if isinstance(ranking_type, str):
+            try:
+                ranking_type = MangaRankingType(ranking_type)
+            except ValueError:
+                raise ValueError(f"ranking_type can't be '{ranking_type}'")
+
+        params = {
+            "ranking_type": ranking_type.value,
+            "limit": limit,
+            "fields": fields.to_payload(),
+            'offset': offset,
+        }
+        temp = self._api_handler.call(uri, params=params)
+        r_class = Node if fields == Fields.node() else MangaObject
+        return PagedResult([r_class(**manga) for manga in temp["data"]], temp['paging'])
```

### Comparing `malclient-upgraded-1.3.4a0/malclient/my_list.py` & `malclient-upgraded-1.4a1/malclient/my_list.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,234 +1,234 @@
-import datetime
-from typing import Union, Literal, Optional
-
-from .Datamodels import MyAnimeListSorting, MyMangaListSorting, MyAnimeListStatus, MyMangaListStatus, Fields, UserFields, User, MangaObject, AnimeObject, PagedResult, ListStatusFields
-from .exceptions import MainAuthRequiredError
-
-__all__ = ["MyList"]
-
-
-class MyList:
-
-    def __init__(self):
-        return
-
-    def update_my_anime_list_status(self, anime_id: int, *,
-                                    status: Optional[Literal["watching", "completed", "on_hold", "dropped", "plan_to_watch"]] = None,
-                                    start_date: Optional[datetime.date] = None,
-                                    finish_date: Optional[datetime.date] = None,
-                                    is_rewatching: Optional[bool] = None,
-                                    score: Optional[int] = None,
-                                    num_watched_episodes: Optional[int] = None,
-                                    priority: Optional[int] = None,
-                                    num_times_rewatched: Optional[int] = None,
-                                    rewatch_value: Optional[int] = None,
-                                    tags: Optional[str] = None,
-                                    comments: Optional[str] = None, **kwargs):
-        """
-
-        Updates myanimelist status for a given anime, takes payload as dictionary as argument.
-        Emit fields to not update. Returns updated entry from list.
-
-        :param int anime_id: id of anime you want to update
-        :param Literal["watching", "completed", "on_hold", "dropped", "plan_to_watch"] status: Watching status of series
-        :params datetime.date start_date: Start watching date
-        :params datetime.date finish_date: Finish watching date
-        :param bool is_rewatching: Defines if series is watched multiple times by user
-        :param int score: score in 1 to 10 scale
-        :param int num_watched_episodes: Number of episodes watched by user
-        :param int priority: Priority level to watch this anime
-        :param int num_times_rewatched: Number of how many times you've re-watched this series, this should not include first time you completed this series
-        :param int rewatch_value: How likely are you to re-watch this series
-        :param str tags: Tags you're willing to give to this series
-        :param str comments: Additional comments you'd like to leave under this series
-        :returns: Updated entry
-        :rtype: MyAnimeListStatus
-        """
-        if not self.authorized:
-            raise MainAuthRequiredError()
-        if score is not None:
-            if 0 > score > 10:
-                raise ValueError("Score must be in range 1 - 10")
-        data = {
-            'status': status,
-            'start_date': start_date.strftime('%Y-%m-%d'),
-            'finish_date': finish_date.strftime('%Y-%m-%d'),
-            'is_rewatching': is_rewatching,
-            'score': score,
-            'num_watched_episodes': num_watched_episodes,
-            'priority': priority,
-            'num_times_rewatch': num_times_rewatched,
-            'rewatch_value': rewatch_value,
-            'tags': tags,
-            'comments': comments
-        }
-        uri = f'anime/{anime_id}/my_list_status'
-        return MyAnimeListStatus(**self._api_handler.call(method="patch", uri=uri, data=data | kwargs))
-
-    # need another function for adding manga to list
-    def delete_my_anime_list_status(self, anime_id: int):
-        """
-        Deletes entry from list for given anime
-
-        :params int manga_id: ID number for anime you want to delete
-        """
-        if not self.authorized:
-            raise MainAuthRequiredError()
-        uri = f'anime/{anime_id}/my_list_status'
-        return self._api_handler.call(method="delete", uri=uri)
-
-    def get_user_anime_list(self, username: str ="@me", *,
-                            sort: Union[MyAnimeListSorting, str, None] = None,
-                            status: Optional[str] = None,
-                            limit: int = 100,
-                            offset: int = 0,
-                            list_status_fields: ListStatusFields = True,
-                            fields: Fields = Fields.from_list(['id', 'title', 'main_picture', 'my_list_status']),
-                            nsfw: bool = None):
-        """
-        Fetches anime list for given user
-
-        :params MyAnimeListSorting sort: Method using which entries will be sorted
-        :params str status: Only entries with provided status will be returned
-        :params int limit: Number of entries returned
-        :params int offset: Position starting from which entries will be fetched
-        :params ListStatusFields list_status_fields: Fields returned inside my_list_status field in entry
-        :params Fields fields: Fields returned alongside each entry
-        :param bool nsfw: If set to True results with nsfw grade 'gray' and 'black' will also be fetched, if omitted it will be inherited from Client class
-
-        :returns: List of objects containing manga information for entries on users' manga list
-        :rtype: PagedResult[AnimeObject]
-        """
-        uri = f'users/{username}/animelist'
-        fields.list_status = list_status_fields
-        if not sort:
-            sort = MyAnimeListSorting.LIST_SCORE
-        elif isinstance(sort, str):
-            sort = MyAnimeListSorting(sort.lower())
-
-        params = {
-            "sort": sort.value,
-            "limit": limit,
-            "fields": fields.to_payload(),
-            "status": status,
-            "offset": offset,
-            "nsfw": nsfw if nsfw is not None else self.nsfw
-        }
-        temp = self._api_handler.call(uri=uri, params=params)
-        return PagedResult([AnimeObject(**entry) for entry in temp['data']], temp['paging']) if len(temp['data']) != 0 else None
-
-    def get_user_info(self, user_id: Union[str, int] = "@me", fields: UserFields = UserFields.basic()):
-        """
-        Gets full information about mentioned user, currently you can fetch info only about authenticated user
-
-        :params str user_id: ID of user you want to fetch data for, currently only supports value @me
-        :params UserFields fields: Fields to be fetched alongside main data
-        :returns: Data for authenticated user
-        :rtype: User
-        """
-        if not self.authorized:
-            raise MainAuthRequiredError()
-        uri = f'users/{user_id}'
-        params = {"fields": fields.to_payload()}
-        return User(**self._api_handler.call(uri, params=params))
-
-    def update_my_manga_list_status(self, manga_id, *,
-                                    status: Optional[Literal["reading", "completed", "on_hold", "dropped", "plan_to_read"]] = None,
-                                    start_date: Optional[datetime.date] = None,
-                                    finish_date: Optional[datetime.date] = None,
-                                    is_rereading: Optional[bool] = None,
-                                    score: Optional[int] = None,
-                                    num_volumes_read: Optional[int] = None,
-                                    num_chapters_read: Optional[int] = None,
-                                    priority: Optional[int] = None,
-                                    num_times_reread: Optional[int] = None,
-                                    reread_value: Optional[int] = None,
-                                    tags: Optional[str] = None,
-                                    comments: Optional[str] = None, **kwargs):
-        """
-
-        Updates myanimelist status for a given manga, takes payload as dictionary as argument.
-        Emit fields to not update. Returns updated entry from list.
-
-        :param int manga_id: id of manga you want to update
-        :param Literal["watching", "completed", "on_hold", "dropped", "plan_to_watch"] status: Watching status of series
-        :params datetime.date start_date: Start reading date
-        :params datetime.date finish_date: Finish reading date
-        :param bool is_rereading: Defines if series is read multiple times by user
-        :param int score: score in 1 to 10 scale
-        :param int num_volumes_read: Number of volumes read by user
-        :param int num_chapters_read: Number of chapters read by user
-        :param int priority: Priority level to watch this anime
-        :param int num_times_reread: Number of how many times you've re-read this series, this should not include first time you completed this series
-        :param int reread_value: How likely are you to re-read this series
-        :param str tags: Tags you're willing to give to this series
-        :param str comments: Additional comments you'd like to leave under this series
-        :returns: Updated entry
-        :rtype: MyMangaListStatus
-        """
-        if not self.authorized:
-            raise MainAuthRequiredError()
-        uri = f'manga/{manga_id}/my_list_status'
-        data = {
-            'status': status,
-            'start_date': start_date.strftime('%Y-%m-%d'),
-            'finish_date': finish_date.strftime('%Y-%m-%d'),
-            'is_rereading': is_rereading,
-            'score': score,
-            'num_volumes_read': num_volumes_read,
-            'num_chapters_read': num_chapters_read,
-            'priority': priority,
-            'num_times_reread': num_times_reread,
-            'reread_value': reread_value,
-            'tags': tags,
-            'comments': comments
-        }
-        return MyMangaListStatus(**self._api_handler.call(method="patch", uri=uri, data=data | kwargs))
-
-    def delete_my_manga_list_status(self, manga_id: int):
-        """
-        Deletes entry from list for given manga
-
-        :params int manga_id: ID number for manga you want to delete
-        """
-        if not self.authorized:
-            raise MainAuthRequiredError()
-        uri = f'manga/{manga_id}/my_list_status'
-        return self._api_handler.call(method="delete", uri=uri)
-
-    def get_user_manga_list(self, username: str ="@me", *,
-                            sort: Union[MyMangaListSorting, str] = MyMangaListSorting.LIST_SCORE,
-                            status: Optional[str] = None,
-                            limit: int = 100,
-                            offset: int = 0,
-                            list_status_fields: ListStatusFields = True,
-                            fields: Fields = Fields.from_list(['id', 'title', 'main_picture']),
-                            nsfw: bool = None):
-        """
-        Fetches manga list for given user
-
-        :params MyMangaListSorting sort: Method using which entries will be sorted
-        :params str status: Only entries with provided status will be returned
-        :params int limit: Number of entries returned
-        :params int offset: Position starting from which entries will be fetched
-        :params ListStatusFields list_status_fields: Fields returned inside my_list_status field in entry
-        :params Fields fields: Fields returned alongside each entry
-        :param bool nsfw: If set to True results with nsfw grade 'gray' and 'black' will also be fetched, if omitted it will be inherited from Client class
-
-        :returns: List of objects containing manga information for entries on users manga list
-        :rtype: PagedResult[MangaObject]
-        """
-        uri = f'users/{username}/mangalist'
-        fields.my_list_status = list_status_fields
-        if isinstance(sort, str):
-            sort = MyMangaListSorting(sort.lower())
-        params = {
-            "sort": sort.value,
-            "limit": limit,
-            "fields": fields.to_payload(),
-            "status": status,
-            "offset": offset,
-            "nfsw": nsfw if nsfw is not None else self.nsfw
-        }
-        temp = self._api_handler.call(uri=uri, params=params)
+import datetime
+from typing import Union, Literal, Optional
+
+from .Datamodels import MyAnimeListSorting, MyMangaListSorting, MyAnimeListStatus, MyMangaListStatus, Fields, UserFields, User, MangaObject, AnimeObject, PagedResult, ListStatusFields
+from .exceptions import MainAuthRequiredError
+
+__all__ = ["MyList"]
+
+
+class MyList:
+
+    def __init__(self):
+        return
+
+    def update_my_anime_list_status(self, anime_id: int, *,
+                                    status: Optional[Literal["watching", "completed", "on_hold", "dropped", "plan_to_watch"]] = None,
+                                    start_date: Optional[datetime.date] = None,
+                                    finish_date: Optional[datetime.date] = None,
+                                    is_rewatching: Optional[bool] = None,
+                                    score: Optional[int] = None,
+                                    num_watched_episodes: Optional[int] = None,
+                                    priority: Optional[int] = None,
+                                    num_times_rewatched: Optional[int] = None,
+                                    rewatch_value: Optional[int] = None,
+                                    tags: Optional[str] = None,
+                                    comments: Optional[str] = None, **kwargs):
+        """
+
+        Updates myanimelist status for a given anime, takes payload as dictionary as argument.
+        Emit fields to not update. Returns updated entry from list.
+
+        :param int anime_id: id of anime you want to update
+        :param Literal["watching", "completed", "on_hold", "dropped", "plan_to_watch"] status: Watching status of series
+        :params datetime.date start_date: Start watching date
+        :params datetime.date finish_date: Finish watching date
+        :param bool is_rewatching: Defines if series is watched multiple times by user
+        :param int score: score in 1 to 10 scale
+        :param int num_watched_episodes: Number of episodes watched by user
+        :param int priority: Priority level to watch this anime
+        :param int num_times_rewatched: Number of how many times you've re-watched this series, this should not include first time you completed this series
+        :param int rewatch_value: How likely are you to re-watch this series
+        :param str tags: Tags you're willing to give to this series
+        :param str comments: Additional comments you'd like to leave under this series
+        :returns: Updated entry
+        :rtype: MyAnimeListStatus
+        """
+        if not self.authorized:
+            raise MainAuthRequiredError()
+        if score is not None:
+            if 0 > score > 10:
+                raise ValueError("Score must be in range 1 - 10")
+        data = {
+            'status': status,
+            'start_date': start_date.strftime('%Y-%m-%d'),
+            'finish_date': finish_date.strftime('%Y-%m-%d'),
+            'is_rewatching': is_rewatching,
+            'score': score,
+            'num_watched_episodes': num_watched_episodes,
+            'priority': priority,
+            'num_times_rewatch': num_times_rewatched,
+            'rewatch_value': rewatch_value,
+            'tags': tags,
+            'comments': comments
+        }
+        uri = f'anime/{anime_id}/my_list_status'
+        return MyAnimeListStatus(**self._api_handler.call(method="patch", uri=uri, data=data | kwargs))
+
+    # need another function for adding manga to list
+    def delete_my_anime_list_status(self, anime_id: int):
+        """
+        Deletes entry from list for given anime
+
+        :params int manga_id: ID number for anime you want to delete
+        """
+        if not self.authorized:
+            raise MainAuthRequiredError()
+        uri = f'anime/{anime_id}/my_list_status'
+        return self._api_handler.call(method="delete", uri=uri)
+
+    def get_user_anime_list(self, username: str ="@me", *,
+                            sort: Union[MyAnimeListSorting, str, None] = None,
+                            status: Optional[str] = None,
+                            limit: int = 100,
+                            offset: int = 0,
+                            list_status_fields: ListStatusFields = True,
+                            fields: Fields = Fields.from_list(['id', 'title', 'main_picture', 'my_list_status']),
+                            nsfw: bool = None):
+        """
+        Fetches anime list for given user
+
+        :params MyAnimeListSorting sort: Method using which entries will be sorted
+        :params str status: Only entries with provided status will be returned
+        :params int limit: Number of entries returned
+        :params int offset: Position starting from which entries will be fetched
+        :params ListStatusFields list_status_fields: Fields returned inside my_list_status field in entry
+        :params Fields fields: Fields returned alongside each entry
+        :param bool nsfw: If set to True results with nsfw grade 'gray' and 'black' will also be fetched, if omitted it will be inherited from Client class
+
+        :returns: List of objects containing manga information for entries on users' manga list
+        :rtype: PagedResult[AnimeObject]
+        """
+        uri = f'users/{username}/animelist'
+        fields.list_status = list_status_fields
+        if not sort:
+            sort = MyAnimeListSorting.LIST_SCORE
+        elif isinstance(sort, str):
+            sort = MyAnimeListSorting(sort.lower())
+
+        params = {
+            "sort": sort.value,
+            "limit": limit,
+            "fields": fields.to_payload(),
+            "status": status,
+            "offset": offset,
+            "nsfw": nsfw if nsfw is not None else self.nsfw
+        }
+        temp = self._api_handler.call(uri=uri, params=params)
+        return PagedResult([AnimeObject(**entry) for entry in temp['data']], temp['paging']) if len(temp['data']) != 0 else None
+
+    def get_user_info(self, user_id: Union[str, int] = "@me", fields: UserFields = UserFields.basic()):
+        """
+        Gets full information about mentioned user, currently you can fetch info only about authenticated user
+
+        :params str user_id: ID of user you want to fetch data for, currently only supports value @me
+        :params UserFields fields: Fields to be fetched alongside main data
+        :returns: Data for authenticated user
+        :rtype: User
+        """
+        if not self.authorized:
+            raise MainAuthRequiredError()
+        uri = f'users/{user_id}'
+        params = {"fields": fields.to_payload()}
+        return User(**self._api_handler.call(uri, params=params))
+
+    def update_my_manga_list_status(self, manga_id, *,
+                                    status: Optional[Literal["reading", "completed", "on_hold", "dropped", "plan_to_read"]] = None,
+                                    start_date: Optional[datetime.date] = None,
+                                    finish_date: Optional[datetime.date] = None,
+                                    is_rereading: Optional[bool] = None,
+                                    score: Optional[int] = None,
+                                    num_volumes_read: Optional[int] = None,
+                                    num_chapters_read: Optional[int] = None,
+                                    priority: Optional[int] = None,
+                                    num_times_reread: Optional[int] = None,
+                                    reread_value: Optional[int] = None,
+                                    tags: Optional[str] = None,
+                                    comments: Optional[str] = None, **kwargs):
+        """
+
+        Updates myanimelist status for a given manga, takes payload as dictionary as argument.
+        Emit fields to not update. Returns updated entry from list.
+
+        :param int manga_id: id of manga you want to update
+        :param Literal["watching", "completed", "on_hold", "dropped", "plan_to_watch"] status: Watching status of series
+        :params datetime.date start_date: Start reading date
+        :params datetime.date finish_date: Finish reading date
+        :param bool is_rereading: Defines if series is read multiple times by user
+        :param int score: score in 1 to 10 scale
+        :param int num_volumes_read: Number of volumes read by user
+        :param int num_chapters_read: Number of chapters read by user
+        :param int priority: Priority level to watch this anime
+        :param int num_times_reread: Number of how many times you've re-read this series, this should not include first time you completed this series
+        :param int reread_value: How likely are you to re-read this series
+        :param str tags: Tags you're willing to give to this series
+        :param str comments: Additional comments you'd like to leave under this series
+        :returns: Updated entry
+        :rtype: MyMangaListStatus
+        """
+        if not self.authorized:
+            raise MainAuthRequiredError()
+        uri = f'manga/{manga_id}/my_list_status'
+        data = {
+            'status': status,
+            'start_date': start_date.strftime('%Y-%m-%d'),
+            'finish_date': finish_date.strftime('%Y-%m-%d'),
+            'is_rereading': is_rereading,
+            'score': score,
+            'num_volumes_read': num_volumes_read,
+            'num_chapters_read': num_chapters_read,
+            'priority': priority,
+            'num_times_reread': num_times_reread,
+            'reread_value': reread_value,
+            'tags': tags,
+            'comments': comments
+        }
+        return MyMangaListStatus(**self._api_handler.call(method="patch", uri=uri, data=data | kwargs))
+
+    def delete_my_manga_list_status(self, manga_id: int):
+        """
+        Deletes entry from list for given manga
+
+        :params int manga_id: ID number for manga you want to delete
+        """
+        if not self.authorized:
+            raise MainAuthRequiredError()
+        uri = f'manga/{manga_id}/my_list_status'
+        return self._api_handler.call(method="delete", uri=uri)
+
+    def get_user_manga_list(self, username: str ="@me", *,
+                            sort: Union[MyMangaListSorting, str] = MyMangaListSorting.LIST_SCORE,
+                            status: Optional[str] = None,
+                            limit: int = 100,
+                            offset: int = 0,
+                            list_status_fields: ListStatusFields = True,
+                            fields: Fields = Fields.from_list(['id', 'title', 'main_picture']),
+                            nsfw: bool = None):
+        """
+        Fetches manga list for given user
+
+        :params MyMangaListSorting sort: Method using which entries will be sorted
+        :params str status: Only entries with provided status will be returned
+        :params int limit: Number of entries returned
+        :params int offset: Position starting from which entries will be fetched
+        :params ListStatusFields list_status_fields: Fields returned inside my_list_status field in entry
+        :params Fields fields: Fields returned alongside each entry
+        :param bool nsfw: If set to True results with nsfw grade 'gray' and 'black' will also be fetched, if omitted it will be inherited from Client class
+
+        :returns: List of objects containing manga information for entries on users manga list
+        :rtype: PagedResult[MangaObject]
+        """
+        uri = f'users/{username}/mangalist'
+        fields.my_list_status = list_status_fields
+        if isinstance(sort, str):
+            sort = MyMangaListSorting(sort.lower())
+        params = {
+            "sort": sort.value,
+            "limit": limit,
+            "fields": fields.to_payload(),
+            "status": status,
+            "offset": offset,
+            "nfsw": nsfw if nsfw is not None else self.nsfw
+        }
+        temp = self._api_handler.call(uri=uri, params=params)
         return PagedResult([MangaObject(**entry) for entry in temp['data']], temp['paging']) if len(temp['data']) != 0 else None
```

### Comparing `malclient-upgraded-1.3.4a0/malclient/request_handler.py` & `malclient-upgraded-1.4a1/malclient/request_handler.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-import datetime
-
-import requests
-from .exceptions import *
-import logging
-
-__all__ = ['APICaller']
-
-
-class APICaller(object):
-    def __init__(self, base_url, headers):
-        self._base_url = base_url
-        self._headers = headers
-
-    def call(self, uri, method="get", params=None, *args, **kwargs):
-        requester = getattr(requests, method.lower())
-        url = self._base_url + uri
-        logging.info(f"{method.upper()} {url} Query Parameters: {params}")
-        response = requester(url=url,
-                             headers=self._headers,
-                             params=params,
-                             *args,
-                             **kwargs)
-        now = datetime.datetime.now()
-        if response.status_code < 400:
-            response = self._parse_response(response, method)
-        elif 400 <= response.status_code:
-            self._parse_error(response, method, url)
-        end = datetime.datetime.now()
-        return response
-
-    @staticmethod
-    def _parse_response(response, method):
-        if method in ["get", "post", "patch", "put"]:
-            response_json = response.json()
-            if response_json and "data" in response_json:
-                list_response = []
-                if isinstance(response_json["data"], list):
-                    for json_obj in response_json["data"]:
-                        new_dict = {}
-                        if "node" in json_obj:
-                            new_dict = new_dict | json_obj['node']
-                            for k, v in new_dict.items():
-                                if isinstance(v, dict) and "node" in v and len(v) == 1:
-                                    new_dict[k] = new_dict[k]['node']
-                        if "list_status" in json_obj:
-                            new_dict = new_dict | {'list_status': json_obj['list_status']}
-                        if "ranking" in json_obj:
-                            new_dict = new_dict | {'ranking': json_obj['ranking']}
-                        list_response.append(new_dict if new_dict != {} else json_obj)
-                elif isinstance(response_json["data"], dict):
-                    list_response = response_json["data"]
-
-                if "paging" in response_json:
-                    list_response = {"data": list_response, "paging": response_json["paging"]}
-                return list_response
-            else:
-                return response_json
-        elif method == "delete":
-            return response.status_code
-
-    @staticmethod
-    def _parse_error(response, method, url):
-        logging.error(f"{method.upper()} {url} {response.status_code} {json.loads(response.text)['error']}: {json.loads(response.text)['message'] if 'message' in json.loads(response.text) or len(json.loads(response.text)) != 0 else ''}")
-        if str(response.status_code) == "400" or str(response.status_code).lower() == "400 bad request":
-            raise BadRequest(response)
-        elif str(response.status_code) == "401" or str(response.status_code).lower() == "401 unauthorized":
-            raise Unauthorized(response)
-        elif str(response.status_code) == "403" or str(response.status_code).lower() == "403 forbidden":
-            raise Forbidden(response)
-        elif str(response.status_code) == "404" or str(response.status_code).lower() == "404 not found":
-            raise NotFound(response)
-        else:
-            raise APIException(response.status_code, json.loads(response.text)['message'], response)
-
-
-
+import datetime
+
+import requests
+from .exceptions import *
+import logging
+
+__all__ = ['APICaller']
+
+
+class APICaller(object):
+    def __init__(self, base_url, headers):
+        self._base_url = base_url
+        self._headers = headers
+
+    def call(self, uri, method="get", params=None, *args, **kwargs):
+        requester = getattr(requests, method.lower())
+        url = self._base_url + uri
+        logging.info(f"{method.upper()} {url} Query Parameters: {params}")
+        response = requester(url=url,
+                             headers=self._headers,
+                             params=params,
+                             *args,
+                             **kwargs)
+        now = datetime.datetime.now()
+        if response.status_code < 400:
+            response = self._parse_response(response, method)
+        elif 400 <= response.status_code:
+            self._parse_error(response, method, url)
+        end = datetime.datetime.now()
+        return response
+
+    @staticmethod
+    def _parse_response(response, method):
+        if method in ["get", "post", "patch", "put"]:
+            response_json = response.json()
+            if response_json and "data" in response_json:
+                list_response = []
+                if isinstance(response_json["data"], list):
+                    for json_obj in response_json["data"]:
+                        new_dict = {}
+                        if "node" in json_obj:
+                            new_dict = new_dict | json_obj['node']
+                            for k, v in new_dict.items():
+                                if isinstance(v, dict) and "node" in v and len(v) == 1:
+                                    new_dict[k] = new_dict[k]['node']
+                        if "list_status" in json_obj:
+                            new_dict = new_dict | {'list_status': json_obj['list_status']}
+                        if "ranking" in json_obj:
+                            new_dict = new_dict | {'ranking': json_obj['ranking']}
+                        list_response.append(new_dict if new_dict != {} else json_obj)
+                elif isinstance(response_json["data"], dict):
+                    list_response = response_json["data"]
+
+                if "paging" in response_json:
+                    list_response = {"data": list_response, "paging": response_json["paging"]}
+                return list_response
+            else:
+                return response_json
+        elif method == "delete":
+            return response.status_code
+
+    @staticmethod
+    def _parse_error(response, method, url):
+        logging.error(f"{method.upper()} {url} {response.status_code} {json.loads(response.text)['error']}: {json.loads(response.text)['message'] if 'message' in json.loads(response.text) or len(json.loads(response.text)) != 0 else ''}")
+        if str(response.status_code) == "400" or str(response.status_code).lower() == "400 bad request":
+            raise BadRequest(response)
+        elif str(response.status_code) == "401" or str(response.status_code).lower() == "401 unauthorized":
+            raise Unauthorized(response)
+        elif str(response.status_code) == "403" or str(response.status_code).lower() == "403 forbidden":
+            raise Forbidden(response)
+        elif str(response.status_code) == "404" or str(response.status_code).lower() == "404 not found":
+            raise NotFound(response)
+        else:
+            raise APIException(response.status_code, json.loads(response.text)['message'], response)
+
+
+
```

### Comparing `malclient-upgraded-1.3.4a0/malclient_upgraded.egg-info/PKG-INFO` & `malclient-upgraded-1.4a1/malclient_upgraded.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: malclient-upgraded
-Version: 1.3.4a0
+Version: 1.4a1
 Summary: Modified and rewritten using modern models version of James Fotherby malclient
 Home-page: https://github.com/ModerNews/MAL-API-Client-Upgraded
 Author: ModerNews
 Author-email: polski.gruzin.biz@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://mal-api-client-upgraded.readthedocs.io
 Platform: UNKNOWN
@@ -22,15 +22,14 @@
 ![Read the Docs](https://img.shields.io/readthedocs/mal-api-client-upgraded?style=for-the-badge&color=3EB049)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/malclient-upgraded?style=for-the-badge&color=3EB049) </br>
 A third party object-oriented python3 client library for MyAnimeList's official REST API.
 Originally created by [@JFryy](https://github.com/JFryy/MAL-API-Client), dropped around 2 years ago, picked up and rewritten by ModerNews to fit more modern standards and new REST API functions.
 
 ## Documentation
 Unsure what to do? [Check out our documentation](https://mal-api-client-upgraded.readthedocs.io) </br>
-There will be quick guide coming up soon as well!
 
 ## Installation
 **Python 3.9 or newer required**, this is due to changes in type hinting guidelines, for more info regarding this issue read [PEP 585](https://peps.python.org/pep-0585/)  
 Install the latest stable version from [PyPI](https://pypi.org/project/malclient-upgraded/)  
 `pip install malclient-upgraded`  
 
 Or current unstable version directly from GitHub:  
@@ -109,15 +108,14 @@
 print(repr(anime))
 
 # Update anime List based off of search results
 anime = client.search_anime("Monogatari", limit=1)
 ```
 
 ### Most Imoprtant To-Do's
-- [ ] Rewrite boards (currently disabled)
 - [ ] Implement additional search endpoint
 
 ### Useful resources
 - [MAL auth guide](https://myanimelist.net/blog.php?eid=835707)
 - [Unofficial API Discord](https://discord.gg/XqzqDkzuFx)
 - [Official MAL API Club](https://myanimelist.net/clubs.php?cid=13727)
```

### Comparing `malclient-upgraded-1.3.4a0/malclient_upgraded.egg-info/SOURCES.txt` & `malclient-upgraded-1.4a1/malclient_upgraded.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `malclient-upgraded-1.3.4a0/setup.py` & `malclient-upgraded-1.4a1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-import setuptools
-
-with open("README.md", "r") as fh:
-    long_description = fh.read()
-
-setuptools.setup(
-    name="malclient-upgraded",
-    version="1.3.4a",
-    author="ModerNews",
-    author_email="polski.gruzin.biz@gmail.com",
-    description=
-    "Modified and rewritten using modern models version of James Fotherby malclient",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/ModerNews/MAL-API-Client-Upgraded",
-    project_urls={"Documentation": "https://mal-api-client-upgraded.readthedocs.io"},
-    install_requires=['requests', 'pydantic'],
-    packages=setuptools.find_packages(),
-    include_package_data=True,
-    classifiers=[
-        "Programming Language :: Python :: 3.9",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
-)
+import setuptools
+
+with open("README.md", "r") as fh:
+    long_description = fh.read()
+
+setuptools.setup(
+    name="malclient-upgraded",
+    version="1.4a1",
+    author="ModerNews",
+    author_email="polski.gruzin.biz@gmail.com",
+    description=
+    "Modified and rewritten using modern models version of James Fotherby malclient",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/ModerNews/MAL-API-Client-Upgraded",
+    project_urls={"Documentation": "https://mal-api-client-upgraded.readthedocs.io"},
+    install_requires=['requests', 'pydantic'],
+    packages=setuptools.find_packages(),
+    include_package_data=True,
+    classifiers=[
+        "Programming Language :: Python :: 3.9",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
+)
```

