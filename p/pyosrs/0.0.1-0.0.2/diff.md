# Comparing `tmp/pyosrs-0.0.1.tar.gz` & `tmp/pyosrs-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyosrs-0.0.1.tar", max compression
+gzip compressed data, was "pyosrs-0.0.2.tar", max compression
```

## Comparing `pyosrs-0.0.1.tar` & `pyosrs-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     7652 2023-04-29 20:20:17.125414 pyosrs-0.0.1/LICENSE
--rw-r--r--   0        0        0     2471 2023-04-29 20:20:17.125414 pyosrs-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-04-29 20:20:17.125414 pyosrs-0.0.1/pyosrs/__init__.py
--rw-r--r--   0        0        0     6175 2023-04-29 20:20:17.125414 pyosrs-0.0.1/pyosrs/client.py
--rw-r--r--   0        0        0     5072 2023-04-29 20:20:17.125414 pyosrs-0.0.1/pyosrs/enums.py
--rw-r--r--   0        0        0      396 2023-04-29 20:20:17.125414 pyosrs-0.0.1/pyosrs/exceptions.py
--rw-r--r--   0        0        0     3893 2023-04-29 20:20:17.125414 pyosrs-0.0.1/pyosrs/models.py
--rw-r--r--   0        0        0      930 2023-04-29 20:20:17.125414 pyosrs-0.0.1/pyosrs/utils.py
--rw-r--r--   0        0        0      768 2023-04-29 20:20:17.125414 pyosrs-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3106 1970-01-01 00:00:00.000000 pyosrs-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     7652 2023-05-01 09:12:56.594442 pyosrs-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2466 2023-05-01 09:12:56.594442 pyosrs-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-01 09:12:56.594442 pyosrs-0.0.2/pyosrs/__init__.py
+-rw-r--r--   0        0        0     6418 2023-05-01 09:12:56.594442 pyosrs-0.0.2/pyosrs/client.py
+-rw-r--r--   0        0        0     5072 2023-05-01 09:12:56.594442 pyosrs-0.0.2/pyosrs/enums.py
+-rw-r--r--   0        0        0      410 2023-05-01 09:12:56.594442 pyosrs-0.0.2/pyosrs/exceptions.py
+-rw-r--r--   0        0        0     3893 2023-05-01 09:12:56.594442 pyosrs-0.0.2/pyosrs/models.py
+-rw-r--r--   0        0        0      901 2023-05-01 09:12:56.594442 pyosrs-0.0.2/pyosrs/utils.py
+-rw-r--r--   0        0        0      768 2023-05-01 09:12:56.594442 pyosrs-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3101 1970-01-01 00:00:00.000000 pyosrs-0.0.2/PKG-INFO
```

### Comparing `pyosrs-0.0.1/LICENSE` & `pyosrs-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyosrs-0.0.1/README.md` & `pyosrs-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -88,8 +88,8 @@
 make mypy
 make tests
 make precommit
 ```
 
 ## License
 
-pyosrs is licensed under the GNU Lesser General Public License. See [LICENSE](https://github.com/phongse/pyosrs-test/blob/main/LICENSE).
+pyosrs is licensed under the GNU Lesser General Public License. See [LICENSE](https://github.com/phongse/pyosrs/blob/main/LICENSE).
```

### Comparing `pyosrs-0.0.1/pyosrs/client.py` & `pyosrs-0.0.2/pyosrs/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,22 +43,24 @@
         self, username: str, game_mode: GAME_MODE = GAME_MODE.MAIN
     ) -> Hiscore:
         """
         Retrieves the hiscore for a given user and game mode.
 
         Args:
             username (str): The username of the player to retrieve hiscore for.
-            game_mode (GAME_MODE, optional): The game mode to retrieve hiscore for. Defaults to GAME_MODE.MAIN.
+            game_mode (GAME_MODE, optional): The game mode to retrieve hiscore
+            for. Defaults to GAME_MODE.MAIN.
 
         Returns:
             Hiscore: The parsed hiscore data for the given username and game mode.
 
         Raises:
             InvalidUserException: If the given username is invalid.
-            InvalidAPIResponseException: If there is a new type of hiscore data response that hasn't been accounted for.
+            InvalidAPIResponseException: If there is a new type of hiscore data
+            response that hasn't been accounted for.
         """
 
         try:
             response = await self._get_hiscore(username, game_mode)
         except httpx.HTTPStatusError:
             raise InvalidUserException(username)
 
