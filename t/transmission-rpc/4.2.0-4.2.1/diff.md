# Comparing `tmp/transmission_rpc-4.2.0.tar.gz` & `tmp/transmission_rpc-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transmission_rpc-4.2.0.tar", max compression
+gzip compressed data, was "transmission_rpc-4.2.1.tar", max compression
```

## Comparing `transmission_rpc-4.2.0.tar` & `transmission_rpc-4.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1127 2023-04-09 09:37:20.250403 transmission_rpc-4.2.0/LICENSE
--rw-r--r--   0        0        0     1630 2023-04-09 09:37:20.250403 transmission_rpc-4.2.0/README.md
--rw-r--r--   0        0        0     3147 2023-04-09 09:37:20.250403 transmission_rpc-4.2.0/pyproject.toml
--rw-r--r--   0        0        0     1982 2023-04-09 09:37:20.250403 transmission_rpc-4.2.0/transmission_rpc/__init__.py
--rw-r--r--   0        0        0    45188 2023-04-09 09:37:20.250403 transmission_rpc-4.2.0/transmission_rpc/client.py
--rw-r--r--   0        0        0    11051 2023-04-09 09:37:20.250403 transmission_rpc-4.2.0/transmission_rpc/constants.py
--rw-r--r--   0        0        0     1639 2023-04-09 09:37:20.250403 transmission_rpc-4.2.0/transmission_rpc/error.py
--rw-r--r--   0        0        0    12990 2023-04-09 09:37:20.250403 transmission_rpc-4.2.0/transmission_rpc/session.py
--rw-r--r--   0        0        0    23663 2023-04-09 09:37:20.250403 transmission_rpc-4.2.0/transmission_rpc/torrent.py
--rw-r--r--   0        0        0     1497 2023-04-09 09:37:20.250403 transmission_rpc-4.2.0/transmission_rpc/types.py
--rw-r--r--   0        0        0     2669 2023-04-09 09:37:20.250403 transmission_rpc-4.2.0/transmission_rpc/utils.py
--rw-r--r--   0        0        0     3016 1970-01-01 00:00:00.000000 transmission_rpc-4.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1127 2023-05-01 04:37:29.821111 transmission_rpc-4.2.1/LICENSE
+-rw-r--r--   0        0        0     1630 2023-05-01 04:37:29.821111 transmission_rpc-4.2.1/README.md
+-rw-r--r--   0        0        0     3262 2023-05-01 04:37:29.821111 transmission_rpc-4.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2087 2023-05-01 04:37:29.821111 transmission_rpc-4.2.1/transmission_rpc/__init__.py
+-rw-r--r--   0        0        0    47198 2023-05-01 04:37:29.821111 transmission_rpc-4.2.1/transmission_rpc/client.py
+-rw-r--r--   0        0        0    11533 2023-05-01 04:37:29.821111 transmission_rpc-4.2.1/transmission_rpc/constants.py
+-rw-r--r--   0        0        0     1639 2023-05-01 04:37:29.821111 transmission_rpc-4.2.1/transmission_rpc/error.py
+-rw-r--r--   0        0        0    12990 2023-05-01 04:37:29.821111 transmission_rpc-4.2.1/transmission_rpc/session.py
+-rw-r--r--   0        0        0    23663 2023-05-01 04:37:29.821111 transmission_rpc-4.2.1/transmission_rpc/torrent.py
+-rw-r--r--   0        0        0     1498 2023-05-01 04:37:29.821111 transmission_rpc-4.2.1/transmission_rpc/types.py
+-rw-r--r--   0        0        0     2669 2023-05-01 04:37:29.821111 transmission_rpc-4.2.1/transmission_rpc/utils.py
+-rw-r--r--   0        0        0     3016 1970-01-01 00:00:00.000000 transmission_rpc-4.2.1/PKG-INFO
```

### Comparing `transmission_rpc-4.2.0/LICENSE` & `transmission_rpc-4.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `transmission_rpc-4.2.0/README.md` & `transmission_rpc-4.2.1/README.md`

 * *Files identical despite different names*

