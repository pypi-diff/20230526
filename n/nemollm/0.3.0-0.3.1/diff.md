# Comparing `tmp/nemollm-0.3.0-py3-none-any.whl.zip` & `tmp/nemollm-0.3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 10068 bytes, number of entries: 10
--rw-rw-r--  2.0 unx       40 b- defN 23-Mar-30 01:56 nemollm/__init__.py
--rw-rw-r--  2.0 unx    18808 b- defN 23-May-04 19:26 nemollm/api.py
+Zip file size: 10363 bytes, number of entries: 10
+-rw-rw-r--  2.0 unx       84 b- defN 23-May-25 22:01 nemollm/__init__.py
+-rw-rw-r--  2.0 unx    21937 b- defN 23-May-25 22:01 nemollm/api.py
 -rw-rw-r--  2.0 unx     9872 b- defN 23-May-04 20:56 nemollm/cli.py
 -rw-rw-r--  2.0 unx     1473 b- defN 23-Mar-30 01:56 nemollm/error.py
--rw-rw-r--  2.0 unx       22 b- defN 23-Mar-30 01:56 nemollm/version.py
--rw-rw-r--  2.0 unx     4030 b- defN 23-May-04 20:56 nemollm-0.3.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-04 20:56 nemollm-0.3.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       46 b- defN 23-May-04 20:56 nemollm-0.3.0.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        8 b- defN 23-May-04 20:56 nemollm-0.3.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      755 b- defN 23-May-04 20:56 nemollm-0.3.0.dist-info/RECORD
-10 files, 35146 bytes uncompressed, 8788 bytes compressed:  75.0%
+-rw-rw-r--  2.0 unx       22 b- defN 23-May-26 16:58 nemollm/version.py
+-rw-rw-r--  2.0 unx     4030 b- defN 23-May-26 16:58 nemollm-0.3.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-26 16:58 nemollm-0.3.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       46 b- defN 23-May-26 16:58 nemollm-0.3.1.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        8 b- defN 23-May-26 16:58 nemollm-0.3.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      755 b- defN 23-May-26 16:58 nemollm-0.3.1.dist-info/RECORD
+10 files, 38319 bytes uncompressed, 9083 bytes compressed:  76.3%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: nemollm/error.py
 Comment: 
 
 Filename: nemollm/version.py
 Comment: 
 
-Filename: nemollm-0.3.0.dist-info/METADATA
+Filename: nemollm-0.3.1.dist-info/METADATA
 Comment: 
 
-Filename: nemollm-0.3.0.dist-info/WHEEL
+Filename: nemollm-0.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: nemollm-0.3.0.dist-info/entry_points.txt
+Filename: nemollm-0.3.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: nemollm-0.3.0.dist-info/top_level.txt
+Filename: nemollm-0.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: nemollm-0.3.0.dist-info/RECORD
+Filename: nemollm-0.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nemollm/__init__.py

```diff
@@ -1 +1,2 @@
+from nemollm.api import Connection, NemoLLM
 from nemollm.version import __version__
```

## nemollm/api.py

