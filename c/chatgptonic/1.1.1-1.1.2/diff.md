# Comparing `tmp/chatgptonic-1.1.1.tar.gz` & `tmp/chatgptonic-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgptonic-1.1.1.tar", last modified: Fri May 26 15:28:18 2023, max compression
+gzip compressed data, was "chatgptonic-1.1.2.tar", last modified: Fri May 26 15:33:46 2023, max compression
```

## Comparing `chatgptonic-1.1.1.tar` & `chatgptonic-1.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 howardmederiros   (501) staff       (20)        0 2023-05-26 15:28:18.179377 chatgptonic-1.1.1/
--rw-r--r--   0 howardmederiros   (501) staff       (20)      537 2023-05-26 15:28:18.179260 chatgptonic-1.1.1/PKG-INFO
--rw-r--r--   0 howardmederiros   (501) staff       (20)      301 2023-03-13 16:03:22.000000 chatgptonic-1.1.1/README.md
-drwxr-xr-x   0 howardmederiros   (501) staff       (20)        0 2023-05-26 15:28:18.178160 chatgptonic-1.1.1/chatgptonic/
--rw-r--r--   0 howardmederiros   (501) staff       (20)       73 2023-03-14 20:08:55.000000 chatgptonic-1.1.1/chatgptonic/__init__.py
--rw-r--r--   0 howardmederiros   (501) staff       (20)     2350 2023-03-14 20:08:55.000000 chatgptonic-1.1.1/chatgptonic/integration.py
-drwxr-xr-x   0 howardmederiros   (501) staff       (20)        0 2023-05-26 15:28:18.179089 chatgptonic-1.1.1/chatgptonic.egg-info/
--rw-r--r--   0 howardmederiros   (501) staff       (20)      537 2023-05-26 15:28:18.000000 chatgptonic-1.1.1/chatgptonic.egg-info/PKG-INFO
--rw-r--r--   0 howardmederiros   (501) staff       (20)      277 2023-05-26 15:28:18.000000 chatgptonic-1.1.1/chatgptonic.egg-info/SOURCES.txt
--rw-r--r--   0 howardmederiros   (501) staff       (20)        1 2023-05-26 15:28:18.000000 chatgptonic-1.1.1/chatgptonic.egg-info/dependency_links.txt
--rw-r--r--   0 howardmederiros   (501) staff       (20)        1 2023-03-13 16:03:25.000000 chatgptonic-1.1.1/chatgptonic.egg-info/not-zip-safe
--rw-r--r--   0 howardmederiros   (501) staff       (20)       89 2023-05-26 15:28:18.000000 chatgptonic-1.1.1/chatgptonic.egg-info/requires.txt
--rw-r--r--   0 howardmederiros   (501) staff       (20)       12 2023-05-26 15:28:18.000000 chatgptonic-1.1.1/chatgptonic.egg-info/top_level.txt
--rw-r--r--   0 howardmederiros   (501) staff       (20)       38 2023-05-26 15:28:18.179420 chatgptonic-1.1.1/setup.cfg
--rw-r--r--   0 howardmederiros   (501) staff       (20)      986 2023-05-26 15:28:00.000000 chatgptonic-1.1.1/setup.py
+drwxr-xr-x   0 howardmederiros   (501) staff       (20)        0 2023-05-26 15:33:46.641603 chatgptonic-1.1.2/
+-rw-r--r--   0 howardmederiros   (501) staff       (20)      537 2023-05-26 15:33:46.641417 chatgptonic-1.1.2/PKG-INFO
+-rw-r--r--   0 howardmederiros   (501) staff       (20)      301 2023-03-13 16:03:22.000000 chatgptonic-1.1.2/README.md
+drwxr-xr-x   0 howardmederiros   (501) staff       (20)        0 2023-05-26 15:33:46.640002 chatgptonic-1.1.2/chatgptonic/
+-rw-r--r--   0 howardmederiros   (501) staff       (20)       67 2023-05-26 15:31:08.000000 chatgptonic-1.1.2/chatgptonic/__init__.py
+-rw-r--r--   0 howardmederiros   (501) staff       (20)     2200 2023-05-26 15:31:08.000000 chatgptonic-1.1.2/chatgptonic/integration.py
+drwxr-xr-x   0 howardmederiros   (501) staff       (20)        0 2023-05-26 15:33:46.641107 chatgptonic-1.1.2/chatgptonic.egg-info/
+-rw-r--r--   0 howardmederiros   (501) staff       (20)      537 2023-05-26 15:33:46.000000 chatgptonic-1.1.2/chatgptonic.egg-info/PKG-INFO
+-rw-r--r--   0 howardmederiros   (501) staff       (20)      277 2023-05-26 15:33:46.000000 chatgptonic-1.1.2/chatgptonic.egg-info/SOURCES.txt
+-rw-r--r--   0 howardmederiros   (501) staff       (20)        1 2023-05-26 15:33:46.000000 chatgptonic-1.1.2/chatgptonic.egg-info/dependency_links.txt
+-rw-r--r--   0 howardmederiros   (501) staff       (20)        1 2023-03-13 16:03:25.000000 chatgptonic-1.1.2/chatgptonic.egg-info/not-zip-safe
+-rw-r--r--   0 howardmederiros   (501) staff       (20)       88 2023-05-26 15:33:46.000000 chatgptonic-1.1.2/chatgptonic.egg-info/requires.txt
+-rw-r--r--   0 howardmederiros   (501) staff       (20)       12 2023-05-26 15:33:46.000000 chatgptonic-1.1.2/chatgptonic.egg-info/top_level.txt
+-rw-r--r--   0 howardmederiros   (501) staff       (20)       38 2023-05-26 15:33:46.641676 chatgptonic-1.1.2/setup.cfg
+-rw-r--r--   0 howardmederiros   (501) staff       (20)      949 2023-05-26 15:33:02.000000 chatgptonic-1.1.2/setup.py
```

### Comparing `chatgptonic-1.1.1/PKG-INFO` & `chatgptonic-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgptonic
-Version: 1.1.1
+Version: 1.1.2
 Summary: A package to facilitate integration with chatgpt
 Home-page: https://github.com/how-dev/chatgpython
 Author: Howard Medeiros (howard.medeiros@gmail.com)
 License: UNKNOWN
 Keywords: chatgptonic
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `chatgptonic-1.1.1/chatgptonic/integration.py` & `chatgptonic-1.1.2/chatgptonic/integration.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,74 +5,57 @@
 
 class ChatGPTMessageException(Exception):
     pass
 
 
 class ChatGPT:
     def __init__(
-        self,
-        api_key: str,
-        chat_model: str = "gpt-3.5-turbo",
-        role: str = "user"
+        self, api_key: str, chat_model: str = "gpt-3.5-turbo", role: str = "user"
     ):
         self.api_key: str = api_key
 
         self.chat_model: str = chat_model
         self.role: str = role
-        self.chat_url: str = (
-            "https://api.openai.com/v1/chat/completions"
-        )
+        self.chat_url: str = "https://api.openai.com/v1/chat/completions"
 
     def _get_headers(self) -> dict:
         return {
             "Content-Type": "application/json",
-            "Authorization": f"Bearer {self.api_key}"
+            "Authorization": f"Bearer {self.api_key}",
         }
 
     def _get_body(self, message: str, creativity: float) -> dict:
         return {
             "model": self.chat_model,
             "messages": [{"role": self.role, "content": message}],
-            "temperature": creativity
+            "temperature": creativity,
         }
 
     def _get_request(self, message: str, creativity: float):
         body = self._get_body(message, creativity)
         headers = self._get_headers()
 
-        return {
-            "url": self.chat_url,
-            "data": json.dumps(body),
-            "headers": headers
-        }
+        return {"url": self.chat_url, "data": json.dumps(body), "headers": headers}
 
-    def send(
-        self,
-        message: str,
-        creativity: float = .7
-    ) -> dict:
+    def send(self, message: str, creativity: float = 0.7) -> dict:
         request = self._get_request(message, creativity)
 
         response = requests.post(**request)
         response_json = json.loads(response.content)
 
         if response.status_code == 200:
             return response_json
         else:
             errors = response_json["error"]["message"]
 
         raise ChatGPTMessageException(
             f"Something went wrong with this error message: {errors}"
         )
 
-    def just_chat(
-        self,
-        message: str,
-        creativity: float = .7
-    ) -> str:
+    def just_chat(self, message: str, creativity: float = 0.7) -> str:
         response = self.send(message, creativity=creativity)
 
         return response["choices"][0]["message"]["content"].replace("\n", "")
 
     def start_interactive_chat(self):
         count = 0
         while True:
```

