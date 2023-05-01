# Comparing `tmp/mtmtool-1.2.3.tar.gz` & `tmp/mtmtool-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mtmtool-1.2.3.tar", last modified: Wed Apr 19 14:29:08 2023, max compression
+gzip compressed data, was "mtmtool-1.2.4.tar", last modified: Mon May  1 08:42:10 2023, max compression
```

## Comparing `mtmtool-1.2.3.tar` & `mtmtool-1.2.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:29:08.484391 mtmtool-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (122)    11324 2023-04-19 14:28:55.000000 mtmtool-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      106 2023-04-19 14:28:55.000000 mtmtool-1.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      682 2023-04-19 14:29:08.484391 mtmtool-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       77 2023-04-19 14:28:55.000000 mtmtool-1.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-19 14:29:08.484391 mtmtool-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2026 2023-04-19 14:28:55.000000 mtmtool-1.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:29:08.480391 mtmtool-1.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:29:08.484391 mtmtool-1.2.3/src/mtmtool/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 14:28:55.000000 mtmtool-1.2.3/src/mtmtool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      685 2023-04-19 14:28:55.000000 mtmtool-1.2.3/src/mtmtool/functool.py
--rw-r--r--   0 runner    (1001) docker     (122)     1718 2023-04-19 14:28:55.000000 mtmtool-1.2.3/src/mtmtool/io.py
--rw-r--r--   0 runner    (1001) docker     (122)      436 2023-04-19 14:28:55.000000 mtmtool-1.2.3/src/mtmtool/itertools.py
--rw-r--r--   0 runner    (1001) docker     (122)     2097 2023-04-19 14:28:55.000000 mtmtool-1.2.3/src/mtmtool/log.py
--rw-r--r--   0 runner    (1001) docker     (122)     1427 2023-04-19 14:28:55.000000 mtmtool-1.2.3/src/mtmtool/pool.py
--rw-r--r--   0 runner    (1001) docker     (122)     3628 2023-04-19 14:28:55.000000 mtmtool-1.2.3/src/mtmtool/projection.py
--rw-r--r--   0 runner    (1001) docker     (122)     1540 2023-04-19 14:28:55.000000 mtmtool-1.2.3/src/mtmtool/time.py
--rw-r--r--   0 runner    (1001) docker     (122)     2322 2023-04-19 14:28:55.000000 mtmtool-1.2.3/src/mtmtool/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:29:08.484391 mtmtool-1.2.3/src/mtmtool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      682 2023-04-19 14:29:08.000000 mtmtool-1.2.3/src/mtmtool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      470 2023-04-19 14:29:08.000000 mtmtool-1.2.3/src/mtmtool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-19 14:29:08.000000 mtmtool-1.2.3/src/mtmtool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-19 14:29:08.000000 mtmtool-1.2.3/src/mtmtool.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-04-19 14:29:08.000000 mtmtool-1.2.3/src/mtmtool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-04-19 14:29:08.000000 mtmtool-1.2.3/src/mtmtool.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:29:08.484391 mtmtool-1.2.3/test/
--rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-04-19 14:28:55.000000 mtmtool-1.2.3/test/test_args2kwargs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 08:42:10.429465 mtmtool-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (122)    11324 2023-05-01 08:41:56.000000 mtmtool-1.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      106 2023-05-01 08:41:56.000000 mtmtool-1.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      682 2023-05-01 08:42:10.429465 mtmtool-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       77 2023-05-01 08:41:56.000000 mtmtool-1.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-01 08:42:10.429465 mtmtool-1.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2026 2023-05-01 08:41:56.000000 mtmtool-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 08:42:10.425464 mtmtool-1.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 08:42:10.429465 mtmtool-1.2.4/src/mtmtool/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-01 08:41:56.000000 mtmtool-1.2.4/src/mtmtool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      685 2023-05-01 08:41:56.000000 mtmtool-1.2.4/src/mtmtool/functool.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1687 2023-05-01 08:41:56.000000 mtmtool-1.2.4/src/mtmtool/io.py
+-rw-r--r--   0 runner    (1001) docker     (122)      436 2023-05-01 08:41:56.000000 mtmtool-1.2.4/src/mtmtool/itertools.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2097 2023-05-01 08:41:56.000000 mtmtool-1.2.4/src/mtmtool/log.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2448 2023-05-01 08:41:56.000000 mtmtool-1.2.4/src/mtmtool/pool.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3628 2023-05-01 08:41:56.000000 mtmtool-1.2.4/src/mtmtool/projection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1540 2023-05-01 08:41:56.000000 mtmtool-1.2.4/src/mtmtool/time.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2393 2023-05-01 08:41:56.000000 mtmtool-1.2.4/src/mtmtool/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 08:42:10.429465 mtmtool-1.2.4/src/mtmtool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      682 2023-05-01 08:42:10.000000 mtmtool-1.2.4/src/mtmtool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      470 2023-05-01 08:42:10.000000 mtmtool-1.2.4/src/mtmtool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-01 08:42:10.000000 mtmtool-1.2.4/src/mtmtool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-01 08:42:10.000000 mtmtool-1.2.4/src/mtmtool.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-01 08:42:10.000000 mtmtool-1.2.4/src/mtmtool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-05-01 08:42:10.000000 mtmtool-1.2.4/src/mtmtool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 08:42:10.429465 mtmtool-1.2.4/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-05-01 08:41:56.000000 mtmtool-1.2.4/test/test_args2kwargs.py
```

### Comparing `mtmtool-1.2.3/LICENSE` & `mtmtool-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mtmtool-1.2.3/PKG-INFO` & `mtmtool-1.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtmtool
-Version: 1.2.3
+Version: 1.2.4
 Summary:  A Personal Python Tool Library.
 Home-page: https://github.com/imutum/imutum_python_tool
 Author: imutum
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Intended Audience :: Developers
```

### Comparing `mtmtool-1.2.3/setup.py` & `mtmtool-1.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os, shutil, sys, glob
 
 package_name = "imutum_python_tool"
 abbreviation_name = "mtmtool"
 description = " A Personal Python Tool Library."
