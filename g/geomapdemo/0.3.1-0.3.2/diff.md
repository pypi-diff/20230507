# Comparing `tmp/geomapdemo-0.3.1.tar.gz` & `tmp/geomapdemo-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geomapdemo-0.3.1.tar", last modified: Sun Apr 30 03:43:43 2023, max compression
+gzip compressed data, was "geomapdemo-0.3.2.tar", last modified: Sun May  7 19:17:29 2023, max compression
```

## Comparing `geomapdemo-0.3.1.tar` & `geomapdemo-0.3.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 03:43:43.130481 geomapdemo-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-30 03:43:28.000000 geomapdemo-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-30 03:43:28.000000 geomapdemo-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-30 03:43:43.130481 geomapdemo-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-30 03:43:28.000000 geomapdemo-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 03:43:43.130481 geomapdemo-0.3.1/geomapdemo/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 03:43:28.000000 geomapdemo-0.3.1/geomapdemo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-04-30 03:43:28.000000 geomapdemo-0.3.1/geomapdemo/chart.py
--rw-r--r--   0 runner    (1001) docker     (123)     8555 2023-04-30 03:43:28.000000 geomapdemo-0.3.1/geomapdemo/foliumap.py
--rw-r--r--   0 runner    (1001) docker     (123)    12397 2023-04-30 03:43:28.000000 geomapdemo-0.3.1/geomapdemo/geomapdemo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 03:43:43.130481 geomapdemo-0.3.1/geomapdemo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-30 03:43:43.000000 geomapdemo-0.3.1/geomapdemo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-30 03:43:43.000000 geomapdemo-0.3.1/geomapdemo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-30 03:43:43.000000 geomapdemo-0.3.1/geomapdemo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 03:43:43.000000 geomapdemo-0.3.1/geomapdemo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-30 03:43:43.000000 geomapdemo-0.3.1/geomapdemo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-30 03:43:43.000000 geomapdemo-0.3.1/geomapdemo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-30 03:43:28.000000 geomapdemo-0.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-30 03:43:43.130481 geomapdemo-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-04-30 03:43:28.000000 geomapdemo-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:17:29.477797 geomapdemo-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-07 19:17:19.000000 geomapdemo-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-07 19:17:19.000000 geomapdemo-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-05-07 19:17:29.477797 geomapdemo-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-07 19:17:19.000000 geomapdemo-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:17:29.473797 geomapdemo-0.3.2/geomapdemo/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-07 19:17:19.000000 geomapdemo-0.3.2/geomapdemo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-05-07 19:17:19.000000 geomapdemo-0.3.2/geomapdemo/chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8555 2023-05-07 19:17:19.000000 geomapdemo-0.3.2/geomapdemo/foliumap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15629 2023-05-07 19:17:19.000000 geomapdemo-0.3.2/geomapdemo/geomapdemo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:17:29.477797 geomapdemo-0.3.2/geomapdemo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-05-07 19:17:29.000000 geomapdemo-0.3.2/geomapdemo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-07 19:17:29.000000 geomapdemo-0.3.2/geomapdemo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-07 19:17:29.000000 geomapdemo-0.3.2/geomapdemo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 19:17:29.000000 geomapdemo-0.3.2/geomapdemo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-07 19:17:29.000000 geomapdemo-0.3.2/geomapdemo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-07 19:17:29.000000 geomapdemo-0.3.2/geomapdemo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-07 19:17:19.000000 geomapdemo-0.3.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-07 19:17:29.477797 geomapdemo-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-07 19:17:19.000000 geomapdemo-0.3.2/setup.py
```

### Comparing `geomapdemo-0.3.1/LICENSE` & `geomapdemo-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `geomapdemo-0.3.1/PKG-INFO` & `geomapdemo-0.3.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomapdemo
-Version: 0.3.1
+Version: 0.3.2
 Summary: A python package for interactive mapping.
 Home-page: https://github.com/zyang91/geomapdemo
 Author: Zhanchao Yang
 Author-email: zyang91@binghamton.edu
 License: MIT license
 Keywords: geomapdemo
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -43,20 +43,17 @@
 ## Features
 
 -   Create random numbers and random text
 -   Basic Mapping and drawing
 -   Vector and raster layer function available
 -   Ipyleaflet based interactive map function
 -   Folium based interactive map function
+-   Chart module for interactive chart making
 
 
 ## Supported Python Version
 - Python 3
 - Python 3.7
 - Python 3.8
 - Python 3.9
 - Python 3.10
 - Python 3.11
-
-
-
-
```

