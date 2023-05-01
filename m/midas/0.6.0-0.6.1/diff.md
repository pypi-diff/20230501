# Comparing `tmp/midas-0.6.0.tar.gz` & `tmp/midas-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midas-0.6.0.tar", last modified: Fri Mar 10 04:29:15 2023, max compression
+gzip compressed data, was "midas-0.6.1.tar", last modified: Mon May  1 20:37:34 2023, max compression
```

## Comparing `midas-0.6.0.tar` & `midas-0.6.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-03-10 04:29:15.896453 midas-0.6.0/
--rw-r--r--   0 a.ruddick   (502) staff       (20)       59 2022-11-16 23:14:07.000000 midas-0.6.0/.gitignore
--rw-r--r--   0 a.ruddick   (502) staff       (20)    18027 2023-03-06 23:12:30.000000 midas-0.6.0/LICENSE
--rw-r--r--   0 a.ruddick   (502) staff       (20)     3205 2023-03-10 04:29:15.896519 midas-0.6.0/PKG-INFO
--rw-r--r--   0 a.ruddick   (502) staff       (20)     2376 2023-03-10 04:22:14.000000 midas-0.6.0/README.md
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-03-10 04:29:15.895308 midas-0.6.0/midas/
--rw-r--r--   0 a.ruddick   (502) staff       (20)      946 2022-11-16 23:14:07.000000 midas-0.6.0/midas/__init__.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)     5844 2022-11-16 23:14:07.000000 midas-0.6.0/midas/driver.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)     4028 2021-06-30 14:46:51.000000 midas-0.6.0/midas/faults.csv
--rw-r--r--   0 a.ruddick   (502) staff       (20)     1698 2022-11-16 23:14:07.000000 midas-0.6.0/midas/mock.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)     5120 2023-03-10 04:22:14.000000 midas-0.6.0/midas/util.py
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-03-10 04:29:15.896339 midas-0.6.0/midas.egg-info/
--rw-r--r--   0 a.ruddick   (502) staff       (20)     3205 2023-03-10 04:29:15.000000 midas-0.6.0/midas.egg-info/PKG-INFO
--rw-r--r--   0 a.ruddick   (502) staff       (20)      302 2023-03-10 04:29:15.000000 midas-0.6.0/midas.egg-info/SOURCES.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)        1 2023-03-10 04:29:15.000000 midas-0.6.0/midas.egg-info/dependency_links.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)       45 2023-03-10 04:29:15.000000 midas-0.6.0/midas.egg-info/entry_points.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)      276 2023-03-10 04:29:15.000000 midas-0.6.0/midas.egg-info/requires.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)        6 2023-03-10 04:29:15.000000 midas-0.6.0/midas.egg-info/top_level.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)      172 2023-03-10 04:29:15.896761 midas-0.6.0/setup.cfg
--rw-r--r--   0 a.ruddick   (502) staff       (20)     1834 2023-03-10 04:22:18.000000 midas-0.6.0/setup.py
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-05-01 20:37:34.117861 midas-0.6.1/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)       69 2023-04-25 18:49:18.000000 midas-0.6.1/.gitignore
+-rw-r--r--   0 a.ruddick   (502) staff       (20)    18026 2023-04-10 19:06:41.000000 midas-0.6.1/LICENSE
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     3205 2023-05-01 20:37:34.117926 midas-0.6.1/PKG-INFO
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     2376 2023-03-10 04:22:14.000000 midas-0.6.1/README.md
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-05-01 20:37:34.116945 midas-0.6.1/midas/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      993 2023-05-01 20:34:55.000000 midas-0.6.1/midas/__init__.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     5904 2023-05-01 20:34:55.000000 midas-0.6.1/midas/driver.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     4028 2021-06-30 14:46:51.000000 midas-0.6.1/midas/faults.csv
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     1811 2023-05-01 20:34:55.000000 midas-0.6.1/midas/mock.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)        0 2023-05-01 20:34:55.000000 midas-0.6.1/midas/py.typed
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     5738 2023-05-01 20:34:55.000000 midas-0.6.1/midas/util.py
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-05-01 20:37:34.117732 midas-0.6.1/midas.egg-info/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     3205 2023-05-01 20:37:34.000000 midas-0.6.1/midas.egg-info/PKG-INFO
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      317 2023-05-01 20:37:34.000000 midas-0.6.1/midas.egg-info/SOURCES.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)        1 2023-05-01 20:37:34.000000 midas-0.6.1/midas.egg-info/dependency_links.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)       45 2023-05-01 20:37:34.000000 midas-0.6.1/midas.egg-info/entry_points.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      254 2023-05-01 20:37:34.000000 midas-0.6.1/midas.egg-info/requires.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)        6 2023-05-01 20:37:34.000000 midas-0.6.1/midas.egg-info/top_level.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      252 2023-05-01 20:37:34.118144 midas-0.6.1/setup.cfg
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     1804 2023-05-01 20:35:04.000000 midas-0.6.1/setup.py
```

### Comparing `midas-0.6.0/LICENSE` & `midas-0.6.1/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -333,8 +333,7 @@
   Ty Coon, President of Vice
 
 This General Public License does not permit incorporating your program into
 proprietary programs.  If your program is a subroutine library, you may
 consider it more useful to permit linking proprietary applications with the
 library.  If this is what you want to do, use the GNU Lesser General
 Public License instead of this License.
