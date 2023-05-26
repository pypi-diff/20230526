# Comparing `tmp/mys_goods_tool-2.0.3.tar.gz` & `tmp/mys_goods_tool-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mys_goods_tool-2.0.3.tar", max compression
+gzip compressed data, was "mys_goods_tool-2.0.4.tar", max compression
```

## Comparing `mys_goods_tool-2.0.3.tar` & `mys_goods_tool-2.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1065 2023-05-12 23:53:05.629523 mys_goods_tool-2.0.3/LICENSE
--rw-r--r--   0        0        0     4239 2023-05-12 23:53:05.629523 mys_goods_tool-2.0.3/README.md
--rw-r--r--   0        0        0        0 2023-05-12 23:53:05.629523 mys_goods_tool-2.0.3/mys_goods_tool/__init__.py
--rw-r--r--   0        0        0     2226 2023-05-12 23:53:05.629523 mys_goods_tool-2.0.3/mys_goods_tool/__main__.py
--rw-r--r--   0        0        0    56571 2023-05-12 23:53:05.629523 mys_goods_tool-2.0.3/mys_goods_tool/api.py
--rw-r--r--   0        0        0     5536 2023-05-12 23:53:05.629523 mys_goods_tool-2.0.3/mys_goods_tool/custom_css.py
--rw-r--r--   0        0        0     7599 2023-05-12 23:53:05.629523 mys_goods_tool-2.0.3/mys_goods_tool/custom_widget.py
--rw-r--r--   0        0        0     9176 2023-05-12 23:53:05.629523 mys_goods_tool-2.0.3/mys_goods_tool/data_model.py
--rw-r--r--   0        0        0    15247 2023-05-12 23:53:05.629523 mys_goods_tool-2.0.3/mys_goods_tool/exchange_mode.py
--rw-r--r--   0        0        0    43505 2023-05-12 23:53:05.629523 mys_goods_tool-2.0.3/mys_goods_tool/exchange_plan_view.py
--rw-r--r--   0        0        0     6442 2023-05-12 23:53:05.629523 mys_goods_tool-2.0.3/mys_goods_tool/geetest-webui/gt4-localized.html
--rw-r--r--   0        0        0     6501 2023-05-12 23:53:05.629523 mys_goods_tool-2.0.3/mys_goods_tool/geetest-webui/gt4.html
--rw-r--r--   0        0        0     6840 2023-05-12 23:53:05.629523 mys_goods_tool-2.0.3/mys_goods_tool/geetest-webui/index.html
--rw-r--r--   0        0        0    10861 2023-05-12 23:53:05.629523 mys_goods_tool-2.0.3/mys_goods_tool/geetest-webui/libs/gt.js
--rw-r--r--   0        0        0    14792 2023-05-12 23:53:05.629523 mys_goods_tool-2.0.3/mys_goods_tool/geetest-webui/libs/gt4.js
--rw-r--r--   0        0        0   366500 2023-05-12 23:53:05.633524 mys_goods_tool-2.0.3/mys_goods_tool/geetest-webui/libs/jquery.js
--rw-r--r--   0        0        0     6910 2023-05-12 23:53:05.633524 mys_goods_tool-2.0.3/mys_goods_tool/geetest-webui/localized.html
--rw-r--r--   0        0        0     9157 2023-05-12 23:53:05.633524 mys_goods_tool-2.0.3/mys_goods_tool/geetest.py
--rw-r--r--   0        0        0    21679 2023-05-12 23:53:05.633524 mys_goods_tool-2.0.3/mys_goods_tool/login_view.py
--rw-r--r--   0        0        0    13119 2023-05-12 23:53:05.633524 mys_goods_tool-2.0.3/mys_goods_tool/tui.py
--rw-r--r--   0        0        0    17830 2023-05-12 23:53:05.633524 mys_goods_tool-2.0.3/mys_goods_tool/user_data.py
--rw-r--r--   0        0        0    11385 2023-05-12 23:53:05.633524 mys_goods_tool-2.0.3/mys_goods_tool/utils.py
--rw-r--r--   0        0        0     1639 2023-05-12 23:53:05.633524 mys_goods_tool-2.0.3/pyproject.toml
--rw-r--r--   0        0        0     5672 1970-01-01 00:00:00.000000 mys_goods_tool-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-26 19:18:19.810899 mys_goods_tool-2.0.4/LICENSE
+-rw-r--r--   0        0        0     3972 2023-05-26 19:18:19.810899 mys_goods_tool-2.0.4/README.md
+-rw-r--r--   0        0        0        0 2023-05-26 19:18:19.810899 mys_goods_tool-2.0.4/mys_goods_tool/__init__.py
+-rw-r--r--   0        0        0     2226 2023-05-26 19:18:19.810899 mys_goods_tool-2.0.4/mys_goods_tool/__main__.py
+-rw-r--r--   0        0        0    58103 2023-05-26 19:18:19.810899 mys_goods_tool-2.0.4/mys_goods_tool/api.py
+-rw-r--r--   0        0        0     5536 2023-05-26 19:18:19.810899 mys_goods_tool-2.0.4/mys_goods_tool/custom_css.py
+-rw-r--r--   0        0        0     7599 2023-05-26 19:18:19.810899 mys_goods_tool-2.0.4/mys_goods_tool/custom_widget.py
+-rw-r--r--   0        0        0     9570 2023-05-26 19:18:19.810899 mys_goods_tool-2.0.4/mys_goods_tool/data_model.py
+-rw-r--r--   0        0        0    17597 2023-05-26 19:18:19.810899 mys_goods_tool-2.0.4/mys_goods_tool/exchange_mode.py
+-rw-r--r--   0        0        0    43505 2023-05-26 19:18:19.810899 mys_goods_tool-2.0.4/mys_goods_tool/exchange_plan_view.py
+-rw-r--r--   0        0        0     6910 2023-05-26 19:18:19.810899 mys_goods_tool-2.0.4/mys_goods_tool/geetest-webui/gt3-localized.html
+-rw-r--r--   0        0        0     6840 2023-05-26 19:18:19.810899 mys_goods_tool-2.0.4/mys_goods_tool/geetest-webui/gt3.html
+-rw-r--r--   0        0        0     6890 2023-05-26 19:18:19.810899 mys_goods_tool-2.0.4/mys_goods_tool/geetest-webui/index.html
+-rw-r--r--   0        0        0    10861 2023-05-26 19:18:19.810899 mys_goods_tool-2.0.4/mys_goods_tool/geetest-webui/libs/gt.js
+-rw-r--r--   0        0        0    14792 2023-05-26 19:18:19.810899 mys_goods_tool-2.0.4/mys_goods_tool/geetest-webui/libs/gt4.js
+-rw-r--r--   0        0        0   366500 2023-05-26 19:18:19.814899 mys_goods_tool-2.0.4/mys_goods_tool/geetest-webui/libs/jquery.js
+-rw-r--r--   0        0        0     6831 2023-05-26 19:18:19.814899 mys_goods_tool-2.0.4/mys_goods_tool/geetest-webui/localized.html
+-rw-r--r--   0        0        0    10717 2023-05-26 19:18:19.814899 mys_goods_tool-2.0.4/mys_goods_tool/geetest.py
+-rw-r--r--   0        0        0    22544 2023-05-26 19:18:19.814899 mys_goods_tool-2.0.4/mys_goods_tool/login_view.py
+-rw-r--r--   0        0        0    13045 2023-05-26 19:18:19.814899 mys_goods_tool-2.0.4/mys_goods_tool/tui.py
+-rw-r--r--   0        0        0    17824 2023-05-26 19:18:19.814899 mys_goods_tool-2.0.4/mys_goods_tool/user_data.py
+-rw-r--r--   0        0        0    11385 2023-05-26 19:18:19.814899 mys_goods_tool-2.0.4/mys_goods_tool/utils.py
+-rw-r--r--   0        0        0     1639 2023-05-26 19:18:19.814899 mys_goods_tool-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0     5357 1970-01-01 00:00:00.000000 mys_goods_tool-2.0.4/PKG-INFO
```

### Comparing `mys_goods_tool-2.0.3/LICENSE` & `mys_goods_tool-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.0.3/README.md` & `mys_goods_tool-2.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -12,32 +12,28 @@
   <img alt="代码行数" src="https://img.shields.io/tokei/lines/github/Ljzd-PRO/Mys_Goods_Tool?style=for-the-badge">
   <img alt="构建结果" src="https://img.shields.io/github/actions/workflow/status/Ljzd-PRO/Mys_Goods_Tool/build-v2.yml?event=pull_request&style=for-the-badge">
   <img alt="Python版本兼容性测试" src="https://img.shields.io/github/actions/workflow/status/Ljzd-PRO/Mys_Goods_Tool/python-package.yml?event=pull_request&label=Versions%20Test&style=for-the-badge">
 </div>
 
 ### 更新说明
 
