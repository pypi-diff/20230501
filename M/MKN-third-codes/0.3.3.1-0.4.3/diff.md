# Comparing `tmp/MKN_third_codes-0.3.3.1.tar.gz` & `tmp/MKN_third_codes-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\MKN_third_codes-0.3.3.1.tar", last modified: Sat Apr 29 16:21:29 2023, max compression
+gzip compressed data, was "dist\MKN_third_codes-0.4.3.tar", last modified: Mon May  1 04:42:33 2023, max compression
```

## Comparing `MKN_third_codes-0.3.3.1.tar` & `MKN_third_codes-0.4.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 16:21:29.742643 MKN_third_codes-0.3.3.1/
--rw-rw-rw-   0        0        0     1073 2023-04-29 11:32:30.000000 MKN_third_codes-0.3.3.1/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-04-29 11:33:13.000000 MKN_third_codes-0.3.3.1/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-04-29 16:21:29.733668 MKN_third_codes-0.3.3.1/MKN_third_codes/
--rw-rw-rw-   0        0        0    18143 2023-04-29 15:06:54.000000 MKN_third_codes-0.3.3.1/MKN_third_codes/solutions.py
-drwxrwxrwx   0        0        0        0 2023-04-29 16:21:29.741646 MKN_third_codes-0.3.3.1/MKN_third_codes.egg-info/
--rw-rw-rw-   0        0        0     2174 2023-04-29 16:21:29.000000 MKN_third_codes-0.3.3.1/MKN_third_codes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-04-29 16:21:29.000000 MKN_third_codes-0.3.3.1/MKN_third_codes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 16:21:29.000000 MKN_third_codes-0.3.3.1/MKN_third_codes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-29 16:21:29.000000 MKN_third_codes-0.3.3.1/MKN_third_codes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2174 2023-04-29 16:21:29.742643 MKN_third_codes-0.3.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     1896 2023-04-29 16:21:01.000000 MKN_third_codes-0.3.3.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-29 16:21:29.742643 MKN_third_codes-0.3.3.1/setup.cfg
--rw-rw-rw-   0        0        0      440 2023-04-29 16:21:27.000000 MKN_third_codes-0.3.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 04:42:33.051550 MKN_third_codes-0.4.3/
+-rw-rw-rw-   0        0        0     1073 2023-04-29 11:32:30.000000 MKN_third_codes-0.4.3/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-04-29 11:33:13.000000 MKN_third_codes-0.4.3/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-05-01 04:42:33.037588 MKN_third_codes-0.4.3/MKN_third_codes/
+-rw-rw-rw-   0        0        0    26387 2023-05-01 04:37:08.000000 MKN_third_codes-0.4.3/MKN_third_codes/solutions.py
+drwxrwxrwx   0        0        0        0 2023-05-01 04:42:33.050553 MKN_third_codes-0.4.3/MKN_third_codes.egg-info/
+-rw-rw-rw-   0        0        0     4015 2023-05-01 04:42:32.000000 MKN_third_codes-0.4.3/MKN_third_codes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-05-01 04:42:32.000000 MKN_third_codes-0.4.3/MKN_third_codes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 04:42:32.000000 MKN_third_codes-0.4.3/MKN_third_codes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-01 04:42:32.000000 MKN_third_codes-0.4.3/MKN_third_codes.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4015 2023-05-01 04:42:33.051550 MKN_third_codes-0.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2950 2023-05-01 04:41:54.000000 MKN_third_codes-0.4.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-01 04:42:33.052547 MKN_third_codes-0.4.3/setup.cfg
+-rw-rw-rw-   0        0        0      502 2023-05-01 04:20:23.000000 MKN_third_codes-0.4.3/setup.py
```

### Comparing `MKN_third_codes-0.3.3.1/LICENSE.txt` & `MKN_third_codes-0.4.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MKN_third_codes-0.3.3.1/MKN_third_codes/solutions.py` & `MKN_third_codes-0.4.3/MKN_third_codes/solutions.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import math
+import re
 
 class Box():
     """
     Класс урны (коробки) для задачи об урнах
 
     Args:
         white (int): кол-во белых шаров (не является параметром)
@@ -200,15 +201,16 @@
             self.waiting_time = waiting_time
         else:
             self.waiting_time = 1
 
     def calculate_square(self, maxEnd:float, waiter_time):
         return ((min(self.end_time, maxEnd) - self.start_time - waiter_time)**2)/2
 
-
+regular_int = r'-?\d+'
+regular_float = r'-?\d+(?:\.\d+)?'
 
 def combinations(k:float=0,n:float=0):
     """
     Функция, считающая число сочетаний из n по k
 
     Args:
         k (float): аргумент k - количество повторений
