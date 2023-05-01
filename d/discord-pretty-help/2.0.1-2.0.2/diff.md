# Comparing `tmp/discord_pretty_help-2.0.1.tar.gz` & `tmp/discord_pretty_help-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord_pretty_help-2.0.1.tar", max compression
+gzip compressed data, was "discord_pretty_help-2.0.2.tar", max compression
```

## Comparing `discord_pretty_help-2.0.1.tar` & `discord_pretty_help-2.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1090 2023-04-25 00:07:00.401776 discord_pretty_help-2.0.1/LICENSE
--rw-r--r--   0        0        0      105 2023-04-24 23:19:49.870141 discord_pretty_help-2.0.1/pretty_help/__init__.py
--rw-r--r--   0        0        0      500 2023-04-24 23:19:49.870141 discord_pretty_help-2.0.1/pretty_help/abc_menu.py
--rw-r--r--   0        0        0     4115 2023-04-24 23:41:04.752836 discord_pretty_help-2.0.1/pretty_help/app_menu.py
--rw-r--r--   0        0        0     5332 2023-04-24 23:19:49.870141 discord_pretty_help-2.0.1/pretty_help/emoji_menu.py
--rw-r--r--   0        0        0    22368 2023-04-24 23:50:49.016730 discord_pretty_help-2.0.1/pretty_help/pretty_help.py
--rw-r--r--   0        0        0      747 2023-04-25 16:51:15.687271 discord_pretty_help-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     3784 2023-04-24 23:33:06.552434 discord_pretty_help-2.0.1/README.md
--rw-r--r--   0        0        0     4460 1970-01-01 00:00:00.000000 discord_pretty_help-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-05-01 15:55:28.427405 discord_pretty_help-2.0.2/LICENSE
+-rw-r--r--   0        0        0      105 2023-05-01 15:55:28.443661 discord_pretty_help-2.0.2/pretty_help/__init__.py
+-rw-r--r--   0        0        0      500 2023-05-01 15:55:28.443661 discord_pretty_help-2.0.2/pretty_help/abc_menu.py
+-rw-r--r--   0        0        0     4184 2023-05-01 15:55:28.444660 discord_pretty_help-2.0.2/pretty_help/app_menu.py
+-rw-r--r--   0        0        0     5332 2023-05-01 15:55:28.445658 discord_pretty_help-2.0.2/pretty_help/emoji_menu.py
+-rw-r--r--   0        0        0    22753 2023-05-01 15:55:28.446687 discord_pretty_help-2.0.2/pretty_help/pretty_help.py
+-rw-r--r--   0        0        0      747 2023-05-01 16:27:57.343550 discord_pretty_help-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3784 2023-05-01 15:55:28.428405 discord_pretty_help-2.0.2/README.md
+-rw-r--r--   0        0        0     4460 1970-01-01 00:00:00.000000 discord_pretty_help-2.0.2/PKG-INFO
```

### Comparing `discord_pretty_help-2.0.1/LICENSE` & `discord_pretty_help-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `discord_pretty_help-2.0.1/pretty_help/app_menu.py` & `discord_pretty_help-2.0.2/pretty_help/app_menu.py`

 * *Files 20% similar despite different names*

```diff
@@ -49,35 +49,35 @@
 
     @discord.ui.button(
         label="Previous",
         style=discord.ButtonStyle.success,
         row=1,
         custom_id="pretty_help:previous",
     )
-    async def previous(self, interaction: discord.Interaction):
+    async def previous(self, interaction: discord.Interaction, button:discord.Button):
         self.index -= 1
         await self.update(interaction)
 
     @discord.ui.button(
         label="Next",
         style=discord.ButtonStyle.primary,
         row=1,
         custom_id="pretty_help:next",
     )
-    async def next(self, interaction: discord.Interaction):
+    async def next(self, interaction: discord.Interaction, button:discord.Button):
         self.index += 1
         await self.update(interaction)
 
     @discord.ui.button(
         label="Delete",
         style=discord.ButtonStyle.danger,
         row=1,
         custom_id="pretty_help:delete",
     )
-    async def _delete(self, interaction: discord.Interaction):
+    async def _delete(self, interaction: discord.Interaction, button:discord.Button):
         await interaction.message.delete()
 
     @discord.ui.select(row=2, custom_id="pretty_help:select")
     async def select(self, interaction: discord.Interaction, select: Select):
         self.index = int(select.values[0])
         await self.update(interaction)
```

### Comparing `discord_pretty_help-2.0.1/pretty_help/emoji_menu.py` & `discord_pretty_help-2.0.2/pretty_help/emoji_menu.py`

 * *Files identical despite different names*

### Comparing `discord_pretty_help-2.0.1/pretty_help/pretty_help.py` & `discord_pretty_help-2.0.2/pretty_help/pretty_help.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 __all__ = ["PrettyHelp", "Paginator"]
 
 from random import randint
-from typing import Any, Dict, List, Optional, Union
+from typing import List, Optional, Union
 
 import discord
 from discord import app_commands
 from discord.ext import commands
 from discord.ext.commands.help import HelpCommand
 
