# Comparing `tmp/desktop-notifier-3.4.3.tar.gz` & `tmp/desktop-notifier-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "desktop-notifier-3.4.3.tar", last modified: Wed Feb  1 20:32:18 2023, max compression
+gzip compressed data, was "desktop-notifier-3.5.0.tar", last modified: Mon May  1 18:29:37 2023, max compression
```

## Comparing `desktop-notifier-3.4.3.tar` & `desktop-notifier-3.5.0.tar`

### file list

```diff
@@ -1,28 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 20:32:18.046089 desktop-notifier-3.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-02-01 20:32:05.000000 desktop-notifier-3.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-02-01 20:32:18.046089 desktop-notifier-3.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-02-01 20:32:05.000000 desktop-notifier-3.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-02-01 20:32:05.000000 desktop-notifier-3.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-02-01 20:32:18.046089 desktop-notifier-3.4.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 20:32:18.046089 desktop-notifier-3.4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 20:32:18.046089 desktop-notifier-3.4.3/src/desktop_notifier/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-02-01 20:32:05.000000 desktop-notifier-3.4.3/src/desktop_notifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10789 2023-02-01 20:32:05.000000 desktop-notifier-3.4.3/src/desktop_notifier/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-02-01 20:32:05.000000 desktop-notifier-3.4.3/src/desktop_notifier/dbus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-02-01 20:32:05.000000 desktop-notifier-3.4.3/src/desktop_notifier/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)    14787 2023-02-01 20:32:05.000000 desktop-notifier-3.4.3/src/desktop_notifier/macos.py
--rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-02-01 20:32:05.000000 desktop-notifier-3.4.3/src/desktop_notifier/macos_legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-02-01 20:32:05.000000 desktop-notifier-3.4.3/src/desktop_notifier/macos_support.py
--rw-r--r--   0 runner    (1001) docker     (123)    13292 2023-02-01 20:32:05.000000 desktop-notifier-3.4.3/src/desktop_notifier/main.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 20:32:05.000000 desktop-notifier-3.4.3/src/desktop_notifier/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 20:32:18.046089 desktop-notifier-3.4.3/src/desktop_notifier/resources/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-01 20:32:05.000000 desktop-notifier-3.4.3/src/desktop_notifier/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-02-01 20:32:05.000000 desktop-notifier-3.4.3/src/desktop_notifier/resources/python.png
--rw-r--r--   0 runner    (1001) docker     (123)    10541 2023-02-01 20:32:05.000000 desktop-notifier-3.4.3/src/desktop_notifier/winrt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 20:32:18.046089 desktop-notifier-3.4.3/src/desktop_notifier.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-02-01 20:32:18.000000 desktop-notifier-3.4.3/src/desktop_notifier.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-02-01 20:32:18.000000 desktop-notifier-3.4.3/src/desktop_notifier.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 20:32:18.000000 desktop-notifier-3.4.3/src/desktop_notifier.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 20:32:18.000000 desktop-notifier-3.4.3/src/desktop_notifier.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-02-01 20:32:18.000000 desktop-notifier-3.4.3/src/desktop_notifier.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-01 20:32:18.000000 desktop-notifier-3.4.3/src/desktop_notifier.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:29:37.212569 desktop-notifier-3.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-01 18:29:19.000000 desktop-notifier-3.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-05-01 18:29:37.212569 desktop-notifier-3.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7383 2023-05-01 18:29:19.000000 desktop-notifier-3.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-01 18:29:19.000000 desktop-notifier-3.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 18:29:37.212569 desktop-notifier-3.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:29:37.208568 desktop-notifier-3.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:29:37.212569 desktop-notifier-3.5.0/src/desktop_notifier/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-01 18:29:19.000000 desktop-notifier-3.5.0/src/desktop_notifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10614 2023-05-01 18:29:19.000000 desktop-notifier-3.5.0/src/desktop_notifier/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-05-01 18:29:19.000000 desktop-notifier-3.5.0/src/desktop_notifier/dbus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-01 18:29:19.000000 desktop-notifier-3.5.0/src/desktop_notifier/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14980 2023-05-01 18:29:19.000000 desktop-notifier-3.5.0/src/desktop_notifier/macos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-05-01 18:29:19.000000 desktop-notifier-3.5.0/src/desktop_notifier/macos_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-01 18:29:19.000000 desktop-notifier-3.5.0/src/desktop_notifier/macos_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12931 2023-05-01 18:29:19.000000 desktop-notifier-3.5.0/src/desktop_notifier/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:29:37.212569 desktop-notifier-3.5.0/src/desktop_notifier/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-01 18:29:19.000000 desktop-notifier-3.5.0/src/desktop_notifier/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9356 2023-05-01 18:29:19.000000 desktop-notifier-3.5.0/src/desktop_notifier/winrt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:29:37.212569 desktop-notifier-3.5.0/src/desktop_notifier.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-05-01 18:29:37.000000 desktop-notifier-3.5.0/src/desktop_notifier.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-01 18:29:37.000000 desktop-notifier-3.5.0/src/desktop_notifier.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 18:29:37.000000 desktop-notifier-3.5.0/src/desktop_notifier.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-01 18:29:37.000000 desktop-notifier-3.5.0/src/desktop_notifier.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 18:29:37.000000 desktop-notifier-3.5.0/src/desktop_notifier.egg-info/top_level.txt
```

### Comparing `desktop-notifier-3.4.3/LICENSE` & `desktop-notifier-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `desktop-notifier-3.4.3/PKG-INFO` & `desktop-notifier-3.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: desktop-notifier
-Version: 3.4.3
+Version: 3.5.0
 Summary: Python library for cross-platform desktop notifications
-Home-page: https://github.com/samschott/desktop-notifier
-Author: Sam Schott
-Author-email: sam.schott@outlook.com
+Author-email: Sam Schott <sam.schott@outlook.com>
 License: MIT
+Project-URL: Homepage, https://github.com/samschott/desktop-notifier
 Keywords: desktop-notifier
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -37,25 +36,38 @@
 * macOS and iOS via the Notification Center framework
 * [**exprimental**] Windows via the WinRT / Python bridge.
 
 ![gif](screenshots/macOS.gif)
 
 ## Features
 
-Where supported by the native platform APIs:
+`desktop-notifier` aims to be a good citizen of the platforms which it supports. It
+therefore stays within the limits of the native platform APIs and does not try to
+work around limitations which are often deliberate UI choices. For example, on macOS
+and iOS, it is not possible to change the app icon which is shown on notifications.
+There are possible workarounds - that would likely be rejected by an App Store review.
 
-* Clickable notifications
+Where supported by the native platform APIs, `desktop-notifier` allows for:
+
+* Clickable notifications with callbacks on user interaction
 * Multiple action buttons
 * A single reply field (e.g., for chat notifications)
-* Asyncio integration: the main API consists of async methods and a running event loop
-  is required to respond to user interactions with a notification
 * Notification sounds
-* Notification threads (e.g., for different conversations)
-* Limit maximum number of notifications shown in the notification center
-* Pure Python dependencies only, no extension modules
+* Notification threads (grouping notifications by topic)
+* Limiting maximum number of notifications shown in the notification center
+
+An exhaustive list of features and their platform support is provided in the
+[documentation](https://desktop-notifier.readthedocs.io/en/latest/background/platform_support.html).
+
+Design choices by `desktop-notifier`:
+
+* Asyncio API: The main API consists of async methods and a running event loop
+  is required to respond to user interactions with a notification.
+* Pure Python dependencies only, no extension modules (with the exception of
+  of the Windows backend).
 
 ## Installation
 
 From PyPI:
 
 ```
 pip3 install -U desktop-notifier
