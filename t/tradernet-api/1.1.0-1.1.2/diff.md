# Comparing `tmp/tradernet_api-1.1.0.tar.gz` & `tmp/tradernet_api-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tradernet_api-1.1.0.tar", max compression
+gzip compressed data, was "tradernet_api-1.1.2.tar", max compression
```

## Comparing `tradernet_api-1.1.0.tar` & `tradernet_api-1.1.2.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0     1080 2022-08-24 22:26:52.698920 tradernet_api-1.1.0/LICENSE
--rw-r--r--   0        0        0     2739 2022-08-24 22:26:52.698920 tradernet_api-1.1.0/README.md
--rw-r--r--   0        0        0     2796 2022-08-24 22:26:52.698920 tradernet_api-1.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-08-24 22:26:52.698920 tradernet_api-1.1.0/tradernet_api/__init__.py
--rw-r--r--   0        0        0      600 2022-08-24 22:26:52.698920 tradernet_api-1.1.0/tradernet_api/api.py
--rw-r--r--   0        0        0     3045 2022-08-24 22:26:52.698920 tradernet_api-1.1.0/tradernet_api/client.py
--rw-r--r--   0        0        0      394 2022-08-24 22:26:52.698920 tradernet_api-1.1.0/tradernet_api/commands/__init__.py
--rw-r--r--   0        0        0      529 2022-08-24 22:26:52.698920 tradernet_api-1.1.0/tradernet_api/commands/delete_order.py
--rw-r--r--   0        0        0      614 2022-08-24 22:26:52.698920 tradernet_api-1.1.0/tradernet_api/commands/get_orders.py
--rw-r--r--   0        0        0      735 2022-08-24 22:26:52.698920 tradernet_api-1.1.0/tradernet_api/commands/get_ticker_info.py
--rw-r--r--   0        0        0     1545 2022-08-24 22:26:52.698920 tradernet_api-1.1.0/tradernet_api/commands/send_order.py
--rw-r--r--   0        0        0      824 2022-08-24 22:26:52.698920 tradernet_api-1.1.0/tradernet_api/commands/set_stop_order.py
--rw-r--r--   0        0        0     1674 2022-08-24 22:26:52.698920 tradernet_api-1.1.0/tradernet_api/const.py
--rw-r--r--   0        0        0        0 2022-08-24 22:26:52.698920 tradernet_api-1.1.0/tradernet_api/models/__init__.py
--rw-r--r--   0        0        0     4199 2022-08-24 22:26:52.698920 tradernet_api-1.1.0/tradernet_api/models/command_model.py
--rw-r--r--   0        0        0      559 2022-08-24 22:26:52.698920 tradernet_api-1.1.0/tradernet_api/models/request_model.py
--rw-r--r--   0        0        0       46 2022-08-24 22:26:52.698920 tradernet_api-1.1.0/tradernet_api/session.py
--rw-r--r--   0        0        0     3544 2022-08-24 22:27:21.128978 tradernet_api-1.1.0/setup.py
--rw-r--r--   0        0        0     3244 2022-08-24 22:27:21.129316 tradernet_api-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-05-01 11:10:08.697760 tradernet_api-1.1.2/LICENSE
+-rw-r--r--   0        0        0     2739 2023-05-01 11:10:08.697760 tradernet_api-1.1.2/README.md
+-rw-r--r--   0        0        0     2775 2023-05-01 11:10:08.697760 tradernet_api-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-01 11:10:08.701760 tradernet_api-1.1.2/tradernet_api/__init__.py
+-rw-r--r--   0        0        0      600 2023-05-01 11:10:08.701760 tradernet_api-1.1.2/tradernet_api/api.py
+-rw-r--r--   0        0        0     3053 2023-05-01 11:10:08.701760 tradernet_api-1.1.2/tradernet_api/client.py
+-rw-r--r--   0        0        0      394 2023-05-01 11:10:08.701760 tradernet_api-1.1.2/tradernet_api/commands/__init__.py
+-rw-r--r--   0        0        0      580 2023-05-01 11:10:08.701760 tradernet_api-1.1.2/tradernet_api/commands/delete_order.py
+-rw-r--r--   0        0        0      658 2023-05-01 11:10:08.701760 tradernet_api-1.1.2/tradernet_api/commands/get_orders.py
+-rw-r--r--   0        0        0      787 2023-05-01 11:10:08.701760 tradernet_api-1.1.2/tradernet_api/commands/get_ticker_info.py
+-rw-r--r--   0        0        0     1594 2023-05-01 11:10:08.701760 tradernet_api-1.1.2/tradernet_api/commands/send_order.py
+-rw-r--r--   0        0        0      879 2023-05-01 11:10:08.701760 tradernet_api-1.1.2/tradernet_api/commands/set_stop_order.py
+-rw-r--r--   0        0        0     1683 2023-05-01 11:10:08.701760 tradernet_api-1.1.2/tradernet_api/const.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:10:08.701760 tradernet_api-1.1.2/tradernet_api/models/__init__.py
+-rw-r--r--   0        0        0     4199 2023-05-01 11:10:08.701760 tradernet_api-1.1.2/tradernet_api/models/command_model.py
+-rw-r--r--   0        0        0      559 2023-05-01 11:10:08.701760 tradernet_api-1.1.2/tradernet_api/models/request_model.py
+-rw-r--r--   0        0        0       46 2023-05-01 11:10:08.701760 tradernet_api-1.1.2/tradernet_api/session.py
+-rw-r--r--   0        0        0     3295 1970-01-01 00:00:00.000000 tradernet_api-1.1.2/PKG-INFO
```

### Comparing `tradernet_api-1.1.0/LICENSE` & `tradernet_api-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tradernet_api-1.1.0/README.md` & `tradernet_api-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `tradernet_api-1.1.0/pyproject.toml` & `tradernet_api-1.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 [tool.poetry]
 name = "tradernet_api"
-version = "1.1.0"
+version = "1.1.2"
 description = "Public API client for working with the Tradernet platform."
 readme = "README.md"
 authors = ["Artur Kutsevol <arthur.kutsevol@gmail.com>"]
 license = "MIT"
 include = ["LICENSE",]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 requests = "^2.27.1"
 pydantic = "^1.9.1"
 
 [tool.poetry.dev-dependencies]
-pre-commit = "^2.19.0"
-pytest = "^7.1.2"
-Faker = "^14.1.0"
-requests-mock = "^1.9.3"
-safety = "^2.1.1"
-bandit = "^1.7.4"
-pytest-cov = "^3.0.0"
-pytest-html = "^3.1.1"
+pre-commit = "^3.0.0"
+pytest = "^7.2.0"
+Faker = "^18.2.0"
+requests-mock = "^1.10.0"
+bandit = "^1.7.5"
+pytest-cov = "^4.0.0"
+pytest-html = "^3.2.0"
 coverage-badge = "^1.1.0"
 isort = {extras = ["colors"], version = "^5.10.1"}
-black = {version = "^22.3.0", allow-prereleases = true}
+black = {version = "^23.3.0", allow-prereleases = true}
 darglint = "^1.8.1"
-mypy = "^0.960"
-pyupgrade = "^2.32.1"
+mypy = "^1.0"
+pyupgrade = "^3.0.0"
 pydocstyle = "^6.1.1"
-pylint = "^2.13.9"
-coverage = "^6.4"
-poetry-types = "^0.2.2"
+pylint = "^2.17.3"
+coverage = "^7.0"
+poetry-types = "^0.3.6"
 
 [tool.black]
 # https://github.com/psf/black
 target-version = ["py310"]
 line-length = 88
 color = true
```

