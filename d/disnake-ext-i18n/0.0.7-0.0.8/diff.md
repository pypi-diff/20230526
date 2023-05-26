# Comparing `tmp/disnake-ext-i18n-0.0.7.tar.gz` & `tmp/disnake-ext-i18n-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "disnake-ext-i18n-0.0.7.tar", last modified: Sun May 21 18:35:02 2023, max compression
+gzip compressed data, was "disnake-ext-i18n-0.0.8.tar", last modified: Fri May 26 16:00:06 2023, max compression
```

## Comparing `disnake-ext-i18n-0.0.7.tar` & `disnake-ext-i18n-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 18:35:02.240462 disnake-ext-i18n-0.0.7/
--rw-rw-rw-   0        0        0     9514 2023-05-21 18:35:02.240462 disnake-ext-i18n-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     8802 2023-05-21 18:17:54.000000 disnake-ext-i18n-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-21 18:35:02.204455 disnake-ext-i18n-0.0.7/disnake/
-drwxrwxrwx   0        0        0        0 2023-05-21 18:35:02.204455 disnake-ext-i18n-0.0.7/disnake/ext/
-drwxrwxrwx   0        0        0        0 2023-05-21 18:35:02.213456 disnake-ext-i18n-0.0.7/disnake/ext/i18n/
--rw-rw-rw-   0        0        0      119 2023-05-21 18:07:42.000000 disnake-ext-i18n-0.0.7/disnake/ext/i18n/__init__.py
--rw-rw-rw-   0        0        0    15450 2023-05-21 17:16:14.000000 disnake-ext-i18n-0.0.7/disnake/ext/i18n/agent.py
--rw-rw-rw-   0        0        0     2496 2023-05-21 16:48:12.000000 disnake-ext-i18n-0.0.7/disnake/ext/i18n/cache.py
--rw-rw-rw-   0        0        0    13517 2023-05-21 16:48:12.000000 disnake-ext-i18n-0.0.7/disnake/ext/i18n/language.py
--rw-rw-rw-   0        0        0    14314 2023-05-21 16:48:12.000000 disnake-ext-i18n-0.0.7/disnake/ext/i18n/preprocess.py
-drwxrwxrwx   0        0        0        0 2023-05-21 18:35:02.239462 disnake-ext-i18n-0.0.7/disnake_ext_i18n.egg-info/
--rw-rw-rw-   0        0        0     9514 2023-05-21 18:35:02.000000 disnake-ext-i18n-0.0.7/disnake_ext_i18n.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      368 2023-05-21 18:35:02.000000 disnake-ext-i18n-0.0.7/disnake_ext_i18n.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 18:35:02.000000 disnake-ext-i18n-0.0.7/disnake_ext_i18n.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-05-21 18:35:02.000000 disnake-ext-i18n-0.0.7/disnake_ext_i18n.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-21 18:35:02.000000 disnake-ext-i18n-0.0.7/disnake_ext_i18n.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2023-05-21 18:35:02.242463 disnake-ext-i18n-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1491 2023-05-21 18:32:48.000000 disnake-ext-i18n-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 16:00:06.301166 disnake-ext-i18n-0.0.8/
+-rw-rw-rw-   0        0        0     9514 2023-05-26 16:00:06.301166 disnake-ext-i18n-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     8802 2023-05-21 18:17:54.000000 disnake-ext-i18n-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 16:00:06.272158 disnake-ext-i18n-0.0.8/disnake/
+drwxrwxrwx   0        0        0        0 2023-05-26 16:00:06.272158 disnake-ext-i18n-0.0.8/disnake/ext/
+drwxrwxrwx   0        0        0        0 2023-05-26 16:00:06.279160 disnake-ext-i18n-0.0.8/disnake/ext/i18n/
+-rw-rw-rw-   0        0        0      119 2023-05-26 16:00:04.000000 disnake-ext-i18n-0.0.8/disnake/ext/i18n/__init__.py
+-rw-rw-rw-   0        0        0    15473 2023-05-26 15:58:45.000000 disnake-ext-i18n-0.0.8/disnake/ext/i18n/agent.py
+-rw-rw-rw-   0        0        0     2496 2023-05-21 16:48:12.000000 disnake-ext-i18n-0.0.8/disnake/ext/i18n/cache.py
+-rw-rw-rw-   0        0        0    13517 2023-05-21 16:48:12.000000 disnake-ext-i18n-0.0.8/disnake/ext/i18n/language.py
+-rw-rw-rw-   0        0        0    14314 2023-05-21 16:48:12.000000 disnake-ext-i18n-0.0.8/disnake/ext/i18n/preprocess.py
+drwxrwxrwx   0        0        0        0 2023-05-26 16:00:06.300164 disnake-ext-i18n-0.0.8/disnake_ext_i18n.egg-info/
+-rw-rw-rw-   0        0        0     9514 2023-05-26 16:00:06.000000 disnake-ext-i18n-0.0.8/disnake_ext_i18n.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      368 2023-05-26 16:00:06.000000 disnake-ext-i18n-0.0.8/disnake_ext_i18n.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 16:00:06.000000 disnake-ext-i18n-0.0.8/disnake_ext_i18n.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-05-26 16:00:06.000000 disnake-ext-i18n-0.0.8/disnake_ext_i18n.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-26 16:00:06.000000 disnake-ext-i18n-0.0.8/disnake_ext_i18n.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      115 2023-05-26 16:00:06.302165 disnake-ext-i18n-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1491 2023-05-21 18:32:48.000000 disnake-ext-i18n-0.0.8/setup.py
```

### Comparing `disnake-ext-i18n-0.0.7/PKG-INFO` & `disnake-ext-i18n-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: disnake-ext-i18n
-Version: 0.0.7
+Version: 0.0.8
 Summary: A fork of the Pycord extension to support automatic text translations in 107 languages to also support Disnake.
 Home-page: https://github.com/jaymart95/disnake-ext-i18n
 Author: Rickaym
 License: MIT
 Project-URL: Issue tracker, https://github.com/jaymart95/disnake-ext-i18n/issues
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: disnake-ext-i18n Version: 0.0.7 Summary: A fork of
+Metadata-Version: 2.1 Name: disnake-ext-i18n Version: 0.0.8 Summary: A fork of
 the Pycord extension to support automatic text translations in 107 languages to
 also support Disnake. Home-page: https://github.com/jaymart95/disnake-ext-i18n
 Author: Rickaym License: MIT Project-URL: Issue tracker, https://github.com/
 jaymart95/disnake-ext-i18n/issues Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Natural Language :: English Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
