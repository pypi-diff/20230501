# Comparing `tmp/nonebot_plugin_zyk_lightNVL-0.1.1.tar.gz` & `tmp/nonebot_plugin_zyk_lightNVL-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_zyk_lightNVL-0.1.1.tar", last modified: Sat Feb  4 06:12:04 2023, max compression
+gzip compressed data, was "nonebot_plugin_zyk_lightNVL-0.2.tar", last modified: Mon May  1 13:05:58 2023, max compression
```

## Comparing `nonebot_plugin_zyk_lightNVL-0.1.1.tar` & `nonebot_plugin_zyk_lightNVL-0.2.tar`

### file list

```diff
@@ -1,17 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-02-04 06:12:04.014754 nonebot_plugin_zyk_lightNVL-0.1.1/
--rw-rw-rw-   0        0        0     1083 2023-01-19 12:36:51.000000 nonebot_plugin_zyk_lightNVL-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      268 2023-02-04 06:12:04.014754 nonebot_plugin_zyk_lightNVL-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2727 2023-02-04 06:11:48.000000 nonebot_plugin_zyk_lightNVL-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-02-04 06:12:03.993811 nonebot_plugin_zyk_lightNVL-0.1.1/nonebot_plugin_zyk_lightNVL/
--rw-rw-rw-   0        0        0     5949 2023-02-04 06:09:39.000000 nonebot_plugin_zyk_lightNVL-0.1.1/nonebot_plugin_zyk_lightNVL/__init__.py
--rw-rw-rw-   0        0        0      595 2023-01-27 14:07:37.000000 nonebot_plugin_zyk_lightNVL-0.1.1/nonebot_plugin_zyk_lightNVL/config.py
--rw-rw-rw-   0        0        0      318 2023-02-04 05:53:43.000000 nonebot_plugin_zyk_lightNVL-0.1.1/nonebot_plugin_zyk_lightNVL/template.html
--rw-rw-rw-   0        0        0     5051 2023-02-04 05:39:49.000000 nonebot_plugin_zyk_lightNVL-0.1.1/nonebot_plugin_zyk_lightNVL/work.py
-drwxrwxrwx   0        0        0        0 2023-02-04 06:12:04.013757 nonebot_plugin_zyk_lightNVL-0.1.1/nonebot_plugin_zyk_lightNVL.egg-info/
--rw-rw-rw-   0        0        0      268 2023-02-04 06:12:03.000000 nonebot_plugin_zyk_lightNVL-0.1.1/nonebot_plugin_zyk_lightNVL.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      436 2023-02-04 06:12:03.000000 nonebot_plugin_zyk_lightNVL-0.1.1/nonebot_plugin_zyk_lightNVL.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-04 06:12:03.000000 nonebot_plugin_zyk_lightNVL-0.1.1/nonebot_plugin_zyk_lightNVL.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       93 2023-02-04 06:12:03.000000 nonebot_plugin_zyk_lightNVL-0.1.1/nonebot_plugin_zyk_lightNVL.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-02-04 06:12:03.000000 nonebot_plugin_zyk_lightNVL-0.1.1/nonebot_plugin_zyk_lightNVL.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-04 06:12:04.014754 nonebot_plugin_zyk_lightNVL-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      558 2023-02-04 05:50:36.000000 nonebot_plugin_zyk_lightNVL-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 13:05:58.738841 nonebot_plugin_zyk_lightNVL-0.2/
+-rw-rw-rw-   0        0        0     1083 2023-04-20 14:30:24.000000 nonebot_plugin_zyk_lightNVL-0.2/LICENSE
+-rw-rw-rw-   0        0        0      266 2023-05-01 13:05:58.736841 nonebot_plugin_zyk_lightNVL-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2727 2023-04-20 14:30:24.000000 nonebot_plugin_zyk_lightNVL-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 13:05:58.667837 nonebot_plugin_zyk_lightNVL-0.2/nonebot_plugin_zyk_lightNVL/
+-rw-rw-rw-   0        0        0     6291 2023-05-01 12:55:09.000000 nonebot_plugin_zyk_lightNVL-0.2/nonebot_plugin_zyk_lightNVL/__init__.py
+-rw-rw-rw-   0        0        0     1218 2023-05-01 13:04:33.000000 nonebot_plugin_zyk_lightNVL-0.2/nonebot_plugin_zyk_lightNVL/config.py
+drwxrwxrwx   0        0        0        0 2023-05-01 13:05:58.729840 nonebot_plugin_zyk_lightNVL-0.2/nonebot_plugin_zyk_lightNVL/phantomjs/
+-rw-rw-rw-   0        0        0    17204 2016-01-24 08:41:06.000000 nonebot_plugin_zyk_lightNVL-0.2/nonebot_plugin_zyk_lightNVL/phantomjs/ChangeLog
+-rw-rw-rw-   0        0        0     1429 2016-01-24 08:41:06.000000 nonebot_plugin_zyk_lightNVL-0.2/nonebot_plugin_zyk_lightNVL/phantomjs/LICENSE.BSD
+-rw-rw-rw-   0        0        0     2502 2016-01-24 08:41:06.000000 nonebot_plugin_zyk_lightNVL-0.2/nonebot_plugin_zyk_lightNVL/phantomjs/README.md
+-rw-rw-rw-   0        0        0     1510 2016-01-24 08:41:06.000000 nonebot_plugin_zyk_lightNVL-0.2/nonebot_plugin_zyk_lightNVL/phantomjs/third-party.txt
+-rw-rw-rw-   0        0        0        0 2023-05-01 12:57:57.000000 nonebot_plugin_zyk_lightNVL-0.2/nonebot_plugin_zyk_lightNVL/template.html
+-rw-rw-rw-   0        0        0     4566 2023-05-01 12:55:42.000000 nonebot_plugin_zyk_lightNVL-0.2/nonebot_plugin_zyk_lightNVL/work.py
+drwxrwxrwx   0        0        0        0 2023-05-01 13:05:58.702839 nonebot_plugin_zyk_lightNVL-0.2/nonebot_plugin_zyk_lightNVL.egg-info/
+-rw-rw-rw-   0        0        0      266 2023-05-01 13:05:58.000000 nonebot_plugin_zyk_lightNVL-0.2/nonebot_plugin_zyk_lightNVL.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      636 2023-05-01 13:05:58.000000 nonebot_plugin_zyk_lightNVL-0.2/nonebot_plugin_zyk_lightNVL.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 13:05:58.000000 nonebot_plugin_zyk_lightNVL-0.2/nonebot_plugin_zyk_lightNVL.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      125 2023-05-01 13:05:58.000000 nonebot_plugin_zyk_lightNVL-0.2/nonebot_plugin_zyk_lightNVL.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-05-01 13:05:58.000000 nonebot_plugin_zyk_lightNVL-0.2/nonebot_plugin_zyk_lightNVL.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-01 13:05:58.741841 nonebot_plugin_zyk_lightNVL-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      609 2023-05-01 13:03:10.000000 nonebot_plugin_zyk_lightNVL-0.2/setup.py
```

### Comparing `nonebot_plugin_zyk_lightNVL-0.1.1/LICENSE` & `nonebot_plugin_zyk_lightNVL-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_zyk_lightNVL-0.1.1/README.md` & `nonebot_plugin_zyk_lightNVL-0.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_zyk_lightNVL-0.1.1/nonebot_plugin_zyk_lightNVL/work.py` & `nonebot_plugin_zyk_lightNVL-0.2/nonebot_plugin_zyk_lightNVL/work.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 from httpx import AsyncClient
 import re