-version = "1.2.3"
+version = "1.2.4"
 
 
 def check_requires(requires: list):
     pip_file = "pip.exe" if "win" in sys.platform else "pip"
     pip_paths = [
         os.path.join(os.path.dirname(sys.executable), "Scripts", pip_file),
         os.path.join(os.path.dirname(sys.executable), pip_file),
```

### Comparing `mtmtool-1.2.3/src/mtmtool/functool.py` & `mtmtool-1.2.4/src/mtmtool/functool.py`

 * *Files identical despite different names*

### Comparing `mtmtool-1.2.3/src/mtmtool/io.py` & `mtmtool-1.2.4/src/mtmtool/io.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from ast import literal_eval
 import pickle
 import json
 import yaml
 import os
 # 加载yaml模块
 try:
     from yaml import CLoader as Loader, CDumper as Dumper
@@ -42,15 +41,15 @@
     with open(path, "w", encoding=encoding) as f:
         f.write(data)
 
 
 def read_json(path):
     with open(path, "r", encoding="utf8") as f:
         data = f.read()
-    res = literal_eval(data)
+    res = json.loads(data)
     return res
 
 
 def write_json(path, data):
     with open(path, "w") as f:
         f.write(json.dumps(data, separators=(',', ':')))
```

### Comparing `mtmtool-1.2.3/src/mtmtool/log.py` & `mtmtool-1.2.4/src/mtmtool/log.py`

 * *Files identical despite different names*

### Comparing `mtmtool-1.2.3/src/mtmtool/pool.py` & `mtmtool-1.2.4/src/mtmtool/pool.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 from functools import partial
 from itertools import product
+from mtmtool.log import create_stream_logger
 from multiprocessing import Pool
 from multiprocessing.pool import ThreadPool
+from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor
 import os
 
-CPUNUM = os.cpu_count() - 2
+logger = create_stream_logger("Pool")
+
+CPUNUM = os.cpu_count()
 
 
 def parfunc(func, *args, **kargs):
     return partial(func, *args, **kargs)
 
 
 """ 
 map 与 starmap 函数的区别:
     map只展开一次, 只能向函数掺入一个参数
     starmap可展开两次, 可以向函数传入多个参数
 product 函数:
     输入多个可迭代参数, 返回所有笛卡尔积元组
 """
+
+
 def pool_process(par_func, iterables, worker_num=CPUNUM):
     with Pool(worker_num) as p:
         res_list = p.map(par_func, iterables)
     return res_list
 
 
 def pool_thread(par_func, iterables, worker_num=CPUNUM):
@@ -44,7 +50,33 @@
         res = []
         for args_t in iters:
             res.append(func(*args_t))
     else:
         with pool(worker_num) as p:
             res = p.starmap(func, iters)
     return res
+
+
+class MapPool:
+    def __init__(self, function=None, max_workers=None, ptype="Thread") -> None:
+        self.max_workers = max_workers
+        self.buffer = []
+        self.set_function(function)
+        self.pool = ProcessPoolExecutor if ptype == "Process" else ThreadPoolExecutor
+
+    def __call__(self, *args, **kwargs):
+        self.buffer.append((args, kwargs))
+        pass
+
+    def set_function(self, func):
+        self.function = func
+
+    def worker_wrapper(self, arg):
+        args, kwargs = arg
+        return self.function(*args, **kwargs)
+
+    def result(self):
+        logger.info("Start running with {} workers, {} tasks".format(self.max_workers), len(self.buffer))
+        with ProcessPoolExecutor(max_workers=self.max_workers) as executor:
+            res = executor.map(self.worker_wrapper, self.buffer)
+        self.buffer = []
+        return res
```

### Comparing `mtmtool-1.2.3/src/mtmtool/projection.py` & `mtmtool-1.2.4/src/mtmtool/projection.py`

 * *Files identical despite different names*

### Comparing `mtmtool-1.2.3/src/mtmtool/time.py` & `mtmtool-1.2.4/src/mtmtool/time.py`

 * *Files identical despite different names*

### Comparing `mtmtool-1.2.3/src/mtmtool/webhook.py` & `mtmtool-1.2.4/src/mtmtool/webhook.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 import requests
 import json
 
 
 def auto_send(message, *args, **kwargs):
-    if args[0].lower() == "telegram":
-        return telegram(message, *args[1:], **kwargs)
-    if args[0].lower() == "pushplus":
-        return pushplus(message, *args[1:], **kwargs)
-    if args[0].lower() == "wechat":
-        return wechat(message, *args[1:], **kwargs)
-    if args[0].lower() == "qq":
-        return qq(message, *args[1:], **kwargs)
-    raise ValueError(f"Not Support API Type {args[0]}")
+    if kwargs.get("platform", None):
+        platform = kwargs["platform"]
+    elif len(args) > 0:
+        args = list(args)
+        platform = args.pop(0).lower()
+    else:
+        raise ValueError(f"API Platform Not Found.")
+    if platform in globals() and callable(globals()[platform]):
+        return globals()[platform](message, *args[1:], **kwargs)
+    raise ValueError(f"Not Support API Platform {args[0]}")
 
 
-def dingding(text, key: str = "", **kargs):
+def dingding(text, key: str = "", **kwargs):
     url = 'https://oapi.dingtalk.com/robot/send?access_token=' + key
     if ':' not in text and "." not in text and "," not in text and "。" not in text:
         text += "."
     data = {
         "msgtype": "text",
         "text": {
             "content": text
         },
     }
     headers = {"Content-Type": "application/json ;charset=utf-8 "}
     html = requests.post(url, data=json.dumps(data), headers=headers)
     return html.ok
 
 
-def wechat(text, key: str = "", **kargs):
+def wechat(text, key: str = "", **kwargs):
     url = 'https://qyapi.weixin.qq.com/cgi-bin/webhook/send?key=' + key
     data = {
         "msgtype": "text",
         "text": {
             "content": text
         },
     }
@@ -45,31 +46,33 @@
 def qq(text, key: str = ""):
     url = "https://qmsg.zendee.cn/send/" + key
     data = {'msg': text}
     html = requests.post(url, data=data)
     return html.ok
 
 
-def mi(text, key: str = "", title="bot", **kargs):
+def mi(text, key: str = "", title="bot", **kwargs):
     url = "https://tdtt.top/send"
     data = {"title": title, "content": text, "alias": key}
     response = requests.post(url, data=data)
     return response.ok
 
 
-def telegram(text: str, bot: str, chat: str, protect_content=False, host="api.telegram.org", **kargs):
-    bot_token = bot
-    chat_id = chat
-    url = f"https://{host}/bot{bot_token}/sendMessage"
+def telegram(text: str, token: str, chat: str, host="api.telegram.org", mono=False, **kwargs):
+    url = f"https://{host}/bot{token}/sendMessage"
+    # 设置字体为等宽字体
+    if mono and "parse_mode" not in kwargs:
+        text = f"<pre>{text}</pre>"
+        kwargs["parse_mode"] = "HTML"
+
     data = {
-        "chat_id": chat_id,
+        "chat_id": chat,
         "text": text,
-        "protect_content": protect_content,
+        **kwargs,
     }
-    res = requests.get(url, data=data)
-    return res.json()
+    return requests.get(url, data=data).json()
 
 
-def pushplus(message, token, title="default", template="html", **kargs):
+def pushplus(message, token, title="default", template="html", **kwargs):
     url = f'http://www.pushplus.plus/send?token={token}&title={title}&content={message}&template={template}'
     resq = requests.get(url=url)
     return resq.text
```

### Comparing `mtmtool-1.2.3/src/mtmtool.egg-info/PKG-INFO` & `mtmtool-1.2.4/src/mtmtool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtmtool
-Version: 1.2.3
+Version: 1.2.4
 Summary:  A Personal Python Tool Library.
 Home-page: https://github.com/imutum/imutum_python_tool
 Author: imutum
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Intended Audience :: Developers
```

### Comparing `mtmtool-1.2.3/test/test_args2kwargs.py` & `mtmtool-1.2.4/test/test_args2kwargs.py`

 * *Files identical despite different names*