### Comparing `geomapdemo-0.3.1/README.md` & `geomapdemo-0.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -20,20 +20,17 @@
 ## Features
 
 -   Create random numbers and random text
 -   Basic Mapping and drawing
 -   Vector and raster layer function available
 -   Ipyleaflet based interactive map function
 -   Folium based interactive map function
+-   Chart module for interactive chart making
 
 
 ## Supported Python Version
 - Python 3
 - Python 3.7
 - Python 3.8
 - Python 3.9
 - Python 3.10
 - Python 3.11
-
-
-
-
```

### Comparing `geomapdemo-0.3.1/geomapdemo/chart.py` & `geomapdemo-0.3.2/geomapdemo/chart.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,14 @@
+'''Chart module for creating interactive chart.'''
+ 
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 import seaborn as sns
 
-'''Since many of the GIS spatial analysis involve the use of charts,
- I recommend the chart section in geomapdemo package, 
- which based on the seaborn to make people convenient to generate the charts.'''
-
-
 def set_default_theme(style='darkgrid', **kwargs):
     '''Set the aesthetic style of the plots.
     Args:
         style (str): darkgrid, darkgrid, dark, white, ticks
         kwargs: Additional parameters to control the aesthetics of the grid.'''
     sns.set_theme(style=style, **kwargs)
 
