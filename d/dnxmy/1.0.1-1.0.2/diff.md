# Comparing `tmp/dnxmy-1.0.1.tar.gz` & `tmp/dnxmy-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dnxmy-1.0.1.tar", last modified: Tue Apr 18 13:52:55 2023, max compression
+gzip compressed data, was "dnxmy-1.0.2.tar", last modified: Sun May  7 14:18:55 2023, max compression
```

## Comparing `dnxmy-1.0.1.tar` & `dnxmy-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 s11528   (906015332) 1796141739        0 2023-04-18 13:52:55.343425 dnxmy-1.0.1/
--rw-r--r--   0 s11528   (906015332) 1796141739     3037 2023-04-18 13:52:55.343123 dnxmy-1.0.1/PKG-INFO
--rw-r--r--   0 s11528   (906015332) 1796141739     1487 2023-04-18 08:08:38.000000 dnxmy-1.0.1/README.md
-drwxr-xr-x   0 s11528   (906015332) 1796141739        0 2023-04-18 13:52:55.339189 dnxmy-1.0.1/dnxmy/
--rw-r--r--   0 s11528   (906015332) 1796141739      109 2023-04-18 08:08:47.000000 dnxmy-1.0.1/dnxmy/__init__.py
--rw-r--r--   0 s11528   (906015332) 1796141739    11965 2023-04-18 07:46:21.000000 dnxmy-1.0.1/dnxmy/config_generator.py
--rw-r--r--   0 s11528   (906015332) 1796141739     6054 2023-04-04 11:18:12.000000 dnxmy-1.0.1/dnxmy/dnxmy.py
--rw-r--r--   0 s11528   (906015332) 1796141739     7144 2023-04-18 07:17:29.000000 dnxmy-1.0.1/dnxmy/variable_generator.py
-drwxr-xr-x   0 s11528   (906015332) 1796141739        0 2023-04-18 13:52:55.342032 dnxmy-1.0.1/dnxmy.egg-info/
--rw-r--r--   0 s11528   (906015332) 1796141739     3037 2023-04-18 13:52:55.000000 dnxmy-1.0.1/dnxmy.egg-info/PKG-INFO
--rw-r--r--   0 s11528   (906015332) 1796141739      249 2023-04-18 13:52:55.000000 dnxmy-1.0.1/dnxmy.egg-info/SOURCES.txt
--rw-r--r--   0 s11528   (906015332) 1796141739        1 2023-04-18 13:52:55.000000 dnxmy-1.0.1/dnxmy.egg-info/dependency_links.txt
--rw-r--r--   0 s11528   (906015332) 1796141739       28 2023-04-18 13:52:55.000000 dnxmy-1.0.1/dnxmy.egg-info/requires.txt
--rw-r--r--   0 s11528   (906015332) 1796141739        6 2023-04-18 13:52:55.000000 dnxmy-1.0.1/dnxmy.egg-info/top_level.txt
--rw-r--r--   0 s11528   (906015332) 1796141739       38 2023-04-18 13:52:55.343557 dnxmy-1.0.1/setup.cfg
--rw-r--r--   0 s11528   (906015332) 1796141739     1743 2023-04-02 14:55:19.000000 dnxmy-1.0.1/setup.py
+drwxr-xr-x   0 s11528   (906015332) 1796141739        0 2023-05-07 14:18:55.733578 dnxmy-1.0.2/
+-rw-r--r--   0 s11528   (906015332) 1796141739     3037 2023-05-07 14:18:55.733293 dnxmy-1.0.2/PKG-INFO
+-rw-r--r--   0 s11528   (906015332) 1796141739     1487 2023-04-18 08:08:38.000000 dnxmy-1.0.2/README.md
+drwxr-xr-x   0 s11528   (906015332) 1796141739        0 2023-05-07 14:18:55.711181 dnxmy-1.0.2/dnxmy/
+-rw-r--r--   0 s11528   (906015332) 1796141739      109 2023-05-07 13:43:56.000000 dnxmy-1.0.2/dnxmy/__init__.py
+-rw-r--r--   0 s11528   (906015332) 1796141739    11830 2023-05-07 14:12:44.000000 dnxmy-1.0.2/dnxmy/config_generator.py
+-rw-r--r--   0 s11528   (906015332) 1796141739     6007 2023-05-07 13:55:11.000000 dnxmy-1.0.2/dnxmy/dnxmy.py
+-rw-r--r--   0 s11528   (906015332) 1796141739     7144 2023-04-18 07:17:29.000000 dnxmy-1.0.2/dnxmy/variable_generator.py
+drwxr-xr-x   0 s11528   (906015332) 1796141739        0 2023-05-07 14:18:55.732792 dnxmy-1.0.2/dnxmy.egg-info/
+-rw-r--r--   0 s11528   (906015332) 1796141739     3037 2023-05-07 14:18:55.000000 dnxmy-1.0.2/dnxmy.egg-info/PKG-INFO
+-rw-r--r--   0 s11528   (906015332) 1796141739      249 2023-05-07 14:18:55.000000 dnxmy-1.0.2/dnxmy.egg-info/SOURCES.txt
+-rw-r--r--   0 s11528   (906015332) 1796141739        1 2023-05-07 14:18:55.000000 dnxmy-1.0.2/dnxmy.egg-info/dependency_links.txt
+-rw-r--r--   0 s11528   (906015332) 1796141739       28 2023-05-07 14:18:55.000000 dnxmy-1.0.2/dnxmy.egg-info/requires.txt
+-rw-r--r--   0 s11528   (906015332) 1796141739        6 2023-05-07 14:18:55.000000 dnxmy-1.0.2/dnxmy.egg-info/top_level.txt
+-rw-r--r--   0 s11528   (906015332) 1796141739       38 2023-05-07 14:18:55.733691 dnxmy-1.0.2/setup.cfg
+-rw-r--r--   0 s11528   (906015332) 1796141739     1743 2023-04-02 14:55:19.000000 dnxmy-1.0.2/setup.py
```

### Comparing `dnxmy-1.0.1/PKG-INFO` & `dnxmy-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnxmy
-Version: 1.0.1
+Version: 1.0.2
 Summary: dnxmy: dummy data generator for machine learning and statistics
 Home-page: https://github.com/roseiricho/dnxmy
 Author: Yuki Yamamoto
 Author-email: curious.yamamon@gmail.com
 Maintainer: Yuki Yamamoto
 Maintainer-email: curious.yamamon@gmail.com
 License: MIT License
