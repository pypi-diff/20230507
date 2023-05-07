# Comparing `tmp/spectrafit-1.0.0b1.tar.gz` & `tmp/spectrafit-1.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectrafit-1.0.0b1.tar", max compression
+gzip compressed data, was "spectrafit-1.0.0b2.tar", max compression
```

## Comparing `spectrafit-1.0.0b1.tar` & `spectrafit-1.0.0b2.tar`

### file list

```diff
@@ -1,85 +1,85 @@
--rw-r--r--   0        0        0     6629 2023-03-18 06:23:52.253288 spectrafit-1.0.0b1/LICENSE
--rw-r--r--   0        0        0     9347 2023-03-18 06:23:52.253288 spectrafit-1.0.0b1/README.md
--rw-r--r--   0        0        0     5848 2023-03-18 06:23:52.277288 spectrafit-1.0.0b1/pyproject.toml
--rw-r--r--   0        0        0       83 2023-03-18 06:23:52.277288 spectrafit-1.0.0b1/spectrafit/__init__.py
--rw-r--r--   0        0        0       55 2023-03-18 06:23:52.277288 spectrafit-1.0.0b1/spectrafit/api/__init__.py
--rw-r--r--   0        0        0     2614 2023-03-18 06:23:52.277288 spectrafit-1.0.0b1/spectrafit/api/cmd_model.py
--rw-r--r--   0        0        0     1763 2023-03-18 06:23:52.277288 spectrafit-1.0.0b1/spectrafit/api/file_model.py
--rw-r--r--   0        0        0    11028 2023-03-18 06:23:52.277288 spectrafit-1.0.0b1/spectrafit/api/models_model.py
--rw-r--r--   0        0        0     6799 2023-03-18 06:23:52.277288 spectrafit-1.0.0b1/spectrafit/api/notebook_model.py
--rw-r--r--   0        0        0     4794 2023-03-18 06:23:52.277288 spectrafit-1.0.0b1/spectrafit/api/report_model.py
--rw-r--r--   0        0        0     3551 2023-03-18 06:23:52.277288 spectrafit-1.0.0b1/spectrafit/api/rixs_model.py
--rw-r--r--   0        0        0       50 2023-03-18 06:23:52.277288 spectrafit-1.0.0b1/spectrafit/api/test/__init__.py
--rw-r--r--   0        0        0     2218 2023-03-18 06:23:52.277288 spectrafit-1.0.0b1/spectrafit/api/test/test_cmd_model.py
--rw-r--r--   0        0        0     2919 2023-03-18 06:23:52.277288 spectrafit-1.0.0b1/spectrafit/api/test/test_file_model.py
--rw-r--r--   0        0        0      668 2023-03-18 06:23:52.277288 spectrafit-1.0.0b1/spectrafit/api/test/test_models_model.py
--rw-r--r--   0        0        0     3029 2023-03-18 06:23:52.277288 spectrafit-1.0.0b1/spectrafit/api/test/test_notebook_model.py
--rw-r--r--   0        0        0     2445 2023-03-18 06:23:52.277288 spectrafit-1.0.0b1/spectrafit/api/test/test_rixs_model.py
--rw-r--r--   0        0        0      411 2023-03-18 06:23:52.277288 spectrafit-1.0.0b1/spectrafit/api/test/test_tools_model.py
--rw-r--r--   0        0        0     3527 2023-03-18 06:23:52.277288 spectrafit-1.0.0b1/spectrafit/api/tools_model.py
--rw-r--r--   0        0        0      635 2023-03-18 06:23:52.277288 spectrafit-1.0.0b1/spectrafit/app/app.py
--rw-r--r--   0        0        0       55 2023-03-18 06:23:52.277288 spectrafit-1.0.0b1/spectrafit/app/test/__init__.py
--rw-r--r--   0        0        0      430 2023-03-18 06:23:52.277288 spectrafit-1.0.0b1/spectrafit/app/test/test_app.py
--rw-r--r--   0        0        0    52668 2023-03-18 06:23:52.277288 spectrafit-1.0.0b1/spectrafit/models.py
--rw-r--r--   0        0        0     5887 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/plotting.py
--rw-r--r--   0        0        0       30 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/plugins/__init__.py
--rw-r--r--   0        0        0     2093 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/plugins/color_schemas.py
--rw-r--r--   0        0        0     1921 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/plugins/converter.py
--rw-r--r--   0        0        0     5000 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/plugins/data_converter.py
--rw-r--r--   0        0        0     4320 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/plugins/file_converter.py
--rw-r--r--   0        0        0    42261 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/plugins/notebook.py
--rw-r--r--   0        0        0     8688 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/plugins/pkl_converter.py
--rw-r--r--   0        0        0     6223 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/plugins/pkl_visualizer.py
--rw-r--r--   0        0        0     7621 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/plugins/rixs_converter.py
--rw-r--r--   0        0        0    22900 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/plugins/rixs_visualizer.py
--rw-r--r--   0        0        0       38 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/plugins/test/__init__.py
--rw-r--r--   0        0        0      895 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/plugins/test/test_color_schemas.py
--rw-r--r--   0        0        0    32789 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/plugins/test/test_converter.py
--rw-r--r--   0        0        0    20401 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/plugins/test/test_notebook.py
--rw-r--r--   0        0        0     3908 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/plugins/test/test_rixs_visualizer.py
--rw-r--r--   0        0        0    18960 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/report.py
--rw-r--r--   0        0        0     9573 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/spectrafit.py
--rw-r--r--   0        0        0       28 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/test/__init__.py
--rw-r--r--   0        0        0        0 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/test/export/place_holder
--rw-r--r--   0        0        0       12 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/test/import/test_abc.txt
--rw-r--r--   0        0        0    38582 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/test/import/test_data.csv
--rw-r--r--   0        0        0    30647 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/test/import/test_data.txt
--rw-r--r--   0        0        0    61631 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/test/import/test_data_global.csv
--rw-r--r--   0        0        0     8420 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/test/import/test_data_global_2.csv
--rw-r--r--   0        0        0     7804 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/test/import/test_data_global_3.csv
--rw-r--r--   0        0        0     1657 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/test/scripts/fitting_input.toml
--rw-r--r--   0        0        0     2025 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/test/scripts/fitting_input.yaml
--rw-r--r--   0        0        0     2563 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/test/scripts/test_globalfit.json
--rw-r--r--   0        0        0     2831 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/test/scripts/test_input_1.json
--rw-r--r--   0        0        0     2854 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/test/scripts/test_input_10.json
--rw-r--r--   0        0        0     1263 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/test/scripts/test_input_11.json
--rw-r--r--   0        0        0     2832 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/test/scripts/test_input_2.json
--rw-r--r--   0        0        0     1416 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/test/scripts/test_input_3.json
--rw-r--r--   0        0        0      941 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/test/scripts/test_input_3.toml
--rw-r--r--   0        0        0     1056 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/test/scripts/test_input_3.yaml
--rw-r--r--   0        0        0     1056 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/test/scripts/test_input_3.yml
--rw-r--r--   0        0        0     1995 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/test/scripts/test_input_4.json
--rw-r--r--   0        0        0     1243 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/test/scripts/test_input_5.json
--rw-r--r--   0        0        0     2207 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/test/scripts/test_input_6.json
--rw-r--r--   0        0        0     2889 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/test/scripts/test_input_7.json
--rw-r--r--   0        0        0     2067 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/test/scripts/test_input_8.json
--rw-r--r--   0        0        0     2060 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/test/scripts/test_input_9.json
--rw-r--r--   0        0        0     3365 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/test/scripts/test_input_all_models.toml
--rw-r--r--   0        0        0     2274 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/test/scripts/test_input_global.json
--rw-r--r--   0        0        0     2050 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/test/scripts/test_input_global_0.json
--rw-r--r--   0        0        0     2101 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/test/scripts/test_input_global_1.json
--rw-r--r--   0        0        0     2136 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/test/scripts/test_missing_parameter_1.json
--rw-r--r--   0        0        0     2144 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/test/scripts/test_missing_parameter_2.json
--rw-r--r--   0        0        0     2136 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/test/scripts/test_missing_parameters_1.json
--rw-r--r--   0        0        0     2144 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/test/scripts/test_missing_parameters_2.json
--rw-r--r--   0        0        0    13811 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/test/test_input.py
--rw-r--r--   0        0        0    44161 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/test/test_models.py
--rw-r--r--   0        0        0     5034 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/test/test_plot.py
--rw-r--r--   0        0        0     5626 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/test/test_report.py
--rw-r--r--   0        0        0    14506 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/test/test_tools.py
--rw-r--r--   0        0        0    25819 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/tools.py
--rw-r--r--   0        0        0       43 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/utilities/__init__.py
--rw-r--r--   0        0        0       40 2023-03-18 06:23:52.281288 spectrafit-1.0.0b1/spectrafit/utilities/test/__init__.py
--rw-r--r--   0        0        0     2937 2023-03-18 06:23:52.285288 spectrafit-1.0.0b1/spectrafit/utilities/test/test_transformer.py
--rw-r--r--   0        0        0     1542 2023-03-18 06:23:52.285288 spectrafit-1.0.0b1/spectrafit/utilities/transformer.py
--rw-r--r--   0        0        0    12478 1970-01-01 00:00:00.000000 spectrafit-1.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0     6629 2023-04-02 20:33:57.052322 spectrafit-1.0.0b2/LICENSE
+-rw-r--r--   0        0        0     9347 2023-04-02 20:33:57.052322 spectrafit-1.0.0b2/README.md
+-rw-r--r--   0        0        0     5892 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/pyproject.toml
+-rw-r--r--   0        0        0       83 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/__init__.py
+-rw-r--r--   0        0        0       55 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/api/__init__.py
+-rw-r--r--   0        0        0     2614 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/api/cmd_model.py
+-rw-r--r--   0        0        0     1763 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/api/file_model.py
+-rw-r--r--   0        0        0    11028 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/api/models_model.py
+-rw-r--r--   0        0        0     6799 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/api/notebook_model.py
+-rw-r--r--   0        0        0     4807 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/api/report_model.py
+-rw-r--r--   0        0        0     3551 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/api/rixs_model.py
+-rw-r--r--   0        0        0       50 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/api/test/__init__.py
+-rw-r--r--   0        0        0     2218 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/api/test/test_cmd_model.py
+-rw-r--r--   0        0        0     2919 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/api/test/test_file_model.py
+-rw-r--r--   0        0        0      668 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/api/test/test_models_model.py
+-rw-r--r--   0        0        0     3029 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/api/test/test_notebook_model.py
+-rw-r--r--   0        0        0     2445 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/api/test/test_rixs_model.py
+-rw-r--r--   0        0        0      411 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/api/test/test_tools_model.py
+-rw-r--r--   0        0        0     3527 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/api/tools_model.py
+-rw-r--r--   0        0        0      635 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/app/app.py
+-rw-r--r--   0        0        0       55 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/app/test/__init__.py
+-rw-r--r--   0        0        0      430 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/app/test/test_app.py
+-rw-r--r--   0        0        0    52668 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/models.py
+-rw-r--r--   0        0        0     5887 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/plotting.py
+-rw-r--r--   0        0        0       30 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/plugins/__init__.py
+-rw-r--r--   0        0        0     2093 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/plugins/color_schemas.py
+-rw-r--r--   0        0        0     1921 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/plugins/converter.py
+-rw-r--r--   0        0        0     5000 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/plugins/data_converter.py
+-rw-r--r--   0        0        0     4320 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/plugins/file_converter.py
+-rw-r--r--   0        0        0    42680 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/plugins/notebook.py
+-rw-r--r--   0        0        0     8688 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/plugins/pkl_converter.py
+-rw-r--r--   0        0        0     6223 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/plugins/pkl_visualizer.py
+-rw-r--r--   0        0        0     7621 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/plugins/rixs_converter.py
+-rw-r--r--   0        0        0    22900 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/plugins/rixs_visualizer.py
+-rw-r--r--   0        0        0       38 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/plugins/test/__init__.py
+-rw-r--r--   0        0        0      895 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/plugins/test/test_color_schemas.py
+-rw-r--r--   0        0        0    32789 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/plugins/test/test_converter.py
+-rw-r--r--   0        0        0    21548 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/plugins/test/test_notebook.py
+-rw-r--r--   0        0        0     3908 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/plugins/test/test_rixs_visualizer.py
+-rw-r--r--   0        0        0    18960 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/report.py
+-rw-r--r--   0        0        0     9573 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/spectrafit.py
+-rw-r--r--   0        0        0       28 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/export/place_holder
+-rw-r--r--   0        0        0       12 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/import/test_abc.txt
+-rw-r--r--   0        0        0    38582 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/import/test_data.csv
+-rw-r--r--   0        0        0    30647 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/import/test_data.txt
+-rw-r--r--   0        0        0    61631 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/import/test_data_global.csv
+-rw-r--r--   0        0        0     8420 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/import/test_data_global_2.csv
+-rw-r--r--   0        0        0     7804 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/import/test_data_global_3.csv
+-rw-r--r--   0        0        0     1657 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/scripts/fitting_input.toml
+-rw-r--r--   0        0        0     2025 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/scripts/fitting_input.yaml
+-rw-r--r--   0        0        0     2563 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/scripts/test_globalfit.json
+-rw-r--r--   0        0        0     2831 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_1.json
+-rw-r--r--   0        0        0     2854 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_10.json
+-rw-r--r--   0        0        0     1263 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_11.json
+-rw-r--r--   0        0        0     2832 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_2.json
+-rw-r--r--   0        0        0     1416 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_3.json
+-rw-r--r--   0        0        0      941 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_3.toml
+-rw-r--r--   0        0        0     1056 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_3.yaml
+-rw-r--r--   0        0        0     1056 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_3.yml
+-rw-r--r--   0        0        0     1995 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_4.json
+-rw-r--r--   0        0        0     1243 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_5.json
+-rw-r--r--   0        0        0     2207 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_6.json
+-rw-r--r--   0        0        0     2889 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_7.json
+-rw-r--r--   0        0        0     2067 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_8.json
+-rw-r--r--   0        0        0     2060 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_9.json
+-rw-r--r--   0        0        0     3365 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_all_models.toml
+-rw-r--r--   0        0        0     2274 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_global.json
+-rw-r--r--   0        0        0     2050 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_global_0.json
+-rw-r--r--   0        0        0     2101 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_global_1.json
+-rw-r--r--   0        0        0     2136 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/scripts/test_missing_parameter_1.json
+-rw-r--r--   0        0        0     2144 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/scripts/test_missing_parameter_2.json
+-rw-r--r--   0        0        0     2136 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/scripts/test_missing_parameters_1.json
+-rw-r--r--   0        0        0     2144 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/scripts/test_missing_parameters_2.json
+-rw-r--r--   0        0        0    13811 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/test_input.py
+-rw-r--r--   0        0        0    44161 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/test_models.py
+-rw-r--r--   0        0        0     5034 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/test_plot.py
+-rw-r--r--   0        0        0     5626 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/test_report.py
+-rw-r--r--   0        0        0    14506 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/test_tools.py
+-rw-r--r--   0        0        0    25819 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/tools.py
+-rw-r--r--   0        0        0       43 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/utilities/__init__.py
+-rw-r--r--   0        0        0       40 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/utilities/test/__init__.py
+-rw-r--r--   0        0        0     2937 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/utilities/test/test_transformer.py
+-rw-r--r--   0        0        0     1542 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/utilities/transformer.py
+-rw-r--r--   0        0        0    12580 1970-01-01 00:00:00.000000 spectrafit-1.0.0b2/PKG-INFO
```

### Comparing `spectrafit-1.0.0b1/LICENSE` & `spectrafit-1.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/README.md` & `spectrafit-1.0.0b2/README.md`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/pyproject.toml` & `spectrafit-1.0.0b2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "SpectraFit"
-version = "1.0.0b1"
+version = "1.0.0b2"
 description = "Fast fitting of 2D- and 3D-Spectra with established routines"
 readme = "README.md"
 authors = ["Anselm Hahn <anselm.hahn@gmail.com>"]
 maintainers = ["Anselm Hahn <anselm.hahn@gmail.com>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/Anselmoo/spectrafit"
 documentation = "https://anselmoo.github.io/spectrafit/"
@@ -24,28 +24,29 @@
   "Environment :: Console",
   "Framework :: Matplotlib",
   "Framework :: Jupyter :: JupyterLab",
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Topic :: Scientific/Engineering :: Physics",
   "Topic :: Scientific/Engineering :: Chemistry",
   "Topic :: Scientific/Engineering :: Information Analysis",
 ]
 include = [
   { path = "spectrafit/test/", format = "sdist" },
   { path = "examples/", format = "sdist" },
 ]
 exclude = ["docs/", "tools/"]
 
 
   [tool.poetry.dependencies]
-  python = ">=3.8,<3.11"
+  python = ">=3.8,<3.12"
   lmfit = "^1.1.0"
   pandas = "^1.5.0"
   numpy = "^1.23.4"
   emcee = "^3.1.2"
   tabulate = "^0.9.0"
   PyYAML = "^6.0"
   openpyxl = "^3.0.9"
@@ -54,15 +55,15 @@
   tqdm = "^4.64.0"
   scikit-learn = "^1.2.0"
   art = "^5.8"
   tomli = "^2.0.1"
   tomli-w = "^1.0.0"
   pydantic = "^1.10.1"
   jupyterlab = { version = "^3.5.2", optional = true }
-  plotly = { version = "^5.11.0", optional = true }
+  plotly = { version = "^5.14.0", optional = true }
   itables = { version = "^1.3.4", optional = true }
   kaleido = { version = "0.2.1", optional = true }
   dtale = { version = "^2.8.1", optional = true }
   networkx = { extras = ["all"], version = "^3.0", optional = true }
   pydot = { version = "^1.4.2", optional = true }
   jupyter-dash = { version = "^0.4.2", optional = true }
   ipywidgets = { version = "^8.0.4", optional = true }
@@ -97,15 +98,15 @@
   mkdocs-literate-nav = ">=0.4.1,<0.7.0"
   mkdocs-section-index = "^0.3.4"
   mike = "^1.1.2"
   mkdocs-autorefs = "^0.4.1"
   mkdocs-minify-plugin = "^0.6.2"
   mkdocs-material = "^9.1.2"
   jupytext = "^1.14.5"
-  mkdocs-jupyter = "^0.23.1"
+  mkdocs-jupyter = "^0.24.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 spectrafit = "spectrafit.spectrafit:command_line_runner"
```