### Comparing `chatgptonic-1.1.1/chatgptonic.egg-info/PKG-INFO` & `chatgptonic-1.1.2/chatgptonic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgptonic
-Version: 1.1.1
+Version: 1.1.2
 Summary: A package to facilitate integration with chatgpt
 Home-page: https://github.com/how-dev/chatgpython
 Author: Howard Medeiros (howard.medeiros@gmail.com)
 License: UNKNOWN
 Keywords: chatgptonic
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `chatgptonic-1.1.1/setup.py` & `chatgptonic-1.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,20 +14,19 @@
         'Programming Language :: Python :: 3.8',
     ],
     description="A package to facilitate integration with chatgpt",
     install_requires=[
         "certifi==2022.12.7",
         "charset-normalizer==3.1.0",
         "idna==3.4",
-        "requests==2.31.0",
+        "requests>=2.0.0",
         "urllib3==1.26.15",
     ],
     include_package_data=True,
     keywords='chatgptonic',
     name='chatgptonic',
-    packages=find_packages(include=['chatgptonic',
-                                    'chatgptonic.*']),
+    packages=find_packages(include=['chatgptonic', 'chatgptonic.*']),
     test_suite='tests',
     url='https://github.com/how-dev/chatgpython',
-    version='1.1.1',
+    version='1.1.2',
     zip_safe=False,
 )
```

