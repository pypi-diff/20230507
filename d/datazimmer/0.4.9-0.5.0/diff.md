# Comparing `tmp/datazimmer-0.4.9.tar.gz` & `tmp/datazimmer-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datazimmer-0.4.9.tar", last modified: Wed Jan 18 17:03:42 2023, max compression
+gzip compressed data, was "datazimmer-0.5.0.tar", last modified: Sun May  7 14:13:03 2023, max compression
```

## Comparing `datazimmer-0.4.9.tar` & `datazimmer-0.5.0.tar`

### file list

```diff
@@ -1,141 +1,146 @@
--rw-r--r--   0        0        0      976 2023-01-18 17:03:38.602541 datazimmer-0.4.9/.github/workflows/compatibility_test.yml
--rw-r--r--   0        0        0     1228 2023-01-18 17:03:38.602541 datazimmer-0.4.9/.github/workflows/test.yml
--rw-r--r--   0        0        0      565 2023-01-18 17:03:38.602541 datazimmer-0.4.9/.github/workflows/twine_release.yml
--rw-r--r--   0        0        0     1795 2023-01-18 17:03:38.602541 datazimmer-0.4.9/.gitignore
--rw-r--r--   0        0        0      288 2023-01-18 17:03:38.602541 datazimmer-0.4.9/.readthedocs.yml
--rw-r--r--   0        0        0      491 2023-01-18 17:03:38.602541 datazimmer-0.4.9/CITATION.cff
--rw-r--r--   0        0        0     1077 2023-01-18 17:03:38.602541 datazimmer-0.4.9/LICENSE
--rw-r--r--   0        0        0     2877 2023-01-18 17:03:38.602541 datazimmer-0.4.9/README.md
--rw-r--r--   0        0        0     3713 2023-01-18 17:03:38.602541 datazimmer-0.4.9/conftest.py
--rw-r--r--   0        0        0      624 2023-01-18 17:03:38.602541 datazimmer-0.4.9/datazimmer/__init__.py
--rw-r--r--   0        0        0     3316 2023-01-18 17:03:38.602541 datazimmer-0.4.9/datazimmer/aswan_integration.py
--rw-r--r--   0        0        0     7970 2023-01-18 17:03:38.602541 datazimmer-0.4.9/datazimmer/config_loading.py
--rw-r--r--   0        0        0      102 2023-01-18 17:03:38.602541 datazimmer-0.4.9/datazimmer/exceptions.py
--rw-r--r--   0        0        0    14626 2023-01-18 17:03:38.602541 datazimmer-0.4.9/datazimmer/explorer.py
--rw-r--r--   0        0        0      624 2023-01-18 17:03:38.602541 datazimmer-0.4.9/datazimmer/get_runtime.py
--rw-r--r--   0        0        0     3197 2023-01-18 17:03:38.602541 datazimmer-0.4.9/datazimmer/gh_actions.py
--rw-r--r--   0        0        0        0 2023-01-18 17:03:38.602541 datazimmer-0.4.9/datazimmer/metadata/__init__.py
--rw-r--r--   0        0        0     3155 2023-01-18 17:03:38.602541 datazimmer-0.4.9/datazimmer/metadata/atoms.py
--rw-r--r--   0        0        0     1344 2023-01-18 17:03:38.602541 datazimmer-0.4.9/datazimmer/metadata/complete_id.py
--rw-r--r--   0        0        0     1744 2023-01-18 17:03:38.602541 datazimmer-0.4.9/datazimmer/metadata/datascript.py
--rw-r--r--   0        0        0     4538 2023-01-18 17:03:38.602541 datazimmer-0.4.9/datazimmer/metadata/high_level.py
--rw-r--r--   0        0        0     6668 2023-01-18 17:03:38.602541 datazimmer-0.4.9/datazimmer/metadata/scrutable.py
--rw-r--r--   0        0        0     3371 2023-01-18 17:03:38.602541 datazimmer-0.4.9/datazimmer/naming.py
--rw-r--r--   0        0        0     1318 2023-01-18 17:03:38.602541 datazimmer-0.4.9/datazimmer/nb_generator.py
--rw-r--r--   0        0        0      526 2023-01-18 17:03:38.602541 datazimmer-0.4.9/datazimmer/persistent_state.py
--rw-r--r--   0        0        0     8136 2023-01-18 17:03:38.602541 datazimmer-0.4.9/datazimmer/pipeline_element.py
--rw-r--r--   0        0        0     7718 2023-01-18 17:03:38.602541 datazimmer-0.4.9/datazimmer/project_runtime.py
--rw-r--r--   0        0        0      935 2023-01-18 17:03:38.602541 datazimmer-0.4.9/datazimmer/raw_data.py
--rw-r--r--   0        0        0     6107 2023-01-18 17:03:38.602541 datazimmer-0.4.9/datazimmer/registry.py
--rw-r--r--   0        0        0      713 2023-01-18 17:03:38.602541 datazimmer-0.4.9/datazimmer/reporting.py
--rw-r--r--   0        0        0        0 2023-01-18 17:03:38.602541 datazimmer-0.4.9/datazimmer/sql/__init__.py
--rw-r--r--   0        0        0       87 2023-01-18 17:03:38.602541 datazimmer-0.4.9/datazimmer/sql/draw.py
--rw-r--r--   0        0        0     9260 2023-01-18 17:03:38.602541 datazimmer-0.4.9/datazimmer/sql/loader.py
--rw-r--r--   0        0        0        0 2023-01-18 17:03:38.602541 datazimmer-0.4.9/datazimmer/tests/__init__.py
--rw-r--r--   0        0        0     6124 2023-01-18 17:03:38.602541 datazimmer-0.4.9/datazimmer/tests/create_dogshow.py
--rw-r--r--   0        0        0      346 2023-01-18 17:03:38.602541 datazimmer-0.4.9/datazimmer/tests/test_config.py
--rw-r--r--   0        0        0     3086 2023-01-18 17:03:38.602541 datazimmer-0.4.9/datazimmer/tests/test_full_integration.py
--rw-r--r--   0        0        0      437 2023-01-18 17:03:38.606541 datazimmer-0.4.9/datazimmer/tests/test_registry.py
--rw-r--r--   0        0        0      350 2023-01-18 17:03:38.606541 datazimmer-0.4.9/datazimmer/tests/test_runtime.py
--rw-r--r--   0        0        0     1819 2023-01-18 17:03:38.606541 datazimmer-0.4.9/datazimmer/tests/test_scrutable.py
--rw-r--r--   0        0        0      152 2023-01-18 17:03:38.606541 datazimmer-0.4.9/datazimmer/tests/test_sql.py
--rw-r--r--   0        0        0      235 2023-01-18 17:03:38.606541 datazimmer-0.4.9/datazimmer/tests/test_util.py
--rw-r--r--   0        0        0      943 2023-01-18 17:03:38.606541 datazimmer-0.4.9/datazimmer/tests/test_validation.py
--rw-r--r--   0        0        0     8534 2023-01-18 17:03:38.606541 datazimmer-0.4.9/datazimmer/typer_commands.py
--rw-r--r--   0        0        0     3125 2023-01-18 17:03:38.606541 datazimmer-0.4.9/datazimmer/utils.py
--rw-r--r--   0        0        0     2877 2023-01-18 17:03:38.606541 datazimmer-0.4.9/datazimmer/validation_functions.py
--rw-r--r--   0        0        0     9464 2023-01-18 17:03:38.606541 datazimmer-0.4.9/datazimmer/zenodo.py
--rw-r--r--   0        0        0      114 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/api/datazimmer.AbstractEntity.rst
--rw-r--r--   0        0        0      123 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/api/datazimmer.CompositeTypeBase.rst
--rw-r--r--   0        0        0      746 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/api/datazimmer.DzAswan.rst
--rw-r--r--   0        0        0      269 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/api/datazimmer.EntityClass.rst
--rw-r--r--   0        0        0       87 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/api/datazimmer.Index.rst
--rw-r--r--   0        0        0       96 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/api/datazimmer.Nullable.rst
--rw-r--r--   0        0        0      444 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/api/datazimmer.PersistentState.rst
--rw-r--r--   0        0        0      592 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/api/datazimmer.ReportFile.rst
--rw-r--r--   0        0        0      565 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/api/datazimmer.ScruTable.rst
--rw-r--r--   0        0        0       99 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/api/datazimmer.SourceUrl.rst
--rw-r--r--   0        0        0      107 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/api/datazimmer.dump_dfs_to_tables.rst
--rw-r--r--   0        0        0      104 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/api/datazimmer.get_raw_data_path.rst
--rw-r--r--   0        0        0       77 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/api/datazimmer.register.rst
--rw-r--r--   0        0        0      113 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/api/datazimmer.register_data_loader.rst
--rw-r--r--   0        0        0      113 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/api/datazimmer.register_env_creator.rst
--rw-r--r--   0        0        0       39 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/autosumm.rst
--rw-r--r--   0        0        0     2402 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/conf.py
--rw-r--r--   0        0        0      263 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/index.rst
--rw-r--r--   0        0        0       77 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/notebooks/doc-001-intro.rst
--rw-r--r--   0        0        0     4171 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/notebooks/doc-002-glossary.rst
--rw-r--r--   0        0        0      616 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/notebooks/doc-003-mock-projects.rst
--rw-r--r--   0        0        0     1269 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/notebooks/doc-004-rules-conventions.rst
--rw-r--r--   0        0        0      284 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/notebooks/doc-005-cli.rst
--rw-r--r--   0        0        0      102 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/release_notes/main.rst
--rw-r--r--   0        0        0       45 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/release_notes/v0.1.0.rst
--rw-r--r--   0        0        0       46 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/release_notes/v0.1.1.rst
--rw-r--r--   0        0        0       27 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/release_notes/v0.1.2.rst
--rw-r--r--   0        0        0       15 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/release_notes/v0.1.3.rst
--rw-r--r--   0        0        0       15 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/release_notes/v0.1.4.rst
--rw-r--r--   0        0        0       15 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/release_notes/v0.1.5.rst
--rw-r--r--   0        0        0       34 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/release_notes/v0.2.1.rst
--rw-r--r--   0        0        0       31 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/release_notes/v0.2.2.rst
--rw-r--r--   0        0        0       31 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/release_notes/v0.2.3.rst
--rw-r--r--   0        0        0       31 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/release_notes/v0.2.4.rst
--rw-r--r--   0        0        0       29 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/release_notes/v0.2.5.rst
--rw-r--r--   0        0        0       39 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/release_notes/v0.2.6.rst
--rw-r--r--   0        0        0       34 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/release_notes/v0.2.7.rst
--rw-r--r--   0        0        0       45 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/release_notes/v0.3.0.rst
--rw-r--r--   0        0        0       32 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/release_notes/v0.3.1.rst
--rw-r--r--   0        0        0       48 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/release_notes/v0.3.10.rst
--rw-r--r--   0        0        0       47 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/release_notes/v0.3.2.rst
--rw-r--r--   0        0        0       39 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/release_notes/v0.3.3.rst
--rw-r--r--   0        0        0       33 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/release_notes/v0.3.4.rst
--rw-r--r--   0        0        0       34 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/release_notes/v0.3.5.rst
--rw-r--r--   0        0        0       32 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/release_notes/v0.3.6.rst
--rw-r--r--   0        0        0       32 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/release_notes/v0.3.7.rst
--rw-r--r--   0        0        0       31 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/release_notes/v0.3.8.rst
--rw-r--r--   0        0        0       35 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/release_notes/v0.3.9.rst
--rw-r--r--   0        0        0       37 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/release_notes/v0.4.0.rst
--rw-r--r--   0        0        0       32 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/release_notes/v0.4.1.rst
--rw-r--r--   0        0        0       52 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/release_notes/v0.4.2.rst
--rw-r--r--   0        0        0       66 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/release_notes/v0.4.3.rst
--rw-r--r--   0        0        0       53 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/release_notes/v0.4.4.rst
--rw-r--r--   0        0        0       45 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/release_notes/v0.4.5.rst
--rw-r--r--   0        0        0       41 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/release_notes/v0.4.6.rst
--rw-r--r--   0        0        0       71 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/release_notes/v0.4.7.rst
--rw-r--r--   0        0        0       47 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/release_notes/v0.4.8.rst
--rw-r--r--   0        0        0       53 2023-01-18 17:03:38.606541 datazimmer-0.4.9/docs/release_notes/v0.4.9.rst
--rw-r--r--   0        0        0      159 2023-01-18 17:03:38.606541 datazimmer-0.4.9/dogshow/confs.yaml
--rw-r--r--   0        0        0     1773 2023-01-18 17:03:38.606541 datazimmer-0.4.9/dogshow/data/photo.csv
--rw-r--r--   0        0        0     3459 2023-01-18 17:03:38.606541 datazimmer-0.4.9/dogshow/explorer/dec-setup/dog_one/sexes.ipynb
--rw-r--r--   0        0        0      655 2023-01-18 17:03:38.606541 datazimmer-0.4.9/dogshow/explorer/dec.yaml
--rw-r--r--   0        0        0      186 2023-01-18 17:03:38.606541 datazimmer-0.4.9/dogshow/explorer2/dec.yaml
--rw-r--r--   0        0        0      655 2023-01-18 17:03:38.606541 datazimmer-0.4.9/dogshow/minimal.py
--rw-r--r--   0        0        0     9861 2023-01-18 17:03:38.606541 datazimmer-0.4.9/dogshow/projects/cc-dog-raw/{{cookiecutter.project}}/notebooks/create-dogshow-test-data.ipynb
--rw-r--r--   0        0        0       57 2023-01-18 17:03:38.606541 datazimmer-0.4.9/dogshow/projects/cc-dog-raw/{{cookiecutter.project}}/zimmer.yaml
--rw-r--r--   0        0        0        0 2023-01-18 17:03:38.606541 datazimmer-0.4.9/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/__init__.py
--rw-r--r--   0        0        0        0 2023-01-18 17:03:38.606541 datazimmer-0.4.9/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/__init__.py
--rw-r--r--   0        0        0     2304 2023-01-18 17:03:38.606541 datazimmer-0.4.9/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/create_envs.py
--rw-r--r--   0        0        0     1566 2023-01-18 17:03:38.606541 datazimmer-0.4.9/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/ns_meta.py
--rw-r--r--   0        0        0     3192 2023-01-18 17:03:38.606541 datazimmer-0.4.9/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/update_data.py
--rw-r--r--   0        0        0      307 2023-01-18 17:03:38.606541 datazimmer-0.4.9/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/zimmer.yaml
--rw-r--r--   0        0        0        0 2023-01-18 17:03:38.606541 datazimmer-0.4.9/dogshow/projects/cc-dogcombine/{{cookiecutter.project}}/src/__init__.py
--rw-r--r--   0        0        0      674 2023-01-18 17:03:38.606541 datazimmer-0.4.9/dogshow/projects/cc-dogcombine/{{cookiecutter.project}}/src/joint_success.py
--rw-r--r--   0        0        0      261 2023-01-18 17:03:38.606541 datazimmer-0.4.9/dogshow/projects/cc-dogcombine/{{cookiecutter.project}}/zimmer.yaml
--rw-r--r--   0        0        0        0 2023-01-18 17:03:38.606541 datazimmer-0.4.9/dogshow/projects/cc-dograce/{{cookiecutter.project}}/src/__init__.py
--rw-r--r--   0        0        0     2530 2023-01-18 17:03:38.606541 datazimmer-0.4.9/dogshow/projects/cc-dograce/{{cookiecutter.project}}/src/core.py
--rw-r--r--   0        0        0      120 2023-01-18 17:03:38.606541 datazimmer-0.4.9/dogshow/projects/cc-dograce/{{cookiecutter.project}}/zimmer.yaml
--rw-r--r--   0        0        0        0 2023-01-18 17:03:38.606541 datazimmer-0.4.9/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/__init__.py
--rw-r--r--   0        0        0       65 2023-01-18 17:03:38.606541 datazimmer-0.4.9/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/counts/__init__.py
--rw-r--r--   0        0        0      421 2023-01-18 17:03:38.606541 datazimmer-0.4.9/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/counts/meta.py
--rw-r--r--   0        0        0      945 2023-01-18 17:03:38.606541 datazimmer-0.4.9/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/counts/proc.py
--rw-r--r--   0        0        0     1093 2023-01-18 17:03:38.606541 datazimmer-0.4.9/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/sex_matches.py
--rw-r--r--   0        0        0     2415 2023-01-18 17:03:38.606541 datazimmer-0.4.9/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/success.py
--rw-r--r--   0        0        0      810 2023-01-18 17:03:38.606541 datazimmer-0.4.9/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/top_report.py
--rw-r--r--   0        0        0      575 2023-01-18 17:03:38.606541 datazimmer-0.4.9/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/zimmer.yaml
--rw-r--r--   0        0        0     2940 2023-01-18 17:03:38.606541 datazimmer-0.4.9/dogshow/todo/complex_success.py
--rw-r--r--   0        0        0      612 2023-01-18 17:03:38.606541 datazimmer-0.4.9/notebooks/doc-001-intro.ipynb
--rw-r--r--   0        0        0     5328 2023-01-18 17:03:38.606541 datazimmer-0.4.9/notebooks/doc-002-glossary.ipynb
--rw-r--r--   0        0        0     1877 2023-01-18 17:03:38.606541 datazimmer-0.4.9/notebooks/doc-003-mock-projects.ipynb
--rw-r--r--   0        0        0     1928 2023-01-18 17:03:38.606541 datazimmer-0.4.9/notebooks/doc-004-rules-conventions.ipynb
--rw-r--r--   0        0        0     1235 2023-01-18 17:03:38.606541 datazimmer-0.4.9/notebooks/doc-005-cli.ipynb
--rw-r--r--   0        0        0     1253 2023-01-18 17:03:38.606541 datazimmer-0.4.9/pyproject.toml
--rw-r--r--   0        0        0     4579 1970-01-01 00:00:00.000000 datazimmer-0.4.9/PKG-INFO
+-rw-r--r--   0        0        0     1003 2023-05-07 14:12:58.174204 datazimmer-0.5.0/.github/workflows/compatibility_test.yml
+-rw-r--r--   0        0        0     1299 2023-05-07 14:12:58.174204 datazimmer-0.5.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      565 2023-05-07 14:12:58.174204 datazimmer-0.5.0/.github/workflows/twine_release.yml
+-rw-r--r--   0        0        0     1795 2023-05-07 14:12:58.174204 datazimmer-0.5.0/.gitignore
+-rw-r--r--   0        0        0      288 2023-05-07 14:12:58.174204 datazimmer-0.5.0/.readthedocs.yml
+-rw-r--r--   0        0        0      491 2023-05-07 14:12:58.174204 datazimmer-0.5.0/CITATION.cff
+-rw-r--r--   0        0        0     1077 2023-05-07 14:12:58.174204 datazimmer-0.5.0/LICENSE
+-rw-r--r--   0        0        0     3122 2023-05-07 14:12:58.174204 datazimmer-0.5.0/README.md
+-rw-r--r--   0        0        0     3754 2023-05-07 14:12:58.174204 datazimmer-0.5.0/conftest.py
+-rw-r--r--   0        0        0      634 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/__init__.py
+-rw-r--r--   0        0        0     3363 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/aswan_integration.py
+-rw-r--r--   0        0        0     7997 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/config_loading.py
+-rw-r--r--   0        0        0      102 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/exceptions.py
+-rw-r--r--   0        0        0      624 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/get_runtime.py
+-rw-r--r--   0        0        0     2420 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/gh_actions.py
+-rw-r--r--   0        0        0        0 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/metadata/__init__.py
+-rw-r--r--   0        0        0     6235 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/metadata/atoms.py
+-rw-r--r--   0        0        0     1344 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/metadata/complete_id.py
+-rw-r--r--   0        0        0     1744 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/metadata/datascript.py
+-rw-r--r--   0        0        0     4537 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/metadata/high_level.py
+-rw-r--r--   0        0        0     4798 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/metadata/scrutable.py
+-rw-r--r--   0        0        0     3334 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/naming.py
+-rw-r--r--   0        0        0      526 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/persistent_state.py
+-rw-r--r--   0        0        0     8281 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/pipeline_element.py
+-rw-r--r--   0        0        0     7718 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/project_runtime.py
+-rw-r--r--   0        0        0      935 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/raw_data.py
+-rw-r--r--   0        0        0     6107 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/registry.py
+-rw-r--r--   0        0        0      713 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/reporting.py
+-rw-r--r--   0        0        0        0 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/sql/__init__.py
+-rw-r--r--   0        0        0       87 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/sql/draw.py
+-rw-r--r--   0        0        0     9253 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/sql/loader.py
+-rw-r--r--   0        0        0        0 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/tests/__init__.py
+-rw-r--r--   0        0        0     4692 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/tests/create_dogshow.py
+-rw-r--r--   0        0        0      845 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/tests/test_commands.py
+-rw-r--r--   0        0        0      346 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/tests/test_config.py
+-rw-r--r--   0        0        0     4264 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/tests/test_full_integration.py
+-rw-r--r--   0        0        0      465 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/tests/test_registry.py
+-rw-r--r--   0        0        0      294 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/tests/test_runtime.py
+-rw-r--r--   0        0        0     1799 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/tests/test_scrutable.py
+-rw-r--r--   0        0        0      152 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/tests/test_sql.py
+-rw-r--r--   0        0        0      235 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/tests/test_util.py
+-rw-r--r--   0        0        0      943 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/tests/test_validation.py
+-rw-r--r--   0        0        0      939 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/tests/util.py
+-rw-r--r--   0        0        0    10122 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/typer_commands.py
+-rw-r--r--   0        0        0     3260 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/utils.py
+-rw-r--r--   0        0        0     2877 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/validation_functions.py
+-rw-r--r--   0        0        0    10327 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/zenodo.py
+-rw-r--r--   0        0        0      114 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/api/datazimmer.AbstractEntity.rst
+-rw-r--r--   0        0        0      123 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/api/datazimmer.CompositeTypeBase.rst
+-rw-r--r--   0        0        0      746 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/api/datazimmer.DzAswan.rst
+-rw-r--r--   0        0        0      739 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/api/datazimmer.EntityClass.rst
+-rw-r--r--   0        0        0       87 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/api/datazimmer.Index.rst
+-rw-r--r--   0        0        0       96 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/api/datazimmer.Nullable.rst
+-rw-r--r--   0        0        0      444 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/api/datazimmer.PersistentState.rst
+-rw-r--r--   0        0        0      592 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/api/datazimmer.ReportFile.rst
+-rw-r--r--   0        0        0      565 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/api/datazimmer.ScruTable.rst
+-rw-r--r--   0        0        0       99 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/api/datazimmer.SourceUrl.rst
+-rw-r--r--   0        0        0      107 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/api/datazimmer.dump_dfs_to_tables.rst
+-rw-r--r--   0        0        0      104 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/api/datazimmer.get_raw_data_path.rst
+-rw-r--r--   0        0        0       77 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/api/datazimmer.parse_df.rst
+-rw-r--r--   0        0        0       77 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/api/datazimmer.register.rst
+-rw-r--r--   0        0        0      113 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/api/datazimmer.register_data_loader.rst
+-rw-r--r--   0        0        0      113 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/api/datazimmer.register_env_creator.rst
+-rw-r--r--   0        0        0       39 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/autosumm.rst
+-rw-r--r--   0        0        0     2402 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/conf.py
+-rw-r--r--   0        0        0      263 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/index.rst
+-rw-r--r--   0        0        0       77 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/notebooks/doc-001-intro.rst
+-rw-r--r--   0        0        0     4171 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/notebooks/doc-002-glossary.rst
+-rw-r--r--   0        0        0      616 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/notebooks/doc-003-mock-projects.rst
+-rw-r--r--   0        0        0     1269 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/notebooks/doc-004-rules-conventions.rst
+-rw-r--r--   0        0        0      284 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/notebooks/doc-005-cli.rst
+-rw-r--r--   0        0        0      102 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/main.rst
+-rw-r--r--   0        0        0       45 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.1.0.rst
+-rw-r--r--   0        0        0       46 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.1.1.rst
+-rw-r--r--   0        0        0       27 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.1.2.rst
+-rw-r--r--   0        0        0       15 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.1.3.rst
+-rw-r--r--   0        0        0       15 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.1.4.rst
+-rw-r--r--   0        0        0       15 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.1.5.rst
+-rw-r--r--   0        0        0       34 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.2.1.rst
+-rw-r--r--   0        0        0       31 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.2.2.rst
+-rw-r--r--   0        0        0       31 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.2.3.rst
+-rw-r--r--   0        0        0       31 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.2.4.rst
+-rw-r--r--   0        0        0       29 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.2.5.rst
+-rw-r--r--   0        0        0       39 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.2.6.rst
+-rw-r--r--   0        0        0       34 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.2.7.rst
+-rw-r--r--   0        0        0       45 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.3.0.rst
+-rw-r--r--   0        0        0       32 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.3.1.rst
+-rw-r--r--   0        0        0       48 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.3.10.rst
+-rw-r--r--   0        0        0       47 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.3.2.rst
+-rw-r--r--   0        0        0       39 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.3.3.rst
+-rw-r--r--   0        0        0       33 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.3.4.rst
+-rw-r--r--   0        0        0       34 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.3.5.rst
+-rw-r--r--   0        0        0       32 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.3.6.rst
+-rw-r--r--   0        0        0       32 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.3.7.rst
+-rw-r--r--   0        0        0       31 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.3.8.rst
+-rw-r--r--   0        0        0       35 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.3.9.rst
+-rw-r--r--   0        0        0       37 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.4.0.rst
+-rw-r--r--   0        0        0       32 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.4.1.rst
+-rw-r--r--   0        0        0       70 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.4.10.rst
+-rw-r--r--   0        0        0       55 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.4.11.rst
+-rw-r--r--   0        0        0       45 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.4.12.rst
+-rw-r--r--   0        0        0       68 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.4.13.rst
+-rw-r--r--   0        0        0       68 2023-05-07 14:12:58.178204 datazimmer-0.5.0/docs/release_notes/v0.4.14.rst
+-rw-r--r--   0        0        0       42 2023-05-07 14:12:58.178204 datazimmer-0.5.0/docs/release_notes/v0.4.15.rst
+-rw-r--r--   0        0        0       52 2023-05-07 14:12:58.178204 datazimmer-0.5.0/docs/release_notes/v0.4.2.rst
+-rw-r--r--   0        0        0       66 2023-05-07 14:12:58.178204 datazimmer-0.5.0/docs/release_notes/v0.4.3.rst
+-rw-r--r--   0        0        0       53 2023-05-07 14:12:58.178204 datazimmer-0.5.0/docs/release_notes/v0.4.4.rst
+-rw-r--r--   0        0        0       45 2023-05-07 14:12:58.178204 datazimmer-0.5.0/docs/release_notes/v0.4.5.rst
+-rw-r--r--   0        0        0       41 2023-05-07 14:12:58.178204 datazimmer-0.5.0/docs/release_notes/v0.4.6.rst
+-rw-r--r--   0        0        0       71 2023-05-07 14:12:58.178204 datazimmer-0.5.0/docs/release_notes/v0.4.7.rst
+-rw-r--r--   0        0        0       47 2023-05-07 14:12:58.178204 datazimmer-0.5.0/docs/release_notes/v0.4.8.rst
+-rw-r--r--   0        0        0       53 2023-05-07 14:12:58.178204 datazimmer-0.5.0/docs/release_notes/v0.4.9.rst
+-rw-r--r--   0        0        0       64 2023-05-07 14:12:58.178204 datazimmer-0.5.0/docs/release_notes/v0.5.0.rst
+-rw-r--r--   0        0        0      159 2023-05-07 14:12:58.178204 datazimmer-0.5.0/dogshow/confs.yaml
+-rw-r--r--   0        0        0     1773 2023-05-07 14:12:58.178204 datazimmer-0.5.0/dogshow/data/photo.csv
+-rw-r--r--   0        0        0      655 2023-05-07 14:12:58.178204 datazimmer-0.5.0/dogshow/minimal.py
+-rw-r--r--   0        0        0     9861 2023-05-07 14:12:58.178204 datazimmer-0.5.0/dogshow/projects/cc-dog-raw/{{cookiecutter.project}}/notebooks/create-dogshow-test-data.ipynb
+-rw-r--r--   0        0        0       57 2023-05-07 14:12:58.178204 datazimmer-0.5.0/dogshow/projects/cc-dog-raw/{{cookiecutter.project}}/zimmer.yaml
+-rw-r--r--   0        0        0        0 2023-05-07 14:12:58.178204 datazimmer-0.5.0/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-07 14:12:58.178204 datazimmer-0.5.0/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/__init__.py
+-rw-r--r--   0        0        0     2304 2023-05-07 14:12:58.178204 datazimmer-0.5.0/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/create_envs.py
+-rw-r--r--   0        0        0     1566 2023-05-07 14:12:58.178204 datazimmer-0.5.0/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/ns_meta.py
+-rw-r--r--   0        0        0     3192 2023-05-07 14:12:58.178204 datazimmer-0.5.0/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/update_data.py
+-rw-r--r--   0        0        0      307 2023-05-07 14:12:58.178204 datazimmer-0.5.0/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/zimmer.yaml
+-rw-r--r--   0        0        0        0 2023-05-07 14:12:58.178204 datazimmer-0.5.0/dogshow/projects/cc-dogcombine/{{cookiecutter.project}}/src/__init__.py
+-rw-r--r--   0        0        0      674 2023-05-07 14:12:58.178204 datazimmer-0.5.0/dogshow/projects/cc-dogcombine/{{cookiecutter.project}}/src/joint_success.py
+-rw-r--r--   0        0        0      261 2023-05-07 14:12:58.178204 datazimmer-0.5.0/dogshow/projects/cc-dogcombine/{{cookiecutter.project}}/zimmer.yaml
+-rw-r--r--   0        0        0        0 2023-05-07 14:12:58.178204 datazimmer-0.5.0/dogshow/projects/cc-dograce/{{cookiecutter.project}}/src/__init__.py
+-rw-r--r--   0        0        0     2533 2023-05-07 14:12:58.178204 datazimmer-0.5.0/dogshow/projects/cc-dograce/{{cookiecutter.project}}/src/core.py
+-rw-r--r--   0        0        0      120 2023-05-07 14:12:58.178204 datazimmer-0.5.0/dogshow/projects/cc-dograce/{{cookiecutter.project}}/zimmer.yaml
+-rw-r--r--   0        0        0        0 2023-05-07 14:12:58.178204 datazimmer-0.5.0/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/__init__.py
+-rw-r--r--   0        0        0       65 2023-05-07 14:12:58.178204 datazimmer-0.5.0/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/counts/__init__.py
+-rw-r--r--   0        0        0      421 2023-05-07 14:12:58.178204 datazimmer-0.5.0/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/counts/meta.py
+-rw-r--r--   0        0        0      945 2023-05-07 14:12:58.178204 datazimmer-0.5.0/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/counts/proc.py
+-rw-r--r--   0        0        0     1093 2023-05-07 14:12:58.178204 datazimmer-0.5.0/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/sex_matches.py
+-rw-r--r--   0        0        0     2415 2023-05-07 14:12:58.178204 datazimmer-0.5.0/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/success.py
+-rw-r--r--   0        0        0      810 2023-05-07 14:12:58.178204 datazimmer-0.5.0/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/top_report.py
+-rw-r--r--   0        0        0      575 2023-05-07 14:12:58.178204 datazimmer-0.5.0/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/zimmer.yaml
+-rw-r--r--   0        0        0     2940 2023-05-07 14:12:58.178204 datazimmer-0.5.0/dogshow/todo/complex_success.py
+-rw-r--r--   0        0        0      612 2023-05-07 14:12:58.178204 datazimmer-0.5.0/notebooks/doc-001-intro.ipynb
+-rw-r--r--   0        0        0     5328 2023-05-07 14:12:58.178204 datazimmer-0.5.0/notebooks/doc-002-glossary.ipynb
+-rw-r--r--   0        0        0     1877 2023-05-07 14:12:58.178204 datazimmer-0.5.0/notebooks/doc-003-mock-projects.ipynb
+-rw-r--r--   0        0        0     1928 2023-05-07 14:12:58.178204 datazimmer-0.5.0/notebooks/doc-004-rules-conventions.ipynb
+-rw-r--r--   0        0        0     1235 2023-05-07 14:12:58.178204 datazimmer-0.5.0/notebooks/doc-005-cli.ipynb
+-rw-r--r--   0        0        0     1121 2023-05-07 14:12:58.178204 datazimmer-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4513 1970-01-01 00:00:00.000000 datazimmer-0.5.0/PKG-INFO
```

### Comparing `datazimmer-0.4.9/.github/workflows/compatibility_test.yml` & `datazimmer-0.5.0/.github/workflows/compatibility_test.yml`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 name: OS Compatibility Test
 
 on:
   pull_request:
-    branches: 
+    branches:
       - main
   push:
     branches:
       - main
 
 jobs:
   comp_test:
     strategy:
       matrix:
-        os: [ubuntu-latest] # [windows-2022, windows-2019, macos-11, macos-10.15]
+        os: [ubuntu-latest, windows-2022, windows-2019, macos-11, macos-10.15]
     runs-on: ${{ matrix.os }}
     steps:
-    - uses: actions/checkout@v3
-    - uses: actions/setup-python@v4
-      with:
-        python-version: '3.10'
-    - name: Install dependencies
-      run: |
-        python -m pip install --upgrade pip
-        pip install -e .[test,profile,explorer,collect,zenodo]
-    - name: Setup Git
-      run: |
-        git config --global receive.denyCurrentBranch updateInstead
-        git config --global init.defaultBranch main
-        git config --global user.email "leo@dumbartonserum.com"
-        git config --global user.name "Leo Dumbarton"
-    - name: Test
-      env:
-        POSTGRES_HOST: sqlite
-        ZENODO_SANDBOX_TOKEN: ${{ secrets.ZENODO_SANDBOX_TOKEN }}
-      run: |
-        branb test
+      - uses: actions/checkout@v3
+      - uses: actions/setup-python@v4
+        with:
+          python-version: "3.10"
+      - name: Install dependencies
+        run: |
+          python -m pip install --upgrade pip
+          pip install -e .[test,profile,collect,zenodo]
+      - name: Setup Git
+        run: |
+          git config --global receive.denyCurrentBranch updateInstead
+          git config --global init.defaultBranch main
+          git config --global user.email "leo@dumbartonserum.com"
+          git config --global user.name "Leo Dumbarton"
+      - name: Test
+        env:
+          POSTGRES_HOST: sqlite
+          ZENODO_SANDBOX_TOKEN: ${{ secrets.ZENODO_SANDBOX_TOKEN }}
+        run: |
+          branb test
```