@@ -104,29 +106,33 @@
             minigames=Minigames(**minigames),
             clues=Clues(**clues),
             bosses=Bosses(**bosses),
         )
 
     async def get_game_mode(self, username: str) -> Tuple[GAME_MODE, Hiscore]:
         """
-        Determines the game mode of a given username by comparing the experience levels across different modes using the hiscore API.
+        Determines the game mode of a given username by comparing the experience
+        levels across different modes using the hiscore API.
 
         Args:
             username (str): The username to search.
 
         Returns:
-            A tuple containing the game mode and the corresponding Hiscore object representing the player's stats in that mode. The game mode can be one of the following:
+            A tuple containing the game mode and the corresponding Hiscore object
+            representing the player's stats in that mode. The game mode can be one
+            of the following:
 
             - GAME_MODE.MAIN: Main mode
             - GAME_MODE.IRONMAN: Ironman mode
             - GAME_MODE.HARDCORE: Hardcore mode
             - GAME_MODE.ULTIMATE: Ultimate mode
 
         Raises:
-            InvalidUserException: If the hiscore API returns an error or no hiscore data is found for the given username.
+            InvalidUserException: If the hiscore API returns an error or no
+            hiscore data is found for the given username.
         """
 
         game_modes = [
             GAME_MODE.MAIN,
             GAME_MODE.IRONMAN,
             GAME_MODE.HARDCORE,
             GAME_MODE.ULTIMATE,
@@ -136,29 +142,30 @@
             for game_mode in game_modes
         ]
         hiscores = {}
         for task in asyncio.as_completed(tasks):
             try:
                 hiscore = await asyncio.shield(task)
                 hiscores[hiscore.game_mode] = hiscore
-            except:
+            except:  # noqa: E722
                 pass
 
-        print(hiscores)
         if not hiscores:
             raise InvalidUserException(username)
 
         if GAME_MODE.MAIN in hiscores:
-            if (
+            if GAME_MODE.IRONMAN not in hiscores or (
                 GAME_MODE.IRONMAN in hiscores
                 and hiscores[GAME_MODE.IRONMAN].skills.overall.experience
                 < hiscores[GAME_MODE.MAIN].skills.overall.experience
             ):
                 return GAME_MODE.MAIN, hiscores[GAME_MODE.MAIN]
 
+        # We want to ensure that the user has an ironman hiscore entry
+        # in case they don't meet the requirements to be on the main hiscore
         if GAME_MODE.IRONMAN not in hiscores:
             raise InvalidUserException(username)
 
         if (
             GAME_MODE.HARDCORE in hiscores
             and hiscores[GAME_MODE.HARDCORE].skills.overall.experience
             >= hiscores[GAME_MODE.IRONMAN].skills.overall.experience
```

### Comparing `pyosrs-0.0.1/pyosrs/enums.py` & `pyosrs-0.0.2/pyosrs/enums.py`

 * *Files identical despite different names*

### Comparing `pyosrs-0.0.1/pyosrs/models.py` & `pyosrs-0.0.2/pyosrs/models.py`

 * *Files identical despite different names*

### Comparing `pyosrs-0.0.1/pyosrs/utils.py` & `pyosrs-0.0.2/pyosrs/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-from .models import Skills
-
-
 def base(defence: int, hitpoints: int, prayer: int) -> float:
     return (1 / 4) * (defence + hitpoints + int(prayer * 0.5))
 
 
 def melee(attack: int, strength: int) -> float:
     return (13 / 40) * (attack + strength)
```

### Comparing `pyosrs-0.0.1/pyproject.toml` & `pyosrs-0.0.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyosrs"
-version = "0.0.1"
+version = "0.0.2"
 description = "A Python library for Oldschool RuneScape."
 authors = ["Phong Tran"]
 repository = "https://github.com/phongse/pyosrs"
 license = "LGPL-3.0-only"
 readme = "README.md"
 
 [tool.poetry.dependencies]
@@ -15,21 +15,21 @@
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 coverage = "^7.2.3"
 factory-boy = "^3.2.1"
-isort = "^5.12.0"
 mypy = "^1.2.0"
 pre-commit = "^3.2.2"
 pytest = "^7.3.1"
 pytest-asyncio = "^0.21.0"
 pytest-mock = "^3.10.0"
 respx = "^0.20.1"
+ruff = "^0.0.263"
 
 [tool.isort]
 profile = "black"
 
 [tool.mypy]
 exclude = [
     "testing/",
```

### Comparing `pyosrs-0.0.1/PKG-INFO` & `pyosrs-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyosrs
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python library for Oldschool RuneScape.
 Home-page: https://github.com/phongse/pyosrs
 License: LGPL-3.0-only
 Author: Phong Tran
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
@@ -105,9 +105,9 @@
 make mypy
 make tests
 make precommit
 ```
 
 ## License
 
-pyosrs is licensed under the GNU Lesser General Public License. See [LICENSE](https://github.com/phongse/pyosrs-test/blob/main/LICENSE).
+pyosrs is licensed under the GNU Lesser General Public License. See [LICENSE](https://github.com/phongse/pyosrs/blob/main/LICENSE).
```

