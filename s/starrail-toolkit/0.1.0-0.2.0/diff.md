# Comparing `tmp/starrail-toolkit-0.1.0.tar.gz` & `tmp/starrail-toolkit-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starrail-toolkit-0.1.0.tar", last modified: Sun Apr 30 15:09:01 2023, max compression
+gzip compressed data, was "starrail-toolkit-0.2.0.tar", last modified: Mon May  1 16:53:28 2023, max compression
```

## Comparing `starrail-toolkit-0.1.0.tar` & `starrail-toolkit-0.2.0.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-04-30 15:09:01.420953 starrail-toolkit-0.1.0/
--rw-r--r--   0 littlenyima   (501) staff       (20)    35149 2023-04-29 06:29:57.000000 starrail-toolkit-0.1.0/LICENSE
--rw-r--r--   0 littlenyima   (501) staff       (20)     1940 2023-04-30 15:09:01.420815 starrail-toolkit-0.1.0/PKG-INFO
--rw-r--r--   0 littlenyima   (501) staff       (20)     1433 2023-04-30 13:32:47.000000 starrail-toolkit-0.1.0/README.md
--rw-r--r--   0 littlenyima   (501) staff       (20)       38 2023-04-30 15:09:01.420995 starrail-toolkit-0.1.0/setup.cfg
--rw-r--r--   0 littlenyima   (501) staff       (20)     4153 2023-04-30 15:06:02.000000 starrail-toolkit-0.1.0/setup.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-04-30 15:09:01.418022 starrail-toolkit-0.1.0/starrail/
--rw-r--r--   0 littlenyima   (501) staff       (20)      129 2023-04-30 09:44:16.000000 starrail-toolkit-0.1.0/starrail/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1257 2023-04-30 12:12:07.000000 starrail-toolkit-0.1.0/starrail/config.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-04-30 15:09:01.418437 starrail-toolkit-0.1.0/starrail/entry/
--rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-04-29 12:32:44.000000 starrail-toolkit-0.1.0/starrail/entry/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      949 2023-04-30 13:23:58.000000 starrail-toolkit-0.1.0/starrail/entry/cli.py
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-04-29 06:50:14.000000 starrail-toolkit-0.1.0/starrail/entry/gui.py
--rw-r--r--   0 littlenyima   (501) staff       (20)       85 2023-04-30 09:44:16.000000 starrail-toolkit-0.1.0/starrail/entry/setup.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-04-30 15:09:01.419710 starrail-toolkit-0.1.0/starrail/gacha/
--rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-04-29 12:32:48.000000 starrail-toolkit-0.1.0/starrail/gacha/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     6599 2023-04-30 12:57:13.000000 starrail-toolkit-0.1.0/starrail/gacha/database.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      817 2023-04-30 12:01:56.000000 starrail-toolkit-0.1.0/starrail/gacha/fetch.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1981 2023-04-30 12:57:47.000000 starrail-toolkit-0.1.0/starrail/gacha/fileio.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     2399 2023-04-30 12:21:48.000000 starrail-toolkit-0.1.0/starrail/gacha/parse.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3225 2023-04-30 13:32:48.000000 starrail-toolkit-0.1.0/starrail/gacha/service.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      501 2023-04-29 09:16:22.000000 starrail-toolkit-0.1.0/starrail/gacha/type.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3448 2023-04-30 09:44:08.000000 starrail-toolkit-0.1.0/starrail/gacha/url.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-04-30 15:09:01.419919 starrail-toolkit-0.1.0/starrail/utils/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-04-30 09:40:38.000000 starrail-toolkit-0.1.0/starrail/utils/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      547 2023-04-30 12:57:13.000000 starrail-toolkit-0.1.0/starrail/utils/loggings.py
--rw-r--r--   0 littlenyima   (501) staff       (20)       22 2023-04-30 12:58:21.000000 starrail-toolkit-0.1.0/starrail/version.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-04-30 15:09:01.420621 starrail-toolkit-0.1.0/starrail_toolkit.egg-info/
--rw-r--r--   0 littlenyima   (501) staff       (20)     1940 2023-04-30 15:09:01.000000 starrail-toolkit-0.1.0/starrail_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 littlenyima   (501) staff       (20)      675 2023-04-30 15:09:01.000000 starrail-toolkit-0.1.0/starrail_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)        1 2023-04-30 15:09:01.000000 starrail-toolkit-0.1.0/starrail_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)       54 2023-04-30 15:09:01.000000 starrail-toolkit-0.1.0/starrail_toolkit.egg-info/entry_points.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)       36 2023-04-30 15:09:01.000000 starrail-toolkit-0.1.0/starrail_toolkit.egg-info/requires.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)        9 2023-04-30 15:09:01.000000 starrail-toolkit-0.1.0/starrail_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-01 16:53:28.895466 starrail-toolkit-0.2.0/
+-rw-r--r--   0 littlenyima   (501) staff       (20)    35149 2023-04-29 06:29:57.000000 starrail-toolkit-0.2.0/LICENSE
+-rw-r--r--   0 littlenyima   (501) staff       (20)     2417 2023-05-01 16:53:28.895319 starrail-toolkit-0.2.0/PKG-INFO
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1910 2023-05-01 16:51:58.000000 starrail-toolkit-0.2.0/README.md
+-rw-r--r--   0 littlenyima   (501) staff       (20)       38 2023-05-01 16:53:28.895503 starrail-toolkit-0.2.0/setup.cfg
+-rw-r--r--   0 littlenyima   (501) staff       (20)     4153 2023-04-30 15:17:38.000000 starrail-toolkit-0.2.0/setup.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-01 16:53:28.892528 starrail-toolkit-0.2.0/starrail/
+-rw-r--r--   0 littlenyima   (501) staff       (20)      724 2023-05-01 08:24:52.000000 starrail-toolkit-0.2.0/starrail/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1257 2023-04-30 15:17:38.000000 starrail-toolkit-0.2.0/starrail/config.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-01 16:53:28.893125 starrail-toolkit-0.2.0/starrail/entry/
+-rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-04-30 15:17:38.000000 starrail-toolkit-0.2.0/starrail/entry/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      957 2023-05-01 15:00:08.000000 starrail-toolkit-0.2.0/starrail/entry/cli.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)       71 2023-05-01 08:24:52.000000 starrail-toolkit-0.2.0/starrail/entry/gui.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1133 2023-05-01 16:49:09.000000 starrail-toolkit-0.2.0/starrail/entry/setup.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-01 16:53:28.894162 starrail-toolkit-0.2.0/starrail/gacha/
+-rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-04-30 15:17:38.000000 starrail-toolkit-0.2.0/starrail/gacha/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     6599 2023-04-30 15:17:38.000000 starrail-toolkit-0.2.0/starrail/gacha/database.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      817 2023-04-30 15:17:38.000000 starrail-toolkit-0.2.0/starrail/gacha/fetch.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3077 2023-05-01 15:06:41.000000 starrail-toolkit-0.2.0/starrail/gacha/fileio.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5088 2023-05-01 14:41:54.000000 starrail-toolkit-0.2.0/starrail/gacha/parse.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3365 2023-05-01 16:53:15.000000 starrail-toolkit-0.2.0/starrail/gacha/service.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      501 2023-04-30 15:17:38.000000 starrail-toolkit-0.2.0/starrail/gacha/type.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3448 2023-04-30 15:17:38.000000 starrail-toolkit-0.2.0/starrail/gacha/url.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-01 16:53:28.894271 starrail-toolkit-0.2.0/starrail/gui/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-01 08:02:28.000000 starrail-toolkit-0.2.0/starrail/gui/__init__.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-01 16:53:28.894445 starrail-toolkit-0.2.0/starrail/utils/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-04-30 15:17:38.000000 starrail-toolkit-0.2.0/starrail/utils/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      546 2023-04-30 15:36:19.000000 starrail-toolkit-0.2.0/starrail/utils/loggings.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)       22 2023-05-01 14:42:38.000000 starrail-toolkit-0.2.0/starrail/version.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-01 16:53:28.895150 starrail-toolkit-0.2.0/starrail_toolkit.egg-info/
+-rw-r--r--   0 littlenyima   (501) staff       (20)     2417 2023-05-01 16:53:28.000000 starrail-toolkit-0.2.0/starrail_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 littlenyima   (501) staff       (20)      700 2023-05-01 16:53:28.000000 starrail-toolkit-0.2.0/starrail_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)        1 2023-05-01 16:53:28.000000 starrail-toolkit-0.2.0/starrail_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)       54 2023-05-01 16:53:28.000000 starrail-toolkit-0.2.0/starrail_toolkit.egg-info/entry_points.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)       46 2023-05-01 16:53:28.000000 starrail-toolkit-0.2.0/starrail_toolkit.egg-info/requires.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)        9 2023-05-01 16:53:28.000000 starrail-toolkit-0.2.0/starrail_toolkit.egg-info/top_level.txt
```

### Comparing `starrail-toolkit-0.1.0/LICENSE` & `starrail-toolkit-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.1.0/PKG-INFO` & `starrail-toolkit-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,66 +1,82 @@
 Metadata-Version: 2.1
 Name: starrail-toolkit
