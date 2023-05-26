# Comparing `tmp/divent-3.4.0.tar.gz` & `tmp/divent-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "divent-3.4.0.tar", max compression
+gzip compressed data, was "divent-3.4.1.tar", max compression
```

## Comparing `divent-3.4.0.tar` & `divent-3.4.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1972 2023-04-10 18:54:14.918615 divent-3.4.0/README.md
--rw-r--r--   0        0        0     8196 2023-04-10 18:54:14.918615 divent-3.4.0/divent/bot.py
--rw-r--r--   0        0        0        0 2023-04-10 18:54:14.918615 divent-3.4.0/divent/py.typed
--rw-r--r--   0        0        0    31000 2023-04-10 18:54:14.918615 divent-3.4.0/divent/static/css/font-awesome.min.css
--rw-r--r--   0        0        0     2903 2023-04-10 18:54:14.918615 divent-3.4.0/divent/static/css/global.css
--rw-r--r--   0        0        0   134808 2023-04-10 18:54:14.922615 divent-3.4.0/divent/static/fonts/FontAwesome.otf
--rw-r--r--   0        0        0   165742 2023-04-10 18:54:14.922615 divent-3.4.0/divent/static/fonts/fontawesome-webfont.eot
--rw-r--r--   0        0        0   444379 2023-04-10 18:54:14.926615 divent-3.4.0/divent/static/fonts/fontawesome-webfont.svg
--rw-r--r--   0        0        0   165548 2023-04-10 18:54:14.926615 divent-3.4.0/divent/static/fonts/fontawesome-webfont.ttf
--rw-r--r--   0        0        0    98024 2023-04-10 18:54:14.926615 divent-3.4.0/divent/static/fonts/fontawesome-webfont.woff
--rw-r--r--   0        0        0    77160 2023-04-10 18:54:14.926615 divent-3.4.0/divent/static/fonts/fontawesome-webfont.woff2
--rw-r--r--   0        0        0    20704 2023-04-10 18:54:14.926615 divent-3.4.0/divent/static/fonts/open-sans-v29-latin-regular.woff
--rw-r--r--   0        0        0    16720 2023-04-10 18:54:14.926615 divent-3.4.0/divent/static/fonts/open-sans-v29-latin-regular.woff2
--rw-r--r--   0        0        0   106618 2023-04-10 18:54:14.926615 divent-3.4.0/divent/static/img/deadlink.png
--rw-r--r--   0        0        0      877 2023-04-10 18:54:14.926615 divent-3.4.0/divent/templates/base.html.j2
--rw-r--r--   0        0        0      555 2023-04-10 18:54:14.926615 divent-3.4.0/divent/templates/error.html.j2
--rw-r--r--   0        0        0      979 2023-04-10 18:54:14.926615 divent-3.4.0/divent/templates/footer.html.j2
--rw-r--r--   0        0        0     2193 2023-04-10 18:54:14.926615 divent-3.4.0/divent/templates/guilds.html.j2
--rw-r--r--   0        0        0     1245 2023-04-10 18:54:14.926615 divent-3.4.0/divent/templates/index.html.j2
--rw-r--r--   0        0        0     2236 2023-04-10 18:54:14.926615 divent-3.4.0/divent/templates/subscribe.html.j2
--rw-r--r--   0        0        0     1484 2023-04-10 18:54:14.926615 divent-3.4.0/divent/translations/fr.json
--rw-r--r--   0        0        0      858 2023-04-10 18:54:14.930615 divent-3.4.0/pyproject.toml
--rw-r--r--   0        0        0     2840 1970-01-01 00:00:00.000000 divent-3.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1972 2023-05-26 10:21:08.073555 divent-3.4.1/README.md
+-rw-r--r--   0        0        0     8066 2023-05-26 10:21:08.073555 divent-3.4.1/divent/bot.py
+-rw-r--r--   0        0        0        0 2023-05-26 10:21:08.073555 divent-3.4.1/divent/py.typed
+-rw-r--r--   0        0        0    31000 2023-05-26 10:21:08.073555 divent-3.4.1/divent/static/css/font-awesome.min.css
+-rw-r--r--   0        0        0     2903 2023-05-26 10:21:08.073555 divent-3.4.1/divent/static/css/global.css
+-rw-r--r--   0        0        0   134808 2023-05-26 10:21:08.073555 divent-3.4.1/divent/static/fonts/FontAwesome.otf
+-rw-r--r--   0        0        0   165742 2023-05-26 10:21:08.073555 divent-3.4.1/divent/static/fonts/fontawesome-webfont.eot
+-rw-r--r--   0        0        0   444379 2023-05-26 10:21:08.077555 divent-3.4.1/divent/static/fonts/fontawesome-webfont.svg
+-rw-r--r--   0        0        0   165548 2023-05-26 10:21:08.077555 divent-3.4.1/divent/static/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0        0        0    98024 2023-05-26 10:21:08.077555 divent-3.4.1/divent/static/fonts/fontawesome-webfont.woff
+-rw-r--r--   0        0        0    77160 2023-05-26 10:21:08.077555 divent-3.4.1/divent/static/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0        0        0    20704 2023-05-26 10:21:08.077555 divent-3.4.1/divent/static/fonts/open-sans-v29-latin-regular.woff
+-rw-r--r--   0        0        0    16720 2023-05-26 10:21:08.077555 divent-3.4.1/divent/static/fonts/open-sans-v29-latin-regular.woff2
+-rw-r--r--   0        0        0   106618 2023-05-26 10:21:08.077555 divent-3.4.1/divent/static/img/deadlink.png
+-rw-r--r--   0        0        0      877 2023-05-26 10:21:08.077555 divent-3.4.1/divent/templates/base.html.j2
+-rw-r--r--   0        0        0      555 2023-05-26 10:21:08.077555 divent-3.4.1/divent/templates/error.html.j2
+-rw-r--r--   0        0        0      979 2023-05-26 10:21:08.077555 divent-3.4.1/divent/templates/footer.html.j2
+-rw-r--r--   0        0        0     2193 2023-05-26 10:21:08.077555 divent-3.4.1/divent/templates/guilds.html.j2
+-rw-r--r--   0        0        0     1245 2023-05-26 10:21:08.077555 divent-3.4.1/divent/templates/index.html.j2
+-rw-r--r--   0        0        0     2236 2023-05-26 10:21:08.077555 divent-3.4.1/divent/templates/subscribe.html.j2
+-rw-r--r--   0        0        0     1484 2023-05-26 10:21:08.077555 divent-3.4.1/divent/translations/fr.json
+-rw-r--r--   0        0        0      834 2023-05-26 10:21:08.081555 divent-3.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2796 1970-01-01 00:00:00.000000 divent-3.4.1/PKG-INFO
```

### Comparing `divent-3.4.0/README.md` & `divent-3.4.1/README.md`

 * *Files identical despite different names*

### Comparing `divent-3.4.0/divent/bot.py` & `divent-3.4.1/divent/bot.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,20 +5,18 @@
 from os import getenv, path
 from typing import Dict, Optional
 
 from disnake import Client, Guild
 from dotenv import load_dotenv
 from ics import Calendar, ContentLine, Event
 from ics.alarm import DisplayAlarm