### Comparing `datazimmer-0.4.9/.github/workflows/test.yml` & `datazimmer-0.5.0/.github/workflows/test.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 name: Python Test
 
 on:
   pull_request:
-    branches: 
+    branches:
       - main
   push:
     branches:
       - main
+  schedule:
+    - cron: 0 10 * * *
 
 jobs:
   test:
     runs-on: ubuntu-latest
     services:
       postgres:
         image: postgres
@@ -20,30 +22,30 @@
           --health-cmd pg_isready
           --health-interval 10s
           --health-timeout 5s
           --health-retries 5
         ports:
           - 5432:5432
     steps:
-    - uses: actions/checkout@v3
-    - uses: actions/setup-python@v4
-      with:
-        python-version: '3.10'
-    - name: Install dependencies
-      run: |
-        python -m pip install --upgrade pip
-        pip install -e .[test,profile,postgres,explorer,collect,zenodo]
-    - name: Setup Git
-      run: |
-        git config --global receive.denyCurrentBranch updateInstead
-        git config --global init.defaultBranch main
-        git config --global user.email "leo@dumbartonserum.com"
-        git config --global user.name "Leo Dumbarton"
-    - name: Test
-      env:
-        POSTGRES_HOST: localhost
-        ZENODO_SANDBOX_TOKEN: ${{ secrets.ZENODO_SANDBOX_TOKEN }}
-      run: |
-        branb test
-    - uses: codecov/codecov-action@v3
-      with:
-        fail_ci_if_error: true
+      - uses: actions/checkout@v3
+      - uses: actions/setup-python@v4
+        with:
+          python-version: "3.10"
+      - name: Install dependencies
+        run: |
+          python -m pip install --upgrade pip
+          pip install -e .[test,profile,postgres,collect,zenodo]
+      - name: Setup Git
+        run: |
+          git config --global receive.denyCurrentBranch updateInstead
+          git config --global init.defaultBranch main
+          git config --global user.email "leo@dumbartonserum.com"
+          git config --global user.name "Leo Dumbarton"
+      - name: Test
+        env:
+          POSTGRES_HOST: localhost
+          ZENODO_SANDBOX_TOKEN: ${{ secrets.ZENODO_SANDBOX_TOKEN }}
+        run: |
+          branb test
+      - uses: codecov/codecov-action@v3
+        with:
+          fail_ci_if_error: true
```

### Comparing `datazimmer-0.4.9/.github/workflows/twine_release.yml` & `datazimmer-0.5.0/.github/workflows/twine_release.yml`

 * *Files identical despite different names*

### Comparing `datazimmer-0.4.9/.gitignore` & `datazimmer-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `datazimmer-0.4.9/LICENSE` & `datazimmer-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datazimmer-0.4.9/conftest.py` & `datazimmer-0.5.0/conftest.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,87 +10,82 @@
 from aswan.constants import DEFAULT_REMOTE_ENV_VAR, DEPOT_ROOT_ENV_VAR
 from aswan.depot.remote import HEX_ENV, PW_ENV
 from dvc.config import Config as DvcConfig
 from zimmauth import ZimmAuth
 from zimmauth.core import LOCAL_HOST_NAMES_ENV_VAR
 
 from datazimmer.config_loading import RunConfig
-from datazimmer.get_runtime import _GLOBAL_RUNTIME
-from datazimmer.metadata.atoms import _GLOBAL_CLS_MAP
 from datazimmer.naming import (
     AUTH_HEX_ENV_VAR,
     AUTH_PASS_ENV_VAR,
     DEFAULT_ENV_NAME,
     MAIN_MODULE_NAME,
-    TEMPLATE_REPO,
 )
 from datazimmer.tests.create_dogshow import dogshow_root
+from datazimmer.tests.util import dz_ctx
 from datazimmer.typer_commands import cleanup, init
-from datazimmer.utils import cd_into, gen_rmtree, git_run
+from datazimmer.utils import cd_into, gen_rmtree
 
 CORE_PY = dogshow_root / "minimal.py"
 
 
 def pytest_addoption(parser):
     # test / explore / live
     parser.addoption("--mode", action="store", default="test")
 
 
 @pytest.fixture(scope="session")
 def empty_template():
-    tmpdir = TemporaryDirectory()
+    _tmp = TemporaryDirectory()
+    tmp_dir = Path(_tmp.name)
+    dvc_rem = tmp_dir / "dvc-rem"
     pname = "test-project"
-    with cd_into(tmpdir.name):
-        init(pname)
-    pdir = Path(tmpdir.name, pname)
+    with cd_into(tmp_dir):
+        check_call(["git", "init", "remote"])
+        init(pname, git_remote=(tmp_dir / "remote").as_posix())
+    pdir = tmp_dir / pname
     with cd_into(pdir):
-        check_call(["dvc", "remote", "add", "testrem", "/nothing"])
+        check_call(["dvc", "remote", "add", "testrem", dvc_rem.as_posix()])
         check_call(["dvc", "remote", "default", "testrem"])
         Path(MAIN_MODULE_NAME, "core.py").write_text(CORE_PY.read_text())
-    yield pdir
-    with cd_into(pdir):
-        cleanup()
-    gen_rmtree(tmpdir.name)
+
+    with dz_ctx([pdir]):
+        yield pdir
+    gen_rmtree(tmp_dir)
 
 
 @pytest.fixture
-def in_template(empty_template):
+def in_template(empty_template: Path):
     with cd_into(empty_template):
-        sys.path.insert(0, empty_template)
-        yield
+        sys.path.insert(0, empty_template.as_posix())
+        yield empty_template
         sys.path.pop(0)
-        global _GLOBAL_CLS_MAP
-        _GLOBAL_CLS_MAP = {}
-        global _GLOBAL_RUNTIME
-        _GLOBAL_RUNTIME = None
 
 
 @pytest.fixture
 def running_template(in_template):
     _env = DEFAULT_ENV_NAME
     with RunConfig(write_env=_env, read_env=_env, profile=True):
         yield
 
 
 @pytest.fixture(scope="session")
 def test_bucket():
-
+    _bconf = {"CreateBucketConfiguration": {"LocationConstraint": "us-west-1"}}
     with moto.mock_s3():
         conn = boto3.resource("s3")
-        conn.create_bucket(Bucket="bucket-1")
-        conn.create_bucket(Bucket="bucket-2")
-        conn.create_bucket(Bucket="bucket-3")
+        conn.create_bucket(Bucket="bucket-1", **_bconf)
+        conn.create_bucket(Bucket="bucket-2", **_bconf)
+        conn.create_bucket(Bucket="bucket-3", **_bconf)
         yield conn
 
 
 @pytest.fixture
 def proper_env():
-
-    conf = DvcConfig()
-    gpath = Path(conf.files.get("global"))
+    gpath = Path(DvcConfig().files.get("global"))
 
     old_conf = None
     if gpath.name and gpath.exists():
         old_conf = gpath.read_text()
 
     tmp_dir = TemporaryDirectory()
     tmp_path = Path(tmp_dir.name)
```