-- 修复定时兑换无效的问题
-- 修复失去网络连接的情况下会导致程序退出的Bug
-- 对于 Linux 使用 Ubuntu 20.04 进行构建，防止出现缺少 GNU libc 对应版本的问题
-- 非 Windows 系统增加 [uvloop](https://github.com/MagicStack/uvloop) 支持，提高性能
+- 修复启动后由于商品数据相关问题而导致的崩溃
+- 修复 Linux 实际不会应用 uvloop 的问题
+- 人机验证更新至
+  GT4（但实际上暂时不可用 [#105](https://github.com/Ljzd-PRO/Mys_Goods_Tool/issues/105#issuecomment-1552727784)）
 
 ## 功能和特性
 
 - [x] 使用 [Textual](https://github.com/Textualize/textual) 终端图形界面库，支持 Windows / Linux / macOS 甚至可能是移动端SSH客户端
 - [x] 短信验证码登录（只需接收一次验证码）
 - [x] 内置人机验证页面，无需前往官网验证
 - [x] 多账号支持
 - [x] 支持米游社所有分区的商品兑换
 
 ### TODO
-
-- [ ] 支持在图形界面中编辑偏好设置
-- [ ] 密码登录
-- [ ] 解决SSH客户端无法跳转人机验证链接的问题
 - [ ] 更新至极验第四代适应性验证
 
 ### 预览图
 
 <details>
   <summary>短信验证登录</summary>
   <img src="https://user-images.githubusercontent.com/63289359/235790425-7c502a69-baac-4ced-ba07-d068a88a7ae9.png" alt="短信验证登录页面" />
@@ -75,12 +71,9 @@
 - 仅供学习时参考
 
 - 相似项目推荐:  \
   **mysTool - 米游社辅助工具插件**  \
   简介：NoneBot2 插件 | 米游社工具-每日米游币任务、游戏签到、商品兑换、免抓包登录、原神树脂提醒  \
   🔗 https://github.com/Ljzd-PRO/nonebot-plugin-mystool
 
-- 本项目已开启[🔗Github Actions](https://github.com/Ljzd-PRO/Mys_Goods_Tool/actions)。
-  欢迎[🔗指出Bug](https://github.com/Ljzd-PRO/Mys_Goods_Tool/issues)
-  和[🔗贡献代码](https://github.com/Ljzd-PRO/Mys_Goods_Tool/pulls)👏
-
-- 开发版分支：[🔗dev](https://github.com/Ljzd-PRO/Mys_Goods_Tool/tree/dev/)
+- [🔗Bug 反馈](https://github.com/Ljzd-PRO/Mys_Goods_Tool/issues)  
+- 如果你知道如何修复一些Bug和新增功能，也欢迎提交你的修订代码 [🔗Pull requests](https://github.com/Ljzd-PRO/Mys_Goods_Tool/pulls)
```

### Comparing `mys_goods_tool-2.0.3/mys_goods_tool/__main__.py` & `mys_goods_tool-2.0.4/mys_goods_tool/__main__.py`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.0.3/mys_goods_tool/api.py` & `mys_goods_tool-2.0.4/mys_goods_tool/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from typing import List, Optional, Tuple, Dict, Any, Union
 from urllib.parse import urlencode
 
 import httpx
 import tenacity
-from httpx import ConnectError
 from pydantic import ValidationError, BaseModel
 from requests.utils import dict_from_cookiejar
 
 from mys_goods_tool.data_model import GameRecord, GameInfo, Good, Address, BaseApiStatus, MmtData, GeetestResult, \
     GetCookieStatus, \
-    CreateMobileCaptchaStatus, GetGoodDetailStatus, ExchangeStatus
+    CreateMobileCaptchaStatus, GetGoodDetailStatus, ExchangeStatus, GeetestResultV4
 from mys_goods_tool.user_data import config as conf, UserAccount, BBSCookies, ExchangePlan, ExchangeResult
 from mys_goods_tool.utils import generate_device_id, logger, generate_ds, Subscribe, \
     NtpTime, get_async_retry
 
 URL_LOGIN_TICKET_BY_CAPTCHA = "https://webapi.account.mihoyo.com/Api/login_by_mobilecaptcha"
 URL_LOGIN_TICKET_BY_PASSWORD = "https://webapi.account.mihoyo.com/Api/login_by_password"
 URL_MULTI_TOKEN_BY_LOGIN_TICKET = "https://api-takumi.mihoyo.com/auth/api/getMultiTokenByLoginTicket?login_ticket={0}&token_types=3&uid={1}"
@@ -282,15 +281,15 @@
         return self.retcode == 1 or self.message in ["成功", "OK"]
 
     @property
     def wrong_captcha(self):
         """
         是否返回验证码错误
         """
-        return self.retcode == -201 or self.message in ["验证码错误", "Captcha not match Err"]
+        return self.retcode in [-201, -302] or self.message in ["验证码错误", "Captcha not match Err"]
 
     @property
     def login_expired(self):
         """
         是否返回登录失效
         """
         return self.retcode in [-100, 10001] or self.message in ["登录失效，请重新登录"]
@@ -627,116 +626,150 @@
             return BaseApiStatus(incorrect_return=True), None
         else:
             logger.exception(f"获取地址数据 - 请求失败")
             return BaseApiStatus(network_error=True), None
     return BaseApiStatus(success=True), address_list
 
 
-async def check_registrable(phone_number: int, retry: bool = True) -> Tuple[BaseApiStatus, Optional[bool]]:
+async def check_registrable(phone_number: int, keep_client: bool = False, retry: bool = True) -> Tuple[
+    BaseApiStatus, Optional[bool], str, Optional[httpx.AsyncClient]]:
     """
     检查用户是否可以注册
 
+    :param keep_client: httpx.AsyncClient 连接是否需要关闭
     :param phone_number: 手机号
     :param retry: 是否允许重试
+    :return: (API返回状态, 用户是否可以注册, 设备ID, httpx.AsyncClient连接对象)
     """
     headers = HEADERS_WEBAPI.copy()
-    headers["x-rpc-device_id"] = generate_device_id()
+    device_id = generate_device_id()
+    headers["x-rpc-device_id"] = device_id
+
+    async def request():
+        """
+        发送请求的闭包函数
+        """
+        time_now = round(NtpTime.time() * 1000)
+        # await client.options(URL_REGISTRABLE.format(mobile=phone_number, t=time_now),
+        #                      headers=headers, timeout=conf.preference.timeout)
+        return await client.get(URL_REGISTRABLE.format(mobile=phone_number, t=time_now),
+                                headers=headers, timeout=conf.preference.timeout)
+
     try:
         async for attempt in get_async_retry(retry):
             with attempt:
-                async with httpx.AsyncClient() as client:
-                    res = await client.get(URL_REGISTRABLE.format(mobile=phone_number, t=round(NtpTime.time() * 1000)),
-                                           headers=headers, timeout=conf.preference.timeout)
-                    api_result = ApiResultHandler(res.json())
-                return BaseApiStatus(success=True), bool(api_result.data["is_registable"])
+                if keep_client:
+                    client = httpx.AsyncClient()
+                else:
+                    async with httpx.AsyncClient() as client:
+                        res = await request()
+                res = await request()
+                api_result = ApiResultHandler(res.json())
+                return BaseApiStatus(success=True), bool(api_result.data["is_registable"]), device_id, client
     except tenacity.RetryError as e:
+        if keep_client:
+            await client.aclose()
         if is_incorrect_return(e):
             logger.exception(f"检查用户 {phone_number} 是否可以注册 - 服务器没有正确返回")
             logger.debug(f"网络请求返回: {res.text}")
-            return BaseApiStatus(incorrect_return=True), None
+            return BaseApiStatus(incorrect_return=True), None, device_id, client
         else:
             logger.exception(f"检查用户 {phone_number} 是否可以注册 - 请求失败")
-            return BaseApiStatus(network_error=True), None
+            return BaseApiStatus(network_error=True), None, device_id, None
 
 
-async def create_mmt(keep_client: bool = False, retry: bool = True) -> Tuple[
-    BaseApiStatus, Optional[MmtData], Optional[httpx.AsyncClient]]:
+async def create_mmt(client: Optional[httpx.AsyncClient] = None,
+                     use_v4: bool = True,
+                     device_id: str = generate_device_id(),
+                     retry: bool = True) -> Tuple[
+    BaseApiStatus, Optional[MmtData], str, Optional[httpx.AsyncClient]]:
     """
     发送短信验证前所需的人机验证任务申请
 
-    :param keep_client: httpx.AsyncClient 连接是否需要关闭
+    :param client: httpx.AsyncClient 连接
+    :param use_v4: 是否使用极验第四代人机验证
+    :param device_id: 设备 ID
     :param retry: 是否允许重试
+    :return: (API返回状态, 人机验证任务数据, 设备ID, httpx.AsyncClient连接对象)
     """
     headers = HEADERS_WEBAPI.copy()
-    headers["x-rpc-device_id"] = generate_device_id()
-
+    headers["x-rpc-device_id"] = device_id
+    if use_v4:
+        headers.setdefault("x-rpc-source", "accountWebsite")
     async def request():
         """
         发送请求的闭包函数
         """
         time_now = round(NtpTime.time() * 1000)
-        await client.options(URL_CREATE_MMT.format(now=time_now, t=time_now),
-                             headers=headers, timeout=conf.preference.timeout)
+        # await client.options(URL_CREATE_MMT.format(now=time_now, t=time_now),
+        #                      headers=headers, timeout=conf.preference.timeout)
         return await client.get(URL_CREATE_MMT.format(now=time_now, t=time_now),
                                 headers=headers, timeout=conf.preference.timeout)
 
     try:
         async for attempt in get_async_retry(retry):
             with attempt:
-                if keep_client:
-                    client = httpx.AsyncClient()
+                if client:
                     res = await request()
                 else:
                     async with httpx.AsyncClient() as client:
                         res = await request()
                 api_result = ApiResultHandler(res.json())
-                return BaseApiStatus(success=True), MmtData.parse_obj(api_result.data["mmt_data"]), client
+                return BaseApiStatus(success=True), MmtData.parse_obj(api_result.data["mmt_data"]), device_id, client
     except tenacity.RetryError as e:
-        if keep_client:
+        if client:
             await client.aclose()
         if is_incorrect_return(e):
             logger.exception(f"获取短信验证-人机验证任务(create_mmt) - 服务器没有正确返回")
             logger.debug(f"网络请求返回: {res.text}")
-            return BaseApiStatus(incorrect_return=True), None, client
+            return BaseApiStatus(incorrect_return=True), None, device_id, client
         else:
             logger.exception(f"获取短信验证-人机验证任务(create_mmt) - 请求失败")
-            return BaseApiStatus(network_error=True), None, None
-    except ConnectError:
-        if keep_client:
-            await client.aclose()
-        logger.exception(f"获取短信验证-人机验证任务(create_mmt) - 网络连接失败")
-        return BaseApiStatus(network_error=True), None, None
+            return BaseApiStatus(network_error=True), None, device_id, None
 
 
 async def create_mobile_captcha(phone_number: int,
                                 mmt_data: MmtData,
-                                geetest_result: GeetestResult,
+                                geetest_result: Union[GeetestResult, GeetestResultV4],
                                 client: Optional[httpx.AsyncClient] = None,
+                                use_v4: bool = True,
+                                device_id: str = generate_device_id(),
                                 retry: bool = True
                                 ) -> Tuple[CreateMobileCaptchaStatus, Optional[httpx.AsyncClient]]:
     """
     发送短信验证码
 
     :param phone_number: 手机号
     :param mmt_data: 人机验证任务数据
     :param geetest_result: 人机验证结果数据
     :param client: httpx.AsyncClient 连接
+    :param use_v4: 是否使用极验第四代人机验证
+    :param device_id: 设备 ID
     :param retry: 是否允许重试
     """
     headers = HEADERS_WEBAPI.copy()
-    headers["x-rpc-device_id"] = generate_device_id()
-    params = {
-        "action_type": "login",
-        "mmt_key": mmt_data.mmt_key,
-        "geetest_challenge": mmt_data.challenge,
-        "geetest_validate": geetest_result.validate,
-        "geetest_seccode": geetest_result.seccode,
-        "mobile": phone_number,
-        "t": round(NtpTime.time() * 1000)
-    }
+    headers["x-rpc-device_id"] = device_id
+    if use_v4 and isinstance(geetest_result, GeetestResultV4):
+        params = {
+            "action_type": "login",
+            "mmt_key": mmt_data.mmt_key,
+            "geetest_v4_data": geetest_result.dict(skip_defaults=True),
+            "mobile": phone_number,
+            "t": round(NtpTime.time() * 1000)
+        }
+    else:
+        params = {
+            "action_type": "login",
+            "mmt_key": mmt_data.mmt_key,
+            "geetest_challenge": mmt_data.challenge,
+            "geetest_validate": geetest_result.validate,
+            "geetest_seccode": geetest_result.seccode,
+            "mobile": phone_number,
+            "t": round(NtpTime.time() * 1000)
+        }
     encoded_params = urlencode(params)
 
     async def request():
         """
         发送请求的闭包函数
         """
         return await client.post(URL_CREATE_MOBILE_CAPTCHA,
@@ -748,15 +781,15 @@
         async for attempt in get_async_retry(retry):
             with attempt:
                 # FIXME 2023/4/13: 似乎会导致卡在连接状态，暂时弃用
                 #   res = await client.options(URL_CREATE_MOBILE_CAPTCHA,
                 #                            headers=headers,
                 #                            timeout=conf.preference.timeout)
                 #   cookies.update(res.cookies)
-                if client is not None:
+                if client and not client.is_closed:
                     res = await request()
                 else:
                     async with httpx.AsyncClient() as client:
                         res = await request()
                 api_result = ApiResultHandler(res.json())
                 if api_result.success:
                     return CreateMobileCaptchaStatus(success=True), client
```

### Comparing `mys_goods_tool-2.0.3/mys_goods_tool/custom_css.py` & `mys_goods_tool-2.0.4/mys_goods_tool/custom_css.py`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.0.3/mys_goods_tool/custom_widget.py` & `mys_goods_tool-2.0.4/mys_goods_tool/custom_widget.py`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.0.3/mys_goods_tool/data_model.py` & `mys_goods_tool-2.0.4/mys_goods_tool/data_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,16 +65,16 @@
     sale_start_time: Optional[str]
     time_by_detail: Optional[int]
     next_num: Optional[int]
     account_exchange_num: int
     """已经兑换次数"""
     account_cycle_limit: int
     """最多可兑换次数"""
-    account_cycle_type: Literal["forever", "month"]
-    """限购类型"""
+    account_cycle_type: str
+    """限购类型 Literal["forever", "month", "not_limit"]"""
     game_biz: Optional[str]
     """商品对应的游戏区服（如 hk4e_cn）（单独查询一个商品时）"""
     game: Optional[str]
     """商品对应的游戏"""
     unlimit: Optional[bool]
     """是否为不限量商品"""
 
@@ -283,18 +283,23 @@
         return self.connect_areacode + " " + self.connect_mobile
 
 
 class MmtData(BaseModel):
     """
     短信验证码-人机验证任务申请-返回数据
     """
-    challenge: str
+    challenge: Optional[str]
     gt: str
     mmt_key: str
     new_captcha: bool
+    risk_type: Optional[str]
+    """任务类型，如滑动拼图 slide"""
+    success: Optional[int]
+    use_v4: Optional[bool]
+    """是否使用极验第四代 GT4"""
 
 
 class BaseApiStatus(BaseModel):
     """
     API返回结果基类
     """
     success = False
@@ -370,7 +375,18 @@
     """未进行兑换任务初始化"""
     account_not_found = False
     """账号不存在"""
 
 
 GeetestResult = NamedTuple("GeetestResult", validate=str, seccode=str)
 """人机验证结果数据"""
+
+
+class GeetestResultV4(BaseModel):
+    """
+    GEETEST GT4 人机验证结果数据
+    """
+    captcha_id: str
+    lot_number: str
+    pass_token: str
+    gen_time: int
+    captcha_output: str
```

### Comparing `mys_goods_tool-2.0.3/mys_goods_tool/exchange_mode.py` & `mys_goods_tool-2.0.4/mys_goods_tool/exchange_mode.py`

 * *Files 10% similar despite different names*

```diff
@@ -118,44 +118,64 @@
 
     @lambda func: scheduler.add_listener(func, EVENT_JOB_EXECUTED)
     def on_executed(event: JobExecutionEvent):
         """
         接收兑换结果
         """
         if event.job_id.startswith("exchange-plan"):
+            thread_id = int(event.job_id.split('-')[-1])
             result: Tuple[ExchangeStatus, Optional[ExchangeResult]] = event.retval
             exchange_status, exchange_result = result
-            plan = exchange_result.plan
 
-            with lock:
-                # 如果已经有一个线程兑换成功，就不再接收结果
-                if True not in finished[plan]:
-                    thread_id = int(event.job_id.split('-')[-1])
-                    if exchange_result.result:
-                        finished[plan].append(True)
-                        logger.info(
-                            f"用户 {plan.account.bbs_uid}"
-                            f" - {plan.good.general_name}"
-                            f" - 线程 {thread_id}"
-                            f" - 兑换成功")
-                    else:
-                        finished[plan].append(False)
-                        logger.error(
-                            f"用户 {plan.account.bbs_uid}"
-                            f" - {plan.good.general_name}"
-                            f" - 线程 {thread_id}"
-                            f" - 兑换失败")
+            if not exchange_status:
+                hash_value = int(event.job_id.split('-')[-2])
+                plan = filter(lambda x: x.__hash__() == hash_value, conf.exchange_plans)
+                plan = next(plan)
+                with lock:
+                    finished[plan].append(False)
+                    logger.error(
+                        f"用户 {plan.account.bbs_uid}"
+                        f" - {plan.good.general_name}"
+                        f" - 线程 {thread_id}"
+                        f" - 兑换请求发送失败")
+                    if len(finished[plan]) == conf.preference.exchange_thread_count:
+                        try:
+                            conf.exchange_plans.remove(plan)
+                        except KeyError:
+                            pass
+                        else:
+                            conf.save()
+
+            else:
+                plan = exchange_result.plan
+                with lock:
+                    # 如果已经有一个线程兑换成功，就不再接收结果
+                    if True not in finished[plan]:
+                        if exchange_result.result:
+                            finished[plan].append(True)
+                            logger.info(
+                                f"用户 {plan.account.bbs_uid}"
+                                f" - {plan.good.general_name}"
+                                f" - 线程 {thread_id}"
+                                f" - 兑换成功")
+                        else:
+                            finished[plan].append(False)
+                            logger.error(
+                                f"用户 {plan.account.bbs_uid}"
+                                f" - {plan.good.general_name}"
+                                f" - 线程 {thread_id}"
+                                f" - 兑换失败")
 
-                if len(finished[plan]) == conf.preference.exchange_thread_count:
-                    try:
-                        conf.exchange_plans.remove(plan)
-                    except KeyError:
-                        pass
-                    else:
-                        conf.save()
+                    if len(finished[plan]) == conf.preference.exchange_thread_count:
+                        try:
+                            conf.exchange_plans.remove(plan)
+                        except KeyError:
+                            pass
+                        else:
+                            conf.save()
 
         elif event.job_id == "exchange-connection_test":
             result: Union[float, bool, None] = event.retval
             if result:
                 print(
                     f"Ping 商品兑换API服务器 {_get_api_host() or 'N/A'} - 延迟 {round(result, 2) if result else 'N/A'} ms")
 
@@ -273,49 +293,70 @@
         """
         接收兑换结果
         """
         try:
             if event.job_id.startswith("exchange-plan"):
                 result: Tuple[ExchangeStatus, Optional[ExchangeResult]] = event.retval
                 exchange_status, exchange_result = result
-                plan = exchange_result.plan
-
-                with cls.lock:
-                    # 如果已经有一个线程兑换成功，就不再接收结果
-                    if True not in cls.finished[plan]:
-                        row = ExchangeResultRow.rows[plan]
-                        thread_id = int(event.job_id.split('-')[-1])
-
-                        if exchange_result.result:
-                            cls.finished[plan].append(True)
-                            logger.info(
-                                f"用户 {plan.account.bbs_uid}"
-                                f" - {plan.good.general_name}"
-                                f" - 线程 {thread_id}"
-                                f" - 兑换成功")
-                            text = f"[bold green]🎉 线程 {thread_id} - 兑换成功[/] "
-                        else:
-                            cls.finished[plan].append(False)
-                            logger.error(
-                                f"用户 {plan.account.bbs_uid}"
-                                f" - {plan.good.general_name}"
-                                f" - 线程 {thread_id}"
-                                f" - 兑换失败")
-                            text = f"[bold red]💦 线程 {thread_id} - 兑换失败[/] "
-
+                thread_id = int(event.job_id.split('-')[-1])
+                if not exchange_status:
+                    hash_value = int(event.job_id.split('-')[-2])
+                    plan = filter(lambda x: x.__hash__() == hash_value, conf.exchange_plans)
+                    plan = next(plan)
+                    row = ExchangeResultRow.rows[plan]
+                    with cls.lock:
+                        cls.finished[plan].append(False)
+                        logger.error(
+                            f"用户 {plan.account.bbs_uid}"
+                            f" - {plan.good.general_name}"
+                            f" - 线程 {thread_id}"
+                            f" - 兑换失败")
+                        text = f"[bold red]💦 线程 {thread_id} - 兑换请求失败[/] "
                         row.result_preview._add_children(ExchangeResultRow.get_result_static(text))
                         row.result_preview.refresh()
-
-                    if len(cls.finished[plan]) == conf.preference.exchange_thread_count:
-                        try:
-                            conf.exchange_plans.remove(plan)
-                        except KeyError:
-                            pass
-                        else:
-                            conf.save()
+                        if len(cls.finished[plan]) == conf.preference.exchange_thread_count:
+                            try:
+                                conf.exchange_plans.remove(plan)
+                            except KeyError:
+                                pass
+                            else:
+                                conf.save()
+                else:
+                    plan = exchange_result.plan
+                    with cls.lock:
+                        # 如果已经有一个线程兑换成功，就不再接收结果
+                        if True not in cls.finished[plan]:
+                            row = ExchangeResultRow.rows[plan]
+                            if exchange_result.result:
+                                cls.finished[plan].append(True)
+                                logger.info(
+                                    f"用户 {plan.account.bbs_uid}"
+                                    f" - {plan.good.general_name}"
+                                    f" - 线程 {thread_id}"
+                                    f" - 兑换成功")
+                                text = f"[bold green]🎉 线程 {thread_id} - 兑换成功[/] "
+                            else:
+                                cls.finished[plan].append(False)
+                                logger.error(
+                                    f"用户 {plan.account.bbs_uid}"
+                                    f" - {plan.good.general_name}"
+                                    f" - 线程 {thread_id}"
+                                    f" - 兑换失败")
+                                text = f"[bold red]💦 线程 {thread_id} - 兑换失败[/] "
+
+                            row.result_preview._add_children(ExchangeResultRow.get_result_static(text))
+                            row.result_preview.refresh()
+
+                        if len(cls.finished[plan]) == conf.preference.exchange_thread_count:
+                            try:
+                                conf.exchange_plans.remove(plan)
+                            except KeyError:
+                                pass
+                            else:
+                                conf.save()
         except:
             logger.exception("接收兑换结果失败")
 
     async def _on_button_pressed(self, event: ControllableButton.Pressed):
         if event.button.id == "button-exchange_mode-enter":
             await self.update_data()
             self.button_refresh.disable()
```

### Comparing `mys_goods_tool-2.0.3/mys_goods_tool/exchange_plan_view.py` & `mys_goods_tool-2.0.4/mys_goods_tool/exchange_plan_view.py`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.0.3/mys_goods_tool/geetest-webui/gt4-localized.html` & `mys_goods_tool-2.0.4/mys_goods_tool/geetest-webui/index.html`

 * *Files 8% similar despite different names*

```diff
@@ -76,17 +76,17 @@
                 <h3>description: </h3>
                 <p id="errorDescription"></p>
             </div>
         </div>
     </div>
 </form>
 
-<script src="/libs/jquery.js"></script>
+<script src="https://apps.bdimg.com/libs/jquery/1.9.1/jquery.js"></script>
 <!-- 引入 gt4.js，既可以使用其中提供的 initGeetest4 初始化函数 -->
-<script src="/libs/gt4.js"></script>
+<script src="https://static.geetest.com/v4/gt4.js"></script>
 <script>
     let success = false;
 
     /**
      * 显示错误信息
      * @param {string} text 提示文本
      * @param {Error} error 错误对象
@@ -137,30 +137,44 @@
     }
 
 
     function start() {
         const queryString = window.location.search;
         const urlParams = new URLSearchParams(queryString);
         const gt = urlParams.get('gt');
+        const mmtKey = urlParams.get('mmtKey');
+        let riskType = urlParams.get('riskType');
 
         let wait = $("#wait");
 
         if (!gt) {
             displayError("URL参数需要提供 gt");
             return alert("URL参数需要提供 gt");
         }
+        if (!mmtKey) {
+            displayError("URL参数需要提供 mmtKey");
+            return alert("URL参数需要提供 mmtKey");
+        }
+        riskType = riskType || "slide";
 
         wait.show();
 
         // 调用 initGeetest 进行初始化
         // 参数1：配置参数
         // 参数2：回调，回调的第一个参数验证码对象，之后可以使用它调用相应的接口
         initGeetest4({
             captchaId: gt,
-            product: "popup"
+            riskType: riskType,
+            timeout: 1e4,
+            language: "zho",
+            product: "popup",
+            hideSuccess: !0,
+            userInfo: JSON.stringify({
+                mmt_key: mmtKey
+            }),
             // 更多前端配置参数说明参见：https://docs.geetest.com/gt4/apirefer/api/web/#%E9%85%8D%E7%BD%AE%E5%8F%82%E6%95%B0
         }, function (captchaObj) {
             captchaObj.appendTo('#captcha');
             captchaObj.onError(function (error) {
                 if (error.code === "error_02") {
                     displayError("使用了旧的验证任务数据，请尝试重新申请人机验证任务", error);
                 } else if (error.code === "error_21") {
@@ -168,16 +182,14 @@
                 } else {
                     displayError("生成验证任务失败", error);
                 }
             });
             captchaObj.onReady(function () {
                 $("#wait").hide();
             });
-            // 更多前端接口说明请参见：http://docs.geetest.com/install/client/web-front/
-
             setInterval(function () {
                 const result = captchaObj.getValidate();
                 if (result && !success) {
                     success = true;
                     displayGeetestResult("已成功获取验证结果", result);
                     $.ajax({
                         url: "/result",
```

### Comparing `mys_goods_tool-2.0.3/mys_goods_tool/geetest-webui/gt4.html` & `mys_goods_tool-2.0.4/mys_goods_tool/geetest-webui/localized.html`

 * *Files 14% similar despite different names*

```diff
@@ -76,17 +76,17 @@
                 <h3>description: </h3>
                 <p id="errorDescription"></p>
             </div>
         </div>
     </div>
 </form>
 
-<script src="https://apps.bdimg.com/libs/jquery/1.9.1/jquery.js"></script>
+<script src="/libs/jquery.js"></script>
 <!-- 引入 gt4.js，既可以使用其中提供的 initGeetest4 初始化函数 -->
-<script src="https://static.geetest.com/v4/gt4.js"></script>
+<script src="/libs/gt4.js"></script>
 <script>
     let success = false;
 
     /**
      * 显示错误信息
      * @param {string} text 提示文本
      * @param {Error} error 错误对象
@@ -137,30 +137,44 @@
     }
 
 
     function start() {
         const queryString = window.location.search;
         const urlParams = new URLSearchParams(queryString);
         const gt = urlParams.get('gt');
+        const mmtKey = urlParams.get('mmtKey');
+        let riskType = urlParams.get('riskType');
 
         let wait = $("#wait");
 
         if (!gt) {
             displayError("URL参数需要提供 gt");
             return alert("URL参数需要提供 gt");
         }
+        if (!mmtKey) {
+            displayError("URL参数需要提供 mmtKey");
+            return alert("URL参数需要提供 mmtKey");
+        }
+        riskType = riskType || "slide";
 
         wait.show();
 
         // 调用 initGeetest 进行初始化
         // 参数1：配置参数
         // 参数2：回调，回调的第一个参数验证码对象，之后可以使用它调用相应的接口
         initGeetest4({
             captchaId: gt,
-            product: "popup"
+            riskType: riskType,
+            timeout: 1e4,
+            language: "zho",
+            product: "popup",
+            hideSuccess: !0,
+            userInfo: JSON.stringify({
+                mmt_key: mmtKey
+            }),
             // 更多前端配置参数说明参见：https://docs.geetest.com/gt4/apirefer/api/web/#%E9%85%8D%E7%BD%AE%E5%8F%82%E6%95%B0
         }, function (captchaObj) {
             captchaObj.appendTo('#captcha');
             captchaObj.onError(function (error) {
                 if (error.code === "error_02") {
                     displayError("使用了旧的验证任务数据，请尝试重新申请人机验证任务", error);
                 } else if (error.code === "error_21") {
@@ -168,16 +182,14 @@
                 } else {
                     displayError("生成验证任务失败", error);
                 }
             });
             captchaObj.onReady(function () {
                 $("#wait").hide();
             });
-            // 更多前端接口说明请参见：http://docs.geetest.com/install/client/web-front/
-
             setInterval(function () {
                 const result = captchaObj.getValidate();
                 if (result && !success) {
                     success = true;
                     displayGeetestResult("已成功获取验证结果", result);
                     $.ajax({
                         url: "/result",
```

### Comparing `mys_goods_tool-2.0.3/mys_goods_tool/geetest-webui/index.html` & `mys_goods_tool-2.0.4/mys_goods_tool/geetest-webui/gt3.html`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.0.3/mys_goods_tool/geetest-webui/libs/gt.js` & `mys_goods_tool-2.0.4/mys_goods_tool/geetest-webui/libs/gt.js`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.0.3/mys_goods_tool/geetest-webui/libs/gt4.js` & `mys_goods_tool-2.0.4/mys_goods_tool/geetest-webui/libs/gt4.js`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.0.3/mys_goods_tool/geetest-webui/libs/jquery.js` & `mys_goods_tool-2.0.4/mys_goods_tool/geetest-webui/libs/jquery.js`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.0.3/mys_goods_tool/geetest-webui/localized.html` & `mys_goods_tool-2.0.4/mys_goods_tool/geetest-webui/gt3-localized.html`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.0.3/mys_goods_tool/geetest.py` & `mys_goods_tool-2.0.4/mys_goods_tool/geetest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 import asyncio
 import json
 import os
 import threading
 import traceback
-from http.server import HTTPServer, SimpleHTTPRequestHandler, ThreadingHTTPServer
+from http.server import HTTPServer, ThreadingHTTPServer, CGIHTTPRequestHandler
+from json import JSONDecodeError
 from multiprocessing import Pipe, Manager, connection
 from pathlib import Path
 from queue import Queue
 from threading import Thread
-from typing import Any, Optional, Callable, Tuple
+from typing import Any, Optional, Callable, Tuple, Union
 from urllib import parse
 
-from mys_goods_tool.data_model import GeetestResult
+from pydantic import ValidationError
+
+from mys_goods_tool.data_model import GeetestResult, GeetestResultV4
 from mys_goods_tool.user_data import config as conf
 from mys_goods_tool.utils import logger, get_free_port, ProcessManager
 
 STATIC_DIRECTORY = Path(__file__).resolve().with_name(
     "geetest-webui") if not conf.preference.geetest_statics_path else conf.preference.geetest_statics_path
 
 
-class GeetestHandler(SimpleHTTPRequestHandler):
-    result_callback: Callable[[GeetestResult], Any]
+class GeetestHandler(CGIHTTPRequestHandler):
+    result_callback: Callable[[Union[GeetestResult, GeetestResultV4]], Any]
     """接收验证结果数据的回调函数"""
+    error_content_type = "application/json"
 
     def log_message(self, format: str, *args: Any) -> None:
         """
         重写父类方法，更改日志输出到loguru
 
         Log an arbitrary message.
 
@@ -39,38 +43,54 @@
         printf!).
 
         The client ip and current date/time are prefixed to
         every message.
         """
         logger.debug(f"HttpServer: {self.address_string()} - - {format % args}")
 
+    def response_ok(self):
+        response = {"code": 200, "message": "OK. Server received"}
+        self.send_response(200, response["message"])
+        self.send_header("Content-Type", "application/json")
+        self.end_headers()
+        self.wfile.write(json.dumps(response).encode())
+
+    def send_error(self, code: int, message: str = None, explain: str = None, to_json: bool = False) -> None:
+        """
+        重写父类方法，返回json格式的错误信息
+        """
+        if to_json:
+            self.send_response(code, message)
+            self.send_header("Content-Type", self.error_content_type)
+            self.end_headers()
+            response = {"code": code, "msg": message, "desc": explain}
+            self.wfile.write(json.dumps(response).encode())
+        else:
+            super().send_error(code, message, explain)
+
     def do_GET(self):
         file_path = self.path
         try:
             if self.path == "/" or not self.path:
                 # 重定向到默认文件
                 self.path = "/index.html"
             elif self.path.startswith("/result"):
                 # 接收验证结果
                 params = parse.parse_qs(parse.urlparse(self.path).query)
                 seccode = params.get("seccode")
                 validate = params.get("validate")
                 if not seccode or not validate:
                     logger.error(
                         f"HTTP服务器 - 收到 {self.address_string()} 的验证结果，但URL参数缺少 seccode 和 validate")
-                    self.send_error(400, "Bad request, missing URL params `seccode` and `validate`")
+                    self.send_error(400, "Bad request, missing URL params `seccode` and `validate`", to_json=True)
                 else:
                     geetest_result = GeetestResult(seccode=seccode[0], validate=validate[0])
                     logger.info(f"HTTP服务器 - 收到 {self.address_string()} 的验证结果 - {geetest_result}")
                     self.result_callback(geetest_result)
-                    response = {"code": 200, "message": "OK. Server received"}
-                    self.send_response(200, response["message"])
-                    self.send_header("Content-Type", "application/json")
-                    self.end_headers()
-                    self.wfile.write(json.dumps(response).encode())
+                    self.response_ok()
                 return
 
             # 构建文件路径
             file_path = STATIC_DIRECTORY / parse.urlparse(self.path).path[1:]
 
             # 检查文件是否存在并且可读
             if not os.path.isfile(file_path):
@@ -91,14 +111,28 @@
             logger.debug(traceback.format_exc())
             self.send_error(404)
         except Exception:
             logger.error(f"HTTP服务器 - 收到 {self.address_string()} 的请求，但处理请求时发生错误")
             logger.debug(traceback.format_exc())
             self.send_error(500)
 
+    def do_POST(self) -> None:
+        if self.path.startswith("/result"):
+            try:
+                content_length = int(self.headers["Content-Length"])
+                geetest_result = GeetestResultV4.parse_raw(self.rfile.read(content_length))
+            except (ValidationError, JSONDecodeError):
+                logger.exception(
+                    f"HTTP服务器 - 收到 {self.address_string()} 的 gt4 验证结果，但传入数据不符合 GeetestResultV4 模型")
+                self.send_error(400, "Bad request, data not match GeetestResultV4 model", to_json=True)
+            else:
+                logger.info(f"HTTP服务器 - 收到 {self.address_string()} 的 gt4 验证结果")
+                self.result_callback(geetest_result)
+                self.response_ok()
+
 
 def set_listen_address():
     """
     设置HTTP服务器监听地址
     """
     if conf.preference.geetest_listen_address:
         if conf.preference.geetest_listen_address[1] == 0:
@@ -127,15 +161,15 @@
     pipe: Tuple[connection.Connection]
     """进程间通信管道，用于终止HTTP服务器"""
     geetest_result_queue: Queue[GeetestResult]
     """由Manager管理的验证结果数据"""
     wait_thread: Thread
 
     @classmethod
-    def result_callback(cls, result: GeetestResult):
+    def result_callback(cls, result: Union[GeetestResult, GeetestResultV4]):
         """
         给主进程发送验证结果
         """
         cls.geetest_result_queue.put(result)
 
     @classmethod
     def wait_until_stop(cls):
```

### Comparing `mys_goods_tool-2.0.3/mys_goods_tool/login_view.py` & `mys_goods_tool-2.0.4/mys_goods_tool/login_view.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from __future__ import annotations
 
 import asyncio
 import queue
 from typing import NamedTuple, Tuple, Optional, Set
+from urllib.parse import urlencode
 
 import httpx
 from rich.markdown import Markdown
 from textual.app import ComposeResult
 from textual.widgets import (
     Input
 )
 
 from mys_goods_tool.api import create_mobile_captcha, create_mmt, get_login_ticket_by_captcha, \
-    get_multi_token_by_login_ticket, get_cookie_token_by_stoken, get_stoken_v2_by_v1, get_ltoken_by_stoken
+    get_multi_token_by_login_ticket, get_cookie_token_by_stoken, get_stoken_v2_by_v1, get_ltoken_by_stoken, \
+    check_registrable
 from mys_goods_tool.custom_css import *
 from mys_goods_tool.custom_widget import RadioStatus, StaticStatus, ControllableButton, LoadingDisplay
 from mys_goods_tool.data_model import GeetestResult, MmtData, GetCookieStatus
 from mys_goods_tool.exchange_plan_view import ExchangePlanView
 from mys_goods_tool.geetest import GeetestProcessManager, SetAddressProcessManager
 from mys_goods_tool.user_data import config as conf, UserAccount, CONFIG_PATH
 from mys_goods_tool.utils import logger
@@ -102,14 +104,16 @@
 
 class PhoneForm(LoginForm):
     """
     手机号 表单
     """
     input = Input(placeholder="手机号", id="login_phone")
     """手机号输入框"""
+    device_id: Optional[str] = None
+    """人机验证过程的设备ID"""
     client: Optional[httpx.AsyncClient] = None
     """人机验证过程的连接对象"""
 
     ButtonTuple = NamedTuple("ButtonTuple",
                              send=ControllableButton,
                              stop_geetest=ControllableButton,
                              success=ControllableButton,
@@ -177,21 +181,22 @@
         while True:
             await asyncio.sleep(1)
             try:
                 geetest_result: GeetestResult = self.geetest_manager.result_queue.get_nowait()
             except queue.Empty:
                 continue
             else:
-                logger.info(f"已收到Geetest验证结果数据 {geetest_result}，将发送验证码至 {self.input.value}")
+                logger.info(f"已收到Geetest验证结果数据，将发送验证码至 {self.input.value}")
                 CaptchaLoginInformation.radio_tuple.geetest_finished.turn_on()
                 self.loading.show()
                 create_captcha_status, PhoneForm.client = await create_mobile_captcha(int(self.input.value),
                                                                                       self.mmt_data,
                                                                                       geetest_result,
-                                                                                      PhoneForm.client)
+                                                                                      PhoneForm.client,
+                                                                                      device_id=PhoneForm.device_id)
                 if create_captcha_status:
                     self.loading.hide()
                     logger.info(f"短信验证码已发送至 {self.input.value}")
                     CaptchaLoginInformation.radio_tuple.create_captcha.turn_on()
                     CaptchaLoginInformation.static_tuple.geetest_text.change_text(CaptchaLoginInformation.GEETEST_TEXT,
                                                                                   "center")
                     self.button.success.show()
@@ -228,16 +233,22 @@
         self.button.stop_geetest.show()
         CaptchaLoginInformation.radio_tuple.http_server.turn_on()
 
         task = self.loop.create_task(self.listen_result())
         self.loop_tasks.add(task)
         task.add_done_callback(self.loop_tasks.discard)
 
-        link = f"http://{address[0]}:{address[1]}/index.html?gt={self.mmt_data.gt}&challenge={self.mmt_data.challenge}"
-        link_localized = f"http://{address[0]}:{address[1]}/localized.html?gt={self.mmt_data.gt}&challenge={self.mmt_data.challenge}"
+        params = {
+            "gt": self.mmt_data.gt,
+            "mmtKey": self.mmt_data.mmt_key,
+            "riskType": self.mmt_data.risk_type
+        }
+        url_params = urlencode(params)
+        link = f"http://{address[0]}:{address[1]}/index.html?{url_params}"
+        link_localized = f"http://{address[0]}:{address[1]}/localized.html?{url_params}"
         CaptchaLoginInformation.static_tuple.geetest_text.change_text(
             renderable=f"\n- 请前往链接进行验证：\n"
                        f"[@click=app.open_link('{link}')]{link}[/]\n"
                        f"\n- 如果页面加载慢或者出错，尝试：\n"
                        f"[@click=app.open_link('{link_localized}')]{link_localized}[/]",
             text_align="left")
         logger.info(f"请前往链接进行人机验证：{link}")
@@ -267,15 +278,23 @@
 
         [i.turn_off() for i in CaptchaLoginInformation.radio_tuple]
         self.button.send.disable()
         self.loading.show()
 
         if PhoneForm.client:
             await PhoneForm.client.aclose()
-        create_mmt_status, self.mmt_data, PhoneForm.client = await create_mmt(keep_client=True)
+        check_registrable_status, registrable, PhoneForm.device_id, PhoneForm.client = await check_registrable(
+            int(self.input.value))
+        if registrable:
+            self.close_create_captcha_send()
+            self.button.error.show()
+            self.app.notice("[red]该手机号尚未注册！[/]")
+            return
+        create_mmt_status, self.mmt_data, PhoneForm.device_id, PhoneForm.client = await create_mmt(PhoneForm.client,
+                                                                                                   device_id=PhoneForm.device_id)
         if not create_mmt_status:
             self.close_create_captcha_send()
             self.button.error.show()
             self.app.notice("[red]获取Geetest行为验证任务数据失败！[/]")
             return
         else:
             logger.info(f"已成功获取Geetest行为验证任务数据 {self.mmt_data}")
@@ -326,15 +345,15 @@
     def __init__(self):
         super().__init__()
         self.login_result: Optional[GetCookieStatus] = None
         """登录操作返回值"""
         self.before_login: bool = True
         """当前状态是否在登录操作之前（不处于正在登录的状态）"""
 
-        self.input = Input(placeholder="为空时点击登录可进行Cookies刷新", id="login_captcha")
+        self.input = Input(placeholder="若发送验证码失败，也可前往米哈游通信证页面手动发送", id="login_captcha")
 
         self.loading = LoadingDisplay()
         self.loading.hide()
 
         self.button = self.ButtonTuple(
             login=ControllableButton("登录 / 刷新Cookies", variant="primary", id="login"),
             success=ControllableButton("完成", variant="success", id="login_success"),
```

### Comparing `mys_goods_tool-2.0.3/mys_goods_tool/tui.py` & `mys_goods_tool-2.0.4/mys_goods_tool/tui.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,31 +27,27 @@
 from mys_goods_tool.user_data import ROOT_PATH, VERSION
 from mys_goods_tool.utils import LOG_FORMAT, logger
 
 WELCOME_MD = """
 # Mys_Goods_Tool - 米游社商品兑换工具
 
 ## 更新说明
-- 修复米游社（大别野）等商品分区无商品的问题
-- 修复图形界面兑换模式下不会执行兑换的问题
-- 删除多余的 `pyperclip` 依赖
-- 解决部分商品兑换时间错误的问题
+- 修复启动后由于商品数据相关问题而导致的崩溃
+- 修复 Linux 实际不会应用 uvloop 的问题
+- 人机验证更新至 GT4（但实际上暂时不可用 [#105](https://github.com/Ljzd-PRO/Mys_Goods_Tool/issues/105#issuecomment-1552727784)）
 
 ## 功能和特性
 
 - 使用 [Textual](https://github.com/Textualize/textual) 终端图形界面库，支持 Windows / Linux / macOS 甚至可能是移动端SSH客户端
 - 短信验证码登录（只需接收一次验证码）
 - 内置人机验证页面，无需前往官网验证
 - 多账号支持
 - 支持米游社所有分区的商品兑换
 
 ### TODO
-- 支持在图形界面中编辑偏好设置
-- 密码登录
-- 解决SSH客户端无法跳转人机验证链接的问题
 - 更新至极验第四代适应性验证
 
 ## 其他
 - [**🔗完整说明文档**](https://github.com/Ljzd-PRO/Mys_Goods_Tool/wiki)
 - 仅供学习时参考
 
 - 相似项目推荐:  \
@@ -402,15 +398,15 @@
             TuiApp.text_log.write(text)
 
     def _on_mount(self, _: events.Mount) -> None:
         TuiApp.app = self
         TuiApp.text_log_writer = TuiApp.TextLogWriter()
         logger.add(self.text_log_writer, diagnose=False, level="DEBUG", format=LOG_FORMAT)
         if sys.platform not in ('win32', 'cygwin', 'cli'):
-            if "uvloop" not in sys.modules.copy():
+            if "uvloop" in sys.modules.copy():
                 import uvloop
                 import asyncio
                 asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
             else:
                 logger.info("在非 Windows 环境下，你可以安装 uvloop 以提高性能")
         self.query_one("Welcome Button", Button).focus()
```

### Comparing `mys_goods_tool-2.0.3/mys_goods_tool/user_data.py` & `mys_goods_tool-2.0.4/mys_goods_tool/user_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 ROOT_PATH = Path("./")
 """程序所在目录"""
 
 CONFIG_PATH = ROOT_PATH / "user_data.json"
 """用户数据文件默认路径"""
 
-VERSION = "2.0.3"
+VERSION = "2.0.4"
 """程序当前版本"""
 
 if TYPE_CHECKING:
     IntStr = Union[int, str]
     DictStrAny = Dict[str, Any]
     AbstractSetIntStr = AbstractSet[IntStr]
     MappingIntStrAny = Mapping[IntStr, Any]
@@ -408,15 +408,15 @@
 
 
 class UserData(BaseModel):
     """
     用户数据类
     """
     version: str = VERSION
-    """本次修改用户数据文件的程序版本号"""
+    """创建用户数据文件的程序版本号"""
     exchange_plans: Union[Set[ExchangePlan], List[ExchangePlan]] = set()
     """兑换计划列表"""
     preference: Preference = Preference()
     """偏好设置"""
     salt_config: SaltConfig = SaltConfig()
     """生成Headers - DS所用salt值"""
     device_config: DeviceConfig = DeviceConfig()
```

### Comparing `mys_goods_tool-2.0.3/mys_goods_tool/utils.py` & `mys_goods_tool-2.0.4/mys_goods_tool/utils.py`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.0.3/pyproject.toml` & `mys_goods_tool-2.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mys-goods-tool"
-version = "2.0.3"
+version = "2.0.4"
 description = "米游社商品兑换工具|短信验证登录|终端TUI界面"
 authors = ["Ljzd-PRO <ljzd@office.ljzd-pro.ml>"]
 readme = "README.md"
 homepage = "https://github.com/Ljzd-PRO/Mys_Goods_Tool"
 repository = "https://github.com/Ljzd-PRO/Mys_Goods_Tool"
 documentation = "https://github.com/Ljzd-PRO/Mys_Goods_Tool/wiki"
 keywords = ["mihoyo", "mihoyobbs", "genshin impact", "textual", "tui"]
```

### Comparing `mys_goods_tool-2.0.3/PKG-INFO` & `mys_goods_tool-2.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: mys-goods-tool
-Version: 2.0.3
+Version: 2.0.4
 Summary: 米游社商品兑换工具|短信验证登录|终端TUI界面
 Home-page: https://github.com/Ljzd-PRO/Mys_Goods_Tool
 Keywords: mihoyo,mihoyobbs,genshin impact,textual,tui
 Author: Ljzd-PRO
 Author-email: ljzd@office.ljzd-pro.ml
 Requires-Python: >=3.9,<3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Requires-Dist: apscheduler (>=3.10.1,<4.0.0)
 Requires-Dist: httpx (>=0.24.0,<0.25.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: ntplib (>=0.4.0,<0.5.0)
 Requires-Dist: ping3 (>=4.0.4,<5.0.0)
 Requires-Dist: pydantic (>=1.10.6,<2.0.0)
 Requires-Dist: requests (>=2.30.0,<3.0.0)
@@ -45,32 +44,28 @@
   <img alt="代码行数" src="https://img.shields.io/tokei/lines/github/Ljzd-PRO/Mys_Goods_Tool?style=for-the-badge">
   <img alt="构建结果" src="https://img.shields.io/github/actions/workflow/status/Ljzd-PRO/Mys_Goods_Tool/build-v2.yml?event=pull_request&style=for-the-badge">
   <img alt="Python版本兼容性测试" src="https://img.shields.io/github/actions/workflow/status/Ljzd-PRO/Mys_Goods_Tool/python-package.yml?event=pull_request&label=Versions%20Test&style=for-the-badge">
 </div>
 
 ### 更新说明
 
-- 修复定时兑换无效的问题
-- 修复失去网络连接的情况下会导致程序退出的Bug
-- 对于 Linux 使用 Ubuntu 20.04 进行构建，防止出现缺少 GNU libc 对应版本的问题
-- 非 Windows 系统增加 [uvloop](https://github.com/MagicStack/uvloop) 支持，提高性能
+- 修复启动后由于商品数据相关问题而导致的崩溃
+- 修复 Linux 实际不会应用 uvloop 的问题
+- 人机验证更新至
+  GT4（但实际上暂时不可用 [#105](https://github.com/Ljzd-PRO/Mys_Goods_Tool/issues/105#issuecomment-1552727784)）
 
 ## 功能和特性
 
 - [x] 使用 [Textual](https://github.com/Textualize/textual) 终端图形界面库，支持 Windows / Linux / macOS 甚至可能是移动端SSH客户端
 - [x] 短信验证码登录（只需接收一次验证码）
 - [x] 内置人机验证页面，无需前往官网验证
 - [x] 多账号支持
 - [x] 支持米游社所有分区的商品兑换
 
 ### TODO
-
-- [ ] 支持在图形界面中编辑偏好设置
-- [ ] 密码登录
-- [ ] 解决SSH客户端无法跳转人机验证链接的问题
 - [ ] 更新至极验第四代适应性验证
 
 ### 预览图
 
 <details>
   <summary>短信验证登录</summary>
   <img src="https://user-images.githubusercontent.com/63289359/235790425-7c502a69-baac-4ced-ba07-d068a88a7ae9.png" alt="短信验证登录页面" />
@@ -108,13 +103,10 @@
 - 仅供学习时参考
 
 - 相似项目推荐:  \
   **mysTool - 米游社辅助工具插件**  \
   简介：NoneBot2 插件 | 米游社工具-每日米游币任务、游戏签到、商品兑换、免抓包登录、原神树脂提醒  \
   🔗 https://github.com/Ljzd-PRO/nonebot-plugin-mystool
 
-- 本项目已开启[🔗Github Actions](https://github.com/Ljzd-PRO/Mys_Goods_Tool/actions)。
-  欢迎[🔗指出Bug](https://github.com/Ljzd-PRO/Mys_Goods_Tool/issues)
-  和[🔗贡献代码](https://github.com/Ljzd-PRO/Mys_Goods_Tool/pulls)👏
-
-- 开发版分支：[🔗dev](https://github.com/Ljzd-PRO/Mys_Goods_Tool/tree/dev/)
+- [🔗Bug 反馈](https://github.com/Ljzd-PRO/Mys_Goods_Tool/issues)  
+- 如果你知道如何修复一些Bug和新增功能，也欢迎提交你的修订代码 [🔗Pull requests](https://github.com/Ljzd-PRO/Mys_Goods_Tool/pulls)
```

