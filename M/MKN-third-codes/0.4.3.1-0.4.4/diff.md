# Comparing `tmp/MKN_third_codes-0.4.3.1.tar.gz` & `tmp/MKN_third_codes-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\MKN_third_codes-0.4.3.1.tar", last modified: Mon May  1 04:48:05 2023, max compression
+gzip compressed data, was "dist\MKN_third_codes-0.4.4.tar", last modified: Mon May  1 04:52:08 2023, max compression
```

## Comparing `MKN_third_codes-0.4.3.1.tar` & `MKN_third_codes-0.4.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 04:48:05.048268 MKN_third_codes-0.4.3.1/
--rw-rw-rw-   0        0        0     1073 2023-04-29 11:32:30.000000 MKN_third_codes-0.4.3.1/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-04-29 11:33:13.000000 MKN_third_codes-0.4.3.1/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-05-01 04:48:05.037270 MKN_third_codes-0.4.3.1/MKN_third_codes/
--rw-rw-rw-   0        0        0    26387 2023-05-01 04:37:08.000000 MKN_third_codes-0.4.3.1/MKN_third_codes/solutions.py
-drwxrwxrwx   0        0        0        0 2023-05-01 04:48:05.046248 MKN_third_codes-0.4.3.1/MKN_third_codes.egg-info/
--rw-rw-rw-   0        0        0     4037 2023-05-01 04:48:04.000000 MKN_third_codes-0.4.3.1/MKN_third_codes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-05-01 04:48:04.000000 MKN_third_codes-0.4.3.1/MKN_third_codes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 04:48:04.000000 MKN_third_codes-0.4.3.1/MKN_third_codes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-01 04:48:04.000000 MKN_third_codes-0.4.3.1/MKN_third_codes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4037 2023-05-01 04:48:05.047243 MKN_third_codes-0.4.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     2950 2023-05-01 04:41:54.000000 MKN_third_codes-0.4.3.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-01 04:48:05.048268 MKN_third_codes-0.4.3.1/setup.cfg
--rw-rw-rw-   0        0        0      504 2023-05-01 04:47:58.000000 MKN_third_codes-0.4.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 04:52:08.109234 MKN_third_codes-0.4.4/
+-rw-rw-rw-   0        0        0     1073 2023-04-29 11:32:30.000000 MKN_third_codes-0.4.4/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-04-29 11:33:13.000000 MKN_third_codes-0.4.4/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-05-01 04:52:08.098265 MKN_third_codes-0.4.4/MKN_third_codes/
+-rw-rw-rw-   0        0        0    26387 2023-05-01 04:37:08.000000 MKN_third_codes-0.4.4/MKN_third_codes/solutions.py
+drwxrwxrwx   0        0        0        0 2023-05-01 04:52:08.108238 MKN_third_codes-0.4.4/MKN_third_codes.egg-info/
+-rw-rw-rw-   0        0        0     4282 2023-05-01 04:52:07.000000 MKN_third_codes-0.4.4/MKN_third_codes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-05-01 04:52:08.000000 MKN_third_codes-0.4.4/MKN_third_codes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 04:52:07.000000 MKN_third_codes-0.4.4/MKN_third_codes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-01 04:52:07.000000 MKN_third_codes-0.4.4/MKN_third_codes.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4282 2023-05-01 04:52:08.109234 MKN_third_codes-0.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2950 2023-05-01 04:51:47.000000 MKN_third_codes-0.4.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-01 04:52:08.109234 MKN_third_codes-0.4.4/setup.cfg
+-rw-rw-rw-   0        0        0      502 2023-05-01 04:50:47.000000 MKN_third_codes-0.4.4/setup.py
```

### Comparing `MKN_third_codes-0.4.3.1/LICENSE.txt` & `MKN_third_codes-0.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MKN_third_codes-0.4.3.1/MKN_third_codes/solutions.py` & `MKN_third_codes-0.4.4/MKN_third_codes/solutions.py`

 * *Files identical despite different names*

### Comparing `MKN_third_codes-0.4.3.1/MKN_third_codes.egg-info/PKG-INFO` & `MKN_third_codes-0.4.4/MKN_third_codes.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MKN-third-codes
-Version: 0.4.3.1
+Version: 0.4.4
 Summary: Python library with standart solutions for probability tasks
 Author: Dolgun Ivan
 Author-email: vanadolgun@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -20,17 +20,17 @@
 
 # 🔩 Использование
 ## 📥 Импортирование
 ### from MKN_third_codes import solutions
 ## 🕹 Функции
 - 📱 любая функция, решающая задачу имеет суффикс '_terminal'. Это значит, что, используя данную функцию, дополнительно ничего писать не надо, т.к. она представляет из себя готовое решение типа задач. Всё взаимодействие происходит в терминале.
 - 📲 любая функция, решающая задачу имеет суффикс '_solution'. Такая функция принимает аргументы на вход, которые ей следует предоставить. В описании каждой функции есть описание возвращаемого объекта.
