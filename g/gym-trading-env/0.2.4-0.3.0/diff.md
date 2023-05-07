# Comparing `tmp/gym-trading-env-0.2.4.tar.gz` & `tmp/gym-trading-env-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gym-trading-env-0.2.4.tar", last modified: Mon May  1 20:30:42 2023, max compression
+gzip compressed data, was "gym-trading-env-0.3.0.tar", last modified: Sun May  7 09:52:45 2023, max compression
```

## Comparing `gym-trading-env-0.2.4.tar` & `gym-trading-env-0.3.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 20:30:42.958728 gym-trading-env-0.2.4/
--rw-rw-rw-   0        0        0     1088 2023-03-28 11:11:31.000000 gym-trading-env-0.2.4/LICENSE.txt
--rw-rw-rw-   0        0        0       44 2023-04-23 18:13:37.000000 gym-trading-env-0.2.4/MANIFEST.in
--rw-rw-rw-   0        0        0     4435 2023-05-01 20:30:42.955736 gym-trading-env-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     2573 2023-04-25 15:30:12.000000 gym-trading-env-0.2.4/README.md
--rw-rw-rw-   0        0        0      853 2023-05-01 20:30:04.000000 gym-trading-env-0.2.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-01 20:30:42.958728 gym-trading-env-0.2.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-01 20:30:42.768658 gym-trading-env-0.2.4/src/
-drwxrwxrwx   0        0        0        0 2023-05-01 20:30:42.809578 gym-trading-env-0.2.4/src/gym_trading_env/
--rw-rw-rw-   0        0        0      333 2023-04-15 09:28:44.000000 gym-trading-env-0.2.4/src/gym_trading_env/__init__.py
--rw-rw-rw-   0        0        0     4164 2023-04-13 12:51:04.000000 gym-trading-env-0.2.4/src/gym_trading_env/downloader.py
--rw-rw-rw-   0        0        0    14568 2023-04-25 14:03:39.000000 gym-trading-env-0.2.4/src/gym_trading_env/environments.py
--rw-rw-rw-   0        0        0     2504 2023-04-24 23:59:53.000000 gym-trading-env-0.2.4/src/gym_trading_env/renderer.py
-drwxrwxrwx   0        0        0        0 2023-05-01 20:30:42.918835 gym-trading-env-0.2.4/src/gym_trading_env/templates/
--rw-rw-rw-   0        0        0     3878 2023-04-25 08:50:20.000000 gym-trading-env-0.2.4/src/gym_trading_env/templates/index.html
-drwxrwxrwx   0        0        0        0 2023-05-01 20:30:42.953741 gym-trading-env-0.2.4/src/gym_trading_env/utils/
--rw-rw-rw-   0        0        0        0 2023-04-02 16:47:36.000000 gym-trading-env-0.2.4/src/gym_trading_env/utils/__init__.py
--rw-rw-rw-   0        0        0    14334 2023-04-05 09:25:28.000000 gym-trading-env-0.2.4/src/gym_trading_env/utils/charts.py
--rw-rw-rw-   0        0        0     3333 2023-04-02 16:57:28.000000 gym-trading-env-0.2.4/src/gym_trading_env/utils/history.py
--rw-rw-rw-   0        0        0     3036 2023-04-02 16:57:45.000000 gym-trading-env-0.2.4/src/gym_trading_env/utils/portfolio.py
-drwxrwxrwx   0        0        0        0 2023-05-01 20:30:42.850018 gym-trading-env-0.2.4/src/gym_trading_env.egg-info/
--rw-rw-rw-   0        0        0     4435 2023-05-01 20:30:42.000000 gym-trading-env-0.2.4/src/gym_trading_env.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      587 2023-05-01 20:30:42.000000 gym-trading-env-0.2.4/src/gym_trading_env.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 20:30:42.000000 gym-trading-env-0.2.4/src/gym_trading_env.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2023-05-01 20:30:42.000000 gym-trading-env-0.2.4/src/gym_trading_env.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-01 20:30:42.000000 gym-trading-env-0.2.4/src/gym_trading_env.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-07 09:52:45.615556 gym-trading-env-0.3.0/
+-rw-rw-rw-   0        0        0     1088 2023-03-29 17:01:42.000000 gym-trading-env-0.3.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       44 2023-05-06 13:10:40.000000 gym-trading-env-0.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4428 2023-05-07 09:52:45.613554 gym-trading-env-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2566 2023-05-06 13:10:40.000000 gym-trading-env-0.3.0/README.md
+-rw-rw-rw-   0        0        0      853 2023-05-07 08:41:42.000000 gym-trading-env-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-07 09:52:45.615556 gym-trading-env-0.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-07 09:52:45.434849 gym-trading-env-0.3.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-07 09:52:45.497874 gym-trading-env-0.3.0/src/gym_trading_env/
+-rw-rw-rw-   0        0        0      333 2023-04-13 13:15:17.000000 gym-trading-env-0.3.0/src/gym_trading_env/__init__.py
+-rw-rw-rw-   0        0        0     4164 2023-04-13 12:39:12.000000 gym-trading-env-0.3.0/src/gym_trading_env/downloader.py
+-rw-rw-rw-   0        0        0    16488 2023-05-07 08:31:47.000000 gym-trading-env-0.3.0/src/gym_trading_env/environments.py
+-rw-rw-rw-   0        0        0     2504 2023-05-06 13:10:40.000000 gym-trading-env-0.3.0/src/gym_trading_env/renderer.py
+drwxrwxrwx   0        0        0        0 2023-05-07 09:52:45.584573 gym-trading-env-0.3.0/src/gym_trading_env/templates/
+-rw-rw-rw-   0        0        0     3878 2023-05-06 13:10:40.000000 gym-trading-env-0.3.0/src/gym_trading_env/templates/index.html
+drwxrwxrwx   0        0        0        0 2023-05-07 09:52:45.609553 gym-trading-env-0.3.0/src/gym_trading_env/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-10 08:13:00.000000 gym-trading-env-0.3.0/src/gym_trading_env/utils/__init__.py
+-rw-rw-rw-   0        0        0    14334 2023-04-10 08:13:00.000000 gym-trading-env-0.3.0/src/gym_trading_env/utils/charts.py
+-rw-rw-rw-   0        0        0     3333 2023-04-13 09:31:51.000000 gym-trading-env-0.3.0/src/gym_trading_env/utils/history.py
+-rw-rw-rw-   0        0        0     3036 2023-04-10 08:13:00.000000 gym-trading-env-0.3.0/src/gym_trading_env/utils/portfolio.py
+drwxrwxrwx   0        0        0        0 2023-05-07 09:52:45.540553 gym-trading-env-0.3.0/src/gym_trading_env.egg-info/
+-rw-rw-rw-   0        0        0     4428 2023-05-07 09:52:45.000000 gym-trading-env-0.3.0/src/gym_trading_env.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      587 2023-05-07 09:52:45.000000 gym-trading-env-0.3.0/src/gym_trading_env.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 09:52:45.000000 gym-trading-env-0.3.0/src/gym_trading_env.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2023-05-07 09:52:45.000000 gym-trading-env-0.3.0/src/gym_trading_env.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-07 09:52:45.000000 gym-trading-env-0.3.0/src/gym_trading_env.egg-info/top_level.txt
```

### Comparing `gym-trading-env-0.2.4/LICENSE.txt` & `gym-trading-env-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.2.4/PKG-INFO` & `gym-trading-env-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym-trading-env
-Version: 0.2.4
+Version: 0.3.0
 Summary: A simple, easy, customizable Open IA Gym environments for trading.
 Author-email: Clement Perroud <clement.perroud.pro@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -55,15 +55,15 @@
          <img src='https://readthedocs.org/projects/gym-trading-env/badge/?version=latest' alt='Documentation Status' />
    </a>
    <a href="https://github.com/ClementPerroud/Gym-Trading-Env">
       <img src="https://img.shields.io/github/stars/ClementPerroud/gym-trading-env?style=social" alt="Github stars">
    </a>
 </section>
   
