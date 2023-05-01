# Comparing `tmp/dwload_server-0.5.0.tar.gz` & `tmp/dwload_server-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dwload_server-0.5.0.tar", max compression
+gzip compressed data, was "dwload_server-0.5.1.tar", max compression
```

## Comparing `dwload_server-0.5.0.tar` & `dwload_server-0.5.1.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0    35122 2022-09-09 18:45:58.158234 dwload_server-0.5.0/LICENSE
--rw-r--r--   0        0        0    10163 2022-09-11 10:58:20.612003 dwload_server-0.5.0/README.md
--rw-r--r--   0        0        0       22 2022-09-11 10:58:28.188055 dwload_server-0.5.0/dwload_server/__init__.py
--rw-r--r--   0        0        0      655 2022-09-10 17:20:01.467712 dwload_server-0.5.0/dwload_server/constants.py
--rw-r--r--   0        0        0     5347 2022-09-11 11:00:11.948772 dwload_server-0.5.0/dwload_server/dev_shell.py
--rw-r--r--   0        0        0     1464 2022-09-10 17:14:51.678969 dwload_server-0.5.0/dwload_server/dwl2bas.py
--rw-r--r--   0        0        0     1325 2022-09-09 19:12:34.138405 dwload_server-0.5.0/dwload_server/exceptions.py
--rw-r--r--   0        0        0        0 2022-09-09 18:45:58.182234 dwload_server-0.5.0/dwload_server/hooks/__init__.py
--rw-r--r--   0        0        0     2231 2022-09-10 17:14:51.690970 dwload_server-0.5.0/dwload_server/hooks/dynamic_dwl.py
--rw-r--r--   0        0        0     2849 2022-09-09 19:12:34.158405 dwload_server-0.5.0/dwload_server/hooks/read_ascii.py
--rw-r--r--   0        0        0     2862 2022-09-10 17:14:51.698969 dwload_server-0.5.0/dwload_server/hooks/save_ascii.py
--rw-r--r--   0        0        0     4598 2022-09-10 18:05:35.209215 dwload_server-0.5.0/dwload_server/pyscripts/autoload_dwl.py
--rw-r--r--   0        0        0     8657 2022-09-10 18:05:35.209215 dwload_server-0.5.0/dwload_server/server_base.py
--rw-r--r--   0        0        0     2590 2022-09-10 16:23:43.565178 dwload_server-0.5.0/dwload_server/server_becker.py
--rw-r--r--   0        0        0     2353 2022-09-10 16:25:19.297399 dwload_server-0.5.0/dwload_server/server_serial.py
--rw-r--r--   0        0        0        0 2022-09-09 18:45:58.182234 dwload_server-0.5.0/dwload_server/utils/__init__.py
--rw-r--r--   0        0        0     2392 2022-09-09 19:12:34.266405 dwload_server-0.5.0/dwload_server/utils/file_tools.py
--rw-r--r--   0        0        0     3209 2022-09-09 19:12:34.282405 dwload_server-0.5.0/dwload_server/utils/hook_handler.py
--rw-r--r--   0        0        0     3024 2022-09-11 11:01:37.525356 dwload_server-0.5.0/pyproject.toml
--rw-r--r--   0        0        0    11388 1970-01-01 00:00:00.000000 dwload_server-0.5.0/setup.py
--rw-r--r--   0        0        0    11325 1970-01-01 00:00:00.000000 dwload_server-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    35122 2023-05-01 15:39:12.414246 dwload_server-0.5.1/LICENSE
+-rw-r--r--   0        0        0    10163 2023-05-01 15:39:12.414246 dwload_server-0.5.1/README.md
+-rw-r--r--   0        0        0       22 2023-05-01 15:45:29.380884 dwload_server-0.5.1/dwload_server/__init__.py
+-rw-r--r--   0        0        0      655 2023-05-01 15:39:12.414246 dwload_server-0.5.1/dwload_server/constants.py
+-rw-r--r--   0        0        0     5347 2023-05-01 15:39:12.414246 dwload_server-0.5.1/dwload_server/dev_shell.py
+-rw-r--r--   0        0        0     1464 2023-05-01 15:39:12.414246 dwload_server-0.5.1/dwload_server/dwl2bas.py
+-rw-r--r--   0        0        0     1325 2023-05-01 15:39:12.414246 dwload_server-0.5.1/dwload_server/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-01 15:39:12.414246 dwload_server-0.5.1/dwload_server/hooks/__init__.py
+-rw-r--r--   0        0        0     2231 2023-05-01 15:39:12.414246 dwload_server-0.5.1/dwload_server/hooks/dynamic_dwl.py
+-rw-r--r--   0        0        0     2849 2023-05-01 15:39:12.414246 dwload_server-0.5.1/dwload_server/hooks/read_ascii.py
+-rw-r--r--   0        0        0     2862 2023-05-01 15:39:12.414246 dwload_server-0.5.1/dwload_server/hooks/save_ascii.py
+-rw-r--r--   0        0        0     4598 2023-05-01 15:39:12.414246 dwload_server-0.5.1/dwload_server/pyscripts/autoload_dwl.py
+-rw-r--r--   0        0        0     8657 2023-05-01 15:39:12.414246 dwload_server-0.5.1/dwload_server/server_base.py
+-rw-r--r--   0        0        0     2590 2023-05-01 15:39:12.414246 dwload_server-0.5.1/dwload_server/server_becker.py
+-rw-r--r--   0        0        0     2353 2023-05-01 15:39:12.414246 dwload_server-0.5.1/dwload_server/server_serial.py
+-rw-r--r--   0        0        0        0 2023-05-01 15:39:12.414246 dwload_server-0.5.1/dwload_server/utils/__init__.py
+-rw-r--r--   0        0        0     2392 2023-05-01 15:39:12.414246 dwload_server-0.5.1/dwload_server/utils/file_tools.py
+-rw-r--r--   0        0        0     3209 2023-05-01 15:39:12.414246 dwload_server-0.5.1/dwload_server/utils/hook_handler.py
+-rw-r--r--   0        0        0     3025 2023-05-01 15:48:00.769379 dwload_server-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0    11326 1970-01-01 00:00:00.000000 dwload_server-0.5.1/PKG-INFO
```

### Comparing `dwload_server-0.5.0/LICENSE` & `dwload_server-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dwload_server-0.5.0/README.md` & `dwload_server-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `dwload_server-0.5.0/dwload_server/constants.py` & `dwload_server-0.5.1/dwload_server/constants.py`

 * *Files identical despite different names*

