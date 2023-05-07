# Comparing `tmp/intecomm-form-validators-0.1.8.tar.gz` & `tmp/intecomm-form-validators-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intecomm-form-validators-0.1.8.tar", last modified: Wed Jan 25 03:02:46 2023, max compression
+gzip compressed data, was "intecomm-form-validators-0.1.9.tar", last modified: Fri Jan 27 03:28:55 2023, max compression
```

## Comparing `intecomm-form-validators-0.1.8.tar` & `intecomm-form-validators-0.1.9.tar`

### file list

```diff
@@ -1,73 +1,76 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-25 03:02:46.215575 intecomm-form-validators-0.1.8/
--rw-r--r--   0 erikvw     (501) staff       (20)       64 2022-11-01 12:38:32.000000 intecomm-form-validators-0.1.8/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-11-01 12:38:32.000000 intecomm-form-validators-0.1.8/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-25 03:02:46.204774 intecomm-form-validators-0.1.8/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-25 03:02:46.208113 intecomm-form-validators-0.1.8/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     1645 2023-01-25 03:02:38.000000 intecomm-form-validators-0.1.8/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1455 2022-11-01 12:38:32.000000 intecomm-form-validators-0.1.8/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1078 2023-01-25 03:02:38.000000 intecomm-form-validators-0.1.8/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-11-01 12:38:32.000000 intecomm-form-validators-0.1.8/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)      243 2022-11-01 12:38:32.000000 intecomm-form-validators-0.1.8/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)       29 2022-11-01 12:38:32.000000 intecomm-form-validators-0.1.8/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2021-11-22 15:26:51.000000 intecomm-form-validators-0.1.8/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)      189 2022-11-01 12:38:32.000000 intecomm-form-validators-0.1.8/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     1773 2023-01-25 03:02:46.215657 intecomm-form-validators-0.1.8/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)      889 2022-11-01 12:38:32.000000 intecomm-form-validators-0.1.8/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-11-01 12:38:32.000000 intecomm-form-validators-0.1.8/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-25 03:02:46.208905 intecomm-form-validators-0.1.8/intecomm_form_validators/
--rw-r--r--   0 erikvw     (501) staff       (20)      661 2023-01-25 03:02:38.000000 intecomm-form-validators-0.1.8/intecomm_form_validators/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      173 2022-11-01 12:38:32.000000 intecomm-form-validators-0.1.8/intecomm_form_validators/apps.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-25 03:02:46.209949 intecomm-form-validators-0.1.8/intecomm_form_validators/consent/
--rw-r--r--   0 erikvw     (501) staff       (20)       72 2022-11-23 01:16:19.000000 intecomm-form-validators-0.1.8/intecomm_form_validators/consent/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1220 2023-01-25 03:02:38.000000 intecomm-form-validators-0.1.8/intecomm_form_validators/consent/subject_consent_form_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)       78 2022-11-16 00:34:06.000000 intecomm-form-validators-0.1.8/intecomm_form_validators/constants.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-25 03:02:46.210333 intecomm-form-validators-0.1.8/intecomm_form_validators/prn/
--rw-r--r--   0 erikvw     (501) staff       (20)       50 2022-11-29 04:31:30.000000 intecomm-form-validators-0.1.8/intecomm_form_validators/prn/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5471 2022-11-29 04:31:30.000000 intecomm-form-validators-0.1.8/intecomm_form_validators/prn/end_of_study.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-25 03:02:46.212069 intecomm-form-validators-0.1.8/intecomm_form_validators/screening/
--rw-r--r--   0 erikvw     (501) staff       (20)      569 2023-01-25 03:02:38.000000 intecomm-form-validators-0.1.8/intecomm_form_validators/screening/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      107 2022-11-20 02:26:48.000000 intecomm-form-validators-0.1.8/intecomm_form_validators/screening/health_facility_form_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)      106 2022-11-07 21:48:38.000000 intecomm-form-validators-0.1.8/intecomm_form_validators/screening/health_talk_log_form_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1012 2022-11-23 01:16:19.000000 intecomm-form-validators-0.1.8/intecomm_form_validators/screening/patient_call_form_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4164 2023-01-25 03:02:38.000000 intecomm-form-validators-0.1.8/intecomm_form_validators/screening/patient_group_form_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4737 2022-11-23 01:16:19.000000 intecomm-form-validators-0.1.8/intecomm_form_validators/screening/patient_log_form_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)      240 2022-11-01 12:38:32.000000 intecomm-form-validators-0.1.8/intecomm_form_validators/screening/subject_refusal.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6389 2023-01-25 03:02:38.000000 intecomm-form-validators-0.1.8/intecomm_form_validators/screening/subject_screening_form_validator.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-25 03:02:46.213908 intecomm-form-validators-0.1.8/intecomm_form_validators/subject/
--rw-r--r--   0 erikvw     (501) staff       (20)      535 2023-01-25 03:02:38.000000 intecomm-form-validators-0.1.8/intecomm_form_validators/subject/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      509 2022-11-29 04:31:30.000000 intecomm-form-validators-0.1.8/intecomm_form_validators/subject/dm_review_form_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)      282 2022-12-05 19:32:43.000000 intecomm-form-validators-0.1.8/intecomm_form_validators/subject/drug_refill_dm_form_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)      430 2022-11-29 06:07:07.000000 intecomm-form-validators-0.1.8/intecomm_form_validators/subject/drug_refill_hiv_form_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)      283 2022-11-29 04:31:30.000000 intecomm-form-validators-0.1.8/intecomm_form_validators/subject/drug_refill_htn_form_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4836 2023-01-25 03:02:38.000000 intecomm-form-validators-0.1.8/intecomm_form_validators/subject/health_economics_form_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)      994 2022-11-29 04:31:30.000000 intecomm-form-validators-0.1.8/intecomm_form_validators/subject/hiv_review_form_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)      541 2022-11-29 04:31:30.000000 intecomm-form-validators-0.1.8/intecomm_form_validators/subject/htn_review_form_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1351 2022-11-29 04:31:30.000000 intecomm-form-validators-0.1.8/intecomm_form_validators/subject/mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2065 2023-01-25 03:02:38.000000 intecomm-form-validators-0.1.8/intecomm_form_validators/subject/social_harms_form_validator.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-25 03:02:46.214251 intecomm-form-validators-0.1.8/intecomm_form_validators/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-01 12:38:32.000000 intecomm-form-validators-0.1.8/intecomm_form_validators/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-25 03:02:46.214370 intecomm-form-validators-0.1.8/intecomm_form_validators/tests/consent/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-23 01:16:19.000000 intecomm-form-validators-0.1.8/intecomm_form_validators/tests/consent/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-25 03:02:46.214473 intecomm-form-validators-0.1.8/intecomm_form_validators/tests/group/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:26:48.000000 intecomm-form-validators-0.1.8/intecomm_form_validators/tests/group/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1844 2023-01-25 03:02:38.000000 intecomm-form-validators-0.1.8/intecomm_form_validators/tests/mock_models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-25 03:02:46.215120 intecomm-form-validators-0.1.8/intecomm_form_validators/tests/screening/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-01 12:38:32.000000 intecomm-form-validators-0.1.8/intecomm_form_validators/tests/screening/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     9475 2023-01-25 03:02:38.000000 intecomm-form-validators-0.1.8/intecomm_form_validators/tests/screening/test_patient_group.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7048 2022-11-23 01:16:19.000000 intecomm-form-validators-0.1.8/intecomm_form_validators/tests/screening/test_patient_log.py
--rw-r--r--   0 erikvw     (501) staff       (20)     9647 2022-11-20 02:26:48.000000 intecomm-form-validators-0.1.8/intecomm_form_validators/tests/screening/test_subject_screening.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-25 03:02:46.215471 intecomm-form-validators-0.1.8/intecomm_form_validators/tests/subject/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-23 01:16:19.000000 intecomm-form-validators-0.1.8/intecomm_form_validators/tests/subject/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4355 2023-01-25 03:02:38.000000 intecomm-form-validators-0.1.8/intecomm_form_validators/tests/subject/test_social_harms.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1909 2023-01-25 03:02:38.000000 intecomm-form-validators-0.1.8/intecomm_form_validators/tests/test_case_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      118 2022-11-01 12:38:32.000000 intecomm-form-validators-0.1.8/intecomm_form_validators/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4902 2023-01-25 03:02:38.000000 intecomm-form-validators-0.1.8/intecomm_form_validators/utils.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-25 03:02:46.209600 intecomm-form-validators-0.1.8/intecomm_form_validators.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     1773 2023-01-25 03:02:46.000000 intecomm-form-validators-0.1.8/intecomm_form_validators.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     2513 2023-01-25 03:02:46.000000 intecomm-form-validators-0.1.8/intecomm_form_validators.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-01-25 03:02:46.000000 intecomm-form-validators-0.1.8/intecomm_form_validators.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-11-01 02:48:50.000000 intecomm-form-validators-0.1.8/intecomm_form_validators.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       25 2023-01-25 03:02:46.000000 intecomm-form-validators-0.1.8/intecomm_form_validators.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1715 2023-01-25 03:02:38.000000 intecomm-form-validators-0.1.8/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     3331 2023-01-25 03:02:38.000000 intecomm-form-validators-0.1.8/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1193 2023-01-25 03:02:46.216027 intecomm-form-validators-0.1.8/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:28:55.556866 intecomm-form-validators-0.1.9/
+-rw-r--r--   0 erikvw     (501) staff       (20)       64 2022-11-01 12:38:32.000000 intecomm-form-validators-0.1.9/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-11-01 12:38:32.000000 intecomm-form-validators-0.1.9/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:28:55.543253 intecomm-form-validators-0.1.9/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:28:55.547544 intecomm-form-validators-0.1.9/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1645 2023-01-25 03:02:38.000000 intecomm-form-validators-0.1.9/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1455 2022-11-01 12:38:32.000000 intecomm-form-validators-0.1.9/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1078 2023-01-25 03:02:38.000000 intecomm-form-validators-0.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-11-01 12:38:32.000000 intecomm-form-validators-0.1.9/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)      243 2022-11-01 12:38:32.000000 intecomm-form-validators-0.1.9/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)       29 2022-11-01 12:38:32.000000 intecomm-form-validators-0.1.9/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2021-11-22 15:26:51.000000 intecomm-form-validators-0.1.9/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)      189 2022-11-01 12:38:32.000000 intecomm-form-validators-0.1.9/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     1773 2023-01-27 03:28:55.556956 intecomm-form-validators-0.1.9/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)      889 2022-11-01 12:38:32.000000 intecomm-form-validators-0.1.9/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-11-01 12:38:32.000000 intecomm-form-validators-0.1.9/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:28:55.548888 intecomm-form-validators-0.1.9/intecomm_form_validators/
+-rw-r--r--   0 erikvw     (501) staff       (20)      661 2023-01-25 03:02:38.000000 intecomm-form-validators-0.1.9/intecomm_form_validators/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      173 2022-11-01 12:38:32.000000 intecomm-form-validators-0.1.9/intecomm_form_validators/apps.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:28:55.550240 intecomm-form-validators-0.1.9/intecomm_form_validators/consent/
+-rw-r--r--   0 erikvw     (501) staff       (20)       72 2022-11-23 01:16:19.000000 intecomm-form-validators-0.1.9/intecomm_form_validators/consent/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      561 2023-01-27 03:28:48.000000 intecomm-form-validators-0.1.9/intecomm_form_validators/consent/subject_consent_form_validator.py
+-rw-r--r--   0 erikvw     (501) staff       (20)       78 2022-11-16 00:34:06.000000 intecomm-form-validators-0.1.9/intecomm_form_validators/constants.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:28:55.550933 intecomm-form-validators-0.1.9/intecomm_form_validators/prn/
+-rw-r--r--   0 erikvw     (501) staff       (20)       50 2022-11-29 04:31:30.000000 intecomm-form-validators-0.1.9/intecomm_form_validators/prn/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5471 2022-11-29 04:31:30.000000 intecomm-form-validators-0.1.9/intecomm_form_validators/prn/end_of_study.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:28:55.552863 intecomm-form-validators-0.1.9/intecomm_form_validators/screening/
+-rw-r--r--   0 erikvw     (501) staff       (20)      569 2023-01-25 03:02:38.000000 intecomm-form-validators-0.1.9/intecomm_form_validators/screening/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      107 2022-11-20 02:26:48.000000 intecomm-form-validators-0.1.9/intecomm_form_validators/screening/health_facility_form_validator.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      106 2022-11-07 21:48:38.000000 intecomm-form-validators-0.1.9/intecomm_form_validators/screening/health_talk_log_form_validator.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1012 2022-11-23 01:16:19.000000 intecomm-form-validators-0.1.9/intecomm_form_validators/screening/patient_call_form_validator.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4164 2023-01-25 03:02:38.000000 intecomm-form-validators-0.1.9/intecomm_form_validators/screening/patient_group_form_validator.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4737 2022-11-23 01:16:19.000000 intecomm-form-validators-0.1.9/intecomm_form_validators/screening/patient_log_form_validator.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      240 2022-11-01 12:38:32.000000 intecomm-form-validators-0.1.9/intecomm_form_validators/screening/subject_refusal.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6581 2023-01-27 03:28:48.000000 intecomm-form-validators-0.1.9/intecomm_form_validators/screening/subject_screening_form_validator.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:28:55.555239 intecomm-form-validators-0.1.9/intecomm_form_validators/subject/
+-rw-r--r--   0 erikvw     (501) staff       (20)      590 2023-01-27 03:28:48.000000 intecomm-form-validators-0.1.9/intecomm_form_validators/subject/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      382 2023-01-27 03:28:48.000000 intecomm-form-validators-0.1.9/intecomm_form_validators/subject/clinical_review_baseline_form_validator.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      509 2022-11-29 04:31:30.000000 intecomm-form-validators-0.1.9/intecomm_form_validators/subject/dm_review_form_validator.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      282 2022-12-05 19:32:43.000000 intecomm-form-validators-0.1.9/intecomm_form_validators/subject/drug_refill_dm_form_validator.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      430 2022-11-29 06:07:07.000000 intecomm-form-validators-0.1.9/intecomm_form_validators/subject/drug_refill_hiv_form_validator.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      283 2022-11-29 04:31:30.000000 intecomm-form-validators-0.1.9/intecomm_form_validators/subject/drug_refill_htn_form_validator.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4836 2023-01-25 03:02:38.000000 intecomm-form-validators-0.1.9/intecomm_form_validators/subject/health_economics_form_validator.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      994 2022-11-29 04:31:30.000000 intecomm-form-validators-0.1.9/intecomm_form_validators/subject/hiv_review_form_validator.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      541 2022-11-29 04:31:30.000000 intecomm-form-validators-0.1.9/intecomm_form_validators/subject/htn_review_form_validator.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1351 2022-11-29 04:31:30.000000 intecomm-form-validators-0.1.9/intecomm_form_validators/subject/mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2065 2023-01-25 03:02:38.000000 intecomm-form-validators-0.1.9/intecomm_form_validators/subject/social_harms_form_validator.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3454 2023-01-27 03:28:48.000000 intecomm-form-validators-0.1.9/intecomm_form_validators/subject/vitals_form_validator.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:28:55.555573 intecomm-form-validators-0.1.9/intecomm_form_validators/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-01 12:38:32.000000 intecomm-form-validators-0.1.9/intecomm_form_validators/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:28:55.555693 intecomm-form-validators-0.1.9/intecomm_form_validators/tests/consent/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-23 01:16:19.000000 intecomm-form-validators-0.1.9/intecomm_form_validators/tests/consent/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:28:55.555802 intecomm-form-validators-0.1.9/intecomm_form_validators/tests/group/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:26:48.000000 intecomm-form-validators-0.1.9/intecomm_form_validators/tests/group/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2753 2023-01-27 03:28:48.000000 intecomm-form-validators-0.1.9/intecomm_form_validators/tests/mock_models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:28:55.556286 intecomm-form-validators-0.1.9/intecomm_form_validators/tests/screening/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-01 12:38:32.000000 intecomm-form-validators-0.1.9/intecomm_form_validators/tests/screening/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     9475 2023-01-25 03:02:38.000000 intecomm-form-validators-0.1.9/intecomm_form_validators/tests/screening/test_patient_group.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7048 2022-11-23 01:16:19.000000 intecomm-form-validators-0.1.9/intecomm_form_validators/tests/screening/test_patient_log.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     9647 2022-11-20 02:26:48.000000 intecomm-form-validators-0.1.9/intecomm_form_validators/tests/screening/test_subject_screening.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:28:55.556755 intecomm-form-validators-0.1.9/intecomm_form_validators/tests/subject/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-23 01:16:19.000000 intecomm-form-validators-0.1.9/intecomm_form_validators/tests/subject/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4355 2023-01-25 03:02:38.000000 intecomm-form-validators-0.1.9/intecomm_form_validators/tests/subject/test_social_harms.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     9083 2023-01-27 03:28:48.000000 intecomm-form-validators-0.1.9/intecomm_form_validators/tests/subject/test_vitals.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2402 2023-01-27 03:28:48.000000 intecomm-form-validators-0.1.9/intecomm_form_validators/tests/test_case_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      118 2022-11-01 12:38:32.000000 intecomm-form-validators-0.1.9/intecomm_form_validators/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5079 2023-01-27 03:28:48.000000 intecomm-form-validators-0.1.9/intecomm_form_validators/utils.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:28:55.549819 intecomm-form-validators-0.1.9/intecomm_form_validators.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1773 2023-01-27 03:28:55.000000 intecomm-form-validators-0.1.9/intecomm_form_validators.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     2701 2023-01-27 03:28:55.000000 intecomm-form-validators-0.1.9/intecomm_form_validators.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-01-27 03:28:55.000000 intecomm-form-validators-0.1.9/intecomm_form_validators.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-11-01 02:48:50.000000 intecomm-form-validators-0.1.9/intecomm_form_validators.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       25 2023-01-27 03:28:55.000000 intecomm-form-validators-0.1.9/intecomm_form_validators.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1741 2023-01-27 03:28:48.000000 intecomm-form-validators-0.1.9/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     3331 2023-01-25 03:02:38.000000 intecomm-form-validators-0.1.9/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1193 2023-01-27 03:28:55.557350 intecomm-form-validators-0.1.9/setup.cfg
```

### Comparing `intecomm-form-validators-0.1.8/.github/workflows/build.yml` & `intecomm-form-validators-0.1.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `intecomm-form-validators-0.1.8/.gitignore` & `intecomm-form-validators-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `intecomm-form-validators-0.1.8/.pre-commit-config.yaml` & `intecomm-form-validators-0.1.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `intecomm-form-validators-0.1.8/LICENSE` & `intecomm-form-validators-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `intecomm-form-validators-0.1.8/PKG-INFO` & `intecomm-form-validators-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intecomm-form-validators
-Version: 0.1.8
+Version: 0.1.9
 Summary: INTECOMM EDC form validators
 Home-page: https://github.com/intecomm-trial/intecomm-form-validators
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc INTECOMM EDC form validators,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `intecomm-form-validators-0.1.8/README.rst` & `intecomm-form-validators-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `intecomm-form-validators-0.1.8/intecomm_form_validators/__init__.py` & `intecomm-form-validators-0.1.9/intecomm_form_validators/__init__.py`

 * *Files identical despite different names*

### Comparing `intecomm-form-validators-0.1.8/intecomm_form_validators/prn/end_of_study.py` & `intecomm-form-validators-0.1.9/intecomm_form_validators/prn/end_of_study.py`

 * *Files identical despite different names*

### Comparing `intecomm-form-validators-0.1.8/intecomm_form_validators/screening/__init__.py` & `intecomm-form-validators-0.1.9/intecomm_form_validators/screening/__init__.py`

 * *Files identical despite different names*

### Comparing `intecomm-form-validators-0.1.8/intecomm_form_validators/screening/patient_call_form_validator.py` & `intecomm-form-validators-0.1.9/intecomm_form_validators/screening/patient_call_form_validator.py`

 * *Files identical despite different names*

### Comparing `intecomm-form-validators-0.1.8/intecomm_form_validators/screening/patient_group_form_validator.py` & `intecomm-form-validators-0.1.9/intecomm_form_validators/screening/patient_group_form_validator.py`

 * *Files identical despite different names*

### Comparing `intecomm-form-validators-0.1.8/intecomm_form_validators/screening/patient_log_form_validator.py` & `intecomm-form-validators-0.1.9/intecomm_form_validators/screening/patient_log_form_validator.py`

 * *Files identical despite different names*

### Comparing `intecomm-form-validators-0.1.8/intecomm_form_validators/screening/subject_screening_form_validator.py` & `intecomm-form-validators-0.1.9/intecomm_form_validators/screening/subject_screening_form_validator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from dateutil.relativedelta import relativedelta
+from django.utils.html import format_html
 from edc_constants.constants import DM, HIV, HTN, MALE, NO, YES
 from edc_form_validators import INVALID_ERROR, FormValidator
 from edc_model import InvalidFormat, duration_to_date
 from edc_screening.form_validator_mixins import SubjectScreeningFormValidatorMixin
 
 INVALID_DURATION_IN_CARE = "invalid_duration_in_care"
 