```

### Comparing `desktop-notifier-3.4.3/README.md` & `desktop-notifier-3.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -11,25 +11,38 @@
 * macOS and iOS via the Notification Center framework
 * [**exprimental**] Windows via the WinRT / Python bridge.
 
 ![gif](screenshots/macOS.gif)
 
 ## Features
 
-Where supported by the native platform APIs:
+`desktop-notifier` aims to be a good citizen of the platforms which it supports. It
+therefore stays within the limits of the native platform APIs and does not try to
+work around limitations which are often deliberate UI choices. For example, on macOS
+and iOS, it is not possible to change the app icon which is shown on notifications.
+There are possible workarounds - that would likely be rejected by an App Store review.
 
-* Clickable notifications
+Where supported by the native platform APIs, `desktop-notifier` allows for:
+
+* Clickable notifications with callbacks on user interaction
 * Multiple action buttons
 * A single reply field (e.g., for chat notifications)
-* Asyncio integration: the main API consists of async methods and a running event loop
-  is required to respond to user interactions with a notification
 * Notification sounds
-* Notification threads (e.g., for different conversations)
-* Limit maximum number of notifications shown in the notification center
-* Pure Python dependencies only, no extension modules
+* Notification threads (grouping notifications by topic)
+* Limiting maximum number of notifications shown in the notification center
+
+An exhaustive list of features and their platform support is provided in the
+[documentation](https://desktop-notifier.readthedocs.io/en/latest/background/platform_support.html).
+
+Design choices by `desktop-notifier`:
+
+* Asyncio API: The main API consists of async methods and a running event loop
+  is required to respond to user interactions with a notification.
+* Pure Python dependencies only, no extension modules (with the exception of
+  of the Windows backend).
 
 ## Installation
 
 From PyPI:
 
 ```
 pip3 install -U desktop-notifier
```

### Comparing `desktop-notifier-3.4.3/src/desktop_notifier/base.py` & `desktop-notifier-3.5.0/src/desktop_notifier/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 # -*- coding: utf-8 -*-
 """
 This module defines base classes for desktop notifications. All platform implementations
 must inherit from :class:`DesktopNotifierBase`.
 """
 
+from __future__ import annotations
+
 # system imports
 import logging
 import pathlib
 from enum import Enum
 from collections import deque
 from typing import (
-    Optional,
     Dict,
     Callable,
     Any,
-    Union,
     Deque,
     List,
     Sequence,
     ContextManager,
 )
 
 try:
-    from importlib.resources import as_file, files  # type:ignore
+    from importlib.resources import as_file, files
 
     def resource_path(package: str, resource: str) -> ContextManager[pathlib.Path]:
         return as_file(files(package) / resource)
 
 except ImportError:
-    from importlib.resources import path as resource_path  # type:ignore
+    from importlib.resources import path as resource_path
 
 
 logger = logging.getLogger(__name__)
 
 PYTHON_ICON_PATH = resource_path("desktop_notifier.resources", "python.png").__enter__()
 
 
@@ -62,20 +62,22 @@
 
     :param title: The button title.
     :param on_pressed: Callback to invoke when the button is pressed. This is called
         without any arguments.
     """
 
     def __init__(
-        self, title: str, on_pressed: Optional[Callable[[], Any]] = None
+        self,
+        title: str,
+        on_pressed: Callable[[], Any] | None = None,
     ) -> None:
         self.title = title
         self.on_pressed = on_pressed
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"<{self.__class__.__name__}(title='{self.title}', on_pressed={self.on_pressed})>"
 
 
 class ReplyField:
     """
     A reply field for interactive notifications
 
@@ -86,21 +88,21 @@
         without any arguments.
     """
 
     def __init__(
         self,
         title: str = "Reply",
         button_title: str = "Send",
-        on_replied: Optional[Callable[[str], Any]] = None,
+        on_replied: Callable[[str], Any] | None = None,
     ) -> None:
         self.title = title
         self.button_title = button_title
         self.on_replied = on_replied
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"<{self.__class__.__name__}(title='{self.title}', on_replied={self.on_replied})>"
 
 
 class Notification:
     """A desktop notification
 
     :param title: Notification title.
@@ -120,76 +122,72 @@
     """
 
     def __init__(
         self,
         title: str,
         message: str,
         urgency: Urgency = Urgency.Normal,
-        icon: Optional[str] = None,
+        icon: str | None = None,
         buttons: Sequence[Button] = (),
-        reply_field: Optional[ReplyField] = None,
-        on_clicked: Optional[Callable[[], Any]] = None,
-        on_dismissed: Optional[Callable[[], Any]] = None,
-        attachment: Optional[str] = None,
+        reply_field: ReplyField | None = None,
+        on_clicked: Callable[[], Any] | None = None,
+        on_dismissed: Callable[[], Any] | None = None,
+        attachment: str | None = None,
         sound: bool = False,
-        thread: Optional[str] = None,
+        thread: str | None = None,
         timeout: int = -1,
     ) -> None:
-
-        self._identifier: Union[str, int, None] = None
+        self._identifier: str | int | None = None
         self.title = title
         self.message = message
         self.urgency = urgency
         self.icon = icon
         self.buttons = buttons
         self.reply_field = reply_field
         self.on_clicked = on_clicked
         self.on_dismissed = on_dismissed
         self.attachment = attachment
         self.sound = sound
         self.thread = thread
         self.timeout = timeout
 
     @property
-    def identifier(self) -> Union[str, int, None]:
+    def identifier(self) -> str | int | None:
         """
         An platform identifier which gets assigned to the notification after it was
         sent. This may be a str or int.
         """
         return self._identifier
 
     @identifier.setter
-    def identifier(self, value: Union[str, int, None]) -> None:
+    def identifier(self, value: str | int | None) -> None:
         """Setter: identifier"""
         self._identifier = value
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"<{self.__class__.__name__}(title='{self.title}', message='{self.message}')>"
 
 
 class DesktopNotifierBase:
     """Base class for desktop notifier implementations
 
     :param app_name: Name to identify the application in the notification center.
-    :param app_icon: Default icon to use for notifications.
     :param notification_limit: Maximum number of notifications to keep in the system's
         notification center.
     """
 
     def __init__(
         self,
         app_name: str = "Python",
-        app_icon: Optional[str] = None,
-        notification_limit: Optional[int] = None,
+        notification_limit: int | None = None,
     ) -> None:
         self.app_name = app_name
-        self.app_icon = app_icon
         self.notification_limit = notification_limit
         self._current_notifications: Deque[Notification] = deque([], notification_limit)
-        self._notification_for_nid: Dict[Union[str, int], Notification] = {}
+        self._notification_for_nid: Dict[str | int, Notification] = {}
 
     async def request_authorisation(self) -> bool:
         """
         Request authorisation to send notifications.
 
         :returns: Whether authorisation has been granted.
         """
@@ -207,15 +205,15 @@
         implementation. This is a wrapper method which mostly performs housekeeping of
         notifications ID and calls :meth:`_send` to actually schedule the notification.
         Platform implementations must implement :meth:`_send`.
 
         :param notification: Notification to send.
         """
 
-        notification_to_replace: Optional[Notification]
+        notification_to_replace: Notification | None
 
         if len(self._current_notifications) == self.notification_limit:
             notification_to_replace = self._current_notifications.popleft()
         else:
             notification_to_replace = None
 
         try:
@@ -248,16 +246,16 @@
                 self._notification_for_nid.pop(notification.identifier)
             except KeyError:
                 pass
 
     async def _send(
         self,
         notification: Notification,
-        notification_to_replace: Optional[Notification],
-    ) -> Union[str, int]:
+        notification_to_replace: Notification | None,
+    ) -> str | int:
         """
         Method to send a notification via the platform. This should be implemented by
         subclasses.
 
         Implementations must raise an exception when the notification could not be
         delivered. If the notification could be delivered but not fully as intended,
         e.g., because associated resources could not be loaded, implementations should
```

### Comparing `desktop-notifier-3.4.3/src/desktop_notifier/dbus.py` & `desktop-notifier-3.5.0/src/desktop_notifier/dbus.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # -*- coding: utf-8 -*-
 """
 Notification backend for Linux. Includes an implementation to send desktop notifications
 over Dbus. Responding to user interaction with a notification requires a running asyncio
 event loop.
 """
 
+from __future__ import annotations
+
 # system imports
 import logging
-from typing import Optional, TypeVar
+from typing import TypeVar, cast
 
 # external imports
 from dbus_next import Variant
 from dbus_next.aio import MessageBus, ProxyInterface
 
 # local imports
 from .base import Notification, DesktopNotifierBase, Urgency
@@ -49,19 +51,18 @@
         Urgency.Normal: Variant("y", 1),
         Urgency.Critical: Variant("y", 2),
     }
 
     def __init__(
         self,
         app_name: str = "Python",
-        app_icon: Optional[str] = None,
-        notification_limit: Optional[int] = None,
+        notification_limit: int | None = None,
     ) -> None:
-        super().__init__(app_name, app_icon, notification_limit)
-        self.interface: Optional[ProxyInterface] = None
+        super().__init__(app_name, notification_limit)
+        self.interface: ProxyInterface | None = None
 
     async def request_authorisation(self) -> bool:
         """
         Request authorisation to send notifications.
 
         :returns: Whether authorisation has been granted.
         """
@@ -70,15 +71,14 @@
     async def has_authorisation(self) -> bool:
         """
         Whether we have authorisation to send notifications.
         """
         return True
 
     async def _init_dbus(self) -> ProxyInterface:
-
         self.bus = await MessageBus().connect()
         introspection = await self.bus.introspect(
             "org.freedesktop.Notifications", "/org/freedesktop/Notifications"
         )
         self.proxy_object = self.bus.get_proxy_object(
             "org.freedesktop.Notifications",
             "/org/freedesktop/Notifications",
@@ -87,25 +87,25 @@
         self.interface = self.proxy_object.get_interface(
             "org.freedesktop.Notifications"
         )
 
         # Some older interfaces may not support notification actions.
 
         if hasattr(self.interface, "on_notification_closed"):
-            self.interface.on_notification_closed(self._on_closed)  # type: ignore
+            self.interface.on_notification_closed(self._on_closed)
 
         if hasattr(self.interface, "on_action_invoked"):
-            self.interface.on_action_invoked(self._on_action)  # type: ignore
+            self.interface.on_action_invoked(self._on_action)
 
         return self.interface
 
     async def _send(
         self,
         notification: Notification,
-        notification_to_replace: Optional[Notification],
+        notification_to_replace: Notification | None,
     ) -> int:
         """
         Asynchronously sends a notification via the Dbus interface.
 
         :param notification: Notification to send.
         :param notification_to_replace: Notification to replace, if any.
         """
@@ -133,47 +133,47 @@
         if notification.attachment:
             hints["image-path"] = Variant("s", notification.attachment)
 
         # get the timeout in ms
         timeout = notification.timeout * 1000 if notification.timeout != -1 else -1
 
         # Post the new notification and record the platform ID assigned to it.
-        platform_nid = await self.interface.call_notify(  # type: ignore
+        platform_nid = await self.interface.call_notify(
             self.app_name,  # app_name
             replaces_nid,  # replaces_id
             notification.icon or "",  # app_icon
             notification.title,  # summary
             notification.message,  # body
             actions,  # actions
             hints,  # hints
             timeout,  # expire_timeout (-1 = default)
         )
 
-        return platform_nid
+        return cast(int, platform_nid)
 
     async def _clear(self, notification: Notification) -> None:
         """
         Asynchronously removes a notification from the notification center
         """
 
         if not self.interface:
             return
 
-        await self.interface.call_close_notification(notification.identifier)  # type: ignore
+        await self.interface.call_close_notification(notification.identifier)
 
     async def _clear_all(self) -> None:
         """
         Asynchronously clears all notifications from notification center
         """
 
         if not self.interface:
             return
 
         for notification in self.current_notifications:
-            await self.interface.call_close_notification(notification.identifier)  # type: ignore
+            await self.interface.call_close_notification(notification.identifier)
 
     # Note that _on_action and _on_closed might be called for the same notification
     # with some notification servers. This is not a problem because the _on_action
     # call will come first, in which case we are no longer interested in calling the
     # on_dismissed callback.
 
     def _on_action(self, nid: int, action_key: str) -> None:
@@ -189,26 +189,25 @@
         # Get the notification instance from the platform ID.
         notification = self._notification_for_nid.get(nid)
 
         # Execute any callbacks for button clicks.
         if notification:
             self._clear_notification_from_cache(notification)
 
-            button_number: Optional[int]
+            button_number: int | None
 
             try:
                 button_number = int(action_key)
             except ValueError:
                 button_number = None
 
             if action_key == "default" and notification.on_clicked:
                 notification.on_clicked()
 
             elif button_number is not None:
-
                 button = notification.buttons[button_number]
 
                 if button.on_pressed:
                     button.on_pressed()
 
     def _on_closed(self, nid: int, reason: int) -> None:
         """