### Comparing `datazimmer-0.4.9/datazimmer/aswan_integration.py` & `datazimmer-0.5.0/datazimmer/aswan_integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,16 @@
 
     def prepare_run(self):
         """this runs prior to running the project"""
         pass  # pragma: no cover
 
     def get_aswan_status(self):
         conf = RunConfig.load()
-
+        if conf.reset_aswan:
+            return
         stage_name = get_stage_name(self._ns, conf.write_env)
         possible_deps = []
         repo = Repo()
 
         aswan_id = get_aswan_leaf_param_id(self.name)
 
         for stage in repo.index.stages:
```

### Comparing `datazimmer-0.4.9/datazimmer/config_loading.py` & `datazimmer-0.5.0/datazimmer/config_loading.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,15 +96,14 @@
         except KeyError:
             self.aswan_projects.append(AswanSpec(name))
             return _get(self.aswan_projects, name)
 
     def create_trepo(
         self, id_: CompleteId, partitioning_cols=None, max_partition_size=None
     ):
-
         envs_of_ns = self.get_data_envs(id_.project, id_.namespace)
         if not envs_of_ns:
             return UnavailableTrepo()
         default_env = self.resolve_ns_env(id_.project, self.default_env)
         parents_dict = {
             env: get_data_path(id_.project, id_.namespace, env) for env in envs_of_ns
         }