-
```

### Comparing `midas-0.6.0/PKG-INFO` & `midas-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midas
-Version: 0.6.0
+Version: 0.6.1
 Summary: Python driver for Honeywell Midas gas detectors.
 Home-page: http://github.com/numat/midas/
 Author: Patrick Fuller
 Author-email: pat@numat-tech.com
 License: GPLv2
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Development Status :: 4 - Beta
```

### Comparing `midas-0.6.0/README.md` & `midas-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `midas-0.6.0/midas/driver.py` & `midas-0.6.1/midas/driver.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,37 +58,37 @@
 
     This driver handles asynchronous Modbus TCP/IP and Midas parsing,
     returning a human-readable dictionary. In particular, this loads fault
     and boolean information specified in the manual and looks up codes so
     you don't have to.
     """
 
-    async def get(self):
+    async def get(self) -> dict:
         """Get current state from the Midas gas detector."""
         return self._parse(await self.read_registers(0, 16))
 
-    async def reset_alarms_and_faults(self):
+    async def reset_alarms_and_faults(self) -> None:
         """Reset all alarms and faults."""
         return await self.write_registers(20, (0x015E, 0x3626))
 
-    async def inhibit_alarms(self):
+    async def inhibit_alarms(self) -> None:
         """Inhibit alarms from triggering."""
         return await self.write_registers(20, (0x025E, 0x3626))
 
-    async def inhibit_alarms_and_faults(self):
+    async def inhibit_alarms_and_faults(self) -> None:
         """Inhibit alarms and faults from triggering."""
         return await self.write_registers(20, (0x035E, 0x3626))
 
-    async def remove_inhibit(self):
+    async def remove_inhibit(self) -> None:
         """Cancel the inhibit state."""
         return await self.write_registers(20, (0x055E, 0x3626))
 
-    def _parse(self, registers):
+    def _parse(self, registers: list) -> dict:
         """Parse the response, returning a dictionary."""
-        result = {'ip': self.ip, 'connected': True}
+        result: dict = {'ip': self.ip, 'connected': True}
         decoder = BinaryPayloadDecoder.fromRegisters(registers,
                                                      byteorder=Endian.Big,
                                                      wordorder=Endian.Little)
         # Register 40001 is a collection of alarm status signals
         b = [decoder.decode_bits(), decoder.decode_bits()]
         reg_40001 = b[1] + b[0]
         # Bits 0-3 map to the monitor state
```

### Comparing `midas-0.6.0/midas/faults.csv` & `midas-0.6.1/midas/faults.csv`

 * *Files identical despite different names*

### Comparing `midas-0.6.0/midas/mock.py` & `midas-0.6.1/midas/mock.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 """Mock Midas interface. Use for debugging systems."""
 
 import asyncio
 from random import random
+from typing import Any
 from unittest.mock import MagicMock
 
 from midas.driver import GasDetector as realGasDetector
 
 
 class AsyncClientMock(MagicMock):
     """Magic mock that works with async methods."""
 
-    async def __call__(self, *args, **kwargs):
+    async def __call__(self, *args, **kwargs):  # type: ignore
         """Convert regular mocks into into an async coroutine."""
         return super().__call__(*args, **kwargs)
 
 
 class GasDetector(realGasDetector):
     """Mock interface to the Midas gas detector."""
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
         """Set an inital mocked state."""
         self.client = AsyncClientMock()
         self.state = {
             "ip": "192.168.0.1",
             "connected": True,
             "state": "Monitoring",
             "fault": {"status": "No fault"},
@@ -32,27 +33,27 @@
             "temperature": 30,
             "life": 556.0833333333334,
             "flow": 482,
             "low-alarm threshold": 5,
             "high-alarm threshold": 8,
         }
 
