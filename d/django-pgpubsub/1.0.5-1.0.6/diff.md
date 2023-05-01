# Comparing `tmp/django_pgpubsub-1.0.5.tar.gz` & `tmp/django_pgpubsub-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_pgpubsub-1.0.5.tar", max compression
+gzip compressed data, was "django_pgpubsub-1.0.6.tar", max compression
```

## Comparing `django_pgpubsub-1.0.5.tar` & `django_pgpubsub-1.0.6.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0     1456 2022-11-05 17:21:11.401611 django_pgpubsub-1.0.5/LICENSE
--rw-r--r--   0        0        0    25976 2023-04-10 16:26:51.399667 django_pgpubsub-1.0.5/README.md
--rw-r--r--   0        0        0      390 2022-11-05 17:21:11.403909 django_pgpubsub-1.0.5/pgpubsub/__init__.py
--rw-r--r--   0        0        0     7341 2023-04-11 13:37:33.189103 django_pgpubsub-1.0.5/pgpubsub/channel.py
--rw-r--r--   0        0        0     4980 2023-02-02 16:18:56.082239 django_pgpubsub-1.0.5/pgpubsub/listen.py
--rw-r--r--   0        0        0     2647 2023-01-10 17:48:32.840212 django_pgpubsub-1.0.5/pgpubsub/listeners.py
--rw-r--r--   0        0        0        0 2022-11-05 17:21:11.404451 django_pgpubsub-1.0.5/pgpubsub/management/__init__.py
--rw-r--r--   0        0        0        0 2022-11-05 17:21:11.404567 django_pgpubsub-1.0.5/pgpubsub/management/commands/__init__.py
--rw-r--r--   0        0        0     1288 2023-02-02 16:18:56.082808 django_pgpubsub-1.0.5/pgpubsub/management/commands/listen.py
--rw-r--r--   0        0        0      751 2023-04-10 16:26:51.407699 django_pgpubsub-1.0.5/pgpubsub/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2022-11-05 17:21:11.405068 django_pgpubsub-1.0.5/pgpubsub/migrations/__init__.py
--rw-r--r--   0        0        0      690 2023-04-10 16:26:51.408192 django_pgpubsub-1.0.5/pgpubsub/models.py
--rw-r--r--   0        0        0     2130 2022-11-05 17:21:11.405511 django_pgpubsub-1.0.5/pgpubsub/notify.py
--rw-r--r--   0        0        0        0 2022-11-05 17:21:11.405631 django_pgpubsub-1.0.5/pgpubsub/tests/__init__.py
--rw-r--r--   0        0        0      164 2022-11-05 17:21:11.405752 django_pgpubsub-1.0.5/pgpubsub/tests/apps.py
--rw-r--r--   0        0        0      640 2023-04-11 08:28:49.364826 django_pgpubsub-1.0.5/pgpubsub/tests/channels.py
--rw-r--r--   0        0        0     1938 2023-04-11 08:32:09.955989 django_pgpubsub-1.0.5/pgpubsub/tests/listeners.py
--rw-r--r--   0        0        0     2734 2022-11-05 17:21:11.406152 django_pgpubsub-1.0.5/pgpubsub/tests/migrations/0001_initial.py
--rw-r--r--   0        0        0      673 2023-04-11 13:37:33.190988 django_pgpubsub-1.0.5/pgpubsub/tests/migrations/0002_auto_20230411_0829.py
--rw-r--r--   0        0        0        0 2022-11-05 17:21:11.406217 django_pgpubsub-1.0.5/pgpubsub/tests/migrations/__init__.py
--rw-r--r--   0        0        0     1348 2023-04-11 13:37:33.192550 django_pgpubsub-1.0.5/pgpubsub/tests/models.py
--rw-r--r--   0        0        0     5876 2023-04-11 13:37:33.193462 django_pgpubsub-1.0.5/pgpubsub/tests/test_core.py
--rw-r--r--   0        0        0     2199 2023-04-11 13:37:33.194348 django_pgpubsub-1.0.5/pgpubsub/tests/test_deserialize.py
--rw-r--r--   0        0        0     4286 2023-04-11 13:37:33.194866 django_pgpubsub-1.0.5/pgpubsub/tests/test_trigger_deserialize.py
--rw-r--r--   0        0        0     1040 2023-04-10 16:26:51.410131 django_pgpubsub-1.0.5/pgpubsub/triggers.py
--rw-r--r--   0        0        0     2082 2023-04-11 13:37:57.567950 django_pgpubsub-1.0.5/pyproject.toml
--rw-r--r--   0        0        0    27299 1970-01-01 00:00:00.000000 django_pgpubsub-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1456 2022-11-05 17:21:11.401611 django_pgpubsub-1.0.6/LICENSE
+-rw-r--r--   0        0        0    25976 2023-04-10 16:26:51.399667 django_pgpubsub-1.0.6/README.md
+-rw-r--r--   0        0        0      390 2022-11-05 17:21:11.403909 django_pgpubsub-1.0.6/pgpubsub/__init__.py
+-rw-r--r--   0        0        0     7492 2023-04-26 18:48:54.103379 django_pgpubsub-1.0.6/pgpubsub/channel.py
+-rw-r--r--   0        0        0     5158 2023-05-01 16:03:41.570536 django_pgpubsub-1.0.6/pgpubsub/listen.py
+-rw-r--r--   0        0        0     2647 2023-01-10 17:48:32.840212 django_pgpubsub-1.0.6/pgpubsub/listeners.py
+-rw-r--r--   0        0        0        0 2022-11-05 17:21:11.404451 django_pgpubsub-1.0.6/pgpubsub/management/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-05 17:21:11.404567 django_pgpubsub-1.0.6/pgpubsub/management/commands/__init__.py
+-rw-r--r--   0        0        0     1288 2023-02-02 16:18:56.082808 django_pgpubsub-1.0.6/pgpubsub/management/commands/listen.py
+-rw-r--r--   0        0        0      751 2023-04-10 16:26:51.407699 django_pgpubsub-1.0.6/pgpubsub/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2022-11-05 17:21:11.405068 django_pgpubsub-1.0.6/pgpubsub/migrations/__init__.py
+-rw-r--r--   0        0        0      690 2023-04-10 16:26:51.408192 django_pgpubsub-1.0.6/pgpubsub/models.py
+-rw-r--r--   0        0        0     2132 2023-05-01 16:03:41.571304 django_pgpubsub-1.0.6/pgpubsub/notify.py
+-rw-r--r--   0        0        0        0 2022-11-05 17:21:11.405631 django_pgpubsub-1.0.6/pgpubsub/tests/__init__.py
+-rw-r--r--   0        0        0      164 2022-11-05 17:21:11.405752 django_pgpubsub-1.0.6/pgpubsub/tests/apps.py
+-rw-r--r--   0        0        0      640 2023-04-11 08:28:49.364826 django_pgpubsub-1.0.6/pgpubsub/tests/channels.py
+-rw-r--r--   0        0        0     1926 2023-05-01 16:03:41.571905 django_pgpubsub-1.0.6/pgpubsub/tests/listeners.py
+-rw-r--r--   0        0        0     2734 2022-11-05 17:21:11.406152 django_pgpubsub-1.0.6/pgpubsub/tests/migrations/0001_initial.py
+-rw-r--r--   0        0        0      673 2023-04-26 17:40:53.933980 django_pgpubsub-1.0.6/pgpubsub/tests/migrations/0002_auto_20230411_0829.py
+-rw-r--r--   0        0        0     2880 2023-04-26 19:11:19.787192 django_pgpubsub-1.0.6/pgpubsub/tests/migrations/0003_author_pgpubsub_160cf_media_pgpubsub_a83de_and_more.py
+-rw-r--r--   0        0        0        0 2022-11-05 17:21:11.406217 django_pgpubsub-1.0.6/pgpubsub/tests/migrations/__init__.py
+-rw-r--r--   0        0        0     1348 2023-04-11 13:37:33.192550 django_pgpubsub-1.0.6/pgpubsub/tests/models.py
+-rw-r--r--   0        0        0     6436 2023-05-01 16:03:41.572816 django_pgpubsub-1.0.6/pgpubsub/tests/test_core.py
+-rw-r--r--   0        0        0     2199 2023-04-11 13:37:33.194348 django_pgpubsub-1.0.6/pgpubsub/tests/test_deserialize.py
+-rw-r--r--   0        0        0     4478 2023-04-26 18:48:54.104075 django_pgpubsub-1.0.6/pgpubsub/tests/test_trigger_deserialize.py
+-rw-r--r--   0        0        0     1040 2023-04-10 16:26:51.410131 django_pgpubsub-1.0.6/pgpubsub/triggers.py
+-rw-r--r--   0        0        0     2082 2023-05-01 16:04:19.432801 django_pgpubsub-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0    27299 1970-01-01 00:00:00.000000 django_pgpubsub-1.0.6/PKG-INFO
```

### Comparing `django_pgpubsub-1.0.5/LICENSE` & `django_pgpubsub-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django_pgpubsub-1.0.5/README.md` & `django_pgpubsub-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `django_pgpubsub-1.0.5/pgpubsub/channel.py` & `django_pgpubsub-1.0.6/pgpubsub/channel.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import hashlib
 from abc import abstractmethod
 from collections import defaultdict
 from dataclasses import dataclass
+from decimal import Decimal
 import datetime
 import inspect
 import json
 from pydoc import locate
 from typing import Callable, Dict, Union, List
 
 from django.apps import apps
 from django.core import serializers
+from django.core.serializers.json import DjangoJSONEncoder
 from django.db import models
 
 
 registry = defaultdict(list)
 
 
 @dataclass
@@ -46,22 +48,22 @@
     def register(cls, callback: Callable):
         registry[cls].append(callback)
 
     @classmethod
     @abstractmethod
     def deserialize(cls, payload: Union[Dict, str]):
         if isinstance(payload, str):
-            payload = json.loads(payload)
+            payload = json.loads(payload, parse_float=Decimal)
         return payload
 
     @classmethod
     def build_from_payload(
-            cls,
-            notification_payload: Union[Dict, str],
-            callbacks: List[Callable],
+        cls,
+        notification_payload: Union[Dict, str],
+        callbacks: List[Callable],
     ):
         deserialized = cls.deserialize(notification_payload)
         channel = cls(**deserialized)
         channel.callbacks.extend(callbacks)
         return channel
 
     @property
@@ -114,14 +116,15 @@
                 }
             elif origin_type in (list, tuple, set):
                 serialized_val = [self._date_serial(x) for x in val]
             serialized_kwargs[kwarg] = serialized_val
         return json.dumps(
             {'kwargs': serialized_kwargs},
             default=self._date_serial,
+            cls=DjangoJSONEncoder,
         )
 
     @staticmethod
     def _date_serial(obj):
         if isinstance(obj, (datetime.datetime, datetime.date)):
             return obj.isoformat()
         return obj
@@ -140,27 +143,25 @@
     model = NotImplementedError
     old: models.Model
     new: models.Model
 
     @classmethod
     def deserialize(cls, payload: Union[Dict, str]):
         payload_dict = super().deserialize(payload)
-        old_model_data = cls._build_model_serializer_data(
-            payload_dict, state='old')
-        new_model_data = cls._build_model_serializer_data(
-            payload_dict, state='new')
+        old_model_data = cls._build_model_serializer_data(payload_dict, state='old')
+        new_model_data = cls._build_model_serializer_data(payload_dict, state='new')
 
         old_deserialized_objects = serializers.deserialize(
             'json',
-            json.dumps(old_model_data),
+            json.dumps(old_model_data, cls=DjangoJSONEncoder),
             ignorenonexistent=True,
         )
         new_deserialized_objects = serializers.deserialize(
             'json',
-            json.dumps(new_model_data),
+            json.dumps(new_model_data, cls=DjangoJSONEncoder),
             ignorenonexistent=True,
         )
 
         old = next(old_deserialized_objects, None)
         if old is not None:
             old = old.object
         new = next(new_deserialized_objects, None)
```