### Comparing `tradernet_api-1.1.0/tradernet_api/api.py` & `tradernet_api-1.1.2/tradernet_api/api.py`

 * *Files identical despite different names*

### Comparing `tradernet_api-1.1.0/tradernet_api/client.py` & `tradernet_api-1.1.2/tradernet_api/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from typing import Mapping
-
 import hashlib
 import hmac
 import time
+from collections.abc import Mapping
 from dataclasses import dataclass
 
 from requests import Response
 
 from tradernet_api.const import api_url
 from tradernet_api.models.request_model import RequestV1, RequestV2
 from tradernet_api.session import session
```

### Comparing `tradernet_api-1.1.0/tradernet_api/commands/delete_order.py` & `tradernet_api-1.1.2/tradernet_api/commands/delete_order.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from typing import Any
 
+from tradernet_api.const import Command
 from tradernet_api.models.command_model import DeleteOrderModel
 
 
 def delete_order(self: Any, order_id: str) -> Any:
     """
     Delete/cancel order
     https://tradernet.com/tradernet-api/orders-delete
 
     :param self: binds with API class
     :param order_id: ID of the order that we want to cancel
     :return: Response
     """
-    command_name = "delTradeOrder"
+    command_name = Command.delete_order.value
 
     order_param = DeleteOrderModel(order_id=order_id)
 
     return self._client_v2.send_request(command=command_name, params=order_param)
