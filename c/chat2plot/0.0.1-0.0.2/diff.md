# Comparing `tmp/chat2plot-0.0.1.tar.gz` & `tmp/chat2plot-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chat2plot-0.0.1.tar", last modified: Sat May  6 01:33:50 2023, max compression
+gzip compressed data, was "chat2plot-0.0.2.tar", last modified: Sun May  7 15:17:36 2023, max compression
```

## Comparing `chat2plot-0.0.1.tar` & `chat2plot-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 nyanp     (1000) nyanp     (1000)        0 2023-05-06 01:33:50.110329 chat2plot-0.0.1/
--rw-r--r--   0 nyanp     (1000) nyanp     (1000)     1062 2023-05-05 05:43:03.000000 chat2plot-0.0.1/LICENSE
--rw-r--r--   0 nyanp     (1000) nyanp     (1000)       24 2023-05-06 01:18:21.000000 chat2plot-0.0.1/MANIFEST.in
--rw-r--r--   0 nyanp     (1000) nyanp     (1000)      950 2023-05-06 01:33:50.110329 chat2plot-0.0.1/PKG-INFO
--rw-r--r--   0 nyanp     (1000) nyanp     (1000)      494 2023-05-06 01:31:12.000000 chat2plot-0.0.1/README.md
-drwxr-xr-x   0 nyanp     (1000) nyanp     (1000)        0 2023-05-06 01:33:50.110329 chat2plot-0.0.1/chat2plot/
--rw-r--r--   0 nyanp     (1000) nyanp     (1000)       50 2023-05-05 17:20:36.000000 chat2plot-0.0.1/chat2plot/__init__.py
--rw-r--r--   0 nyanp     (1000) nyanp     (1000)     5648 2023-05-06 01:28:24.000000 chat2plot-0.0.1/chat2plot/chat2plot.py
--rw-r--r--   0 nyanp     (1000) nyanp     (1000)      104 2023-05-05 06:03:09.000000 chat2plot-0.0.1/chat2plot/dataset_description.py
--rw-r--r--   0 nyanp     (1000) nyanp     (1000)     3873 2023-05-05 17:46:25.000000 chat2plot-0.0.1/chat2plot/render.py
--rw-r--r--   0 nyanp     (1000) nyanp     (1000)     3177 2023-05-05 17:35:57.000000 chat2plot-0.0.1/chat2plot/schema.py
--rw-r--r--   0 nyanp     (1000) nyanp     (1000)     1555 2023-05-05 17:37:56.000000 chat2plot-0.0.1/chat2plot/transform.py
--rw-r--r--   0 nyanp     (1000) nyanp     (1000)       22 2023-05-06 01:14:28.000000 chat2plot-0.0.1/chat2plot/version.py
-drwxr-xr-x   0 nyanp     (1000) nyanp     (1000)        0 2023-05-06 01:33:50.110329 chat2plot-0.0.1/chat2plot.egg-info/
--rw-r--r--   0 nyanp     (1000) nyanp     (1000)      950 2023-05-06 01:33:50.000000 chat2plot-0.0.1/chat2plot.egg-info/PKG-INFO
--rw-r--r--   0 nyanp     (1000) nyanp     (1000)      406 2023-05-06 01:33:50.000000 chat2plot-0.0.1/chat2plot.egg-info/SOURCES.txt
--rw-r--r--   0 nyanp     (1000) nyanp     (1000)        1 2023-05-06 01:33:50.000000 chat2plot-0.0.1/chat2plot.egg-info/dependency_links.txt
--rw-r--r--   0 nyanp     (1000) nyanp     (1000)       71 2023-05-06 01:33:50.000000 chat2plot-0.0.1/chat2plot.egg-info/requires.txt
--rw-r--r--   0 nyanp     (1000) nyanp     (1000)       10 2023-05-06 01:33:50.000000 chat2plot-0.0.1/chat2plot.egg-info/top_level.txt
--rw-r--r--   0 nyanp     (1000) nyanp     (1000)      289 2023-05-05 06:05:57.000000 chat2plot-0.0.1/pyproject.toml
--rw-r--r--   0 nyanp     (1000) nyanp     (1000)       71 2023-05-05 18:06:35.000000 chat2plot-0.0.1/requirements.txt
--rw-r--r--   0 nyanp     (1000) nyanp     (1000)      710 2023-05-06 01:33:50.110329 chat2plot-0.0.1/setup.cfg
--rw-r--r--   0 nyanp     (1000) nyanp     (1000)     1302 2023-05-06 01:16:57.000000 chat2plot-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:17:36.426111 chat2plot-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-07 15:17:25.000000 chat2plot-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-07 15:17:25.000000 chat2plot-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-07 15:17:36.426111 chat2plot-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-07 15:17:25.000000 chat2plot-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:17:36.426111 chat2plot-0.0.2/chat2plot/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-07 15:17:25.000000 chat2plot-0.0.2/chat2plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9223 2023-05-07 15:17:25.000000 chat2plot-0.0.2/chat2plot/chat2plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-07 15:17:25.000000 chat2plot-0.0.2/chat2plot/dataset_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-05-07 15:17:25.000000 chat2plot-0.0.2/chat2plot/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-05-07 15:17:25.000000 chat2plot-0.0.2/chat2plot/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-07 15:17:25.000000 chat2plot-0.0.2/chat2plot/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-07 15:17:25.000000 chat2plot-0.0.2/chat2plot/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:17:36.426111 chat2plot-0.0.2/chat2plot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-07 15:17:36.000000 chat2plot-0.0.2/chat2plot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-07 15:17:36.000000 chat2plot-0.0.2/chat2plot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 15:17:36.000000 chat2plot-0.0.2/chat2plot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-07 15:17:36.000000 chat2plot-0.0.2/chat2plot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-07 15:17:36.000000 chat2plot-0.0.2/chat2plot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-07 15:17:25.000000 chat2plot-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-07 15:17:25.000000 chat2plot-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-07 15:17:36.426111 chat2plot-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-07 15:17:25.000000 chat2plot-0.0.2/setup.py
```

### Comparing `chat2plot-0.0.1/LICENSE` & `chat2plot-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chat2plot-0.0.1/chat2plot/render.py` & `chat2plot-0.0.2/chat2plot/render.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,43 @@
+import copy
+from typing import Any
+
+import altair as alt
 import pandas as pd
 import plotly.express as px