### Comparing `dwload_server-0.5.0/dwload_server/dev_shell.py` & `dwload_server-0.5.1/dwload_server/dev_shell.py`

 * *Files identical despite different names*

### Comparing `dwload_server-0.5.0/dwload_server/dwl2bas.py` & `dwload_server-0.5.1/dwload_server/dwl2bas.py`

 * *Files identical despite different names*

### Comparing `dwload_server-0.5.0/dwload_server/exceptions.py` & `dwload_server-0.5.1/dwload_server/exceptions.py`

 * *Files identical despite different names*

### Comparing `dwload_server-0.5.0/dwload_server/hooks/dynamic_dwl.py` & `dwload_server-0.5.1/dwload_server/hooks/dynamic_dwl.py`

 * *Files identical despite different names*

### Comparing `dwload_server-0.5.0/dwload_server/hooks/read_ascii.py` & `dwload_server-0.5.1/dwload_server/hooks/read_ascii.py`

 * *Files identical despite different names*

### Comparing `dwload_server-0.5.0/dwload_server/hooks/save_ascii.py` & `dwload_server-0.5.1/dwload_server/hooks/save_ascii.py`

 * *Files identical despite different names*

### Comparing `dwload_server-0.5.0/dwload_server/pyscripts/autoload_dwl.py` & `dwload_server-0.5.1/dwload_server/pyscripts/autoload_dwl.py`

 * *Files identical despite different names*

### Comparing `dwload_server-0.5.0/dwload_server/server_base.py` & `dwload_server-0.5.1/dwload_server/server_base.py`

 * *Files identical despite different names*

### Comparing `dwload_server-0.5.0/dwload_server/server_becker.py` & `dwload_server-0.5.1/dwload_server/server_becker.py`

 * *Files identical despite different names*

### Comparing `dwload_server-0.5.0/dwload_server/server_serial.py` & `dwload_server-0.5.1/dwload_server/server_serial.py`

 * *Files identical despite different names*

### Comparing `dwload_server-0.5.0/dwload_server/utils/file_tools.py` & `dwload_server-0.5.1/dwload_server/utils/file_tools.py`

 * *Files identical despite different names*

### Comparing `dwload_server-0.5.0/dwload_server/utils/hook_handler.py` & `dwload_server-0.5.1/dwload_server/utils/hook_handler.py`

 * *Files identical despite different names*