### Comparing `django_pgpubsub-1.0.5/pgpubsub/listen.py` & `django_pgpubsub-1.0.6/pgpubsub/listen.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,58 +12,59 @@
     ChannelNotFound,
     locate_channel,
     registry,
 )
 from pgpubsub.models import Notification
 
 
+POLL = True
+
+
 def listen(
-    channels: Union[List[BaseChannel], List[str]]=None,
-    recover: bool=False,
-    poll_count: Union[None, int]=None,
+    channels: Union[List[BaseChannel], List[str]] = None,
+    recover: bool = False,
 ):
     multiprocessing.set_start_method('fork', force=True)
     pg_connection = listen_to_channels(channels)
+
     if recover:
         process_stored_notifications(channels)
         process_notifications(pg_connection)
-    poll_count = poll_count or float('inf')
-    print('Listening for notifications...')
-    while poll_count:
+
+    print('Listening for notifications... \n')
+    while POLL:
         if select.select([pg_connection], [], [], 1) == ([], [], []):
             pass
         else:
             try:
                 process_notifications(pg_connection)
             except Exception as e:
                 print(f'Encountered exception {e}')
                 print('Restarting process')
                 connection.close()
-                process = multiprocessing.Process(
-                    target=listen, args=(channels,))
+                process = multiprocessing.Process(target=listen, args=(channels,))
                 process.start()
                 raise