@@ -272,14 +274,56 @@
         txt += hypo.summary_text + " + "
     
     print(f"Обозначим событие B - достать шар из {len(boxes)+1} урны")
     txt = txt[:-3]
     txt += f"\nP(B) = {result[1]}"
     print(txt)
 
+def buckets_n_balls_request(text: str = None):
+    """
+    Решение задачи о n урнах с белыми и чёрными шарами, когда из каждой урны берут Ki шаров, перекладывают их в n+1 урну.
+    Функция предоставляет ответы на запросы для этой задачи
+
+    Args:
+        text (str): текст запроса, который может быть None или вводом пользователя
+    
+    Returns:
+        list: массив строчек ответа
+    """
+    if text == None:
+        return ["""Введите количество урн (число n)
+В следующих n строках введите количество белых и чёрных шаров (пара чисел через пробел) в i-ой урне
+В последних n строках введите количество шаров, забираемых из i-ой урны"""]
+    else:
+        try:
+            request = [int(parameter) for parameter in re.findall(regular_int, text)]
+
+            answer = []
+
+            box_num = request[0]
+
+            boxes = [Box(request[1+2*i], request[2+2*i], request[1+box_num*2+i]) for i in range(box_num)]
+
+            result = buckets_n_balls_solution(boxes)
+
+            answer.append("Обозначим событие A - достать Белый шар")
+
+            txt = "P(B) = "
+            for hypo in result[0]:
+                answer.append(hypo.hypo_text)
+                txt += hypo.summary_text + " + "
+            
+            answer.append(f"Обозначим событие B - достать шар из {len(boxes)+1} урны")
+            txt = txt[:-3]
+            txt += f"\nP(B) = {result[1]}"
+            answer.append(txt)
+            return answer
+        except:
+            return ["""Возникла ошибка при обработке введённых данных. Проверьте правильность ввода."""]
+
 def things_complexity_terminal():
     """
     Общее решение задачи о 'невнимательной секретарше' (сколько людей получат свои вещи)
     WARNING: Очень неоптимизированное! Не рекоммендую пытаться решить для количества людей > 11
     """
     humans = int(input("Введите количество человек: "))
     result = things_complexity_solution(humans)
@@ -323,14 +367,47 @@
 
     #пересчёт вероятностей
     for j in range(0, humans+1):
         myTable.cells[j].reset_probability()
     
     return myTable
 
