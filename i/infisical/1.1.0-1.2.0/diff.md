# Comparing `tmp/infisical-1.1.0.tar.gz` & `tmp/infisical-1.2.0.tar.gz`

## Comparing `infisical-1.1.0.tar` & `infisical-1.2.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 infisical-1.1.0/.editorconfig
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 infisical-1.1.0/CHANGELOG.md
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 infisical-1.1.0/.vscode/settings.json
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/__version__.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/constants.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/logger.py
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/api/__init__.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/api/create_secret.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/api/delete_secret.py
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/api/get_secret.py
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/api/get_secrets.py
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/api/get_service_token_data.py
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/api/models.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/api/update_secret.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/client/__init__.py
--rw-r--r--   0        0        0     3717 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/client/infisicalclient.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/exceptions/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/helpers/__init__.py
--rw-r--r--   0        0        0     7274 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/helpers/client.py
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/helpers/secrets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/models/__init__.py
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/models/api.py
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/models/models.py
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/models/secret_service.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/services/__init__.py
--rw-r--r--   0        0        0     7259 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/services/secret_service.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/utils/__init__.py
--rw-r--r--   0        0        0     6078 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/utils/crypto.py
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/utils/http.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 infisical-1.1.0/scripts/format.sh
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 infisical-1.1.0/scripts/lint.sh
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 infisical-1.1.0/scripts/test.sh
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 infisical-1.1.0/tests/__init__.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 infisical-1.1.0/tests/test_infisical.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infisical-1.1.0/tests/test_client/__init__.py
--rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 infisical-1.1.0/tests/test_client/test_infisical_client.py
--rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 infisical-1.1.0/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 infisical-1.1.0/LICENSE
--rw-r--r--   0        0        0     6881 2020-02-02 00:00:00.000000 infisical-1.1.0/README.md
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 infisical-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     9002 2020-02-02 00:00:00.000000 infisical-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 infisical-1.2.0/.editorconfig
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 infisical-1.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 infisical-1.2.0/.vscode/settings.json
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 infisical-1.2.0/infisical/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 infisical-1.2.0/infisical/__version__.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 infisical-1.2.0/infisical/constants.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 infisical-1.2.0/infisical/logger.py
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 infisical-1.2.0/infisical/api/__init__.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 infisical-1.2.0/infisical/api/create_secret.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 infisical-1.2.0/infisical/api/delete_secret.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 infisical-1.2.0/infisical/api/get_secret.py
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 infisical-1.2.0/infisical/api/get_secrets.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 infisical-1.2.0/infisical/api/get_service_token_data.py
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 infisical-1.2.0/infisical/api/models.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 infisical-1.2.0/infisical/api/update_secret.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infisical-1.2.0/infisical/client/__init__.py
+-rw-r--r--   0        0        0     3717 2020-02-02 00:00:00.000000 infisical-1.2.0/infisical/client/infisicalclient.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 infisical-1.2.0/infisical/exceptions/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infisical-1.2.0/infisical/helpers/__init__.py
+-rw-r--r--   0        0        0     7274 2020-02-02 00:00:00.000000 infisical-1.2.0/infisical/helpers/client.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 infisical-1.2.0/infisical/helpers/secrets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infisical-1.2.0/infisical/models/__init__.py
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 infisical-1.2.0/infisical/models/api.py
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 infisical-1.2.0/infisical/models/models.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 infisical-1.2.0/infisical/models/secret_service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infisical-1.2.0/infisical/services/__init__.py
+-rw-r--r--   0        0        0     7259 2020-02-02 00:00:00.000000 infisical-1.2.0/infisical/services/secret_service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infisical-1.2.0/infisical/utils/__init__.py
+-rw-r--r--   0        0        0     6078 2020-02-02 00:00:00.000000 infisical-1.2.0/infisical/utils/crypto.py
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 infisical-1.2.0/infisical/utils/http.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 infisical-1.2.0/scripts/format.sh
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 infisical-1.2.0/scripts/lint.sh
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 infisical-1.2.0/scripts/test.sh
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 infisical-1.2.0/tests/__init__.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 infisical-1.2.0/tests/test_infisical.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infisical-1.2.0/tests/test_client/__init__.py
+-rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 infisical-1.2.0/tests/test_client/test_infisical_client.py
+-rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 infisical-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 infisical-1.2.0/LICENSE
+-rw-r--r--   0        0        0     7572 2020-02-02 00:00:00.000000 infisical-1.2.0/README.md
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 infisical-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     9693 2020-02-02 00:00:00.000000 infisical-1.2.0/PKG-INFO
```

### Comparing `infisical-1.1.0/infisical/api/__init__.py` & `infisical-1.2.0/infisical/api/__init__.py`

 * *Files identical despite different names*

### Comparing `infisical-1.1.0/infisical/api/create_secret.py` & `infisical-1.2.0/infisical/api/create_secret.py`

 * *Files identical despite different names*

### Comparing `infisical-1.1.0/infisical/api/get_secrets.py` & `infisical-1.2.0/infisical/api/get_secrets.py`

 * *Files identical despite different names*

### Comparing `infisical-1.1.0/infisical/api/get_service_token_data.py` & `infisical-1.2.0/infisical/api/get_service_token_data.py`

 * *Files identical despite different names*

### Comparing `infisical-1.1.0/infisical/api/update_secret.py` & `infisical-1.2.0/infisical/api/update_secret.py`

 * *Files identical despite different names*

### Comparing `infisical-1.1.0/infisical/client/infisicalclient.py` & `infisical-1.2.0/infisical/client/infisicalclient.py`

 * *Files identical despite different names*

### Comparing `infisical-1.1.0/infisical/helpers/client.py` & `infisical-1.2.0/infisical/helpers/client.py`

 * *Files identical despite different names*

### Comparing `infisical-1.1.0/infisical/helpers/secrets.py` & `infisical-1.2.0/infisical/helpers/secrets.py`

 * *Files identical despite different names*

### Comparing `infisical-1.1.0/infisical/models/api.py` & `infisical-1.2.0/infisical/models/api.py`

 * *Files identical despite different names*

### Comparing `infisical-1.1.0/infisical/models/models.py` & `infisical-1.2.0/infisical/models/models.py`

 * *Files identical despite different names*

### Comparing `infisical-1.1.0/infisical/services/secret_service.py` & `infisical-1.2.0/infisical/services/secret_service.py`

 * *Files identical despite different names*

### Comparing `infisical-1.1.0/infisical/utils/crypto.py` & `infisical-1.2.0/infisical/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `infisical-1.1.0/infisical/utils/http.py` & `infisical-1.2.0/infisical/utils/http.py`

 * *Files identical despite different names*