```diff
@@ -90,16 +90,16 @@
         status_code = response.status_code
 
         is_binary_content = (
             'content-disposition' in response.headers
             and response.headers['content-disposition'].startswith('attachment')
             or response.headers.get('content-type') == 'application/octet-stream'
         )
-
-        if stream:
+        # only set streaming content when success, else raise error to users
+        if stream and status_code < 400:
             decoded_content = 'Streaming content'
         elif is_binary_content:
             decoded_content = 'Binary content'
         else:
             decoded_content = response.content.decode()
         # successful
         if status_code < 400:
@@ -389,15 +389,14 @@
             params["page_size"] = page_size
         if shared is not None:
             params["shared"] = shared
         if sort_by is not None:
             params["sort_by"] = sort_by
         if order is not None:
             params["order"] = order
-        print(params)
         response = _thread_context.session.get(url, headers=self.headers, params=params, timeout=REQUESTS_TIMEOUT_SECS)
         NemoLLM.handle_response(response)
         return response.json()
 
     def list_files(self):
         url = f"{self.api_host}/files"
         if not hasattr(_thread_context, 'session'):
@@ -455,7 +454,93 @@
     def get_customization_training_metrics(self, model, customization_id):
         url = f"https://api.llm.ngc.nvidia.com/v1/models/{model}/customizations/{customization_id}/metrics"
         if not hasattr(_thread_context, 'session'):
             _thread_context.session = create_session()
         response = _thread_context.session.get(url, headers=self.headers, timeout=REQUESTS_TIMEOUT_SECS)
         NemoLLM.handle_response(response)
         return response.json()
+
+
+class Connection(NemoLLM):
+    def __init__(self, access_token=None, host=None):
+        warnings.warn(
+            f'{self.__class__.__name__} will be deprecated in version 0.4.0. Please use NemoLLM instead',
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        super().__init__(api_key=access_token, api_host=host)
+
+    def generate_completion(
+        self,
+        model_id: str,
+        prompt: str,
+        tokens_to_generate: Optional[bool] = None,
+        logprobs: Optional[bool] = None,
+        temperature: Optional[float] = None,
+        top_p: Optional[float] = None,
+        top_k: Optional[int] = None,
+        stop: Optional[List[str]] = None,
+        random_seed: Optional[int] = None,
+        repetition_penalty: Optional[float] = None,
+        beam_search_diversity_rate: Optional[float] = None,
+        beam_width: Optional[int] = None,
+        length_penalty: Optional[int] = None,
+    ):
+        warnings.warn(
+            'This method will be deprecated in version 0.4.0. Please use NemoLLM().generate instead',
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        return self.generate(
+            model=model_id,
+            prompt=prompt,
+            tokens_to_generate=tokens_to_generate,
+            logprobs=logprobs,
+            temperature=temperature,
+            top_p=top_p,
+            top_k=top_k,
+            stop=stop,
+            random_seed=random_seed,
+            repetition_penalty=repetition_penalty,
+            beam_search_diversity_rate=beam_search_diversity_rate,
+            beam_width=beam_width,
+            length_penalty=length_penalty,
+        )
+
+    def generate_customization_completion(
+        self,
+        model_id: str,
+        prompt: str,
+        customization_id: str = None,
+        tokens_to_generate: Optional[bool] = None,
+        logprobs: Optional[bool] = None,
+        temperature: Optional[float] = None,
+        top_p: Optional[float] = None,
+        top_k: Optional[int] = None,
+        stop: Optional[List[str]] = None,
+        random_seed: Optional[int] = None,
+        repetition_penalty: Optional[float] = None,
+        beam_search_diversity_rate: Optional[float] = None,
+        beam_width: Optional[int] = None,
+        length_penalty: Optional[int] = None,
+    ):
+        warnings.warn(
+            'This method will be deprecated in version 0.4.0. Please use NemoLLM().generate instead',
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        return self.generate(
+            model=model_id,
+            prompt=prompt,
+            customization_id=customization_id,
+            tokens_to_generate=tokens_to_generate,
+            logprobs=logprobs,
+            temperature=temperature,
+            top_p=top_p,
+            top_k=top_k,
+            stop=stop,
+            random_seed=random_seed,
+            repetition_penalty=repetition_penalty,
+            beam_search_diversity_rate=beam_search_diversity_rate,
+            beam_width=beam_width,
+            length_penalty=length_penalty,
+        )
```

## nemollm/version.py

```diff
@@ -1 +1 @@
-__version__ = "0.3.0"
+__version__ = "0.3.1"
```

## Comparing `nemollm-0.3.0.dist-info/METADATA` & `nemollm-0.3.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nemollm
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python client library for the NeMo LLM API
 Home-page: https://pypi.org/project/nemollm
 Author: NVIDIA NeMo LLM
 Author-email: nvidia-nemollm@nvidia.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

