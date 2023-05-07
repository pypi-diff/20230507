# Comparing `tmp/wn-0.9.3.tar.gz` & `tmp/wn-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wn-0.9.3.tar", last modified: Mon Nov 14 06:35:29 2022, max compression
+gzip compressed data, was "wn-0.9.4.tar", last modified: Sun May  7 18:55:12 2023, max compression
```

## Comparing `wn-0.9.3.tar` & `wn-0.9.4.tar`

### file list

```diff
@@ -1,90 +1,90 @@
--rw-r--r--   0        0        0     1098 2022-11-14 06:35:10.544525 wn-0.9.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0     1117 2022-11-14 06:35:10.544525 wn-0.9.3/.github/ISSUE_TEMPLATE/data-issue.md
--rw-r--r--   0        0        0      604 2022-11-14 06:35:10.544525 wn-0.9.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1230 2022-11-14 06:35:10.544525 wn-0.9.3/.github/workflows/checks.yml
--rw-r--r--   0        0        0      850 2022-11-14 06:35:10.544525 wn-0.9.3/.github/workflows/release.yml
--rw-r--r--   0        0        0     1817 2022-11-14 06:35:10.544525 wn-0.9.3/.gitignore
--rw-r--r--   0        0        0    19365 2022-11-14 06:35:10.544525 wn-0.9.3/CHANGELOG.md
--rw-r--r--   0        0        0     1204 2022-11-14 06:35:10.544525 wn-0.9.3/CITATION.cff
--rw-r--r--   0        0        0     2979 2022-11-14 06:35:10.548525 wn-0.9.3/CONTRIBUTING.md
--rw-r--r--   0        0        0     1078 2022-11-14 06:35:10.548525 wn-0.9.3/LICENSE
--rw-r--r--   0        0        0    11778 2022-11-14 06:35:10.548525 wn-0.9.3/README.md
--rw-r--r--   0        0        0      634 2022-11-14 06:35:10.548525 wn-0.9.3/docs/Makefile
--rw-r--r--   0        0        0      205 2022-11-14 06:35:10.548525 wn-0.9.3/docs/_static/css/svg.css
--rw-r--r--   0        0        0    23062 2022-11-14 06:35:10.548525 wn-0.9.3/docs/_static/demo.ipynb
--rw-r--r--   0        0        0     1570 2022-11-14 06:35:10.548525 wn-0.9.3/docs/_static/wn-logo-rotate.svg
--rw-r--r--   0        0        0      871 2022-11-14 06:35:10.548525 wn-0.9.3/docs/_static/wn-logo.svg
--rw-r--r--   0        0        0     9110 2022-11-14 06:35:10.548525 wn-0.9.3/docs/api/wn.constants.rst
--rw-r--r--   0        0        0     7040 2022-11-14 06:35:10.548525 wn-0.9.3/docs/api/wn.ic.rst
--rw-r--r--   0        0        0      121 2022-11-14 06:35:10.548525 wn-0.9.3/docs/api/wn.lmf.rst
--rw-r--r--   0        0        0     3210 2022-11-14 06:35:10.548525 wn-0.9.3/docs/api/wn.morphy.rst
--rw-r--r--   0        0        0      439 2022-11-14 06:35:10.548525 wn-0.9.3/docs/api/wn.project.rst
--rw-r--r--   0        0        0     8403 2022-11-14 06:35:10.548525 wn-0.9.3/docs/api/wn.rst
--rw-r--r--   0        0        0     6086 2022-11-14 06:35:10.548525 wn-0.9.3/docs/api/wn.similarity.rst
--rw-r--r--   0        0        0     2206 2022-11-14 06:35:10.548525 wn-0.9.3/docs/api/wn.taxonomy.rst
--rw-r--r--   0        0        0      628 2022-11-14 06:35:10.548525 wn-0.9.3/docs/api/wn.util.rst
--rw-r--r--   0        0        0       82 2022-11-14 06:35:10.548525 wn-0.9.3/docs/api/wn.validate.rst
--rw-r--r--   0        0        0    12574 2022-11-14 06:35:10.548525 wn-0.9.3/docs/api/wn.web.rst
--rw-r--r--   0        0        0     2889 2022-11-14 06:35:10.548525 wn-0.9.3/docs/cli.rst
--rw-r--r--   0        0        0     3793 2022-11-14 06:35:10.548525 wn-0.9.3/docs/conf.py
--rw-r--r--   0        0        0       52 2022-11-14 06:35:10.548525 wn-0.9.3/docs/docutils.conf
--rw-r--r--   0        0        0     5386 2022-11-14 06:35:10.548525 wn-0.9.3/docs/faq.rst
--rw-r--r--   0        0        0     8841 2022-11-14 06:35:10.548525 wn-0.9.3/docs/guides/basic.rst
--rw-r--r--   0        0        0     9536 2022-11-14 06:35:10.548525 wn-0.9.3/docs/guides/images/sense-sense.svg
--rw-r--r--   0        0        0    10742 2022-11-14 06:35:10.548525 wn-0.9.3/docs/guides/images/sense-synset.svg
--rw-r--r--   0        0        0    14876 2022-11-14 06:35:10.548525 wn-0.9.3/docs/guides/images/synset-synset.svg
--rw-r--r--   0        0        0    17621 2022-11-14 06:35:10.548525 wn-0.9.3/docs/guides/images/word-sense-synset.svg
--rw-r--r--   0        0        0     8552 2022-11-14 06:35:10.548525 wn-0.9.3/docs/guides/interlingual.rst
--rw-r--r--   0        0        0     9766 2022-11-14 06:35:10.548525 wn-0.9.3/docs/guides/lemmatization.rst
--rw-r--r--   0        0        0     6671 2022-11-14 06:35:10.548525 wn-0.9.3/docs/guides/lexicons.rst
--rw-r--r--   0        0        0     4370 2022-11-14 06:35:10.548525 wn-0.9.3/docs/guides/nltk-migration.rst
--rw-r--r--   0        0        0     5917 2022-11-14 06:35:10.548525 wn-0.9.3/docs/guides/wordnet.rst
--rw-r--r--   0        0        0     1320 2022-11-14 06:35:10.548525 wn-0.9.3/docs/index.rst
--rw-r--r--   0        0        0      795 2022-11-14 06:35:10.548525 wn-0.9.3/docs/make.bat
--rw-r--r--   0        0        0       62 2022-11-14 06:35:10.548525 wn-0.9.3/docs/requirements.txt
--rw-r--r--   0        0        0     3584 2022-11-14 06:35:10.548525 wn-0.9.3/docs/setup.rst
--rw-r--r--   0        0        0      320 2022-11-14 06:35:10.548525 wn-0.9.3/noxfile.py
--rw-r--r--   0        0        0     1659 2022-11-14 06:35:10.548525 wn-0.9.3/pyproject.toml
--rw-r--r--   0        0        0     1951 2022-11-14 06:35:10.548525 wn-0.9.3/tests/conftest.py
--rw-r--r--   0        0        0       98 2022-11-14 06:35:10.548525 wn-0.9.3/tests/data/README.md
--rw-r--r--   0        0        0     8838 2022-11-14 06:35:10.548525 wn-0.9.3/tests/data/mini-lmf-1.0.xml
--rw-r--r--   0        0        0     5677 2022-11-14 06:35:10.548525 wn-0.9.3/tests/data/mini-lmf-1.1.xml
--rw-r--r--   0        0        0     1854 2022-11-14 06:35:10.548525 wn-0.9.3/tests/db_test.py
--rw-r--r--   0        0        0      752 2022-11-14 06:35:10.548525 wn-0.9.3/tests/export_test.py
--rw-r--r--   0        0        0     3833 2022-11-14 06:35:10.548525 wn-0.9.3/tests/ic_test.py
--rw-r--r--   0        0        0     3263 2022-11-14 06:35:10.548525 wn-0.9.3/tests/lmf_test.py
--rw-r--r--   0        0        0     2140 2022-11-14 06:35:10.548525 wn-0.9.3/tests/morphy_test.py
--rw-r--r--   0        0        0     9281 2022-11-14 06:35:10.548525 wn-0.9.3/tests/primary_query_test.py
--rw-r--r--   0        0        0     4188 2022-11-14 06:35:10.548525 wn-0.9.3/tests/relations_test.py
--rw-r--r--   0        0        0     4600 2022-11-14 06:35:10.548525 wn-0.9.3/tests/secondary_query_test.py
--rw-r--r--   0        0        0     6901 2022-11-14 06:35:10.548525 wn-0.9.3/tests/similarity_test.py
--rw-r--r--   0        0        0     4142 2022-11-14 06:35:10.548525 wn-0.9.3/tests/taxonomy_test.py
--rw-r--r--   0        0        0      361 2022-11-14 06:35:10.548525 wn-0.9.3/tests/util_test.py
--rw-r--r--   0        0        0     2754 2022-11-14 06:35:10.548525 wn-0.9.3/tests/wordnet_test.py
--rw-r--r--   0        0        0      974 2022-11-14 06:35:10.548525 wn-0.9.3/wn/__init__.py
--rw-r--r--   0        0        0     5022 2022-11-14 06:35:10.548525 wn-0.9.3/wn/__main__.py
--rw-r--r--   0        0        0    32182 2022-11-14 06:35:10.548525 wn-0.9.3/wn/_add.py
--rw-r--r--   0        0        0     9060 2022-11-14 06:35:10.548525 wn-0.9.3/wn/_config.py
--rw-r--r--   0        0        0    49402 2022-11-14 06:35:10.552525 wn-0.9.3/wn/_core.py
--rw-r--r--   0        0        0     3860 2022-11-14 06:35:10.552525 wn-0.9.3/wn/_db.py
--rw-r--r--   0        0        0     4759 2022-11-14 06:35:10.552525 wn-0.9.3/wn/_download.py
--rw-r--r--   0        0        0      674 2022-11-14 06:35:10.552525 wn-0.9.3/wn/_exceptions.py
--rw-r--r--   0        0        0    10885 2022-11-14 06:35:10.552525 wn-0.9.3/wn/_export.py
--rw-r--r--   0        0        0     1072 2022-11-14 06:35:10.552525 wn-0.9.3/wn/_ili.py
--rw-r--r--   0        0        0    23194 2022-11-14 06:35:10.552525 wn-0.9.3/wn/_queries.py
--rw-r--r--   0        0        0      919 2022-11-14 06:35:10.552525 wn-0.9.3/wn/_types.py
--rw-r--r--   0        0        0     1843 2022-11-14 06:35:10.552525 wn-0.9.3/wn/_util.py
--rw-r--r--   0        0        0     7710 2022-11-14 06:35:10.552525 wn-0.9.3/wn/constants.py
--rw-r--r--   0        0        0     6698 2022-11-14 06:35:10.552525 wn-0.9.3/wn/ic.py
--rw-r--r--   0        0        0    14846 2022-11-14 06:35:10.552525 wn-0.9.3/wn/index.toml
--rw-r--r--   0        0        0    29674 2022-11-14 06:35:10.552525 wn-0.9.3/wn/lmf.py
--rw-r--r--   0        0        0      268 2022-11-14 06:35:10.552525 wn-0.9.3/wn/metrics.py
--rw-r--r--   0        0        0     4924 2022-11-14 06:35:10.552525 wn-0.9.3/wn/morphy.py
--rw-r--r--   0        0        0     6788 2022-11-14 06:35:10.552525 wn-0.9.3/wn/project.py
--rw-r--r--   0        0        0     9170 2022-11-14 06:35:10.552525 wn-0.9.3/wn/schema.sql
--rw-r--r--   0        0        0     8113 2022-11-14 06:35:10.552525 wn-0.9.3/wn/similarity.py
--rw-r--r--   0        0        0    11236 2022-11-14 06:35:10.552525 wn-0.9.3/wn/taxonomy.py
--rw-r--r--   0        0        0     6358 2022-11-14 06:35:10.552525 wn-0.9.3/wn/util.py
--rw-r--r--   0        0        0    10790 2022-11-14 06:35:10.552525 wn-0.9.3/wn/validate.py
--rw-r--r--   0        0        0     9594 2022-11-14 06:35:10.552525 wn-0.9.3/wn/web.py
--rw-r--r--   0        0        0    13662 1970-01-01 00:00:00.000000 wn-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0     1098 2023-05-07 18:54:48.995710 wn-0.9.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0     1117 2023-05-07 18:54:48.995710 wn-0.9.4/.github/ISSUE_TEMPLATE/data-issue.md
+-rw-r--r--   0        0        0      604 2023-05-07 18:54:48.995710 wn-0.9.4/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1230 2023-05-07 18:54:48.995710 wn-0.9.4/.github/workflows/checks.yml
+-rw-r--r--   0        0        0      850 2023-05-07 18:54:48.995710 wn-0.9.4/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1817 2023-05-07 18:54:48.995710 wn-0.9.4/.gitignore
+-rw-r--r--   0        0        0    19640 2023-05-07 18:54:48.995710 wn-0.9.4/CHANGELOG.md
+-rw-r--r--   0        0        0     1204 2023-05-07 18:54:48.995710 wn-0.9.4/CITATION.cff
+-rw-r--r--   0        0        0     2979 2023-05-07 18:54:48.995710 wn-0.9.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1078 2023-05-07 18:54:48.995710 wn-0.9.4/LICENSE
+-rw-r--r--   0        0        0    11835 2023-05-07 18:54:48.995710 wn-0.9.4/README.md
+-rw-r--r--   0        0        0      634 2023-05-07 18:54:48.995710 wn-0.9.4/docs/Makefile
+-rw-r--r--   0        0        0      205 2023-05-07 18:54:48.995710 wn-0.9.4/docs/_static/css/svg.css
+-rw-r--r--   0        0        0    23062 2023-05-07 18:54:48.995710 wn-0.9.4/docs/_static/demo.ipynb
+-rw-r--r--   0        0        0     1570 2023-05-07 18:54:48.995710 wn-0.9.4/docs/_static/wn-logo-rotate.svg
+-rw-r--r--   0        0        0      871 2023-05-07 18:54:48.995710 wn-0.9.4/docs/_static/wn-logo.svg
+-rw-r--r--   0        0        0     9110 2023-05-07 18:54:48.995710 wn-0.9.4/docs/api/wn.constants.rst
+-rw-r--r--   0        0        0     7040 2023-05-07 18:54:48.995710 wn-0.9.4/docs/api/wn.ic.rst
+-rw-r--r--   0        0        0      121 2023-05-07 18:54:48.995710 wn-0.9.4/docs/api/wn.lmf.rst
+-rw-r--r--   0        0        0     3210 2023-05-07 18:54:48.995710 wn-0.9.4/docs/api/wn.morphy.rst
+-rw-r--r--   0        0        0      439 2023-05-07 18:54:48.995710 wn-0.9.4/docs/api/wn.project.rst
+-rw-r--r--   0        0        0     8403 2023-05-07 18:54:48.995710 wn-0.9.4/docs/api/wn.rst
+-rw-r--r--   0        0        0     6086 2023-05-07 18:54:48.995710 wn-0.9.4/docs/api/wn.similarity.rst
+-rw-r--r--   0        0        0     2206 2023-05-07 18:54:48.995710 wn-0.9.4/docs/api/wn.taxonomy.rst
+-rw-r--r--   0        0        0      628 2023-05-07 18:54:48.999710 wn-0.9.4/docs/api/wn.util.rst
+-rw-r--r--   0        0        0       82 2023-05-07 18:54:48.999710 wn-0.9.4/docs/api/wn.validate.rst
+-rw-r--r--   0        0        0    12574 2023-05-07 18:54:48.999710 wn-0.9.4/docs/api/wn.web.rst
+-rw-r--r--   0        0        0     2931 2023-05-07 18:54:48.999710 wn-0.9.4/docs/cli.rst
+-rw-r--r--   0        0        0     3793 2023-05-07 18:54:48.999710 wn-0.9.4/docs/conf.py
+-rw-r--r--   0        0        0       52 2023-05-07 18:54:48.999710 wn-0.9.4/docs/docutils.conf
+-rw-r--r--   0        0        0     5386 2023-05-07 18:54:48.999710 wn-0.9.4/docs/faq.rst
+-rw-r--r--   0        0        0     8841 2023-05-07 18:54:48.999710 wn-0.9.4/docs/guides/basic.rst
+-rw-r--r--   0        0        0     9536 2023-05-07 18:54:48.999710 wn-0.9.4/docs/guides/images/sense-sense.svg
+-rw-r--r--   0        0        0    10742 2023-05-07 18:54:48.999710 wn-0.9.4/docs/guides/images/sense-synset.svg
+-rw-r--r--   0        0        0    14876 2023-05-07 18:54:48.999710 wn-0.9.4/docs/guides/images/synset-synset.svg
+-rw-r--r--   0        0        0    17621 2023-05-07 18:54:48.999710 wn-0.9.4/docs/guides/images/word-sense-synset.svg
+-rw-r--r--   0        0        0     8552 2023-05-07 18:54:48.999710 wn-0.9.4/docs/guides/interlingual.rst
+-rw-r--r--   0        0        0     9766 2023-05-07 18:54:48.999710 wn-0.9.4/docs/guides/lemmatization.rst
+-rw-r--r--   0        0        0     6671 2023-05-07 18:54:48.999710 wn-0.9.4/docs/guides/lexicons.rst
+-rw-r--r--   0        0        0     4370 2023-05-07 18:54:48.999710 wn-0.9.4/docs/guides/nltk-migration.rst
+-rw-r--r--   0        0        0     5917 2023-05-07 18:54:48.999710 wn-0.9.4/docs/guides/wordnet.rst
+-rw-r--r--   0        0        0     1320 2023-05-07 18:54:48.999710 wn-0.9.4/docs/index.rst
+-rw-r--r--   0        0        0      795 2023-05-07 18:54:48.999710 wn-0.9.4/docs/make.bat
+-rw-r--r--   0        0        0       62 2023-05-07 18:54:48.999710 wn-0.9.4/docs/requirements.txt
+-rw-r--r--   0        0        0     3584 2023-05-07 18:54:48.999710 wn-0.9.4/docs/setup.rst
+-rw-r--r--   0        0        0      320 2023-05-07 18:54:48.999710 wn-0.9.4/noxfile.py
+-rw-r--r--   0        0        0     1610 2023-05-07 18:54:48.999710 wn-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0     1951 2023-05-07 18:54:48.999710 wn-0.9.4/tests/conftest.py
+-rw-r--r--   0        0        0       98 2023-05-07 18:54:48.999710 wn-0.9.4/tests/data/README.md
+-rw-r--r--   0        0        0     8838 2023-05-07 18:54:48.999710 wn-0.9.4/tests/data/mini-lmf-1.0.xml
+-rw-r--r--   0        0        0     5677 2023-05-07 18:54:48.999710 wn-0.9.4/tests/data/mini-lmf-1.1.xml
+-rw-r--r--   0        0        0     1854 2023-05-07 18:54:48.999710 wn-0.9.4/tests/db_test.py
+-rw-r--r--   0        0        0      752 2023-05-07 18:54:48.999710 wn-0.9.4/tests/export_test.py
+-rw-r--r--   0        0        0     3833 2023-05-07 18:54:48.999710 wn-0.9.4/tests/ic_test.py
+-rw-r--r--   0        0        0     3263 2023-05-07 18:54:48.999710 wn-0.9.4/tests/lmf_test.py
+-rw-r--r--   0        0        0     2140 2023-05-07 18:54:48.999710 wn-0.9.4/tests/morphy_test.py
+-rw-r--r--   0        0        0     9281 2023-05-07 18:54:48.999710 wn-0.9.4/tests/primary_query_test.py
+-rw-r--r--   0        0        0     4188 2023-05-07 18:54:48.999710 wn-0.9.4/tests/relations_test.py
+-rw-r--r--   0        0        0     4600 2023-05-07 18:54:48.999710 wn-0.9.4/tests/secondary_query_test.py
+-rw-r--r--   0        0        0     6901 2023-05-07 18:54:48.999710 wn-0.9.4/tests/similarity_test.py
+-rw-r--r--   0        0        0     4142 2023-05-07 18:54:48.999710 wn-0.9.4/tests/taxonomy_test.py
+-rw-r--r--   0        0        0      361 2023-05-07 18:54:48.999710 wn-0.9.4/tests/util_test.py
+-rw-r--r--   0        0        0     2754 2023-05-07 18:54:48.999710 wn-0.9.4/tests/wordnet_test.py
+-rw-r--r--   0        0        0      974 2023-05-07 18:54:48.999710 wn-0.9.4/wn/__init__.py
+-rw-r--r--   0        0        0     5022 2023-05-07 18:54:48.999710 wn-0.9.4/wn/__main__.py
+-rw-r--r--   0        0        0    32182 2023-05-07 18:54:48.999710 wn-0.9.4/wn/_add.py
+-rw-r--r--   0        0        0     9060 2023-05-07 18:54:48.999710 wn-0.9.4/wn/_config.py
+-rw-r--r--   0        0        0    49402 2023-05-07 18:54:48.999710 wn-0.9.4/wn/_core.py
+-rw-r--r--   0        0        0     3860 2023-05-07 18:54:48.999710 wn-0.9.4/wn/_db.py
+-rw-r--r--   0        0        0     4759 2023-05-07 18:54:48.999710 wn-0.9.4/wn/_download.py
+-rw-r--r--   0        0        0      674 2023-05-07 18:54:48.999710 wn-0.9.4/wn/_exceptions.py
+-rw-r--r--   0        0        0    10885 2023-05-07 18:54:48.999710 wn-0.9.4/wn/_export.py
+-rw-r--r--   0        0        0     1072 2023-05-07 18:54:48.999710 wn-0.9.4/wn/_ili.py
+-rw-r--r--   0        0        0    23194 2023-05-07 18:54:48.999710 wn-0.9.4/wn/_queries.py
+-rw-r--r--   0        0        0      919 2023-05-07 18:54:48.999710 wn-0.9.4/wn/_types.py
+-rw-r--r--   0        0        0     1843 2023-05-07 18:54:48.999710 wn-0.9.4/wn/_util.py
+-rw-r--r--   0        0        0     7710 2023-05-07 18:54:48.999710 wn-0.9.4/wn/constants.py
+-rw-r--r--   0        0        0     6698 2023-05-07 18:54:48.999710 wn-0.9.4/wn/ic.py
+-rw-r--r--   0        0        0    15066 2023-05-07 18:54:49.003710 wn-0.9.4/wn/index.toml
+-rw-r--r--   0        0        0    29674 2023-05-07 18:54:49.003710 wn-0.9.4/wn/lmf.py
+-rw-r--r--   0        0        0      268 2023-05-07 18:54:49.003710 wn-0.9.4/wn/metrics.py
+-rw-r--r--   0        0        0     4924 2023-05-07 18:54:49.003710 wn-0.9.4/wn/morphy.py
+-rw-r--r--   0        0        0     6901 2023-05-07 18:54:49.003710 wn-0.9.4/wn/project.py
+-rw-r--r--   0        0        0     9170 2023-05-07 18:54:49.003710 wn-0.9.4/wn/schema.sql
+-rw-r--r--   0        0        0     8113 2023-05-07 18:54:49.003710 wn-0.9.4/wn/similarity.py
+-rw-r--r--   0        0        0    11236 2023-05-07 18:54:49.003710 wn-0.9.4/wn/taxonomy.py
+-rw-r--r--   0        0        0     6358 2023-05-07 18:54:49.003710 wn-0.9.4/wn/util.py
+-rw-r--r--   0        0        0    10790 2023-05-07 18:54:49.003710 wn-0.9.4/wn/validate.py
+-rw-r--r--   0        0        0     9599 2023-05-07 18:54:49.003710 wn-0.9.4/wn/web.py
+-rw-r--r--   0        0        0    13660 1970-01-01 00:00:00.000000 wn-0.9.4/PKG-INFO
```

### Comparing `wn-0.9.3/.github/ISSUE_TEMPLATE/bug_report.md` & `wn-0.9.4/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/.github/ISSUE_TEMPLATE/data-issue.md` & `wn-0.9.4/.github/ISSUE_TEMPLATE/data-issue.md`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/.github/ISSUE_TEMPLATE/feature_request.md` & `wn-0.9.4/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/.github/workflows/checks.yml` & `wn-0.9.4/.github/workflows/checks.yml`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/.github/workflows/release.yml` & `wn-0.9.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/.gitignore` & `wn-0.9.4/.gitignore`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/CHANGELOG.md` & `wn-0.9.4/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,27 @@
 # Change Log
 
-## [Unreleased]
+## [v0.9.4]
+
+**Release date: 2023-05-07**
+
+### Index
+
+* Added `oewn:2022` ([#181])
 
 
 ## [v0.9.3]
 
 **Release date: 2022-11-13**
 
+### Python Support
+
+* Removed support for Python 3.6
+* Added support for Python 3.11
+
 ### Fixed
 
 * `wn.Synset.relations()` no longer raises a `KeyError` when no
   relation types are given and relations are found via ILI ([#177])
 
 
 ## [v0.9.2]
@@ -515,14 +526,16 @@
 **Release date: 2020-11-25**
 
 This is the initial release of the new Wn library. On PyPI it replaces
 the https://github.com/nltk/wordnet/ code which had been effectively
 abandoned, but this is an entirely new codebase.
 
 
+[v0.9.4]: ../../releases/tag/v0.9.4
+[v0.9.3]: ../../releases/tag/v0.9.3
 [v0.9.2]: ../../releases/tag/v0.9.2
 [v0.9.1]: ../../releases/tag/v0.9.1
 [v0.9.0]: ../../releases/tag/v0.9.0
 [v0.8.3]: ../../releases/tag/v0.8.3
 [v0.8.2]: ../../releases/tag/v0.8.2
 [v0.8.1]: ../../releases/tag/v0.8.1
 [v0.8.0]: ../../releases/tag/v0.8.0
@@ -605,7 +618,8 @@
 [#154]: https://github.com/goodmami/wn/issues/154
 [#155]: https://github.com/goodmami/wn/issues/155
 [#156]: https://github.com/goodmami/wn/issues/156
 [#157]: https://github.com/goodmami/wn/issues/157
 [#168]: https://github.com/goodmami/wn/issues/168
 [#169]: https://github.com/goodmami/wn/issues/169
 [#177]: https://github.com/goodmami/wn/issues/177
+[#181]: https://github.com/goodmami/wn/issues/181
```