### Comparing `transmission_rpc-4.2.0/pyproject.toml` & `transmission_rpc-4.2.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "transmission-rpc"
-version = "4.2.0"
+version = "4.2.1"
 description = "Python module that implements the Transmission bittorent client JSON-RPC protocol"
 authors = ["Trim21 <i@trim21.me>"]
 readme = 'README.md'
 repository = 'https://github.com/Trim21/transmission-rpc'
 license = 'MIT'
 packages = [{ include = 'transmission_rpc' }]
 keywords = ['transmission', 'rpc']
@@ -29,43 +29,37 @@
 [tool.poetry.dependencies]
 python = "^3.7"
 # dependencies
 requests = "^2.23.0"
 typing-extensions = "*"
 
 [tool.poetry.group.docs.dependencies]
-sphinx = { version = "==6.1.3", python = "^3.9" }
+sphinx = { version = "==6.2.1", python = "^3.9" }
 sphinx-rtd-theme = { version = "==1.2.0", python = "^3.9" }
 sphinx-autobuild = { version = "2021.3.14", python = "^3.9" }
 
 [tool.poetry.group.dev.dependencies]
 python-dotenv = [
     { version = "0.21.1", python = "<3.8" },
     { version = "^1.0.0", python = "^3.8" }
 ]
 
-yarl = "==1.8.2"
+yarl = "==1.9.2"
 # tests
-pytest = "==7.2.2"
+pytest = "==7.3.1"
 pytest-github-actions-annotate-failures = "==0.1.8"
-coverage = "==7.2.2"
+coverage = "==7.2.5"
 
 # linter and formatter
-pre-commit = { version = "==3.2.1", markers = "implementation_name != 'pypy'", python = "^3.9" }
-mypy = { version = "==1.1.1", markers = "implementation_name != 'pypy'", python = "^3.9" }
-
-flake8 = { version = "6.0.0", python = "^3.9" }
-flake8-comprehensions = { version = "==3.11.1", python = "^3.9" }
-flake8-bugbear = { version = "==23.3.23", python = "^3.9" }
-flake8-mutable = { version = "1.2.0", python = "^3.9" }
-flake8-pyproject = { version = "1.2.3", python = "^3.9" }
-flake8-pytest-style = { version = "==1.7.2", python = "^3.9" }
+pre-commit = { version = "==3.2.2", markers = "implementation_name != 'pypy'", python = "^3.9" }
+mypy = { version = "==1.2.0", markers = "implementation_name != 'pypy'", python = "^3.9" }
+ruff = "0.0.263"
 
 # stubs
-types-requests = "==2.28.11.17"
+types-requests = "==2.29.0.0"
 pytz = "==2023.3"
 
 [tool.poetry-plugin-bump]
 commit_msg = 'bump: v{version}'
 
 [tool.isort]
 default_section = 'THIRDPARTY'
@@ -84,40 +78,83 @@
 [tool.mypy]
 disallow_untyped_defs = true
 ignore_missing_imports = true
 warn_return_any = false
 warn_unused_configs = true
 show_error_codes = true
 
-[tool.flake8]
-max-line-length = 120
+[tool.black]
+line-length = 120
+target-version = ['py37']
+
+
+[tool.ruff]
+extend-exclude = ["docs"]
+line-length = 120
+select = [
+    "B",
+    "C",
+    "E",
+    "F",
+    "G",
+    "I",
+    "N",
+    "Q",
+    "S",
+    "W",
+    "BLE",
+    "EXE",
+    "ICN",
+    "INP",
+    "ISC",
+    "NPY",
+    "PD",
+    "PGH",
+    "PIE",
+    "PL",
+    "PT",
+    "PYI",
+    "RET",
+    "RSE",
+    "RUF",
+    "SIM",
+    "SLF",
+    "TCH",
+    "TID",
+    "TRY",
+    "YTT",
+]
+
 ignore = [
-    'C103',
-    'C111',
-    'R903',
-    'W503',
-    'W504',
-    'C812',
-    'C813',
-    'C815',
-    'C819',
-    'B008',
-    'E265',
+    'PLR0911',
+    'INP001',
+    'N806',
+    'N802',
+    'N803',
     'E501',
+    'BLE001',
+    'RUF002',
+    'S301',
+    'S314',
+    'S101',
+    'N815',
+    'S104',
+    'C901',
+    'ISC003',
+    'PLR0913',
+    'I001',
+    'RUF001',
+    'SIM108',
+    'TCH003',
+    'RUF003',
+    'RET504',
+    'TRY300',
+    'TRY003',
+    'TRY201',
+    'TRY301',
+    'PLR0912',
+    'PLR0915',
+    'PLR2004',
+    'PGH003',
 ]
