# Comparing `tmp/openai_forward-0.1.2.tar.gz` & `tmp/openai_forward-0.1.3.tar.gz`

## Comparing `openai_forward-0.1.2.tar` & `openai_forward-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 openai_forward-0.1.2/openai_forward/__init__.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 openai_forward-0.1.2/openai_forward/__main__.py
--rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 openai_forward-0.1.2/openai_forward/_base.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 openai_forward-0.1.2/openai_forward/app.py
--rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 openai_forward-0.1.2/openai_forward/config.py
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 openai_forward-0.1.2/openai_forward/openai.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.1.2/openai_forward/content/__init__.py
--rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 openai_forward-0.1.2/openai_forward/content/chat.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.1.2/openai_forward/content/image.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.1.2/openai_forward/routers/__init__.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 openai_forward-0.1.2/openai_forward/routers/openai_v1.py
--rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 openai_forward-0.1.2/openai_forward/routers/schemas.py
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 openai_forward-0.1.2/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 openai_forward-0.1.2/LICENSE
--rw-r--r--   0        0        0     6451 2020-02-02 00:00:00.000000 openai_forward-0.1.2/README.md
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 openai_forward-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     7721 2020-02-02 00:00:00.000000 openai_forward-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 openai_forward-0.1.3/openai_forward/__init__.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 openai_forward-0.1.3/openai_forward/__main__.py
+-rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 openai_forward-0.1.3/openai_forward/_base.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 openai_forward-0.1.3/openai_forward/app.py
+-rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 openai_forward-0.1.3/openai_forward/config.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 openai_forward-0.1.3/openai_forward/openai.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.1.3/openai_forward/content/__init__.py
+-rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 openai_forward-0.1.3/openai_forward/content/chat.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.1.3/openai_forward/content/image.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.1.3/openai_forward/routers/__init__.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 openai_forward-0.1.3/openai_forward/routers/openai_v1.py
+-rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 openai_forward-0.1.3/openai_forward/routers/schemas.py
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 openai_forward-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 openai_forward-0.1.3/LICENSE
+-rw-r--r--   0        0        0     6251 2020-02-02 00:00:00.000000 openai_forward-0.1.3/README.md
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 openai_forward-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     7521 2020-02-02 00:00:00.000000 openai_forward-0.1.3/PKG-INFO
```

### Comparing `openai_forward-0.1.2/openai_forward/app.py` & `openai_forward-0.1.3/openai_forward/app.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 app = create_app(title="openai_forward", version="1.0")
 openai = Openai()
 use_http2 = False
 
 
 @app.on_event('startup')
 async def startup_event():
-    app.state.client = httpx.AsyncClient(base_url=Openai.base_url, http2=use_http2)
+    app.state.client = httpx.AsyncClient(base_url=Openai._base_url, http2=use_http2)
 
 
 @app.on_event('shutdown')
 async def shutdown_event():
     await app.state.client.aclose()
 
 