-from oauthlib.oauth2 import TokenExpiredError
+from oauthlib.oauth2 import OAuth2Error
 from quart import Quart, redirect, render_template, request, session, url_for
 from requests_oauthlib import OAuth2Session  # type: ignore
-import sentry_sdk
-from sentry_sdk.integrations.quart import QuartIntegration
-from uvicorn.middleware.proxy_headers import ProxyHeadersMiddleware  # type: ignore
+from uvicorn.middleware.proxy_headers import ProxyHeadersMiddleware
 
 
 load_dotenv()
 
 DISCORD_TOKEN = getenv("DISCORD_TOKEN")
 OAUTH2_CLIENT_ID = getenv("OAUTH2_CLIENT_ID")
 OAUTH2_CLIENT_SECRET = getenv("OAUTH2_CLIENT_SECRET")
@@ -29,18 +27,14 @@
 if not OAUTH2_CLIENT_SECRET:
     raise Exception("Missing OAUTH2_CLIENT_SECRET")
 
 QUART_DEBUG = getenv("QUART_DEBUG", False)
 if QUART_DEBUG:
     logging.basicConfig(level=logging.DEBUG)
 
-SENTRY_DSN = getenv("SENTRY_DSN")
-if SENTRY_DSN:
-    sentry_sdk.init(SENTRY_DSN, integrations=[QuartIntegration()])
-
 API_BASE_URL = getenv("API_BASE_URL", "https://discordapp.com/api")
 AUTHORIZATION_BASE_URL = f"{API_BASE_URL}/oauth2/authorize"
 TOKEN_URL = f"{API_BASE_URL}/oauth2/token"
 
 
 class Discord(Client):
     async def on_ready(self):