### Comparing `wn-0.9.3/CITATION.cff` & `wn-0.9.4/CITATION.cff`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/CONTRIBUTING.md` & `wn-0.9.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/LICENSE` & `wn-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/README.md` & `wn-0.9.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -20,24 +20,24 @@
 ---
 
 Wn is a Python library for exploring information in wordnets. Install
 it from PyPI and download some data:
 
 ```console
 $ pip install wn
-$ python -m wn download oewn:2021  # the Open English WordNet 2021
+$ python -m wn download oewn:2022  # the Open English WordNet 2022
 ```
 
 Then start exploring:
 
 ```python
 >>> import wn
->>> en = wn.Wordnet('oewn:2021')  # Create Wordnet object to query
->>> ss = en.synsets('win')[0]     # Get the first synset for 'win'
->>> ss.definition()               # Get the synset's definition
+>>> en = wn.Wordnet('oewn:2022')        # Create Wordnet object to query
+>>> ss = en.synsets('win', pos='v')[0]  # Get the first synset for 'win'
+>>> ss.definition()                     # Get the synset's definition
 'be the winner in a contest or competition; be victorious'
 ```
 
 
 ## Features
 
 - Multilingual by design; first-class support for wordnets in any language
@@ -69,15 +69,15 @@
 stricter compatibility needs for, e.g., experiment replicability, you
 may try the [OMW English Wordnet based on WordNet 3.0] (compatible with
 the Princeton WordNet 3.0 and with the [NLTK]), or [OpenWordnet-EN] (for
 use with the Portuguese wordnet [OpenWordnet-PT]).
 
 | Name                                       | Specifier              | # Synsets | Notes |
 | ------------------------------------------ | ---------------------- | --------: | ----- |