-    def __getattr__(self, attr):
+    def __getattr__(self, attr):  # type: ignore
         """Return False for any undefined method."""
 
-        def handler(*args, **kwargs):
+        def handler(*args, **kwargs):  # type: ignore
             return False
 
         return handler
 
-    async def get(self):
+    async def get(self) -> dict:
         """Return a mock state with the same object structure."""
         await asyncio.sleep(random() * 0.1)
         return self.state
 
-    async def inhibit_alarms(self):
+    async def inhibit_alarms(self) -> None:
         """Inhibit alarms from triggering."""
         self.state["state"] = "Monitoring with alarms inhibited"
 
-    async def remove_inhibit(self):
+    async def remove_inhibit(self) -> None:
         """Cancel the inhibit state."""
         self.state["state"] = "Monitoring"
```

### Comparing `midas-0.6.0/midas/util.py` & `midas-0.6.1/midas/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,107 +1,119 @@
 """Base functionality for modbus communication.
 
 Distributed under the GNU General Public License v2
 Copyright (C) 2022 NuMat Technologies
 """
 import asyncio
+from typing import Any, Literal, Union, overload
 
 try:
     from pymodbus.client import AsyncModbusTcpClient  # 3.x
+    from pymodbus.pdu import ModbusResponse
+    from pymodbus.register_read_message import ReadHoldingRegistersResponse
 except ImportError:  # 2.4.x - 2.5.x
     from pymodbus.client.asynchronous.async_io import (  # type: ignore
-        ReconnectingAsyncioModbusTcpClient)
+        ReconnectingAsyncioModbusTcpClient,
+    )
 import pymodbus.exceptions
 
 
-class AsyncioModbusClient(object):
+class AsyncioModbusClient:
     """A generic asyncio client.
 
     This expands upon the pymodbus AsyncModbusTcpClient by
     including standard timeouts, async context manager, and queued requests.
     """
 
-    def __init__(self, address, timeout=1):
+    def __init__(self, address: str, timeout: float = 1) -> None:
         """Set up communication parameters."""
         self.ip = address
         self.timeout = timeout
         try:
             self.client = AsyncModbusTcpClient(address, timeout=timeout)  # 3.0
             self.pymodbus32plus = not hasattr(self.client, 'protocol')  # >= 3.2.0
         except NameError:
             self.client = ReconnectingAsyncioModbusTcpClient()  # 2.4.x - 2.5.x
         self.lock = asyncio.Lock()
         self.connectTask = asyncio.create_task(self._connect())
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> Any:
         """Asynchronously connect with the context manager."""
         return self
 
-    async def __aexit__(self, *args):
+    async def __aexit__(self, *args: Any) -> None:
         """Provide exit to the context manager."""
         await self._close()
 
-    async def _connect(self):
+    async def _connect(self) -> None:
         """Start asynchronous reconnect loop."""
         async with self.lock:
             try:
                 try:
                     await asyncio.wait_for(self.client.connect(), timeout=self.timeout)  # 3.x
                 except AttributeError:  # 2.4.x - 2.5.x
                     await self.client.start(self.ip)  # type: ignore
-            except Exception:
-                raise IOError(f"Could not connect to '{self.ip}'.")
+            except Exception as e:
+                raise OSError(f"Could not connect to '{self.ip}'.") from e
 
-    async def read_coils(self, address, count):
-        """Read modbus output coils (0 address prefix)."""
-        return await self._request('read_coils', address, count)
-
-    async def read_registers(self, address, count):
+    async def read_registers(self, address: int, count: int) -> list:
         """Read modbus registers.
 
         The Modbus protocol doesn't allow responses longer than 250 bytes
         (ie. 125 registers, 62 DF addresses), which this function manages by
         chunking larger requests.
         """
-        registers = []
+        registers: list = []
         while count > 124:
             r = await self._request('read_holding_registers', address, 124)
             registers += r.registers
             address, count = address + 124, count - 124
         r = await self._request('read_holding_registers', address, count)
         registers += r.registers
         return registers
 
-    async def write_coil(self, address, value):
-        """Write modbus coils."""
+    async def write_coil(self, address: int, value: bool) -> None:
+        """Write a modbus coil."""
         await self._request('write_coil', address, value)
 
-    async def write_coils(self, address, values):
+    async def write_coils(self, address: int, values: list) -> None:
         """Write modbus coils."""
         await self._request('write_coils', address, values)
 