```

### Comparing `tradernet_api-1.1.0/tradernet_api/commands/get_orders.py` & `tradernet_api-1.1.2/tradernet_api/commands/get_orders.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from typing import Any
 
+from tradernet_api.const import Command
 from tradernet_api.models.command_model import GetOrdersModel
 
 
 def get_orders(self: Any, active_only: bool | None = True) -> Any:
     """
     Receive orders in the current period and subscribe for changes.
     https://tradernet.com/tradernet-api/orders-get-current-history
 
     :param self: binds with API class
     :param active_only: 1/0 We show only active orders. Optional
     :return: Response
     """
-    command_name = "getNotifyOrderJson"
+    command_name = Command.get_orders.value
 
     order_param = GetOrdersModel(active_only=active_only)
 
     return self._client_v2.send_request(command=command_name, params=order_param)
```

### Comparing `tradernet_api-1.1.0/tradernet_api/commands/get_ticker_info.py` & `tradernet_api-1.1.2/tradernet_api/commands/get_ticker_info.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from typing import Any
 
+from tradernet_api.const import Command
 from tradernet_api.models.command_model import GetTickerInfoModel
 
 
 def get_ticker_info(self: Any, ticker: str, sup: bool | None = False) -> Any:
     """
     Retrieving ticker data from the server.
     https://tradernet.com/tradernet-api/quotes-get-info
 
     :param self: binds with API class
     :param ticker: the name of the ticker, required to retrieve data from the server
     :param sup: IMS and trading system format. Optional
     :return: Response (https://tradernet.com/tradernet-api/securities)
     """
-    command_name = "getSecurityInfo"
+    command_name = Command.get_ticker_info.value
 
     order_param = GetTickerInfoModel(ticker=f"{ticker}.US".upper(), sup=sup)
 
     return self._client_v1.send_request(command=command_name, params=order_param)
```

### Comparing `tradernet_api-1.1.0/tradernet_api/commands/send_order.py` & `tradernet_api-1.1.2/tradernet_api/commands/send_order.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Any
 
