# Comparing `tmp/webuiapi-0.8.1-py3-none-any.whl.zip` & `tmp/webuiapi-0.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 12329 bytes, number of entries: 7
--rw-r--r--  2.0 unx      484 b- defN 23-May-21 06:47 webuiapi/__init__.py
--rw-r--r--  2.0 unx    33972 b- defN 23-May-21 06:46 webuiapi/webuiapi.py
--rw-r--r--  2.0 unx     1079 b- defN 23-May-21 06:49 webuiapi-0.8.1.dist-info/LICENSE
--rw-r--r--  2.0 unx    12995 b- defN 23-May-21 06:49 webuiapi-0.8.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-21 06:49 webuiapi-0.8.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-May-21 06:49 webuiapi-0.8.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      545 b- defN 23-May-21 06:49 webuiapi-0.8.1.dist-info/RECORD
-7 files, 49176 bytes uncompressed, 11367 bytes compressed:  76.9%
+Zip file size: 12425 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      532 b- defN 23-May-26 01:18 webuiapi/__init__.py
+-rw-r--r--  2.0 unx    34359 b- defN 23-May-26 01:18 webuiapi/webuiapi.py
+-rw-r--r--  2.0 unx     1079 b- defN 23-May-26 01:18 webuiapi-0.9.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    12995 b- defN 23-May-26 01:18 webuiapi-0.9.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-26 01:18 webuiapi-0.9.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-May-26 01:18 webuiapi-0.9.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      545 b- defN 23-May-26 01:18 webuiapi-0.9.0.dist-info/RECORD
+7 files, 49611 bytes uncompressed, 11463 bytes compressed:  76.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: webuiapi/__init__.py
 Comment: 
 
 Filename: webuiapi/webuiapi.py
 Comment: 
 
-Filename: webuiapi-0.8.1.dist-info/LICENSE
+Filename: webuiapi-0.9.0.dist-info/LICENSE
 Comment: 
 
-Filename: webuiapi-0.8.1.dist-info/METADATA
+Filename: webuiapi-0.9.0.dist-info/METADATA
 Comment: 
 
-Filename: webuiapi-0.8.1.dist-info/WHEEL
+Filename: webuiapi-0.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: webuiapi-0.8.1.dist-info/top_level.txt
+Filename: webuiapi-0.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: webuiapi-0.8.1.dist-info/RECORD
+Filename: webuiapi-0.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## webuiapi/__init__.py

```diff
@@ -1,18 +1,29 @@
-from .webuiapi import WebUIApi, WebUIApiResult, Upscaler, HiResUpscaler, b64_img, raw_b64_img, ModelKeywordResult, ModelKeywordInterface, InstructPix2PixInterface, ControlNetInterface, ControlNetUnit
+from .webuiapi import (
+    WebUIApi,
+    WebUIApiResult,
+    Upscaler,
+    HiResUpscaler,
+    b64_img,
+    raw_b64_img,
+    ModelKeywordResult,
+    ModelKeywordInterface,
+    InstructPix2PixInterface,
+    ControlNetInterface,
+    ControlNetUnit,
+)
 
-__version__ = "0.8.1"
+__version__ = "0.9.0"
 
 __all__ = [
     "__version__",
     "WebUIApi",
     "WebUIApiResult",
     "Upscaler",
     "HiResUpscaler",
     "b64_img",
     "ModelKeywordResult",
     "ModelKeywordInterface",
     "InstructPix2PixInterface",
     "ControlNetInterface",
     "ControlNetUnit",
 ]
-
```

## webuiapi/webuiapi.py

