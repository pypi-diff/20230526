# Comparing `tmp/talk_codebase-0.1.1.tar.gz` & `tmp/talk_codebase-0.1.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talk_codebase-0.1.1.tar", max compression
+gzip compressed data, was "talk_codebase-0.1.12.tar", max compression
```

## Comparing `talk_codebase-0.1.1.tar` & `talk_codebase-0.1.12.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1050 2023-05-26 01:40:21.126978 talk_codebase-0.1.1/README.md
--rw-r--r--   0        0        0      726 2023-05-26 01:41:17.078920 talk_codebase-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-25 23:09:11.014748 talk_codebase-0.1.1/talk_codebase/__init__.py
--rw-r--r--   0        0        0     1914 2023-05-26 01:36:18.685169 talk_codebase-0.1.1/talk_codebase/cli.py
--rw-r--r--   0        0        0      517 2023-05-25 20:48:02.619519 talk_codebase-0.1.1/talk_codebase/consts.py
--rw-r--r--   0        0        0      595 2023-05-26 01:14:26.805445 talk_codebase-0.1.1/talk_codebase/llm.py
--rw-r--r--   0        0        0     1881 2023-05-26 00:32:10.231483 talk_codebase-0.1.1/talk_codebase/utils.py
--rw-r--r--   0        0        0     1750 1970-01-01 00:00:00.000000 talk_codebase-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1045 2023-05-26 12:00:38.586380 talk_codebase-0.1.12/README.md
+-rw-r--r--   0        0        0      727 2023-05-26 12:00:38.586380 talk_codebase-0.1.12/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-26 12:00:38.586380 talk_codebase-0.1.12/talk_codebase/__init__.py
+-rw-r--r--   0        0        0     1895 2023-05-26 12:00:38.586380 talk_codebase-0.1.12/talk_codebase/cli.py
+-rw-r--r--   0        0        0      517 2023-05-26 12:00:38.586380 talk_codebase-0.1.12/talk_codebase/consts.py
+-rw-r--r--   0        0        0     1377 2023-05-26 12:00:38.586380 talk_codebase-0.1.12/talk_codebase/llm.py
+-rw-r--r--   0        0        0     1368 2023-05-26 12:00:38.586380 talk_codebase-0.1.12/talk_codebase/utils.py
+-rw-r--r--   0        0        0     1746 1970-01-01 00:00:00.000000 talk_codebase-0.1.12/PKG-INFO
```

### Comparing `talk_codebase-0.1.1/README.md` & `talk_codebase-0.1.12/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# talk-codebase is a powerful tool for querying and analyzing codebases
+# talk-codebase is a powerful tool for chatting with your codebase
 
 <p align="center">
-  <img src="https://github.com/rsaryev/talk-codebase/assets/70219513/b0cb4d00-94b6-407e-8545-92e79d442d89" width="800" alt="chat">
+  <img src="https://github.com/rsaryev/talk-codebase/assets/70219513/87a031ec-51e2-4123-abe6-91bb4d248b4d" width="800" alt="chat">
 </p>
 
 ## Description
 
 In the chat, you can ask questions about the codebase. AI will answer your questions, and if necessary, it will offer code improvements. This is very convenient when you want to quickly find something in the codebase, but don't want to waste time searching. It is also convenient when you want to improve a specific function, you can ask "How can I improve the function {function name}?" and AI will suggest improvements. Codebase is analyzed using openai.
 
 ## Installation
```

### Comparing `talk_codebase-0.1.1/pyproject.toml` & `talk_codebase-0.1.12/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "talk-codebase"
-version = "0.1.1"
+version = "0.1.12"
 description = "talk-codebase is a powerful tool for querying and analyzing codebases."
 authors = ["Saryev Rustam <rustam1997@gmail.com>"]
 readme = "README.md"
 packages = [{include = "talk_codebase"}]
 keywords = ["chatgpt", "openai", "cli"]
 
 [tool.poetry.dependencies]
```

### Comparing `talk_codebase-0.1.1/talk_codebase/cli.py` & `talk_codebase-0.1.12/talk_codebase/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import os
 import fire
 import yaml
-from talk_codebase.utils import create_retriever
-from talk_codebase.llm import send_question
+from talk_codebase.llm import create_vector_store, send_question
 
 
 def get_config():
     home_dir = os.path.expanduser("~")
     config_path = os.path.join(home_dir, ".config.yaml")
     if os.path.exists(config_path):
         with open(config_path, "r") as f:
@@ -36,23 +35,23 @@
     try:
         config = get_config()
         api_key = config.get("api_key")
         model_name = config.get("model_name")
         if not (api_key and model_name):
             configure()
             chat(root_dir)
-        retriever = create_retriever(root_dir, api_key)
+        vector_store = create_vector_store(root_dir, api_key)
         while True:
             question = input("👉 ")
             if not question:
                 print("🤖 Please enter a question.")
                 continue
             if question.lower() in ('exit', 'quit'):
                 break
-            send_question(question, retriever, api_key, model_name)
+            send_question(question, vector_store, api_key, model_name)
     except KeyboardInterrupt:
         print("\n🤖 Bye!")
     except Exception as e:
         if str(e) == "<empty message>":
             print("🤖 Please configure your API key.")
             configure()
             chat(root_dir)
```

### Comparing `talk_codebase-0.1.1/talk_codebase/consts.py` & `talk_codebase-0.1.12/talk_codebase/consts.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.1/talk_codebase/utils.py` & `talk_codebase-0.1.12/talk_codebase/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 import os
 import sys
 
-from langchain import FAISS
 from langchain.callbacks.streaming_stdout import StreamingStdOutCallbackHandler
 from langchain.document_loaders import TextLoader
-from langchain.embeddings import OpenAIEmbeddings
-from langchain.text_splitter import CharacterTextSplitter
 
 from talk_codebase.consts import EXCLUDE_DIRS, EXCLUDE_FILES, ALLOW_FILES
 
 
 class StreamStdOut(StreamingStdOutCallbackHandler):
     def on_llm_new_token(self, token: str, **kwargs) -> None:
         sys.stdout.write(token)
@@ -36,19 +33,7 @@
                 try:
                     loader = TextLoader(os.path.join(dirpath, file), encoding='utf-8')
                     docs.extend(loader.load_and_split())
                 except Exception as e:
                     print(f"Error loading file {file}: {e}")
     print(f"🤖 Loaded {len(docs)} documents")
     return docs
-
-
-def create_retriever(root_dir, openai_api_key):
-    docs = load_files(root_dir)
-    text_splitter = CharacterTextSplitter(chunk_size=1000, chunk_overlap=0)
-    texts = text_splitter.split_documents(docs)
-
-    embeddings = OpenAIEmbeddings(openai_api_key=openai_api_key)
-    db = FAISS.from_documents(texts, embeddings)
-    retriever = db.as_retriever()
-
-    return retriever
```

### Comparing `talk_codebase-0.1.1/PKG-INFO` & `talk_codebase-0.1.12/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talk-codebase
-Version: 0.1.1
+Version: 0.1.12
 Summary: talk-codebase is a powerful tool for querying and analyzing codebases.
 Keywords: chatgpt,openai,cli
 Author: Saryev Rustam
 Author-email: rustam1997@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -13,18 +13,18 @@
 Requires-Dist: faiss-cpu (>=1.7.4,<2.0.0)
 Requires-Dist: fire (>=0.5.0,<0.6.0)
 Requires-Dist: langchain (>=0.0.180,<0.0.181)
 Requires-Dist: openai (>=0.27.7,<0.28.0)
 Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
 Description-Content-Type: text/markdown
 
-# talk-codebase is a powerful tool for querying and analyzing codebases
+# talk-codebase is a powerful tool for chatting with your codebase
 
 <p align="center">
-  <img src="https://github.com/rsaryev/talk-codebase/assets/70219513/b0cb4d00-94b6-407e-8545-92e79d442d89" width="800" alt="chat">
+  <img src="https://github.com/rsaryev/talk-codebase/assets/70219513/87a031ec-51e2-4123-abe6-91bb4d248b4d" width="800" alt="chat">
 </p>
 
 ## Description
 
 In the chat, you can ask questions about the codebase. AI will answer your questions, and if necessary, it will offer code improvements. This is very convenient when you want to quickly find something in the codebase, but don't want to waste time searching. It is also convenient when you want to improve a specific function, you can ask "How can I improve the function {function name}?" and AI will suggest improvements. Codebase is analyzed using openai.
 
 ## Installation
```

