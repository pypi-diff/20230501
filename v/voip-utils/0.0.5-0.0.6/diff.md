# Comparing `tmp/voip-utils-0.0.5.tar.gz` & `tmp/voip-utils-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voip-utils-0.0.5.tar", last modified: Thu Apr 20 22:02:34 2023, max compression
+gzip compressed data, was "voip-utils-0.0.6.tar", last modified: Mon May  1 15:26:07 2023, max compression
```

## Comparing `voip-utils-0.0.5.tar` & `voip-utils-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-20 22:02:34.428660 voip-utils-0.0.5/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11357 2022-11-22 20:23:02.000000 voip-utils-0.0.5/LICENSE.md
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      777 2023-04-20 22:02:34.428660 voip-utils-0.0.5/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       39 2023-04-06 16:12:50.000000 voip-utils-0.0.5/README.md
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1969 2023-04-20 22:02:22.000000 voip-utils-0.0.5/pyproject.toml
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      299 2023-04-20 22:02:34.428660 voip-utils-0.0.5/setup.cfg
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-20 22:02:34.428660 voip-utils-0.0.5/voip_utils/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      158 2023-04-06 17:22:11.000000 voip-utils-0.0.5/voip_utils/__init__.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      170 2023-04-06 15:51:26.000000 voip-utils-0.0.5/voip_utils/error.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7191 2023-04-20 20:08:03.000000 voip-utils-0.0.5/voip_utils/rtp_audio.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5984 2023-04-20 17:19:08.000000 voip-utils-0.0.5/voip_utils/sip.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      257 2023-04-06 18:58:36.000000 voip-utils-0.0.5/voip_utils/util.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     6284 2023-04-20 21:46:06.000000 voip-utils-0.0.5/voip_utils/voip.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-20 22:02:34.428660 voip-utils-0.0.5/voip_utils.egg-info/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      777 2023-04-20 22:02:34.000000 voip-utils-0.0.5/voip_utils.egg-info/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      366 2023-04-20 22:02:34.000000 voip-utils-0.0.5/voip_utils.egg-info/SOURCES.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-04-20 22:02:34.000000 voip-utils-0.0.5/voip_utils.egg-info/dependency_links.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       15 2023-04-20 22:02:34.000000 voip-utils-0.0.5/voip_utils.egg-info/requires.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       11 2023-04-20 22:02:34.000000 voip-utils-0.0.5/voip_utils.egg-info/top_level.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-04-06 18:58:14.000000 voip-utils-0.0.5/voip_utils.egg-info/zip-safe
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-05-01 15:26:07.727852 voip-utils-0.0.6/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11357 2022-11-22 20:23:02.000000 voip-utils-0.0.6/LICENSE.md
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      785 2023-05-01 15:26:07.727852 voip-utils-0.0.6/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       39 2023-04-06 16:12:50.000000 voip-utils-0.0.6/README.md
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1977 2023-05-01 15:25:43.000000 voip-utils-0.0.6/pyproject.toml
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      299 2023-05-01 15:26:07.727852 voip-utils-0.0.6/setup.cfg
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-05-01 15:26:07.723852 voip-utils-0.0.6/voip_utils/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      158 2023-04-06 17:22:11.000000 voip-utils-0.0.6/voip_utils/__init__.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      170 2023-04-06 15:51:26.000000 voip-utils-0.0.6/voip_utils/error.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7191 2023-04-23 03:37:26.000000 voip-utils-0.0.6/voip_utils/rtp_audio.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7603 2023-05-01 15:11:40.000000 voip-utils-0.0.6/voip_utils/sip.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      257 2023-04-06 18:58:36.000000 voip-utils-0.0.6/voip_utils/util.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     6284 2023-04-23 03:37:26.000000 voip-utils-0.0.6/voip_utils/voip.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-05-01 15:26:07.723852 voip-utils-0.0.6/voip_utils.egg-info/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      785 2023-05-01 15:26:07.000000 voip-utils-0.0.6/voip_utils.egg-info/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      366 2023-05-01 15:26:07.000000 voip-utils-0.0.6/voip_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-05-01 15:26:07.000000 voip-utils-0.0.6/voip_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       15 2023-05-01 15:26:07.000000 voip-utils-0.0.6/voip_utils.egg-info/requires.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       11 2023-05-01 15:26:07.000000 voip-utils-0.0.6/voip_utils.egg-info/top_level.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-04-06 18:58:14.000000 voip-utils-0.0.6/voip_utils.egg-info/zip-safe
```

### Comparing `voip-utils-0.0.5/LICENSE.md` & `voip-utils-0.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `voip-utils-0.0.5/PKG-INFO` & `voip-utils-0.0.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: voip-utils
-Version: 0.0.5
+Version: 0.0.6
 Summary: Voice over IP Utilities
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
-Project-URL: Source Code, https://github.com/home-assistant/intents
+Project-URL: Source Code, https://github.com/home-assistant-libs/voip-utils
 Keywords: home,assistant,voip,phone
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Communications :: Internet Phone
 Classifier: Topic :: Communications :: Telephony
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `voip-utils-0.0.5/pyproject.toml` & `voip-utils-0.0.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=62.3", "wheel~=0.37.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "voip-utils"
-version     = "0.0.5"
+version     = "0.0.6"
 license     = {text = "Apache-2.0"}
 description = "Voice over IP Utilities"
 readme      = "README.md"
 authors     = [
     {name = "The Home Assistant Authors", email = "hello@home-assistant.io"}
 ]
 keywords    = ["home", "assistant", "voip", "phone"]
