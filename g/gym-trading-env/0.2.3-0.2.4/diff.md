# Comparing `tmp/gym-trading-env-0.2.3.tar.gz` & `tmp/gym-trading-env-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gym-trading-env-0.2.3.tar", last modified: Tue Apr 25 12:46:34 2023, max compression
+gzip compressed data, was "gym-trading-env-0.2.4.tar", last modified: Mon May  1 20:30:42 2023, max compression
```

## Comparing `gym-trading-env-0.2.3.tar` & `gym-trading-env-0.2.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 12:46:34.488030 gym-trading-env-0.2.3/
--rw-rw-rw-   0        0        0     1088 2023-03-28 11:11:31.000000 gym-trading-env-0.2.3/LICENSE.txt
--rw-rw-rw-   0        0        0       44 2023-04-23 18:13:37.000000 gym-trading-env-0.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0     4431 2023-04-25 12:46:34.486034 gym-trading-env-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     2569 2023-04-25 12:45:18.000000 gym-trading-env-0.2.3/README.md
--rw-rw-rw-   0        0        0      870 2023-04-25 12:45:19.000000 gym-trading-env-0.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-25 12:46:34.489028 gym-trading-env-0.2.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-25 12:46:34.382312 gym-trading-env-0.2.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-25 12:46:34.420211 gym-trading-env-0.2.3/src/gym_trading_env/
--rw-rw-rw-   0        0        0      333 2023-04-15 09:28:44.000000 gym-trading-env-0.2.3/src/gym_trading_env/__init__.py
--rw-rw-rw-   0        0        0     4164 2023-04-13 12:51:04.000000 gym-trading-env-0.2.3/src/gym_trading_env/downloader.py
--rw-rw-rw-   0        0        0    14459 2023-04-25 09:39:29.000000 gym-trading-env-0.2.3/src/gym_trading_env/environments.py
--rw-rw-rw-   0        0        0     2504 2023-04-24 23:59:53.000000 gym-trading-env-0.2.3/src/gym_trading_env/renderer.py
-drwxrwxrwx   0        0        0        0 2023-04-25 12:46:34.465091 gym-trading-env-0.2.3/src/gym_trading_env/templates/
--rw-rw-rw-   0        0        0     3878 2023-04-25 08:50:20.000000 gym-trading-env-0.2.3/src/gym_trading_env/templates/index.html
-drwxrwxrwx   0        0        0        0 2023-04-25 12:46:34.481048 gym-trading-env-0.2.3/src/gym_trading_env/utils/
--rw-rw-rw-   0        0        0        0 2023-04-02 16:47:36.000000 gym-trading-env-0.2.3/src/gym_trading_env/utils/__init__.py
--rw-rw-rw-   0        0        0    14334 2023-04-05 09:25:28.000000 gym-trading-env-0.2.3/src/gym_trading_env/utils/charts.py
--rw-rw-rw-   0        0        0     3333 2023-04-02 16:57:28.000000 gym-trading-env-0.2.3/src/gym_trading_env/utils/history.py
--rw-rw-rw-   0        0        0     3036 2023-04-02 16:57:45.000000 gym-trading-env-0.2.3/src/gym_trading_env/utils/portfolio.py
-drwxrwxrwx   0        0        0        0 2023-04-25 12:46:34.463097 gym-trading-env-0.2.3/src/gym_trading_env.egg-info/
--rw-rw-rw-   0        0        0     4431 2023-04-25 12:46:34.000000 gym-trading-env-0.2.3/src/gym_trading_env.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      587 2023-04-25 12:46:34.000000 gym-trading-env-0.2.3/src/gym_trading_env.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 12:46:34.000000 gym-trading-env-0.2.3/src/gym_trading_env.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      116 2023-04-25 12:46:34.000000 gym-trading-env-0.2.3/src/gym_trading_env.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-25 12:46:34.000000 gym-trading-env-0.2.3/src/gym_trading_env.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 20:30:42.958728 gym-trading-env-0.2.4/
+-rw-rw-rw-   0        0        0     1088 2023-03-28 11:11:31.000000 gym-trading-env-0.2.4/LICENSE.txt
+-rw-rw-rw-   0        0        0       44 2023-04-23 18:13:37.000000 gym-trading-env-0.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     4435 2023-05-01 20:30:42.955736 gym-trading-env-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2573 2023-04-25 15:30:12.000000 gym-trading-env-0.2.4/README.md
+-rw-rw-rw-   0        0        0      853 2023-05-01 20:30:04.000000 gym-trading-env-0.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-01 20:30:42.958728 gym-trading-env-0.2.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-01 20:30:42.768658 gym-trading-env-0.2.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-01 20:30:42.809578 gym-trading-env-0.2.4/src/gym_trading_env/
+-rw-rw-rw-   0        0        0      333 2023-04-15 09:28:44.000000 gym-trading-env-0.2.4/src/gym_trading_env/__init__.py
+-rw-rw-rw-   0        0        0     4164 2023-04-13 12:51:04.000000 gym-trading-env-0.2.4/src/gym_trading_env/downloader.py
+-rw-rw-rw-   0        0        0    14568 2023-04-25 14:03:39.000000 gym-trading-env-0.2.4/src/gym_trading_env/environments.py
+-rw-rw-rw-   0        0        0     2504 2023-04-24 23:59:53.000000 gym-trading-env-0.2.4/src/gym_trading_env/renderer.py
+drwxrwxrwx   0        0        0        0 2023-05-01 20:30:42.918835 gym-trading-env-0.2.4/src/gym_trading_env/templates/
+-rw-rw-rw-   0        0        0     3878 2023-04-25 08:50:20.000000 gym-trading-env-0.2.4/src/gym_trading_env/templates/index.html
+drwxrwxrwx   0        0        0        0 2023-05-01 20:30:42.953741 gym-trading-env-0.2.4/src/gym_trading_env/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-02 16:47:36.000000 gym-trading-env-0.2.4/src/gym_trading_env/utils/__init__.py
+-rw-rw-rw-   0        0        0    14334 2023-04-05 09:25:28.000000 gym-trading-env-0.2.4/src/gym_trading_env/utils/charts.py
+-rw-rw-rw-   0        0        0     3333 2023-04-02 16:57:28.000000 gym-trading-env-0.2.4/src/gym_trading_env/utils/history.py
+-rw-rw-rw-   0        0        0     3036 2023-04-02 16:57:45.000000 gym-trading-env-0.2.4/src/gym_trading_env/utils/portfolio.py
+drwxrwxrwx   0        0        0        0 2023-05-01 20:30:42.850018 gym-trading-env-0.2.4/src/gym_trading_env.egg-info/
+-rw-rw-rw-   0        0        0     4435 2023-05-01 20:30:42.000000 gym-trading-env-0.2.4/src/gym_trading_env.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      587 2023-05-01 20:30:42.000000 gym-trading-env-0.2.4/src/gym_trading_env.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 20:30:42.000000 gym-trading-env-0.2.4/src/gym_trading_env.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2023-05-01 20:30:42.000000 gym-trading-env-0.2.4/src/gym_trading_env.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-01 20:30:42.000000 gym-trading-env-0.2.4/src/gym_trading_env.egg-info/top_level.txt
```

### Comparing `gym-trading-env-0.2.3/LICENSE.txt` & `gym-trading-env-0.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.2.3/PKG-INFO` & `gym-trading-env-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym-trading-env
-Version: 0.2.3
+Version: 0.2.4
 Summary: A simple, easy, customizable Open IA Gym environments for trading.
 Author-email: Clement Perroud <clement.perroud.pro@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -55,30 +55,30 @@
          <img src='https://readthedocs.org/projects/gym-trading-env/badge/?version=latest' alt='Documentation Status' />
    </a>
    <a href="https://github.com/ClementPerroud/Gym-Trading-Env">
       <img src="https://img.shields.io/github/stars/ClementPerroud/gym-trading-env?style=social" alt="Github stars">
    </a>
 </section>
   