-| [Open English WordNet] | `oewn:2021`<br/> `ewn:2020`<br/> `ewn:2019` | 120039<br/>120053<br/>117791 | Recommended<br/>&nbsp;<br/>&nbsp; |
+| [Open English WordNet] | `oewn:2022`<br/> `oewn:2021`<br/> `ewn:2020`<br/> `ewn:2019` | 120068<br/>120039<br/>120053<br/>117791 | Recommended<br/>&nbsp;<br/>&nbsp;<br/>&nbsp; |
 | [OMW English Wordnet based on WordNet 3.0] | `omw-en:1.4` | 117659 | Included with `omw:1.4` |
 | [OMW English Wordnet based on WordNet 3.1] | `omw-en31:1.4` | 117791 |  |
 | [OpenWordnet-EN] | `own-en:1.0.0` | 117659 | Included with `own:1.0.0` |
 
 [Open English WordNet]: https://en-word.net
 [Open Multilingual Wordnet]: https://github.com/omwn
 [OMW English Wordnet based on WordNet 3.0]: https://github.com/omwn/omw-data
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
                                   [Wn logo]
                         a Python library for wordnets
          [PyPI_link] [Python Support] [tests] [Documentation_Status]
    Available_Wordnets | Documentation | FAQ | Migrating_from_NLTK | Roadmap
 --- Wn is a Python library for exploring information in wordnets. Install it
 from PyPI and download some data: ```console $ pip install wn $ python -m wn
-download oewn:2021 # the Open English WordNet 2021 ``` Then start exploring:
-```python >>> import wn >>> en = wn.Wordnet('oewn:2021') # Create Wordnet
-object to query >>> ss = en.synsets('win')[0] # Get the first synset for 'win'
->>> ss.definition() # Get the synset's definition 'be the winner in a contest
-or competition; be victorious' ``` ## Features - Multilingual by design; first-
-class support for wordnets in any language - Interlingual queries via the
-[Collaborative Interlingual Index](https://github.com/globalwordnet/cili/) -
-Six [similarity metrics](https://wn.readthedocs.io/en/latest/api/
+download oewn:2022 # the Open English WordNet 2022 ``` Then start exploring:
+```python >>> import wn >>> en = wn.Wordnet('oewn:2022') # Create Wordnet
+object to query >>> ss = en.synsets('win', pos='v')[0] # Get the first synset
+for 'win' >>> ss.definition() # Get the synset's definition 'be the winner in a
+contest or competition; be victorious' ``` ## Features - Multilingual by
+design; first-class support for wordnets in any language - Interlingual queries
+via the [Collaborative Interlingual Index](https://github.com/globalwordnet/
+cili/) - Six [similarity metrics](https://wn.readthedocs.io/en/latest/api/
 wn.similarity.html) - Functions for [exploring taxonomies](https://
 wn.readthedocs.io/en/latest/api/wn.taxonomy.html) - Support for [lemmatization]
 ([Morphy] for English is built-in) and unicode [normalization] - Full support
 of the [WN-LMF 1.1](https://globalwordnet.github.io/schemas/) format, including
 word pronunciations and lexicon extensions - SQL-based backend offers very fast
 startup and improved performance on many kinds of queries [lemmatization]:
 https://wn.readthedocs.io/en/latest/guides/lemmatization.html#lemmatization
@@ -30,20 +30,23 @@
 available. In general it is recommended to use the latest [Open English
 Wordnet], but if you have stricter compatibility needs for, e.g., experiment
 replicability, you may try the [OMW English Wordnet based on WordNet 3.0]
 (compatible with the Princeton WordNet 3.0 and with the [NLTK]), or
 [OpenWordnet-EN] (for use with the Portuguese wordnet [OpenWordnet-PT]). | Name
 | Specifier | # Synsets | Notes | | -----------------------------------------
 - | ---------------------- | --------: | ----- | | [Open English WordNet] |
+`oewn:2022`
 `oewn:2021`
 `ewn:2020`
-`ewn:2019` | 120039
+`ewn:2019` | 120068
+120039
 120053
 117791 | Recommended
  
+ 
   | | [OMW English Wordnet based on WordNet 3.0] | `omw-en:1.4` | 117659 |
 Included with `omw:1.4` | | [OMW English Wordnet based on WordNet 3.1] | `omw-
 en31:1.4` | 117791 | | | [OpenWordnet-EN] | `own-en:1.0.0` | 117659 | Included
 with `own:1.0.0` | [Open English WordNet]: https://en-word.net [Open
 Multilingual Wordnet]: https://github.com/omwn [OMW English Wordnet based on
 WordNet 3.0]: https://github.com/omwn/omw-data [OMW English Wordnet based on
 WordNet 3.1]: https://github.com/omwn/omw-data [OpenWordnet-EN]: https://