### Comparing `spectrafit-1.0.0b1/spectrafit/api/cmd_model.py` & `spectrafit-1.0.0b2/spectrafit/api/cmd_model.py`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/api/file_model.py` & `spectrafit-1.0.0b2/spectrafit/api/file_model.py`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/api/models_model.py` & `spectrafit-1.0.0b2/spectrafit/api/models_model.py`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/api/notebook_model.py` & `spectrafit-1.0.0b2/spectrafit/api/notebook_model.py`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/api/report_model.py` & `spectrafit-1.0.0b2/spectrafit/api/report_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 class FitMethodAPI(BaseModel):
     """Fit method API model."""
 
     global_fitting: Union[bool, int] = Field(
         default=False,
         description="Fitting in the global fashion",
     )
-    confidence_interval: Dict[str, Any] = Field(
+    confidence_interval: Union[bool, Dict[str, Any]] = Field(
         ...,
         description="Settings for the confidence interval calculation",
     )
     configurations: Dict[str, Any] = Field(
         ..., description="Settings for the fitting configuration"
     )
```

### Comparing `spectrafit-1.0.0b1/spectrafit/api/rixs_model.py` & `spectrafit-1.0.0b2/spectrafit/api/rixs_model.py`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/api/test/test_cmd_model.py` & `spectrafit-1.0.0b2/spectrafit/api/test/test_cmd_model.py`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/api/test/test_file_model.py` & `spectrafit-1.0.0b2/spectrafit/api/test/test_file_model.py`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/api/test/test_models_model.py` & `spectrafit-1.0.0b2/spectrafit/api/test/test_models_model.py`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/api/test/test_notebook_model.py` & `spectrafit-1.0.0b2/spectrafit/api/test/test_notebook_model.py`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/api/test/test_rixs_model.py` & `spectrafit-1.0.0b2/spectrafit/api/test/test_rixs_model.py`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/api/tools_model.py` & `spectrafit-1.0.0b2/spectrafit/api/tools_model.py`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/app/app.py` & `spectrafit-1.0.0b2/spectrafit/app/app.py`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/models.py` & `spectrafit-1.0.0b2/spectrafit/models.py`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/plotting.py` & `spectrafit-1.0.0b2/spectrafit/plotting.py`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/plugins/color_schemas.py` & `spectrafit-1.0.0b2/spectrafit/plugins/color_schemas.py`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/plugins/converter.py` & `spectrafit-1.0.0b2/spectrafit/plugins/converter.py`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/plugins/data_converter.py` & `spectrafit-1.0.0b2/spectrafit/plugins/data_converter.py`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/plugins/file_converter.py` & `spectrafit-1.0.0b2/spectrafit/plugins/file_converter.py`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/plugins/notebook.py` & `spectrafit-1.0.0b2/spectrafit/plugins/notebook.py`

 * *Files 1% similar despite different names*

```diff
@@ -565,29 +565,37 @@
         Returns:
             Dict[str, Any]: Linear correlation of the spectra, fit, and components
                  as dictionary.
         """
         return self.args_out["linear_correlation"]
 
     @property
-    def settings_conf_interval(self) -> Dict[str, Any]:
+    def settings_conf_interval(self) -> Union[bool, Dict[str, Any]]:
         """Confidence interval settings.
 
         Returns:
-            Dict[str, Any]: Confidence interval settings.
+            Union[bool, Dict[str, Any]]: Confidence interval settings.
         """
+        if isinstance(self.args_out["conf_interval"], dict):
+            self.args_out["conf_interval"] = {
+                key: value if value is not None else {}
+                for key, value in self.args_out["conf_interval"].items()
+            }
         return self.args_out["conf_interval"]
 
     @property
     def get_confidence_interval(self) -> Dict[Any, Any]:
         """Get the confidence interval.
 
         Returns:
-            Dict[Any, Any]: Confidence interval as dictionary.
+            Dict[Any, Any]: Confidence interval as dictionary with or without the
+                    confidence interval results.
         """
+        if self.args_out["conf_interval"] is False:
+            return {}
         return self.args_out["confidence_interval"]
 
     @property
     def get_current_metric(self) -> pd.DataFrame:
         """Get the current metric.
 
         !!! note "About the regression metrics"
```

### Comparing `spectrafit-1.0.0b1/spectrafit/plugins/pkl_converter.py` & `spectrafit-1.0.0b2/spectrafit/plugins/pkl_converter.py`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/plugins/pkl_visualizer.py` & `spectrafit-1.0.0b2/spectrafit/plugins/pkl_visualizer.py`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/plugins/rixs_converter.py` & `spectrafit-1.0.0b2/spectrafit/plugins/rixs_converter.py`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/plugins/rixs_visualizer.py` & `spectrafit-1.0.0b2/spectrafit/plugins/rixs_visualizer.py`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/plugins/test/test_color_schemas.py` & `spectrafit-1.0.0b2/spectrafit/plugins/test/test_color_schemas.py`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/plugins/test/test_converter.py` & `spectrafit-1.0.0b2/spectrafit/plugins/test/test_converter.py`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/plugins/test/test_notebook.py` & `spectrafit-1.0.0b2/spectrafit/plugins/test/test_notebook.py`

 * *Files 2% similar despite different names*

```diff
@@ -567,19 +567,56 @@
                 show_metric=True,
                 show_peaks=True,
                 conf_interval={},
             )
 
             mock_show.assert_called_once()
 