-        poll_count -= 1
 
 
-def listen_to_channels(channels: Union[List[BaseChannel], List[str]]=None):
+def listen_to_channels(channels: Union[List[BaseChannel], List[str]] = None):
     if channels is None:
         channels = registry
     else:
         channels = [locate_channel(channel) for channel in channels]
         channels = {
             channel: callbacks
             for channel, callbacks in registry.items()
             if issubclass(channel, tuple(channels))
         }
     if not channels:
         raise ChannelNotFound()
     cursor = connection.cursor()
     for channel in channels:
-        print(f'Listening on {channel.name()}')
+        print(f'Listening on {channel.name()}\n')
         cursor.execute(f'LISTEN {channel.listen_safe_name()};')
     return connection.connection
 
 
 def process_notifications(pg_connection):
     pg_connection.poll()
     while pg_connection.notifies:
@@ -82,33 +83,30 @@
                     processor.process()
                     break
 
 
 class NotificationProcessor:
     def __init__(self, notification: Notify, pg_connection):
         self.notification = notification
-        self.channel_cls, self.callbacks = Channel.get(
-            notification.channel)
+        self.channel_cls, self.callbacks = Channel.get(notification.channel)
         self.pg_connection = pg_connection
         self.validate()
 
     def validate(self):
         if self.channel_cls.lock_notifications:
             raise InvalidNotificationProcessor
 
     def process(self):