-from os import path
-from lxml import html
-from nonebot_plugin_htmlrender import html_to_pic
 from fake_useragent import UserAgent
 from time import time
+from .config import *
 
 
 async def get_checkcode():
     checkcode_api = "https://w.linovelib.com/checkcode.php"
     headers = {
         "origin": "https://w.linovelib.com",
         "referer": "https://w.linovelib.com/login.php",
         "User-Agent": UserAgent().random
     }
     param = {
         "rand": int(time())
     }
 
-    client = AsyncClient(headers=headers, timeout=None)
+    client = AsyncClient(headers=headers, timeout=None, cookies=cookies)
     r = await client.get(checkcode_api, params=param)
 
     return client, r.content
 
 
 async def login(client: AsyncClient, username, password, checkcode):
     login_api = "https://w.linovelib.com/login.php?do=submit&jumpurl=https%3A%2F%2Fw.linovelib.com%2F"
@@ -32,116 +30,118 @@
         "checkcode": checkcode,
         "act": "login",
         "usecookie": "86400",
         "submit": ""
     }
     resp = await client.post(url=login_api, data=data)
 
+    # 登录成功将会重定向
     if resp.status_code != 302:
         info = re.findall(r'<div class="aui-ver-form">(.*?)<br>', resp.text, re.S)[0].replace("\n", "")
         return False, info