```

### Comparing `dnxmy-1.0.1/README.md` & `dnxmy-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `dnxmy-1.0.1/dnxmy/config_generator.py` & `dnxmy-1.0.2/dnxmy/config_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 
-def generate_default_config(i: int, column_config: dict = None) -> dict:
+def generate_default_config(column_config: dict = None) -> dict:
   """
   Generate a dictionary with default values for column configurations.
 
   Args:
-      i (int): Index of the column.
       column_config (dict, optional): Dictionary containing column configurations.
         Defaults to None.
 
   Returns:
       dict: Dictionary with default values for column configurations.
   """
 
   default_config = {
-    'column_name': f"x_{i}",
     'variable_type': 'independent',
     'probability_distribution': {
       'type': 'uniform',
       'parameter': {
         'low': 0,
         'high': 1
       }
@@ -36,38 +34,37 @@
     Initialize the DnxmyConfig class.
 
     Returns:
         DnxmyConfig: DnxmyConfig class.
     """
 
     # initialize the class attributes
-    self.dataset_config: list = []
-    self.missing_config: list = []
+    self.dataset_config: dict = {}
+    self.missing_config: dict = {}
 
 
   def add_independent_column(self, col_name: str, probability_distribution_type: str = 'uniform', probability_distribution_params: dict = {'low': 0, 'high': 1}):
     """
     Add a column configuration for an independent variable.
 
     Args:
         col_name (str): Name of the column.
         probability_distribution_type (str): Type of the probability distribution.
           Defaults to 'uniform'.
         probability_distribution_params (dict, optional): Parameters of the probability distribution.
           Defaults to {'low': 0, 'high': 1}.
     """
     # create the configuration for the column
-    self.dataset_config.append({
-      'column_name': col_name,
+    self.dataset_config[col_name] = {
       'variable_type': 'independent',
       'probability_distribution': {
         'type': probability_distribution_type,
         'parameter': probability_distribution_params
       }
-    })
+    }
 
 
   def add_categorical_column(self, col_name: str, value: list, probability: list):
     """
     Add a column configuration for a categorical variable.
 
     Args:
@@ -79,64 +76,61 @@
     for i in range(len(value)):
       categories.append({
         'value': value[i],
         'probability': probability[i]
       })
 
     # add a column configuration for the categorical variable
-    self.dataset_config.append({
-      'column_name': col_name,
+    self.dataset_config[col_name] = {
       'variable_type': 'independent',
       'probability_distribution': {
         'type': 'categorical',
         'parameter': {
           'categories': categories
         }
       }
-    })
+    }
 
 
   def add_constant_column(self, col_name: str, constant_value: float = 1):
     """
     Add a column configuration for a constant variable.
 
     Args:
         col_name (str): Name of the column.
         constant_value (float): Value of the constant.
           Defaults to 1.
     """
     # add a column configuration for the constant variable
-    self.dataset_config.append({
-      'column_name': col_name,
+    self.dataset_config[col_name] = {
       'variable_type': 'constant',
       'constant_value': constant_value
-    })
+    }
 
 
   def add_time_part_column(self, col_name: str, start_time: str, time_unit: str, time_format: str = '%Y-%m-%d'):
     """
     Add a column configuration for a time part variable.
 
     Args:
         col_name (str): Name of the column.
         start_time (str): Start time of the time variable.
         time_unit (str): Time unit of the time variable.
         time_format (str): Time format of the time variable.
           Defaults to '%Y-%m-%d'.
     """
     # add a column configuration for the time variable
-    self.dataset_config.append({
-      'column_name': col_name,
+    self.dataset_config[col_name] = {
       'variable_type': 'time_part',
       'time_part_config': {
         'start_time': start_time,
         'time_unit': time_unit,
         'time_format': time_format
       }
-    })
+    }
 
 
   def add_arma_column(self, 
                       col_name:str, 
                       intercept: float = 0, 
                       sigma: float = 0, 
                       ar_initial: float = None, 
@@ -194,16 +188,15 @@
     if ma_shock_time is not None or ma_shock_type is not None or ma_shock_value is not None:
       for i, t, v in zip(ma_shock_time, ma_shock_type, ma_shock_value):
         ma_shock_dict[i] = {}
         ma_shock_dict[i]['type'] = t
         ma_shock_dict[i]['value'] = v
 
     # create the column configuration dictionary
-    self.dataset_config.append({
-      'column_name': col_name,
+    self.dataset_config[col_name] = {
       'variable_type': 'time_series',
       'time_series_config': {
         'intercept': intercept,
         'sigma': sigma,
         'ar_params': {
           'initial': ar_initial,
           'order': ar_order,
@@ -213,15 +206,15 @@
         'ma_params': {
           'initial': ma_initial,
           'order': ma_order,
           'params': ma_params,
           'shock': ma_shock_dict
         }
       }
-    })
+    }
 
 
   def add_dependent_column(self, 
                           col_name: str, 
                           variables: list, 
                           beta: list, 
                           intercept: float, 
@@ -240,54 +233,50 @@
           Defaults to None.
         offset_function (str): Function to use for the offset.
           Defaults to 'default'.
         link_function (str): Link function to use for the dependent variable.
           Defaults to 'identity'.
     """
     # add a column configuration for the dependent variable
-    self.dataset_config.append({
-      'column_name': col_name,
+    self.dataset_config[col_name] = {
       'variable_type': 'dependent',
       'dependent_on': {
         'variables': variables,
         'beta': beta,
         'intercept': intercept,
         'offset': {
           'column_name': offset_column,
           'function': offset_function
         },
         'link_function': link_function
       }
-    })
+    }
   
   
   def delete_column_config(self, col_name: str):
     """
     Delete a column configuration.
 
     Args:
         col_name (str): Name of the column.
     """
-    for col in self.dataset_config:
-      if col['column_name'] == col_name:
-        self.dataset_config.remove(col)
-        break
+    del self.dataset_config[col_name]
 
 
   def t_sort(self):
     """
     Optimize the order of dataset configuration using topological sorting.
     """
     sorted_list = []
     dependency_dict = {}
     column_dict = {}
 
     # create a dictionary of dependencies
-    for col in self.dataset_config:
-      col_name = col['column_name']
+    for col_name in self.dataset_config:
+      col = self.dataset_config[col_name]
       if col['variable_type'] == 'dependent':
         dependency_dict[col_name] = col['dependent_on']['variables'].copy()
         if col['dependent_on'].get('offset')['column_name'] is not None:
           dependency_dict[col_name].append(col['dependent_on']['offset']['column_name'])
       else:
         dependency_dict[col_name] = []
 
@@ -302,31 +291,38 @@
       sorted_list.extend(independent_cols)
       for col in independent_cols:
         del dependency_dict[col]
         for dep_cols in dependency_dict.values():
           for dep_col in dep_cols:
             if col == dep_col:
               dep_cols.remove(col)
-
-    column_dict = {col['column_name']: col for col in self.dataset_config}
-    self.dataset_config = [column_dict[col] for col in sorted_list if col in column_dict]
+              
+    column_dict = {col_name: self.dataset_config[col_name] for col_name in sorted_list}
+    
+    self.dataset_config = column_dict
 
 
   def set_dataset_config(self, m: int):
     """
     Set dataset configurations based on the provided configurations or the default configurations.
     """
-    for i in range(m):
-      if i < len(self.dataset_config):
-        column_config = self.dataset_config[i]
+    col_names = list(self.dataset_config.keys())
+    if len(self.dataset_config) <= m:
+      for i in range(m - len(self.dataset_config)):
+        if 'col_' + str(i) in col_names:
+          i += 1
+        col_names.append('col_' + str(i))
+    
+    for col_name in col_names:
+      if self.dataset_config.get(col_name) is not None:
+        column_config = self.dataset_config[col_name]
       else:
         column_config = None
-        self.dataset_config.append(column_config)
-
-      self.dataset_config[i] = generate_default_config(i, column_config)
+      
+      self.dataset_config[col_name] = generate_default_config(column_config)
 
 
   def add_missing_config(self, target_col_name: str, missing_type: str = 'MCAR', missing_rate: float = None, dependent_on: str = None):
     """
     Generate a missing configuration dictionary.
 
     Args:
@@ -341,15 +337,14 @@
     Returns:
         dict: Dictionary of missing configurations.
     """
     if missing_type not in ['MCAR', 'MAR', 'MNAR']:
       raise ValueError("Missing type must be one of 'MCAR', 'MAR', or 'MNAR'!")
     
     # add a missing configuration
-    self.missing_config.append({
+    self.missing_config[target_col_name] = {
       'missing_type': missing_type,
-      'target_column_name': target_col_name,
       'missing_params': {
         'missing_rate': missing_rate,
         'dependent_on': dependent_on
       }
-    })
+    }
```