@@ -196,33 +195,32 @@
     @classmethod
     def _cpath(cls) -> Path:
         return ...
 
 
 @dataclass
 class RunConfig(_IoConf):
-
     profile: bool = False
     write_env: Optional[str] = None
     read_env: Optional[str] = None
+    reset_aswan: bool = False
 
     def __enter__(self):
         self.dump()
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self._cpath().unlink()
 
     @classmethod
     def _cpath(cls):
         return RUN_CONF_PATH
 
 
 @dataclass
 class UserConfig(_IoConf):
-
     first_name: str
     last_name: str
     orcid: str
 
     @classmethod
     def _cpath(cls):
         return USER_CONF_PATH
```

### Comparing `datazimmer-0.4.9/datazimmer/get_runtime.py` & `datazimmer-0.5.0/datazimmer/get_runtime.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.4.9/datazimmer/gh_actions.py` & `datazimmer-0.5.0/datazimmer/gh_actions.py`

 * *Files 18% similar despite different names*

```diff
@@ -37,21 +37,17 @@
         if not project.cron:
             continue
         funs = [(tc.run_aswan_project, f"--project={project.name}")]
         cron_dic = _get_cron_dic(project.cron, project.name, *funs)
         write_action(cron_dic, _GHA / f"asw_{project.name}_schedule.yml")
 
 
-def write_book_actions(cron):
-    write_action(_get_book_dic(cron), _GHA / "deploy.yml")
-
-
 _env_keys = [AUTH_HEX_ENV_VAR, AUTH_PASS_ENV_VAR, GIT_TOKEN_ENV_VAR]
 try:
-    from aswan.depot import DEFAULT_REMOTE_ENV_VAR, HEX_ENV, PW_ENV
+    from aswan.constants import DEFAULT_REMOTE_ENV_VAR, HEX_ENV, PW_ENV
 
     _env_keys.extend([PW_ENV, HEX_ENV, DEFAULT_REMOTE_ENV_VAR])
 except ImportError:
     pass  # pragma: no cover
 
 _env = {k: r"${{ secrets." + k + r" }}" for k in _env_keys}
 
@@ -76,30 +72,7 @@
 def _get_cron_dic(cron, name, *funs):
     step = {"name": f"Scheduled {name}", "env": _env, "run": cli_run(*funs)}
     return {
         "name": f"Scheduled {name}",
         "on": {"schedule": [{"cron": cron}]},
         "jobs": _get_jobs_dic(f"cron-run-{name}", [step]),
     }
-
-
-def _get_book_dic(cron):
-    from . import typer_commands as tc
-
-    book_comm = cli_run(tc.load_explorer_data, tc.build_explorer)
-
-    steps = [
-        {"name": "Build the book", "run": book_comm, "env": _env},
-        {
-            "name": "GitHub Pages action",
-            "uses": "peaceiris/actions-gh-pages@v3",
-            "with": {
-                "github_token": "${{ secrets.GITHUB_TOKEN }}",
-                "publish_dir": "book/_build/html",
-            },
-        },
-    ]
-    return {
-        "name": "Build and Deploy Book",
-        "on": {"push": {"branches": ["main"]}, "schedule": [{"cron": cron}]},
-        "jobs": _get_jobs_dic("build-and-deploy-book", steps),
-    }
```

### Comparing `datazimmer-0.4.9/datazimmer/metadata/complete_id.py` & `datazimmer-0.5.0/datazimmer/metadata/complete_id.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.4.9/datazimmer/metadata/datascript.py` & `datazimmer-0.5.0/datazimmer/metadata/datascript.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.4.9/datazimmer/metadata/high_level.py` & `datazimmer-0.5.0/datazimmer/metadata/high_level.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,14 @@
     def __getattribute__(self, att: str):
         project: ProjectMetadata = super().__getattribute__("_p")
         return chain(*[getattr(ns, att) for ns in project.namespaces.values()])
 
 
 @dataclass
 class ProjectMetadata:
-
     uri: str
     tags: list[str]
     cron: str = ""
     namespaces: dict[str, NamespaceMetadata] = field(default_factory=dict)
     complete: NsCollection = field(init=False, repr=False)
     # TODO maybe eliminate / rename namespace to module
```

### Comparing `datazimmer-0.4.9/datazimmer/metadata/scrutable.py` & `datazimmer-0.5.0/datazimmer/metadata/scrutable.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 from contextlib import contextmanager
 from dataclasses import dataclass
-from functools import partial
 from typing import Callable, Optional, TypeVar
 
 import pandas as pd
-import sqlalchemy as sa
-from colassigner.constants import PREFIX_SEP
 from colassigner.meta_base import ColMeta
 from structlog import get_logger
 
 from ..config_loading import Config, RunConfig, UnavailableTrepo
 from ..exceptions import ProjectRuntimeException
-from ..utils import camel_to_snake, chainmap, get_creation_module_name
-from .atoms import CompositeFeature, EntityClass, ObjectProperty, PrimitiveFeature
+from ..utils import camel_to_snake, get_creation_module_name
+from .atoms import EntityClass, parse_df
 from .complete_id import CompleteId, CompleteIdBase
-from .datascript import AbstractEntity, PrimitiveType, get_np_type, get_sa_type
+from .datascript import AbstractEntity
 
 logger = get_logger()
 
 T = TypeVar("T")
 
 
 class ScruTable:
@@ -31,32 +28,31 @@
     ) -> None:
         # TODO: somehow add possibility for a description
 
         self._conf = Config.load()
         self.__module__ = get_creation_module_name()
         self.id_: CompleteId = self._infer_id(entity, self.__module__)
         self.key_map = _parse_entity_map(entity_key_table_map)
-        self.entity_class: EntityClass = EntityClass.from_cls(entity)
+        self.abstract_entity = entity
+        self.entity_class = EntityClass.from_cls(entity)
 
         self.name = self.id_.obj_id
         self.index = self.entity_class.identifiers
         self.features = self.entity_class.properties
-        self.index_map = to_dt_map(self.index)
-        self.features_map = to_dt_map(self.features)
-        self.dtype_map = {**self.index_map, **self.features_map}
-        self.index_cols = [*self.index_map.keys()]
-        self.feature_cols = [*self.features_map.keys()]
-        self.all_cols = self.index_cols + self.feature_cols
+        self.index_map = self.entity_class.table_index_dt_map
+        self.features_map = self.entity_class.table_feature_dt_map
+        self.dtype_map = self.entity_class.table_full_dt_map
+        self.index_cols = self.entity_class.table_index_cols
+        self.feature_cols = self.entity_class.table_feature_cols
+        self.all_cols = self.entity_class.table_all_columns
 
         self.partitioning_cols = partitioning_cols
         self.max_partition_size = max_partition_size
         self.trepo = self._conf.create_trepo(
-            self.id_,
-            self.partitioning_cols,
-            self.max_partition_size,
+            self.id_, self.partitioning_cols, self.max_partition_size
         )
         self.get_full_df = self._read_wrap(self.trepo.get_full_df)
         self.map_partitions = self._read_wrap(self.trepo.map_partitions)
 
         self.extend = self._write_wrap(self.trepo.extend)
         self.replace_all = self._write_wrap(self.trepo.replace_all)
         self.replace_records = self._write_wrap(self.trepo.replace_records)
@@ -91,97 +87,50 @@
         if isinstance(self.trepo, UnavailableTrepo):
             raise ProjectRuntimeException(f"trepo unavailable for {self.id_}")
         true_env = self._conf.resolve_ns_env(self.id_.project, env)
         with self.trepo.env_ctx(true_env):
             yield
 
     def _read_wrap(self, fun: Callable[..., T]) -> Callable[..., T]:
-        def f(env=None, **kwargs):
-            with self.env_ctx(env or RunConfig.load().read_env):
-                return fun(**kwargs)
-
-        return f
+        return _RWrap(fun, self.env_ctx)
 
     def _write_wrap(self, fun):
-        def f(df, parse=True, verbose=True, env=None, **kwargs):
-            with self.env_ctx(env or RunConfig.load().write_env):
-                return fun(self._parse_df(df, verbose) if parse else df, **kwargs)
-
-        return f
+        return _WWrap(fun, self.env_ctx, self._parse_df)
 
     def _parse_df(self, df: pd.DataFrame, verbose=True):
         if verbose:
             logger.info("parsing", table=self.name, namespace=self.id_.namespace)
-        full_dic = self.features_map.copy()
-        set_ind = self.index_map and (set(df.index.names) != set(self.index_cols))
-        if set_ind:
-            if verbose:
-                logger.info("indexing needed", inds=self.index_cols)
-            full_dic.update(self.index_map)
-
-        missing_cols = set(full_dic.keys()) - set(df.columns)
-        if missing_cols:
-            logger.warning(f"missing from columns {missing_cols}", present=df.columns)
-        out = df.astype(full_dic)
-        indexed_out = out.set_index(self.index_cols) if set_ind else out
-        return indexed_out.loc[:, self.feature_cols]
 
-    def _infer_id(self, entity_cls, initing_module_name) -> str:
+        return parse_df(df, self.abstract_entity, verbose)
+
+    def _infer_id(self, entity_cls, initing_module_name):
         id_base = CompleteIdBase.from_module_name(initing_module_name, self._conf.name)
         return id_base.to_id(camel_to_snake(entity_cls.__name__))
 
 
