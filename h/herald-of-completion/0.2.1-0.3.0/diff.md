# Comparing `tmp/herald-of-completion-0.2.1.tar.gz` & `tmp/herald-of-completion-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "herald-of-completion-0.2.1.tar", last modified: Thu Apr 27 02:20:38 2023, max compression
+gzip compressed data, was "herald-of-completion-0.3.0.tar", last modified: Sun Apr 30 22:50:27 2023, max compression
```

## Comparing `herald-of-completion-0.2.1.tar` & `herald-of-completion-0.3.0.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 02:20:38.083356 herald-of-completion-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-27 02:20:24.000000 herald-of-completion-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7372 2023-04-27 02:20:38.083356 herald-of-completion-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-04-27 02:20:24.000000 herald-of-completion-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-27 02:20:24.000000 herald-of-completion-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-27 02:20:38.083356 herald-of-completion-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 02:20:38.079356 herald-of-completion-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 02:20:38.079356 herald-of-completion-0.2.1/src/herald/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-27 02:20:24.000000 herald-of-completion-0.2.1/src/herald/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-04-27 02:20:24.000000 herald-of-completion-0.2.1/src/herald/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 02:20:38.083356 herald-of-completion-0.2.1/src/herald/messengers/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-27 02:20:24.000000 herald-of-completion-0.2.1/src/herald/messengers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-27 02:20:24.000000 herald-of-completion-0.2.1/src/herald/messengers/desktop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-04-27 02:20:24.000000 herald-of-completion-0.2.1/src/herald/messengers/discord.py
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-04-27 02:20:24.000000 herald-of-completion-0.2.1/src/herald/messengers/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-04-27 02:20:24.000000 herald-of-completion-0.2.1/src/herald/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 02:20:38.083356 herald-of-completion-0.2.1/src/herald_of_completion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7372 2023-04-27 02:20:38.000000 herald-of-completion-0.2.1/src/herald_of_completion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-27 02:20:38.000000 herald-of-completion-0.2.1/src/herald_of_completion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 02:20:38.000000 herald-of-completion-0.2.1/src/herald_of_completion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-27 02:20:38.000000 herald-of-completion-0.2.1/src/herald_of_completion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-27 02:20:38.000000 herald-of-completion-0.2.1/src/herald_of_completion.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 02:20:38.083356 herald-of-completion-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-27 02:20:24.000000 herald-of-completion-0.2.1/tests/test_herald.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-27 02:20:24.000000 herald-of-completion-0.2.1/tests/test_messenger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:50:27.544426 herald-of-completion-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-30 22:50:13.000000 herald-of-completion-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-04-30 22:50:27.544426 herald-of-completion-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7813 2023-04-30 22:50:13.000000 herald-of-completion-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-30 22:50:13.000000 herald-of-completion-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-30 22:50:27.544426 herald-of-completion-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:50:27.540426 herald-of-completion-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:50:27.540426 herald-of-completion-0.3.0/src/herald/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-30 22:50:13.000000 herald-of-completion-0.3.0/src/herald/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-04-30 22:50:13.000000 herald-of-completion-0.3.0/src/herald/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:50:27.544426 herald-of-completion-0.3.0/src/herald/messengers/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-30 22:50:13.000000 herald-of-completion-0.3.0/src/herald/messengers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-30 22:50:13.000000 herald-of-completion-0.3.0/src/herald/messengers/desktop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-04-30 22:50:13.000000 herald-of-completion-0.3.0/src/herald/messengers/discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-04-30 22:50:13.000000 herald-of-completion-0.3.0/src/herald/messengers/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-04-30 22:50:13.000000 herald-of-completion-0.3.0/src/herald/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-04-30 22:50:13.000000 herald-of-completion-0.3.0/src/herald/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:50:27.544426 herald-of-completion-0.3.0/src/herald_of_completion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-04-30 22:50:27.000000 herald-of-completion-0.3.0/src/herald_of_completion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-30 22:50:27.000000 herald-of-completion-0.3.0/src/herald_of_completion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 22:50:27.000000 herald-of-completion-0.3.0/src/herald_of_completion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-30 22:50:27.000000 herald-of-completion-0.3.0/src/herald_of_completion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-30 22:50:27.000000 herald-of-completion-0.3.0/src/herald_of_completion.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:50:27.544426 herald-of-completion-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-04-30 22:50:13.000000 herald-of-completion-0.3.0/tests/test_arg_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-30 22:50:13.000000 herald-of-completion-0.3.0/tests/test_herald.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-04-30 22:50:13.000000 herald-of-completion-0.3.0/tests/test_messenger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-30 22:50:13.000000 herald-of-completion-0.3.0/tests/test_utils.py
```

### Comparing `herald-of-completion-0.2.1/LICENSE` & `herald-of-completion-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `herald-of-completion-0.2.1/PKG-INFO` & `herald-of-completion-0.3.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,47 +1,19 @@
-Metadata-Version: 2.1
-Name: herald-of-completion
-Version: 0.2.1
-Summary: Hark! The herald of completion has arrived ... to let you know when your long-running tasks are done.
-Home-page: https://github.com/sho-87/herald-of-completion
-Author: Simon Ho
-Author-email: simonho.ubc@gmail.com
-Keywords: notification,task,completion,function,long-running
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Natural Language :: English
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Communications :: Chat
-Classifier: Topic :: Communications :: Email
-Classifier: Topic :: System :: Monitoring
-Classifier: Topic :: Utilities
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # Herald of Completion
 
 [![Version](https://img.shields.io/github/v/release/sho-87/herald-of-completion?include_prereleases&sort=semver)](https://pypi.org/project/herald-of-completion/)
 [![pypi](https://img.shields.io/pypi/pyversions/herald-of-completion)](https://pypi.org/project/herald-of-completion/)
 ![CI](https://img.shields.io/github/actions/workflow/status/sho-87/herald-of-completion/lint_test.yml?branch=develop)
 [![Issues](https://img.shields.io/github/issues/sho-87/herald-of-completion)](https://github.com/sho-87/herald-of-completion/issues)
 [![Donate](https://img.shields.io/badge/Buy%20me%20a%20coffee-donate-blue "Donate")](https://www.buymeacoffee.com/simonho)
 
+<p align="center">
+    <img src="https://raw.githubusercontent.com/sho-87/herald-of-completion/master/docs/source/_static/herald.png" >
+</p>
+
 Hark! The herald of completion has arrived ... to let you know when your long-running tasks are done.
 
 Decorate your functions with messengers, who will send a notification to you when your function has finished running.
 
 The notification can contain a message and, optionally, the traceback if your function failed.
 
 ## Installation
@@ -82,39 +54,67 @@
 
 @herald([discord, email])  # multiple messengers can be used at the same time
 def my_function():
     a = [1, 2, 3]
     return a
 ```
 