### Comparing `dnxmy-1.0.1/dnxmy/dnxmy.py` & `dnxmy-1.0.2/dnxmy/dnxmy.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,31 +43,30 @@
     if self.m < len(self.dnxmy_config.dataset_config):
       self.m = len(self.dnxmy_config.dataset_config)
 
     # set the column configurations
     self.dnxmy_config.set_dataset_config(self.m)
     self.dnxmy_config.t_sort()
     self.dataset_config = self.dnxmy_config.dataset_config
-
-    column_names = [column_config['column_name'] for column_config in self.dataset_config]
     
     # generate the data
     self.df = pd.DataFrame()
 
-    for column_config in self.dataset_config:
+    for column_name in self.dataset_config.keys():
+      column_config = self.dataset_config[column_name]
       if column_config['variable_type'] == 'independent':
-        self.df = pd.concat([self.df, generate_random_samples(column_config['column_name'], column_config['probability_distribution'], self.n)], axis=1)
+        self.df = pd.concat([self.df, generate_random_samples(column_name, column_config['probability_distribution'], self.n)], axis=1)
       elif column_config['variable_type'] == 'constant':
-        self.df = pd.concat([self.df, pd.Series([column_config['constant_value']] * self.n, name=column_config['column_name'])], axis=1)
+        self.df = pd.concat([self.df, pd.Series([column_config['constant_value']] * self.n, name = column_name)], axis=1)
       elif column_config['variable_type'] == 'time_part':