-        print(
-            f'Processing notification for {self.channel_cls.name()}')
+        print(f'Processing notification for {self.channel_cls.name()}\n')
         return self._execute()
 
     def _execute(self):
         channel = self.channel_cls.build_from_payload(
             self.notification.payload, self.callbacks)
         channel.execute_callbacks()
-        print('\n')
         self.pg_connection.poll()
 
 
 class LockableNotificationProcessor(NotificationProcessor):
 
     def validate(self):
         if self.notification.payload == 'null':
@@ -128,33 +126,37 @@
             print(f'Could not obtain a lock on notification '
                   f'{self.notification.pid}')
             print('\n')
         else:
             print(f'Obtained lock on {notification}')
             self.notification = notification
             self._execute()
-
-    def _execute(self):
-        super()._execute()
-        self.notification.delete()
+            self.notification.delete()
 
 
 class NotificationRecoveryProcessor(LockableNotificationProcessor):
 
     def validate(self):
         if self.notification.payload != 'null':
             raise InvalidNotificationProcessor
 
     def process(self):
-        print(f'Processing all notifications for '
-              f'channel {self.channel_cls.name()}')
+        print(f'Processing all notifications for channel {self.channel_cls.name()} \n')
         notifications = (
             Notification.objects.select_for_update(
                 skip_locked=True).filter(channel=self.notification.channel)
         )
+        print(f'Found notifications: {notifications}')
         for notification in notifications:
             self.notification = notification
-            self._execute()
+            try:
+                with transaction.atomic():
+                    self._execute()
+            except Exception as e:
+                print(f'Encountered {e} exception when processing notification {notification}')
+            else:
+                print(f'Successfully processed notification {notification}')
+                self.notification.delete()
 
 
 class InvalidNotificationProcessor(Exception):
     pass