```

### Comparing `disnake-ext-i18n-0.0.7/README.md` & `disnake-ext-i18n-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `disnake-ext-i18n-0.0.7/disnake/ext/i18n/agent.py` & `disnake-ext-i18n-0.0.8/disnake/ext/i18n/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 Messageable_send = Messageable.send
 Message_edit = Message.edit
 HTTPClient_edit_message = HTTPClient.edit_message
 HTTPClient_send_message = HTTPClient.send_message
 InteractionResponse_send_message = InteractionResponse.send_message
 InteractionResponse_edit_message = InteractionResponse.edit_message
-InteractionResponse_send_modal = InteractionResponse.send_modal
+#InteractionResponse_send_modal = InteractionResponse.send_modal
 AsyncWebhookAdapter_create_interaction_response = (
     AsyncWebhookAdapter.create_interaction_response
 )
 AsyncWebhookAdapter_execute_webhook = AsyncWebhookAdapter.execute_webhook
 Webhook_send = Webhook.send
 WebhookMessage_edit = WebhookMessage.edit
 
@@ -146,28 +146,28 @@
                     kwds["payload"]["content"],
                 ) = TranslationAgent.translate_payload(
                     lang, kwds["payload"], content, **Agent.translate_config()
                 )
     return AsyncWebhookAdapter_execute_webhook(self, *args, **kwds)
 
 
-async def i18n_InteractionResponse_send_modal(self: InteractionResponse, modal: Modal):
-    """
-    Language code is appended to the modal title if there is a language
-    preference.
-
-    TODO: Very problematic if translation functions are slow, often ends up
-    timing out on responses.
-    """
-    dest_lang = await Agent.detector.first_language_of(self)
-    if dest_lang:
-        modal.title = TranslationAgent.encode_lang_str(
-            Agent.source_lang, modal.title, dest_lang
-        )
-    return await InteractionResponse_send_modal(self, modal)
+#async def i18n_InteractionResponse_send_modal(self: InteractionResponse, modal: Modal):
+#    """
+#    Language code is appended to the modal title if there is a language
+#    preference.
+#
+#    TODO: Very problematic if translation functions are slow, often ends up
+#    timing out on responses.
+#    """
+#    dest_lang = await Agent.detector.first_language_of(self)
+#    if dest_lang:
+#        modal.title = TranslationAgent.encode_lang_str(
+#            Agent.source_lang, modal.title, dest_lang
+#        )
+#    return await InteractionResponse_send_modal(self, modal)
 
 
 def isinstancemethod(func: Callable) -> bool:
     """
     Returns whether if a given function is a staticmethod or an
     instancemethod/classmethod.
     """
@@ -245,15 +245,15 @@
     def __init__(
         self,
         translate_all: Optional[bool] = None,
         translate_messages: Optional[bool] = None,
         translate_embeds: Optional[bool] = None,
         translate_buttons: Optional[bool] = None,
         translate_selects: Optional[bool] = None,
-        translate_modals: Optional[bool] = None,
+        #translate_modals: Optional[bool] = None,
         source_lang: Optional[Language] = None,
     ):
         """
         A context menu to temporarily reconfigure the translation settings until
         it has been exited.
 
         ### Parameters:
@@ -287,15 +287,15 @@
         """
 
         vmap = {
             "translate_messages": translate_messages,
             "translate_embeds": translate_embeds,
             "translate_buttons": translate_buttons,
             "translate_selects": translate_selects,
-            "translate_modals": translate_modals,
+            #"translate_modals": translate_modals,
             "source_lang": source_lang,
         }
         self.prior = {key: getattr(Agent, key, None) for key in vmap}
 
         for key, val in vmap.items():
             if translate_all and key.startswith("translate_"):
                 setattr(Agent, key, True)
@@ -315,28 +315,28 @@
     translator = Translator()
     detector = Detector()
 
     translate_messages = True
     translate_embeds = False
     translate_buttons = False
     translate_selects = False
-    translate_modals = False
+    #translate_modals = False
     source_lang = Language.English
     _instantiated = False
 
     def __init__(
         self,
         translator: Optional[Translator] = None,
         detector: Optional[Detector] = None,
         translate_all: Optional[bool] = None,
         translate_messages: Optional[bool] = None,
         translate_embeds: Optional[bool] = None,
         translate_buttons: Optional[bool] = None,
         translate_selects: Optional[bool] = None,
-        translate_modals: Optional[bool] = None,
+        #translate_modals: Optional[bool] = None,
         source_lang: Optional[Language] = None,
         handle_webhooks: bool = True,
     ):
         """
         Sets initialized injectors to override high and low level.
         At any given case, you cannot initialize this class more than
         once.
@@ -377,24 +377,24 @@
         setattr(
             InteractionResponse,
             "edit_message",
             wrap_i18n_editer(InteractionResponse_edit_message),
         )
         setattr(WebhookMessage, "edit", wrap_i18n_editer(WebhookMessage_edit))
         setattr(HTTPClient, "edit_message", i18n_HTTPClient_edit_message)
-        setattr(InteractionResponse, "send_modal", i18n_InteractionResponse_send_modal)
+        #setattr(InteractionResponse, "send_modal", i18n_InteractionResponse_send_modal)
 
         for key, val in {
             "translator": translator,
             "detector": detector,
             "translate_messages": translate_messages,
             "translate_embeds": translate_embeds,
             "translate_buttons": translate_buttons,
             "translate_selects": translate_selects,
-            "translate_modals": translate_modals,
+            #"translate_modals": translate_modals,
             "source_lang": source_lang,
         }.items():
             if translate_all and key.startswith("translate_"):
                 setattr(Agent, key, True)
             elif val is not None:
                 setattr(Agent, key, val)
 
@@ -406,15 +406,15 @@
         """
         return {
             "source_lang": Agent.source_lang,
             "translator": Agent.translator,
             "translate_components": (
                 Agent.translate_buttons
                 or Agent.translate_selects
-                or Agent.translate_modals
+                #or Agent.translate_modals
             ),
             "translate_messages": Agent.translate_messages,
             "translate_embeds": Agent.translate_embeds,
             "translate_buttons": Agent.translate_buttons,
             "translate_selects": Agent.translate_selects,
-            "translate_modals": Agent.translate_modals,
+            #"translate_modals": Agent.translate_modals,
         }
```