-        self.df = pd.concat([self.df, generate_time_part(column_config['column_name'], column_config['time_part_config'], self.n)], axis=1)
+        self.df = pd.concat([self.df, generate_time_part(column_name, column_config['time_part_config'], self.n)], axis=1)
       elif column_config['variable_type'] == 'time_series':
-        self.df = pd.concat([self.df, generate_arma_samples(column_config['column_name'], column_config['time_series_config'], self.n)], axis=1)
+        self.df = pd.concat([self.df, generate_arma_samples(column_name, column_config['time_series_config'], self.n)], axis=1)
       elif column_config['variable_type'] == 'dependent':
-        self.df = pd.concat([self.df, generate_dependent_samples(column_config['column_name'], self.dataset_config, self.df, column_config['dependent_on'], self.n)], axis=1)
+        self.df = pd.concat([self.df, generate_dependent_samples(column_name, self.dataset_config, self.df, column_config['dependent_on'], self.n)], axis=1)
 
     return self.df
 
 
   def add_samples(self, n: int) -> pd.DataFrame:
     """
     Add samples to the generated data.
@@ -79,25 +78,26 @@
         pd.DataFrame: DataFrame containing the generated data with added samples.
     """
     if self.df is None:
       raise Exception('Data has not been generated yet')
 
     self.df_add = pd.DataFrame()
 