@@ -21,15 +21,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 requires-python = ">=3.9.0"
 dependencies = ["opuslib==3.0.1"]
 
 [project.urls]
-"Source Code" = "https://github.com/home-assistant/intents"
+"Source Code" = "https://github.com/home-assistant-libs/voip-utils"
 
 [tool.setuptools]
 platforms = ["any"]
 zip-safe  = true
 include-package-data = true
 
 [tool.setuptools.packages.find]
```

### Comparing `voip-utils-0.0.5/voip_utils/rtp_audio.py` & `voip-utils-0.0.6/voip_utils/rtp_audio.py`

 * *Files identical despite different names*

### Comparing `voip-utils-0.0.5/voip_utils/sip.py` & `voip-utils-0.0.6/voip_utils/sip.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Implementation of SIP (Session Initiation Protocol)."""
 import asyncio
 import logging
+import re
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from typing import Dict, Optional, Tuple
 
 from .error import VoipError
 from .util import is_ipv4_address
 
@@ -39,29 +40,33 @@
 class SipDatagramProtocol(asyncio.DatagramProtocol, ABC):
     """UDP server for the Session Initiation Protocol (SIP)."""
 
     def __init__(self, sdp_info: SdpInfo) -> None:
         """Set up SIP server."""
         self.sdp_info = sdp_info
         self.transport = None
+        self._opus_payload = _OPUS_PAYLOAD
 
     def connection_made(self, transport):
         """Server ready."""
         self.transport = transport
 
     def datagram_received(self, data: bytes, addr):
         """Handle INVITE SIP messages."""
         try:
             message = data.decode()
-            method, headers, body = self._parse_sip(message)
+            method, ruri, headers, body = self._parse_sip(message)
 
             if method and (method.lower() != "invite"):
                 # Not an INVITE message
                 return
 
+            if not ruri:
+                raise ValueError("Empty receiver URI")
+
             caller_ip, caller_sip_port = addr
             _LOGGER.debug(
                 "Incoming call from ip=%s, port=%s",
                 caller_ip,
                 caller_sip_port,
             )
 
@@ -73,25 +78,50 @@
                 line = line.strip()
                 if line:
                     key, value = line.split("=", maxsplit=1)
                     if key == "m":
                         parts = value.split()
                         if parts[0] == "audio":
                             caller_rtp_port = int(parts[1])
+                    elif key == "a" and value.startswith("rtpmap:"):
+                        # a=rtpmap:123 opus/48000/2
+                        codec_str = value.split(":", maxsplit=1)[1]
+                        codec_parts = codec_str.split()
+                        if (len(codec_parts) > 1) and (
+                            codec_parts[1].lower().startswith("opus")
+                        ):
+                            self._opus_payload = codec_parts[0]
+                            _LOGGER.debug(
+                                "Detected OPUS payload type as %s", self._opus_payload
+                            )
 
             if caller_rtp_port is None:
                 raise VoipError("No caller RTP port")
 
-            # Extract our visible IP from SIP header.
-            # <sip:123.123.123.123:1234>;tag=...
-            sip_ip_str = headers["to"].partition(";")[0]
-            sip_ip_str = sip_ip_str[1:-1]
-            _sip, server_ip, _port = sip_ip_str.split(":", maxsplit=2)
+            # Extract host from ruri
+            # sip:user@123.123.123.123:1234
+            re_splituri = re.compile(
+                r"(?P<scheme>\w+):"  # Scheme
+                + r"(?:(?P<user>[\w\.]+):?(?P<password>[\w\.]+)?@)?"  # User:Password
+                + r"\[?(?P<host>"  # Begin group host
+                + r"(?:\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})|"  # IPv4 address Host Or
+                + r"(?:(?:[0-9a-fA-F]{1,4}):){7}[0-9a-fA-F]{1,4}|"  # IPv6 address Host Or
+                + r"(?:(?:[0-9A-Za-z]+\.)+[0-9A-Za-z]+)"  # Hostname string
+                + r")\]?:?"  # End group host
+                + r"(?P<port>\d{1,6})?"  # port
+                + r"(?:\;(?P<params>[^\?]*))?"  # parameters
+                + r"(?:\?(?P<headers>.*))?"  # headers
+            )
+            re_uri = re_splituri.search(ruri)
+            if re_uri is None:
+                raise ValueError("Receiver URI did not match expected pattern")
+
+            server_ip = re_uri.group("host")
             if not is_ipv4_address(server_ip):
-                raise VoipError(f"Invalid IPv4 address in {sip_ip_str}")
+                raise VoipError(f"Invalid IPv4 address in {ruri}")
 
             self.on_call(
                 CallInfo(
                     caller_ip=caller_ip,
                     caller_sip_port=caller_sip_port,
                     caller_rtp_port=caller_rtp_port,
                     server_ip=server_ip,
@@ -118,15 +148,15 @@
         # See: https://datatracker.ietf.org/doc/html/rfc2327
         body_lines = [
             "v=0",
             f"o={self.sdp_info.username} {self.sdp_info.id} 1 IN IP4 {call_info.server_ip}",
             f"s={self.sdp_info.session_name}",
             f"c=IN IP4 {call_info.server_ip}",
             "t=0 0",
-            f"m=audio {server_rtp_port} RTP/AVP {_OPUS_PAYLOAD}",
+            f"m=audio {server_rtp_port} RTP/AVP {self._opus_payload}",
             f"a=rtpmap:{_OPUS_PAYLOAD} opus/48000/2",
             "a=ptime:20",
             "a=maxptime:150",
             "a=sendrecv",
             _CRLF,
         ]
         body = _CRLF.join(body_lines)
@@ -159,31 +189,36 @@
         _LOGGER.debug(
             "Sent OK to ip=%s, port=%s with rtp_port=%s",
             call_info.caller_ip,
             call_info.caller_sip_port,
             server_rtp_port,
         )
 
-    def _parse_sip(self, message: str) -> Tuple[Optional[str], Dict[str, str], str]:
+    def _parse_sip(
+        self, message: str
+    ) -> Tuple[Optional[str], Optional[str], Dict[str, str], str]:
         """Parse SIP message and return method, headers, and body."""
         lines = message.splitlines()
 
         method: Optional[str] = None
+        ruri: Optional[str] = None
         headers: dict[str, str] = {}
         offset: int = 0
 
         # See: https://datatracker.ietf.org/doc/html/rfc3261
         for i, line in enumerate(lines):
             if line:
                 offset += len(line) + len(_CRLF)
 
             if i == 0:
-                method = line.split()[0]
+                line_parts = line.split()
+                method = line_parts[0]
+                ruri = line_parts[1]
             elif not line:
                 break
             else:
                 key, value = line.split(":", maxsplit=1)
                 headers[key.lower()] = value.strip()
 
         body = message[offset:]
 
-        return method, headers, body
+        return method, ruri, headers, body
```

### Comparing `voip-utils-0.0.5/voip_utils/voip.py` & `voip-utils-0.0.6/voip_utils/voip.py`

 * *Files identical despite different names*

### Comparing `voip-utils-0.0.5/voip_utils.egg-info/PKG-INFO` & `voip-utils-0.0.6/voip_utils.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: voip-utils
-Version: 0.0.5
+Version: 0.0.6
 Summary: Voice over IP Utilities
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
-Project-URL: Source Code, https://github.com/home-assistant/intents
+Project-URL: Source Code, https://github.com/home-assistant-libs/voip-utils
 Keywords: home,assistant,voip,phone
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Communications :: Internet Phone
 Classifier: Topic :: Communications :: Telephony
 Classifier: License :: OSI Approved :: Apache Software License
```

