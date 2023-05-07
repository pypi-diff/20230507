# Comparing `tmp/superwise-8.2.8.tar.gz` & `tmp/superwise-8.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/superwise-8.2.8.tar", last modified: Tue Dec 13 14:20:15 2022, max compression
+gzip compressed data, was "dist/superwise-8.2.9.tar", last modified: Wed Mar 29 09:17:11 2023, max compression
```

## Comparing `superwise-8.2.8.tar` & `superwise-8.2.9.tar`

### file list

```diff
@@ -1,157 +1,157 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 14:20:15.000000 superwise-8.2.8/
--rw-rw-rw-   0 root         (0) root         (0)      738 2022-12-13 14:18:39.000000 superwise-8.2.8/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     6589 2022-12-13 14:18:39.000000 superwise-8.2.8/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)     1069 2022-12-13 14:18:39.000000 superwise-8.2.8/LICENCE
--rw-rw-rw-   0 root         (0) root         (0)      166 2022-12-13 14:18:39.000000 superwise-8.2.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1275 2022-12-13 14:20:15.000000 superwise-8.2.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      608 2022-12-13 14:18:39.000000 superwise-8.2.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 14:20:15.000000 superwise-8.2.8/assets/
--rw-rw-rw-   0 root         (0) root         (0)      598 2022-12-13 14:18:39.000000 superwise-8.2.8/assets/favicon.png
--rw-rw-rw-   0 root         (0) root         (0)   142061 2022-12-13 14:18:39.000000 superwise-8.2.8/assets/image.png
--rw-rw-rw-   0 root         (0) root         (0)    18864 2022-12-13 14:18:39.000000 superwise-8.2.8/assets/superwise.png
--rwxrwxrwx   0 root         (0) root         (0)      261 2022-12-13 14:18:39.000000 superwise-8.2.8/build-docs.sh
--rw-rw-rw-   0 root         (0) root         (0)     2187 2022-12-13 14:18:39.000000 superwise-8.2.8/docs.py
--rw-rw-rw-   0 root         (0) root         (0)      455 2022-12-13 14:18:39.000000 superwise-8.2.8/index.md
--rw-rw-rw-   0 root         (0) root         (0)      759 2022-12-13 14:18:39.000000 superwise-8.2.8/mkdocs.yml
--rw-rw-rw-   0 root         (0) root         (0)       69 2022-12-13 14:18:39.000000 superwise-8.2.8/project_root.py
--rw-rw-rw-   0 root         (0) root         (0)      360 2022-12-13 14:18:39.000000 superwise-8.2.8/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-12-13 14:20:15.000000 superwise-8.2.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1309 2022-12-13 14:18:39.000000 superwise-8.2.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 14:20:15.000000 superwise-8.2.8/superwise/
--rw-rw-rw-   0 root         (0) root         (0)     4094 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1173 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 14:20:15.000000 superwise-8.2.8/superwise/controller/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/controller/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7936 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/controller/base.py
--rw-rw-rw-   0 root         (0) root         (0)     6959 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/controller/dataentity.py
--rw-rw-rw-   0 root         (0) root         (0)    11872 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/controller/dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     1353 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/controller/infer.py
--rw-rw-rw-   0 root         (0) root         (0)      813 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/controller/model.py
--rw-rw-rw-   0 root         (0) root         (0)     3452 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/controller/notification.py
--rw-rw-rw-   0 root         (0) root         (0)      800 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/controller/policy.py
--rw-rw-rw-   0 root         (0) root         (0)      488 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/controller/project.py
--rw-rw-rw-   0 root         (0) root         (0)      941 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/controller/role.py
--rw-rw-rw-   0 root         (0) root         (0)      493 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/controller/segment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 14:20:15.000000 superwise-8.2.8/superwise/controller/summary/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/controller/summary/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      926 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/controller/summary/boolean_summary_generator.py
--rw-rw-rw-   0 root         (0) root         (0)     2701 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/controller/summary/categorical_summary_generator.py
--rw-rw-rw-   0 root         (0) root         (0)    17004 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/controller/summary/entities_validator.py
--rw-rw-rw-   0 root         (0) root         (0)      941 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/controller/summary/entity_summary_generator.py
--rw-rw-rw-   0 root         (0) root         (0)     6747 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/controller/summary/feature_importance.py
--rw-rw-rw-   0 root         (0) root         (0)     6887 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/controller/summary/numeric_summary_generator.py
--rw-rw-rw-   0 root         (0) root         (0)     2328 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/controller/summary/summary.py
--rw-rw-rw-   0 root         (0) root         (0)      129 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/controller/summary/timestamp_summary_generator.py
--rw-rw-rw-   0 root         (0) root         (0)      127 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/controller/summary/unknown_summary_generator.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/controller/summary.py
--rw-rw-rw-   0 root         (0) root         (0)    11276 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/controller/transaction.py
--rw-rw-rw-   0 root         (0) root         (0)     2779 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/controller/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 14:20:15.000000 superwise-8.2.8/superwise/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1430 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/models/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2610 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/models/data_entity.py
--rw-rw-rw-   0 root         (0) root         (0)     3373 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/models/dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     1280 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/models/model.py
--rw-rw-rw-   0 root         (0) root         (0)     1215 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/models/notification.py
--rw-rw-rw-   0 root         (0) root         (0)      850 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/models/project.py
--rw-rw-rw-   0 root         (0) root         (0)     1117 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/models/role.py
--rw-rw-rw-   0 root         (0) root         (0)     3129 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/models/segment.py
--rw-rw-rw-   0 root         (0) root         (0)     1968 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/models/transaction.py
--rw-rw-rw-   0 root         (0) root         (0)     1430 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/models/validation_error.py
--rw-rw-rw-   0 root         (0) root         (0)     1163 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/models/version.py
--rw-rw-rw-   0 root         (0) root         (0)      234 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 14:20:15.000000 superwise-8.2.8/superwise/resources/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/resources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5609 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/resources/superwise_enums.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 14:20:15.000000 superwise-8.2.8/superwise/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8538 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/utils/client.py
--rw-rw-rw-   0 root         (0) root         (0)     1941 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/utils/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)      139 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/utils/file_path.py
--rw-rw-rw-   0 root         (0) root         (0)      316 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/utils/singelton.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 14:20:15.000000 superwise-8.2.8/superwise/utils/storage/
--rw-rw-rw-   0 root         (0) root         (0)     1499 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/utils/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2949 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/utils/storage/azure_storage.py
--rw-rw-rw-   0 root         (0) root         (0)      767 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/utils/storage/dataframe.py
--rw-rw-rw-   0 root         (0) root         (0)     3923 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/utils/storage/gcs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 14:20:15.000000 superwise-8.2.8/superwise/utils/storage/internal_storage/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/utils/storage/internal_storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1107 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/utils/storage/internal_storage/aws.py
--rw-rw-rw-   0 root         (0) root         (0)     1651 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/utils/storage/internal_storage/azure.py
--rw-rw-rw-   0 root         (0) root         (0)     1966 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/utils/storage/internal_storage/gcs.py
--rw-rw-rw-   0 root         (0) root         (0)     2004 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/utils/storage/internal_storage/internal_storage.py
--rw-rw-rw-   0 root         (0) root         (0)     1255 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/utils/storage/internal_storage/internal_storage_factory.py
--rw-rw-rw-   0 root         (0) root         (0)      481 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/utils/storage/local.py
--rw-rw-rw-   0 root         (0) root         (0)     4420 2022-12-13 14:18:39.000000 superwise-8.2.8/superwise/utils/storage/s3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 14:20:15.000000 superwise-8.2.8/superwise.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1275 2022-12-13 14:20:15.000000 superwise-8.2.8/superwise.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4958 2022-12-13 14:20:15.000000 superwise-8.2.8/superwise.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-13 14:20:15.000000 superwise-8.2.8/superwise.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-13 14:20:15.000000 superwise-8.2.8/superwise.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      234 2022-12-13 14:20:15.000000 superwise-8.2.8/superwise.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2022-12-13 14:20:15.000000 superwise-8.2.8/superwise.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 14:20:15.000000 superwise-8.2.8/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1091 2022-12-13 14:18:39.000000 superwise-8.2.8/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 14:20:15.000000 superwise-8.2.8/tests/conf/
--rw-rw-rw-   0 root         (0) root         (0)       46 2022-12-13 14:18:39.000000 superwise-8.2.8/tests/conf/config.example.json
--rw-rw-rw-   0 root         (0) root         (0)      219 2022-12-13 14:18:39.000000 superwise-8.2.8/tests/conf/config.py
--rw-rw-rw-   0 root         (0) root         (0)     5550 2022-12-13 14:18:39.000000 superwise-8.2.8/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 14:20:15.000000 superwise-8.2.8/tests/resources/
--rw-rw-rw-   0 root         (0) root         (0)     5936 2022-12-13 14:18:39.000000 superwise-8.2.8/tests/resources/basic_schema.json
--rw-rw-rw-   0 root         (0) root         (0)    11185 2022-12-13 14:18:39.000000 superwise-8.2.8/tests/resources/data.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 14:20:15.000000 superwise-8.2.8/tests/resources/data_entity/
--rw-rw-rw-   0 root         (0) root         (0)      128 2022-12-13 14:18:39.000000 superwise-8.2.8/tests/resources/data_entity/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 14:20:15.000000 superwise-8.2.8/tests/resources/data_entity/assets/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 14:20:15.000000 superwise-8.2.8/tests/resources/data_entity/assets/baseline/
--rw-rw-rw-   0 root         (0) root         (0)     1057 2022-12-13 14:18:39.000000 superwise-8.2.8/tests/resources/data_entity/assets/baseline/basic_baseline.json
--rw-rw-rw-   0 root         (0) root         (0)     1400 2022-12-13 14:18:39.000000 superwise-8.2.8/tests/resources/data_entity/assets/baseline/basic_schema.json
--rw-rw-rw-   0 root         (0) root         (0)    22934 2022-12-13 14:18:39.000000 superwise-8.2.8/tests/resources/data_entity/assets/entities.json
--rw-rw-rw-   0 root         (0) root         (0)    20583 2022-12-13 14:18:39.000000 superwise-8.2.8/tests/resources/data_entity/assets/entities_with_feature_importance.json
--rw-rw-rw-   0 root         (0) root         (0)      730 2022-12-13 14:18:39.000000 superwise-8.2.8/tests/resources/data_entity/assets/entity_with_feature_importance.json
--rw-rw-rw-   0 root         (0) root         (0)      433 2022-12-13 14:18:39.000000 superwise-8.2.8/tests/resources/data_entity/assets/new_summary.json
--rw-rw-rw-   0 root         (0) root         (0)      803 2022-12-13 14:18:39.000000 superwise-8.2.8/tests/resources/data_entity/assets/patched_response.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 14:20:15.000000 superwise-8.2.8/tests/resources/data_entity/assets/summary/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 14:20:15.000000 superwise-8.2.8/tests/resources/data_entity/assets/summary/boolean/
--rw-rw-rw-   0 root         (0) root         (0)      289 2022-12-13 14:18:39.000000 superwise-8.2.8/tests/resources/data_entity/assets/summary/boolean/flag.json
--rw-rw-rw-   0 root         (0) root         (0)      273 2022-12-13 14:18:39.000000 superwise-8.2.8/tests/resources/data_entity/assets/summary/boolean/numeric.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 14:20:15.000000 superwise-8.2.8/tests/resources/data_entity/assets/summary/categorical/
--rw-rw-rw-   0 root         (0) root         (0)      271 2022-12-13 14:18:39.000000 superwise-8.2.8/tests/resources/data_entity/assets/summary/categorical/constant.json
--rw-rw-rw-   0 root         (0) root         (0)      462 2022-12-13 14:18:39.000000 superwise-8.2.8/tests/resources/data_entity/assets/summary/categorical/dense.json
--rw-rw-rw-   0 root         (0) root         (0)       52 2022-12-13 14:18:39.000000 superwise-8.2.8/tests/resources/data_entity/assets/summary/categorical/sparse.json
--rw-rw-rw-   0 root         (0) root         (0)       52 2022-12-13 14:18:39.000000 superwise-8.2.8/tests/resources/data_entity/assets/summary/categorical/sparse_freq_cats.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 14:20:15.000000 superwise-8.2.8/tests/resources/data_entity/assets/summary/numeric/
--rw-rw-rw-   0 root         (0) root         (0)     7742 2022-12-13 14:18:39.000000 superwise-8.2.8/tests/resources/data_entity/assets/summary/numeric/num_centered.json
--rw-rw-rw-   0 root         (0) root         (0)     7742 2022-12-13 14:18:39.000000 superwise-8.2.8/tests/resources/data_entity/assets/summary/numeric/num_left_tail.json
--rw-rw-rw-   0 root         (0) root         (0)     7742 2022-12-13 14:18:39.000000 superwise-8.2.8/tests/resources/data_entity/assets/summary/numeric/num_right_tail.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 14:20:15.000000 superwise-8.2.8/tests/resources/data_entity/assets/summary/numeric/with_previous/
--rw-rw-rw-   0 root         (0) root         (0)     2630 2022-12-13 14:18:39.000000 superwise-8.2.8/tests/resources/data_entity/assets/summary/numeric/with_previous/num_centered.json
--rw-rw-rw-   0 root         (0) root         (0)     1628 2022-12-13 14:18:39.000000 superwise-8.2.8/tests/resources/data_entity/assets/summary/numeric/with_previous/num_left_tail.json
--rw-rw-rw-   0 root         (0) root         (0)     1628 2022-12-13 14:18:39.000000 superwise-8.2.8/tests/resources/data_entity/assets/summary/numeric/with_previous/num_right_tail.json
--rw-rw-rw-   0 root         (0) root         (0)       67 2022-12-13 14:18:39.000000 superwise-8.2.8/tests/resources/data_entity/assets/summary/timestamp.json
--rw-rw-rw-   0 root         (0) root         (0)       52 2022-12-13 14:18:39.000000 superwise-8.2.8/tests/resources/data_entity/assets/summary/unknown.json
--rw-rw-rw-   0 root         (0) root         (0)     1373 2022-12-13 14:18:39.000000 superwise-8.2.8/tests/resources/data_entity/expected_infer.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 14:20:15.000000 superwise-8.2.8/tests/resources/dataset/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-13 14:18:39.000000 superwise-8.2.8/tests/resources/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       54 2022-12-13 14:18:39.000000 superwise-8.2.8/tests/resources/dataset/test.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 14:20:15.000000 superwise-8.2.8/tests/resources/internal_sdk/
--rw-rw-rw-   0 root         (0) root         (0)     5890 2022-12-13 14:18:39.000000 superwise-8.2.8/tests/resources/internal_sdk/basic_schema.json
--rw-rw-rw-   0 root         (0) root         (0)     5890 2022-12-13 14:18:39.000000 superwise-8.2.8/tests/resources/internal_sdk/basic_schema_todel.json
--rw-rw-rw-   0 root         (0) root         (0)     6215 2022-12-13 14:18:39.000000 superwise-8.2.8/tests/resources/internal_sdk/basic_schema_too_much_dimension.json
--rw-rw-rw-   0 root         (0) root         (0)    35657 2022-12-13 14:18:39.000000 superwise-8.2.8/tests/resources/internal_sdk/data.json
--rw-rw-rw-   0 root         (0) root         (0)     5030 2022-12-13 14:18:39.000000 superwise-8.2.8/tests/resources/internal_sdk/data_basic.json
--rw-rw-rw-   0 root         (0) root         (0)    35577 2022-12-13 14:18:39.000000 superwise-8.2.8/tests/resources/internal_sdk/data_bool.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 14:20:15.000000 superwise-8.2.8/tests/resources/transaction/
--rw-rw-rw-   0 root         (0) root         (0)      164 2022-12-13 14:18:39.000000 superwise-8.2.8/tests/resources/transaction/local_records_file.json
--rw-rw-rw-   0 root         (0) root         (0)      326 2022-12-13 14:18:39.000000 superwise-8.2.8/tests/resources/transaction/records_payload.json
--rw-rw-rw-   0 root         (0) root         (0)     7358 2022-12-13 14:18:39.000000 superwise-8.2.8/tests/test_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     2424 2022-12-13 14:18:39.000000 superwise-8.2.8/tests/test_e2e.py
--rw-rw-rw-   0 root         (0) root         (0)     7895 2022-12-13 14:18:39.000000 superwise-8.2.8/tests/test_entity_validator.py
--rw-rw-rw-   0 root         (0) root         (0)     3714 2022-12-13 14:18:39.000000 superwise-8.2.8/tests/test_http_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1833 2022-12-13 14:18:39.000000 superwise-8.2.8/tests/test_infer_unit.py
--rw-rw-rw-   0 root         (0) root         (0)     5603 2022-12-13 14:18:39.000000 superwise-8.2.8/tests/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)     3158 2022-12-13 14:18:39.000000 superwise-8.2.8/tests/test_notification.py
--rw-rw-rw-   0 root         (0) root         (0)     2461 2022-12-13 14:18:39.000000 superwise-8.2.8/tests/test_projects.py
--rw-rw-rw-   0 root         (0) root         (0)     5022 2022-12-13 14:18:39.000000 superwise-8.2.8/tests/test_segments.py
--rw-rw-rw-   0 root         (0) root         (0)     3744 2022-12-13 14:18:39.000000 superwise-8.2.8/tests/test_summary_unit.py
--rw-rw-rw-   0 root         (0) root         (0)     6636 2022-12-13 14:18:39.000000 superwise-8.2.8/tests/test_transaction.py
--rw-rw-rw-   0 root         (0) root         (0)     8558 2022-12-13 14:18:39.000000 superwise-8.2.8/tests/test_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 09:17:11.000000 superwise-8.2.9/
+-rw-rw-rw-   0 root         (0) root         (0)      738 2023-03-29 09:16:01.000000 superwise-8.2.9/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     6589 2023-03-29 09:16:01.000000 superwise-8.2.9/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-03-29 09:16:01.000000 superwise-8.2.9/LICENCE
+-rw-rw-rw-   0 root         (0) root         (0)      166 2023-03-29 09:16:01.000000 superwise-8.2.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1275 2023-03-29 09:17:11.000000 superwise-8.2.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      608 2023-03-29 09:16:01.000000 superwise-8.2.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 09:17:10.000000 superwise-8.2.9/assets/
+-rw-rw-rw-   0 root         (0) root         (0)      598 2023-03-29 09:16:01.000000 superwise-8.2.9/assets/favicon.png
+-rw-rw-rw-   0 root         (0) root         (0)   142061 2023-03-29 09:16:01.000000 superwise-8.2.9/assets/image.png
+-rw-rw-rw-   0 root         (0) root         (0)    18864 2023-03-29 09:16:01.000000 superwise-8.2.9/assets/superwise.png
+-rwxrwxrwx   0 root         (0) root         (0)      261 2023-03-29 09:16:01.000000 superwise-8.2.9/build-docs.sh
+-rw-rw-rw-   0 root         (0) root         (0)     2187 2023-03-29 09:16:01.000000 superwise-8.2.9/docs.py
+-rw-rw-rw-   0 root         (0) root         (0)      455 2023-03-29 09:16:01.000000 superwise-8.2.9/index.md
+-rw-rw-rw-   0 root         (0) root         (0)      759 2023-03-29 09:16:01.000000 superwise-8.2.9/mkdocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-03-29 09:16:01.000000 superwise-8.2.9/project_root.py
+-rw-rw-rw-   0 root         (0) root         (0)      360 2023-03-29 09:16:01.000000 superwise-8.2.9/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-03-29 09:17:11.000000 superwise-8.2.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1309 2023-03-29 09:16:01.000000 superwise-8.2.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 09:17:11.000000 superwise-8.2.9/superwise/
+-rw-rw-rw-   0 root         (0) root         (0)     4094 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1173 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 09:17:11.000000 superwise-8.2.9/superwise/controller/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/controller/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7936 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/controller/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6959 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/controller/dataentity.py
+-rw-rw-rw-   0 root         (0) root         (0)    11872 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/controller/dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     1353 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/controller/infer.py
+-rw-rw-rw-   0 root         (0) root         (0)      813 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/controller/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3452 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/controller/notification.py
+-rw-rw-rw-   0 root         (0) root         (0)      800 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/controller/policy.py
+-rw-rw-rw-   0 root         (0) root         (0)      488 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/controller/project.py
+-rw-rw-rw-   0 root         (0) root         (0)      941 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/controller/role.py
+-rw-rw-rw-   0 root         (0) root         (0)      493 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/controller/segment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 09:17:11.000000 superwise-8.2.9/superwise/controller/summary/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/controller/summary/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      926 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/controller/summary/boolean_summary_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     2701 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/controller/summary/categorical_summary_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)    17004 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/controller/summary/entities_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)      941 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/controller/summary/entity_summary_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     6747 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/controller/summary/feature_importance.py
+-rw-rw-rw-   0 root         (0) root         (0)     6887 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/controller/summary/numeric_summary_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     2328 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/controller/summary/summary.py
+-rw-rw-rw-   0 root         (0) root         (0)      129 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/controller/summary/timestamp_summary_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)      127 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/controller/summary/unknown_summary_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/controller/summary.py
+-rw-rw-rw-   0 root         (0) root         (0)    11276 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/controller/transaction.py
+-rw-rw-rw-   0 root         (0) root         (0)     2779 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/controller/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 09:17:11.000000 superwise-8.2.9/superwise/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1430 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/models/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2610 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/models/data_entity.py
+-rw-rw-rw-   0 root         (0) root         (0)     3341 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/models/dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     1280 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/models/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1215 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/models/notification.py
+-rw-rw-rw-   0 root         (0) root         (0)      850 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/models/project.py
+-rw-rw-rw-   0 root         (0) root         (0)     1117 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/models/role.py
+-rw-rw-rw-   0 root         (0) root         (0)     3129 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/models/segment.py
+-rw-rw-rw-   0 root         (0) root         (0)     1968 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/models/transaction.py
+-rw-rw-rw-   0 root         (0) root         (0)     1430 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/models/validation_error.py
+-rw-rw-rw-   0 root         (0) root         (0)     1163 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/models/version.py
+-rw-rw-rw-   0 root         (0) root         (0)      234 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 09:17:11.000000 superwise-8.2.9/superwise/resources/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/resources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5609 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/resources/superwise_enums.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 09:17:11.000000 superwise-8.2.9/superwise/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8532 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/utils/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1941 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/utils/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)      139 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/utils/file_path.py
+-rw-rw-rw-   0 root         (0) root         (0)      316 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/utils/singelton.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 09:17:11.000000 superwise-8.2.9/superwise/utils/storage/
+-rw-rw-rw-   0 root         (0) root         (0)     1499 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/utils/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2949 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/utils/storage/azure_storage.py
+-rw-rw-rw-   0 root         (0) root         (0)      767 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/utils/storage/dataframe.py
+-rw-rw-rw-   0 root         (0) root         (0)     3923 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/utils/storage/gcs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 09:17:11.000000 superwise-8.2.9/superwise/utils/storage/internal_storage/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/utils/storage/internal_storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1107 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/utils/storage/internal_storage/aws.py
+-rw-rw-rw-   0 root         (0) root         (0)     1651 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/utils/storage/internal_storage/azure.py
+-rw-rw-rw-   0 root         (0) root         (0)     1966 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/utils/storage/internal_storage/gcs.py
+-rw-rw-rw-   0 root         (0) root         (0)     2004 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/utils/storage/internal_storage/internal_storage.py
+-rw-rw-rw-   0 root         (0) root         (0)     1255 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/utils/storage/internal_storage/internal_storage_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)      481 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/utils/storage/local.py
+-rw-rw-rw-   0 root         (0) root         (0)     4420 2023-03-29 09:16:01.000000 superwise-8.2.9/superwise/utils/storage/s3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 09:17:11.000000 superwise-8.2.9/superwise.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1275 2023-03-29 09:17:10.000000 superwise-8.2.9/superwise.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4958 2023-03-29 09:17:10.000000 superwise-8.2.9/superwise.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-29 09:17:10.000000 superwise-8.2.9/superwise.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-29 09:17:10.000000 superwise-8.2.9/superwise.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      234 2023-03-29 09:17:10.000000 superwise-8.2.9/superwise.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-03-29 09:17:10.000000 superwise-8.2.9/superwise.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 09:17:11.000000 superwise-8.2.9/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1091 2023-03-29 09:16:01.000000 superwise-8.2.9/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 09:17:11.000000 superwise-8.2.9/tests/conf/
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-03-29 09:16:01.000000 superwise-8.2.9/tests/conf/config.example.json
+-rw-rw-rw-   0 root         (0) root         (0)      219 2023-03-29 09:16:01.000000 superwise-8.2.9/tests/conf/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     5550 2023-03-29 09:16:01.000000 superwise-8.2.9/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 09:17:11.000000 superwise-8.2.9/tests/resources/
+-rw-rw-rw-   0 root         (0) root         (0)     5936 2023-03-29 09:16:01.000000 superwise-8.2.9/tests/resources/basic_schema.json
+-rw-rw-rw-   0 root         (0) root         (0)    11185 2023-03-29 09:16:01.000000 superwise-8.2.9/tests/resources/data.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 09:17:11.000000 superwise-8.2.9/tests/resources/data_entity/
+-rw-rw-rw-   0 root         (0) root         (0)      128 2023-03-29 09:16:01.000000 superwise-8.2.9/tests/resources/data_entity/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 09:17:11.000000 superwise-8.2.9/tests/resources/data_entity/assets/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 09:17:11.000000 superwise-8.2.9/tests/resources/data_entity/assets/baseline/
+-rw-rw-rw-   0 root         (0) root         (0)     1057 2023-03-29 09:16:01.000000 superwise-8.2.9/tests/resources/data_entity/assets/baseline/basic_baseline.json
+-rw-rw-rw-   0 root         (0) root         (0)     1400 2023-03-29 09:16:01.000000 superwise-8.2.9/tests/resources/data_entity/assets/baseline/basic_schema.json
+-rw-rw-rw-   0 root         (0) root         (0)    22934 2023-03-29 09:16:01.000000 superwise-8.2.9/tests/resources/data_entity/assets/entities.json
+-rw-rw-rw-   0 root         (0) root         (0)    20583 2023-03-29 09:16:01.000000 superwise-8.2.9/tests/resources/data_entity/assets/entities_with_feature_importance.json
+-rw-rw-rw-   0 root         (0) root         (0)      730 2023-03-29 09:16:01.000000 superwise-8.2.9/tests/resources/data_entity/assets/entity_with_feature_importance.json
+-rw-rw-rw-   0 root         (0) root         (0)      433 2023-03-29 09:16:01.000000 superwise-8.2.9/tests/resources/data_entity/assets/new_summary.json
+-rw-rw-rw-   0 root         (0) root         (0)      803 2023-03-29 09:16:01.000000 superwise-8.2.9/tests/resources/data_entity/assets/patched_response.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 09:17:11.000000 superwise-8.2.9/tests/resources/data_entity/assets/summary/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 09:17:11.000000 superwise-8.2.9/tests/resources/data_entity/assets/summary/boolean/
+-rw-rw-rw-   0 root         (0) root         (0)      289 2023-03-29 09:16:01.000000 superwise-8.2.9/tests/resources/data_entity/assets/summary/boolean/flag.json
+-rw-rw-rw-   0 root         (0) root         (0)      273 2023-03-29 09:16:01.000000 superwise-8.2.9/tests/resources/data_entity/assets/summary/boolean/numeric.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 09:17:11.000000 superwise-8.2.9/tests/resources/data_entity/assets/summary/categorical/
+-rw-rw-rw-   0 root         (0) root         (0)      271 2023-03-29 09:16:01.000000 superwise-8.2.9/tests/resources/data_entity/assets/summary/categorical/constant.json
+-rw-rw-rw-   0 root         (0) root         (0)      462 2023-03-29 09:16:01.000000 superwise-8.2.9/tests/resources/data_entity/assets/summary/categorical/dense.json
+-rw-rw-rw-   0 root         (0) root         (0)       52 2023-03-29 09:16:01.000000 superwise-8.2.9/tests/resources/data_entity/assets/summary/categorical/sparse.json
+-rw-rw-rw-   0 root         (0) root         (0)       52 2023-03-29 09:16:01.000000 superwise-8.2.9/tests/resources/data_entity/assets/summary/categorical/sparse_freq_cats.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 09:17:11.000000 superwise-8.2.9/tests/resources/data_entity/assets/summary/numeric/
+-rw-rw-rw-   0 root         (0) root         (0)     7742 2023-03-29 09:16:01.000000 superwise-8.2.9/tests/resources/data_entity/assets/summary/numeric/num_centered.json
+-rw-rw-rw-   0 root         (0) root         (0)     7742 2023-03-29 09:16:01.000000 superwise-8.2.9/tests/resources/data_entity/assets/summary/numeric/num_left_tail.json
+-rw-rw-rw-   0 root         (0) root         (0)     7742 2023-03-29 09:16:01.000000 superwise-8.2.9/tests/resources/data_entity/assets/summary/numeric/num_right_tail.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 09:17:11.000000 superwise-8.2.9/tests/resources/data_entity/assets/summary/numeric/with_previous/
+-rw-rw-rw-   0 root         (0) root         (0)     2630 2023-03-29 09:16:01.000000 superwise-8.2.9/tests/resources/data_entity/assets/summary/numeric/with_previous/num_centered.json
+-rw-rw-rw-   0 root         (0) root         (0)     1628 2023-03-29 09:16:01.000000 superwise-8.2.9/tests/resources/data_entity/assets/summary/numeric/with_previous/num_left_tail.json
+-rw-rw-rw-   0 root         (0) root         (0)     1628 2023-03-29 09:16:01.000000 superwise-8.2.9/tests/resources/data_entity/assets/summary/numeric/with_previous/num_right_tail.json
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-03-29 09:16:01.000000 superwise-8.2.9/tests/resources/data_entity/assets/summary/timestamp.json
+-rw-rw-rw-   0 root         (0) root         (0)       52 2023-03-29 09:16:01.000000 superwise-8.2.9/tests/resources/data_entity/assets/summary/unknown.json
+-rw-rw-rw-   0 root         (0) root         (0)     1373 2023-03-29 09:16:01.000000 superwise-8.2.9/tests/resources/data_entity/expected_infer.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 09:17:11.000000 superwise-8.2.9/tests/resources/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-29 09:16:01.000000 superwise-8.2.9/tests/resources/dataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       54 2023-03-29 09:16:01.000000 superwise-8.2.9/tests/resources/dataset/test.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 09:17:11.000000 superwise-8.2.9/tests/resources/internal_sdk/
+-rw-rw-rw-   0 root         (0) root         (0)     5890 2023-03-29 09:16:01.000000 superwise-8.2.9/tests/resources/internal_sdk/basic_schema.json
+-rw-rw-rw-   0 root         (0) root         (0)     5890 2023-03-29 09:16:01.000000 superwise-8.2.9/tests/resources/internal_sdk/basic_schema_todel.json
+-rw-rw-rw-   0 root         (0) root         (0)     6215 2023-03-29 09:16:01.000000 superwise-8.2.9/tests/resources/internal_sdk/basic_schema_too_much_dimension.json
+-rw-rw-rw-   0 root         (0) root         (0)    35657 2023-03-29 09:16:01.000000 superwise-8.2.9/tests/resources/internal_sdk/data.json
+-rw-rw-rw-   0 root         (0) root         (0)     5030 2023-03-29 09:16:01.000000 superwise-8.2.9/tests/resources/internal_sdk/data_basic.json
+-rw-rw-rw-   0 root         (0) root         (0)    35577 2023-03-29 09:16:01.000000 superwise-8.2.9/tests/resources/internal_sdk/data_bool.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 09:17:11.000000 superwise-8.2.9/tests/resources/transaction/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-03-29 09:16:01.000000 superwise-8.2.9/tests/resources/transaction/local_records_file.json
+-rw-rw-rw-   0 root         (0) root         (0)      326 2023-03-29 09:16:01.000000 superwise-8.2.9/tests/resources/transaction/records_payload.json
+-rw-rw-rw-   0 root         (0) root         (0)     7358 2023-03-29 09:16:01.000000 superwise-8.2.9/tests/test_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     2424 2023-03-29 09:16:01.000000 superwise-8.2.9/tests/test_e2e.py
+-rw-rw-rw-   0 root         (0) root         (0)     7895 2023-03-29 09:16:01.000000 superwise-8.2.9/tests/test_entity_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)     3714 2023-03-29 09:16:01.000000 superwise-8.2.9/tests/test_http_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1833 2023-03-29 09:16:01.000000 superwise-8.2.9/tests/test_infer_unit.py
+-rw-rw-rw-   0 root         (0) root         (0)     5603 2023-03-29 09:16:01.000000 superwise-8.2.9/tests/test_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     3158 2023-03-29 09:16:01.000000 superwise-8.2.9/tests/test_notification.py
+-rw-rw-rw-   0 root         (0) root         (0)     2461 2023-03-29 09:16:01.000000 superwise-8.2.9/tests/test_projects.py
+-rw-rw-rw-   0 root         (0) root         (0)     5022 2023-03-29 09:16:01.000000 superwise-8.2.9/tests/test_segments.py
+-rw-rw-rw-   0 root         (0) root         (0)     3744 2023-03-29 09:16:01.000000 superwise-8.2.9/tests/test_summary_unit.py
+-rw-rw-rw-   0 root         (0) root         (0)     6636 2023-03-29 09:16:01.000000 superwise-8.2.9/tests/test_transaction.py
+-rw-rw-rw-   0 root         (0) root         (0)     8558 2023-03-29 09:16:01.000000 superwise-8.2.9/tests/test_version.py
```

### Comparing `superwise-8.2.8/.pre-commit-config.yaml` & `superwise-8.2.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/CHANGELOG.md` & `superwise-8.2.9/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/LICENCE` & `superwise-8.2.9/LICENCE`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/PKG-INFO` & `superwise-8.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superwise
-Version: 8.2.8
+Version: 8.2.9
 Summary: Superwise SDK
 Home-page: https://docs.superwise.ai/docs/python-sdk
 Author: Superwise.ai
 Author-email: tech@superwise.com
 License: MIT
 Description: # Superwise Python SDK
```