-app.add_route(openai.ROUTE_PREFIX+'/{api_path:path}', openai.reverse_proxy,
+app.add_route(openai._ROUTE_PREFIX + '/{api_path:path}', openai.reverse_proxy,
               methods=['GET', 'POST', 'PUT', 'DELETE', 'OPTIONS', 'HEAD', 'PATCH', 'TRACE'])
 app.include_router(router_v1)
```

### Comparing `openai_forward-0.1.2/openai_forward/config.py` & `openai_forward-0.1.3/openai_forward/config.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.1.2/openai_forward/openai.py` & `openai_forward-0.1.3/openai_forward/openai.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from ._base import OpenaiBase
 from .routers.schemas import OpenAIV1ChatCompletion
-from fastapi import Request, HTTPException, status
+from fastapi import Request
 from .config import setting_log
 
 setting_log(log_name="openai_forward.log")
 
 
 class Openai(OpenaiBase):
     def __init__(self):
-        self.validate_host = False
+        if self.IP_BLACKLIST or self.IP_WHITELIST:
+            self.validate_host = True
+        else:
+            self.validate_host = False
 
     async def reverse_proxy(self, request: Request):
         if self.validate_host:
-            if not self.validate_request_host(request.client.host):
-                raise HTTPException(status_code=status.HTTP_403_FORBIDDEN,
-                                    detail=f"Forbidden, please add ip={request.client.host} to `allow_ips`")
-
+            self.validate_request_host(request.client.host)
         return await self._reverse_proxy(request)
 
     async def v1_chat_completions(self, data: OpenAIV1ChatCompletion, request: Request):
         ...
```

### Comparing `openai_forward-0.1.2/openai_forward/content/chat.py` & `openai_forward-0.1.3/openai_forward/content/chat.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.1.2/openai_forward/routers/schemas.py` & `openai_forward-0.1.3/openai_forward/routers/schemas.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,29 +5,32 @@
 
 
 class OpenAIV1ChatCompletion(BaseModel):
     """Creates a completion for the chat message"""
     model: str = Field(..., description="The model to use for the completion", example="gpt-3.5-turbo")
     messages: List[Dict[str, str]] = Field(..., description="The message to complete",
                                            example=[{"role": "user", "content": "hi"}])
-    temperature: float = Field(default=1, description="The temperature to use for the completion")
-    top_p: float = Field(default=1, description="""An alternative to sampling with temperature, called nucleus sampling, where the model considers the results of the tokens with top_p probability mass. So 0.1 means only the tokens comprising the top 10% probability mass are considered.\nWe generally recommend altering this or temperature but not both.""")
+    temperature: float = Field(default=1, description="0会导致更确定的结果，1会导致更随机的结果")
+    top_p: float = Field(default=1, description="0会导致更确定的结果，1会导致更随机的结果")
     n: int = Field(default=1, description="How many chat completion choices to generate for each input message.")
     stream: bool = Field(default=False)
     stop: Union[List[str], str, None] = Field(default=None,
                                               description="Up to 4 sequences where the API will stop generating further tokens.")
     max_tokens: Union[int, None] = Field(default=None, description="The maximum number of tokens to generate in the chat completion. The total length of input tokens and generated tokens is limited by the model's context length.")
     presence_penalty: float = Field(default=0, description="Number between -2.0 and 2.0. ")
     frequency_penalty: float = Field(default=0, description="Number between -2.0 and 2.0. ")
-    logit_bias: Optional[Dict[str, float]] = Field(default=None, description="A dictionary of token to bias. ")
+    logit_bias: Optional[Dict[str, float]] = Field(default=None, description="取值[-100, 100]， 取值越大，生成的结果越偏向于该token。 取-100表示完全不考虑该token。")
     user: Optional[str] = Field(default=None,
                                 description="A unique identifier representing your end-user, which can help OpenAI to monitor and detect abuse. ",
                                 )
 
     class Config:
         schema_extra = {
             "example": {
                 "model": "gpt-3.5-turbo",
                 "messages": [{"role": "user", "content": "hi"}],
-                "stream": False
+                "stream": False,
+                "temperature": 1,
+                "top_p": 1,
+                "logit_bias": None,
             }
         }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `openai_forward-0.1.2/.gitignore` & `openai_forward-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `openai_forward-0.1.2/LICENSE` & `openai_forward-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_forward-0.1.2/README.md` & `openai_forward-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 <h1 align="center">
     <br>
     OpenAI Forward
     <br>
 </h1>
 <p align="center">
     <b> OpenAI API 接口转发服务 <br/>
-    The fastest way to deploy openai api forward proxy </b>
+    The fastest way to deploy openai api forwarding </b>
 </p>
 
 <p align="center">
     <a href="https://pypi.org/project/openai-forward/"><img src="https://img.shields.io/pypi/v/openai-forward?color=brightgreen" alt="PyPI version" ></a>
     <a href="https://github.com/beidongjiedeguang/openai-forward/blob/main/LICENSE">
         <img alt="License" src="https://img.shields.io/github/license/beidongjiedeguang/openai-forward.svg?color=blue&style=flat-square">
     </a>
@@ -30,37 +30,38 @@
     <a href="https://pypi.org/project/openai_forward/">
         <img alt="pypi downloads" src="https://img.shields.io/pypi/dm/openai_forward">
     </a>
 
 </p>
 This project is designed to solve the problem of some regions being unable to directly access OpenAI. The service is deployed on a server that can access the OpenAI API, and OpenAI requests are forwarded through the service, i.e. a reverse proxy service is set up. 
 
-Test access: https://caloi.top/v1/chat/completions is equivalent to https://api.openai.com/v1/chat/completions 
+Test access: https://caloi.top/v1/chat/completions is equivalent to https://api.openai.com/v1/chat/completions
 
-# Table of Contents 
+# Table of Contents
 
-- [Features](#Features) 
-- [Usage](#Usage) 
-- [Service Deployment](#Service-Deployment) 
-- [Service Usage](#Service-Usage) 
+- [Features](#Features)
+- [Usage](#Usage)
+- [Service Deployment](#Service-Deployment)
+- [Service Usage](#Service-Usage)
 - [Configuration](#Configuration)
 
-# Features 
-- [x] Supports forwarding of all OpenAI interfaces 
-- [x] Supports request IP verification 
-- [x] Supports streaming forwarding 
-- [x] Supports default API key 
-- [x] pip installation and deployment 
-- [x] Docker deployment 
+# Features
+
+- [x] Supports forwarding of all OpenAI interfaces
+- [x] Supports request IP verification
+- [x] Supports streaming forwarding
+- [x] Supports default API key
+- [x] pip installation and deployment
+- [x] Docker deployment
 - [x] Support for multiple worker processes
 - [x] Support for specifying the forwarding routing prefix.
-- [ ] Chat content security: Chat content streaming filtering 
 
-# Usage 
-> Here, the proxy address set up by the individual, https://caloi.top, is used as an example 
+# Usage
+
+> Here, the proxy address set up by the individual, https://caloi.top, is used as an example
 
 ### Using in a module
 
 **JS/TS**
 
 ```diff
   import { Configuration } from "openai";
@@ -68,79 +69,104 @@
   const configuration = new Configuration({
 + basePath: "https://caloi.top",
   apiKey: "sk-******",
   });
 ```
 
 **Python**
+
 ```diff
   import openai
-+ openai.api_base = "https://caloi.top"
++ openai.api_base = "https://caloi.top/v1"
   openai.api_key = "sk-******"
 ```
 
 ### Image Generation (DALL-E):
+
 ```bash 
 curl --location 'https://caloi.top/v1/images/generations' \ 
 --header 'Authorization: Bearer sk-******' \ 
 --header 'Content-Type: application/json' \ 
 --data '{ 
     "prompt": "A photo of a cat", 
     "n": 1, 
     "size": "512x512"
 }' 
 ``` 
 
-### [chatgpt-web](https://github.com/Chanzhaoyu/chatgpt-web) 
-Modify the `OPENAI_API_BASE_URL` in [Docker Compose](https://github.com/Chanzhaoyu/chatgpt-web#docker-compose) to the address of the proxy service we set up: 
+### [chatgpt-web](https://github.com/Chanzhaoyu/chatgpt-web)
+
+Modify the `OPENAI_API_BASE_URL` in [Docker Compose](https://github.com/Chanzhaoyu/chatgpt-web#docker-compose) to the
+address of the proxy service we set up:
+
 ```bash 
 OPENAI_API_BASE_URL: https://caloi.top 
 ``` 
 
-### [ChatGPT-Next-Web](https://github.com/Yidadaa/ChatGPT-Next-Web) 
-Replace `BASE_URL` in the docker startup command with the address of the proxy service we set up: 
+### [ChatGPT-Next-Web](https://github.com/Yidadaa/ChatGPT-Next-Web)
+
+Replace `BASE_URL` in the docker startup command with the address of the proxy service we set up:
+
 ```bash 
 docker run -d -p 3000:3000 -e OPENAI_API_KEY="sk-******" -e CODE="<your password>" -e BASE_URL="caloi.top" yidadaa/chatgpt-next-web 
 ``` 
 
-# Service Deployment 
-Two service deployment methods are provided, choose one 
+# Service Deployment
+
+Two service deployment methods are provided, choose one
+
+## Use `pip`  (recommended)
+
+**Installation**
 
-## Use `pip` 
-**Installation** 
 ```bash 
 pip install openai-forward 
 ``` 
-**Run forwarding service** 
-The port number can be specified through `--port`, which defaults to `8000`, and the number of worker processes can be specified through `--workers`, which defaults to `1`. 
+
+**Run forwarding service**
+The port number can be specified through `--port`, which defaults to `8000`, and the number of worker processes can be
+specified through `--workers`, which defaults to `1`.
+
 ```bash 
 openai_forward run --port=9999 --workers=1 
 ``` 
-The service is now set up, and the usage is to replace `https://api.openai.com` with the port number of the service `http://{ip}:{port}`. 
 
-Of course, OPENAI_API_KEY can also be passed in as an environment variable as the default API key, so that the client does not need to pass in the Authorization in the header when requesting the relevant route. 
-Startup command with default API key: 
+The service is now set up, and the usage is to replace `https://api.openai.com` with the port number of the
+service `http://{ip}:{port}`.
+
+Of course, OPENAI_API_KEY can also be passed in as an environment variable as the default API key, so that the client
+does not need to pass in the Authorization in the header when requesting the relevant route.
+Startup command with default API key:
+
 ```bash 
 OPENAI_API_KEY="sk-xxx" openai_forward run --port=9999 --workers=1 
 ``` 
-Note: If both the default API key and the API key passed in the request header exist, the API key in the request header will override the default API key. 
 
-## Use Docker (recommended) 
+Note: If both the default API key and the API key passed in the request header exist, the API key in the request header
+will override the default API key.
+
+## Use Docker
+
 ```bash 
 docker run --name="openai-forward" -d -p 9999:8000 beidongjiedeguang/openai-forward:latest 
 ``` 
-The 9999 port of the host is mapped, and the service can be accessed through `http://{ip}:9999`. 
-Note: You can also pass in the environment variable OPENAI_API_KEY=sk-xxx as the default API key in the startup command. 
 
-# Service Usage 
-Simply replace the OpenAI API address with the address of the service we set up, such as: 
+The 9999 port of the host is mapped, and the service can be accessed through `http://{ip}:9999`.
+Note: You can also pass in the environment variable OPENAI_API_KEY=sk-xxx as the default API key in the startup command.
+
+# Service Usage
+
+Simply replace the OpenAI API address with the address of the service we set up, such as:
+
 ```bash 
 https://api.openai.com/v1/chat/completions 
 ``` 
-Replace with 
+
+Replace with
+
 ```bash 
 http://{ip}:{port}/v1/chat/completions 
 ```
 
 # Configuration
 
 **`openai-forward run` Parameter Configuration Options**
@@ -155,14 +181,9 @@
 
 | Environment Variable  | Description | Default Value |
 |-----------------|------------|:------------------------:|
 | OPENAI_API_KEY  | Default API key | None |
 | OPENAI_BASE_URL | Forwarding base URL | `https://api.openai.com` |
 |LOG_CHAT| Whether to log chat content | `true` |
 |ROUTE_PREFIX| Route prefix | None |
-
-**TODO**
-
-| Environment Variable | Description | Default Value |
-|-----------------|------------|:------------------------:|
 | IP_WHITELIST    | IP whitelist | None |
-| IP_BLACKLIST    | IP blacklist | None |
+| IP_BLACKLIST    | IP blacklist | None |
```

#### html2text {}

```diff
@@ -1,70 +1,66 @@
 [**ä¸­æ**](./README_ZH.md) | **English**
                                     ******
                                 OpenAI Forward
                                      ******
                         OpenAI API æ¥å£è½¬åæå¡
-              The fastest way to deploy openai api forward proxy
+                The fastest way to deploy openai api forwarding
  [PyPI_version] [License] [Release_(latest_by_date)] [GitHub_repo_size] [docer
                      image_size] [tests] [pypi_downloads]
 This project is designed to solve the problem of some regions being unable to
 directly access OpenAI. The service is deployed on a server that can access the
 OpenAI API, and OpenAI requests are forwarded through the service, i.e. a
 reverse proxy service is set up. Test access: https://caloi.top/v1/chat/
 completions is equivalent to https://api.openai.com/v1/chat/completions # Table
 of Contents - [Features](#Features) - [Usage](#Usage) - [Service Deployment]
 (#Service-Deployment) - [Service Usage](#Service-Usage) - [Configuration]
 (#Configuration) # Features - [x] Supports forwarding of all OpenAI interfaces
 - [x] Supports request IP verification - [x] Supports streaming forwarding -
 [x] Supports default API key - [x] pip installation and deployment - [x] Docker
 deployment - [x] Support for multiple worker processes - [x] Support for
-specifying the forwarding routing prefix. - [ ] Chat content security: Chat
-content streaming filtering # Usage > Here, the proxy address set up by the
-individual, https://caloi.top, is used as an example ### Using in a module
-**JS/TS** ```diff import { Configuration } from "openai"; const configuration =
-new Configuration({ + basePath: "https://caloi.top", apiKey: "sk-******", });
-``` **Python** ```diff import openai + openai.api_base = "https://caloi.top"
-openai.api_key = "sk-******" ``` ### Image Generation (DALL-E): ```bash curl --
-location 'https://caloi.top/v1/images/generations' \ --header 'Authorization:
-Bearer sk-******' \ --header 'Content-Type: application/json' \ --data '
-{ "prompt": "A photo of a cat", "n": 1, "size": "512x512" }' ``` ### [chatgpt-
-web](https://github.com/Chanzhaoyu/chatgpt-web) Modify the
-`OPENAI_API_BASE_URL` in [Docker Compose](https://github.com/Chanzhaoyu/
-chatgpt-web#docker-compose) to the address of the proxy service we set up:
-```bash OPENAI_API_BASE_URL: https://caloi.top ``` ### [ChatGPT-Next-Web]
-(https://github.com/Yidadaa/ChatGPT-Next-Web) Replace `BASE_URL` in the docker
-startup command with the address of the proxy service we set up: ```bash docker
-run -d -p 3000:3000 -e OPENAI_API_KEY="sk-******" -e CODE="" -
+specifying the forwarding routing prefix. # Usage > Here, the proxy address set
+up by the individual, https://caloi.top, is used as an example ### Using in a
+module **JS/TS** ```diff import { Configuration } from "openai"; const
+configuration = new Configuration({ + basePath: "https://caloi.top", apiKey:
+"sk-******", }); ``` **Python** ```diff import openai + openai.api_base =
+"https://caloi.top/v1" openai.api_key = "sk-******" ``` ### Image Generation
+(DALL-E): ```bash curl --location 'https://caloi.top/v1/images/generations' \ -
+-header 'Authorization: Bearer sk-******' \ --header 'Content-Type:
+application/json' \ --data '{ "prompt": "A photo of a cat", "n": 1, "size":
+"512x512" }' ``` ### [chatgpt-web](https://github.com/Chanzhaoyu/chatgpt-web)
+Modify the `OPENAI_API_BASE_URL` in [Docker Compose](https://github.com/
+Chanzhaoyu/chatgpt-web#docker-compose) to the address of the proxy service we
+set up: ```bash OPENAI_API_BASE_URL: https://caloi.top ``` ### [ChatGPT-Next-
+Web](https://github.com/Yidadaa/ChatGPT-Next-Web) Replace `BASE_URL` in the
+docker startup command with the address of the proxy service we set up: ```bash
+docker run -d -p 3000:3000 -e OPENAI_API_KEY="sk-******" -e CODE="" -
 e BASE_URL="caloi.top" yidadaa/chatgpt-next-web ``` # Service Deployment Two
-service deployment methods are provided, choose one ## Use `pip`
+service deployment methods are provided, choose one ## Use `pip` (recommended)
 **Installation** ```bash pip install openai-forward ``` **Run forwarding
 service** The port number can be specified through `--port`, which defaults to
 `8000`, and the number of worker processes can be specified through `--
 workers`, which defaults to `1`. ```bash openai_forward run --port=9999 --
 workers=1 ``` The service is now set up, and the usage is to replace `https://
 api.openai.com` with the port number of the service `http://{ip}:{port}`. Of
 course, OPENAI_API_KEY can also be passed in as an environment variable as the
 default API key, so that the client does not need to pass in the Authorization
 in the header when requesting the relevant route. Startup command with default
 API key: ```bash OPENAI_API_KEY="sk-xxx" openai_forward run --port=9999 --
 workers=1 ``` Note: If both the default API key and the API key passed in the
 request header exist, the API key in the request header will override the
-default API key. ## Use Docker (recommended) ```bash docker run --name="openai-
-forward" -d -p 9999:8000 beidongjiedeguang/openai-forward:latest ``` The 9999
-port of the host is mapped, and the service can be accessed through `http://
-{ip}:9999`. Note: You can also pass in the environment variable
-OPENAI_API_KEY=sk-xxx as the default API key in the startup command. # Service
-Usage Simply replace the OpenAI API address with the address of the service we
-set up, such as: ```bash https://api.openai.com/v1/chat/completions ``` Replace
-with ```bash http://{ip}:{port}/v1/chat/completions ``` # Configuration
-**`openai-forward run` Parameter Configuration Options** | Configuration Option
-| Description | Default Value | |-----------| --- | :---: | | --port | Service
-port number | 8000 | | --workers | Number of worker processes | 1 |
-**Environment Variable Configuration Options** refer to the `.env` file in the
-project root directory | Environment Variable | Description | Default Value |
-|-----------------|------------|:------------------------:| | OPENAI_API_KEY |
-Default API key | None | | OPENAI_BASE_URL | Forwarding base URL | `https://
-api.openai.com` | |LOG_CHAT| Whether to log chat content | `true` |
-|ROUTE_PREFIX| Route prefix | None | **TODO** | Environment Variable |
-Description | Default Value | |-----------------|------------|:----------------
---------:| | IP_WHITELIST | IP whitelist | None | | IP_BLACKLIST | IP blacklist
-| None |
+default API key. ## Use Docker ```bash docker run --name="openai-forward" -d -
+p 9999:8000 beidongjiedeguang/openai-forward:latest ``` The 9999 port of the
+host is mapped, and the service can be accessed through `http://{ip}:9999`.
+Note: You can also pass in the environment variable OPENAI_API_KEY=sk-xxx as
+the default API key in the startup command. # Service Usage Simply replace the
+OpenAI API address with the address of the service we set up, such as: ```bash
+https://api.openai.com/v1/chat/completions ``` Replace with ```bash http://
+{ip}:{port}/v1/chat/completions ``` # Configuration **`openai-forward run`
+Parameter Configuration Options** | Configuration Option | Description |
+Default Value | |-----------| --- | :---: | | --port | Service port number |
+8000 | | --workers | Number of worker processes | 1 | **Environment Variable
+Configuration Options** refer to the `.env` file in the project root directory
+| Environment Variable | Description | Default Value | |-----------------|-----
+-------|:------------------------:| | OPENAI_API_KEY | Default API key | None |
+| OPENAI_BASE_URL | Forwarding base URL | `https://api.openai.com` | |LOG_CHAT|
+Whether to log chat content | `true` | |ROUTE_PREFIX| Route prefix | None | |
+IP_WHITELIST | IP whitelist | None | | IP_BLACKLIST | IP blacklist | None |
```

### Comparing `openai_forward-0.1.2/pyproject.toml` & `openai_forward-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openai_forward-0.1.2/PKG-INFO` & `openai_forward-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_forward
-Version: 0.1.2
+Version: 0.1.3
 Summary: 🚀 Openai api forward · OpenAI 接口转发服务 · streaming forward
 Project-URL: Homepage, https://github.com/beidongjiedeguang/openai-forward
 Project-URL: Documentation, https://github.com/beidongjiedeguang/openai-forward#openai-forward
 Project-URL: Issues, https://github.com/beidongjiedeguang/openai-forward/issues
 Project-URL: Source, https://github.com/beidongjiedeguang/openai-forward
 Author-email: kunyuan <beidongjiedeguang@gmail.com>
 License-File: LICENSE
@@ -35,15 +35,15 @@
 <h1 align="center">
     <br>
     OpenAI Forward
     <br>
 </h1>
 <p align="center">
     <b> OpenAI API 接口转发服务 <br/>
-    The fastest way to deploy openai api forward proxy </b>
+    The fastest way to deploy openai api forwarding </b>
 </p>
 
 <p align="center">
     <a href="https://pypi.org/project/openai-forward/"><img src="https://img.shields.io/pypi/v/openai-forward?color=brightgreen" alt="PyPI version" ></a>
     <a href="https://github.com/beidongjiedeguang/openai-forward/blob/main/LICENSE">
         <img alt="License" src="https://img.shields.io/github/license/beidongjiedeguang/openai-forward.svg?color=blue&style=flat-square">
     </a>
@@ -62,37 +62,38 @@
     <a href="https://pypi.org/project/openai_forward/">
         <img alt="pypi downloads" src="https://img.shields.io/pypi/dm/openai_forward">
     </a>
 
 </p>
 This project is designed to solve the problem of some regions being unable to directly access OpenAI. The service is deployed on a server that can access the OpenAI API, and OpenAI requests are forwarded through the service, i.e. a reverse proxy service is set up. 
 
-Test access: https://caloi.top/v1/chat/completions is equivalent to https://api.openai.com/v1/chat/completions 
+Test access: https://caloi.top/v1/chat/completions is equivalent to https://api.openai.com/v1/chat/completions
 
-# Table of Contents 
+# Table of Contents
 
-- [Features](#Features) 
-- [Usage](#Usage) 
-- [Service Deployment](#Service-Deployment) 
-- [Service Usage](#Service-Usage) 
+- [Features](#Features)
+- [Usage](#Usage)
+- [Service Deployment](#Service-Deployment)
+- [Service Usage](#Service-Usage)
 - [Configuration](#Configuration)
 
-# Features 
-- [x] Supports forwarding of all OpenAI interfaces 
-- [x] Supports request IP verification 
-- [x] Supports streaming forwarding 
-- [x] Supports default API key 
-- [x] pip installation and deployment 
-- [x] Docker deployment 
+# Features
+
+- [x] Supports forwarding of all OpenAI interfaces
+- [x] Supports request IP verification
+- [x] Supports streaming forwarding
+- [x] Supports default API key
+- [x] pip installation and deployment
+- [x] Docker deployment
 - [x] Support for multiple worker processes
 - [x] Support for specifying the forwarding routing prefix.
-- [ ] Chat content security: Chat content streaming filtering 
 
-# Usage 
-> Here, the proxy address set up by the individual, https://caloi.top, is used as an example 
+# Usage
+
+> Here, the proxy address set up by the individual, https://caloi.top, is used as an example
 
 ### Using in a module
 
 **JS/TS**
 
 ```diff
   import { Configuration } from "openai";
@@ -100,79 +101,104 @@
   const configuration = new Configuration({
 + basePath: "https://caloi.top",
   apiKey: "sk-******",
   });
 ```
 
 **Python**
+
 ```diff
   import openai
-+ openai.api_base = "https://caloi.top"
++ openai.api_base = "https://caloi.top/v1"
   openai.api_key = "sk-******"
 ```
 
 ### Image Generation (DALL-E):
+
 ```bash 
 curl --location 'https://caloi.top/v1/images/generations' \ 
 --header 'Authorization: Bearer sk-******' \ 
 --header 'Content-Type: application/json' \ 
 --data '{ 
     "prompt": "A photo of a cat", 
     "n": 1, 
     "size": "512x512"
 }' 
 ``` 
 
-### [chatgpt-web](https://github.com/Chanzhaoyu/chatgpt-web) 
-Modify the `OPENAI_API_BASE_URL` in [Docker Compose](https://github.com/Chanzhaoyu/chatgpt-web#docker-compose) to the address of the proxy service we set up: 
+### [chatgpt-web](https://github.com/Chanzhaoyu/chatgpt-web)
+
+Modify the `OPENAI_API_BASE_URL` in [Docker Compose](https://github.com/Chanzhaoyu/chatgpt-web#docker-compose) to the
+address of the proxy service we set up:
+
 ```bash 
 OPENAI_API_BASE_URL: https://caloi.top 
 ``` 
 
-### [ChatGPT-Next-Web](https://github.com/Yidadaa/ChatGPT-Next-Web) 
-Replace `BASE_URL` in the docker startup command with the address of the proxy service we set up: 
+### [ChatGPT-Next-Web](https://github.com/Yidadaa/ChatGPT-Next-Web)
+
+Replace `BASE_URL` in the docker startup command with the address of the proxy service we set up:
+
 ```bash 
 docker run -d -p 3000:3000 -e OPENAI_API_KEY="sk-******" -e CODE="<your password>" -e BASE_URL="caloi.top" yidadaa/chatgpt-next-web 
 ``` 
 
-# Service Deployment 
-Two service deployment methods are provided, choose one 
+# Service Deployment
+
+Two service deployment methods are provided, choose one
+
+## Use `pip`  (recommended)
+
+**Installation**
 
-## Use `pip` 
-**Installation** 
 ```bash 
 pip install openai-forward 
 ``` 
-**Run forwarding service** 
-The port number can be specified through `--port`, which defaults to `8000`, and the number of worker processes can be specified through `--workers`, which defaults to `1`. 
+
+**Run forwarding service**
+The port number can be specified through `--port`, which defaults to `8000`, and the number of worker processes can be
+specified through `--workers`, which defaults to `1`.
+
 ```bash 
 openai_forward run --port=9999 --workers=1 
 ``` 
-The service is now set up, and the usage is to replace `https://api.openai.com` with the port number of the service `http://{ip}:{port}`. 
 
-Of course, OPENAI_API_KEY can also be passed in as an environment variable as the default API key, so that the client does not need to pass in the Authorization in the header when requesting the relevant route. 
-Startup command with default API key: 
+The service is now set up, and the usage is to replace `https://api.openai.com` with the port number of the
+service `http://{ip}:{port}`.
+
+Of course, OPENAI_API_KEY can also be passed in as an environment variable as the default API key, so that the client
+does not need to pass in the Authorization in the header when requesting the relevant route.
+Startup command with default API key:
+
 ```bash 
 OPENAI_API_KEY="sk-xxx" openai_forward run --port=9999 --workers=1 
 ``` 
-Note: If both the default API key and the API key passed in the request header exist, the API key in the request header will override the default API key. 
 
-## Use Docker (recommended) 
+Note: If both the default API key and the API key passed in the request header exist, the API key in the request header
+will override the default API key.
+
+## Use Docker
+
 ```bash 
 docker run --name="openai-forward" -d -p 9999:8000 beidongjiedeguang/openai-forward:latest 
 ``` 
-The 9999 port of the host is mapped, and the service can be accessed through `http://{ip}:9999`. 
-Note: You can also pass in the environment variable OPENAI_API_KEY=sk-xxx as the default API key in the startup command. 
 
-# Service Usage 
-Simply replace the OpenAI API address with the address of the service we set up, such as: 
+The 9999 port of the host is mapped, and the service can be accessed through `http://{ip}:9999`.
+Note: You can also pass in the environment variable OPENAI_API_KEY=sk-xxx as the default API key in the startup command.
+
+# Service Usage
+
+Simply replace the OpenAI API address with the address of the service we set up, such as:
+
 ```bash 
 https://api.openai.com/v1/chat/completions 
 ``` 
-Replace with 
+
+Replace with
+
 ```bash 
 http://{ip}:{port}/v1/chat/completions 
 ```
 
 # Configuration
 
 **`openai-forward run` Parameter Configuration Options**
@@ -187,14 +213,9 @@
 
 | Environment Variable  | Description | Default Value |
 |-----------------|------------|:------------------------:|
 | OPENAI_API_KEY  | Default API key | None |
 | OPENAI_BASE_URL | Forwarding base URL | `https://api.openai.com` |
 |LOG_CHAT| Whether to log chat content | `true` |
 |ROUTE_PREFIX| Route prefix | None |
-
-**TODO**
-
-| Environment Variable | Description | Default Value |
-|-----------------|------------|:------------------------:|
 | IP_WHITELIST    | IP whitelist | None |
-| IP_BLACKLIST    | IP blacklist | None |
+| IP_BLACKLIST    | IP blacklist | None |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openai_forward Version: 0.1.2 Summary: ð Openai
+Metadata-Version: 2.1 Name: openai_forward Version: 0.1.3 Summary: ð Openai
 api forward Â· OpenAI æ¥å£è½¬åæå¡ Â· streaming forward Project-URL:
 Homepage, https://github.com/beidongjiedeguang/openai-forward Project-URL:
 Documentation, https://github.com/beidongjiedeguang/openai-forward#openai-
 forward Project-URL: Issues, https://github.com/beidongjiedeguang/openai-
 forward/issues Project-URL: Source, https://github.com/beidongjiedeguang/
 openai-forward Author-email: kunyuan
 gmail.com> License-File: LICENSE Keywords:
@@ -17,72 +17,68 @@
 extra == 'edge' Provides-Extra: ssl Requires-Dist: certbot; extra == 'ssl'
 Description-Content-Type: text/markdown [**ä¸­æ**](./README_ZH.md) |
 **English**
                                     ******
                                 OpenAI Forward
                                      ******
                         OpenAI API æ¥å£è½¬åæå¡
-              The fastest way to deploy openai api forward proxy
+                The fastest way to deploy openai api forwarding
  [PyPI_version] [License] [Release_(latest_by_date)] [GitHub_repo_size] [docer
                      image_size] [tests] [pypi_downloads]
 This project is designed to solve the problem of some regions being unable to
 directly access OpenAI. The service is deployed on a server that can access the
 OpenAI API, and OpenAI requests are forwarded through the service, i.e. a
 reverse proxy service is set up. Test access: https://caloi.top/v1/chat/
 completions is equivalent to https://api.openai.com/v1/chat/completions # Table
 of Contents - [Features](#Features) - [Usage](#Usage) - [Service Deployment]
 (#Service-Deployment) - [Service Usage](#Service-Usage) - [Configuration]
 (#Configuration) # Features - [x] Supports forwarding of all OpenAI interfaces
 - [x] Supports request IP verification - [x] Supports streaming forwarding -
 [x] Supports default API key - [x] pip installation and deployment - [x] Docker
 deployment - [x] Support for multiple worker processes - [x] Support for
-specifying the forwarding routing prefix. - [ ] Chat content security: Chat
-content streaming filtering # Usage > Here, the proxy address set up by the
-individual, https://caloi.top, is used as an example ### Using in a module
-**JS/TS** ```diff import { Configuration } from "openai"; const configuration =
-new Configuration({ + basePath: "https://caloi.top", apiKey: "sk-******", });
-``` **Python** ```diff import openai + openai.api_base = "https://caloi.top"
-openai.api_key = "sk-******" ``` ### Image Generation (DALL-E): ```bash curl --
-location 'https://caloi.top/v1/images/generations' \ --header 'Authorization:
-Bearer sk-******' \ --header 'Content-Type: application/json' \ --data '
-{ "prompt": "A photo of a cat", "n": 1, "size": "512x512" }' ``` ### [chatgpt-
-web](https://github.com/Chanzhaoyu/chatgpt-web) Modify the
-`OPENAI_API_BASE_URL` in [Docker Compose](https://github.com/Chanzhaoyu/
-chatgpt-web#docker-compose) to the address of the proxy service we set up:
-```bash OPENAI_API_BASE_URL: https://caloi.top ``` ### [ChatGPT-Next-Web]
-(https://github.com/Yidadaa/ChatGPT-Next-Web) Replace `BASE_URL` in the docker
-startup command with the address of the proxy service we set up: ```bash docker
-run -d -p 3000:3000 -e OPENAI_API_KEY="sk-******" -e CODE="" -
+specifying the forwarding routing prefix. # Usage > Here, the proxy address set
+up by the individual, https://caloi.top, is used as an example ### Using in a
+module **JS/TS** ```diff import { Configuration } from "openai"; const
+configuration = new Configuration({ + basePath: "https://caloi.top", apiKey:
+"sk-******", }); ``` **Python** ```diff import openai + openai.api_base =
+"https://caloi.top/v1" openai.api_key = "sk-******" ``` ### Image Generation
+(DALL-E): ```bash curl --location 'https://caloi.top/v1/images/generations' \ -
+-header 'Authorization: Bearer sk-******' \ --header 'Content-Type:
+application/json' \ --data '{ "prompt": "A photo of a cat", "n": 1, "size":
+"512x512" }' ``` ### [chatgpt-web](https://github.com/Chanzhaoyu/chatgpt-web)
+Modify the `OPENAI_API_BASE_URL` in [Docker Compose](https://github.com/
+Chanzhaoyu/chatgpt-web#docker-compose) to the address of the proxy service we
+set up: ```bash OPENAI_API_BASE_URL: https://caloi.top ``` ### [ChatGPT-Next-
+Web](https://github.com/Yidadaa/ChatGPT-Next-Web) Replace `BASE_URL` in the
+docker startup command with the address of the proxy service we set up: ```bash
+docker run -d -p 3000:3000 -e OPENAI_API_KEY="sk-******" -e CODE="" -
 e BASE_URL="caloi.top" yidadaa/chatgpt-next-web ``` # Service Deployment Two
-service deployment methods are provided, choose one ## Use `pip`
+service deployment methods are provided, choose one ## Use `pip` (recommended)
 **Installation** ```bash pip install openai-forward ``` **Run forwarding
 service** The port number can be specified through `--port`, which defaults to
 `8000`, and the number of worker processes can be specified through `--
 workers`, which defaults to `1`. ```bash openai_forward run --port=9999 --
 workers=1 ``` The service is now set up, and the usage is to replace `https://
 api.openai.com` with the port number of the service `http://{ip}:{port}`. Of
 course, OPENAI_API_KEY can also be passed in as an environment variable as the
 default API key, so that the client does not need to pass in the Authorization
 in the header when requesting the relevant route. Startup command with default
 API key: ```bash OPENAI_API_KEY="sk-xxx" openai_forward run --port=9999 --
 workers=1 ``` Note: If both the default API key and the API key passed in the
 request header exist, the API key in the request header will override the
-default API key. ## Use Docker (recommended) ```bash docker run --name="openai-
-forward" -d -p 9999:8000 beidongjiedeguang/openai-forward:latest ``` The 9999
-port of the host is mapped, and the service can be accessed through `http://
-{ip}:9999`. Note: You can also pass in the environment variable
-OPENAI_API_KEY=sk-xxx as the default API key in the startup command. # Service
-Usage Simply replace the OpenAI API address with the address of the service we
-set up, such as: ```bash https://api.openai.com/v1/chat/completions ``` Replace
-with ```bash http://{ip}:{port}/v1/chat/completions ``` # Configuration
-**`openai-forward run` Parameter Configuration Options** | Configuration Option
-| Description | Default Value | |-----------| --- | :---: | | --port | Service
-port number | 8000 | | --workers | Number of worker processes | 1 |
-**Environment Variable Configuration Options** refer to the `.env` file in the
-project root directory | Environment Variable | Description | Default Value |
-|-----------------|------------|:------------------------:| | OPENAI_API_KEY |
-Default API key | None | | OPENAI_BASE_URL | Forwarding base URL | `https://
-api.openai.com` | |LOG_CHAT| Whether to log chat content | `true` |
-|ROUTE_PREFIX| Route prefix | None | **TODO** | Environment Variable |
-Description | Default Value | |-----------------|------------|:----------------
---------:| | IP_WHITELIST | IP whitelist | None | | IP_BLACKLIST | IP blacklist
-| None |
+default API key. ## Use Docker ```bash docker run --name="openai-forward" -d -
+p 9999:8000 beidongjiedeguang/openai-forward:latest ``` The 9999 port of the
+host is mapped, and the service can be accessed through `http://{ip}:9999`.
+Note: You can also pass in the environment variable OPENAI_API_KEY=sk-xxx as
+the default API key in the startup command. # Service Usage Simply replace the
+OpenAI API address with the address of the service we set up, such as: ```bash
+https://api.openai.com/v1/chat/completions ``` Replace with ```bash http://
+{ip}:{port}/v1/chat/completions ``` # Configuration **`openai-forward run`
+Parameter Configuration Options** | Configuration Option | Description |
+Default Value | |-----------| --- | :---: | | --port | Service port number |
+8000 | | --workers | Number of worker processes | 1 | **Environment Variable
+Configuration Options** refer to the `.env` file in the project root directory
+| Environment Variable | Description | Default Value | |-----------------|-----
+-------|:------------------------:| | OPENAI_API_KEY | Default API key | None |
+| OPENAI_BASE_URL | Forwarding base URL | `https://api.openai.com` | |LOG_CHAT|
+Whether to log chat content | `true` | |ROUTE_PREFIX| Route prefix | None | |
+IP_WHITELIST | IP whitelist | None | | IP_BLACKLIST | IP blacklist | None |
```