+from altair.utils.data import to_values
 from plotly.graph_objs import Figure
 
-from chat2plot.schema import AggregationType, AxisOrder, ChartType, Filter, PlotConfig
+from chat2plot.schema import (
+    AggregationType,
+    ChartType,
+    Filter,
+    PlotConfig,
+    SortingCriteria,
+    SortOrder,
+)
 from chat2plot.transform import transform
 
 
 def _ax_config(config: PlotConfig, x: str, y: str) -> dict[str, str | dict[str, str]]:
-    ax = {"x": x, "y": y}
-    labels = {}
+    ax: dict[str, str | dict[str, str]] = {"x": x, "y": y}
+    labels: dict[str, str] = {}
 
     if config.xlabel:
         labels[x] = config.xlabel
     if config.ylabel:
         labels[y] = config.ylabel
 
     if labels:
         ax["labels"] = labels
 
     return ax
 
 
-def draw_plotly(df: pd.DataFrame, config: PlotConfig) -> Figure:
+def draw_plotly(df: pd.DataFrame, config: PlotConfig, show: bool = True) -> Figure:
     df_filtered = filter_data(df, config.filters).copy()
     df_filtered = transform(df, config)
 
     chart_type = config.chart_type
 
     if chart_type in [ChartType.BAR, ChartType.HORIZONTAL_BAR]:
         agg = groupby_agg(df_filtered, config)
@@ -68,17 +80,32 @@
                 **_ax_config(
                     config, config.dimension.column, config.measures[0].column
                 ),
             )
     else:
         raise ValueError(f"Unknown chart_type: {chart_type}")
 
+    if show:
+        fig.show()
+
     return fig
 
 
+def draw_altair(
+    df: pd.DataFrame, config: dict[str, Any], show: bool = True
+) -> alt.Chart:
+    spec = copy.deepcopy(config)
+    spec["data"] = to_values(df)
+    chart = alt.Chart.from_dict(spec)
+    if show:
+        chart.show()
+
+    return chart
+
+
 def groupby_agg(df: pd.DataFrame, config: PlotConfig) -> pd.DataFrame:
     assert len(config.measures) == 1
 
     group_by = [config.dimension.column] if config.dimension is not None else []
 
     if config.hue and config.hue != config.dimension:
         group_by.append(config.hue.column)
@@ -101,18 +128,20 @@
         )
     else:
         agg = (
             df.groupby(group_by, dropna=False)[m.column]
             .agg(agg_method[m.aggregation_method])
             .rename(str(m))
         )
