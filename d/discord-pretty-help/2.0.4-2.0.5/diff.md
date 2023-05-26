# Comparing `tmp/discord_pretty_help-2.0.4.tar.gz` & `tmp/discord_pretty_help-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord_pretty_help-2.0.4.tar", max compression
+gzip compressed data, was "discord_pretty_help-2.0.5.tar", max compression
```

## Comparing `discord_pretty_help-2.0.4.tar` & `discord_pretty_help-2.0.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1090 2023-04-29 11:31:31.530107 discord_pretty_help-2.0.4/LICENSE
--rw-r--r--   0        0        0      105 2023-05-14 10:50:13.591307 discord_pretty_help-2.0.4/pretty_help/__init__.py
--rw-r--r--   0        0        0      500 2023-04-29 11:31:31.540118 discord_pretty_help-2.0.4/pretty_help/abc_menu.py
--rw-r--r--   0        0        0     4197 2023-05-14 04:50:39.398654 discord_pretty_help-2.0.4/pretty_help/app_menu.py
--rw-r--r--   0        0        0     5332 2023-04-29 11:31:31.540118 discord_pretty_help-2.0.4/pretty_help/emoji_menu.py
--rw-r--r--   0        0        0    23111 2023-05-14 10:49:47.368955 discord_pretty_help-2.0.4/pretty_help/pretty_help.py
--rw-r--r--   0        0        0      748 2023-05-14 08:41:21.929133 discord_pretty_help-2.0.4/pyproject.toml
--rw-r--r--   0        0        0     3952 2023-05-14 10:49:13.991504 discord_pretty_help-2.0.4/README.md
--rw-r--r--   0        0        0     4626 1970-01-01 00:00:00.000000 discord_pretty_help-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-04-29 11:31:31.530107 discord_pretty_help-2.0.5/LICENSE
+-rw-r--r--   0        0        0      105 2023-05-26 22:10:20.050937 discord_pretty_help-2.0.5/pretty_help/__init__.py
+-rw-r--r--   0        0        0      500 2023-04-29 11:31:31.540118 discord_pretty_help-2.0.5/pretty_help/abc_menu.py
+-rw-r--r--   0        0        0     4685 2023-05-26 22:08:01.160304 discord_pretty_help-2.0.5/pretty_help/app_menu.py
+-rw-r--r--   0        0        0     5332 2023-04-29 11:31:31.540118 discord_pretty_help-2.0.5/pretty_help/emoji_menu.py
+-rw-r--r--   0        0        0    23111 2023-05-14 10:49:47.368955 discord_pretty_help-2.0.5/pretty_help/pretty_help.py
+-rw-r--r--   0        0        0      748 2023-05-26 22:10:05.024664 discord_pretty_help-2.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3952 2023-05-14 10:49:13.991504 discord_pretty_help-2.0.5/README.md
+-rw-r--r--   0        0        0     4626 1970-01-01 00:00:00.000000 discord_pretty_help-2.0.5/PKG-INFO
```

### Comparing `discord_pretty_help-2.0.4/LICENSE` & `discord_pretty_help-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `discord_pretty_help-2.0.4/pretty_help/app_menu.py` & `discord_pretty_help-2.0.5/pretty_help/app_menu.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,22 +18,24 @@
         timeout (Optional[float], optional): The duration the interaction will be active for. Defaults to None.
         ephemeral (Optional[bool], optional): Send as an ephemeral message. Defaults to False.
     """
 
     index = 0
 
     def __init__(
-            self,
-            pages: List[discord.Embed] = None,
-            timeout: Optional[float] = None,
-            ephemeral: Optional[bool] = False,
+        self,
+        pages: List[discord.Embed] = None,
+        timeout: Optional[float] = None,
+        ephemeral: Optional[bool] = False,
+        allowed_user: Optional[discord.Member] = None,
     ):
         super().__init__(timeout=timeout)
         self.page_count = len(pages) if pages else None
         self.pages = pages
+        self.allowed_user = allowed_user
 
         if pages and len(pages) == 1:
             self.remove_item(self.previous)
             self.remove_item(self.next)
             self.remove_item(self.select)
 
         if ephemeral:
@@ -49,81 +51,92 @@
 
     @discord.ui.button(
         label="Previous",
         style=discord.ButtonStyle.success,
         row=1,
         custom_id="pretty_help:previous",
     )
-    async def previous(self, interaction: discord.Interaction, button:discord.Button):
+    async def previous(self, interaction: discord.Interaction, button: discord.Button):
         self.index -= 1
         await self.update(interaction)
 
     @discord.ui.button(
         label="Next",
         style=discord.ButtonStyle.primary,
         row=1,
         custom_id="pretty_help:next",
     )
-    async def next(self, interaction: discord.Interaction, button:discord.Button):
+    async def next(self, interaction: discord.Interaction, button: discord.Button):
         self.index += 1
         await self.update(interaction)
 
     @discord.ui.button(
         label="Delete",
         style=discord.ButtonStyle.danger,
         row=1,
         custom_id="pretty_help:delete",
     )
-    async def _delete(self, interaction: discord.Interaction, button:discord.Button):
+    async def _delete(self, interaction: discord.Interaction, button: discord.Button):
         await interaction.message.delete()
 
     @discord.ui.select(row=2, custom_id="pretty_help:select")
     async def select(self, interaction: discord.Interaction, select: Select):
         self.index = int(select.values[0])
         await self.update(interaction)
 
     async def update(self, interaction: discord.Interaction):
         await interaction.response.edit_message(
             embed=self.pages[self.index % self.page_count], view=self
         )
 
+    async def interaction_check(self, interaction: discord.Interaction) -> bool:
+        if (
+            not self.allowed_user
+            and interaction.data.get("custom_id") == self._delete.custom_id
+        ):
+            return True
+        return interaction.user == self.allowed_user
+
 
 class AppMenu(PrettyMenu):
     """
     Navigate pages using the Discord UI components.
 
     This menu can be *partially* persistent with `client.add_view(AppMenu())`
     This will allow the delete button to work on past messages
 
     Args:
         timeout (Optional[float], optional): The duration the interaction will be active for. Defaults to None.
         ephemeral (Optional[bool], optional): Send as an ephemeral message. Defaults to False.
     """
 
     def __init__(
-            self,
-            timeout: Optional[float] = None,
-            ephemeral: Optional[bool] = False,
+        self,
+        timeout: Optional[float] = None,
+        ephemeral: Optional[bool] = False,
     ) -> None:
         # super().__init__()
         self.timeout = timeout
         self.ephemeral = ephemeral
 
     async def send_pages(
-            self,
-            ctx: commands.Context,
-            destination: discord.abc.Messageable,
-            pages: List[discord.Embed],
+        self,
+        ctx: commands.Context,
+        destination: discord.abc.Messageable,
+        pages: List[discord.Embed],
     ):
-
         if ctx.interaction:
             await ctx.interaction.response.send_message(
                 embed=pages[0],
                 view=AppNav(
-                    pages=pages, timeout=self.timeout, ephemeral=self.ephemeral
+                    pages=pages,
+                    timeout=self.timeout,
+                    ephemeral=self.ephemeral,
+                    allowed_user=ctx.author,
                 ),
                 ephemeral=self.ephemeral,
             )
         else:
             await destination.send(
-                embed=pages[0], view=AppNav(pages=pages, timeout=self.timeout)
+                embed=pages[0],
+                view=AppNav(pages=pages, timeout=self.timeout, allowed_user=ctx.author),
             )
```