-exclude = [
-    '.venv',
-    '.git',
-    '__pycache__',
-    'docs/source/conf.py',
-    'old',
-    'build',
-    'dist',
-    'tmp',
-    'api',
-]
-ban-relative-imports = 'parents'
 
-
-[tool.black]
-line-length = 120
-target-version = ['py37', 'py38']
+target-version = "py37"
```

### Comparing `transmission_rpc-4.2.0/transmission_rpc/__init__.py` & `transmission_rpc-4.2.1/transmission_rpc/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,29 +3,41 @@
 from typing import Union
 
 from transmission_rpc.error import TransmissionError
 from transmission_rpc.types import File, Group
 from transmission_rpc.client import Client
 from transmission_rpc.session import Session
 from transmission_rpc.torrent import Torrent
-from transmission_rpc.constants import LOGGER, PRIORITY, RATIO_LIMIT, DEFAULT_TIMEOUT, Priority, IdleLimit, RatioLimit
+from transmission_rpc.constants import (
+    LOGGER,
+    PRIORITY,
+    RATIO_LIMIT,
+    DEFAULT_TIMEOUT,
+    IdleMode,
+    Priority,
+    IdleLimit,
+    RatioLimit,
+    RatioLimitMode,
+)
 
 __all__ = [
     "Client",
     "Group",
     "DEFAULT_TIMEOUT",
     "PRIORITY",
     "RATIO_LIMIT",
     "LOGGER",
     "TransmissionError",
     "Session",
     "Torrent",
     "File",
     "from_url",
     "Priority",
+    "RatioLimitMode",
+    "IdleMode",
     "RatioLimit",
     "IdleLimit",
 ]
 
 
 def from_url(
     url: str,
```

### Comparing `transmission_rpc-4.2.0/transmission_rpc/client.py` & `transmission_rpc-4.2.1/transmission_rpc/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-import os
 import json
 import time
 import types
 import string
 import logging
 import pathlib
+import warnings
 import urllib.parse
 from typing import Any, Dict, List, Type, Tuple, Union, BinaryIO, Iterable, Optional
 from urllib.parse import quote
 
 import requests
 import requests.auth
 import requests.exceptions
@@ -86,14 +86,28 @@
         password: Optional[str] = None,
         host: str = "127.0.0.1",
         port: int = 9091,
         path: str = "/transmission/rpc",
         timeout: Union[int, float] = DEFAULT_TIMEOUT,
         logger: logging.Logger = LOGGER,
     ):
+        """
+
+        Parameters
+        ----------
+        protocol
+        username
+        password
+        host
+        port
+        path:
+          rpc request target path, default ``/transmission/rpc``
+        timeout
+        logger
+        """
         if isinstance(logger, logging.Logger):
             self.logger = logger
         else:
             raise TypeError(
                 "logger must be instance of `logging.Logger`, default: logging.getLogger('transmission-rpc')"
             )
         self._query_timeout: _Timeout = timeout