+def things_complexity_request(text: str = None):
+    """
+    Решение задачи о 'невнимательной секретарше' (сколько людей получат свои вещи)
+    WARNING: Очень неоптимизированное! Не рекоммендую пытаться решить для количества людей > 11
+
+    Args:
+        text (str): текст запроса, который может быть None или вводом пользователя
+    
+    Returns:
+        list: массив строчек ответа
+    """
+    if text == None:
+        return ["""Введите количество человек (число n)"""]
+    else:
+        try:
+            request = [int(parameter) for parameter in re.findall(regular_int, text)]
+            if len(request) == 1:
+                answer = []
+
+                humans_num = request[0]
+
+                result = things_complexity_solution(humans_num)
+
+                answer.append("Таблица:")
+
+                for cell in result.cells:
+                    answer.append(f"E = {cell.etta_value}; P = {cell.probability} ({cell.good_th}/{cell.bad_th})")
+                return answer
+            else:
+                return ["""Возникла ошибка при обработке введённых данных. Проверьте правильность ввода."""]
+        except:
+            return ["""Возникла ошибка при обработке введённых данных. Проверьте правильность ввода."""]
+
 def geometric_meeting_terminal():
     """
     Общее решение задачи о встрече двух участников
     """
     ln = float(input("Введите отрезок меры: "))
     fM = Meetiner(float(input("Введите начальный момент, когда может появиться участник первый (-1 для расширения на полный отрезок): ")), 
     float(input("Введите конечный момент, когда может появиться участник первый (-1 для расширения на полный отрезок): ")), 
@@ -351,15 +428,112 @@
         length (float): длина участка меры, на которой могут встретиться участники
         firstAim (Meetiner): первый участник
         secondAim (Meetiner): второй участник
 
     Returns:
         float: вероятность встречи первого и второго участника
     """
-    square = ( length - max([firstAim.start_time, secondAim.start_time, 0]) - ( length - min([firstAim.end_time, secondAim.end_time, length]) ) )**2
+    square = ( length)**2
     square -= firstAim.calculate_square(length, secondAim.waiting_time)
     square -= secondAim.calculate_square(length, firstAim.waiting_time)
 
     return square/(length**2)
 
+def geometric_meeting_request(text: str = None):
+    """
+    Решение задачи о встрече двух участников
+
+    Args:
+        text (str): текст запроса, который может быть None или вводом пользователя
+    
+    Returns:
+        list: массив строчек ответа
+    """
+    if text == None:
+        return ["""Введите отрезок меры
+Введите НАЧАЛЬНЫЙ и КОНЕЧНЫЙ моменты, когда может появиться участник ПЕРВЫЙ (-1 для расширения на полный отрезок)
+Введите, сколько времени будет ждать участник ПЕРВЫЙ
+Введите НАЧАЛЬНЫЙ и КОНЕЧНЫЙ моменты, когда может появиться участник ВТОРОЙ (-1 для расширения на полный отрезок)
+Введите, сколько времени будет ждать участник ВТОРОЙ"""]
+    else:
+        try:
+            request = [float(parameter) for parameter in re.findall(regular_float, text)]
+            if len(request) == 7:
+                answer = []
+
+                ln = request[0]
+                fM = Meetiner(request[1], request[2], request[3])
+                sM = Meetiner(request[4], request[5], request[6])
+
+                result = geometric_meeting_solution(ln, fM, sM)
+
+                answer.append("Обозначим за A - участники встретятся")
+                answer.append(f"P(A) = {result}")
+
+                return answer
+            else:
+                return ["""Возникла ошибка при обработке введённых данных. Проверьте правильность ввода."""]
+        except:
+            return ["""Возникла ошибка при обработке введённых данных. Проверьте правильность ввода."""]
+
+def find_math_prediction_solution(table: EttaTable = None):
+    """
+    Нахождение МО по таблице значений случайных величин
+
+    Args:
+        table (EttaTable): таблица значений случайных величин
+    
+    Returns:
+        float: Математическое ожидание
+    """
+    if table == None:
+        return "Wrong Table"
+    else:
+        matP = 0
+        for cell in table.cells:
+            matP += cell.etta_value*cell.probability
+        return matP
+
+def find_math_prediction_terminal():
+    """
+    Нахождение МО по таблице значений случайных величин
+    """
+    n = int(input("Введите количество значений в таблице: "))
+    table = EttaTable()
+    for i in range(0, n):
+        v, p = map(int, input(f"введите пару чисел (значение, вероятность) для {i+1}-го значения").split())
+        table.cells.append(EttaTableCell(etta_value=v, probability=p))
+    print(f"Me = {find_math_prediction_solution(table)}")
+
+def find_math_prediction_request(text: str = None):
+    """
+    Нахождение МО по таблице значений случайных величин
+
+    Args:
+        text (str): текст запроса, который может быть None или вводом пользователя
+    
+    Returns:
+        list: массив строчек ответа
+    """
+    if text == None:
+        return ["""Введите количество значений таблицы (число n)
+В следующих n строчках введите пары чисел: значение СВ, вероятность (любой разделитель, кроме точки)"""]
+    else:
+        try:
+            request = [float(parameter) for parameter in re.findall(regular_float, text)]
+
+            n = int(request[0])
+            table = EttaTable()
+
+            for i in range(0, n):
+                table.cells.append(EttaTableCell(etta_value=request[1+i*2], probability=request[2+i*2]))
+
+            answer = []
+
+            answer.append(f"Me = {find_math_prediction_solution(table)}")
+
+            return answer
+        except:
+            return ["""Возникла ошибка при обработке введённых данных. Проверьте правильность ввода."""]
+
 __all__ = ['combinations', 'buckets_n_balls_solution', 'buckets_n_balls_terminal', 'things_complexity_solution', 'things_complexity_terminal',
 'geometric_meeting_solution', 'geometric_meeting_terminal']
```

### Comparing `MKN_third_codes-0.3.3.1/MKN_third_codes.egg-info/PKG-INFO` & `MKN_third_codes-0.4.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-Metadata-Version: 2.1
-Name: MKN-third-codes
-Version: 0.3.3.1
-Summary: Python library with standart solutions for probability tasks
-Author: Dolgun Ivan
-Author-email: vanadolgun@gmail.com
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 ### Здарова! Библиотека немного помогает с тервером по МКН 3
 
-## Версия: 0.3.3
+## 📦 Версия: 0.4.3
 
 - Функции buckets_n_balls => задачи про урны
 - Функции things_complexity => задачи про путаницу вещей
 - Функции geometric_meeting => задачи про встречи
+- Функции find_math_prediction => нахождение Математического ожидания
 - Функция combinations => число сочетаний
 
-# Использование
+# 🔩 Использование
+## 📥 Импортирование
+### from MKN_third_codes import solutions
 ## 🕹 Функции
-- 📱 любая функция имеет суффикс '_terminal'. Это значит, что, используя данную функцию, дополнительно ничего писать не надо, т.к. она представляет из себя готовое решение типа задач. Всё взаимодействие происходит в терминале.
-- 📲 любая функция имеет суффикс '_solution'. Такая функция принимает аргументы на вход, которые ей следует предоставить. В описании каждой функции есть описание возвращаемого объекта.
+- 📱 любая функция, решающая задачу имеет суффикс '_terminal'. Это значит, что, используя данную функцию, дополнительно ничего писать не надо, т.к. она представляет из себя готовое решение типа задач. Всё взаимодействие происходит в терминале.
+- 📲 любая функция, решающая задачу имеет суффикс '_solution'. Такая функция принимает аргументы на вход, которые ей следует предоставить. В описании каждой функции есть описание возвращаемого объекта.
+- 📨 любая функция, решающая задачу имеет суффикс '_request'. Этот тип функций озволяет взаимодействовать с ней извне, например, отсылая в качестве входного параметра ввод пользователя.
 ## 🧱 Классы
 - Классы данной библиотеки можно использовать вне функций, предавстовляемых данной библиотекой, но т.к. классы заточены под неё, то ими возможно будет неудобно пользоваться.
 
-# Установка
+# ✅ Установка
 ### Консоль: pip install --upgrade MKN_third_codes
-### Страница библиотеки: [MKN_lib][libaPage]
+## Страница библиотеки: [MKN_lib][libaPage]
+
+# 🧀 Не хотите париться с библиотекой?
+## Бот [Lengendary Solver Bot][AlekseiBot] предоставляет возможность использования всех возможностей библиотеки в удобном интерфейсе телеграма.
+### Автор: [Алексей Шумков][LehaVK]
 
-## Контакты
+## ☎️ Контакты
 ### Я в ВК: [Долгун Иван][vkCom]
 ### Я в Discord: ИVAN#2599
 
 [vkCom]: https://vk.com/ivandolgun
 [libaPage]: https://pypi.org/project/MKN-third-codes/
+[AlekseiBot]: https://t.me/mkn_solver_bot
+[LehaVK]: https://vk.com/miranchuk5959
```

### Comparing `MKN_third_codes-0.3.3.1/PKG-INFO` & `MKN_third_codes-0.4.3/MKN_third_codes.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,70 @@
 Metadata-Version: 2.1
-Name: MKN_third_codes
-Version: 0.3.3.1
+Name: MKN-third-codes
+Version: 0.4.3
 Summary: Python library with standart solutions for probability tasks
 Author: Dolgun Ivan
 Author-email: vanadolgun@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 ### Здарова! Библиотека немного помогает с тервером по МКН 3
 
-## Версия: 0.3.3
+## 📦 Версия: 0.4.3
 
 - Функции buckets_n_balls => задачи про урны
 - Функции things_complexity => задачи про путаницу вещей
 - Функции geometric_meeting => задачи про встречи
+- Функции find_math_prediction => нахождение Математического ожидания
 - Функция combinations => число сочетаний
 
-# Использование
+# 🔩 Использование
+## 📥 Импортирование
+### from MKN_third_codes import solutions
 ## 🕹 Функции
-- 📱 любая функция имеет суффикс '_terminal'. Это значит, что, используя данную функцию, дополнительно ничего писать не надо, т.к. она представляет из себя готовое решение типа задач. Всё взаимодействие происходит в терминале.
-- 📲 любая функция имеет суффикс '_solution'. Такая функция принимает аргументы на вход, которые ей следует предоставить. В описании каждой функции есть описание возвращаемого объекта.
+- 📱 любая функция, решающая задачу имеет суффикс '_terminal'. Это значит, что, используя данную функцию, дополнительно ничего писать не надо, т.к. она представляет из себя готовое решение типа задач. Всё взаимодействие происходит в терминале.
+- 📲 любая функция, решающая задачу имеет суффикс '_solution'. Такая функция принимает аргументы на вход, которые ей следует предоставить. В описании каждой функции есть описание возвращаемого объекта.
+- 📨 любая функция, решающая задачу имеет суффикс '_request'. Этот тип функций озволяет взаимодействовать с ней извне, например, отсылая в качестве входного параметра ввод пользователя.
 ## 🧱 Классы
 - Классы данной библиотеки можно использовать вне функций, предавстовляемых данной библиотекой, но т.к. классы заточены под неё, то ими возможно будет неудобно пользоваться.
 
-# Установка
+# ✅ Установка
 ### Консоль: pip install --upgrade MKN_third_codes
-### Страница библиотеки: [MKN_lib][libaPage]
+## Страница библиотеки: [MKN_lib][libaPage]
 
-## Контакты
+# 🧀 Не хотите париться с библиотекой?
+## Бот [Lengendary Solver Bot][AlekseiBot] предоставляет возможность использования всех возможностей библиотеки в удобном интерфейсе телеграма.
+### Автор: [Алексей Шумков][LehaVK]
+
+## ☎️ Контакты
 ### Я в ВК: [Долгун Иван][vkCom]
 ### Я в Discord: ИVAN#2599
 
 [vkCom]: https://vk.com/ivandolgun
 [libaPage]: https://pypi.org/project/MKN-third-codes/
+[AlekseiBot]: https://t.me/mkn_solver_bot
+[LehaVK]: https://vk.com/miranchuk5959
+
+### Change Log
+====================
+
+## 0.4.3 (01/05/2023)
+# ------------------
+┏ добавлены '_request' типы для всех функций
+┣ исправлена ошибка в вычислениях для задач о встречах
+┗ добавлены 'find_math_prediction' решения
+# ------------------
+### 0.3.3 (29/04/2023)
+# ------------------
+━ починил README для PYPI
+### 0.3.2 (29/04/2023)
+# ------------------
+━ README.md
+# ------------------
+## 0.3.1 (29/04/2023)
+# ------------------
+┏ оптимизированы 'things_complexity' решения
+┣ добавлены 'geometric_meeting' решения
+┃   ┗ новый класс 'Meetiner'
+┗ добавлен Change Log
+# ------------------
```