```

### Comparing `wn-0.9.3/docs/Makefile` & `wn-0.9.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/docs/_static/demo.ipynb` & `wn-0.9.4/docs/_static/demo.ipynb`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/docs/_static/wn-logo-rotate.svg` & `wn-0.9.4/docs/_static/wn-logo-rotate.svg`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/docs/_static/wn-logo.svg` & `wn-0.9.4/docs/_static/wn-logo.svg`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/docs/api/wn.constants.rst` & `wn-0.9.4/docs/api/wn.constants.rst`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/docs/api/wn.ic.rst` & `wn-0.9.4/docs/api/wn.ic.rst`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/docs/api/wn.morphy.rst` & `wn-0.9.4/docs/api/wn.morphy.rst`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/docs/api/wn.rst` & `wn-0.9.4/docs/api/wn.rst`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/docs/api/wn.similarity.rst` & `wn-0.9.4/docs/api/wn.similarity.rst`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/docs/api/wn.taxonomy.rst` & `wn-0.9.4/docs/api/wn.taxonomy.rst`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/docs/api/wn.util.rst` & `wn-0.9.4/docs/api/wn.util.rst`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/docs/api/wn.web.rst` & `wn-0.9.4/docs/api/wn.web.rst`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/docs/cli.rst` & `wn-0.9.4/docs/cli.rst`

 * *Files 3% similar despite different names*

