# Comparing `tmp/characterai-0.5.0.tar.gz` & `tmp/characterai-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\characterai-0.5.0.tar", last modified: Wed May 24 22:23:09 2023, max compression
+gzip compressed data, was "dist\characterai-0.5.1.tar", last modified: Fri May 26 09:36:12 2023, max compression
```

## Comparing `characterai-0.5.0.tar` & `characterai-0.5.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 22:23:09.325900 characterai-0.5.0/
--rw-rw-rw-   0        0        0     1082 2023-04-28 16:51:34.000000 characterai-0.5.0/LICENSE
--rw-rw-rw-   0        0        0     1873 2023-05-24 22:23:09.323901 characterai-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     1481 2023-05-01 15:25:41.000000 characterai-0.5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-24 22:23:09.259431 characterai-0.5.0/characterai/
--rw-rw-rw-   0        0        0       90 2023-05-05 18:13:37.000000 characterai-0.5.0/characterai/__init__.py
--rw-rw-rw-   0        0        0     8871 2023-05-24 22:17:50.000000 characterai-0.5.0/characterai/characterai.py
--rw-rw-rw-   0        0        0      126 2023-05-16 17:53:10.000000 characterai-0.5.0/characterai/errors.py
--rw-rw-rw-   0        0        0     9177 2023-05-24 22:17:56.000000 characterai-0.5.0/characterai/pyasynccai.py
-drwxrwxrwx   0        0        0        0 2023-05-24 22:23:09.318900 characterai-0.5.0/characterai.egg-info/
--rw-rw-rw-   0        0        0     1873 2023-05-24 22:23:08.000000 characterai-0.5.0/characterai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-05-24 22:23:09.000000 characterai-0.5.0/characterai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 22:23:08.000000 characterai-0.5.0/characterai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-05-24 22:23:08.000000 characterai-0.5.0/characterai.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-24 22:23:08.000000 characterai-0.5.0/characterai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-24 22:23:09.325900 characterai-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0      622 2023-05-24 22:19:52.000000 characterai-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 09:36:12.047120 characterai-0.5.1/
+-rw-rw-rw-   0        0        0     1082 2023-04-28 16:51:34.000000 characterai-0.5.1/LICENSE
+-rw-rw-rw-   0        0        0     1873 2023-05-26 09:36:12.046120 characterai-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1481 2023-05-01 15:25:41.000000 characterai-0.5.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 09:36:11.986474 characterai-0.5.1/characterai/
+-rw-rw-rw-   0        0        0       90 2023-05-05 18:13:37.000000 characterai-0.5.1/characterai/__init__.py
+-rw-rw-rw-   0        0        0     9061 2023-05-26 09:30:05.000000 characterai-0.5.1/characterai/characterai.py
+-rw-rw-rw-   0        0        0      126 2023-05-16 17:53:10.000000 characterai-0.5.1/characterai/errors.py
+-rw-rw-rw-   0        0        0     9455 2023-05-26 09:29:05.000000 characterai-0.5.1/characterai/pyasynccai.py
+drwxrwxrwx   0        0        0        0 2023-05-26 09:36:12.044122 characterai-0.5.1/characterai.egg-info/
+-rw-rw-rw-   0        0        0     1873 2023-05-26 09:36:11.000000 characterai-0.5.1/characterai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-05-26 09:36:11.000000 characterai-0.5.1/characterai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 09:36:11.000000 characterai-0.5.1/characterai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-05-26 09:36:11.000000 characterai-0.5.1/characterai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-26 09:36:11.000000 characterai-0.5.1/characterai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 09:36:12.048122 characterai-0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0      622 2023-05-26 09:28:56.000000 characterai-0.5.1/setup.py
```

### Comparing `characterai-0.5.0/LICENSE` & `characterai-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `characterai-0.5.0/PKG-INFO` & `characterai-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: characterai
-Version: 0.5.0
+Version: 0.5.1
 Summary: An unofficial API for character.ai for Python
 Home-page: https://github.com/kramcat/characterai
 Author: kramcat
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `characterai-0.5.0/README.md` & `characterai-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `characterai-0.5.0/characterai/characterai.py` & `characterai-0.5.1/characterai/characterai.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 
 def GetResponse(link: str, *, wait: bool = False, token: str = None) -> Dict[str, str]:
     goto(f'https://beta.character.ai/{link}/', wait=wait, token=token)
     data = json.loads(page.locator('body').inner_text())
 
     return data
 
-def PostResponse(link: str, post_link: str, data: str, headers: str, *, json: bool = True, wait: bool = False) -> Dict[str, str]:
-    goto(link, wait=wait)
+def PostResponse(link: str, post_link: str, data: str, headers: str, *, json: bool = True, wait: bool = False, token: str = None) -> Dict[str, str]:
+    goto(link, wait=wait, token=token)
 
     with page.expect_response(post_link) as response_info:
         # From HearYourWaifu
         page.evaluate("const {fetch: origFetch} = window;window.fetch = async (...args) => {const response = await origFetch(...args);const raw_text = await new Response(response.clone().body).text();return response;};")
         
         page.evaluate("fetch('" + post_link + "', {method: 'POST',body: JSON.stringify(" + str(data) + "),headers: new Headers(" + str(headers) + "),})")
 
@@ -77,15 +77,16 @@
                 return GetResponse('chat/user', wait=wait, token=token)
             else:
                 return PostResponse(
                     link=f'https://beta.character.ai/public-profile/?username={username}',
                     post_link='https://beta.character.ai/chat/user/public/',
                     data={'username': username},
                     headers={'Authorization': f'Token {token}','Content-Type': 'application/json'},
-                    wait=wait
+                    wait=wait,
+                    token=token
                 )
 
         def posts(self, *, wait: bool = False, token: str = None) -> Dict[str, str]:
             return GetResponse(link='chat/posts/user/?scope=user&page=1&posts_to_load=5', wait=wait, token=token)
 
         def followers(self, *, wait: bool = False, token: str = None) -> Dict[str, str]:
             return GetResponse(link='chat/user/followers', wait=wait, token=token)
@@ -132,15 +133,16 @@
                 link=f'https://beta.character.ai/chat?char={char}',
                 post_link='https://beta.character.ai/chat/character/histories/',
                 data={
                     "external_id": char,
                     "number": 50,
                 },
                 headers={'Authorization': f'Token {token}','Content-Type': 'application/json'},
-                wait=wait
+                wait=wait,
+                token=token
             )
 
         def get_history(self, char: str, *, wait: bool = False, token: str = None) -> Dict[str, str]:
             """
             Getting character chat history, return json response
 
             chat.get_history('CHAR')
@@ -165,15 +167,16 @@
             # Get history_external_id and tgt
             if history_external_id == None and tgt == None:
                 info = PostResponse(
                     link=f'https://beta.character.ai/chat?char={char}',
                     post_link='https://beta.character.ai/chat/history/continue/',
                     data={'character_external_id': char},
                     headers={'Authorization': f'Token {token}','Content-Type': 'application/json'},
-                    wait=wait
+                    wait=wait,
+                    token=token
                 )
 
                 history_external_id = info['external_id']
                 tgt = info['participants'][1]['user']['username']
 
             response = PostResponse(
                 link=f'https://beta.character.ai/chat?char={char}',
@@ -182,15 +185,16 @@
                     "history_external_id": history_external_id,
                     "character_external_id": char,
                     "text": message,
                     "tgt": tgt
                 },
                 headers={'Authorization': f'Token {token}','Content-Type': 'application/json'},
                 wait=wait,
-                json=False
+                json=False,
+                token=token
             )
 
             try:
                 return json.loads('{"replies": ' + str(response.split('{"replies": ')[-1].split('\n')[0]))
             except:
                 return response
 
@@ -201,9 +205,10 @@
             chat.new_chat('CHAR')
             """
             return PostResponse(
                 link=f'https://beta.character.ai/chat?char={char}',
                 post_link='https://beta.character.ai/chat/history/create/',
                 data={'character_external_id': char},
                 headers={'Authorization': f'Token {token}', 'Content-Type': 'application/json'},
-                wait=wait
+                wait=wait,
+                token=token
             )
```