### Comparing `disnake-ext-i18n-0.0.7/disnake/ext/i18n/cache.py` & `disnake-ext-i18n-0.0.8/disnake/ext/i18n/cache.py`

 * *Files identical despite different names*

### Comparing `disnake-ext-i18n-0.0.7/disnake/ext/i18n/language.py` & `disnake-ext-i18n-0.0.8/disnake/ext/i18n/language.py`

 * *Files identical despite different names*

### Comparing `disnake-ext-i18n-0.0.7/disnake/ext/i18n/preprocess.py` & `disnake-ext-i18n-0.0.8/disnake/ext/i18n/preprocess.py`

 * *Files identical despite different names*

### Comparing `disnake-ext-i18n-0.0.7/disnake_ext_i18n.egg-info/PKG-INFO` & `disnake-ext-i18n-0.0.8/disnake_ext_i18n.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: disnake-ext-i18n
-Version: 0.0.7
+Version: 0.0.8
 Summary: A fork of the Pycord extension to support automatic text translations in 107 languages to also support Disnake.
 Home-page: https://github.com/jaymart95/disnake-ext-i18n
 Author: Rickaym
 License: MIT
 Project-URL: Issue tracker, https://github.com/jaymart95/disnake-ext-i18n/issues
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: disnake-ext-i18n Version: 0.0.7 Summary: A fork of
+Metadata-Version: 2.1 Name: disnake-ext-i18n Version: 0.0.8 Summary: A fork of
 the Pycord extension to support automatic text translations in 107 languages to
 also support Disnake. Home-page: https://github.com/jaymart95/disnake-ext-i18n
 Author: Rickaym License: MIT Project-URL: Issue tracker, https://github.com/
 jaymart95/disnake-ext-i18n/issues Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Natural Language :: English Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
```

### Comparing `disnake-ext-i18n-0.0.7/setup.py` & `disnake-ext-i18n-0.0.8/setup.py`

 * *Files identical despite different names*

