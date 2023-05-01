# Comparing `tmp/commonX-0.4.1.tar.gz` & `tmp/commonX-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\commonX-0.4.1.tar", last modified: Tue Apr 18 03:29:36 2023, max compression
+gzip compressed data, was "dist\commonX-0.4.3.tar", last modified: Mon May  1 08:00:05 2023, max compression
```

## Comparing `commonX-0.4.1.tar` & `commonX-0.4.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 03:29:36.000000 commonX-0.4.1/
--rw-rw-rw-   0        0        0      714 2023-04-18 03:29:36.000000 commonX-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0       77 2023-04-18 03:29:05.000000 commonX-0.4.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 03:29:35.000000 commonX-0.4.1/common/
--rw-rw-rw-   0        0        0       86 2023-04-18 03:29:05.000000 commonX-0.4.1/common/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 03:29:36.000000 commonX-0.4.1/common/base/
--rw-rw-rw-   0        0        0      622 2023-04-18 03:29:05.000000 commonX-0.4.1/common/base/__init__.py
--rw-rw-rw-   0        0        0     1894 2023-04-18 03:29:05.000000 commonX-0.4.1/common/base/entity.py
--rw-rw-rw-   0        0        0      359 2023-04-18 03:29:05.000000 commonX-0.4.1/common/base/factory.py
--rw-rw-rw-   0        0        0     2927 2023-04-18 03:29:05.000000 commonX-0.4.1/common/base/genor.py
--rw-rw-rw-   0        0        0     2916 2023-04-18 03:29:05.000000 commonX-0.4.1/common/base/hook.py
--rw-rw-rw-   0        0        0     4135 2023-04-18 03:29:05.000000 commonX-0.4.1/common/base/logger.py
--rw-rw-rw-   0        0        0     5710 2023-04-18 03:29:05.000000 commonX-0.4.1/common/base/mapper.py
--rw-rw-rw-   0        0        0     8399 2023-04-18 03:29:05.000000 commonX-0.4.1/common/base/multi_task.py
--rw-rw-rw-   0        0        0     5182 2023-04-18 03:29:05.000000 commonX-0.4.1/common/base/packer.py
--rw-rw-rw-   0        0        0     1968 2023-04-18 03:29:05.000000 commonX-0.4.1/common/base/registry.py
-drwxrwxrwx   0        0        0        0 2023-04-18 03:29:36.000000 commonX-0.4.1/common/ext/
--rw-rw-rw-   0        0        0      187 2023-04-18 03:29:05.000000 commonX-0.4.1/common/ext/__init__.py
--rw-rw-rw-   0        0        0     2174 2023-04-18 03:29:05.000000 commonX-0.4.1/common/ext/cookie_parser.py
--rw-rw-rw-   0        0        0     3845 2023-04-18 03:29:05.000000 commonX-0.4.1/common/ext/iphone_client.py
--rw-rw-rw-   0        0        0      220 2023-04-18 03:29:05.000000 commonX-0.4.1/common/ext/ocr_support.py
--rw-rw-rw-   0        0        0     1862 2023-04-18 03:29:05.000000 commonX-0.4.1/common/ext/qq_email.py
-drwxrwxrwx   0        0        0        0 2023-04-18 03:29:36.000000 commonX-0.4.1/common/postman/
--rw-rw-rw-   0        0        0       87 2023-04-18 03:29:05.000000 commonX-0.4.1/common/postman/__init__.py
--rw-rw-rw-   0        0        0     5086 2023-04-18 03:29:05.000000 commonX-0.4.1/common/postman/postman_api.py
--rw-rw-rw-   0        0        0     3316 2023-04-18 03:29:05.000000 commonX-0.4.1/common/postman/postman_impl.py
--rw-rw-rw-   0        0        0     4274 2023-04-18 03:29:05.000000 commonX-0.4.1/common/postman/postman_proxy.py
-drwxrwxrwx   0        0        0        0 2023-04-18 03:29:36.000000 commonX-0.4.1/common/util/
--rw-rw-rw-   0        0        0      246 2023-04-18 03:29:05.000000 commonX-0.4.1/common/util/__init__.py
--rw-rw-rw-   0        0        0      791 2023-04-18 03:29:05.000000 commonX-0.4.1/common/util/args_util.py
--rw-rw-rw-   0        0        0     2176 2023-04-18 03:29:05.000000 commonX-0.4.1/common/util/assert_util.py
--rw-rw-rw-   0        0        0     3273 2023-04-18 03:29:05.000000 commonX-0.4.1/common/util/decorator_util.py
--rw-rw-rw-   0        0        0     4855 2023-04-18 03:29:05.000000 commonX-0.4.1/common/util/file_util.py
--rw-rw-rw-   0        0        0     2765 2023-04-18 03:29:05.000000 commonX-0.4.1/common/util/json_util.py
--rw-rw-rw-   0        0        0     6494 2023-04-18 03:29:05.000000 commonX-0.4.1/common/util/requests_util.py
--rw-rw-rw-   0        0        0     4616 2023-04-18 03:29:05.000000 commonX-0.4.1/common/util/sys_util.py
--rw-rw-rw-   0        0        0      898 2023-04-18 03:29:05.000000 commonX-0.4.1/common/util/time_util.py
--rw-rw-rw-   0        0        0      715 2023-04-18 03:29:05.000000 commonX-0.4.1/common/util/typing_util.py
-drwxrwxrwx   0        0        0        0 2023-04-18 03:29:35.000000 commonX-0.4.1/commonX.egg-info/
--rw-rw-rw-   0        0        0      714 2023-04-18 03:29:35.000000 commonX-0.4.1/commonX.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      896 2023-04-18 03:29:35.000000 commonX-0.4.1/commonX.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 03:29:35.000000 commonX-0.4.1/commonX.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-18 03:29:35.000000 commonX-0.4.1/commonX.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-18 03:29:36.000000 commonX-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1089 2023-04-18 03:29:21.000000 commonX-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 08:00:05.000000 commonX-0.4.3/
+-rw-rw-rw-   0        0        0      714 2023-05-01 08:00:05.000000 commonX-0.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0       77 2023-05-01 07:59:31.000000 commonX-0.4.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 08:00:04.000000 commonX-0.4.3/common/
+-rw-rw-rw-   0        0        0       86 2023-05-01 07:59:31.000000 commonX-0.4.3/common/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 08:00:04.000000 commonX-0.4.3/common/base/
+-rw-rw-rw-   0        0        0      622 2023-05-01 07:59:30.000000 commonX-0.4.3/common/base/__init__.py
+-rw-rw-rw-   0        0        0     1894 2023-05-01 07:59:30.000000 commonX-0.4.3/common/base/entity.py
+-rw-rw-rw-   0        0        0      359 2023-05-01 07:59:30.000000 commonX-0.4.3/common/base/factory.py
+-rw-rw-rw-   0        0        0     2927 2023-05-01 07:59:30.000000 commonX-0.4.3/common/base/genor.py
+-rw-rw-rw-   0        0        0     2916 2023-05-01 07:59:30.000000 commonX-0.4.3/common/base/hook.py
+-rw-rw-rw-   0        0        0     4135 2023-05-01 07:59:30.000000 commonX-0.4.3/common/base/logger.py
+-rw-rw-rw-   0        0        0     5710 2023-05-01 07:59:30.000000 commonX-0.4.3/common/base/mapper.py
+-rw-rw-rw-   0        0        0     8399 2023-05-01 07:59:30.000000 commonX-0.4.3/common/base/multi_task.py
+-rw-rw-rw-   0        0        0     5182 2023-05-01 07:59:30.000000 commonX-0.4.3/common/base/packer.py
+-rw-rw-rw-   0        0        0     1968 2023-05-01 07:59:30.000000 commonX-0.4.3/common/base/registry.py
+drwxrwxrwx   0        0        0        0 2023-05-01 08:00:04.000000 commonX-0.4.3/common/ext/
+-rw-rw-rw-   0        0        0      187 2023-05-01 07:59:30.000000 commonX-0.4.3/common/ext/__init__.py
+-rw-rw-rw-   0        0        0     2174 2023-05-01 07:59:30.000000 commonX-0.4.3/common/ext/cookie_parser.py
+-rw-rw-rw-   0        0        0     3845 2023-05-01 07:59:30.000000 commonX-0.4.3/common/ext/iphone_client.py
+-rw-rw-rw-   0        0        0      220 2023-05-01 07:59:30.000000 commonX-0.4.3/common/ext/ocr_support.py
+-rw-rw-rw-   0        0        0     1862 2023-05-01 07:59:30.000000 commonX-0.4.3/common/ext/qq_email.py
+drwxrwxrwx   0        0        0        0 2023-05-01 08:00:04.000000 commonX-0.4.3/common/postman/
+-rw-rw-rw-   0        0        0       87 2023-05-01 07:59:30.000000 commonX-0.4.3/common/postman/__init__.py
+-rw-rw-rw-   0        0        0     5086 2023-05-01 07:59:30.000000 commonX-0.4.3/common/postman/postman_api.py
+-rw-rw-rw-   0        0        0     4903 2023-05-01 07:59:30.000000 commonX-0.4.3/common/postman/postman_impl.py
+-rw-rw-rw-   0        0        0     4418 2023-05-01 07:59:30.000000 commonX-0.4.3/common/postman/postman_proxy.py
+drwxrwxrwx   0        0        0        0 2023-05-01 08:00:04.000000 commonX-0.4.3/common/util/
+-rw-rw-rw-   0        0        0      246 2023-05-01 07:59:31.000000 commonX-0.4.3/common/util/__init__.py
+-rw-rw-rw-   0        0        0      791 2023-05-01 07:59:30.000000 commonX-0.4.3/common/util/args_util.py
+-rw-rw-rw-   0        0        0     2176 2023-05-01 07:59:30.000000 commonX-0.4.3/common/util/assert_util.py
+-rw-rw-rw-   0        0        0     3273 2023-05-01 07:59:30.000000 commonX-0.4.3/common/util/decorator_util.py
+-rw-rw-rw-   0        0        0     7244 2023-05-01 07:59:30.000000 commonX-0.4.3/common/util/file_util.py
+-rw-rw-rw-   0        0        0     2921 2023-05-01 07:59:30.000000 commonX-0.4.3/common/util/json_util.py
+-rw-rw-rw-   0        0        0     6928 2023-05-01 07:59:31.000000 commonX-0.4.3/common/util/requests_util.py
+-rw-rw-rw-   0        0        0     4616 2023-05-01 07:59:31.000000 commonX-0.4.3/common/util/sys_util.py
+-rw-rw-rw-   0        0        0      898 2023-05-01 07:59:31.000000 commonX-0.4.3/common/util/time_util.py
+-rw-rw-rw-   0        0        0      715 2023-05-01 07:59:31.000000 commonX-0.4.3/common/util/typing_util.py
+drwxrwxrwx   0        0        0        0 2023-05-01 08:00:04.000000 commonX-0.4.3/commonX.egg-info/
+-rw-rw-rw-   0        0        0      714 2023-05-01 08:00:04.000000 commonX-0.4.3/commonX.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      896 2023-05-01 08:00:04.000000 commonX-0.4.3/commonX.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 08:00:04.000000 commonX-0.4.3/commonX.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-01 08:00:04.000000 commonX-0.4.3/commonX.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-01 08:00:05.000000 commonX-0.4.3/setup.cfg
+-rw-rw-rw-   0        0        0     1089 2023-05-01 07:59:55.000000 commonX-0.4.3/setup.py
```

### Comparing `commonX-0.4.1/PKG-INFO` & `commonX-0.4.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commonX
-Version: 0.4.1
+Version: 0.4.3
 Summary: python common toolkit
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,toolkit,postman
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `commonX-0.4.1/common/base/__init__.py` & `commonX-0.4.3/common/base/__init__.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.1/common/base/entity.py` & `commonX-0.4.3/common/base/entity.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.1/common/base/genor.py` & `commonX-0.4.3/common/base/genor.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.1/common/base/hook.py` & `commonX-0.4.3/common/base/hook.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.1/common/base/logger.py` & `commonX-0.4.3/common/base/logger.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.1/common/base/mapper.py` & `commonX-0.4.3/common/base/mapper.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.1/common/base/multi_task.py` & `commonX-0.4.3/common/base/multi_task.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.1/common/base/packer.py` & `commonX-0.4.3/common/base/packer.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.1/common/base/registry.py` & `commonX-0.4.3/common/base/registry.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.1/common/ext/cookie_parser.py` & `commonX-0.4.3/common/ext/cookie_parser.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.1/common/ext/iphone_client.py` & `commonX-0.4.3/common/ext/iphone_client.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.1/common/ext/qq_email.py` & `commonX-0.4.3/common/ext/qq_email.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.1/common/postman/postman_api.py` & `commonX-0.4.3/common/postman/postman_api.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.1/common/postman/postman_impl.py` & `commonX-0.4.3/common/postman/postman_impl.py`

 * *Files 22% similar despite different names*