### Comparing `characterai-0.5.0/characterai/pyasynccai.py` & `characterai-0.5.1/characterai/pyasynccai.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 
 async def GetResponse(link: str, *, wait: bool = False, token: str = None) -> Dict[str, str]:
     await goto(f'https://beta.character.ai/{link}/', wait=wait, token=token)
     data = json.loads(await (page.locator('body').inner_text()))
 
     return data
 
-async def PostResponse(link: str, post_link: str, data: str, headers: str, *, json: bool = True, wait: bool = False) -> Dict[str, str]:
-    await goto(link, wait=wait)
+async def PostResponse(link: str, post_link: str, data: str, headers: str, *, json: bool = True, wait: bool = False, token: str = None) -> Dict[str, str]:
+    await goto(link, wait=wait, token=token)
 
     async with page.expect_response(post_link) as response_info:
         # From HearYourWaifu
         await page.evaluate("const {fetch: origFetch} = window;window.fetch = async (...args) => {const response = await origFetch(...args);const raw_text = await new Response(response.clone().body).text();return response;};")
         
         await page.evaluate("fetch('" + post_link + "', {method: 'POST',body: JSON.stringify(" + str(data) + "),headers: new Headers(" + str(headers) + "),})")
     
@@ -73,15 +73,16 @@
                 return await GetResponse('chat/user', wait=wait, token=token)
             else:
                 return await PostResponse(
                     link=f'https://beta.character.ai/public-profile/?username={username}',
                     post_link='https://beta.character.ai/chat/user/public/',
                     data={'username': username},
                     headers={'Authorization': f'Token {token}','Content-Type': 'application/json'},
-                    wait=wait
+                    wait=wait,
+                    token=token
                 )
 
         async def posts(self, *, wait: bool = False, token: str = None) -> Dict[str, str]:
             return await GetResponse('chat/posts/user/?scope=user&page=1&posts_to_load=5', wait=wait, token=token)
 
         async def followers(self, *, wait: bool = False, token: str = None) -> Dict[str, str]:
             return await GetResponse('chat/user/followers', wait=wait, token=token)