+from .abc_menu import PrettyMenu
 from .app_menu import AppMenu
 
 
 class Paginator:
     """A class that creates pages for Discord messages.
 
     Attributes
@@ -31,24 +32,28 @@
     thumbnail_url: Optional[:class:`str`]
         The url of the thumbnail to be used on the embed
     """
 
     ending_note: str
 
     def __init__(
-        self, show_index, color=0, image_url: str = None, thumbnail_url: str = None
+        self,
+        show_index: bool,
+        color: discord.Color = 0,
+        image_url: str = None,
+        thumbnail_url: str = None,
     ):
-        # self.ending_note = None
-        self.color = color
         self.char_limit = 6000
+        self.color = color
+        self.ending_note = ""
         self.field_limit = 25
+        self.image_url = image_url
         self.prefix = "```"
-        self.suffix = "```"
         self.show_index = show_index
-        self.image_url = image_url
+        self.suffix = "```"
         self.thumbnail_url = thumbnail_url
         self.clear()
 
     def clear(self):
         """Clears the paginator to have no pages."""
         self._pages = []
 
@@ -124,15 +129,14 @@
         Args:
             embed (discord.Embed): The page to add command descriptions
             page_title (str): The title of the page
             commands_list(List[Union[commands.Command, app_commands.commands.Command]]): The list of commands for the fields
         """
 
         for command in command_list:
-
             if isinstance(command, commands.Command):
                 short_doc = command.short_doc
             else:
                 short_doc = command.description.split("\n", 1)[0]
             if not self._check_embed(
                 embed,
                 self.ending_note,
@@ -328,35 +332,47 @@
         Defaults to ``True``.
     image_url: Optional[:class:`str`]
         The url of the image to be used on the embed
     thumbnail_url: Optional[:class:`str`]
         The url of the thumbnail to be used on the embed
     """
 
-    def __init__(self, **options):
-
-        self.dm_help = options.pop("dm_help", False)
-        self.index_title = options.pop("index_title", "Categories")
-        self.no_category = options.pop("no_category", "No Category")
-        self.sort_commands = options.pop("sort_commands", True)
-        self.menu = options.pop("menu", AppMenu())
-        self.paginator = Paginator(
-            show_index=options.pop("show_index", True),
-            color=options.pop(
-                "color",
-                discord.Color.from_rgb(
-                    randint(0, 255), randint(0, 255), randint(0, 255)
-                ),
-            ),
-            image_url=options.pop("image_url", None),
-            thumbnail_url=options.pop("thumbnail_url", None),
+    def __init__(
+        self,
+        case_insensitive: Optional[bool] = False,
+        color: Optional[discord.Color] = discord.Color.from_rgb(
+            randint(0, 255), randint(0, 255), randint(0, 255)
+        ),
+        delete_invoke: Optional[bool] = False,
+        dm_help: Optional[bool] = False,
+        ending_note: Optional[str] = "",
+        image_url: Optional[str] = None,
+        index_title: Optional[str] = "Categories",
+        menu: Optional[PrettyMenu] = AppMenu(),
+        no_category: Optional[str] = "No Category",
+        paginator: Optional[Paginator] = None,
+        show_index: Optional[bool] = True,
+        sort_commands: Optional[bool] = True,
+        thumbnail_url: Optional[str] = None,
+        **options,
+    ):
+        self.dm_help = dm_help
+        self.index_title = index_title
+        self.no_category = no_category
+        self.sort_commands = sort_commands
+        self.menu = menu
+        self.paginator = paginator or Paginator(
+            show_index=show_index,
+            color=color,
+            image_url=image_url,
+            thumbnail_url=thumbnail_url,
         )
-        self.case_insensitive = options.pop("case_insensitive", False)
-        self.ending_note = options.pop("ending_note", "")
-        self.delete_invoke = options.pop("delete_invoke", False)
+        self.case_insensitive = case_insensitive
+        self.ending_note = ending_note
+        self.delete_invoke = delete_invoke
 
         super().__init__(**options)
 
     def _add_to_bot(self, bot: commands.Bot) -> None:
         super()._add_to_bot(bot)
         self.bot = bot
         bot.tree.add_command(self._app_command_callback)
```

### Comparing `discord_pretty_help-2.0.1/pyproject.toml` & `discord_pretty_help-2.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "discord-pretty-help"
-version = "2.0.1"
+version = "2.0.2"
 description = "And nicer looking interactive help menu for discord.py"
 authors = ["CasuallyCalm <29642143+casuallycalm@users.noreply.github.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/casuallycalm/discord-pretty-help"
 keywords=["discord", "discord.py", "discord bot"]
 packages = [
```

### Comparing `discord_pretty_help-2.0.1/README.md` & `discord_pretty_help-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `discord_pretty_help-2.0.1/PKG-INFO` & `discord_pretty_help-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-pretty-help
-Version: 2.0.1
+Version: 2.0.2
 Summary: And nicer looking interactive help menu for discord.py
 Home-page: https://github.com/casuallycalm/discord-pretty-help
 License: MIT
 Keywords: discord,discord.py,discord bot
 Author: CasuallyCalm
 Author-email: 29642143+casuallycalm@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
```