```diff
@@ -3,55 +3,59 @@
 import io
 import base64
 from PIL import Image
 from dataclasses import dataclass
 from enum import Enum
 from typing import List, Dict, Any
 
+
 class Upscaler(str, Enum):
-    none = 'None'
-    Lanczos = 'Lanczos'
-    Nearest = 'Nearest'
-    LDSR = 'LDSR'
-    BSRGAN = 'BSRGAN'
-    ESRGAN_4x = 'ESRGAN_4x'
-    R_ESRGAN_General_4xV3 = 'R-ESRGAN General 4xV3'
-    ScuNET_GAN = 'ScuNET GAN'
-    ScuNET_PSNR = 'ScuNET PSNR'
-    SwinIR_4x = 'SwinIR 4x'
+    none = "None"
+    Lanczos = "Lanczos"
+    Nearest = "Nearest"
+    LDSR = "LDSR"
+    BSRGAN = "BSRGAN"
+    ESRGAN_4x = "ESRGAN_4x"
+    R_ESRGAN_General_4xV3 = "R-ESRGAN General 4xV3"
+    ScuNET_GAN = "ScuNET GAN"
+    ScuNET_PSNR = "ScuNET PSNR"
+    SwinIR_4x = "SwinIR 4x"
+
 
 class HiResUpscaler(str, Enum):
-    none = 'None'
-    Latent = 'Latent'
-    LatentAntialiased = 'Latent (antialiased)'
-    LatentBicubic = 'Latent (bicubic)'
-    LatentBicubicAntialiased = 'Latent (bicubic antialiased)'
-    LatentNearest = 'Latent (nearist)'
-    LatentNearestExact = 'Latent (nearist-exact)'
-    Lanczos = 'Lanczos'
-    Nearest = 'Nearest'
-    ESRGAN_4x = 'ESRGAN_4x'
-    LDSR = 'LDSR'
-    ScuNET_GAN = 'ScuNET GAN'
-    ScuNET_PSNR = 'ScuNET PSNR'
-    SwinIR_4x = 'SwinIR 4x'
+    none = "None"
+    Latent = "Latent"
+    LatentAntialiased = "Latent (antialiased)"
+    LatentBicubic = "Latent (bicubic)"
+    LatentBicubicAntialiased = "Latent (bicubic antialiased)"
+    LatentNearest = "Latent (nearist)"
+    LatentNearestExact = "Latent (nearist-exact)"
+    Lanczos = "Lanczos"
+    Nearest = "Nearest"
+    ESRGAN_4x = "ESRGAN_4x"
+    LDSR = "LDSR"
+    ScuNET_GAN = "ScuNET GAN"
+    ScuNET_PSNR = "ScuNET PSNR"
+    SwinIR_4x = "SwinIR 4x"
 
 
 @dataclass
 class WebUIApiResult:
     images: list
     parameters: dict
     info: dict
 
     @property
     def image(self):
         return self.images[0]
-    
+
+
 class ControlNetUnit:
-    def __init__(self,
+    def __init__(
+        self,
         input_image: Image = None,
         mask: Image = None,
         module: str = "none",
         model: str = "None",
         weight: float = 1.0,
         resize_mode: str = "Resize and Fill",
         lowvram: bool = False,
@@ -59,32 +63,33 @@
         threshold_a: float = 64,
         threshold_b: float = 64,
         guidance: float = 1.0,
         guidance_start: float = 0.0,
         guidance_end: float = 1.0,
         control_mode: int = 0,
         pixel_perfect: bool = False,
-        guessmode: int = None, # deprecated: use control_mode
-        ):
-        
+        guessmode: int = None,  # deprecated: use control_mode
+    ):
         self.input_image = input_image
         self.mask = mask
         self.module = module
         self.model = model
         self.weight = weight
         self.resize_mode = resize_mode
         self.lowvram = lowvram
         self.processor_res = processor_res
         self.threshold_a = threshold_a
         self.threshold_b = threshold_b
         self.guidance = guidance
         self.guidance_start = guidance_start
         self.guidance_end = guidance_end
         if guessmode:
-            print('ControlNetUnit guessmode is deprecated. Please use control_mode instead.')
+            print(
+                "ControlNetUnit guessmode is deprecated. Please use control_mode instead."
+            )
             control_mode = guessmode
         self.control_mode = control_mode
         self.pixel_perfect = pixel_perfect
 
     def to_dict(self):
         return {
             "input_image": raw_b64_img(self.input_image) if self.input_image else "",
@@ -100,149 +105,184 @@
             "guidance": self.guidance,
             "guidance_start": self.guidance_start,
             "guidance_end": self.guidance_end,
             "control_mode": self.control_mode,
             "pixel_perfect": self.pixel_perfect,
         }
 
+
 def b64_img(image: Image):
     buffered = io.BytesIO()
     image.save(buffered, format="PNG")
-    img_base64 = 'data:image/png;base64,' + str(base64.b64encode(buffered.getvalue()), 'utf-8')
+    img_base64 = "data:image/png;base64," + str(
+        base64.b64encode(buffered.getvalue()), "utf-8"
+    )
     return img_base64
 
+
 def raw_b64_img(image: Image):
     # XXX controlnet only accepts RAW base64 without headers
     buffered = io.BytesIO()
     image.save(buffered, format="PNG")
-    img_base64 = str(base64.b64encode(buffered.getvalue()), 'utf-8')
+    img_base64 = str(base64.b64encode(buffered.getvalue()), "utf-8")
     return img_base64
 
-class WebUIApi:
 
+class WebUIApi:
     has_controlnet = False
 
-    def __init__(self,
-                 host='127.0.0.1',
-                 port=7860,
-                 baseurl=None,
-                 sampler='Euler a',
-                 steps=20,
-                 use_https=False):
+    def __init__(
+        self,
+        host="127.0.0.1",
+        port=7860,
+        baseurl=None,
+        sampler="Euler a",
+        steps=20,
+        use_https=False,
+    ):
         if baseurl is None:
             if use_https:
-                baseurl = f'https://{host}:{port}/sdapi/v1'
+                baseurl = f"https://{host}:{port}/sdapi/v1"
             else:
-                baseurl = f'http://{host}:{port}/sdapi/v1'
+                baseurl = f"http://{host}:{port}/sdapi/v1"
 
         self.baseurl = baseurl
         self.default_sampler = sampler
         self.default_steps = steps
 
         self.session = requests.Session()
 
         self.check_controlnet()
 
     def check_controlnet(self):
         try:
             scripts = self.get_scripts()
-            self.has_controlnet = 'controlnet m2m' in scripts['txt2img']
+            self.has_controlnet = "controlnet m2m" in scripts["txt2img"]
         except:
             pass
 
     def set_auth(self, username, password):
         self.session.auth = (username, password)
 
     def _to_api_result(self, response):
-
         if response.status_code != 200:
             raise RuntimeError(response.status_code, response.text)
 
         r = response.json()
         images = []
-        if 'images' in r.keys():
-            images = [Image.open(io.BytesIO(base64.b64decode(i))) for i in r['images']]
-        elif 'image' in r.keys():
-            images = [Image.open(io.BytesIO(base64.b64decode(r['image'])))]
+        if "images" in r.keys():
+            images = [Image.open(io.BytesIO(base64.b64decode(i))) for i in r["images"]]
+        elif "image" in r.keys():
+            images = [Image.open(io.BytesIO(base64.b64decode(r["image"])))]
 
-        info = ''
-        if 'info' in r.keys():
+        info = ""
+        if "info" in r.keys():
             try:
-                info = json.loads(r['info'])
+                info = json.loads(r["info"])
             except:
-                info = r['info']
-        elif 'html_info' in r.keys():
-            info = r['html_info']
-        elif 'caption' in r.keys():
-            info = r['caption']
-
-        parameters = ''
-        if 'parameters' in r.keys():
-            parameters = r['parameters']
+                info = r["info"]
+        elif "html_info" in r.keys():
+            info = r["html_info"]
+        elif "caption" in r.keys():
+            info = r["caption"]
+
+        parameters = ""
+        if "parameters" in r.keys():
+            parameters = r["parameters"]
 
         return WebUIApiResult(images, parameters, info)
 
-    def txt2img(self,
-                enable_hr=False,
-                denoising_strength=0.7,
-                firstphase_width=0,
-                firstphase_height=0,
-                hr_scale=2,
-                hr_upscaler=HiResUpscaler.Latent,
-                hr_second_pass_steps=0,
-                hr_resize_x=0,
-                hr_resize_y=0,
-                prompt="",
-                styles=[],
-                seed=-1,
-                subseed=-1,
-                subseed_strength=0.0,
-                seed_resize_from_h=0,
-                seed_resize_from_w=0,
-                sampler_name=None,  # use this instead of sampler_index
-                batch_size=1,
-                n_iter=1,
-                steps=None,
-                cfg_scale=7.0,
-                width=512,
-                height=512,
-                restore_faces=False,
-                tiling=False,
-                do_not_save_samples=False,
-                do_not_save_grid=False,
-                negative_prompt="",
-                eta=1.0,
-                s_churn=0,
-                s_tmax=0,
-                s_tmin=0,
-                s_noise=1,
-                override_settings={},
-                override_settings_restore_afterwards=True,
-                script_args=None,  # List of arguments for the script "script_name"
-                script_name=None,
-                send_images=True,
-                save_images=False,
-                alwayson_scripts={},
-                controlnet_units: List[ControlNetUnit] = [],
-                sampler_index=None, # deprecated: use sampler_name
-                use_deprecated_controlnet=False,
-                ):
+    async def _to_api_result_async(self, response):
+        if response.status != 200:
+            raise RuntimeError(response.status, await response.text)
+
+        r = await response.json()
+        images = []
+        if "images" in r.keys():
+            images = [Image.open(io.BytesIO(base64.b64decode(i))) for i in r["images"]]
+        elif "image" in r.keys():
+            images = [Image.open(io.BytesIO(base64.b64decode(r["image"])))]
+
+        info = ""
+        if "info" in r.keys():
+            try:
+                info = json.loads(r["info"])
+            except:
+                info = r["info"]
+        elif "html_info" in r.keys():
+            info = r["html_info"]
+        elif "caption" in r.keys():
+            info = r["caption"]
+
+        parameters = ""
+        if "parameters" in r.keys():
+            parameters = r["parameters"]
+
+        return WebUIApiResult(images, parameters, info)
+
+    def txt2img(
+        self,
+        enable_hr=False,
+        denoising_strength=0.7,
+        firstphase_width=0,
+        firstphase_height=0,
+        hr_scale=2,
+        hr_upscaler=HiResUpscaler.Latent,
+        hr_second_pass_steps=0,
+        hr_resize_x=0,
+        hr_resize_y=0,
+        prompt="",
+        styles=[],
+        seed=-1,
+        subseed=-1,
+        subseed_strength=0.0,
+        seed_resize_from_h=0,
+        seed_resize_from_w=0,
+        sampler_name=None,  # use this instead of sampler_index
+        batch_size=1,
+        n_iter=1,
+        steps=None,
+        cfg_scale=7.0,
+        width=512,
+        height=512,
+        restore_faces=False,
+        tiling=False,
+        do_not_save_samples=False,
+        do_not_save_grid=False,
+        negative_prompt="",
+        eta=1.0,
+        s_churn=0,
+        s_tmax=0,
+        s_tmin=0,
+        s_noise=1,
+        override_settings={},
+        override_settings_restore_afterwards=True,
+        script_args=None,  # List of arguments for the script "script_name"
+        script_name=None,
+        send_images=True,
+        save_images=False,
+        alwayson_scripts={},
+        controlnet_units: List[ControlNetUnit] = [],
+        sampler_index=None,  # deprecated: use sampler_name
+        use_deprecated_controlnet=False,
+        use_async=False,
+    ):
         if sampler_index is None:
             sampler_index = self.default_sampler
         if sampler_name is None:
             sampler_name = self.default_sampler
         if steps is None:
             steps = self.default_steps
         if script_args is None:
             script_args = []
         payload = {
             "enable_hr": enable_hr,
-            "hr_scale" : hr_scale,
-            "hr_upscaler" : hr_upscaler,
-            "hr_second_pass_steps" : hr_second_pass_steps,
+            "hr_scale": hr_scale,
+            "hr_upscaler": hr_upscaler,
+            "hr_second_pass_steps": hr_second_pass_steps,
             "hr_resize_x": hr_resize_x,
             "hr_resize_y": hr_resize_y,
             "denoising_strength": denoising_strength,
             "firstphase_width": firstphase_width,
             "firstphase_height": firstphase_height,
             "prompt": prompt,
             "styles": styles,
@@ -274,77 +314,98 @@
             "script_name": script_name,
             "script_args": script_args,
             "send_images": send_images,
             "save_images": save_images,
             "alwayson_scripts": alwayson_scripts,
         }
 
-        if use_deprecated_controlnet and controlnet_units and len(controlnet_units)>0:
+        if use_deprecated_controlnet and controlnet_units and len(controlnet_units) > 0:
             payload["controlnet_units"] = [x.to_dict() for x in controlnet_units]
-            return self.custom_post('controlnet/txt2img', payload=payload)
+            return self.custom_post(
+                "controlnet/txt2img", payload=payload, use_async=use_async
+            )
 
-        if controlnet_units and len(controlnet_units)>0:
+        if controlnet_units and len(controlnet_units) > 0:
             payload["alwayson_scripts"]["ControlNet"] = {
                 "args": [x.to_dict() for x in controlnet_units]
             }
         elif self.has_controlnet:
             # workaround : if not passed, webui will use previous args!
             payload["alwayson_scripts"]["ControlNet"] = {"args": []}
 
-        response = self.session.post(url=f'{self.baseurl}/txt2img', json=payload)
-        return self._to_api_result(response)
+        return self.post_and_get_api_result(
+            f"{self.baseurl}/txt2img", payload, use_async
+        )
+
+    def post_and_get_api_result(self, url, json, use_async):
+        if use_async:
+            import asyncio
+
+            return asyncio.ensure_future(self.async_post(url=url, json=json))
+        else:
+            response = self.session.post(url=url, json=json)
+            return self._to_api_result(response)
 
-    def img2img(self,
-                images=[],  # list of PIL Image
-                resize_mode=0,
-                denoising_strength=0.75,
-                image_cfg_scale=1.5,
-                mask_image=None,  # PIL Image mask
-                mask_blur=4,
-                inpainting_fill=0,
-                inpaint_full_res=True,
-                inpaint_full_res_padding=0,
-                inpainting_mask_invert=0,
-                initial_noise_multiplier=1,
-                prompt="",
-                styles=[],
-                seed=-1,
-                subseed=-1,
-                subseed_strength=0,
-                seed_resize_from_h=0,
-                seed_resize_from_w=0,
-                sampler_name=None,  # use this instead of sampler_index
-                batch_size=1,
-                n_iter=1,
-                steps=None,
-                cfg_scale=7.0,
-                width=512,
-                height=512,
-                restore_faces=False,
-                tiling=False,
-                do_not_save_samples=False,
-                do_not_save_grid=False,
-                negative_prompt="",
-                eta=1.0,
-                s_churn=0,
-                s_tmax=0,
-                s_tmin=0,
-                s_noise=1,
-                override_settings={},
-                override_settings_restore_afterwards=True,
-                script_args=None,  # List of arguments for the script "script_name"
-                sampler_index=None,  # deprecated: use sampler_name
-                include_init_images=False,
-                script_name=None,
-                send_images=True,
-                save_images=False,
-                alwayson_scripts={},
-                controlnet_units: List[ControlNetUnit] = [],
-                use_deprecated_controlnet = False,
-                ):
+    async def async_post(self, url, json):
+        import aiohttp
+
+        async with aiohttp.ClientSession() as session:
+            async with session.post(url, json=json) as response:
+                return await self._to_api_result_async(response)
+
+    def img2img(
+        self,
+        images=[],  # list of PIL Image
+        resize_mode=0,
+        denoising_strength=0.75,
+        image_cfg_scale=1.5,
+        mask_image=None,  # PIL Image mask
+        mask_blur=4,
+        inpainting_fill=0,
+        inpaint_full_res=True,
+        inpaint_full_res_padding=0,
+        inpainting_mask_invert=0,
+        initial_noise_multiplier=1,
+        prompt="",
+        styles=[],
+        seed=-1,
+        subseed=-1,
+        subseed_strength=0,
+        seed_resize_from_h=0,
+        seed_resize_from_w=0,
+        sampler_name=None,  # use this instead of sampler_index
+        batch_size=1,
+        n_iter=1,
+        steps=None,
+        cfg_scale=7.0,
+        width=512,
+        height=512,
+        restore_faces=False,
+        tiling=False,
+        do_not_save_samples=False,
+        do_not_save_grid=False,
+        negative_prompt="",
+        eta=1.0,
+        s_churn=0,
+        s_tmax=0,
+        s_tmin=0,
+        s_noise=1,
+        override_settings={},
+        override_settings_restore_afterwards=True,
+        script_args=None,  # List of arguments for the script "script_name"
+        sampler_index=None,  # deprecated: use sampler_name
+        include_init_images=False,
+        script_name=None,
+        send_images=True,
+        save_images=False,
+        alwayson_scripts={},
+        controlnet_units: List[ControlNetUnit] = [],
+        use_deprecated_controlnet=False,
+        use_async=False,
+    ):
         if sampler_name is None:
             sampler_name = self.default_sampler
         if sampler_index is None:
             sampler_index = self.default_sampler
         if steps is None:
             steps = self.default_steps
         if script_args is None:
@@ -392,46 +453,51 @@
             "script_name": script_name,
             "script_args": script_args,
             "send_images": send_images,
             "save_images": save_images,
             "alwayson_scripts": alwayson_scripts,
         }
         if mask_image is not None:
-            payload['mask'] = b64_img(mask_image)
-            
-        if use_deprecated_controlnet and controlnet_units and len(controlnet_units)>0:
+            payload["mask"] = b64_img(mask_image)
+
+        if use_deprecated_controlnet and controlnet_units and len(controlnet_units) > 0:
             payload["controlnet_units"] = [x.to_dict() for x in controlnet_units]
-            return self.custom_post('controlnet/img2img', payload=payload)
+            return self.custom_post(
+                "controlnet/img2img", payload=payload, use_async=use_async
+            )
 
-        if controlnet_units and len(controlnet_units)>0:
+        if controlnet_units and len(controlnet_units) > 0:
             payload["alwayson_scripts"]["ControlNet"] = {
                 "args": [x.to_dict() for x in controlnet_units]
             }
         elif self.has_controlnet:
             payload["alwayson_scripts"]["ControlNet"] = {"args": []}
 
-        response = self.session.post(url=f'{self.baseurl}/img2img', json=payload)
-        return self._to_api_result(response)
-
-    def extra_single_image(self,
-                           image,  # PIL Image
-                           resize_mode=0,
-                           show_extras_results=True,
-                           gfpgan_visibility=0,
-                           codeformer_visibility=0,
-                           codeformer_weight=0,
-                           upscaling_resize=2,
-                           upscaling_resize_w=512,
-                           upscaling_resize_h=512,
-                           upscaling_crop=True,
-                           upscaler_1="None",
-                           upscaler_2="None",
-                           extras_upscaler_2_visibility=0,
-                           upscale_first=False,
-                           ):
+        return self.post_and_get_api_result(
+            f"{self.baseurl}/img2img", payload, use_async
+        )
+
+    def extra_single_image(
+        self,
+        image,  # PIL Image
+        resize_mode=0,
+        show_extras_results=True,
+        gfpgan_visibility=0,
+        codeformer_visibility=0,
+        codeformer_weight=0,
+        upscaling_resize=2,
+        upscaling_resize_w=512,
+        upscaling_resize_h=512,
+        upscaling_crop=True,
+        upscaler_1="None",
+        upscaler_2="None",
+        extras_upscaler_2_visibility=0,
+        upscale_first=False,
+        use_async=False,
+    ):
         payload = {
             "resize_mode": resize_mode,
             "show_extras_results": show_extras_results,
             "gfpgan_visibility": gfpgan_visibility,
             "codeformer_visibility": codeformer_visibility,
             "codeformer_weight": codeformer_weight,
             "upscaling_resize": upscaling_resize,
@@ -441,47 +507,47 @@
             "upscaler_1": upscaler_1,
             "upscaler_2": upscaler_2,
             "extras_upscaler_2_visibility": extras_upscaler_2_visibility,
             "upscale_first": upscale_first,
             "image": b64_img(image),
         }
 
-        response = self.session.post(url=f'{self.baseurl}/extra-single-image', json=payload)
-        return self._to_api_result(response)
-
-    def extra_batch_images(self,
-                           images,  # list of PIL images
-                           name_list=None,  # list of image names
-                           resize_mode=0,
-                           show_extras_results=True,
-                           gfpgan_visibility=0,
-                           codeformer_visibility=0,
-                           codeformer_weight=0,
-                           upscaling_resize=2,
-                           upscaling_resize_w=512,
-                           upscaling_resize_h=512,
-                           upscaling_crop=True,
-                           upscaler_1="None",
-                           upscaler_2="None",
-                           extras_upscaler_2_visibility=0,
-                           upscale_first=False,
-                           ):
+        return self.post_and_get_api_result(
+            f"{self.baseurl}/extra-single-image", payload, use_async
+        )
+
+    def extra_batch_images(
+        self,
+        images,  # list of PIL images
+        name_list=None,  # list of image names
+        resize_mode=0,
+        show_extras_results=True,
+        gfpgan_visibility=0,
+        codeformer_visibility=0,
+        codeformer_weight=0,
+        upscaling_resize=2,
+        upscaling_resize_w=512,
+        upscaling_resize_h=512,
+        upscaling_crop=True,
+        upscaler_1="None",
+        upscaler_2="None",
+        extras_upscaler_2_visibility=0,
+        upscale_first=False,
+        use_async=False,
+    ):
         if name_list is not None:
             if len(name_list) != len(images):
-                raise RuntimeError('len(images) != len(name_list)')
+                raise RuntimeError("len(images) != len(name_list)")
         else:
-            name_list = [f'image{i + 1:05}' for i in range(len(images))]
+            name_list = [f"image{i + 1:05}" for i in range(len(images))]
         images = [b64_img(x) for x in images]
 
         image_list = []
         for name, image in zip(name_list, images):
-            image_list.append({
-                "data": image,
-                "name": name
-            })
+            image_list.append({"data": image, "name": name})
 
         payload = {
             "resize_mode": resize_mode,
             "show_extras_results": show_extras_results,
             "gfpgan_visibility": gfpgan_visibility,
             "codeformer_visibility": codeformer_visibility,
             "codeformer_weight": codeformer_weight,
@@ -492,293 +558,329 @@
             "upscaler_1": upscaler_1,
             "upscaler_2": upscaler_2,
             "extras_upscaler_2_visibility": extras_upscaler_2_visibility,
             "upscale_first": upscale_first,
             "imageList": image_list,
         }
 
-        response = self.session.post(url=f'{self.baseurl}/extra-batch-images', json=payload)
-        return self._to_api_result(response)
+        return self.post_and_get_api_result(
+            f"{self.baseurl}/extra-batch-images", payload, use_async
+        )
 
     # XXX 500 error (2022/12/26)
     def png_info(self, image):
         payload = {
             "image": b64_img(image),
         }
 
-        response = self.session.post(url=f'{self.baseurl}/png-info', json=payload)
+        response = self.session.post(url=f"{self.baseurl}/png-info", json=payload)
         return self._to_api_result(response)
 
     # XXX always returns empty info (2022/12/26)
     def interrogate(self, image):
         payload = {
             "image": b64_img(image),
         }
 
-        response = self.session.post(url=f'{self.baseurl}/interrogate', json=payload)
+        response = self.session.post(url=f"{self.baseurl}/interrogate", json=payload)
         return self._to_api_result(response)
-    
+
     def interrupt(self):
-        response = self.session.post(url=f'{self.baseurl}/interrupt')
+        response = self.session.post(url=f"{self.baseurl}/interrupt")
         return response.json()
-    
+
     def skip(self):
-        response = self.session.post(url=f'{self.baseurl}/skip')
+        response = self.session.post(url=f"{self.baseurl}/skip")
         return response.json()
 
-
     def get_options(self):
-        response = self.session.get(url=f'{self.baseurl}/options')
+        response = self.session.get(url=f"{self.baseurl}/options")
         return response.json()
+
     def set_options(self, options):
-        response = self.session.post(url=f'{self.baseurl}/options', json=options)
+        response = self.session.post(url=f"{self.baseurl}/options", json=options)
         return response.json()
 
     def get_cmd_flags(self):
-        response = self.session.get(url=f'{self.baseurl}/cmd-flags')
+        response = self.session.get(url=f"{self.baseurl}/cmd-flags")
         return response.json()
 
     def get_progress(self):
-        response = self.session.get(url=f'{self.baseurl}/progress')
+        response = self.session.get(url=f"{self.baseurl}/progress")
         return response.json()
 
     def get_cmd_flags(self):
-        response = self.session.get(url=f'{self.baseurl}/cmd-flags')
+        response = self.session.get(url=f"{self.baseurl}/cmd-flags")
         return response.json()
-    def get_samplers(self):        
-        response = self.session.get(url=f'{self.baseurl}/samplers')
+
+    def get_samplers(self):
+        response = self.session.get(url=f"{self.baseurl}/samplers")
         return response.json()
-    def get_upscalers(self):        
-        response = self.session.get(url=f'{self.baseurl}/upscalers')
+
+    def get_upscalers(self):
+        response = self.session.get(url=f"{self.baseurl}/upscalers")
         return response.json()
-    def get_sd_models(self):        
-        response = self.session.get(url=f'{self.baseurl}/sd-models')
+
+    def get_sd_models(self):
+        response = self.session.get(url=f"{self.baseurl}/sd-models")
         return response.json()
-    def get_hypernetworks(self):        
-        response = self.session.get(url=f'{self.baseurl}/hypernetworks')
+
+    def get_hypernetworks(self):
+        response = self.session.get(url=f"{self.baseurl}/hypernetworks")
         return response.json()
-    def get_face_restorers(self):        
-        response = self.session.get(url=f'{self.baseurl}/face-restorers')
+
+    def get_face_restorers(self):
+        response = self.session.get(url=f"{self.baseurl}/face-restorers")
         return response.json()
-    def get_realesrgan_models(self):        
-        response = self.session.get(url=f'{self.baseurl}/realesrgan-models')
+
+    def get_realesrgan_models(self):
+        response = self.session.get(url=f"{self.baseurl}/realesrgan-models")
         return response.json()
-    def get_prompt_styles(self):        
-        response = self.session.get(url=f'{self.baseurl}/prompt-styles')
+
+    def get_prompt_styles(self):
+        response = self.session.get(url=f"{self.baseurl}/prompt-styles")
         return response.json()
-    def get_artist_categories(self): # deprecated ?   
-        response = self.session.get(url=f'{self.baseurl}/artist-categories')
+
+    def get_artist_categories(self):  # deprecated ?
+        response = self.session.get(url=f"{self.baseurl}/artist-categories")
         return response.json()
-    def get_artists(self): # deprecated ?
-        response = self.session.get(url=f'{self.baseurl}/artists')
+
+    def get_artists(self):  # deprecated ?
+        response = self.session.get(url=f"{self.baseurl}/artists")
         return response.json()
+
     def refresh_checkpoints(self):
-        response = self.session.post(url=f'{self.baseurl}/refresh-checkpoints')
+        response = self.session.post(url=f"{self.baseurl}/refresh-checkpoints")
         return response.json()
+
     def get_scripts(self):
-        response = self.session.get(url=f'{self.baseurl}/scripts')
+        response = self.session.get(url=f"{self.baseurl}/scripts")
         return response.json()
-    def get_embeddings(self):        
-        response = self.session.get(url=f'{self.baseurl}/embeddings')
+
+    def get_embeddings(self):
+        response = self.session.get(url=f"{self.baseurl}/embeddings")
         return response.json()
-    def get_memory(self):        
-        response = self.session.get(url=f'{self.baseurl}/memory')
+
+    def get_memory(self):
+        response = self.session.get(url=f"{self.baseurl}/memory")
         return response.json()
-    
+
     def get_endpoint(self, endpoint, baseurl):
         if baseurl:
-            return f'{self.baseurl}/{endpoint}'
+            return f"{self.baseurl}/{endpoint}"
         else:
             from urllib.parse import urlparse, urlunparse
+
             parsed_url = urlparse(self.baseurl)
             basehost = parsed_url.netloc
-            parsed_url2 = (parsed_url[0], basehost, endpoint, '', '', '')
+            parsed_url2 = (parsed_url[0], basehost, endpoint, "", "", "")
             return urlunparse(parsed_url2)
+
     def custom_get(self, endpoint, baseurl=False):
         url = self.get_endpoint(endpoint, baseurl)
         response = self.session.get(url=url)
         return response.json()
-    def custom_post(self, endpoint, payload={}, baseurl=False):
+
+    def custom_post(self, endpoint, payload={}, baseurl=False, use_async=False):
         url = self.get_endpoint(endpoint, baseurl)
-        response = self.session.post(url=url, json=payload)
-        return self._to_api_result(response)
+        if use_async:
+            import asyncio
+
+            return asyncio.ensure_future(self.async_post(url=url, json=payload))
+        else:
+            response = self.session.post(url=url, json=payload)
+            return self._to_api_result(response)
 
     def controlnet_version(self):
-        r = self.custom_get('controlnet/version')
-        return r['version']
+        r = self.custom_get("controlnet/version")
+        return r["version"]
 
     def controlnet_model_list(self):
-        r = self.custom_get('controlnet/model_list')
-        return r['model_list']
-    
+        r = self.custom_get("controlnet/model_list")
+        return r["model_list"]
+
     def controlnet_module_list(self):
-        r = self.custom_get('controlnet/module_list')
-        return r['module_list']
+        r = self.custom_get("controlnet/module_list")
+        return r["module_list"]
 
-    def controlnet_detect(self, images, module="none", processor_res=512, threshold_a=64, threshold_b=64):
+    def controlnet_detect(
+        self, images, module="none", processor_res=512, threshold_a=64, threshold_b=64
+    ):
         input_images = [b64_img(x) for x in images]
         payload = {
             "controlnet_module": module,
             "controlnet_input_images": input_images,
             "controlnet_processor_res": processor_res,
             "controlnet_threshold_a": threshold_a,
             "controlnet_threshold_b": threshold_b,
         }
-        r = self.custom_post('controlnet/detect', payload=payload)
+        r = self.custom_post("controlnet/detect", payload=payload)
         return r
-        
+
     def util_get_model_names(self):
-        return sorted([x['title'] for x in self.get_sd_models()])
+        return sorted([x["title"] for x in self.get_sd_models()])
+
     def util_set_model(self, name, find_closest=True):
         if find_closest:
             name = name.lower()
         models = self.util_get_model_names()
         found_model = None
         if name in models:
             found_model = name
         elif find_closest:
             import difflib
+
             def str_simularity(a, b):
                 return difflib.SequenceMatcher(None, a, b).ratio()
+
             max_sim = 0.0
             max_model = models[0]
             for model in models:
                 sim = str_simularity(name, model)
                 if sim >= max_sim:
                     max_sim = sim
                     max_model = model
             found_model = max_model
         if found_model:
-            print(f'loading {found_model}')
+            print(f"loading {found_model}")
             options = {}
-            options['sd_model_checkpoint'] = found_model
+            options["sd_model_checkpoint"] = found_model
             self.set_options(options)
-            print(f'model changed to {found_model}')
+            print(f"model changed to {found_model}")
         else:
-            print('model not found')
+            print("model not found")
 
     def util_get_current_model(self):
-        return self.get_options()['sd_model_checkpoint']
+        return self.get_options()["sd_model_checkpoint"]
 
     def util_wait_for_ready(self, check_interval=5.0):
         import time
+
         while True:
-            result =  self.get_progress()
-            progress = result['progress']
-            job_count = result['state']['job_count']
+            result = self.get_progress()
+            progress = result["progress"]
+            job_count = result["state"]["job_count"]
             if progress == 0.0 and job_count == 0:
                 break
             else:
-                print(f'[WAIT]: progress = {progress:.4f}, job_count = {job_count}')
+                print(f"[WAIT]: progress = {progress:.4f}, job_count = {job_count}")
                 time.sleep(check_interval)
 
 
-
 ## Interface for extensions
 
+
 # https://github.com/mix1009/model-keyword
 @dataclass
 class ModelKeywordResult:
     keywords: list
     model: str
     oldhash: str
     match_source: str
-    
+
+
 class ModelKeywordInterface:
     def __init__(self, webuiapi):
         self.api = webuiapi
+
     def get_keywords(self):
-        result = self.api.custom_get('model_keyword/get_keywords')
-        keywords = result['keywords']
-        model = result['model']
-        oldhash = result['hash']
-        match_source = result['match_source']
+        result = self.api.custom_get("model_keyword/get_keywords")
+        keywords = result["keywords"]
+        model = result["model"]
+        oldhash = result["hash"]
+        match_source = result["match_source"]
         return ModelKeywordResult(keywords, model, oldhash, match_source)
 
+
 # https://github.com/Klace/stable-diffusion-webui-instruct-pix2pix
 class InstructPix2PixInterface:
     def __init__(self, webuiapi):
         self.api = webuiapi
-    def img2img(self, 
+
+    def img2img(
+        self,
         images=[],
-        prompt: str = '',
-        negative_prompt: str = '',
+        prompt: str = "",
+        negative_prompt: str = "",
         output_batches: int = 1,
-        sampler: str = 'Euler a',
+        sampler: str = "Euler a",
         steps: int = 20,
         seed: int = 0,
         randomize_seed: bool = True,
         text_cfg: float = 7.5,
         image_cfg: float = 1.5,
         randomize_cfg: bool = False,
-        output_image_width: int = 512
-        ):
+        output_image_width: int = 512,
+    ):
         init_images = [b64_img(x) for x in images]
         payload = {
             "init_images": init_images,
             "prompt": prompt,
             "negative_prompt": negative_prompt,
             "output_batches": output_batches,
             "sampler": sampler,
             "steps": steps,
             "seed": seed,
             "randomize_seed": randomize_seed,
             "text_cfg": text_cfg,
             "image_cfg": image_cfg,
             "randomize_cfg": randomize_cfg,
-            "output_image_width": output_image_width
+            "output_image_width": output_image_width,
         }
-        return self.api.custom_post('instruct-pix2pix/img2img', payload=payload)
+        return self.api.custom_post("instruct-pix2pix/img2img", payload=payload)
 
 
 # https://github.com/Mikubill/sd-webui-controlnet
 class ControlNetInterface:
     def __init__(self, webuiapi, show_deprecation_warning=True):
         self.api = webuiapi
         self.show_deprecation_warning = show_deprecation_warning
-        
+
     def print_deprecation_warning(self):
-        print('ControlNetInterface txt2img/img2img is deprecated. Please use normal txt2img/img2img with controlnet_units param')
-        
-    def txt2img(self,
+        print(
+            "ControlNetInterface txt2img/img2img is deprecated. Please use normal txt2img/img2img with controlnet_units param"
+        )
+
+    def txt2img(
+        self,
         prompt: str = "",
         negative_prompt: str = "",
         controlnet_input_image: [] = [],
         controlnet_mask: [] = [],
         controlnet_module: str = "",
         controlnet_model: str = "",
         controlnet_weight: float = 0.5,
         controlnet_resize_mode: str = "Scale to Fit (Inner Fit)",
         controlnet_lowvram: bool = False,
         controlnet_processor_res: int = 512,
         controlnet_threshold_a: int = 64,
         controlnet_threshold_b: int = 64,
         controlnet_guidance: float = 1.0,
-        enable_hr: bool = False, # hiresfix
+        enable_hr: bool = False,  # hiresfix
         denoising_strength: float = 0.5,
         hr_scale: float = 1.5,
         hr_upscale: str = "Latent",
         guess_mode: bool = True,
         seed: int = -1,
         subseed: int = -1,
         subseed_strength: int = -1,
         sampler_index: str = "Euler a",
         batch_size: int = 1,
-        n_iter: int = 1, # Iteration
+        n_iter: int = 1,  # Iteration
         steps: int = 20,
         cfg_scale: float = 7,
         width: int = 512,
         height: int = 512,
         restore_faces: bool = False,
-        override_settings: Dict[str, Any] = None, 
-        override_settings_restore_afterwards: bool = True):
-        
+        override_settings: Dict[str, Any] = None,
+        override_settings_restore_afterwards: bool = True,
+    ):
         if self.show_deprecation_warning:
             self.print_deprecation_warning()
-        
+
         controlnet_input_image_b64 = [raw_b64_img(x) for x in controlnet_input_image]
         controlnet_mask_b64 = [raw_b64_img(x) for x in controlnet_mask]
 
         payload = {
             "prompt": prompt,
             "negative_prompt": negative_prompt,
             "controlnet_input_image": controlnet_input_image_b64,
@@ -807,17 +909,18 @@
             "cfg_scale": cfg_scale,
             "width": width,
             "height": height,
             "restore_faces": restore_faces,
             "override_settings": override_settings,
             "override_settings_restore_afterwards": override_settings_restore_afterwards,
         }
-        return self.api.custom_post('controlnet/txt2img', payload=payload)
-    
-    def img2img(self,
+        return self.api.custom_post("controlnet/txt2img", payload=payload)
+
+    def img2img(
+        self,
         init_images: [] = [],
         mask: str = None,
         mask_blur: int = 30,
         inpainting_fill: int = 0,
         inpaint_full_res: bool = True,
         inpaint_full_res_padding: int = 1,
         inpainting_mask_invert: int = 1,
@@ -838,24 +941,24 @@
         controlnet_guidance: float = 1.0,
         guess_mode: bool = True,
         seed: int = -1,
         subseed: int = -1,
         subseed_strength: int = -1,
         sampler_index: str = "",
         batch_size: int = 1,
-        n_iter: int = 1, # Iteration
+        n_iter: int = 1,  # Iteration
         steps: int = 20,
         cfg_scale: float = 7,
         width: int = 512,
         height: int = 512,
         restore_faces: bool = False,
         include_init_images: bool = True,
-        override_settings: Dict[str, Any] = None, 
-        override_settings_restore_afterwards: bool = True):
-        
+        override_settings: Dict[str, Any] = None,
+        override_settings_restore_afterwards: bool = True,
+    ):
         if self.show_deprecation_warning:
             self.print_deprecation_warning()
 
         init_images_b64 = [raw_b64_img(x) for x in init_images]
         controlnet_input_image_b64 = [raw_b64_img(x) for x in controlnet_input_image]
         controlnet_mask_b64 = [raw_b64_img(x) for x in controlnet_mask]
 
@@ -894,12 +997,12 @@
             "width": width,
             "height": height,
             "restore_faces": restore_faces,
             "include_init_images": include_init_images,
             "override_settings": override_settings,
             "override_settings_restore_afterwards": override_settings_restore_afterwards,
         }
-        return self.api.custom_post('controlnet/img2img', payload=payload)
-    
+        return self.api.custom_post("controlnet/img2img", payload=payload)
+
     def model_list(self):
-        r = self.api.custom_get('controlnet/model_list')
-        return r['model_list']
+        r = self.api.custom_get("controlnet/model_list")
+        return r["model_list"]
```

## Comparing `webuiapi-0.8.1.dist-info/LICENSE` & `webuiapi-0.9.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `webuiapi-0.8.1.dist-info/METADATA` & `webuiapi-0.9.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webuiapi
-Version: 0.8.1
+Version: 0.9.0
 Summary: Python API client for AUTOMATIC1111/stable-diffusion-webui
 Home-page: https://github.com/mix1009/sdwebuiapi
 Author: ChunKoo Park
 Author-email: mix1009@gmail.com
 License: MIT
 Keywords: stable-diffuion-webui,AUTOMATIC1111,stable-diffusion,api
 Requires-Python: >=3.7, <4
```

