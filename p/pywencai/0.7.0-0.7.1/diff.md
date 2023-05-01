# Comparing `tmp/pywencai-0.7.0.tar.gz` & `tmp/pywencai-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywencai-0.7.0.tar", max compression
+gzip compressed data, was "pywencai-0.7.1.tar", max compression
```

## Comparing `pywencai-0.7.0.tar` & `pywencai-0.7.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1062 2023-04-28 09:32:32.601654 pywencai-0.7.0/LICENSE
--rw-r--r--   0        0        0     2147 2023-04-28 09:32:32.601654 pywencai-0.7.0/README.md
--rw-r--r--   0        0        0      530 2023-04-28 09:32:32.605654 pywencai-0.7.0/pyproject.toml
--rw-r--r--   0        0        0       23 2023-04-28 09:32:32.605654 pywencai-0.7.0/pywencai/__init__.py
--rw-r--r--   0        0        0    39677 2023-04-28 09:32:32.605654 pywencai-0.7.0/pywencai/hexin-v.js
--rw-r--r--   0        0        0     4111 2023-04-28 09:32:32.605654 pywencai-0.7.0/pywencai/wencai.py
--rw-r--r--   0        0        0     2732 1970-01-01 00:00:00.000000 pywencai-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-05-01 04:28:42.043050 pywencai-0.7.1/LICENSE
+-rw-r--r--   0        0        0     2310 2023-05-01 04:28:42.043050 pywencai-0.7.1/README.md
+-rw-r--r--   0        0        0      530 2023-05-01 04:28:42.043050 pywencai-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0       23 2023-05-01 04:28:42.043050 pywencai-0.7.1/pywencai/__init__.py
+-rw-r--r--   0        0        0    39677 2023-05-01 04:28:42.043050 pywencai-0.7.1/pywencai/hexin-v.js
+-rw-r--r--   0        0        0     4241 2023-05-01 04:28:42.043050 pywencai-0.7.1/pywencai/wencai.py
+-rw-r--r--   0        0        0     2895 1970-01-01 00:00:00.000000 pywencai-0.7.1/PKG-INFO
```

### Comparing `pywencai-0.7.0/LICENSE` & `pywencai-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pywencai-0.7.0/README.md` & `pywencai-0.7.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -89,16 +89,27 @@
 
 非必填，默认为0，表示循环请求时，每次请求间隔多少秒。
 
 #### log
 
 非必填，默认为Flase，是否在控制台打印日志。
 
+#### cookie
+
+非必填，默认为None，付费版可以尝试传入cookie，获取付费使用权限。
+
 ### 返回值
 
 该方法返回一个`pandas`的`Dataframe`
 
 ## 联系方式
 
 欢迎加入QQ群，分享量化技术！
 
-<img src="./qrcode.png" width=400>
+<img src="./qrcode.png" width=400>
+
+微信公众号
+
+<img src="./weixin.jpg" width=400>
+
+
+
```

### Comparing `pywencai-0.7.0/pyproject.toml` & `pywencai-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pywencai"
-version = "0.7.0"
+version = "0.7.1"
 description = ""
 authors = ["pluto <mayuanchi1029@gmail.com>"]
 readme = "README.md"
 
 [[tool.poetry.source]]
 name = "tsinghua"
 url = "https://pypi.tuna.tsinghua.edu.cn/simple/"
```

### Comparing `pywencai-0.7.0/pywencai/hexin-v.js` & `pywencai-0.7.1/pywencai/hexin-v.js`

 * *Files identical despite different names*

### Comparing `pywencai-0.7.0/pywencai/wencai.py` & `pywencai-0.7.1/pywencai/wencai.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 # 获取condition
 def get_robot_data(**kwargs):
   retry = kwargs.get('retry', 10)
   sleep = kwargs.get('sleep', 0)
   question = kwargs.get('query')
   log = kwargs.get('log', False)
   query_type = kwargs.get('query_type', 'stock')
+  cookie = kwargs.get('cookie', None)
   data = {
     'perpage': 10,
     'page': 1,
     'source': 'Ths_iwencai_Xuangu',
     'secondary_intent': query_type,
     'question': question
   }
@@ -43,15 +44,16 @@
     time.sleep(sleep)
     res = rq.request(
       method='POST',
       url='http://www.iwencai.com/customized/chart/get-robot-data',
       json=data,
       headers={
         'hexin-v': get_token(),
-        'User-Agent': ua.random
+        'User-Agent': ua.random,
+        'cookie': cookie
       }
     )
     result = json.loads(res.text)
     content = result['data']['answer'][0]['txt'][0]['content']
     if type(content) == str:
       content = json.loads(content)
     components0 = content['components'][0]
@@ -85,14 +87,15 @@
 
 
 # 获取每页数据
 def get_page(**kwargs):
   retry = kwargs.pop('retry', 10)
   sleep = kwargs.pop('sleep', 0)
   log = kwargs.pop('log', False)
+  cookie = kwargs.pop('cookie', None)
 
   data = {
     'perpage': 100,
     'page': 1,
     'source': 'Ths_iwencai_Xuangu',
     **kwargs
   }
@@ -104,15 +107,16 @@
     try: 
       res = rq.request(
         method='POST',
         url='http://www.iwencai.com/gateway/urp/v7/landing/getDataList',
         data=data,
         headers={
           'hexin-v': get_token(),
-          'User-Agent': ua.random
+          'User-Agent': ua.random,
+          'cookie': cookie
         },
         timeout=(5, 10)
       )
       result = json.loads(res.text)
       list = result['answer']['components'][0]['data']['datas']
       log and logging.info(f'第{data.get("page")}页成功')
       return pd.DataFrame.from_dict(list)
```

### Comparing `pywencai-0.7.0/PKG-INFO` & `pywencai-0.7.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywencai
-Version: 0.7.0
+Version: 0.7.1
 Summary: 
 Author: pluto
 Author-email: mayuanchi1029@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -107,16 +107,28 @@
 
 非必填，默认为0，表示循环请求时，每次请求间隔多少秒。
 
 #### log
 
 非必填，默认为Flase，是否在控制台打印日志。
 
+#### cookie
+
+非必填，默认为None，付费版可以尝试传入cookie，获取付费使用权限。
+
 ### 返回值
 
 该方法返回一个`pandas`的`Dataframe`
 
 ## 联系方式
 
 欢迎加入QQ群，分享量化技术！
 
 <img src="./qrcode.png" width=400>
+
+微信公众号
+
+<img src="./weixin.jpg" width=400>
+
+
+
+
```