```

### Comparing `django_pgpubsub-1.0.5/pgpubsub/listeners.py` & `django_pgpubsub-1.0.6/pgpubsub/listeners.py`

 * *Files identical despite different names*

### Comparing `django_pgpubsub-1.0.5/pgpubsub/management/commands/listen.py` & `django_pgpubsub-1.0.6/pgpubsub/management/commands/listen.py`

 * *Files identical despite different names*

### Comparing `django_pgpubsub-1.0.5/pgpubsub/migrations/0001_initial.py` & `django_pgpubsub-1.0.6/pgpubsub/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_pgpubsub-1.0.5/pgpubsub/models.py` & `django_pgpubsub-1.0.6/pgpubsub/models.py`

 * *Files identical despite different names*

### Comparing `django_pgpubsub-1.0.5/pgpubsub/notify.py` & `django_pgpubsub-1.0.6/pgpubsub/notify.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,12 +46,12 @@
         }
     with connection.cursor() as cursor:
         lock_channels = [c for c in channels if c.lock_notifications]
         for channel_cls in lock_channels:
             payload = 'null'
             print(
                 f'Notifying channel {channel_cls.name()} to recover '
-                f'previously stored notifications.')
+                f'previously stored notifications.\n')
             cursor.execute(
                 f"select pg_notify('{channel_cls.listen_safe_name()}', '{payload}');")