### Comparing `discord_pretty_help-2.0.4/pretty_help/emoji_menu.py` & `discord_pretty_help-2.0.5/pretty_help/emoji_menu.py`

 * *Files identical despite different names*

### Comparing `discord_pretty_help-2.0.4/pretty_help/pretty_help.py` & `discord_pretty_help-2.0.5/pretty_help/pretty_help.py`

 * *Files identical despite different names*

### Comparing `discord_pretty_help-2.0.4/pyproject.toml` & `discord_pretty_help-2.0.5/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "discord-pretty-help"
-version = "2.0.4"
+version = "2.0.5"
 description = "And nicer looking interactive help menu for discord.py"
 authors = ["CasuallyCalm <29642143+casuallycalm@users.noreply.github.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/casuallycalm/discord-pretty-help"
 keywords=["discord", "discord.py", "discord bot"]
 packages = [
```

### Comparing `discord_pretty_help-2.0.4/README.md` & `discord_pretty_help-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `discord_pretty_help-2.0.4/PKG-INFO` & `discord_pretty_help-2.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-pretty-help
-Version: 2.0.4
+Version: 2.0.5
 Summary: And nicer looking interactive help menu for discord.py
 Home-page: https://github.com/casuallycalm/discord-pretty-help
 License: MIT
 Keywords: discord,discord.py,discord bot
 Author: CasuallyCalm
 Author-email: 29642143+casuallycalm@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
```