+from tradernet_api.const import Command
 from tradernet_api.models.command_model import SendOrderModel
 
 
 def send_order(
     self: Any,
     ticker: str,
     side: str,
@@ -28,15 +29,15 @@
                       `gtc` - good-til-cancelled, until the order is completed or canceled
     :param market_order: Execute market order (optional)
     :param limit_price: Price for limit order (optional)
     :param stop_price: Price for stop order (optional)
 
     :return: Response
     """
-    command_name = "putTradeOrder"
+    command_name = Command.send_order.value
 
     order_param = SendOrderModel(
         instr_name=f"{ticker}.US".upper(),
         side=side,
         margin=margin,
         qty=count,
         expiry=order_exp,
```

### Comparing `tradernet_api-1.1.0/tradernet_api/commands/set_stop_order.py` & `tradernet_api-1.1.2/tradernet_api/commands/set_stop_order.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Any
 
+from tradernet_api.const import Command
 from tradernet_api.models.command_model import SetStopOrderModel
 
 
 def set_stop_order(
     self: Any,
     ticker: str,
     stop_loss: float | None = 0,
@@ -16,14 +17,14 @@
     :param self: binds with API class
     :param ticker: The instrument used to issue an order
     :param stop_loss: Stop Loss order price. Optional
     :param take_profit: Take profit order price. Optional
 
     :return: Response
     """
-    command_name = "putStopLoss"
+    command_name = Command.set_stop_order.value
 
     order_param = SetStopOrderModel(
         ticker=f"{ticker}.US".upper(), stop_loss=stop_loss, take_profit=take_profit
     )
 
     return self._client_v2.send_request(command=command_name, params=order_param)
```

### Comparing `tradernet_api-1.1.0/tradernet_api/const.py` & `tradernet_api-1.1.2/tradernet_api/const.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from enum import Enum
 
 api_url = "https://tradernet.ru/api"
 
 
 class Command(Enum):
-    send_order = "send_order"
-    delete_order = "delete_order"
-    get_orders = "get_orders"
-    get_ticker_info = "get_ticker_info"
-    set_stop_order = "set_stop_order"
+    send_order = "putTradeOrder"
+    delete_order = "delTradeOrder"
+    get_orders = "getNotifyOrderJson"
+    get_ticker_info = "getSecurityInfo"
+    set_stop_order = "putStopLoss"
 
 
 class SendOrderField(Enum):
     action_id = "action_id"
     expiry = "expiry"
     expiration_id = "expiration_id"
     side = "side"
```

### Comparing `tradernet_api-1.1.0/tradernet_api/models/command_model.py` & `tradernet_api-1.1.2/tradernet_api/models/command_model.py`

 * *Files identical despite different names*

### Comparing `tradernet_api-1.1.0/tradernet_api/models/request_model.py` & `tradernet_api-1.1.2/tradernet_api/models/request_model.py`

 * *Files identical despite different names*

### Comparing `tradernet_api-1.1.0/setup.py` & `tradernet_api-1.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,83 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: tradernet-api
+Version: 1.1.2
+Summary: Public API client for working with the Tradernet platform.
+License: MIT
+Author: Artur Kutsevol
+Author-email: arthur.kutsevol@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pydantic (>=1.9.1,<2.0.0)
+Requires-Dist: requests (>=2.27.1,<3.0.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['tradernet_api', 'tradernet_api.commands', 'tradernet_api.models']
+<div align="center">
 
-package_data = \
-{'': ['*']}
+[![Upload Python Package](https://github.com/kutsevol/tradernet-api/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/kutsevol/tradernet-api/actions/workflows/ci.yml)
+[![Python Version](https://img.shields.io/pypi/pyversions/tradernet_api.svg)](https://pypi.org/project/tradernet_api/)
+[![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/tradernet-api/tradernet_api/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
 
-install_requires = \
-['pydantic>=1.9.1,<2.0.0', 'requests>=2.27.1,<3.0.0']
-
-setup_kwargs = {
-    'name': 'tradernet-api',
-    'version': '1.1.0',
-    'description': 'Public API client for working with the Tradernet platform.',
-    'long_description': '<div align="center">\n\n[![Upload Python Package](https://github.com/kutsevol/tradernet-api/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/kutsevol/tradernet-api/actions/workflows/ci.yml)\n[![Python Version](https://img.shields.io/pypi/pyversions/tradernet_api.svg)](https://pypi.org/project/tradernet_api/)\n[![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/tradernet-api/tradernet_api/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)\n\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)\n[![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/tradernet-api/tradernet_api/blob/master/.pre-commit-config.yaml)\n[![Semantic Versions](https://img.shields.io/badge/semantic--versions-python-e10079.svg)](https://github.com/kutsevol/tradernet-api/releases)\n[![License](https://img.shields.io/github/license/kutsevol/tradernet-api)](https://github.com/kutsevol/tradernet-api/blob/main/LICENSE)\n![Coverage Report](assets/images/coverage.svg)\n</div>\n\n# Tradernet API\nPublic API client for working with the Tradernet platform. </br>\n[Official API documentation](https://tradernet.com/tradernet-api)\n\n## Installation\n\n### Install package\n\n```bash\npip install -U tradernet-api\n```\n\nor \n\n```bash\npoetry add tradernet-api@latest\n```\n\n### Getting Started\n\n```python\nfrom tradernet_api.api import API\n\n# Setup client\napi_client = API(api_key="YOUR API KEY", secret_key="YOUR SECRET KEY")\n\n# Get only active orders by default\napi_client.get_orders()\n\n# Get all orders\napi_client.get_orders(active_only=False)\n\n# Get ticker info\napi_client.get_ticker_info(ticker="AAPL")\n\n# Send order to the platform\napi_client.send_order(ticker="AAPL", side="buy", margin=True, count=1, order_exp="day", market_order=True)\napi_client.send_order(ticker="MSFT", side="sell", margin=False, count=2, order_exp="ext", limit_price=200)\napi_client.send_order(ticker="TSLA", side="sell", margin=True, count=3, order_exp="gtc", stop_price=1000)\n\n# Delete/cancel active order\napi_client.delete_order(order_id=123456789)\n\n# Set stop loss and/or take profit\napi_client.set_stop_order(ticker="AAPL", stop_loss=1, take_profit=2)\n```\n\n## 🛡 License\n\n[![License](https://img.shields.io/github/license/kutsevol/tradernet-api)](https://github.com/kutsevol/tradernet-api/blob/main/LICENSE)\n\nThis project is licensed under the terms of the `MIT` license. See [LICENSE](https://github.com/kutsevol/tradernet-api/blob/main/LICENSE) for more details.\n',
-    'author': 'Artur Kutsevol',
-    'author_email': 'arthur.kutsevol@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.10,<4.0',
-}
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)
+[![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/tradernet-api/tradernet_api/blob/master/.pre-commit-config.yaml)
+[![Semantic Versions](https://img.shields.io/badge/semantic--versions-python-e10079.svg)](https://github.com/kutsevol/tradernet-api/releases)
+[![License](https://img.shields.io/github/license/kutsevol/tradernet-api)](https://github.com/kutsevol/tradernet-api/blob/main/LICENSE)
+![Coverage Report](assets/images/coverage.svg)
+</div>
 
+# Tradernet API
+Public API client for working with the Tradernet platform. </br>
+[Official API documentation](https://tradernet.com/tradernet-api)
+
+## Installation
+
+### Install package
+
+```bash
+pip install -U tradernet-api
+```
+
+or 
+
+```bash
+poetry add tradernet-api@latest
+```
+
+### Getting Started
+
+```python
+from tradernet_api.api import API
+
+# Setup client
+api_client = API(api_key="YOUR API KEY", secret_key="YOUR SECRET KEY")
+
+# Get only active orders by default
+api_client.get_orders()
+
+# Get all orders
+api_client.get_orders(active_only=False)
+
+# Get ticker info
+api_client.get_ticker_info(ticker="AAPL")
+
+# Send order to the platform
+api_client.send_order(ticker="AAPL", side="buy", margin=True, count=1, order_exp="day", market_order=True)
+api_client.send_order(ticker="MSFT", side="sell", margin=False, count=2, order_exp="ext", limit_price=200)
+api_client.send_order(ticker="TSLA", side="sell", margin=True, count=3, order_exp="gtc", stop_price=1000)
+
+# Delete/cancel active order
+api_client.delete_order(order_id=123456789)
+
+# Set stop loss and/or take profit
+api_client.set_stop_order(ticker="AAPL", stop_loss=1, take_profit=2)
+```
+
+## 🛡 License
+
+[![License](https://img.shields.io/github/license/kutsevol/tradernet-api)](https://github.com/kutsevol/tradernet-api/blob/main/LICENSE)
+
+This project is licensed under the terms of the `MIT` license. See [LICENSE](https://github.com/kutsevol/tradernet-api/blob/main/LICENSE) for more details.
 
-setup(**setup_kwargs)
```