-Cryto Trading Env is an OpenAI Gym environment for simulating stocks and train Reinforcement Learning (RL) trading agents.
-It was designed to be fast and customizable for easy RL trading algorythms implementation.
+Crypto Trading Env is an OpenAI Gym environment for simulating stocks and training Reinforcement Learning (RL) trading agents.
+It was designed to be fast and customizable for easy RL trading algorithms implementation.
 
 
 | [Documentation](https://gym-trading-env.readthedocs.io/en/latest/index.html) |
 
 
 Key features
 ---------------
 
 This package aims to greatly simplify the research phase by offering :
 
 * Easy and quick download technical data on several exchanges
 * A simple and fast environment for the user and the AI, but which allows complex operations (Short, Margin trading).
 * A high performance rendering (can display several hundred thousand candles simultaneously), customizable to visualize the actions of its agent and its results.
-* (Coming soon) An easy way to backtest any RL-Agents or any king 
+* (Coming soon) An easy way to backtest any RL-Agents or any kind 
 
 ![Render animated image](https://raw.githubusercontent.com/ClementPerroud/Gym-Trading-Env/main/docs/source/images/render.gif)
 
 Installation
 ---------------
 
 Crypto Trading Env supports Python 3.9+ on Windows, Mac, and Linux. You can install it using pip:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gym-trading-env Version: 0.2.3 Summary: A simple,
+Metadata-Version: 2.1 Name: gym-trading-env Version: 0.2.4 Summary: A simple,
 easy, customizable Open IA Gym environments for trading. Author-email: Clement
 Perroud
 perroud.pro@gmail.com> License: MIT License Copyright (c) [year] [fullname]
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
@@ -20,25 +20,25 @@
 ClementPerroud/Gym-Trading-Env/issues Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.7 Description-Content-
 Type: text/markdown License-File: LICENSE.txt
 ****** [https://github.com/ClementPerroud/Gym-Trading-Env/raw/main/docs/source/
                        images/logo_light-bg.png] ******
  [python] [PyPI] [Apache_2.0_with_Commons_Clause] [Documentation_Status]
-[Github_stars]  Cryto Trading Env is an OpenAI Gym environment for simulating
-stocks and train Reinforcement Learning (RL) trading agents. It was designed to
-be fast and customizable for easy RL trading algorythms implementation. |
+[Github_stars]  Crypto Trading Env is an OpenAI Gym environment for simulating
+stocks and training Reinforcement Learning (RL) trading agents. It was designed
+to be fast and customizable for easy RL trading algorithms implementation. |
 [Documentation](https://gym-trading-env.readthedocs.io/en/latest/index.html) |
 Key features --------------- This package aims to greatly simplify the research
 phase by offering : * Easy and quick download technical data on several
 exchanges * A simple and fast environment for the user and the AI, but which
 allows complex operations (Short, Margin trading). * A high performance
 rendering (can display several hundred thousand candles simultaneously),
 customizable to visualize the actions of its agent and its results. * (Coming
-soon) An easy way to backtest any RL-Agents or any king ![Render animated
+soon) An easy way to backtest any RL-Agents or any kind ![Render animated
 image](https://raw.githubusercontent.com/ClementPerroud/Gym-Trading-Env/main/
 docs/source/images/render.gif) Installation --------------- Crypto Trading Env
 supports Python 3.9+ on Windows, Mac, and Linux. You can install it using pip:
 ```bash pip install gym-trading-env ``` Or using git : ```bash git clone https:
 //github.com/ClementPerroud/Gym-Trading-Env ``` [Documentation available here]
 (https://gym-trading-env.readthedocs.io/en/latest/index.html) -----------------
 ------------------------------------------------------------------------------
```

### Comparing `gym-trading-env-0.2.3/README.md` & `gym-trading-env-0.2.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -20,30 +20,30 @@
          <img src='https://readthedocs.org/projects/gym-trading-env/badge/?version=latest' alt='Documentation Status' />
    </a>
    <a href="https://github.com/ClementPerroud/Gym-Trading-Env">
       <img src="https://img.shields.io/github/stars/ClementPerroud/gym-trading-env?style=social" alt="Github stars">
    </a>
 </section>
   
-Cryto Trading Env is an OpenAI Gym environment for simulating stocks and train Reinforcement Learning (RL) trading agents.
-It was designed to be fast and customizable for easy RL trading algorythms implementation.
+Crypto Trading Env is an OpenAI Gym environment for simulating stocks and training Reinforcement Learning (RL) trading agents.
+It was designed to be fast and customizable for easy RL trading algorithms implementation.
 
 
 | [Documentation](https://gym-trading-env.readthedocs.io/en/latest/index.html) |
 
 
 Key features
 ---------------
 
 This package aims to greatly simplify the research phase by offering :
 
 * Easy and quick download technical data on several exchanges
 * A simple and fast environment for the user and the AI, but which allows complex operations (Short, Margin trading).
 * A high performance rendering (can display several hundred thousand candles simultaneously), customizable to visualize the actions of its agent and its results.
-* (Coming soon) An easy way to backtest any RL-Agents or any king 
+* (Coming soon) An easy way to backtest any RL-Agents or any kind 
 
 ![Render animated image](https://raw.githubusercontent.com/ClementPerroud/Gym-Trading-Env/main/docs/source/images/render.gif)
 
 Installation
 ---------------
 
 Crypto Trading Env supports Python 3.9+ on Windows, Mac, and Linux. You can install it using pip:
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
 ****** [https://github.com/ClementPerroud/Gym-Trading-Env/raw/main/docs/source/
                        images/logo_light-bg.png] ******
  [python] [PyPI] [Apache_2.0_with_Commons_Clause] [Documentation_Status]
-[Github_stars]  Cryto Trading Env is an OpenAI Gym environment for simulating
-stocks and train Reinforcement Learning (RL) trading agents. It was designed to
-be fast and customizable for easy RL trading algorythms implementation. |
+[Github_stars]  Crypto Trading Env is an OpenAI Gym environment for simulating
+stocks and training Reinforcement Learning (RL) trading agents. It was designed
+to be fast and customizable for easy RL trading algorithms implementation. |
 [Documentation](https://gym-trading-env.readthedocs.io/en/latest/index.html) |
 Key features --------------- This package aims to greatly simplify the research
 phase by offering : * Easy and quick download technical data on several
 exchanges * A simple and fast environment for the user and the AI, but which
 allows complex operations (Short, Margin trading). * A high performance
 rendering (can display several hundred thousand candles simultaneously),
 customizable to visualize the actions of its agent and its results. * (Coming
-soon) An easy way to backtest any RL-Agents or any king ![Render animated
+soon) An easy way to backtest any RL-Agents or any kind ![Render animated
 image](https://raw.githubusercontent.com/ClementPerroud/Gym-Trading-Env/main/
 docs/source/images/render.gif) Installation --------------- Crypto Trading Env
 supports Python 3.9+ on Windows, Mac, and Linux. You can install it using pip:
 ```bash pip install gym-trading-env ``` Or using git : ```bash git clone https:
 //github.com/ClementPerroud/Gym-Trading-Env ``` [Documentation available here]
 (https://gym-trading-env.readthedocs.io/en/latest/index.html) -----------------
 ------------------------------------------------------------------------------
```

### Comparing `gym-trading-env-0.2.3/pyproject.toml` & `gym-trading-env-0.2.4/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gym-trading-env"
-version = "0.2.3"
+version = "0.2.4"
 license = {file = "LICENSE.txt"}
 authors = [
   { name="Clement Perroud", email="clement.perroud.pro@gmail.com" },
 ]
 description = "A simple, easy, customizable Open IA Gym environments for trading."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-dependencies = ["pandas>=1.5.3", "numpy>=1.23.1", "gymnasium>=0.28.1", "flask>=2.2.3", "pyecharts>=2.0.2", "ccxt==3.0.59", "numpy>=1.24.2", "nest_asyncio"]
+dependencies = ["pandas>=1.5.3", "numpy>=1.21.1", "gymnasium>=0.28.1", "flask>=2.2.3", "pyecharts>=2.0.2", "ccxt==3.0.59", "nest_asyncio"]
 
 [project.urls]
 "Homepage" = "https://github.com/ClementPerroud/Gym-Trading-Env"
 "Bug Tracker" = "https://github.com/ClementPerroud/Gym-Trading-Env/issues"
```

### Comparing `gym-trading-env-0.2.3/src/gym_trading_env/downloader.py` & `gym-trading-env-0.2.4/src/gym_trading_env/downloader.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.2.3/src/gym_trading_env/environments.py` & `gym-trading-env-0.2.4/src/gym_trading_env/environments.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,33 +32,33 @@
 
     :param positions: List of the positions allowed by the environment.
     :type positions: optional - list[int or float]
 
     :param reward_function: Take the History object of the environment and must return a float.
     :type reward_function: optional - function<History->float>
 
-    :param windows: Default is None. If it is set to an int: N, every step observation will return the past N observations. It is recommended for Reccurent Neural Network based Agents.
+    :param windows: Default is None. If it is set to an int: N, every step observation will return the past N observations. It is recommended for Recurrent Neural Network based Agents.
     :type windows: optional - None or int
 
-    :param trading_fees: Transaction trading fees (buy and sell operations). eg: 0.01 correspondss to 1% fees
+    :param trading_fees: Transaction trading fees (buy and sell operations). eg: 0.01 corresponds to 1% fees
     :type trading_fees: optional - float
 
-    :param borrow_interest_rate: Borrow interest rate per step (only when position < 0 or position > 1). eg: 0.01 correspond to 1% borrow interest rate per STEP ; if your know that your borrow interest rate is 0.05% per day and that your timestep is 1 hour, you need to divide it by 24 -> 0.05/100/24.
+    :param borrow_interest_rate: Borrow interest rate per step (only when position < 0 or position > 1). eg: 0.01 corresponds to 1% borrow interest rate per STEP ; if your know that your borrow interest rate is 0.05% per day and that your timestep is 1 hour, you need to divide it by 24 -> 0.05/100/24.
     :type borrow_interest_rate: optional - float
 
     :param portfolio_initial_value: Initial valuation of the portfolio.
     :type portfolio_initial_value: float or int
 
-    :param initial_position: Initial position of the environmnent. It must contained in the list parameter 'positions'.
+    :param initial_position: Initial position of the environment. It must contained in the list parameter 'positions'.
     :type initial_position: optional - float or int
 
     :param include_position_in_features: Whether or not you want the current position to be added to the step observations. If windows is set an int, it will add the last N-step positions.
     :type include_position_in_features: optional - bool
 
-    :param verbose: If 0, no log is outputed. If 1, the env send episode result logs.
+    :param verbose: If 0, no log is outputted. If 1, the env send episode result logs.
     :type verbose: optional - int
     
     :param name: The name of the environment (eg. 'BTC/USDT')
     :type name: optional - str
     
     """
     metadata = {'render_modes': ['logs']}
@@ -253,16 +253,16 @@
         render_df = self.df.join(history_df, how = "inner")
         
         if not os.path.exists(dir):os.makedirs(dir)
         render_df.to_pickle(f"{dir}/{self.name}_{datetime.datetime.now().strftime('%Y-%m-%d_%H-%M-%S')}.pkl")
 
 class MultiDatasetTradingEnv(TradingEnv):
     """
-    (Inherits from TradingEnv) A TradingEnv environment that handle multiple datasets.
-    It automatically switchs from one dataset to another at the end of an episode.
+    (Inherits from TradingEnv) A TradingEnv environment that handles multiple datasets.
+    It automatically switches from one dataset to another at the end of an episode.
     Bringing diversity by having several datasets, even from the same pair from different exchanges, is a good idea.
     This should help avoiding overfitting.
 
     It is recommended to use it this way :
     
     .. code-block:: python
 
@@ -271,20 +271,20 @@
         env = gym.make('MultiDatasetTradingEnv',
             dataset_dir = 'data/*.pkl',
             ...
         )
     
     
     
-    :param dataset_dir: A `glob path <https://docs.python.org/3.6/library/glob.html>`_ that needs to match your datasets. All of your datasets needs to match the dataset requirements (see docs from TradingEnv).
+    :param dataset_dir: A `glob path <https://docs.python.org/3.6/library/glob.html>`_ that needs to match your datasets. All of your datasets needs to match the dataset requirements (see docs from TradingEnv). If it is not the case, you can use the ``preprocess`` param to make your datasets match the requirements.
     :type dataset_dir: str
 
     :param preprocess: This function takes a pandas.DataFrame and returns a pandas.DataFrame. This function is applied to each dataset before being used in the environment.
         
-        For example, imagine you have a folder named 'data' with several datasets (formated as .pkl)
+        For example, imagine you have a folder named 'data' with several datasets (formatted as .pkl)
 
         .. code-block:: python
 
             import pandas as pd
             import numpy as np
             import gymnasium as gym
             from gym_trading_env
```

### Comparing `gym-trading-env-0.2.3/src/gym_trading_env/renderer.py` & `gym-trading-env-0.2.4/src/gym_trading_env/renderer.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.2.3/src/gym_trading_env/templates/index.html` & `gym-trading-env-0.2.4/src/gym_trading_env/templates/index.html`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.2.3/src/gym_trading_env/utils/charts.py` & `gym-trading-env-0.2.4/src/gym_trading_env/utils/charts.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.2.3/src/gym_trading_env/utils/history.py` & `gym-trading-env-0.2.4/src/gym_trading_env/utils/history.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.2.3/src/gym_trading_env/utils/portfolio.py` & `gym-trading-env-0.2.4/src/gym_trading_env/utils/portfolio.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.2.3/src/gym_trading_env.egg-info/PKG-INFO` & `gym-trading-env-0.2.4/src/gym_trading_env.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym-trading-env
-Version: 0.2.3
+Version: 0.2.4
 Summary: A simple, easy, customizable Open IA Gym environments for trading.
 Author-email: Clement Perroud <clement.perroud.pro@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -55,30 +55,30 @@
          <img src='https://readthedocs.org/projects/gym-trading-env/badge/?version=latest' alt='Documentation Status' />
    </a>
    <a href="https://github.com/ClementPerroud/Gym-Trading-Env">
       <img src="https://img.shields.io/github/stars/ClementPerroud/gym-trading-env?style=social" alt="Github stars">
    </a>
 </section>
   
-Cryto Trading Env is an OpenAI Gym environment for simulating stocks and train Reinforcement Learning (RL) trading agents.
-It was designed to be fast and customizable for easy RL trading algorythms implementation.
+Crypto Trading Env is an OpenAI Gym environment for simulating stocks and training Reinforcement Learning (RL) trading agents.
+It was designed to be fast and customizable for easy RL trading algorithms implementation.
 
 
 | [Documentation](https://gym-trading-env.readthedocs.io/en/latest/index.html) |
 
 
 Key features
 ---------------
 
 This package aims to greatly simplify the research phase by offering :
 
 * Easy and quick download technical data on several exchanges
 * A simple and fast environment for the user and the AI, but which allows complex operations (Short, Margin trading).
 * A high performance rendering (can display several hundred thousand candles simultaneously), customizable to visualize the actions of its agent and its results.
-* (Coming soon) An easy way to backtest any RL-Agents or any king 
+* (Coming soon) An easy way to backtest any RL-Agents or any kind 
 
 ![Render animated image](https://raw.githubusercontent.com/ClementPerroud/Gym-Trading-Env/main/docs/source/images/render.gif)
 
 Installation
 ---------------
 
 Crypto Trading Env supports Python 3.9+ on Windows, Mac, and Linux. You can install it using pip:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gym-trading-env Version: 0.2.3 Summary: A simple,
+Metadata-Version: 2.1 Name: gym-trading-env Version: 0.2.4 Summary: A simple,
 easy, customizable Open IA Gym environments for trading. Author-email: Clement
 Perroud
 perroud.pro@gmail.com> License: MIT License Copyright (c) [year] [fullname]
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
@@ -20,25 +20,25 @@
 ClementPerroud/Gym-Trading-Env/issues Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.7 Description-Content-
 Type: text/markdown License-File: LICENSE.txt
 ****** [https://github.com/ClementPerroud/Gym-Trading-Env/raw/main/docs/source/
                        images/logo_light-bg.png] ******
  [python] [PyPI] [Apache_2.0_with_Commons_Clause] [Documentation_Status]
-[Github_stars]  Cryto Trading Env is an OpenAI Gym environment for simulating
-stocks and train Reinforcement Learning (RL) trading agents. It was designed to
-be fast and customizable for easy RL trading algorythms implementation. |
+[Github_stars]  Crypto Trading Env is an OpenAI Gym environment for simulating
+stocks and training Reinforcement Learning (RL) trading agents. It was designed
+to be fast and customizable for easy RL trading algorithms implementation. |
 [Documentation](https://gym-trading-env.readthedocs.io/en/latest/index.html) |
 Key features --------------- This package aims to greatly simplify the research
 phase by offering : * Easy and quick download technical data on several
 exchanges * A simple and fast environment for the user and the AI, but which
 allows complex operations (Short, Margin trading). * A high performance
 rendering (can display several hundred thousand candles simultaneously),
 customizable to visualize the actions of its agent and its results. * (Coming
-soon) An easy way to backtest any RL-Agents or any king ![Render animated
+soon) An easy way to backtest any RL-Agents or any kind ![Render animated
 image](https://raw.githubusercontent.com/ClementPerroud/Gym-Trading-Env/main/
 docs/source/images/render.gif) Installation --------------- Crypto Trading Env
 supports Python 3.9+ on Windows, Mac, and Linux. You can install it using pip:
 ```bash pip install gym-trading-env ``` Or using git : ```bash git clone https:
 //github.com/ClementPerroud/Gym-Trading-Env ``` [Documentation available here]
 (https://gym-trading-env.readthedocs.io/en/latest/index.html) -----------------
 ------------------------------------------------------------------------------
```

### Comparing `gym-trading-env-0.2.3/src/gym_trading_env.egg-info/SOURCES.txt` & `gym-trading-env-0.2.4/src/gym_trading_env.egg-info/SOURCES.txt`

 * *Files identical despite different names*