@@ -128,15 +129,16 @@
                 link=f'https://beta.character.ai/chat?char={char}',
                 post_link='https://beta.character.ai/chat/character/histories/',
                 data={
                     "external_id": char,
                     "number": 50,
                 },
                 headers={'Authorization': f'Token {token}','Content-Type': 'application/json'},
-                wait=wait
+                wait=wait,
+                token=token
             )
 
         async def get_history(self, char: str, *, wait: bool = False, token: str = None) -> Dict[str, str]:
             """
             Getting character chat history, return json response
 
             chat.get_history('CHAR')
@@ -161,32 +163,37 @@
             # Get history_external_id and tgt
             if history_external_id == None and tgt == None:
                 info = await PostResponse(
                     link=f'https://beta.character.ai/chat?char={char}',
                     post_link='https://beta.character.ai/chat/history/continue/',
                     data={'character_external_id': char},
                     headers={'Authorization': f'Token {token}','Content-Type': 'application/json'},
-                    wait=wait
+                    wait=wait,
+                    token=token
                 )
 
-                history_external_id = info['external_id']
-                tgt = info['participants'][1]['user']['username']
+                try:
+                    history_external_id = info['external_id']
+                    tgt = info['participants'][1]['user']['username']
+                except:
+                    return info
 
             response = await PostResponse(
                 link=f'https://beta.character.ai/chat?char={char}',
                 post_link='https://beta.character.ai/chat/streaming/',
                 data={
                     "history_external_id": history_external_id,
                     "character_external_id": char,
                     "text": message,
                     "tgt": tgt
                 },
                 headers={'Authorization': f'Token {token}','Content-Type': 'application/json'},
                 wait=wait,
-                json=False
+                json=False,
+                token=token
             )
 
             try:
                 return json.loads('{"replies": ' + str(response.split('{"replies": ')[-1].split('\n')[0]))
             except:
                 return response
         
@@ -197,9 +204,10 @@
             chat.new_chat('CHAR')
             """
             return await PostResponse(
                 link=f'https://beta.character.ai/chat?char={char}',
                 post_link='https://beta.character.ai/chat/history/create/',
                 data={'character_external_id': char},
                 headers={'Authorization': f'Token {token}', 'Content-Type': 'application/json'},
-                wait=wait
+                wait=wait,
+                token=token
             )
```

### Comparing `characterai-0.5.0/characterai.egg-info/PKG-INFO` & `characterai-0.5.1/characterai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: characterai
-Version: 0.5.0
+Version: 0.5.1
 Summary: An unofficial API for character.ai for Python
 Home-page: https://github.com/kramcat/characterai
 Author: kramcat
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `characterai-0.5.0/setup.py` & `characterai-0.5.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', encoding='utf8') as f:
     long_description = f.read()
 
 setup(
     name='characterai',
-    version='0.5.0',
+    version='0.5.1',
     author='kramcat',
     description='An unofficial API for character.ai for Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/kramcat/characterai',
     packages=find_packages(),
     install_requires=["playwright>=1.32.1"],
```