-@dataclass
-class Column:
-    name: str
-    dtype: PrimitiveType
-    nullable: bool = False
-
-
-def feats_to_cols(feats, proc_fk=None, wrap=lambda x: x) -> list[Column]:
-    return chainmap(partial(feat_to_cols, proc_fk=proc_fk, wrap=wrap), feats)
-
-
-def feat_to_cols(feat, proc_fk, wrap, init_prefix=(), open_to_fk=True) -> list:
-
-    new_open_to_fk = True
-    fk_to = None
-    if isinstance(feat, PrimitiveFeature):
-        name = PREFIX_SEP.join([*init_prefix, feat.name])
-        return [wrap(Column(name, feat.dtype, feat.nullable))]
-
-    new_feat_prefix = (*init_prefix, feat.prefix)
-    if isinstance(feat, CompositeFeature):
-        subfeats = feat.dtype.features
-    elif isinstance(feat, ObjectProperty):
-        new_open_to_fk = False
-        fk_to = feat.target
-        subfeats = fk_to.identifiers
-
-    new_fun = partial(
-        feat_to_cols,
-        init_prefix=new_feat_prefix,
-        open_to_fk=new_open_to_fk,
-        proc_fk=proc_fk,
-        wrap=wrap,
-    )
-    out = chainmap(new_fun, subfeats)
-    if fk_to is not None and open_to_fk and proc_fk:
-        proc_fk(out, fk_to, new_feat_prefix)
-    return out
-
-
-def to_dt_map(feats):
-    return {c.name: get_np_type(c.dtype, c.nullable) for c in feats_to_cols(feats)}
-
-
-def to_sa_col(col: Column, pk=False):
-    sa_dt = get_sa_type(col.dtype)
-    return sa.Column(col.name, sa_dt, nullable=col.nullable, primary_key=pk)
-
-
 def _parse_entity_map(entity_map: dict):
     d = {}
     for k, v in (entity_map or {}).items():
         if isinstance(k, ColMeta):
             d[k._parent_prefixes] = v
     return d
+
+
+@dataclass
+class _RWrap:
+    fun: Callable
+    env_ctx: Callable
+
+    def __call__(self, env=None, **kwargs):
+        with self.env_ctx(env or RunConfig.load().read_env):
+            return self.fun(**kwargs)
+
+
+@dataclass
+class _WWrap:
+    fun: Callable
+    env_ctx: Callable
+    parse_df: Callable
+
+    def __call__(self, df, parse=True, verbose=True, env=None, **kwargs):
+        with self.env_ctx(env or RunConfig.load().write_env):
+            return self.fun(self.parse_df(df, verbose) if parse else df, **kwargs)
```

### Comparing `datazimmer-0.4.9/datazimmer/naming.py` & `datazimmer-0.5.0/datazimmer/naming.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
 VERSION_PREFIX = "zimmer-v0"
 VERSION_SEPARATOR = "/"
 
 RUN_CONF_PATH = Path("__run_conf.yaml")
 BASE_CONF_PATH = Path("zimmer.yaml")
 USER_CONF_PATH = Path.home() / ".config" / "datazimmer.yaml"
-EXPLORE_CONF_PATH = Path("dec.yaml")
 REQUIREMENTS_FILE = Path("requirements.txt")
 README_PATH = Path("README.md")
 
 DATA_PATH = Path("data")
 PROFILES_PATH = Path("run-profiles")
 REGISTRY_ROOT_DIR = Path.home() / "zimmer-registries"
 SANDBOX_DIR = Path.home() / "zimmer-sandbox"
```

### Comparing `datazimmer-0.4.9/datazimmer/persistent_state.py` & `datazimmer-0.5.0/datazimmer/persistent_state.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.4.9/datazimmer/pipeline_element.py` & `datazimmer-0.5.0/datazimmer/pipeline_element.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 from .reporting import ReportFile
 
 logger = get_logger()
 
 
 @dataclass
 class PipelineElement:
-
     runner: callable
     dependencies: list = field(default_factory=list)
     outputs: list = field(default_factory=list)
     outputs_nocache: list = field(default_factory=list)
     outputs_persist: list = field(default_factory=list)
     write_envs: list = field(default_factory=list)
     read_env: Optional[str] = None
@@ -91,14 +90,18 @@
                 outs_persist=_parser(self.outputs_persist),
                 deps=_parse_list([self.runner, *self.dependencies], _true_read_env),
                 params=[{BASE_CONF_PATH.as_posix(): param_ids}] if param_ids else None,
                 force=True,
             )
             yield self.stage_name(write_env)
 
+    def get_no_cache_outs(self, env):
+        for e in [env] if env else self.write_envs:
+            yield _parse_list(self.outputs_nocache, e)
+
     def stage_name(self, env):
         return get_stage_name(self.ns, env)
 
     @property
     def ns(self):
         return CompleteIdBase.from_cls(self.runner).namespace
```

### Comparing `datazimmer-0.4.9/datazimmer/project_runtime.py` & `datazimmer-0.5.0/datazimmer/project_runtime.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.4.9/datazimmer/raw_data.py` & `datazimmer-0.5.0/datazimmer/raw_data.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.4.9/datazimmer/registry.py` & `datazimmer-0.5.0/datazimmer/registry.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.4.9/datazimmer/reporting.py` & `datazimmer-0.5.0/datazimmer/reporting.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.4.9/datazimmer/sql/loader.py` & `datazimmer-0.5.0/datazimmer/sql/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 import sqlalchemy as sa
 from colassigner.constants import PREFIX_SEP
 from sqlalchemy.orm import sessionmaker
 from structlog import get_logger
 
 from ..config_loading import RunConfig
 from ..get_runtime import get_runtime
-from ..metadata.atoms import EntityClass
+from ..metadata.atoms import EntityClass, feats_to_cols, to_sa_col
 from ..metadata.high_level import NamespaceMetadata
-from ..metadata.scrutable import ScruTable, feats_to_cols, to_sa_col
+from ..metadata.scrutable import ScruTable
 from ..utils import is_postgres
 
 if TYPE_CHECKING:
     from ..project_runtime import ProjectRuntime  # pragma: no cover
 
 
 logger = get_logger(ctx="sql loader")
