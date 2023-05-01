# Comparing `tmp/MKN_third_codes-0.4.4.1.tar.gz` & `tmp/MKN_third_codes-0.6.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\MKN_third_codes-0.4.4.1.tar", last modified: Mon May  1 04:54:24 2023, max compression
+gzip compressed data, was "dist\MKN_third_codes-0.6.0.3.tar", last modified: Mon May  1 14:05:29 2023, max compression
```

## Comparing `MKN_third_codes-0.4.4.1.tar` & `MKN_third_codes-0.6.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 04:54:24.982121 MKN_third_codes-0.4.4.1/
--rw-rw-rw-   0        0        0     1073 2023-04-29 11:32:30.000000 MKN_third_codes-0.4.4.1/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-04-29 11:33:13.000000 MKN_third_codes-0.4.4.1/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-05-01 04:54:24.971150 MKN_third_codes-0.4.4.1/MKN_third_codes/
--rw-rw-rw-   0        0        0    26387 2023-05-01 04:37:08.000000 MKN_third_codes-0.4.4.1/MKN_third_codes/solutions.py
-drwxrwxrwx   0        0        0        0 2023-05-01 04:54:24.980127 MKN_third_codes-0.4.4.1/MKN_third_codes.egg-info/
--rw-rw-rw-   0        0        0     4285 2023-05-01 04:54:24.000000 MKN_third_codes-0.4.4.1/MKN_third_codes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-05-01 04:54:24.000000 MKN_third_codes-0.4.4.1/MKN_third_codes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 04:54:24.000000 MKN_third_codes-0.4.4.1/MKN_third_codes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-01 04:54:24.000000 MKN_third_codes-0.4.4.1/MKN_third_codes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4285 2023-05-01 04:54:24.981124 MKN_third_codes-0.4.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     2950 2023-05-01 04:53:21.000000 MKN_third_codes-0.4.4.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-01 04:54:24.982121 MKN_third_codes-0.4.4.1/setup.cfg
--rw-rw-rw-   0        0        0      505 2023-05-01 04:54:23.000000 MKN_third_codes-0.4.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 14:05:29.016172 MKN_third_codes-0.6.0.3/
+-rw-rw-rw-   0        0        0     1073 2023-04-29 11:32:30.000000 MKN_third_codes-0.6.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-04-29 11:33:13.000000 MKN_third_codes-0.6.0.3/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-05-01 14:05:29.008195 MKN_third_codes-0.6.0.3/MKN_third_codes/
+-rw-rw-rw-   0        0        0    31448 2023-05-01 13:56:42.000000 MKN_third_codes-0.6.0.3/MKN_third_codes/solutions.py
+drwxrwxrwx   0        0        0        0 2023-05-01 14:05:29.016172 MKN_third_codes-0.6.0.3/MKN_third_codes.egg-info/
+-rw-rw-rw-   0        0        0     5190 2023-05-01 14:05:28.000000 MKN_third_codes-0.6.0.3/MKN_third_codes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-05-01 14:05:28.000000 MKN_third_codes-0.6.0.3/MKN_third_codes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 14:05:28.000000 MKN_third_codes-0.6.0.3/MKN_third_codes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-01 14:05:28.000000 MKN_third_codes-0.6.0.3/MKN_third_codes.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5190 2023-05-01 14:05:29.016172 MKN_third_codes-0.6.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3541 2023-05-01 14:04:28.000000 MKN_third_codes-0.6.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-01 14:05:29.017170 MKN_third_codes-0.6.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      505 2023-05-01 14:05:24.000000 MKN_third_codes-0.6.0.3/setup.py
```

### Comparing `MKN_third_codes-0.4.4.1/LICENSE.txt` & `MKN_third_codes-0.6.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MKN_third_codes-0.4.4.1/MKN_third_codes/solutions.py` & `MKN_third_codes-0.6.0.3/MKN_third_codes/solutions.py`

 * *Files 8% similar despite different names*

```diff
@@ -143,30 +143,30 @@
 class EttaTableCell():
     """
     Ячейка таблицы Етта, со значением и вероятностью
 
     Args:
         etta_value (int): значение СВ "Етта"
         good_th (int): количество удачных исходов
-        bad_th (int): количество неудачных исходов
+        all_th (int): количество всех исходов
         probability (float): вероятность
 
     Methods:
         reset_probability
     """