@@ -130,15 +144,15 @@
         Set timeout for HTTP queries.
         """
         if isinstance(value, (tuple, list)):
             if len(value) != 2:
                 raise ValueError("timeout tuple can only include 2 numbers elements")
             for v in value:
                 if not isinstance(v, (float, int)):
-                    raise ValueError("element of timeout tuple can only be int of float")
+                    raise TypeError("element of timeout tuple can only be int of float")
             self._query_timeout = (value[0], value[1])  # for type checker
         elif value is None:
             self._query_timeout = DEFAULT_TIMEOUT
         else:
             self._query_timeout = float(value)
 
     @timeout.deleter
@@ -199,19 +213,19 @@
         require_ids: bool = False,
         timeout: Optional[_Timeout] = None,
     ) -> dict:
         """
         Send json-rpc request to Transmission using http POST
         """
         if not isinstance(method, str):
-            raise ValueError("request takes method as string")
+            raise TypeError("request takes method as string")
         if arguments is None:
             arguments = {}
         if not isinstance(arguments, dict):
-            raise ValueError("request takes arguments as dict")
+            raise TypeError("request takes arguments should be dict")
 
         ids = _parse_torrent_ids(ids)
         if len(ids) > 0:
             arguments["ids"] = ids
         elif require_ids:
             raise ValueError("request require ids")
 
@@ -222,17 +236,17 @@
         http_data = self._http_query(query, timeout)
         elapsed = time.time() - start
         self.logger.info("http request took %.3f s", elapsed)
 
         try:
             data: ResponseData = json.loads(http_data)
         except ValueError as error:
-            self.logger.error("Error: %s", str(error))
-            self.logger.error('Request: "%s"', query)
-            self.logger.error('HTTP data: "%s"', http_data)
+            self.logger.exception("Error: %s")
+            self.logger.exception('Request: "%s"', query)
+            self.logger.exception('HTTP data: "%s"', http_data)
             raise TransmissionError(
                 "failed to parse response as json", method=method, argument=arguments, rawResponse=http_data
             ) from error
 
         self.logger.debug(json.dumps(data, indent=2))
         if "result" not in data:
             raise TransmissionError(
@@ -253,15 +267,15 @@
             )
 
         res = data["arguments"]
 
         results = {}
         if method == RpcMethod.TorrentGet:
             return res
-        elif method == RpcMethod.TorrentAdd:
+        if method == RpcMethod.TorrentAdd:
             item = None
             if "torrent-added" in res:
                 item = res["torrent-added"]
             elif "torrent-duplicate" in res:
                 item = res["torrent-duplicate"]
             if item:
                 results[item["id"]] = Torrent(fields=item)
@@ -275,16 +289,15 @@
                 )
         elif method == RpcMethod.SessionGet:
             self.raw_session.update(res)
         elif method == RpcMethod.SessionStats:
             # older versions of T has the return data in "session-stats"
             if "session-stats" in res:
                 return res["session-stats"]
-            else:
-                return res
+            return res
         elif method in (
             RpcMethod.PortTest,
             RpcMethod.BlocklistUpdate,
             RpcMethod.FreeSpace,
             RpcMethod.TorrentRenamePath,
         ):
             return res
@@ -297,17 +310,15 @@
         """Decode the Transmission version string, if available."""
         self.semver_version = self.raw_session.get("rpc-version-semver")
         self.server_version = self.raw_session["version"]
         self.protocol_version = self.raw_session["rpc-version"]
 
     @property
     def rpc_version(self) -> int:
-        """
-        Get the Transmission RPC version. Trying to deduct if the server don't have a version value.
-        """
+        """Get the Transmission daemon RPC version."""
         return self.protocol_version
 
     def _rpc_version_warning(self, required_version: int) -> None:
         """
         Add a warning to the log if the Transmission RPC version is lower then the provided version.
         """
         if self.rpc_version < required_version:
@@ -334,52 +345,52 @@
         labels: Optional[Iterable[str]] = None,
         bandwidthPriority: Optional[int] = None,
     ) -> Torrent:
         """
         Add torrent to transfers list. ``torrent`` can be:
 
         - ``http://``, ``https://`` or  ``magnet:`` URL
-        - torrent file-like object in binary mode
+        - torrent file-like object in **binary mode**
         - bytes of torrent content
         - ``pathlib.Path`` for local torrent file, will be read and encoded as base64.
 
         Warnings
         --------
         base64 string or ``file://`` protocol URL are not supported in v4.
 
         Parameters
         ----------
         torrent:
             torrent to add
         timeout:
             request timeout
-        labels:
-            Array of string labels.
-            Add in rpc 17.
         bandwidthPriority:
             Priority for this transfer.
         cookies:
             One or more HTTP cookie(s).
         download_dir:
             The directory where the downloaded contents will be saved in.
         files_unwanted:
             A list of file id's that shouldn't be downloaded.
         files_wanted:
             A list of file id's that should be downloaded.
         paused:
-            If True, does not start the transfer when added.
+            If ``True``, does not start the transfer when added.
             Magnet url will always start to downloading torrents.
         peer_limit:
             Maximum number of peers allowed.
         priority_high:
             A list of file id's that should have high priority.
         priority_low:
             A list of file id's that should have low priority.
         priority_normal:
             A list of file id's that should have normal priority.
