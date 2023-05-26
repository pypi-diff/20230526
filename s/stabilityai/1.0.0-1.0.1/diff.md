# Comparing `tmp/stabilityai-1.0.0.tar.gz` & `tmp/stabilityai-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stabilityai-1.0.0.tar", last modified: Fri May 26 14:35:22 2023, max compression
+gzip compressed data, was "stabilityai-1.0.1.tar", last modified: Fri May 26 19:16:33 2023, max compression
```

## Comparing `stabilityai-1.0.0.tar` & `stabilityai-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:35:22.877523 stabilityai-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:35:22.873520 stabilityai-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:35:22.873520 stabilityai-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-26 14:35:09.000000 stabilityai-1.0.0/.github/workflows/build-and-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-05-26 14:35:09.000000 stabilityai-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-26 14:35:09.000000 stabilityai-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-26 14:35:22.877523 stabilityai-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-26 14:35:09.000000 stabilityai-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-26 14:35:09.000000 stabilityai-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-26 14:35:09.000000 stabilityai-1.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 14:35:22.877523 stabilityai-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:35:22.877523 stabilityai-1.0.0/stabilityai/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-26 14:35:09.000000 stabilityai-1.0.0/stabilityai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-05-26 14:35:09.000000 stabilityai-1.0.0/stabilityai/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-26 14:35:09.000000 stabilityai-1.0.0/stabilityai/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-26 14:35:09.000000 stabilityai-1.0.0/stabilityai/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-05-26 14:35:09.000000 stabilityai-1.0.0/stabilityai/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-26 14:35:09.000000 stabilityai-1.0.0/stabilityai/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:35:22.877523 stabilityai-1.0.0/stabilityai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-26 14:35:22.000000 stabilityai-1.0.0/stabilityai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-26 14:35:22.000000 stabilityai-1.0.0/stabilityai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 14:35:22.000000 stabilityai-1.0.0/stabilityai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-26 14:35:22.000000 stabilityai-1.0.0/stabilityai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 14:35:22.000000 stabilityai-1.0.0/stabilityai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:16:33.181263 stabilityai-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:16:33.177263 stabilityai-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:16:33.177263 stabilityai-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-26 19:16:22.000000 stabilityai-1.0.1/.github/workflows/build-and-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-05-26 19:16:22.000000 stabilityai-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-26 19:16:22.000000 stabilityai-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-26 19:16:33.181263 stabilityai-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-26 19:16:22.000000 stabilityai-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-26 19:16:22.000000 stabilityai-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-26 19:16:22.000000 stabilityai-1.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 19:16:33.181263 stabilityai-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:16:33.177263 stabilityai-1.0.1/stabilityai/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-26 19:16:22.000000 stabilityai-1.0.1/stabilityai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8889 2023-05-26 19:16:22.000000 stabilityai-1.0.1/stabilityai/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-26 19:16:22.000000 stabilityai-1.0.1/stabilityai/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-26 19:16:22.000000 stabilityai-1.0.1/stabilityai/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-05-26 19:16:22.000000 stabilityai-1.0.1/stabilityai/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-26 19:16:22.000000 stabilityai-1.0.1/stabilityai/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:16:33.181263 stabilityai-1.0.1/stabilityai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-26 19:16:33.000000 stabilityai-1.0.1/stabilityai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-26 19:16:33.000000 stabilityai-1.0.1/stabilityai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 19:16:33.000000 stabilityai-1.0.1/stabilityai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-26 19:16:33.000000 stabilityai-1.0.1/stabilityai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 19:16:33.000000 stabilityai-1.0.1/stabilityai.egg-info/top_level.txt
```

### Comparing `stabilityai-1.0.0/.github/workflows/build-and-publish.yml` & `stabilityai-1.0.1/.github/workflows/build-and-publish.yml`

 * *Files identical despite different names*

### Comparing `stabilityai-1.0.0/.gitignore` & `stabilityai-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `stabilityai-1.0.0/LICENSE` & `stabilityai-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stabilityai-1.0.0/pyproject.toml` & `stabilityai-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stabilityai-1.0.0/stabilityai/client.py` & `stabilityai-1.0.1/stabilityai/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -30,16 +30,18 @@
     InitImage,
     InitImageMode,
     InitImageStrength,
     ListEnginesResponseBody,
     Sampler,
     Samples,
     Seed,
+    SingleTextPrompt,
     Steps,
     StylePreset,
+    TextPrompt,
     TextPrompts,
     TextToImageRequestBody,
     TextToImageResponseBody,
     UpscaleImageHeight,
     UpscaleImageWidth,
 )
 from stabilityai.utils import omit_none
@@ -115,18 +117,56 @@
                         myclient.text_to_image(...)
 
                 Note that it's `async with` and not `with`.
                 """
                 )
             )
 
+    def _normalize_text_prompts(
+        self,
+        text_prompts: Optional[TextPrompts],
+        text_prompt: Optional[SingleTextPrompt]
+    ):
+        if not bool(text_prompt) ^ bool(text_prompts):
+            raise RuntimeError(
+                textwrap.dedent(
+                    f"""\
+                    You must provide one of text_prompt and text_prompts.
+
+                    Do this
+
+                        stability.text_to_image(
+                            text_prompt="A beautiful sunrise"
+                        )
+
+                    Or this
+
+                        from stabilityai.models import TextPrompt
+
+                        stability.text_to_image(
+                            text_prompts=[
+                                TextPrompt(text="A beautiful sunrise", weight=1.0)
+                            ],
+                        )
+                    """ 
+                )
+            )
+
+        if text_prompt:
+            text_prompts = [TextPrompt(text=text_prompt)]
+
+        # After this moment text_prompts can't be None.
+        assert text_prompts is not None
+        return text_prompts
+
     @validate_arguments
     async def text_to_image(
         self,
-        text_prompts: TextPrompts,
+        text_prompts: Optional[TextPrompts] = None,
+        text_prompt: Optional[SingleTextPrompt] = None,
         *,
         engine: Optional[Engine] = None,
         cfg_scale: Optional[CfgScale] = None,
         clip_guidance_preset: Optional[ClipGuidancePreset] = None,
         height: Optional[DiffuseImageHeight] = None,
         sampler: Optional[Sampler] = None,
         samples: Optional[Samples] = None,
@@ -134,14 +174,15 @@
         steps: Optional[Steps] = None,
         style_preset: Optional[StylePreset] = None,
         width: Optional[DiffuseImageWidth] = None,
         extras: Optional[Extras] = None,
     ):
         self._oops_no_session()
 
+        text_prompts = self._normalize_text_prompts(text_prompts, text_prompt)
         engine_id = engine.id if engine else DEFAULT_GENERATION_ENGINE
 
         request_body = TextToImageRequestBody(
             cfg_scale=cfg_scale,
             clip_guidance_preset=clip_guidance_preset,
             height=height,
             sampler=sampler,
@@ -154,21 +195,23 @@
             extras=extras,
         )
 
         res = await self.session.post(
             f"/v1/generation/{engine_id}/text-to-image",
             data=json.dumps(omit_none(json.loads(request_body.json()))),
         )
+        Sampler.K_DPMPP_2M
 
         return TextToImageResponseBody.parse_obj(await res.json())
 
     @validate_arguments
     async def image_to_image(
         self,
         text_prompts: TextPrompts,
+        text_prompt: SingleTextPrompt,
         init_image: InitImage,
         *,
         init_image_mode: Optional[InitImageMode] = None,
         image_strength: InitImageStrength,
         engine: Optional[Engine] = None,
         cfg_scale: Optional[CfgScale] = None,
         clip_guidance_preset: Optional[ClipGuidancePreset] = None,
@@ -177,14 +220,15 @@
         seed: Optional[Seed] = None,
         steps: Optional[Steps] = None,
         style_preset: Optional[StylePreset] = None,
         extras: Optional[Extras] = None,
     ):
         self._oops_no_session()
 
+        text_prompts = self._normalize_text_prompts(text_prompts, text_prompt)
         engine_id = engine.id if engine else DEFAULT_GENERATION_ENGINE
 
         request_body = ImageToImageRequestBody(
             cfg_scale=cfg_scale,
             clip_guidance_preset=clip_guidance_preset,
             init_image=init_image,
             init_image_mode=init_image_mode,
```

### Comparing `stabilityai-1.0.0/stabilityai/models.py` & `stabilityai-1.0.1/stabilityai/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,14 +99,15 @@
     tile_texture = "tile-texture"
 
 
 class TextPrompt(BaseModel):
     text: Annotated[str, constr(max_length=2000)]
     weight: Optional[float] = None
 
+SingleTextPrompt = str
 
 TextPrompts = List[TextPrompt]
 
 InitImage = bytes
 
 InitImageStrength = Annotated[float, confloat(ge=0.0, le=1.0)]
```