```diff
@@ -53,15 +53,14 @@
                 meta_data[v] = meta_data.pop(k)
         return meta_data
 
 
 class CffiPostman(AbstractPostman):
 
     def __init__(self, kwargs) -> None:
-        kwargs.setdefault('impersonate', 'chrome101')
         super().__init__(kwargs)
 
     def __get__(self):
         from curl_cffi import requests
         return requests.get
 
     def __post__(self):
@@ -71,15 +70,14 @@
 
 class CffiSessionPostman(AbstractSessionPostman):
     from curl_cffi import requests
     Session = requests.Session
     CffiResp = requests.Response
 
     def __init__(self, kwargs: dict) -> None:
-        kwargs.setdefault('impersonate', 'chrome101')
         super().__init__(kwargs)
 
     def create_session(self, kwargs):
         return self.new_cffi_session(kwargs)
 
     def new_cffi_session(self, kwargs: dict):
         return self.Session(**kwargs)
@@ -105,9 +103,56 @@
         'cffi': CffiPostman,
         'cffi_Session': CffiSessionPostman,
         # 注意: tls_client 不支持 response.content 和 cookies维护
         # 'tls_client': TslClientSessionPostman,
     }
 
     @classmethod
-    def get_impl_clazz(cls, key: str) -> PostmanImplClazz:
+    def get_impl_clazz(cls, key='requests') -> PostmanImplClazz:
         return cls.postman_impl_class_dict[key]
+
+    @classmethod
+    def build_from_config_file(cls,
+                               filepath='./postman.yml',
+                               data=None,
+                               ) -> Postman:
+        if data is None:
+            from common import PackerUtil
+            data = PackerUtil.unpack(filepath)[0]
+            if data is None:
+                raise AssertionError(f'空配置文件: {filepath}')
+
+        return cls.PostmanDslHandler().build_postman(data)
+
+    # noinspection PyMethodMayBeStatic
+    class PostmanDslHandler:
+
+        def __init__(self) -> None:
+            self.dsl_handler_list: list[Callable[[Dict], Union[Postman, None]]] = [
+                self.proxy_handler,
+                self.impltype_handler,
+            ]
+
+        def proxy_handler(self, data: dict, key='proxies'):
+            meta_data = data.get('meta_data', {})
+
+            from common import ProxyBuilder
+
+            proxies = meta_data.get(key, None)
+
+            # 无代理，或代理已配置好好的
+            if proxies is None or isinstance(proxies, dict):
+                return
+
+            meta_data[key] = ProxyBuilder.build_by_str(proxies)
+
+        def impltype_handler(self, data: dict, key='type'):
+            impl_clazz = Postmans.get_impl_clazz(data.get(key, 'requests'))
+            return impl_clazz(data.get('meta_data', {}))
+
+        def build_postman(self, data):
+            for handler in self.dsl_handler_list:
+                postman = handler(data)
+                if postman is not None:
+                    return postman
+
+            raise NotImplementedError('no available handler to build your postman')
```