-Version: 0.1.0
+Version: 0.2.0
 Summary: Honkai Star Rail Toolkit
 Home-page: https://github.com/LittleNyima/honkai-starrail-toolkit
 Author: LittleNyima
 Author-email: littlenyima@163.com
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 《崩坏：星穹铁道》工具箱
 
+<div style="min-height: 275px">
 <img src="https://s1.ax1x.com/2023/04/30/p98Cv26.png" alt="logo" align="left" vertical-align="center" />
 
 ```
 Starrail Toolkit
 
-- 主分支版本：0.1.0
-- 开发分支版本：0.1.0
+- 主分支版本：0.2.0
+- 开发分支版本：0.2.0
+- PyPI 版本：0.2.0
 ```
+</div>
 
 <br clear="left">
 
 ## 开发状态
 
 - [x] 支持命令行导出 csv、xlsx、json 格式抽卡记录
-- [ ] 支持命令行显示抽卡报告
+- [x] 支持命令行显示抽卡报告
+- [x] 支持导出 markdown 格式抽卡报告
 - [ ] 支持导出网页版抽卡报告
 - [ ] 支持 Windows 平台游戏中自动检测 API URL
 - [ ] 实现用户界面并编译到 Windows 与 macOS 平台
 - [ ] 支持自动检查更新
 