-    async def write_register(self, address, value, skip_encode=False):
+    async def write_register(self, address: int, value: int,
+                             skip_encode: bool = False) -> None:
         """Write a modbus register."""
         await self._request('write_register', address, value, skip_encode=skip_encode)
 
-    async def write_registers(self, address, values, skip_encode=False):
+    async def write_registers(self, address: int, values: Union[list, tuple],
+                              skip_encode: bool = False) -> None:
         """Write modbus registers.
 
         The Modbus protocol doesn't allow requests longer than 250 bytes
         (ie. 125 registers, 62 DF addresses), which this function manages by
         chunking larger requests.
         """
         while len(values) > 62:
             await self._request('write_registers',
                                 address, values, skip_encode=skip_encode)
             address, values = address + 124, values[62:]
         await self._request('write_registers',
                             address, values, skip_encode=skip_encode)
 
-    async def _request(self, method, *args, **kwargs):
+    @overload
+    async def _request(self, method: Literal['read_holding_registers'],
+                       *args: Any, **kwargs: Any) -> ReadHoldingRegistersResponse:
+        ...
+
+    @overload
+    async def _request(self, method: str,
+                       *args: Any, **kwargs: Any) -> ModbusResponse:
+        ...
+
+    async def _request(self, method: str, *args: Any, **kwargs: Any) -> ModbusResponse:
         """Send a request to the device and awaits a response.
 
         This mainly ensures that requests are sent serially, as the Modbus
         protocol does not allow simultaneous requests (it'll ignore any
         request sent while it's processing something). The driver handles this
         by assuming there is only one client instance. If other clients
         exist, other logic will have to be added to either prevent or manage
@@ -113,16 +125,16 @@
                 raise ConnectionError("Not connected to Midas.")
             try:
                 if self.pymodbus32plus:
                     future = getattr(self.client, method)
                 else:
                     future = getattr(self.client.protocol, method)  # type: ignore
                 return await future(*args, **kwargs)
-            except (asyncio.TimeoutError, pymodbus.exceptions.ConnectionException):
-                raise TimeoutError("Not connected to Midas.")
+            except (asyncio.TimeoutError, pymodbus.exceptions.ConnectionException) as e:
+                raise TimeoutError("Not connected to Midas.") from e
 
-    async def _close(self):
+    async def _close(self) -> None:
         """Close the TCP connection."""
         try:
             await self.client.close()  # 3.x
         except AttributeError:  # 2.4.x - 2.5.x
             self.client.stop()  # type: ignore
```

### Comparing `midas-0.6.0/midas.egg-info/PKG-INFO` & `midas-0.6.1/midas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midas
-Version: 0.6.0
+Version: 0.6.1
 Summary: Python driver for Honeywell Midas gas detectors.
 Home-page: http://github.com/numat/midas/
 Author: Patrick Fuller
 Author-email: pat@numat-tech.com
 License: GPLv2
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Development Status :: 4 - Beta
```

### Comparing `midas-0.6.0/setup.py` & `midas-0.6.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,42 +2,41 @@
 from sys import version_info
 
 from setuptools import setup
 
 if version_info < (3, 8):
     raise ImportError("This module requires Python >=3.8.  Use 0.5.1 for Python3.7")
 
-with open('README.md', 'r') as in_file:
+with open('README.md') as in_file:
     long_description = in_file.read()
 
 setup(
     name="midas",
-    version="0.6.0",
+    version="0.6.1",
     description="Python driver for Honeywell Midas gas detectors.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="http://github.com/numat/midas/",
     author="Patrick Fuller",
     author_email="pat@numat-tech.com",
     packages=['midas'],
-    package_data={'midas': ['faults.csv']},
+    package_data={'midas': ['faults.csv', 'py.typed']},
     install_requires=[
         'pymodbus>=2.4.0,<3; python_version == "3.7"',
         'pymodbus>=2.4.0; python_version == "3.8"',
         'pymodbus>=2.4.0; python_version == "3.9"',
         'pymodbus>=3.0.2,<3.3.0; python_version >= "3.10"',
     ],
     extras_require={
         'test': [
-            'flake8>=3,<7',
-            'flake8-docstrings==1.*',
             'mypy>=1.1.1',
             'pytest',
             'pytest-cov',
             'pytest-asyncio',
+            'ruff==0.0.263',
         ],
     },
     entry_points={
         'console_scripts': [('midas = midas:command_line')]
     },
     license='GPLv2',
     classifiers=[
```