@@ -39,37 +39,37 @@
         constr : str, optional
             constring where database is found, by default "sqlite:///:memory:"
             but needs to be postgres for foreign keys to be validated
         """
 
         self.runtime = get_runtime()
         self.engine = sa.create_engine(constr, echo=echo)
-        self.sql_meta = sa.MetaData(bind=self.engine)
+        self.sql_meta = sa.MetaData()
         self._Session = sessionmaker(self.engine)
         self._batch_size = batch_size
 
     def setup_schema(self):
         for nsm in self._get_ns_mappers(False):
             nsm.create_schema()
-        self.sql_meta.create_all(self.engine)
+        self.sql_meta.create_all(bind=self.engine)
 
     def load_data(self, env):
         with RunConfig(read_env=env):
             with self._Session() as session:
                 for nsm in self._get_ns_mappers():
                     nsm.load_data(session)
                 session.commit()
 
     def validate_data(self, env):
         with RunConfig(read_env=env):
             for nsm in self._get_ns_mappers():
                 nsm.validate_data()
 
     def purge(self):
-        self.sql_meta.drop_all(self.engine)
+        self.sql_meta.drop_all(bind=self.engine)
 
     def _get_ns_mappers(self, data_only=True):
         f_args = (self.runtime, self.sql_meta, self.engine, self._batch_size)
         _mapped = set()
         for ns in self.runtime.metadata.namespaces.values():
             _mapped.add((self.runtime.name, ns.name))
             yield NamespaceMapper(self.runtime.name, ns, *f_args)
@@ -89,15 +89,14 @@
                     continue
                 _mapped.add(_id)
                 yield NamespaceMapper(proj_name, ns, *f_args)
 
 
 @dataclass
 class NamespaceMapper:
-
     project_name: str
     ns_meta: NamespaceMetadata
     runtime: "ProjectRuntime"
     sql_meta: sa.MetaData
     engine: sa.engine.Engine
     batch_size: int
```

### Comparing `datazimmer-0.4.9/datazimmer/tests/create_dogshow.py` & `datazimmer-0.5.0/datazimmer/tests/create_dogshow.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,107 +1,71 @@
-import json
 import os
 import sys
 from contextlib import contextmanager
 from pathlib import Path
-from shutil import copytree
 from subprocess import check_call
 
 from cookiecutter.main import generate_files
-from jinja2 import Template
 from structlog import get_logger
 from yaml import safe_load
 
-from datazimmer.explorer import SETUP_DIR
-from datazimmer.naming import BASE_CONF_PATH, EXPLORE_CONF_PATH, MAIN_MODULE_NAME
+from datazimmer.naming import BASE_CONF_PATH, MAIN_MODULE_NAME
 from datazimmer.typer_commands import init
 from datazimmer.utils import cd_into, gen_rmtree, git_run, package_root
 
 logger = get_logger()
 
 dogshow_root = package_root / "dogshow"
 project_cc_root = dogshow_root / "projects"
-dec_src_root = dogshow_root / "explorer"
 
 _PROJECTS = ["dog-raw", "dog-show", "dograce", "dogsuccess", "dogcombine"]
 _VERSIONS = {"dog-show": ["0.0", "0.1"], "dogsuccess": ["1.0"]}
 _RAW_IMPORTS = {"dog-show": ["dog-raw"], "dograce": ["dog-raw"]}
+_PRIVATE_ZEN = {"dogsuccess": "sex_matches"}
 
 
 class DogshowContextCreator:
-    def __init__(
-        self, local_root, remote_root=None, dvc_remotes=None, explore_remote=None
-    ):
+    def __init__(self, local_root, remote_root=None, dvc_remotes=None):
         self.local_root = Path(local_root)
         gen_rmtree(self.local_root)
         self.local_root.mkdir()
         self.ran_dirs = []
         self.remote_root = Path(remote_root or self.local_root / "remotes")
         self.dvc_remotes = [*self._get_dvc_remotes(dvc_remotes)]
         _reg = self.remote_root / "dogshow-registry"
         self.cc_context = {
             "test_registry": self._init_if_local(_reg, True),
-            "explore_remote": json.dumps(explore_remote),
             "remote2": self.dvc_remotes[1][0],
         }
         self.all_contexts = map(self.project_ctx, _PROJECTS)
 
     @contextmanager
     def project_ctx(self, name: str):
+        git_remote = self._init_if_local(self.remote_root / f"dogshow-{name}")
         with cd_into(self.local_root):
-            init(name)
+            init(name, git_remote=git_remote)
         root_dir = self.local_root / name
         template_path = project_cc_root / f"cc-{name}"
-        git_remote = self._init_if_local(self.remote_root / f"dogshow-{name}")
-        check_call(["git", "remote", "add", "origin", git_remote], cwd=root_dir)
         generate_files(
             template_path,
             {"cookiecutter": {"project": name}, **self.cc_context},
             self.local_root,
             overwrite_if_exists=True,
         )
         self.ran_dirs.append(root_dir)
         with cd_into(root_dir):
             sys.path.insert(0, Path.cwd().as_posix())
             for remote_name, remote_id in self.dvc_remotes:
                 check_call(["dvc", "remote", "add", remote_name, remote_id])
             check_call(["dvc", "remote", "default", self.dvc_remotes[0][0]])
-            git_run(add=["*"], msg=f"setup {name} project")
-            check_call(["git", "push", "--set-upstream", "origin", "main"])
-            yield name, _VERSIONS.get(name, []), _RAW_IMPORTS.get(name, [])
+            git_run(add=["*"], msg=f"setup {name} project", push=True)
+            pzen = _PRIVATE_ZEN.get(name, "")
+            yield name, _VERSIONS.get(name, []), _RAW_IMPORTS.get(name, []), pzen
             sys.path.pop(0)
 
-    def explorer(self):
-        return self._explorer("explorer")
-
-    def explorer2(self):
-        # bucket is from conftest.py
-        return self._explorer("explorer2", {"explore_remote": "bucket-3"}, False)
-
-    @contextmanager
-    def _explorer(self, name: str, extras: dict = {}, push=True):
-        root_dir = self.local_root / name
-        root_dir.mkdir()
-        conf_template = dogshow_root / name / EXPLORE_CONF_PATH
-        setup_dir = dogshow_root / name / SETUP_DIR
-        cc_ctx = {**self.cc_context, **extras}
-        conf_str = Template(conf_template.read_text()).render(cc_ctx)
-        if setup_dir.exists():
-            copytree(setup_dir, root_dir / SETUP_DIR)
-        with cd_into(root_dir):
-            EXPLORE_CONF_PATH.write_text(conf_str)
-            yield
-            if not push:
-                return
-            remote = self._init_if_local(self.remote_root / f"dogshow-{name}")
-            check_call(["git", "init"])
-            check_call(["git", "remote", "add", "origin", remote])
-            git_run(add=["*"], msg="setup-dec")
-            check_call(["git", "push", "--set-upstream", "origin", "main"])
-
     def check_sdists(self):
         pass  # TODO check builds
 
     @classmethod
     def load(cls, mode: str, tmp_path: Path):
         if mode == "test":
             kwargs = {"local_root": tmp_path}
```

### Comparing `datazimmer-0.4.9/datazimmer/tests/test_scrutable.py` & `datazimmer-0.5.0/datazimmer/tests/test_scrutable.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 import pandas as pd
 import pytest
-import sqlalchemy as sa
 
 from datazimmer import ScruTable
 from datazimmer.config_loading import RunConfig
 from datazimmer.exceptions import ProjectSetupException
 from datazimmer.get_runtime import get_runtime
 from datazimmer.naming import DEFAULT_ENV_NAME
 from datazimmer.sql.loader import SqlLoader, tmp_constr
 
 
 def test_scrutable_parsing(running_template):
-
     df = pd.DataFrame(
         {
             "ind": [5, 20],
             "d": ["2020-01-01", "1999-04-04"],
             "num": ["3", "4"],
             "c": ["A", "B"],
         }
@@ -25,15 +23,15 @@
 
     scrutable: ScruTable
     scrutable.replace_all(df)
 
     parsed_df = scrutable.get_full_df()
     assert not parsed_df.equals(df)
     pd.testing.assert_frame_equal(
-        df.astype({"d": "datetime64", "num": float}).set_index("ind"),
+        df.astype({"d": "datetime64[ns]", "num": float}).set_index("ind"),
         parsed_df.sort_index().reindex(df.columns[1:], axis=1),
     )
     for fp in scrutable.paths:
         assert DEFAULT_ENV_NAME in fp.as_posix()
 
     assert next(scrutable.get_partition_paths(Thing.c))
     scrutable.purge()
@@ -41,24 +39,23 @@
 
     with pytest.raises(KeyError):
         scrutable.replace_all(pd.DataFrame({"ind": [1]}))
     assert "thing" in scrutable.__repr__()
 
 
 def test_run_scrutable(in_template):
-
     from src.core import scrutable
 
     with pytest.raises(ProjectSetupException):
         scrutable.replace_all(...)
 
 
 def test_sql(in_template):
     runtime = get_runtime()
     with RunConfig(False, write_env=DEFAULT_ENV_NAME, read_env=DEFAULT_ENV_NAME):
         runtime.run_step("core", DEFAULT_ENV_NAME)
 
     with tmp_constr() as constr:
         loader = SqlLoader(constr)
-        sa.MetaData.reflect(loader.sql_meta)
+        loader.sql_meta.reflect(loader.engine)
         loader.load_data(DEFAULT_ENV_NAME)
         loader.validate_data(DEFAULT_ENV_NAME)
```

### Comparing `datazimmer-0.4.9/datazimmer/tests/test_validation.py` & `datazimmer-0.5.0/datazimmer/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.4.9/datazimmer/typer_commands.py` & `datazimmer-0.5.0/datazimmer/typer_commands.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import datetime as dt
 import re
 from dataclasses import asdict
+from itertools import chain
 from pathlib import Path
 from subprocess import check_call
+from typing import TYPE_CHECKING
 
 import typer
 from dvc.repo import Repo
 from structlog import get_logger
 
 from .config_loading import CONF_KEYS, Config, RunConfig, UserConfig
 from .exceptions import ProjectSetupException
-from .explorer import build_explorer, init_explorer, load_explorer_data
 from .get_runtime import get_runtime
 from .gh_actions import write_aswan_crons, write_project_cron
 from .metadata.high_level import ProjectMetadata
 from .naming import (
     BASE_CONF_PATH,
     MAIN_MODULE_NAME,
     README_PATH,
@@ -25,41 +26,60 @@
     get_tag,
     meta_version_from_tag,
 )
 from .raw_data import IMPORTED_RAW_DATA_DIR, RAW_DATA_DIR, RAW_ENV_NAME
 from .registry import Registry
 from .sql.draw import dump_graph
 from .sql.loader import tmp_constr
-from .utils import command_out_w_prefix, gen_rmtree, get_git_diffs, git_run
+from .utils import cd_into, command_out_w_prefix, gen_rmtree, get_git_diffs, git_run
 from .validation_functions import validate
 from .zenodo import CITATION_FILE, ZenApi
 
+if TYPE_CHECKING:  # pragma: no cover
+    from .project_runtime import ProjectRuntime
+
 logger = get_logger(ctx="CLI command")
 app = typer.Typer()
 
 app.command()(validate)
-app.command()(init_explorer)
-app.command()(build_explorer)
-app.command()(load_explorer_data)
 
 
 @app.command()
 def run_step(name: str, env: str):
     get_runtime().run_step(name, env)
 
 
 @app.command()
-def init(name: str):
+def init(name: str, github_org: str = "", git_remote: str = ""):
     git_run(clone=(TEMPLATE_REPO, name), depth=None)
-    c_p = name / BASE_CONF_PATH
-    cstr = re.sub(f"{CONF_KEYS.name}: .+", f"{CONF_KEYS.name}: {name}", c_p.read_text())
-    c_p.write_text(cstr)
-    rm_p = name / README_PATH
-    rm_p.write_text(rm_p.read_text().replace("{{title}}", name))
-    check_call(["git", "remote", "rm", "origin"], cwd=name)
+    comms = [["git", "remote", "rm", "origin"]]
+    if github_org:  # pragma: no cover
+        from ghapi.all import GhApi
+
+        api = GhApi()
+        api.repos.create_in_org(github_org, name)
+        git_remote = f"git@github.com:{github_org}/{name}.git"
+    if git_remote:
+        comms.extend(
+            [
+                ["git", "remote", "add", "origin", git_remote],
+                ["git", "push", "-u", "origin", "main"],
+            ]
+        )
+    with cd_into(name):
+        cstr = re.sub(
+            f"{CONF_KEYS.name}: .+",
+            f"{CONF_KEYS.name}: {name}",
+            BASE_CONF_PATH.read_text(),
+        )
+        BASE_CONF_PATH.write_text(cstr)
+        README_PATH.write_text(README_PATH.read_text().replace("{{title}}", name))
+        for c in comms:
+            check_call(c)
+        git_run(add=["*"], msg=f"init {name}", push=bool(git_remote))
 
 
 @app.command()
 def update(registry: bool = True, code: bool = True, dvc: bool = True):
     if registry:
         Registry(Config.load()).update()
     if code:
@@ -76,26 +96,28 @@
 
 @app.command()
 def set_whoami(first_name: str, last_name: str, orcid: str):
     UserConfig(first_name, last_name, orcid).dump()
 
 
 @app.command()
-def import_raw(project: str, tag: str = ""):
+def import_raw(project: str, tag: str = "", commit: bool = False):
     dvc_repo = Repo()
     reg = get_runtime().registry
     v = meta_version_from_tag(tag) if tag else None
     uri = ProjectMetadata(**reg.get_project_meta_base(project, v)).uri
     IMPORTED_RAW_DATA_DIR.mkdir(exist_ok=True)
     dvc_repo.imp(
         uri,
         path=RAW_DATA_DIR.as_posix(),
         out=(IMPORTED_RAW_DATA_DIR / project).as_posix(),
         rev=tag or None,
     )
+    if commit:
+        _dvc_commit(paths=[f"{IMPORTED_RAW_DATA_DIR}/*"], msg=f"import raw {project}")
 
 
 @app.command()
 def publish_data():
     build_meta()
     # TODO: ensure that this build gets published
     _validate_empty_vc("publishing data")
@@ -110,60 +132,68 @@
         check_call(["git", "tag", vtag])
         vtags.append(vtag)
 
     default_remote = runtime.config.get_env(runtime.config.default_env).remote
     if RAW_DATA_DIR.exists():
         dvc_repo.add(RAW_DATA_DIR.as_posix())
         dvc_repo.push(targets=RAW_DATA_DIR.as_posix(), remote=default_remote)
-        git_run(add=[f"{RAW_DATA_DIR}.dvc"], msg="save raw data", check=True)
+        _dvc_commit([RAW_DATA_DIR], "save raw data")
         _tag(RAW_ENV_NAME, default_remote)
     for env in runtime.config.sorted_envs:
         targets = runtime.step_names_of_env(env.name)
         logger.info("pushing targets", targets=targets, env=env.name)
         dvc_repo.push(targets=targets, remote=env.remote)
         _tag(env.name, env.remote)
     git_run(push=True, pull=True)
     for tag_to_push in vtags:
         check_call(["git", "push", "origin", tag_to_push])
     runtime.registry.publish()
 
 
 @app.command()
-def publish_to_zenodo(env: str = "", test: bool = False):
+def deposit_to_zenodo(
+    env: str = "",
+    publish: bool = False,
+    test: bool = False,
+    path_filter: str = "",
+    private: bool = False,
+    key_path: str = "",
+):
+    """path_filter: regex to filter paths to be uploaded
+    key_path: used if private=True, a path to a fernet key file in hex text"""
     # must be at a zimmer tag
+    if private and not key_path:
+        raise ValueError("if upload is private, a fernet key path is needed")
     _validate_empty_vc("publishing to zenodo")
     runtime = get_runtime()
     tag_env, tag = _get_current_tag_of_env(env)
     if tag is None:
         if not env:
             raise ProjectSetupException(
                 "cant publish untagged commit. "
                 f"either checkout a published tag or run {publish_data}"
             )
         else:
-            raise ValueError(f"can't find {env} amond tags of HEAD")
+            raise ValueError(f"can't find {env} among tags of HEAD")
 
-    zapi = ZenApi(runtime.config, test=test, tag=tag)
-    did = zapi.get_depo_id()
+    zapi = ZenApi(runtime.config, private=private, test=test, tag=tag)
     if tag_env == RAW_ENV_NAME:
-        zapi.upload_directory(RAW_DATA_DIR, depo_id=did)
+        paths_to_upload = [RAW_DATA_DIR]
+    else:
+        paths_to_upload = _iter_dvc_paths(runtime, tag_env)
+    for path in paths_to_upload:
+        if (path_filter != "") and (not re.findall(path_filter, path.as_posix())):
+            continue
+        zapi.upload(path, key_path if private else None)
+    if publish:
+        zapi.publish()
+        zapi.update_readme()
+        git_run(add=[README_PATH, CITATION_FILE], msg=f"doi for {tag}", check=True)
     else:
-        dvc_repo = Repo()
-        for step in runtime.step_names_of_env(tag_env):
-            for out in dvc_repo.index.stage_collector.get_target(step).outs:
-                op = Path(out.fs_path)
-                if op.is_absolute():
-                    op = op.relative_to(Path.cwd())
-                if op.is_dir():
-                    zapi.upload_directory(op, depo_id=did)
-                elif op.exists():
-                    zapi.upload_file(op, depo_id=did)
-    zapi.publish(zid=did)
-    zapi.update_readme(depo_id=did)
-    git_run(add=[README_PATH, CITATION_FILE], msg=f"doi for {tag}", check=True)
+        logger.info(f"{zapi.url_base}/deposit/{zapi.depo_id}")
 
 
 @app.command()
 def build_meta(global_conf: bool = False):
     config = Config.load()
     Registry(config).full_build(global_conf)
     if config.cron:
@@ -179,16 +209,15 @@
     should probably be a bit more clever,
     but dvc handles quite a lot of caching
     """
     runtime = get_runtime()
     logger.info("loading external data", envs=runtime.data_to_load)
     posixes = runtime.load_all_data(env=env)
     if git_commit and posixes:
-        vc_paths = ["*.gitignore", *[f"{p}.dvc" for p in posixes]]
-        git_run(add=vc_paths, msg="add imported datasets", check=True)
+        _dvc_commit(posixes, "add imported datasets")
 
 
 @app.command()
 def cleanup():
     conf = Config.load()
     Registry(conf).purge()
     gen_rmtree(SANDBOX_DIR)
@@ -203,58 +232,80 @@
         asw_project(global_run=True).run()
     if publish:
         git_run(add=(BASE_CONF_PATH,), msg="asw-run", push=True, pull=True, check=True)
 
 
 @app.command()
 def run(
-    stage: bool = True, profile: bool = False, env: str = None, commit: bool = False
+    stage: bool = True,
+    profile: bool = False,
+    env: str = None,
+    commit: bool = False,
+    reset_aswan: bool = False,
 ):
+    # TODO: add validation that all scrutables belong somewhere as an output
     dvc_repo = Repo(config={"core": {"autostage": stage}})
     runtime = get_runtime()
-    stage_names = [
-        stage_name
-        for step in runtime.metadata.complete.pipeline_elements
-        for stage_name in step.add_stages(dvc_repo)
-    ]
-    for stage in dvc_repo.stages:
-        if stage.is_data_source or stage.is_import or (stage.name in stage_names):
+    stage_names = []
+    no_cache_outputs = []
+    for step in runtime.metadata.complete.pipeline_elements:
+        no_cache_outputs.extend(chain(*step.get_no_cache_outs(env)))
+        stage_names.extend(step.add_stages(dvc_repo))
+
+    for dvc_stage in dvc_repo.stages:
+        if (
+            dvc_stage.is_data_source
+            or dvc_stage.is_import
+            or (dvc_stage.name in stage_names)
+        ):
             continue
-        logger.info("removing dvc stage", stage=stage.name)
-        dvc_repo.remove(stage.name)
+        logger.info("removing dvc stage", stage=dvc_stage.name)
+        dvc_repo.remove(dvc_stage.name)
         dvc_repo.lock.lock()
-        stage.remove_outs(force=True)
+        dvc_stage.remove_outs(force=True)
         dvc_repo.lock.unlock()
     if not stage_names:
         return
     targets = runtime.step_names_of_env(env) if env else None
-    rconf = RunConfig(profile=profile)
+    rconf = RunConfig(profile=profile, reset_aswan=reset_aswan)
     with rconf:
         logger.info("running repro", targets=targets, **asdict(rconf))
         runs = dvc_repo.reproduce(targets=targets, pull=True)