-        if config.order_by == AxisOrder.NAME:
-            agg = agg.sort_index()
-        elif config.order_by == AxisOrder.VALUE:
-            agg = agg.sort_values(ascending=False)
+        ascending = config.sort_order == SortOrder.ASC
+
+        if config.sort_criteria == SortingCriteria.NAME:
+            agg = agg.sort_index(ascending=ascending)
+        elif config.sort_criteria == SortingCriteria.VALUE:
+            agg = agg.sort_values(ascending=ascending)
 
         return agg.reset_index()
 
 
 def is_aggregation(config: PlotConfig) -> bool:
     return (
         len(config.measures) == 1 and config.measures[0].aggregation_method is not None
```

### Comparing `chat2plot-0.0.1/chat2plot/schema.py` & `chat2plot-0.0.2/chat2plot/schema.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,24 +19,30 @@
     MIN = "MIN"
     MAX = "MAX"
     COUNT = "COUNT"
     DISTINCT_COUNT = "DISTINCT_COUNT"
 
 
 class ResponseType(Enum):
-    CHART = "chart"
+    SUCCESS = "success"
     NOT_RELATED = "not related"
     UNKNOWN = "unknown"
+    FAILED_TO_RENDER = "failed to render"
 
 
-class AxisOrder(Enum):
+class SortingCriteria(Enum):
     NAME = "name"
     VALUE = "value"
 
 
+class SortOrder(Enum):
+    ASC = "asc"
+    DESC = "desc"
+
+
 @dataclass(frozen=True)
 class Measure:
     column: str
     aggregation_method: AggregationType | None = None
 
     @classmethod
     def from_text(cls, text: str) -> "Measure":
@@ -73,15 +79,16 @@
     hue: Dimension | None = None
     xmin: float | None = None
     xmax: float | None = None
     ymin: float | None = None
     ymax: float | None = None
     xlabel: str | None = None
     ylabel: str | None = None
-    order_by: AxisOrder | None = None
+    sort_criteria: SortingCriteria | None = None
+    sort_order: SortOrder | None = None
 
     @property
     def required_columns(self) -> list[str]:
         columns = [m.column for m in self.measures]
         if self.dimension:
             columns.append(self.dimension.column)
         return columns
@@ -89,15 +96,15 @@
     @classmethod
     def from_json(cls, json_data: dict[str, Any]) -> "PlotConfig":
         assert "chart_type" in json_data
         assert "dimension" in json_data
 
         def wrap_if_not_list(value: str | list[str]) -> list[str]:
             if not isinstance(value, list):
-                return [value]
+                return [] if value is None else [value]
             else:
                 return value
 
         chart_type = ChartType(json_data["chart_type"])
         measures = [
             Measure.from_text(m)
             for m in wrap_if_not_list(json_data.get("measures", []))
@@ -115,15 +122,18 @@
             Dimension(json_data["hue"]) if json_data.get("hue") else None,
             json_data.get("xmin"),
             json_data.get("xmax"),
             json_data.get("ymin"),
             json_data.get("ymax"),
             json_data.get("xlabel"),
             json_data.get("ylabel"),
-            AxisOrder(json_data["order_by"]) if json_data.get("order_by") else None,
+            SortingCriteria(json_data["sort_criteria"])
+            if json_data.get("sort_criteria")
+            else None,
+            SortOrder(json_data["sort_order"]) if json_data.get("sort_order") else None,
         )
 
 
 @dataclass
 class LLMResponse:
     response_type: ResponseType
     config: PlotConfig | None = None
```

### Comparing `chat2plot-0.0.1/chat2plot/transform.py` & `chat2plot-0.0.2/chat2plot/transform.py`

 * *Files identical despite different names*

### Comparing `chat2plot-0.0.1/setup.cfg` & `chat2plot-0.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `chat2plot-0.0.1/setup.py` & `chat2plot-0.0.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,47 +3,43 @@
 
 from setuptools import find_packages, setup
 
 
 def get_long_description():
     here = path.abspath(path.dirname(__file__))
 
-    with open(path.join(here, 'README.md'), encoding='utf-8') as f:
+    with open(path.join(here, "README.md"), encoding="utf-8") as f:
         long_description = f.read()
     return long_description
 
 
 def get_version():
-    version_filepath = path.join(path.dirname(__file__), 'chat2plot', 'version.py')
+    version_filepath = path.join(path.dirname(__file__), "chat2plot", "version.py")
     with open(version_filepath) as f:
         for line in f:
-            if line.startswith('__version__'):
+            if line.startswith("__version__"):
                 return line.strip().split()[-1][1:-1]
 
 
 def requirements_from_file(filename):
     return open(filename).read().splitlines()
 
 
 setup(
-    name='chat2plot',
+    name="chat2plot",
     packages=find_packages(),
-
     version=get_version(),
-
-    license='MIT',
-
+    license="MIT",
     install_requires=requirements_from_file("requirements.txt"),
-
-    author='nyanp',
-    author_email='Noumi.Taiga@gmail.com',
-    url='https://github.com/nyanp/chat2plot',
-    description='chat to visualization with LLM',
+    author="nyanp",
+    author_email="Noumi.Taiga@gmail.com",
+    url="https://github.com/nyanp/chat2plot",
+    description="chat to visualization with LLM",
     long_description=get_long_description(),
-    long_description_content_type='text/markdown',
-    keywords='llm visualization chart gpt',
+    long_description_content_type="text/markdown",
+    keywords="llm visualization chart gpt",
     classifiers=[
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11'
-    ]
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+    ],
 )
```