+        labels:
+            Array of string labels.
+            Add in rpc 17.
         """
         if torrent is None:
             raise ValueError("add_torrent requires data or a URI.")
 
         kwargs: Dict[str, Any] = {}
         if download_dir is not None:
             kwargs["download-dir"] = download_dir
@@ -421,16 +432,17 @@
         else:
             kwargs["filename"] = torrent
 
         return list(self._request(RpcMethod.TorrentAdd, kwargs, timeout=timeout).values())[0]
 
     def remove_torrent(self, ids: _TorrentIDs, delete_data: bool = False, timeout: Optional[_Timeout] = None) -> None:
         """
-        remove torrent(s) with provided id(s). Local data is removed if
-        delete_data is True, otherwise not.
+        remove torrent(s) with provided id(s).
+
+        Local data will be removed by transmission daemon if ``delete_data`` is set to ``True``.
         """
         self._request(
             RpcMethod.TorrentRemove,
             {"delete-local-data": delete_data},
             ids,
             True,
             timeout=timeout,
@@ -497,14 +509,18 @@
 
         arguments:
             fetched torrent arguments, in most cases you don't need to set this,
             transmission-rpc will fetch all torrent fields it supported.
 
         timeout:
             requests timeout
+
+        Raises
+        ------
+        KeyError: torrent with given ``torrent_id`` not found
         """
         if arguments:
             arguments = list(set(arguments) | {"id", "hashString"})
         else:
             arguments = self.torrent_get_arguments
         torrent_id = _parse_torrent_id(torrent_id)
         if torrent_id is None:
@@ -526,15 +542,15 @@
     def get_torrents(
         self,
         ids: Optional[_TorrentIDs] = None,
         arguments: Optional[Iterable[str]] = None,
         timeout: Optional[_Timeout] = None,
     ) -> List[Torrent]:
         """
-        Get information for torrents with provided ids. For more information see ``get_torrent``.
+        Get information for torrents with provided ids. For more information see :py:meth:`Client.get_torrent`.
 
         Returns a list of Torrent object.
         """
         if arguments:
             arguments = list(set(arguments) | {"id", "hashString"})
         else:
             arguments = self.torrent_get_arguments
@@ -632,53 +648,63 @@
         priority_low
             list of file id to set low download priority
         priority_normal
             list of file id to set normal download priority
         seed_ratio_limit
             Seed inactivity limit in minutes.
         seed_ratio_mode
-            Which ratio to use.
-
-            0 = Use session limit
-
-            1 = Use transfer limit
+            Torrent seed ratio mode
 
-            2 = Disable limit.
+            Valid options are :py:class:`transmission_rpc.constants.RatioLimitMode`
         seed_idle_limit
             torrent-level seeding ratio
         seed_idle_mode
             Seed inactivity mode.
 
-            0 = Use session limit
+            Valid options are :py:class:`transmission_rpc.constants.IdleMode`
 
-            1 = Use transfer limit
-
-            2 = Disable limit.
-        tracker_add
+        tracker_add:
             Array of string with announce URLs to add.
-        tracker_remove
+
+            Warnings
+            --------
+            since transmission daemon 4.0.0, this argument is deprecated, use ``tracker_list`` instead.
+
+        tracker_remove:
             Array of ids of trackers to remove.
-        tracker_replace
-            Array of (id, url) tuples where the announce URL should be replaced.
+
+            Warnings
+            --------
+            since transmission daemon 4.0.0, this argument is deprecated, use ``tracker_list`` instead.
+
+        tracker_replace:
+            Array of (id, url) tuples where the announcement URL should be replaced.
+
+            Warnings
+            --------
+            since transmission daemon 4.0.0, this argument is deprecated, use ``tracker_list`` instead.
+
         labels
             Array of string labels.
             Add in rpc 16.
+
         group
             The name of this torrent's bandwidth group.
             Add in rpc 17.
+
         tracker_list
             A ``Iterable[Iterable[str]]``, each ``Iterable[str]`` for a tracker tier.
             Add in rpc 17.
 
 
         Warnings
         ----
         ``kwargs`` is for the future features not supported yet, it's not compatibility promising.
 