-    else:
-        cookie_path = path.join(path.abspath(path.dirname(__file__)), "cookie.txt")
-        with open(file=cookie_path, mode="w", encoding="utf-8") as f:
-            f.write(resp.headers["set-cookie"])
-        return True, client
+
+    client.follow_redirects = True
+        
+    return True, client
 
 
 async def search(client: AsyncClient, name, retry_num):
 
     # 检索书名
-    url = "https://w.linovelib.com/S8/"
+    url = "https://w.linovelib.com/search.html"
     data = {
         "searchkey": name,
-        "searchtype": "all"
+    }
+    headers = {
+        "referer": "https://w.linovelib.com/search.html",
+        "oringin": "https://w.linovelib.com",
+        "method": "POST",
+        "User-Agent": UserAgent().random
     }
 
-    resp = await client.get(url=url, params=data)
+    resp = await client.post(url=url, data=data, headers=headers)
     info = resp.text
 
-    # 获取书名信息列表
-    book_list = re.findall(r'class="book-cover" alt="(.*?)">', info)
+    # 重定向（直接跳转到书页）
+    if "/novel/" in str(resp.url):
+        return "book_page", info
 
     # 没有重定向且有多个结果
-    if len(book_list) > 1:
-        href_list = [
-            "https://w.linovelib.com" + href
-            for href in re.findall(r'<a href="(.*?)" class="book-layout"', info)
-        ]
-        next_page = re.findall(r'</span><a href="(.*?)" class="next">', info)[0]
-        if next_page == "#":
+    elif '<meta name="robots" content="noindex,nofollow">' not in info:
+        book_list, href_list, next_page = search_parse(info)
+        if (next_page is None) or (show_all is False):
             return book_list, href_list
 
-        # 不止一页
+        # 不止一页，根据retry_num选择需要多少页
         if retry_num < 30:
             page = 1
         else:
             page = retry_num // 30
             if retry_num % 30 != 0:
                 page += 1
 
-        for _ in range(page-1):
+        for _ in range(page - 1):
             if next_page == "#":
                 break
-            next_page = "https://w.linovelib.com" + next_page
             info = (await client.get(url=next_page)).text
             # 获取书名信息列表
             books = re.findall(r'class="book-cover" alt="(.*?)">', info)
             hrefs = [
                 "https://w.linovelib.com" + href
                 for href in re.findall(r'<a href="(.*?)" class="book-layout"', info)
             ]
             book_list += books
             href_list += hrefs
-
+            
             next_page = re.findall(r'</span><a href="(.*?)" class="next">', info)[0]
 
         return book_list, href_list
 
-    # 重定向（直接跳转到书页）
-    elif "/novel/" in str(resp.url):
-        pattern = re.compile(r'<meta property="og:title" content="(.*?)" />')
-        book_name = [re.findall(pattern, info)[0]]
-
-        return book_name, [str(resp.url)]
-
+    # 无结果
     else:
         return False
 
 