-Passing `send_result=True` to the decorator will send the return value of your function through the messenger. This also includes notifying you of any exceptions that were raised:
+### Options
 
-```python
-from herald.decorators import Herald
-from herald.messengers import DiscordMessenger
+By default, Herald will send a basic notification message indicating whether the function finished successfully or with an error. You can pass in a custom message to use instead:
 
-herald = Herald(".env")
+```python
+@herald(email, message="My custom message")
+```
 
-discord = DiscordMessenger()
+Passing `send_result=True` to the decorator will send the return value of your function through the messenger. This also includes notifying you of any exceptions that were raised:
 
-@herald(discord, send_result=True)
+```python
+@herald(email, send_result=True)  # defaults to True
 def my_function():
     a = [1, 2, 3]
     return a[100]  # if an exception is raised, `send_result=True` will also send the traceback
 ```
 
-For more details, the full API documentation can be found here: [Documentation](https://sho-87.github.io/herald-of-completion/)
+Passing `send_args=True` will show the `args` and `kwargs` the function was called with:
+
+```python
+@herald(email, send_args=True)  # defaults to True
+def my_function(var1, var2):
+    return ", ".join([var1, var2])
+
+my_function("Hello", var2="world")  # function call will be notified with all args and kwargs
+```
+
+### Manual notifications
+
+There may be times where you want to send a notification without using a decorator / tying it to a specific function.
+
+A utility function, `send_notification()`, can be used for this purpose. To use this, you'll need to construct your own `TaskInfo` object (see: [fields](https://github.com/sho-87/herald-of-completion/blob/master/src/herald/types.py)) containing the notification contents:
+
+```python
+from herald.types import TaskInfo
+from herald.utils import send_notification  # import the utility
+
+discord = DiscordMessenger()
+email = EmailMessenger()
+info = TaskInfo(message="custom message", ...)  # create TaskInfo with contents of the message
+
+send_notification([discord, email], info, ".env")  # pass in path to your .env file, if required
+```
+
+For more details about usage, the full API documentation can be found here: [documentation](https://sho-87.github.io/herald-of-completion/)
 
 ### .env settings
 
 Some messengers require credentials and/or additional settings to work. These values are stored in a `.env` file.
 
 Pass the location of this file to the `Herald` constructor, which will pass the values down to your messengers.
 
-The `.env` file should look something like this. You only need settings for the messengers you want to use:
+The `.env` file should look something like [this](https://github.com/sho-87/herald-of-completion/blob/master/tests/test.env). You only need settings for the messengers you want to use:
 
 ```text
 # Discord settings
 WEBHOOK_URL="https://discord.com/..."
 
 # Email settings
 SMTP_SERVER="smtp.gmail.com"