@@ -40,22 +41,23 @@
 
         self.required_if(
             YES, field="unsuitable_for_study", field_required="reasons_unsuitable"
         )
 
     def validate_stable_in_care_on_patient_log(self):
         if self.patient_log.stable != YES:
-            self.raise_validation_error(
-                {
-                    "__all__": (
-                        "Invalid. Patient not reported as stable in care. See Patient Log."
-                    )
-                },
-                INVALID_ERROR,
+            link = (
+                f'<a href="{self.patient_log.get_changelist_url()}?'
+                f'q={str(self.patient_log.id)}">{self.patient_log}</a>'
+            )
+            errmsg = format_html(
+                "Invalid. Patient is not known to be stable and in-care. "
+                f"See patient log for {link}."
             )
+            self.raise_validation_error(errmsg, error_code=INVALID_ERROR)
 
         pass
 
     def validate_gender_against_patient_log(self):
         if self.cleaned_data.get("gender") != self.patient_log.gender:
             self.raise_validation_error(
                 {
```

### Comparing `intecomm-form-validators-0.1.8/intecomm_form_validators/subject/__init__.py` & `intecomm-form-validators-0.1.9/intecomm_form_validators/subject/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,7 +2,8 @@
 from .drug_refill_dm_form_validator import DrugRefillDmFormValidator
 from .drug_refill_hiv_form_validator import DrugRefillHivFormValidator
 from .drug_refill_htn_form_validator import DrugRefillHtnFormValidator
 from .health_economics_form_validator import HealthEconomicsFormValidator
 from .hiv_review_form_validator import HivReviewFormValidator
 from .htn_review_form_validator import HtnReviewFormValidator
 from .social_harms_form_validator import SocialHarmsFormValidator
+from .vitals_form_validator import VitalsFormValidator
```

### Comparing `intecomm-form-validators-0.1.8/intecomm_form_validators/subject/health_economics_form_validator.py` & `intecomm-form-validators-0.1.9/intecomm_form_validators/subject/health_economics_form_validator.py`

 * *Files identical despite different names*

### Comparing `intecomm-form-validators-0.1.8/intecomm_form_validators/subject/hiv_review_form_validator.py` & `intecomm-form-validators-0.1.9/intecomm_form_validators/subject/hiv_review_form_validator.py`

 * *Files identical despite different names*

### Comparing `intecomm-form-validators-0.1.8/intecomm_form_validators/subject/htn_review_form_validator.py` & `intecomm-form-validators-0.1.9/intecomm_form_validators/subject/htn_review_form_validator.py`

 * *Files identical despite different names*

### Comparing `intecomm-form-validators-0.1.8/intecomm_form_validators/subject/mixins.py` & `intecomm-form-validators-0.1.9/intecomm_form_validators/subject/mixins.py`

 * *Files identical despite different names*

### Comparing `intecomm-form-validators-0.1.8/intecomm_form_validators/subject/social_harms_form_validator.py` & `intecomm-form-validators-0.1.9/intecomm_form_validators/subject/social_harms_form_validator.py`

 * *Files identical despite different names*

### Comparing `intecomm-form-validators-0.1.8/intecomm_form_validators/tests/mock_models.py` & `intecomm-form-validators-0.1.9/intecomm_form_validators/tests/mock_models.py`

 * *Files 14% similar despite different names*

```diff
@@ -56,7 +56,32 @@
 
 
 class SocialHarmsMockModel(MockModel):
     def __init__(self, *args, **kwargs):
         kwargs["mock_name"] = "SocialHarms"
         super().__init__(*args, **kwargs)
         self._meta.label_lower = "intecomm_subject.socialharms"
+
+
+class VitalsMockModel(MockModel):
+    def __init__(self, *args, **kwargs):
+        kwargs["mock_name"] = "Vitals"
+        super().__init__(*args, **kwargs)
+        self._meta.label_lower = "intecomm_subject.vitals"
+
+
+class AppointmentMockModel(MockModel):
+    def __init__(self, *args, **kwargs):
+        kwargs["mock_name"] = "Appointment"
+        super().__init__(*args, **kwargs)
+        self.visit_schedule_name = "visit_schedule"
+        self._meta.label_lower = "edc_appointment.appointment"
+
+
+class SubjectVisitMockModel(MockModel):
+    def __init__(self, appointment, *args, **kwargs):
+        kwargs["mock_name"] = "SubjectVisit"
+        super().__init__(*args, **kwargs)
+        self.appointment = appointment
+        self.visit_schedule_name = appointment.visit_schedule_name
+        self.schedule_name = appointment.schedule_name
+        self._meta.label_lower = "intecomm_subject.subjectvisit"
```

### Comparing `intecomm-form-validators-0.1.8/intecomm_form_validators/tests/screening/test_patient_group.py` & `intecomm-form-validators-0.1.9/intecomm_form_validators/tests/screening/test_patient_group.py`

 * *Files identical despite different names*

### Comparing `intecomm-form-validators-0.1.8/intecomm_form_validators/tests/screening/test_patient_log.py` & `intecomm-form-validators-0.1.9/intecomm_form_validators/tests/screening/test_patient_log.py`

 * *Files identical despite different names*

### Comparing `intecomm-form-validators-0.1.8/intecomm_form_validators/tests/screening/test_subject_screening.py` & `intecomm-form-validators-0.1.9/intecomm_form_validators/tests/screening/test_subject_screening.py`

 * *Files identical despite different names*

### Comparing `intecomm-form-validators-0.1.8/intecomm_form_validators/tests/subject/test_social_harms.py` & `intecomm-form-validators-0.1.9/intecomm_form_validators/tests/subject/test_social_harms.py`

 * *Files identical despite different names*

### Comparing `intecomm-form-validators-0.1.8/intecomm_form_validators/tests/test_case_mixin.py` & `intecomm-form-validators-0.1.9/intecomm_form_validators/tests/test_case_mixin.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from __future__ import annotations
 
 from django.test import TestCase
 from django_mock_queries.query import MockSet
 from edc_constants.constants import DM, HIV, HTN, NO, YES
 
-from intecomm_form_validators.tests.mock_models import (
+from .mock_models import (
+    AppointmentMockModel,
     ConditionsMockModel,
     PatientLogMockModel,
+    SubjectVisitMockModel,
 )
 
 
 class TestCaseMixin(TestCase):
     def get_mock_patients(
         self,
         ratio: list[int, int, int] | None = None,
@@ -47,7 +49,22 @@
             stable=stable,
             screening_identifier=screening_identifier,
             subject_identifier=subject_identifier,
             conditions=MockSet(
                 *[ConditionsMockModel(name=x) for x in conditions],
             ),
         )
+
+    @staticmethod
+    def get_subject_visit(
+        schedule_name: str = None,
+        visit_code: str = None,
+        visit_code_sequence: int = None,
+        timepoint: int = None,
+    ):
+        appointment = AppointmentMockModel(
+            schedule_name=schedule_name,
+            visit_code=visit_code,
+            visit_code_sequence=visit_code_sequence,
+            timepoint=timepoint,
+        )
+        return SubjectVisitMockModel(appointment=appointment)
```

### Comparing `intecomm-form-validators-0.1.8/intecomm_form_validators/utils.py` & `intecomm-form-validators-0.1.9/intecomm_form_validators/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import Tuple
 
 from django.conf import settings
 from django.db.models import QuerySet
 from django.utils.html import format_html
 from edc_constants.constants import DM, HIV, HTN, YES
 from edc_utils import round_up
+from edc_visit_schedule.constants import MONTH12
 
 
 class PatientNotStableError(Exception):
     pass
 
 
 class PatientNotScreenedError(Exception):
@@ -30,14 +31,18 @@
     pass
 
 
 class PatientGroupMakeupError(Exception):
     pass
 
 
+def is_end_of_study(subject_visit):
+    return subject_visit.visit_code == MONTH12 and subject_visit.visit_code_sequence == 0
+
+
 def get_min_group_size() -> int:
     """Returns minimum number of patients needed to form a group"""
     return getattr(settings, "INTECOMM_MIN_GROUP_SIZE", 14)
 
 
 def get_group_size_for_ratio() -> int:
     """Returns number of patients to use to determine the condition
```

### Comparing `intecomm-form-validators-0.1.8/intecomm_form_validators.egg-info/PKG-INFO` & `intecomm-form-validators-0.1.9/intecomm_form_validators.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intecomm-form-validators
-Version: 0.1.8
+Version: 0.1.9
 Summary: INTECOMM EDC form validators
 Home-page: https://github.com/intecomm-trial/intecomm-form-validators
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc INTECOMM EDC form validators,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `intecomm-form-validators-0.1.8/intecomm_form_validators.egg-info/SOURCES.txt` & `intecomm-form-validators-0.1.9/intecomm_form_validators.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -32,27 +32,30 @@
 intecomm_form_validators/screening/health_talk_log_form_validator.py
 intecomm_form_validators/screening/patient_call_form_validator.py
 intecomm_form_validators/screening/patient_group_form_validator.py
 intecomm_form_validators/screening/patient_log_form_validator.py
 intecomm_form_validators/screening/subject_refusal.py
 intecomm_form_validators/screening/subject_screening_form_validator.py
 intecomm_form_validators/subject/__init__.py
+intecomm_form_validators/subject/clinical_review_baseline_form_validator.py
 intecomm_form_validators/subject/dm_review_form_validator.py
 intecomm_form_validators/subject/drug_refill_dm_form_validator.py
 intecomm_form_validators/subject/drug_refill_hiv_form_validator.py
 intecomm_form_validators/subject/drug_refill_htn_form_validator.py
 intecomm_form_validators/subject/health_economics_form_validator.py
 intecomm_form_validators/subject/hiv_review_form_validator.py
 intecomm_form_validators/subject/htn_review_form_validator.py
 intecomm_form_validators/subject/mixins.py
 intecomm_form_validators/subject/social_harms_form_validator.py
+intecomm_form_validators/subject/vitals_form_validator.py
 intecomm_form_validators/tests/__init__.py
 intecomm_form_validators/tests/mock_models.py
 intecomm_form_validators/tests/test_case_mixin.py
 intecomm_form_validators/tests/consent/__init__.py
 intecomm_form_validators/tests/group/__init__.py
 intecomm_form_validators/tests/screening/__init__.py
 intecomm_form_validators/tests/screening/test_patient_group.py
 intecomm_form_validators/tests/screening/test_patient_log.py
 intecomm_form_validators/tests/screening/test_subject_screening.py
 intecomm_form_validators/tests/subject/__init__.py
-intecomm_form_validators/tests/subject/test_social_harms.py
+intecomm_form_validators/tests/subject/test_social_harms.py
+intecomm_form_validators/tests/subject/test_vitals.py
```

### Comparing `intecomm-form-validators-0.1.8/pyproject.toml` & `intecomm-form-validators-0.1.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -59,14 +59,15 @@
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/third_party_dev.txt
     dj41: Django>=4.1,<4.2
     djdev: https://github.com/django/django/tarball/main
 
 commands =
     pip install -U pip
     pip --version
+    pip install -U edc-rx
     pip freeze
     coverage run -a runtests.py
     coverage report
 
 [testenv:lint]
 deps = -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/lint.txt
 commands =
```

### Comparing `intecomm-form-validators-0.1.8/runtests.py` & `intecomm-form-validators-0.1.9/runtests.py`

 * *Files identical despite different names*

### Comparing `intecomm-form-validators-0.1.8/setup.cfg` & `intecomm-form-validators-0.1.9/setup.cfg`

 * *Files identical despite different names*