-async def get_content(client: AsyncClient, book_url):
-    book_info = (await client.get(url=book_url)).text
+def search_parse(res):
+    # 获取书名信息列表
+    book_list = re.findall(r'alt="(.*?)"', res, re.S)
+    href_list = [
+        "https://w.linovelib.com" + href
+        for href in re.findall(r'<li class="book-li"><a href="(.*?)" class="book-layout">', res)
+    ]
+    next_page = re.findall(r'</span><a href="(.*?)" class="next">', res)[0]
+    if next_page == "#":
+        return book_list, href_list, None
+    else:
+        return book_list, href_list, "https://w.linovelib.com" + next_page
+
 
-    content_pattern = re.compile(r'(<div class="module module-merge">.*?)<div class="module">', re.S)
-    index_pattern = re.compile(r'<li class="btn-group-cell"><a href="(.*?)"')
-    info_pattern = re.compile(r'<div id="bookDetailWrapper" class="module module-merge book-detail-x">.*?</span>\n</p>\n\n</div>\n</div>', re.S)
+async def get_content(book_info):
 
-    info = re.findall(info_pattern, book_info)[0]
+    content_pattern = re.compile(r'(<!DOCTYPE html>.*)<style>.page-fans', re.S)
+ 
     content = re.findall(content_pattern, book_info)[0]
-    index_url = "https://w.linovelib.com" + re.findall(index_pattern, book_info)[0]
-
-    try:
-        book_id = re.findall(r'https://w.linovelib.com/novel/(\d+).html', book_url)[0]
-    except IndexError:
-        book_id = re.findall(r'acode=i_(\d+)', book_url)[0]
 
     html_path = path.join(path.abspath(path.dirname(__file__)), "template.html")
-    with open(html_path, "r", encoding="utf-8") as h:
-        template = h.read()
-    content = template.format(content=content, info=info)
-    pic = await html_to_pic(html=content)
+    with open(html_path, "w+", encoding="utf-8") as h:
+        h.write(content)
 
-    return pic, index_url, book_id
+    driver.get(f'file:///{html_path}')
+    driver.implicitly_wait(1)
+    pic = driver.get_screenshot_as_png()
+
+    return pic
 
 
 async def get_bookcase(client: AsyncClient):
     resp = await client.get(url="https://w.linovelib.com/bookcase.php")
 
     if "login" in str(resp.url):
         return False
+
     case_info = resp.text
     book_pattern = re.compile(r'<h4 class="book-title">(.*?)</h4>')
     url_pattern = re.compile(r'<a href="(.*?)" class="mybook-to-detail">')
     books = re.findall(book_pattern, case_info)
     urls = re.findall(url_pattern, case_info)
 
     return books, urls
