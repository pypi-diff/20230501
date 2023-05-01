# Comparing `tmp/MKN_third_codes-0.4.4.tar.gz` & `tmp/MKN_third_codes-0.4.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\MKN_third_codes-0.4.4.tar", last modified: Mon May  1 04:52:08 2023, max compression
+gzip compressed data, was "dist\MKN_third_codes-0.4.4.1.tar", last modified: Mon May  1 04:54:24 2023, max compression
```

## Comparing `MKN_third_codes-0.4.4.tar` & `MKN_third_codes-0.4.4.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 04:52:08.109234 MKN_third_codes-0.4.4/
--rw-rw-rw-   0        0        0     1073 2023-04-29 11:32:30.000000 MKN_third_codes-0.4.4/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-04-29 11:33:13.000000 MKN_third_codes-0.4.4/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-05-01 04:52:08.098265 MKN_third_codes-0.4.4/MKN_third_codes/
--rw-rw-rw-   0        0        0    26387 2023-05-01 04:37:08.000000 MKN_third_codes-0.4.4/MKN_third_codes/solutions.py
-drwxrwxrwx   0        0        0        0 2023-05-01 04:52:08.108238 MKN_third_codes-0.4.4/MKN_third_codes.egg-info/
--rw-rw-rw-   0        0        0     4282 2023-05-01 04:52:07.000000 MKN_third_codes-0.4.4/MKN_third_codes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-05-01 04:52:08.000000 MKN_third_codes-0.4.4/MKN_third_codes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 04:52:07.000000 MKN_third_codes-0.4.4/MKN_third_codes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-01 04:52:07.000000 MKN_third_codes-0.4.4/MKN_third_codes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4282 2023-05-01 04:52:08.109234 MKN_third_codes-0.4.4/PKG-INFO
--rw-rw-rw-   0        0        0     2950 2023-05-01 04:51:47.000000 MKN_third_codes-0.4.4/README.md
--rw-rw-rw-   0        0        0       42 2023-05-01 04:52:08.109234 MKN_third_codes-0.4.4/setup.cfg
--rw-rw-rw-   0        0        0      502 2023-05-01 04:50:47.000000 MKN_third_codes-0.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 04:54:24.982121 MKN_third_codes-0.4.4.1/
+-rw-rw-rw-   0        0        0     1073 2023-04-29 11:32:30.000000 MKN_third_codes-0.4.4.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-04-29 11:33:13.000000 MKN_third_codes-0.4.4.1/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-05-01 04:54:24.971150 MKN_third_codes-0.4.4.1/MKN_third_codes/
+-rw-rw-rw-   0        0        0    26387 2023-05-01 04:37:08.000000 MKN_third_codes-0.4.4.1/MKN_third_codes/solutions.py
+drwxrwxrwx   0        0        0        0 2023-05-01 04:54:24.980127 MKN_third_codes-0.4.4.1/MKN_third_codes.egg-info/
+-rw-rw-rw-   0        0        0     4285 2023-05-01 04:54:24.000000 MKN_third_codes-0.4.4.1/MKN_third_codes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-05-01 04:54:24.000000 MKN_third_codes-0.4.4.1/MKN_third_codes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 04:54:24.000000 MKN_third_codes-0.4.4.1/MKN_third_codes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-01 04:54:24.000000 MKN_third_codes-0.4.4.1/MKN_third_codes.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4285 2023-05-01 04:54:24.981124 MKN_third_codes-0.4.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2950 2023-05-01 04:53:21.000000 MKN_third_codes-0.4.4.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-01 04:54:24.982121 MKN_third_codes-0.4.4.1/setup.cfg
+-rw-rw-rw-   0        0        0      505 2023-05-01 04:54:23.000000 MKN_third_codes-0.4.4.1/setup.py
```

### Comparing `MKN_third_codes-0.4.4/LICENSE.txt` & `MKN_third_codes-0.4.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MKN_third_codes-0.4.4/MKN_third_codes/solutions.py` & `MKN_third_codes-0.4.4.1/MKN_third_codes/solutions.py`

 * *Files identical despite different names*

### Comparing `MKN_third_codes-0.4.4/MKN_third_codes.egg-info/PKG-INFO` & `MKN_third_codes-0.4.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: MKN-third-codes
-Version: 0.4.4
+Name: MKN_third_codes
+Version: 0.4.4.1
 Summary: Python library with standart solutions for probability tasks
 Author: Dolgun Ivan
 Author-email: vanadolgun@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 ### Здарова! Библиотека немного помогает с тервером по МКН 3
 
-## 📦 Версия: 0.4.3
+## 📦 Версия: 0.4.4
 
 - Функции buckets_n_balls => задачи про урны
 - Функции things_complexity => задачи про путаницу вещей
 - Функции geometric_meeting => задачи про встречи
 - Функции find_math_prediction => нахождение Математического ожидания
 - Функция combinations => число сочетаний
 
@@ -40,15 +40,15 @@
 ### Я в ВК: [Долгун Иван][vkCom]
 ### Я в Discord: ИVAN#2599
 
 [vkCom]: https://vk.com/ivandolgun
 [libaPage]: https://pypi.org/project/MKN-third-codes/
 [AlekseiBot]: https://t.me/mkn_solver_bot
 [LehaVK]: https://vk.com/miranchuk5959
-
+#
 ### Change Log
 ====================
 
 ## 0.4.4 (01/05/2023)
 ```
 ------------------
 ━ исправлено отображение Change Log
```

### Comparing `MKN_third_codes-0.4.4/PKG-INFO` & `MKN_third_codes-0.4.4.1/MKN_third_codes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: MKN_third_codes
-Version: 0.4.4
+Name: MKN-third-codes
+Version: 0.4.4.1
 Summary: Python library with standart solutions for probability tasks
 Author: Dolgun Ivan
 Author-email: vanadolgun@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 ### Здарова! Библиотека немного помогает с тервером по МКН 3
 
-## 📦 Версия: 0.4.3
+## 📦 Версия: 0.4.4
 
 - Функции buckets_n_balls => задачи про урны
 - Функции things_complexity => задачи про путаницу вещей
 - Функции geometric_meeting => задачи про встречи
 - Функции find_math_prediction => нахождение Математического ожидания
 - Функция combinations => число сочетаний
 
@@ -40,15 +40,15 @@
 ### Я в ВК: [Долгун Иван][vkCom]
 ### Я в Discord: ИVAN#2599
 
 [vkCom]: https://vk.com/ivandolgun
 [libaPage]: https://pypi.org/project/MKN-third-codes/
 [AlekseiBot]: https://t.me/mkn_solver_bot
 [LehaVK]: https://vk.com/miranchuk5959
-
+#
 ### Change Log
 ====================
 
 ## 0.4.4 (01/05/2023)
 ```
 ------------------
 ━ исправлено отображение Change Log
```

### Comparing `MKN_third_codes-0.4.4/README.md` & `MKN_third_codes-0.4.4.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ### Здарова! Библиотека немного помогает с тервером по МКН 3
 
-## 📦 Версия: 0.4.3
+## 📦 Версия: 0.4.4
 
 - Функции buckets_n_balls => задачи про урны
 - Функции things_complexity => задачи про путаницу вещей
 - Функции geometric_meeting => задачи про встречи
 - Функции find_math_prediction => нахождение Математического ожидания
 - Функция combinations => число сочетаний
```