### Comparing `commonX-0.4.1/common/postman/postman_proxy.py` & `commonX-0.4.3/common/postman/postman_proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,38 +44,42 @@
                  postman: Postman,
                  retry_times: int,
                  ):
         super().__init__(postman)
         self.retry_times = retry_times
 
     def retry_request(self, request, url, **kwargs):
-        for _ in range(self.retry_times):
+        for i in range(self.retry_times):
             try:
                 return request(url, **kwargs)
             except KeyboardInterrupt as e:
                 raise e
             except Exception as e:
                 self.excp_handle(e)
+                self.tip_retrying(i, request, url, kwargs)
 
         return self.fallback(url, kwargs)
 
     def get(self, *args, **kwargs):
-        return self.retry_request(super().get, *args, **kwargs)
+        return self.retry_request(self.postman.get, *args, **kwargs)
 
     def post(self, *args, **kwargs):
-        return self.retry_request(super().post, *args, **kwargs)
+        return self.retry_request(self.postman.post, *args, **kwargs)
 
     def fallback(self, url, kwargs):
         raise RuntimeError(f"请求失败，重试了{self.retry_times}次后依然失败: {url}，携带参数: {kwargs}")
 
     # noinspection PyMethodMayBeStatic,PyUnusedLocal
     def excp_handle(self, e):
         from common import traceback_print_exec
         traceback_print_exec()
 