-    git_run(add=["dvc.yaml", "dvc.lock", BASE_CONF_PATH])
+    git_run(add=["dvc.yaml", "dvc.lock", BASE_CONF_PATH, *no_cache_outputs])
     if commit:
         now = dt.datetime.now().isoformat(" ", "minutes")
         git_run(msg=f"at {now} ran: {runs}", check=True)
     return runs
 
 
+def _iter_dvc_paths(runtime: "ProjectRuntime", env):
+    dvc_repo = Repo()
+    for step in runtime.step_names_of_env(env):
+        for out in list(dvc_repo.stage.collect(step))[0].outs:
+            op = Path(out.fs_path)
+            yield op.relative_to(Path.cwd()) if op.is_absolute() else op
+
+
 def _get_current_tag_of_env(env: str):
     tag_comm = ["git", "tag", "--points-at", "HEAD"]
     for tag in command_out_w_prefix(tag_comm, VERSION_PREFIX):
         tag_env = env_from_tag(tag)
         if (env == tag_env) or not env:
             return tag_env, tag
     return None, None
 
 
 def _commit_dvc_default(remote):
     check_call(["dvc", "remote", "default", remote])
     git_run(add=[".dvc"], msg=f"update dvc default remote to {remote}", check=True)
 
 
+def _dvc_commit(paths, msg):
+    git_run(add=["*.gitignore", *[f"{p}.dvc" for p in paths]], msg=msg, check=True)
+
+
 def _validate_empty_vc(attempt, prefs=("dvc.", MAIN_MODULE_NAME)):
     # TODO: in case of raw data, might need to check notebooks
-    for fp in get_git_diffs() + get_git_diffs(True):
+    for fp in get_git_diffs() + get_git_diffs(True) + get_git_diffs(untracked=True):
         if any([*[fp.startswith(pref) for pref in prefs], fp == BASE_CONF_PATH]):
             msg = f"{fp} should be committed to git before {attempt}"
             raise ProjectSetupException(msg)
```

### Comparing `datazimmer-0.4.9/datazimmer/utils.py` & `datazimmer-0.5.0/datazimmer/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,18 +46,21 @@
     _run(batch_one)
 
     if check and (not get_git_diffs(True, wd=wd)):
         return
     _run([(msg, ["commit", "-m", msg]), (push, ["push"])])
 
 
-def get_git_diffs(staged=False, wd=None):
-    comm = ["git", "diff", "--name-only"]
-    if staged:
-        comm.append("--cached")
+def get_git_diffs(staged=False, wd=None, untracked=False):
+    if untracked:
+        comm = ["git", "ls-files", "-o", "--exclude-standard", "--full-name"]
+    else:
+        comm = ["git", "diff", "--name-only"]
+        if staged:
+            comm.append("--cached")
     diffs = check_output(comm, cwd=wd)
     return [*filter(None, diffs.decode("utf-8").strip().split("\n"))]
 
 
 @contextmanager
 def cd_into(dirpath: Union[str, Path]):
     wd = os.getcwd()
```

### Comparing `datazimmer-0.4.9/datazimmer/validation_functions.py` & `datazimmer-0.5.0/datazimmer/validation_functions.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.4.9/datazimmer/zenodo.py` & `datazimmer-0.5.0/datazimmer/zenodo.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import calendar
 import datetime as dt
 import json
 import os
 import re
 from dataclasses import asdict, dataclass, field
-from functools import partial, reduce
+from functools import cached_property, partial, reduce
 from pathlib import Path
 
 import yaml
+from cryptography.fernet import Fernet
 
 from .config_loading import Config, UserConfig
 from .naming import README_PATH
 
 ZENODO_TOKEN_ENV_VAR = "ZENODO_TOKEN"
 ZENODO_TEST_TOKEN_ENV_VAR = "ZENODO_SANDBOX_TOKEN"
 CITATION_FILE = Path("CITATION.cff")
@@ -92,40 +93,38 @@
             type=meta["resource_type"]["type"],
             date_released=meta["publication_date"],
         )
 
 
 @dataclass
 class Citation(ShortCitation):
-
     authors: list[Author]
     keywords: list[str]
     license: str
     message: str
     url: str
     references: list[ShortCitation] = field(default_factory=list)
     cff_version: str = "1.2.0"
 
     @classmethod
-    def from_zen_dic(cls, dic) -> "Citation":
+    def from_zen_dic(cls, dic):
         short = ShortCitation.from_zen_dic(dic)
         meta = dic["metadata"]