```

### Comparing `desktop-notifier-3.4.3/src/desktop_notifier/dummy.py` & `desktop-notifier-3.5.0/src/desktop_notifier/dummy.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # -*- coding: utf-8 -*-
 """
 Dummy backend for unsupported platforms.
 """
 
+from __future__ import annotations
+
 # system imports
 import uuid
-from typing import Optional
 
 # local imports
 from .base import Notification, DesktopNotifierBase
 
 
 class DummyNotificationCenter(DesktopNotifierBase):
     """A dummy backend for unsupported platforms"""
 
     def __init__(
         self,
         app_name: str = "Python",
-        app_icon: Optional[str] = None,
-        notification_limit: Optional[int] = None,
+        notification_limit: int | None = None,
     ) -> None:
-        super().__init__(app_name, app_icon, notification_limit)
+        super().__init__(app_name, notification_limit)
 
     async def request_authorisation(self) -> bool:
         """
         Request authorisation to send notifications.
 
         :returns: Whether authorisation has been granted.
         """
@@ -35,15 +35,15 @@
         Whether we have authorisation to send notifications.
         """
         return True
 
     async def _send(
         self,
         notification: Notification,
-        notification_to_replace: Optional[Notification],
+        notification_to_replace: Notification | None,
     ) -> str:
         if notification_to_replace:
             return str(notification_to_replace.identifier)
         else:
             return str(uuid.uuid4())
 
     async def _clear(self, notification: Notification) -> None:
```

### Comparing `desktop-notifier-3.4.3/src/desktop_notifier/macos.py` & `desktop-notifier-3.5.0/src/desktop_notifier/macos.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,27 +6,29 @@
 * Cross-platform with iOS and iPadOS.
 * Only available from signed app bundles if called from the main executable or from a
   signed Python framework (for example from python.org).
 * Requires a running CFRunLoop to invoke callbacks.
 
 """
 