+    def tip_retrying(self, time, _request, url, kwargs):
+        pass
+
 
 class MultiPartPostman(PostmanProxy):
 
     def build_headers(self, data, kwargs):
         headers = kwargs.get('headers', None)
         if headers is None:
             headers = self.get_meta_data().get('headers', {})
```

### Comparing `commonX-0.4.1/common/util/args_util.py` & `commonX-0.4.3/common/util/args_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.1/common/util/assert_util.py` & `commonX-0.4.3/common/util/assert_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.1/common/util/decorator_util.py` & `commonX-0.4.3/common/util/decorator_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.1/common/util/json_util.py` & `commonX-0.4.3/common/util/json_util.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,14 +29,21 @@
 
     def __getitem__(self, item):
         return self._data[item]
 
     def __contains__(self, item):
         return item in self._data
 
+    @property
+    def src_dict(self):
+        return self._data
+
+    def get(self, *args, **kwargs):
+        return self._data.get(*args, **kwargs)
+
 
 def dict_2_obj(data: dict):
     return DictModel(data)
 
 
 def json_loadf(filepath,
                encoding='utf-8',
```

### Comparing `commonX-0.4.1/common/util/requests_util.py` & `commonX-0.4.3/common/util/requests_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,17 +12,27 @@
         return proxies
 
     @classmethod
     def clash_proxy(cls, ip='127.0.0.1', port='7890'):
         return cls.build_proxy(cls.addr_f.format(ip, port))
 
     @classmethod
-    def v2Ray_proxy(cls, ip='127.0.0.1', port='10809'):
+    def v2ray_proxy(cls, ip='127.0.0.1', port='10809'):
         return cls.build_proxy(cls.addr_f.format(ip, port))
 
+    @classmethod
+    def build_by_str(cls, text):
+        """
+        :param text: 127.0.0.1:1234 / clash / v2ray
+        """
+        proxy = getattr(cls, text + '_proxy', None)
+        return proxy() or cls.build_proxy(text)
+
+    v2Ray_proxy = v2ray_proxy
+
 
 def save_resp_content(resp, filepath: str):
     from .file_util import of_dir_path
     of_dir_path(filepath, mkdir=True)
     with open(filepath, 'wb') as f:
         f.write(resp.content)
 
@@ -100,14 +110,18 @@
     args_str = args_str.replace("\'", "\"")
     return args_str
 
 
 class IResp:
 
     @property
+    def http_code(self) -> str:
+        raise NotImplementedError
+
+    @property
     def is_success(self) -> bool:
         raise NotImplementedError
 
     @property
     def is_not_success(self) -> bool:
         return not self.is_success
 
@@ -152,14 +166,18 @@
 
 class CommonResp(IResp):
 
     def __init__(self, resp):
         self.resp = resp
 
     @property
+    def http_code(self):
+        return self.resp.status_code
+
+    @property
     def is_success(self) -> bool:
         return self.resp.status_code == 200
 
     @property
     def text(self) -> str:
         return self.resp.text
```

### Comparing `commonX-0.4.1/common/util/sys_util.py` & `commonX-0.4.3/common/util/sys_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.1/common/util/time_util.py` & `commonX-0.4.3/common/util/time_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.1/common/util/typing_util.py` & `commonX-0.4.3/common/util/typing_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.1/commonX.egg-info/PKG-INFO` & `commonX-0.4.3/commonX.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commonX
-Version: 0.4.1
+Version: 0.4.3
 Summary: python common toolkit
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,toolkit,postman
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `commonX-0.4.1/commonX.egg-info/SOURCES.txt` & `commonX-0.4.3/commonX.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `commonX-0.4.1/setup.py` & `commonX-0.4.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from setuptools import setup, find_packages
 
 here = os.path.abspath(os.path.dirname(__file__))
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = "\n" + f.read()
 
-VERSION = '0.4.1'
+VERSION = '0.4.3'
 DESCRIPTION = 'python common toolkit'
 
 setup(
     name='commonX',
     version=VERSION,
     description=DESCRIPTION,
     author='hect0x7',
```