```diff
@@ -82,14 +82,15 @@
 The ``projects`` subcommand lists all known projects in Wn's
 index. This is helpful to see what is available for downloading.
 
 .. code-block::
 
    $ python -m wn projects
    ic	cili	1.0	[---]	Collaborative Interlingual Index
+   ic	oewn	2022	[en]	Open English WordNet
    ic	oewn	2021	[en]	Open English WordNet
    ic	ewn	2020	[en]	Open English WordNet
    ic	ewn	2019	[en]	Open English WordNet
    i-	odenet	1.4	[de]	Open German WordNet
    ic	odenet	1.3	[de]	Open German WordNet
    ic	omw	1.4	[mul]	Open Multilingual Wordnet
    ic	omw-en	1.4	[en]	OMW English Wordnet based on WordNet 3.0
```

### Comparing `wn-0.9.3/docs/conf.py` & `wn-0.9.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/docs/faq.rst` & `wn-0.9.4/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/docs/guides/basic.rst` & `wn-0.9.4/docs/guides/basic.rst`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/docs/guides/images/sense-sense.svg` & `wn-0.9.4/docs/guides/images/sense-sense.svg`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/docs/guides/images/sense-synset.svg` & `wn-0.9.4/docs/guides/images/sense-synset.svg`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/docs/guides/images/synset-synset.svg` & `wn-0.9.4/docs/guides/images/synset-synset.svg`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/docs/guides/images/word-sense-synset.svg` & `wn-0.9.4/docs/guides/images/word-sense-synset.svg`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/docs/guides/interlingual.rst` & `wn-0.9.4/docs/guides/interlingual.rst`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/docs/guides/lemmatization.rst` & `wn-0.9.4/docs/guides/lemmatization.rst`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/docs/guides/lexicons.rst` & `wn-0.9.4/docs/guides/lexicons.rst`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/docs/guides/nltk-migration.rst` & `wn-0.9.4/docs/guides/nltk-migration.rst`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/docs/guides/wordnet.rst` & `wn-0.9.4/docs/guides/wordnet.rst`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/docs/index.rst` & `wn-0.9.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/docs/make.bat` & `wn-0.9.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/docs/setup.rst` & `wn-0.9.4/docs/setup.rst`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/pyproject.toml` & `wn-0.9.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,14 @@
   "Topic :: Software Development :: Libraries :: Python Modules",
   "Topic :: Text Processing :: Linguistic",
 ]
 
 dependencies = [
   "requests",
   "tomli",
-  "importlib_resources; python_version < '3.7'",
   "typing-extensions; python_version < '3.8'",
 ]
 
 [project.optional-dependencies]
 web = [
     "starlette",
 ]