@@ -67,9 +64,34 @@
     '''
     if isinstance(data, str):
         df = pd.read_csv(data)
     else:
         df = data
     sns.violinplot(x=df[variable], **kwargs)
 
+def box_plot(data, x, y, hue= None, **kwargs):
+    '''Plot data and regression model fits across a FacetGrid.
+    Args:
+        data (DataFrame): CSV file path or DataFrame object.
+        x, y (str): Variables that specify positions on the x and y axes.
+        hue (str): Variable in data to map plot aspects to different colors.
+        kwargs: Additional keyword arguments are passed to the function used to draw the plot on the joint Axes, superseding items in the joint_kws dictionary.
+    '''
+    if isinstance(data, str):
+        df = pd.read_csv(data)
+    else:
+        df = data
+    sns.boxplot(data=df, x=x, y=y, hue=hue, **kwargs)
 
+def single_box_plot(data, variable, **kwargs):
+    '''Plot data and regression model fits across a FacetGrid.
+    Aegs:
+        data (DataFrame): CSV file path or DataFrame object.
+        variable (str): Variables that specify positions on the x and y axes.
+        kwargs: Additional keyword arguments are passed to the function used to draw the plot on the joint Axes, superseding items in the joint_kws dictionary.
+    '''
+    if isinstance(data, str):
+        df = pd.read_csv(data)
+    else:
+        df = data
+    sns.boxplot(data=df,x=df[variable], **kwargs)
```

### Comparing `geomapdemo-0.3.1/geomapdemo/foliumap.py` & `geomapdemo-0.3.2/geomapdemo/foliumap.py`

 * *Files identical despite different names*

### Comparing `geomapdemo-0.3.1/geomapdemo/geomapdemo.py` & `geomapdemo-0.3.2/geomapdemo/geomapdemo.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Main module."""
 
 import random
 import string
 import ipyleaflet
+import ipywidgets as widgets
 
 
 
 
 class Map(ipyleaflet.Map):
 
     def __init__(self, center = [40, -100], zoom = 4, **kwargs) -> None:
@@ -113,18 +114,18 @@
         Args:
             position (str, optional): The position of the layers control. Defaults to "topright".
             **kwargs: Keyword arguments to be passed to the layers control.
         """        
         layers_control = ipyleaflet.LayersControl(position=position, **kwargs)
         self.add_control(layers_control)
     
-    def add_fullscreen_control(self, position ="topright", **kwargs):
+    def add_fullscreen_control(self, position ="topleft", **kwargs):
         """Adds a fullscreen control to the map
         Args:
-            position (str, optional): The position of the fullscreen control. Defaults to "topright".
+            position (str, optional): The position of the fullscreen control. Defaults to "topleft".
             **kwargs: Keyword arguments to be passed to the fullscreen control.
         """        
         fullscreen_control = ipyleaflet.FullScreenControl(position=position, **kwargs)
         self.add_control(fullscreen_control)
     
     def add_search_control(self, position ="topleft", **kwargs):
         """Adds a search control to the map
@@ -289,14 +290,94 @@
         try:
             from localtileserver import get_leaflet_tile_layer, TileClient
             client = TileClient(filepath)
             tile_layer = get_leaflet_tile_layer(client)
             self.add_layer(tile_layer, **kwargs)
         except:
             raise ImportError("Please install localtileserver")
+    
+    def add_opacity_control(self, value, min, max, **kwargs):
+        """Adds an opacity control to the map
+        Args:
+            value (float): The initial value of the opacity control.
+            min (float): The minimum value of the opacity control.
+            max (float): The maximum value of the opacity control.
+            **kwargs: Keyword arguments to be passed to the opacity control.
+        """ 
+        slider = widgets.FloatSlider(value=value, min=min, max=max, **kwargs)
+        widgets.jslink((slider, 'value'), (self.layers[-1], 'opacity'))
+        control = ipyleaflet.WidgetControl(widget=slider, position='bottomright')
+        self.add_control(control)
+    
+    def add_custom_html(self, html, position='bottomright'):
+        """Adds custom HTML to the map
+        Args:
+            html (str): The HTML string.
+            position (str, optional): The position of the HTML. Defaults to 'bottomright'.
+        """ 
+        from ipyleaflet import WidgetControl
+        control = WidgetControl(widget=widgets.HTML(html), position=position)
+        self.add_control(control)
+    
+    def add_logo(self, url, width = 100, height=100,  position='bottomright'):
+        """Adds a logo to the map
+        Args:
+            url (str): The url of the logo.
+            width (int, optional): The width of the logo. Defaults to 100.
+            height (int, optional): The height of the logo. Defaults to 100.
+            position (str, optional): The position of the logo. Defaults to 'bottomright'.
+        """ 
+        from ipyleaflet import WidgetControl
+        logo = widgets.HTML(f'<img src="{url}" alt="Logo" width="{width}" height="{height}">')
+        control = WidgetControl(widget=logo, position=position)
+        self.add_control(control)
+
+
+    def add_toolbar(self, position='topright', widget_width='250px'):
+        '''adds a toolbar to the map'''
+        from ipyleaflet import WidgetControl
+        padding= '0px 0px 0px 4px'
+        
+        toolbar_button=widgets.ToggleButton(
+            value=False,
+            tooltip='Toolbar',
+            icon='wrench',
+            button_style='primary',
+            layout=widgets.Layout(width='28px', height='28px', padding= padding),
+        )
+        
+        close_button=widgets.ToggleButton(
+            value=False,
+            tooltip='Close',
+            icon='times',
+            button_style='warning',
+            layout=widgets.Layout(width='28px', height='28px', padding= padding),
+        )
+        
+        int_slider = widgets.IntSlider(
+            value= 4,
+            min=1,
+            max=24,
+            description="Zoom level: ",
+            readout=True,
+            continuous_update=True,
+            layout=widgets.Layout(width=widget_width, padding=padding),
+            style={"description_width": "initial"},
+        )
+        widgets.jslink((self, 'zoom'), (int_slider, 'value'))
+        toolbar_widget = widgets.VBox()
+        toolbar_widget.children = [
+            widgets.HBox([close_button, toolbar_button]),
+            int_slider,
+        ]       
+        toolbar_control = WidgetControl(widget=toolbar_widget, position= position)
+        self.add_control(toolbar_control)
+
+
+
 
 
 def generate_random_string(length=10, upper=False, punctuations=False, digits=False):
     """Generates a random string of fixed length
 
     Args:
         length (int, optional): The length of the string. Defaults to 10.
```

### Comparing `geomapdemo-0.3.1/geomapdemo.egg-info/PKG-INFO` & `geomapdemo-0.3.2/geomapdemo.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomapdemo
-Version: 0.3.1
+Version: 0.3.2
 Summary: A python package for interactive mapping.
 Home-page: https://github.com/zyang91/geomapdemo
 Author: Zhanchao Yang
 Author-email: zyang91@binghamton.edu
 License: MIT license
 Keywords: geomapdemo
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -43,20 +43,17 @@
 ## Features
 
 -   Create random numbers and random text
 -   Basic Mapping and drawing
 -   Vector and raster layer function available
 -   Ipyleaflet based interactive map function
 -   Folium based interactive map function
+-   Chart module for interactive chart making
 
 
 ## Supported Python Version
 - Python 3
 - Python 3.7
 - Python 3.8
 - Python 3.9
 - Python 3.10
 - Python 3.11
-
-
-
-
```

### Comparing `geomapdemo-0.3.1/setup.py` & `geomapdemo-0.3.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,10 +50,10 @@
     keywords='geomapdemo',
     name='geomapdemo',
     packages=find_packages(include=['geomapdemo', 'geomapdemo.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/zyang91/geomapdemo',
-    version='0.3.1',
+    version='0.3.2',
     zip_safe=False,
 )
```