+from __future__ import annotations
+
 # system imports
 import uuid
 import logging
 import enum
 import asyncio
 from concurrent.futures import Future
 from urllib.parse import urlparse, unquote
-from typing import Optional, cast
+from typing import cast
 
 # external imports
 from packaging.version import Version
-from rubicon.objc import NSObject, ObjCClass, objc_method, py_from_ns  # type: ignore
-from rubicon.objc.runtime import load_library, objc_id, objc_block  # type: ignore
+from rubicon.objc import NSObject, ObjCClass, objc_method, py_from_ns
+from rubicon.objc.runtime import load_library, objc_id, objc_block
 
 # local imports
 from .base import Notification, DesktopNotifierBase, AuthorisationError, Urgency
 from .macos_support import macos_version
 
 
 __all__ = ["CocoaNotificationCenter"]
@@ -40,17 +42,19 @@
 UNMutableNotificationContent = ObjCClass("UNMutableNotificationContent")
 UNNotificationRequest = ObjCClass("UNNotificationRequest")
 UNNotificationAction = ObjCClass("UNNotificationAction")
 UNTextInputNotificationAction = ObjCClass("UNTextInputNotificationAction")
 UNNotificationCategory = ObjCClass("UNNotificationCategory")
 UNNotificationSound = ObjCClass("UNNotificationSound")
 UNNotificationAttachment = ObjCClass("UNNotificationAttachment")
+UNNotificationSettings = ObjCClass("UNNotificationSettings")
 
 NSURL = ObjCClass("NSURL")
 NSSet = ObjCClass("NSSet")