```

### Comparing `wn-0.9.3/tests/conftest.py` & `wn-0.9.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/tests/data/mini-lmf-1.0.xml` & `wn-0.9.4/tests/data/mini-lmf-1.0.xml`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/tests/data/mini-lmf-1.1.xml` & `wn-0.9.4/tests/data/mini-lmf-1.1.xml`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/tests/db_test.py` & `wn-0.9.4/tests/db_test.py`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/tests/export_test.py` & `wn-0.9.4/tests/export_test.py`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/tests/ic_test.py` & `wn-0.9.4/tests/ic_test.py`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/tests/lmf_test.py` & `wn-0.9.4/tests/lmf_test.py`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/tests/morphy_test.py` & `wn-0.9.4/tests/morphy_test.py`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/tests/primary_query_test.py` & `wn-0.9.4/tests/primary_query_test.py`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/tests/relations_test.py` & `wn-0.9.4/tests/relations_test.py`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/tests/secondary_query_test.py` & `wn-0.9.4/tests/secondary_query_test.py`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/tests/similarity_test.py` & `wn-0.9.4/tests/similarity_test.py`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/tests/taxonomy_test.py` & `wn-0.9.4/tests/taxonomy_test.py`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/tests/wordnet_test.py` & `wn-0.9.4/tests/wordnet_test.py`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/wn/__init__.py` & `wn-0.9.4/wn/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,8 +53,8 @@
     word, words, Word, Form, Pronunciation, Tag,
     sense, senses, Sense, Count,
     synset, synsets, Synset,
     ili, ilis, ILI,
     Wordnet
 )
 
-__version__ = '0.9.3'
+__version__ = '0.9.4'
```

