# Comparing `tmp/lecture-automator-0.2.0.tar.gz` & `tmp/lecture-automator-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lecture-automator-0.2.0.tar", max compression
+gzip compressed data, was "lecture-automator-0.2.1.tar", max compression
```

## Comparing `lecture-automator-0.2.0.tar` & `lecture-automator-0.2.1.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0     2209 2023-04-23 14:22:41.590194 lecture-automator-0.2.0/README.md
--rw-r--r--   0        0        0     1224 2023-04-23 14:22:41.590664 lecture-automator-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-09 16:38:42.823945 lecture-automator-0.2.0/src/lecture_automator/__init__.py
--rw-r--r--   0        0        0     1273 2023-04-23 14:22:41.590863 lecture-automator-0.2.0/src/lecture_automator/cli.py
--rw-r--r--   0        0        0     1393 2023-04-23 14:22:41.591129 lecture-automator-0.2.0/src/lecture_automator/command_handler.py
--rw-r--r--   0        0        0     1934 2023-04-11 16:44:42.058381 lecture-automator-0.2.0/src/lecture_automator/gen_speech.py
--rw-r--r--   0        0        0     1995 2023-04-13 20:31:53.497461 lecture-automator-0.2.0/src/lecture_automator/gen_video.py
--rw-r--r--   0        0        0     1089 2023-04-23 14:22:41.591679 lecture-automator-0.2.0/src/lecture_automator/marp_api.py
--rw-r--r--   0        0        0     4492 2023-04-23 14:22:41.591888 lecture-automator-0.2.0/src/lecture_automator/parser.py
--rw-r--r--   0        0        0      192 2023-04-11 15:39:34.023953 lecture-automator-0.2.0/src/lecture_automator/settings.py
--rw-r--r--   0        0        0     3209 2023-04-23 14:22:57.699255 lecture-automator-0.2.0/setup.py
--rw-r--r--   0        0        0     2846 2023-04-23 14:22:57.699481 lecture-automator-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2209 2023-05-01 10:48:41.606355 lecture-automator-0.2.1/README.md
+-rw-r--r--   0        0        0     1224 2023-05-01 10:48:09.375810 lecture-automator-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-09 16:38:42.823945 lecture-automator-0.2.1/src/lecture_automator/__init__.py
+-rw-r--r--   0        0        0     1284 2023-05-01 10:48:09.376089 lecture-automator-0.2.1/src/lecture_automator/cli.py
+-rw-r--r--   0        0        0     1393 2023-04-23 14:22:41.591129 lecture-automator-0.2.1/src/lecture_automator/command_handler.py
+-rw-r--r--   0        0        0        0 2023-05-01 10:48:09.376126 lecture-automator-0.2.1/src/lecture_automator/gen_speech/__init__.py
+-rw-r--r--   0        0        0     7098 2023-05-01 10:48:09.376513 lecture-automator-0.2.1/src/lecture_automator/gen_speech/gen_speech.py
+-rw-r--r--   0        0        0     1953 2023-05-01 10:48:09.376811 lecture-automator-0.2.1/src/lecture_automator/gen_speech/utils.py
+-rw-r--r--   0        0        0     1995 2023-04-13 20:31:53.497461 lecture-automator-0.2.1/src/lecture_automator/gen_video.py
+-rw-r--r--   0        0        0     1089 2023-04-23 14:22:41.591679 lecture-automator-0.2.1/src/lecture_automator/marp_api.py
+-rw-r--r--   0        0        0     4492 2023-04-23 14:22:41.591888 lecture-automator-0.2.1/src/lecture_automator/parser.py
+-rw-r--r--   0        0        0      192 2023-04-11 15:39:34.023953 lecture-automator-0.2.1/src/lecture_automator/settings.py
+-rw-r--r--   0        0        0     3241 2023-05-01 10:49:39.205483 lecture-automator-0.2.1/setup.py
+-rw-r--r--   0        0        0     2846 2023-05-01 10:49:39.205726 lecture-automator-0.2.1/PKG-INFO
```

### Comparing `lecture-automator-0.2.0/README.md` & `lecture-automator-0.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 С помощью pip (также необходимо установить ffmpeg и [Marp](https://github.com/marp-team/marp-cli)):
 ```
 pip install lecture-automator
 ```
 
 ## Использование
 
-Для использование необходимо создать Markdown-файл с описаниями слайдов (см. [Marp](https://marp.app/#get-started)) и [управляющими конструкциями](#управляющие-конструкции):
+Для использования необходимо создать Markdown-файл с описаниями слайдов (см. [Marp](https://marp.app/#get-started)) и [управляющими конструкциями](#управляющие-конструкции):
 ````md
 # Python
 
 ```
 print('Привет, мир')
 ```
 
@@ -31,21 +31,21 @@
 print(a * b)
 ```
 
 /speech{А здесь представлена другая программа, которая умножается число два на число четыре.}
 
 ````
 
-Затем для генерации необходимо использовать следующий CLI команду в терминале:
+Затем для генерации необходимо использовать следующую CLI команду в терминале:
 ```bash
 lecture-automator Example.md Example.mp4
 ```
 
 Пример сгенерированного видео:
 
 [Example.webm](https://user-images.githubusercontent.com/33065236/231875817-1d3aae09-2a63-4bb1-8380-8b7f024bbe45.webm)
 
 
 ### Управляющие конструкции 
 
-На данный момент реализованы следующий управляющие конструкции:
+На данный момент реализованы следующие управляющие конструкции:
 - `/speech{...}` - текст для озвучивания слайда (каждый слайд должен содержать данную конструкцию).
```

### Comparing `lecture-automator-0.2.0/pyproject.toml` & `lecture-automator-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lecture-automator"
-version = "0.2.0"
+version = "0.2.1"
 description = ""
 authors = ["CapBlood <stalker.anonim@mail.ru>"]
 readme = "README.md"
 homepage = "https://github.com/CapBlood/lecture-automator.git"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `lecture-automator-0.2.0/src/lecture_automator/cli.py` & `lecture-automator-0.2.1/src/lecture_automator/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import glob
 import tempfile
 
 import click
 
 from lecture_automator.parser import parse_md
 from lecture_automator.marp_api import generate_marp_slides
-from lecture_automator.gen_speech import texts_to_speeches
+from lecture_automator.gen_speech.gen_speech import texts_to_speeches
 from lecture_automator.gen_video import generate_video
 
 
 @click.command()
 @click.argument(
     'input_md', 
     type=click.STRING,
```

### Comparing `lecture-automator-0.2.0/src/lecture_automator/command_handler.py` & `lecture-automator-0.2.1/src/lecture_automator/command_handler.py`

 * *Files identical despite different names*

### Comparing `lecture-automator-0.2.0/src/lecture_automator/gen_video.py` & `lecture-automator-0.2.1/src/lecture_automator/gen_video.py`

 * *Files identical despite different names*

### Comparing `lecture-automator-0.2.0/src/lecture_automator/marp_api.py` & `lecture-automator-0.2.1/src/lecture_automator/marp_api.py`

 * *Files identical despite different names*

### Comparing `lecture-automator-0.2.0/src/lecture_automator/parser.py` & `lecture-automator-0.2.1/src/lecture_automator/parser.py`

 * *Files identical despite different names*

### Comparing `lecture-automator-0.2.0/setup.py` & `lecture-automator-0.2.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 package_dir = \
 {'': 'src'}
 
 packages = \
-['lecture_automator']
+['lecture_automator', 'lecture_automator.gen_speech']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['click>=8.1.3,<9.0.0',
  'ffmpeg-python>=0.2.0,<0.3.0',
@@ -18,17 +18,17 @@
 
 entry_points = \
 {'console_scripts': ['lecture-automator = '
                      'lecture_automator.cli:convert_md_to_mp4']}
 
 setup_kwargs = {
     'name': 'lecture-automator',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': '',
-    'long_description': "# Lecture Automator\n\nLecture Automator позволяет автоматически генерировать презентации с озвучкой для каждого из слайдов. Всё, что вам нужно сделать - написать текстовый файл Markdown со специальной разметкой, а остальное за вас сделает Lecture Automator.\n\n## Установка\n\nС помощью pip (также необходимо установить ffmpeg и [Marp](https://github.com/marp-team/marp-cli)):\n```\npip install lecture-automator\n```\n\n## Использование\n\nДля использование необходимо создать Markdown-файл с описаниями слайдов (см. [Marp](https://marp.app/#get-started)) и [управляющими конструкциями](#управляющие-конструкции):\n````md\n# Python\n\n```\nprint('Привет, мир')\n```\n\n/speech{На этом слайде представлена простейшая программа, написанная на языке програмирования Пайтон. Эта программа просто выводит указанные слова в терминал.}\n\n---\n\n# Python\n\n```\na = 2\nb = 4\nprint(a * b)\n```\n\n/speech{А здесь представлена другая программа, которая умножается число два на число четыре.}\n\n````\n\nЗатем для генерации необходимо использовать следующий CLI команду в терминале:\n```bash\nlecture-automator Example.md Example.mp4\n```\n\nПример сгенерированного видео:\n\n[Example.webm](https://user-images.githubusercontent.com/33065236/231875817-1d3aae09-2a63-4bb1-8380-8b7f024bbe45.webm)\n\n\n### Управляющие конструкции \n\nНа данный момент реализованы следующий управляющие конструкции:\n- `/speech{...}` - текст для озвучивания слайда (каждый слайд должен содержать данную конструкцию). \n",
+    'long_description': "# Lecture Automator\n\nLecture Automator позволяет автоматически генерировать презентации с озвучкой для каждого из слайдов. Всё, что вам нужно сделать - написать текстовый файл Markdown со специальной разметкой, а остальное за вас сделает Lecture Automator.\n\n## Установка\n\nС помощью pip (также необходимо установить ffmpeg и [Marp](https://github.com/marp-team/marp-cli)):\n```\npip install lecture-automator\n```\n\n## Использование\n\nДля использования необходимо создать Markdown-файл с описаниями слайдов (см. [Marp](https://marp.app/#get-started)) и [управляющими конструкциями](#управляющие-конструкции):\n````md\n# Python\n\n```\nprint('Привет, мир')\n```\n\n/speech{На этом слайде представлена простейшая программа, написанная на языке програмирования Пайтон. Эта программа просто выводит указанные слова в терминал.}\n\n---\n\n# Python\n\n```\na = 2\nb = 4\nprint(a * b)\n```\n\n/speech{А здесь представлена другая программа, которая умножается число два на число четыре.}\n\n````\n\nЗатем для генерации необходимо использовать следующую CLI команду в терминале:\n```bash\nlecture-automator Example.md Example.mp4\n```\n\nПример сгенерированного видео:\n\n[Example.webm](https://user-images.githubusercontent.com/33065236/231875817-1d3aae09-2a63-4bb1-8380-8b7f024bbe45.webm)\n\n\n### Управляющие конструкции \n\nНа данный момент реализованы следующие управляющие конструкции:\n- `/speech{...}` - текст для озвучивания слайда (каждый слайд должен содержать данную конструкцию). \n",
     'author': 'CapBlood',
     'author_email': 'stalker.anonim@mail.ru',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/CapBlood/lecture-automator.git',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `lecture-automator-0.2.0/PKG-INFO` & `lecture-automator-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lecture-automator
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Home-page: https://github.com/CapBlood/lecture-automator.git
 Author: CapBlood
 Author-email: stalker.anonim@mail.ru
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -26,15 +26,15 @@
 С помощью pip (также необходимо установить ffmpeg и [Marp](https://github.com/marp-team/marp-cli)):
 ```
 pip install lecture-automator
 ```
 
 ## Использование
 
-Для использование необходимо создать Markdown-файл с описаниями слайдов (см. [Marp](https://marp.app/#get-started)) и [управляющими конструкциями](#управляющие-конструкции):
+Для использования необходимо создать Markdown-файл с описаниями слайдов (см. [Marp](https://marp.app/#get-started)) и [управляющими конструкциями](#управляющие-конструкции):
 ````md
 # Python
 
 ```
 print('Привет, мир')
 ```
 
@@ -50,22 +50,22 @@
 print(a * b)
 ```
 
 /speech{А здесь представлена другая программа, которая умножается число два на число четыре.}
 
 ````
 
-Затем для генерации необходимо использовать следующий CLI команду в терминале:
+Затем для генерации необходимо использовать следующую CLI команду в терминале:
 ```bash
 lecture-automator Example.md Example.mp4
 ```
 
 Пример сгенерированного видео:
 
 [Example.webm](https://user-images.githubusercontent.com/33065236/231875817-1d3aae09-2a63-4bb1-8380-8b7f024bbe45.webm)
 
 
 ### Управляющие конструкции 
 
-На данный момент реализованы следующий управляющие конструкции:
+На данный момент реализованы следующие управляющие конструкции:
 - `/speech{...}` - текст для озвучивания слайда (каждый слайд должен содержать данную конструкцию).
```