-    def __init__(self, etta_value:int=0, good_th:int=1, bad_th:int=1, probability:float=None):
+    def __init__(self, etta_value:int=0, good_th:int=1, all_th:int=1, probability:float=None):
         self.etta_value = etta_value
         self.good_th = good_th
-        self.bad_th = bad_th
+        self.all_th = all_th
         self.probability = probability
         if self.probability == None:
             self.reset_probability()
 
     def reset_probability(self):
-        self.probability = self.good_th/(self.good_th+self.bad_th)
+        self.probability = self.good_th/self.all_th
 
 class EttaTable():
     """
     Таблица значений Етта
 
     Args:
         cells (): массив ячеек
@@ -325,15 +325,15 @@
     Общее решение задачи о 'невнимательной секретарше' (сколько людей получат свои вещи)
     WARNING: Очень неоптимизированное! Не рекоммендую пытаться решить для количества людей > 11
     """
     humans = int(input("Введите количество человек: "))
     result = things_complexity_solution(humans)
     print("Таблица:")
     for cell in result.cells:
-        print(f"E = {cell.etta_value}; P = {cell.probability} ({cell.good_th}/{cell.bad_th})")
+        print(f"E = {cell.etta_value}; P = {cell.probability} ({cell.good_th}/{cell.all_th})")
 
 def things_complexity_solution(humans:int = 0):
     """
     Решение задачи о 'невнимательной секретарше' (сколько людей получат свои вещи)
     WARNING: Очень неоптимизированное! Не рекоммендую пытаться решить для количества людей > 11
 
     Args:
@@ -393,15 +393,15 @@
                 humans_num = request[0]
 
                 result = things_complexity_solution(humans_num)
 
                 answer.append("Таблица:")
 
                 for cell in result.cells:
-                    answer.append(f"E = {cell.etta_value}; P = {cell.probability} ({cell.good_th}/{cell.bad_th})")
+                    answer.append(f"E = {cell.etta_value}; P = {cell.probability} ({cell.good_th}/{cell.all_th})")
                 return answer
             else:
                 return ["""Возникла ошибка при обработке введённых данных. Проверьте правильность ввода."""]
         except:
             return ["""Возникла ошибка при обработке введённых данных. Проверьте правильность ввода."""]
 
 def geometric_meeting_terminal():
@@ -471,42 +471,42 @@
 
                 return answer
             else:
                 return ["""Возникла ошибка при обработке введённых данных. Проверьте правильность ввода."""]
         except:
             return ["""Возникла ошибка при обработке введённых данных. Проверьте правильность ввода."""]
 
-def find_math_prediction_solution(table: EttaTable = None):
+def find_math_prediction_solution(table: EttaTable = None, degree: float = 1):
     """
     Нахождение МО по таблице значений случайных величин
 
     Args:
         table (EttaTable): таблица значений случайных величин
     
     Returns:
         float: Математическое ожидание
     """
     if table == None:
         return "Wrong Table"
     else:
         matP = 0
         for cell in table.cells:
-            matP += cell.etta_value*cell.probability
+            matP += (cell.etta_value**degree)*cell.probability
         return matP
 
 def find_math_prediction_terminal():
     """
     Нахождение МО по таблице значений случайных величин
     """
     n = int(input("Введите количество значений в таблице: "))
     table = EttaTable()
     for i in range(0, n):
         v, p = map(int, input(f"введите пару чисел (значение, вероятность) для {i+1}-го значения").split())
         table.cells.append(EttaTableCell(etta_value=v, probability=p))
-    print(f"Me = {find_math_prediction_solution(table)}")
+    print(f"Mx = ⁱ⁼¹∑ⁿ(xi * pi) = {find_math_prediction_solution(table)}")
 
 def find_math_prediction_request(text: str = None):
     """
     Нахождение МО по таблице значений случайных величин
 
     Args:
         text (str): текст запроса, который может быть None или вводом пользователя