@@ -163,21 +157,25 @@
 
 @app.route("/callback")
 async def callback():
     request_values = await request.values
     if request_values.get("error"):
         return errorhandler(request_values.get("error"))
 
-    discord = make_session(state=session.get("oauth2_state"))
-    token = discord.fetch_token(
-        TOKEN_URL,
-        client_secret=OAUTH2_CLIENT_SECRET,
-        authorization_response=request.url,
-    )
-    token_updater(token)
+    try:
+        discord = make_session(state=session.get("oauth2_state"))
+        token = discord.fetch_token(
+            TOKEN_URL,
+            client_secret=OAUTH2_CLIENT_SECRET,
+            authorization_response=request.url,
+        )
+        token_updater(token)
+    except OAuth2Error as e:
+        return errorhandler(e)
+
     return redirect(session.pop("redirect_url", url_for(".guilds")))
 
 
 @app.route("/guilds")
 @login_required
 async def guilds():
     guild = get_guild_by_id(request.args.get("guild"))
@@ -187,15 +185,15 @@
             url_for(".subscribe", guild_id=guild.vanity_url_code or guild.id)
         )
 
     try:
         discord = make_session(token=session.get("oauth2_token"))
         user = discord.get(f"{API_BASE_URL}/users/@me").json()
         user_guilds = discord.get(f"{API_BASE_URL}/users/@me/guilds").json()
-    except TokenExpiredError:
+    except OAuth2Error:
         return redirect(url_for(".login"))
 
     common_guilds = []
     for bot_guild in client.guilds:
         for user_guild in user_guilds:
             if str(bot_guild.id) == user_guild["id"]:
                 common_guilds.append(bot_guild)
@@ -211,15 +209,15 @@
     guild = get_guild_by_id(guild_id)
     if guild is None:
         return redirect(url_for(".login"))
 
     try:
         discord = make_session(token=session.get("oauth2_token"))
         user_guilds = discord.get(f"{API_BASE_URL}/users/@me/guilds").json()
-    except TokenExpiredError:
+    except OAuth2Error:
         return redirect(url_for(".login"))
 
     if not any(str(guild.id) == user_guild["id"] for user_guild in user_guilds):
         return redirect(url_for(".login"))
 
     return await render_template("subscribe.html.j2", guild=guild)
```

### Comparing `divent-3.4.0/divent/static/css/font-awesome.min.css` & `divent-3.4.1/divent/static/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `divent-3.4.0/divent/static/css/global.css` & `divent-3.4.1/divent/static/css/global.css`

 * *Files identical despite different names*

### Comparing `divent-3.4.0/divent/static/fonts/FontAwesome.otf` & `divent-3.4.1/divent/static/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `divent-3.4.0/divent/static/fonts/fontawesome-webfont.eot` & `divent-3.4.1/divent/static/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `divent-3.4.0/divent/static/fonts/fontawesome-webfont.svg` & `divent-3.4.1/divent/static/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `divent-3.4.0/divent/static/fonts/fontawesome-webfont.ttf` & `divent-3.4.1/divent/static/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `divent-3.4.0/divent/static/fonts/fontawesome-webfont.woff` & `divent-3.4.1/divent/static/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `divent-3.4.0/divent/static/fonts/fontawesome-webfont.woff2` & `divent-3.4.1/divent/static/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `divent-3.4.0/divent/static/fonts/open-sans-v29-latin-regular.woff` & `divent-3.4.1/divent/static/fonts/open-sans-v29-latin-regular.woff`

 * *Files identical despite different names*