-        it will be bypassed to request arguments.
+        It will be bypassed to request arguments **as-is**, the underline in the key will not be replaced, so you should use kwargs like ``{'a-argument': 'value'}``
         """
 
         args: Dict[str, Any] = {}
 
         if bandwidth_priority is not None:
             args["bandwidthPriority"] = bandwidth_priority
 
@@ -742,62 +768,106 @@
             ValueError("No arguments to set")
 
     def move_torrent_data(
         self,
         ids: _TorrentIDs,
         location: Union[str, pathlib.Path],
         timeout: Optional[_Timeout] = None,
+        *,
+        move: bool = True,
     ) -> None:
-        """Move torrent data to the new location."""
-        args = {"location": ensure_location_str(location), "move": True}
+        """
+        Move torrent data to the new location.
+
+        See Also
+        --------
+
+        `RPC Spec: moving-a-torrent <https://github.com/transmission/transmission/blob/main/docs/rpc-spec.md#36-moving-a-torrent>`_
+        """
+        args = {"location": ensure_location_str(location), "move": bool(move)}
         self._request(RpcMethod.TorrentSetLocation, args, ids, True, timeout=timeout)
 
     def locate_torrent_data(
         self,
         ids: _TorrentIDs,
         location: Union[str, pathlib.Path],
         timeout: Optional[_Timeout] = None,
     ) -> None:
-        """Locate torrent data at the provided location."""
-        args = {"location": ensure_location_str(location), "move": False}
-        self._request(RpcMethod.TorrentSetLocation, args, ids, True, timeout=timeout)
+        """
+        Locate torrent data at the provided location.
+
+        Warnings
+        --------
+            since transmission-rpc version 4.2.1, this method is deprecated.
+
+            Use ``client.move_torrent_data(ids, location, move=False)`` instead
+
+        this is same rpc call as :py:meth:`Client.move_torrent_data`, but with arguments ``move=False``
+
+        See Also
+        --------
+
+        `RPC Spec: moving-a-torrent <https://github.com/transmission/transmission/blob/main/docs/rpc-spec.md#36-moving-a-torrent>`_
+        """
+        warnings.warn(
+            "locate_torrent_data is deprecated since version 4.2.1, please use `move_torrent_data` with 'move=False'",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        return self.move_torrent_data(ids=ids, location=location, timeout=timeout, move=False)
 
     def rename_torrent_path(
         self,
         torrent_id: _TorrentID,
-        location: Union[str, pathlib.Path],
+        location: str,
         name: str,
         timeout: Optional[_Timeout] = None,
     ) -> Tuple[str, str]:
         """
-        https://github.com/transmission/transmission/blob/main/docs/rpc-spec.md#37-renaming-a-torrents-path
-
+        Warnings
+        --------
         This method can only be called on single torrent.
+
+        Warnings
+        --------
+        This is not the method to move torrent data directory,
+
+        See Also
+        --------
+        `RPC Spec: renaming-a-torrents-path <https://github.com/transmission/transmission/blob/main/docs/rpc-spec.md#37-renaming-a-torrents-path>`_
         """
         self._rpc_version_warning(15)
         torrent_id = _parse_torrent_id(torrent_id)
+
         name = name.strip()  # https://github.com/trim21/transmission-rpc/issues/185
-        dirname = os.path.dirname(name)
-        if len(dirname) > 0:
-            raise ValueError("Target name cannot contain a path delimiter")
+
         result = self._request(
             RpcMethod.TorrentRenamePath,
             {"path": ensure_location_str(location), "name": name},
             torrent_id,
             True,
             timeout=timeout,
         )
+
         return result["path"], result["name"]
 
     def queue_top(self, ids: _TorrentIDs, timeout: Optional[_Timeout] = None) -> None:
-        """Move transfer to the top of the queue:_Timeout."""
+        """
+        Move transfer to the top of the queue.
+
+        https://github.com/transmission/transmission/blob/main/docs/rpc-spec.md#46-queue-movement-requests
+        """
         self._request(RpcMethod.QueueMoveTop, ids=ids, require_ids=True, timeout=timeout)
 
     def queue_bottom(self, ids: _TorrentIDs, timeout: Optional[_Timeout] = None) -> None:
-        """Move transfer to the bottom of the queue."""
+        """
+        Move transfer to the bottom of the queue.
+
+        https://github.com/transmission/transmission/blob/main/docs/rpc-spec.md#46-queue-movement-requests
+        """
         self._request(RpcMethod.QueueMoveBottom, ids=ids, require_ids=True, timeout=timeout)
 
     def queue_up(self, ids: _TorrentIDs, timeout: Optional[_Timeout] = None) -> None:
         """Move transfer up in the queue."""
         self._request(RpcMethod.QueueMoveUp, ids=ids, require_ids=True, timeout=timeout)
 
     def queue_down(self, ids: _TorrentIDs, timeout: Optional[_Timeout] = None) -> None:
@@ -967,17 +1037,17 @@
         script_torrent_done_seeding_enabled:
             whether or not to call the ``seeding-done`` script
         script_torrent_done_seeding_filename:
             filename of the script to run
 
         Warnings
         ----
-        ``kwargs`` is for the future features not supported yet, it's not compatibility promising.
+        ``kwargs`` is pass the arguments not supported yet future, it's not compatibility promising.
 
-        it will be bypassed to request arguments.
+        transmission-rpc will merge ``kwargs`` in rpc arguments *as-is*
         """
         args: Dict[str, Any] = {}
 
         if alt_speed_down is not None:
             args["alt-speed-down"] = alt_speed_down
         if alt_speed_enabled is not None:
             args["alt-speed-enabled"] = alt_speed_enabled