+## 导出结果示例
+
+- Excel 结果示例（为保护隐私已隐藏部分信息）
+
+  ![xlsx](https://s1.ax1x.com/2023/05/02/p9GJKts.md.png)
+
+- Markdown 结果示例：
+
+  ![markdown](https://s1.ax1x.com/2023/05/02/p9GJMhn.md.png)
+
 ## 安装方式
 
 目前仅提供命令行版本，用户交互界面版本正在开发中。
 
 ### 命令行安装
 
 Python 用户可以直接使用 pip 安装本工具：
 
 ```shell
-pip install starrail-toolkit --upgrade
+pip install starrail-toolkit --upgrade -i https://pypi.tuna.tsinghua.edu.cn/simple
 ```
 
 ## 使用指南
 
 ### 获取抽卡查询 API URL
 
+请参考[【这个教程】](docs/how-to-get-api-url)获取查询链接。
+
 由此可以获得一个形如 `https://api-takumi.mihoyo.com/common/gacha_record/api/getGachaLog?xxxxx` 的 URL，后续步骤使用的就是这个 URL。注意：API URL 会在一定时间后过期，过期后需要重新获取。
 
 ### 导出抽卡记录
 
 #### 命令行导出
 
 可以使用如下命令导出：
 
 ```shell
-hksr https://api-takumi.mihoyo.com/xxx --export all
+hksr --api https://api-takumi.mihoyo.com/xxx --export all
 ```
 
-参数：`--export` 为导出格式，默认为导出全部格式，若仅需导出部分格式，可将对应参数替换。目前支持的格式有 `csv`、`json`、`xlsx`，替换方式例如 `--export json xlsx`。
+参数：`--export` 为导出格式，默认为导出全部格式，若仅需导出部分格式，可将对应参数替换。目前支持的格式有 `csv`、`json`、`md`、`xlsx`，替换方式例如 `--export json xlsx`。
```

### Comparing `starrail-toolkit-0.1.0/README.md` & `starrail-toolkit-0.2.0/starrail_toolkit.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,82 @@
+Metadata-Version: 2.1
+Name: starrail-toolkit
+Version: 0.2.0
+Summary: Honkai Star Rail Toolkit
+Home-page: https://github.com/LittleNyima/honkai-starrail-toolkit
+Author: LittleNyima
+Author-email: littlenyima@163.com
+License: GPLv3
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # 《崩坏：星穹铁道》工具箱
 
+<div style="min-height: 275px">
 <img src="https://s1.ax1x.com/2023/04/30/p98Cv26.png" alt="logo" align="left" vertical-align="center" />
 
 ```
 Starrail Toolkit
 
-- 主分支版本：0.1.0
-- 开发分支版本：0.1.0
+- 主分支版本：0.2.0
+- 开发分支版本：0.2.0
+- PyPI 版本：0.2.0
 ```
+</div>
 
 <br clear="left">
 
 ## 开发状态
 
 - [x] 支持命令行导出 csv、xlsx、json 格式抽卡记录
-- [ ] 支持命令行显示抽卡报告
+- [x] 支持命令行显示抽卡报告
+- [x] 支持导出 markdown 格式抽卡报告
 - [ ] 支持导出网页版抽卡报告
 - [ ] 支持 Windows 平台游戏中自动检测 API URL
 - [ ] 实现用户界面并编译到 Windows 与 macOS 平台
 - [ ] 支持自动检查更新
 
+## 导出结果示例
+
+- Excel 结果示例（为保护隐私已隐藏部分信息）
+
+  ![xlsx](https://s1.ax1x.com/2023/05/02/p9GJKts.md.png)
+
+- Markdown 结果示例：
+
+  ![markdown](https://s1.ax1x.com/2023/05/02/p9GJMhn.md.png)
+
 ## 安装方式
 
 目前仅提供命令行版本，用户交互界面版本正在开发中。
 
 ### 命令行安装
 
 Python 用户可以直接使用 pip 安装本工具：
 
 ```shell
-pip install starrail-toolkit --upgrade
+pip install starrail-toolkit --upgrade -i https://pypi.tuna.tsinghua.edu.cn/simple
 ```
 
 ## 使用指南
 
 ### 获取抽卡查询 API URL
 
+请参考[【这个教程】](docs/how-to-get-api-url)获取查询链接。
+
 由此可以获得一个形如 `https://api-takumi.mihoyo.com/common/gacha_record/api/getGachaLog?xxxxx` 的 URL，后续步骤使用的就是这个 URL。注意：API URL 会在一定时间后过期，过期后需要重新获取。
 
 ### 导出抽卡记录
 
 #### 命令行导出
 
 可以使用如下命令导出：
 
 ```shell
-hksr https://api-takumi.mihoyo.com/xxx --export all
+hksr --api https://api-takumi.mihoyo.com/xxx --export all
 ```
 
-参数：`--export` 为导出格式，默认为导出全部格式，若仅需导出部分格式，可将对应参数替换。目前支持的格式有 `csv`、`json`、`xlsx`，替换方式例如 `--export json xlsx`。
+参数：`--export` 为导出格式，默认为导出全部格式，若仅需导出部分格式，可将对应参数替换。目前支持的格式有 `csv`、`json`、`md`、`xlsx`，替换方式例如 `--export json xlsx`。
```

### Comparing `starrail-toolkit-0.1.0/setup.py` & `starrail-toolkit-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.1.0/starrail/config.py` & `starrail-toolkit-0.2.0/starrail/config.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.1.0/starrail/entry/cli.py` & `starrail-toolkit-0.2.0/starrail/entry/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 
 def parse_args():
     parser = argparse.ArgumentParser(
         prog='hksr',
         description='Honkai: Star Rail Toolkit',
     )
     parser.add_argument(
-        'api', type=str,
+        '--api', type=str,
         help='URL of the gacha api, please refer to README.md for details.',
     )
     parser.add_argument(
         '--export', nargs='+', type=str,
-        choices=['all', 'json', 'xlsx', 'csv'],  # TODO: html
+        choices=['all', 'json', 'xlsx', 'csv', 'md'],  # TODO: html
         help='Types of expected export formats.',
     )
 
     return parser.parse_args()
 
 
 def cli_entry():
```

### Comparing `starrail-toolkit-0.1.0/starrail/gacha/database.py` & `starrail-toolkit-0.2.0/starrail/gacha/database.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.1.0/starrail/gacha/fetch.py` & `starrail-toolkit-0.2.0/starrail/gacha/fetch.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.1.0/starrail/gacha/fileio.py` & `starrail-toolkit-0.2.0/starrail/gacha/fileio.py`

 * *Files 13% similar despite different names*

```diff
@@ -46,9 +46,35 @@
     data_list = []
     for gacha_type in GachaType:
         data_list.extend(manager.gacha[gacha_type.value].tolist())
     df = pd.json_normalize(data_list)
     df.to_csv(output_path, encoding='utf-8')
 
 
+def export_as_md(manager: GachaDataManager, output_path: str) -> None:
+    md = '# Gacha Report\n\n'
+    for gacha_type in GachaType:
+        md += f'## {gacha_type.name}\n\n'
+        md += '| Type | Count | Basic Prob. | True Prob. | Since Last |\n'
+        md += '| ---- | ----- | ----------- | ---------- | ---------- |\n'
+        stats = manager.gacha[gacha_type.value].stats
+        for item in stats:
+            rtype = item['rank_type']
+            count = item['count']
+            basic = item['basic_prob']
+            compr = item['compr_prob']
+            since_last = item['since_last']
+            md += f'|{rtype}|{count}|{basic}|{compr}|{since_last}|\n'
+        md += '\n'
+        if stats[0]['attempts']:
+            attempt_string = ' '.join(stats[0]['attempts'])
+            average = stats[0]['average']
+            md += 'History of 5-star gacha attempts: '
+            md += f'**{attempt_string}**'
+            md += '\n\n'
+            md += f'Average gacha per 5-star: **{average}**\n\n'
+    with open(output_path, 'w', encoding='utf-8') as fout:
+        fout.write(md)
+
+
 def export_as_html(manager: GachaDataManager, output_path: str) -> None:
     raise NotImplementedError
```

### Comparing `starrail-toolkit-0.1.0/starrail/gacha/service.py` & `starrail-toolkit-0.2.0/starrail/gacha/service.py`

 * *Files 12% similar despite different names*

```diff
@@ -55,14 +55,15 @@
         data_list = response['data']['list']
         r.extend(data_list)
         end_id = data_list[-1]['id']
     return r
 
 
 def export_gacha_from_api(api_url, export):
+    assert api_url, 'API URL should be provided, auto-detect is coming soon'
     response, code = fetch_json(api_url)
     valid = check_response(response, code)
     if not valid:
         logger.fatal('Error while checking response from api URL, exitting')
         raise ValueError('Invalid api URL, please check your input')
 
     api_template = get_url_template(api_url)
@@ -76,22 +77,25 @@
         records = export_gacha_type(api_template, gacha_type)
         manager.add_records(gacha_type.value, records)
         manager.gacha[gacha_type.value].sort()
         logger.info(f'Finish downloading records of {gacha_type.name}')
 
     fileio.export_as_sql(manager, manager.cache_path)
 
+    manager.log_stats()
+
     export_hooks = dict(
         csv=fileio.export_as_csv,
         html=fileio.export_as_html,
         json=fileio.export_as_json,
+        md=fileio.export_as_md,
         xlsx=fileio.export_as_xlsx,
     )
     if 'all' in export:
-        export = ['csv', 'json', 'xlsx']  # html
+        export = ['csv', 'json', 'md', 'xlsx']  # html
 
     timestamp = datetime.now().strftime('%Y%d%m%H%M%S')
 
     for format in export:
         logger.info(f'Exporting gacha data as {format} format')
         output_dir = os.getcwd()
         filename = f'HKSR-export-{uid}-{timestamp}.{format}'
```

### Comparing `starrail-toolkit-0.1.0/starrail/gacha/url.py` & `starrail-toolkit-0.2.0/starrail/gacha/url.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.1.0/starrail/utils/loggings.py` & `starrail-toolkit-0.2.0/starrail/utils/loggings.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from starrail import package_path
 
 
 def setup_logging():
     format = (
         '%(asctime)s %(name)s Line %(lineno)d - '
-        '[%(levelname)8s] %(message)s'
+        '[%(levelname)s] %(message)s'
     )
     formatter = logging.Formatter(format)
 
     stream = logging.StreamHandler()
     stream.setFormatter(formatter)
     logging.getLogger().addHandler(stream)
     logging.getLogger().setLevel(logging.DEBUG)
```

### Comparing `starrail-toolkit-0.1.0/starrail_toolkit.egg-info/PKG-INFO` & `starrail-toolkit-0.2.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,66 +1,67 @@
-Metadata-Version: 2.1
-Name: starrail-toolkit
-Version: 0.1.0
-Summary: Honkai Star Rail Toolkit
-Home-page: https://github.com/LittleNyima/honkai-starrail-toolkit
-Author: LittleNyima
-Author-email: littlenyima@163.com
-License: GPLv3
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # 《崩坏：星穹铁道》工具箱
 
+<div style="min-height: 275px">
 <img src="https://s1.ax1x.com/2023/04/30/p98Cv26.png" alt="logo" align="left" vertical-align="center" />
 
 ```
 Starrail Toolkit
 
-- 主分支版本：0.1.0
-- 开发分支版本：0.1.0
+- 主分支版本：0.2.0
+- 开发分支版本：0.2.0
+- PyPI 版本：0.2.0
 ```
+</div>
 
 <br clear="left">
 
 ## 开发状态
 
 - [x] 支持命令行导出 csv、xlsx、json 格式抽卡记录
-- [ ] 支持命令行显示抽卡报告
+- [x] 支持命令行显示抽卡报告
+- [x] 支持导出 markdown 格式抽卡报告
 - [ ] 支持导出网页版抽卡报告
 - [ ] 支持 Windows 平台游戏中自动检测 API URL
 - [ ] 实现用户界面并编译到 Windows 与 macOS 平台
 - [ ] 支持自动检查更新
 
+## 导出结果示例
+
+- Excel 结果示例（为保护隐私已隐藏部分信息）
+
+  ![xlsx](https://s1.ax1x.com/2023/05/02/p9GJKts.md.png)
+
+- Markdown 结果示例：
+
+  ![markdown](https://s1.ax1x.com/2023/05/02/p9GJMhn.md.png)
+
 ## 安装方式
 
 目前仅提供命令行版本，用户交互界面版本正在开发中。
 
 ### 命令行安装
 
 Python 用户可以直接使用 pip 安装本工具：
 
 ```shell
-pip install starrail-toolkit --upgrade
+pip install starrail-toolkit --upgrade -i https://pypi.tuna.tsinghua.edu.cn/simple
 ```
 
 ## 使用指南
 
 ### 获取抽卡查询 API URL
 
+请参考[【这个教程】](docs/how-to-get-api-url)获取查询链接。
+
 由此可以获得一个形如 `https://api-takumi.mihoyo.com/common/gacha_record/api/getGachaLog?xxxxx` 的 URL，后续步骤使用的就是这个 URL。注意：API URL 会在一定时间后过期，过期后需要重新获取。
 
 ### 导出抽卡记录
 
 #### 命令行导出
 
 可以使用如下命令导出：
 
 ```shell
-hksr https://api-takumi.mihoyo.com/xxx --export all
+hksr --api https://api-takumi.mihoyo.com/xxx --export all
 ```
 
-参数：`--export` 为导出格式，默认为导出全部格式，若仅需导出部分格式，可将对应参数替换。目前支持的格式有 `csv`、`json`、`xlsx`，替换方式例如 `--export json xlsx`。
+参数：`--export` 为导出格式，默认为导出全部格式，若仅需导出部分格式，可将对应参数替换。目前支持的格式有 `csv`、`json`、`md`、`xlsx`，替换方式例如 `--export json xlsx`。
```

### Comparing `starrail-toolkit-0.1.0/starrail_toolkit.egg-info/SOURCES.txt` & `starrail-toolkit-0.2.0/starrail_toolkit.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 starrail/gacha/database.py
 starrail/gacha/fetch.py
 starrail/gacha/fileio.py
 starrail/gacha/parse.py
 starrail/gacha/service.py
 starrail/gacha/type.py
 starrail/gacha/url.py
+starrail/gui/__init__.py
 starrail/utils/__init__.py
 starrail/utils/loggings.py
 starrail_toolkit.egg-info/PKG-INFO
 starrail_toolkit.egg-info/SOURCES.txt
 starrail_toolkit.egg-info/dependency_links.txt
 starrail_toolkit.egg-info/entry_points.txt
 starrail_toolkit.egg-info/requires.txt
```

