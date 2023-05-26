# Comparing `tmp/talk_codebase-0.1.0.tar.gz` & `tmp/talk_codebase-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talk_codebase-0.1.0.tar", max compression
+gzip compressed data, was "talk_codebase-0.1.1.tar", max compression
```

## Comparing `talk_codebase-0.1.0.tar` & `talk_codebase-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      894 2023-05-26 00:52:21.977643 talk_codebase-0.1.0/README.md
--rw-r--r--   0        0        0      726 2023-05-26 01:14:56.810245 talk_codebase-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-25 23:09:11.014748 talk_codebase-0.1.0/talk_codebase/__init__.py
--rw-r--r--   0        0        0     1870 2023-05-26 01:22:09.453976 talk_codebase-0.1.0/talk_codebase/cli.py
--rw-r--r--   0        0        0      517 2023-05-25 20:48:02.619519 talk_codebase-0.1.0/talk_codebase/consts.py
--rw-r--r--   0        0        0      595 2023-05-26 01:14:26.805445 talk_codebase-0.1.0/talk_codebase/llm.py
--rw-r--r--   0        0        0     1881 2023-05-26 00:32:10.231483 talk_codebase-0.1.0/talk_codebase/utils.py
--rw-r--r--   0        0        0     1594 1970-01-01 00:00:00.000000 talk_codebase-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1050 2023-05-26 01:40:21.126978 talk_codebase-0.1.1/README.md
+-rw-r--r--   0        0        0      726 2023-05-26 01:41:17.078920 talk_codebase-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-25 23:09:11.014748 talk_codebase-0.1.1/talk_codebase/__init__.py
+-rw-r--r--   0        0        0     1914 2023-05-26 01:36:18.685169 talk_codebase-0.1.1/talk_codebase/cli.py
+-rw-r--r--   0        0        0      517 2023-05-25 20:48:02.619519 talk_codebase-0.1.1/talk_codebase/consts.py
+-rw-r--r--   0        0        0      595 2023-05-26 01:14:26.805445 talk_codebase-0.1.1/talk_codebase/llm.py
+-rw-r--r--   0        0        0     1881 2023-05-26 00:32:10.231483 talk_codebase-0.1.1/talk_codebase/utils.py
+-rw-r--r--   0        0        0     1750 1970-01-01 00:00:00.000000 talk_codebase-0.1.1/PKG-INFO
```

### Comparing `talk_codebase-0.1.0/README.md` & `talk_codebase-0.1.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # talk-codebase is a powerful tool for querying and analyzing codebases
 
+<p align="center">
+  <img src="https://github.com/rsaryev/talk-codebase/assets/70219513/b0cb4d00-94b6-407e-8545-92e79d442d89" width="800" alt="chat">
+</p>
+
 ## Description
 
 In the chat, you can ask questions about the codebase. AI will answer your questions, and if necessary, it will offer code improvements. This is very convenient when you want to quickly find something in the codebase, but don't want to waste time searching. It is also convenient when you want to improve a specific function, you can ask "How can I improve the function {function name}?" and AI will suggest improvements. Codebase is analyzed using openai.
 
 ## Installation
 
 ```bash
```

### Comparing `talk_codebase-0.1.0/pyproject.toml` & `talk_codebase-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "talk-codebase"
-version = "0.1.0"
+version = "0.1.1"
 description = "talk-codebase is a powerful tool for querying and analyzing codebases."
 authors = ["Saryev Rustam <rustam1997@gmail.com>"]
 readme = "README.md"
 packages = [{include = "talk_codebase"}]
 keywords = ["chatgpt", "openai", "cli"]
 
 [tool.poetry.dependencies]
```

### Comparing `talk_codebase-0.1.0/talk_codebase/cli.py` & `talk_codebase-0.1.1/talk_codebase/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -39,31 +39,33 @@
         model_name = config.get("model_name")
         if not (api_key and model_name):
             configure()
             chat(root_dir)
         retriever = create_retriever(root_dir, api_key)
         while True:
             question = input("👉 ")
+            if not question:
+                print("🤖 Please enter a question.")
+                continue
             if question.lower() in ('exit', 'quit'):
                 break
             send_question(question, retriever, api_key, model_name)
     except KeyboardInterrupt:
         print("\n🤖 Bye!")
     except Exception as e:
         if str(e) == "<empty message>":
             print("🤖 Please configure your API key.")
             configure()
             chat(root_dir)
         else:
-            print("🤖 Sorry, I don't know how to answer that. Please try again.")
-            raise e
+            print(f"🤖 Error: {e}")
 
 
 def main():
     fire.Fire({
         "chat": chat,
         "configure": configure,
     })
 
 
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `talk_codebase-0.1.0/talk_codebase/consts.py` & `talk_codebase-0.1.1/talk_codebase/consts.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.0/talk_codebase/llm.py` & `talk_codebase-0.1.1/talk_codebase/llm.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.0/talk_codebase/utils.py` & `talk_codebase-0.1.1/talk_codebase/utils.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.0/PKG-INFO` & `talk_codebase-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talk-codebase
-Version: 0.1.0
+Version: 0.1.1
 Summary: talk-codebase is a powerful tool for querying and analyzing codebases.
 Keywords: chatgpt,openai,cli
 Author: Saryev Rustam
 Author-email: rustam1997@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -15,14 +15,18 @@
 Requires-Dist: langchain (>=0.0.180,<0.0.181)
 Requires-Dist: openai (>=0.27.7,<0.28.0)
 Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
 Description-Content-Type: text/markdown
 
 # talk-codebase is a powerful tool for querying and analyzing codebases
 
+<p align="center">
+  <img src="https://github.com/rsaryev/talk-codebase/assets/70219513/b0cb4d00-94b6-407e-8545-92e79d442d89" width="800" alt="chat">
+</p>
+
 ## Description
 
 In the chat, you can ask questions about the codebase. AI will answer your questions, and if necessary, it will offer code improvements. This is very convenient when you want to quickly find something in the codebase, but don't want to waste time searching. It is also convenient when you want to improve a specific function, you can ask "How can I improve the function {function name}?" and AI will suggest improvements. Codebase is analyzed using openai.
 
 ## Installation
 
 ```bash
```