### Comparing `dwload_server-0.5.0/pyproject.toml` & `dwload_server-0.5.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dwload_server"
-version = "0.5.0"
+version = "0.5.1"
 description = "DWLOAD server implemented in Python"
 authors = ["JensDiemer <dwload_server@jensdiemer.de>"]
 packages = [{ include = "dwload_server" }]
 keywords=["DWLOAD","DriveWire","6809","Dragon","CoCo"]
 classifiers = [
     # http://pypi.python.org/pypi?%3Aaction=list_classifiers
     "Development Status :: 5 - Production/Stable",
@@ -21,15 +21,15 @@
     "Programming Language :: Python :: 3",
 ]
 readme="README.md"
 homepage="https://github.com/6809/DwLoadServer"
 
 
 [tool.poetry.dependencies]
-python = ">=3.8,<4.0"
+python = ">=3.9,<4.0"
 dragonlib = "*"  # https://github.com/6809/dragonlib
 pyserial = "*"  # https://github.com/pyserial/pyserial
 
 [tool.poetry.dev-dependencies]
 dev_shell = "*"  # https://github.com/jedie/dev-shell
 cmd2_ext_test = "*"
 poetry_publish = "*"
@@ -109,15 +109,15 @@
 
 
 [tool.tox]
 # https://tox.readthedocs.io/en/latest/example/basic.html#pyproject-toml-tox-legacy-ini
 legacy_tox_ini = """
 [tox]
 isolated_build = True
-envlist = py310,py39,py38
+envlist = py311,py310,py39
 skip_missing_interpreters = True
 [testenv]
 passenv = *
 whitelist_externals = pytest
 commands =
     pytest
 """
```

### Comparing `dwload_server-0.5.0/setup.py` & `dwload_server-0.5.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,259 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: dwload-server
+Version: 0.5.1
+Summary: DWLOAD server implemented in Python
+Home-page: https://github.com/6809/DwLoadServer
+Keywords: DWLOAD,DriveWire,6809,Dragon,CoCo
+Author: JensDiemer
+Author-email: dwload_server@jensdiemer.de
+Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: MacOS X
+Classifier: Environment :: Other Environment
+Classifier: Environment :: Win32 (MS Windows)
+Classifier: Environment :: X11 Applications
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Requires-Dist: dragonlib
+Requires-Dist: pyserial
+Description-Content-Type: text/markdown
 
