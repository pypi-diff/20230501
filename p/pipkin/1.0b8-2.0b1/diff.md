# Comparing `tmp/pipkin-1.0b8.tar.gz` & `tmp/pipkin-2.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipkin-1.0b8.tar", last modified: Sat Jan 14 19:15:33 2023, max compression
+gzip compressed data, was "pipkin-2.0b1.tar", last modified: Mon May  1 05:02:01 2023, max compression
```

## Comparing `pipkin-1.0b8.tar` & `pipkin-2.0b1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-01-14 19:15:33.605021 pipkin-1.0b8/
--rw-rw-rw-   0        0        0     1070 2023-01-01 17:36:20.000000 pipkin-1.0b8/LICENSE
--rw-rw-rw-   0        0        0       25 2022-02-28 07:29:10.000000 pipkin-1.0b8/MANIFEST.in
--rw-rw-rw-   0        0        0    10908 2023-01-14 19:15:33.605021 pipkin-1.0b8/PKG-INFO
--rw-rw-rw-   0        0        0     9404 2022-08-14 16:11:16.000000 pipkin-1.0b8/README.rst
-drwxrwxrwx   0        0        0        0 2023-01-14 19:15:33.589394 pipkin-1.0b8/pipkin/
--rw-rw-rw-   0        0        0     1738 2023-01-14 19:14:55.000000 pipkin-1.0b8/pipkin/__init__.py
--rw-rw-rw-   0        0        0     2137 2022-03-19 10:59:37.000000 pipkin-1.0b8/pipkin/__main__.py
--rw-rw-rw-   0        0        0    16912 2022-12-27 13:41:27.000000 pipkin-1.0b8/pipkin/adapters.py
--rw-rw-rw-   0        0        0    33595 2022-12-27 13:41:27.000000 pipkin-1.0b8/pipkin/bare_metal.py
--rw-rw-rw-   0        0        0      355 2022-03-19 10:59:37.000000 pipkin-1.0b8/pipkin/common.py
--rw-rw-rw-   0        0        0     6235 2022-08-14 16:11:16.000000 pipkin-1.0b8/pipkin/connection.py
--rw-rw-rw-   0        0        0    10546 2022-03-19 10:59:37.000000 pipkin-1.0b8/pipkin/parser.py
--rw-rw-rw-   0        0        0    18969 2022-10-30 15:51:33.000000 pipkin-1.0b8/pipkin/proxy.py
--rw-rw-rw-   0        0        0     6599 2022-12-28 09:16:11.000000 pipkin-1.0b8/pipkin/serial_connection.py
--rw-rw-rw-   0        0        0    27822 2023-01-01 17:14:54.000000 pipkin-1.0b8/pipkin/session.py
--rw-rw-rw-   0        0        0     6702 2022-10-30 15:51:33.000000 pipkin-1.0b8/pipkin/util.py
--rw-rw-rw-   0        0        0     4580 2022-08-14 16:11:16.000000 pipkin-1.0b8/pipkin/webrepl_connection.py
-drwxrwxrwx   0        0        0        0 2023-01-14 19:15:33.605021 pipkin-1.0b8/pipkin.egg-info/
--rw-rw-rw-   0        0        0    10908 2023-01-14 19:15:33.000000 pipkin-1.0b8/pipkin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      492 2023-01-14 19:15:33.000000 pipkin-1.0b8/pipkin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-14 19:15:33.000000 pipkin-1.0b8/pipkin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-01-14 19:15:33.000000 pipkin-1.0b8/pipkin.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       36 2023-01-14 19:15:33.000000 pipkin-1.0b8/pipkin.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-01-14 19:15:33.000000 pipkin-1.0b8/pipkin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      155 2022-02-28 07:29:10.000000 pipkin-1.0b8/pyproject.toml
--rw-rw-rw-   0        0        0       36 2022-10-22 13:56:00.000000 pipkin-1.0b8/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-01-14 19:15:33.605021 pipkin-1.0b8/setup.cfg
--rw-rw-rw-   0        0        0     2105 2022-02-28 07:29:10.000000 pipkin-1.0b8/setup.py
+drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-05-01 05:02:01.486686 pipkin-2.0b1/
+-rw-r--r--   0 aivarannamaa   (502) staff       (20)     1070 2023-04-27 17:16:03.000000 pipkin-2.0b1/LICENSE
+-rw-r--r--   0 aivarannamaa   (502) staff       (20)       25 2023-04-27 17:16:03.000000 pipkin-2.0b1/MANIFEST.in
+-rw-r--r--   0 aivarannamaa   (502) staff       (20)    10700 2023-05-01 05:02:01.486524 pipkin-2.0b1/PKG-INFO
+-rw-r--r--   0 aivarannamaa   (502) staff       (20)     9404 2023-04-27 17:16:03.000000 pipkin-2.0b1/README.rst
+drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-05-01 05:02:01.482029 pipkin-2.0b1/pipkin/
+-rw-r--r--   0 aivarannamaa   (502) staff       (20)     1738 2023-05-01 04:58:42.000000 pipkin-2.0b1/pipkin/__init__.py
+-rw-r--r--   0 aivarannamaa   (502) staff       (20)     2114 2023-04-27 17:16:03.000000 pipkin-2.0b1/pipkin/__main__.py
+-rw-r--r--   0 aivarannamaa   (502) staff       (20)    16912 2023-04-30 17:06:48.000000 pipkin-2.0b1/pipkin/adapters.py
+-rw-r--r--   0 aivarannamaa   (502) staff       (20)    33592 2023-04-30 06:24:37.000000 pipkin-2.0b1/pipkin/bare_metal.py
+-rw-r--r--   0 aivarannamaa   (502) staff       (20)      355 2023-04-27 17:16:03.000000 pipkin-2.0b1/pipkin/common.py
+-rw-r--r--   0 aivarannamaa   (502) staff       (20)     6242 2023-04-30 06:23:56.000000 pipkin-2.0b1/pipkin/connection.py
+-rw-r--r--   0 aivarannamaa   (502) staff       (20)    10546 2023-04-27 17:16:03.000000 pipkin-2.0b1/pipkin/parser.py
+-rw-r--r--   0 aivarannamaa   (502) staff       (20)    23522 2023-04-30 07:11:11.000000 pipkin-2.0b1/pipkin/proxy.py
+-rw-r--r--   0 aivarannamaa   (502) staff       (20)     6597 2023-04-30 06:10:39.000000 pipkin-2.0b1/pipkin/serial_connection.py
+-rw-r--r--   0 aivarannamaa   (502) staff       (20)    27819 2023-04-30 06:10:39.000000 pipkin-2.0b1/pipkin/session.py
+-rw-r--r--   0 aivarannamaa   (502) staff       (20)     7156 2023-04-30 08:11:24.000000 pipkin-2.0b1/pipkin/util.py
+-rw-r--r--   0 aivarannamaa   (502) staff       (20)     4600 2023-04-30 06:25:03.000000 pipkin-2.0b1/pipkin/webrepl_connection.py
+drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-05-01 05:02:01.486312 pipkin-2.0b1/pipkin.egg-info/
+-rw-r--r--   0 aivarannamaa   (502) staff       (20)    10700 2023-05-01 05:02:01.000000 pipkin-2.0b1/pipkin.egg-info/PKG-INFO
+-rw-r--r--   0 aivarannamaa   (502) staff       (20)      492 2023-05-01 05:02:01.000000 pipkin-2.0b1/pipkin.egg-info/SOURCES.txt
+-rw-r--r--   0 aivarannamaa   (502) staff       (20)        1 2023-05-01 05:02:01.000000 pipkin-2.0b1/pipkin.egg-info/dependency_links.txt
+-rw-r--r--   0 aivarannamaa   (502) staff       (20)       39 2023-05-01 05:02:01.000000 pipkin-2.0b1/pipkin.egg-info/entry_points.txt
+-rw-r--r--   0 aivarannamaa   (502) staff       (20)       34 2023-05-01 05:02:01.000000 pipkin-2.0b1/pipkin.egg-info/requires.txt
+-rw-r--r--   0 aivarannamaa   (502) staff       (20)        7 2023-05-01 05:02:01.000000 pipkin-2.0b1/pipkin.egg-info/top_level.txt
+-rw-r--r--   0 aivarannamaa   (502) staff       (20)      155 2023-04-27 17:16:03.000000 pipkin-2.0b1/pyproject.toml
+-rw-r--r--   0 aivarannamaa   (502) staff       (20)       34 2023-05-01 05:01:05.000000 pipkin-2.0b1/requirements.txt
+-rw-r--r--   0 aivarannamaa   (502) staff       (20)       38 2023-05-01 05:02:01.486732 pipkin-2.0b1/setup.cfg
+-rw-r--r--   0 aivarannamaa   (502) staff       (20)     2105 2023-04-27 17:16:03.000000 pipkin-2.0b1/setup.py
```

### Comparing `pipkin-1.0b8/LICENSE` & `pipkin-2.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `pipkin-1.0b8/PKG-INFO` & `pipkin-2.0b1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,206 +1,204 @@
-Metadata-Version: 2.1
-Name: pipkin
-Version: 1.0b8
-Summary: Tool for installing packages for MicroPython and CircuitPython
-Home-page: https://github.com/aivarannamaa/pipkin
-Author: Aivar Annamaa
-License: MIT
-Project-URL: Source code, https://github.com/aivarannamaa/pipkin
-Project-URL: Bug tracker, https://github.com/aivarannamaa/pipkin/issues
-Keywords: MicroPython CircuitPython pip upip
-Platform: Windows
-Platform: macOS
-Platform: Linux
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: License :: Freeware
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development
-Requires-Python: >=3.7
-License-File: LICENSE
-
-pipkin
-=======
-Tool for managing distribution packages for MicroPython and CircuitPython on target devices or in a local directory.
-
-Supports both `upip-compatible packages <https://docs.micropython.org/en/latest/reference/packages.html>`_,
-and regular pip-compatible packages.
-
-By default it prefers packages at micropython.org-s index. If the package or the required version is not
-found there, then it turns to PyPI.
-
-Unlike some of the package managers for MicroPython and CircuitPython, pipkin keeps a minimal set of package
-metadata (trimmed .dist-info/METADATA and .dist-info/RECORD) next to the package itself, just like pip.
-This enables straigthforward approach for uninstalling, listing and freezing.
-
-When installing with ``--compile`` switch, pipkin uses suitable `mpy-cross` to compile the
-py-files on the fly and transfers resulting mpy-files to the target.
-
-Installation
---------------
-``pip install pipkin``
-
-Usage
------
-
-The basic structure of the command line is ``pipkin <target selection> <command> <command arguments>``.
-For example:
-
-* ``pipkin --port /dev/ttyACM0 install micropython-logging``
-* ``pipkin --mount G:\lib install adafruit-circuitpython-ssd1306``
-* ``pipkin --mount G:\lib install --compile adafruit-circuitpython-ssd1306``
-* ``pipkin --dir my_project/lib install micropython-logging micropython-oled``
-* ``pipkin --port COM5 uninstall micropython-logging micropython-oled``
-* ``pipkin --port COM5 list --outdated``
-
-If you have attached a single CircuitPython device (with its filesystem mounted as a disk) or
-a single well known MicroPython device (eg. Raspberry Pi Pico), then you can omit the target selection
-part:
-
-* ``pipkin install adafruit-circuitpython-ssd1306``
-
-pipkin -h
-----------
-
-::
-
-    usage: pipkin [-h] [-V] [-v | -q] [-p <port> | -m <path> | -d <path>] {install,uninstall,list,show,freeze,check,download,wheel,cache} ...
-
-    Tool for managing MicroPython and CircuitPython packages
-
-    general:
-      -h, --help            Show this help message and exit
-      -V, --version         Show program version and exit
-      -v, --verbose         Show more details about the process
-      -q, --quiet           Don't show non-error output
-
-    target selection (pick one or let pipkin autodetect the port or mount):
-      -p <port>, --port <port>
-                            Serial port of the target device
-      -m <path>, --mount <path>
-                            Mount point (volume, disk, drive) of the target device
-      -d <path>, --dir <path>
-                            Directory in the local filesystem
-
-    commands:
-      Use "pipkin <command> -h" for usage help of a command
-
-      {install,uninstall,list,show,freeze,check,download,wheel,cache}
-        install             Install packages.
-        uninstall           Uninstall packages.
-        list                List installed packages.
-        show                Show information about one or more installed packages.
-        freeze              Output installed packages in requirements format.
-        check               Verify installed packages have compatible dependencies.
-        download            Download packages.
-        wheel               Build Wheel archives for your requirements and dependencies.
-        cache               Inspect and manage pipkin cache.
-
-pipkin install -h
-------------------
-
-::
-
-    usage: pipkin install [-h] [-r [<file> [<file> ...]]] [-c [<file> [<file> ...]]] [--no-deps] [--pre] [-i <url>] [--extra-index-url [<url> [<url> ...]]]
-                               [--no-index] [--no-mp-org] [-f <url|file|dir>] [-U] [--upgrade-strategy <upgrade_strategy>] [--force-reinstall] [--compile]
-                               [<spec> [<spec> ...]]
-
-    Installs upip or pip compatible distribution packages onto a MicroPython/CircuitPython device or into a local directory.
-
-    positional arguments:
-      <spec>                Package specification, eg. 'micropython-os' or 'micropython-os>=0.6'
-
-    optional arguments:
-      -h, --help            show this help message and exit
-      -U, --upgrade         Upgrade all specified packages to the newest available version. The handling of dependencies depends on the upgrade-strategy used.
-      --upgrade-strategy <upgrade_strategy>
-                            Determines how dependency upgrading should be handled [default: only-if-needed]. 'eager' - dependencies are upgraded regardless of
-                            whether the currently installed version satisfies the requirements of the upgraded package(s). 'only-if-needed' - are upgraded only when
-                            they do not satisfy the requirements of the upgraded package(s).
-      --force-reinstall     Reinstall all packages even if they are already up-to-date.
-      --compile             Compile and install mpy files.
-
-    package selection:
-      -r [<file> [<file> ...]], --requirement [<file> [<file> ...]]
-                            Install from the given requirements file.
-      -c [<file> [<file> ...]], --constraint [<file> [<file> ...]]
-                            Constrain versions using the given constraints file.
-      --no-deps             Don't install package dependencies.
-      --pre                 Include pre-release and development versions. By default, pipkin only finds stable versions.
-
-    index selection:
-      -i <url>, --index-url <url>
-                            Base URL of the Python Package Index (default https://pypi.org/simple).
-      --extra-index-url [<url> [<url> ...]]
-                            Extra URLs of package indexes to use in addition to --index-url.
-      --no-index            Ignore package index (only looking at --find-links URLs instead).
-      --no-mp-org           Don't let micropython.org/pi override other indexes.
-      -f <url|file|dir>, --find-links <url|file|dir>
-                            If a URL or path to an html file, then parse for links to archives such as sdist (.tar.gz) or wheel (.whl) files. If a local path or
-                            file:// URL that's a directory, then look for archives in the directory listing.
-
-Adafruit-Blinka and co
-----------------------
-`Adafruit-Blinka <https://pypi.org/project/Adafruit-Blinka/>`_ is a compatibility library which allows
-running CircuitPython code with CPython. When publishing CircuitPython libraries at PyPI, Adafruit
-and the community have so far targeted only CPython users, because tools for connecting PyPI with bare metal
-CircuitPython did not exist (or because at the moment it is not clear how to publish wheels for Pythons
-which can't run pip themselves). Therefore the CircuitPython libraries at PyPI usually have Adafruit-Blinka
-dependency, which is not relevant (and would even cause problems) on bare metal CircuitPython devices.
-
-pipkin's current approach is to have its proxy-index return dummy Adafruit-Blinka distribution, which contains
-no modules and has no dependencies. This means when you're installing a library which depends on Adafruit-Blinka,
-you'll get Blinka's .dist-info directory with METADATA and RECORD, but nothing else. Let's call it
-an optimized build.
-
-Dummies are returned for all dists, which are currently omitted by
-`adafruit/circuitpython-build-tools <https://github.com/adafruit/circuitpython-build-tools/blob/de44a709f6287d2759df14c89707f2d8f5a026f5/circuitpython_build_tools/scripts/build_bundles.py#L42>`_
-
-Current state and goals
------------------------
-Handling packages meant for upip, micropython.org/pi overrides and the problems outlined in the
-previous section, all together make pipkin less elegant and slower than one would like. Still, this is just
-a start. There are several optimizations possible within current approach. Also, PyPI, pip, wheel
-and packaging standards are evolving -- in the future it may become easy to publish separate wheels
-for MicroPython and/or CircuitPython and pip may become usable for "cross-installing" packages for
-other platforms.
-
-Even if clumsy at times, pipkin tries to be the proof-of-concept for demonstrating that even in
-the world of MicroPython and CircuitPython, we could continue publishing standard sdists
-and wheels on PyPI and re-use the familiar approach for package management. While introducing
-new formats and distribution mechanisms have their benefits, we shouldn't dismiss the standard approach
-yet.
-
-Implementation
---------------
-pipkin delegates most of its work to our old friend pip. This is the reason it is able to offer
-so much functionality.
-
-Both upip-compatibility and support for micropython.org-s
-index is achieved by using up a temporary local index, which proxies both PyPI (or another specified index)
-and micropython.org/pi and restores missing setup.py for upip-compatible packages.
-
-Non-CPython installation target is achieved by creating and maintaining private working environment (venv).
-(As creating a venv can be slow in Windows, be prepared for longer wait when using pipkin for the first time.)
-
-In the beginning of the session, pipkin collects package metadata from the target (eg. from the /lib directory
-of the device connected over serial) and creates corresponding dummy packages in the working environment.
-Then it starts the temporary local index and invokes venv-s pip aginst it. When pip finishes, it detects the
-distributions which are removed, added or changed and applies corresponding changes to the target device or
-directory.
-
-
-
+Metadata-Version: 2.1
+Name: pipkin
+Version: 2.0b1
+Summary: Tool for installing packages for MicroPython and CircuitPython
+Home-page: https://github.com/aivarannamaa/pipkin
+Author: Aivar Annamaa
+License: MIT
+Project-URL: Source code, https://github.com/aivarannamaa/pipkin
+Project-URL: Bug tracker, https://github.com/aivarannamaa/pipkin/issues
+Keywords: MicroPython CircuitPython pip upip
+Platform: Windows
+Platform: macOS
+Platform: Linux
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: Freeware
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Software Development
+Requires-Python: >=3.7
+License-File: LICENSE
+
+pipkin
+=======
+Tool for managing distribution packages for MicroPython and CircuitPython on target devices or in a local directory.
+
+Supports both `upip-compatible packages <https://docs.micropython.org/en/latest/reference/packages.html>`_,
+and regular pip-compatible packages.
+
+By default it prefers packages at micropython.org-s index. If the package or the required version is not
+found there, then it turns to PyPI.
+
+Unlike some of the package managers for MicroPython and CircuitPython, pipkin keeps a minimal set of package
+metadata (trimmed .dist-info/METADATA and .dist-info/RECORD) next to the package itself, just like pip.
+This enables straigthforward approach for uninstalling, listing and freezing.
+
+When installing with ``--compile`` switch, pipkin uses suitable `mpy-cross` to compile the
+py-files on the fly and transfers resulting mpy-files to the target.
+
+Installation
+--------------
+``pip install pipkin``
+
+Usage
+-----
+
+The basic structure of the command line is ``pipkin <target selection> <command> <command arguments>``.
+For example:
+
+* ``pipkin --port /dev/ttyACM0 install micropython-logging``
+* ``pipkin --mount G:\lib install adafruit-circuitpython-ssd1306``
+* ``pipkin --mount G:\lib install --compile adafruit-circuitpython-ssd1306``
+* ``pipkin --dir my_project/lib install micropython-logging micropython-oled``
+* ``pipkin --port COM5 uninstall micropython-logging micropython-oled``
+* ``pipkin --port COM5 list --outdated``
+
+If you have attached a single CircuitPython device (with its filesystem mounted as a disk) or
+a single well known MicroPython device (eg. Raspberry Pi Pico), then you can omit the target selection
+part:
+
+* ``pipkin install adafruit-circuitpython-ssd1306``
+
+pipkin -h
+----------
+
+::
+
+    usage: pipkin [-h] [-V] [-v | -q] [-p <port> | -m <path> | -d <path>] {install,uninstall,list,show,freeze,check,download,wheel,cache} ...
+
+    Tool for managing MicroPython and CircuitPython packages
+
+    general:
+      -h, --help            Show this help message and exit
+      -V, --version         Show program version and exit
+      -v, --verbose         Show more details about the process
+      -q, --quiet           Don't show non-error output
+
+    target selection (pick one or let pipkin autodetect the port or mount):
+      -p <port>, --port <port>
+                            Serial port of the target device
+      -m <path>, --mount <path>
+                            Mount point (volume, disk, drive) of the target device
+      -d <path>, --dir <path>
+                            Directory in the local filesystem
+
+    commands:
+      Use "pipkin <command> -h" for usage help of a command
+
+      {install,uninstall,list,show,freeze,check,download,wheel,cache}
+        install             Install packages.
+        uninstall           Uninstall packages.
+        list                List installed packages.
+        show                Show information about one or more installed packages.
+        freeze              Output installed packages in requirements format.
+        check               Verify installed packages have compatible dependencies.
+        download            Download packages.
+        wheel               Build Wheel archives for your requirements and dependencies.
+        cache               Inspect and manage pipkin cache.
+
+pipkin install -h
+------------------
+
+::
+
+    usage: pipkin install [-h] [-r [<file> [<file> ...]]] [-c [<file> [<file> ...]]] [--no-deps] [--pre] [-i <url>] [--extra-index-url [<url> [<url> ...]]]
+                               [--no-index] [--no-mp-org] [-f <url|file|dir>] [-U] [--upgrade-strategy <upgrade_strategy>] [--force-reinstall] [--compile]
+                               [<spec> [<spec> ...]]
+
+    Installs upip or pip compatible distribution packages onto a MicroPython/CircuitPython device or into a local directory.
+
+    positional arguments:
+      <spec>                Package specification, eg. 'micropython-os' or 'micropython-os>=0.6'
+
+    optional arguments:
+      -h, --help            show this help message and exit
+      -U, --upgrade         Upgrade all specified packages to the newest available version. The handling of dependencies depends on the upgrade-strategy used.
+      --upgrade-strategy <upgrade_strategy>
+                            Determines how dependency upgrading should be handled [default: only-if-needed]. 'eager' - dependencies are upgraded regardless of
+                            whether the currently installed version satisfies the requirements of the upgraded package(s). 'only-if-needed' - are upgraded only when
+                            they do not satisfy the requirements of the upgraded package(s).
+      --force-reinstall     Reinstall all packages even if they are already up-to-date.
+      --compile             Compile and install mpy files.
+
+    package selection:
+      -r [<file> [<file> ...]], --requirement [<file> [<file> ...]]
+                            Install from the given requirements file.
+      -c [<file> [<file> ...]], --constraint [<file> [<file> ...]]
+                            Constrain versions using the given constraints file.
+      --no-deps             Don't install package dependencies.
+      --pre                 Include pre-release and development versions. By default, pipkin only finds stable versions.
+
+    index selection:
+      -i <url>, --index-url <url>
+                            Base URL of the Python Package Index (default https://pypi.org/simple).
+      --extra-index-url [<url> [<url> ...]]
+                            Extra URLs of package indexes to use in addition to --index-url.
+      --no-index            Ignore package index (only looking at --find-links URLs instead).
+      --no-mp-org           Don't let micropython.org/pi override other indexes.
+      -f <url|file|dir>, --find-links <url|file|dir>
+                            If a URL or path to an html file, then parse for links to archives such as sdist (.tar.gz) or wheel (.whl) files. If a local path or
+                            file:// URL that's a directory, then look for archives in the directory listing.
+
+Adafruit-Blinka and co
+----------------------
+`Adafruit-Blinka <https://pypi.org/project/Adafruit-Blinka/>`_ is a compatibility library which allows
+running CircuitPython code with CPython. When publishing CircuitPython libraries at PyPI, Adafruit
+and the community have so far targeted only CPython users, because tools for connecting PyPI with bare metal
+CircuitPython did not exist (or because at the moment it is not clear how to publish wheels for Pythons
+which can't run pip themselves). Therefore the CircuitPython libraries at PyPI usually have Adafruit-Blinka
+dependency, which is not relevant (and would even cause problems) on bare metal CircuitPython devices.
+
+pipkin's current approach is to have its proxy-index return dummy Adafruit-Blinka distribution, which contains
+no modules and has no dependencies. This means when you're installing a library which depends on Adafruit-Blinka,
+you'll get Blinka's .dist-info directory with METADATA and RECORD, but nothing else. Let's call it
+an optimized build.
+
+Dummies are returned for all dists, which are currently omitted by
+`adafruit/circuitpython-build-tools <https://github.com/adafruit/circuitpython-build-tools/blob/de44a709f6287d2759df14c89707f2d8f5a026f5/circuitpython_build_tools/scripts/build_bundles.py#L42>`_
+
+Current state and goals
+-----------------------
+Handling packages meant for upip, micropython.org/pi overrides and the problems outlined in the
+previous section, all together make pipkin less elegant and slower than one would like. Still, this is just
+a start. There are several optimizations possible within current approach. Also, PyPI, pip, wheel
+and packaging standards are evolving -- in the future it may become easy to publish separate wheels
+for MicroPython and/or CircuitPython and pip may become usable for "cross-installing" packages for
+other platforms.
+
+Even if clumsy at times, pipkin tries to be the proof-of-concept for demonstrating that even in
+the world of MicroPython and CircuitPython, we could continue publishing standard sdists
+and wheels on PyPI and re-use the familiar approach for package management. While introducing
+new formats and distribution mechanisms have their benefits, we shouldn't dismiss the standard approach
+yet.
+
+Implementation
+--------------
+pipkin delegates most of its work to our old friend pip. This is the reason it is able to offer
+so much functionality.
+
+Both upip-compatibility and support for micropython.org-s
+index is achieved by using up a temporary local index, which proxies both PyPI (or another specified index)
+and micropython.org/pi and restores missing setup.py for upip-compatible packages.
+
+Non-CPython installation target is achieved by creating and maintaining private working environment (venv).
+(As creating a venv can be slow in Windows, be prepared for longer wait when using pipkin for the first time.)
+
+In the beginning of the session, pipkin collects package metadata from the target (eg. from the /lib directory
+of the device connected over serial) and creates corresponding dummy packages in the working environment.
+Then it starts the temporary local index and invokes venv-s pip aginst it. When pip finishes, it detects the
+distributions which are removed, added or changed and applies corresponding changes to the target device or
+directory.
+
```

### Comparing `pipkin-1.0b8/README.rst` & `pipkin-2.0b1/README.rst`

 * *Files identical despite different names*

### Comparing `pipkin-1.0b8/pipkin/__init__.py` & `pipkin-2.0b1/pipkin/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from pipkin.adapters import Adapter, DummyAdapter, create_adapter
 from pipkin.common import ManagementError, UserError
 from pipkin.session import Session
 
 logger = logging.getLogger("pipkin")
 
-__version__ = "1.0b8"
+__version__ = "2.0b1"
 
 
 def error(msg):
     msg = "ERROR: " + msg
     print(msg, file=sys.stderr)
 
     return 1
```

### Comparing `pipkin-1.0b8/pipkin/__main__.py` & `pipkin-2.0b1/pipkin/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python3
 """
 MIT License
 
 Copyright (c) 2022 Aivar Annamaa
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pipkin-1.0b8/pipkin/adapters.py` & `pipkin-2.0b1/pipkin/adapters.py`

 * *Files 0% similar despite different names*

```diff
@@ -456,15 +456,15 @@
 
     def fetch_sys_path(self) -> List[str]:
         # This means, list command without --path will consider this directory
         return ["/"]
 
     def fetch_sys_implementation(self) -> Tuple[str, str, int]:
         # TODO:
-        return ("micropython", "1.18", 0)
+        return ("micropython", "1.20", 0)
 
     def get_default_target(self) -> str:
         return "/"
 
 
 def create_adapter(port: Optional[str], mount: Optional[str], dir: Optional[str], **kw) -> Adapter:
     if port:
```

### Comparing `pipkin-1.0b8/pipkin/bare_metal.py` & `pipkin-2.0b1/pipkin/bare_metal.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,14 @@
 
     def _infer_submit_parameters(
         self,
         submit_mode: Optional[str] = None,
         write_block_size: Optional[int] = None,
         write_block_delay: Optional[float] = None,
     ) -> Tuple[str, int, float]:
-
         if submit_mode is None:
             submit_mode = RAW_PASTE_SUBMIT_MODE
 
         if write_block_size is None:
             write_block_size = 255
 
         if write_block_delay is None:
@@ -190,15 +189,14 @@
     def fetch_sys_implementation(self) -> Tuple[str, str, int]:
         return self._evaluate("__pipkin_helper.builtins.tuple(__pipkin_helper.sys.implementation)")
 
     def get_user_packages_path(self) -> Optional[str]:
         return None
 
     def read_file(self, path: str) -> bytes:
-
         hex_mode = self._should_hexlify(path)
 
         open_script = f"__pipkin_fp = __pipkin_helper.builtins.open({path!r}, 'rb')"
         out, err = self._execute_and_capture_output(open_script)
 
         if (out + err).strip():
             if any(str(nr) in out + err for nr in [errno.ENOENT, errno.ENODEV]):
@@ -494,15 +492,15 @@
         if self._last_prompt == NORMAL_PROMPT and not force:
             return
 
         logger.debug("requesting normal mode at %r", self._last_prompt)
         self._write(NORMAL_MODE_CMD)
         self._log_output_until_active_prompt()
         assert self._last_prompt == NORMAL_PROMPT, (
-            "Could not get normal prompt, got %s" % self._last_prompt
+            "Could not get normal prompt, got %r" % self._last_prompt
         )
 
     def _log_output_until_active_prompt(self, timeout: float = WAIT_OR_CRASH_TIMEOUT) -> None:
         def collect_output(data, stream):
             if data:
                 logger.info("Discarding %s: %r", stream, data)
 
@@ -519,15 +517,14 @@
         return output["stdout"], output["stderr"]
 
     def _process_output_until_active_prompt(
         self,
         output_consumer: OutputConsumer,
         timeout: float,
     ):
-
         PROMPT_MARKERS = [NORMAL_PROMPT, EOT + RAW_PROMPT, FIRST_RAW_PROMPT]
         PROMPT_MARKERS_RE = re.compile(
             b"|".join(
                 map(
                     re.escape,
                     PROMPT_MARKERS,
                 )
```

### Comparing `pipkin-1.0b8/pipkin/connection.py` & `pipkin-2.0b1/pipkin/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     unread data).
 
     Allows unreading data.
     """
 
     def __init__(self):
         self.encoding = "utf-8"
-        self._read_queue = Queue()  # populated by reader thread
+        self._read_queue: Queue = Queue()  # populated by reader thread
         self._read_buffer = bytearray()  # used for unreading and postponing bytes
         self.num_bytes_received = 0
         self.startup_time = time.time()
         self.text_mode = True
         self._error = None
         self._reader_stopped = False
```

### Comparing `pipkin-1.0b8/pipkin/parser.py` & `pipkin-2.0b1/pipkin/parser.py`

 * *Files identical despite different names*

### Comparing `pipkin-1.0b8/pipkin/proxy.py` & `pipkin-2.0b1/pipkin/proxy.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python3
 """
 MIT License
 
 Copyright (c) 2022 Aivar Annamaa
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
@@ -21,35 +20,46 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 import copy
 import email.parser
 import errno
+import hashlib
 import io
 import json
 import logging
 import os.path
 import shlex
+import socket
 import subprocess
 import sys
 import tarfile
 import tempfile
+import textwrap
 import threading
+import zipfile
+from abc import ABC
 from html.parser import HTMLParser
 from http.server import BaseHTTPRequestHandler, HTTPServer
 from socketserver import BaseServer
 from textwrap import dedent
-from typing import Dict, List, Optional, Tuple
+from typing import Any, Dict, List, Optional, Tuple, Union
 from urllib.error import HTTPError
 from urllib.request import urlopen
 
-from pipkin.util import normalize_dist_name, parse_dist_file_name
+from pkg_resources import safe_name, safe_version
 
-MP_ORG_INDEX = "https://micropython.org/pi"
+from pipkin.util import (
+    create_dist_info_version_name,
+    custom_normalize_dist_name,
+    parse_dist_file_name,
+)
+
+MP_ORG_INDEX_V2 = "https://micropython.org/pi/v2"
 PYPI_SIMPLE_INDEX = "https://pypi.org/simple"
 SERVER_ENCODING = "utf-8"
 
 # https://github.com/adafruit/circuitpython-build-tools/blob/de44a709f6287d2759df14c89707f2d8f5a026f5/circuitpython_build_tools/scripts/build_bundles.py#L42
 NORMALIZED_IRRELEVANT_PACKAGE_NAMES = {
     "adafruit_blinka",
     "adafruit_blinka_bleio",
@@ -94,30 +104,45 @@
                 if att == "href":
                     self.file_urls[data] = val
 
     def handle_endtag(self, tag):
         pass
 
 
-class BaseIndexDownloader:
+class BaseIndexDownloader(ABC):
     def __init__(self, index_url: str):
         self._index_url = index_url.rstrip("/")
-        self._file_urls_cache: Dict[str, Dict[str, str]] = {}
-
-    def get_file_urls(self, dist_name: str) -> Dict[str, str]:
-        if dist_name not in self._file_urls_cache:
-            self._file_urls_cache[dist_name] = self._download_file_urls(dist_name)
 
-        return self._file_urls_cache[dist_name]
+    def get_dist_file_names(self, dist_name: str) -> Optional[List[str]]:
+        raise NotImplementedError()
 
-    def _download_file_urls(self, dist_name) -> Optional[Dict[str, str]]:
+    def get_file_content(self, dist_name: str, file_name: str) -> bytes:
         raise NotImplementedError()
 
 
 class SimpleIndexDownloader(BaseIndexDownloader):
+    def __init__(self, index_url: str):
+        super().__init__(index_url)
+        self._dist_urls_cache: Dict[str, Dict[str, str]] = {}
+
+    def get_dist_file_names(self, dist_name: str) -> Optional[List[str]]:
+        urls = self._get_dist_urls(dist_name)
+        if urls is None:
+            return None
+        return list(urls.keys())
+
+    def _get_dist_urls(self, dist_name: str) -> Optional[Dict[str, str]]:
+        """
+        Returns file names and url-s for constructing the dist index page.
+        """
+        if dist_name not in self._dist_urls_cache:
+            self._dist_urls_cache[dist_name] = self._download_file_urls(dist_name)
+
+        return self._dist_urls_cache[dist_name]
+
     def _download_file_urls(self, dist_name) -> Optional[Dict[str, str]]:
         url = f"{self._index_url}/{dist_name}"
         logger.info("Downloading file urls from simple index %s", url)
 
         try:
             with urlopen(url) as fp:
                 parser = SimpleUrlsParser()
@@ -125,163 +150,33 @@
                 return parser.file_urls
         except HTTPError as e:
             if e.code == 404:
                 return None
             else:
                 raise e
 
-
-class JsonIndexDownloader(BaseIndexDownloader):
-    def _download_file_urls(self, dist_name) -> Optional[Dict[str, str]]:
-        metadata_url = f"{self._index_url}/{dist_name}/json"
-        logger.info("Downloading file urls from json index at %s", metadata_url)
-
-        result = {}
-        try:
-            with urlopen(metadata_url) as fp:
-                data = json.load(fp)
-                releases = data["releases"]
-                for ver in releases:
-                    for file in releases[ver]:
-                        file_url = file["url"]
-                        if "filename" in file:
-                            file_name = file["filename"]
-                        else:
-                            # micropython.org/pi doesn't have it
-                            file_name = file_url.split("/")[-1]
-                            # may be missing micropython prefix
-                            if not file_name.startswith(dist_name):
-                                # Let's hope version part doesn't contain dashes
-                                _, suffix = file_name.split("-")
-                                file_name = dist_name + "-" + suffix
-                        result[file_name] = file_url
-        except HTTPError as e:
-            if e.code == 404:
-                return None
-            else:
-                raise e
-        return result
-
-
-class MpOrgIndexDownloader(JsonIndexDownloader):
-    def _download_file_urls(self, dist_name) -> Optional[Dict[str, str]]:
-        if not normalize_dist_name(dist_name).startswith("micropython_"):
-            return None
-
-        return super()._download_file_urls(dist_name)
-
-
-class PipkinProxy(HTTPServer):
-    def __init__(
-        self, no_mp_org: bool, index_url: Optional[str], extra_index_urls: List[str], port: int
-    ):
-        self._downloaders: List[BaseIndexDownloader] = []
-        self._downloaders_by_dist_name: Dict[str, Optional[BaseIndexDownloader]] = {}
-        if not no_mp_org:
-            self._downloaders.append(MpOrgIndexDownloader(MP_ORG_INDEX))
-        self._downloaders.append(SimpleIndexDownloader(index_url or PYPI_SIMPLE_INDEX))
-        for url in extra_index_urls:
-            self._downloaders.append(SimpleIndexDownloader(url))
-        super().__init__(("127.0.0.1", port), PipkinProxyHandler)
-
-    def get_downloader_for_dist(self, dist_name: str) -> Optional[BaseIndexDownloader]:
-        if dist_name not in self._downloaders_by_dist_name:
-            for downloader in self._downloaders:
-                file_urls = downloader.get_file_urls(dist_name)
-                if file_urls is not None:
-                    self._downloaders_by_dist_name[dist_name] = downloader
-                    break
-            else:
-                self._downloaders_by_dist_name[dist_name] = None
-
-        return self._downloaders_by_dist_name[dist_name]
-
-    def get_index_url(self) -> str:
-        return f"http://127.0.0.1:{self.server_port}"
-
-
-class PipkinProxyHandler(BaseHTTPRequestHandler):
-    def __init__(self, request: bytes, client_address: Tuple[str, int], server: BaseServer):
-        logger.debug("Creating new handler")
-        assert isinstance(server, PipkinProxy)
-        self.proxy: PipkinProxy = server
-        super().__init__(request, client_address, server)
-
-    def do_GET(self) -> None:
-        path = self.path.strip("/")
-        logger.debug("do_GET for %s", path)
-        if "/" in path:
-            assert path.count("/") == 1
-            self._serve_file(*path.split("/"))
-        else:
-            self._serve_distribution_page(path)
-
-    def _serve_distribution_page(self, dist_name: str) -> None:
-        logger.debug("Serving index page for %s", dist_name)
-        downloader = self.proxy.get_downloader_for_dist(dist_name)
-        if downloader is None:
-            self.send_response(404)
-            self.end_headers()
-            return
-
-        # TODO: check https://discuss.python.org/t/community-testing-of-packaging-tools-against-non-warehouse-indexes/13442
-
-        file_urls = downloader.get_file_urls(dist_name)
-        # logger.debug("File urls: %r", file_urls)
-        self.send_response(200)
-        self.send_header("Content-type", f"text/html; charset={SERVER_ENCODING}")
-        self.send_header("Cache-Control", "max-age=600, public")
-        self.end_headers()
-        self.wfile.write("<!DOCTYPE html><html><body>\n".encode(SERVER_ENCODING))
-        for file_name in file_urls:
-            self.wfile.write(
-                f"<a href='/{dist_name}/{file_name}/'>{file_name}</a>\n".encode(SERVER_ENCODING)
-            )
-        self.wfile.write("</body></html>".encode(SERVER_ENCODING))
-
-    def _serve_file(self, dist_name: str, file_name: str):
-        logger.debug("Serving %s for %s", file_name, dist_name)
-
+    def get_file_content(self, dist_name: str, file_name: str) -> bytes:
         if self._should_return_dummy(dist_name):
-            tweaked_bytes = create_dummy_dist(dist_name, file_name)
+            return create_dummy_dist(dist_name, file_name)
         else:
             original_bytes = self._download_file(dist_name, file_name)
-            tweaked_bytes = self._tweak_file(dist_name, file_name, original_bytes)
-
-        self.send_response(200)
-        self.send_header("Content-Type", "application/octet-stream")
-        self.send_header("Cache-Control", "max-age=365000000, immutable, public")
-        self.end_headers()
-
-        block_size = 4096
-        for start_index in range(0, len(tweaked_bytes), block_size):
-            block = tweaked_bytes[start_index : start_index + block_size]
-            self.wfile.write(block)
+            return self._tweak_file(dist_name, file_name, original_bytes)
 
     def _download_file(self, dist_name: str, file_name: str) -> bytes:
-        downloader = self.proxy.get_downloader_for_dist(dist_name)
-        assert downloader is not None
-
-        urls = downloader.get_file_urls(dist_name)
+        urls = self._get_dist_urls(dist_name)
         assert urls
 
         assert file_name in urls
         url = urls[file_name]
+
         logger.debug("Downloading file from %s", url)
         with urlopen(url) as result:
             logger.debug("Headers: %r", result.headers.items())
             return result.read()
 
-    def _should_return_dummy(self, dist_name: str) -> bool:
-        return normalize_dist_name(
-            dist_name
-        ) in NORMALIZED_IRRELEVANT_PACKAGE_NAMES or normalize_dist_name(dist_name).startswith(
-            "adafruit_blinka_"
-        )
-
     def _tweak_file(self, dist_name: str, file_name: str, original_bytes: bytes) -> bytes:
         if not file_name.lower().endswith(".tar.gz"):
             return original_bytes
 
         # In case of upip packages (tar.gz-s without setup.py) reverse following process:
         # https://github.com/micropython/micropython-lib/commit/3a6ab0b
 
@@ -308,15 +203,17 @@
 
             if "/" in info.name:
                 wrapper_dir, rel_name = info.name.split("/", maxsplit=1)
             else:
                 assert info.isdir()
                 wrapper_dir, rel_name = info.name, ""
 
-            assert normalize_dist_name(wrapper_dir).startswith(normalize_dist_name(dist_name))
+            assert custom_normalize_dist_name(wrapper_dir).startswith(
+                custom_normalize_dist_name(dist_name)
+            )
 
             rel_name = rel_name.strip("/")
             rel_segments = rel_name.split("/")
 
             # collect information about the original tar
             if rel_name == "setup.py":
                 logger.debug("The archive contains setup.py. No tweaks needed")
@@ -392,14 +289,23 @@
 
     def _add_file_to_tar(self, name: str, content: bytes, tar: tarfile.TarFile) -> None:
         stream = io.BytesIO(content)
         info = tarfile.TarInfo(name=name)
         info.size = len(content)
         tar.addfile(info, stream)
 
+    def _should_return_dummy(self, dist_name: str) -> bool:
+        return custom_normalize_dist_name(
+            dist_name
+        ) in NORMALIZED_IRRELEVANT_PACKAGE_NAMES or custom_normalize_dist_name(
+            dist_name
+        ).startswith(
+            "adafruit_blinka_"
+        )
+
     def _parse_metadata(self, metadata_bytes) -> Dict[str, str]:
         metadata = email.parser.Parser().parsestr(metadata_bytes.decode("utf-8"))
         return {
             key: metadata.get(key)
             for key in (
                 "Metadata-Version",
                 "Name",
@@ -415,15 +321,14 @@
     def _create_setup_py(
         self,
         metadata: Dict[str, str],
         py_modules: List[str],
         packages: List[str],
         requirements: List[str],
     ) -> str:
-
         src = dedent(
             """
             from setuptools import setup
             setup (
             """
         ).lstrip()
 
@@ -451,14 +356,238 @@
         # include all other files as package data
         src += "    package_data={'*': ['*', '*/*', '*/*/*', '*/*/*/*', '*/*/*/*/*', '*/*/*/*/*/*', '*/*/*/*/*/*/*', '*/*/*/*/*/*/*/*']}\n"
 
         src += ")\n"
         return src
 
 
+class MpOrgV2IndexDownloader(BaseIndexDownloader):
+    def __init__(self, index_url):
+        self._packages = None
+        super().__init__(index_url)
+
+    def get_dist_file_names(self, dist_name: str) -> Optional[List[str]]:
+        # there is no per-package, all-versions metadata resource. Need to use the global index
+        meta = self._get_dist_metadata(dist_name)
+        if meta is None:
+            return None
+
+        # Collect relationship between version and constructed file names so that I won't need to parse file name later.
+        meta["original_versions_per_file_name"] = {}
+
+        result = []
+        for version in meta["versions"]["py"]:
+            file_name = create_dist_info_version_name(dist_name, version) + "-py3-none-any.whl"
+            meta["original_versions_per_file_name"][file_name] = version
+            result.append(file_name)
+
+        return result
+
+    def get_file_content(self, dist_name: str, file_name: str) -> bytes:
+        dist_meta = self._get_dist_metadata(dist_name)
+        original_name = dist_meta["name"]
+
+        original_versions = dist_meta.get("original_versions_per_file_name", None)
+        assert isinstance(original_versions, dict)
+        original_version = original_versions.get(file_name, None)
+        assert isinstance(original_version, str)
+
+        version_meta_url = f"{self._index_url}/package/py/{original_name}/{original_version}.json"
+        with urlopen(version_meta_url) as fp:
+            version_meta = json.load(fp)
+
+        return self._construct_wheel_content(dist_meta, version_meta)
+
+    def _construct_wheel_content(
+        self, dist_meta: Dict[str, Any], version_meta: Dict[str, Any]
+    ) -> bytes:
+        urls_per_wheel_path = {}
+
+        for wheel_path, short_hash in version_meta.get("hashes", []):
+            urls_per_wheel_path[
+                wheel_path
+            ] = f"{self._index_url}/file/{short_hash[:2]}/{short_hash}"
+
+        for wheel_path, url in version_meta.get("urls", []):
+            urls_per_wheel_path[wheel_path] = url
+
+        bytes_per_wheel_path = {}
+        for wheel_path, url in urls_per_wheel_path.items():
+            with urlopen(url) as fp:
+                bytes_per_wheel_path[wheel_path] = fp.read()
+
+        # construct metadata files
+        meta_dir_prefix = create_dist_info_version_name(dist_meta["name"], version_meta["version"])
+        meta_dir = f"{meta_dir_prefix}.dist-info"
+        summary = dist_meta.get("description", "").replace("\r\n", "\n").replace("\n", " ")
+
+        metadata = textwrap.dedent(
+            f"""
+            Metadata-Version: 2.1
+            Name: {safe_name(dist_meta["name"])}
+            Version: {safe_version(version_meta["version"])}
+            Summary: {summary}
+            Author: {dist_meta.get("author", "")}
+            License: {dist_meta.get("license", "")}
+            """
+        ).lstrip()
+
+        for dep_name, dep_version in version_meta.get("deps", []):
+            metadata += f"Requires-Dist: {dep_name}"
+            if dep_version and dep_version != "latest":
+                metadata += " ("
+                if dep_version[0] not in "<>=":
+                    metadata += "=="
+                metadata += dep_version
+                metadata += ")"
+            metadata += "\n"
+
+        bytes_per_wheel_path[f"{meta_dir}/METADATA"] = metadata.encode("utf-8")
+
+        bytes_per_wheel_path[f"{meta_dir}/WHEEL"] = (
+            textwrap.dedent(
+                """
+            Wheel-Version: 1.0
+            Generator: bdist_wheel (0.37.1)
+            Root-Is-Purelib: true
+            Tag: py3-none-any
+            """
+            )
+            .lstrip()
+            .encode("utf-8")
+        )
+
+        record_lines = []
+        for wheel_path, content in bytes_per_wheel_path.items():
+            digest = hashlib.sha256(content).hexdigest()
+            record_lines.append(f"{wheel_path},sha256={digest},{len(content)}")
+        record_lines.append(f"{meta_dir}/RECORD,,")
+
+        bytes_per_wheel_path[f"{meta_dir}/RECORD"] = ("\n".join(record_lines) + "\n").encode(
+            "utf-8"
+        )
+
+        zip_buffer = io.BytesIO()
+        with zipfile.ZipFile(
+            zip_buffer, mode="a", compression=zipfile.ZIP_DEFLATED, allowZip64=False
+        ) as fp:
+            for wheel_path, content in bytes_per_wheel_path.items():
+                fp.writestr(wheel_path, content)
+
+        with open(os.path.expanduser("~/out.whl"), "wb") as fp:
+            fp.write(zip_buffer.getvalue())
+        return zip_buffer.getvalue()
+
+    def _get_dist_metadata(self, dist_name: str) -> Optional[Dict[Any, Any]]:
+        if self._packages is None:
+            with urlopen(MP_ORG_INDEX_V2 + "/index.json") as fp:
+                self._packages = json.load(fp)["packages"]
+
+        for package in self._packages:
+            if custom_normalize_dist_name(package["name"]) == custom_normalize_dist_name(dist_name):
+                return package
+
+        return None
+
+
+class PipkinProxy(HTTPServer):
+    def __init__(
+        self, no_mp_org: bool, index_url: Optional[str], extra_index_urls: List[str], port: int
+    ):
+        self._downloaders: List[BaseIndexDownloader] = []
+        self._downloaders_by_dist_name: Dict[str, Optional[BaseIndexDownloader]] = {}
+        if not no_mp_org:
+            self._downloaders.append(MpOrgV2IndexDownloader(MP_ORG_INDEX_V2))
+        self._downloaders.append(SimpleIndexDownloader(index_url or PYPI_SIMPLE_INDEX))
+        for url in extra_index_urls:
+            self._downloaders.append(SimpleIndexDownloader(url))
+        super().__init__(("127.0.0.1", port), PipkinProxyHandler)
+
+    def get_downloader_for_dist(self, dist_name: str) -> Optional[BaseIndexDownloader]:
+        if dist_name not in self._downloaders_by_dist_name:
+            for downloader in self._downloaders:
+                logger.debug("Checking if %s has %r", downloader, dist_name)
+                file_names = downloader.get_dist_file_names(dist_name)
+                if file_names is not None:
+                    logger.debug("Got %r file names", len(file_names))
+                    self._downloaders_by_dist_name[dist_name] = downloader
+                    break
+                else:
+                    logger.debug("Got None. Trying next downloader")
+            else:
+                self._downloaders_by_dist_name[dist_name] = None
+
+        return self._downloaders_by_dist_name[dist_name]
+
+    def get_index_url(self) -> str:
+        return f"http://127.0.0.1:{self.server_port}"
+
+
+class PipkinProxyHandler(BaseHTTPRequestHandler):
+    def __init__(
+        self,
+        request: Union[socket.socket, Tuple[bytes, socket.socket]],
+        client_address: Tuple[str, int],
+        server: BaseServer,
+    ):
+        logger.debug("Creating new handler")
+        assert isinstance(server, PipkinProxy)
+        self.proxy: PipkinProxy = server
+        super().__init__(request, client_address, server)
+
+    def do_GET(self) -> None:
+        path = self.path.strip("/")
+        logger.debug("do_GET for %s", path)
+        if "/" in path:
+            assert path.count("/") == 1
+            self._serve_file(*path.split("/"))
+        else:
+            self._serve_distribution_page(path)
+
+    def _serve_distribution_page(self, dist_name: str) -> None:
+        logger.debug("Serving index page for %s", dist_name)
+        downloader = self.proxy.get_downloader_for_dist(dist_name)
+        if downloader is None:
+            self.send_response(404)
+            self.end_headers()
+            return
+
+        # TODO: check https://discuss.python.org/t/community-testing-of-packaging-tools-against-non-warehouse-indexes/13442
+
+        file_names = downloader.get_dist_file_names(dist_name)
+        # logger.debug("File urls: %r", file_names)
+        self.send_response(200)
+        self.send_header("Content-type", f"text/html; charset={SERVER_ENCODING}")
+        self.send_header("Cache-Control", "max-age=600, public")
+        self.end_headers()
+        self.wfile.write("<!DOCTYPE html><html><body>\n".encode(SERVER_ENCODING))
+        for file_name in file_names:
+            self.wfile.write(
+                f"<a href='/{dist_name}/{file_name}/'>{file_name}</a>\n".encode(SERVER_ENCODING)
+            )
+        self.wfile.write("</body></html>".encode(SERVER_ENCODING))
+
+    def _serve_file(self, dist_name: str, file_name: str):
+        logger.debug("Serving %s for %s", file_name, dist_name)
+
+        downloader = self.proxy.get_downloader_for_dist(dist_name)
+        assert downloader is not None
+        file_content = downloader.get_file_content(dist_name, file_name)
+
+        self.send_response(200)
+        self.send_header("Content-Type", "application/octet-stream")
+        self.send_header("Cache-Control", "max-age=365000000, immutable, public")
+        self.end_headers()
+
+        block_size = 4096
+        for start_index in range(0, len(file_content), block_size):
+            block = file_content[start_index : start_index + block_size]
+            self.wfile.write(block)
+
+
 def start_proxy(
     no_mp_org: bool,
     index_url: Optional[str],
     extra_index_urls: List[str],
 ) -> PipkinProxy:
     try:
         proxy = PipkinProxy(no_mp_org, index_url, extra_index_urls, PREFERRED_PORT)
@@ -473,15 +602,15 @@
 
     return proxy
 
 
 def create_dummy_dist(dist_name: str, file_name: str) -> bytes:
     logger.info("Creating dummy content for %s", file_name)
     parsed_dist_name, version, suffix = parse_dist_file_name(file_name)
-    assert normalize_dist_name(dist_name) == normalize_dist_name(parsed_dist_name)
+    assert custom_normalize_dist_name(dist_name) == custom_normalize_dist_name(parsed_dist_name)
 
     with tempfile.TemporaryDirectory(prefix="pipkin-proxy") as tmp:
         setup_py_path = os.path.join(tmp, "setup.py")
         with open(setup_py_path, "w", encoding="utf-8") as fp:
             fp.write(
                 dedent(
                     f"""
```

### Comparing `pipkin-1.0b8/pipkin/serial_connection.py` & `pipkin-2.0b1/pipkin/serial_connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 
 logger = getLogger(__name__)
 
 
 class SerialConnection(MicroPythonConnection):
     def __init__(self, port, baudrate=115200, dtr=None, rts=None, skip_reader=False):
-
         import serial
         from serial.serialutil import SerialException
 
         super().__init__()
 
         try:
             self._serial = serial.Serial(
@@ -155,15 +154,14 @@
                     logger.exception("Couldn't close serial")
 
 
 class DifficultSerialConnection(SerialConnection):
     """For hardening the communication protocol"""
 
     def _make_output_available(self, data, block=True):
-
         # output prompts in parts
         if FIRST_RAW_PROMPT in data or NORMAL_PROMPT in data:
             if FIRST_RAW_PROMPT in data:
                 start = data.find(FIRST_RAW_PROMPT)
                 end = start + len(FIRST_RAW_PROMPT)
             else:
                 start = data.find(NORMAL_PROMPT)
```

### Comparing `pipkin-1.0b8/pipkin/session.py` & `pipkin-2.0b1/pipkin/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -209,15 +209,14 @@
         index_url: Optional[str] = None,
         extra_index_urls: Optional[List[str]] = None,
         no_index: bool = False,
         find_links: Optional[str] = None,
         excludes: Optional[List[str]] = None,
         **_,
     ):
-
         args = ["list"]
 
         if outdated:
             args.append("--outdated")
         if uptodate:
             args.append("--uptodate")
         if not_required:
@@ -260,15 +259,14 @@
     def freeze(
         self,
         paths: Optional[List[str]] = None,
         user: bool = False,
         excludes: Optional[List[str]] = None,
         **_,
     ):
-
         args = ["freeze"]
 
         args += self._format_exclusion_args(excludes)
 
         self._populate_venv(paths=paths, user=user)
         self._invoke_pip(args)
 
@@ -694,15 +692,14 @@
         pip_args: List[str],
         no_mp_org: bool,
         index_url: str,
         extra_index_urls: List[str],
         no_index: bool,
         find_links: Optional[str],
     ):
-
         if no_index:
             assert find_links
             self._invoke_pip(pip_args + ["--no-index", "--find-links", find_links])
         else:
             proxy = start_proxy(no_mp_org, index_url, extra_index_urls)
             logger.info("Using PipkinProxy at %s", proxy.get_index_url())
```

### Comparing `pipkin-1.0b8/pipkin/util.py` & `pipkin-2.0b1/pipkin/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import re
 import subprocess
 import sys
 from dataclasses import dataclass
 from logging import getLogger
 from typing import List, Optional, Set, Tuple
 
+import pkg_resources
+
 logger = getLogger(__name__)
 
 
 @dataclass
 class ParsedWheelFilename:
     project: str
     version: str
@@ -45,14 +47,22 @@
         build=m.group("build"),
         python_tags=m.group("python_tags").split("."),
         abi_tags=m.group("abi_tags").split("."),
         platform_tags=m.group("platform_tags").split("."),
     )
 
 
+def create_dist_info_version_name(dist_name: str, version: str) -> str:
+    # https://packaging.python.org/en/latest/specifications/binary-distribution-format/#escaping-and-unicode
+    # https://peps.python.org/pep-0440/
+    safe_name = pkg_resources.safe_name(dist_name).replace("-", "_")
+    safe_version = pkg_resources.safe_version(version)
+    return f"{safe_name}-{safe_version}"
+
+
 def get_windows_folder(ID: int) -> str:
     # http://stackoverflow.com/a/3859336/261181
     # http://www.installmate.com/support/im9/using/symbols/functions/csidls.htm
     if sys.platform == "win32":
         import ctypes.wintypes
 
         SHGFP_TYPE_CURRENT = 0
@@ -159,17 +169,17 @@
     return len(data) > 0 and is_continuation_byte(data[0])
 
 
 def is_continuation_byte(byte: int) -> bool:
     return (byte & 0b11000000) == 0b10000000
 
 
-def normalize_dist_name(name: str) -> str:
+def custom_normalize_dist_name(name: str) -> str:
     # https://peps.python.org/pep-0503/#normalized-names
-    return re.sub(r"[-_.]+", "-", name).lower()
+    return pkg_resources.safe_name(name).lower().replace("-", "_").replace(".", "_")
 
 
 def list_volumes(skip_letters: Optional[Set[str]] = None) -> List[str]:
     skip_letters = skip_letters or set()
 
     "Adapted from https://github.com/ntoll/uflash/blob/master/uflash.py"
     if sys.platform == "win32":
```

### Comparing `pipkin-1.0b8/pipkin/webrepl_connection.py` & `pipkin-2.0b1/pipkin/webrepl_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,34 +13,33 @@
     Problem with block size:
     https://github.com/micropython/micropython/issues/2497
     Start with conservative delay.
     Client may later reduce it for better efficiency
     """
 
     def __init__(self, url, password, num_bytes_received=0):
-
         self.num_bytes_received = num_bytes_received
         super().__init__()
 
         try:
             import websockets  # @UnusedImport
         except Exception:
             print(
                 "Can't import `websockets`. You can install it via 'Tools => Manage plug-ins'.",
                 file=sys.stderr,
             )
             sys.exit(-1)
         self._url = url
         self._password = password
-        self._write_responses = Queue()
+        self._write_responses: Queue = Queue()
 
         # Some tricks are needed to use async library in a sync program.
         # Using thread-safe queues to communicate with async world in another thread
-        self._write_queue = Queue()
-        self._connection_result = Queue()
+        self._write_queue: Queue = Queue()
+        self._connection_result: Queue = Queue()
         self._ws_thread = threading.Thread(target=self._wrap_ws_main, daemon=True)
         self._ws_thread.start()
 
         # Wait until connection was made
         res = self._connection_result.get()
         if res != "OK":
             raise res
```

### Comparing `pipkin-1.0b8/pipkin.egg-info/PKG-INFO` & `pipkin-2.0b1/pipkin.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,206 +1,204 @@
-Metadata-Version: 2.1
-Name: pipkin
-Version: 1.0b8
-Summary: Tool for installing packages for MicroPython and CircuitPython
-Home-page: https://github.com/aivarannamaa/pipkin
-Author: Aivar Annamaa
-License: MIT
-Project-URL: Source code, https://github.com/aivarannamaa/pipkin
-Project-URL: Bug tracker, https://github.com/aivarannamaa/pipkin/issues
-Keywords: MicroPython CircuitPython pip upip
-Platform: Windows
-Platform: macOS
-Platform: Linux
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: License :: Freeware
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development
-Requires-Python: >=3.7
-License-File: LICENSE
-
-pipkin
-=======
-Tool for managing distribution packages for MicroPython and CircuitPython on target devices or in a local directory.
-
-Supports both `upip-compatible packages <https://docs.micropython.org/en/latest/reference/packages.html>`_,
-and regular pip-compatible packages.
-
-By default it prefers packages at micropython.org-s index. If the package or the required version is not
-found there, then it turns to PyPI.
-
-Unlike some of the package managers for MicroPython and CircuitPython, pipkin keeps a minimal set of package
-metadata (trimmed .dist-info/METADATA and .dist-info/RECORD) next to the package itself, just like pip.
-This enables straigthforward approach for uninstalling, listing and freezing.
-
-When installing with ``--compile`` switch, pipkin uses suitable `mpy-cross` to compile the
-py-files on the fly and transfers resulting mpy-files to the target.
-
-Installation
---------------
-``pip install pipkin``
-
-Usage
------
-
-The basic structure of the command line is ``pipkin <target selection> <command> <command arguments>``.
-For example:
-
-* ``pipkin --port /dev/ttyACM0 install micropython-logging``
-* ``pipkin --mount G:\lib install adafruit-circuitpython-ssd1306``
-* ``pipkin --mount G:\lib install --compile adafruit-circuitpython-ssd1306``
-* ``pipkin --dir my_project/lib install micropython-logging micropython-oled``
-* ``pipkin --port COM5 uninstall micropython-logging micropython-oled``
-* ``pipkin --port COM5 list --outdated``
-
-If you have attached a single CircuitPython device (with its filesystem mounted as a disk) or
-a single well known MicroPython device (eg. Raspberry Pi Pico), then you can omit the target selection
-part:
-
-* ``pipkin install adafruit-circuitpython-ssd1306``
-
-pipkin -h
-----------
-
-::
-
-    usage: pipkin [-h] [-V] [-v | -q] [-p <port> | -m <path> | -d <path>] {install,uninstall,list,show,freeze,check,download,wheel,cache} ...
-
-    Tool for managing MicroPython and CircuitPython packages
-
-    general:
-      -h, --help            Show this help message and exit
-      -V, --version         Show program version and exit
-      -v, --verbose         Show more details about the process
-      -q, --quiet           Don't show non-error output
-
-    target selection (pick one or let pipkin autodetect the port or mount):
-      -p <port>, --port <port>
-                            Serial port of the target device
-      -m <path>, --mount <path>
-                            Mount point (volume, disk, drive) of the target device
-      -d <path>, --dir <path>
-                            Directory in the local filesystem
-
-    commands:
-      Use "pipkin <command> -h" for usage help of a command
-
-      {install,uninstall,list,show,freeze,check,download,wheel,cache}
-        install             Install packages.
-        uninstall           Uninstall packages.
-        list                List installed packages.
-        show                Show information about one or more installed packages.
-        freeze              Output installed packages in requirements format.
-        check               Verify installed packages have compatible dependencies.
-        download            Download packages.
-        wheel               Build Wheel archives for your requirements and dependencies.
-        cache               Inspect and manage pipkin cache.
-
-pipkin install -h
-------------------
-
-::
-
-    usage: pipkin install [-h] [-r [<file> [<file> ...]]] [-c [<file> [<file> ...]]] [--no-deps] [--pre] [-i <url>] [--extra-index-url [<url> [<url> ...]]]
-                               [--no-index] [--no-mp-org] [-f <url|file|dir>] [-U] [--upgrade-strategy <upgrade_strategy>] [--force-reinstall] [--compile]
-                               [<spec> [<spec> ...]]
-
-    Installs upip or pip compatible distribution packages onto a MicroPython/CircuitPython device or into a local directory.
-
-    positional arguments:
-      <spec>                Package specification, eg. 'micropython-os' or 'micropython-os>=0.6'
-
-    optional arguments:
-      -h, --help            show this help message and exit
-      -U, --upgrade         Upgrade all specified packages to the newest available version. The handling of dependencies depends on the upgrade-strategy used.
-      --upgrade-strategy <upgrade_strategy>
-                            Determines how dependency upgrading should be handled [default: only-if-needed]. 'eager' - dependencies are upgraded regardless of
-                            whether the currently installed version satisfies the requirements of the upgraded package(s). 'only-if-needed' - are upgraded only when
-                            they do not satisfy the requirements of the upgraded package(s).
-      --force-reinstall     Reinstall all packages even if they are already up-to-date.
-      --compile             Compile and install mpy files.
-
-    package selection:
-      -r [<file> [<file> ...]], --requirement [<file> [<file> ...]]
-                            Install from the given requirements file.
-      -c [<file> [<file> ...]], --constraint [<file> [<file> ...]]
-                            Constrain versions using the given constraints file.
-      --no-deps             Don't install package dependencies.
-      --pre                 Include pre-release and development versions. By default, pipkin only finds stable versions.
-
-    index selection:
-      -i <url>, --index-url <url>
-                            Base URL of the Python Package Index (default https://pypi.org/simple).
-      --extra-index-url [<url> [<url> ...]]
-                            Extra URLs of package indexes to use in addition to --index-url.
-      --no-index            Ignore package index (only looking at --find-links URLs instead).
-      --no-mp-org           Don't let micropython.org/pi override other indexes.
-      -f <url|file|dir>, --find-links <url|file|dir>
-                            If a URL or path to an html file, then parse for links to archives such as sdist (.tar.gz) or wheel (.whl) files. If a local path or
-                            file:// URL that's a directory, then look for archives in the directory listing.
-
-Adafruit-Blinka and co
-----------------------
-`Adafruit-Blinka <https://pypi.org/project/Adafruit-Blinka/>`_ is a compatibility library which allows
-running CircuitPython code with CPython. When publishing CircuitPython libraries at PyPI, Adafruit
-and the community have so far targeted only CPython users, because tools for connecting PyPI with bare metal
-CircuitPython did not exist (or because at the moment it is not clear how to publish wheels for Pythons
-which can't run pip themselves). Therefore the CircuitPython libraries at PyPI usually have Adafruit-Blinka
-dependency, which is not relevant (and would even cause problems) on bare metal CircuitPython devices.
-
-pipkin's current approach is to have its proxy-index return dummy Adafruit-Blinka distribution, which contains
-no modules and has no dependencies. This means when you're installing a library which depends on Adafruit-Blinka,
-you'll get Blinka's .dist-info directory with METADATA and RECORD, but nothing else. Let's call it
-an optimized build.
-
-Dummies are returned for all dists, which are currently omitted by
-`adafruit/circuitpython-build-tools <https://github.com/adafruit/circuitpython-build-tools/blob/de44a709f6287d2759df14c89707f2d8f5a026f5/circuitpython_build_tools/scripts/build_bundles.py#L42>`_
-
-Current state and goals
------------------------
-Handling packages meant for upip, micropython.org/pi overrides and the problems outlined in the
-previous section, all together make pipkin less elegant and slower than one would like. Still, this is just
-a start. There are several optimizations possible within current approach. Also, PyPI, pip, wheel
-and packaging standards are evolving -- in the future it may become easy to publish separate wheels
-for MicroPython and/or CircuitPython and pip may become usable for "cross-installing" packages for
-other platforms.
-
-Even if clumsy at times, pipkin tries to be the proof-of-concept for demonstrating that even in
-the world of MicroPython and CircuitPython, we could continue publishing standard sdists
-and wheels on PyPI and re-use the familiar approach for package management. While introducing
-new formats and distribution mechanisms have their benefits, we shouldn't dismiss the standard approach
-yet.
-
-Implementation
---------------
-pipkin delegates most of its work to our old friend pip. This is the reason it is able to offer
-so much functionality.
-
-Both upip-compatibility and support for micropython.org-s
-index is achieved by using up a temporary local index, which proxies both PyPI (or another specified index)
-and micropython.org/pi and restores missing setup.py for upip-compatible packages.
-
-Non-CPython installation target is achieved by creating and maintaining private working environment (venv).
-(As creating a venv can be slow in Windows, be prepared for longer wait when using pipkin for the first time.)
-
-In the beginning of the session, pipkin collects package metadata from the target (eg. from the /lib directory
-of the device connected over serial) and creates corresponding dummy packages in the working environment.
-Then it starts the temporary local index and invokes venv-s pip aginst it. When pip finishes, it detects the
-distributions which are removed, added or changed and applies corresponding changes to the target device or
-directory.
-
-
-
+Metadata-Version: 2.1
+Name: pipkin
+Version: 2.0b1
+Summary: Tool for installing packages for MicroPython and CircuitPython
+Home-page: https://github.com/aivarannamaa/pipkin
+Author: Aivar Annamaa
+License: MIT
+Project-URL: Source code, https://github.com/aivarannamaa/pipkin
+Project-URL: Bug tracker, https://github.com/aivarannamaa/pipkin/issues
+Keywords: MicroPython CircuitPython pip upip
+Platform: Windows
+Platform: macOS
+Platform: Linux
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: Freeware
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Software Development
+Requires-Python: >=3.7
+License-File: LICENSE
+
+pipkin
+=======
+Tool for managing distribution packages for MicroPython and CircuitPython on target devices or in a local directory.
+
+Supports both `upip-compatible packages <https://docs.micropython.org/en/latest/reference/packages.html>`_,
+and regular pip-compatible packages.
+
+By default it prefers packages at micropython.org-s index. If the package or the required version is not
+found there, then it turns to PyPI.
+
+Unlike some of the package managers for MicroPython and CircuitPython, pipkin keeps a minimal set of package
+metadata (trimmed .dist-info/METADATA and .dist-info/RECORD) next to the package itself, just like pip.
+This enables straigthforward approach for uninstalling, listing and freezing.
+
+When installing with ``--compile`` switch, pipkin uses suitable `mpy-cross` to compile the
+py-files on the fly and transfers resulting mpy-files to the target.
+
+Installation
+--------------
+``pip install pipkin``
+
+Usage
+-----
+
+The basic structure of the command line is ``pipkin <target selection> <command> <command arguments>``.
+For example:
+
+* ``pipkin --port /dev/ttyACM0 install micropython-logging``
+* ``pipkin --mount G:\lib install adafruit-circuitpython-ssd1306``
+* ``pipkin --mount G:\lib install --compile adafruit-circuitpython-ssd1306``
+* ``pipkin --dir my_project/lib install micropython-logging micropython-oled``
+* ``pipkin --port COM5 uninstall micropython-logging micropython-oled``
+* ``pipkin --port COM5 list --outdated``
+
+If you have attached a single CircuitPython device (with its filesystem mounted as a disk) or
+a single well known MicroPython device (eg. Raspberry Pi Pico), then you can omit the target selection
+part:
+
+* ``pipkin install adafruit-circuitpython-ssd1306``
+
+pipkin -h
+----------
+
+::
+
+    usage: pipkin [-h] [-V] [-v | -q] [-p <port> | -m <path> | -d <path>] {install,uninstall,list,show,freeze,check,download,wheel,cache} ...
+
+    Tool for managing MicroPython and CircuitPython packages
+
+    general:
+      -h, --help            Show this help message and exit
+      -V, --version         Show program version and exit
+      -v, --verbose         Show more details about the process
+      -q, --quiet           Don't show non-error output
+
+    target selection (pick one or let pipkin autodetect the port or mount):
+      -p <port>, --port <port>
+                            Serial port of the target device
+      -m <path>, --mount <path>
+                            Mount point (volume, disk, drive) of the target device
+      -d <path>, --dir <path>
+                            Directory in the local filesystem
+
+    commands:
+      Use "pipkin <command> -h" for usage help of a command
+
+      {install,uninstall,list,show,freeze,check,download,wheel,cache}
+        install             Install packages.
+        uninstall           Uninstall packages.
+        list                List installed packages.
+        show                Show information about one or more installed packages.
+        freeze              Output installed packages in requirements format.
+        check               Verify installed packages have compatible dependencies.
+        download            Download packages.
+        wheel               Build Wheel archives for your requirements and dependencies.
+        cache               Inspect and manage pipkin cache.
+
+pipkin install -h
+------------------
+
+::
+
+    usage: pipkin install [-h] [-r [<file> [<file> ...]]] [-c [<file> [<file> ...]]] [--no-deps] [--pre] [-i <url>] [--extra-index-url [<url> [<url> ...]]]
+                               [--no-index] [--no-mp-org] [-f <url|file|dir>] [-U] [--upgrade-strategy <upgrade_strategy>] [--force-reinstall] [--compile]
+                               [<spec> [<spec> ...]]
+
+    Installs upip or pip compatible distribution packages onto a MicroPython/CircuitPython device or into a local directory.
+
+    positional arguments:
+      <spec>                Package specification, eg. 'micropython-os' or 'micropython-os>=0.6'
+
+    optional arguments:
+      -h, --help            show this help message and exit
+      -U, --upgrade         Upgrade all specified packages to the newest available version. The handling of dependencies depends on the upgrade-strategy used.
+      --upgrade-strategy <upgrade_strategy>
+                            Determines how dependency upgrading should be handled [default: only-if-needed]. 'eager' - dependencies are upgraded regardless of
+                            whether the currently installed version satisfies the requirements of the upgraded package(s). 'only-if-needed' - are upgraded only when
+                            they do not satisfy the requirements of the upgraded package(s).
+      --force-reinstall     Reinstall all packages even if they are already up-to-date.
+      --compile             Compile and install mpy files.
+
+    package selection:
+      -r [<file> [<file> ...]], --requirement [<file> [<file> ...]]
+                            Install from the given requirements file.
+      -c [<file> [<file> ...]], --constraint [<file> [<file> ...]]
+                            Constrain versions using the given constraints file.
+      --no-deps             Don't install package dependencies.
+      --pre                 Include pre-release and development versions. By default, pipkin only finds stable versions.
+
+    index selection:
+      -i <url>, --index-url <url>
+                            Base URL of the Python Package Index (default https://pypi.org/simple).
+      --extra-index-url [<url> [<url> ...]]
+                            Extra URLs of package indexes to use in addition to --index-url.
+      --no-index            Ignore package index (only looking at --find-links URLs instead).
+      --no-mp-org           Don't let micropython.org/pi override other indexes.
+      -f <url|file|dir>, --find-links <url|file|dir>
+                            If a URL or path to an html file, then parse for links to archives such as sdist (.tar.gz) or wheel (.whl) files. If a local path or
+                            file:// URL that's a directory, then look for archives in the directory listing.
+
+Adafruit-Blinka and co
+----------------------
+`Adafruit-Blinka <https://pypi.org/project/Adafruit-Blinka/>`_ is a compatibility library which allows
+running CircuitPython code with CPython. When publishing CircuitPython libraries at PyPI, Adafruit
+and the community have so far targeted only CPython users, because tools for connecting PyPI with bare metal
+CircuitPython did not exist (or because at the moment it is not clear how to publish wheels for Pythons
+which can't run pip themselves). Therefore the CircuitPython libraries at PyPI usually have Adafruit-Blinka
+dependency, which is not relevant (and would even cause problems) on bare metal CircuitPython devices.
+
+pipkin's current approach is to have its proxy-index return dummy Adafruit-Blinka distribution, which contains
+no modules and has no dependencies. This means when you're installing a library which depends on Adafruit-Blinka,
+you'll get Blinka's .dist-info directory with METADATA and RECORD, but nothing else. Let's call it
+an optimized build.
+
+Dummies are returned for all dists, which are currently omitted by
+`adafruit/circuitpython-build-tools <https://github.com/adafruit/circuitpython-build-tools/blob/de44a709f6287d2759df14c89707f2d8f5a026f5/circuitpython_build_tools/scripts/build_bundles.py#L42>`_
+
+Current state and goals
+-----------------------
+Handling packages meant for upip, micropython.org/pi overrides and the problems outlined in the
+previous section, all together make pipkin less elegant and slower than one would like. Still, this is just
+a start. There are several optimizations possible within current approach. Also, PyPI, pip, wheel
+and packaging standards are evolving -- in the future it may become easy to publish separate wheels
+for MicroPython and/or CircuitPython and pip may become usable for "cross-installing" packages for
+other platforms.
+
+Even if clumsy at times, pipkin tries to be the proof-of-concept for demonstrating that even in
+the world of MicroPython and CircuitPython, we could continue publishing standard sdists
+and wheels on PyPI and re-use the familiar approach for package management. While introducing
+new formats and distribution mechanisms have their benefits, we shouldn't dismiss the standard approach
+yet.
+
+Implementation
+--------------
+pipkin delegates most of its work to our old friend pip. This is the reason it is able to offer
+so much functionality.
+
+Both upip-compatibility and support for micropython.org-s
+index is achieved by using up a temporary local index, which proxies both PyPI (or another specified index)
+and micropython.org/pi and restores missing setup.py for upip-compatible packages.
+
+Non-CPython installation target is achieved by creating and maintaining private working environment (venv).
+(As creating a venv can be slow in Windows, be prepared for longer wait when using pipkin for the first time.)
+
+In the beginning of the session, pipkin collects package metadata from the target (eg. from the /lib directory
+of the device connected over serial) and creates corresponding dummy packages in the working environment.
+Then it starts the temporary local index and invokes venv-s pip aginst it. When pip finishes, it detects the
+distributions which are removed, added or changed and applies corresponding changes to the target device or
+directory.
+
```

### Comparing `pipkin-1.0b8/setup.py` & `pipkin-2.0b1/setup.py`

 * *Files identical despite different names*