+NSError = ObjCClass("NSError")
 
 # UserNotifications.h
 
 UNNotificationDefaultActionIdentifier = (
     "com.apple.UNNotificationDefaultActionIdentifier"
 )
 UNNotificationDismissActionIdentifier = (
@@ -94,45 +98,40 @@
     TimeSensitive = 2
     Critical = 3
 
 
 class NotificationCenterDelegate(NSObject):  # type: ignore
     """Delegate to handle user interactions with notifications"""
 
-    @objc_method
+    @objc_method  # type:ignore
     def userNotificationCenter_didReceiveNotificationResponse_withCompletionHandler_(
         self, center, response, completion_handler: objc_block
     ) -> None:
-
         # Get the notification which was clicked from the platform ID.
         platform_nid = py_from_ns(response.notification.request.identifier)
         py_notification = self.interface._notification_for_nid[platform_nid]
         py_notification = cast(Notification, py_notification)
 
         self.interface._clear_notification_from_cache(py_notification)
 
         # Invoke the callback which corresponds to the user interaction.
         if response.actionIdentifier == UNNotificationDefaultActionIdentifier:
-
             if py_notification.on_clicked:
                 py_notification.on_clicked()
 
         elif response.actionIdentifier == UNNotificationDismissActionIdentifier:
-
             if py_notification.on_dismissed:
                 py_notification.on_dismissed()
 
         elif response.actionIdentifier == ReplyActionIdentifier:
-
             if py_notification.reply_field.on_replied:
                 reply_text = py_from_ns(response.userText)
                 py_notification.reply_field.on_replied(reply_text)
 
         else:
-
             button_number = int(py_from_ns(response.actionIdentifier))
             callback = py_notification.buttons[button_number].on_pressed
 
             if callback:
                 callback()
 
         completion_handler()
@@ -143,33 +142,30 @@
 
     Can be used with macOS Catalina and newer. Both app name and bundle identifier
     will be ignored. The notification center automatically uses the values provided
     by the app bundle.
 
     :param app_name: The name of the app. Does not have any effect because the app
         name is automatically determined from the bundle or framework.
-    :param app_icon: The icon of the app. Does not have any effect because the app
-        icon is automatically determined from the bundle or framework.
     :param notification_limit: Maximum number of notifications to keep in the system's
         notification center.
     """
 
     _to_native_urgency = {
         Urgency.Low: UNNotificationInterruptionLevel.Passive,
         Urgency.Normal: UNNotificationInterruptionLevel.Active,
         Urgency.Critical: UNNotificationInterruptionLevel.TimeSensitive,
     }
 
     def __init__(
         self,
         app_name: str = "Python",
-        app_icon: Optional[str] = None,
-        notification_limit: Optional[int] = None,
+        notification_limit: int | None = None,
     ) -> None:
-        super().__init__(app_name, app_icon, notification_limit)
+        super().__init__(app_name, notification_limit)
         self.nc = UNUserNotificationCenter.currentNotificationCenter()
         self.nc_delegate = NotificationCenterDelegate.alloc().init()
         self.nc_delegate.interface = self
         self.nc.delegate = self.nc_delegate
 
         self._clear_notification_categories()
 
@@ -179,15 +175,15 @@
         first time for an app, the call will only return once the user has granted or
         denied the request. Otherwise, the call will just return the current
         authorisation status without prompting the user.
 
         :returns: Whether authorisation has been granted.
         """
 
-        future: Future = Future()
+        future: Future[tuple[bool, str]] = Future()
 
         def on_auth_completed(granted: bool, error: objc_id) -> None:
             ns_error = py_from_ns(error)
             error_str = str(ns_error.localizedDescription) if ns_error else ""
             future.set_result((granted, error_str))
 
         self.nc.requestAuthorizationWithOptions(
@@ -205,39 +201,39 @@
         return granted
 
     async def has_authorisation(self) -> bool:
         """Whether we have authorisation to send notifications."""
 
         # Get existing notification categories.
 
-        future: Future = Future()
+        future: Future[UNNotificationSettings] = Future()  # type:ignore
 
         def handler(settings: objc_id) -> None:
             settings = py_from_ns(settings)
             settings.retain()
             future.set_result(settings)
 
         self.nc.getNotificationSettingsWithCompletionHandler(handler)
 
         settings = await asyncio.wrap_future(future)
 
-        authorized = settings.authorizationStatus in (
+        authorized = settings.authorizationStatus in (  # type:ignore
             UNAuthorizationStatusAuthorized,
             UNAuthorizationStatusProvisional,
             UNAuthorizationStatusEphemeral,
         )
 
-        settings.release()
+        settings.release()  # type:ignore
 
         return authorized
 
     async def _send(
         self,
         notification: Notification,
-        notification_to_replace: Optional[Notification],
+        notification_to_replace: Notification | None,
     ) -> str:
         """
         Uses UNUserNotificationCenter to schedule a notification.
 
         :param notification: Notification to send.
         :param notification_to_replace: Notification to replace, if any.
         """
@@ -271,56 +267,58 @@
             )
             content.attachments = [attachment]
 
         notification_request = UNNotificationRequest.requestWithIdentifier(
             platform_nid, content=content, trigger=None
         )
 
-        future: Future = Future()
+        future: Future[NSError] = Future()  # type:ignore
 
         def handler(error: objc_id) -> None:
             ns_error = py_from_ns(error)
             if ns_error:
                 ns_error.retain()
             future.set_result(ns_error)
 
         # Post the notification.
         self.nc.addNotificationRequest(
             notification_request, withCompletionHandler=handler
         )
 
         # Error handling.
-
         error = await asyncio.wrap_future(future)
 
         if error:
-            error.autorelease()
+            error.autorelease()  # type:ignore
 
-            if error.domain == UNErrorDomain:
-                if error.code == UNErrorCode.NotificationsNotAllowed:
+            if error.domain == UNErrorDomain:  # type:ignore
+                if error.code == UNErrorCode.NotificationsNotAllowed:  # type:ignore
                     raise AuthorisationError("Not authorised")
-                elif error.code == UNErrorCode.NotificationInvalidNoDate:
+                elif error.code == UNErrorCode.NotificationInvalidNoDate:  # type:ignore
                     raise RuntimeError("Missing notification date")
-                elif error.code == UNErrorCode.NotificationInvalidNoContent:
+                elif (
+                    error.code  # type:ignore
+                    == UNErrorCode.NotificationInvalidNoContent
+                ):
                     raise RuntimeError("Missing notification content")
                 else:
                     # In case of attachment errors, the notification will still be
                     # delivered, just without an attachment. We therefore do not raise
                     # the error.
                     logger.warning(
-                        f"{error.localizedDescription}: {notification.attachment}"
+                        f"{error.localizedDescription}: {notification.attachment}"  # type:ignore
                     )
             else:
-                raise RuntimeError(error.localizedDescription)
+                raise RuntimeError(error.localizedDescription)  # type:ignore
 
         return platform_nid
 
     async def _create_category_for_notification(
         self, notification: Notification
-    ) -> Optional[str]:
+    ) -> str | None:
         """
         Registers a new notification category with UNNotificationCenter for the given
         notification or retrieves an existing one if it exists for our set of buttons.
 
         :param notification: Notification instance.
         :returns: The identifier of the existing or created notification category.
         """
@@ -336,15 +334,14 @@
         # modified by other Python processes using desktop-notifier.
 
         categories = await self._get_notification_categories()
         category_ids = set(py_from_ns(c.identifier) for c in categories.allObjects())  # type: ignore
 
         # Register new category if necessary.
         if category_id not in category_ids:
-
             # Create action for each button.
             actions = []
 
             if notification.reply_field:
                 action = UNTextInputNotificationAction.actionWithIdentifier(
                     ReplyActionIdentifier,
                     title=notification.reply_field.title,
@@ -370,28 +367,28 @@
                     options=UNNotificationCategoryOptionNone,
                 )
             )
             self.nc.setNotificationCategories(new_categories)
 
         return category_id
 
-    async def _get_notification_categories(self) -> NSSet:  # type: ignore
+    async def _get_notification_categories(self) -> NSSet:  # type:ignore
         """Returns the registered notification categories for this app / Python."""
 
-        future: Future = Future()
+        future: Future[NSSet] = Future()  # type:ignore
 
         def handler(categories: objc_id) -> None:
             categories = py_from_ns(categories)
             categories.retain()
             future.set_result(categories)
 
         self.nc.getNotificationCategoriesWithCompletionHandler(handler)
 
         categories = await asyncio.wrap_future(future)
-        categories.autorelease()
+        categories.autorelease()  # type:ignore
 
         return categories
 
     def _clear_notification_categories(self) -> None:
         """Clears all registered notification categories for this application."""
         empty_set = NSSet.alloc().init()
         self.nc.setNotificationCategories(empty_set)
```

### Comparing `desktop-notifier-3.4.3/src/desktop_notifier/macos_legacy.py` & `desktop-notifier-3.5.0/src/desktop_notifier/macos_legacy.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,23 +4,25 @@
 
 * Should be used for macOS 10.13 and earlier.
 * Deprecated but still available in macOS 11.0.
 * Requires a running CFRunLoop to invoke callbacks.
 
 """
 
+from __future__ import annotations
+
 # system imports
 import uuid
 import platform
 import logging
-from typing import Optional, cast
+from typing import cast
 
 # external imports
-from rubicon.objc import NSObject, ObjCClass, objc_method, py_from_ns  # type: ignore
-from rubicon.objc.runtime import load_library  # type: ignore
+from rubicon.objc import NSObject, ObjCClass, objc_method, py_from_ns
+from rubicon.objc.runtime import load_library
 
 # local imports
 from .base import Notification, DesktopNotifierBase
 
 
 __all__ = ["CocoaNotificationCenterLegacy"]
 
@@ -39,38 +41,35 @@
 
 NSUserNotificationDefaultSoundName = "DefaultSoundName"
 
 
 class NotificationCenterDelegate(NSObject):  # type: ignore
     """Delegate to handle user interactions with notifications"""
 
-    @objc_method
+    @objc_method  # type:ignore
     def userNotificationCenter_didActivateNotification_(
         self, center, notification
     ) -> None:
-
         platform_nid = py_from_ns(notification.identifier)
         py_notification = self.interface._notification_for_nid[platform_nid]
         py_notification = cast(Notification, py_notification)
 
         self.interface._clear_notification_from_cache(py_notification)
 
         if (
             notification.activationType
             == NSUserNotificationActivationTypeContentsClicked
         ):
-
             if py_notification.on_clicked:
                 py_notification.on_clicked()
 
         elif (
             notification.activationType
             == NSUserNotificationActivationTypeActionButtonClicked
         ):
-
             callback = py_notification.buttons[0].on_pressed
 
             if callback:
                 callback()
 
 
 class CocoaNotificationCenterLegacy(DesktopNotifierBase):
@@ -79,27 +78,24 @@
     Should be used for macOS High Sierra and earlier. Supports only a single button per
     notification. Both app name and bundle identifier will be ignored. The notification
     center automatically uses the values provided by the app bundle or the Python
     framework.
 
     :param app_name: The name of the app. Does not have any effect because the app
         name is automatically determined from the bundle or framework.
-    :param app_icon: The icon of the app. Does not have any effect because the app
-        icon is automatically determined from the bundle or framework.
     :param notification_limit: Maximum number of notifications to keep in the system's
         notification center.
     """
 
     def __init__(
         self,
         app_name: str = "Python",
-        app_icon: Optional[str] = None,
-        notification_limit: Optional[int] = None,
+        notification_limit: int | None = None,
     ) -> None:
-        super().__init__(app_name, app_icon, notification_limit)
+        super().__init__(app_name, notification_limit)
 
         self.nc = NSUserNotificationCenter.defaultUserNotificationCenter
         self.nc_delegate = NotificationCenterDelegate.alloc().init()
         self.nc_delegate.interface = self
         self.nc.delegate = self.nc_delegate
 
     async def request_authorisation(self) -> bool:
@@ -115,23 +111,22 @@
         Whether we have authorisation to send notifications.
         """
         return True
 
     async def _send(
         self,
         notification: Notification,
-        notification_to_replace: Optional[Notification],
+        notification_to_replace: Notification | None,
     ) -> str:
         """
         Uses NSUserNotificationCenter to schedule a notification.
 
         :param notification: Notification to send.
         :param notification_to_replace: Notification to replace, if any.
         """
-
         if notification_to_replace:
             platform_nid = str(notification_to_replace.identifier)
         else:
             platform_nid = str(uuid.uuid4())
 
         n = NSUserNotification.alloc().init()
         n.title = notification.title
@@ -159,17 +154,15 @@
 
     async def _clear(self, notification: Notification) -> None:
         """
         Removes a notifications from the notification center
 
         :param notification: Notification to clear.
         """
-
         if hasattr(notification, "_native"):
-            self.nc.removeDeliveredNotification(notification._native)  # type: ignore
+            self.nc.removeDeliveredNotification(notification._native)
 
     async def _clear_all(self) -> None:
         """
         Clears all notifications from notification center
         """
-
         self.nc.removeAllDeliveredNotifications()
```

### Comparing `desktop-notifier-3.4.3/src/desktop_notifier/macos_support.py` & `desktop-notifier-3.5.0/src/desktop_notifier/macos_support.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 Support module for macOS.
 
 """
 
 import platform
 import ctypes
 
+from typing import cast
+
 from packaging.version import Version
 from rubicon.objc import ObjCClass
 from rubicon.objc.runtime import load_library
 
 
 macos_version = Version(platform.mac_ver()[0])
 
@@ -75,8 +77,8 @@
     signed_status = sec.SecStaticCodeCheckValidityWithErrors(
         static_code,
         kSecCSCheckAllArchitectures | kSecCSCheckNestedCode | kSecCSStrictValidate,
         None,
         None,
     )
 
-    return signed_status == 0
+    return cast(int, signed_status) == 0
```

### Comparing `desktop-notifier-3.4.3/src/desktop_notifier/main.py` & `desktop-notifier-3.5.0/src/desktop_notifier/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # -*- coding: utf-8 -*-
 """
 This module handles desktop notifications and supports multiple backends, depending on
 the platform.
 """
 
+from __future__ import annotations
+
 # system imports
 import platform
 from threading import RLock
 import logging
 import asyncio
 from pathlib import Path
 from typing import (
     Type,
-    Union,
-    Optional,
     Callable,
     Coroutine,
     List,
     Any,
     TypeVar,
     Sequence,
 )
@@ -55,15 +55,14 @@
     """
     Return the backend class depending on the platform and version.
 
     :returns: A desktop notification backend suitable for the current platform.
     :raises RuntimeError: when passing ``macos_legacy = True`` on macOS 12.0 and later.
     """
     if platform.system() == "Darwin":
-
         from .macos_support import is_bundle, is_signed_bundle, macos_version
 
         has_unusernotificationcenter = macos_version >= Version("10.14")
         has_nsusernotificationcenter = macos_version < Version("12.0")
         is_signed = is_signed_bundle()
 
         if has_unusernotificationcenter and is_signed:
@@ -137,27 +136,31 @@
         icon theme. If None, the icon of the calling application will be used if it
         can be determined. On macOS, this argument is ignored and the app icon is
         identified by the bundle ID of the sending program (e.g., Python).
     :param notification_limit: Maximum number of notifications to keep in the system's
         notification center. This may be ignored by some implementations.
     """
 
+    app_icon: str | None
+
     def __init__(
         self,
         app_name: str = "Python",
-        app_icon: Union[Path, str, None] = PYTHON_ICON_PATH,
-        notification_limit: Optional[int] = None,
+        app_icon: Path | str | None = PYTHON_ICON_PATH,
+        notification_limit: int | None = None,
     ) -> None:
         impl_cls = get_implementation()
 
         if isinstance(app_icon, Path):
-            app_icon = app_icon.as_uri()
+            self.app_icon = app_icon.as_uri()
+        else:
+            self.app_icon = app_icon
 
         self._lock = RLock()
-        self._impl = impl_cls(app_name, app_icon, notification_limit)
+        self._impl = impl_cls(app_name, notification_limit)
         self._did_request_authorisation = False
 
         # Use our own event loop for the sync API so that we don't interfere with any
         # other ansycio event loops / threads, etc.
         self._loop = default_event_loop_policy.new_event_loop()
 
     def _run_coro_sync(self, coro: Coroutine[None, None, T]) -> T:
@@ -179,27 +182,14 @@
         return self._impl.app_name
 
     @app_name.setter
     def app_name(self, value: str) -> None:
         """Setter: app_name"""
         self._impl.app_name = value
 
-    @property
-    def app_icon(self) -> Optional[str]:
-        """The application icon: a URI for a local file or an icon name."""
-        return self._impl.app_icon
-
-    @app_icon.setter
-    def app_icon(self, value: Union[Path, str, None]) -> None:
-        """Setter: app_icon"""
-        if isinstance(value, Path):
-            value = value.as_uri()
-
-        self._impl.app_icon = value
-
     async def request_authorisation(self) -> bool:
         """
         Requests authorisation to send user notifications. This will be automatically
         called for you when sending a notification for the first time. It also can be
         called manually to request authorisation in advance.
 
         On some platforms such as macOS and iOS, a prompt will be shown to the user