```

### Comparing `transmission_rpc-4.2.0/transmission_rpc/constants.py` & `transmission_rpc-4.2.1/transmission_rpc/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,39 +35,53 @@
 
 # TODO: remove this in 5.0
 TR_RATIOLIMIT_GLOBAL = 0  # follow the global settings
 TR_RATIOLIMIT_SINGLE = 1  # override the global settings, seeding until a certain ratio
 TR_RATIOLIMIT_UNLIMITED = 2  # override the global settings, seeding regardless of ratio
 
 
-class RatioLimit(enum.IntEnum):
+class RatioLimitMode(enum.IntEnum):
+    """torrent radio limit mode"""
+
+    #: follow the global settings
     Global = TR_RATIOLIMIT_GLOBAL
+    #: override the global settings, seeding until a certain ratio
     Single = TR_RATIOLIMIT_SINGLE
+    #: override the global settings, seeding regardless of ratio
     Unlimited = TR_RATIOLIMIT_UNLIMITED
 
 
+# TODO: remove these in 5.0
+RatioLimit = RatioLimitMode
+
 RATIO_LIMIT = mirror_dict(
     {
         "global": TR_RATIOLIMIT_GLOBAL,
         "single": TR_RATIOLIMIT_SINGLE,
         "unlimited": TR_RATIOLIMIT_UNLIMITED,
     }
 )
 
 
-class IdleLimit(enum.IntEnum):
+class IdleMode(enum.IntEnum):
+    """torrent idle mode"""
+
+    #: follow the global settings
     Global = 0
+    #: override the global settings, seeding until a certain idle time
     Single = 1
+    #: override the global settings, seeding regardless of activity
     Unlimited = 2
 
 