### Comparing `superwise-8.2.8/README.md` & `superwise-8.2.9/README.md`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/assets/favicon.png` & `superwise-8.2.9/assets/favicon.png`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/assets/image.png` & `superwise-8.2.9/assets/image.png`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/assets/superwise.png` & `superwise-8.2.9/assets/superwise.png`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/docs.py` & `superwise-8.2.9/docs.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/mkdocs.yml` & `superwise-8.2.9/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/setup.py` & `superwise-8.2.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("superwise/requirements.txt", "r") as f:
     requirements = [x.strip() for x in f.readlines()]
 
 setuptools.setup(
     name="superwise",
-    version="8.2.8",
+    version="8.2.9",
     description="Superwise SDK",
     url="https://docs.superwise.ai/docs/python-sdk",
     author="Superwise.ai",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email="tech@superwise.com",
     license="MIT",
```

### Comparing `superwise-8.2.8/superwise/__init__.py` & `superwise-8.2.9/superwise/__init__.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/superwise/config.py` & `superwise-8.2.9/superwise/config.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/superwise/controller/base.py` & `superwise-8.2.9/superwise/controller/base.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/superwise/controller/dataentity.py` & `superwise-8.2.9/superwise/controller/dataentity.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/superwise/controller/dataset.py` & `superwise-8.2.9/superwise/controller/dataset.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/superwise/controller/infer.py` & `superwise-8.2.9/superwise/controller/infer.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/superwise/controller/model.py` & `superwise-8.2.9/superwise/controller/model.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/superwise/controller/notification.py` & `superwise-8.2.9/superwise/controller/notification.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/superwise/controller/policy.py` & `superwise-8.2.9/superwise/controller/policy.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/superwise/controller/role.py` & `superwise-8.2.9/superwise/controller/role.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/superwise/controller/summary/boolean_summary_generator.py` & `superwise-8.2.9/superwise/controller/summary/boolean_summary_generator.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/superwise/controller/summary/categorical_summary_generator.py` & `superwise-8.2.9/superwise/controller/summary/categorical_summary_generator.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/superwise/controller/summary/entities_validator.py` & `superwise-8.2.9/superwise/controller/summary/entities_validator.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/superwise/controller/summary/entity_summary_generator.py` & `superwise-8.2.9/superwise/controller/summary/entity_summary_generator.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/superwise/controller/summary/feature_importance.py` & `superwise-8.2.9/superwise/controller/summary/feature_importance.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/superwise/controller/summary/numeric_summary_generator.py` & `superwise-8.2.9/superwise/controller/summary/numeric_summary_generator.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/superwise/controller/summary/summary.py` & `superwise-8.2.9/superwise/controller/summary/summary.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/superwise/controller/transaction.py` & `superwise-8.2.9/superwise/controller/transaction.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/superwise/controller/version.py` & `superwise-8.2.9/superwise/controller/version.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/superwise/models/base.py` & `superwise-8.2.9/superwise/models/base.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/superwise/models/data_entity.py` & `superwise-8.2.9/superwise/models/data_entity.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/superwise/models/dataset.py` & `superwise-8.2.9/superwise/models/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,22 +14,22 @@
 class Dataset(BaseModel):
     """DataSet"""
 
     _from_dataframe = False
     _tempfile_path = None
 
     def __init__(
-            self,
-            name: str,
-            files: Union[str, List[str]],
-            project_id: int,
-            type: Union[DatasetType, str] = DatasetType.TRAIN,
-            dtypes: Dict[str, str] = None,
-            roles: Dict[str, str] = None,
-            **kwargs
+        self,
+        name: str,
+        files: Union[str, List[str]],
+        project_id: int,
+        type: Union[DatasetType, str] = DatasetType.TRAIN,
+        dtypes: Dict[str, str] = None,
+        roles: Dict[str, str] = None,
+        **kwargs
     ):
         """
         ### Description:
 
         Constructor for Dataset class
 
         ### Args:
```

### Comparing `superwise-8.2.8/superwise/models/model.py` & `superwise-8.2.9/superwise/models/model.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/superwise/models/notification.py` & `superwise-8.2.9/superwise/models/notification.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/superwise/models/project.py` & `superwise-8.2.9/superwise/models/project.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/superwise/models/role.py` & `superwise-8.2.9/superwise/models/role.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/superwise/models/segment.py` & `superwise-8.2.9/superwise/models/segment.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/superwise/models/transaction.py` & `superwise-8.2.9/superwise/models/transaction.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/superwise/models/validation_error.py` & `superwise-8.2.9/superwise/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/superwise/models/version.py` & `superwise-8.2.9/superwise/models/version.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/superwise/resources/superwise_enums.py` & `superwise-8.2.9/superwise/resources/superwise_enums.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/superwise/utils/client.py` & `superwise-8.2.9/superwise/utils/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,14 @@
         self._accessToken = None
         self._accessToken = self.get_access_token()
         self._refreshToken = None
         self._expires = None
         self._expiresIn = None
         self.tenant_id = self.get_tenant_id(self.accessToken)
         self.logger = logger
-        self.headers = self.build_headers()
 
     def get_access_token(self):
         if self._accessToken is not None:
             return self._accessToken
         return self.get_token().get("accessToken", None)
 
     def get_tenant_id(self, token) -> str:
@@ -316,7 +315,8 @@
         ### Return:
 
         URL string
         """
         return "https://{}/{}/{}".format(self.api_host, self.tenant_id, path)
 
     accessToken = property(get_access_token)
+    headers = property(build_headers)
```

### Comparing `superwise-8.2.8/superwise/utils/exceptions.py` & `superwise-8.2.9/superwise/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/superwise/utils/storage/__init__.py` & `superwise-8.2.9/superwise/utils/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/superwise/utils/storage/azure_storage.py` & `superwise-8.2.9/superwise/utils/storage/azure_storage.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/superwise/utils/storage/dataframe.py` & `superwise-8.2.9/superwise/utils/storage/dataframe.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/superwise/utils/storage/gcs.py` & `superwise-8.2.9/superwise/utils/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/superwise/utils/storage/internal_storage/aws.py` & `superwise-8.2.9/superwise/utils/storage/internal_storage/aws.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/superwise/utils/storage/internal_storage/azure.py` & `superwise-8.2.9/superwise/utils/storage/internal_storage/azure.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/superwise/utils/storage/internal_storage/gcs.py` & `superwise-8.2.9/superwise/utils/storage/internal_storage/gcs.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/superwise/utils/storage/internal_storage/internal_storage.py` & `superwise-8.2.9/superwise/utils/storage/internal_storage/internal_storage.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/superwise/utils/storage/internal_storage/internal_storage_factory.py` & `superwise-8.2.9/superwise/utils/storage/internal_storage/internal_storage_factory.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/superwise/utils/storage/s3.py` & `superwise-8.2.9/superwise/utils/storage/s3.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/superwise.egg-info/PKG-INFO` & `superwise-8.2.9/superwise.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superwise
-Version: 8.2.8
+Version: 8.2.9
 Summary: Superwise SDK
 Home-page: https://docs.superwise.ai/docs/python-sdk
 Author: Superwise.ai
 Author-email: tech@superwise.com
 License: MIT
 Description: # Superwise Python SDK
```

### Comparing `superwise-8.2.8/superwise.egg-info/SOURCES.txt` & `superwise-8.2.9/superwise.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/tests/__init__.py` & `superwise-8.2.9/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/tests/conftest.py` & `superwise-8.2.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/tests/resources/basic_schema.json` & `superwise-8.2.9/tests/resources/basic_schema.json`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/tests/resources/data.json` & `superwise-8.2.9/tests/resources/data.json`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/tests/resources/data_entity/assets/baseline/basic_baseline.json` & `superwise-8.2.9/tests/resources/data_entity/assets/baseline/basic_baseline.json`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/tests/resources/data_entity/assets/baseline/basic_schema.json` & `superwise-8.2.9/tests/resources/data_entity/assets/baseline/basic_schema.json`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/tests/resources/data_entity/assets/entities.json` & `superwise-8.2.9/tests/resources/data_entity/assets/entities.json`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/tests/resources/data_entity/assets/entities_with_feature_importance.json` & `superwise-8.2.9/tests/resources/data_entity/assets/entities_with_feature_importance.json`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/tests/resources/data_entity/assets/entity_with_feature_importance.json` & `superwise-8.2.9/tests/resources/data_entity/assets/entity_with_feature_importance.json`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/tests/resources/data_entity/assets/patched_response.json` & `superwise-8.2.9/tests/resources/data_entity/assets/patched_response.json`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/tests/resources/data_entity/assets/summary/numeric/num_centered.json` & `superwise-8.2.9/tests/resources/data_entity/assets/summary/numeric/num_centered.json`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/tests/resources/data_entity/assets/summary/numeric/num_left_tail.json` & `superwise-8.2.9/tests/resources/data_entity/assets/summary/numeric/num_left_tail.json`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/tests/resources/data_entity/assets/summary/numeric/num_right_tail.json` & `superwise-8.2.9/tests/resources/data_entity/assets/summary/numeric/num_right_tail.json`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/tests/resources/data_entity/assets/summary/numeric/with_previous/num_centered.json` & `superwise-8.2.9/tests/resources/data_entity/assets/summary/numeric/with_previous/num_centered.json`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/tests/resources/data_entity/assets/summary/numeric/with_previous/num_left_tail.json` & `superwise-8.2.9/tests/resources/data_entity/assets/summary/numeric/with_previous/num_left_tail.json`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/tests/resources/data_entity/assets/summary/numeric/with_previous/num_right_tail.json` & `superwise-8.2.9/tests/resources/data_entity/assets/summary/numeric/with_previous/num_right_tail.json`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/tests/resources/data_entity/expected_infer.json` & `superwise-8.2.9/tests/resources/data_entity/expected_infer.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -1,22 +1,22 @@
 {
+    "F0": "Numeric",
     "binary_bool_full": "Boolean",
     "binary_bool_null": "Boolean",
     "binary_float_full": "Boolean",
     "binary_float_null": "Boolean",
     "binary_str_full": "Boolean",
     "binary_str_null": "Boolean",
     "cat_int_full": "Numeric",
     "cat_int_null": "Categorical",
     "cat_str_full": "Numeric",
     "cat_str_null": "Numeric",
     "const_full": "Numeric",
     "const_null": "Boolean",
     "est_country": "Categorical",
-    "F0": "Numeric",
     "f1": "Numeric",
     "f10": "Numeric",
     "f11": "Numeric",
     "f12": "Numeric",
     "f16": "Numeric",
     "f17": "Categorical",
     "f18": "Numeric",
```

### Comparing `superwise-8.2.8/tests/resources/internal_sdk/basic_schema.json` & `superwise-8.2.9/tests/resources/internal_sdk/basic_schema.json`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/tests/resources/internal_sdk/basic_schema_todel.json` & `superwise-8.2.9/tests/resources/internal_sdk/basic_schema_todel.json`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/tests/resources/internal_sdk/basic_schema_too_much_dimension.json` & `superwise-8.2.9/tests/resources/internal_sdk/basic_schema_too_much_dimension.json`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/tests/resources/internal_sdk/data.json` & `superwise-8.2.9/tests/resources/internal_sdk/data.json`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/tests/resources/internal_sdk/data_basic.json` & `superwise-8.2.9/tests/resources/internal_sdk/data_basic.json`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/tests/resources/internal_sdk/data_bool.json` & `superwise-8.2.9/tests/resources/internal_sdk/data_bool.json`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/tests/test_dataset.py` & `superwise-8.2.9/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/tests/test_e2e.py` & `superwise-8.2.9/tests/test_e2e.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/tests/test_entity_validator.py` & `superwise-8.2.9/tests/test_entity_validator.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/tests/test_http_client.py` & `superwise-8.2.9/tests/test_http_client.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/tests/test_infer_unit.py` & `superwise-8.2.9/tests/test_infer_unit.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/tests/test_models.py` & `superwise-8.2.9/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/tests/test_notification.py` & `superwise-8.2.9/tests/test_notification.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/tests/test_projects.py` & `superwise-8.2.9/tests/test_projects.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/tests/test_segments.py` & `superwise-8.2.9/tests/test_segments.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/tests/test_summary_unit.py` & `superwise-8.2.9/tests/test_summary_unit.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/tests/test_transaction.py` & `superwise-8.2.9/tests/test_transaction.py`

 * *Files identical despite different names*

### Comparing `superwise-8.2.8/tests/test_version.py` & `superwise-8.2.9/tests/test_version.py`

 * *Files identical despite different names*