### Comparing `infisical-1.1.0/tests/test_client/test_infisical_client.py` & `infisical-1.2.0/tests/test_client/test_infisical_client.py`

 * *Files identical despite different names*

### Comparing `infisical-1.1.0/.gitignore` & `infisical-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `infisical-1.1.0/LICENSE` & `infisical-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `infisical-1.1.0/README.md` & `infisical-1.2.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -29,21 +29,20 @@
 ## Links
 
 - [SDK docs](https://infisical.com/docs/sdks/languages/python)
 
 ## Basic Usage
 
 ```py
-import os
-import infisical
 from flask import Flask
+from infisical import InfisicalClient
 
 app = Flask(__name__)
 
-client = infisical(token="your_infisical_token")
+client = InfisicalClient(token="your_infisical_token")
 
 @app.route("/")
 def hello_world():
     # access value
     name = client.get_secret("NAME")
     return f"Hello! My name is: {name.secret_value}"
 ```
@@ -56,21 +55,21 @@
 
 ```console
 $ pip install infisical
 ```
 
 ## Configuration
 
-Import the SDK and create a client instance with your Infisical token
+Import the SDK and create a client instance with your [Infisical Token](https://infisical.com/docs/getting-started/dashboard/token).
 
 
 ```py
-import infisical
+from infisical import InfisicalClient
 
-client = infisical(token="your_infisical_token")
+client = InfisicalClient(token="your_infisical_token")
 ```
 
 ### Options
 
 | Parameter | Type     | Description |
 | --------- | -------- | ----------- |
 | `token`   | `string` | An Infisical Token scoped to a project and environment. |
@@ -88,15 +87,15 @@
 
 ```py
 secrets = client.get_all_secrets()
 ```
 
 Retrieve all secrets within the Infisical project and environment
 
-## Get Secret
+### Get Secret
 
 ```py
 secret = client.get_secret("API_KEY")
 value = secret.secret_value # get its value
 ```
 
 By default, `get_secret()` fetches and returns a personal secret. If not found, it returns a shared secret, or tries to retrieve the value from `os.environ`. If a secret is fetched, `get_secret()` caches it to reduce excessive calls and re-fetches periodically based on the `cacheTTL` option (default is 300 seconds) when initializing the client — for more information, see the caching section.
@@ -109,43 +108,43 @@
 ```
 
 ### Parameters
 
 - `secret_name` (string): The key of the secret to retrieve.
 - `type` (string, optional): The type of the secret. Valid options are "shared" or "personal". If not specified, the default value is "personal".
 
-## Create Secret
+### Create Secret
 
 Create a new secret in Infisical
 
 ```py
 new_api_key = client.create_secret("API_KEY", "FOO")
 ```
 
 ### Parameters
 
 - `secret_name` (string): The key of the secret to create.
 - `secret_value` (string): The value of the secret.
 - `type` (string, optional): The type of the secret. Valid options are "shared" or "personal". If not specified, the default value is "shared". A personal secret can only be created if a shared secret with the same name exists.
 
-## Update Secret
+### Update Secret
 
 Update an existing secret in Infisical
 
 ```py
 updated_api_key = client.update_secret("API_KEY", "BAR")
 ```
 
 ### Parameters
 
 - `secret_name` (string): The key of the secret to update.
 - `secret_value` (string): The new value of the secret.
 - `type` (string, optional): The type of the secret. Valid options are "shared" or "personal". If not specified, the default value is "shared".
 
-## Delete Secret
+### Delete Secret
 
 Delete a secret in Infisical
 
 ```py
 deleted_secret = client.delete_secret("API_KEY")
 ```
 
@@ -154,14 +153,22 @@
 - `secret_name` (string): The key of the secret to delete.
 - `type` (string, optional): The type of the secret. Valid options are "shared" or "personal". If not specified, the default value is "shared".
 
 ## Contributing
 
 Bug fixes, docs, and library improvements are always welcome. Please refer to our [Contributing Guide](https://infisical.com/docs/contributing/overview) for detailed information on how you can contribute.
 
+[//]: contributor-faces
+
+<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
+<!-- prettier-ignore-start -->
+<!-- markdownlint-disable -->
+
+<a href="https://github.com/Astropilot"><img src="https://avatars.githubusercontent.com/u/11898378?v=4" width="50" height="50" alt=""/></a> <a href="https://github.com/dangtony98"><img src="https://avatars.githubusercontent.com/u/25857006?v=4" width="50" height="50" alt=""/></a> <a href="https://github.com/Nnahoy"><img src="https://avatars.githubusercontent.com/u/86289996?v=4" width="50" height="50" alt=""/></a>
+
 ## Getting Started
 
 If you want to familiarize yourself with the SDK, you can start by [forking the repository](https://docs.github.com/en/get-started/quickstart/fork-a-repo) and [cloning it in your local development environment](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository). 
 
 After cloning the repository, we recommend that you create a virtual environment:
 
 ```console
```

### Comparing `infisical-1.1.0/pyproject.toml` & `infisical-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `infisical-1.1.0/PKG-INFO` & `infisical-1.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infisical
-Version: 1.1.0
+Version: 1.2.0
 Summary: Official Infisical SDK for Python
 Project-URL: Documentation, https://github.com/Infisical/infisical-python#readme
 Project-URL: Issues, https://github.com/Infisical/infisical-python/issues
 Project-URL: Source, https://github.com/Infisical/infisical-python
 Maintainer-email: Yohann MARTIN <contact@codexus.fr>, Tony Dang <tony@infisical.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -74,21 +74,20 @@
 ## Links
 
 - [SDK docs](https://infisical.com/docs/sdks/languages/python)
 
 ## Basic Usage
 
 ```py
-import os
-import infisical
 from flask import Flask
+from infisical import InfisicalClient
 
 app = Flask(__name__)
 
-client = infisical(token="your_infisical_token")
+client = InfisicalClient(token="your_infisical_token")
 
 @app.route("/")
 def hello_world():
     # access value
     name = client.get_secret("NAME")
     return f"Hello! My name is: {name.secret_value}"
 ```
@@ -101,21 +100,21 @@
 
 ```console
 $ pip install infisical
 ```
 
 ## Configuration
 
-Import the SDK and create a client instance with your Infisical token
+Import the SDK and create a client instance with your [Infisical Token](https://infisical.com/docs/getting-started/dashboard/token).
 
 
 ```py
-import infisical
+from infisical import InfisicalClient
 
-client = infisical(token="your_infisical_token")
+client = InfisicalClient(token="your_infisical_token")
 ```
 
 ### Options
 
 | Parameter | Type     | Description |
 | --------- | -------- | ----------- |
 | `token`   | `string` | An Infisical Token scoped to a project and environment. |
@@ -133,15 +132,15 @@
 
 ```py
 secrets = client.get_all_secrets()
 ```
 
 Retrieve all secrets within the Infisical project and environment
 
-## Get Secret
+### Get Secret
 
 ```py
 secret = client.get_secret("API_KEY")
 value = secret.secret_value # get its value
 ```
 
 By default, `get_secret()` fetches and returns a personal secret. If not found, it returns a shared secret, or tries to retrieve the value from `os.environ`. If a secret is fetched, `get_secret()` caches it to reduce excessive calls and re-fetches periodically based on the `cacheTTL` option (default is 300 seconds) when initializing the client — for more information, see the caching section.
@@ -154,43 +153,43 @@
 ```
 
 ### Parameters
 
 - `secret_name` (string): The key of the secret to retrieve.
 - `type` (string, optional): The type of the secret. Valid options are "shared" or "personal". If not specified, the default value is "personal".
 
-## Create Secret
+### Create Secret
 
 Create a new secret in Infisical
 
 ```py
 new_api_key = client.create_secret("API_KEY", "FOO")
 ```
 
 ### Parameters
 
 - `secret_name` (string): The key of the secret to create.
 - `secret_value` (string): The value of the secret.
 - `type` (string, optional): The type of the secret. Valid options are "shared" or "personal". If not specified, the default value is "shared". A personal secret can only be created if a shared secret with the same name exists.
 
-## Update Secret
+### Update Secret
 
 Update an existing secret in Infisical
 
 ```py
 updated_api_key = client.update_secret("API_KEY", "BAR")
 ```
 
 ### Parameters
 
 - `secret_name` (string): The key of the secret to update.
 - `secret_value` (string): The new value of the secret.
 - `type` (string, optional): The type of the secret. Valid options are "shared" or "personal". If not specified, the default value is "shared".
 
-## Delete Secret
+### Delete Secret
 
 Delete a secret in Infisical
 
 ```py
 deleted_secret = client.delete_secret("API_KEY")
 ```
 
@@ -199,14 +198,22 @@
 - `secret_name` (string): The key of the secret to delete.
 - `type` (string, optional): The type of the secret. Valid options are "shared" or "personal". If not specified, the default value is "shared".
 
 ## Contributing
 
 Bug fixes, docs, and library improvements are always welcome. Please refer to our [Contributing Guide](https://infisical.com/docs/contributing/overview) for detailed information on how you can contribute.
 
+[//]: contributor-faces
+
+<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
+<!-- prettier-ignore-start -->
+<!-- markdownlint-disable -->
+
+<a href="https://github.com/Astropilot"><img src="https://avatars.githubusercontent.com/u/11898378?v=4" width="50" height="50" alt=""/></a> <a href="https://github.com/dangtony98"><img src="https://avatars.githubusercontent.com/u/25857006?v=4" width="50" height="50" alt=""/></a> <a href="https://github.com/Nnahoy"><img src="https://avatars.githubusercontent.com/u/86289996?v=4" width="50" height="50" alt=""/></a>
+
 ## Getting Started
 
 If you want to familiarize yourself with the SDK, you can start by [forking the repository](https://docs.github.com/en/get-started/quickstart/fork-a-repo) and [cloning it in your local development environment](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository). 
 
 After cloning the repository, we recommend that you create a virtual environment:
 
 ```console
```