-packages = \
-['dwload_server',
- 'dwload_server.hooks',
- 'dwload_server.pyscripts',
- 'dwload_server.utils']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['dragonlib', 'pyserial']
-
-entry_points = \
-{'console_scripts': ['DragonPy = '
-                     'dragodwload_servernpy.core.gui_starter:gui_mainloop',
-                     'devshell = dwload_server.dev_shell:devshell_cmdloop']}
-
-setup_kwargs = {
-    'name': 'dwload-server',
-    'version': '0.5.0',
-    'description': 'DWLOAD server implemented in Python',
-    'long_description': '# DWLOAD Server\n\nDWLOAD server implemented in Python (OpenSource, GPL v3 or above).\n\nConnect your Dragon 32 into your PC and LOAD/SAVE basic listings.\n\n![Dragon32DriveWire1small.jpeg](https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/DwLoadServer/Dragon32DriveWire1small.jpeg "Dragon32DriveWire1small.jpeg")\n\n\n## Quickstart\n\n```bash\n~$ git clone https://github.com/6809/DwLoadServer.git\n~$ cd DwLoadServer\n~/DwLoadServer$ ./devshell.py run serial\n```\n\n\n## features\n\n* load/save files via DWLOAD\n* on-the-fly converting ASCII BASIC listing (see below)\n* dynamic "AUTOLOAD.DWL" (see below)\n* backup all files on save\n* Support [USB Adapter](http://archive.worldofdragon.org/index.php?title=Dragon_32/64_Drivewire_Adapter) and [Becker TCP/IP Interface](http://www.6809.org.uk/xroar/doc/xroar.shtml#Becker-port).\n\n### current state\n\nTested DWEEBS:\n\n| DWEEB      | example                     | Description                                  |\n| ---------- | --------------------------- | -------------------------------------------- |\n| **DLOAD**  | `DLOAD`                     | Load `AUTOLOAD.DWL` (Used on Dragon startup) |\n| **SAVE**   | `DLOAD"SAVE""MYFILE.BAS"`   | Save BASIC listing                           |\n| **RESAVE** | `DLOAD"RESAVE""MYFILE.BAS"` | Save BASIC listing                           |\n\nImplemented DriveWire Transactions:\n\n| hex | dez | DW name           | Description                                                              |\n|-----| --- | ----------------- | ------------------------------------------------------------------------ |\n| $00 | 0   | OP_NOP            | NOP Transaction -> ignored                                               |\n| $01 | 1   | OP_NAMEOBJ_MOUNT  | Mount a file to a virtual drive number                                   |\n| $02 | 2   | OP_NAMEOBJ_CREATE | (Does in this implementation the same as OP_NAMEOBJ_MOUNT)               |\n| $d2 | 210 | OP_READEX         | Send 256 bytes sector from the DWLOAD server to the client               |\n| $57 | 87  | OP_WRITE          | Write 256 bytes sector of data from the client into a file on the server |\n\n### TODO\n\n* enhance `AUTOLOAD.DWL.py`, see: [http://archive.worldofdragon.org/phpBB3/viewtopic.php?f=5&t=4977](http://archive.worldofdragon.org/phpBB3/viewtopic.php?f=5&t=4977)\n* compare checksum\n* write unittests\n\n### pyscripts\n\nThere is a general machanism to generate DLOAD responses via Python:\n\n* Store in server root a python script, e.g.: "FOO.BAR.py"\n* DLOAD the file (without .py extension) on client, e.g.: `DLOAD"FOO.BAR"`\n\nThe script will be called via subprocess and it must write the Dragon DOS binary data back to stdout.\n\nCurrently, there is only one _pyscript_ file: `AUTOLOAD.DWL.py` (see below)\n\n#### dynamic "AUTOLOAD.DWL"\n\nThere exist a way to generate a dynamic DWLOAD menu.\nJust copy the file [/dwload-demo-files/AUTOLOAD.DWL.py](https://github.com/6809/DwLoadServer/blob/master/dwload-demo-files/AUTOLOAD.DWL.py) into your server root.\n\nThe _pyscript_ reads the server root directory and list all files into the DLOAD menu.\ne.g. the server root looks like this:\n```\n/HOME/FOO/DWLOAD-FILES\n  +--- AUTOLOAD.DWL.py\n  +--- HEXVIEW.BAS\n  +--- TEST.BAS\n  \\--- SAVE\n```\n\nThe generated listing looks like this:\n```\n10 CLS\n20 PRINT" *** DYNAMIC MENU ***  14:11:18"\n30 PRINT"/HOME/FOO/DWLOAD-FILES"\n40 PRINT" 0 - HEXVIEW.BAS"\n50 PRINT" 1 - TEST.BAS"\n60 PRINT" 2 - SAVE"\n70 PRINT"PLEASE SELECT (X FOR RELOAD) !"\n80 A$=INKEY$:IF A$="" GOTO 80\n90 IF A$="X" THEN DLOAD\n100 IF A$="0" THEN DLOAD"HEXVIEW.BAS"\n110 IF A$="1" THEN DLOAD"TEST.BAS"\n120 IF A$="2" THEN DLOAD"SAVE"\n130 GOTO 10\n```\n\ns.: [http://archive.worldofdragon.org/phpBB3/viewtopic.php?f=5&t=4977](http://archive.worldofdragon.org/phpBB3/viewtopic.php?f=5&t=4977)\n\nYou must only call **DLOAD** on you Dragon to get this menu. Because a **DLOAD** will request **AUTOLOAD.DWL** and the Python server will all **.py** and call **AUTOLOAD.DWL.py** if exist.\n\nThis feature make the following file:\n\n| [/dwload_server/hooks/dynamic_dwl.py](https://github.com/6809/DwLoadServer/blob/master/dwload_server/hooks/dynamic_dwl.py)           | general API to \'pyscript\' files |\n| [/dwload_server/pyscripts/autoload_dwl.py](https://github.com/6809/DwLoadServer/blob/master/dwload_server/pyscripts/autoload_dwl.py) | generates the DWLOAD menu       |\n\n### on-the-fly converting ASCII BASIC listing\n\nThe server read/save ASCII BASIC listing and send/store them to the DWLOAD client on-the-fly.\nSo you can edit listings on your PC and try them on your Dragon without any external conventions!\n\ne.g.: save\n```\n10 PRINT"HELLO WORLD!"\nDLOAD"SAVE""HELLO.BAS"\nDWLOAD\n!\nOK\n```\n\nThe server will create two files:\n\n| filename  | format               | description                                                      |\n| --------- | -------------------- | ---------------------------------------------------------------- |\n| HELLO.DWL | raw tokenized binary | Dragon DOS Binary Format data from the Dragon (256 Bytes padded) |\n| HELLO.BAS | ASCII listing        | on-the-fly converted ASCII BASIC listing                         |\n\ne.g. load (and execute):\n```\nDLOAD"HELLO.BAS"\n!HELLO WORLD!\nOK\n```\n\n(Note: the first `!` is from DWLOAD ROM routine)\n\nThe server will read the `HELLO.BAS` ASCII listing and convert is on-the-fly to the needed Dragon DOS Binary Format\nand send this back to the Dragon.\n\nThis feature make the following files:\n\n| [/dwload_server/hooks/read_ascii.py](https://github.com/6809/DwLoadServer/blob/master/dwload_server/hooks/read_ascii.py) | read ASCII listing and send as binary to client |\n| [/dwload_server/hooks/save_ascii.py](https://github.com/6809/DwLoadServer/blob/master/dwload_server/hooks/save_ascii.py) | save binary from client as ASCII on server      |\n\n## installation\n\nClone sources and bootstrap via [dev-shell](https://github.com/jedie/dev-shell), e.g.:\n\n```bash\n~$ git clone https://github.com/6809/DwLoadServer.git\n~$ cd DwLoadServer\n~/DwLoadServer$ ./devshell.py\n\n...\n\nDeveloper shell - DWLOAD Server - v0.4.0\n\n\nDocumented commands (use \'help -v\' for verbose/\'help <topic>\' for details):\n\ndev-shell commands\n==================\nfix_code_style      poetry   pytest     tox\nlist_venv_packages  publish  pyupgrade  update\n\nDWLOAD Server Commands\n======================\nrun\n\nUncategorized\n=============\nalias  help  history  macro  quit  set  shortcuts\n\n\n(dwload_server) run --help\nUsage: run [-h] [--root-dir ROOT_DIR] [--log-level {0, 10, 20, 30, 30, 40, 50, 50, 99, 100}] {becker, serial} ...\n\noptional arguments:\n  -h, --help            show this help message and exit\n  --root-dir ROOT_DIR\n  --log-level {0, 10, 20, 30, 30, 40, 50, 50, 99, 100}\n                        Logging level: 10=DEBUG, 20=INFO, 30=WARNING, 40=ERROR, 50=CRITICAL/FATAL (default: 20)\n\nInterface:\n  {becker, serial}\n    becker              Use the Becker interface\n    serial              Use the serial interface\n\n(dwload_server) run serial\n```\n\nYou can also run as cli, e.g.: Start serial DWLOAD server:\n```bash\n~/DwLoadServer$ ./devshell.py run serial\n```\n\n\n## History\n\n* [**dev**](https://github.com/6809/DwLoadServer/compare/v0.5.0...main)\n  * ...tbc...\n* [11.09.2022 - v0.5.0](https://github.com/6809/DwLoadServer/compare/v0.4.0...v0.5.0)\n  * Modernize project\n  * Easier bootstrap via dev-shell\n* [20.11.2014 - v0.4.0](https://github.com/6809/DwLoadServer/compare/v0.3.0...v0.4.0)\n  * dynamic `AUTOLOAD.DWL` via Python script\n* [19.11.2014 - v0.3.0](https://github.com/6809/DwLoadServer/compare/v0.2.0...v0.3.0)\n  * Convert "ASCII BASIC listing" <-> "Dragon DOS Binary" on-the-fly while read/write\n* [17.11.2014 - v0.2.0](https://github.com/6809/DwLoadServer/compare/v0.1.1...v0.2.0)\n  * Support Becker and Serial interface.\n* 14.11.2014 - v0.1.0 - Create bootstrap file that work under linux and windows.\n* 12.11.2014 - v0.0.1 - send a file works rudimentary\n* 30.09.2014 - Idea was born: [Forum post 11893](http://archive.worldofdragon.org/phpBB3/viewtopic.php?f=8&t=4946#p11893)\n\n## Links\n\n|                   |                                                                                                                                                                                   |\n|-------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|\n| Forum Thread (en) | [worldofdragon.org](https://archive.worldofdragon.org/phpBB3/viewtopic.php?f=8&t=4946)                                                                                            |\n| Forum Thread (de) | [forum.classic-computing.de](https://forum.classic-computing.de/forum/index.php?thread/20839-dwload-drivewire-for-everybody-daten%C3%BCbertragung-pc-dragon-32-64/&postID=245227) |\n| PyPi              | [https://pypi.python.org/pypi/dwload_server/](https://pypi.python.org/pypi/dwload_server/)                                                                                        |\n| Github            | [https://github.com/6809/DwLoadServer](https://github.com/6809/DwLoadServer)                                                                                                      |\n\nsome project related links:\n\n* About DWLOAD: [http://archive.worldofdragon.org/phpBB3/viewtopic.php?f=5&t=4964](http://archive.worldofdragon.org/phpBB3/viewtopic.php?f=5&t=4964)\n* DWEEBS application Thread: [http://archive.worldofdragon.org/phpBB3/viewtopic.php?f=5&t=4968](http://archive.worldofdragon.org/phpBB3/viewtopic.php?f=5&t=4968)\n* Dragon 32/64 DriveWire Adapter: [http://archive.worldofdragon.org/index.php?title=Dragon_32/64_Drivewire_Adapter](http://archive.worldofdragon.org/index.php?title=Dragon_32/64_Drivewire_Adapter)\n* Drivewire for dummies: [http://archive.worldofdragon.org/index.php?title=Drivewire_for_dummies](http://archive.worldofdragon.org/index.php?title=Drivewire_for_dummies)\n* [http://sourceforge.net/p/drivewireserver/wiki/DriveWire_Specification/](http://sourceforge.net/p/drivewireserver/wiki/DriveWire_Specification/)\n* [http://sourceforge.net/p/drivewireserver/wiki/](http://sourceforge.net/p/drivewireserver/wiki/)\n',
-    'author': 'JensDiemer',
-    'author_email': 'dwload_server@jensdiemer.de',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/6809/DwLoadServer',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
+# DWLOAD Server
 
+DWLOAD server implemented in Python (OpenSource, GPL v3 or above).
+
+Connect your Dragon 32 into your PC and LOAD/SAVE basic listings.
+
+![Dragon32DriveWire1small.jpeg](https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/DwLoadServer/Dragon32DriveWire1small.jpeg "Dragon32DriveWire1small.jpeg")
+
+
+## Quickstart
+
+```bash
+~$ git clone https://github.com/6809/DwLoadServer.git
+~$ cd DwLoadServer
+~/DwLoadServer$ ./devshell.py run serial
+```
+
+
+## features
+
+* load/save files via DWLOAD
+* on-the-fly converting ASCII BASIC listing (see below)
+* dynamic "AUTOLOAD.DWL" (see below)
+* backup all files on save
+* Support [USB Adapter](http://archive.worldofdragon.org/index.php?title=Dragon_32/64_Drivewire_Adapter) and [Becker TCP/IP Interface](http://www.6809.org.uk/xroar/doc/xroar.shtml#Becker-port).
+
+### current state
+
+Tested DWEEBS:
+
+| DWEEB      | example                     | Description                                  |
+| ---------- | --------------------------- | -------------------------------------------- |
+| **DLOAD**  | `DLOAD`                     | Load `AUTOLOAD.DWL` (Used on Dragon startup) |
+| **SAVE**   | `DLOAD"SAVE""MYFILE.BAS"`   | Save BASIC listing                           |
+| **RESAVE** | `DLOAD"RESAVE""MYFILE.BAS"` | Save BASIC listing                           |
+
+Implemented DriveWire Transactions:
+
+| hex | dez | DW name           | Description                                                              |
+|-----| --- | ----------------- | ------------------------------------------------------------------------ |
+| $00 | 0   | OP_NOP            | NOP Transaction -> ignored                                               |
+| $01 | 1   | OP_NAMEOBJ_MOUNT  | Mount a file to a virtual drive number                                   |
+| $02 | 2   | OP_NAMEOBJ_CREATE | (Does in this implementation the same as OP_NAMEOBJ_MOUNT)               |
+| $d2 | 210 | OP_READEX         | Send 256 bytes sector from the DWLOAD server to the client               |
+| $57 | 87  | OP_WRITE          | Write 256 bytes sector of data from the client into a file on the server |
+
+### TODO
+
+* enhance `AUTOLOAD.DWL.py`, see: [http://archive.worldofdragon.org/phpBB3/viewtopic.php?f=5&t=4977](http://archive.worldofdragon.org/phpBB3/viewtopic.php?f=5&t=4977)
+* compare checksum
+* write unittests
+
+### pyscripts
+
+There is a general machanism to generate DLOAD responses via Python:
+
+* Store in server root a python script, e.g.: "FOO.BAR.py"
+* DLOAD the file (without .py extension) on client, e.g.: `DLOAD"FOO.BAR"`
+
+The script will be called via subprocess and it must write the Dragon DOS binary data back to stdout.
+
+Currently, there is only one _pyscript_ file: `AUTOLOAD.DWL.py` (see below)
+
+#### dynamic "AUTOLOAD.DWL"
+
+There exist a way to generate a dynamic DWLOAD menu.
+Just copy the file [/dwload-demo-files/AUTOLOAD.DWL.py](https://github.com/6809/DwLoadServer/blob/master/dwload-demo-files/AUTOLOAD.DWL.py) into your server root.
+
+The _pyscript_ reads the server root directory and list all files into the DLOAD menu.
+e.g. the server root looks like this:
+```
+/HOME/FOO/DWLOAD-FILES
+  +--- AUTOLOAD.DWL.py
+  +--- HEXVIEW.BAS
+  +--- TEST.BAS
+  \--- SAVE
+```
+
+The generated listing looks like this:
+```
+10 CLS
+20 PRINT" *** DYNAMIC MENU ***  14:11:18"
+30 PRINT"/HOME/FOO/DWLOAD-FILES"
+40 PRINT" 0 - HEXVIEW.BAS"
+50 PRINT" 1 - TEST.BAS"
+60 PRINT" 2 - SAVE"
+70 PRINT"PLEASE SELECT (X FOR RELOAD) !"
+80 A$=INKEY$:IF A$="" GOTO 80
+90 IF A$="X" THEN DLOAD
+100 IF A$="0" THEN DLOAD"HEXVIEW.BAS"
+110 IF A$="1" THEN DLOAD"TEST.BAS"
+120 IF A$="2" THEN DLOAD"SAVE"
+130 GOTO 10
+```
+
+s.: [http://archive.worldofdragon.org/phpBB3/viewtopic.php?f=5&t=4977](http://archive.worldofdragon.org/phpBB3/viewtopic.php?f=5&t=4977)
+
+You must only call **DLOAD** on you Dragon to get this menu. Because a **DLOAD** will request **AUTOLOAD.DWL** and the Python server will all **.py** and call **AUTOLOAD.DWL.py** if exist.
+
+This feature make the following file:
+
+| [/dwload_server/hooks/dynamic_dwl.py](https://github.com/6809/DwLoadServer/blob/master/dwload_server/hooks/dynamic_dwl.py)           | general API to 'pyscript' files |
+| [/dwload_server/pyscripts/autoload_dwl.py](https://github.com/6809/DwLoadServer/blob/master/dwload_server/pyscripts/autoload_dwl.py) | generates the DWLOAD menu       |
+
+### on-the-fly converting ASCII BASIC listing
+
+The server read/save ASCII BASIC listing and send/store them to the DWLOAD client on-the-fly.
+So you can edit listings on your PC and try them on your Dragon without any external conventions!
+
+e.g.: save
+```
+10 PRINT"HELLO WORLD!"
+DLOAD"SAVE""HELLO.BAS"
+DWLOAD
+!
+OK
+```
+
+The server will create two files:
+
+| filename  | format               | description                                                      |
+| --------- | -------------------- | ---------------------------------------------------------------- |
+| HELLO.DWL | raw tokenized binary | Dragon DOS Binary Format data from the Dragon (256 Bytes padded) |
+| HELLO.BAS | ASCII listing        | on-the-fly converted ASCII BASIC listing                         |
+
+e.g. load (and execute):
+```
+DLOAD"HELLO.BAS"
+!HELLO WORLD!
+OK
+```
+
+(Note: the first `!` is from DWLOAD ROM routine)
+
+The server will read the `HELLO.BAS` ASCII listing and convert is on-the-fly to the needed Dragon DOS Binary Format
+and send this back to the Dragon.
+
+This feature make the following files:
+
+| [/dwload_server/hooks/read_ascii.py](https://github.com/6809/DwLoadServer/blob/master/dwload_server/hooks/read_ascii.py) | read ASCII listing and send as binary to client |
+| [/dwload_server/hooks/save_ascii.py](https://github.com/6809/DwLoadServer/blob/master/dwload_server/hooks/save_ascii.py) | save binary from client as ASCII on server      |
+
+## installation
+
+Clone sources and bootstrap via [dev-shell](https://github.com/jedie/dev-shell), e.g.:
+
+```bash
+~$ git clone https://github.com/6809/DwLoadServer.git
+~$ cd DwLoadServer
+~/DwLoadServer$ ./devshell.py
+
+...
+
+Developer shell - DWLOAD Server - v0.4.0
+
+
+Documented commands (use 'help -v' for verbose/'help <topic>' for details):
+
+dev-shell commands
+==================
+fix_code_style      poetry   pytest     tox
+list_venv_packages  publish  pyupgrade  update
+
+DWLOAD Server Commands
+======================
+run
+
+Uncategorized
+=============
+alias  help  history  macro  quit  set  shortcuts
+
+
+(dwload_server) run --help
+Usage: run [-h] [--root-dir ROOT_DIR] [--log-level {0, 10, 20, 30, 30, 40, 50, 50, 99, 100}] {becker, serial} ...
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --root-dir ROOT_DIR
+  --log-level {0, 10, 20, 30, 30, 40, 50, 50, 99, 100}
+                        Logging level: 10=DEBUG, 20=INFO, 30=WARNING, 40=ERROR, 50=CRITICAL/FATAL (default: 20)
+
+Interface:
+  {becker, serial}
+    becker              Use the Becker interface
+    serial              Use the serial interface
+
+(dwload_server) run serial
+```
+
+You can also run as cli, e.g.: Start serial DWLOAD server:
+```bash
+~/DwLoadServer$ ./devshell.py run serial
+```
+
+
+## History
+
+* [**dev**](https://github.com/6809/DwLoadServer/compare/v0.5.0...main)
+  * ...tbc...
+* [11.09.2022 - v0.5.0](https://github.com/6809/DwLoadServer/compare/v0.4.0...v0.5.0)
+  * Modernize project
+  * Easier bootstrap via dev-shell
+* [20.11.2014 - v0.4.0](https://github.com/6809/DwLoadServer/compare/v0.3.0...v0.4.0)
+  * dynamic `AUTOLOAD.DWL` via Python script
+* [19.11.2014 - v0.3.0](https://github.com/6809/DwLoadServer/compare/v0.2.0...v0.3.0)
+  * Convert "ASCII BASIC listing" <-> "Dragon DOS Binary" on-the-fly while read/write
+* [17.11.2014 - v0.2.0](https://github.com/6809/DwLoadServer/compare/v0.1.1...v0.2.0)
+  * Support Becker and Serial interface.
+* 14.11.2014 - v0.1.0 - Create bootstrap file that work under linux and windows.
+* 12.11.2014 - v0.0.1 - send a file works rudimentary
+* 30.09.2014 - Idea was born: [Forum post 11893](http://archive.worldofdragon.org/phpBB3/viewtopic.php?f=8&t=4946#p11893)
+
+## Links
+
+|                   |                                                                                                                                                                                   |
+|-------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| Forum Thread (en) | [worldofdragon.org](https://archive.worldofdragon.org/phpBB3/viewtopic.php?f=8&t=4946)                                                                                            |
+| Forum Thread (de) | [forum.classic-computing.de](https://forum.classic-computing.de/forum/index.php?thread/20839-dwload-drivewire-for-everybody-daten%C3%BCbertragung-pc-dragon-32-64/&postID=245227) |
+| PyPi              | [https://pypi.python.org/pypi/dwload_server/](https://pypi.python.org/pypi/dwload_server/)                                                                                        |
+| Github            | [https://github.com/6809/DwLoadServer](https://github.com/6809/DwLoadServer)                                                                                                      |
+
+some project related links:
+
+* About DWLOAD: [http://archive.worldofdragon.org/phpBB3/viewtopic.php?f=5&t=4964](http://archive.worldofdragon.org/phpBB3/viewtopic.php?f=5&t=4964)
+* DWEEBS application Thread: [http://archive.worldofdragon.org/phpBB3/viewtopic.php?f=5&t=4968](http://archive.worldofdragon.org/phpBB3/viewtopic.php?f=5&t=4968)
+* Dragon 32/64 DriveWire Adapter: [http://archive.worldofdragon.org/index.php?title=Dragon_32/64_Drivewire_Adapter](http://archive.worldofdragon.org/index.php?title=Dragon_32/64_Drivewire_Adapter)
+* Drivewire for dummies: [http://archive.worldofdragon.org/index.php?title=Drivewire_for_dummies](http://archive.worldofdragon.org/index.php?title=Drivewire_for_dummies)
+* [http://sourceforge.net/p/drivewireserver/wiki/DriveWire_Specification/](http://sourceforge.net/p/drivewireserver/wiki/DriveWire_Specification/)
+* [http://sourceforge.net/p/drivewireserver/wiki/](http://sourceforge.net/p/drivewireserver/wiki/)
 
-setup(**setup_kwargs)
```