-- 📨 любая функция, решающая задачу имеет суффикс '_request'. Этот тип функций озволяет взаимодействовать с ней извне, например, отсылая в качестве входного параметра ввод пользователя.
+- 📨 любая функция, решающая задачу имеет суффикс '_request'. Этот тип функций позволяет взаимодействовать с ней извне, например, отсылая в качестве входного параметра ввод пользователя.
 ## 🧱 Классы
-- Классы данной библиотеки можно использовать вне функций, предавстовляемых данной библиотекой, но т.к. классы заточены под неё, то ими возможно будет неудобно пользоваться.
+- Классы данной библиотеки можно использовать вне функций, предоставляемых данной библиотекой, но т.к. классы заточены под неё, то ими возможно будет неудобно пользоваться.
 
 # ✅ Установка
 ### Консоль: pip install --upgrade MKN_third_codes
 ## Страница библиотеки: [MKN_lib][libaPage]
 
 # 🧀 Не хотите париться с библиотекой?
 ## Бот [Lengendary Solver Bot][AlekseiBot] предоставляет возможность использования всех возможностей библиотеки в удобном интерфейсе телеграма.
@@ -44,31 +44,46 @@
 [libaPage]: https://pypi.org/project/MKN-third-codes/
 [AlekseiBot]: https://t.me/mkn_solver_bot
 [LehaVK]: https://vk.com/miranchuk5959
 
 ### Change Log
 ====================
 
-## 0.4.3 (01/05/2023)
+## 0.4.4 (01/05/2023)
+```
+------------------
+━ исправлено отображение Change Log
+------------------
+```
 # ------------------
+## 0.4.3 (01/05/2023)
 ```
+------------------
 ┏ добавлены '_request' типы для всех функций
 ┣ исправлена ошибка в вычислениях для задач о встречах
 ┗ добавлены 'find_math_prediction' решения
+------------------
 ```
 # ------------------
 ### 0.3.3 (29/04/2023)
-# ------------------
+```
+------------------
 ━ починил README для PYPI
-### 0.3.2 (29/04/2023)
+------------------
+```
 # ------------------
+### 0.3.2 (29/04/2023)
+```
+------------------
 ━ README.md
+------------------
+```
 # ------------------
 ## 0.3.1 (29/04/2023)
-# ------------------
 ```
+------------------
 ┏ оптимизированы 'things_complexity' решения
 ┣ добавлены 'geometric_meeting' решения
 ┃   ┗ новый класс 'Meetiner'
 ┗ добавлен Change Log
+------------------
 ```
-# ------------------
```

### Comparing `MKN_third_codes-0.4.3.1/PKG-INFO` & `MKN_third_codes-0.4.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MKN_third_codes
-Version: 0.4.3.1
+Version: 0.4.4
 Summary: Python library with standart solutions for probability tasks
 Author: Dolgun Ivan
 Author-email: vanadolgun@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -20,17 +20,17 @@
 
 # 🔩 Использование
 ## 📥 Импортирование
 ### from MKN_third_codes import solutions
 ## 🕹 Функции
 - 📱 любая функция, решающая задачу имеет суффикс '_terminal'. Это значит, что, используя данную функцию, дополнительно ничего писать не надо, т.к. она представляет из себя готовое решение типа задач. Всё взаимодействие происходит в терминале.
 - 📲 любая функция, решающая задачу имеет суффикс '_solution'. Такая функция принимает аргументы на вход, которые ей следует предоставить. В описании каждой функции есть описание возвращаемого объекта.