@@ -525,15 +525,130 @@
             table = EttaTable()
 
             for i in range(0, n):
                 table.cells.append(EttaTableCell(etta_value=request[1+i*2], probability=request[2+i*2]))
 
             answer = []
 
-            answer.append(f"Me = {find_math_prediction_solution(table)}")
+            answer.append(f"Mx = ⁱ⁼¹∑ⁿ(xi * pi) = {find_math_prediction_solution(table)}")
 
             return answer
         except:
             return ["""Возникла ошибка при обработке введённых данных. Проверьте правильность ввода."""]
 
-__all__ = ['combinations', 'buckets_n_balls_solution', 'buckets_n_balls_terminal', 'things_complexity_solution', 'things_complexity_terminal',
-'geometric_meeting_solution', 'geometric_meeting_terminal']
+def find_dispersion_solution(table: EttaTable):
+    """
+    Функция, считающая дисперсию для таблицы СВ
+
+    Args:
+        table (EttaTable): таблица СВ
+
+    Returns:
+        float: дисперсия СВ
+    """
+    if table != None:
+        summ = 0
+        math_prediction = find_math_prediction_solution(table, 1)
+        for cell in table.cells:
+            summ += (cell.etta_value - math_prediction)**2 * cell.probability
+        return summ
+
+def find_dispersion_terminal():
+    """
+    Функция, считающая дисперсию для таблицы СВ
+    """
+    n = int(input("Введите количество значений в таблице: "))
+    table = EttaTable()
+    for i in range(0, n):
+        v, p = map(int, input(f"введите пару чисел (значение, вероятность) для {i+1}-го значения").split())
+        table.cells.append(EttaTableCell(etta_value=v, probability=p))
+    print(f"Dx = ⁱ⁼¹∑ⁿ( (xi - M(X))² pi ) = {find_dispersion_solution(table)}")
+
+def find_dispersion_request(text: str = None):
+    """
+    Нахождение дисперси СВ по таблице значений СВ
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
+            answer.append(f"Dx = ⁱ⁼¹∑ⁿ( (xi - M(X))² pi ) = {find_dispersion_solution(table)}")
+
+            return answer
+        except:
+            return ["""Возникла ошибка при обработке введённых данных. Проверьте правильность ввода."""]
+
+def table_analysis_solution(table: EttaTable):
+    """
+    Находит Мx и Dx для таблицы значений СВ
+
+    Args:
+        table (EttaTable): таблица значений СВ
+
+    Returns:
+        list: [float, float] - массив со значениями Mx и Dx
+    """
+    mat_prediction = find_math_prediction_solution(table)
+    dispersion = find_dispersion_solution(table)
+
+    return [mat_prediction, dispersion]
+
+def table_analysis_terminal():
+    """
+    Функция, считающая дисперсию и математическое ожидание для таблицы СВ
+    """
+    n = int(input("Введите количество значений в таблице: "))
+    table = EttaTable()
+    for i in range(0, n):
+        v, p = map(int, input(f"введите пару чисел (значение, вероятность) для {i+1}-го значения").split())
+        table.cells.append(EttaTableCell(etta_value=v, probability=p))
+    result = table_analysis_solution(table)
+    print(f"Mx = ⁱ⁼¹∑ⁿ(xi * pi) = {result[0]}\nDx = ⁱ⁼¹∑ⁿ( (xi - M(X))² pi ) = {result[1]}")
+
+def table_analysis_request(text: str = None):
+    """
+    Нахождение дисперси и математического ожидания СВ по таблице значений СВ
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
+            result = table_analysis_solution(table)
+            answer.append(f"Mx = ⁱ⁼¹∑ⁿ(xi * pi) = {result[0]}")
+            answer.append(f"Dx = ⁱ⁼¹∑ⁿ( (xi - M(X))² pi ) = {result[1]}")
+
+            return answer
+        except:
+            return ["""Возникла ошибка при обработке введённых данных. Проверьте правильность ввода."""]
```

### Comparing `MKN_third_codes-0.4.4.1/MKN_third_codes.egg-info/PKG-INFO` & `MKN_third_codes-0.6.0.3/MKN_third_codes.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,57 +1,68 @@
 Metadata-Version: 2.1
 Name: MKN-third-codes