### Comparing `divent-3.4.0/divent/static/fonts/open-sans-v29-latin-regular.woff2` & `divent-3.4.1/divent/static/fonts/open-sans-v29-latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `divent-3.4.0/divent/static/img/deadlink.png` & `divent-3.4.1/divent/static/img/deadlink.png`

 * *Files identical despite different names*

### Comparing `divent-3.4.0/divent/templates/base.html.j2` & `divent-3.4.1/divent/templates/base.html.j2`

 * *Files identical despite different names*

### Comparing `divent-3.4.0/divent/templates/error.html.j2` & `divent-3.4.1/divent/templates/error.html.j2`

 * *Files identical despite different names*

### Comparing `divent-3.4.0/divent/templates/footer.html.j2` & `divent-3.4.1/divent/templates/footer.html.j2`

 * *Files identical despite different names*

### Comparing `divent-3.4.0/divent/templates/guilds.html.j2` & `divent-3.4.1/divent/templates/guilds.html.j2`

 * *Files identical despite different names*

### Comparing `divent-3.4.0/divent/templates/index.html.j2` & `divent-3.4.1/divent/templates/index.html.j2`

 * *Files identical despite different names*

### Comparing `divent-3.4.0/divent/templates/subscribe.html.j2` & `divent-3.4.1/divent/templates/subscribe.html.j2`

 * *Files identical despite different names*

### Comparing `divent-3.4.0/divent/translations/fr.json` & `divent-3.4.1/divent/translations/fr.json`

 * *Files identical despite different names*

### Comparing `divent-3.4.0/pyproject.toml` & `divent-3.4.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "divent"
-version = "3.4.0"
+version = "3.4.1"
 description = "The discord scheduled event calendar generator"
 authors = ["Xéfir Destiny"]
 license = "WTFPL"
 readme = "README.md"
 homepage = "https://divent.crystalyx.net/"
 repository = "https://git.crystalyx.net/Xefir/Divent"
 
@@ -12,27 +12,26 @@
 divent = 'divent.bot:__main__'
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 disnake = "^2.8.1"
 ics = "0.8.0.dev0"
 python-dotenv = "^1.0.0"
-quart = "^0.18.3"
+quart = "^0.18.4"
 requests-oauthlib = "^1.3.1"
-sentry-sdk = "^1.19.1"
-uvicorn = "^0.21.1"
+uvicorn = "^0.22.0"
 
 [tool.poetry.dev-dependencies]
 black = "^23.3.0"
-djlint = "^1.19.16"
+djlint = "^1.29.0"
 flake8 = "^6.0.0"
-flake8-alphabetize = "^0.0.20"
+flake8-alphabetize = "^0.0.21"
 flake8-black = "^0.3.6"
-mypy = "^1.1.1"
-types-oauthlib = "^3.2.0.7"
+mypy = "^1.3.0"
+types-oauthlib = "^3.2.0.8"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.djlint]
 extension = "j2"
```

### Comparing `divent-3.4.0/PKG-INFO` & `divent-3.4.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: divent
-Version: 3.4.0
+Version: 3.4.1
 Summary: The discord scheduled event calendar generator
 Home-page: https://divent.crystalyx.net/
 License: WTFPL
 Author: Xéfir Destiny
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: disnake (>=2.8.1,<3.0.0)
 Requires-Dist: ics (==0.8.0.dev0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
-Requires-Dist: quart (>=0.18.3,<0.19.0)
+Requires-Dist: quart (>=0.18.4,<0.19.0)
 Requires-Dist: requests-oauthlib (>=1.3.1,<2.0.0)
-Requires-Dist: sentry-sdk (>=1.19.1,<2.0.0)
-Requires-Dist: uvicorn (>=0.21.1,<0.22.0)
+Requires-Dist: uvicorn (>=0.22.0,<0.23.0)
 Project-URL: Repository, https://git.crystalyx.net/Xefir/Divent
 Description-Content-Type: text/markdown
 
 # Divent
 > The discord scheduled event calendar generator
 
 [![Build Status](https://ci.crystalyx.net/api/badges/Xefir/Divent/status.svg)](https://ci.crystalyx.net/Xefir/Divent)
```