-        return Citation(
+        return cls(
             **asdict(short),
             authors=list(map(Author.from_zdic, meta["creators"])),
             keywords=meta.get("keywords", []),
-            license=meta["license"]["id"],
+            license=meta.get("license", {"id": "closed"})["id"],
             message=meta.get(
                 "notes", "If you use this software, please cite it as below."
             ),
             url=f"https://doi.org/{short.doi}",
         )
 
     def to_bib(self):
-
         pairs = [
             ("author", " and ".join(map(Author.comma_name, self.authors))),
             ("title", self.title),
             ("month", self.month),
             ("year", str(self.year)),
             ("publisher", self.publisher),
             ("version", self.version),
@@ -169,24 +168,25 @@
 
     @property
     def _date(self):
         return dt.date.fromisoformat(self.date_released)
 
 
 class ZenodoMeta:
-    def __init__(self, title, version, lines) -> None:
+    def __init__(self, title, version, lines, private: bool) -> None:
         import markdown2
 
         self.title: str = title  # from git remote last 2 elems
         self.version: str = version  # from git tag
         self.publication_date = dt.date.today().isoformat()
         self.upload_type: str = "dataset"  # /software/other
         self.description: str = markdown2.markdown("\n".join(lines))
-        self.access_right: str = "open"  # embargoed/restricted/closed
-        self.license: str = "MIT"  # if open/embargoed list at /api/licenses
+        self.access_right = "closed" if private else "open"
+        # embargoed/restricted/closed
+        self.license: str = "" if private else "MIT"
         # self.keywords: list[str] = []
         self.related_identifiers: list[dict] = get_cites()
         uconf = UserConfig.load()
         # TODO: optionally add more
         self.creators: list[dict] = [
             {
                 "name": ", ".join([uconf.last_name, uconf.first_name]),
@@ -198,98 +198,92 @@
         # access_conditions: str (html) if restricted
 
     def data(self):
         return {"metadata": self.__dict__}
 
 
 class ZenApi:
-    def __init__(self, conf: Config, tag: str, test: bool = True):
+    def __init__(self, conf: Config, private: bool, tag: str, test: bool = True):
         import requests
 
         self.live = not test
         self.name = conf.name
         self.tag = tag
-        self.url = _get_z_url(test)
+        self.private = private
+        self.url_base = _get_z_url(test)
+        self.url = self.url_base + "/api"
         self.env_var = ZENODO_TEST_TOKEN_ENV_VAR if test else ZENODO_TOKEN_ENV_VAR
 
         self.s = requests.Session()
         self.s.params = {"access_token": os.environ[self.env_var]}
         self.readme_lines = []
 
-    def get_depo_id(self):
-        zid = self.zid_from_readme()
-        if not zid:
-            return self.new_deposition().json()["id"]
-
-        ver_resp = self.s.post(f"{self._dep_path()}/{zid}/actions/newversion")
-        if ver_resp.ok:
-            id_ = ver_resp.json()["links"]["latest_draft"].split("/")[-1]
-            for file in ver_resp.json()["files"]:
-                self.s.delete(f"{self._dep_path()}/{id_}/files/{file['id']}")
-            self.s.put(f"{self._dep_path()}/{id_}", data=self.meta.data())
-            return id_
-        return self.new_deposition().json()["id"]
-
-    def publish(self, zid):
-        resp = self.s.post(f"{self._dep_path()}/{zid}/actions/publish")
+    def publish(self):
+        resp = self.s.post(f"{self._dep_path()}/{self.depo_id}/actions/publish")
         assert resp.ok, resp.content.decode("utf-8")
 
     def get(self, **params):
         return self.s.get(self._dep_path(), params=params)
 
     def new_deposition(self):
+        return self.s.post(self._dep_path(), **self._meta_kwargs())
 
+    def upload(self, fpath: Path, key_path=""):
+        assert fpath.exists(), f"{fpath} must exist to upload to zenodo"
+        if fpath.is_dir():
+            self.upload_directory(fpath, key_path)
+        else:
+            self.upload_file(fpath, key_path)
+
+    def upload_file(self, fpath: Path, key_path=""):
+        if key_path:
+            fern = Fernet(bytes.fromhex(Path(key_path).read_text()))
+            enc_fpath = Path(fpath.parent, fpath.name + ".encrypted")
+            enc_fpath.write_bytes(fern.encrypt(fpath.read_bytes()))
+            fpath = enc_fpath
         return self.s.post(
-            self._dep_path(),
-            headers={"Content-Type": "application/json"},
-            data=json.dumps(self.meta.data()),
-        )
-
-    def upload_file(self, fpath: Path, depo_id):
-        return self.s.post(
-            f"{self._dep_path()}/{depo_id}/files",
+            f"{self._dep_path()}/{self.depo_id}/files",
             data={"name": fpath.as_posix()},
             files={"file": fpath.open(mode="rb")},
         )
 
-    def upload_directory(self, dirpath, depo_id):
+    def upload_directory(self, dirpath, key_path=""):
         for root, _, files in os.walk(dirpath):
             for f in files:
-                self.upload_file(Path(root, f), depo_id)
+                self.upload_file(Path(root, f), key_path)
 
-    def cite(self, zid, bib=True, live=False):
+    def cite(self, did: str, bib=True, live=False):
         headers = {}
         if bib:
             headers["accept"] = "application/x-bibtex"
-        return self.s.get(f"{_get_z_url(not live)}/records/{zid}", headers=headers)
+        return self.s.get(f"{_get_z_url(not live)}/api/records/{did}", headers=headers)
 
     def zid_from_readme(self):
         zid = None
         for readme_line in README_PATH.read_text().split("\n"):
             if readme_line == CITE_HEADER:
                 break
             found = re.findall(z_rex, readme_line)
             if not found:
                 self.readme_lines.append(readme_line)
             else:
                 zid = int(found[0][-1])
         return zid
 
-    def update_readme(self, depo_id):
+    def update_readme(self):
         new_zen_line = rm_frame.format(
-            url_base="zenodo.org", doi_num="10.5281", zid=depo_id
+            url_base="zenodo.org", doi_num="10.5281", zid=self.depo_id
         )
         self.readme_lines.insert(2, new_zen_line)
         # todo: this is the latest dz bib, but cant search with version
         dz_dic = self.cite(dz_concept_zid, live=True, bib=False).json()
         dz = Citation.from_zen_dic(dz_dic)
         datac = Citation.from_zen_dic(
-            self.cite(depo_id, live=self.live, bib=False).json()
+            self.cite(self.depo_id, live=self.live, bib=False).json()
         )
-
         cite_inst = cite_frame.format(
             dz_bib=dz.to_bib(),
             bib=datac.to_bib(),
             short_data=datac.to_short(),
             short_dz=dz.to_short(),
             ama_data=datac.to_ama(),
             ama_dz=dz.to_ama(),
@@ -299,21 +293,43 @@
         datac.references.append(ShortCitation.from_zen_dic(dz_dic))
         CITATION_FILE.write_bytes(
             yaml.safe_dump(as_yaml_dict(datac), encoding="utf-8", allow_unicode=True)
         )
 
     @property
     def meta(self):
-        return ZenodoMeta(self.name, self.tag, self.readme_lines)
+        return ZenodoMeta(self.name, self.tag, self.readme_lines, self.private)
+
+    @cached_property
+    def depo_id(self):
+        zid = self.zid_from_readme()
+        if not zid:
+            return self.new_deposition().json()["id"]
+
+        ver_resp = self.s.post(f"{self._dep_path()}/{zid}/actions/newversion")
+        if ver_resp.ok:
+            id_ = ver_resp.json()["links"]["latest_draft"].split("/")[-1]
+            for file in ver_resp.json()["files"]:
+                self.s.delete(f"{self._dep_path()}/{id_}/files/{file['id']}")
+            resp = self.s.put(f"{self._dep_path()}/{id_}", **self._meta_kwargs())
+            assert resp.ok, resp.content.decode("utf-8")
+            return id_
+        return self.new_deposition().json()["id"]
 
     def _dep_path(self):
         return f"{self.url}/deposit/depositions"
 
+    def _meta_kwargs(self):
+        return dict(
+            headers={"Content-Type": "application/json"},
+            data=json.dumps(self.meta.data()),
+        )
+
 
 def _get_z_url(sandbox: bool):
-    return f"https://{'sandbox.' if sandbox else ''}zenodo.org/api"
+    return f"https://{'sandbox.' if sandbox else ''}zenodo.org"
 
 
 def _to_bibline(kv):
     k = kv[0]
     v = "{%s}" % kv[1]
     return f"  {k}{' ' * (12 -len(k))} = {v}"
```

### Comparing `datazimmer-0.4.9/docs/api/datazimmer.DzAswan.rst` & `datazimmer-0.5.0/docs/api/datazimmer.DzAswan.rst`

 * *Files identical despite different names*

### Comparing `datazimmer-0.4.9/docs/api/datazimmer.ReportFile.rst` & `datazimmer-0.5.0/docs/api/datazimmer.ReportFile.rst`

 * *Files identical despite different names*

### Comparing `datazimmer-0.4.9/docs/api/datazimmer.ScruTable.rst` & `datazimmer-0.5.0/docs/api/datazimmer.ScruTable.rst`

 * *Files identical despite different names*

### Comparing `datazimmer-0.4.9/docs/conf.py` & `datazimmer-0.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.4.9/docs/notebooks/doc-002-glossary.rst` & `datazimmer-0.5.0/docs/notebooks/doc-002-glossary.rst`

 * *Files identical despite different names*

### Comparing `datazimmer-0.4.9/docs/notebooks/doc-003-mock-projects.rst` & `datazimmer-0.5.0/docs/notebooks/doc-003-mock-projects.rst`

 * *Files identical despite different names*

### Comparing `datazimmer-0.4.9/docs/notebooks/doc-004-rules-conventions.rst` & `datazimmer-0.5.0/docs/notebooks/doc-004-rules-conventions.rst`

 * *Files identical despite different names*

### Comparing `datazimmer-0.4.9/dogshow/data/photo.csv` & `datazimmer-0.5.0/dogshow/data/photo.csv`

 * *Files identical despite different names*

### Comparing `datazimmer-0.4.9/dogshow/minimal.py` & `datazimmer-0.5.0/dogshow/minimal.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.4.9/dogshow/projects/cc-dog-raw/{{cookiecutter.project}}/notebooks/create-dogshow-test-data.ipynb` & `datazimmer-0.5.0/dogshow/projects/cc-dog-raw/{{cookiecutter.project}}/notebooks/create-dogshow-test-data.ipynb`

 * *Files identical despite different names*

### Comparing `datazimmer-0.4.9/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/create_envs.py` & `datazimmer-0.5.0/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/create_envs.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.4.9/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/ns_meta.py` & `datazimmer-0.5.0/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/ns_meta.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.4.9/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/update_data.py` & `datazimmer-0.5.0/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/update_data.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.4.9/dogshow/projects/cc-dogcombine/{{cookiecutter.project}}/src/joint_success.py` & `datazimmer-0.5.0/dogshow/projects/cc-dogcombine/{{cookiecutter.project}}/src/joint_success.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.4.9/dogshow/projects/cc-dograce/{{cookiecutter.project}}/src/core.py` & `datazimmer-0.5.0/dogshow/projects/cc-dograce/{{cookiecutter.project}}/src/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,30 +55,29 @@
 def create_data():
     raw_src = "dog-raw"
     dogsize_df = pd.read_csv(dz.get_raw_data_path("sizes.csv", raw_src))
     dog_df = pd.read_csv(dz.get_raw_data_path("dog2.csv", raw_src))
     comp_df = (
         pd.read_csv(dz.get_raw_data_path("race.csv", raw_src))
         .set_index(Competition.competition_id)
-        .astype({Competition.held_date: "datetime64"})
+        .astype({Competition.held_date: "datetime64[ns]"})
     )
     dotm_df = pd.read_csv(dz.get_raw_data_path("dog_of_the_month.csv", raw_src))
     dz.dump_dfs_to_tables(
         [
             (dogsize_df, dog_size_table),
             (dog_df, dog_table),
             (comp_df, competition_table),
             (dotm_df, dog_of_the_month_table),
         ],
     )
 
 
 @dz.register_env_creator
 def create_environments(dog_sizes):
-
     dog_size_set = set(dog_sizes)
     dogsize_df = dog_size_table.get_full_df().loc[dog_sizes, :]
     dog_df = dog_table.get_full_df().loc[
         lambda df: df[SizedDog.size.dogsize_name].isin(dog_size_set), :
     ]
     comp_df = competition_table.get_full_df().loc[
         lambda df: df[Competition.champion.cid].isin(dog_df.index), :
```

### Comparing `datazimmer-0.4.9/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/counts/proc.py` & `datazimmer-0.5.0/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/counts/proc.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.4.9/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/sex_matches.py` & `datazimmer-0.5.0/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/sex_matches.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.4.9/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/success.py` & `datazimmer-0.5.0/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/success.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.4.9/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/top_report.py` & `datazimmer-0.5.0/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/top_report.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.4.9/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/zimmer.yaml` & `datazimmer-0.5.0/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/zimmer.yaml`

 * *Files identical despite different names*

### Comparing `datazimmer-0.4.9/dogshow/todo/complex_success.py` & `datazimmer-0.5.0/dogshow/todo/complex_success.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.4.9/notebooks/doc-001-intro.ipynb` & `datazimmer-0.5.0/notebooks/doc-001-intro.ipynb`

 * *Files identical despite different names*

### Comparing `datazimmer-0.4.9/notebooks/doc-002-glossary.ipynb` & `datazimmer-0.5.0/notebooks/doc-002-glossary.ipynb`

 * *Files identical despite different names*

### Comparing `datazimmer-0.4.9/notebooks/doc-003-mock-projects.ipynb` & `datazimmer-0.5.0/notebooks/doc-003-mock-projects.ipynb`

 * *Files identical despite different names*

### Comparing `datazimmer-0.4.9/notebooks/doc-004-rules-conventions.ipynb` & `datazimmer-0.5.0/notebooks/doc-004-rules-conventions.ipynb`

 * *Files identical despite different names*

### Comparing `datazimmer-0.4.9/notebooks/doc-005-cli.ipynb` & `datazimmer-0.5.0/notebooks/doc-005-cli.ipynb`

 * *Files identical despite different names*

### Comparing `datazimmer-0.4.9/pyproject.toml` & `datazimmer-0.5.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -9,38 +9,31 @@
 dependencies = [
     "flit",
     "wheel>=0.37.0",
     "pip>=22.0.0",
     "setuptools>=60.0.0",
     "dvc[s3,ssh]",
     "parquetranger>=0.2.3",
+    "pandas>=2.0.1",
     "colassigner>=0.2.2",
+    "sqlalchemy>=2.0.0",
     "pyyaml",
     "structlog",
-    "sqlalchemy",
     "toml",
     "typer",
     "cookiecutter",
     "sqlmermaid",
     "metazimmer",
     "zimmauth"
 ]
 
 [project.optional-dependencies]
 collect = ["aswan[remote]>=0.4.2"]
 postgres = ["psycopg2"]
 profile = ["pyinstrument"]
-explorer = [
-    "pandas_profiling", 
-    "jupyter-book==0.12.2", 
-    "sphinxcontrib-mermaid", 
-    "beautifulsoup4",
-    "html5lib",
-    "cron-descriptor",
-]
 zenodo = ["requests", "markdown2"]
 test = ["branthebuilder", "zimmauth[test]", "atqo", "faker"]
 doc = ["branthebuilder[doc]"]
 [project.urls]
 Homepage = "https://github.com/sscu-budapest/datazimmer"
 
 [build-system]
```

### Comparing `datazimmer-0.4.9/PKG-INFO` & `datazimmer-0.5.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,114 +1,116 @@
 Metadata-Version: 2.1
 Name: datazimmer
-Version: 0.4.9
+Version: 0.5.0
 Summary: sscu-budapest utilities for scientific data engineering
 Author-email: Social Science Computing Unit Budapest <borza.endre@krtk.hu>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: flit
 Requires-Dist: wheel>=0.37.0
 Requires-Dist: pip>=22.0.0
 Requires-Dist: setuptools>=60.0.0
 Requires-Dist: dvc[s3,ssh]
 Requires-Dist: parquetranger>=0.2.3
+Requires-Dist: pandas>=2.0.1
 Requires-Dist: colassigner>=0.2.2
+Requires-Dist: sqlalchemy>=2.0.0
 Requires-Dist: pyyaml
 Requires-Dist: structlog
-Requires-Dist: sqlalchemy
 Requires-Dist: toml
 Requires-Dist: typer
 Requires-Dist: cookiecutter
 Requires-Dist: sqlmermaid
 Requires-Dist: metazimmer
 Requires-Dist: zimmauth
 Requires-Dist: aswan[remote]>=0.4.2 ; extra == "collect"
 Requires-Dist: branthebuilder[doc] ; extra == "doc"
-Requires-Dist: pandas_profiling ; extra == "explorer"
-Requires-Dist: jupyter-book==0.12.2 ; extra == "explorer"
-Requires-Dist: sphinxcontrib-mermaid ; extra == "explorer"
-Requires-Dist: beautifulsoup4 ; extra == "explorer"
-Requires-Dist: html5lib ; extra == "explorer"
-Requires-Dist: cron-descriptor ; extra == "explorer"
 Requires-Dist: psycopg2 ; extra == "postgres"
 Requires-Dist: pyinstrument ; extra == "profile"
 Requires-Dist: branthebuilder ; extra == "test"
 Requires-Dist: zimmauth[test] ; extra == "test"
 Requires-Dist: atqo ; extra == "test"
 Requires-Dist: faker ; extra == "test"
 Requires-Dist: requests ; extra == "zenodo"
 Requires-Dist: markdown2 ; extra == "zenodo"
 Project-URL: Homepage, https://github.com/sscu-budapest/datazimmer
 Provides-Extra: collect
 Provides-Extra: doc
-Provides-Extra: explorer
 Provides-Extra: postgres
 Provides-Extra: profile
 Provides-Extra: test
 Provides-Extra: zenodo
 
 # datazimmer
 
 [![Documentation Status](https://readthedocs.org/projects/datazimmer/badge/?version=latest)](https://datazimmer.readthedocs.io/en/latest)
 [![codeclimate](https://img.shields.io/codeclimate/maintainability/sscu-budapest/datazimmer.svg)](https://codeclimate.com/github/sscu-budapest/datazimmer)
 [![codecov](https://img.shields.io/codecov/c/github/sscu-budapest/datazimmer)](https://codecov.io/gh/sscu-budapest/datazimmer)
 [![pypi](https://img.shields.io/pypi/v/datazimmer.svg)](https://pypi.org/project/datazimmer/)
 [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.7499121.svg)](https://doi.org/10.5281/zenodo.7499121)
 
 
-Some utility function to help with
-
-- setting up data environments
-- simplified dvc pipeline registry
-
-these are used in the [project-template](https://github.com/sscu-budapest/project-template)
-
-Make sure that `python` points to `python>=3.8` and you have `pip` and `git`
-
-### To create a new project
+## To create a new project
 
+- make sure that `python` points to `python>=3.8` and you have `pip` and `git` then `pip install datazimmer`
 - run `dz init project-name`
+  - pulls [project-template](https://github.com/sscu-budapest/project-template)
+- add a remote
+  - both to git and dvc (can run `dz build-meta` to see available dvc remotes)
+  - git remote can be given with `dz init`
 - create, register and document steps in a pipeline you will run in different [environments](TODO)
 - build metadata to exportable and serialized format with `dz build-meta`
   - if you defined importable data from other artifacts in the config, you can import them with `load-external-data` 
   - ensure that you import envs that are served from sources you have access to
 - build and run pipeline steps by running `dz run`
 - validate that the data matches the [datascript](TODO) description with `dz validate`
 
-## Test projects
-
-TODO: document dogshow and everything else much better here
-
+### Scheduling
 
-## Functions
-
-### Tinker
+- a project as a whole has a cron expression in `zimmer.yaml` to determine the schedule of reruns
+- additionally, aswan projects within the dz project can have different cron expressions for scheduling new runs of the aswan projects
 
-> check out a table or few, with a notebook and some basic analysis to help
+### Test projects
 
-### Engineer Research
+TODO: document dogshow and everything else much better here
 
-## Scheduling
-
-- a project as a whole has a cron expression to determine the schedule of reruns
-- additionally, aswan projects within the dz project can have different cron expressions for scheduling new runs of the aswan projects
 
 ## Lookahead
 
 - overlapping names convention
 - resolve naming confusion with colassigner, colaccessor and table feature / composite type / index base classes
 - abstract composite type + subclass of entity class
   - import ACT, inherit from it and specify 
   - importing composite type is impossible now if it contains foreign key :(
-- automatic filter for env creation based on foreign key metadata
 - add option to infer data type of assigned feature
   - can be problematic b/c pandas int/float/nan issue
-- sharing functions among projects
-  - functions specific to processing certain composite / named types
-  - e.g. function dealing with fitting into a limit in dogshow project 1
 - create similar sets of features in a dry way
-- detecting reliance of composite type given by assigner
-  - can wait, as initial import is just the assigner transformed to accessor
 - overlapping in entities
   - detect / signal the same type of entity
-- properly assert importing
+- exports: postgres, postgis , superset
+
+
+### W3C compliancy plan
 
+- test suite for compliance: https://w3c.github.io/csvw/publishing-snapshots/PR-earl/earl.html
+- https://github.com/w3c/csvw
+  - https://www.w3.org/TR/2015/REC-tabular-data-model-20151217/
+  - https://www.w3.org/TR/tabular-metadata/
+
+
+```
+@article{tennison2015model,
+  title={Model for tabular data and metadata on the web},
+  author={Tennison, Jeni and Kellogg, Gregg and Herman, Ivan},
+  year={2015}
+}
+```
+
+```
+@article{pollock2015metadata,
+  title={Metadata vocabulary for tabular data},
+  author={Pollock, Rufus and Tennison, Jeni and Kellogg, Gregg and Herman, Ivan},
+  journal={W3C Recommendation},
+  volume={17},
+  year={2015}
+}
+```
```