-Version: 0.4.4.1
+Version: 0.6.0.3
 Summary: Python library with standart solutions for probability tasks
 Author: Dolgun Ivan
 Author-email: vanadolgun@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 ### Здарова! Библиотека немного помогает с тервером по МКН 3
 
-## 📦 Версия: 0.4.4
+# 📦 Версия: 0.6.0
 
 - Функции buckets_n_balls => задачи про урны
 - Функции things_complexity => задачи про путаницу вещей
 - Функции geometric_meeting => задачи про встречи
-- Функции find_math_prediction => нахождение Математического ожидания
+- Функции find_math_prediction => нахождение математического ожидания для таблицы СВ
+- Функции find_disperion => нахождение дисперсии для таблицы СВ
+- Функции table_analysis => нахождение МО и Дисперсии для таблицы СВ
 - Функция combinations => число сочетаний
 
 # 🔩 Использование
 ## 📥 Импортирование
-### from MKN_third_codes import solutions
+### `from MKN_third_codes import solutions`
 ## 🕹 Функции
 - 📱 любая функция, решающая задачу имеет суффикс '_terminal'. Это значит, что, используя данную функцию, дополнительно ничего писать не надо, т.к. она представляет из себя готовое решение типа задач. Всё взаимодействие происходит в терминале.
 - 📲 любая функция, решающая задачу имеет суффикс '_solution'. Такая функция принимает аргументы на вход, которые ей следует предоставить. В описании каждой функции есть описание возвращаемого объекта.
 - 📨 любая функция, решающая задачу имеет суффикс '_request'. Этот тип функций позволяет взаимодействовать с ней извне, например, отсылая в качестве входного параметра ввод пользователя.
 ## 🧱 Классы
 - Классы данной библиотеки можно использовать вне функций, предоставляемых данной библиотекой, но т.к. классы заточены под неё, то ими возможно будет неудобно пользоваться.
 
 # ✅ Установка
-### Консоль: pip install --upgrade MKN_third_codes
+### Консоль: `pip install --upgrade MKN_third_codes`
 ## Страница библиотеки: [MKN_lib][libaPage]
 
 # 🧀 Не хотите париться с библиотекой?
 ## Бот [Lengendary Solver Bot][AlekseiBot] предоставляет возможность использования всех возможностей библиотеки в удобном интерфейсе телеграма.
-### Автор: [Алексей Шумков][LehaVK]
+### Автор бота: [Алексей Шумков][LehaVK]
 
-## ☎️ Контакты
-### Я в ВК: [Долгун Иван][vkCom]
-### Я в Discord: ИVAN#2599
+# ☎️ Контакты #
+## Я в ВК: <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/f3/VK_Compact_Logo_%282021-present%29.svg/2048px-VK_Compact_Logo_%282021-present%29.svg.png" alt="мл-icon" height="10%">[Долгун Иван][vkCom]
+## Я в Discord: <img src="https://uxwing.com/wp-content/themes/uxwing/download/brands-and-social-media/discord-square-color-icon.png" alt="discord-icon" height="20rem">ИVAN#2599
 
 [vkCom]: https://vk.com/ivandolgun
 [libaPage]: https://pypi.org/project/MKN-third-codes/
 [AlekseiBot]: https://t.me/mkn_solver_bot
 [LehaVK]: https://vk.com/miranchuk5959
 #
-### Change Log
+## Change Log
 ====================
 
+## 0.6.0 (01/05/2023)
+```
+------------------
+┏ добавлены 'find_dispersion' решения
+┣ добавлены 'table_analysis' решения
+┗ иправлена ошибка в вычислениях задачи о путанице вещей
+------------------
+```
+# ------------------
 ## 0.4.4 (01/05/2023)
 ```
 ------------------
 ━ исправлено отображение Change Log
 ------------------
 ```
 # ------------------
```

### Comparing `MKN_third_codes-0.4.4.1/PKG-INFO` & `MKN_third_codes-0.6.0.3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,89 +1,38 @@
-Metadata-Version: 2.1
-Name: MKN_third_codes
-Version: 0.4.4.1
-Summary: Python library with standart solutions for probability tasks
-Author: Dolgun Ivan
-Author-email: vanadolgun@gmail.com
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 ### Здарова! Библиотека немного помогает с тервером по МКН 3
 