-# TODO: remove this in 5.0
-TR_IDLELIMIT_GLOBAL = IdleLimit.Global  # follow the global settings
-TR_IDLELIMIT_SINGLE = IdleLimit.Single  # override the global settings, seeding until a certain idle time
-TR_IDLELIMIT_UNLIMITED = IdleLimit.Unlimited  # override the global settings, seeding regardless of activity
+# TODO: remove these in 5.0
+IdleLimit = IdleMode
+TR_IDLELIMIT_GLOBAL = IdleMode.Global  # follow the global settings
+TR_IDLELIMIT_SINGLE = IdleMode.Single  # override the global settings, seeding until a certain idle time
+TR_IDLELIMIT_UNLIMITED = IdleMode.Unlimited  # override the global settings, seeding regardless of activity
 
 IDLE_LIMIT = mirror_dict(
     {
         "global": TR_RATIOLIMIT_GLOBAL,
         "single": TR_RATIOLIMIT_SINGLE,
         "unlimited": TR_RATIOLIMIT_UNLIMITED,
     }
@@ -101,16 +115,14 @@
     string = "string"
     array = "array"
     boolean = "boolean"
     double = "double"
     object = "object"
 
 
-trackerListDescription = "A Iterable[Iterable[str]] for a set of announce URLs, each inner list is for a tier"
-
 TORRENT_GET_ARGS: Dict[str, Args] = {
     "activityDate": Args(Type.number, 1, description="Last time of upload or download activity."),
     "addedDate": Args(Type.number, 1, description="The date when this torrent was first added."),
     "bandwidthPriority": Args(Type.number, 5, description="Bandwidth priority. Low (-1), Normal (0) or High (1)."),
     "comment": Args(Type.string, 1, description="Torrent comment."),
     "corruptEver": Args(Type.number, 1, description="Number of bytes of corrupt data downloaded."),
     "creator": Args(Type.string, 1, description="Torrent creator."),
@@ -195,30 +207,34 @@
     "uploadLimit": Args(Type.number, 1, None, None, None, "Upload limit in Kbps"),
     "uploadLimited": Args(Type.boolean, 5, None, None, None, "Upload limit enabled."),
     "uploadRatio": Args(Type.double, 1, None, None, None, "Seed ratio."),
     "wanted": Args(Type.array, 1, description="Array of booleans indicated wanted files."),
     "webseeds": Args(Type.array, 1, None, None, None, "Array of webseeds objects"),
     "webseedsSendingToUs": Args(Type.number, 1, None, None, None, "Number of webseeds seeding to us."),
     "file-count": Args(Type.number, 17),
-    "trackerList": Args(Type.array, 17, description=trackerListDescription),
+    "trackerList": Args(
+        Type.array,
+        17,
+        description="A Iterable[Iterable[str]] for a set of announce URLs, each inner list is for a tier",
+    ),
 }
 
 
 class RpcMethod(str, enum.Enum):
     SessionSet = "session-set"
     SessionGet = "session-get"
     SessionStats = "session-stats"
 
     TorrentGet = "torrent-get"
     TorrentAdd = "torrent-add"
     TorrentSet = "torrent-set"
     TorrentRemove = "torrent-remove"
 
     TorrentStart = "torrent-start"
-    TorrentStartNow = "torrent-start-now"
+    TorrentStartNow = "torrent-start-now"  # added in 2.40
     TorrentStop = "torrent-stop"
 
     TorrentVerify = "torrent-verify"
     TorrentReannounce = "torrent-reannounce"
 
     TorrentSetLocation = "torrent-set-location"
     TorrentRenamePath = "torrent-rename-path"
```

### Comparing `transmission_rpc-4.2.0/transmission_rpc/error.py` & `transmission_rpc-4.2.1/transmission_rpc/error.py`

 * *Files identical despite different names*

### Comparing `transmission_rpc-4.2.0/transmission_rpc/session.py` & `transmission_rpc-4.2.1/transmission_rpc/session.py`

 * *Files identical despite different names*

### Comparing `transmission_rpc-4.2.0/transmission_rpc/torrent.py` & `transmission_rpc-4.2.1/transmission_rpc/torrent.py`

 * *Files identical despite different names*

### Comparing `transmission_rpc-4.2.0/transmission_rpc/types.py` & `transmission_rpc-4.2.1/transmission_rpc/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 class Container:
     fields: Dict[str, Any]  #: raw fields
 
     def __init__(self, *, fields: Dict[str, Any]):
         self.fields = fields
 
     def get(self, key: str, default: Optional[T] = None) -> Any:
-        """get the raw value from files by the **raw keys**"""
+        """get the raw value by the **raw rpc response key**"""
         return self.fields.get(key, default)
 
 
 class File(NamedTuple):
     name: str  # file name
     size: int  # file size in bytes
     completed: int  # bytes completed
```

### Comparing `transmission_rpc-4.2.0/transmission_rpc/utils.py` & `transmission_rpc-4.2.1/transmission_rpc/utils.py`

 * *Files identical despite different names*

### Comparing `transmission_rpc-4.2.0/PKG-INFO` & `transmission_rpc-4.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transmission-rpc
-Version: 4.2.0
+Version: 4.2.1
 Summary: Python module that implements the Transmission bittorent client JSON-RPC protocol
 Home-page: https://github.com/Trim21/transmission-rpc
 License: MIT
 Keywords: transmission,rpc
 Author: Trim21
 Author-email: i@trim21.me
 Requires-Python: >=3.7,<4.0
```