@@ -145,20 +145,22 @@
 
 1. Create a new module in `src/herald/messengers/`
 2. Your class name should take the form `<Name>Messenger` and inherit the base `Messenger` abstract class. Example: `class DiscordMessenger(Messenger): ...`
 3. Your class must implement the abstract methods defined in the base `Messenger` class [here](https://github.com/sho-87/herald-of-completion/blob/develop/src/herald/types.py)
 4. Those methods define how your messenger sets it's secret values, and how it uses those settings to send a notification
 5. Finally, import your messenger in the `__init__.py` file [here](https://github.com/sho-87/herald-of-completion/blob/develop/src/herald/messengers/__init__.py). This shortens the import path for users.
 
+The `notify()` method of your messenger will receive a [TaskInfo](https://github.com/sho-87/herald-of-completion/blob/master/src/herald/types.py) dataclass object. You can use the dataclass' fields (e.g. `name`, `header`) to construct custom notification messages.
+
 **Note**: Pull requests should be made to the `develop` branch.
 
 ### Tests
 
 Unit and integration tests are located [here](https://github.com/sho-87/herald-of-completion/tree/develop/tests).
 
 Tests should be run using `pytest`.
 
 ### Code style
 
 The project is formatted using the `black` formatter.
 
-Docstrings should follow the [Google style](https://google.github.io/styleguide/pyguide.html#38-comments-and-docstrings). This will help with automatic generation of documentation.
+Docstrings should follow the [Google style](https://google.github.io/styleguide/pyguide.html#38-comments-and-docstrings) (with a few tweaks to help with Sphinx generation of documentation pages). Use the docstrings throughout the codebase as a guide.
```

### Comparing `herald-of-completion-0.2.1/setup.cfg` & `herald-of-completion-0.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `herald-of-completion-0.2.1/src/herald/decorators.py` & `herald-of-completion-0.3.0/src/herald/decorators.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,79 +14,83 @@
    def my_function():
        pass
 """
 import traceback
 from functools import wraps
 from typing import Any, Callable, List, Union
 
-from dotenv import dotenv_values
-
-from .types import Messenger, TaskInfo
-
-# NOTE: observer pattern?
-# TODO: add notes on using messengers directly, without a decorator
-# TODO: allow customizable messages for each messenger
+from .types import Messenger, Secrets, TaskInfo
+from .utils import load_secrets
 
 
 class Herald:
     """Class for creating a decorator instance.
 
     This class is used to set up the decorator with the .env file. \
     The resulting decorator can be used to decorate long-running functions.
 
     Args:
-        secrets: Dictionary containing the secrets from the .env file.
+        secrets: Secrets object containing the secrets from the .env file.
     """
 
-    def __init__(self, secrets: str = ".env"):
+    def __init__(self, env: str = ".env"):
         """Initializes the instance with the .env file.
 
         Args:
-            secrets: String containing the path to the .env file.
+            env: String containing the path to the .env file.
         """
-        self.secrets: dict = dotenv_values(secrets)
+        self.secrets: Secrets = load_secrets(env)
 
     def __call__(
-        self, messengers: Union[Messenger, List[Messenger]], send_result: bool = True
+        self,
+        messengers: Union[Messenger, List[Messenger]],
+        message: Union[str, None] = None,
+        send_result: bool = True,
+        send_function: bool = True,
+        send_args: bool = True,
     ) -> Callable:
         """Creates a decorator instance with the given messengers.
 
         Args:
             messengers: Messenger, or list of Messenger, to send the messages.
+            message: String containing a custom message to send.
             send_result: Boolean indicating whether to send the result of the function.
+            send_function: Boolean indicating whether to send the name of the original \
+            calling function.
+            send_args: Boolean indicating whether to send the args and kwargs that \
+            were passed to the function.
 
         Returns:
             A decorator instance that can be used to wrap functions.
         """
 
         def decorator(func: Callable) -> Callable:
             @wraps(func)
             def wrapper(*args: Any, **kwargs: Any):
                 info = TaskInfo(
                     name=func.__name__,
+                    message=message,
+                    send_result=send_result,
+                    send_function=send_function,
+                    send_args=send_args,
                     header="Herald: Task Status",
+                    args=args,
+                    kwargs=kwargs,
                 )
 
                 try:
                     result = func(*args, **kwargs)
-
-                    info.message = f"Task `{func.__name__}` has finished successfully."
                     info.has_errored = False
-                    if send_result:
-                        info.result = f"```\n{str(result)}\n```"
+                    info.result = str(result)
                     self._notify_messengers(messengers, info)
-
                     return result
                 except Exception as e:
-                    info.message = f"Task `{func.__name__}` has finished with errors."
                     info.has_errored = True
-                    if send_result:
-                        info.result = f"```\n{str(traceback.format_exc())}\n```"
+                    info.result = str(traceback.format_exc())
                     self._notify_messengers(messengers, info)
-
                     raise e
 
             return wrapper
 
         return decorator
 
     def _notify_messengers(
```

### Comparing `herald-of-completion-0.2.1/src/herald/messengers/desktop.py` & `herald-of-completion-0.3.0/src/herald/messengers/desktop.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,41 +15,52 @@
 
    @herald(desktop)
    def my_function():
        pass
 """
 from plyer import notification
 
-from ..types import Messenger, TaskInfo
+from ..types import Messenger, TaskInfo, Secrets
 
 
 class DesktopMessenger(Messenger):
     """A class used to send OS-native desktop notifications."""
 
     def __init__(self):
         """Initializes the DesktopMessenger class."""
         pass
 
-    def set_secrets(self, secrets: dict) -> None:
+    def set_secrets(self, secrets: Secrets) -> None:
         """Sets the secrets for the DesktopMessenger class.
 
         Must be implemented as a result of inheriting from the Messenger class. \
         However, the DesktopMessenger itself does not require any secrets.
 
         Args:
-            secrets: A dictionary of secrets to be used by the messenger.
+            secrets: Secrets to be used by the messenger.
         """
         pass
 
     def notify(self, info: TaskInfo) -> None:
         """Constructs and sends a desktop notification using the function information.
 
         Args:
             info: TaskInfo object containing information about the function. \
             Contents should be used to construct the notification message.
         """
         opts = {
             "title": info.header,
-            "message": info.message,
             "timeout": 10,
         }
-        notification.notify(**opts)
+
+        if info.message:
+            opts["message"] = info.message
+        else:
+            if info.has_errored:
+                opts["message"] = f"Task `{info.name}` failed with an error."
+            else:
+                opts["message"] = f"Task `{info.name}` finished successfully."
+
+        try:
+            notification.notify(**opts)
+        except Exception as e:
+            raise e
```

### Comparing `herald-of-completion-0.2.1/src/herald_of_completion.egg-info/SOURCES.txt` & `herald-of-completion-0.3.0/src/herald_of_completion.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 src/herald/__init__.py
 src/herald/decorators.py
 src/herald/types.py
+src/herald/utils.py
 src/herald/messengers/__init__.py
 src/herald/messengers/desktop.py
 src/herald/messengers/discord.py
 src/herald/messengers/email.py
 src/herald_of_completion.egg-info/PKG-INFO
 src/herald_of_completion.egg-info/SOURCES.txt
 src/herald_of_completion.egg-info/dependency_links.txt
 src/herald_of_completion.egg-info/requires.txt
 src/herald_of_completion.egg-info/top_level.txt
+tests/test_arg_types.py
 tests/test_herald.py
-tests/test_messenger.py
+tests/test_messenger.py
+tests/test_utils.py
```

### Comparing `herald-of-completion-0.2.1/tests/test_herald.py` & `herald-of-completion-0.3.0/tests/test_herald.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pytest
 
 from herald.decorators import Herald
-from herald.types import Messenger
+from herald.types import Messenger, Secrets
 
-herald = Herald(secrets="tests/test.env")
+herald = Herald(env="tests/test.env")
 
 
 class DummyMessenger(Messenger):
     def __init__(self):
         self.secrets = None
 
     def set_secrets(self, secrets) -> None:
@@ -33,15 +33,15 @@
         return x[len(x) + 1]
 
     with pytest.raises(IndexError):
         get_item()
 
 
 def test_secrets_are_loaded():
-    assert isinstance(herald.secrets, dict)
+    assert isinstance(herald.secrets, Secrets)
 
 
 def test_messenger_secrets_are_set():
     test_messenger = DummyMessenger()
     herald._set_messenger_secrets(test_messenger)
     assert test_messenger.secrets is not None
-    assert len(test_messenger.secrets) > 0
+    assert test_messenger.secrets == herald.secrets
```