```

#### html2text {}

 * *error from `html2text {}` (b):*

 * *File "/tmp/diffoscope_lvvoinos_/tmpqdkd5cvf_TarContainer/0/13.py", line 148, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_lvvoinos_/tmpqdkd5cvf_TarContainer/0/13.py", line 148, column 0: CDATA terminal not found*

```diff
@@ -1,58 +1,41 @@
-from httpx import AsyncClient import re from os import path from lxml import
-html from nonebot_plugin_htmlrender import html_to_pic from fake_useragent
-import UserAgent from time import time async def get_checkcode(): checkcode_api
-= "https://w.linovelib.com/checkcode.php" headers = { "origin": "https://
-w.linovelib.com", "referer": "https://w.linovelib.com/login.php", "User-Agent":
-UserAgent().random } param = { "rand": int(time()) } client = AsyncClient
-(headers=headers, timeout=None) r = await client.get(checkcode_api,
-params=param) return client, r.content async def login(client: AsyncClient,
-username, password, checkcode): login_api = "https://w.linovelib.com/
-login.php?do=submit&jumpurl=https%3A%2F%2Fw.linovelib.com%2F" data =
-{ "username": username, "password": password, "checkcode": checkcode, "act":
-"login", "usecookie": "86400", "submit": "" } resp = await client.post
-(url=login_api, data=data) if resp.status_code != 302: info = re.findall(r'
+from httpx import AsyncClient import re from fake_useragent import UserAgent
+from time import time from .config import * async def get_checkcode():
+checkcode_api = "https://w.linovelib.com/checkcode.php" headers = { "origin":
+"https://w.linovelib.com", "referer": "https://w.linovelib.com/login.php",
+"User-Agent": UserAgent().random } param = { "rand": int(time()) } client =
+AsyncClient(headers=headers, timeout=None, cookies=cookies) r = await
+client.get(checkcode_api, params=param) return client, r.content async def
+login(client: AsyncClient, username, password, checkcode): login_api = "https:/
+/w.linovelib.com/login.php?do=submit&jumpurl=https%3A%2F%2Fw.linovelib.com%2F"
+data = { "username": username, "password": password, "checkcode": checkcode,
+"act": "login", "usecookie": "86400", "submit": "" } resp = await client.post
+(url=login_api, data=data) # ç»å½æåå°ä¼éå®å if resp.status_code !=
+302: info = re.findall(r'
 (.*?)
-', resp.text, re.S)[0].replace("\n", "") return False, info else: cookie_path =
-path.join(path.abspath(path.dirname(__file__)), "cookie.txt") with open
-(file=cookie_path, mode="w", encoding="utf-8") as f: f.write(resp.headers["set-
-cookie"]) return True, client async def search(client: AsyncClient, name,
-retry_num): # æ£ç´¢ä¹¦å url = "https://w.linovelib.com/S8/" data =
-{ "searchkey": name, "searchtype": "all" } resp = await client.get(url=url,
-params=data) info = resp.text # è·åä¹¦åä¿¡æ¯åè¡¨ book_list = re.findall
-(r'class="book-cover" alt="(.*?)">', info) # æ²¡æéå®åä¸æå¤ä¸ªç»æ
-if len(book_list) > 1: href_list = [ "https://w.linovelib.com" + href for href
-in re.findall(r'
-, info) ] next_page = re.findall(r'',_info)[0]_if_next_page_==_"#":_return
-book_list,_href_list_#_ä¸æ­¢ä¸é¡µ_if_retry_num_<_30:_page_=_1_else:_page_=
-retry_num_//_30_if_retry_num_%_30_!=_0:_page_+=_1_for___in_range(page-1):_if
-next_page_==_"#":_break_next_page_=_"https://w.linovelib.com"_+_next_page_info
-=_(await_client.get(url=next_page)).text_#_è·åä¹¦åä¿¡æ¯åè¡¨_books_=
-re.findall(r'class="book-cover"_alt="(.*?)">',_info)_hrefs_=_[_"https://
-w.linovelib.com"_+_href_for_href_in_re.findall(r',_info)_]_book_list_+=_books
-href_list_+=_hrefs_next_page_=_re.findall(r'',_info)[0]_return_book_list,
-href_list_#_éå®åï¼ç´æ¥è·³è½¬å°ä¹¦é¡µï¼_elif_"/novel/"_in_str
-(resp.url):_pattern_=_re.compile(r'
-') book_name = [re.findall(pattern, info)[0]] return book_name, [str(resp.url)]
-else: return False async def get_content(client: AsyncClient, book_url):
-book_info = (await client.get(url=book_url)).text content_pattern = re.compile
-(r'(
-.*?)
-', re.S) index_pattern = re.compile(r'
-) info_pattern = re.compile(r'
-.*?\n
-\n\n
-\n
-', re.S) info = re.findall(info_pattern, book_info)[0] content = re.findall
-(content_pattern, book_info)[0] index_url = "https://w.linovelib.com" +
-re.findall(index_pattern, book_info)[0] try: book_id = re.findall(r'https://
-w.linovelib.com/novel/(\d+).html', book_url)[0] except IndexError: book_id =
-re.findall(r'acode=i_(\d+)', book_url)[0] html_path = path.join(path.abspath
-(path.dirname(__file__)), "template.html") with open(html_path, "r",
-encoding="utf-8") as h: template = h.read() content = template.format
-(content=content, info=info) pic = await html_to_pic(html=content) return pic,
-index_url, book_id async def get_bookcase(client: AsyncClient): resp = await
-client.get(url="https://w.linovelib.com/bookcase.php") if "login" in str
-(resp.url): return False case_info = resp.text book_pattern = re.compile(r'
-*** (.*?) ***
-') url_pattern = re.compile(r'')_books_=_re.findall(book_pattern,_case_info)
-urls_=_re.findall(url_pattern,_case_info)_return_books,_urls_
+', resp.text, re.S)[0].replace("\n", "") return False, info
+client.follow_redirects = True return True, client async def search(client:
+AsyncClient, name, retry_num): # æ£ç´¢ä¹¦å url = "https://w.linovelib.com/
+search.html" data = { "searchkey": name, } headers = { "referer": "https://
+w.linovelib.com/search.html", "oringin": "https://w.linovelib.com", "method":
+"POST", "User-Agent": UserAgent().random } resp = await client.post(url=url,
+data=data, headers=headers) info = resp.text #
+éå®åï¼ç´æ¥è·³è½¬å°ä¹¦é¡µï¼ if "/novel/" in str(resp.url): return
+"book_page", info # æ²¡æéå®åä¸æå¤ä¸ªç»æ elif '
+' not in info: book_list, href_list, next_page = search_parse(info) if
+(next_page is None) or (show_all is False): return book_list, href_list #
+ä¸æ­¢ä¸é¡µï¼æ ¹æ®retry_numéæ©éè¦å¤å°é¡µ if retry_num < 30: page = 1
+else: page = retry_num // 30 if retry_num % 30 != 0: page += 1 for _ in range
+(page - 1): if next_page == "#": break info = (await client.get
+(url=next_page)).text # è·åä¹¦åä¿¡æ¯åè¡¨ books = re.findall
+(r'class="book-cover" alt="(.*?)">', info) hrefs = [ "https://w.linovelib.com"
++ href for href in re.findall(r'
+, info) ] book_list += books href_list += hrefs next_page = re.findall(r'',
+info)[0]_return_book_list,_href_list_#_æ ç»æ_else:_return_False_def
+search_parse(res):_#_è·åä¹¦åä¿¡æ¯åè¡¨_book_list_=_re.findall(r'alt="
+(.*?)"',_res,_re.S)_href_list_=_[_"https://w.linovelib.com"_+_href_for_href_in
+re.findall(r'
+',_res)_]_next_page_=_re.findall(r'',_res)[0]_if_next_page_==_"#":_return
+book_list,_href_list,_None_else:_return_book_list,_href_list,_"https://
+w.linovelib.com"_+_next_page_async_def_get_content(book_info):_content_pattern
+=_re.compile(r'(
+.*)
```

### Comparing `nonebot_plugin_zyk_lightNVL-0.1.1/setup.py` & `nonebot_plugin_zyk_lightNVL-0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name='nonebot_plugin_zyk_lightNVL',
-    version='0.1.1',
+    version='0.2',
     packages=find_packages(),
     url='https://github.com/ZYKsslm/nonebot_plugin_zyk_lightNVL',
     license='MIT LICENSE',
     author='ZYKsslm',
     author_email='3119964735@qq.com',
     description='A plugin for nonebot2',
-    install_requires=["httpx", "colorama", "lxml", "fake_useragent", "nonebot2", "nonebot_plugin_htmlrender", "nonebot_adapter_onebot"],
-    package_data={"nonebot_plugin_zyk_lightNVL": ["template.html"]}
+    install_requires=["httpx", "colorama", "lxml", "fake_useragent", "nonebot2", "nonebot_plugin_htmlrender", "nonebot_adapter_onebot", "selenium<=3.3.0", "browser_cookie3"],
+    package_data={"nonebot_plugin_zyk_lightNVL": ["template.html", "phantomjs/*"]}
 )
```