@@ -217,22 +207,22 @@
         return await self._impl.has_authorisation()
 
     async def send(
         self,
         title: str,
         message: str,
         urgency: Urgency = Urgency.Normal,
-        icon: Union[Path, str, None] = None,
+        icon: Path | str | None = None,
         buttons: Sequence[Button] = (),
-        reply_field: Optional[ReplyField] = None,
-        on_clicked: Optional[Callable[[], Any]] = None,
-        on_dismissed: Optional[Callable[[], Any]] = None,
-        attachment: Union[Path, str, None] = None,
+        reply_field: ReplyField | None = None,
+        on_clicked: Callable[[], Any] | None = None,
+        on_dismissed: Callable[[], Any] | None = None,
+        attachment: Path | str | None = None,
         sound: bool = False,
-        thread: Optional[str] = None,
+        thread: str | None = None,
         timeout: int = -1,
     ) -> Notification:
         """
         Sends a desktop notification.
 
         Some arguments may be ignored, depending on the backend.
 
@@ -315,22 +305,22 @@
             return notification
 
     def send_sync(
         self,
         title: str,
         message: str,
         urgency: Urgency = Urgency.Normal,
-        icon: Union[Path, str, None] = None,
+        icon: Path | str | None = None,
         buttons: Sequence[Button] = (),
-        reply_field: Optional[ReplyField] = None,
-        on_clicked: Optional[Callable[[], Any]] = None,
-        on_dismissed: Optional[Callable[[], Any]] = None,
-        attachment: Union[Path, str, None] = None,
+        reply_field: ReplyField | None = None,
+        on_clicked: Callable[[], Any] | None = None,
+        on_dismissed: Callable[[], Any] | None = None,
+        attachment: Path | str | None = None,
         sound: bool = False,
-        thread: Optional[str] = None,
+        thread: str | None = None,
         timeout: int = -1,
     ) -> Notification:
         """
         Synchronous call of :meth:`send`, for use without an asyncio event loop.
 
         :returns: The scheduled notification instance.
         """
```

### Comparing `desktop-notifier-3.4.3/src/desktop_notifier/winrt.py` & `desktop-notifier-3.5.0/src/desktop_notifier/winrt.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,146 +3,109 @@
 Notification backend for Windows. Unlike other platforms, sending rich "toast"
 notifications cannot be done via FFI / ctypes because the C winapi only supports basic
 notifications with a title and message. This backend therefore requires interaction with
 the Windows Runtime and uses the winrt package with compiled components published by
 Microsoft (https://github.com/microsoft/xlang, https://pypi.org/project/winrt/).
 """
 
+from __future__ import annotations
+
 # system imports
 import uuid
 import logging
 from xml.etree.ElementTree import Element, SubElement, tostring
-from typing import Optional, TypeVar, cast
+from typing import TypeVar, Any, cast
 
 # external imports
+import winreg
 from winsdk.windows.ui.notifications import (
     ToastNotificationManager,
     ToastNotificationPriority,
     NotificationSetting,
     ToastNotification,
     ToastActivatedEventArgs,
     ToastDismissalReason,
 )
 from winsdk.windows.data.xml import dom
 from winsdk.windows.applicationmodel.core import CoreApplication
-from winsdk.windows.applicationmodel.background import (
-    BackgroundTaskRegistration,
-    BackgroundTaskBuilder,
-    BackgroundExecutionManager,
-    BackgroundAccessStatus,
-    ToastNotificationActionTrigger,
-)
 from winsdk.windows.foundation import IPropertyValue, PropertyType
+import winsdk._winrt as _winrt
 
 # local imports
 from .base import Notification, DesktopNotifierBase, Urgency
 
 
 __all__ = ["WinRTDesktopNotifier"]
 
 logger = logging.getLogger(__name__)
 
 T = TypeVar("T")
 
 
+def register_hkey(app_id: str, app_name: str) -> None:
+    winreg.ConnectRegistry(None, winreg.HKEY_CURRENT_USER)  # type:ignore
+    key_path = f"SOFTWARE\\Classes\\AppUserModelId\\{app_id}"
+    with winreg.CreateKeyEx(  # type:ignore
+        winreg.HKEY_CURRENT_USER, key_path  # type:ignore
+    ) as master_key:
+        winreg.SetValueEx(  # type:ignore
+            master_key, "DisplayName", 0, winreg.REG_SZ, app_name  # type:ignore
+        )
+
+
 class WinRTDesktopNotifier(DesktopNotifierBase):
     """Notification backend for the Windows Runtime
 
     :param app_name: The name of the app. This has no effect since the app name will be
         automatically determined.
-    :param app_icon: The default icon to use for notifications. This has no effect since
-        the app icon will be automatically determined.
     :param notification_limit: Maximum number of notifications to keep in the system's
         notification center.
     """
 
     _to_native_urgency = {
         Urgency.Low: ToastNotificationPriority.DEFAULT,
         Urgency.Normal: ToastNotificationPriority.DEFAULT,
         Urgency.Critical: ToastNotificationPriority.HIGH,
     }
 
-    background_task_name = "DesktopNotifier-ToastBackgroundTask"
-
     def __init__(
         self,
         app_name: str = "Python",
-        app_icon: Optional[str] = None,
-        notification_limit: Optional[int] = None,
+        notification_limit: int | None = None,
     ) -> None:
-        super().__init__(app_name, app_icon, notification_limit)
-        self._appid = CoreApplication.get_id()
+        super().__init__(app_name, notification_limit)
         self.manager = ToastNotificationManager.get_default()
-        self.notifier: ToastNotification | None = None
-        if self._appid == "":
-            logger.warning(
-                "Only applications can send desktop notifications. "
-                "Could not find App ID for process."
-            )
+
+        # Prefer using the real App ID if detected, fall back to user-provided name
+        # and icon otherwise.
+        if CoreApplication.id != "":
+            self.app_id = CoreApplication.id
         else:
-            self.notifier = self.manager.create_toast_notifier(self._appid)
+            self.app_id = app_name
+            register_hkey(app_name, app_name)
+        self.notifier = self.manager.create_toast_notifier(self.app_id)
 
     async def request_authorisation(self) -> bool:
         """
         Request authorisation to send notifications.
 
         :returns: Whether authorisation has been granted.
         """
-        if not await self._request_background_task_access():
-            return False
-        return await self.has_authorisation()
+        return bool(self.notifier.setting == NotificationSetting.ENABLED)
 
     async def has_authorisation(self) -> bool:
         """
         Whether we have authorisation to send notifications.
         """