-- 📨 любая функция, решающая задачу имеет суффикс '_request'. Этот тип функций озволяет взаимодействовать с ней извне, например, отсылая в качестве входного параметра ввод пользователя.
+- 📨 любая функция, решающая задачу имеет суффикс '_request'. Этот тип функций позволяет взаимодействовать с ней извне, например, отсылая в качестве входного параметра ввод пользователя.
 ## 🧱 Классы
-- Классы данной библиотеки можно использовать вне функций, предавстовляемых данной библиотекой, но т.к. классы заточены под неё, то ими возможно будет неудобно пользоваться.
+- Классы данной библиотеки можно использовать вне функций, предоставляемых данной библиотекой, но т.к. классы заточены под неё, то ими возможно будет неудобно пользоваться.
 
 # ✅ Установка
 ### Консоль: pip install --upgrade MKN_third_codes
 ## Страница библиотеки: [MKN_lib][libaPage]
 
 # 🧀 Не хотите париться с библиотекой?
 ## Бот [Lengendary Solver Bot][AlekseiBot] предоставляет возможность использования всех возможностей библиотеки в удобном интерфейсе телеграма.
@@ -44,31 +44,46 @@
 [libaPage]: https://pypi.org/project/MKN-third-codes/
 [AlekseiBot]: https://t.me/mkn_solver_bot
 [LehaVK]: https://vk.com/miranchuk5959
 
 ### Change Log
 ====================
 
-## 0.4.3 (01/05/2023)
+## 0.4.4 (01/05/2023)
+```
+------------------
+━ исправлено отображение Change Log
+------------------
+```
 # ------------------
+## 0.4.3 (01/05/2023)
 ```
+------------------
 ┏ добавлены '_request' типы для всех функций
 ┣ исправлена ошибка в вычислениях для задач о встречах
 ┗ добавлены 'find_math_prediction' решения
+------------------
 ```
 # ------------------
 ### 0.3.3 (29/04/2023)
-# ------------------
+```
+------------------
 ━ починил README для PYPI
-### 0.3.2 (29/04/2023)
+------------------
+```
 # ------------------
+### 0.3.2 (29/04/2023)
+```
+------------------
 ━ README.md
+------------------
+```
 # ------------------
 ## 0.3.1 (29/04/2023)
-# ------------------
 ```
+------------------
 ┏ оптимизированы 'things_complexity' решения
 ┣ добавлены 'geometric_meeting' решения
 ┃   ┗ новый класс 'Meetiner'
 ┗ добавлен Change Log
+------------------
 ```
-# ------------------
```

### Comparing `MKN_third_codes-0.4.3.1/README.md` & `MKN_third_codes-0.4.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 
 # 🔩 Использование
 ## 📥 Импортирование
 ### from MKN_third_codes import solutions
 ## 🕹 Функции
 - 📱 любая функция, решающая задачу имеет суффикс '_terminal'. Это значит, что, используя данную функцию, дополнительно ничего писать не надо, т.к. она представляет из себя готовое решение типа задач. Всё взаимодействие происходит в терминале.
 - 📲 любая функция, решающая задачу имеет суффикс '_solution'. Такая функция принимает аргументы на вход, которые ей следует предоставить. В описании каждой функции есть описание возвращаемого объекта.
-- 📨 любая функция, решающая задачу имеет суффикс '_request'. Этот тип функций озволяет взаимодействовать с ней извне, например, отсылая в качестве входного параметра ввод пользователя.
+- 📨 любая функция, решающая задачу имеет суффикс '_request'. Этот тип функций позволяет взаимодействовать с ней извне, например, отсылая в качестве входного параметра ввод пользователя.
 ## 🧱 Классы
-- Классы данной библиотеки можно использовать вне функций, предавстовляемых данной библиотекой, но т.к. классы заточены под неё, то ими возможно будет неудобно пользоваться.
+- Классы данной библиотеки можно использовать вне функций, предоставляемых данной библиотекой, но т.к. классы заточены под неё, то ими возможно будет неудобно пользоваться.
 
 # ✅ Установка
 ### Консоль: pip install --upgrade MKN_third_codes
 ## Страница библиотеки: [MKN_lib][libaPage]
 
 # 🧀 Не хотите париться с библиотекой?
 ## Бот [Lengendary Solver Bot][AlekseiBot] предоставляет возможность использования всех возможностей библиотеки в удобном интерфейсе телеграма.
```