+    def test_conv_no(
+        self,
+        class_spectrafit_fit: SpectraFitNotebook,
+        initial_model: List[Dict[str, Dict[str, Dict[str, Any]]]],
+    ) -> None:
+        """Test conf interval via bool for false."""
+        sp = class_spectrafit_fit
+
+        with mock.patch(__plotly_io_show__) as mock_show:
+            sp.solver_model(
+                initial_model=initial_model,
+                show_plot=False,
+                show_df=True,
+                show_metric=True,
+                show_peaks=True,
+                conf_interval=False,
+            )
+
+            mock_show.assert_called_once()
+
     def test_display_current_df(
         self,
         class_spectrafit_fit: SpectraFitNotebook,
         dataframe_2: pd.DataFrame,
     ) -> None:
         """Test the display_current_df function."""
         sp = class_spectrafit_fit
         sp.df_pre = sp.df_org = sp.df_fit = dataframe_2
         sp.display_current_df()
         sp.display_original_df()
         sp.display_preprocessed_df()
         sp.display_fit_df()
+
+    def test_confidence_interval_false_expot(
+        self,
+        class_spectrafit_fit: SpectraFitNotebook,
+        initial_model: List[Dict[str, Dict[str, Dict[str, Any]]]],
+    ) -> None:
+        """Test the confidence interval function."""
+        sp = class_spectrafit_fit
+        sp.solver_model(
+            initial_model=initial_model,
+            show_plot=False,
+            show_df=False,
+            show_metric=False,
+            show_peaks=False,
+            conf_interval=False,
+        )
+        sp.generate_report
```

### Comparing `spectrafit-1.0.0b1/spectrafit/plugins/test/test_rixs_visualizer.py` & `spectrafit-1.0.0b2/spectrafit/plugins/test/test_rixs_visualizer.py`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/report.py` & `spectrafit-1.0.0b2/spectrafit/report.py`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/spectrafit.py` & `spectrafit-1.0.0b2/spectrafit/spectrafit.py`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/test/import/test_data.csv` & `spectrafit-1.0.0b2/spectrafit/test/import/test_data.csv`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/test/import/test_data.txt` & `spectrafit-1.0.0b2/spectrafit/test/import/test_data.txt`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/test/import/test_data_global.csv` & `spectrafit-1.0.0b2/spectrafit/test/import/test_data_global.csv`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/test/import/test_data_global_2.csv` & `spectrafit-1.0.0b2/spectrafit/test/import/test_data_global_2.csv`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/test/import/test_data_global_3.csv` & `spectrafit-1.0.0b2/spectrafit/test/import/test_data_global_3.csv`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/test/scripts/fitting_input.toml` & `spectrafit-1.0.0b2/spectrafit/test/scripts/fitting_input.toml`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/test/scripts/fitting_input.yaml` & `spectrafit-1.0.0b2/spectrafit/test/scripts/fitting_input.yaml`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/test/scripts/test_globalfit.json` & `spectrafit-1.0.0b2/spectrafit/test/scripts/test_globalfit.json`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/test/scripts/test_input_1.json` & `spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_1.json`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/test/scripts/test_input_10.json` & `spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_10.json`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/test/scripts/test_input_11.json` & `spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_11.json`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/test/scripts/test_input_2.json` & `spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_2.json`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/test/scripts/test_input_3.json` & `spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_3.json`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/test/scripts/test_input_3.toml` & `spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_3.toml`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/test/scripts/test_input_3.yaml` & `spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_3.yaml`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/test/scripts/test_input_3.yml` & `spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_3.yml`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/test/scripts/test_input_4.json` & `spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_4.json`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/test/scripts/test_input_5.json` & `spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_5.json`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/test/scripts/test_input_6.json` & `spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_6.json`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/test/scripts/test_input_7.json` & `spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_7.json`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/test/scripts/test_input_8.json` & `spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_8.json`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/test/scripts/test_input_9.json` & `spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_9.json`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/test/scripts/test_input_all_models.toml` & `spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_all_models.toml`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/test/scripts/test_input_global.json` & `spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_global.json`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/test/scripts/test_input_global_0.json` & `spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_global_0.json`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/test/scripts/test_input_global_1.json` & `spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_global_1.json`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/test/scripts/test_missing_parameter_1.json` & `spectrafit-1.0.0b2/spectrafit/test/scripts/test_missing_parameter_1.json`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/test/scripts/test_missing_parameter_2.json` & `spectrafit-1.0.0b2/spectrafit/test/scripts/test_missing_parameter_2.json`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/test/scripts/test_missing_parameters_1.json` & `spectrafit-1.0.0b2/spectrafit/test/scripts/test_missing_parameters_1.json`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/test/scripts/test_missing_parameters_2.json` & `spectrafit-1.0.0b2/spectrafit/test/scripts/test_missing_parameters_2.json`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/test/test_input.py` & `spectrafit-1.0.0b2/spectrafit/test/test_input.py`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/test/test_models.py` & `spectrafit-1.0.0b2/spectrafit/test/test_models.py`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/test/test_plot.py` & `spectrafit-1.0.0b2/spectrafit/test/test_plot.py`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/test/test_report.py` & `spectrafit-1.0.0b2/spectrafit/test/test_report.py`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/test/test_tools.py` & `spectrafit-1.0.0b2/spectrafit/test/test_tools.py`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/tools.py` & `spectrafit-1.0.0b2/spectrafit/tools.py`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/utilities/test/test_transformer.py` & `spectrafit-1.0.0b2/spectrafit/utilities/test/test_transformer.py`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/spectrafit/utilities/transformer.py` & `spectrafit-1.0.0b2/spectrafit/utilities/transformer.py`

 * *Files identical despite different names*

### Comparing `spectrafit-1.0.0b1/PKG-INFO` & `spectrafit-1.0.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.1
 Name: spectrafit
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: Fast fitting of 2D- and 3D-Spectra with established routines
 Home-page: https://pypi.org/project/spectrafit/
 License: BSD-3-Clause
 Keywords: 2D-Spectra,3D-Spectra,fitting,curve-fitting,peak-fitting,spectrum
 Author: Anselm Hahn
 Author-email: anselm.hahn@gmail.com
 Maintainer: Anselm Hahn
 Maintainer-email: anselm.hahn@gmail.com
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Framework :: Jupyter :: JupyterLab
 Classifier: Framework :: Matplotlib
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Physics
 Provides-Extra: all
@@ -45,15 +47,15 @@
 Requires-Dist: kaleido (==0.2.1) ; extra == "jupyter" or extra == "all"
 Requires-Dist: lmfit (>=1.1.0,<2.0.0)
 Requires-Dist: networkx[all] (>=3.0,<4.0) ; extra == "graph" or extra == "all"
 Requires-Dist: numdifftools (>=0.9.41,<0.10.0)
 Requires-Dist: numpy (>=1.23.4,<2.0.0)
 Requires-Dist: openpyxl (>=3.0.9,<4.0.0)
 Requires-Dist: pandas (>=1.5.0,<2.0.0)
-Requires-Dist: plotly (>=5.11.0,<6.0.0) ; extra == "jupyter" or extra == "all"
+Requires-Dist: plotly (>=5.14.0,<6.0.0) ; extra == "jupyter" or extra == "all"
 Requires-Dist: pydantic (>=1.10.1,<2.0.0)
 Requires-Dist: pydot (>=1.4.2,<2.0.0) ; extra == "graph" or extra == "all"
 Requires-Dist: scikit-learn (>=1.2.0,<2.0.0)
 Requires-Dist: seaborn (>=0.12.0,<0.13.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Requires-Dist: tomli-w (>=1.0.0,<2.0.0)
```