-## 📦 Версия: 0.4.4
+# 📦 Версия: 0.6.0
 
 - Функции buckets_n_balls => задачи про урны
 - Функции things_complexity => задачи про путаницу вещей
 - Функции geometric_meeting => задачи про встречи
-- Функции find_math_prediction => нахождение Математического ожидания
+- Функции find_math_prediction => нахождение математического ожидания для таблицы СВ
+- Функции find_disperion => нахождение дисперсии для таблицы СВ
+- Функции table_analysis => нахождение МО и Дисперсии для таблицы СВ
 - Функция combinations => число сочетаний
 
 # 🔩 Использование
 ## 📥 Импортирование
-### from MKN_third_codes import solutions
+### `from MKN_third_codes import solutions`
 ## 🕹 Функции
 - 📱 любая функция, решающая задачу имеет суффикс '_terminal'. Это значит, что, используя данную функцию, дополнительно ничего писать не надо, т.к. она представляет из себя готовое решение типа задач. Всё взаимодействие происходит в терминале.
 - 📲 любая функция, решающая задачу имеет суффикс '_solution'. Такая функция принимает аргументы на вход, которые ей следует предоставить. В описании каждой функции есть описание возвращаемого объекта.
 - 📨 любая функция, решающая задачу имеет суффикс '_request'. Этот тип функций позволяет взаимодействовать с ней извне, например, отсылая в качестве входного параметра ввод пользователя.
 ## 🧱 Классы
 - Классы данной библиотеки можно использовать вне функций, предоставляемых данной библиотекой, но т.к. классы заточены под неё, то ими возможно будет неудобно пользоваться.
 
 # ✅ Установка
-### Консоль: pip install --upgrade MKN_third_codes
+### Консоль: `pip install --upgrade MKN_third_codes`
 ## Страница библиотеки: [MKN_lib][libaPage]
 
 # 🧀 Не хотите париться с библиотекой?
 ## Бот [Lengendary Solver Bot][AlekseiBot] предоставляет возможность использования всех возможностей библиотеки в удобном интерфейсе телеграма.
-### Автор: [Алексей Шумков][LehaVK]
+### Автор бота: [Алексей Шумков][LehaVK]
 
-## ☎️ Контакты
-### Я в ВК: [Долгун Иван][vkCom]
-### Я в Discord: ИVAN#2599
+# ☎️ Контакты #
+## Я в ВК: <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/f3/VK_Compact_Logo_%282021-present%29.svg/2048px-VK_Compact_Logo_%282021-present%29.svg.png" alt="мл-icon" height="10%">[Долгун Иван][vkCom]
+## Я в Discord: <img src="https://uxwing.com/wp-content/themes/uxwing/download/brands-and-social-media/discord-square-color-icon.png" alt="discord-icon" height="20rem">ИVAN#2599
 
 [vkCom]: https://vk.com/ivandolgun
 [libaPage]: https://pypi.org/project/MKN-third-codes/
 [AlekseiBot]: https://t.me/mkn_solver_bot
-[LehaVK]: https://vk.com/miranchuk5959
-#
-### Change Log
-====================
-
-## 0.4.4 (01/05/2023)
-```
-------------------
-━ исправлено отображение Change Log
-------------------
-```
-# ------------------
-## 0.4.3 (01/05/2023)
-```
-------------------
-┏ добавлены '_request' типы для всех функций
-┣ исправлена ошибка в вычислениях для задач о встречах
-┗ добавлены 'find_math_prediction' решения
-------------------
-```
-# ------------------
-### 0.3.3 (29/04/2023)
-```
-------------------
-━ починил README для PYPI
-------------------
-```
-# ------------------
-### 0.3.2 (29/04/2023)
-```
-------------------
-━ README.md
-------------------
-```
-# ------------------
-## 0.3.1 (29/04/2023)
-```
-------------------
-┏ оптимизированы 'things_complexity' решения
-┣ добавлены 'geometric_meeting' решения
-┃   ┗ новый класс 'Meetiner'
-┗ добавлен Change Log
-------------------
-```
+[LehaVK]: https://vk.com/miranchuk5959
```