```

### Comparing `django_pgpubsub-1.0.5/pgpubsub/tests/channels.py` & `django_pgpubsub-1.0.6/pgpubsub/tests/channels.py`

 * *Files identical despite different names*

### Comparing `django_pgpubsub-1.0.5/pgpubsub/tests/listeners.py` & `django_pgpubsub-1.0.6/pgpubsub/tests/listeners.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import time
 from collections import defaultdict
 import datetime
 
 from django.db.transaction import atomic
 
 import pgpubsub
 from pgpubsub.tests.channels import (
```

### Comparing `django_pgpubsub-1.0.5/pgpubsub/tests/migrations/0001_initial.py` & `django_pgpubsub-1.0.6/pgpubsub/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_pgpubsub-1.0.5/pgpubsub/tests/migrations/0002_auto_20230411_0829.py` & `django_pgpubsub-1.0.6/pgpubsub/tests/migrations/0002_auto_20230411_0829.py`

 * *Files identical despite different names*

### Comparing `django_pgpubsub-1.0.5/pgpubsub/tests/models.py` & `django_pgpubsub-1.0.6/pgpubsub/tests/models.py`

 * *Files identical despite different names*

### Comparing `django_pgpubsub-1.0.5/pgpubsub/tests/test_core.py` & `django_pgpubsub-1.0.6/pgpubsub/tests/test_core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 import datetime
+import json
+from unittest.mock import patch
 
+from django.contrib.auth.models import User
 from django.db.transaction import atomic
 import pytest
 
 from pgpubsub.listen import listen_to_channels, process_notifications, listen
 from pgpubsub.models import Notification
 from pgpubsub.notify import process_stored_notifications
 from pgpubsub.tests.channels import (
@@ -132,37 +135,52 @@
     assert 2 == Notification.objects.count()
     assert 0 == Post.objects.count()
     # Simulate when the listener fails to
     # receive notifications
     pg_connection.notifies = []
     pg_connection.poll()
     assert 0 == len(pg_connection.notifies)
-    listen(recover=True, poll_count=1)
+    with patch('pgpubsub.listen.POLL', False):
+        listen(recover=True)
     pg_connection.poll()
     assert 0 == Notification.objects.count()
     assert 2 == Post.objects.count()
 
 
 @pytest.mark.django_db(transaction=True)
-def test_do_not_recover_notifications(pg_connection):
-    Author.objects.create(name='Billy')
+def test_recover_notifications_after_exception(pg_connection):
+    user = User.objects.create(username='Billy')
+    author = Author.objects.create(name='Billy', user=user)
+
+    # Create a Notification with a payload which will produce
+    # an exception
+    notification = Notification.objects.last()
+    payload = json.loads(notification.payload)
+    payload['new']['user_id'] = int(author.user_id) + 1
+    notification.payload = str(payload)
+    notification.pk = None
+    notification.save()
+
     Author.objects.create(name='Billy2')
+
     pg_connection.poll()
     assert 2 == len(pg_connection.notifies)
-    assert 2 == Notification.objects.count()
+
+    assert 3 == Notification.objects.count()
     assert 0 == Post.objects.count()
-    # Simulate when the listener fails to
-    # receive notifications
+
+    # Simulate when the listener fails to receive notifications
     pg_connection.notifies = []
     pg_connection.poll()
     assert 0 == len(pg_connection.notifies)
-    listen(recover=False, poll_count=1)
+    with patch('pgpubsub.listen.POLL', False):
+        listen(recover=True)
     pg_connection.poll()
-    assert 2 == Notification.objects.count()
-    assert 0 == Post.objects.count()
+    assert 1 == Notification.objects.count()
+    assert 2 == Post.objects.count()
 
 
 @pytest.mark.django_db(transaction=True)
 def test_media_insert_notify(pg_connection):
     Media.objects.create(name='avatar.jpg', content_type='image/png', size=15000)
     assert 1 == len(pg_connection.notifies)
     stored_notification = Notification.from_channel(
```

### Comparing `django_pgpubsub-1.0.5/pgpubsub/tests/test_deserialize.py` & `django_pgpubsub-1.0.6/pgpubsub/tests/test_deserialize.py`

 * *Files identical despite different names*

### Comparing `django_pgpubsub-1.0.5/pgpubsub/tests/test_trigger_deserialize.py` & `django_pgpubsub-1.0.6/pgpubsub/tests/test_trigger_deserialize.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import datetime
 import json
 from dataclasses import dataclass
+from decimal import Decimal
 
 import pytest
 from django.contrib.auth.models import User
+from django.core.serializers.json import DjangoJSONEncoder
 from django.utils import timezone
 
 from pgpubsub import TriggerChannel
 from pgpubsub.models import Notification
 from pgpubsub.tests.channels import (
     AuthorTriggerChannel,
     MediaTriggerChannel,
@@ -18,30 +20,32 @@
 
 def test_deserialize_post_trigger_channel():
     @dataclass
     class MyChannel(TriggerChannel):
         model: Post
 
     some_datetime = datetime.datetime.utcnow()
-    post = Post(content='some-content', date=some_datetime, pk=1)
+    post = Post(content='some-content', date=some_datetime, pk=1, rating=Decimal("1.1"))
 
     deserialized = MyChannel.deserialize(
         json.dumps(
             {
                 'app': 'tests',
                 'model': 'Post',
                 'old': None,
                 'new': {
                     'content': 'some-content',
                     'date': some_datetime.isoformat(),
                     'id': post.pk,
                     # See https://github.com/Opus10/django-pgpubsub/issues/29
                     'old_field': 'foo',
+                    'rating': Decimal("1.1"),
                 },
-            }
+            },
+            cls=DjangoJSONEncoder,
         )
     )
     assert deserialized['new'].date == some_datetime
     assert deserialized['new'].content == post.content
     assert deserialized['new'].rating == post.rating
     assert deserialized['new'].author == post.author
```

### Comparing `django_pgpubsub-1.0.5/pgpubsub/triggers.py` & `django_pgpubsub-1.0.6/pgpubsub/triggers.py`

 * *Files identical despite different names*

### Comparing `django_pgpubsub-1.0.5/pyproject.toml` & `django_pgpubsub-1.0.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 fail_under = 100
 
 [tool.poetry]
 name = "django-pgpubsub"
 packages = [
   { include = "pgpubsub" }
 ]
-version = "1.0.5"
+version = "1.0.6"
 description = "A distributed task processing framework for Django built on top of the Postgres NOTIFY/LISTEN protocol."
 authors = ["Opus 10 Engineering"]
 classifiers = [
   "Intended Audience :: Developers",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.7",
```

### Comparing `django_pgpubsub-1.0.5/PKG-INFO` & `django_pgpubsub-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pgpubsub
-Version: 1.0.5
+Version: 1.0.6
 Summary: A distributed task processing framework for Django built on top of the Postgres NOTIFY/LISTEN protocol.
 Home-page: https://github.com/Opus10/django-pgpubsub
 License: BSD-3-Clause
 Author: Opus 10 Engineering
 Requires-Python: >=3.7.0,<4
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
```