-        if not self.notifier:
-            return False
-        return (
-            self.notifier.setting == NotificationSetting.ENABLED
-            and await self._has_background_task_access()
-        )
-
-    async def _has_background_task_access(self) -> bool:
-        res = await BackgroundExecutionManager.request_access_async(self._appid)
-        return res not in {
-            BackgroundAccessStatus.DENIED_BY_SYSTEM_POLICY,
-            BackgroundAccessStatus.DENIED_BY_USER,
-        }
-
-    def _has_registered_background_task(self) -> bool:
-        tasks = BackgroundTaskRegistration.get_all_tasks()
-        return any(t.name == self.background_task_name for t in tasks.values())
-
-    async def _request_background_task_access(self) -> bool:
-        """Request permission to activate in the background."""
-        if not self.notifier:
-            return False
-
-        if not await self._has_background_task_access():
-            logger.warning("This app is not allowed to run background tasks.")
-            return False
-
-        # If background task is already registered, do nothing.
-        if self._has_registered_background_task():
-            return True
-
-        # Create the background tasks.
-        builder = BackgroundTaskBuilder()
-        builder.name = self.background_task_name
-
-        builder.set_trigger(ToastNotificationActionTrigger())
-        builder.register()
-
-        return True
+        return bool(self.notifier.setting == NotificationSetting.ENABLED)
 
     async def _send(
         self,
         notification: Notification,
-        notification_to_replace: Optional[Notification],
+        notification_to_replace: Notification | None,
     ) -> str:
         """
         Asynchronously sends a notification.
 
         :param notification: Notification to send.
         :param notification_to_replace: Notification to replace, if any.
         """
@@ -229,41 +192,42 @@
         native.priority = self._to_native_urgency[notification.urgency]
 
         if notification.thread:
             native.group = notification.thread
         else:
             native.group = "default"
 
-        def on_activated(sender, boxed_activated_args):
+        def on_activated(sender, boxed_activated_args) -> None:  # type:ignore
             activated_args = ToastActivatedEventArgs._from(boxed_activated_args)
             action_id = cast(str, activated_args.arguments)
 
             if action_id == "default":
                 if notification.on_clicked:
                     notification.on_clicked()
 
             elif action_id == "action=reply&amp":
-                if notification.reply_field.on_replied:
+                if notification.reply_field and notification.reply_field.on_replied:
                     boxed_text = activated_args.user_input["textBox"]
                     text = unbox_winrt(boxed_text)
                     notification.reply_field.on_replied(text)
 
             elif action_id.isnumeric():
                 action_number = int(action_id)
-                notification.buttons[action_number].on_pressed()
-
-        def on_dismissed(sender, dismissed_args):
+                callback = notification.buttons[action_number].on_pressed
+                if callback:
+                    callback()
 
+        def on_dismissed(sender, dismissed_args) -> None:  # type:ignore
             self._clear_notification_from_cache(notification)
 
             if dismissed_args.reason == ToastDismissalReason.USER_CANCELED:
                 if notification.on_dismissed:
                     notification.on_dismissed()
 
-        def on_failed(sender, failed_args):
+        def on_failed(sender, failed_args) -> None:  # type:ignore
             logger.warning(
                 f"Notification failed (error code {failed_args.error_code.value})"
             )
 
         native.add_activated(on_activated)
         native.add_dismissed(on_dismissed)
         native.add_failed(on_failed)
@@ -273,24 +237,24 @@
         return platform_nid
 
     async def _clear(self, notification: Notification) -> None:
         """c
         Asynchronously removes a notification from the notification center.
         """
         group = notification.thread or "default"
-        self.manager.history.remove(notification.identifier, group, self._appid)
+        self.manager.history.remove(notification.identifier, group, self.app_id)
 
     async def _clear_all(self) -> None:
         """
         Asynchronously clears all notifications from notification center.
         """
-        self.manager.history.clear(self._appid)
+        self.manager.history.clear(self.app_id)
 
 
-def unbox_winrt(boxed_value):
+def unbox_winrt(boxed_value: _winrt.Object) -> Any:
     """
     Unbox winrt object. See https://github.com/pywinrt/pywinrt/issues/8.
     """
     if boxed_value is None:
         return boxed_value
 
     value = IPropertyValue._from(boxed_value)
```

### Comparing `desktop-notifier-3.4.3/src/desktop_notifier.egg-info/PKG-INFO` & `desktop-notifier-3.5.0/src/desktop_notifier.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: desktop-notifier
-Version: 3.4.3
+Version: 3.5.0
 Summary: Python library for cross-platform desktop notifications
-Home-page: https://github.com/samschott/desktop-notifier
-Author: Sam Schott
-Author-email: sam.schott@outlook.com
+Author-email: Sam Schott <sam.schott@outlook.com>
 License: MIT
+Project-URL: Homepage, https://github.com/samschott/desktop-notifier
 Keywords: desktop-notifier
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -37,25 +36,38 @@
 * macOS and iOS via the Notification Center framework
 * [**exprimental**] Windows via the WinRT / Python bridge.
 
 ![gif](screenshots/macOS.gif)
 
 ## Features
 
-Where supported by the native platform APIs:
+`desktop-notifier` aims to be a good citizen of the platforms which it supports. It
+therefore stays within the limits of the native platform APIs and does not try to
+work around limitations which are often deliberate UI choices. For example, on macOS
+and iOS, it is not possible to change the app icon which is shown on notifications.
+There are possible workarounds - that would likely be rejected by an App Store review.
 
-* Clickable notifications
+Where supported by the native platform APIs, `desktop-notifier` allows for:
+
+* Clickable notifications with callbacks on user interaction
 * Multiple action buttons
 * A single reply field (e.g., for chat notifications)
-* Asyncio integration: the main API consists of async methods and a running event loop
-  is required to respond to user interactions with a notification
 * Notification sounds
-* Notification threads (e.g., for different conversations)
-* Limit maximum number of notifications shown in the notification center
-* Pure Python dependencies only, no extension modules
+* Notification threads (grouping notifications by topic)
+* Limiting maximum number of notifications shown in the notification center
+
+An exhaustive list of features and their platform support is provided in the
+[documentation](https://desktop-notifier.readthedocs.io/en/latest/background/platform_support.html).
+
+Design choices by `desktop-notifier`:
+
+* Asyncio API: The main API consists of async methods and a running event loop
+  is required to respond to user interactions with a notification.
+* Pure Python dependencies only, no extension modules (with the exception of
+  of the Windows backend).
 
 ## Installation
 
 From PyPI:
 
 ```
 pip3 install -U desktop-notifier
```

### Comparing `desktop-notifier-3.4.3/src/desktop_notifier.egg-info/SOURCES.txt` & `desktop-notifier-3.5.0/src/desktop_notifier.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 LICENSE
 README.md
 pyproject.toml
-setup.cfg
 src/desktop_notifier/__init__.py
 src/desktop_notifier/base.py
 src/desktop_notifier/dbus.py
 src/desktop_notifier/dummy.py
 src/desktop_notifier/macos.py
 src/desktop_notifier/macos_legacy.py
 src/desktop_notifier/macos_support.py
 src/desktop_notifier/main.py
-src/desktop_notifier/py.typed
 src/desktop_notifier/winrt.py
 src/desktop_notifier.egg-info/PKG-INFO
 src/desktop_notifier.egg-info/SOURCES.txt
 src/desktop_notifier.egg-info/dependency_links.txt
-src/desktop_notifier.egg-info/not-zip-safe
 src/desktop_notifier.egg-info/requires.txt
 src/desktop_notifier.egg-info/top_level.txt
-src/desktop_notifier/resources/__init__.py
-src/desktop_notifier/resources/python.png
+src/desktop_notifier/resources/__init__.py
```