-Crypto Trading Env is an OpenAI Gym environment for simulating stocks and training Reinforcement Learning (RL) trading agents.
+Gym Trading Env is an Gymnasium environment for simulating stocks and training Reinforcement Learning (RL) trading agents.
 It was designed to be fast and customizable for easy RL trading algorithms implementation.
 
 
 | [Documentation](https://gym-trading-env.readthedocs.io/en/latest/index.html) |
 
 
 Key features
@@ -77,15 +77,15 @@
 * (Coming soon) An easy way to backtest any RL-Agents or any kind 
 
 ![Render animated image](https://raw.githubusercontent.com/ClementPerroud/Gym-Trading-Env/main/docs/source/images/render.gif)
 
 Installation
 ---------------
 
-Crypto Trading Env supports Python 3.9+ on Windows, Mac, and Linux. You can install it using pip:
+Gym Trading Env supports Python 3.9+ on Windows, Mac, and Linux. You can install it using pip:
 
 ```bash
 pip install gym-trading-env
 ```
 
 Or using git :
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gym-trading-env Version: 0.2.4 Summary: A simple,
+Metadata-Version: 2.1 Name: gym-trading-env Version: 0.3.0 Summary: A simple,
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
-[Github_stars]  Crypto Trading Env is an OpenAI Gym environment for simulating
+[Github_stars]  Gym Trading Env is an Gymnasium environment for simulating
 stocks and training Reinforcement Learning (RL) trading agents. It was designed
 to be fast and customizable for easy RL trading algorithms implementation. |
 [Documentation](https://gym-trading-env.readthedocs.io/en/latest/index.html) |
 Key features --------------- This package aims to greatly simplify the research
 phase by offering : * Easy and quick download technical data on several
 exchanges * A simple and fast environment for the user and the AI, but which
 allows complex operations (Short, Margin trading). * A high performance
 rendering (can display several hundred thousand candles simultaneously),
 customizable to visualize the actions of its agent and its results. * (Coming
 soon) An easy way to backtest any RL-Agents or any kind ![Render animated
 image](https://raw.githubusercontent.com/ClementPerroud/Gym-Trading-Env/main/
-docs/source/images/render.gif) Installation --------------- Crypto Trading Env
+docs/source/images/render.gif) Installation --------------- Gym Trading Env
 supports Python 3.9+ on Windows, Mac, and Linux. You can install it using pip:
 ```bash pip install gym-trading-env ``` Or using git : ```bash git clone https:
 //github.com/ClementPerroud/Gym-Trading-Env ``` [Documentation available here]
 (https://gym-trading-env.readthedocs.io/en/latest/index.html) -----------------
 ------------------------------------------------------------------------------
```

### Comparing `gym-trading-env-0.2.4/README.md` & `gym-trading-env-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
          <img src='https://readthedocs.org/projects/gym-trading-env/badge/?version=latest' alt='Documentation Status' />
    </a>
    <a href="https://github.com/ClementPerroud/Gym-Trading-Env">
       <img src="https://img.shields.io/github/stars/ClementPerroud/gym-trading-env?style=social" alt="Github stars">
    </a>
 </section>
   
-Crypto Trading Env is an OpenAI Gym environment for simulating stocks and training Reinforcement Learning (RL) trading agents.
+Gym Trading Env is an Gymnasium environment for simulating stocks and training Reinforcement Learning (RL) trading agents.
 It was designed to be fast and customizable for easy RL trading algorithms implementation.
 
 
 | [Documentation](https://gym-trading-env.readthedocs.io/en/latest/index.html) |
 
 
 Key features
@@ -42,15 +42,15 @@
 * (Coming soon) An easy way to backtest any RL-Agents or any kind 
 
 ![Render animated image](https://raw.githubusercontent.com/ClementPerroud/Gym-Trading-Env/main/docs/source/images/render.gif)
 
 Installation
 ---------------
 
-Crypto Trading Env supports Python 3.9+ on Windows, Mac, and Linux. You can install it using pip:
+Gym Trading Env supports Python 3.9+ on Windows, Mac, and Linux. You can install it using pip:
 
 ```bash
 pip install gym-trading-env
 ```
 
 Or using git :
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
 ****** [https://github.com/ClementPerroud/Gym-Trading-Env/raw/main/docs/source/
                        images/logo_light-bg.png] ******
  [python] [PyPI] [Apache_2.0_with_Commons_Clause] [Documentation_Status]
-[Github_stars]  Crypto Trading Env is an OpenAI Gym environment for simulating
+[Github_stars]  Gym Trading Env is an Gymnasium environment for simulating
 stocks and training Reinforcement Learning (RL) trading agents. It was designed
 to be fast and customizable for easy RL trading algorithms implementation. |
 [Documentation](https://gym-trading-env.readthedocs.io/en/latest/index.html) |
 Key features --------------- This package aims to greatly simplify the research
 phase by offering : * Easy and quick download technical data on several
 exchanges * A simple and fast environment for the user and the AI, but which
 allows complex operations (Short, Margin trading). * A high performance
 rendering (can display several hundred thousand candles simultaneously),
 customizable to visualize the actions of its agent and its results. * (Coming
 soon) An easy way to backtest any RL-Agents or any kind ![Render animated
 image](https://raw.githubusercontent.com/ClementPerroud/Gym-Trading-Env/main/
-docs/source/images/render.gif) Installation --------------- Crypto Trading Env
+docs/source/images/render.gif) Installation --------------- Gym Trading Env
 supports Python 3.9+ on Windows, Mac, and Linux. You can install it using pip:
 ```bash pip install gym-trading-env ``` Or using git : ```bash git clone https:
 //github.com/ClementPerroud/Gym-Trading-Env ``` [Documentation available here]
 (https://gym-trading-env.readthedocs.io/en/latest/index.html) -----------------
 ------------------------------------------------------------------------------
```

### Comparing `gym-trading-env-0.2.4/pyproject.toml` & `gym-trading-env-0.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gym-trading-env"
-version = "0.2.4"
+version = "0.3.0"
 license = {file = "LICENSE.txt"}
 authors = [
   { name="Clement Perroud", email="clement.perroud.pro@gmail.com" },
 ]
 description = "A simple, easy, customizable Open IA Gym environments for trading."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `gym-trading-env-0.2.4/src/gym_trading_env/downloader.py` & `gym-trading-env-0.3.0/src/gym_trading_env/downloader.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.2.4/src/gym_trading_env/environments.py` & `gym-trading-env-0.3.0/src/gym_trading_env/environments.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,20 +44,23 @@
 
     :param borrow_interest_rate: Borrow interest rate per step (only when position < 0 or position > 1). eg: 0.01 corresponds to 1% borrow interest rate per STEP ; if your know that your borrow interest rate is 0.05% per day and that your timestep is 1 hour, you need to divide it by 24 -> 0.05/100/24.
     :type borrow_interest_rate: optional - float
 
     :param portfolio_initial_value: Initial valuation of the portfolio.
     :type portfolio_initial_value: float or int
 
-    :param initial_position: Initial position of the environment. It must contained in the list parameter 'positions'.
+    :param initial_position: You can specify the initial position of the environment or set it to 'random'. It must contained in the list parameter 'positions'.
     :type initial_position: optional - float or int
 
     :param include_position_in_features: Whether or not you want the current position to be added to the step observations. If windows is set an int, it will add the last N-step positions.
     :type include_position_in_features: optional - bool
 
+    :param max_episode_duration: Can be set to an Integer or to 'max'. If a interger value is set, each episode will be truncated after reaching the max amount of steps (by returning `truncated` as `True`) and each episode will start at a random starting point to maximize exploration.
+    :type max_episode_duration: optional - int or 'max'
+
     :param verbose: If 0, no log is outputted. If 1, the env send episode result logs.
     :type verbose: optional - int
     
     :param name: The name of the environment (eg. 'BTC/USDT')
     :type name: optional - str
     
     """
@@ -66,38 +69,38 @@
                 df : pd.DataFrame,
                 positions : list = [0, 1],
                 reward_function = basic_reward_function,
                 windows = None,
                 trading_fees = 0,
                 borrow_interest_rate = 0,
                 portfolio_initial_value = 1000,
-                initial_position = None,
+                initial_position ='random',
                 include_position_in_features = True,
+                max_episode_duration = 'max',
                 verbose = 1,
                 name = "Stock",
                 render_mode= "logs"
                 ):
+        self.max_episode_duration = max_episode_duration
         self.name = name
         self.verbose = verbose
 
         self.positions = positions
         self.reward_function = reward_function
         self.windows = windows
         self.trading_fees = trading_fees
         self.borrow_interest_rate = borrow_interest_rate
         self.portfolio_initial_value = float(portfolio_initial_value)
         self.initial_position = initial_position
-        if self.initial_position is None: self.initial_position = positions[0]
-        assert self.initial_position in self.positions, "The 'initial_position' parameter must one position mentionned in the 'position' (default is [0, 1]) parameter."
+        assert self.initial_position in self.positions or self.initial_position == 'random', "The 'initial_position' parameter must be 'random' or a position mentionned in the 'position' (default is [0, 1]) parameter."
         self.include_position_in_features = include_position_in_features
         assert render_mode is None or render_mode in self.metadata["render_modes"]
         self.render_mode = render_mode
         self._set_df(df)
         
-
         self.action_space = spaces.Discrete(len(positions))
         self.observation_space = spaces.Box(
             -np.inf,
             np.inf,
             shape = [self._nb_features]
         )
         if self.windows is not None:
@@ -111,58 +114,67 @@
 
 
     def _set_df(self, df):
         df = df.copy()
         self._features_columns = [col for col in df.columns if "feature" in col]
         self._info_columns = list(set(list(df.columns) + ["close"]) - set(self._features_columns))
         self._nb_features = len(self._features_columns)
+    
 
         if self.include_position_in_features:
-            df["feature_position"] = self.initial_position
+            df["feature_position"] = 0
             self._features_columns.append("feature_position")
             self._nb_features += 1
         self.df = df
         self._obs_array = np.array(self.df[self._features_columns], dtype= np.float32)
         self._info_array = np.array(self.df[self._info_columns])
         self._price_array = np.array(self.df["close"])
 
+
     
     def _get_ticker(self, delta = 0):
-        return self.df.iloc[self._step + delta]
+        return self.df.iloc[self._step + self._starting_idx + delta]
     def _get_price(self, delta = 0):
-        return self._price_array[self._step + delta]
+        return self._price_array[self._step + self._starting_idx + delta]
     
     def _get_obs(self):
-        if self.include_position_in_features: self._obs_array[self._step, -1] = self._position
+        if self.include_position_in_features: self._obs_array[self._step + self._starting_idx, -1] = self._position
         if self.windows is None:
-            _step_index = self._step
+            _step_index = self._step + self._starting_idx
         else: 
-            _step_index = np.arange(self._step + 1 - self.windows , self._step + 1)
+            _step_index = np.arange(self._step + self._starting_idx + 1 - self.windows , self._step + self._starting_idx + 1)
         return self._obs_array[_step_index]
 
     
     def reset(self, seed = None, options=None):
         super().reset(seed = seed)
         self._step = 0
+        self._position = np.random.choice(self.positions) if self.initial_position == 'random' else self.initial_position
         self._limit_orders = {}
-        if self.windows is not None: self._step = self.windows
+        
+        self._starting_idx = 0
+
+        if self.max_episode_duration != 'max' and len(self.df) - self.max_episode_duration > 0:
+            windows_adjustement = 0 if self.windows is None else self.windows - 1
+            self._starting_idx = np.random.choice(len(self.df)- self.max_episode_duration - windows_adjustement)
+        if self.windows is not None: self._starting_idx += self.windows - 1
 
         self._portfolio  = TargetPortfolio(
-            position=self.initial_position,
-            value= self.portfolio_initial_value,
+            position = self._position,
+            value = self.portfolio_initial_value,
             price = self._get_price()
         )
-        self._position = self.initial_position
+        
         self.historical_info = History(max_size= len(self.df))
         self.historical_info.set(
             step = self._step,
-            date = self.df.index.values[self._step],
-            position_index =self.positions.index(self.initial_position),
+            date = self.df.index.values[self._step + self._starting_idx],
+            position_index =self.positions.index(self._position),
             position = self._position,
-            data =  dict(zip(self._info_columns, self._info_array[self._step])),
+            data =  dict(zip(self._info_columns, self._info_array[self._step + self._starting_idx])),
             portfolio_valuation = self.portfolio_initial_value,
             portfolio_distribution = self._portfolio.get_portfolio_distribution(),
             reward = 0,
         )
 
         return self._get_obs(), self.historical_info[0]
 
@@ -203,34 +215,39 @@
         self._step += 1
 
         self._take_action_order_limit()
         price = self._get_price()
         self._portfolio.update_interest(borrow_interest_rate= self.borrow_interest_rate)
         portfolio_value = self._portfolio.valorisation(price)
         portfolio_distribution = self._portfolio.get_portfolio_distribution()
+
         done, truncated = False, False
         if portfolio_value <= 0: done = True
-        if self._step >= len(self.df) - 1:
+        if self._step + self._starting_idx >= len(self.df) - 1:
             truncated = True
-        
+        if isinstance(self.max_episode_duration,int) and self._step >= self.max_episode_duration - 1:
+            truncated = True
+
         self.historical_info.add(
             step = self._step,
-            date = self.df.index.values[self._step],
+            date = self.df.index.values[self._step + self._starting_idx],
             position_index =position_index,
             position = self._position,
-            data =  dict(zip(self._info_columns, self._info_array[self._step])),
+            data =  dict(zip(self._info_columns, self._info_array[self._step + self._starting_idx])),
             portfolio_valuation = portfolio_value,
             portfolio_distribution = portfolio_distribution, 
             reward = 0
         )
         if not done:
             reward = self.reward_function(self.historical_info)
             self.historical_info["reward", -1] = reward
 
-        if done or truncated: self.log()
+        if done or truncated:
+            self.log()
+
         return self._get_obs(),  self.historical_info["reward", -1], done, truncated, self.historical_info[-1]
     def add_metric(self, name, function):
         self.log_metrics.append({
             'name': name,
             'function': function
         })
     def log(self):
@@ -303,33 +320,48 @@
             env = gym.make(
                     "MultiDatasetTradingEnv",
                     dataset_dir= 'examples/data/*.pkl',
                     preprocess= preprocess,
                 )
     
     :type preprocess: function<pandas.DataFrame->pandas.DataFrame>
+
+    :param episodes_between_dataset_switch: The number of time a dataset will be used for an episode before switching to another dataset. It can be useful for performances when `max_episode_duration` is low.
+    :type episodes_between_dataset_switch: optional - int
+
     """
-    def __init__(self, dataset_dir, *args, preprocess = lambda df : df,**kwargs):
+    def __init__(self,
+                dataset_dir, 
+                *args, 
+
+                preprocess = lambda df : df,
+                episodes_between_dataset_switch = 1,
+                **kwargs):
         self.dataset_dir = dataset_dir
         self.preprocess = preprocess
+        self.episodes_between_dataset_switch = episodes_between_dataset_switch
+
         self.dataset_pathes = glob.glob(self.dataset_dir)
         self.dataset_nb_uses = np.zeros(shape=(len(self.dataset_pathes), ))
         super().__init__(self.next_dataset(), *args, **kwargs)
 
     def next_dataset(self):
+        self._episodes_on_this_dataset = 0
         # Find the indexes of the less explored dataset
         potential_dataset_pathes = np.where(self.dataset_nb_uses == self.dataset_nb_uses.min())[0]
         # Pick one of them
         random_int = np.random.randint(potential_dataset_pathes.size)
         dataset_path = self.dataset_pathes[random_int]
         self.dataset_nb_uses[random_int] += 1 # Update nb use counts
 
         self.name = Path(dataset_path).name
         return self.preprocess(pd.read_pickle(dataset_path))
 
     def reset(self, seed=None):
-        self._set_df(
-            self.next_dataset()
-        )
+        self._episodes_on_this_dataset += 1
+        if self._episodes_on_this_dataset % self.episodes_between_dataset_switch == 0:
+            self._set_df(
+                self.next_dataset()
+            )
         if self.verbose > 1: print(f"Selected dataset {self.name} ...")
         return super().reset(seed)
```

### Comparing `gym-trading-env-0.2.4/src/gym_trading_env/renderer.py` & `gym-trading-env-0.3.0/src/gym_trading_env/renderer.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.2.4/src/gym_trading_env/templates/index.html` & `gym-trading-env-0.3.0/src/gym_trading_env/templates/index.html`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.2.4/src/gym_trading_env/utils/charts.py` & `gym-trading-env-0.3.0/src/gym_trading_env/utils/charts.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.2.4/src/gym_trading_env/utils/history.py` & `gym-trading-env-0.3.0/src/gym_trading_env/utils/history.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.2.4/src/gym_trading_env/utils/portfolio.py` & `gym-trading-env-0.3.0/src/gym_trading_env/utils/portfolio.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.2.4/src/gym_trading_env.egg-info/PKG-INFO` & `gym-trading-env-0.3.0/src/gym_trading_env.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym-trading-env
-Version: 0.2.4
+Version: 0.3.0
 Summary: A simple, easy, customizable Open IA Gym environments for trading.
 Author-email: Clement Perroud <clement.perroud.pro@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -55,15 +55,15 @@
          <img src='https://readthedocs.org/projects/gym-trading-env/badge/?version=latest' alt='Documentation Status' />
    </a>
    <a href="https://github.com/ClementPerroud/Gym-Trading-Env">
       <img src="https://img.shields.io/github/stars/ClementPerroud/gym-trading-env?style=social" alt="Github stars">
    </a>
 </section>
   
-Crypto Trading Env is an OpenAI Gym environment for simulating stocks and training Reinforcement Learning (RL) trading agents.
+Gym Trading Env is an Gymnasium environment for simulating stocks and training Reinforcement Learning (RL) trading agents.
 It was designed to be fast and customizable for easy RL trading algorithms implementation.
 
 
 | [Documentation](https://gym-trading-env.readthedocs.io/en/latest/index.html) |
 
 
 Key features
@@ -77,15 +77,15 @@
 * (Coming soon) An easy way to backtest any RL-Agents or any kind 
 
 ![Render animated image](https://raw.githubusercontent.com/ClementPerroud/Gym-Trading-Env/main/docs/source/images/render.gif)
 
 Installation
 ---------------
 
-Crypto Trading Env supports Python 3.9+ on Windows, Mac, and Linux. You can install it using pip:
+Gym Trading Env supports Python 3.9+ on Windows, Mac, and Linux. You can install it using pip:
 
 ```bash
 pip install gym-trading-env
 ```
 
 Or using git :
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gym-trading-env Version: 0.2.4 Summary: A simple,
+Metadata-Version: 2.1 Name: gym-trading-env Version: 0.3.0 Summary: A simple,
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
-[Github_stars]  Crypto Trading Env is an OpenAI Gym environment for simulating
+[Github_stars]  Gym Trading Env is an Gymnasium environment for simulating
 stocks and training Reinforcement Learning (RL) trading agents. It was designed
 to be fast and customizable for easy RL trading algorithms implementation. |
 [Documentation](https://gym-trading-env.readthedocs.io/en/latest/index.html) |
 Key features --------------- This package aims to greatly simplify the research
 phase by offering : * Easy and quick download technical data on several
 exchanges * A simple and fast environment for the user and the AI, but which
 allows complex operations (Short, Margin trading). * A high performance
 rendering (can display several hundred thousand candles simultaneously),
 customizable to visualize the actions of its agent and its results. * (Coming
 soon) An easy way to backtest any RL-Agents or any kind ![Render animated
 image](https://raw.githubusercontent.com/ClementPerroud/Gym-Trading-Env/main/
-docs/source/images/render.gif) Installation --------------- Crypto Trading Env
+docs/source/images/render.gif) Installation --------------- Gym Trading Env
 supports Python 3.9+ on Windows, Mac, and Linux. You can install it using pip:
 ```bash pip install gym-trading-env ``` Or using git : ```bash git clone https:
 //github.com/ClementPerroud/Gym-Trading-Env ``` [Documentation available here]
 (https://gym-trading-env.readthedocs.io/en/latest/index.html) -----------------
 ------------------------------------------------------------------------------
```

### Comparing `gym-trading-env-0.2.4/src/gym_trading_env.egg-info/SOURCES.txt` & `gym-trading-env-0.3.0/src/gym_trading_env.egg-info/SOURCES.txt`

 * *Files identical despite different names*