### Comparing `wn-0.9.3/wn/__main__.py` & `wn-0.9.4/wn/__main__.py`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/wn/_add.py` & `wn-0.9.4/wn/_add.py`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/wn/_config.py` & `wn-0.9.4/wn/_config.py`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/wn/_core.py` & `wn-0.9.4/wn/_core.py`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/wn/_db.py` & `wn-0.9.4/wn/_db.py`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/wn/_download.py` & `wn-0.9.4/wn/_download.py`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/wn/_exceptions.py` & `wn-0.9.4/wn/_exceptions.py`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/wn/_export.py` & `wn-0.9.4/wn/_export.py`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/wn/_ili.py` & `wn-0.9.4/wn/_ili.py`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/wn/_queries.py` & `wn-0.9.4/wn/_queries.py`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/wn/_types.py` & `wn-0.9.4/wn/_types.py`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/wn/_util.py` & `wn-0.9.4/wn/_util.py`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/wn/constants.py` & `wn-0.9.4/wn/constants.py`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/wn/ic.py` & `wn-0.9.4/wn/ic.py`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/wn/index.toml` & `wn-0.9.4/wn/index.toml`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,19 @@
     url = "https://github.com/globalwordnet/cili/releases/download/v1.0/cili.tsv.xz"
 
 
 [oewn]
   label = "Open English WordNet"
   language = "en"
   license = "https://creativecommons.org/licenses/by/4.0/"
+  [oewn.versions.2022]
+    url = """
+      https://en-word.net/static/english-wordnet-2022.xml.gz
+      https://github.com/globalwordnet/english-wordnet/releases/download/2022-edition/english-wordnet-2022.xml.gz
+    """
   [oewn.versions.2021]
     url = "https://en-word.net/static/english-wordnet-2021.xml.gz"
   [oewn.versions.2020]
     error = "Use 'ewn' as the ID prior to version 2021 ('ewn:2020')"
   [oewn.versions.2019]
     error = "Use 'ewn' as the ID prior to version 2021 ('ewn:2019')"
```

### Comparing `wn-0.9.3/wn/lmf.py` & `wn-0.9.4/wn/lmf.py`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/wn/morphy.py` & `wn-0.9.4/wn/morphy.py`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/wn/project.py` & `wn-0.9.4/wn/project.py`

 * *Files 3% similar despite different names*

```diff
@@ -177,20 +177,21 @@
     xzipped = is_lzma(source)
     if not (gzipped or xzipped):
         yield source
     else:
         tmp = tempfile.NamedTemporaryFile(suffix='.xml', delete=False)
         path = Path(tmp.name)
         try:
+            # for typing issues, see https://github.com/python/mypy/issues/15031
             if gzipped:
                 with gzip.open(source, 'rb') as gzip_src:
-                    shutil.copyfileobj(gzip_src, tmp)
+                    shutil.copyfileobj(gzip_src, tmp)  # type: ignore
             else:  # xzipped
                 with lzma.open(source, 'rb') as lzma_src:
-                    shutil.copyfileobj(lzma_src, tmp)
+                    shutil.copyfileobj(lzma_src, tmp)  # type: ignore
 
             tmp.close()  # Windows cannot reliably reopen until it's closed
 
             yield path
 
         except (OSError, EOFError, lzma.LZMAError) as exc:
             raise wn.Error(f'could not decompress file: {source}') from exc
```

### Comparing `wn-0.9.3/wn/schema.sql` & `wn-0.9.4/wn/schema.sql`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/wn/similarity.py` & `wn-0.9.4/wn/similarity.py`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/wn/taxonomy.py` & `wn-0.9.4/wn/taxonomy.py`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/wn/util.py` & `wn-0.9.4/wn/util.py`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/wn/validate.py` & `wn-0.9.4/wn/validate.py`

 * *Files identical despite different names*

### Comparing `wn-0.9.3/wn/web.py` & `wn-0.9.4/wn/web.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 ) -> str:
     if lexicon is None:
         lexicon = obj.lexicon().specifier()
     kwargs = {
         'lexicon': lexicon,
         name: obj.id
     }