-    for column_config in self.dataset_config:
+    for column_name in self.dataset_config.keys():
+      column_config = self.dataset_config[column_name]
       if column_config['variable_type'] == 'independent':
-        self.df_add = pd.concat([self.df_add, generate_random_samples(column_config['column_name'], column_config['probability_distribution'], n)], axis=1)
+        self.df_add = pd.concat([self.df_add, generate_random_samples(column_name, column_config['probability_distribution'], n)], axis=1)
       elif column_config['variable_type'] == 'constant':
-        self.df_add = pd.concat([self.df_add, pd.Series([column_config['constant_value']] * n, name=column_config['column_name'])], axis=1)
+        self.df_add = pd.concat([self.df_add, pd.Series([column_config['constant_value']] * n, name = column_name)], axis=1)
       elif column_config['variable_type'] == 'time_part':
-        self.df_add = pd.concat([self.df_add, generate_time_part(column_config['column_name'], column_config['time_part_config'], n)], axis=1)
+        self.df_add = pd.concat([self.df_add, generate_time_part(column_name, column_config['time_part_config'], n)], axis=1)
       elif column_config['variable_type'] == 'time_series':
-        self.df_add = pd.concat([self.df_add, generate_arma_samples(column_config['column_name'], column_config['time_series_config'], n)], axis=1)
+        self.df_add = pd.concat([self.df_add, generate_arma_samples(column_name, column_config['time_series_config'], n)], axis=1)
       elif column_config['variable_type'] == 'dependent':
-        self.df_add = pd.concat([self.df_add, generate_dependent_samples(column_config['column_name'], self.dataset_config, self.df_add, column_config['dependent_on'], n)], axis=1)
+        self.df_add = pd.concat([self.df_add, generate_dependent_samples(column_name, self.dataset_config, self.df_add, column_config['dependent_on'], n)], axis=1)
 
     # add the new samples to the existing data
     self.df = pd.concat([self.df, self.df_add], ignore_index=True)
     
     # update the number of samples
     self.n += n
 
@@ -116,17 +116,20 @@
     # set the seed
     if self.seed is not None:
       np.random.seed(self.seed)
     
     # set the missing configurations
     self.missing_config = self.dnxmy_config.missing_config
     
-    for missing_column_config in self.missing_config:
+    missing_column_names = self.missing_config.keys()
+
+    for missing_column_name in missing_column_names:
+      missing_column_config = self.missing_config[missing_column_name]
       missing_type = missing_column_config.get('missing_type', None)
-      target_column_name = missing_column_config.get('target_column_name', None)
+      target_column_name = missing_column_name
       missing_rate = missing_column_config.get('missing_params', {}).get('missing_rate', None)
       dependent_on = missing_column_config.get('missing_params', {}).get('dependent_on', None)
 
       # missing
       if missing_type == 'MCAR':
         missing_index = np.random.choice(self.n, int(self.n * missing_rate), replace=False)
         df_missing.loc[missing_index, target_column_name] = np.nan
```

### Comparing `dnxmy-1.0.1/dnxmy/variable_generator.py` & `dnxmy-1.0.2/dnxmy/variable_generator.py`

 * *Files identical despite different names*

### Comparing `dnxmy-1.0.1/dnxmy.egg-info/PKG-INFO` & `dnxmy-1.0.2/dnxmy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnxmy
-Version: 1.0.1
+Version: 1.0.2
 Summary: dnxmy: dummy data generator for machine learning and statistics
 Home-page: https://github.com/roseiricho/dnxmy
 Author: Yuki Yamamoto
 Author-email: curious.yamamon@gmail.com
 Maintainer: Yuki Yamamoto
 Maintainer-email: curious.yamamon@gmail.com
 License: MIT License
```

### Comparing `dnxmy-1.0.1/setup.py` & `dnxmy-1.0.2/setup.py`

 * *Files identical despite different names*