-    return request.url_for(name, **kwargs)
+    return str(request.url_for(name, **kwargs))
 
 
 def make_lexicon(lex: wn.Lexicon, request: Request) -> dict:
     spec = lex.specifier()
     return {
         'id': spec,
         'type': 'lexicon',
```

### Comparing `wn-0.9.3/PKG-INFO` & `wn-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wn
-Version: 0.9.3
+Version: 0.9.4
 Summary: Wordnet interface library
 Keywords: wordnet,interlingual,linguistics,language,library
 Author-email: Michael Wayne Goodman <goodman.m.w@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -19,15 +19,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Linguistic
 Requires-Dist: requests
 Requires-Dist: tomli
-Requires-Dist: importlib_resources; python_version < '3.7'
 Requires-Dist: typing-extensions; python_version < '3.8'
 Requires-Dist: sphinx ; extra == "doc"
 Requires-Dist: furo ; extra == "doc"
 Requires-Dist: sphinx-copybutton ; extra == "doc"
 Requires-Dist: wn-editor ; extra == "editor"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: mypy ; extra == "test"
@@ -65,24 +64,24 @@
 ---
 
 Wn is a Python library for exploring information in wordnets. Install
 it from PyPI and download some data:
 
 ```console
 $ pip install wn
-$ python -m wn download oewn:2021  # the Open English WordNet 2021
+$ python -m wn download oewn:2022  # the Open English WordNet 2022
 ```
 
 Then start exploring:
 
 ```python
 >>> import wn
->>> en = wn.Wordnet('oewn:2021')  # Create Wordnet object to query
->>> ss = en.synsets('win')[0]     # Get the first synset for 'win'
->>> ss.definition()               # Get the synset's definition
+>>> en = wn.Wordnet('oewn:2022')        # Create Wordnet object to query
+>>> ss = en.synsets('win', pos='v')[0]  # Get the first synset for 'win'
+>>> ss.definition()                     # Get the synset's definition
 'be the winner in a contest or competition; be victorious'
 ```
 
 
 ## Features
 
 - Multilingual by design; first-class support for wordnets in any language
@@ -114,15 +113,15 @@
 stricter compatibility needs for, e.g., experiment replicability, you
 may try the [OMW English Wordnet based on WordNet 3.0] (compatible with
 the Princeton WordNet 3.0 and with the [NLTK]), or [OpenWordnet-EN] (for
 use with the Portuguese wordnet [OpenWordnet-PT]).
 
 | Name                                       | Specifier              | # Synsets | Notes |
 | ------------------------------------------ | ---------------------- | --------: | ----- |
-| [Open English WordNet] | `oewn:2021`<br/> `ewn:2020`<br/> `ewn:2019` | 120039<br/>120053<br/>117791 | Recommended<br/>&nbsp;<br/>&nbsp; |
+| [Open English WordNet] | `oewn:2022`<br/> `oewn:2021`<br/> `ewn:2020`<br/> `ewn:2019` | 120068<br/>120039<br/>120053<br/>117791 | Recommended<br/>&nbsp;<br/>&nbsp;<br/>&nbsp; |
 | [OMW English Wordnet based on WordNet 3.0] | `omw-en:1.4` | 117659 | Included with `omw:1.4` |
 | [OMW English Wordnet based on WordNet 3.1] | `omw-en31:1.4` | 117791 |  |
 | [OpenWordnet-EN] | `own-en:1.0.0` | 117659 | Included with `own:1.0.0` |
 
 [Open English WordNet]: https://en-word.net
 [Open Multilingual Wordnet]: https://github.com/omwn
 [OMW English Wordnet based on WordNet 3.0]: https://github.com/omwn/omw-data
```

#### html2text {}

```diff
@@ -1,47 +1,46 @@
-Metadata-Version: 2.1 Name: wn Version: 0.9.3 Summary: Wordnet interface
+Metadata-Version: 2.1 Name: wn Version: 0.9.4 Summary: Wordnet interface
 library Keywords: wordnet,interlingual,linguistics,language,library Author-
 email: Michael Wayne Goodman
 m.w@gmail.com> Requires-Python: >=3.7 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Information Technology Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
 Scientific/Engineering :: Information Analysis Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Topic :: Text Processing
 :: Linguistic Requires-Dist: requests Requires-Dist: tomli Requires-Dist:
-importlib_resources; python_version < '3.7' Requires-Dist: typing-extensions;
-python_version < '3.8' Requires-Dist: sphinx ; extra == "doc" Requires-Dist:
-furo ; extra == "doc" Requires-Dist: sphinx-copybutton ; extra == "doc"
-Requires-Dist: wn-editor ; extra == "editor" Requires-Dist: pytest ; extra ==
-"test" Requires-Dist: mypy ; extra == "test" Requires-Dist: flake8 ; extra ==
-"test" Requires-Dist: nox ; extra == "test" Requires-Dist: types-requests ;
-extra == "test" Requires-Dist: starlette ; extra == "web" Project-URL:
-changelog, https://github.com/goodmami/wn/blob/main/CHANGELOG.md Project-URL:
-documentation, https://wn.readthedocs.io Project-URL: homepage, https://
-github.com/goodmami/wn Provides-Extra: doc Provides-Extra: editor Provides-
-Extra: test Provides-Extra: web
+typing-extensions; python_version < '3.8' Requires-Dist: sphinx ; extra ==
+"doc" Requires-Dist: furo ; extra == "doc" Requires-Dist: sphinx-copybutton ;
+extra == "doc" Requires-Dist: wn-editor ; extra == "editor" Requires-Dist:
+pytest ; extra == "test" Requires-Dist: mypy ; extra == "test" Requires-Dist:
+flake8 ; extra == "test" Requires-Dist: nox ; extra == "test" Requires-Dist:
+types-requests ; extra == "test" Requires-Dist: starlette ; extra == "web"
+Project-URL: changelog, https://github.com/goodmami/wn/blob/main/CHANGELOG.md
+Project-URL: documentation, https://wn.readthedocs.io Project-URL: homepage,
+https://github.com/goodmami/wn Provides-Extra: doc Provides-Extra: editor
+Provides-Extra: test Provides-Extra: web
                                   [Wn logo]
                         a Python library for wordnets
          [PyPI_link] [Python Support] [tests] [Documentation_Status]
    Available_Wordnets | Documentation | FAQ | Migrating_from_NLTK | Roadmap
 --- Wn is a Python library for exploring information in wordnets. Install it
 from PyPI and download some data: ```console $ pip install wn $ python -m wn
-download oewn:2021 # the Open English WordNet 2021 ``` Then start exploring:
-```python >>> import wn >>> en = wn.Wordnet('oewn:2021') # Create Wordnet
-object to query >>> ss = en.synsets('win')[0] # Get the first synset for 'win'
->>> ss.definition() # Get the synset's definition 'be the winner in a contest
-or competition; be victorious' ``` ## Features - Multilingual by design; first-
-class support for wordnets in any language - Interlingual queries via the
-[Collaborative Interlingual Index](https://github.com/globalwordnet/cili/) -
-Six [similarity metrics](https://wn.readthedocs.io/en/latest/api/
+download oewn:2022 # the Open English WordNet 2022 ``` Then start exploring:
+```python >>> import wn >>> en = wn.Wordnet('oewn:2022') # Create Wordnet
+object to query >>> ss = en.synsets('win', pos='v')[0] # Get the first synset
+for 'win' >>> ss.definition() # Get the synset's definition 'be the winner in a
+contest or competition; be victorious' ``` ## Features - Multilingual by
+design; first-class support for wordnets in any language - Interlingual queries
+via the [Collaborative Interlingual Index](https://github.com/globalwordnet/
+cili/) - Six [similarity metrics](https://wn.readthedocs.io/en/latest/api/
 wn.similarity.html) - Functions for [exploring taxonomies](https://
 wn.readthedocs.io/en/latest/api/wn.taxonomy.html) - Support for [lemmatization]
 ([Morphy] for English is built-in) and unicode [normalization] - Full support
 of the [WN-LMF 1.1](https://globalwordnet.github.io/schemas/) format, including
 word pronunciations and lexicon extensions - SQL-based backend offers very fast
 startup and improved performance on many kinds of queries [lemmatization]:
 https://wn.readthedocs.io/en/latest/guides/lemmatization.html#lemmatization
@@ -56,20 +55,23 @@
 available. In general it is recommended to use the latest [Open English
 Wordnet], but if you have stricter compatibility needs for, e.g., experiment
 replicability, you may try the [OMW English Wordnet based on WordNet 3.0]
 (compatible with the Princeton WordNet 3.0 and with the [NLTK]), or
 [OpenWordnet-EN] (for use with the Portuguese wordnet [OpenWordnet-PT]). | Name
 | Specifier | # Synsets | Notes | | -----------------------------------------
 - | ---------------------- | --------: | ----- | | [Open English WordNet] |
+`oewn:2022`
 `oewn:2021`
 `ewn:2020`
-`ewn:2019` | 120039
+`ewn:2019` | 120068
+120039
 120053
 117791 | Recommended
  
+ 
   | | [OMW English Wordnet based on WordNet 3.0] | `omw-en:1.4` | 117659 |
 Included with `omw:1.4` | | [OMW English Wordnet based on WordNet 3.1] | `omw-
 en31:1.4` | 117791 | | | [OpenWordnet-EN] | `own-en:1.0.0` | 117659 | Included
 with `own:1.0.0` | [Open English WordNet]: https://en-word.net [Open
 Multilingual Wordnet]: https://github.com/omwn [OMW English Wordnet based on
 WordNet 3.0]: https://github.com/omwn/omw-data [OMW English Wordnet based on
 WordNet 3.1]: https://github.com/omwn/omw-data [OpenWordnet-EN]: https://
```

