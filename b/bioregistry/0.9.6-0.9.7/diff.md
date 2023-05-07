# Comparing `tmp/bioregistry-0.9.6.tar.gz` & `tmp/bioregistry-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioregistry-0.9.6.tar", last modified: Sat May  6 01:22:35 2023, max compression
+gzip compressed data, was "bioregistry-0.9.7.tar", last modified: Sun May  7 01:27:33 2023, max compression
```

## Comparing `bioregistry-0.9.6.tar` & `bioregistry-0.9.7.tar`

### file list

```diff
@@ -1,341 +1,341 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:22:35.303106 bioregistry-0.9.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-06 00:43:45.000000 bioregistry-0.9.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-06 00:43:45.000000 bioregistry-0.9.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    31510 2023-05-06 01:22:35.303106 bioregistry-0.9.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    30194 2023-05-06 00:43:45.000000 bioregistry-0.9.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:22:35.179105 bioregistry-0.9.6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-05-06 00:43:45.000000 bioregistry-0.9.6/docs/bulk_prefix_request_template.tsv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:22:35.187105 bioregistry-0.9.6/docs/img/
--rw-r--r--   0 runner    (1001) docker     (123)    48331 2023-05-06 01:07:48.000000 bioregistry-0.9.6/docs/img/bibliography_years.svg
--rw-r--r--   0 runner    (1001) docker     (123)   157010 2023-05-06 01:08:09.000000 bioregistry-0.9.6/docs/img/bioregistry_coverage.svg
--rw-r--r--   0 runner    (1001) docker     (123)   107004 2023-05-06 01:08:08.000000 bioregistry-0.9.6/docs/img/bioregistry_coverage_bar.svg
--rw-r--r--   0 runner    (1001) docker     (123)    84710 2023-05-06 01:08:10.000000 bioregistry-0.9.6/docs/img/bioregistry_coverage_bar_short.svg
--rw-r--r--   0 runner    (1001) docker     (123)    77372 2023-05-06 00:43:45.000000 bioregistry-0.9.6/docs/img/datamodel_umls.svg
--rw-r--r--   0 runner    (1001) docker     (123)  1382043 2023-05-06 01:12:31.000000 bioregistry-0.9.6/docs/img/external_overlap.svg
--rw-r--r--   0 runner    (1001) docker     (123)    72498 2023-05-06 01:08:38.000000 bioregistry-0.9.6/docs/img/has_attribute.svg
--rw-r--r--   0 runner    (1001) docker     (123)    28419 2023-05-06 01:12:33.000000 bioregistry-0.9.6/docs/img/providers.svg
--rw-r--r--   0 runner    (1001) docker     (123)    22283 2023-05-06 01:12:34.000000 bioregistry-0.9.6/docs/img/regex_report.svg
--rw-r--r--   0 runner    (1001) docker     (123)    51528 2023-05-06 01:08:07.000000 bioregistry-0.9.6/docs/img/xrefs.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:22:35.187105 bioregistry-0.9.6/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-06 00:43:45.000000 bioregistry-0.9.6/docs/source/alignment.rst
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-06 00:43:45.000000 bioregistry-0.9.6/docs/source/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7033 2023-05-06 01:22:23.000000 bioregistry-0.9.6/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-05-06 00:43:45.000000 bioregistry-0.9.6/docs/source/deployment.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-05-06 00:43:45.000000 bioregistry-0.9.6/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)   214468 2023-05-06 00:43:45.000000 bioregistry-0.9.6/docs/source/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-06 00:43:45.000000 bioregistry-0.9.6/docs/source/pandas.rst
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-06 00:43:45.000000 bioregistry-0.9.6/docs/source/reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-06 00:43:45.000000 bioregistry-0.9.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-05-06 01:22:35.307107 bioregistry-0.9.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:22:35.167105 bioregistry-0.9.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:22:35.195105 bioregistry-0.9.6/src/bioregistry/
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:22:35.199105 bioregistry-0.9.6/src/bioregistry/align/
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/align/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/align/aberowl.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/align/bartoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/align/biocontext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/align/biolink.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/align/bioportal.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/align/cellosaurus.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/align/cheminf.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/align/cropoct.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/align/edam.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/align/fairsharing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/align/go.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/align/hl7.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/align/miriam.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/align/n2t.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/align/ncbi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/align/obofoundry.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/align/ols.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/align/ontobee.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/align/prefixcommons.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/align/re3data.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/align/uniprot.py
--rw-r--r--   0 runner    (1001) docker     (123)    10718 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/align/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/align/wikidata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:22:35.199105 bioregistry-0.9.6/src/bioregistry/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5007 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/analysis/title_tfidf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:22:35.203105 bioregistry-0.9.6/src/bioregistry/app/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17624 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/app/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/app/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/app/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    10179 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/app/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/app/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:22:35.203105 bioregistry-0.9.6/src/bioregistry/app/static/
--rw-r--r--   0 runner    (1001) docker     (123)   801449 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/app/static/logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:22:35.207105 bioregistry-0.9.6/src/bioregistry/app/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/app/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/app/templates/collection.html
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/app/templates/collections.html
--rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/app/templates/context.html
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/app/templates/contexts.html
--rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/app/templates/contributor.html
--rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/app/templates/contributors.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:22:35.207105 bioregistry-0.9.6/src/bioregistry/app/templates/highlights/
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/app/templates/highlights/keywords.html
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/app/templates/highlights/owners.html
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/app/templates/highlights/relations.html
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/app/templates/highlights/twitter.html
--rw-r--r--   0 runner    (1001) docker     (123)    15622 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/app/templates/home.html
--rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/app/templates/macros.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:22:35.207105 bioregistry-0.9.6/src/bioregistry/app/templates/meta/
--rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/app/templates/meta/access.html
--rw-r--r--   0 runner    (1001) docker     (123)    19835 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/app/templates/meta/acknowledgements.html
--rw-r--r--   0 runner    (1001) docker     (123)    10695 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/app/templates/meta/download.html
--rw-r--r--   0 runner    (1001) docker     (123)    16544 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/app/templates/meta/related.html
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/app/templates/meta/schema.html
--rw-r--r--   0 runner    (1001) docker     (123)    19312 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/app/templates/meta/summary.html
--rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/app/templates/meta/sustainability.html
--rw-r--r--   0 runner    (1001) docker     (123)     8460 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/app/templates/metaresource.html
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/app/templates/metaresources.html
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/app/templates/prose.html
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/app/templates/reference.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:22:35.211105 bioregistry-0.9.6/src/bioregistry/app/templates/resolve_errors/
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/app/templates/resolve_errors/disallowed_identifier.html
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/app/templates/resolve_errors/invalid_identifier.html
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/app/templates/resolve_errors/missing_prefix.html
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/app/templates/resolve_errors/missing_providers.html
--rw-r--r--   0 runner    (1001) docker     (123)    32484 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/app/templates/resource.html
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/app/templates/resources.html
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/app/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    19423 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/app/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/app/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/app/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:22:35.211105 bioregistry-0.9.6/src/bioregistry/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/benchmarks/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/benchmarks/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/benchmarks/curie_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/benchmarks/curie_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/benchmarks/uri_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/bibliometrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/collection_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    23802 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:22:35.215105 bioregistry-0.9.6/src/bioregistry/curation/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/curation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/curation/add_co_providers.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/curation/add_descriptions_from_gs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/curation/add_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/curation/add_examples_from_javert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/curation/add_examples_from_ols.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/curation/add_ontology_regexes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/curation/bulk_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/curation/clean_licenses.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/curation/clean_name_suffixes.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/curation/clean_publications.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/curation/cleanup_authors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/curation/deprecation_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/curation/enrich_publications.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/curation/import_pc_semiautomatic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/curation/make_description_curation_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/curation/map_bartoc_via_wikidata.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/curation/map_re3data_via_fairsharing.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/curation/rename_metaprefix.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/curation/review_pc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/curation/suggest_author_curation.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/curation/suggest_uniprot_providers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:22:35.227106 bioregistry-0.9.6/src/bioregistry/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/data/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  4590847 2023-05-06 01:05:41.000000 bioregistry-0.9.6/src/bioregistry/data/bioregistry.json
--rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-05-06 01:05:41.000000 bioregistry-0.9.6/src/bioregistry/data/collections.json
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-06 01:05:41.000000 bioregistry-0.9.6/src/bioregistry/data/contexts.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:22:35.175105 bioregistry-0.9.6/src/bioregistry/data/external/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:22:35.231106 bioregistry-0.9.6/src/bioregistry/data/external/aberowl/
--rw-r--r--   0 runner    (1001) docker     (123)   302996 2023-05-06 00:58:40.000000 bioregistry-0.9.6/src/bioregistry/data/external/aberowl/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)   623964 2023-05-06 00:58:40.000000 bioregistry-0.9.6/src/bioregistry/data/external/aberowl/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)  1281529 2023-05-06 00:58:32.000000 bioregistry-0.9.6/src/bioregistry/data/external/aberowl/raw.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:22:35.235106 bioregistry-0.9.6/src/bioregistry/data/external/agroportal/
--rw-r--r--   0 runner    (1001) docker     (123)    42168 2023-05-06 00:53:36.000000 bioregistry-0.9.6/src/bioregistry/data/external/agroportal/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)   124136 2023-05-06 00:53:36.000000 bioregistry-0.9.6/src/bioregistry/data/external/agroportal/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)   663568 2023-05-06 00:53:36.000000 bioregistry-0.9.6/src/bioregistry/data/external/agroportal/raw.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:22:35.235106 bioregistry-0.9.6/src/bioregistry/data/external/bartoc/
--rw-r--r--   0 runner    (1001) docker     (123)  1835101 2023-05-06 01:05:02.000000 bioregistry-0.9.6/src/bioregistry/data/external/bartoc/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)  2216766 2023-05-06 01:05:02.000000 bioregistry-0.9.6/src/bioregistry/data/external/bartoc/processed.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:22:35.239106 bioregistry-0.9.6/src/bioregistry/data/external/biocontext/
--rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-05-06 01:05:37.000000 bioregistry-0.9.6/src/bioregistry/data/external/biocontext/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    74913 2023-05-06 01:05:36.000000 bioregistry-0.9.6/src/bioregistry/data/external/biocontext/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)    55878 2023-05-06 01:05:36.000000 bioregistry-0.9.6/src/bioregistry/data/external/biocontext/raw.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:22:35.243106 bioregistry-0.9.6/src/bioregistry/data/external/biolink/
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-06 00:58:21.000000 bioregistry-0.9.6/src/bioregistry/data/external/biolink/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    10406 2023-05-06 00:58:21.000000 bioregistry-0.9.6/src/bioregistry/data/external/biolink/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)   355095 2023-05-06 00:58:19.000000 bioregistry-0.9.6/src/bioregistry/data/external/biolink/raw.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:22:35.247106 bioregistry-0.9.6/src/bioregistry/data/external/bioportal/
--rw-r--r--   0 runner    (1001) docker     (123)   253653 2023-05-06 00:58:17.000000 bioregistry-0.9.6/src/bioregistry/data/external/bioportal/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)   606735 2023-05-06 00:58:17.000000 bioregistry-0.9.6/src/bioregistry/data/external/bioportal/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)  3539152 2023-05-06 00:58:17.000000 bioregistry-0.9.6/src/bioregistry/data/external/bioportal/raw.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:22:35.251106 bioregistry-0.9.6/src/bioregistry/data/external/cellosaurus/
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-05-06 00:53:40.000000 bioregistry-0.9.6/src/bioregistry/data/external/cellosaurus/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    28730 2023-05-06 00:53:39.000000 bioregistry-0.9.6/src/bioregistry/data/external/cellosaurus/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)    32374 2023-05-06 00:53:39.000000 bioregistry-0.9.6/src/bioregistry/data/external/cellosaurus/raw.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:22:35.251106 bioregistry-0.9.6/src/bioregistry/data/external/cheminf/
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-06 01:05:40.000000 bioregistry-0.9.6/src/bioregistry/data/external/cheminf/processed.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:22:35.251106 bioregistry-0.9.6/src/bioregistry/data/external/cropoct/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-06 01:05:27.000000 bioregistry-0.9.6/src/bioregistry/data/external/cropoct/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    11407 2023-05-06 01:05:27.000000 bioregistry-0.9.6/src/bioregistry/data/external/cropoct/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)    25353 2023-05-06 01:05:27.000000 bioregistry-0.9.6/src/bioregistry/data/external/cropoct/raw.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:22:35.255106 bioregistry-0.9.6/src/bioregistry/data/external/ecoportal/
--rw-r--r--   0 runner    (1001) docker     (123)     9198 2023-05-06 01:05:24.000000 bioregistry-0.9.6/src/bioregistry/data/external/ecoportal/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    18773 2023-05-06 01:05:23.000000 bioregistry-0.9.6/src/bioregistry/data/external/ecoportal/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)    98149 2023-05-06 01:05:23.000000 bioregistry-0.9.6/src/bioregistry/data/external/ecoportal/raw.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:22:35.255106 bioregistry-0.9.6/src/bioregistry/data/external/edam/
--rw-r--r--   0 runner    (1001) docker     (123)    14599 2023-05-06 00:53:46.000000 bioregistry-0.9.6/src/bioregistry/data/external/edam/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    45616 2023-05-06 00:53:45.000000 bioregistry-0.9.6/src/bioregistry/data/external/edam/processed.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:22:35.255106 bioregistry-0.9.6/src/bioregistry/data/external/fairsharing/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-06 00:43:45.000000 bioregistry-0.9.6/src/bioregistry/data/external/fairsharing/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   253879 2023-05-06 01:04:57.000000 bioregistry-0.9.6/src/bioregistry/data/external/fairsharing/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)   745109 2023-05-06 01:04:57.000000 bioregistry-0.9.6/src/bioregistry/data/external/fairsharing/processed.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:22:35.259106 bioregistry-0.9.6/src/bioregistry/data/external/go/
--rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-05-06 01:05:31.000000 bioregistry-0.9.6/src/bioregistry/data/external/go/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)   143024 2023-05-06 01:05:30.000000 bioregistry-0.9.6/src/bioregistry/data/external/go/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)   115035 2023-05-06 01:05:29.000000 bioregistry-0.9.6/src/bioregistry/data/external/go/raw.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:22:35.259106 bioregistry-0.9.6/src/bioregistry/data/external/hl7/
--rw-r--r--   0 runner    (1001) docker     (123)   157660 2023-05-06 00:52:06.000000 bioregistry-0.9.6/src/bioregistry/data/external/hl7/curation.tsv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:22:35.263106 bioregistry-0.9.6/src/bioregistry/data/external/miriam/
--rw-r--r--   0 runner    (1001) docker     (123)   576520 2023-05-06 00:44:46.000000 bioregistry-0.9.6/src/bioregistry/data/external/miriam/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)  1987182 2023-05-06 00:44:46.000000 bioregistry-0.9.6/src/bioregistry/data/external/miriam/raw.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:22:35.267106 bioregistry-0.9.6/src/bioregistry/data/external/n2t/
--rw-r--r--   0 runner    (1001) docker     (123)   425371 2023-05-06 00:53:54.000000 bioregistry-0.9.6/src/bioregistry/data/external/n2t/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)  1279133 2023-05-06 00:53:48.000000 bioregistry-0.9.6/src/bioregistry/data/external/n2t/raw.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:22:35.271106 bioregistry-0.9.6/src/bioregistry/data/external/ncbi/
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-06 00:58:44.000000 bioregistry-0.9.6/src/bioregistry/data/external/ncbi/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    18072 2023-05-06 00:58:43.000000 bioregistry-0.9.6/src/bioregistry/data/external/ncbi/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)   103465 2023-05-06 00:58:43.000000 bioregistry-0.9.6/src/bioregistry/data/external/ncbi/raw.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:22:35.271106 bioregistry-0.9.6/src/bioregistry/data/external/obofoundry/
--rw-r--r--   0 runner    (1001) docker     (123)   212323 2023-05-06 00:52:02.000000 bioregistry-0.9.6/src/bioregistry/data/external/obofoundry/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)   350196 2023-05-06 00:52:01.000000 bioregistry-0.9.6/src/bioregistry/data/external/obofoundry/raw.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:22:35.271106 bioregistry-0.9.6/src/bioregistry/data/external/ols/
--rw-r--r--   0 runner    (1001) docker     (123)   141937 2023-05-06 01:05:12.000000 bioregistry-0.9.6/src/bioregistry/data/external/ols/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)   805618 2023-05-06 01:05:12.000000 bioregistry-0.9.6/src/bioregistry/data/external/ols/raw.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:22:35.275106 bioregistry-0.9.6/src/bioregistry/data/external/ontobee/
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-06 01:05:34.000000 bioregistry-0.9.6/src/bioregistry/data/external/ontobee/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    23684 2023-05-06 01:05:34.000000 bioregistry-0.9.6/src/bioregistry/data/external/ontobee/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)   192177 2023-05-06 01:05:33.000000 bioregistry-0.9.6/src/bioregistry/data/external/ontobee/raw.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:22:35.275106 bioregistry-0.9.6/src/bioregistry/data/external/prefixcommons/
--rw-r--r--   0 runner    (1001) docker     (123)   111600 2023-05-06 00:58:25.000000 bioregistry-0.9.6/src/bioregistry/data/external/prefixcommons/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)   505834 2023-05-06 00:58:25.000000 bioregistry-0.9.6/src/bioregistry/data/external/prefixcommons/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)   883990 2023-05-06 00:58:25.000000 bioregistry-0.9.6/src/bioregistry/data/external/prefixcommons/raw.tsv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:22:35.283106 bioregistry-0.9.6/src/bioregistry/data/external/re3data/
--rw-r--r--   0 runner    (1001) docker     (123)  1742778 2023-05-06 00:51:59.000000 bioregistry-0.9.6/src/bioregistry/data/external/re3data/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)  2439371 2023-05-06 00:51:58.000000 bioregistry-0.9.6/src/bioregistry/data/external/re3data/processed.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:22:35.287106 bioregistry-0.9.6/src/bioregistry/data/external/uniprot/
--rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-05-06 00:44:51.000000 bioregistry-0.9.6/src/bioregistry/data/external/uniprot/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    67268 2023-05-06 00:44:50.000000 bioregistry-0.9.6/src/bioregistry/data/external/uniprot/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)    89621 2023-05-06 00:44:50.000000 bioregistry-0.9.6/src/bioregistry/data/external/uniprot/raw.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:22:35.287106 bioregistry-0.9.6/src/bioregistry/data/external/wikidata/
--rw-r--r--   0 runner    (1001) docker     (123)   125505 2023-05-06 00:52:11.000000 bioregistry-0.9.6/src/bioregistry/data/external/wikidata/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)   319146 2023-05-06 00:52:11.000000 bioregistry-0.9.6/src/bioregistry/data/external/wikidata/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)    47301 2023-05-06 01:05:41.000000 bioregistry-0.9.6/src/bioregistry/data/metaregistry.json
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-05-06 01:05:41.000000 bioregistry-0.9.6/src/bioregistry/data/mismatch.json
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/data/processing_biolink.json
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/data/processing_go.json
--rw-r--r--   0 runner    (1001) docker     (123)    29821 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/data/processing_ols.json
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/data/processing_wikidata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:22:35.291106 bioregistry-0.9.6/src/bioregistry/export/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/export/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/export/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/export/prefix_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     8861 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/export/rdf_export.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/export/schema_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/export/sssom_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/export/tables_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/export/tsv_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/export/warnings_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/export/yaml_export.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:22:35.295107 bioregistry-0.9.6/src/bioregistry/external/
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/external/aberowl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/external/bartoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/external/biocontext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/external/biolink.py
--rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/external/bioportal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/external/cellosaurus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/external/cheminf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/external/cropoct.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/external/edam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/external/fairsharing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/external/go.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:22:35.295107 bioregistry-0.9.6/src/bioregistry/external/hl7/
--rw-r--r--   0 runner    (1001) docker     (123)   319976 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/external/hl7/OID_Report.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/external/hl7/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/external/miriam.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/external/n2t.py
--rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/external/ncbi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/external/obofoundry.py
--rw-r--r--   0 runner    (1001) docker     (123)     7610 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/external/ols.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/external/ontobee.py
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/external/prefixcommons.py
--rw-r--r--   0 runner    (1001) docker     (123)     6191 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/external/re3data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/external/uniprot.py
--rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/external/wikidata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:22:35.295107 bioregistry-0.9.6/src/bioregistry/gh/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/gh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8350 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/gh/github_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9789 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/gh/new_prefix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:22:35.299106 bioregistry-0.9.6/src/bioregistry/health/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/health/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/health/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/health/check_homepages.py
--rw-r--r--   0 runner    (1001) docker     (123)     7053 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/health/check_providers.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/health/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8571 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/license_standardizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/lint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/metaresource_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18936 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/parse_iri.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13281 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/record_accumulator.py
--rw-r--r--   0 runner    (1001) docker     (123)    33164 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)    17532 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/resolve_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    63936 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/resource_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:22:35.299106 bioregistry-0.9.6/src/bioregistry/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13218 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/schema/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    42222 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/schema/schema.json
--rw-r--r--   0 runner    (1001) docker     (123)   106540 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/schema/struct.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/schema/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8188 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10183 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/upload_ndex.py
--rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/uri_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     8067 2023-05-06 00:43:46.000000 bioregistry-0.9.6/src/bioregistry/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-06 01:22:23.000000 bioregistry-0.9.6/src/bioregistry/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:22:35.195105 bioregistry-0.9.6/src/bioregistry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    31510 2023-05-06 01:22:35.000000 bioregistry-0.9.6/src/bioregistry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11252 2023-05-06 01:22:35.000000 bioregistry-0.9.6/src/bioregistry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 01:22:35.000000 bioregistry-0.9.6/src/bioregistry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-06 01:22:35.000000 bioregistry-0.9.6/src/bioregistry.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 00:43:59.000000 bioregistry-0.9.6/src/bioregistry.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-06 01:22:35.000000 bioregistry-0.9.6/src/bioregistry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-06 01:22:35.000000 bioregistry-0.9.6/src/bioregistry.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:22:35.303106 bioregistry-0.9.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-06 00:43:46.000000 bioregistry-0.9.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-06 00:43:46.000000 bioregistry-0.9.6/tests/test_acquisition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-06 00:43:46.000000 bioregistry-0.9.6/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-05-06 00:43:46.000000 bioregistry-0.9.6/tests/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-05-06 00:43:46.000000 bioregistry-0.9.6/tests/test_contexts.py
--rw-r--r--   0 runner    (1001) docker     (123)    46880 2023-05-06 00:43:46.000000 bioregistry-0.9.6/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-06 00:43:46.000000 bioregistry-0.9.6/tests/test_duplicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-05-06 00:43:46.000000 bioregistry-0.9.6/tests/test_identifiers_org.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-06 00:43:46.000000 bioregistry-0.9.6/tests/test_indra.py
--rw-r--r--   0 runner    (1001) docker     (123)     9604 2023-05-06 00:43:46.000000 bioregistry-0.9.6/tests/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-05-06 00:43:46.000000 bioregistry-0.9.6/tests/test_metaregistry.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-06 00:43:46.000000 bioregistry-0.9.6/tests/test_obofoundry.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-06 00:43:46.000000 bioregistry-0.9.6/tests/test_ols.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-05-06 00:43:46.000000 bioregistry-0.9.6/tests/test_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-05-06 00:43:46.000000 bioregistry-0.9.6/tests/test_resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-05-06 00:43:46.000000 bioregistry-0.9.6/tests/test_sparql.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-06 00:43:46.000000 bioregistry-0.9.6/tests/test_usages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-06 00:43:46.000000 bioregistry-0.9.6/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:22:35.303106 bioregistry-0.9.6/tests/test_web/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-06 00:43:46.000000 bioregistry-0.9.6/tests/test_web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-05-06 00:43:46.000000 bioregistry-0.9.6/tests/test_web/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7824 2023-05-06 00:43:46.000000 bioregistry-0.9.6/tests/test_web/test_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.807938 bioregistry-0.9.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-07 00:50:30.000000 bioregistry-0.9.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-07 00:50:30.000000 bioregistry-0.9.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    31510 2023-05-07 01:27:33.807938 bioregistry-0.9.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    30194 2023-05-07 00:50:30.000000 bioregistry-0.9.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.715937 bioregistry-0.9.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-05-07 00:50:30.000000 bioregistry-0.9.7/docs/bulk_prefix_request_template.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.719937 bioregistry-0.9.7/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    48331 2023-05-07 01:13:48.000000 bioregistry-0.9.7/docs/img/bibliography_years.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   157010 2023-05-07 01:14:08.000000 bioregistry-0.9.7/docs/img/bioregistry_coverage.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   107004 2023-05-07 01:14:07.000000 bioregistry-0.9.7/docs/img/bioregistry_coverage_bar.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    84710 2023-05-07 01:14:08.000000 bioregistry-0.9.7/docs/img/bioregistry_coverage_bar_short.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    77372 2023-05-07 00:50:30.000000 bioregistry-0.9.7/docs/img/datamodel_umls.svg
+-rw-r--r--   0 runner    (1001) docker     (123)  1382043 2023-05-07 01:18:05.000000 bioregistry-0.9.7/docs/img/external_overlap.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    72498 2023-05-07 01:14:35.000000 bioregistry-0.9.7/docs/img/has_attribute.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    28419 2023-05-07 01:18:06.000000 bioregistry-0.9.7/docs/img/providers.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    22283 2023-05-07 01:18:07.000000 bioregistry-0.9.7/docs/img/regex_report.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    51528 2023-05-07 01:14:06.000000 bioregistry-0.9.7/docs/img/xrefs.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.719937 bioregistry-0.9.7/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-07 00:50:30.000000 bioregistry-0.9.7/docs/source/alignment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-07 00:50:30.000000 bioregistry-0.9.7/docs/source/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7033 2023-05-07 01:27:22.000000 bioregistry-0.9.7/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-05-07 00:50:30.000000 bioregistry-0.9.7/docs/source/deployment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-05-07 00:50:30.000000 bioregistry-0.9.7/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   214468 2023-05-07 00:50:30.000000 bioregistry-0.9.7/docs/source/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-07 00:50:30.000000 bioregistry-0.9.7/docs/source/pandas.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-07 00:50:30.000000 bioregistry-0.9.7/docs/source/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-07 00:50:30.000000 bioregistry-0.9.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-05-07 01:27:33.811938 bioregistry-0.9.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.707937 bioregistry-0.9.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.723937 bioregistry-0.9.7/src/bioregistry/
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.727937 bioregistry-0.9.7/src/bioregistry/align/
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/align/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/align/aberowl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/align/bartoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/align/biocontext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/align/biolink.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/align/bioportal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/align/cellosaurus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/align/cheminf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/align/cropoct.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/align/edam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/align/fairsharing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/align/go.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/align/hl7.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/align/miriam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/align/n2t.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/align/ncbi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/align/obofoundry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/align/ols.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/align/ontobee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/align/prefixcommons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/align/re3data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/align/uniprot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10718 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/align/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/align/wikidata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.727937 bioregistry-0.9.7/src/bioregistry/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5007 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/analysis/title_tfidf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.727937 bioregistry-0.9.7/src/bioregistry/app/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17624 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10179 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.727937 bioregistry-0.9.7/src/bioregistry/app/static/
+-rw-r--r--   0 runner    (1001) docker     (123)   801449 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/static/logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.731938 bioregistry-0.9.7/src/bioregistry/app/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/collections.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/context.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/contexts.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/contributor.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/contributors.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.731938 bioregistry-0.9.7/src/bioregistry/app/templates/highlights/
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/highlights/keywords.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/highlights/owners.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/highlights/relations.html
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/highlights/twitter.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15622 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/home.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/macros.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.731938 bioregistry-0.9.7/src/bioregistry/app/templates/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/meta/access.html
+-rw-r--r--   0 runner    (1001) docker     (123)    19835 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/meta/acknowledgements.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10695 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/meta/download.html
+-rw-r--r--   0 runner    (1001) docker     (123)    16544 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/meta/related.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/meta/schema.html
+-rw-r--r--   0 runner    (1001) docker     (123)    19312 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/meta/summary.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/meta/sustainability.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8460 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/metaresource.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/metaresources.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/prose.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/reference.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.731938 bioregistry-0.9.7/src/bioregistry/app/templates/resolve_errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/resolve_errors/disallowed_identifier.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/resolve_errors/invalid_identifier.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/resolve_errors/missing_prefix.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/resolve_errors/missing_providers.html
+-rw-r--r--   0 runner    (1001) docker     (123)    32484 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/resource.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/resources.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19423 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.735937 bioregistry-0.9.7/src/bioregistry/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/benchmarks/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/benchmarks/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/benchmarks/curie_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/benchmarks/curie_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/benchmarks/uri_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/bibliometrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/collection_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23802 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.735937 bioregistry-0.9.7/src/bioregistry/curation/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/curation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/curation/add_co_providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/curation/add_descriptions_from_gs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/curation/add_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/curation/add_examples_from_javert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/curation/add_examples_from_ols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/curation/add_ontology_regexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/curation/bulk_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/curation/clean_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/curation/clean_name_suffixes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/curation/clean_publications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/curation/cleanup_authors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/curation/deprecation_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/curation/enrich_publications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/curation/import_pc_semiautomatic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/curation/make_description_curation_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/curation/map_bartoc_via_wikidata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/curation/map_re3data_via_fairsharing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/curation/rename_metaprefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/curation/review_pc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/curation/suggest_author_curation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/curation/suggest_uniprot_providers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.743938 bioregistry-0.9.7/src/bioregistry/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/data/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  4590847 2023-05-07 01:11:50.000000 bioregistry-0.9.7/src/bioregistry/data/bioregistry.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-05-07 01:11:50.000000 bioregistry-0.9.7/src/bioregistry/data/collections.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-07 01:11:50.000000 bioregistry-0.9.7/src/bioregistry/data/contexts.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.711937 bioregistry-0.9.7/src/bioregistry/data/external/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.743938 bioregistry-0.9.7/src/bioregistry/data/external/aberowl/
+-rw-r--r--   0 runner    (1001) docker     (123)   302996 2023-05-07 00:57:27.000000 bioregistry-0.9.7/src/bioregistry/data/external/aberowl/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)   623964 2023-05-07 00:57:27.000000 bioregistry-0.9.7/src/bioregistry/data/external/aberowl/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1281529 2023-05-07 00:57:20.000000 bioregistry-0.9.7/src/bioregistry/data/external/aberowl/raw.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.751938 bioregistry-0.9.7/src/bioregistry/data/external/agroportal/
+-rw-r--r--   0 runner    (1001) docker     (123)    42168 2023-05-07 00:53:01.000000 bioregistry-0.9.7/src/bioregistry/data/external/agroportal/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)   124136 2023-05-07 00:53:01.000000 bioregistry-0.9.7/src/bioregistry/data/external/agroportal/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)   663568 2023-05-07 00:53:01.000000 bioregistry-0.9.7/src/bioregistry/data/external/agroportal/raw.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.755938 bioregistry-0.9.7/src/bioregistry/data/external/bartoc/
+-rw-r--r--   0 runner    (1001) docker     (123)  1835101 2023-05-07 00:53:06.000000 bioregistry-0.9.7/src/bioregistry/data/external/bartoc/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)  2216766 2023-05-07 00:53:06.000000 bioregistry-0.9.7/src/bioregistry/data/external/bartoc/processed.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.759938 bioregistry-0.9.7/src/bioregistry/data/external/biocontext/
+-rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-05-07 01:05:06.000000 bioregistry-0.9.7/src/bioregistry/data/external/biocontext/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    74913 2023-05-07 01:05:06.000000 bioregistry-0.9.7/src/bioregistry/data/external/biocontext/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)    55878 2023-05-07 01:05:06.000000 bioregistry-0.9.7/src/bioregistry/data/external/biocontext/raw.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.759938 bioregistry-0.9.7/src/bioregistry/data/external/biolink/
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-07 00:53:19.000000 bioregistry-0.9.7/src/bioregistry/data/external/biolink/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    10406 2023-05-07 00:53:18.000000 bioregistry-0.9.7/src/bioregistry/data/external/biolink/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)   355095 2023-05-07 00:53:17.000000 bioregistry-0.9.7/src/bioregistry/data/external/biolink/raw.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.759938 bioregistry-0.9.7/src/bioregistry/data/external/bioportal/
+-rw-r--r--   0 runner    (1001) docker     (123)   253653 2023-05-07 00:57:10.000000 bioregistry-0.9.7/src/bioregistry/data/external/bioportal/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)   606737 2023-05-07 00:57:09.000000 bioregistry-0.9.7/src/bioregistry/data/external/bioportal/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)  3539154 2023-05-07 00:57:09.000000 bioregistry-0.9.7/src/bioregistry/data/external/bioportal/raw.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.767938 bioregistry-0.9.7/src/bioregistry/data/external/cellosaurus/
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-05-07 00:53:09.000000 bioregistry-0.9.7/src/bioregistry/data/external/cellosaurus/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    28730 2023-05-07 00:53:09.000000 bioregistry-0.9.7/src/bioregistry/data/external/cellosaurus/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)    32374 2023-05-07 00:53:09.000000 bioregistry-0.9.7/src/bioregistry/data/external/cellosaurus/raw.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.767938 bioregistry-0.9.7/src/bioregistry/data/external/cheminf/
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-07 01:05:04.000000 bioregistry-0.9.7/src/bioregistry/data/external/cheminf/processed.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.767938 bioregistry-0.9.7/src/bioregistry/data/external/cropoct/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-07 01:05:00.000000 bioregistry-0.9.7/src/bioregistry/data/external/cropoct/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    11407 2023-05-07 01:05:00.000000 bioregistry-0.9.7/src/bioregistry/data/external/cropoct/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)    25353 2023-05-07 01:05:00.000000 bioregistry-0.9.7/src/bioregistry/data/external/cropoct/raw.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.767938 bioregistry-0.9.7/src/bioregistry/data/external/ecoportal/
+-rw-r--r--   0 runner    (1001) docker     (123)     9198 2023-05-07 01:04:57.000000 bioregistry-0.9.7/src/bioregistry/data/external/ecoportal/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    18773 2023-05-07 01:04:57.000000 bioregistry-0.9.7/src/bioregistry/data/external/ecoportal/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)    98149 2023-05-07 01:04:57.000000 bioregistry-0.9.7/src/bioregistry/data/external/ecoportal/raw.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.767938 bioregistry-0.9.7/src/bioregistry/data/external/edam/
+-rw-r--r--   0 runner    (1001) docker     (123)    14599 2023-05-07 00:53:15.000000 bioregistry-0.9.7/src/bioregistry/data/external/edam/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    45616 2023-05-07 00:53:14.000000 bioregistry-0.9.7/src/bioregistry/data/external/edam/processed.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.767938 bioregistry-0.9.7/src/bioregistry/data/external/fairsharing/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/data/external/fairsharing/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   253879 2023-05-07 01:11:32.000000 bioregistry-0.9.7/src/bioregistry/data/external/fairsharing/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)   745109 2023-05-07 01:11:31.000000 bioregistry-0.9.7/src/bioregistry/data/external/fairsharing/processed.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.771938 bioregistry-0.9.7/src/bioregistry/data/external/go/
+-rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-05-07 00:57:13.000000 bioregistry-0.9.7/src/bioregistry/data/external/go/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)   143024 2023-05-07 00:57:12.000000 bioregistry-0.9.7/src/bioregistry/data/external/go/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)   115035 2023-05-07 00:57:12.000000 bioregistry-0.9.7/src/bioregistry/data/external/go/raw.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.771938 bioregistry-0.9.7/src/bioregistry/data/external/hl7/
+-rw-r--r--   0 runner    (1001) docker     (123)   157660 2023-05-07 01:04:45.000000 bioregistry-0.9.7/src/bioregistry/data/external/hl7/curation.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.771938 bioregistry-0.9.7/src/bioregistry/data/external/miriam/
+-rw-r--r--   0 runner    (1001) docker     (123)   576520 2023-05-07 01:04:36.000000 bioregistry-0.9.7/src/bioregistry/data/external/miriam/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1987182 2023-05-07 01:04:36.000000 bioregistry-0.9.7/src/bioregistry/data/external/miriam/raw.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.775938 bioregistry-0.9.7/src/bioregistry/data/external/n2t/
+-rw-r--r--   0 runner    (1001) docker     (123)   425371 2023-05-07 01:05:15.000000 bioregistry-0.9.7/src/bioregistry/data/external/n2t/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1279133 2023-05-07 01:05:09.000000 bioregistry-0.9.7/src/bioregistry/data/external/n2t/raw.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.779938 bioregistry-0.9.7/src/bioregistry/data/external/ncbi/
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-07 01:04:43.000000 bioregistry-0.9.7/src/bioregistry/data/external/ncbi/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    18072 2023-05-07 01:04:42.000000 bioregistry-0.9.7/src/bioregistry/data/external/ncbi/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)   103465 2023-05-07 01:04:42.000000 bioregistry-0.9.7/src/bioregistry/data/external/ncbi/raw.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.779938 bioregistry-0.9.7/src/bioregistry/data/external/obofoundry/
+-rw-r--r--   0 runner    (1001) docker     (123)   212323 2023-05-07 00:51:32.000000 bioregistry-0.9.7/src/bioregistry/data/external/obofoundry/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)   350196 2023-05-07 00:51:31.000000 bioregistry-0.9.7/src/bioregistry/data/external/obofoundry/raw.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.779938 bioregistry-0.9.7/src/bioregistry/data/external/ols/
+-rw-r--r--   0 runner    (1001) docker     (123)   141937 2023-05-07 01:11:49.000000 bioregistry-0.9.7/src/bioregistry/data/external/ols/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)   805618 2023-05-07 01:11:49.000000 bioregistry-0.9.7/src/bioregistry/data/external/ols/raw.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.783938 bioregistry-0.9.7/src/bioregistry/data/external/ontobee/
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-07 01:04:39.000000 bioregistry-0.9.7/src/bioregistry/data/external/ontobee/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    23684 2023-05-07 01:04:39.000000 bioregistry-0.9.7/src/bioregistry/data/external/ontobee/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)   192177 2023-05-07 01:04:39.000000 bioregistry-0.9.7/src/bioregistry/data/external/ontobee/raw.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.783938 bioregistry-0.9.7/src/bioregistry/data/external/prefixcommons/
+-rw-r--r--   0 runner    (1001) docker     (123)   111600 2023-05-07 00:57:31.000000 bioregistry-0.9.7/src/bioregistry/data/external/prefixcommons/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)   505834 2023-05-07 00:57:30.000000 bioregistry-0.9.7/src/bioregistry/data/external/prefixcommons/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)   883990 2023-05-07 00:57:30.000000 bioregistry-0.9.7/src/bioregistry/data/external/prefixcommons/raw.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.787938 bioregistry-0.9.7/src/bioregistry/data/external/re3data/
+-rw-r--r--   0 runner    (1001) docker     (123)  1742778 2023-05-07 01:04:33.000000 bioregistry-0.9.7/src/bioregistry/data/external/re3data/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)  2439371 2023-05-07 01:04:32.000000 bioregistry-0.9.7/src/bioregistry/data/external/re3data/processed.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.791938 bioregistry-0.9.7/src/bioregistry/data/external/uniprot/
+-rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-05-07 01:11:40.000000 bioregistry-0.9.7/src/bioregistry/data/external/uniprot/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    67268 2023-05-07 01:11:39.000000 bioregistry-0.9.7/src/bioregistry/data/external/uniprot/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)    89621 2023-05-07 01:11:39.000000 bioregistry-0.9.7/src/bioregistry/data/external/uniprot/raw.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.791938 bioregistry-0.9.7/src/bioregistry/data/external/wikidata/
+-rw-r--r--   0 runner    (1001) docker     (123)   125505 2023-05-07 01:11:36.000000 bioregistry-0.9.7/src/bioregistry/data/external/wikidata/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)   319146 2023-05-07 01:11:36.000000 bioregistry-0.9.7/src/bioregistry/data/external/wikidata/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)    47301 2023-05-07 01:11:50.000000 bioregistry-0.9.7/src/bioregistry/data/metaregistry.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-05-07 01:11:50.000000 bioregistry-0.9.7/src/bioregistry/data/mismatch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/data/processing_biolink.json
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/data/processing_go.json
+-rw-r--r--   0 runner    (1001) docker     (123)    29821 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/data/processing_ols.json
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/data/processing_wikidata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.795938 bioregistry-0.9.7/src/bioregistry/export/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/export/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/export/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/export/prefix_maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8861 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/export/rdf_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/export/schema_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/export/sssom_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/export/tables_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/export/tsv_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/export/warnings_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/export/yaml_export.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.799938 bioregistry-0.9.7/src/bioregistry/external/
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/external/aberowl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/external/bartoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/external/biocontext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/external/biolink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/external/bioportal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/external/cellosaurus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/external/cheminf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/external/cropoct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/external/edam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/external/fairsharing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/external/go.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.799938 bioregistry-0.9.7/src/bioregistry/external/hl7/
+-rw-r--r--   0 runner    (1001) docker     (123)   319976 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/external/hl7/OID_Report.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/external/hl7/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/external/miriam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/external/n2t.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/external/ncbi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/external/obofoundry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7610 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/external/ols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/external/ontobee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/external/prefixcommons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6191 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/external/re3data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/external/uniprot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/external/wikidata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.799938 bioregistry-0.9.7/src/bioregistry/gh/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/gh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8350 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/gh/github_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9789 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/gh/new_prefix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.803938 bioregistry-0.9.7/src/bioregistry/health/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/health/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/health/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/health/check_homepages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7053 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/health/check_providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/health/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8571 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/license_standardizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/lint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/metaresource_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18936 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/parse_iri.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13281 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/record_accumulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33164 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17532 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/resolve_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63936 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/resource_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.803938 bioregistry-0.9.7/src/bioregistry/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13218 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/schema/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42222 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/schema/schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)   106540 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/schema/struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/schema/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8188 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10183 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/upload_ndex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/uri_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8067 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-07 01:27:22.000000 bioregistry-0.9.7/src/bioregistry/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.723937 bioregistry-0.9.7/src/bioregistry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    31510 2023-05-07 01:27:33.000000 bioregistry-0.9.7/src/bioregistry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11252 2023-05-07 01:27:33.000000 bioregistry-0.9.7/src/bioregistry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 01:27:33.000000 bioregistry-0.9.7/src/bioregistry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-07 01:27:33.000000 bioregistry-0.9.7/src/bioregistry.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 00:50:47.000000 bioregistry-0.9.7/src/bioregistry.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-07 01:27:33.000000 bioregistry-0.9.7/src/bioregistry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-07 01:27:33.000000 bioregistry-0.9.7/src/bioregistry.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.807938 bioregistry-0.9.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-07 00:50:30.000000 bioregistry-0.9.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-07 00:50:30.000000 bioregistry-0.9.7/tests/test_acquisition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-07 00:50:30.000000 bioregistry-0.9.7/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-05-07 00:50:30.000000 bioregistry-0.9.7/tests/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-05-07 00:50:30.000000 bioregistry-0.9.7/tests/test_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46880 2023-05-07 00:50:30.000000 bioregistry-0.9.7/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-07 00:50:30.000000 bioregistry-0.9.7/tests/test_duplicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-05-07 00:50:30.000000 bioregistry-0.9.7/tests/test_identifiers_org.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-07 00:50:30.000000 bioregistry-0.9.7/tests/test_indra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9604 2023-05-07 00:50:30.000000 bioregistry-0.9.7/tests/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-05-07 00:50:30.000000 bioregistry-0.9.7/tests/test_metaregistry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-07 00:50:30.000000 bioregistry-0.9.7/tests/test_obofoundry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-07 00:50:30.000000 bioregistry-0.9.7/tests/test_ols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-05-07 00:50:30.000000 bioregistry-0.9.7/tests/test_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-05-07 00:50:30.000000 bioregistry-0.9.7/tests/test_resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-05-07 00:50:30.000000 bioregistry-0.9.7/tests/test_sparql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-07 00:50:30.000000 bioregistry-0.9.7/tests/test_usages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-07 00:50:30.000000 bioregistry-0.9.7/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.807938 bioregistry-0.9.7/tests/test_web/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-07 00:50:30.000000 bioregistry-0.9.7/tests/test_web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-05-07 00:50:30.000000 bioregistry-0.9.7/tests/test_web/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7824 2023-05-07 00:50:30.000000 bioregistry-0.9.7/tests/test_web/test_ui.py
```

### Comparing `bioregistry-0.9.6/LICENSE` & `bioregistry-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/MANIFEST.in` & `bioregistry-0.9.7/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/PKG-INFO` & `bioregistry-0.9.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioregistry
-Version: 0.9.6
+Version: 0.9.7
 Summary: Integrated registry of biological databases and nomenclatures
 Home-page: https://github.com/biopragmatics/bioregistry
 Download-URL: https://github.com/biopragmatics/bioregistry/releases
 Author: Charles Tapley Hoyt
 Author-email: cthoyt@gmail.com
 Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bioregistry Version: 0.9.6 Summary: Integrated
+Metadata-Version: 2.1 Name: bioregistry Version: 0.9.7 Summary: Integrated
 registry of biological databases and nomenclatures Home-page: https://
 github.com/biopragmatics/bioregistry Download-URL: https://github.com/
 biopragmatics/bioregistry/releases Author: Charles Tapley Hoyt Author-email:
 cthoyt@gmail.com Maintainer: Charles Tapley Hoyt Maintainer-email:
 cthoyt@gmail.com License: MIT Project-URL: Bug Tracker, https://github.com/
 biopragmatics/bioregistry/issues Keywords: databases,biological
 databases,biomedical databases Classifier: Development Status :: 4 - Beta
```

### Comparing `bioregistry-0.9.6/README.md` & `bioregistry-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/docs/bulk_prefix_request_template.tsv` & `bioregistry-0.9.7/docs/bulk_prefix_request_template.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/docs/img/bibliography_years.svg` & `bioregistry-0.9.7/docs/img/bibliography_years.svg`

 * *Files 8% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 000001c0: 3032 2f32 322d 7264 662d 7379 6e74 6178  02/22-rdf-syntax
 000001d0: 2d6e 7323 223e 0a20 2020 3c63 633a 576f  -ns#">.   <cc:Wo
 000001e0: 726b 3e0a 2020 2020 3c64 633a 7479 7065  rk>.    <dc:type
 000001f0: 2072 6466 3a72 6573 6f75 7263 653d 2268   rdf:resource="h
 00000200: 7474 703a 2f2f 7075 726c 2e6f 7267 2f64  ttp://purl.org/d
 00000210: 632f 6463 6d69 7479 7065 2f53 7469 6c6c  c/dcmitype/Still
 00000220: 496d 6167 6522 2f3e 0a20 2020 203c 6463  Image"/>.    <dc
-00000230: 3a64 6174 653e 3230 3233 2d30 352d 3036  :date>2023-05-06
-00000240: 5430 313a 3037 3a34 382e 3031 3231 3036  T01:07:48.012106
+00000230: 3a64 6174 653e 3230 3233 2d30 352d 3037  :date>2023-05-07
+00000240: 5430 313a 3133 3a34 382e 3838 3835 3439  T01:13:48.888549
 00000250: 3c2f 6463 3a64 6174 653e 0a20 2020 203c  </dc:date>.    <
 00000260: 6463 3a66 6f72 6d61 743e 696d 6167 652f  dc:format>image/
 00000270: 7376 672b 786d 6c3c 2f64 633a 666f 726d  svg+xml</dc:form
 00000280: 6174 3e0a 2020 2020 3c64 633a 6372 6561  at>.    <dc:crea
 00000290: 746f 723e 0a20 2020 2020 3c63 633a 4167  tor>.     <cc:Ag
 000002a0: 656e 743e 0a20 2020 2020 203c 6463 3a74  ent>.      <dc:t
 000002b0: 6974 6c65 3e4d 6174 706c 6f74 6c69 6220  itle>Matplotlib 
@@ -78,392 +78,392 @@
 000004d0: 3c70 6174 6820 643d 224d 2034 362e 3238  <path d="M 46.28
 000004e0: 3836 3535 2032 3038 2e39 3938 3731 3420  8655 208.998714 
 000004f0: 0a4c 2036 302e 3033 3738 3939 2032 3038  .L 60.037899 208
 00000500: 2e39 3938 3731 3420 0a4c 2036 302e 3033  .998714 .L 60.03
 00000510: 3738 3939 2032 3038 2e39 3938 3731 3420  7899 208.998714 
 00000520: 0a4c 2034 362e 3238 3836 3535 2032 3038  .L 46.288655 208
 00000530: 2e39 3938 3731 3420 0a7a 0a22 2063 6c69  .998714 .z." cli
-00000540: 702d 7061 7468 3d22 7572 6c28 2370 6266  p-path="url(#pbf
-00000550: 3265 3139 6631 6634 2922 2073 7479 6c65  2e19f1f4)" style
+00000540: 702d 7061 7468 3d22 7572 6c28 2370 3232  p-path="url(#p22
+00000550: 6131 3661 3664 6264 2922 2073 7479 6c65  a16a6dbd)" style
 00000560: 3d22 6669 6c6c 3a20 2365 6139 3661 3322  ="fill: #ea96a3"
 00000570: 2f3e 0a20 2020 3c2f 673e 0a20 2020 3c67  />.   </g>.   <g
 00000580: 2069 643d 2270 6174 6368 5f34 223e 0a20   id="patch_4">. 
 00000590: 2020 203c 7061 7468 2064 3d22 4d20 3633     <path d="M 63
 000005a0: 2e34 3735 3231 2032 3038 2e39 3938 3731  .47521 208.99871
 000005b0: 3420 0a4c 2037 372e 3232 3434 3534 2032  4 .L 77.224454 2
 000005c0: 3038 2e39 3938 3731 3420 0a4c 2037 372e  08.998714 .L 77.
 000005d0: 3232 3434 3534 2032 3033 2e38 3937 3335  224454 203.89735
 000005e0: 200a 4c20 3633 2e34 3735 3231 2032 3033   .L 63.47521 203
 000005f0: 2e38 3937 3335 200a 7a0a 2220 636c 6970  .89735 .z." clip
-00000600: 2d70 6174 683d 2275 726c 2823 7062 6632  -path="url(#pbf2
-00000610: 6531 3966 3166 3429 2220 7374 796c 653d  e19f1f4)" style=
+00000600: 2d70 6174 683d 2275 726c 2823 7032 3261  -path="url(#p22a
+00000610: 3136 6136 6462 6429 2220 7374 796c 653d  16a6dbd)" style=
 00000620: 2266 696c 6c3a 2023 6539 3937 3931 222f  "fill: #e99791"/
 00000630: 3e0a 2020 203c 2f67 3e0a 2020 203c 6720  >.   </g>.   <g 
 00000640: 6964 3d22 7061 7463 685f 3522 3e0a 2020  id="patch_5">.  
 00000650: 2020 3c70 6174 6820 643d 224d 2038 302e    <path d="M 80.
 00000660: 3636 3137 3635 2032 3038 2e39 3938 3731  661765 208.99871
 00000670: 3420 0a4c 2039 342e 3431 3130 3038 2032  4 .L 94.411008 2
 00000680: 3038 2e39 3938 3731 3420 0a4c 2039 342e  08.998714 .L 94.
 00000690: 3431 3130 3038 2031 3938 2e37 3935 3938  411008 198.79598
 000006a0: 3520 0a4c 2038 302e 3636 3137 3635 2031  5 .L 80.661765 1
 000006b0: 3938 2e37 3935 3938 3520 0a7a 0a22 2063  98.795985 .z." c
 000006c0: 6c69 702d 7061 7468 3d22 7572 6c28 2370  lip-path="url(#p
-000006d0: 6266 3265 3139 6631 6634 2922 2073 7479  bf2e19f1f4)" sty
+000006d0: 3232 6131 3661 3664 6264 2922 2073 7479  22a16a6dbd)" sty
 000006e0: 6c65 3d22 6669 6c6c 3a20 2365 3539 3437  le="fill: #e5947
 000006f0: 3122 2f3e 0a20 2020 3c2f 673e 0a20 2020  1"/>.   </g>.   
 00000700: 3c67 2069 643d 2270 6174 6368 5f36 223e  <g id="patch_6">
 00000710: 0a20 2020 203c 7061 7468 2064 3d22 4d20  .    <path d="M 
 00000720: 3937 2e38 3438 3331 3920 3230 382e 3939  97.848319 208.99
 00000730: 3837 3134 200a 4c20 3131 312e 3539 3735  8714 .L 111.5975
 00000740: 3633 2032 3038 2e39 3938 3731 3420 0a4c  63 208.998714 .L
 00000750: 2031 3131 2e35 3937 3536 3320 3137 382e   111.597563 178.
 00000760: 3339 3035 3237 200a 4c20 3937 2e38 3438  390527 .L 97.848
 00000770: 3331 3920 3137 382e 3339 3035 3237 200a  319 178.390527 .
 00000780: 7a0a 2220 636c 6970 2d70 6174 683d 2275  z." clip-path="u
-00000790: 726c 2823 7062 6632 6531 3966 3166 3429  rl(#pbf2e19f1f4)
+00000790: 726c 2823 7032 3261 3136 6136 6462 6429  rl(#p22a16a6dbd)
 000007a0: 2220 7374 796c 653d 2266 696c 6c3a 2023  " style="fill: #
 000007b0: 6437 3934 3465 222f 3e0a 2020 203c 2f67  d7944e"/>.   </g
 000007c0: 3e0a 2020 203c 6720 6964 3d22 7061 7463  >.   <g id="patc
 000007d0: 685f 3722 3e0a 2020 2020 3c70 6174 6820  h_7">.    <path 
 000007e0: 643d 224d 2031 3135 2e30 3334 3837 3420  d="M 115.034874 
 000007f0: 3230 382e 3939 3837 3134 200a 4c20 3132  208.998714 .L 12
 00000800: 382e 3738 3431 3137 2032 3038 2e39 3938  8.784117 208.998
 00000810: 3731 3420 0a4c 2031 3238 2e37 3834 3131  714 .L 128.78411
 00000820: 3720 3138 382e 3539 3332 3536 200a 4c20  7 188.593256 .L 
 00000830: 3131 352e 3033 3438 3734 2031 3838 2e35  115.034874 188.5
 00000840: 3933 3235 3620 0a7a 0a22 2063 6c69 702d  93256 .z." clip-
-00000850: 7061 7468 3d22 7572 6c28 2370 6266 3265  path="url(#pbf2e
-00000860: 3139 6631 6634 2922 2073 7479 6c65 3d22  19f1f4)" style="
+00000850: 7061 7468 3d22 7572 6c28 2370 3232 6131  path="url(#p22a1
+00000860: 3661 3664 6264 2922 2073 7479 6c65 3d22  6a6dbd)" style="
 00000870: 6669 6c6c 3a20 2363 3639 3934 6222 2f3e  fill: #c6994b"/>
 00000880: 0a20 2020 3c2f 673e 0a20 2020 3c67 2069  .   </g>.   <g i
 00000890: 643d 2270 6174 6368 5f38 223e 0a20 2020  d="patch_8">.   
 000008a0: 203c 7061 7468 2064 3d22 4d20 3133 322e   <path d="M 132.
 000008b0: 3232 3134 3238 2032 3038 2e39 3938 3731  221428 208.99871
 000008c0: 3420 0a4c 2031 3435 2e39 3730 3637 3220  4 .L 145.970672 
 000008d0: 3230 382e 3939 3837 3134 200a 4c20 3134  208.998714 .L 14
 000008e0: 352e 3937 3036 3732 2031 3733 2e32 3839  5.970672 173.289
 000008f0: 3136 3220 0a4c 2031 3332 2e32 3231 3432  162 .L 132.22142
 00000900: 3820 3137 332e 3238 3931 3632 200a 7a0a  8 173.289162 .z.
 00000910: 2220 636c 6970 2d70 6174 683d 2275 726c  " clip-path="url
-00000920: 2823 7062 6632 6531 3966 3166 3429 2220  (#pbf2e19f1f4)" 
+00000920: 2823 7032 3261 3136 6136 6462 6429 2220  (#p22a16a6dbd)" 
 00000930: 7374 796c 653d 2266 696c 6c3a 2023 6238  style="fill: #b8
 00000940: 3963 3439 222f 3e0a 2020 203c 2f67 3e0a  9c49"/>.   </g>.
 00000950: 2020 203c 6720 6964 3d22 7061 7463 685f     <g id="patch_
 00000960: 3922 3e0a 2020 2020 3c70 6174 6820 643d  9">.    <path d=
 00000970: 224d 2031 3439 2e34 3037 3938 3320 3230  "M 149.407983 20
 00000980: 382e 3939 3837 3134 200a 4c20 3136 332e  8.998714 .L 163.
 00000990: 3135 3732 3236 2032 3038 2e39 3938 3731  157226 208.99871
 000009a0: 3420 0a4c 2031 3633 2e31 3537 3232 3620  4 .L 163.157226 
 000009b0: 3135 372e 3938 3530 3639 200a 4c20 3134  157.985069 .L 14
 000009c0: 392e 3430 3739 3833 2031 3537 2e39 3835  9.407983 157.985
 000009d0: 3036 3920 0a7a 0a22 2063 6c69 702d 7061  069 .z." clip-pa
-000009e0: 7468 3d22 7572 6c28 2370 6266 3265 3139  th="url(#pbf2e19
-000009f0: 6631 6634 2922 2073 7479 6c65 3d22 6669  f1f4)" style="fi
+000009e0: 7468 3d22 7572 6c28 2370 3232 6131 3661  th="url(#p22a16a
+000009f0: 3664 6264 2922 2073 7479 6c65 3d22 6669  6dbd)" style="fi
 00000a00: 6c6c 3a20 2361 6239 6534 3722 2f3e 0a20  ll: #ab9e47"/>. 
 00000a10: 2020 3c2f 673e 0a20 2020 3c67 2069 643d    </g>.   <g id=
 00000a20: 2270 6174 6368 5f31 3022 3e0a 2020 2020  "patch_10">.    
 00000a30: 3c70 6174 6820 643d 224d 2031 3636 2e35  <path d="M 166.5
 00000a40: 3934 3533 3720 3230 382e 3939 3837 3134  94537 208.998714
 00000a50: 200a 4c20 3138 302e 3334 3337 3831 2032   .L 180.343781 2
 00000a60: 3038 2e39 3938 3731 3420 0a4c 2031 3830  08.998714 .L 180
 00000a70: 2e33 3433 3738 3120 3138 332e 3439 3138  .343781 183.4918
 00000a80: 3932 200a 4c20 3136 362e 3539 3435 3337  92 .L 166.594537
 00000a90: 2031 3833 2e34 3931 3839 3220 0a7a 0a22   183.491892 .z."
 00000aa0: 2063 6c69 702d 7061 7468 3d22 7572 6c28   clip-path="url(
-00000ab0: 2370 6266 3265 3139 6631 6634 2922 2073  #pbf2e19f1f4)" s
+00000ab0: 2370 3232 6131 3661 3664 6264 2922 2073  #p22a16a6dbd)" s
 00000ac0: 7479 6c65 3d22 6669 6c6c 3a20 2339 6561  tyle="fill: #9ea
 00000ad0: 3034 3522 2f3e 0a20 2020 3c2f 673e 0a20  045"/>.   </g>. 
 00000ae0: 2020 3c67 2069 643d 2270 6174 6368 5f31    <g id="patch_1
 00000af0: 3122 3e0a 2020 2020 3c70 6174 6820 643d  1">.    <path d=
 00000b00: 224d 2031 3833 2e37 3831 3039 3220 3230  "M 183.781092 20
 00000b10: 382e 3939 3837 3134 200a 4c20 3139 372e  8.998714 .L 197.
 00000b20: 3533 3033 3335 2032 3038 2e39 3938 3731  530335 208.99871
 00000b30: 3420 0a4c 2031 3937 2e35 3330 3333 3520  4 .L 197.530335 
 00000b40: 3133 372e 3537 3936 3131 200a 4c20 3138  137.579611 .L 18
 00000b50: 332e 3738 3130 3932 2031 3337 2e35 3739  3.781092 137.579
 00000b60: 3631 3120 0a7a 0a22 2063 6c69 702d 7061  611 .z." clip-pa
-00000b70: 7468 3d22 7572 6c28 2370 6266 3265 3139  th="url(#pbf2e19
-00000b80: 6631 6634 2922 2073 7479 6c65 3d22 6669  f1f4)" style="fi
+00000b70: 7468 3d22 7572 6c28 2370 3232 6131 3661  th="url(#p22a16a
+00000b80: 3664 6264 2922 2073 7479 6c65 3d22 6669  6dbd)" style="fi
 00000b90: 6c6c 3a20 2339 3161 3434 3622 2f3e 0a20  ll: #91a446"/>. 
 00000ba0: 2020 3c2f 673e 0a20 2020 3c67 2069 643d    </g>.   <g id=
 00000bb0: 2270 6174 6368 5f31 3222 3e0a 2020 2020  "patch_12">.    
 00000bc0: 3c70 6174 6820 643d 224d 2032 3030 2e39  <path d="M 200.9
 00000bd0: 3637 3634 3620 3230 382e 3939 3837 3134  67646 208.998714
 00000be0: 200a 4c20 3231 342e 3731 3638 3920 3230   .L 214.71689 20
 00000bf0: 382e 3939 3837 3134 200a 4c20 3231 342e  8.998714 .L 214.
 00000c00: 3731 3638 3920 3133 322e 3437 3832 3436  71689 132.478246
 00000c10: 200a 4c20 3230 302e 3936 3736 3436 2031   .L 200.967646 1
 00000c20: 3332 2e34 3738 3234 3620 0a7a 0a22 2063  32.478246 .z." c
 00000c30: 6c69 702d 7061 7468 3d22 7572 6c28 2370  lip-path="url(#p
-00000c40: 6266 3265 3139 6631 6634 2922 2073 7479  bf2e19f1f4)" sty
+00000c40: 3232 6131 3661 3664 6264 2922 2073 7479  22a16a6dbd)" sty
 00000c50: 6c65 3d22 6669 6c6c 3a20 2337 6661 3934  le="fill: #7fa94
 00000c60: 3622 2f3e 0a20 2020 3c2f 673e 0a20 2020  6"/>.   </g>.   
 00000c70: 3c67 2069 643d 2270 6174 6368 5f31 3322  <g id="patch_13"
 00000c80: 3e0a 2020 2020 3c70 6174 6820 643d 224d  >.    <path d="M
 00000c90: 2032 3138 2e31 3534 3230 3120 3230 382e   218.154201 208.
 00000ca0: 3939 3837 3134 200a 4c20 3233 312e 3930  998714 .L 231.90
 00000cb0: 3334 3435 2032 3038 2e39 3938 3731 3420  3445 208.998714 
 00000cc0: 0a4c 2032 3331 2e39 3033 3434 3520 3335  .L 231.903445 35
 00000cd0: 2e35 3532 3332 200a 4c20 3231 382e 3135  .55232 .L 218.15
 00000ce0: 3432 3031 2033 352e 3535 3233 3220 0a7a  4201 35.55232 .z
 00000cf0: 0a22 2063 6c69 702d 7061 7468 3d22 7572  ." clip-path="ur
-00000d00: 6c28 2370 6266 3265 3139 6631 6634 2922  l(#pbf2e19f1f4)"
+00000d00: 6c28 2370 3232 6131 3661 3664 6264 2922  l(#p22a16a6dbd)"
 00000d10: 2073 7479 6c65 3d22 6669 6c6c 3a20 2336   style="fill: #6
 00000d20: 3061 6534 3722 2f3e 0a20 2020 3c2f 673e  0ae47"/>.   </g>
 00000d30: 0a20 2020 3c67 2069 643d 2270 6174 6368  .   <g id="patch
 00000d40: 5f31 3422 3e0a 2020 2020 3c70 6174 6820  _14">.    <path 
 00000d50: 643d 224d 2032 3335 2e33 3430 3735 3520  d="M 235.340755 
 00000d60: 3230 382e 3939 3837 3134 200a 4c20 3234  208.998714 .L 24
 00000d70: 392e 3038 3939 3939 2032 3038 2e39 3938  9.089999 208.998
 00000d80: 3731 3420 0a4c 2032 3439 2e30 3839 3939  714 .L 249.08999
 00000d90: 3920 3831 2e34 3634 3630 3120 0a4c 2032  9 81.464601 .L 2
 00000da0: 3335 2e33 3430 3735 3520 3831 2e34 3634  35.340755 81.464
 00000db0: 3630 3120 0a7a 0a22 2063 6c69 702d 7061  601 .z." clip-pa
-00000dc0: 7468 3d22 7572 6c28 2370 6266 3265 3139  th="url(#pbf2e19
-00000dd0: 6631 6634 2922 2073 7479 6c65 3d22 6669  f1f4)" style="fi
+00000dc0: 7468 3d22 7572 6c28 2370 3232 6131 3661  th="url(#p22a16a
+00000dd0: 3664 6264 2922 2073 7479 6c65 3d22 6669  6dbd)" style="fi
 00000de0: 6c6c 3a20 2334 3862 3036 6122 2f3e 0a20  ll: #48b06a"/>. 
 00000df0: 2020 3c2f 673e 0a20 2020 3c67 2069 643d    </g>.   <g id=
 00000e00: 2270 6174 6368 5f31 3522 3e0a 2020 2020  "patch_15">.    
 00000e10: 3c70 6174 6820 643d 224d 2032 3532 2e35  <path d="M 252.5
 00000e20: 3237 3331 2032 3038 2e39 3938 3731 3420  2731 208.998714 
 00000e30: 0a4c 2032 3636 2e32 3736 3535 3420 3230  .L 266.276554 20
 00000e40: 382e 3939 3837 3134 200a 4c20 3236 362e  8.998714 .L 266.
 00000e50: 3237 3635 3534 2034 302e 3635 3336 3834  276554 40.653684
 00000e60: 200a 4c20 3235 322e 3532 3733 3120 3430   .L 252.52731 40
 00000e70: 2e36 3533 3638 3420 0a7a 0a22 2063 6c69  .653684 .z." cli
-00000e80: 702d 7061 7468 3d22 7572 6c28 2370 6266  p-path="url(#pbf
-00000e90: 3265 3139 6631 6634 2922 2073 7479 6c65  2e19f1f4)" style
+00000e80: 702d 7061 7468 3d22 7572 6c28 2370 3232  p-path="url(#p22
+00000e90: 6131 3661 3664 6264 2922 2073 7479 6c65  a16a6dbd)" style
 00000ea0: 3d22 6669 6c6c 3a20 2334 3961 6538 3322  ="fill: #49ae83"
 00000eb0: 2f3e 0a20 2020 3c2f 673e 0a20 2020 3c67  />.   </g>.   <g
 00000ec0: 2069 643d 2270 6174 6368 5f31 3622 3e0a   id="patch_16">.
 00000ed0: 2020 2020 3c70 6174 6820 643d 224d 2032      <path d="M 2
 00000ee0: 3639 2e37 3133 3836 3520 3230 382e 3939  69.713865 208.99
 00000ef0: 3837 3134 200a 4c20 3238 332e 3436 3331  8714 .L 283.4631
 00000f00: 3038 2032 3038 2e39 3938 3731 3420 0a4c  08 208.998714 .L
 00000f10: 2032 3833 2e34 3633 3130 3820 3631 2e30   283.463108 61.0
 00000f20: 3539 3134 3220 0a4c 2032 3639 2e37 3133  59142 .L 269.713
 00000f30: 3836 3520 3631 2e30 3539 3134 3220 0a7a  865 61.059142 .z
 00000f40: 0a22 2063 6c69 702d 7061 7468 3d22 7572  ." clip-path="ur
-00000f50: 6c28 2370 6266 3265 3139 6631 6634 2922  l(#pbf2e19f1f4)"
+00000f50: 6c28 2370 3232 6131 3661 3664 6264 2922  l(#p22a16a6dbd)"
 00000f60: 2073 7479 6c65 3d22 6669 6c6c 3a20 2334   style="fill: #4
 00000f70: 6161 6439 3122 2f3e 0a20 2020 3c2f 673e  aad91"/>.   </g>
 00000f80: 0a20 2020 3c67 2069 643d 2270 6174 6368  .   <g id="patch
 00000f90: 5f31 3722 3e0a 2020 2020 3c70 6174 6820  _17">.    <path 
 00000fa0: 643d 224d 2032 3836 2e39 3030 3431 3920  d="M 286.900419 
 00000fb0: 3230 382e 3939 3837 3134 200a 4c20 3330  208.998714 .L 30
 00000fc0: 302e 3634 3936 3633 2032 3038 2e39 3938  0.649663 208.998
 00000fd0: 3731 3420 0a4c 2033 3030 2e36 3439 3636  714 .L 300.64966
 00000fe0: 3320 3335 2e35 3532 3332 200a 4c20 3238  3 35.55232 .L 28
 00000ff0: 362e 3930 3034 3139 2033 352e 3535 3233  6.900419 35.5523
 00001000: 3220 0a7a 0a22 2063 6c69 702d 7061 7468  2 .z." clip-path
-00001010: 3d22 7572 6c28 2370 6266 3265 3139 6631  ="url(#pbf2e19f1
-00001020: 6634 2922 2073 7479 6c65 3d22 6669 6c6c  f4)" style="fill
+00001010: 3d22 7572 6c28 2370 3232 6131 3661 3664  ="url(#p22a16a6d
+00001020: 6264 2922 2073 7479 6c65 3d22 6669 6c6c  bd)" style="fill
 00001030: 3a20 2334 6161 6339 6222 2f3e 0a20 2020  : #4aac9b"/>.   
 00001040: 3c2f 673e 0a20 2020 3c67 2069 643d 2270  </g>.   <g id="p
 00001050: 6174 6368 5f31 3822 3e0a 2020 2020 3c70  atch_18">.    <p
 00001060: 6174 6820 643d 224d 2033 3034 2e30 3836  ath d="M 304.086
 00001070: 3937 3420 3230 382e 3939 3837 3134 200a  974 208.998714 .
 00001080: 4c20 3331 372e 3833 3632 3137 2032 3038  L 317.836217 208
 00001090: 2e39 3938 3731 3420 0a4c 2033 3137 2e38  .998714 .L 317.8
 000010a0: 3336 3231 3720 3731 2e32 3631 3837 3220  36217 71.261872 
 000010b0: 0a4c 2033 3034 2e30 3836 3937 3420 3731  .L 304.086974 71
 000010c0: 2e32 3631 3837 3220 0a7a 0a22 2063 6c69  .261872 .z." cli
-000010d0: 702d 7061 7468 3d22 7572 6c28 2370 6266  p-path="url(#pbf
-000010e0: 3265 3139 6631 6634 2922 2073 7479 6c65  2e19f1f4)" style
+000010d0: 702d 7061 7468 3d22 7572 6c28 2370 3232  p-path="url(#p22
+000010e0: 6131 3661 3664 6264 2922 2073 7479 6c65  a16a6dbd)" style
 000010f0: 3d22 6669 6c6c 3a20 2334 6261 6261 3422  ="fill: #4baba4"
 00001100: 2f3e 0a20 2020 3c2f 673e 0a20 2020 3c67  />.   </g>.   <g
 00001110: 2069 643d 2270 6174 6368 5f31 3922 3e0a   id="patch_19">.
 00001120: 2020 2020 3c70 6174 6820 643d 224d 2033      <path d="M 3
 00001130: 3231 2e32 3733 3532 3820 3230 382e 3939  21.273528 208.99
 00001140: 3837 3134 200a 4c20 3333 352e 3032 3237  8714 .L 335.0227
 00001150: 3732 2032 3038 2e39 3938 3731 3420 0a4c  72 208.998714 .L
 00001160: 2033 3335 2e30 3232 3737 3220 3631 2e30   335.022772 61.0
 00001170: 3539 3134 3220 0a4c 2033 3231 2e32 3733  59142 .L 321.273
 00001180: 3532 3820 3631 2e30 3539 3134 3220 0a7a  528 61.059142 .z
 00001190: 0a22 2063 6c69 702d 7061 7468 3d22 7572  ." clip-path="ur
-000011a0: 6c28 2370 6266 3265 3139 6631 6634 2922  l(#pbf2e19f1f4)"
+000011a0: 6c28 2370 3232 6131 3661 3664 6264 2922  l(#p22a16a6dbd)"
 000011b0: 2073 7479 6c65 3d22 6669 6c6c 3a20 2334   style="fill: #4
 000011c0: 6361 6261 6422 2f3e 0a20 2020 3c2f 673e  cabad"/>.   </g>
 000011d0: 0a20 2020 3c67 2069 643d 2270 6174 6368  .   <g id="patch
 000011e0: 5f32 3022 3e0a 2020 2020 3c70 6174 6820  _20">.    <path 
 000011f0: 643d 224d 2033 3338 2e34 3630 3038 3320  d="M 338.460083 
 00001200: 3230 382e 3939 3837 3134 200a 4c20 3335  208.998714 .L 35
 00001210: 322e 3230 3933 3236 2032 3038 2e39 3938  2.209326 208.998
 00001220: 3731 3420 0a4c 2033 3532 2e32 3039 3332  714 .L 352.20932
 00001230: 3620 3335 2e35 3532 3332 200a 4c20 3333  6 35.55232 .L 33
 00001240: 382e 3436 3030 3833 2033 352e 3535 3233  8.460083 35.5523
 00001250: 3220 0a7a 0a22 2063 6c69 702d 7061 7468  2 .z." clip-path
-00001260: 3d22 7572 6c28 2370 6266 3265 3139 6631  ="url(#pbf2e19f1
-00001270: 6634 2922 2073 7479 6c65 3d22 6669 6c6c  f4)" style="fill
+00001260: 3d22 7572 6c28 2370 3232 6131 3661 3664  ="url(#p22a16a6d
+00001270: 6264 2922 2073 7479 6c65 3d22 6669 6c6c  bd)" style="fill
 00001280: 3a20 2334 6561 6262 3722 2f3e 0a20 2020  : #4eabb7"/>.   
 00001290: 3c2f 673e 0a20 2020 3c67 2069 643d 2270  </g>.   <g id="p
 000012a0: 6174 6368 5f32 3122 3e0a 2020 2020 3c70  atch_21">.    <p
 000012b0: 6174 6820 643d 224d 2033 3535 2e36 3436  ath d="M 355.646
 000012c0: 3633 3720 3230 382e 3939 3837 3134 200a  637 208.998714 .
 000012d0: 4c20 3336 392e 3339 3538 3831 2032 3038  L 369.395881 208
 000012e0: 2e39 3938 3731 3420 0a4c 2033 3639 2e33  .998714 .L 369.3
 000012f0: 3935 3838 3120 3530 2e38 3536 3431 3320  95881 50.856413 
 00001300: 0a4c 2033 3535 2e36 3436 3633 3720 3530  .L 355.646637 50
 00001310: 2e38 3536 3431 3320 0a7a 0a22 2063 6c69  .856413 .z." cli
-00001320: 702d 7061 7468 3d22 7572 6c28 2370 6266  p-path="url(#pbf
-00001330: 3265 3139 6631 6634 2922 2073 7479 6c65  2e19f1f4)" style
+00001320: 702d 7061 7468 3d22 7572 6c28 2370 3232  p-path="url(#p22
+00001330: 6131 3661 3664 6264 2922 2073 7479 6c65  a16a6dbd)" style
 00001340: 3d22 6669 6c6c 3a20 2335 3061 6363 3322  ="fill: #50acc3"
 00001350: 2f3e 0a20 2020 3c2f 673e 0a20 2020 3c67  />.   </g>.   <g
 00001360: 2069 643d 2270 6174 6368 5f32 3222 3e0a   id="patch_22">.
 00001370: 2020 2020 3c70 6174 6820 643d 224d 2033      <path d="M 3
 00001380: 3732 2e38 3333 3139 3220 3230 382e 3939  72.833192 208.99
 00001390: 3837 3134 200a 4c20 3338 362e 3538 3234  8714 .L 386.5824
 000013a0: 3335 2032 3038 2e39 3938 3731 3420 0a4c  35 208.998714 .L
 000013b0: 2033 3836 2e35 3832 3433 3520 3435 2e37   386.582435 45.7
 000013c0: 3535 3034 3920 0a4c 2033 3732 2e38 3333  55049 .L 372.833
 000013d0: 3139 3220 3435 2e37 3535 3034 3920 0a7a  192 45.755049 .z
 000013e0: 0a22 2063 6c69 702d 7061 7468 3d22 7572  ." clip-path="ur
-000013f0: 6c28 2370 6266 3265 3139 6631 6634 2922  l(#pbf2e19f1f4)"
+000013f0: 6c28 2370 3232 6131 3661 3664 6264 2922  l(#p22a16a6dbd)"
 00001400: 2073 7479 6c65 3d22 6669 6c6c 3a20 2335   style="fill: #5
 00001410: 3461 6364 3122 2f3e 0a20 2020 3c2f 673e  4acd1"/>.   </g>
 00001420: 0a20 2020 3c67 2069 643d 2270 6174 6368  .   <g id="patch
 00001430: 5f32 3322 3e0a 2020 2020 3c70 6174 6820  _23">.    <path 
 00001440: 643d 224d 2033 3930 2e30 3139 3734 3620  d="M 390.019746 
 00001450: 3230 382e 3939 3837 3134 200a 4c20 3430  208.998714 .L 40
 00001460: 332e 3736 3839 3920 3230 382e 3939 3837  3.76899 208.9987
 00001470: 3134 200a 4c20 3430 332e 3736 3839 3920  14 .L 403.76899 
 00001480: 3131 322e 3037 3237 3838 200a 4c20 3339  112.072788 .L 39
 00001490: 302e 3031 3937 3436 2031 3132 2e30 3732  0.019746 112.072
 000014a0: 3738 3820 0a7a 0a22 2063 6c69 702d 7061  788 .z." clip-pa
-000014b0: 7468 3d22 7572 6c28 2370 6266 3265 3139  th="url(#pbf2e19
-000014c0: 6631 6634 2922 2073 7479 6c65 3d22 6669  f1f4)" style="fi
+000014b0: 7468 3d22 7572 6c28 2370 3232 6131 3661  th="url(#p22a16a
+000014c0: 3664 6264 2922 2073 7479 6c65 3d22 6669  6dbd)" style="fi
 000014d0: 6c6c 3a20 2336 6461 6565 3222 2f3e 0a20  ll: #6daee2"/>. 
 000014e0: 2020 3c2f 673e 0a20 2020 3c67 2069 643d    </g>.   <g id=
 000014f0: 2270 6174 6368 5f32 3422 3e0a 2020 2020  "patch_24">.    
 00001500: 3c70 6174 6820 643d 224d 2034 3037 2e32  <path d="M 407.2
 00001510: 3036 3330 3120 3230 382e 3939 3837 3134  06301 208.998714
 00001520: 200a 4c20 3432 302e 3935 3535 3435 2032   .L 420.955545 2
 00001530: 3038 2e39 3938 3731 3420 0a4c 2034 3230  08.998714 .L 420
 00001540: 2e39 3535 3534 3520 3132 322e 3237 3535  .955545 122.2755
 00001550: 3137 200a 4c20 3430 372e 3230 3633 3031  17 .L 407.206301
 00001560: 2031 3232 2e32 3735 3531 3720 0a7a 0a22   122.275517 .z."
 00001570: 2063 6c69 702d 7061 7468 3d22 7572 6c28   clip-path="url(
-00001580: 2370 6266 3265 3139 6631 6634 2922 2073  #pbf2e19f1f4)" s
+00001580: 2370 3232 6131 3661 3664 6264 2922 2073  #p22a16a6dbd)" s
 00001590: 7479 6c65 3d22 6669 6c6c 3a20 2339 3461  tyle="fill: #94a
 000015a0: 6565 3822 2f3e 0a20 2020 3c2f 673e 0a20  ee8"/>.   </g>. 
 000015b0: 2020 3c67 2069 643d 2270 6174 6368 5f32    <g id="patch_2
 000015c0: 3522 3e0a 2020 2020 3c70 6174 6820 643d  5">.    <path d=
 000015d0: 224d 2034 3234 2e33 3932 3835 3520 3230  "M 424.392855 20
 000015e0: 382e 3939 3837 3134 200a 4c20 3433 382e  8.998714 .L 438.
 000015f0: 3134 3230 3939 2032 3038 2e39 3938 3731  142099 208.99871
 00001600: 3420 0a4c 2034 3338 2e31 3432 3039 3920  4 .L 438.142099 
 00001610: 3831 2e34 3634 3630 3120 0a4c 2034 3234  81.464601 .L 424
 00001620: 2e33 3932 3835 3520 3831 2e34 3634 3630  .392855 81.46460
 00001630: 3120 0a7a 0a22 2063 6c69 702d 7061 7468  1 .z." clip-path
-00001640: 3d22 7572 6c28 2370 6266 3265 3139 6631  ="url(#pbf2e19f1
-00001650: 6634 2922 2073 7479 6c65 3d22 6669 6c6c  f4)" style="fill
+00001640: 3d22 7572 6c28 2370 3232 6131 3661 3664  ="url(#p22a16a6d
+00001650: 6264 2922 2073 7479 6c65 3d22 6669 6c6c  bd)" style="fill
 00001660: 3a20 2361 6461 6265 6222 2f3e 0a20 2020  : #adabeb"/>.   
 00001670: 3c2f 673e 0a20 2020 3c67 2069 643d 2270  </g>.   <g id="p
 00001680: 6174 6368 5f32 3622 3e0a 2020 2020 3c70  atch_26">.    <p
 00001690: 6174 6820 643d 224d 2034 3431 2e35 3739  ath d="M 441.579
 000016a0: 3431 2032 3038 2e39 3938 3731 3420 0a4c  41 208.998714 .L
 000016b0: 2034 3535 2e33 3238 3635 3420 3230 382e   455.328654 208.
 000016c0: 3939 3837 3134 200a 4c20 3435 352e 3332  998714 .L 455.32
 000016d0: 3836 3534 2031 3638 2e31 3837 3739 3820  8654 168.187798 
 000016e0: 0a4c 2034 3431 2e35 3739 3431 2031 3638  .L 441.57941 168
 000016f0: 2e31 3837 3739 3820 0a7a 0a22 2063 6c69  .187798 .z." cli
-00001700: 702d 7061 7468 3d22 7572 6c28 2370 6266  p-path="url(#pbf
-00001710: 3265 3139 6631 6634 2922 2073 7479 6c65  2e19f1f4)" style
+00001700: 702d 7061 7468 3d22 7572 6c28 2370 3232  p-path="url(#p22
+00001710: 6131 3661 3664 6264 2922 2073 7479 6c65  a16a6dbd)" style
 00001720: 3d22 6669 6c6c 3a20 2362 6561 3465 6122  ="fill: #bea4ea"
 00001730: 2f3e 0a20 2020 3c2f 673e 0a20 2020 3c67  />.   </g>.   <g
 00001740: 2069 643d 2270 6174 6368 5f32 3722 3e0a   id="patch_27">.
 00001750: 2020 2020 3c70 6174 6820 643d 224d 2034      <path d="M 4
 00001760: 3538 2e37 3635 3936 3520 3230 382e 3939  58.765965 208.99
 00001770: 3837 3134 200a 4c20 3437 322e 3531 3532  8714 .L 472.5152
 00001780: 3038 2032 3038 2e39 3938 3731 3420 0a4c  08 208.998714 .L
 00001790: 2034 3732 2e35 3135 3230 3820 3135 322e   472.515208 152.
 000017a0: 3838 3337 3034 200a 4c20 3435 382e 3736  883704 .L 458.76
 000017b0: 3539 3635 2031 3532 2e38 3833 3730 3420  5965 152.883704 
 000017c0: 0a7a 0a22 2063 6c69 702d 7061 7468 3d22  .z." clip-path="
-000017d0: 7572 6c28 2370 6266 3265 3139 6631 6634  url(#pbf2e19f1f4
+000017d0: 7572 6c28 2370 3232 6131 3661 3664 6264  url(#p22a16a6dbd
 000017e0: 2922 2073 7479 6c65 3d22 6669 6c6c 3a20  )" style="fill: 
 000017f0: 2363 6539 6265 3922 2f3e 0a20 2020 3c2f  #ce9be9"/>.   </
 00001800: 673e 0a20 2020 3c67 2069 643d 2270 6174  g>.   <g id="pat
 00001810: 6368 5f32 3822 3e0a 2020 2020 3c70 6174  ch_28">.    <pat
 00001820: 6820 643d 224d 2034 3735 2e39 3532 3531  h d="M 475.95251
 00001830: 3920 3230 382e 3939 3837 3134 200a 4c20  9 208.998714 .L 
 00001840: 3438 392e 3730 3137 3633 2032 3038 2e39  489.701763 208.9
 00001850: 3938 3731 3420 0a4c 2034 3839 2e37 3031  98714 .L 489.701
 00001860: 3736 3320 3134 372e 3738 3233 3420 0a4c  763 147.78234 .L
 00001870: 2034 3735 2e39 3532 3531 3920 3134 372e   475.952519 147.
 00001880: 3738 3233 3420 0a7a 0a22 2063 6c69 702d  78234 .z." clip-
-00001890: 7061 7468 3d22 7572 6c28 2370 6266 3265  path="url(#pbf2e
-000018a0: 3139 6631 6634 2922 2073 7479 6c65 3d22  19f1f4)" style="
+00001890: 7061 7468 3d22 7572 6c28 2370 3232 6131  path="url(#p22a1
+000018a0: 3661 3664 6264 2922 2073 7479 6c65 3d22  6a6dbd)" style="
 000018b0: 6669 6c6c 3a20 2364 6638 6665 3722 2f3e  fill: #df8fe7"/>
 000018c0: 0a20 2020 3c2f 673e 0a20 2020 3c67 2069  .   </g>.   <g i
 000018d0: 643d 2270 6174 6368 5f32 3922 3e0a 2020  d="patch_29">.  
 000018e0: 2020 3c70 6174 6820 643d 224d 2034 3933    <path d="M 493
 000018f0: 2e31 3339 3037 3420 3230 382e 3939 3837  .139074 208.9987
 00001900: 3134 200a 4c20 3530 362e 3838 3833 3137  14 .L 506.888317
 00001910: 2032 3038 2e39 3938 3731 3420 0a4c 2035   208.998714 .L 5
 00001920: 3036 2e38 3838 3331 3720 3134 322e 3638  06.888317 142.68
 00001930: 3039 3735 200a 4c20 3439 332e 3133 3930  0975 .L 493.1390
 00001940: 3734 2031 3432 2e36 3830 3937 3520 0a7a  74 142.680975 .z
 00001950: 0a22 2063 6c69 702d 7061 7468 3d22 7572  ." clip-path="ur
-00001960: 6c28 2370 6266 3265 3139 6631 6634 2922  l(#pbf2e19f1f4)"
+00001960: 6c28 2370 3232 6131 3661 3664 6264 2922  l(#p22a16a6dbd)"
 00001970: 2073 7479 6c65 3d22 6669 6c6c 3a20 2365   style="fill: #e
 00001980: 3738 6264 6222 2f3e 0a20 2020 3c2f 673e  78bdb"/>.   </g>
 00001990: 0a20 2020 3c67 2069 643d 2270 6174 6368  .   <g id="patch
 000019a0: 5f33 3022 3e0a 2020 2020 3c70 6174 6820  _30">.    <path 
 000019b0: 643d 224d 2035 3130 2e33 3235 3632 3820  d="M 510.325628 
 000019c0: 3230 382e 3939 3837 3134 200a 4c20 3532  208.998714 .L 52
 000019d0: 342e 3037 3438 3732 2032 3038 2e39 3938  4.074872 208.998
 000019e0: 3731 3420 0a4c 2035 3234 2e30 3734 3837  714 .L 524.07487
 000019f0: 3220 3133 372e 3537 3936 3131 200a 4c20  2 137.579611 .L 
 00001a00: 3531 302e 3332 3536 3238 2031 3337 2e35  510.325628 137.5
 00001a10: 3739 3631 3120 0a7a 0a22 2063 6c69 702d  79611 .z." clip-
-00001a20: 7061 7468 3d22 7572 6c28 2370 6266 3265  path="url(#pbf2e
-00001a30: 3139 6631 6634 2922 2073 7479 6c65 3d22  19f1f4)" style="
+00001a20: 7061 7468 3d22 7572 6c28 2370 3232 6131  path="url(#p22a1
+00001a30: 3661 3664 6264 2922 2073 7479 6c65 3d22  6a6dbd)" style="
 00001a40: 6669 6c6c 3a20 2365 3838 6663 6322 2f3e  fill: #e88fcc"/>
 00001a50: 0a20 2020 3c2f 673e 0a20 2020 3c67 2069  .   </g>.   <g i
 00001a60: 643d 2270 6174 6368 5f33 3122 3e0a 2020  d="patch_31">.  
 00001a70: 2020 3c70 6174 6820 643d 224d 2035 3237    <path d="M 527
 00001a80: 2e35 3132 3138 3320 3230 382e 3939 3837  .512183 208.9987
 00001a90: 3134 200a 4c20 3534 312e 3236 3134 3236  14 .L 541.261426
 00001aa0: 2032 3038 2e39 3938 3731 3420 0a4c 2035   208.998714 .L 5
 00001ab0: 3431 2e32 3631 3432 3620 3136 382e 3138  41.261426 168.18
 00001ac0: 3737 3938 200a 4c20 3532 372e 3531 3231  7798 .L 527.5121
 00001ad0: 3833 2031 3638 2e31 3837 3739 3820 0a7a  83 168.187798 .z
 00001ae0: 0a22 2063 6c69 702d 7061 7468 3d22 7572  ." clip-path="ur
-00001af0: 6c28 2370 6266 3265 3139 6631 6634 2922  l(#pbf2e19f1f4)"
+00001af0: 6c28 2370 3232 6131 3661 3664 6264 2922  l(#p22a16a6dbd)"
 00001b00: 2073 7479 6c65 3d22 6669 6c6c 3a20 2365   style="fill: #e
 00001b10: 3839 3162 6622 2f3e 0a20 2020 3c2f 673e  891bf"/>.   </g>
 00001b20: 0a20 2020 3c67 2069 643d 2270 6174 6368  .   <g id="patch
 00001b30: 5f33 3222 3e0a 2020 2020 3c70 6174 6820  _32">.    <path 
 00001b40: 643d 224d 2035 3434 2e36 3938 3733 3720  d="M 544.698737 
 00001b50: 3230 382e 3939 3837 3134 200a 4c20 3535  208.998714 .L 55
 00001b60: 382e 3434 3739 3831 2032 3038 2e39 3938  8.447981 208.998
 00001b70: 3731 3420 0a4c 2035 3538 2e34 3437 3938  714 .L 558.44798
 00001b80: 3120 3139 332e 3639 3436 3231 200a 4c20  1 193.694621 .L 
 00001b90: 3534 342e 3639 3837 3337 2031 3933 2e36  544.698737 193.6
 00001ba0: 3934 3632 3120 0a7a 0a22 2063 6c69 702d  94621 .z." clip-
-00001bb0: 7061 7468 3d22 7572 6c28 2370 6266 3265  path="url(#pbf2e
-00001bc0: 3139 6631 6634 2922 2073 7479 6c65 3d22  19f1f4)" style="
+00001bb0: 7061 7468 3d22 7572 6c28 2370 3232 6131  path="url(#p22a1
+00001bc0: 3661 3664 6264 2922 2073 7479 6c65 3d22  6a6dbd)" style="
 00001bd0: 6669 6c6c 3a20 2365 3939 3462 3222 2f3e  fill: #e994b2"/>
 00001be0: 0a20 2020 3c2f 673e 0a20 2020 3c67 2069  .   </g>.   <g i
 00001bf0: 643d 226d 6174 706c 6f74 6c69 622e 6178  d="matplotlib.ax
 00001c00: 6973 5f31 223e 0a20 2020 203c 6720 6964  is_1">.    <g id
 00001c10: 3d22 7874 6963 6b5f 3122 3e0a 2020 2020  ="xtick_1">.    
 00001c20: 203c 6720 6964 3d22 6c69 6e65 3264 5f31   <g id="line2d_1
 00001c30: 223e 0a20 2020 2020 203c 6465 6673 3e0a  ">.      <defs>.
 00001c40: 2020 2020 2020 203c 7061 7468 2069 643d         <path id=
-00001c50: 226d 3963 3065 6562 6161 6163 2220 643d  "m9c0eebaaac" d=
+00001c50: 226d 6437 6633 3538 6131 3664 2220 643d  "md7f358a16d" d=
 00001c60: 224d 2030 2030 200a 4c20 3020 332e 3520  "M 0 0 .L 0 3.5 
 00001c70: 0a22 2073 7479 6c65 3d22 7374 726f 6b65  ." style="stroke
 00001c80: 3a20 2330 3030 3030 303b 2073 7472 6f6b  : #000000; strok
 00001c90: 652d 7769 6474 683a 2030 2e38 222f 3e0a  e-width: 0.8"/>.
 00001ca0: 2020 2020 2020 3c2f 6465 6673 3e0a 2020        </defs>.  
 00001cb0: 2020 2020 3c67 3e0a 2020 2020 2020 203c      <g>.       <
 00001cc0: 7573 6520 786c 696e 6b3a 6872 6566 3d22  use xlink:href="
-00001cd0: 236d 3963 3065 6562 6161 6163 2220 783d  #m9c0eebaaac" x=
+00001cd0: 236d 6437 6633 3538 6131 3664 2220 783d  #md7f358a16d" x=
 00001ce0: 2235 332e 3136 3332 3737 2220 793d 2232  "53.163277" y="2
 00001cf0: 3038 2e39 3938 3731 3422 2073 7479 6c65  08.998714" style
 00001d00: 3d22 7374 726f 6b65 3a20 2330 3030 3030  ="stroke: #00000
 00001d10: 303b 2073 7472 6f6b 652d 7769 6474 683a  0; stroke-width:
 00001d20: 2030 2e38 222f 3e0a 2020 2020 2020 3c2f   0.8"/>.      </
 00001d30: 673e 0a20 2020 2020 3c2f 673e 0a20 2020  g>.     </g>.   
 00001d40: 2020 3c67 2069 643d 2274 6578 745f 3122    <g id="text_1"
@@ -561,15 +561,15 @@
 00002300: 222f 3e0a 2020 2020 2020 3c2f 673e 0a20  "/>.      </g>. 
 00002310: 2020 2020 3c2f 673e 0a20 2020 203c 2f67      </g>.    </g
 00002320: 3e0a 2020 2020 3c67 2069 643d 2278 7469  >.    <g id="xti
 00002330: 636b 5f32 223e 0a20 2020 2020 3c67 2069  ck_2">.     <g i
 00002340: 643d 226c 696e 6532 645f 3222 3e0a 2020  d="line2d_2">.  
 00002350: 2020 2020 3c67 3e0a 2020 2020 2020 203c      <g>.       <
 00002360: 7573 6520 786c 696e 6b3a 6872 6566 3d22  use xlink:href="
-00002370: 236d 3963 3065 6562 6161 6163 2220 783d  #m9c0eebaaac" x=
+00002370: 236d 6437 6633 3538 6131 3664 2220 783d  #md7f358a16d" x=
 00002380: 2237 302e 3334 3938 3332 2220 793d 2232  "70.349832" y="2
 00002390: 3038 2e39 3938 3731 3422 2073 7479 6c65  08.998714" style
 000023a0: 3d22 7374 726f 6b65 3a20 2330 3030 3030  ="stroke: #00000
 000023b0: 303b 2073 7472 6f6b 652d 7769 6474 683a  0; stroke-width:
 000023c0: 2030 2e38 222f 3e0a 2020 2020 2020 3c2f   0.8"/>.      </
 000023d0: 673e 0a20 2020 2020 3c2f 673e 0a20 2020  g>.     </g>.   
 000023e0: 2020 3c67 2069 643d 2274 6578 745f 3222    <g id="text_2"
@@ -628,16 +628,16 @@
 00002730: 783d 2231 3930 2e38 3639 3134 3122 2f3e  x="190.869141"/>
 00002740: 0a20 2020 2020 203c 2f67 3e0a 2020 2020  .      </g>.    
 00002750: 203c 2f67 3e0a 2020 2020 3c2f 673e 0a20   </g>.    </g>. 
 00002760: 2020 203c 6720 6964 3d22 7874 6963 6b5f     <g id="xtick_
 00002770: 3322 3e0a 2020 2020 203c 6720 6964 3d22  3">.     <g id="
 00002780: 6c69 6e65 3264 5f33 223e 0a20 2020 2020  line2d_3">.     
 00002790: 203c 673e 0a20 2020 2020 2020 3c75 7365   <g>.       <use
-000027a0: 2078 6c69 6e6b 3a68 7265 663d 2223 6d39   xlink:href="#m9
-000027b0: 6330 6565 6261 6161 6322 2078 3d22 3837  c0eebaaac" x="87
+000027a0: 2078 6c69 6e6b 3a68 7265 663d 2223 6d64   xlink:href="#md
+000027b0: 3766 3335 3861 3136 6422 2078 3d22 3837  7f358a16d" x="87
 000027c0: 2e35 3336 3338 3622 2079 3d22 3230 382e  .536386" y="208.
 000027d0: 3939 3837 3134 2220 7374 796c 653d 2273  998714" style="s
 000027e0: 7472 6f6b 653a 2023 3030 3030 3030 3b20  troke: #000000; 
 000027f0: 7374 726f 6b65 2d77 6964 7468 3a20 302e  stroke-width: 0.
 00002800: 3822 2f3e 0a20 2020 2020 203c 2f67 3e0a  8"/>.      </g>.
 00002810: 2020 2020 203c 2f67 3e0a 2020 2020 203c       </g>.     <
 00002820: 6720 6964 3d22 7465 7874 5f33 223e 0a20  g id="text_3">. 
@@ -705,16 +705,16 @@
 00002c00: 2e38 3639 3134 3122 2f3e 0a20 2020 2020  .869141"/>.     
 00002c10: 203c 2f67 3e0a 2020 2020 203c 2f67 3e0a   </g>.     </g>.
 00002c20: 2020 2020 3c2f 673e 0a20 2020 203c 6720      </g>.    <g 
 00002c30: 6964 3d22 7874 6963 6b5f 3422 3e0a 2020  id="xtick_4">.  
 00002c40: 2020 203c 6720 6964 3d22 6c69 6e65 3264     <g id="line2d
 00002c50: 5f34 223e 0a20 2020 2020 203c 673e 0a20  _4">.      <g>. 
 00002c60: 2020 2020 2020 3c75 7365 2078 6c69 6e6b        <use xlink
-00002c70: 3a68 7265 663d 2223 6d39 6330 6565 6261  :href="#m9c0eeba
-00002c80: 6161 6322 2078 3d22 3130 342e 3732 3239  aac" x="104.7229
+00002c70: 3a68 7265 663d 2223 6d64 3766 3335 3861  :href="#md7f358a
+00002c80: 3136 6422 2078 3d22 3130 342e 3732 3239  16d" x="104.7229
 00002c90: 3431 2220 793d 2232 3038 2e39 3938 3731  41" y="208.99871
 00002ca0: 3422 2073 7479 6c65 3d22 7374 726f 6b65  4" style="stroke
 00002cb0: 3a20 2330 3030 3030 303b 2073 7472 6f6b  : #000000; strok
 00002cc0: 652d 7769 6474 683a 2030 2e38 222f 3e0a  e-width: 0.8"/>.
 00002cd0: 2020 2020 2020 3c2f 673e 0a20 2020 2020        </g>.     
 00002ce0: 3c2f 673e 0a20 2020 2020 3c67 2069 643d  </g>.     <g id=
 00002cf0: 2274 6578 745f 3422 3e0a 2020 2020 2020  "text_4">.      
@@ -752,15 +752,15 @@
 00002ef0: 3122 2f3e 0a20 2020 2020 203c 2f67 3e0a  1"/>.      </g>.
 00002f00: 2020 2020 203c 2f67 3e0a 2020 2020 3c2f       </g>.    </
 00002f10: 673e 0a20 2020 203c 6720 6964 3d22 7874  g>.    <g id="xt
 00002f20: 6963 6b5f 3522 3e0a 2020 2020 203c 6720  ick_5">.     <g 
 00002f30: 6964 3d22 6c69 6e65 3264 5f35 223e 0a20  id="line2d_5">. 
 00002f40: 2020 2020 203c 673e 0a20 2020 2020 2020       <g>.       
 00002f50: 3c75 7365 2078 6c69 6e6b 3a68 7265 663d  <use xlink:href=
-00002f60: 2223 6d39 6330 6565 6261 6161 6322 2078  "#m9c0eebaaac" x
+00002f60: 2223 6d64 3766 3335 3861 3136 6422 2078  "#md7f358a16d" x
 00002f70: 3d22 3132 312e 3930 3934 3935 2220 793d  ="121.909495" y=
 00002f80: 2232 3038 2e39 3938 3731 3422 2073 7479  "208.998714" sty
 00002f90: 6c65 3d22 7374 726f 6b65 3a20 2330 3030  le="stroke: #000
 00002fa0: 3030 303b 2073 7472 6f6b 652d 7769 6474  000; stroke-widt
 00002fb0: 683a 2030 2e38 222f 3e0a 2020 2020 2020  h: 0.8"/>.      
 00002fc0: 3c2f 673e 0a20 2020 2020 3c2f 673e 0a20  </g>.     </g>. 
 00002fd0: 2020 2020 3c67 2069 643d 2274 6578 745f      <g id="text_
@@ -840,15 +840,15 @@
 00003470: 2f3e 0a20 2020 2020 203c 2f67 3e0a 2020  />.      </g>.  
 00003480: 2020 203c 2f67 3e0a 2020 2020 3c2f 673e     </g>.    </g>
 00003490: 0a20 2020 203c 6720 6964 3d22 7874 6963  .    <g id="xtic
 000034a0: 6b5f 3622 3e0a 2020 2020 203c 6720 6964  k_6">.     <g id
 000034b0: 3d22 6c69 6e65 3264 5f36 223e 0a20 2020  ="line2d_6">.   
 000034c0: 2020 203c 673e 0a20 2020 2020 2020 3c75     <g>.       <u
 000034d0: 7365 2078 6c69 6e6b 3a68 7265 663d 2223  se xlink:href="#
-000034e0: 6d39 6330 6565 6261 6161 6322 2078 3d22  m9c0eebaaac" x="
+000034e0: 6d64 3766 3335 3861 3136 6422 2078 3d22  md7f358a16d" x="
 000034f0: 3133 392e 3039 3630 3522 2079 3d22 3230  139.09605" y="20
 00003500: 382e 3939 3837 3134 2220 7374 796c 653d  8.998714" style=
 00003510: 2273 7472 6f6b 653a 2023 3030 3030 3030  "stroke: #000000
 00003520: 3b20 7374 726f 6b65 2d77 6964 7468 3a20  ; stroke-width: 
 00003530: 302e 3822 2f3e 0a20 2020 2020 203c 2f67  0.8"/>.      </g
 00003540: 3e0a 2020 2020 203c 2f67 3e0a 2020 2020  >.     </g>.    
 00003550: 203c 6720 6964 3d22 7465 7874 5f36 223e   <g id="text_6">
@@ -874,16 +874,16 @@
 00003690: 302e 3836 3931 3431 222f 3e0a 2020 2020  0.869141"/>.    
 000036a0: 2020 3c2f 673e 0a20 2020 2020 3c2f 673e    </g>.     </g>
 000036b0: 0a20 2020 203c 2f67 3e0a 2020 2020 3c67  .    </g>.    <g
 000036c0: 2069 643d 2278 7469 636b 5f37 223e 0a20   id="xtick_7">. 
 000036d0: 2020 2020 3c67 2069 643d 226c 696e 6532      <g id="line2
 000036e0: 645f 3722 3e0a 2020 2020 2020 3c67 3e0a  d_7">.      <g>.
 000036f0: 2020 2020 2020 203c 7573 6520 786c 696e         <use xlin
-00003700: 6b3a 6872 6566 3d22 236d 3963 3065 6562  k:href="#m9c0eeb
-00003710: 6161 6163 2220 783d 2231 3536 2e32 3832  aaac" x="156.282
+00003700: 6b3a 6872 6566 3d22 236d 6437 6633 3538  k:href="#md7f358
+00003710: 6131 3664 2220 783d 2231 3536 2e32 3832  a16d" x="156.282
 00003720: 3630 3522 2079 3d22 3230 382e 3939 3837  605" y="208.9987
 00003730: 3134 2220 7374 796c 653d 2273 7472 6f6b  14" style="strok
 00003740: 653a 2023 3030 3030 3030 3b20 7374 726f  e: #000000; stro
 00003750: 6b65 2d77 6964 7468 3a20 302e 3822 2f3e  ke-width: 0.8"/>
 00003760: 0a20 2020 2020 203c 2f67 3e0a 2020 2020  .      </g>.    
 00003770: 203c 2f67 3e0a 2020 2020 203c 6720 6964   </g>.     <g id
 00003780: 3d22 7465 7874 5f37 223e 0a20 2020 2020  ="text_7">.     
@@ -970,15 +970,15 @@
 00003c90: 3931 3431 222f 3e0a 2020 2020 2020 3c2f  9141"/>.      </
 00003ca0: 673e 0a20 2020 2020 3c2f 673e 0a20 2020  g>.     </g>.   
 00003cb0: 203c 2f67 3e0a 2020 2020 3c67 2069 643d   </g>.    <g id=
 00003cc0: 2278 7469 636b 5f38 223e 0a20 2020 2020  "xtick_8">.     
 00003cd0: 3c67 2069 643d 226c 696e 6532 645f 3822  <g id="line2d_8"
 00003ce0: 3e0a 2020 2020 2020 3c67 3e0a 2020 2020  >.      <g>.    
 00003cf0: 2020 203c 7573 6520 786c 696e 6b3a 6872     <use xlink:hr
-00003d00: 6566 3d22 236d 3963 3065 6562 6161 6163  ef="#m9c0eebaaac
+00003d00: 6566 3d22 236d 6437 6633 3538 6131 3664  ef="#md7f358a16d
 00003d10: 2220 783d 2231 3733 2e34 3639 3135 3922  " x="173.469159"
 00003d20: 2079 3d22 3230 382e 3939 3837 3134 2220   y="208.998714" 
 00003d30: 7374 796c 653d 2273 7472 6f6b 653a 2023  style="stroke: #
 00003d40: 3030 3030 3030 3b20 7374 726f 6b65 2d77  000000; stroke-w
 00003d50: 6964 7468 3a20 302e 3822 2f3e 0a20 2020  idth: 0.8"/>.   
 00003d60: 2020 203c 2f67 3e0a 2020 2020 203c 2f67     </g>.     </g
 00003d70: 3e0a 2020 2020 203c 6720 6964 3d22 7465  >.     <g id="te
@@ -1005,15 +1005,15 @@
 00003ec0: 3e0a 2020 2020 2020 3c2f 673e 0a20 2020  >.      </g>.   
 00003ed0: 2020 3c2f 673e 0a20 2020 203c 2f67 3e0a    </g>.    </g>.
 00003ee0: 2020 2020 3c67 2069 643d 2278 7469 636b      <g id="xtick
 00003ef0: 5f39 223e 0a20 2020 2020 3c67 2069 643d  _9">.     <g id=
 00003f00: 226c 696e 6532 645f 3922 3e0a 2020 2020  "line2d_9">.    
 00003f10: 2020 3c67 3e0a 2020 2020 2020 203c 7573    <g>.       <us
 00003f20: 6520 786c 696e 6b3a 6872 6566 3d22 236d  e xlink:href="#m
-00003f30: 3963 3065 6562 6161 6163 2220 783d 2231  9c0eebaaac" x="1
+00003f30: 6437 6633 3538 6131 3664 2220 783d 2231  d7f358a16d" x="1
 00003f40: 3930 2e36 3535 3731 3422 2079 3d22 3230  90.655714" y="20
 00003f50: 382e 3939 3837 3134 2220 7374 796c 653d  8.998714" style=
 00003f60: 2273 7472 6f6b 653a 2023 3030 3030 3030  "stroke: #000000
 00003f70: 3b20 7374 726f 6b65 2d77 6964 7468 3a20  ; stroke-width: 
 00003f80: 302e 3822 2f3e 0a20 2020 2020 203c 2f67  0.8"/>.      </g
 00003f90: 3e0a 2020 2020 203c 2f67 3e0a 2020 2020  >.     </g>.    
 00003fa0: 203c 6720 6964 3d22 7465 7874 5f39 223e   <g id="text_9">
@@ -1039,16 +1039,16 @@
 000040e0: 302e 3836 3931 3431 222f 3e0a 2020 2020  0.869141"/>.    
 000040f0: 2020 3c2f 673e 0a20 2020 2020 3c2f 673e    </g>.     </g>
 00004100: 0a20 2020 203c 2f67 3e0a 2020 2020 3c67  .    </g>.    <g
 00004110: 2069 643d 2278 7469 636b 5f31 3022 3e0a   id="xtick_10">.
 00004120: 2020 2020 203c 6720 6964 3d22 6c69 6e65       <g id="line
 00004130: 3264 5f31 3022 3e0a 2020 2020 2020 3c67  2d_10">.      <g
 00004140: 3e0a 2020 2020 2020 203c 7573 6520 786c  >.       <use xl
-00004150: 696e 6b3a 6872 6566 3d22 236d 3963 3065  ink:href="#m9c0e
-00004160: 6562 6161 6163 2220 783d 2232 3037 2e38  ebaaac" x="207.8
+00004150: 696e 6b3a 6872 6566 3d22 236d 6437 6633  ink:href="#md7f3
+00004160: 3538 6131 3664 2220 783d 2232 3037 2e38  58a16d" x="207.8
 00004170: 3432 3236 3822 2079 3d22 3230 382e 3939  42268" y="208.99
 00004180: 3837 3134 2220 7374 796c 653d 2273 7472  8714" style="str
 00004190: 6f6b 653a 2023 3030 3030 3030 3b20 7374  oke: #000000; st
 000041a0: 726f 6b65 2d77 6964 7468 3a20 302e 3822  roke-width: 0.8"
 000041b0: 2f3e 0a20 2020 2020 203c 2f67 3e0a 2020  />.      </g>.  
 000041c0: 2020 203c 2f67 3e0a 2020 2020 203c 6720     </g>.     <g 
 000041d0: 6964 3d22 7465 7874 5f31 3022 3e0a 2020  id="text_10">.  
@@ -1118,16 +1118,16 @@
 000045d0: 3639 3134 3122 2f3e 0a20 2020 2020 203c  69141"/>.      <
 000045e0: 2f67 3e0a 2020 2020 203c 2f67 3e0a 2020  /g>.     </g>.  
 000045f0: 2020 3c2f 673e 0a20 2020 203c 6720 6964    </g>.    <g id
 00004600: 3d22 7874 6963 6b5f 3131 223e 0a20 2020  ="xtick_11">.   
 00004610: 2020 3c67 2069 643d 226c 696e 6532 645f    <g id="line2d_
 00004620: 3131 223e 0a20 2020 2020 203c 673e 0a20  11">.      <g>. 
 00004630: 2020 2020 2020 3c75 7365 2078 6c69 6e6b        <use xlink
-00004640: 3a68 7265 663d 2223 6d39 6330 6565 6261  :href="#m9c0eeba
-00004650: 6161 6322 2078 3d22 3232 352e 3032 3838  aac" x="225.0288
+00004640: 3a68 7265 663d 2223 6d64 3766 3335 3861  :href="#md7f358a
+00004650: 3136 6422 2078 3d22 3232 352e 3032 3838  16d" x="225.0288
 00004660: 3233 2220 793d 2232 3038 2e39 3938 3731  23" y="208.99871
 00004670: 3422 2073 7479 6c65 3d22 7374 726f 6b65  4" style="stroke
 00004680: 3a20 2330 3030 3030 303b 2073 7472 6f6b  : #000000; strok
 00004690: 652d 7769 6474 683a 2030 2e38 222f 3e0a  e-width: 0.8"/>.
 000046a0: 2020 2020 2020 3c2f 673e 0a20 2020 2020        </g>.     
 000046b0: 3c2f 673e 0a20 2020 2020 3c67 2069 643d  </g>.     <g id=
 000046c0: 2274 6578 745f 3131 223e 0a20 2020 2020  "text_11">.     
@@ -1153,15 +1153,15 @@
 00004800: 3431 222f 3e0a 2020 2020 2020 3c2f 673e  41"/>.      </g>
 00004810: 0a20 2020 2020 3c2f 673e 0a20 2020 203c  .     </g>.    <
 00004820: 2f67 3e0a 2020 2020 3c67 2069 643d 2278  /g>.    <g id="x
 00004830: 7469 636b 5f31 3222 3e0a 2020 2020 203c  tick_12">.     <
 00004840: 6720 6964 3d22 6c69 6e65 3264 5f31 3222  g id="line2d_12"
 00004850: 3e0a 2020 2020 2020 3c67 3e0a 2020 2020  >.      <g>.    
 00004860: 2020 203c 7573 6520 786c 696e 6b3a 6872     <use xlink:hr
-00004870: 6566 3d22 236d 3963 3065 6562 6161 6163  ef="#m9c0eebaaac
+00004870: 6566 3d22 236d 6437 6633 3538 6131 3664  ef="#md7f358a16d
 00004880: 2220 783d 2232 3432 2e32 3135 3337 3722  " x="242.215377"
 00004890: 2079 3d22 3230 382e 3939 3837 3134 2220   y="208.998714" 
 000048a0: 7374 796c 653d 2273 7472 6f6b 653a 2023  style="stroke: #
 000048b0: 3030 3030 3030 3b20 7374 726f 6b65 2d77  000000; stroke-w
 000048c0: 6964 7468 3a20 302e 3822 2f3e 0a20 2020  idth: 0.8"/>.   
 000048d0: 2020 203c 2f67 3e0a 2020 2020 203c 2f67     </g>.     </g
 000048e0: 3e0a 2020 2020 203c 6720 6964 3d22 7465  >.     <g id="te
@@ -1188,15 +1188,15 @@
 00004a30: 2f3e 0a20 2020 2020 203c 2f67 3e0a 2020  />.      </g>.  
 00004a40: 2020 203c 2f67 3e0a 2020 2020 3c2f 673e     </g>.    </g>
 00004a50: 0a20 2020 203c 6720 6964 3d22 7874 6963  .    <g id="xtic
 00004a60: 6b5f 3133 223e 0a20 2020 2020 3c67 2069  k_13">.     <g i
 00004a70: 643d 226c 696e 6532 645f 3133 223e 0a20  d="line2d_13">. 
 00004a80: 2020 2020 203c 673e 0a20 2020 2020 2020       <g>.       
 00004a90: 3c75 7365 2078 6c69 6e6b 3a68 7265 663d  <use xlink:href=
-00004aa0: 2223 6d39 6330 6565 6261 6161 6322 2078  "#m9c0eebaaac" x
+00004aa0: 2223 6d64 3766 3335 3861 3136 6422 2078  "#md7f358a16d" x
 00004ab0: 3d22 3235 392e 3430 3139 3332 2220 793d  ="259.401932" y=
 00004ac0: 2232 3038 2e39 3938 3731 3422 2073 7479  "208.998714" sty
 00004ad0: 6c65 3d22 7374 726f 6b65 3a20 2330 3030  le="stroke: #000
 00004ae0: 3030 303b 2073 7472 6f6b 652d 7769 6474  000; stroke-widt
 00004af0: 683a 2030 2e38 222f 3e0a 2020 2020 2020  h: 0.8"/>.      
 00004b00: 3c2f 673e 0a20 2020 2020 3c2f 673e 0a20  </g>.     </g>. 
 00004b10: 2020 2020 3c67 2069 643d 2274 6578 745f      <g id="text_
@@ -1223,15 +1223,15 @@
 00004c60: 2020 2020 2020 3c2f 673e 0a20 2020 2020        </g>.     
 00004c70: 3c2f 673e 0a20 2020 203c 2f67 3e0a 2020  </g>.    </g>.  
 00004c80: 2020 3c67 2069 643d 2278 7469 636b 5f31    <g id="xtick_1
 00004c90: 3422 3e0a 2020 2020 203c 6720 6964 3d22  4">.     <g id="
 00004ca0: 6c69 6e65 3264 5f31 3422 3e0a 2020 2020  line2d_14">.    
 00004cb0: 2020 3c67 3e0a 2020 2020 2020 203c 7573    <g>.       <us
 00004cc0: 6520 786c 696e 6b3a 6872 6566 3d22 236d  e xlink:href="#m
-00004cd0: 3963 3065 6562 6161 6163 2220 783d 2232  9c0eebaaac" x="2
+00004cd0: 6437 6633 3538 6131 3664 2220 783d 2232  d7f358a16d" x="2
 00004ce0: 3736 2e35 3838 3438 3622 2079 3d22 3230  76.588486" y="20
 00004cf0: 382e 3939 3837 3134 2220 7374 796c 653d  8.998714" style=
 00004d00: 2273 7472 6f6b 653a 2023 3030 3030 3030  "stroke: #000000
 00004d10: 3b20 7374 726f 6b65 2d77 6964 7468 3a20  ; stroke-width: 
 00004d20: 302e 3822 2f3e 0a20 2020 2020 203c 2f67  0.8"/>.      </g
 00004d30: 3e0a 2020 2020 203c 2f67 3e0a 2020 2020  >.     </g>.    
 00004d40: 203c 6720 6964 3d22 7465 7874 5f31 3422   <g id="text_14"
@@ -1257,16 +1257,16 @@
 00004e80: 3930 2e38 3639 3134 3122 2f3e 0a20 2020  90.869141"/>.   
 00004e90: 2020 203c 2f67 3e0a 2020 2020 203c 2f67     </g>.     </g
 00004ea0: 3e0a 2020 2020 3c2f 673e 0a20 2020 203c  >.    </g>.    <
 00004eb0: 6720 6964 3d22 7874 6963 6b5f 3135 223e  g id="xtick_15">
 00004ec0: 0a20 2020 2020 3c67 2069 643d 226c 696e  .     <g id="lin
 00004ed0: 6532 645f 3135 223e 0a20 2020 2020 203c  e2d_15">.      <
 00004ee0: 673e 0a20 2020 2020 2020 3c75 7365 2078  g>.       <use x
-00004ef0: 6c69 6e6b 3a68 7265 663d 2223 6d39 6330  link:href="#m9c0
-00004f00: 6565 6261 6161 6322 2078 3d22 3239 332e  eebaaac" x="293.
+00004ef0: 6c69 6e6b 3a68 7265 663d 2223 6d64 3766  link:href="#md7f
+00004f00: 3335 3861 3136 6422 2078 3d22 3239 332e  358a16d" x="293.
 00004f10: 3737 3530 3431 2220 793d 2232 3038 2e39  775041" y="208.9
 00004f20: 3938 3731 3422 2073 7479 6c65 3d22 7374  98714" style="st
 00004f30: 726f 6b65 3a20 2330 3030 3030 303b 2073  roke: #000000; s
 00004f40: 7472 6f6b 652d 7769 6474 683a 2030 2e38  troke-width: 0.8
 00004f50: 222f 3e0a 2020 2020 2020 3c2f 673e 0a20  "/>.      </g>. 
 00004f60: 2020 2020 3c2f 673e 0a20 2020 2020 3c67      </g>.     <g
 00004f70: 2069 643d 2274 6578 745f 3135 223e 0a20   id="text_15">. 
@@ -1292,16 +1292,16 @@
 000050b0: 3639 3134 3122 2f3e 0a20 2020 2020 203c  69141"/>.      <
 000050c0: 2f67 3e0a 2020 2020 203c 2f67 3e0a 2020  /g>.     </g>.  
 000050d0: 2020 3c2f 673e 0a20 2020 203c 6720 6964    </g>.    <g id
 000050e0: 3d22 7874 6963 6b5f 3136 223e 0a20 2020  ="xtick_16">.   
 000050f0: 2020 3c67 2069 643d 226c 696e 6532 645f    <g id="line2d_
 00005100: 3136 223e 0a20 2020 2020 203c 673e 0a20  16">.      <g>. 
 00005110: 2020 2020 2020 3c75 7365 2078 6c69 6e6b        <use xlink
-00005120: 3a68 7265 663d 2223 6d39 6330 6565 6261  :href="#m9c0eeba
-00005130: 6161 6322 2078 3d22 3331 302e 3936 3135  aac" x="310.9615
+00005120: 3a68 7265 663d 2223 6d64 3766 3335 3861  :href="#md7f358a
+00005130: 3136 6422 2078 3d22 3331 302e 3936 3135  16d" x="310.9615
 00005140: 3935 2220 793d 2232 3038 2e39 3938 3731  95" y="208.99871
 00005150: 3422 2073 7479 6c65 3d22 7374 726f 6b65  4" style="stroke
 00005160: 3a20 2330 3030 3030 303b 2073 7472 6f6b  : #000000; strok
 00005170: 652d 7769 6474 683a 2030 2e38 222f 3e0a  e-width: 0.8"/>.
 00005180: 2020 2020 2020 3c2f 673e 0a20 2020 2020        </g>.     
 00005190: 3c2f 673e 0a20 2020 2020 3c67 2069 643d  </g>.     <g id=
 000051a0: 2274 6578 745f 3136 223e 0a20 2020 2020  "text_16">.     
@@ -1327,15 +1327,15 @@
 000052e0: 3431 222f 3e0a 2020 2020 2020 3c2f 673e  41"/>.      </g>
 000052f0: 0a20 2020 2020 3c2f 673e 0a20 2020 203c  .     </g>.    <
 00005300: 2f67 3e0a 2020 2020 3c67 2069 643d 2278  /g>.    <g id="x
 00005310: 7469 636b 5f31 3722 3e0a 2020 2020 203c  tick_17">.     <
 00005320: 6720 6964 3d22 6c69 6e65 3264 5f31 3722  g id="line2d_17"
 00005330: 3e0a 2020 2020 2020 3c67 3e0a 2020 2020  >.      <g>.    
 00005340: 2020 203c 7573 6520 786c 696e 6b3a 6872     <use xlink:hr
-00005350: 6566 3d22 236d 3963 3065 6562 6161 6163  ef="#m9c0eebaaac
+00005350: 6566 3d22 236d 6437 6633 3538 6131 3664  ef="#md7f358a16d
 00005360: 2220 783d 2233 3238 2e31 3438 3135 2220  " x="328.14815" 
 00005370: 793d 2232 3038 2e39 3938 3731 3422 2073  y="208.998714" s
 00005380: 7479 6c65 3d22 7374 726f 6b65 3a20 2330  tyle="stroke: #0
 00005390: 3030 3030 303b 2073 7472 6f6b 652d 7769  00000; stroke-wi
 000053a0: 6474 683a 2030 2e38 222f 3e0a 2020 2020  dth: 0.8"/>.    
 000053b0: 2020 3c2f 673e 0a20 2020 2020 3c2f 673e    </g>.     </g>
 000053c0: 0a20 2020 2020 3c67 2069 643d 2274 6578  .     <g id="tex
@@ -1362,15 +1362,15 @@
 00005510: 3e0a 2020 2020 2020 3c2f 673e 0a20 2020  >.      </g>.   
 00005520: 2020 3c2f 673e 0a20 2020 203c 2f67 3e0a    </g>.    </g>.
 00005530: 2020 2020 3c67 2069 643d 2278 7469 636b      <g id="xtick
 00005540: 5f31 3822 3e0a 2020 2020 203c 6720 6964  _18">.     <g id
 00005550: 3d22 6c69 6e65 3264 5f31 3822 3e0a 2020  ="line2d_18">.  
 00005560: 2020 2020 3c67 3e0a 2020 2020 2020 203c      <g>.       <
 00005570: 7573 6520 786c 696e 6b3a 6872 6566 3d22  use xlink:href="
-00005580: 236d 3963 3065 6562 6161 6163 2220 783d  #m9c0eebaaac" x=
+00005580: 236d 6437 6633 3538 6131 3664 2220 783d  #md7f358a16d" x=
 00005590: 2233 3435 2e33 3334 3730 3522 2079 3d22  "345.334705" y="
 000055a0: 3230 382e 3939 3837 3134 2220 7374 796c  208.998714" styl
 000055b0: 653d 2273 7472 6f6b 653a 2023 3030 3030  e="stroke: #0000
 000055c0: 3030 3b20 7374 726f 6b65 2d77 6964 7468  00; stroke-width
 000055d0: 3a20 302e 3822 2f3e 0a20 2020 2020 203c  : 0.8"/>.      <
 000055e0: 2f67 3e0a 2020 2020 203c 2f67 3e0a 2020  /g>.     </g>.  
 000055f0: 2020 203c 6720 6964 3d22 7465 7874 5f31     <g id="text_1
@@ -1396,16 +1396,16 @@
 00005730: 2231 3930 2e38 3639 3134 3122 2f3e 0a20  "190.869141"/>. 
 00005740: 2020 2020 203c 2f67 3e0a 2020 2020 203c       </g>.     <
 00005750: 2f67 3e0a 2020 2020 3c2f 673e 0a20 2020  /g>.    </g>.   
 00005760: 203c 6720 6964 3d22 7874 6963 6b5f 3139   <g id="xtick_19
 00005770: 223e 0a20 2020 2020 3c67 2069 643d 226c  ">.     <g id="l
 00005780: 696e 6532 645f 3139 223e 0a20 2020 2020  ine2d_19">.     
 00005790: 203c 673e 0a20 2020 2020 2020 3c75 7365   <g>.       <use
-000057a0: 2078 6c69 6e6b 3a68 7265 663d 2223 6d39   xlink:href="#m9
-000057b0: 6330 6565 6261 6161 6322 2078 3d22 3336  c0eebaaac" x="36
+000057a0: 2078 6c69 6e6b 3a68 7265 663d 2223 6d64   xlink:href="#md
+000057b0: 3766 3335 3861 3136 6422 2078 3d22 3336  7f358a16d" x="36
 000057c0: 322e 3532 3132 3539 2220 793d 2232 3038  2.521259" y="208
 000057d0: 2e39 3938 3731 3422 2073 7479 6c65 3d22  .998714" style="
 000057e0: 7374 726f 6b65 3a20 2330 3030 3030 303b  stroke: #000000;
 000057f0: 2073 7472 6f6b 652d 7769 6474 683a 2030   stroke-width: 0
 00005800: 2e38 222f 3e0a 2020 2020 2020 3c2f 673e  .8"/>.      </g>
 00005810: 0a20 2020 2020 3c2f 673e 0a20 2020 2020  .     </g>.     
 00005820: 3c67 2069 643d 2274 6578 745f 3139 223e  <g id="text_19">
@@ -1431,16 +1431,16 @@
 00005960: 302e 3836 3931 3431 222f 3e0a 2020 2020  0.869141"/>.    
 00005970: 2020 3c2f 673e 0a20 2020 2020 3c2f 673e    </g>.     </g>
 00005980: 0a20 2020 203c 2f67 3e0a 2020 2020 3c67  .    </g>.    <g
 00005990: 2069 643d 2278 7469 636b 5f32 3022 3e0a   id="xtick_20">.
 000059a0: 2020 2020 203c 6720 6964 3d22 6c69 6e65       <g id="line
 000059b0: 3264 5f32 3022 3e0a 2020 2020 2020 3c67  2d_20">.      <g
 000059c0: 3e0a 2020 2020 2020 203c 7573 6520 786c  >.       <use xl
-000059d0: 696e 6b3a 6872 6566 3d22 236d 3963 3065  ink:href="#m9c0e
-000059e0: 6562 6161 6163 2220 783d 2233 3739 2e37  ebaaac" x="379.7
+000059d0: 696e 6b3a 6872 6566 3d22 236d 6437 6633  ink:href="#md7f3
+000059e0: 3538 6131 3664 2220 783d 2233 3739 2e37  58a16d" x="379.7
 000059f0: 3037 3831 3422 2079 3d22 3230 382e 3939  07814" y="208.99
 00005a00: 3837 3134 2220 7374 796c 653d 2273 7472  8714" style="str
 00005a10: 6f6b 653a 2023 3030 3030 3030 3b20 7374  oke: #000000; st
 00005a20: 726f 6b65 2d77 6964 7468 3a20 302e 3822  roke-width: 0.8"
 00005a30: 2f3e 0a20 2020 2020 203c 2f67 3e0a 2020  />.      </g>.  
 00005a40: 2020 203c 2f67 3e0a 2020 2020 203c 6720     </g>.     <g 
 00005a50: 6964 3d22 7465 7874 5f32 3022 3e0a 2020  id="text_20">.  
@@ -1466,16 +1466,16 @@
 00005b90: 3639 3134 3122 2f3e 0a20 2020 2020 203c  69141"/>.      <
 00005ba0: 2f67 3e0a 2020 2020 203c 2f67 3e0a 2020  /g>.     </g>.  
 00005bb0: 2020 3c2f 673e 0a20 2020 203c 6720 6964    </g>.    <g id
 00005bc0: 3d22 7874 6963 6b5f 3231 223e 0a20 2020  ="xtick_21">.   
 00005bd0: 2020 3c67 2069 643d 226c 696e 6532 645f    <g id="line2d_
 00005be0: 3231 223e 0a20 2020 2020 203c 673e 0a20  21">.      <g>. 
 00005bf0: 2020 2020 2020 3c75 7365 2078 6c69 6e6b        <use xlink
-00005c00: 3a68 7265 663d 2223 6d39 6330 6565 6261  :href="#m9c0eeba
-00005c10: 6161 6322 2078 3d22 3339 362e 3839 3433  aac" x="396.8943
+00005c00: 3a68 7265 663d 2223 6d64 3766 3335 3861  :href="#md7f358a
+00005c10: 3136 6422 2078 3d22 3339 362e 3839 3433  16d" x="396.8943
 00005c20: 3638 2220 793d 2232 3038 2e39 3938 3731  68" y="208.99871
 00005c30: 3422 2073 7479 6c65 3d22 7374 726f 6b65  4" style="stroke
 00005c40: 3a20 2330 3030 3030 303b 2073 7472 6f6b  : #000000; strok
 00005c50: 652d 7769 6474 683a 2030 2e38 222f 3e0a  e-width: 0.8"/>.
 00005c60: 2020 2020 2020 3c2f 673e 0a20 2020 2020        </g>.     
 00005c70: 3c2f 673e 0a20 2020 2020 3c67 2069 643d  </g>.     <g id=
 00005c80: 2274 6578 745f 3231 223e 0a20 2020 2020  "text_21">.     
@@ -1501,15 +1501,15 @@
 00005dc0: 3431 222f 3e0a 2020 2020 2020 3c2f 673e  41"/>.      </g>
 00005dd0: 0a20 2020 2020 3c2f 673e 0a20 2020 203c  .     </g>.    <
 00005de0: 2f67 3e0a 2020 2020 3c67 2069 643d 2278  /g>.    <g id="x
 00005df0: 7469 636b 5f32 3222 3e0a 2020 2020 203c  tick_22">.     <
 00005e00: 6720 6964 3d22 6c69 6e65 3264 5f32 3222  g id="line2d_22"
 00005e10: 3e0a 2020 2020 2020 3c67 3e0a 2020 2020  >.      <g>.    
 00005e20: 2020 203c 7573 6520 786c 696e 6b3a 6872     <use xlink:hr
-00005e30: 6566 3d22 236d 3963 3065 6562 6161 6163  ef="#m9c0eebaaac
+00005e30: 6566 3d22 236d 6437 6633 3538 6131 3664  ef="#md7f358a16d
 00005e40: 2220 783d 2234 3134 2e30 3830 3932 3322  " x="414.080923"
 00005e50: 2079 3d22 3230 382e 3939 3837 3134 2220   y="208.998714" 
 00005e60: 7374 796c 653d 2273 7472 6f6b 653a 2023  style="stroke: #
 00005e70: 3030 3030 3030 3b20 7374 726f 6b65 2d77  000000; stroke-w
 00005e80: 6964 7468 3a20 302e 3822 2f3e 0a20 2020  idth: 0.8"/>.   
 00005e90: 2020 203c 2f67 3e0a 2020 2020 203c 2f67     </g>.     </g
 00005ea0: 3e0a 2020 2020 203c 6720 6964 3d22 7465  >.     <g id="te
@@ -1536,15 +1536,15 @@
 00005ff0: 2f3e 0a20 2020 2020 203c 2f67 3e0a 2020  />.      </g>.  
 00006000: 2020 203c 2f67 3e0a 2020 2020 3c2f 673e     </g>.    </g>
 00006010: 0a20 2020 203c 6720 6964 3d22 7874 6963  .    <g id="xtic
 00006020: 6b5f 3233 223e 0a20 2020 2020 3c67 2069  k_23">.     <g i
 00006030: 643d 226c 696e 6532 645f 3233 223e 0a20  d="line2d_23">. 
 00006040: 2020 2020 203c 673e 0a20 2020 2020 2020       <g>.       
 00006050: 3c75 7365 2078 6c69 6e6b 3a68 7265 663d  <use xlink:href=
-00006060: 2223 6d39 6330 6565 6261 6161 6322 2078  "#m9c0eebaaac" x
+00006060: 2223 6d64 3766 3335 3861 3136 6422 2078  "#md7f358a16d" x
 00006070: 3d22 3433 312e 3236 3734 3737 2220 793d  ="431.267477" y=
 00006080: 2232 3038 2e39 3938 3731 3422 2073 7479  "208.998714" sty
 00006090: 6c65 3d22 7374 726f 6b65 3a20 2330 3030  le="stroke: #000
 000060a0: 3030 303b 2073 7472 6f6b 652d 7769 6474  000; stroke-widt
 000060b0: 683a 2030 2e38 222f 3e0a 2020 2020 2020  h: 0.8"/>.      
 000060c0: 3c2f 673e 0a20 2020 2020 3c2f 673e 0a20  </g>.     </g>. 
 000060d0: 2020 2020 3c67 2069 643d 2274 6578 745f      <g id="text_
@@ -1571,15 +1571,15 @@
 00006220: 2020 2020 2020 3c2f 673e 0a20 2020 2020        </g>.     
 00006230: 3c2f 673e 0a20 2020 203c 2f67 3e0a 2020  </g>.    </g>.  
 00006240: 2020 3c67 2069 643d 2278 7469 636b 5f32    <g id="xtick_2
 00006250: 3422 3e0a 2020 2020 203c 6720 6964 3d22  4">.     <g id="
 00006260: 6c69 6e65 3264 5f32 3422 3e0a 2020 2020  line2d_24">.    
 00006270: 2020 3c67 3e0a 2020 2020 2020 203c 7573    <g>.       <us
 00006280: 6520 786c 696e 6b3a 6872 6566 3d22 236d  e xlink:href="#m
-00006290: 3963 3065 6562 6161 6163 2220 783d 2234  9c0eebaaac" x="4
+00006290: 6437 6633 3538 6131 3664 2220 783d 2234  d7f358a16d" x="4
 000062a0: 3438 2e34 3534 3033 3222 2079 3d22 3230  48.454032" y="20
 000062b0: 382e 3939 3837 3134 2220 7374 796c 653d  8.998714" style=
 000062c0: 2273 7472 6f6b 653a 2023 3030 3030 3030  "stroke: #000000
 000062d0: 3b20 7374 726f 6b65 2d77 6964 7468 3a20  ; stroke-width: 
 000062e0: 302e 3822 2f3e 0a20 2020 2020 203c 2f67  0.8"/>.      </g
 000062f0: 3e0a 2020 2020 203c 2f67 3e0a 2020 2020  >.     </g>.    
 00006300: 203c 6720 6964 3d22 7465 7874 5f32 3422   <g id="text_24"
@@ -1605,16 +1605,16 @@
 00006440: 3930 2e38 3639 3134 3122 2f3e 0a20 2020  90.869141"/>.   
 00006450: 2020 203c 2f67 3e0a 2020 2020 203c 2f67     </g>.     </g
 00006460: 3e0a 2020 2020 3c2f 673e 0a20 2020 203c  >.    </g>.    <
 00006470: 6720 6964 3d22 7874 6963 6b5f 3235 223e  g id="xtick_25">
 00006480: 0a20 2020 2020 3c67 2069 643d 226c 696e  .     <g id="lin
 00006490: 6532 645f 3235 223e 0a20 2020 2020 203c  e2d_25">.      <
 000064a0: 673e 0a20 2020 2020 2020 3c75 7365 2078  g>.       <use x
-000064b0: 6c69 6e6b 3a68 7265 663d 2223 6d39 6330  link:href="#m9c0
-000064c0: 6565 6261 6161 6322 2078 3d22 3436 352e  eebaaac" x="465.
+000064b0: 6c69 6e6b 3a68 7265 663d 2223 6d64 3766  link:href="#md7f
+000064c0: 3335 3861 3136 6422 2078 3d22 3436 352e  358a16d" x="465.
 000064d0: 3634 3035 3836 2220 793d 2232 3038 2e39  640586" y="208.9
 000064e0: 3938 3731 3422 2073 7479 6c65 3d22 7374  98714" style="st
 000064f0: 726f 6b65 3a20 2330 3030 3030 303b 2073  roke: #000000; s
 00006500: 7472 6f6b 652d 7769 6474 683a 2030 2e38  troke-width: 0.8
 00006510: 222f 3e0a 2020 2020 2020 3c2f 673e 0a20  "/>.      </g>. 
 00006520: 2020 2020 3c2f 673e 0a20 2020 2020 3c67      </g>.     <g
 00006530: 2069 643d 2274 6578 745f 3235 223e 0a20   id="text_25">. 
@@ -1640,16 +1640,16 @@
 00006670: 3836 3931 3431 222f 3e0a 2020 2020 2020  869141"/>.      
 00006680: 3c2f 673e 0a20 2020 2020 3c2f 673e 0a20  </g>.     </g>. 
 00006690: 2020 203c 2f67 3e0a 2020 2020 3c67 2069     </g>.    <g i
 000066a0: 643d 2278 7469 636b 5f32 3622 3e0a 2020  d="xtick_26">.  
 000066b0: 2020 203c 6720 6964 3d22 6c69 6e65 3264     <g id="line2d
 000066c0: 5f32 3622 3e0a 2020 2020 2020 3c67 3e0a  _26">.      <g>.
 000066d0: 2020 2020 2020 203c 7573 6520 786c 696e         <use xlin
-000066e0: 6b3a 6872 6566 3d22 236d 3963 3065 6562  k:href="#m9c0eeb
-000066f0: 6161 6163 2220 783d 2234 3832 2e38 3237  aaac" x="482.827
+000066e0: 6b3a 6872 6566 3d22 236d 6437 6633 3538  k:href="#md7f358
+000066f0: 6131 3664 2220 783d 2234 3832 2e38 3237  a16d" x="482.827
 00006700: 3134 3122 2079 3d22 3230 382e 3939 3837  141" y="208.9987
 00006710: 3134 2220 7374 796c 653d 2273 7472 6f6b  14" style="strok
 00006720: 653a 2023 3030 3030 3030 3b20 7374 726f  e: #000000; stro
 00006730: 6b65 2d77 6964 7468 3a20 302e 3822 2f3e  ke-width: 0.8"/>
 00006740: 0a20 2020 2020 203c 2f67 3e0a 2020 2020  .      </g>.    
 00006750: 203c 2f67 3e0a 2020 2020 203c 6720 6964   </g>.     <g id
 00006760: 3d22 7465 7874 5f32 3622 3e0a 2020 2020  ="text_26">.    
@@ -1675,15 +1675,15 @@
 000068a0: 3431 222f 3e0a 2020 2020 2020 3c2f 673e  41"/>.      </g>
 000068b0: 0a20 2020 2020 3c2f 673e 0a20 2020 203c  .     </g>.    <
 000068c0: 2f67 3e0a 2020 2020 3c67 2069 643d 2278  /g>.    <g id="x
 000068d0: 7469 636b 5f32 3722 3e0a 2020 2020 203c  tick_27">.     <
 000068e0: 6720 6964 3d22 6c69 6e65 3264 5f32 3722  g id="line2d_27"
 000068f0: 3e0a 2020 2020 2020 3c67 3e0a 2020 2020  >.      <g>.    
 00006900: 2020 203c 7573 6520 786c 696e 6b3a 6872     <use xlink:hr
-00006910: 6566 3d22 236d 3963 3065 6562 6161 6163  ef="#m9c0eebaaac
+00006910: 6566 3d22 236d 6437 6633 3538 6131 3664  ef="#md7f358a16d
 00006920: 2220 783d 2235 3030 2e30 3133 3639 3522  " x="500.013695"
 00006930: 2079 3d22 3230 382e 3939 3837 3134 2220   y="208.998714" 
 00006940: 7374 796c 653d 2273 7472 6f6b 653a 2023  style="stroke: #
 00006950: 3030 3030 3030 3b20 7374 726f 6b65 2d77  000000; stroke-w
 00006960: 6964 7468 3a20 302e 3822 2f3e 0a20 2020  idth: 0.8"/>.   
 00006970: 2020 203c 2f67 3e0a 2020 2020 203c 2f67     </g>.     </g
 00006980: 3e0a 2020 2020 203c 6720 6964 3d22 7465  >.     <g id="te
@@ -1710,15 +1710,15 @@
 00006ad0: 2f3e 0a20 2020 2020 203c 2f67 3e0a 2020  />.      </g>.  
 00006ae0: 2020 203c 2f67 3e0a 2020 2020 3c2f 673e     </g>.    </g>
 00006af0: 0a20 2020 203c 6720 6964 3d22 7874 6963  .    <g id="xtic
 00006b00: 6b5f 3238 223e 0a20 2020 2020 3c67 2069  k_28">.     <g i
 00006b10: 643d 226c 696e 6532 645f 3238 223e 0a20  d="line2d_28">. 
 00006b20: 2020 2020 203c 673e 0a20 2020 2020 2020       <g>.       
 00006b30: 3c75 7365 2078 6c69 6e6b 3a68 7265 663d  <use xlink:href=
-00006b40: 2223 6d39 6330 6565 6261 6161 6322 2078  "#m9c0eebaaac" x
+00006b40: 2223 6d64 3766 3335 3861 3136 6422 2078  "#md7f358a16d" x
 00006b50: 3d22 3531 372e 3230 3032 3522 2079 3d22  ="517.20025" y="
 00006b60: 3230 382e 3939 3837 3134 2220 7374 796c  208.998714" styl
 00006b70: 653d 2273 7472 6f6b 653a 2023 3030 3030  e="stroke: #0000
 00006b80: 3030 3b20 7374 726f 6b65 2d77 6964 7468  00; stroke-width
 00006b90: 3a20 302e 3822 2f3e 0a20 2020 2020 203c  : 0.8"/>.      <
 00006ba0: 2f67 3e0a 2020 2020 203c 2f67 3e0a 2020  /g>.     </g>.  
 00006bb0: 2020 203c 6720 6964 3d22 7465 7874 5f32     <g id="text_2
@@ -1744,16 +1744,16 @@
 00006cf0: 2231 3930 2e38 3639 3134 3122 2f3e 0a20  "190.869141"/>. 
 00006d00: 2020 2020 203c 2f67 3e0a 2020 2020 203c       </g>.     <
 00006d10: 2f67 3e0a 2020 2020 3c2f 673e 0a20 2020  /g>.    </g>.   
 00006d20: 203c 6720 6964 3d22 7874 6963 6b5f 3239   <g id="xtick_29
 00006d30: 223e 0a20 2020 2020 3c67 2069 643d 226c  ">.     <g id="l
 00006d40: 696e 6532 645f 3239 223e 0a20 2020 2020  ine2d_29">.     
 00006d50: 203c 673e 0a20 2020 2020 2020 3c75 7365   <g>.       <use
-00006d60: 2078 6c69 6e6b 3a68 7265 663d 2223 6d39   xlink:href="#m9
-00006d70: 6330 6565 6261 6161 6322 2078 3d22 3533  c0eebaaac" x="53
+00006d60: 2078 6c69 6e6b 3a68 7265 663d 2223 6d64   xlink:href="#md
+00006d70: 3766 3335 3861 3136 6422 2078 3d22 3533  7f358a16d" x="53
 00006d80: 342e 3338 3638 3035 2220 793d 2232 3038  4.386805" y="208
 00006d90: 2e39 3938 3731 3422 2073 7479 6c65 3d22  .998714" style="
 00006da0: 7374 726f 6b65 3a20 2330 3030 3030 303b  stroke: #000000;
 00006db0: 2073 7472 6f6b 652d 7769 6474 683a 2030   stroke-width: 0
 00006dc0: 2e38 222f 3e0a 2020 2020 2020 3c2f 673e  .8"/>.      </g>
 00006dd0: 0a20 2020 2020 3c2f 673e 0a20 2020 2020  .     </g>.     
 00006de0: 3c67 2069 643d 2274 6578 745f 3239 223e  <g id="text_29">
@@ -1779,16 +1779,16 @@
 00006f20: 302e 3836 3931 3431 222f 3e0a 2020 2020  0.869141"/>.    
 00006f30: 2020 3c2f 673e 0a20 2020 2020 3c2f 673e    </g>.     </g>
 00006f40: 0a20 2020 203c 2f67 3e0a 2020 2020 3c67  .    </g>.    <g
 00006f50: 2069 643d 2278 7469 636b 5f33 3022 3e0a   id="xtick_30">.
 00006f60: 2020 2020 203c 6720 6964 3d22 6c69 6e65       <g id="line
 00006f70: 3264 5f33 3022 3e0a 2020 2020 2020 3c67  2d_30">.      <g
 00006f80: 3e0a 2020 2020 2020 203c 7573 6520 786c  >.       <use xl
-00006f90: 696e 6b3a 6872 6566 3d22 236d 3963 3065  ink:href="#m9c0e
-00006fa0: 6562 6161 6163 2220 783d 2235 3531 2e35  ebaaac" x="551.5
+00006f90: 696e 6b3a 6872 6566 3d22 236d 6437 6633  ink:href="#md7f3
+00006fa0: 3538 6131 3664 2220 783d 2235 3531 2e35  58a16d" x="551.5
 00006fb0: 3733 3335 3922 2079 3d22 3230 382e 3939  73359" y="208.99
 00006fc0: 3837 3134 2220 7374 796c 653d 2273 7472  8714" style="str
 00006fd0: 6f6b 653a 2023 3030 3030 3030 3b20 7374  oke: #000000; st
 00006fe0: 726f 6b65 2d77 6964 7468 3a20 302e 3822  roke-width: 0.8"
 00006ff0: 2f3e 0a20 2020 2020 203c 2f67 3e0a 2020  />.      </g>.  
 00007000: 2020 203c 2f67 3e0a 2020 2020 203c 6720     </g>.     <g 
 00007010: 6964 3d22 7465 7874 5f33 3022 3e0a 2020  id="text_30">.  
@@ -1816,24 +1816,24 @@
 00007170: 2020 3c2f 673e 0a20 2020 3c2f 673e 0a20    </g>.   </g>. 
 00007180: 2020 3c67 2069 643d 226d 6174 706c 6f74    <g id="matplot
 00007190: 6c69 622e 6178 6973 5f32 223e 0a20 2020  lib.axis_2">.   
 000071a0: 203c 6720 6964 3d22 7974 6963 6b5f 3122   <g id="ytick_1"
 000071b0: 3e0a 2020 2020 203c 6720 6964 3d22 6c69  >.     <g id="li
 000071c0: 6e65 3264 5f33 3122 3e0a 2020 2020 2020  ne2d_31">.      
 000071d0: 3c64 6566 733e 0a20 2020 2020 2020 3c70  <defs>.       <p
-000071e0: 6174 6820 6964 3d22 6d65 6138 6263 3265  ath id="mea8bc2e
-000071f0: 3438 3022 2064 3d22 4d20 3020 3020 0a4c  480" d="M 0 0 .L
+000071e0: 6174 6820 6964 3d22 6d30 3034 6533 3533  ath id="m004e353
+000071f0: 3338 3922 2064 3d22 4d20 3020 3020 0a4c  389" d="M 0 0 .L
 00007200: 202d 332e 3520 3020 0a22 2073 7479 6c65   -3.5 0 ." style
 00007210: 3d22 7374 726f 6b65 3a20 2330 3030 3030  ="stroke: #00000
 00007220: 303b 2073 7472 6f6b 652d 7769 6474 683a  0; stroke-width:
 00007230: 2030 2e38 222f 3e0a 2020 2020 2020 3c2f   0.8"/>.      </
 00007240: 6465 6673 3e0a 2020 2020 2020 3c67 3e0a  defs>.      <g>.
 00007250: 2020 2020 2020 203c 7573 6520 786c 696e         <use xlin
-00007260: 6b3a 6872 6566 3d22 236d 6561 3862 6332  k:href="#mea8bc2
-00007270: 6534 3830 2220 783d 2234 342e 3537 2220  e480" x="44.57" 
+00007260: 6b3a 6872 6566 3d22 236d 3030 3465 3335  k:href="#m004e35
+00007270: 3333 3839 2220 783d 2234 342e 3537 2220  3389" x="44.57" 
 00007280: 793d 2232 3038 2e39 3938 3731 3422 2073  y="208.998714" s
 00007290: 7479 6c65 3d22 7374 726f 6b65 3a20 2330  tyle="stroke: #0
 000072a0: 3030 3030 303b 2073 7472 6f6b 652d 7769  00000; stroke-wi
 000072b0: 6474 683a 2030 2e38 222f 3e0a 2020 2020  dth: 0.8"/>.    
 000072c0: 2020 3c2f 673e 0a20 2020 2020 3c2f 673e    </g>.     </g>
 000072d0: 0a20 2020 2020 3c67 2069 643d 2274 6578  .     <g id="tex
 000072e0: 745f 3331 223e 0a20 2020 2020 203c 212d  t_31">.      <!-
@@ -1847,15 +1847,15 @@
 00007360: 3330 222f 3e0a 2020 2020 2020 3c2f 673e  30"/>.      </g>
 00007370: 0a20 2020 2020 3c2f 673e 0a20 2020 203c  .     </g>.    <
 00007380: 2f67 3e0a 2020 2020 3c67 2069 643d 2279  /g>.    <g id="y
 00007390: 7469 636b 5f32 223e 0a20 2020 2020 3c67  tick_2">.     <g
 000073a0: 2069 643d 226c 696e 6532 645f 3332 223e   id="line2d_32">
 000073b0: 0a20 2020 2020 203c 673e 0a20 2020 2020  .      <g>.     
 000073c0: 2020 3c75 7365 2078 6c69 6e6b 3a68 7265    <use xlink:hre
-000073d0: 663d 2223 6d65 6138 6263 3265 3438 3022  f="#mea8bc2e480"
+000073d0: 663d 2223 6d30 3034 6533 3533 3338 3922  f="#m004e353389"
 000073e0: 2078 3d22 3434 2e35 3722 2079 3d22 3138   x="44.57" y="18
 000073f0: 332e 3439 3138 3932 2220 7374 796c 653d  3.491892" style=
 00007400: 2273 7472 6f6b 653a 2023 3030 3030 3030  "stroke: #000000
 00007410: 3b20 7374 726f 6b65 2d77 6964 7468 3a20  ; stroke-width: 
 00007420: 302e 3822 2f3e 0a20 2020 2020 203c 2f67  0.8"/>.      </g
 00007430: 3e0a 2020 2020 203c 2f67 3e0a 2020 2020  >.     </g>.    
 00007440: 203c 6720 6964 3d22 7465 7874 5f33 3222   <g id="text_32"
@@ -1869,16 +1869,16 @@
 000074c0: 656a 6156 7553 616e 732d 3335 222f 3e0a  ejaVuSans-35"/>.
 000074d0: 2020 2020 2020 3c2f 673e 0a20 2020 2020        </g>.     
 000074e0: 3c2f 673e 0a20 2020 203c 2f67 3e0a 2020  </g>.    </g>.  
 000074f0: 2020 3c67 2069 643d 2279 7469 636b 5f33    <g id="ytick_3
 00007500: 223e 0a20 2020 2020 3c67 2069 643d 226c  ">.     <g id="l
 00007510: 696e 6532 645f 3333 223e 0a20 2020 2020  ine2d_33">.     
 00007520: 203c 673e 0a20 2020 2020 2020 3c75 7365   <g>.       <use
-00007530: 2078 6c69 6e6b 3a68 7265 663d 2223 6d65   xlink:href="#me
-00007540: 6138 6263 3265 3438 3022 2078 3d22 3434  a8bc2e480" x="44
+00007530: 2078 6c69 6e6b 3a68 7265 663d 2223 6d30   xlink:href="#m0
+00007540: 3034 6533 3533 3338 3922 2078 3d22 3434  04e353389" x="44
 00007550: 2e35 3722 2079 3d22 3135 372e 3938 3530  .57" y="157.9850
 00007560: 3639 2220 7374 796c 653d 2273 7472 6f6b  69" style="strok
 00007570: 653a 2023 3030 3030 3030 3b20 7374 726f  e: #000000; stro
 00007580: 6b65 2d77 6964 7468 3a20 302e 3822 2f3e  ke-width: 0.8"/>
 00007590: 0a20 2020 2020 203c 2f67 3e0a 2020 2020  .      </g>.    
 000075a0: 203c 2f67 3e0a 2020 2020 203c 6720 6964   </g>.     <g id
 000075b0: 3d22 7465 7874 5f33 3322 3e0a 2020 2020  ="text_33">.    
@@ -1896,15 +1896,15 @@
 00007670: 2f3e 0a20 2020 2020 203c 2f67 3e0a 2020  />.      </g>.  
 00007680: 2020 203c 2f67 3e0a 2020 2020 3c2f 673e     </g>.    </g>
 00007690: 0a20 2020 203c 6720 6964 3d22 7974 6963  .    <g id="ytic
 000076a0: 6b5f 3422 3e0a 2020 2020 203c 6720 6964  k_4">.     <g id
 000076b0: 3d22 6c69 6e65 3264 5f33 3422 3e0a 2020  ="line2d_34">.  
 000076c0: 2020 2020 3c67 3e0a 2020 2020 2020 203c      <g>.       <
 000076d0: 7573 6520 786c 696e 6b3a 6872 6566 3d22  use xlink:href="
-000076e0: 236d 6561 3862 6332 6534 3830 2220 783d  #mea8bc2e480" x=
+000076e0: 236d 3030 3465 3335 3333 3839 2220 783d  #m004e353389" x=
 000076f0: 2234 342e 3537 2220 793d 2231 3332 2e34  "44.57" y="132.4
 00007700: 3738 3234 3622 2073 7479 6c65 3d22 7374  78246" style="st
 00007710: 726f 6b65 3a20 2330 3030 3030 303b 2073  roke: #000000; s
 00007720: 7472 6f6b 652d 7769 6474 683a 2030 2e38  troke-width: 0.8
 00007730: 222f 3e0a 2020 2020 2020 3c2f 673e 0a20  "/>.      </g>. 
 00007740: 2020 2020 3c2f 673e 0a20 2020 2020 3c67      </g>.     <g
 00007750: 2069 643d 2274 6578 745f 3334 223e 0a20   id="text_34">. 
@@ -1922,15 +1922,15 @@
 00007810: 3437 222f 3e0a 2020 2020 2020 3c2f 673e  47"/>.      </g>
 00007820: 0a20 2020 2020 3c2f 673e 0a20 2020 203c  .     </g>.    <
 00007830: 2f67 3e0a 2020 2020 3c67 2069 643d 2279  /g>.    <g id="y
 00007840: 7469 636b 5f35 223e 0a20 2020 2020 3c67  tick_5">.     <g
 00007850: 2069 643d 226c 696e 6532 645f 3335 223e   id="line2d_35">
 00007860: 0a20 2020 2020 203c 673e 0a20 2020 2020  .      <g>.     
 00007870: 2020 3c75 7365 2078 6c69 6e6b 3a68 7265    <use xlink:hre
-00007880: 663d 2223 6d65 6138 6263 3265 3438 3022  f="#mea8bc2e480"
+00007880: 663d 2223 6d30 3034 6533 3533 3338 3922  f="#m004e353389"
 00007890: 2078 3d22 3434 2e35 3722 2079 3d22 3130   x="44.57" y="10
 000078a0: 362e 3937 3134 3233 2220 7374 796c 653d  6.971423" style=
 000078b0: 2273 7472 6f6b 653a 2023 3030 3030 3030  "stroke: #000000
 000078c0: 3b20 7374 726f 6b65 2d77 6964 7468 3a20  ; stroke-width: 
 000078d0: 302e 3822 2f3e 0a20 2020 2020 203c 2f67  0.8"/>.      </g
 000078e0: 3e0a 2020 2020 203c 2f67 3e0a 2020 2020  >.     </g>.    
 000078f0: 203c 6720 6964 3d22 7465 7874 5f33 3522   <g id="text_35"
@@ -1948,16 +1948,16 @@
 000079b0: 3233 3034 3722 2f3e 0a20 2020 2020 203c  23047"/>.      <
 000079c0: 2f67 3e0a 2020 2020 203c 2f67 3e0a 2020  /g>.     </g>.  
 000079d0: 2020 3c2f 673e 0a20 2020 203c 6720 6964    </g>.    <g id
 000079e0: 3d22 7974 6963 6b5f 3622 3e0a 2020 2020  ="ytick_6">.    
 000079f0: 203c 6720 6964 3d22 6c69 6e65 3264 5f33   <g id="line2d_3
 00007a00: 3622 3e0a 2020 2020 2020 3c67 3e0a 2020  6">.      <g>.  
 00007a10: 2020 2020 203c 7573 6520 786c 696e 6b3a       <use xlink:
-00007a20: 6872 6566 3d22 236d 6561 3862 6332 6534  href="#mea8bc2e4
-00007a30: 3830 2220 783d 2234 342e 3537 2220 793d  80" x="44.57" y=
+00007a20: 6872 6566 3d22 236d 3030 3465 3335 3333  href="#m004e3533
+00007a30: 3839 2220 783d 2234 342e 3537 2220 793d  89" x="44.57" y=
 00007a40: 2238 312e 3436 3436 3031 2220 7374 796c  "81.464601" styl
 00007a50: 653d 2273 7472 6f6b 653a 2023 3030 3030  e="stroke: #0000
 00007a60: 3030 3b20 7374 726f 6b65 2d77 6964 7468  00; stroke-width
 00007a70: 3a20 302e 3822 2f3e 0a20 2020 2020 203c  : 0.8"/>.      <
 00007a80: 2f67 3e0a 2020 2020 203c 2f67 3e0a 2020  /g>.     </g>.  
 00007a90: 2020 203c 6720 6964 3d22 7465 7874 5f33     <g id="text_3
 00007aa0: 3622 3e0a 2020 2020 2020 3c21 2d2d 2032  6">.      <!-- 2
@@ -1974,16 +1974,16 @@
 00007b50: 3632 3330 3437 222f 3e0a 2020 2020 2020  623047"/>.      
 00007b60: 3c2f 673e 0a20 2020 2020 3c2f 673e 0a20  </g>.     </g>. 
 00007b70: 2020 203c 2f67 3e0a 2020 2020 3c67 2069     </g>.    <g i
 00007b80: 643d 2279 7469 636b 5f37 223e 0a20 2020  d="ytick_7">.   
 00007b90: 2020 3c67 2069 643d 226c 696e 6532 645f    <g id="line2d_
 00007ba0: 3337 223e 0a20 2020 2020 203c 673e 0a20  37">.      <g>. 
 00007bb0: 2020 2020 2020 3c75 7365 2078 6c69 6e6b        <use xlink
-00007bc0: 3a68 7265 663d 2223 6d65 6138 6263 3265  :href="#mea8bc2e
-00007bd0: 3438 3022 2078 3d22 3434 2e35 3722 2079  480" x="44.57" y
+00007bc0: 3a68 7265 663d 2223 6d30 3034 6533 3533  :href="#m004e353
+00007bd0: 3338 3922 2078 3d22 3434 2e35 3722 2079  389" x="44.57" y
 00007be0: 3d22 3535 2e39 3537 3737 3822 2073 7479  ="55.957778" sty
 00007bf0: 6c65 3d22 7374 726f 6b65 3a20 2330 3030  le="stroke: #000
 00007c00: 3030 303b 2073 7472 6f6b 652d 7769 6474  000; stroke-widt
 00007c10: 683a 2030 2e38 222f 3e0a 2020 2020 2020  h: 0.8"/>.      
 00007c20: 3c2f 673e 0a20 2020 2020 3c2f 673e 0a20  </g>.     </g>. 
 00007c30: 2020 2020 3c67 2069 643d 2274 6578 745f      <g id="text_
 00007c40: 3337 223e 0a20 2020 2020 203c 212d 2d20  37">.      <!-- 
@@ -2000,16 +2000,16 @@
 00007cf0: 2e36 3233 3034 3722 2f3e 0a20 2020 2020  .623047"/>.     
 00007d00: 203c 2f67 3e0a 2020 2020 203c 2f67 3e0a   </g>.     </g>.
 00007d10: 2020 2020 3c2f 673e 0a20 2020 203c 6720      </g>.    <g 
 00007d20: 6964 3d22 7974 6963 6b5f 3822 3e0a 2020  id="ytick_8">.  
 00007d30: 2020 203c 6720 6964 3d22 6c69 6e65 3264     <g id="line2d
 00007d40: 5f33 3822 3e0a 2020 2020 2020 3c67 3e0a  _38">.      <g>.
 00007d50: 2020 2020 2020 203c 7573 6520 786c 696e         <use xlin
-00007d60: 6b3a 6872 6566 3d22 236d 6561 3862 6332  k:href="#mea8bc2
-00007d70: 6534 3830 2220 783d 2234 342e 3537 2220  e480" x="44.57" 
+00007d60: 6b3a 6872 6566 3d22 236d 3030 3465 3335  k:href="#m004e35
+00007d70: 3333 3839 2220 783d 2234 342e 3537 2220  3389" x="44.57" 
 00007d80: 793d 2233 302e 3435 3039 3535 2220 7374  y="30.450955" st
 00007d90: 796c 653d 2273 7472 6f6b 653a 2023 3030  yle="stroke: #00
 00007da0: 3030 3030 3b20 7374 726f 6b65 2d77 6964  0000; stroke-wid
 00007db0: 7468 3a20 302e 3822 2f3e 0a20 2020 2020  th: 0.8"/>.     
 00007dc0: 203c 2f67 3e0a 2020 2020 203c 2f67 3e0a   </g>.     </g>.
 00007dd0: 2020 2020 203c 6720 6964 3d22 7465 7874       <g id="text
 00007de0: 5f33 3822 3e0a 2020 2020 2020 3c21 2d2d  _38">.      <!--
@@ -2354,289 +2354,289 @@
 00009310: 6b3a 6872 6566 3d22 2344 656a 6156 7553  k:href="#DejaVuS
 00009320: 616e 732d 3733 2220 783d 2235 3438 2e37  ans-73" x="548.7
 00009330: 3837 3130 3922 2f3e 0a20 2020 2020 3c2f  87109"/>.     </
 00009340: 673e 0a20 2020 203c 2f67 3e0a 2020 203c  g>.    </g>.   <
 00009350: 2f67 3e0a 2020 203c 6720 6964 3d22 6c69  /g>.   <g id="li
 00009360: 6e65 3264 5f33 3922 3e0a 2020 2020 3c70  ne2d_39">.    <p
 00009370: 6174 6820 636c 6970 2d70 6174 683d 2275  ath clip-path="u
-00009380: 726c 2823 7062 6632 6531 3966 3166 3429  rl(#pbf2e19f1f4)
+00009380: 726c 2823 7032 3261 3136 6136 6462 6429  rl(#p22a16a6dbd)
 00009390: 2220 7374 796c 653d 2266 696c 6c3a 206e  " style="fill: n
 000093a0: 6f6e 653b 2073 7472 6f6b 653a 2023 3432  one; stroke: #42
 000093b0: 3432 3432 3b20 7374 726f 6b65 2d77 6964  4242; stroke-wid
 000093c0: 7468 3a20 322e 373b 2073 7472 6f6b 652d  th: 2.7; stroke-
 000093d0: 6c69 6e65 6361 703a 2073 7175 6172 6522  linecap: square"
 000093e0: 2f3e 0a20 2020 3c2f 673e 0a20 2020 3c67  />.   </g>.   <g
 000093f0: 2069 643d 226c 696e 6532 645f 3430 223e   id="line2d_40">
 00009400: 0a20 2020 203c 7061 7468 2063 6c69 702d  .    <path clip-
-00009410: 7061 7468 3d22 7572 6c28 2370 6266 3265  path="url(#pbf2e
-00009420: 3139 6631 6634 2922 2073 7479 6c65 3d22  19f1f4)" style="
+00009410: 7061 7468 3d22 7572 6c28 2370 3232 6131  path="url(#p22a1
+00009420: 3661 3664 6264 2922 2073 7479 6c65 3d22  6a6dbd)" style="
 00009430: 6669 6c6c 3a20 6e6f 6e65 3b20 7374 726f  fill: none; stro
 00009440: 6b65 3a20 2334 3234 3234 323b 2073 7472  ke: #424242; str
 00009450: 6f6b 652d 7769 6474 683a 2032 2e37 3b20  oke-width: 2.7; 
 00009460: 7374 726f 6b65 2d6c 696e 6563 6170 3a20  stroke-linecap: 
 00009470: 7371 7561 7265 222f 3e0a 2020 203c 2f67  square"/>.   </g
 00009480: 3e0a 2020 203c 6720 6964 3d22 6c69 6e65  >.   <g id="line
 00009490: 3264 5f34 3122 3e0a 2020 2020 3c70 6174  2d_41">.    <pat
 000094a0: 6820 636c 6970 2d70 6174 683d 2275 726c  h clip-path="url
-000094b0: 2823 7062 6632 6531 3966 3166 3429 2220  (#pbf2e19f1f4)" 
+000094b0: 2823 7032 3261 3136 6136 6462 6429 2220  (#p22a16a6dbd)" 
 000094c0: 7374 796c 653d 2266 696c 6c3a 206e 6f6e  style="fill: non
 000094d0: 653b 2073 7472 6f6b 653a 2023 3432 3432  e; stroke: #4242
 000094e0: 3432 3b20 7374 726f 6b65 2d77 6964 7468  42; stroke-width
 000094f0: 3a20 322e 373b 2073 7472 6f6b 652d 6c69  : 2.7; stroke-li
 00009500: 6e65 6361 703a 2073 7175 6172 6522 2f3e  necap: square"/>
 00009510: 0a20 2020 3c2f 673e 0a20 2020 3c67 2069  .   </g>.   <g i
 00009520: 643d 226c 696e 6532 645f 3432 223e 0a20  d="line2d_42">. 
 00009530: 2020 203c 7061 7468 2063 6c69 702d 7061     <path clip-pa
-00009540: 7468 3d22 7572 6c28 2370 6266 3265 3139  th="url(#pbf2e19
-00009550: 6631 6634 2922 2073 7479 6c65 3d22 6669  f1f4)" style="fi
+00009540: 7468 3d22 7572 6c28 2370 3232 6131 3661  th="url(#p22a16a
+00009550: 3664 6264 2922 2073 7479 6c65 3d22 6669  6dbd)" style="fi
 00009560: 6c6c 3a20 6e6f 6e65 3b20 7374 726f 6b65  ll: none; stroke
 00009570: 3a20 2334 3234 3234 323b 2073 7472 6f6b  : #424242; strok
 00009580: 652d 7769 6474 683a 2032 2e37 3b20 7374  e-width: 2.7; st
 00009590: 726f 6b65 2d6c 696e 6563 6170 3a20 7371  roke-linecap: sq
 000095a0: 7561 7265 222f 3e0a 2020 203c 2f67 3e0a  uare"/>.   </g>.
 000095b0: 2020 203c 6720 6964 3d22 6c69 6e65 3264     <g id="line2d
 000095c0: 5f34 3322 3e0a 2020 2020 3c70 6174 6820  _43">.    <path 
 000095d0: 636c 6970 2d70 6174 683d 2275 726c 2823  clip-path="url(#
-000095e0: 7062 6632 6531 3966 3166 3429 2220 7374  pbf2e19f1f4)" st
+000095e0: 7032 3261 3136 6136 6462 6429 2220 7374  p22a16a6dbd)" st
 000095f0: 796c 653d 2266 696c 6c3a 206e 6f6e 653b  yle="fill: none;
 00009600: 2073 7472 6f6b 653a 2023 3432 3432 3432   stroke: #424242
 00009610: 3b20 7374 726f 6b65 2d77 6964 7468 3a20  ; stroke-width: 
 00009620: 322e 373b 2073 7472 6f6b 652d 6c69 6e65  2.7; stroke-line
 00009630: 6361 703a 2073 7175 6172 6522 2f3e 0a20  cap: square"/>. 
 00009640: 2020 3c2f 673e 0a20 2020 3c67 2069 643d    </g>.   <g id=
 00009650: 226c 696e 6532 645f 3434 223e 0a20 2020  "line2d_44">.   
 00009660: 203c 7061 7468 2063 6c69 702d 7061 7468   <path clip-path
-00009670: 3d22 7572 6c28 2370 6266 3265 3139 6631  ="url(#pbf2e19f1
-00009680: 6634 2922 2073 7479 6c65 3d22 6669 6c6c  f4)" style="fill
+00009670: 3d22 7572 6c28 2370 3232 6131 3661 3664  ="url(#p22a16a6d
+00009680: 6264 2922 2073 7479 6c65 3d22 6669 6c6c  bd)" style="fill
 00009690: 3a20 6e6f 6e65 3b20 7374 726f 6b65 3a20  : none; stroke: 
 000096a0: 2334 3234 3234 323b 2073 7472 6f6b 652d  #424242; stroke-
 000096b0: 7769 6474 683a 2032 2e37 3b20 7374 726f  width: 2.7; stro
 000096c0: 6b65 2d6c 696e 6563 6170 3a20 7371 7561  ke-linecap: squa
 000096d0: 7265 222f 3e0a 2020 203c 2f67 3e0a 2020  re"/>.   </g>.  
 000096e0: 203c 6720 6964 3d22 6c69 6e65 3264 5f34   <g id="line2d_4
 000096f0: 3522 3e0a 2020 2020 3c70 6174 6820 636c  5">.    <path cl
-00009700: 6970 2d70 6174 683d 2275 726c 2823 7062  ip-path="url(#pb
-00009710: 6632 6531 3966 3166 3429 2220 7374 796c  f2e19f1f4)" styl
+00009700: 6970 2d70 6174 683d 2275 726c 2823 7032  ip-path="url(#p2
+00009710: 3261 3136 6136 6462 6429 2220 7374 796c  2a16a6dbd)" styl
 00009720: 653d 2266 696c 6c3a 206e 6f6e 653b 2073  e="fill: none; s
 00009730: 7472 6f6b 653a 2023 3432 3432 3432 3b20  troke: #424242; 
 00009740: 7374 726f 6b65 2d77 6964 7468 3a20 322e  stroke-width: 2.
 00009750: 373b 2073 7472 6f6b 652d 6c69 6e65 6361  7; stroke-lineca
 00009760: 703a 2073 7175 6172 6522 2f3e 0a20 2020  p: square"/>.   
 00009770: 3c2f 673e 0a20 2020 3c67 2069 643d 226c  </g>.   <g id="l
 00009780: 696e 6532 645f 3436 223e 0a20 2020 203c  ine2d_46">.    <
 00009790: 7061 7468 2063 6c69 702d 7061 7468 3d22  path clip-path="
-000097a0: 7572 6c28 2370 6266 3265 3139 6631 6634  url(#pbf2e19f1f4
+000097a0: 7572 6c28 2370 3232 6131 3661 3664 6264  url(#p22a16a6dbd
 000097b0: 2922 2073 7479 6c65 3d22 6669 6c6c 3a20  )" style="fill: 
 000097c0: 6e6f 6e65 3b20 7374 726f 6b65 3a20 2334  none; stroke: #4
 000097d0: 3234 3234 323b 2073 7472 6f6b 652d 7769  24242; stroke-wi
 000097e0: 6474 683a 2032 2e37 3b20 7374 726f 6b65  dth: 2.7; stroke
 000097f0: 2d6c 696e 6563 6170 3a20 7371 7561 7265  -linecap: square
 00009800: 222f 3e0a 2020 203c 2f67 3e0a 2020 203c  "/>.   </g>.   <
 00009810: 6720 6964 3d22 6c69 6e65 3264 5f34 3722  g id="line2d_47"
 00009820: 3e0a 2020 2020 3c70 6174 6820 636c 6970  >.    <path clip
-00009830: 2d70 6174 683d 2275 726c 2823 7062 6632  -path="url(#pbf2
-00009840: 6531 3966 3166 3429 2220 7374 796c 653d  e19f1f4)" style=
+00009830: 2d70 6174 683d 2275 726c 2823 7032 3261  -path="url(#p22a
+00009840: 3136 6136 6462 6429 2220 7374 796c 653d  16a6dbd)" style=
 00009850: 2266 696c 6c3a 206e 6f6e 653b 2073 7472  "fill: none; str
 00009860: 6f6b 653a 2023 3432 3432 3432 3b20 7374  oke: #424242; st
 00009870: 726f 6b65 2d77 6964 7468 3a20 322e 373b  roke-width: 2.7;
 00009880: 2073 7472 6f6b 652d 6c69 6e65 6361 703a   stroke-linecap:
 00009890: 2073 7175 6172 6522 2f3e 0a20 2020 3c2f   square"/>.   </
 000098a0: 673e 0a20 2020 3c67 2069 643d 226c 696e  g>.   <g id="lin
 000098b0: 6532 645f 3438 223e 0a20 2020 203c 7061  e2d_48">.    <pa
 000098c0: 7468 2063 6c69 702d 7061 7468 3d22 7572  th clip-path="ur
-000098d0: 6c28 2370 6266 3265 3139 6631 6634 2922  l(#pbf2e19f1f4)"
+000098d0: 6c28 2370 3232 6131 3661 3664 6264 2922  l(#p22a16a6dbd)"
 000098e0: 2073 7479 6c65 3d22 6669 6c6c 3a20 6e6f   style="fill: no
 000098f0: 6e65 3b20 7374 726f 6b65 3a20 2334 3234  ne; stroke: #424
 00009900: 3234 323b 2073 7472 6f6b 652d 7769 6474  242; stroke-widt
 00009910: 683a 2032 2e37 3b20 7374 726f 6b65 2d6c  h: 2.7; stroke-l
 00009920: 696e 6563 6170 3a20 7371 7561 7265 222f  inecap: square"/
 00009930: 3e0a 2020 203c 2f67 3e0a 2020 203c 6720  >.   </g>.   <g 
 00009940: 6964 3d22 6c69 6e65 3264 5f34 3922 3e0a  id="line2d_49">.
 00009950: 2020 2020 3c70 6174 6820 636c 6970 2d70      <path clip-p
-00009960: 6174 683d 2275 726c 2823 7062 6632 6531  ath="url(#pbf2e1
-00009970: 3966 3166 3429 2220 7374 796c 653d 2266  9f1f4)" style="f
+00009960: 6174 683d 2275 726c 2823 7032 3261 3136  ath="url(#p22a16
+00009970: 6136 6462 6429 2220 7374 796c 653d 2266  a6dbd)" style="f
 00009980: 696c 6c3a 206e 6f6e 653b 2073 7472 6f6b  ill: none; strok
 00009990: 653a 2023 3432 3432 3432 3b20 7374 726f  e: #424242; stro
 000099a0: 6b65 2d77 6964 7468 3a20 322e 373b 2073  ke-width: 2.7; s
 000099b0: 7472 6f6b 652d 6c69 6e65 6361 703a 2073  troke-linecap: s
 000099c0: 7175 6172 6522 2f3e 0a20 2020 3c2f 673e  quare"/>.   </g>
 000099d0: 0a20 2020 3c67 2069 643d 226c 696e 6532  .   <g id="line2
 000099e0: 645f 3530 223e 0a20 2020 203c 7061 7468  d_50">.    <path
 000099f0: 2063 6c69 702d 7061 7468 3d22 7572 6c28   clip-path="url(
-00009a00: 2370 6266 3265 3139 6631 6634 2922 2073  #pbf2e19f1f4)" s
+00009a00: 2370 3232 6131 3661 3664 6264 2922 2073  #p22a16a6dbd)" s
 00009a10: 7479 6c65 3d22 6669 6c6c 3a20 6e6f 6e65  tyle="fill: none
 00009a20: 3b20 7374 726f 6b65 3a20 2334 3234 3234  ; stroke: #42424
 00009a30: 323b 2073 7472 6f6b 652d 7769 6474 683a  2; stroke-width:
 00009a40: 2032 2e37 3b20 7374 726f 6b65 2d6c 696e   2.7; stroke-lin
 00009a50: 6563 6170 3a20 7371 7561 7265 222f 3e0a  ecap: square"/>.
 00009a60: 2020 203c 2f67 3e0a 2020 203c 6720 6964     </g>.   <g id
 00009a70: 3d22 6c69 6e65 3264 5f35 3122 3e0a 2020  ="line2d_51">.  
 00009a80: 2020 3c70 6174 6820 636c 6970 2d70 6174    <path clip-pat
-00009a90: 683d 2275 726c 2823 7062 6632 6531 3966  h="url(#pbf2e19f
-00009aa0: 3166 3429 2220 7374 796c 653d 2266 696c  1f4)" style="fil
+00009a90: 683d 2275 726c 2823 7032 3261 3136 6136  h="url(#p22a16a6
+00009aa0: 6462 6429 2220 7374 796c 653d 2266 696c  dbd)" style="fil
 00009ab0: 6c3a 206e 6f6e 653b 2073 7472 6f6b 653a  l: none; stroke:
 00009ac0: 2023 3432 3432 3432 3b20 7374 726f 6b65   #424242; stroke
 00009ad0: 2d77 6964 7468 3a20 322e 373b 2073 7472  -width: 2.7; str
 00009ae0: 6f6b 652d 6c69 6e65 6361 703a 2073 7175  oke-linecap: squ
 00009af0: 6172 6522 2f3e 0a20 2020 3c2f 673e 0a20  are"/>.   </g>. 
 00009b00: 2020 3c67 2069 643d 226c 696e 6532 645f    <g id="line2d_
 00009b10: 3532 223e 0a20 2020 203c 7061 7468 2063  52">.    <path c
 00009b20: 6c69 702d 7061 7468 3d22 7572 6c28 2370  lip-path="url(#p
-00009b30: 6266 3265 3139 6631 6634 2922 2073 7479  bf2e19f1f4)" sty
+00009b30: 3232 6131 3661 3664 6264 2922 2073 7479  22a16a6dbd)" sty
 00009b40: 6c65 3d22 6669 6c6c 3a20 6e6f 6e65 3b20  le="fill: none; 
 00009b50: 7374 726f 6b65 3a20 2334 3234 3234 323b  stroke: #424242;
 00009b60: 2073 7472 6f6b 652d 7769 6474 683a 2032   stroke-width: 2
 00009b70: 2e37 3b20 7374 726f 6b65 2d6c 696e 6563  .7; stroke-linec
 00009b80: 6170 3a20 7371 7561 7265 222f 3e0a 2020  ap: square"/>.  
 00009b90: 203c 2f67 3e0a 2020 203c 6720 6964 3d22   </g>.   <g id="
 00009ba0: 6c69 6e65 3264 5f35 3322 3e0a 2020 2020  line2d_53">.    
 00009bb0: 3c70 6174 6820 636c 6970 2d70 6174 683d  <path clip-path=
-00009bc0: 2275 726c 2823 7062 6632 6531 3966 3166  "url(#pbf2e19f1f
-00009bd0: 3429 2220 7374 796c 653d 2266 696c 6c3a  4)" style="fill:
+00009bc0: 2275 726c 2823 7032 3261 3136 6136 6462  "url(#p22a16a6db
+00009bd0: 6429 2220 7374 796c 653d 2266 696c 6c3a  d)" style="fill:
 00009be0: 206e 6f6e 653b 2073 7472 6f6b 653a 2023   none; stroke: #
 00009bf0: 3432 3432 3432 3b20 7374 726f 6b65 2d77  424242; stroke-w
 00009c00: 6964 7468 3a20 322e 373b 2073 7472 6f6b  idth: 2.7; strok
 00009c10: 652d 6c69 6e65 6361 703a 2073 7175 6172  e-linecap: squar
 00009c20: 6522 2f3e 0a20 2020 3c2f 673e 0a20 2020  e"/>.   </g>.   
 00009c30: 3c67 2069 643d 226c 696e 6532 645f 3534  <g id="line2d_54
 00009c40: 223e 0a20 2020 203c 7061 7468 2063 6c69  ">.    <path cli
-00009c50: 702d 7061 7468 3d22 7572 6c28 2370 6266  p-path="url(#pbf
-00009c60: 3265 3139 6631 6634 2922 2073 7479 6c65  2e19f1f4)" style
+00009c50: 702d 7061 7468 3d22 7572 6c28 2370 3232  p-path="url(#p22
+00009c60: 6131 3661 3664 6264 2922 2073 7479 6c65  a16a6dbd)" style
 00009c70: 3d22 6669 6c6c 3a20 6e6f 6e65 3b20 7374  ="fill: none; st
 00009c80: 726f 6b65 3a20 2334 3234 3234 323b 2073  roke: #424242; s
 00009c90: 7472 6f6b 652d 7769 6474 683a 2032 2e37  troke-width: 2.7
 00009ca0: 3b20 7374 726f 6b65 2d6c 696e 6563 6170  ; stroke-linecap
 00009cb0: 3a20 7371 7561 7265 222f 3e0a 2020 203c  : square"/>.   <
 00009cc0: 2f67 3e0a 2020 203c 6720 6964 3d22 6c69  /g>.   <g id="li
 00009cd0: 6e65 3264 5f35 3522 3e0a 2020 2020 3c70  ne2d_55">.    <p
 00009ce0: 6174 6820 636c 6970 2d70 6174 683d 2275  ath clip-path="u
-00009cf0: 726c 2823 7062 6632 6531 3966 3166 3429  rl(#pbf2e19f1f4)
+00009cf0: 726c 2823 7032 3261 3136 6136 6462 6429  rl(#p22a16a6dbd)
 00009d00: 2220 7374 796c 653d 2266 696c 6c3a 206e  " style="fill: n
 00009d10: 6f6e 653b 2073 7472 6f6b 653a 2023 3432  one; stroke: #42
 00009d20: 3432 3432 3b20 7374 726f 6b65 2d77 6964  4242; stroke-wid
 00009d30: 7468 3a20 322e 373b 2073 7472 6f6b 652d  th: 2.7; stroke-
 00009d40: 6c69 6e65 6361 703a 2073 7175 6172 6522  linecap: square"
 00009d50: 2f3e 0a20 2020 3c2f 673e 0a20 2020 3c67  />.   </g>.   <g
 00009d60: 2069 643d 226c 696e 6532 645f 3536 223e   id="line2d_56">
 00009d70: 0a20 2020 203c 7061 7468 2063 6c69 702d  .    <path clip-
-00009d80: 7061 7468 3d22 7572 6c28 2370 6266 3265  path="url(#pbf2e
-00009d90: 3139 6631 6634 2922 2073 7479 6c65 3d22  19f1f4)" style="
+00009d80: 7061 7468 3d22 7572 6c28 2370 3232 6131  path="url(#p22a1
+00009d90: 3661 3664 6264 2922 2073 7479 6c65 3d22  6a6dbd)" style="
 00009da0: 6669 6c6c 3a20 6e6f 6e65 3b20 7374 726f  fill: none; stro
 00009db0: 6b65 3a20 2334 3234 3234 323b 2073 7472  ke: #424242; str
 00009dc0: 6f6b 652d 7769 6474 683a 2032 2e37 3b20  oke-width: 2.7; 
 00009dd0: 7374 726f 6b65 2d6c 696e 6563 6170 3a20  stroke-linecap: 
 00009de0: 7371 7561 7265 222f 3e0a 2020 203c 2f67  square"/>.   </g
 00009df0: 3e0a 2020 203c 6720 6964 3d22 6c69 6e65  >.   <g id="line
 00009e00: 3264 5f35 3722 3e0a 2020 2020 3c70 6174  2d_57">.    <pat
 00009e10: 6820 636c 6970 2d70 6174 683d 2275 726c  h clip-path="url
-00009e20: 2823 7062 6632 6531 3966 3166 3429 2220  (#pbf2e19f1f4)" 
+00009e20: 2823 7032 3261 3136 6136 6462 6429 2220  (#p22a16a6dbd)" 
 00009e30: 7374 796c 653d 2266 696c 6c3a 206e 6f6e  style="fill: non
 00009e40: 653b 2073 7472 6f6b 653a 2023 3432 3432  e; stroke: #4242
 00009e50: 3432 3b20 7374 726f 6b65 2d77 6964 7468  42; stroke-width
 00009e60: 3a20 322e 373b 2073 7472 6f6b 652d 6c69  : 2.7; stroke-li
 00009e70: 6e65 6361 703a 2073 7175 6172 6522 2f3e  necap: square"/>
 00009e80: 0a20 2020 3c2f 673e 0a20 2020 3c67 2069  .   </g>.   <g i
 00009e90: 643d 226c 696e 6532 645f 3538 223e 0a20  d="line2d_58">. 
 00009ea0: 2020 203c 7061 7468 2063 6c69 702d 7061     <path clip-pa
-00009eb0: 7468 3d22 7572 6c28 2370 6266 3265 3139  th="url(#pbf2e19
-00009ec0: 6631 6634 2922 2073 7479 6c65 3d22 6669  f1f4)" style="fi
+00009eb0: 7468 3d22 7572 6c28 2370 3232 6131 3661  th="url(#p22a16a
+00009ec0: 3664 6264 2922 2073 7479 6c65 3d22 6669  6dbd)" style="fi
 00009ed0: 6c6c 3a20 6e6f 6e65 3b20 7374 726f 6b65  ll: none; stroke
 00009ee0: 3a20 2334 3234 3234 323b 2073 7472 6f6b  : #424242; strok
 00009ef0: 652d 7769 6474 683a 2032 2e37 3b20 7374  e-width: 2.7; st
 00009f00: 726f 6b65 2d6c 696e 6563 6170 3a20 7371  roke-linecap: sq
 00009f10: 7561 7265 222f 3e0a 2020 203c 2f67 3e0a  uare"/>.   </g>.
 00009f20: 2020 203c 6720 6964 3d22 6c69 6e65 3264     <g id="line2d
 00009f30: 5f35 3922 3e0a 2020 2020 3c70 6174 6820  _59">.    <path 
 00009f40: 636c 6970 2d70 6174 683d 2275 726c 2823  clip-path="url(#
-00009f50: 7062 6632 6531 3966 3166 3429 2220 7374  pbf2e19f1f4)" st
+00009f50: 7032 3261 3136 6136 6462 6429 2220 7374  p22a16a6dbd)" st
 00009f60: 796c 653d 2266 696c 6c3a 206e 6f6e 653b  yle="fill: none;
 00009f70: 2073 7472 6f6b 653a 2023 3432 3432 3432   stroke: #424242
 00009f80: 3b20 7374 726f 6b65 2d77 6964 7468 3a20  ; stroke-width: 
 00009f90: 322e 373b 2073 7472 6f6b 652d 6c69 6e65  2.7; stroke-line
 00009fa0: 6361 703a 2073 7175 6172 6522 2f3e 0a20  cap: square"/>. 
 00009fb0: 2020 3c2f 673e 0a20 2020 3c67 2069 643d    </g>.   <g id=
 00009fc0: 226c 696e 6532 645f 3630 223e 0a20 2020  "line2d_60">.   
 00009fd0: 203c 7061 7468 2063 6c69 702d 7061 7468   <path clip-path
-00009fe0: 3d22 7572 6c28 2370 6266 3265 3139 6631  ="url(#pbf2e19f1
-00009ff0: 6634 2922 2073 7479 6c65 3d22 6669 6c6c  f4)" style="fill
+00009fe0: 3d22 7572 6c28 2370 3232 6131 3661 3664  ="url(#p22a16a6d
+00009ff0: 6264 2922 2073 7479 6c65 3d22 6669 6c6c  bd)" style="fill
 0000a000: 3a20 6e6f 6e65 3b20 7374 726f 6b65 3a20  : none; stroke: 
 0000a010: 2334 3234 3234 323b 2073 7472 6f6b 652d  #424242; stroke-
 0000a020: 7769 6474 683a 2032 2e37 3b20 7374 726f  width: 2.7; stro
 0000a030: 6b65 2d6c 696e 6563 6170 3a20 7371 7561  ke-linecap: squa
 0000a040: 7265 222f 3e0a 2020 203c 2f67 3e0a 2020  re"/>.   </g>.  
 0000a050: 203c 6720 6964 3d22 6c69 6e65 3264 5f36   <g id="line2d_6
 0000a060: 3122 3e0a 2020 2020 3c70 6174 6820 636c  1">.    <path cl
-0000a070: 6970 2d70 6174 683d 2275 726c 2823 7062  ip-path="url(#pb
-0000a080: 6632 6531 3966 3166 3429 2220 7374 796c  f2e19f1f4)" styl
+0000a070: 6970 2d70 6174 683d 2275 726c 2823 7032  ip-path="url(#p2
+0000a080: 3261 3136 6136 6462 6429 2220 7374 796c  2a16a6dbd)" styl
 0000a090: 653d 2266 696c 6c3a 206e 6f6e 653b 2073  e="fill: none; s
 0000a0a0: 7472 6f6b 653a 2023 3432 3432 3432 3b20  troke: #424242; 
 0000a0b0: 7374 726f 6b65 2d77 6964 7468 3a20 322e  stroke-width: 2.
 0000a0c0: 373b 2073 7472 6f6b 652d 6c69 6e65 6361  7; stroke-lineca
 0000a0d0: 703a 2073 7175 6172 6522 2f3e 0a20 2020  p: square"/>.   
 0000a0e0: 3c2f 673e 0a20 2020 3c67 2069 643d 226c  </g>.   <g id="l
 0000a0f0: 696e 6532 645f 3632 223e 0a20 2020 203c  ine2d_62">.    <
 0000a100: 7061 7468 2063 6c69 702d 7061 7468 3d22  path clip-path="
-0000a110: 7572 6c28 2370 6266 3265 3139 6631 6634  url(#pbf2e19f1f4
+0000a110: 7572 6c28 2370 3232 6131 3661 3664 6264  url(#p22a16a6dbd
 0000a120: 2922 2073 7479 6c65 3d22 6669 6c6c 3a20  )" style="fill: 
 0000a130: 6e6f 6e65 3b20 7374 726f 6b65 3a20 2334  none; stroke: #4
 0000a140: 3234 3234 323b 2073 7472 6f6b 652d 7769  24242; stroke-wi
 0000a150: 6474 683a 2032 2e37 3b20 7374 726f 6b65  dth: 2.7; stroke
 0000a160: 2d6c 696e 6563 6170 3a20 7371 7561 7265  -linecap: square
 0000a170: 222f 3e0a 2020 203c 2f67 3e0a 2020 203c  "/>.   </g>.   <
 0000a180: 6720 6964 3d22 6c69 6e65 3264 5f36 3322  g id="line2d_63"
 0000a190: 3e0a 2020 2020 3c70 6174 6820 636c 6970  >.    <path clip
-0000a1a0: 2d70 6174 683d 2275 726c 2823 7062 6632  -path="url(#pbf2
-0000a1b0: 6531 3966 3166 3429 2220 7374 796c 653d  e19f1f4)" style=
+0000a1a0: 2d70 6174 683d 2275 726c 2823 7032 3261  -path="url(#p22a
+0000a1b0: 3136 6136 6462 6429 2220 7374 796c 653d  16a6dbd)" style=
 0000a1c0: 2266 696c 6c3a 206e 6f6e 653b 2073 7472  "fill: none; str
 0000a1d0: 6f6b 653a 2023 3432 3432 3432 3b20 7374  oke: #424242; st
 0000a1e0: 726f 6b65 2d77 6964 7468 3a20 322e 373b  roke-width: 2.7;
 0000a1f0: 2073 7472 6f6b 652d 6c69 6e65 6361 703a   stroke-linecap:
 0000a200: 2073 7175 6172 6522 2f3e 0a20 2020 3c2f   square"/>.   </
 0000a210: 673e 0a20 2020 3c67 2069 643d 226c 696e  g>.   <g id="lin
 0000a220: 6532 645f 3634 223e 0a20 2020 203c 7061  e2d_64">.    <pa
 0000a230: 7468 2063 6c69 702d 7061 7468 3d22 7572  th clip-path="ur
-0000a240: 6c28 2370 6266 3265 3139 6631 6634 2922  l(#pbf2e19f1f4)"
+0000a240: 6c28 2370 3232 6131 3661 3664 6264 2922  l(#p22a16a6dbd)"
 0000a250: 2073 7479 6c65 3d22 6669 6c6c 3a20 6e6f   style="fill: no
 0000a260: 6e65 3b20 7374 726f 6b65 3a20 2334 3234  ne; stroke: #424
 0000a270: 3234 323b 2073 7472 6f6b 652d 7769 6474  242; stroke-widt
 0000a280: 683a 2032 2e37 3b20 7374 726f 6b65 2d6c  h: 2.7; stroke-l
 0000a290: 696e 6563 6170 3a20 7371 7561 7265 222f  inecap: square"/
 0000a2a0: 3e0a 2020 203c 2f67 3e0a 2020 203c 6720  >.   </g>.   <g 
 0000a2b0: 6964 3d22 6c69 6e65 3264 5f36 3522 3e0a  id="line2d_65">.
 0000a2c0: 2020 2020 3c70 6174 6820 636c 6970 2d70      <path clip-p
-0000a2d0: 6174 683d 2275 726c 2823 7062 6632 6531  ath="url(#pbf2e1
-0000a2e0: 3966 3166 3429 2220 7374 796c 653d 2266  9f1f4)" style="f
+0000a2d0: 6174 683d 2275 726c 2823 7032 3261 3136  ath="url(#p22a16
+0000a2e0: 6136 6462 6429 2220 7374 796c 653d 2266  a6dbd)" style="f
 0000a2f0: 696c 6c3a 206e 6f6e 653b 2073 7472 6f6b  ill: none; strok
 0000a300: 653a 2023 3432 3432 3432 3b20 7374 726f  e: #424242; stro
 0000a310: 6b65 2d77 6964 7468 3a20 322e 373b 2073  ke-width: 2.7; s
 0000a320: 7472 6f6b 652d 6c69 6e65 6361 703a 2073  troke-linecap: s
 0000a330: 7175 6172 6522 2f3e 0a20 2020 3c2f 673e  quare"/>.   </g>
 0000a340: 0a20 2020 3c67 2069 643d 226c 696e 6532  .   <g id="line2
 0000a350: 645f 3636 223e 0a20 2020 203c 7061 7468  d_66">.    <path
 0000a360: 2063 6c69 702d 7061 7468 3d22 7572 6c28   clip-path="url(
-0000a370: 2370 6266 3265 3139 6631 6634 2922 2073  #pbf2e19f1f4)" s
+0000a370: 2370 3232 6131 3661 3664 6264 2922 2073  #p22a16a6dbd)" s
 0000a380: 7479 6c65 3d22 6669 6c6c 3a20 6e6f 6e65  tyle="fill: none
 0000a390: 3b20 7374 726f 6b65 3a20 2334 3234 3234  ; stroke: #42424
 0000a3a0: 323b 2073 7472 6f6b 652d 7769 6474 683a  2; stroke-width:
 0000a3b0: 2032 2e37 3b20 7374 726f 6b65 2d6c 696e   2.7; stroke-lin
 0000a3c0: 6563 6170 3a20 7371 7561 7265 222f 3e0a  ecap: square"/>.
 0000a3d0: 2020 203c 2f67 3e0a 2020 203c 6720 6964     </g>.   <g id
 0000a3e0: 3d22 6c69 6e65 3264 5f36 3722 3e0a 2020  ="line2d_67">.  
 0000a3f0: 2020 3c70 6174 6820 636c 6970 2d70 6174    <path clip-pat
-0000a400: 683d 2275 726c 2823 7062 6632 6531 3966  h="url(#pbf2e19f
-0000a410: 3166 3429 2220 7374 796c 653d 2266 696c  1f4)" style="fil
+0000a400: 683d 2275 726c 2823 7032 3261 3136 6136  h="url(#p22a16a6
+0000a410: 6462 6429 2220 7374 796c 653d 2266 696c  dbd)" style="fil
 0000a420: 6c3a 206e 6f6e 653b 2073 7472 6f6b 653a  l: none; stroke:
 0000a430: 2023 3432 3432 3432 3b20 7374 726f 6b65   #424242; stroke
 0000a440: 2d77 6964 7468 3a20 322e 373b 2073 7472  -width: 2.7; str
 0000a450: 6f6b 652d 6c69 6e65 6361 703a 2073 7175  oke-linecap: squ
 0000a460: 6172 6522 2f3e 0a20 2020 3c2f 673e 0a20  are"/>.   </g>. 
 0000a470: 2020 3c67 2069 643d 226c 696e 6532 645f    <g id="line2d_
 0000a480: 3638 223e 0a20 2020 203c 7061 7468 2063  68">.    <path c
 0000a490: 6c69 702d 7061 7468 3d22 7572 6c28 2370  lip-path="url(#p
-0000a4a0: 6266 3265 3139 6631 6634 2922 2073 7479  bf2e19f1f4)" sty
+0000a4a0: 3232 6131 3661 3664 6264 2922 2073 7479  22a16a6dbd)" sty
 0000a4b0: 6c65 3d22 6669 6c6c 3a20 6e6f 6e65 3b20  le="fill: none; 
 0000a4c0: 7374 726f 6b65 3a20 2334 3234 3234 323b  stroke: #424242;
 0000a4d0: 2073 7472 6f6b 652d 7769 6474 683a 2032   stroke-width: 2
 0000a4e0: 2e37 3b20 7374 726f 6b65 2d6c 696e 6563  .7; stroke-linec
 0000a4f0: 6170 3a20 7371 7561 7265 222f 3e0a 2020  ap: square"/>.  
 0000a500: 203c 2f67 3e0a 2020 203c 6720 6964 3d22   </g>.   <g id="
 0000a510: 7061 7463 685f 3333 223e 0a20 2020 203c  patch_33">.    <
@@ -3007,15 +3007,15 @@
 0000bbe0: 392e 3936 3837 3522 2f3e 0a20 2020 2020  9.96875"/>.     
 0000bbf0: 3c75 7365 2078 6c69 6e6b 3a68 7265 663d  <use xlink:href=
 0000bc00: 2223 4465 6a61 5675 5361 6e73 2d37 3322  "#DejaVuSans-73"
 0000bc10: 2078 3d22 3231 3931 2e34 3932 3138 3822   x="2191.492188"
 0000bc20: 2f3e 0a20 2020 203c 2f67 3e0a 2020 203c  />.    </g>.   <
 0000bc30: 2f67 3e0a 2020 3c2f 673e 0a20 3c2f 673e  /g>.  </g>. </g>
 0000bc40: 0a20 3c64 6566 733e 0a20 203c 636c 6970  . <defs>.  <clip
-0000bc50: 5061 7468 2069 643d 2270 6266 3265 3139  Path id="pbf2e19
-0000bc60: 6631 6634 223e 0a20 2020 3c72 6563 7420  f1f4">.   <rect 
+0000bc50: 5061 7468 2069 643d 2270 3232 6131 3661  Path id="p22a16a
+0000bc60: 3664 6264 223e 0a20 2020 3c72 6563 7420  6dbd">.   <rect 
 0000bc70: 783d 2234 342e 3537 2220 793d 2232 362e  x="44.57" y="26.
 0000bc80: 3838 2220 7769 6474 683d 2235 3135 2e35  88" width="515.5
 0000bc90: 3936 3633 3622 2068 6569 6768 743d 2231  96636" height="1
 0000bca0: 3832 2e31 3138 3731 3422 2f3e 0a20 203c  82.118714"/>.  <
 0000bcb0: 2f63 6c69 7050 6174 683e 0a20 3c2f 6465  /clipPath>. </de
 0000bcc0: 6673 3e0a 3c2f 7376 673e 0a              fs>.</svg>.
```

### Comparing `bioregistry-0.9.6/docs/img/bioregistry_coverage.svg` & `bioregistry-0.9.7/docs/img/bioregistry_coverage.svg`

 * *Files 2% similar despite different names*

```diff
@@ -30,16 +30,16 @@
 000001d0: 6178 2d6e 7323 223e 0a20 2020 3c63 633a  ax-ns#">.   <cc:
 000001e0: 576f 726b 3e0a 2020 2020 3c64 633a 7479  Work>.    <dc:ty
 000001f0: 7065 2072 6466 3a72 6573 6f75 7263 653d  pe rdf:resource=
 00000200: 2268 7474 703a 2f2f 7075 726c 2e6f 7267  "http://purl.org
 00000210: 2f64 632f 6463 6d69 7479 7065 2f53 7469  /dc/dcmitype/Sti
 00000220: 6c6c 496d 6167 6522 2f3e 0a20 2020 203c  llImage"/>.    <
 00000230: 6463 3a64 6174 653e 3230 3233 2d30 352d  dc:date>2023-05-
-00000240: 3036 5430 313a 3038 3a30 392e 3633 3134  06T01:08:09.6314
-00000250: 3236 3c2f 6463 3a64 6174 653e 0a20 2020  26</dc:date>.   
+00000240: 3037 5430 313a 3134 3a30 382e 3138 3238  07T01:14:08.1828
+00000250: 3035 3c2f 6463 3a64 6174 653e 0a20 2020  05</dc:date>.   
 00000260: 203c 6463 3a66 6f72 6d61 743e 696d 6167   <dc:format>imag
 00000270: 652f 7376 672b 786d 6c3c 2f64 633a 666f  e/svg+xml</dc:fo
 00000280: 726d 6174 3e0a 2020 2020 3c64 633a 6372  rmat>.    <dc:cr
 00000290: 6561 746f 723e 0a20 2020 2020 3c63 633a  eator>.     <cc:
 000002a0: 4167 656e 743e 0a20 2020 2020 203c 6463  Agent>.      <dc
 000002b0: 3a74 6974 6c65 3e4d 6174 706c 6f74 6c69  :title>Matplotli
 000002c0: 6220 7633 2e37 2e31 2c20 6874 7470 733a  b v3.7.1, https:
@@ -196,15 +196,15 @@
 00000c30: 3920 3939 2e30 3133 3639 2031 3731 2e33  9 99.01369 171.3
 00000c40: 3438 3334 3420 3932 2e37 3535 3034 3920  48344 92.755049 
 00000c50: 0a43 2031 3734 2e30 3338 3534 3920 3836  .C 174.038549 86
 00000c60: 2e34 3936 3430 3820 3137 352e 3437 3630  .496408 175.4760
 00000c70: 3220 3739 2e37 3730 3639 3420 3137 352e  2 79.770694 175.
 00000c80: 3537 3932 3733 2037 322e 3935 3931 3520  579273 72.95915 
 00000c90: 0a22 2063 6c69 702d 7061 7468 3d22 7572  ." clip-path="ur
-00000ca0: 6c28 2370 6261 3363 3735 3634 3339 2922  l(#pba3c756439)"
+00000ca0: 6c28 2370 3662 3436 3639 3465 3236 2922  l(#p6b46694e26)"
 00000cb0: 2073 7479 6c65 3d22 6669 6c6c 3a20 2363   style="fill: #c
 00000cc0: 3063 3063 303b 206f 7061 6369 7479 3a20  0c0c0; opacity: 
 00000cd0: 302e 3422 2f3e 0a20 2020 3c2f 673e 0a20  0.4"/>.   </g>. 
 00000ce0: 2020 3c67 2069 643d 2270 6174 6368 5f33    <g id="patch_3
 00000cf0: 223e 0a20 2020 203c 7061 7468 2064 3d22  ">.    <path d="
 00000d00: 4d20 3137 352e 3537 3932 3733 2037 312e  M 175.579273 71.
 00000d10: 3337 3839 3139 200a 4320 3137 352e 3538  378919 .C 175.58
@@ -221,15 +221,15 @@
 00000dc0: 3433 3234 3820 3137 352e 3539 3435 3031  43248 175.594501
 00000dd0: 2037 322e 3136 3930 3335 200a 4320 3137   72.169035 .C 17
 00000de0: 352e 3539 3435 3031 2037 312e 3930 3535  5.594501 71.9055
 00000df0: 3920 3137 352e 3538 3934 3234 2037 312e  9 175.589424 71.
 00000e00: 3634 3231 3639 2031 3735 2e35 3739 3237  642169 175.57927
 00000e10: 3320 3731 2e33 3738 3931 3920 0a22 2063  3 71.378919 ." c
 00000e20: 6c69 702d 7061 7468 3d22 7572 6c28 2370  lip-path="url(#p
-00000e30: 6261 3363 3735 3634 3339 2922 2073 7479  ba3c756439)" sty
+00000e30: 3662 3436 3639 3465 3236 2922 2073 7479  6b46694e26)" sty
 00000e40: 6c65 3d22 6669 6c6c 3a20 2361 3663 6565  le="fill: #a6cee
 00000e50: 333b 206f 7061 6369 7479 3a20 302e 3422  3; opacity: 0.4"
 00000e60: 2f3e 0a20 2020 3c2f 673e 0a20 2020 3c67  />.   </g>.   <g
 00000e70: 2069 643d 2270 6174 6368 5f34 223e 0a20   id="patch_4">. 
 00000e80: 2020 203c 7061 7468 2064 3d22 4d20 3137     <path d="M 17
 00000e90: 352e 3537 3932 3733 2037 322e 3935 3931  5.579273 72.9591
 00000ea0: 3520 0a43 2031 3735 2e35 3833 3236 3520  5 .C 175.583265 
@@ -303,15 +303,15 @@
 000012e0: 3620 3833 2e30 3731 3839 3120 3137 332e  6 83.071891 173.
 000012f0: 3735 3832 3435 2038 302e 3635 3035 3132  758245 80.650512
 00001300: 200a 4320 3137 342e 3835 3832 3733 2037   .C 174.858273 7
 00001310: 382e 3232 3931 3333 2031 3735 2e34 3736  8.229133 175.476
 00001320: 3739 3720 3735 2e36 3136 3731 3320 3137  797 75.616713 17
 00001330: 352e 3537 3932 3733 2037 322e 3935 3931  5.579273 72.9591
 00001340: 3520 0a22 2063 6c69 702d 7061 7468 3d22  5 ." clip-path="
-00001350: 7572 6c28 2370 6261 3363 3735 3634 3339  url(#pba3c756439
+00001350: 7572 6c28 2370 3662 3436 3639 3465 3236  url(#p6b46694e26
 00001360: 2922 2073 7479 6c65 3d22 6669 6c6c 3a20  )" style="fill: 
 00001370: 2366 6266 6666 663b 206f 7061 6369 7479  #fbffff; opacity
 00001380: 3a20 302e 3422 2f3e 0a20 2020 3c2f 673e  : 0.4"/>.   </g>
 00001390: 0a20 2020 3c67 2069 643d 2274 6578 745f  .   <g id="text_
 000013a0: 3122 3e0a 2020 2020 3c21 2d2d 2031 3339  1">.    <!-- 139
 000013b0: 3320 2d2d 3e0a 2020 2020 3c67 2073 7479  3 -->.    <g sty
 000013c0: 6c65 3d22 6669 6c6c 3a20 2332 3632 3632  le="fill: #26262
@@ -1031,15 +1031,15 @@
 00004060: 392e 3033 3038 3439 2034 3030 2e35 3434  9.030849 400.544
 00004070: 3038 3720 3932 2e37 3734 3230 3620 0a43  087 92.774206 .C
 00004080: 2034 3033 2e32 3336 3420 3836 2e35 3137   403.2364 86.517
 00004090: 3536 3220 3430 342e 3637 3635 3337 2037  562 404.676537 7
 000040a0: 392e 3739 3334 3733 2034 3034 2e37 3832  9.793473 404.782
 000040b0: 3838 3820 3732 2e39 3832 3938 200a 2220  888 72.98298 ." 
 000040c0: 636c 6970 2d70 6174 683d 2275 726c 2823  clip-path="url(#
-000040d0: 7063 3334 3737 3937 6461 6329 2220 7374  pc347797dac)" st
+000040d0: 7062 6665 3339 3532 3337 6129 2220 7374  pbfe395237a)" st
 000040e0: 796c 653d 2266 696c 6c3a 2023 6330 6330  yle="fill: #c0c0
 000040f0: 6330 3b20 6f70 6163 6974 793a 2030 2e34  c0; opacity: 0.4
 00004100: 222f 3e0a 2020 203c 2f67 3e0a 2020 203c  "/>.   </g>.   <
 00004110: 6720 6964 3d22 7061 7463 685f 3622 3e0a  g id="patch_6">.
 00004120: 2020 2020 3c70 6174 6820 643d 224d 2034      <path d="M 4
 00004130: 3034 2e37 3832 3838 3820 3731 2e33 3535  04.782888 71.355
 00004140: 3039 200a 4320 3430 342e 3738 3731 3235  09 .C 404.787125
@@ -1055,16 +1055,16 @@
 000041e0: 342e 3739 3834 3833 2037 322e 3434 3034  4.798483 72.4404
 000041f0: 3234 2034 3034 2e37 3938 3438 3320 3732  24 404.798483 72
 00004200: 2e31 3639 3033 3520 0a43 2034 3034 2e37  .169035 .C 404.7
 00004210: 3938 3438 3320 3731 2e38 3937 3634 3520  98483 71.897645 
 00004220: 3430 342e 3739 3332 3834 2037 312e 3632  404.793284 71.62
 00004230: 3632 3831 2034 3034 2e37 3832 3838 3820  6281 404.782888 
 00004240: 3731 2e33 3535 3039 200a 2220 636c 6970  71.35509 ." clip
-00004250: 2d70 6174 683d 2275 726c 2823 7063 3334  -path="url(#pc34
-00004260: 3737 3937 6461 6329 2220 7374 796c 653d  7797dac)" style=
+00004250: 2d70 6174 683d 2275 726c 2823 7062 6665  -path="url(#pbfe
+00004260: 3339 3532 3337 6129 2220 7374 796c 653d  395237a)" style=
 00004270: 2266 696c 6c3a 2023 3166 3738 6234 3b20  "fill: #1f78b4; 
 00004280: 6f70 6163 6974 793a 2030 2e34 222f 3e0a  opacity: 0.4"/>.
 00004290: 2020 203c 2f67 3e0a 2020 203c 6720 6964     </g>.   <g id
 000042a0: 3d22 7061 7463 685f 3722 3e0a 2020 2020  ="patch_7">.    
 000042b0: 3c70 6174 6820 643d 224d 2034 3034 2e37  <path d="M 404.7
 000042c0: 3832 3838 3820 3732 2e39 3832 3938 200a  82888 72.98298 .
 000042d0: 4320 3430 342e 3738 3731 3235 2037 322e  C 404.787125 72.
@@ -1137,15 +1137,15 @@
 00004700: 3620 3833 2e34 3633 3931 3420 3430 322e  6 83.463914 402.
 00004710: 3839 3733 3732 2038 302e 3935 3432 3936  897372 80.954296
 00004720: 200a 4320 3430 342e 3033 3638 3834 2037   .C 404.036884 7
 00004730: 382e 3434 3436 3738 2034 3034 2e36 3737  8.444678 404.677
 00004740: 3331 3420 3735 2e37 3337 3136 3220 3430  314 75.737162 40
 00004750: 342e 3738 3238 3838 2037 322e 3938 3239  4.782888 72.9829
 00004760: 3820 0a22 2063 6c69 702d 7061 7468 3d22  8 ." clip-path="
-00004770: 7572 6c28 2370 6333 3437 3739 3764 6163  url(#pc347797dac
+00004770: 7572 6c28 2370 6266 6533 3935 3233 3761  url(#pbfe395237a
 00004780: 2922 2073 7479 6c65 3d22 6669 6c6c 3a20  )" style="fill: 
 00004790: 2339 6364 6166 663b 206f 7061 6369 7479  #9cdaff; opacity
 000047a0: 3a20 302e 3422 2f3e 0a20 2020 3c2f 673e  : 0.4"/>.   </g>
 000047b0: 0a20 2020 3c67 2069 643d 2274 6578 745f  .   <g id="text_
 000047c0: 3622 3e0a 2020 2020 3c21 2d2d 2031 3337  6">.    <!-- 137
 000047d0: 3520 2d2d 3e0a 2020 2020 3c67 2073 7479  5 -->.    <g sty
 000047e0: 6c65 3d22 6669 6c6c 3a20 2332 3632 3632  le="fill: #26262
@@ -1924,15 +1924,15 @@
 00007830: 3431 3431 2031 3331 2e37 3634 3833 2032  4141 131.76483 2
 00007840: 3534 2e34 3632 3231 3920 0a43 2031 3336  54.462219 .C 136
 00007850: 2e30 3130 3732 2032 3531 2e30 3230 3239  .01072 251.02029
 00007860: 3720 3133 392e 3637 3431 3333 2032 3436  7 139.674133 246
 00007870: 2e39 3136 3332 3220 3134 322e 3631 3338  .916322 142.6138
 00007880: 3736 2032 3432 2e33 3038 3436 3820 0a22  76 242.308468 ."
 00007890: 2063 6c69 702d 7061 7468 3d22 7572 6c28   clip-path="url(
-000078a0: 2370 6639 3437 3131 3337 3432 2922 2073  #pf947113742)" s
+000078a0: 2370 6563 3237 6461 6130 6336 2922 2073  #pec27daa0c6)" s
 000078b0: 7479 6c65 3d22 6669 6c6c 3a20 2363 3063  tyle="fill: #c0c
 000078c0: 3063 303b 206f 7061 6369 7479 3a20 302e  0c0; opacity: 0.
 000078d0: 3422 2f3e 0a20 2020 3c2f 673e 0a20 2020  4"/>.   </g>.   
 000078e0: 3c67 2069 643d 2270 6174 6368 5f31 3222  <g id="patch_12"
 000078f0: 3e0a 2020 2020 3c70 6174 6820 643d 224d  >.    <path d="M
 00007900: 2031 3432 2e36 3133 3837 3620 3138 372e   142.613876 187.
 00007910: 3539 3936 3038 200a 4320 3134 372e 3832  599608 .C 147.82
@@ -1975,15 +1975,15 @@
 00007b60: 3932 3820 3136 302e 3231 3532 3737 2031  928 160.215277 1
 00007b70: 3830 2e36 3534 3431 200a 4320 3135 332e  80.65441 .C 153.
 00007b80: 3831 3536 3835 2031 3831 2e32 3831 3839  815685 181.28189
 00007b90: 3320 3134 372e 3731 3736 3420 3138 332e  3 147.71764 183.
 00007ba0: 3638 3830 3733 2031 3432 2e36 3133 3837  688073 142.61387
 00007bb0: 3620 3138 372e 3539 3936 3038 200a 2220  6 187.599608 ." 
 00007bc0: 636c 6970 2d70 6174 683d 2275 726c 2823  clip-path="url(#
-00007bd0: 7066 3934 3731 3133 3734 3229 2220 7374  pf947113742)" st
+00007bd0: 7065 6332 3764 6161 3063 3629 2220 7374  pec27daa0c6)" st
 00007be0: 796c 653d 2266 696c 6c3a 2023 3333 6130  yle="fill: #33a0
 00007bf0: 3263 3b20 6f70 6163 6974 793a 2030 2e34  2c; opacity: 0.4
 00007c00: 222f 3e0a 2020 203c 2f67 3e0a 2020 203c  "/>.   </g>.   <
 00007c10: 6720 6964 3d22 7061 7463 685f 3133 223e  g id="patch_13">
 00007c20: 0a20 2020 203c 7061 7468 2064 3d22 4d20  .    <path d="M 
 00007c30: 3134 322e 3631 3338 3736 2032 3432 2e33  142.613876 242.3
 00007c40: 3038 3436 3820 0a43 2031 3437 2e38 3236  08468 .C 147.826
@@ -2009,15 +2009,15 @@
 00007d80: 3220 3133 322e 3637 3238 3920 3233 302e  2 132.67289 230.
 00007d90: 3230 3631 3234 200a 4320 3133 352e 3031  206124 .C 135.01
 00007da0: 3337 3639 2032 3334 2e39 3439 3437 3520  3769 234.949475 
 00007db0: 3133 382e 3431 3535 3337 2032 3339 2e30  138.415537 239.0
 00007dc0: 3930 3835 3220 3134 322e 3631 3338 3736  90852 142.613876
 00007dd0: 2032 3432 2e33 3038 3436 3820 0a22 2063   242.308468 ." c
 00007de0: 6c69 702d 7061 7468 3d22 7572 6c28 2370  lip-path="url(#p
-00007df0: 6639 3437 3131 3337 3432 2922 2073 7479  f947113742)" sty
+00007df0: 6563 3237 6461 6130 6336 2922 2073 7479  ec27daa0c6)" sty
 00007e00: 6c65 3d22 6669 6c6c 3a20 2361 6166 3661  le="fill: #aaf6a
 00007e10: 353b 206f 7061 6369 7479 3a20 302e 3422  5; opacity: 0.4"
 00007e20: 2f3e 0a20 2020 3c2f 673e 0a20 2020 3c67  />.   </g>.   <g
 00007e30: 2069 643d 2274 6578 745f 3136 223e 0a20   id="text_16">. 
 00007e40: 2020 203c 212d 2d20 3134 3738 202d 2d3e     <!-- 1478 -->
 00007e50: 0a20 2020 203c 6720 7374 796c 653d 2266  .    <g style="f
 00007e60: 696c 6c3a 2023 3236 3236 3236 2220 7472  ill: #262626" tr
@@ -3113,15 +3113,15 @@
 0000c280: 3038 3033 3934 2031 3234 2e39 3938 3937  080394 124.99897
 0000c290: 3820 3430 312e 3534 3435 3733 200a 4320  8 401.544573 .C 
 0000c2a0: 3132 392e 3337 3835 3737 2033 3939 2e30  129.378577 399.0
 0000c2b0: 3038 3735 3320 3133 332e 3335 3332 3236  08753 133.353226
 0000c2c0: 2033 3935 2e38 3330 3431 3420 3133 362e   395.830414 136.
 0000c2d0: 3739 3031 3436 2033 3932 2e31 3135 3733  790146 392.11573
 0000c2e0: 3320 0a22 2063 6c69 702d 7061 7468 3d22  3 ." clip-path="
-0000c2f0: 7572 6c28 2370 3764 3631 6235 3539 6161  url(#p7d61b559aa
+0000c2f0: 7572 6c28 2370 3336 3762 6264 3436 3063  url(#p367bbd460c
 0000c300: 2922 2073 7479 6c65 3d22 6669 6c6c 3a20  )" style="fill: 
 0000c310: 2363 3063 3063 303b 206f 7061 6369 7479  #c0c0c0; opacity
 0000c320: 3a20 302e 3422 2f3e 0a20 2020 3c2f 673e  : 0.4"/>.   </g>
 0000c330: 0a20 2020 3c67 2069 643d 2270 6174 6368  .   <g id="patch
 0000c340: 5f32 3122 3e0a 2020 2020 3c70 6174 6820  _21">.    <path 
 0000c350: 643d 224d 2031 3336 2e37 3930 3134 3620  d="M 136.790146 
 0000c360: 3332 332e 3336 3233 3520 0a43 2031 3435  323.36235 .C 145
@@ -3164,15 +3164,15 @@
 0000c5b0: 3137 2e33 3939 3136 3220 3135 372e 3030  17.399162 157.00
 0000c5c0: 3234 3820 3331 372e 3531 3931 3720 0a43  248 317.51917 .C
 0000c5d0: 2031 3439 2e38 3636 3530 3820 3331 372e   149.866508 317.
 0000c5e0: 3633 3931 3737 2031 3432 2e38 3839 3339  639177 142.88939
 0000c5f0: 3720 3331 392e 3635 3631 3839 2031 3336  7 319.656189 136
 0000c600: 2e37 3930 3134 3620 3332 332e 3336 3233  .790146 323.3623
 0000c610: 3520 0a22 2063 6c69 702d 7061 7468 3d22  5 ." clip-path="
-0000c620: 7572 6c28 2370 3764 3631 6235 3539 6161  url(#p7d61b559aa
+0000c620: 7572 6c28 2370 3336 3762 6264 3436 3063  url(#p367bbd460c
 0000c630: 2922 2073 7479 6c65 3d22 6669 6c6c 3a20  )" style="fill: 
 0000c640: 2366 6462 6636 663b 206f 7061 6369 7479  #fdbf6f; opacity
 0000c650: 3a20 302e 3422 2f3e 0a20 2020 3c2f 673e  : 0.4"/>.   </g>
 0000c660: 0a20 2020 3c67 2069 643d 2270 6174 6368  .   <g id="patch
 0000c670: 5f32 3222 3e0a 2020 2020 3c70 6174 6820  _22">.    <path 
 0000c680: 643d 224d 2031 3336 2e37 3930 3134 3620  d="M 136.790146 
 0000c690: 3339 322e 3131 3537 3333 200a 4320 3134  392.115733 .C 14
@@ -3198,16 +3198,16 @@
 0000c7d0: 3337 312e 3433 3934 3237 2031 3232 2e36  371.439427 122.6
 0000c7e0: 3139 3233 3220 3337 372e 3436 3030 3334  19232 377.460034
 0000c7f0: 200a 4320 3132 362e 3030 3538 3135 2033   .C 126.005815 3
 0000c800: 3833 2e34 3830 3634 3220 3133 302e 3838  83.480642 130.88
 0000c810: 3638 3137 2033 3838 2e35 3238 3632 3320  6817 388.528623 
 0000c820: 3133 362e 3739 3031 3436 2033 3932 2e31  136.790146 392.1
 0000c830: 3135 3733 3320 0a22 2063 6c69 702d 7061  15733 ." clip-pa
-0000c840: 7468 3d22 7572 6c28 2370 3764 3631 6235  th="url(#p7d61b5
-0000c850: 3539 6161 2922 2073 7479 6c65 3d22 6669  59aa)" style="fi
+0000c840: 7468 3d22 7572 6c28 2370 3336 3762 6264  th="url(#p367bbd
+0000c850: 3436 3063 2922 2073 7479 6c65 3d22 6669  460c)" style="fi
 0000c860: 6c6c 3a20 2366 6666 6664 343b 206f 7061  ll: #ffffd4; opa
 0000c870: 6369 7479 3a20 302e 3422 2f3e 0a20 2020  city: 0.4"/>.   
 0000c880: 3c2f 673e 0a20 2020 3c67 2069 643d 2274  </g>.   <g id="t
 0000c890: 6578 745f 3331 223e 0a20 2020 203c 212d  ext_31">.    <!-
 0000c8a0: 2d20 3133 3237 202d 2d3e 0a20 2020 203c  - 1327 -->.    <
 0000c8b0: 6720 7374 796c 653d 2266 696c 6c3a 2023  g style="fill: #
 0000c8c0: 3236 3236 3236 2220 7472 616e 7366 6f72  262626" transfor
@@ -3471,15 +3471,15 @@
 0000d8e0: 2e31 3134 3739 3920 3336 322e 3535 3836  .114799 362.5586
 0000d8f0: 3437 2034 3032 2e36 3732 3030 3520 0a43  47 402.672005 .C
 0000d900: 2033 3637 2e30 3033 3033 3520 3430 302e   367.003035 400.
 0000d910: 3232 3932 3131 2033 3731 2e30 3630 3520  229211 371.0605 
 0000d920: 3339 372e 3134 3034 3737 2033 3734 2e35  397.140477 374.5
 0000d930: 3938 3334 3520 3339 332e 3530 3638 3137  98345 393.506817
 0000d940: 200a 2220 636c 6970 2d70 6174 683d 2275   ." clip-path="u
-0000d950: 726c 2823 7065 3433 6335 3165 6630 3129  rl(#pe43c51ef01)
+0000d950: 726c 2823 7066 3230 6233 3938 3135 3329  rl(#pf20b398153)
 0000d960: 2220 7374 796c 653d 2266 696c 6c3a 2023  " style="fill: #
 0000d970: 6330 6330 6330 3b20 6f70 6163 6974 793a  c0c0c0; opacity:
 0000d980: 2030 2e34 222f 3e0a 2020 203c 2f67 3e0a   0.4"/>.   </g>.
 0000d990: 2020 203c 6720 6964 3d22 7061 7463 685f     <g id="patch_
 0000d9a0: 3234 223e 0a20 2020 203c 7061 7468 2064  24">.    <path d
 0000d9b0: 3d22 4d20 3337 342e 3539 3833 3435 2033  ="M 374.598345 3
 0000d9c0: 3231 2e39 3731 3236 3620 0a43 2033 3833  21.971266 .C 383
@@ -3522,16 +3522,16 @@
 0000dc10: 3037 3920 3332 332e 3436 3436 3037 2033  079 323.464607 3
 0000dc20: 3930 2e37 3239 3633 3520 3332 322e 3139  90.729635 322.19
 0000dc30: 3131 3636 200a 4320 3338 352e 3433 3631  1166 .C 385.4361
 0000dc40: 3920 3332 302e 3931 3737 3236 2033 3739  9 320.917726 379
 0000dc50: 2e39 3234 3533 3520 3332 302e 3834 3235  .924535 320.8425
 0000dc60: 3931 2033 3734 2e35 3938 3334 3520 3332  91 374.598345 32
 0000dc70: 312e 3937 3132 3636 200a 2220 636c 6970  1.971266 ." clip
-0000dc80: 2d70 6174 683d 2275 726c 2823 7065 3433  -path="url(#pe43
-0000dc90: 6335 3165 6630 3129 2220 7374 796c 653d  c51ef01)" style=
+0000dc80: 2d70 6174 683d 2275 726c 2823 7066 3230  -path="url(#pf20
+0000dc90: 6233 3938 3135 3329 2220 7374 796c 653d  b398153)" style=
 0000dca0: 2266 696c 6c3a 2023 6666 3766 3030 3b20  "fill: #ff7f00; 
 0000dcb0: 6f70 6163 6974 793a 2030 2e34 222f 3e0a  opacity: 0.4"/>.
 0000dcc0: 2020 203c 2f67 3e0a 2020 203c 6720 6964     </g>.   <g id
 0000dcd0: 3d22 7061 7463 685f 3235 223e 0a20 2020  ="patch_25">.   
 0000dce0: 203c 7061 7468 2064 3d22 4d20 3337 342e   <path d="M 374.
 0000dcf0: 3539 3833 3435 2033 3933 2e35 3036 3831  598345 393.50681
 0000dd00: 3720 0a43 2033 3833 2e39 3135 3734 3220  7 .C 383.915742 
@@ -3557,15 +3557,15 @@
 0000de40: 3731 3834 2033 3533 2e37 3730 3937 3120  7184 353.770971 
 0000de50: 3338 302e 3735 3730 3720 0a43 2033 3539  380.75707 .C 359
 0000de60: 2e30 3435 3930 3720 3338 372e 3236 3639  .045907 387.2669
 0000de70: 3536 2033 3636 2e34 3031 3630 3920 3339  56 366.401609 39
 0000de80: 312e 3736 3938 3435 2033 3734 2e35 3938  1.769845 374.598
 0000de90: 3334 3520 3339 332e 3530 3638 3137 200a  345 393.506817 .
 0000dea0: 2220 636c 6970 2d70 6174 683d 2275 726c  " clip-path="url
-0000deb0: 2823 7065 3433 6335 3165 6630 3129 2220  (#pe43c51ef01)" 
+0000deb0: 2823 7066 3230 6233 3938 3135 3329 2220  (#pf20b398153)" 
 0000dec0: 7374 796c 653d 2266 696c 6c3a 2023 6666  style="fill: #ff
 0000ded0: 6466 3836 3b20 6f70 6163 6974 793a 2030  df86; opacity: 0
 0000dee0: 2e34 222f 3e0a 2020 203c 2f67 3e0a 2020  .4"/>.   </g>.  
 0000def0: 203c 6720 6964 3d22 7465 7874 5f33 3622   <g id="text_36"
 0000df00: 3e0a 2020 2020 3c21 2d2d 2031 3139 3620  >.    <!-- 1196 
 0000df10: 2d2d 3e0a 2020 2020 3c67 2073 7479 6c65  -->.    <g style
 0000df20: 3d22 6669 6c6c 3a20 2332 3632 3632 3622  ="fill: #262626"
@@ -4283,15 +4283,15 @@
 00010ba0: 3534 2031 3632 2e39 3032 3835 3520 3533  54 162.902855 53
 00010bb0: 302e 3438 3236 3420 0a43 2031 3636 2e35  0.48264 .C 166.5
 00010bc0: 3139 3936 3820 3532 352e 3333 3939 3236  19968 525.339926
 00010bd0: 2031 3639 2e31 3735 3938 3520 3531 392e   169.175985 519.
 00010be0: 3538 3433 3839 2031 3730 2e37 3432 3038  584389 170.74208
 00010bf0: 3320 3531 332e 3439 3531 3920 0a22 2063  3 513.49519 ." c
 00010c00: 6c69 702d 7061 7468 3d22 7572 6c28 2370  lip-path="url(#p
-00010c10: 3239 3462 6432 3434 3763 2922 2073 7479  294bd2447c)" sty
+00010c10: 3738 3031 3830 6335 3564 2922 2073 7479  780180c55d)" sty
 00010c20: 6c65 3d22 6669 6c6c 3a20 2363 3063 3063  le="fill: #c0c0c
 00010c30: 303b 206f 7061 6369 7479 3a20 302e 3422  0; opacity: 0.4"
 00010c40: 2f3e 0a20 2020 3c2f 673e 0a20 2020 3c67  />.   </g>.   <g
 00010c50: 2069 643d 2270 6174 6368 5f33 3022 3e0a   id="patch_30">.
 00010c60: 2020 2020 3c70 6174 6820 643d 224d 2031      <path d="M 1
 00010c70: 3730 2e37 3432 3038 3320 3438 372e 3535  70.742083 487.55
 00010c80: 3239 200a 4320 3137 312e 3833 3139 3536  29 .C 171.831956
@@ -4317,15 +4317,15 @@
 00010dc0: 3733 3333 2031 3736 2e35 3433 3231 3620  7333 176.543216 
 00010dd0: 3439 322e 3931 3834 3638 200a 4320 3137  492.918468 .C 17
 00010de0: 352e 3134 3131 3934 2034 3930 2e36 3239  5.141194 490.629
 00010df0: 3630 3320 3137 332e 3133 3332 3031 2034  603 173.133201 4
 00010e00: 3838 2e37 3732 3337 3720 3137 302e 3734  88.772377 170.74
 00010e10: 3230 3833 2034 3837 2e35 3532 3920 0a22  2083 487.5529 ."
 00010e20: 2063 6c69 702d 7061 7468 3d22 7572 6c28   clip-path="url(
-00010e30: 2370 3239 3462 6432 3434 3763 2922 2073  #p294bd2447c)" s
+00010e30: 2370 3738 3031 3830 6335 3564 2922 2073  #p780180c55d)" s
 00010e40: 7479 6c65 3d22 6669 6c6c 3a20 2336 6133  tyle="fill: #6a3
 00010e50: 6439 613b 206f 7061 6369 7479 3a20 302e  d9a; opacity: 0.
 00010e60: 3422 2f3e 0a20 2020 3c2f 673e 0a20 2020  4"/>.   </g>.   
 00010e70: 3c67 2069 643d 2270 6174 6368 5f33 3122  <g id="patch_31"
 00010e80: 3e0a 2020 2020 3c70 6174 6820 643d 224d  >.    <path d="M
 00010e90: 2031 3730 2e37 3432 3038 3320 3531 332e   170.742083 513.
 00010ea0: 3439 3531 3920 0a43 2031 3731 2e38 3331  49519 .C 171.831
@@ -4368,15 +4368,15 @@
 000110f0: 2e39 3736 3533 3420 3136 332e 3535 3932  .976534 163.5592
 00011100: 3439 2035 3135 2e30 3733 3634 3820 0a43  49 515.073648 .C
 00011110: 2031 3636 2e30 3438 3938 2035 3135 2e31   166.04898 515.1
 00011120: 3730 3736 3120 3136 382e 3532 3234 3539  70761 168.522459
 00011130: 2035 3134 2e36 3237 3230 3420 3137 302e   514.627204 170.
 00011140: 3734 3230 3833 2035 3133 2e34 3935 3139  742083 513.49519
 00011150: 200a 2220 636c 6970 2d70 6174 683d 2275   ." clip-path="u
-00011160: 726c 2823 7032 3934 6264 3234 3437 6329  rl(#p294bd2447c)
+00011160: 726c 2823 7037 3830 3138 3063 3535 6429  rl(#p780180c55d)
 00011170: 2220 7374 796c 653d 2266 696c 6c3a 2023  " style="fill: #
 00011180: 6431 6231 6632 3b20 6f70 6163 6974 793a  d1b1f2; opacity:
 00011190: 2030 2e34 222f 3e0a 2020 203c 2f67 3e0a   0.4"/>.   </g>.
 000111a0: 2020 203c 6720 6964 3d22 7465 7874 5f34     <g id="text_4
 000111b0: 3622 3e0a 2020 2020 3c21 2d2d 2031 3534  6">.    <!-- 154
 000111c0: 3420 2d2d 3e0a 2020 2020 3c67 2073 7479  4 -->.    <g sty
 000111d0: 6c65 3d22 6669 6c6c 3a20 2332 3632 3632  le="fill: #26262
@@ -4614,16 +4614,16 @@
 00012050: 362e 3430 3534 3935 2033 3839 2e31 3031  6.405495 389.101
 00012060: 3032 3620 3533 312e 3339 3535 3531 200a  026 531.395551 .
 00012070: 4320 3339 322e 3739 3531 3733 2035 3236  C 392.795173 526
 00012080: 2e33 3835 3630 3820 3339 352e 3536 3032  .385608 395.5602
 00012090: 3536 2035 3230 2e37 3533 3032 3420 3339  56 520.753024 39
 000120a0: 372e 3236 3435 3033 2035 3134 2e37 3636  7.264503 514.766
 000120b0: 3232 3220 0a22 2063 6c69 702d 7061 7468  222 ." clip-path
-000120c0: 3d22 7572 6c28 2370 6432 3134 3361 6561  ="url(#pd2143aea
-000120d0: 3333 2922 2073 7479 6c65 3d22 6669 6c6c  33)" style="fill
+000120c0: 3d22 7572 6c28 2370 3665 3766 3966 6461  ="url(#p6e7f9fda
+000120d0: 3932 2922 2073 7479 6c65 3d22 6669 6c6c  92)" style="fill
 000120e0: 3a20 2363 3063 3063 303b 206f 7061 6369  : #c0c0c0; opaci
 000120f0: 7479 3a20 302e 3422 2f3e 0a20 2020 3c2f  ty: 0.4"/>.   </
 00012100: 673e 0a20 2020 3c67 2069 643d 2270 6174  g>.   <g id="pat
 00012110: 6368 5f33 3322 3e0a 2020 2020 3c70 6174  ch_33">.    <pat
 00012120: 6820 643d 224d 2033 3937 2e32 3634 3530  h d="M 397.26450
 00012130: 3320 3438 362e 3238 3138 3638 200a 4320  3 486.281868 .C 
 00012140: 3339 382e 3538 3332 3131 2034 3930 2e39  398.583211 490.9
@@ -4648,16 +4648,16 @@
 00012270: 3520 3439 332e 3536 3239 3235 2034 3036  5 493.562925 406
 00012280: 2e34 3236 3838 3920 3439 302e 3933 3330  .426889 490.9330
 00012290: 3331 200a 4320 3430 342e 3035 3431 3534  31 .C 404.054154
 000122a0: 2034 3838 2e33 3033 3133 3620 3430 302e   488.303136 400.
 000122b0: 3738 3738 3938 2034 3836 2e36 3435 3036  787898 486.64506
 000122c0: 3520 3339 372e 3236 3435 3033 2034 3836  5 397.264503 486
 000122d0: 2e32 3831 3836 3820 0a22 2063 6c69 702d  .281868 ." clip-
-000122e0: 7061 7468 3d22 7572 6c28 2370 6432 3134  path="url(#pd214
-000122f0: 3361 6561 3333 2922 2073 7479 6c65 3d22  3aea33)" style="
+000122e0: 7061 7468 3d22 7572 6c28 2370 3665 3766  path="url(#p6e7f
+000122f0: 3966 6461 3932 2922 2073 7479 6c65 3d22  9fda92)" style="
 00012300: 6669 6c6c 3a20 2366 6666 6639 393b 206f  fill: #ffff99; o
 00012310: 7061 6369 7479 3a20 302e 3422 2f3e 0a20  pacity: 0.4"/>. 
 00012320: 2020 3c2f 673e 0a20 2020 3c67 2069 643d    </g>.   <g id=
 00012330: 2270 6174 6368 5f33 3422 3e0a 2020 2020  "patch_34">.    
 00012340: 3c70 6174 6820 643d 224d 2033 3937 2e32  <path d="M 397.2
 00012350: 3634 3530 3320 3531 342e 3736 3632 3232  64503 514.766222
 00012360: 200a 4320 3339 382e 3538 3332 3131 2035   .C 398.583211 5
@@ -4700,15 +4700,15 @@
 000125b0: 3132 3135 3420 3339 312e 3335 3135 3731  12154 391.351571
 000125c0: 2035 3134 2e31 3334 3237 3920 0a43 2033   514.134279 .C 3
 000125d0: 3933 2e32 3536 3534 3320 3531 342e 3735  93.256543 514.75
 000125e0: 3634 3035 2033 3935 2e32 3731 3038 2035  6405 395.27108 5
 000125f0: 3134 2e39 3731 3730 3820 3339 372e 3236  14.971708 397.26
 00012600: 3435 3033 2035 3134 2e37 3636 3232 3220  4503 514.766222 
 00012610: 0a22 2063 6c69 702d 7061 7468 3d22 7572  ." clip-path="ur
-00012620: 6c28 2370 6432 3134 3361 6561 3333 2922  l(#pd2143aea33)"
+00012620: 6c28 2370 3665 3766 3966 6461 3932 2922  l(#p6e7f9fda92)"
 00012630: 2073 7479 6c65 3d22 6669 6c6c 3a20 2366   style="fill: #f
 00012640: 6666 6666 323b 206f 7061 6369 7479 3a20  ffff2; opacity: 
 00012650: 302e 3422 2f3e 0a20 2020 3c2f 673e 0a20  0.4"/>.   </g>. 
 00012660: 2020 3c67 2069 643d 2274 6578 745f 3531    <g id="text_51
 00012670: 223e 0a20 2020 203c 212d 2d20 3135 3732  ">.    <!-- 1572
 00012680: 202d 2d3e 0a20 2020 203c 6720 7374 796c   -->.    <g styl
 00012690: 653d 2266 696c 6c3a 2023 3236 3236 3236  e="fill: #262626
@@ -4915,16 +4915,16 @@
 00013320: 3033 3920 3533 382e 3134 3637 3132 2036  039 538.146712 6
 00013330: 3134 2e36 3839 3032 3720 3533 332e 3433  14.689027 533.43
 00013340: 3633 3332 200a 4320 3631 382e 3534 3730  6332 .C 618.5470
 00013350: 3134 2035 3238 2e37 3235 3935 3320 3632  14 528.725953 62
 00013360: 312e 3534 3638 3937 2035 3233 2e33 3733  1.546897 523.373
 00013370: 3720 3632 332e 3535 3134 3134 2035 3137  7 623.551414 517
 00013380: 2e36 3234 3436 3920 0a22 2063 6c69 702d  .624469 ." clip-
-00013390: 7061 7468 3d22 7572 6c28 2370 6532 6363  path="url(#pe2cc
-000133a0: 6334 6537 3532 2922 2073 7479 6c65 3d22  c4e752)" style="
+00013390: 7061 7468 3d22 7572 6c28 2370 3465 3235  path="url(#p4e25
+000133a0: 3131 3766 3932 2922 2073 7479 6c65 3d22  117f92)" style="
 000133b0: 6669 6c6c 3a20 2363 3063 3063 303b 206f  fill: #c0c0c0; o
 000133c0: 7061 6369 7479 3a20 302e 3422 2f3e 0a20  pacity: 0.4"/>. 
 000133d0: 2020 3c2f 673e 0a20 2020 3c67 2069 643d    </g>.   <g id=
 000133e0: 2270 6174 6368 5f33 3622 3e0a 2020 2020  "patch_36">.    
 000133f0: 3c70 6174 6820 643d 224d 2036 3233 2e35  <path d="M 623.5
 00013400: 3531 3431 3420 3438 332e 3432 3336 3231  51414 483.423621
 00013410: 200a 4320 3632 352e 3436 3831 3634 2034   .C 625.468164 4
@@ -4967,15 +4967,15 @@
 00013660: 3239 3137 2036 3330 2e32 3534 3730 3120  2917 630.254701 
 00013670: 3438 342e 3537 3435 3339 200a 4320 3632  484.574539 .C 62
 00013680: 382e 3131 3938 3731 2034 3833 2e37 3436  8.119871 483.746
 00013690: 3136 2036 3235 2e38 3430 3239 3320 3438  16 625.840293 48
 000136a0: 332e 3335 3437 3639 2036 3233 2e35 3531  3.354769 623.551
 000136b0: 3431 3420 3438 332e 3432 3336 3231 200a  414 483.423621 .
 000136c0: 2220 636c 6970 2d70 6174 683d 2275 726c  " clip-path="url
-000136d0: 2823 7065 3263 6363 3465 3735 3229 2220  (#pe2ccc4e752)" 
+000136d0: 2823 7034 6532 3531 3137 6639 3229 2220  (#p4e25117f92)" 
 000136e0: 7374 796c 653d 2266 696c 6c3a 2023 6231  style="fill: #b1
 000136f0: 3539 3238 3b20 6f70 6163 6974 793a 2030  5928; opacity: 0
 00013700: 2e34 222f 3e0a 2020 203c 2f67 3e0a 2020  .4"/>.   </g>.  
 00013710: 203c 6720 6964 3d22 7061 7463 685f 3337   <g id="patch_37
 00013720: 223e 0a20 2020 203c 7061 7468 2064 3d22  ">.    <path d="
 00013730: 4d20 3632 332e 3535 3134 3134 2035 3137  M 623.551414 517
 00013740: 2e36 3234 3436 3920 0a43 2036 3235 2e34  .624469 .C 625.4
@@ -5001,16 +5001,16 @@
 00013880: 3530 392e 3234 3638 3631 2036 3131 2e37  509.246861 611.7
 00013890: 3837 3939 3620 3531 322e 3433 3830 3835  87996 512.438085
 000138a0: 200a 4320 3631 342e 3838 3436 3638 2035   .C 614.884668 5
 000138b0: 3135 2e36 3239 3330 3920 3631 392e 3130  15.629309 619.10
 000138c0: 3637 3038 2035 3137 2e34 3930 3736 3820  6708 517.490768 
 000138d0: 3632 332e 3535 3134 3134 2035 3137 2e36  623.551414 517.6
 000138e0: 3234 3436 3920 0a22 2063 6c69 702d 7061  24469 ." clip-pa
-000138f0: 7468 3d22 7572 6c28 2370 6532 6363 6334  th="url(#pe2ccc4
-00013900: 6537 3532 2922 2073 7479 6c65 3d22 6669  e752)" style="fi
+000138f0: 7468 3d22 7572 6c28 2370 3465 3235 3131  th="url(#p4e2511
+00013900: 3766 3932 2922 2073 7479 6c65 3d22 6669  7f92)" style="fi
 00013910: 6c6c 3a20 2366 6663 3561 323b 206f 7061  ll: #ffc5a2; opa
 00013920: 6369 7479 3a20 302e 3422 2f3e 0a20 2020  city: 0.4"/>.   
 00013930: 3c2f 673e 0a20 2020 3c67 2069 643d 2274  </g>.   <g id="t
 00013940: 6578 745f 3536 223e 0a20 2020 203c 212d  ext_56">.    <!-
 00013950: 2d20 3135 3531 202d 2d3e 0a20 2020 203c  - 1551 -->.    <
 00013960: 6720 7374 796c 653d 2266 696c 6c3a 2023  g style="fill: #
 00013970: 3236 3236 3236 2220 7472 616e 7366 6f72  262626" transfor
@@ -5265,16 +5265,16 @@
 00014900: 2036 3738 2e36 3132 3232 3320 3136 322e   678.612223 162.
 00014910: 3139 3439 3037 2036 3733 2e35 3032 3935  194907 673.50295
 00014920: 3220 0a43 2031 3635 2e38 3332 3137 3420  2 .C 165.832174 
 00014930: 3636 382e 3339 3336 3831 2031 3638 2e35  668.393681 168.5
 00014940: 3136 3436 3720 3636 322e 3636 3839 3633  16467 662.668963
 00014950: 2031 3730 2e31 3138 3137 3320 3635 362e   170.118173 656.
 00014960: 3630 3532 3237 200a 2220 636c 6970 2d70  605227 ." clip-p
-00014970: 6174 683d 2275 726c 2823 7037 6534 3038  ath="url(#p7e408
-00014980: 6266 3238 6529 2220 7374 796c 653d 2266  bf28e)" style="f
+00014970: 6174 683d 2275 726c 2823 7039 3661 3530  ath="url(#p96a50
+00014980: 3331 6262 3829 2220 7374 796c 653d 2266  31bb8)" style="f
 00014990: 696c 6c3a 2023 6330 6330 6330 3b20 6f70  ill: #c0c0c0; op
 000149a0: 6163 6974 793a 2030 2e34 222f 3e0a 2020  acity: 0.4"/>.  
 000149b0: 203c 2f67 3e0a 2020 203c 6720 6964 3d22   </g>.   <g id="
 000149c0: 7061 7463 685f 3339 223e 0a20 2020 203c  patch_39">.    <
 000149d0: 7061 7468 2064 3d22 4d20 3137 302e 3131  path d="M 170.11
 000149e0: 3831 3733 2036 3330 2e30 3132 3837 200a  8173 630.01287 .
 000149f0: 4320 3137 312e 3236 3433 3236 2036 3334  C 171.264326 634
@@ -5300,15 +5300,15 @@
 00014b30: 3320 3137 362e 3731 3436 3939 2036 3335  3 176.714699 635
 00014b40: 2e32 3537 3339 3420 0a43 2031 3735 2e30  .257394 .C 175.0
 00014b50: 3934 3036 3320 3633 322e 3838 3534 3134  94063 632.885414
 00014b60: 2031 3732 2e37 3934 3432 3520 3633 312e   172.794425 631.
 00014b70: 3035 3731 3032 2031 3730 2e31 3138 3137  057102 170.11817
 00014b80: 3320 3633 302e 3031 3238 3720 0a22 2063  3 630.01287 ." c
 00014b90: 6c69 702d 7061 7468 3d22 7572 6c28 2370  lip-path="url(#p
-00014ba0: 3765 3430 3862 6632 3865 2922 2073 7479  7e408bf28e)" sty
+00014ba0: 3936 6135 3033 3162 6238 2922 2073 7479  96a5031bb8)" sty
 00014bb0: 6c65 3d22 6669 6c6c 3a20 2361 3663 6565  le="fill: #a6cee
 00014bc0: 333b 206f 7061 6369 7479 3a20 302e 3422  3; opacity: 0.4"
 00014bd0: 2f3e 0a20 2020 3c2f 673e 0a20 2020 3c67  />.   </g>.   <g
 00014be0: 2069 643d 2270 6174 6368 5f34 3022 3e0a   id="patch_40">.
 00014bf0: 2020 2020 3c70 6174 6820 643d 224d 2031      <path d="M 1
 00014c00: 3730 2e31 3138 3137 3320 3635 362e 3630  70.118173 656.60
 00014c10: 3532 3237 200a 4320 3137 312e 3236 3433  5227 .C 171.2643
@@ -5351,15 +5351,15 @@
 00014e60: 2e32 3235 3936 3620 3136 332e 3331 3131  .225966 163.3111
 00014e70: 3120 3635 372e 3438 3933 3831 200a 4320  1 657.489381 .C 
 00014e80: 3136 352e 3631 3831 3434 2036 3537 2e37  165.618144 657.7
 00014e90: 3532 3739 3620 3136 372e 3935 3439 3834  52796 167.954984
 00014ea0: 2036 3537 2e34 3439 3236 3920 3137 302e   657.449269 170.
 00014eb0: 3131 3831 3733 2036 3536 2e36 3035 3232  118173 656.60522
 00014ec0: 3720 0a22 2063 6c69 702d 7061 7468 3d22  7 ." clip-path="
-00014ed0: 7572 6c28 2370 3765 3430 3862 6632 3865  url(#p7e408bf28e
+00014ed0: 7572 6c28 2370 3936 6135 3033 3162 6238  url(#p96a5031bb8
 00014ee0: 2922 2073 7479 6c65 3d22 6669 6c6c 3a20  )" style="fill: 
 00014ef0: 2366 6266 6666 663b 206f 7061 6369 7479  #fbffff; opacity
 00014f00: 3a20 302e 3422 2f3e 0a20 2020 3c2f 673e  : 0.4"/>.   </g>
 00014f10: 0a20 2020 3c67 2069 643d 2274 6578 745f  .   <g id="text_
 00014f20: 3631 223e 0a20 2020 203c 212d 2d20 3135  61">.    <!-- 15
 00014f30: 3534 202d 2d3e 0a20 2020 203c 6720 7374  54 -->.    <g st
 00014f40: 796c 653d 2266 696c 6c3a 2023 3236 3236  yle="fill: #2626
@@ -6314,16 +6314,16 @@
 00018a90: 3637 2038 3331 2e37 3433 3930 3820 3132  67 831.743908 12
 00018aa0: 392e 3637 3037 3336 2038 3238 2e39 3339  9.670736 828.939
 00018ab0: 3635 3720 0a43 2031 3334 2e30 3436 3830  657 .C 134.04680
 00018ac0: 3320 3832 362e 3133 3534 3035 2031 3337  3 826.135405 137
 00018ad0: 2e39 3637 3533 3220 3832 322e 3637 3732  .967532 822.6772
 00018ae0: 3034 2031 3431 2e32 3936 3239 2038 3138  04 141.29629 818
 00018af0: 2e36 3835 3536 3820 0a22 2063 6c69 702d  .685568 ." clip-
-00018b00: 7061 7468 3d22 7572 6c28 2370 6434 3166  path="url(#pd41f
-00018b10: 3237 3161 3535 2922 2073 7479 6c65 3d22  271a55)" style="
+00018b00: 7061 7468 3d22 7572 6c28 2370 6538 3132  path="url(#pe812
+00018b10: 6666 3134 3265 2922 2073 7479 6c65 3d22  ff142e)" style="
 00018b20: 6669 6c6c 3a20 2363 3063 3063 303b 206f  fill: #c0c0c0; o
 00018b30: 7061 6369 7479 3a20 302e 3422 2f3e 0a20  pacity: 0.4"/>. 
 00018b40: 2020 3c2f 673e 0a20 2020 3c67 2069 643d    </g>.   <g id=
 00018b50: 2270 6174 6368 5f34 3822 3e0a 2020 2020  "patch_48">.    
 00018b60: 3c70 6174 6820 643d 224d 2031 3431 2e32  <path d="M 141.2
 00018b70: 3936 3239 2037 3533 2e35 3032 3533 3520  9629 753.502535 
 00018b80: 0a43 2031 3438 2e39 3232 3831 3720 3736  .C 148.922817 76
@@ -6365,16 +6365,16 @@
 00018dc0: 3937 3930 3138 2037 3439 2e33 3338 3232  979018 749.33822
 00018dd0: 2031 3539 2e36 3035 3237 3820 3734 392e   159.605278 749.
 00018de0: 3137 3537 3333 200a 4320 3135 332e 3233  175733 .C 153.23
 00018df0: 3135 3338 2037 3439 2e30 3133 3234 3520  1538 749.013245 
 00018e00: 3134 362e 3932 3330 3332 2037 3530 2e35  146.923032 750.5
 00018e10: 3034 3037 3920 3134 312e 3239 3632 3920  04079 141.29629 
 00018e20: 3735 332e 3530 3235 3335 200a 2220 636c  753.502535 ." cl
-00018e30: 6970 2d70 6174 683d 2275 726c 2823 7064  ip-path="url(#pd
-00018e40: 3431 6632 3731 6135 3529 2220 7374 796c  41f271a55)" styl
+00018e30: 6970 2d70 6174 683d 2275 726c 2823 7065  ip-path="url(#pe
+00018e40: 3831 3266 6631 3432 6529 2220 7374 796c  812ff142e)" styl
 00018e50: 653d 2266 696c 6c3a 2023 3333 6130 3263  e="fill: #33a02c
 00018e60: 3b20 6f70 6163 6974 793a 2030 2e34 222f  ; opacity: 0.4"/
 00018e70: 3e0a 2020 203c 2f67 3e0a 2020 203c 6720  >.   </g>.   <g 
 00018e80: 6964 3d22 7061 7463 685f 3439 223e 0a20  id="patch_49">. 
 00018e90: 2020 203c 7061 7468 2064 3d22 4d20 3134     <path d="M 14
 00018ea0: 312e 3239 3632 3920 3831 382e 3638 3535  1.29629 818.6855
 00018eb0: 3638 200a 4320 3134 382e 3932 3238 3137  68 .C 148.922817
@@ -6399,16 +6399,16 @@
 00018fe0: 3534 3336 2037 3939 2e33 3539 3635 3620  5436 799.359656 
 00018ff0: 3132 362e 3939 3938 3738 2038 3035 2e30  126.999878 805.0
 00019000: 3939 3936 200a 4320 3133 302e 3434 3533  9996 .C 130.4453
 00019010: 3936 2038 3130 2e38 3430 3236 3320 3133  96 810.840263 13
 00019020: 352e 3338 3738 3832 2038 3135 2e35 3337  5.387882 815.537
 00019030: 3031 3420 3134 312e 3239 3632 3920 3831  014 141.29629 81
 00019040: 382e 3638 3535 3638 200a 2220 636c 6970  8.685568 ." clip
-00019050: 2d70 6174 683d 2275 726c 2823 7064 3431  -path="url(#pd41
-00019060: 6632 3731 6135 3529 2220 7374 796c 653d  f271a55)" style=
+00019050: 2d70 6174 683d 2275 726c 2823 7065 3831  -path="url(#pe81
+00019060: 3266 6631 3432 6529 2220 7374 796c 653d  2ff142e)" style=
 00019070: 2266 696c 6c3a 2023 6161 6636 6135 3b20  "fill: #aaf6a5; 
 00019080: 6f70 6163 6974 793a 2030 2e34 222f 3e0a  opacity: 0.4"/>.
 00019090: 2020 203c 2f67 3e0a 2020 203c 6720 6964     </g>.   <g id
 000190a0: 3d22 7465 7874 5f37 3622 3e0a 2020 2020  ="text_76">.    
 000190b0: 3c21 2d2d 2031 3335 3920 2d2d 3e0a 2020  <!-- 1359 -->.  
 000190c0: 2020 3c67 2073 7479 6c65 3d22 6669 6c6c    <g style="fill
 000190d0: 3a20 2332 3632 3632 3622 2074 7261 6e73  : #262626" trans
@@ -6670,16 +6670,16 @@
 0001a0d0: 3232 2e37 3238 3531 2033 3836 2e30 3034  22.72851 386.004
 0001a0e0: 3138 3520 3831 372e 3835 3433 3831 200a  185 817.854381 .
 0001a0f0: 4320 3338 392e 3737 3033 3838 2038 3132  C 389.770388 812
 0001a100: 2e39 3830 3235 3320 3339 322e 3633 3937  .980253 392.6397
 0001a110: 3637 2038 3037 2e34 3734 3834 3820 3339  67 807.474848 39
 0001a120: 342e 3437 3830 3034 2038 3031 2e35 3935  4.478004 801.595
 0001a130: 3837 3720 0a22 2063 6c69 702d 7061 7468  877 ." clip-path
-0001a140: 3d22 7572 6c28 2370 3233 3930 3431 3534  ="url(#p23904154
-0001a150: 6437 2922 2073 7479 6c65 3d22 6669 6c6c  d7)" style="fill
+0001a140: 3d22 7572 6c28 2370 6334 3065 6430 3335  ="url(#pc40ed035
+0001a150: 6333 2922 2073 7479 6c65 3d22 6669 6c6c  c3)" style="fill
 0001a160: 3a20 2363 3063 3063 303b 206f 7061 6369  : #c0c0c0; opaci
 0001a170: 7479 3a20 302e 3422 2f3e 0a20 2020 3c2f  ty: 0.4"/>.   </
 0001a180: 673e 0a20 2020 3c67 2069 643d 2270 6174  g>.   <g id="pat
 0001a190: 6368 5f35 3122 3e0a 2020 2020 3c70 6174  ch_51">.    <pat
 0001a1a0: 6820 643d 224d 2033 3934 2e34 3738 3030  h d="M 394.47800
 0001a1b0: 3420 3737 302e 3539 3232 3236 200a 4320  4 770.592226 .C 
 0001a1c0: 3339 362e 3034 3639 3332 2037 3735 2e36  396.046932 775.6
@@ -6721,16 +6721,16 @@
 0001a400: 3237 2037 3731 2e36 3938 3031 3520 3430  27 771.698015 40
 0001a410: 312e 3132 3034 3132 2037 3731 2e30 3635  1.120412 771.065
 0001a420: 3833 3420 0a43 2033 3938 2e39 3635 3839  834 .C 398.96589
 0001a430: 3820 3737 302e 3433 3336 3532 2033 3936  8 770.433652 396
 0001a440: 2e37 3030 3431 3720 3737 302e 3237 3231  .700417 770.2721
 0001a450: 3232 2033 3934 2e34 3738 3030 3420 3737  22 394.478004 77
 0001a460: 302e 3539 3232 3236 200a 2220 636c 6970  0.592226 ." clip
-0001a470: 2d70 6174 683d 2275 726c 2823 7032 3339  -path="url(#p239
-0001a480: 3034 3135 3464 3729 2220 7374 796c 653d  04154d7)" style=
+0001a470: 2d70 6174 683d 2275 726c 2823 7063 3430  -path="url(#pc40
+0001a480: 6564 3033 3563 3329 2220 7374 796c 653d  ed035c3)" style=
 0001a490: 2266 696c 6c3a 2023 6662 3961 3939 3b20  "fill: #fb9a99; 
 0001a4a0: 6f70 6163 6974 793a 2030 2e34 222f 3e0a  opacity: 0.4"/>.
 0001a4b0: 2020 203c 2f67 3e0a 2020 203c 6720 6964     </g>.   <g id
 0001a4c0: 3d22 7061 7463 685f 3532 223e 0a20 2020  ="patch_52">.   
 0001a4d0: 203c 7061 7468 2064 3d22 4d20 3339 342e   <path d="M 394.
 0001a4e0: 3437 3830 3034 2038 3031 2e35 3935 3837  478004 801.59587
 0001a4f0: 3720 0a43 2033 3936 2e30 3436 3933 3220  7 .C 396.046932 
@@ -6756,15 +6756,15 @@
 0001a630: 3434 2033 3834 2e38 3733 3131 3820 3739  44 384.873118 79
 0001a640: 362e 3334 3838 3633 200a 4320 3338 372e  6.348863 .C 387.
 0001a650: 3333 3839 3238 2037 3939 2e31 3935 3238  338928 799.19528
 0001a660: 3220 3339 302e 3735 3035 3239 2038 3031  2 390.750529 801
 0001a670: 2e30 3538 3939 3120 3339 342e 3437 3830  .058991 394.4780
 0001a680: 3034 2038 3031 2e35 3935 3837 3720 0a22  04 801.595877 ."
 0001a690: 2063 6c69 702d 7061 7468 3d22 7572 6c28   clip-path="url(
-0001a6a0: 2370 3233 3930 3431 3534 6437 2922 2073  #p23904154d7)" s
+0001a6a0: 2370 6334 3065 6430 3335 6333 2922 2073  #pc40ed035c3)" s
 0001a6b0: 7479 6c65 3d22 6669 6c6c 3a20 2366 6666  tyle="fill: #fff
 0001a6c0: 3266 323b 206f 7061 6369 7479 3a20 302e  2f2; opacity: 0.
 0001a6d0: 3422 2f3e 0a20 2020 3c2f 673e 0a20 2020  4"/>.   </g>.   
 0001a6e0: 3c67 2069 643d 2274 6578 745f 3831 223e  <g id="text_81">
 0001a6f0: 0a20 2020 203c 212d 2d20 3135 3739 202d  .    <!-- 1579 -
 0001a700: 2d3e 0a20 2020 203c 6720 7374 796c 653d  ->.    <g style=
 0001a710: 2266 696c 6c3a 2023 3236 3236 3236 2220  "fill: #262626" 
@@ -7302,16 +7302,16 @@
 0001c850: 3820 3937 392e 3738 3639 2031 3032 2e32  8 979.7869 102.2
 0001c860: 3638 3936 3220 3937 372e 3934 3236 3336  68962 977.942636
 0001c870: 200a 4320 3131 312e 3932 3837 3935 2039   .C 111.928795 9
 0001c880: 3736 2e30 3938 3337 3220 3132 302e 3833  76.098372 120.83
 0001c890: 3231 3832 2039 3731 2e34 3431 3734 3220  2182 971.441742 
 0001c8a0: 3132 372e 3835 3731 3036 2039 3634 2e35  127.857106 964.5
 0001c8b0: 3539 3538 3220 0a22 2063 6c69 702d 7061  59582 ." clip-pa
-0001c8c0: 7468 3d22 7572 6c28 2370 6563 3935 6236  th="url(#pec95b6
-0001c8d0: 3335 3762 2922 2073 7479 6c65 3d22 6669  357b)" style="fi
+0001c8c0: 7468 3d22 7572 6c28 2370 3237 6561 6465  th="url(#p27eade
+0001c8d0: 3034 3538 2922 2073 7479 6c65 3d22 6669  0458)" style="fi
 0001c8e0: 6c6c 3a20 2363 3063 3063 303b 206f 7061  ll: #c0c0c0; opa
 0001c8f0: 6369 7479 3a20 302e 3422 2f3e 0a20 2020  city: 0.4"/>.   
 0001c900: 3c2f 673e 0a20 2020 3c67 2069 643d 2270  </g>.   <g id="p
 0001c910: 6174 6368 5f35 3722 3e0a 2020 2020 3c70  atch_57">.    <p
 0001c920: 6174 6820 643d 224d 2031 3237 2e38 3537  ath d="M 127.857
 0001c930: 3130 3620 3839 332e 3139 3835 3238 200a  106 893.198528 .
 0001c940: 4320 3133 322e 3630 3432 3637 2038 3937  C 132.604267 897
@@ -7362,16 +7362,16 @@
 0001cc10: 3836 3838 2038 3831 2e37 3134 3131 3820  8688 881.714118 
 0001cc20: 3135 312e 3633 3134 3832 2038 3832 2e38  151.631482 882.8
 0001cc30: 3338 3533 3520 0a43 2031 3432 2e38 3834  38535 .C 142.884
 0001cc40: 3237 3620 3838 332e 3936 3239 3532 2031  276 883.962952 1
 0001cc50: 3334 2e36 3336 3032 3520 3838 372e 3535  34.636025 887.55
 0001cc60: 3732 3335 2031 3237 2e38 3537 3130 3620  7235 127.857106 
 0001cc70: 3839 332e 3139 3835 3238 200a 2220 636c  893.198528 ." cl
-0001cc80: 6970 2d70 6174 683d 2275 726c 2823 7065  ip-path="url(#pe
-0001cc90: 6339 3562 3633 3537 6229 2220 7374 796c  c95b6357b)" styl
+0001cc80: 6970 2d70 6174 683d 2275 726c 2823 7032  ip-path="url(#p2
+0001cc90: 3765 6164 6530 3435 3829 2220 7374 796c  7eade0458)" styl
 0001cca0: 653d 2266 696c 6c3a 2023 6664 6266 3666  e="fill: #fdbf6f
 0001ccb0: 3b20 6f70 6163 6974 793a 2030 2e34 222f  ; opacity: 0.4"/
 0001ccc0: 3e0a 2020 203c 2f67 3e0a 2020 203c 6720  >.   </g>.   <g 
 0001ccd0: 6964 3d22 7061 7463 685f 3538 223e 0a20  id="patch_58">. 
 0001cce0: 2020 203c 7061 7468 2064 3d22 4d20 3132     <path d="M 12
 0001ccf0: 372e 3835 3731 3036 2039 3634 2e35 3539  7.857106 964.559
 0001cd00: 3538 3220 0a43 2031 3332 2e36 3034 3236  582 .C 132.60426
@@ -7405,16 +7405,16 @@
 0001cec0: 2039 3432 2e34 3136 3330 3420 3131 352e   942.416304 115.
 0001ced0: 3531 3936 3233 2039 3438 2e35 3832 3336  519623 948.58236
 0001cee0: 3120 0a43 2031 3138 2e34 3130 3230 3520  1 .C 118.410205 
 0001cef0: 3935 342e 3734 3834 3137 2031 3232 2e36  954.748417 122.6
 0001cf00: 3232 3537 3820 3936 302e 3230 3335 3031  22578 960.203501
 0001cf10: 2031 3237 2e38 3537 3130 3620 3936 342e   127.857106 964.
 0001cf20: 3535 3935 3832 200a 2220 636c 6970 2d70  559582 ." clip-p
-0001cf30: 6174 683d 2275 726c 2823 7065 6339 3562  ath="url(#pec95b
-0001cf40: 3633 3537 6229 2220 7374 796c 653d 2266  6357b)" style="f
+0001cf30: 6174 683d 2275 726c 2823 7032 3765 6164  ath="url(#p27ead
+0001cf40: 6530 3435 3829 2220 7374 796c 653d 2266  e0458)" style="f
 0001cf50: 696c 6c3a 2023 6666 6666 6434 3b20 6f70  ill: #ffffd4; op
 0001cf60: 6163 6974 793a 2030 2e34 222f 3e0a 2020  acity: 0.4"/>.  
 0001cf70: 203c 2f67 3e0a 2020 203c 6720 6964 3d22   </g>.   <g id="
 0001cf80: 7465 7874 5f39 3122 3e0a 2020 2020 3c21  text_91">.    <!
 0001cf90: 2d2d 2031 3332 3020 2d2d 3e0a 2020 2020  -- 1320 -->.    
 0001cfa0: 3c67 2073 7479 6c65 3d22 6669 6c6c 3a20  <g style="fill: 
 0001cfb0: 2332 3632 3632 3622 2074 7261 6e73 666f  #262626" transfo
@@ -7725,16 +7725,16 @@
 0001e2c0: 3737 3720 3935 372e 3937 3032 3635 2033  777 957.970265 3
 0001e2d0: 3938 2e39 3039 3937 3320 3935 312e 3938  98.909973 951.98
 0001e2e0: 3335 3033 200a 4320 3430 312e 3837 3031  3503 .C 401.8701
 0001e2f0: 3638 2039 3435 2e39 3936 3734 3220 3430  68 945.996742 40
 0001e300: 332e 3635 3234 3120 3933 392e 3439 3634  3.65241 939.4964
 0001e310: 3838 2034 3034 2e31 3539 3532 3920 3933  88 404.159529 93
 0001e320: 322e 3833 3731 3431 200a 2220 636c 6970  2.837141 ." clip
-0001e330: 2d70 6174 683d 2275 726c 2823 7064 6239  -path="url(#pdb9
-0001e340: 3138 6536 3736 6529 2220 7374 796c 653d  18e676e)" style=
+0001e330: 2d70 6174 683d 2275 726c 2823 7066 6131  -path="url(#pfa1
+0001e340: 6362 6436 3263 6329 2220 7374 796c 653d  cbd62cc)" style=
 0001e350: 2266 696c 6c3a 2023 6330 6330 6330 3b20  "fill: #c0c0c0; 
 0001e360: 6f70 6163 6974 793a 2030 2e34 222f 3e0a  opacity: 0.4"/>.
 0001e370: 2020 203c 2f67 3e0a 2020 203c 6720 6964     </g>.   <g id
 0001e380: 3d22 7061 7463 685f 3630 223e 0a20 2020  ="patch_60">.   
 0001e390: 203c 7061 7468 2064 3d22 4d20 3430 342e   <path d="M 404.
 0001e3a0: 3135 3935 3239 2039 3234 2e39 3230 3936  159529 924.92096
 0001e3b0: 3920 0a43 2034 3034 2e32 3539 3831 3920  9 .C 404.259819 
@@ -7751,16 +7751,16 @@
 0001e460: 3933 302e 3237 3535 3931 2034 3035 2e32  930.275591 405.2
 0001e470: 3732 3935 3220 3932 382e 3837 3930 3535  72952 928.879055
 0001e480: 200a 4320 3430 352e 3237 3239 3532 2039   .C 405.272952 9
 0001e490: 3237 2e34 3832 3531 3920 3430 342e 3838  27.482519 404.88
 0001e4a0: 3736 3135 2039 3236 2e31 3132 3639 3220  7615 926.112692 
 0001e4b0: 3430 342e 3135 3935 3239 2039 3234 2e39  404.159529 924.9
 0001e4c0: 3230 3936 3920 0a22 2063 6c69 702d 7061  20969 ." clip-pa
-0001e4d0: 7468 3d22 7572 6c28 2370 6462 3931 3865  th="url(#pdb918e
-0001e4e0: 3637 3665 2922 2073 7479 6c65 3d22 6669  676e)" style="fi
+0001e4d0: 7468 3d22 7572 6c28 2370 6661 3163 6264  th="url(#pfa1cbd
+0001e4e0: 3632 6363 2922 2073 7479 6c65 3d22 6669  62cc)" style="fi
 0001e4f0: 6c6c 3a20 2366 6637 6630 303b 206f 7061  ll: #ff7f00; opa
 0001e500: 6369 7479 3a20 302e 3422 2f3e 0a20 2020  city: 0.4"/>.   
 0001e510: 3c2f 673e 0a20 2020 3c67 2069 643d 2270  </g>.   <g id="p
 0001e520: 6174 6368 5f36 3122 3e0a 2020 2020 3c70  atch_61">.    <p
 0001e530: 6174 6820 643d 224d 2034 3034 2e31 3539  ath d="M 404.159
 0001e540: 3532 3920 3933 322e 3833 3731 3431 200a  529 932.837141 .
 0001e550: 4320 3430 342e 3235 3938 3139 2039 3331  C 404.259819 931
@@ -7837,15 +7837,15 @@
 0001e9c0: 3930 3720 3430 322e 3536 3135 3035 2039  907 402.561505 9
 0001e9d0: 3334 2e36 3934 3432 3420 0a43 2034 3033  34.694424 .C 403
 0001e9e0: 2e31 3931 3231 3820 3933 342e 3136 3539  .191218 934.1659
 0001e9f0: 3420 3430 332e 3733 3039 3331 2039 3333  4 403.730931 933
 0001ea00: 2e35 3338 3636 3520 3430 342e 3135 3935  .538665 404.1595
 0001ea10: 3239 2039 3332 2e38 3337 3134 3120 0a22  29 932.837141 ."
 0001ea20: 2063 6c69 702d 7061 7468 3d22 7572 6c28   clip-path="url(
-0001ea30: 2370 6462 3931 3865 3637 3665 2922 2073  #pdb918e676e)" s
+0001ea30: 2370 6661 3163 6264 3632 6363 2922 2073  #pfa1cbd62cc)" s
 0001ea40: 7479 6c65 3d22 6669 6c6c 3a20 2366 6664  tyle="fill: #ffd
 0001ea50: 6638 363b 206f 7061 6369 7479 3a20 302e  f86; opacity: 0.
 0001ea60: 3422 2f3e 0a20 2020 3c2f 673e 0a20 2020  4"/>.   </g>.   
 0001ea70: 3c67 2069 643d 2274 6578 745f 3936 223e  <g id="text_96">
 0001ea80: 0a20 2020 203c 212d 2d20 3136 3136 202d  .    <!-- 1616 -
 0001ea90: 2d3e 0a20 2020 203c 6720 7374 796c 653d  ->.    <g style=
 0001eaa0: 2266 696c 6c3a 2023 3236 3236 3236 2220  "fill: #262626" 
@@ -8093,15 +8093,15 @@
 0001f9c0: 3820 3630 372e 3731 3032 3233 2039 3634  8 607.710223 964
 0001f9d0: 2e33 3939 3337 3520 0a43 2036 3131 2e37  .399375 .C 611.7
 0001f9e0: 3533 3534 3620 3936 302e 3131 3836 3632  53546 960.118662
 0001f9f0: 2036 3135 2e30 3336 3432 3620 3935 352e   615.036426 955.
 0001fa00: 3137 3838 3231 2036 3137 2e34 3137 3130  178821 617.41710
 0001fa10: 3520 3934 392e 3739 3331 3632 200a 2220  5 949.793162 ." 
 0001fa20: 636c 6970 2d70 6174 683d 2275 726c 2823  clip-path="url(#
-0001fa30: 7066 6636 6162 6665 3562 3829 2220 7374  pff6abfe5b8)" st
+0001fa30: 7038 3662 3132 3838 3464 3729 2220 7374  p86b12884d7)" st
 0001fa40: 796c 653d 2266 696c 6c3a 2023 6330 6330  yle="fill: #c0c0
 0001fa50: 6330 3b20 6f70 6163 6974 793a 2030 2e34  c0; opacity: 0.4
 0001fa60: 222f 3e0a 2020 203c 2f67 3e0a 2020 203c  "/>.   </g>.   <
 0001fa70: 6720 6964 3d22 7061 7463 685f 3633 223e  g id="patch_63">
 0001fa80: 0a20 2020 203c 7061 7468 2064 3d22 4d20  .    <path d="M 
 0001fa90: 3631 372e 3431 3731 3035 2039 3037 2e39  617.417105 907.9
 0001faa0: 3634 3934 3820 0a43 2036 3230 2e33 3239  64948 .C 620.329
@@ -8144,16 +8144,16 @@
 0001fcf0: 2e30 3237 3234 3420 3632 372e 3432 3938  .027244 627.4298
 0001fd00: 3936 2039 3037 2e34 3236 3330 3520 0a43  96 907.426305 .C
 0001fd10: 2036 3234 2e30 3935 3934 3220 3930 362e   624.095942 906.
 0001fd20: 3832 3533 3635 2036 3230 2e36 3637 3334  825365 620.66734
 0001fd30: 3920 3930 372e 3030 3938 3038 2036 3137  9 907.009808 617
 0001fd40: 2e34 3137 3130 3520 3930 372e 3936 3439  .417105 907.9649
 0001fd50: 3438 200a 2220 636c 6970 2d70 6174 683d  48 ." clip-path=
-0001fd60: 2275 726c 2823 7066 6636 6162 6665 3562  "url(#pff6abfe5b
-0001fd70: 3829 2220 7374 796c 653d 2266 696c 6c3a  8)" style="fill:
+0001fd60: 2275 726c 2823 7038 3662 3132 3838 3464  "url(#p86b12884d
+0001fd70: 3729 2220 7374 796c 653d 2266 696c 6c3a  7)" style="fill:
 0001fd80: 2023 6361 6232 6436 3b20 6f70 6163 6974   #cab2d6; opacit
 0001fd90: 793a 2030 2e34 222f 3e0a 2020 203c 2f67  y: 0.4"/>.   </g
 0001fda0: 3e0a 2020 203c 6720 6964 3d22 7061 7463  >.   <g id="patc
 0001fdb0: 685f 3634 223e 0a20 2020 203c 7061 7468  h_64">.    <path
 0001fdc0: 2064 3d22 4d20 3631 372e 3431 3731 3035   d="M 617.417105
 0001fdd0: 2039 3439 2e37 3933 3136 3220 0a43 2036   949.793162 .C 6
 0001fde0: 3230 2e33 3239 3132 3520 3934 332e 3230  20.329125 943.20
@@ -8178,16 +8178,16 @@
 0001ff10: 3937 3320 3933 382e 3137 3130 3436 2036  973 938.171046 6
 0001ff20: 3036 2e31 3131 3036 3320 3934 312e 3934  06.111063 941.94
 0001ff30: 3034 3531 200a 4320 3630 382e 3933 3231  0451 .C 608.9321
 0001ff40: 3532 2039 3435 2e37 3039 3835 3520 3631  52 945.709855 61
 0001ff50: 322e 3839 3939 3334 2039 3438 2e34 3635  2.899934 948.465
 0001ff60: 3731 3320 3631 372e 3431 3731 3035 2039  713 617.417105 9
 0001ff70: 3439 2e37 3933 3136 3220 0a22 2063 6c69  49.793162 ." cli
-0001ff80: 702d 7061 7468 3d22 7572 6c28 2370 6666  p-path="url(#pff
-0001ff90: 3661 6266 6535 6238 2922 2073 7479 6c65  6abfe5b8)" style
+0001ff80: 702d 7061 7468 3d22 7572 6c28 2370 3836  p-path="url(#p86
+0001ff90: 6231 3238 3834 6437 2922 2073 7479 6c65  b12884d7)" style
 0001ffa0: 3d22 6669 6c6c 3a20 2366 6666 6666 663b  ="fill: #ffffff;
 0001ffb0: 206f 7061 6369 7479 3a20 302e 3422 2f3e   opacity: 0.4"/>
 0001ffc0: 0a20 2020 3c2f 673e 0a20 2020 3c67 2069  .   </g>.   <g i
 0001ffd0: 643d 2274 6578 745f 3130 3122 3e0a 2020  d="text_101">.  
 0001ffe0: 2020 3c21 2d2d 2031 3533 3120 2d2d 3e0a    <!-- 1531 -->.
 0001fff0: 2020 2020 3c67 2073 7479 6c65 3d22 6669      <g style="fi
 00020000: 6c6c 3a20 2332 3632 3632 3622 2074 7261  ll: #262626" tra
@@ -8417,15 +8417,15 @@
 00020e00: 3939 2e39 3235 3536 3920 3131 3032 2e38  99.925569 1102.8
 00020e10: 3032 3439 3920 0a43 2031 3033 2e30 3934  02499 .C 103.094
 00020e20: 3430 3120 3131 3030 2e38 3036 3230 3620  401 1100.806206 
 00020e30: 3130 352e 3934 3030 3135 2031 3039 382e  105.940015 1098.
 00020e40: 3333 3738 3431 2031 3038 2e33 3633 3935  337841 108.36395
 00020e50: 3220 3130 3935 2e34 3832 3830 3920 0a22  2 1095.482809 ."
 00020e60: 2063 6c69 702d 7061 7468 3d22 7572 6c28   clip-path="url(
-00020e70: 2370 6233 3664 6438 3730 3533 2922 2073  #pb36dd87053)" s
+00020e70: 2370 6434 3731 6131 3563 3738 2922 2073  #pd471a15c78)" s
 00020e80: 7479 6c65 3d22 6669 6c6c 3a20 2363 3063  tyle="fill: #c0c
 00020e90: 3063 303b 206f 7061 6369 7479 3a20 302e  0c0; opacity: 0.
 00020ea0: 3422 2f3e 0a20 2020 3c2f 673e 0a20 2020  4"/>.   </g>.   
 00020eb0: 3c67 2069 643d 2270 6174 6368 5f36 3622  <g id="patch_66"
 00020ec0: 3e0a 2020 2020 3c70 6174 6820 643d 224d  >.    <path d="M
 00020ed0: 2031 3038 2e33 3633 3935 3220 3130 3437   108.363952 1047
 00020ee0: 2e38 3435 3330 3820 0a43 2031 3134 2e30  .845308 .C 114.0
@@ -8506,15 +8506,15 @@
 00021390: 3634 3320 3131 382e 3533 3432 3236 2031  643 118.534226 1
 000213a0: 3033 342e 3635 3231 3331 200a 4320 3131  034.652131 .C 11
 000213b0: 342e 3433 3733 3620 3130 3338 2e34 3536  4.43736 1038.456
 000213c0: 3631 3920 3131 312e 3030 3034 3539 2031  619 111.000459 1
 000213d0: 3034 322e 3931 3530 3637 2031 3038 2e33  042.915067 108.3
 000213e0: 3633 3935 3220 3130 3437 2e38 3435 3330  63952 1047.84530
 000213f0: 3820 0a22 2063 6c69 702d 7061 7468 3d22  8 ." clip-path="
-00021400: 7572 6c28 2370 6233 3664 6438 3730 3533  url(#pb36dd87053
+00021400: 7572 6c28 2370 6434 3731 6131 3563 3738  url(#pd471a15c78
 00021410: 2922 2073 7479 6c65 3d22 6669 6c6c 3a20  )" style="fill: 
 00021420: 2336 6133 6439 613b 206f 7061 6369 7479  #6a3d9a; opacity
 00021430: 3a20 302e 3422 2f3e 0a20 2020 3c2f 673e  : 0.4"/>.   </g>
 00021440: 0a20 2020 3c67 2069 643d 2270 6174 6368  .   <g id="patch
 00021450: 5f36 3722 3e0a 2020 2020 3c70 6174 6820  _67">.    <path 
 00021460: 643d 224d 2031 3038 2e33 3633 3935 3220  d="M 108.363952 
 00021470: 3130 3935 2e34 3832 3830 3920 0a43 2031  1095.482809 .C 1
@@ -8533,15 +8533,15 @@
 00021540: 2e33 3935 3139 3120 3130 3731 2e36 3634  .395191 1071.664
 00021550: 3035 3820 0a43 2031 3032 2e33 3935 3139  058 .C 102.39519
 00021560: 3120 3130 3739 2e39 3733 3236 3920 3130  1 1079.973269 10
 00021570: 342e 3434 3535 3835 2031 3038 382e 3135  4.445585 1088.15
 00021580: 3535 3035 2031 3038 2e33 3633 3935 3220  5505 108.363952 
 00021590: 3130 3935 2e34 3832 3830 3920 0a22 2063  1095.482809 ." c
 000215a0: 6c69 702d 7061 7468 3d22 7572 6c28 2370  lip-path="url(#p
-000215b0: 6233 3664 6438 3730 3533 2922 2073 7479  b36dd87053)" sty
+000215b0: 6434 3731 6131 3563 3738 2922 2073 7479  d471a15c78)" sty
 000215c0: 6c65 3d22 6669 6c6c 3a20 2364 3162 3166  le="fill: #d1b1f
 000215d0: 323b 206f 7061 6369 7479 3a20 302e 3422  2; opacity: 0.4"
 000215e0: 2f3e 0a20 2020 3c2f 673e 0a20 2020 3c67  />.   </g>.   <g
 000215f0: 2069 643d 2274 6578 745f 3130 3622 3e0a   id="text_106">.
 00021600: 2020 2020 3c21 2d2d 2031 3436 3520 2d2d      <!-- 1465 --
 00021610: 3e0a 2020 2020 3c67 2073 7479 6c65 3d22  >.    <g style="
 00021620: 6669 6c6c 3a20 2332 3632 3632 3622 2074  fill: #262626" t
@@ -9090,16 +9090,16 @@
 00023810: 2031 3039 382e 3530 3137 3037 2035 3539   1098.501707 559
 00023820: 2e33 3938 3120 3130 3935 2e35 3739 3430  .3981 1095.57940
 00023830: 3920 0a43 2035 3632 2e31 3236 3935 3920  9 .C 562.126959 
 00023840: 3130 3932 2e36 3537 3131 3120 3536 342e  1092.657111 564.
 00023850: 3333 3536 3233 2031 3038 392e 3238 3931  335623 1089.2891
 00023860: 3920 3536 352e 3932 3832 3637 2031 3038  9 565.928267 108
 00023870: 352e 3632 3137 3638 200a 2220 636c 6970  5.621768 ." clip
-00023880: 2d70 6174 683d 2275 726c 2823 7062 6361  -path="url(#pbca
-00023890: 3534 3339 3038 6229 2220 7374 796c 653d  543908b)" style=
+00023880: 2d70 6174 683d 2275 726c 2823 7066 3535  -path="url(#pf55
+00023890: 6165 3039 6239 6629 2220 7374 796c 653d  ae09b9f)" style=
 000238a0: 2266 696c 6c3a 2023 6330 6330 6330 3b20  "fill: #c0c0c0; 
 000238b0: 6f70 6163 6974 793a 2030 2e34 222f 3e0a  opacity: 0.4"/>.
 000238c0: 2020 203c 2f67 3e0a 2020 203c 6720 6964     </g>.   <g id
 000238d0: 3d22 7061 7463 685f 3732 223e 0a20 2020  ="patch_72">.   
 000238e0: 203c 7061 7468 2064 3d22 4d20 3536 352e   <path d="M 565.
 000238f0: 3932 3832 3637 2031 3035 372e 3730 3633  928267 1057.7063
 00023900: 3439 200a 4320 3536 372e 3834 3130 3338  49 .C 567.841038
@@ -9179,16 +9179,16 @@
 00023da0: 2e37 3339 3733 3620 3537 332e 3838 3831  .739736 573.8881
 00023db0: 3336 2031 3034 312e 3539 3230 3820 0a43  36 1041.59208 .C
 00023dc0: 2035 3730 2e32 3932 3937 3520 3130 3436   570.292975 1046
 00023dd0: 2e34 3434 3432 3320 3536 372e 3539 3639  .444423 567.5969
 00023de0: 3337 2031 3035 312e 3930 3233 3839 2035  37 1051.902389 5
 00023df0: 3635 2e39 3238 3236 3720 3130 3537 2e37  65.928267 1057.7
 00023e00: 3036 3334 3920 0a22 2063 6c69 702d 7061  06349 ." clip-pa
-00023e10: 7468 3d22 7572 6c28 2370 6263 6135 3433  th="url(#pbca543
-00023e20: 3930 3862 2922 2073 7479 6c65 3d22 6669  908b)" style="fi
+00023e10: 7468 3d22 7572 6c28 2370 6635 3561 6530  th="url(#pf55ae0
+00023e20: 3962 3966 2922 2073 7479 6c65 3d22 6669  9b9f)" style="fi
 00023e30: 6c6c 3a20 2362 3135 3932 383b 206f 7061  ll: #b15928; opa
 00023e40: 6369 7479 3a20 302e 3422 2f3e 0a20 2020  city: 0.4"/>.   
 00023e50: 3c2f 673e 0a20 2020 3c67 2069 643d 2270  </g>.   <g id="p
 00023e60: 6174 6368 5f37 3322 3e0a 2020 2020 3c70  atch_73">.    <p
 00023e70: 6174 6820 643d 224d 2035 3635 2e39 3238  ath d="M 565.928
 00023e80: 3236 3720 3130 3835 2e36 3231 3736 3820  267 1085.621768 
 00023e90: 0a43 2035 3637 2e38 3431 3033 3820 3130  .C 567.841038 10
@@ -9206,15 +9206,15 @@
 00023f50: 2035 3633 2e39 3631 3634 3120 3130 3731   563.961641 1071
 00023f60: 2e36 3634 3035 3820 0a43 2035 3633 2e39  .664058 .C 563.9
 00023f70: 3631 3634 3120 3130 3736 2e33 3835 3634  61641 1076.38564
 00023f80: 3620 3536 342e 3632 3336 3334 2031 3038  6 564.623634 108
 00023f90: 312e 3038 3430 3031 2035 3635 2e39 3238  1.084001 565.928
 00023fa0: 3236 3720 3130 3835 2e36 3231 3736 3820  267 1085.621768 
 00023fb0: 0a22 2063 6c69 702d 7061 7468 3d22 7572  ." clip-path="ur
-00023fc0: 6c28 2370 6263 6135 3433 3930 3862 2922  l(#pbca543908b)"
+00023fc0: 6c28 2370 6635 3561 6530 3962 3966 2922  l(#pf55ae09b9f)"
 00023fd0: 2073 7479 6c65 3d22 6669 6c6c 3a20 2366   style="fill: #f
 00023fe0: 6663 3561 323b 206f 7061 6369 7479 3a20  fc5a2; opacity: 
 00023ff0: 302e 3422 2f3e 0a20 2020 3c2f 673e 0a20  0.4"/>.   </g>. 
 00024000: 2020 3c67 2069 643d 2274 6578 745f 3131    <g id="text_11
 00024010: 3622 3e0a 2020 2020 3c21 2d2d 2031 3631  6">.    <!-- 161
 00024020: 3120 2d2d 3e0a 2020 2020 3c67 2073 7479  1 -->.    <g sty
 00024030: 6c65 3d22 6669 6c6c 3a20 2332 3632 3632  le="fill: #26262
@@ -9350,15 +9350,15 @@
 00024850: 3930 3632 222f 3e0a 2020 2020 3c2f 673e  9062"/>.    </g>
 00024860: 0a20 2020 3c2f 673e 0a20 203c 2f67 3e0a  .   </g>.  </g>.
 00024870: 2020 3c67 2069 643d 2274 6578 745f 3132    <g id="text_12
 00024880: 3122 3e0a 2020 203c 212d 2d20 6874 7470  1">.   <!-- http
 00024890: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f62  s://github.com/b
 000248a0: 696f 7072 6167 6d61 7469 6373 2f62 696f  iopragmatics/bio
 000248b0: 7265 6769 7374 7279 2028 3230 3233 2d30  registry (2023-0
-000248c0: 352d 3036 2920 2d2d 3e0a 2020 203c 6720  5-06) -->.   <g 
+000248c0: 352d 3037 2920 2d2d 3e0a 2020 203c 6720  5-07) -->.   <g 
 000248d0: 7374 796c 653d 2266 696c 6c3a 2023 3830  style="fill: #80
 000248e0: 3830 3830 3b20 6f70 6163 6974 793a 2030  8080; opacity: 0
 000248f0: 2e35 2220 7472 616e 7366 6f72 6d3d 2274  .5" transform="t
 00024900: 7261 6e73 6c61 7465 2832 3333 2e36 3736  ranslate(233.676
 00024910: 3235 2031 3135 302e 3333 3632 3529 2073  25 1150.33625) s
 00024920: 6361 6c65 2830 2e30 3820 2d30 2e30 3829  cale(0.08 -0.08)
 00024930: 223e 0a20 2020 203c 6465 6673 3e0a 2020  ">.    <defs>.  
@@ -9617,45 +9617,45 @@
 00025900: 5675 5361 6e73 2d32 6422 2078 3d22 3237  VuSans-2d" x="27
 00025910: 3330 2e37 3537 3831 3222 2f3e 0a20 2020  30.757812"/>.   
 00025920: 203c 7573 6520 786c 696e 6b3a 6872 6566   <use xlink:href
 00025930: 3d22 2344 656a 6156 7553 616e 732d 3330  ="#DejaVuSans-30
 00025940: 2220 783d 2232 3736 362e 3834 3137 3937  " x="2766.841797
 00025950: 222f 3e0a 2020 2020 3c75 7365 2078 6c69  "/>.    <use xli
 00025960: 6e6b 3a68 7265 663d 2223 4465 6a61 5675  nk:href="#DejaVu
-00025970: 5361 6e73 2d33 3622 2078 3d22 3238 3330  Sans-36" x="2830
+00025970: 5361 6e73 2d33 3722 2078 3d22 3238 3330  Sans-37" x="2830
 00025980: 2e34 3634 3834 3422 2f3e 0a20 2020 203c  .464844"/>.    <
 00025990: 7573 6520 786c 696e 6b3a 6872 6566 3d22  use xlink:href="
 000259a0: 2344 656a 6156 7553 616e 732d 3239 2220  #DejaVuSans-29" 
 000259b0: 783d 2232 3839 342e 3038 3738 3931 222f  x="2894.087891"/
 000259c0: 3e0a 2020 203c 2f67 3e0a 2020 3c2f 673e  >.   </g>.  </g>
 000259d0: 0a20 3c2f 673e 0a20 3c64 6566 733e 0a20  . </g>. <defs>. 
 000259e0: 203c 636c 6970 5061 7468 2069 643d 2270   <clipPath id="p
-000259f0: 6261 3363 3735 3634 3339 223e 0a20 2020  ba3c756439">.   
+000259f0: 3662 3436 3639 3465 3236 223e 0a20 2020  6b46694e26">.   
 00025a00: 3c72 6563 7420 783d 2236 322e 3038 3638  <rect x="62.0868
 00025a10: 3738 2220 793d 2231 302e 3822 2077 6964  78" y="10.8" wid
 00025a20: 7468 3d22 3132 322e 3734 3733 3039 2220  th="122.747309" 
 00025a30: 6865 6967 6874 3d22 3132 322e 3733 3830  height="122.7380
 00025a40: 3722 2f3e 0a20 203c 2f63 6c69 7050 6174  7"/>.  </clipPat
 00025a50: 683e 0a20 203c 636c 6970 5061 7468 2069  h>.  <clipPath i
-00025a60: 643d 2270 6333 3437 3739 3764 6163 223e  d="pc347797dac">
+00025a60: 643d 2270 6266 6533 3935 3233 3761 223e  d="pbfe395237a">
 00025a70: 0a20 2020 3c72 6563 7420 783d 2232 3931  .   <rect x="291
 00025a80: 2e32 3930 3836 2220 793d 2231 302e 3822  .29086" y="10.8"
 00025a90: 2077 6964 7468 3d22 3132 322e 3734 3733   width="122.7473
 00025aa0: 3039 2220 6865 6967 6874 3d22 3132 322e  09" height="122.
 00025ab0: 3733 3830 3722 2f3e 0a20 203c 2f63 6c69  73807"/>.  </cli
 00025ac0: 7050 6174 683e 0a20 203c 636c 6970 5061  pPath>.  <clipPa
 00025ad0: 7468 2069 643d 2270 3963 3837 6166 3135  th id="p9c87af15
 00025ae0: 3038 223e 0a20 2020 3c72 6563 7420 783d  08">.   <rect x=
 00025af0: 2235 3230 2e32 3937 3834 3522 2079 3d22  "520.297845" y="
 00025b00: 3130 2e38 2220 7769 6474 683d 2231 3233  10.8" width="123
 00025b10: 2e31 3431 3330 3322 2068 6569 6768 743d  .141303" height=
 00025b20: 2231 3232 2e37 3338 3037 222f 3e0a 2020  "122.73807"/>.  
 00025b30: 3c2f 636c 6970 5061 7468 3e0a 2020 3c63  </clipPath>.  <c
-00025b40: 6c69 7050 6174 6820 6964 3d22 7066 3934  lipPath id="pf94
-00025b50: 3731 3133 3734 3222 3e0a 2020 203c 7265  7113742">.   <re
+00025b40: 6c69 7050 6174 6820 6964 3d22 7065 6332  lipPath id="pec2
+00025b50: 3764 6161 3063 3622 3e0a 2020 203c 7265  7daa0c6">.   <re
 00025b60: 6374 2078 3d22 3338 2e33 3638 3536 3722  ct x="38.368567"
 00025b70: 2079 3d22 3135 332e 3538 3530 3033 2220   y="153.585003" 
 00025b80: 7769 6474 683d 2231 3730 2e31 3833 3933  width="170.18393
 00025b90: 2220 6865 6967 6874 3d22 3132 322e 3733  " height="122.73
 00025ba0: 3830 3722 2f3e 0a20 203c 2f63 6c69 7050  807"/>.  </clipP
 00025bb0: 6174 683e 0a20 203c 636c 6970 5061 7468  ath>.  <clipPath
 00025bc0: 2069 643d 2270 6532 3866 3637 3161 6266   id="pe28f671abf
@@ -9669,61 +9669,61 @@
 00025c40: 6363 6564 3339 6230 3431 223e 0a20 2020  cced39b041">.   
 00025c50: 3c72 6563 7420 783d 2235 3131 2e34 3830  <rect x="511.480
 00025c60: 3834 3922 2079 3d22 3135 332e 3538 3530  849" y="153.5850
 00025c70: 3033 2220 7769 6474 683d 2231 3430 2e37  03" width="140.7
 00025c80: 3735 3239 3622 2068 6569 6768 743d 2231  75296" height="1
 00025c90: 3232 2e37 3338 3037 222f 3e0a 2020 3c2f  22.73807"/>.  </
 00025ca0: 636c 6970 5061 7468 3e0a 2020 3c63 6c69  clipPath>.  <cli
-00025cb0: 7050 6174 6820 6964 3d22 7037 6436 3162  pPath id="p7d61b
-00025cc0: 3535 3961 6122 3e0a 2020 203c 7265 6374  559aa">.   <rect
+00025cb0: 7050 6174 6820 6964 3d22 7033 3637 6262  pPath id="p367bb
+00025cc0: 6434 3630 6322 3e0a 2020 203c 7265 6374  d460c">.   <rect
 00025cd0: 2078 3d22 3338 2e32 3636 3231 3222 2079   x="38.266212" y
 00025ce0: 3d22 3239 362e 3337 3030 3037 2220 7769  ="296.370007" wi
 00025cf0: 6474 683d 2231 3730 2e33 3838 3634 3122  dth="170.388641"
 00025d00: 2068 6569 6768 743d 2231 3232 2e37 3338   height="122.738
 00025d10: 3037 222f 3e0a 2020 3c2f 636c 6970 5061  07"/>.  </clipPa
 00025d20: 7468 3e0a 2020 3c63 6c69 7050 6174 6820  th>.  <clipPath 
-00025d30: 6964 3d22 7065 3433 6335 3165 6630 3122  id="pe43c51ef01"
+00025d30: 6964 3d22 7066 3230 6233 3938 3135 3322  id="pf20b398153"
 00025d40: 3e0a 2020 203c 7265 6374 2078 3d22 3237  >.   <rect x="27
 00025d50: 362e 3439 3238 3531 2220 793d 2232 3936  6.492851" y="296
 00025d60: 2e33 3730 3030 3722 2077 6964 7468 3d22  .370007" width="
 00025d70: 3135 322e 3334 3333 3237 2220 6865 6967  152.343327" heig
 00025d80: 6874 3d22 3132 322e 3733 3830 3722 2f3e  ht="122.73807"/>
 00025d90: 0a20 203c 2f63 6c69 7050 6174 683e 0a20  .  </clipPath>. 
 00025da0: 203c 636c 6970 5061 7468 2069 643d 2270   <clipPath id="p
 00025db0: 6163 3861 6463 6532 6665 223e 0a20 2020  ac8adce2fe">.   
 00025dc0: 3c72 6563 7420 783d 2235 3135 2e35 3530  <rect x="515.550
 00025dd0: 3433 2220 793d 2232 3936 2e33 3730 3030  43" y="296.37000
 00025de0: 3722 2077 6964 7468 3d22 3133 322e 3633  7" width="132.63
 00025df0: 3631 3334 2220 6865 6967 6874 3d22 3132  6134" height="12
 00025e00: 322e 3733 3830 3722 2f3e 0a20 203c 2f63  2.73807"/>.  </c
 00025e10: 6c69 7050 6174 683e 0a20 203c 636c 6970  lipPath>.  <clip
-00025e20: 5061 7468 2069 643d 2270 3239 3462 6432  Path id="p294bd2
-00025e30: 3434 3763 223e 0a20 2020 3c72 6563 7420  447c">.   <rect 
+00025e20: 5061 7468 2069 643d 2270 3738 3031 3830  Path id="p780180
+00025e30: 6335 3564 223e 0a20 2020 3c72 6563 7420  c55d">.   <rect 
 00025e40: 783d 2235 382e 3933 3934 3922 2079 3d22  x="58.93949" y="
 00025e50: 3433 392e 3135 3530 3122 2077 6964 7468  439.15501" width
 00025e60: 3d22 3132 392e 3034 3230 3835 2220 6865  ="129.042085" he
 00025e70: 6967 6874 3d22 3132 322e 3733 3830 3722  ight="122.73807"
 00025e80: 2f3e 0a20 203c 2f63 6c69 7050 6174 683e  />.  </clipPath>
 00025e90: 0a20 203c 636c 6970 5061 7468 2069 643d  .  <clipPath id=
-00025ea0: 2270 6432 3134 3361 6561 3333 223e 0a20  "pd2143aea33">. 
+00025ea0: 2270 3665 3766 3966 6461 3932 223e 0a20  "p6e7f9fda92">. 
 00025eb0: 2020 3c72 6563 7420 783d 2232 3835 2e38    <rect x="285.8
 00025ec0: 3634 3534 3122 2079 3d22 3433 392e 3135  64541" y="439.15
 00025ed0: 3530 3122 2077 6964 7468 3d22 3133 332e  501" width="133.
 00025ee0: 3539 3939 3438 2220 6865 6967 6874 3d22  599948" height="
 00025ef0: 3132 322e 3733 3830 3722 2f3e 0a20 203c  122.73807"/>.  <
 00025f00: 2f63 6c69 7050 6174 683e 0a20 203c 636c  /clipPath>.  <cl
-00025f10: 6970 5061 7468 2069 643d 2270 6532 6363  ipPath id="pe2cc
-00025f20: 6334 6537 3532 223e 0a20 2020 3c72 6563  c4e752">.   <rec
+00025f10: 6970 5061 7468 2069 643d 2270 3465 3235  ipPath id="p4e25
+00025f20: 3131 3766 3932 223e 0a20 2020 3c72 6563  117f92">.   <rec
 00025f30: 7420 783d 2235 3133 2e31 3335 3939 3622  t x="513.135996"
 00025f40: 2079 3d22 3433 392e 3135 3530 3122 2077   y="439.15501" w
 00025f50: 6964 7468 3d22 3133 372e 3436 3530 3032  idth="137.465002
 00025f60: 2220 6865 6967 6874 3d22 3132 322e 3733  " height="122.73
 00025f70: 3830 3722 2f3e 0a20 203c 2f63 6c69 7050  807"/>.  </clipP
 00025f80: 6174 683e 0a20 203c 636c 6970 5061 7468  ath>.  <clipPath
-00025f90: 2069 643d 2270 3765 3430 3862 6632 3865   id="p7e408bf28e
+00025f90: 2069 643d 2270 3936 6135 3033 3162 6238   id="p96a5031bb8
 00025fa0: 223e 0a20 2020 3c72 6563 7420 783d 2235  ">.   <rect x="5
 00025fb0: 382e 3431 3234 3732 2220 793d 2235 3831  8.412472" y="581
 00025fc0: 2e39 3430 3031 3322 2077 6964 7468 3d22  .940013" width="
 00025fd0: 3133 302e 3039 3631 3231 2220 6865 6967  130.096121" heig
 00025fe0: 6874 3d22 3132 322e 3733 3830 3722 2f3e  ht="122.73807"/>
 00025ff0: 0a20 203c 2f63 6c69 7050 6174 683e 0a20  .  </clipPath>. 
 00026000: 203c 636c 6970 5061 7468 2069 643d 2270   <clipPath id="p
@@ -9738,77 +9738,77 @@
 00026090: 6634 6532 3422 3e0a 2020 203c 7265 6374  f4e24">.   <rect
 000260a0: 2078 3d22 3531 392e 3335 3639 3732 2220   x="519.356972" 
 000260b0: 793d 2235 3831 2e39 3430 3031 3322 2077  y="581.940013" w
 000260c0: 6964 7468 3d22 3132 352e 3032 3330 3522  idth="125.02305"
 000260d0: 2068 6569 6768 743d 2231 3232 2e37 3338   height="122.738
 000260e0: 3037 222f 3e0a 2020 3c2f 636c 6970 5061  07"/>.  </clipPa
 000260f0: 7468 3e0a 2020 3c63 6c69 7050 6174 6820  th>.  <clipPath 
-00026100: 6964 3d22 7064 3431 6632 3731 6135 3522  id="pd41f271a55"
+00026100: 6964 3d22 7065 3831 3266 6631 3432 6522  id="pe812ff142e"
 00026110: 3e0a 2020 203c 7265 6374 2078 3d22 3430  >.   <rect x="40
 00026120: 2e38 3435 3537 3222 2079 3d22 3732 342e  .845572" y="724.
 00026130: 3732 3530 3137 2220 7769 6474 683d 2231  725017" width="1
 00026140: 3635 2e32 3239 3932 3122 2068 6569 6768  65.229921" heigh
 00026150: 743d 2231 3232 2e37 3338 3037 222f 3e0a  t="122.73807"/>.
 00026160: 2020 3c2f 636c 6970 5061 7468 3e0a 2020    </clipPath>.  
-00026170: 3c63 6c69 7050 6174 6820 6964 3d22 7032  <clipPath id="p2
-00026180: 3339 3034 3135 3464 3722 3e0a 2020 203c  3904154d7">.   <
+00026170: 3c63 6c69 7050 6174 6820 6964 3d22 7063  <clipPath id="pc
+00026180: 3430 6564 3033 3563 3322 3e0a 2020 203c  40ed035c3">.   <
 00026190: 7265 6374 2078 3d22 3238 332e 3533 3137  rect x="283.5317
 000261a0: 3034 2220 793d 2237 3234 2e37 3235 3031  04" y="724.72501
 000261b0: 3722 2077 6964 7468 3d22 3133 382e 3236  7" width="138.26
 000261c0: 3536 3231 2220 6865 6967 6874 3d22 3132  5621" height="12
 000261d0: 322e 3733 3830 3722 2f3e 0a20 203c 2f63  2.73807"/>.  </c
 000261e0: 6c69 7050 6174 683e 0a20 203c 636c 6970  lipPath>.  <clip
 000261f0: 5061 7468 2069 643d 2270 3730 3265 6431  Path id="p702ed1
 00026200: 6662 6531 223e 0a20 2020 3c72 6563 7420  fbe1">.   <rect 
 00026210: 783d 2235 3135 2e35 3233 3937 2220 793d  x="515.52397" y=
 00026220: 2237 3234 2e37 3235 3031 3722 2077 6964  "724.725017" wid
 00026230: 7468 3d22 3133 322e 3638 3930 3533 2220  th="132.689053" 
 00026240: 6865 6967 6874 3d22 3132 322e 3733 3830  height="122.7380
 00026250: 3722 2f3e 0a20 203c 2f63 6c69 7050 6174  7"/>.  </clipPat
 00026260: 683e 0a20 203c 636c 6970 5061 7468 2069  h>.  <clipPath i
-00026270: 643d 2270 6563 3935 6236 3335 3762 223e  d="pec95b6357b">
+00026270: 643d 2270 3237 6561 6465 3034 3538 223e  d="p27eade0458">
 00026280: 0a20 2020 3c72 6563 7420 783d 2233 312e  .   <rect x="31.
 00026290: 3533 3236 3632 2220 793d 2238 3637 2e35  532662" y="867.5
 000262a0: 3130 3032 2220 7769 6474 683d 2231 3833  1002" width="183
 000262b0: 2e38 3535 3734 3122 2068 6569 6768 743d  .855741" height=
 000262c0: 2231 3232 2e37 3338 3037 222f 3e0a 2020  "122.73807"/>.  
 000262d0: 3c2f 636c 6970 5061 7468 3e0a 2020 3c63  </clipPath>.  <c
-000262e0: 6c69 7050 6174 6820 6964 3d22 7064 6239  lipPath id="pdb9
-000262f0: 3138 6536 3736 6522 3e0a 2020 203c 7265  18e676e">.   <re
+000262e0: 6c69 7050 6174 6820 6964 3d22 7066 6131  lipPath id="pfa1
+000262f0: 6362 6436 3263 6322 3e0a 2020 203c 7265  cbd62cc">.   <re
 00026300: 6374 2078 3d22 3239 302e 3831 3430 3133  ct x="290.814013
 00026310: 2220 793d 2238 3637 2e35 3130 3032 2220  " y="867.51002" 
 00026320: 7769 6474 683d 2231 3233 2e37 3031 3030  width="123.70100
 00026330: 3422 2068 6569 6768 743d 2231 3232 2e37  4" height="122.7
 00026340: 3338 3037 222f 3e0a 2020 3c2f 636c 6970  3807"/>.  </clip
 00026350: 5061 7468 3e0a 2020 3c63 6c69 7050 6174  Path>.  <clipPat
-00026360: 6820 6964 3d22 7066 6636 6162 6665 3562  h id="pff6abfe5b
-00026370: 3822 3e0a 2020 203c 7265 6374 2078 3d22  8">.   <rect x="
+00026360: 6820 6964 3d22 7038 3662 3132 3838 3464  h id="p86b12884d
+00026370: 3722 3e0a 2020 203c 7265 6374 2078 3d22  7">.   <rect x="
 00026380: 3530 382e 3733 3534 3039 2220 793d 2238  508.735409" y="8
 00026390: 3637 2e35 3130 3032 2220 7769 6474 683d  67.51002" width=
 000263a0: 2231 3436 2e32 3636 3137 3622 2068 6569  "146.266176" hei
 000263b0: 6768 743d 2231 3232 2e37 3338 3037 222f  ght="122.73807"/
 000263c0: 3e0a 2020 3c2f 636c 6970 5061 7468 3e0a  >.  </clipPath>.
 000263d0: 2020 3c63 6c69 7050 6174 6820 6964 3d22    <clipPath id="
-000263e0: 7062 3336 6464 3837 3035 3322 3e0a 2020  pb36dd87053">.  
+000263e0: 7064 3437 3161 3135 6337 3822 3e0a 2020  pd471a15c78">.  
 000263f0: 203c 7265 6374 2078 3d22 3332 2e36 3437   <rect x="32.647
 00026400: 3237 3422 2079 3d22 3130 3130 2e32 3935  274" y="1010.295
 00026410: 3032 3322 2077 6964 7468 3d22 3138 312e  023" width="181.
 00026420: 3632 3635 3136 2220 6865 6967 6874 3d22  626516" height="
 00026430: 3132 322e 3733 3830 3722 2f3e 0a20 203c  122.73807"/>.  <
 00026440: 2f63 6c69 7050 6174 683e 0a20 203c 636c  /clipPath>.  <cl
 00026450: 6970 5061 7468 2069 643d 2270 3066 6239  ipPath id="p0fb9
 00026460: 3939 3737 6363 223e 0a20 2020 3c72 6563  9977cc">.   <rec
 00026470: 7420 783d 2232 3639 2e32 3936 3437 3122  t x="269.296471"
 00026480: 2079 3d22 3130 3130 2e32 3935 3032 3322   y="1010.295023"
 00026490: 2077 6964 7468 3d22 3136 362e 3733 3630   width="166.7360
 000264a0: 3837 2220 6865 6967 6874 3d22 3132 322e  87" height="122.
 000264b0: 3733 3830 3722 2f3e 0a20 203c 2f63 6c69  73807"/>.  </cli
 000264c0: 7050 6174 683e 0a20 203c 636c 6970 5061  pPath>.  <clipPa
-000264d0: 7468 2069 643d 2270 6263 6135 3433 3930  th id="pbca54390
-000264e0: 3862 223e 0a20 2020 3c72 6563 7420 783d  8b">.   <rect x=
+000264d0: 7468 2069 643d 2270 6635 3561 6530 3962  th id="pf55ae09b
+000264e0: 3966 223e 0a20 2020 3c72 6563 7420 783d  9f">.   <rect x=
 000264f0: 2234 3837 2e38 3932 3035 2220 793d 2231  "487.89205" y="1
 00026500: 3031 302e 3239 3530 3233 2220 7769 6474  010.295023" widt
 00026510: 683d 2231 3837 2e39 3532 3839 3422 2068  h="187.952894" h
 00026520: 6569 6768 743d 2231 3232 2e37 3338 3037  eight="122.73807
 00026530: 222f 3e0a 2020 3c2f 636c 6970 5061 7468  "/>.  </clipPath
 00026540: 3e0a 203c 2f64 6566 733e 0a3c 2f73 7667  >. </defs>.</svg
 00026550: 3e0a                                     >.
```

### Comparing `bioregistry-0.9.6/docs/img/bioregistry_coverage_bar.svg` & `bioregistry-0.9.7/docs/img/bioregistry_coverage_bar.svg`

 * *Files 0% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 000001c0: 3032 2f32 322d 7264 662d 7379 6e74 6178  02/22-rdf-syntax
 000001d0: 2d6e 7323 223e 0a20 2020 3c63 633a 576f  -ns#">.   <cc:Wo
 000001e0: 726b 3e0a 2020 2020 3c64 633a 7479 7065  rk>.    <dc:type
 000001f0: 2072 6466 3a72 6573 6f75 7263 653d 2268   rdf:resource="h
 00000200: 7474 703a 2f2f 7075 726c 2e6f 7267 2f64  ttp://purl.org/d
 00000210: 632f 6463 6d69 7479 7065 2f53 7469 6c6c  c/dcmitype/Still
 00000220: 496d 6167 6522 2f3e 0a20 2020 203c 6463  Image"/>.    <dc
-00000230: 3a64 6174 653e 3230 3233 2d30 352d 3036  :date>2023-05-06
-00000240: 5430 313a 3038 3a30 382e 3039 3539 3836  T01:08:08.095986
+00000230: 3a64 6174 653e 3230 3233 2d30 352d 3037  :date>2023-05-07
+00000240: 5430 313a 3134 3a30 372e 3035 3932 3935  T01:14:07.059295
 00000250: 3c2f 6463 3a64 6174 653e 0a20 2020 203c  </dc:date>.    <
 00000260: 6463 3a66 6f72 6d61 743e 696d 6167 652f  dc:format>image/
 00000270: 7376 672b 786d 6c3c 2f64 633a 666f 726d  svg+xml</dc:form
 00000280: 6174 3e0a 2020 2020 3c64 633a 6372 6561  at>.    <dc:crea
 00000290: 746f 723e 0a20 2020 2020 3c63 633a 4167  tor>.     <cc:Ag
 000002a0: 656e 743e 0a20 2020 2020 203c 6463 3a74  ent>.      <dc:t
 000002b0: 6974 6c65 3e4d 6174 706c 6f74 6c69 6220  itle>Matplotlib
```

### Comparing `bioregistry-0.9.6/docs/img/bioregistry_coverage_bar_short.svg` & `bioregistry-0.9.7/docs/img/bioregistry_coverage_bar_short.svg`

 * *Files 0% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 000001c0: 3032 2f32 322d 7264 662d 7379 6e74 6178  02/22-rdf-syntax
 000001d0: 2d6e 7323 223e 0a20 2020 3c63 633a 576f  -ns#">.   <cc:Wo
 000001e0: 726b 3e0a 2020 2020 3c64 633a 7479 7065  rk>.    <dc:type
 000001f0: 2072 6466 3a72 6573 6f75 7263 653d 2268   rdf:resource="h
 00000200: 7474 703a 2f2f 7075 726c 2e6f 7267 2f64  ttp://purl.org/d
 00000210: 632f 6463 6d69 7479 7065 2f53 7469 6c6c  c/dcmitype/Still
 00000220: 496d 6167 6522 2f3e 0a20 2020 203c 6463  Image"/>.    <dc
-00000230: 3a64 6174 653e 3230 3233 2d30 352d 3036  :date>2023-05-06
-00000240: 5430 313a 3038 3a31 302e 3137 3439 3632  T01:08:10.174962
+00000230: 3a64 6174 653e 3230 3233 2d30 352d 3037  :date>2023-05-07
+00000240: 5430 313a 3134 3a30 382e 3538 3130 3532  T01:14:08.581052
 00000250: 3c2f 6463 3a64 6174 653e 0a20 2020 203c  </dc:date>.    <
 00000260: 6463 3a66 6f72 6d61 743e 696d 6167 652f  dc:format>image/
 00000270: 7376 672b 786d 6c3c 2f64 633a 666f 726d  svg+xml</dc:form
 00000280: 6174 3e0a 2020 2020 3c64 633a 6372 6561  at>.    <dc:crea
 00000290: 746f 723e 0a20 2020 2020 3c63 633a 4167  tor>.     <cc:Ag
 000002a0: 656e 743e 0a20 2020 2020 203c 6463 3a74  ent>.      <dc:t
 000002b0: 6974 6c65 3e4d 6174 706c 6f74 6c69 6220  itle>Matplotlib
```

### Comparing `bioregistry-0.9.6/docs/img/datamodel_umls.svg` & `bioregistry-0.9.7/docs/img/datamodel_umls.svg`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/docs/img/external_overlap.svg` & `bioregistry-0.9.7/docs/img/external_overlap.svg`

 * *Files 0% similar despite different names*

```diff
@@ -30,16 +30,16 @@
 000001d0: 6e74 6178 2d6e 7323 223e 0a20 2020 3c63  ntax-ns#">.   <c
 000001e0: 633a 576f 726b 3e0a 2020 2020 3c64 633a  c:Work>.    <dc:
 000001f0: 7479 7065 2072 6466 3a72 6573 6f75 7263  type rdf:resourc
 00000200: 653d 2268 7474 703a 2f2f 7075 726c 2e6f  e="http://purl.o
 00000210: 7267 2f64 632f 6463 6d69 7479 7065 2f53  rg/dc/dcmitype/S
 00000220: 7469 6c6c 496d 6167 6522 2f3e 0a20 2020  tillImage"/>.   
 00000230: 203c 6463 3a64 6174 653e 3230 3233 2d30   <dc:date>2023-0
-00000240: 352d 3036 5430 313a 3132 3a32 392e 3231  5-06T01:12:29.21
-00000250: 3739 3138 3c2f 6463 3a64 6174 653e 0a20  7918</dc:date>. 
+00000240: 352d 3037 5430 313a 3138 3a30 332e 3232  5-07T01:18:03.22
+00000250: 3034 3933 3c2f 6463 3a64 6174 653e 0a20  0493</dc:date>. 
 00000260: 2020 203c 6463 3a66 6f72 6d61 743e 696d     <dc:format>im
 00000270: 6167 652f 7376 672b 786d 6c3c 2f64 633a  age/svg+xml</dc:
 00000280: 666f 726d 6174 3e0a 2020 2020 3c64 633a  format>.    <dc:
 00000290: 6372 6561 746f 723e 0a20 2020 2020 3c63  creator>.     <c
 000002a0: 633a 4167 656e 743e 0a20 2020 2020 203c  c:Agent>.      <
 000002b0: 6463 3a74 6974 6c65 3e4d 6174 706c 6f74  dc:title>Matplot
 000002c0: 6c69 6220 7633 2e37 2e31 2c20 6874 7470  lib v3.7.1, http
@@ -48028,15 +48028,15 @@
 000bb9b0: 3132 3536 2037 3237 2e37 3430 3331 3320  1256 727.740313 
 000bb9c0: 3639 3335 2e37 3336 3930 3120 0a43 2037  6935.736901 .C 7
 000bb9d0: 3238 2e38 3833 3731 2036 3933 342e 3430  28.88371 6934.40
 000bb9e0: 3235 3436 2037 3239 2e37 3835 3932 3920  2546 729.785929 
 000bb9f0: 3639 3332 2e38 3739 3132 3220 3733 302e  6932.879122 730.
 000bba00: 3430 3634 3237 2036 3933 312e 3233 3530  406427 6931.2350
 000bba10: 3920 0a22 2063 6c69 702d 7061 7468 3d22  9 ." clip-path="
-000bba20: 7572 6c28 2370 6531 3662 3537 6666 3864  url(#pe16b57ff8d
+000bba20: 7572 6c28 2370 3238 3330 3938 3033 3233  url(#p2830980323
 000bba30: 2922 2073 7479 6c65 3d22 6669 6c6c 3a20  )" style="fill: 
 000bba40: 2366 6637 6630 303b 206f 7061 6369 7479  #ff7f00; opacity
 000bba50: 3a20 302e 3422 2f3e 0a20 2020 3c2f 673e  : 0.4"/>.   </g>
 000bba60: 0a20 2020 3c67 2069 643d 2270 6174 6368  .   <g id="patch
 000bba70: 5f34 3537 223e 0a20 2020 203c 7061 7468  _457">.    <path
 000bba80: 2064 3d22 4d20 3733 302e 3430 3634 3237   d="M 730.406427
 000bba90: 2036 3932 302e 3535 3039 3739 200a 4320   6920.550979 .C 
@@ -48117,16 +48117,16 @@
 000bbf40: 2e37 3236 3935 3920 3733 342e 3339 3339  .726959 734.3939
 000bbf50: 3631 2036 3930 392e 3937 3437 3039 200a  61 6909.974709 .
 000bbf60: 4320 3733 322e 3432 3038 3035 2036 3931  C 732.420805 691
 000bbf70: 332e 3232 3234 3539 2037 3331 2e30 3638  3.222459 731.068
 000bbf80: 3630 3120 3639 3136 2e38 3038 3935 3320  601 6916.808953 
 000bbf90: 3733 302e 3430 3634 3237 2036 3932 302e  730.406427 6920.
 000bbfa0: 3535 3039 3739 200a 2220 636c 6970 2d70  550979 ." clip-p
-000bbfb0: 6174 683d 2275 726c 2823 7065 3136 6235  ath="url(#pe16b5
-000bbfc0: 3766 6638 6429 2220 7374 796c 653d 2266  7ff8d)" style="f
+000bbfb0: 6174 683d 2275 726c 2823 7032 3833 3039  ath="url(#p28309
+000bbfc0: 3830 3332 3329 2220 7374 796c 653d 2266  80323)" style="f
 000bbfd0: 696c 6c3a 2023 6231 3539 3238 3b20 6f70  ill: #b15928; op
 000bbfe0: 6163 6974 793a 2030 2e34 222f 3e0a 2020  acity: 0.4"/>.  
 000bbff0: 203c 2f67 3e0a 2020 203c 6720 6964 3d22   </g>.   <g id="
 000bc000: 7061 7463 685f 3435 3822 3e0a 2020 2020  patch_458">.    
 000bc010: 3c70 6174 6820 643d 224d 2037 3330 2e34  <path d="M 730.4
 000bc020: 3036 3432 3720 3639 3331 2e32 3335 3039  06427 6931.23509
 000bc030: 200a 4320 3733 312e 3035 3038 3034 2036   .C 731.050804 6
@@ -48144,15 +48144,15 @@
 000bc0f0: 3920 3732 392e 3933 3734 3135 2036 3932  9 729.937415 692
 000bc100: 352e 3839 3330 3334 200a 4320 3732 392e  5.893034 .C 729.
 000bc110: 3933 3734 3135 2036 3932 372e 3638 3339  937415 6927.6839
 000bc120: 3939 2037 3330 2e30 3934 3335 3320 3639  99 730.094353 69
 000bc130: 3239 2e34 3731 3532 3420 3733 302e 3430  29.471524 730.40
 000bc140: 3634 3237 2036 3933 312e 3233 3530 3920  6427 6931.23509 
 000bc150: 0a22 2063 6c69 702d 7061 7468 3d22 7572  ." clip-path="ur
-000bc160: 6c28 2370 6531 3662 3537 6666 3864 2922  l(#pe16b57ff8d)"
+000bc160: 6c28 2370 3238 3330 3938 3033 3233 2922  l(#p2830980323)"
 000bc170: 2073 7479 6c65 3d22 6669 6c6c 3a20 2366   style="fill: #f
 000bc180: 6639 3731 633b 206f 7061 6369 7479 3a20  f971c; opacity: 
 000bc190: 302e 3422 2f3e 0a20 2020 3c2f 673e 0a20  0.4"/>.   </g>. 
 000bc1a0: 2020 3c67 2069 643d 2274 6578 745f 3736    <g id="text_76
 000bc1b0: 3522 3e0a 2020 2020 3c21 2d2d 2038 3233  5">.    <!-- 823
 000bc1c0: 202d 2d3e 0a20 2020 203c 6720 7374 796c   -->.    <g styl
 000bc1d0: 653d 2266 696c 6c3a 2023 3236 3236 3236  e="fill: #262626
@@ -61316,16 +61316,16 @@
 000ef830: 3238 3039 3120 3733 382e 3237 3033 3936  28091 738.270396
 000ef840: 2038 3931 372e 3333 3037 3133 200a 4320   8917.330713 .C 
 000ef850: 3733 392e 3739 3336 3039 2038 3931 352e  739.793609 8915.
 000ef860: 3338 3035 3136 2037 3430 2e39 3538 3634  380516 740.95864
 000ef870: 3520 3839 3133 2e31 3735 3334 3320 3734  5 8913.175343 74
 000ef880: 312e 3731 3131 3936 2038 3931 302e 3831  1.711196 8910.81
 000ef890: 3739 3920 0a22 2063 6c69 702d 7061 7468  799 ." clip-path
-000ef8a0: 3d22 7572 6c28 2370 3234 6132 6237 6236  ="url(#p24a2b7b6
-000ef8b0: 3335 2922 2073 7479 6c65 3d22 6669 6c6c  35)" style="fill
+000ef8a0: 3d22 7572 6c28 2370 6262 3839 6362 6135  ="url(#pbb89cba5
+000ef8b0: 3339 2922 2073 7479 6c65 3d22 6669 6c6c  39)" style="fill
 000ef8c0: 3a20 2362 3135 3932 383b 206f 7061 6369  : #b15928; opaci
 000ef8d0: 7479 3a20 302e 3422 2f3e 0a20 2020 3c2f  ty: 0.4"/>.   </
 000ef8e0: 673e 0a20 2020 3c67 2069 643d 2270 6174  g>.   <g id="pat
 000ef8f0: 6368 5f35 3834 223e 0a20 2020 203c 7061  ch_584">.    <pa
 000ef900: 7468 2064 3d22 4d20 3734 312e 3731 3131  th d="M 741.7111
 000ef910: 3936 2038 3839 382e 3039 3836 3435 200a  96 8898.098645 .
 000ef920: 4320 3734 322e 3336 3735 3632 2038 3930  C 742.367562 890
@@ -61405,16 +61405,16 @@
 000efdc0: 372e 3336 3737 3233 2037 3435 2e35 3334  7.367723 745.534
 000efdd0: 3935 3320 3838 3839 2e38 3630 3537 3520  953 8889.860575 
 000efde0: 0a43 2037 3433 2e37 3733 3931 3120 3838  .C 743.773911 88
 000efdf0: 3932 2e33 3533 3432 3720 3734 322e 3437  92.353427 742.47
 000efe00: 3834 3134 2038 3839 352e 3134 3435 3033  8414 8895.144503
 000efe10: 2037 3431 2e37 3131 3139 3620 3838 3938   741.711196 8898
 000efe20: 2e30 3938 3634 3520 0a22 2063 6c69 702d  .098645 ." clip-
-000efe30: 7061 7468 3d22 7572 6c28 2370 3234 6132  path="url(#p24a2
-000efe40: 6237 6236 3335 2922 2073 7479 6c65 3d22  b7b635)" style="
+000efe30: 7061 7468 3d22 7572 6c28 2370 6262 3839  path="url(#pbb89
+000efe40: 6362 6135 3339 2922 2073 7479 6c65 3d22  cba539)" style="
 000efe50: 6669 6c6c 3a20 2331 6637 3862 343b 206f  fill: #1f78b4; o
 000efe60: 7061 6369 7479 3a20 302e 3422 2f3e 0a20  pacity: 0.4"/>. 
 000efe70: 2020 3c2f 673e 0a20 2020 3c67 2069 643d    </g>.   <g id=
 000efe80: 2270 6174 6368 5f35 3835 223e 0a20 2020  "patch_585">.   
 000efe90: 203c 7061 7468 2064 3d22 4d20 3734 312e   <path d="M 741.
 000efea0: 3731 3131 3936 2038 3931 302e 3831 3739  711196 8910.8179
 000efeb0: 3920 0a43 2037 3432 2e33 3637 3536 3220  9 .C 742.367562 
@@ -61432,15 +61432,15 @@
 000eff70: 3634 2037 3430 2e38 3938 3833 3820 3839  64 740.898838 89
 000eff80: 3034 2e34 3538 3331 3720 0a43 2037 3430  04.458317 .C 740
 000eff90: 2e38 3938 3833 3820 3839 3036 2e36 3034  .898838 8906.604
 000effa0: 3037 3120 3734 312e 3137 3138 3137 2038  071 741.171817 8
 000effb0: 3930 382e 3734 3131 3334 2037 3431 2e37  908.741134 741.7
 000effc0: 3131 3139 3620 3839 3130 2e38 3137 3939  11196 8910.81799
 000effd0: 200a 2220 636c 6970 2d70 6174 683d 2275   ." clip-path="u
-000effe0: 726c 2823 7032 3461 3262 3762 3633 3529  rl(#p24a2b7b635)
+000effe0: 726c 2823 7062 6238 3963 6261 3533 3929  rl(#pbb89cba539)
 000efff0: 2220 7374 796c 653d 2266 696c 6c3a 2023  " style="fill: #
 000f0000: 3932 3932 3961 3b20 6f70 6163 6974 793a  92929a; opacity:
 000f0010: 2030 2e34 222f 3e0a 2020 203c 2f67 3e0a   0.4"/>.   </g>.
 000f0020: 2020 203c 6720 6964 3d22 7465 7874 5f39     <g id="text_9
 000f0030: 3830 223e 0a20 2020 203c 212d 2d20 3137  80">.    <!-- 17
 000f0040: 3720 2d2d 3e0a 2020 2020 3c67 2073 7479  7 -->.    <g sty
 000f0050: 6c65 3d22 6669 6c6c 3a20 2332 3632 3632  le="fill: #26262
@@ -65518,16 +65518,16 @@
 000ffed0: 3837 3134 3638 2033 3135 2e31 3632 3733  871468 315.16273
 000ffee0: 3720 3936 3338 2e39 3737 3339 3620 0a43  7 9638.977396 .C
 000ffef0: 2033 3136 2e38 3837 3932 3220 3936 3337   316.887922 9637
 000fff00: 2e30 3833 3332 3320 3331 382e 3237 3434  .083323 318.2744
 000fff10: 3339 2039 3633 342e 3930 3634 3735 2033  39 9634.906475 3
 000fff20: 3139 2e32 3631 3531 3220 3936 3332 2e35  19.261512 9632.5
 000fff30: 3432 3237 3220 0a22 2063 6c69 702d 7061  42272 ." clip-pa
-000fff40: 7468 3d22 7572 6c28 2370 6465 3839 6562  th="url(#pde89eb
-000fff50: 6532 3231 2922 2073 7479 6c65 3d22 6669  e221)" style="fi
+000fff40: 7468 3d22 7572 6c28 2370 6335 3734 6539  th="url(#pc574e9
+000fff50: 3162 3738 2922 2073 7479 6c65 3d22 6669  1b78)" style="fi
 000fff60: 6c6c 3a20 2361 3663 6565 333b 206f 7061  ll: #a6cee3; opa
 000fff70: 6369 7479 3a20 302e 3422 2f3e 0a20 2020  city: 0.4"/>.   
 000fff80: 3c2f 673e 0a20 2020 3c67 2069 643d 2270  </g>.   <g id="p
 000fff90: 6174 6368 5f36 3234 223e 0a20 2020 203c  atch_624">.    <
 000fffa0: 7061 7468 2064 3d22 4d20 3331 392e 3236  path d="M 319.26
 000fffb0: 3135 3132 2039 3631 352e 3333 3039 3332  1512 9615.330932
 000fffc0: 200a 4320 3332 302e 3339 3937 3333 2039   .C 320.399733 9
@@ -65607,16 +65607,16 @@
 00100460: 3035 2e38 3236 3536 3820 3332 332e 3537  05.826568 323.57
 00100470: 3439 3136 2039 3630 382e 3030 3036 3120  4916 9608.00061 
 00100480: 0a43 2033 3231 2e37 3231 3838 3820 3936  .C 321.721888 96
 00100490: 3130 2e31 3734 3635 3220 3332 302e 3236  10.174652 320.26
 001004a0: 3231 3735 2039 3631 322e 3635 3533 3331  2175 9612.655331
 001004b0: 2033 3139 2e32 3631 3531 3220 3936 3135   319.261512 9615
 001004c0: 2e33 3330 3933 3220 0a22 2063 6c69 702d  .330932 ." clip-
-001004d0: 7061 7468 3d22 7572 6c28 2370 6465 3839  path="url(#pde89
-001004e0: 6562 6532 3231 2922 2073 7479 6c65 3d22  ebe221)" style="
+001004d0: 7061 7468 3d22 7572 6c28 2370 6335 3734  path="url(#pc574
+001004e0: 6539 3162 3738 2922 2073 7479 6c65 3d22  e91b78)" style="
 001004f0: 6669 6c6c 3a20 2366 6239 6139 393b 206f  fill: #fb9a99; o
 00100500: 7061 6369 7479 3a20 302e 3422 2f3e 0a20  pacity: 0.4"/>. 
 00100510: 2020 3c2f 673e 0a20 2020 3c67 2069 643d    </g>.   <g id=
 00100520: 2270 6174 6368 5f36 3235 223e 0a20 2020  "patch_625">.   
 00100530: 203c 7061 7468 2064 3d22 4d20 3331 392e   <path d="M 319.
 00100540: 3236 3135 3132 2039 3633 322e 3534 3232  261512 9632.5422
 00100550: 3732 200a 4320 3332 302e 3339 3937 3333  72 .C 320.399733
@@ -65634,16 +65634,16 @@
 00100610: 3038 3320 3331 372e 3730 3439 3233 2039  083 317.704923 9
 00100620: 3632 332e 3933 3636 3032 200a 4320 3331  623.936602 .C 31
 00100630: 372e 3730 3439 3233 2039 3632 362e 3837  7.704923 9626.87
 00100640: 3531 3231 2033 3138 2e32 3332 3135 3420  5121 318.232154 
 00100650: 3936 3239 2e37 3839 3934 3320 3331 392e  9629.789943 319.
 00100660: 3236 3135 3132 2039 3633 322e 3534 3232  261512 9632.5422
 00100670: 3732 200a 2220 636c 6970 2d70 6174 683d  72 ." clip-path=
-00100680: 2275 726c 2823 7064 6538 3965 6265 3232  "url(#pde89ebe22
-00100690: 3129 2220 7374 796c 653d 2266 696c 6c3a  1)" style="fill:
+00100680: 2275 726c 2823 7063 3537 3465 3931 6237  "url(#pc574e91b7
+00100690: 3829 2220 7374 796c 653d 2266 696c 6c3a  8)" style="fill:
 001006a0: 2023 6666 6663 6666 3b20 6f70 6163 6974   #fffcff; opacit
 001006b0: 793a 2030 2e34 222f 3e0a 2020 203c 2f67  y: 0.4"/>.   </g
 001006c0: 3e0a 2020 203c 6720 6964 3d22 7465 7874  >.   <g id="text
 001006d0: 5f31 3034 3822 3e0a 2020 2020 3c21 2d2d  _1048">.    <!--
 001006e0: 2031 3231 202d 2d3e 0a20 2020 203c 6720   121 -->.    <g 
 001006f0: 7374 796c 653d 2266 696c 6c3a 2023 3236  style="fill: #26
 00100700: 3236 3236 2220 7472 616e 7366 6f72 6d3d  2626" transform=
@@ -67566,15 +67566,15 @@
 00107ed0: 2037 362e 3732 3135 3833 2039 3938 392e   76.721583 9989.
 00107ee0: 3230 3835 3432 200a 4320 3737 2e33 3138  208542 .C 77.318
 00107ef0: 3834 3420 3939 3838 2e37 3134 3336 3820  844 9988.714368 
 00107f00: 3737 2e38 3332 3136 3520 3939 3838 2e31  77.832165 9988.1
 00107f10: 3236 3732 3820 3738 2e32 3431 3538 3720  26728 78.241587 
 00107f20: 3939 3837 2e34 3638 3437 3120 0a22 2063  9987.468471 ." c
 00107f30: 6c69 702d 7061 7468 3d22 7572 6c28 2370  lip-path="url(#p
-00107f40: 6338 3463 6464 6366 6431 2922 2073 7479  c84cddcfd1)" sty
+00107f40: 3936 6436 3238 6236 3233 2922 2073 7479  96d628b623)" sty
 00107f50: 6c65 3d22 6669 6c6c 3a20 2361 3663 6565  le="fill: #a6cee
 00107f60: 333b 206f 7061 6369 7479 3a20 302e 3422  3; opacity: 0.4"
 00107f70: 2f3e 0a20 2020 3c2f 673e 0a20 2020 3c67  />.   </g>.   <g
 00107f80: 2069 643d 2270 6174 6368 5f36 3433 223e   id="patch_643">
 00107f90: 0a20 2020 203c 7061 7468 2064 3d22 4d20  .    <path d="M 
 00107fa0: 3738 2e32 3431 3538 3720 3939 3739 2e38  78.241587 9979.8
 00107fb0: 3833 3031 3820 0a43 2037 382e 3934 3935  83018 .C 78.9495
@@ -67654,16 +67654,16 @@
 00108450: 312e 3935 3739 3834 2038 322e 3333 3037  1.957984 82.3307
 00108460: 3439 2039 3936 362e 3231 3332 3433 200a  49 9966.213243 .
 00108470: 4320 3830 2e31 3131 3437 3520 3939 3730  C 80.111475 9970
 00108480: 2e34 3638 3530 3120 3738 2e37 3233 3539  .468501 78.72359
 00108490: 3720 3939 3735 2e31 3038 3037 3620 3738  7 9975.108076 78
 001084a0: 2e32 3431 3538 3720 3939 3739 2e38 3833  .241587 9979.883
 001084b0: 3031 3820 0a22 2063 6c69 702d 7061 7468  018 ." clip-path
-001084c0: 3d22 7572 6c28 2370 6338 3463 6464 6366  ="url(#pc84cddcf
-001084d0: 6431 2922 2073 7479 6c65 3d22 6669 6c6c  d1)" style="fill
+001084c0: 3d22 7572 6c28 2370 3936 6436 3238 6236  ="url(#p96d628b6
+001084d0: 3233 2922 2073 7479 6c65 3d22 6669 6c6c  23)" style="fill
 001084e0: 3a20 2362 3135 3932 383b 206f 7061 6369  : #b15928; opaci
 001084f0: 7479 3a20 302e 3422 2f3e 0a20 2020 3c2f  ty: 0.4"/>.   </
 00108500: 673e 0a20 2020 3c67 2069 643d 2270 6174  g>.   <g id="pat
 00108510: 6368 5f36 3434 223e 0a20 2020 203c 7061  ch_644">.    <pa
 00108520: 7468 2064 3d22 4d20 3738 2e32 3431 3538  th d="M 78.24158
 00108530: 3720 3939 3837 2e34 3638 3437 3120 0a43  7 9987.468471 .C
 00108540: 2037 382e 3934 3935 3436 2039 3938 362e   78.949546 9986.
@@ -67680,15 +67680,15 @@
 001085f0: 3120 3738 2e30 3530 3634 3220 3939 3833  1 78.050642 9983
 00108600: 2e36 3735 3734 3520 0a43 2037 382e 3035  .675745 .C 78.05
 00108610: 3036 3432 2039 3938 342e 3934 3233 3839  0642 9984.942389
 00108620: 2037 382e 3131 3433 3731 2039 3938 362e   78.114371 9986.
 00108630: 3230 3832 3331 2037 382e 3234 3135 3837  208231 78.241587
 00108640: 2039 3938 372e 3436 3834 3731 200a 2220   9987.468471 ." 
 00108650: 636c 6970 2d70 6174 683d 2275 726c 2823  clip-path="url(#
-00108660: 7063 3834 6364 6463 6664 3129 2220 7374  pc84cddcfd1)" st
+00108660: 7039 3664 3632 3862 3632 3329 2220 7374  p96d628b623)" st
 00108670: 796c 653d 2266 696c 6c3a 2023 6630 6365  yle="fill: #f0ce
 00108680: 6262 3b20 6f70 6163 6974 793a 2030 2e34  bb; opacity: 0.4
 00108690: 222f 3e0a 2020 203c 2f67 3e0a 2020 203c  "/>.   </g>.   <
 001086a0: 6720 6964 3d22 7465 7874 5f31 3038 3122  g id="text_1081"
 001086b0: 3e0a 2020 2020 3c21 2d2d 2031 3139 202d  >.    <!-- 119 -
 001086c0: 2d3e 0a20 2020 203c 6720 7374 796c 653d  ->.    <g style=
 001086d0: 2266 696c 6c3a 2023 3236 3236 3236 2220  "fill: #262626" 
@@ -67899,16 +67899,16 @@
 001093a0: 3030 3035 2e34 3135 3333 2033 3433 2e32  0005.41533 343.2
 001093b0: 3335 3832 3420 3130 3030 312e 3538 3336  35824 10001.5836
 001093c0: 3431 200a 4320 3334 352e 3437 3039 3732  41 .C 345.470972
 001093d0: 2039 3939 372e 3735 3139 3532 2033 3436   9997.751952 346
 001093e0: 2e39 3639 3132 3220 3939 3933 2e35 3335  .969122 9993.535
 001093f0: 3434 3820 3334 372e 3635 3236 3932 2039  448 347.652692 9
 00109400: 3938 392e 3135 3234 3734 200a 2220 636c  989.152474 ." cl
-00109410: 6970 2d70 6174 683d 2275 726c 2823 7033  ip-path="url(#p3
-00109420: 6635 3666 6132 6465 3029 2220 7374 796c  f56fa2de0)" styl
+00109410: 6970 2d70 6174 683d 2275 726c 2823 7037  ip-path="url(#p7
+00109420: 6437 3934 3039 3136 6329 2220 7374 796c  d7940916c)" styl
 00109430: 653d 2266 696c 6c3a 2023 3166 3738 6234  e="fill: #1f78b4
 00109440: 3b20 6f70 6163 6974 793a 2030 2e34 222f  ; opacity: 0.4"/
 00109450: 3e0a 2020 203c 2f67 3e0a 2020 203c 6720  >.   </g>.   <g 
 00109460: 6964 3d22 7061 7463 685f 3634 3622 3e0a  id="patch_646">.
 00109470: 2020 2020 3c70 6174 6820 643d 224d 2033      <path d="M 3
 00109480: 3437 2e36 3532 3639 3220 3939 3738 2e31  47.652692 9978.1
 00109490: 3939 3031 3520 0a43 2033 3437 2e39 3335  99015 .C 347.935
@@ -67988,16 +67988,16 @@
 00109930: 3735 2e31 3433 3737 3420 3334 392e 3830  75.143774 349.80
 00109940: 3939 3231 2039 3937 352e 3831 3730 3535  9921 9975.817055
 00109950: 200a 4320 3334 382e 3936 3738 3835 2039   .C 348.967885 9
 00109960: 3937 362e 3439 3033 3336 2033 3438 2e32  976.490336 348.2
 00109970: 3339 3530 3720 3939 3737 2e32 3934 3539  39507 9977.29459
 00109980: 3420 3334 372e 3635 3236 3932 2039 3937  4 347.652692 997
 00109990: 382e 3139 3930 3135 200a 2220 636c 6970  8.199015 ." clip
-001099a0: 2d70 6174 683d 2275 726c 2823 7033 6635  -path="url(#p3f5
-001099b0: 3666 6132 6465 3029 2220 7374 796c 653d  6fa2de0)" style=
+001099a0: 2d70 6174 683d 2275 726c 2823 7037 6437  -path="url(#p7d7
+001099b0: 3934 3039 3136 6329 2220 7374 796c 653d  940916c)" style=
 001099c0: 2266 696c 6c3a 2023 6232 6466 3861 3b20  "fill: #b2df8a; 
 001099d0: 6f70 6163 6974 793a 2030 2e34 222f 3e0a  opacity: 0.4"/>.
 001099e0: 2020 203c 2f67 3e0a 2020 203c 6720 6964     </g>.   <g id
 001099f0: 3d22 7061 7463 685f 3634 3722 3e0a 2020  ="patch_647">.  
 00109a00: 2020 3c70 6174 6820 643d 224d 2033 3437    <path d="M 347
 00109a10: 2e36 3532 3639 3220 3939 3839 2e31 3532  .652692 9989.152
 00109a20: 3437 3420 0a43 2033 3437 2e39 3335 3237  474 .C 347.93527
@@ -68015,16 +68015,16 @@
 00109ae0: 3231 3231 2033 3436 2e30 3331 3632 3220  2121 346.031622 
 00109af0: 3939 3833 2e36 3735 3734 3520 0a43 2033  9983.675745 .C 3
 00109b00: 3436 2e30 3331 3632 3220 3939 3835 2e36  46.031622 9985.6
 00109b10: 3139 3336 3920 3334 362e 3539 3437 3831  19369 346.594781
 00109b20: 2039 3938 372e 3532 3139 3833 2033 3437   9987.521983 347
 00109b30: 2e36 3532 3639 3220 3939 3839 2e31 3532  .652692 9989.152
 00109b40: 3437 3420 0a22 2063 6c69 702d 7061 7468  474 ." clip-path
-00109b50: 3d22 7572 6c28 2370 3366 3536 6661 3264  ="url(#p3f56fa2d
-00109b60: 6530 2922 2073 7479 6c65 3d22 6669 6c6c  e0)" style="fill
+00109b50: 3d22 7572 6c28 2370 3764 3739 3430 3931  ="url(#p7d794091
+00109b60: 3663 2922 2073 7479 6c65 3d22 6669 6c6c  6c)" style="fill
 00109b70: 3a20 2339 3266 3064 663b 206f 7061 6369  : #92f0df; opaci
 00109b80: 7479 3a20 302e 3422 2f3e 0a20 2020 3c2f  ty: 0.4"/>.   </
 00109b90: 673e 0a20 2020 3c67 2069 643d 2274 6578  g>.   <g id="tex
 00109ba0: 745f 3130 3836 223e 0a20 2020 203c 212d  t_1086">.    <!-
 00109bb0: 2d20 3236 3120 2d2d 3e0a 2020 2020 3c67  - 261 -->.    <g
 00109bc0: 2073 7479 6c65 3d22 6669 6c6c 3a20 2332   style="fill: #2
 00109bd0: 3632 3632 3622 2074 7261 6e73 666f 726d  62626" transform
@@ -77479,16 +77479,16 @@
 0012ea60: 2031 3134 3238 2e36 3634 3835 3820 3738   11428.664858 78
 0012ea70: 2e39 3339 3735 3220 3131 3432 372e 3936  .939752 11427.96
 0012ea80: 3536 200a 4320 3739 2e35 3535 3733 2031  56 .C 79.55573 1
 0012ea90: 3134 3237 2e32 3636 3334 3120 3830 2e30  1427.266341 80.0
 0012eaa0: 3435 3933 3420 3131 3432 362e 3436 3536  45934 11426.4656
 0012eab0: 3234 2038 302e 3338 3835 3820 3131 3432  24 80.38858 1142
 0012eac0: 352e 3539 3930 3331 200a 2220 636c 6970  5.599031 ." clip
-0012ead0: 2d70 6174 683d 2275 726c 2823 7030 6634  -path="url(#p0f4
-0012eae0: 3433 6465 3238 3029 2220 7374 796c 653d  43de280)" style=
+0012ead0: 2d70 6174 683d 2275 726c 2823 7031 6232  -path="url(#p1b2
+0012eae0: 3465 3936 3366 3229 2220 7374 796c 653d  4e963f2)" style=
 0012eaf0: 2266 696c 6c3a 2023 6662 3961 3939 3b20  "fill: #fb9a99; 
 0012eb00: 6f70 6163 6974 793a 2030 2e34 222f 3e0a  opacity: 0.4"/>.
 0012eb10: 2020 203c 2f67 3e0a 2020 203c 6720 6964     </g>.   <g id
 0012eb20: 3d22 7061 7463 685f 3733 3522 3e0a 2020  ="patch_735">.  
 0012eb30: 2020 3c70 6174 6820 643d 224d 2038 302e    <path d="M 80.
 0012eb40: 3338 3835 3820 3131 3431 392e 3636 3535  38858 11419.6655
 0012eb50: 3937 200a 4320 3830 2e37 3632 3032 3920  97 .C 80.762029 
@@ -77570,16 +77570,16 @@
 0012f010: 3031 3134 3631 2038 342e 3134 3237 3735  011461 84.142775
 0012f020: 2031 3134 3036 2e32 3133 3838 3520 0a43   11406.213885 .C
 0012f030: 2038 322e 3034 3235 3634 2031 3134 3130   82.042564 11410
 0012f040: 2e34 3136 3330 3920 3830 2e37 3638 3037  .416309 80.76807
 0012f050: 3620 3131 3431 342e 3938 3239 3435 2038  6 11414.982945 8
 0012f060: 302e 3338 3835 3820 3131 3431 392e 3636  0.38858 11419.66
 0012f070: 3535 3937 200a 2220 636c 6970 2d70 6174  5597 ." clip-pat
-0012f080: 683d 2275 726c 2823 7030 6634 3433 6465  h="url(#p0f443de
-0012f090: 3238 3029 2220 7374 796c 653d 2266 696c  280)" style="fil
+0012f080: 683d 2275 726c 2823 7031 6232 3465 3936  h="url(#p1b24e96
+0012f090: 3366 3229 2220 7374 796c 653d 2266 696c  3f2)" style="fil
 0012f0a0: 6c3a 2023 3661 3364 3961 3b20 6f70 6163  l: #6a3d9a; opac
 0012f0b0: 6974 793a 2030 2e34 222f 3e0a 2020 203c  ity: 0.4"/>.   <
 0012f0c0: 2f67 3e0a 2020 203c 6720 6964 3d22 7061  /g>.   <g id="pa
 0012f0d0: 7463 685f 3733 3622 3e0a 2020 2020 3c70  tch_736">.    <p
 0012f0e0: 6174 6820 643d 224d 2038 302e 3338 3835  ath d="M 80.3885
 0012f0f0: 3820 3131 3432 352e 3539 3930 3331 200a  8 11425.599031 .
 0012f100: 4320 3830 2e37 3632 3032 3920 3131 3432  C 80.762029 1142
@@ -77596,16 +77596,16 @@
 0012f1b0: 3131 3432 312e 3634 3231 3935 2038 302e  11421.642195 80.
 0012f1c0: 3236 3835 3631 2031 3134 3232 2e36 3332  268561 11422.632
 0012f1d0: 3331 3420 0a43 2038 302e 3236 3835 3631  314 .C 80.268561
 0012f1e0: 2031 3134 3233 2e36 3232 3433 3320 3830   11423.622433 80
 0012f1f0: 2e33 3038 3620 3131 3432 342e 3631 3231  .3086 11424.6121
 0012f200: 3438 2038 302e 3338 3835 3820 3131 3432  48 80.38858 1142
 0012f210: 352e 3539 3930 3331 200a 2220 636c 6970  5.599031 ." clip
-0012f220: 2d70 6174 683d 2275 726c 2823 7030 6634  -path="url(#p0f4
-0012f230: 3433 6465 3238 3029 2220 7374 796c 653d  43de280)" style=
+0012f220: 2d70 6174 683d 2275 726c 2823 7031 6232  -path="url(#p1b2
+0012f230: 3465 3936 3366 3229 2220 7374 796c 653d  4e963f2)" style=
 0012f240: 2266 696c 6c3a 2023 6661 3936 6437 3b20  "fill: #fa96d7; 
 0012f250: 6f70 6163 6974 793a 2030 2e34 222f 3e0a  opacity: 0.4"/>.
 0012f260: 2020 203c 2f67 3e0a 2020 203c 6720 6964     </g>.   <g id
 0012f270: 3d22 7465 7874 5f31 3233 3722 3e0a 2020  ="text_1237">.  
 0012f280: 2020 3c21 2d2d 2031 3438 202d 2d3e 0a20    <!-- 148 -->. 
 0012f290: 2020 203c 6720 7374 796c 653d 2266 696c     <g style="fil
 0012f2a0: 6c3a 2023 3236 3236 3236 2220 7472 616e  l: #262626" tran
@@ -78446,16 +78446,16 @@
 001326d0: 2e39 3139 3538 3720 3730 372e 3337 3136  .919587 707.3716
 001326e0: 3535 2031 3134 3237 2e39 3533 3835 3620  55 11427.953856 
 001326f0: 0a43 2037 3038 2e32 3833 3132 3320 3131  .C 708.283123 11
 00132700: 3432 372e 3938 3831 3235 2037 3039 2e31  427.988125 709.1
 00132710: 3838 3239 3220 3131 3432 372e 3738 3736  88292 11427.7876
 00132720: 3533 2037 3130 2e30 3030 3035 3420 3131  53 710.000054 11
 00132730: 3432 372e 3337 3137 3332 200a 2220 636c  427.371732 ." cl
-00132740: 6970 2d70 6174 683d 2275 726c 2823 7061  ip-path="url(#pa
-00132750: 6637 3433 3330 3330 3429 2220 7374 796c  f74330304)" styl
+00132740: 6970 2d70 6174 683d 2275 726c 2823 7038  ip-path="url(#p8
+00132750: 3037 3139 6365 6662 3529 2220 7374 796c  0719cefb5)" styl
 00132760: 653d 2266 696c 6c3a 2023 6533 3161 3163  e="fill: #e31a1c
 00132770: 3b20 6f70 6163 6974 793a 2030 2e34 222f  ; opacity: 0.4"/
 00132780: 3e0a 2020 203c 2f67 3e0a 2020 203c 6720  >.   </g>.   <g 
 00132790: 6964 3d22 7061 7463 685f 3734 3422 3e0a  id="patch_744">.
 001327a0: 2020 2020 3c70 6174 6820 643d 224d 2037      <path d="M 7
 001327b0: 3130 2e30 3030 3035 3420 3131 3431 372e  10.000054 11417.
 001327c0: 3839 3238 3936 200a 4320 3731 302e 3837  892896 .C 710.87
@@ -78548,16 +78548,16 @@
 00132d30: 3536 2037 3134 2e35 3636 3335 3720 3131  56 714.566357 11
 00132d40: 3430 332e 3439 3532 3133 200a 4320 3731  403.495213 .C 71
 00132d50: 322e 3134 3833 3820 3131 3430 372e 3936  2.14838 11407.96
 00132d60: 3237 3720 3731 302e 3539 3838 3831 2031  277 710.598881 1
 00132d70: 3134 3132 2e38 3438 3338 3620 3731 302e  1412.848386 710.
 00132d80: 3030 3030 3534 2031 3134 3137 2e38 3932  000054 11417.892
 00132d90: 3839 3620 0a22 2063 6c69 702d 7061 7468  896 ." clip-path
-00132da0: 3d22 7572 6c28 2370 6166 3734 3333 3033  ="url(#paf743303
-00132db0: 3034 2922 2073 7479 6c65 3d22 6669 6c6c  04)" style="fill
+00132da0: 3d22 7572 6c28 2370 3830 3731 3963 6566  ="url(#p80719cef
+00132db0: 6235 2922 2073 7479 6c65 3d22 6669 6c6c  b5)" style="fill
 00132dc0: 3a20 2366 6462 6636 663b 206f 7061 6369  : #fdbf6f; opaci
 00132dd0: 7479 3a20 302e 3422 2f3e 0a20 2020 3c2f  ty: 0.4"/>.   </
 00132de0: 673e 0a20 2020 3c67 2069 643d 2270 6174  g>.   <g id="pat
 00132df0: 6368 5f37 3435 223e 0a20 2020 203c 7061  ch_745">.    <pa
 00132e00: 7468 2064 3d22 4d20 3731 302e 3030 3030  th d="M 710.0000
 00132e10: 3534 2031 3134 3237 2e33 3731 3733 3220  54 11427.371732 
 00132e20: 0a43 2037 3130 2e38 3732 3231 3620 3131  .C 710.872216 11
@@ -78585,15 +78585,15 @@
 00132f80: 392e 3731 3937 3334 2031 3134 3232 2e36  9.719734 11422.6
 00132f90: 3332 3331 3420 0a43 2037 3039 2e37 3139  32314 .C 709.719
 00132fa0: 3733 3420 3131 3432 342e 3231 3632 3632  734 11424.216262
 00132fb0: 2037 3039 2e38 3133 3333 3720 3131 3432   709.813337 1142
 00132fc0: 352e 3739 3838 3237 2037 3130 2e30 3030  5.798827 710.000
 00132fd0: 3035 3420 3131 3432 372e 3337 3137 3332  054 11427.371732
 00132fe0: 200a 2220 636c 6970 2d70 6174 683d 2275   ." clip-path="u
-00132ff0: 726c 2823 7061 6637 3433 3330 3330 3429  rl(#paf74330304)
+00132ff0: 726c 2823 7038 3037 3139 6365 6662 3529  rl(#p80719cefb5)
 00133000: 2220 7374 796c 653d 2266 696c 6c3a 2023  " style="fill: #
 00133010: 6666 3938 3631 3b20 6f70 6163 6974 793a  ff9861; opacity:
 00133020: 2030 2e34 222f 3e0a 2020 203c 2f67 3e0a   0.4"/>.   </g>.
 00133030: 2020 203c 6720 6964 3d22 7465 7874 5f31     <g id="text_1
 00133040: 3235 3222 3e0a 2020 2020 3c21 2d2d 2031  252">.    <!-- 1
 00133050: 3920 2d2d 3e0a 2020 2020 3c67 2073 7479  9 -->.    <g sty
 00133060: 6c65 3d22 6669 6c6c 3a20 2332 3632 3632  le="fill: #26262
@@ -79571,16 +79571,16 @@
 00136d20: 3230 3739 2037 312e 3034 3737 3533 2031  2079 71.047753 1
 00136d30: 3137 3835 2e30 3738 3139 3620 0a43 2037  1785.078196 .C 7
 00136d40: 312e 3333 3832 3135 2031 3137 3834 2e38  1.338215 11784.8
 00136d50: 3434 3331 3420 3731 2e35 3839 3134 3620  44314 71.589146 
 00136d60: 3131 3738 342e 3536 3531 3934 2037 312e  11784.565194 71.
 00136d70: 3739 3039 3032 2031 3137 3834 2e32 3531  790902 11784.251
 00136d80: 3536 3420 0a22 2063 6c69 702d 7061 7468  564 ." clip-path
-00136d90: 3d22 7572 6c28 2370 3763 6361 6563 3664  ="url(#p7ccaec6d
-00136da0: 6139 2922 2073 7479 6c65 3d22 6669 6c6c  a9)" style="fill
+00136d90: 3d22 7572 6c28 2370 3138 3766 3938 6565  ="url(#p187f98ee
+00136da0: 3663 2922 2073 7479 6c65 3d22 6669 6c6c  6c)" style="fill
 00136db0: 3a20 2365 3331 6131 633b 206f 7061 6369  : #e31a1c; opaci
 00136dc0: 7479 3a20 302e 3422 2f3e 0a20 2020 3c2f  ty: 0.4"/>.   </
 00136dd0: 673e 0a20 2020 3c67 2069 643d 2270 6174  g>.   <g id="pat
 00136de0: 6368 5f37 3535 223e 0a20 2020 203c 7061  ch_755">.    <pa
 00136df0: 7468 2064 3d22 4d20 3731 2e37 3930 3930  th d="M 71.79090
 00136e00: 3220 3131 3738 302e 3439 3133 3439 200a  2 11780.491349 .
 00136e10: 4320 3732 2e31 3531 3537 3420 3131 3738  C 72.151574 1178
@@ -79662,16 +79662,16 @@
 001372d0: 3035 3120 3735 2e35 3035 3833 3420 3131  051 75.505834 11
 001372e0: 3736 352e 3238 3932 3737 200a 4320 3733  765.289277 .C 73
 001372f0: 2e32 3935 3832 3420 3131 3737 302e 3036  .295824 11770.06
 00137300: 3835 3032 2037 322e 3033 3431 3431 2031  8502 72.034141 1
 00137310: 3137 3735 2e32 3331 3530 3420 3731 2e37  1775.231504 71.7
 00137320: 3930 3930 3220 3131 3738 302e 3439 3133  90902 11780.4913
 00137330: 3439 200a 2220 636c 6970 2d70 6174 683d  49 ." clip-path=
-00137340: 2275 726c 2823 7037 6363 6165 6336 6461  "url(#p7ccaec6da
-00137350: 3929 2220 7374 796c 653d 2266 696c 6c3a  9)" style="fill:
+00137340: 2275 726c 2823 7031 3837 6639 3865 6536  "url(#p187f98ee6
+00137350: 6329 2220 7374 796c 653d 2266 696c 6c3a  c)" style="fill:
 00137360: 2023 6231 3539 3238 3b20 6f70 6163 6974   #b15928; opacit
 00137370: 793a 2030 2e34 222f 3e0a 2020 203c 2f67  y: 0.4"/>.   </g
 00137380: 3e0a 2020 203c 6720 6964 3d22 7061 7463  >.   <g id="patc
 00137390: 685f 3735 3622 3e0a 2020 2020 3c70 6174  h_756">.    <pat
 001373a0: 6820 643d 224d 2037 312e 3739 3039 3032  h d="M 71.790902
 001373b0: 2031 3137 3834 2e32 3531 3536 3420 0a43   11784.251564 .C
 001373c0: 2037 322e 3135 3135 3734 2031 3137 3833   72.151574 11783
@@ -79688,16 +79688,16 @@
 00137470: 3137 3831 2e37 3434 3530 3320 3731 2e37  1781.744503 71.7
 00137480: 3437 3435 3320 3131 3738 322e 3337 3134  47453 11782.3714
 00137490: 3537 200a 4320 3731 2e37 3437 3435 3320  57 .C 71.747453 
 001374a0: 3131 3738 322e 3939 3834 3120 3731 2e37  11782.99841 71.7
 001374b0: 3631 3934 2031 3137 3833 2e36 3235 3238  6194 11783.62528
 001374c0: 2037 312e 3739 3039 3032 2031 3137 3834   71.790902 11784
 001374d0: 2e32 3531 3536 3420 0a22 2063 6c69 702d  .251564 ." clip-
-001374e0: 7061 7468 3d22 7572 6c28 2370 3763 6361  path="url(#p7cca
-001374f0: 6563 3664 6139 2922 2073 7479 6c65 3d22  ec6da9)" style="
+001374e0: 7061 7468 3d22 7572 6c28 2370 3138 3766  path="url(#p187f
+001374f0: 3938 6565 3663 2922 2073 7479 6c65 3d22  98ee6c)" style="
 00137500: 6669 6c6c 3a20 2366 6635 3033 303b 206f  fill: #ff5030; o
 00137510: 7061 6369 7479 3a20 302e 3422 2f3e 0a20  pacity: 0.4"/>. 
 00137520: 2020 3c2f 673e 0a20 2020 3c67 2069 643d    </g>.   <g id=
 00137530: 2274 6578 745f 3132 3733 223e 0a20 2020  "text_1273">.   
 00137540: 203c 212d 2d20 3234 202d 2d3e 0a20 2020   <!-- 24 -->.   
 00137550: 203c 6720 7374 796c 653d 2266 696c 6c3a   <g style="fill:
 00137560: 2023 3236 3236 3236 2220 7472 616e 7366   #262626" transf
@@ -82465,16 +82465,16 @@
 00142200: 2e32 3931 3437 3820 3733 362e 3530 3133  .291478 736.5013
 00142210: 3633 2031 3231 3537 2e37 3130 3333 3220  63 12157.710332 
 00142220: 0a43 2037 3338 2e32 3233 3739 3920 3132  .C 738.223799 12
 00142230: 3135 362e 3132 3931 3836 2037 3339 2e36  156.129186 739.6
 00142240: 3732 3533 2031 3231 3534 2e32 3733 3632  7253 12154.27362
 00142250: 3820 3734 302e 3738 3836 3535 2031 3231  8 740.788655 121
 00142260: 3532 2e32 3139 3130 3320 0a22 2063 6c69  52.219103 ." cli
-00142270: 702d 7061 7468 3d22 7572 6c28 2370 3332  p-path="url(#p32
-00142280: 6530 3930 6338 3031 2922 2073 7479 6c65  e090c801)" style
+00142270: 702d 7061 7468 3d22 7572 6c28 2370 3962  p-path="url(#p9b
+00142280: 6633 3038 3236 3638 2922 2073 7479 6c65  f3082668)" style
 00142290: 3d22 6669 6c6c 3a20 2363 6162 3264 363b  ="fill: #cab2d6;
 001422a0: 206f 7061 6369 7479 3a20 302e 3422 2f3e   opacity: 0.4"/>
 001422b0: 0a20 2020 3c2f 673e 0a20 2020 3c67 2069  .   </g>.   <g i
 001422c0: 643d 2270 6174 6368 5f37 3833 223e 0a20  d="patch_783">. 
 001422d0: 2020 203c 7061 7468 2064 3d22 4d20 3734     <path d="M 74
 001422e0: 302e 3738 3836 3535 2031 3231 3332 2e30  0.788655 12132.0
 001422f0: 3032 3039 3520 0a43 2037 3432 2e34 3734  02095 .C 742.474
@@ -82558,15 +82558,15 @@
 001427d0: 2037 3435 2e36 3039 3532 3820 3132 3132   745.609528 1212
 001427e0: 342e 3431 3732 3736 200a 4320 3734 332e  4.417276 .C 743.
 001427f0: 3537 3933 3420 3132 3132 362e 3635 3032  57934 12126.6502
 00142800: 3039 2037 3431 2e39 3438 3533 3720 3132  09 741.948537 12
 00142810: 3132 392e 3231 3620 3734 302e 3738 3836  129.216 740.7886
 00142820: 3535 2031 3231 3332 2e30 3032 3039 3520  55 12132.002095 
 00142830: 0a22 2063 6c69 702d 7061 7468 3d22 7572  ." clip-path="ur
-00142840: 6c28 2370 3332 6530 3930 6338 3031 2922  l(#p32e090c801)"
+00142840: 6c28 2370 3962 6633 3038 3236 3638 2922  l(#p9bf3082668)"
 00142850: 2073 7479 6c65 3d22 6669 6c6c 3a20 2366   style="fill: #f
 00142860: 6666 6639 393b 206f 7061 6369 7479 3a20  fff99; opacity: 
 00142870: 302e 3422 2f3e 0a20 2020 3c2f 673e 0a20  0.4"/>.   </g>. 
 00142880: 2020 3c67 2069 643d 2270 6174 6368 5f37    <g id="patch_7
 00142890: 3834 223e 0a20 2020 203c 7061 7468 2064  84">.    <path d
 001428a0: 3d22 4d20 3734 302e 3738 3836 3535 2031  ="M 740.788655 1
 001428b0: 3231 3532 2e32 3139 3130 3320 0a43 2037  2152.219103 .C 7
@@ -82585,16 +82585,16 @@
 00142980: 3039 3137 2037 3338 2e37 3638 3534 3820  0917 738.768548 
 00142990: 3132 3134 322e 3131 3035 3939 200a 4320  12142.110599 .C 
 001429a0: 3733 382e 3736 3835 3438 2031 3231 3435  738.768548 12145
 001429b0: 2e35 3830 3238 3120 3733 392e 3435 3531  .580281 739.4551
 001429c0: 3333 2031 3231 3439 2e30 3135 3931 3520  33 12149.015915 
 001429d0: 3734 302e 3738 3836 3535 2031 3231 3532  740.788655 12152
 001429e0: 2e32 3139 3130 3320 0a22 2063 6c69 702d  .219103 ." clip-
-001429f0: 7061 7468 3d22 7572 6c28 2370 3332 6530  path="url(#p32e0
-00142a00: 3930 6338 3031 2922 2073 7479 6c65 3d22  90c801)" style="
+001429f0: 7061 7468 3d22 7572 6c28 2370 3962 6633  path="url(#p9bf3
+00142a00: 3038 3236 3638 2922 2073 7479 6c65 3d22  082668)" style="
 00142a10: 6669 6c6c 3a20 2366 6666 6666 663b 206f  fill: #ffffff; o
 00142a20: 7061 6369 7479 3a20 302e 3422 2f3e 0a20  pacity: 0.4"/>. 
 00142a30: 2020 3c2f 673e 0a20 2020 3c67 2069 643d    </g>.   <g id=
 00142a40: 2274 6578 745f 3133 3233 223e 0a20 2020  "text_1323">.   
 00142a50: 203c 212d 2d20 3238 3020 2d2d 3e0a 2020   <!-- 280 -->.  
 00142a60: 2020 3c67 2073 7479 6c65 3d22 6669 6c6c    <g style="fill
 00142a70: 3a20 2332 3632 3632 3622 2074 7261 6e73  : #262626" trans
@@ -83069,16 +83069,16 @@
 001447c0: 3333 382e 3330 3333 3231 2031 3233 3337  338.303321 12337
 001447d0: 2e38 3432 3536 3220 0a43 2033 3430 2e33  .842562 .C 340.3
 001447e0: 3031 3535 3320 3132 3333 342e 3231 3838  01553 12334.2188
 001447f0: 3132 2033 3431 2e35 3937 3136 3720 3132  12 341.597167 12
 00144800: 3333 302e 3234 3938 3937 2033 3432 2e31  330.249897 342.1
 00144810: 3231 3833 3720 3132 3332 362e 3134 3531  21837 12326.1451
 00144820: 3137 200a 2220 636c 6970 2d70 6174 683d  17 ." clip-path=
-00144830: 2275 726c 2823 7061 6237 3934 3561 3463  "url(#pab7945a4c
-00144840: 3829 2220 7374 796c 653d 2266 696c 6c3a  8)" style="fill:
+00144830: 2275 726c 2823 7033 3261 3235 6266 3632  "url(#p32a25bf62
+00144840: 3929 2220 7374 796c 653d 2266 696c 6c3a  9)" style="fill:
 00144850: 2023 3661 3364 3961 3b20 6f70 6163 6974   #6a3d9a; opacit
 00144860: 793a 2030 2e34 222f 3e0a 2020 203c 2f67  y: 0.4"/>.   </g
 00144870: 3e0a 2020 203c 6720 6964 3d22 7061 7463  >.   <g id="patc
 00144880: 685f 3738 3922 3e0a 2020 2020 3c70 6174  h_789">.    <pat
 00144890: 6820 643d 224d 2033 3432 2e31 3231 3833  h d="M 342.12183
 001448a0: 3720 3132 3331 372e 3831 3532 3233 200a  7 12317.815223 .
 001448b0: 4320 3334 322e 3239 3833 3933 2031 3233  C 342.298393 123
@@ -83161,16 +83161,16 @@
 00144d80: 3334 342e 3236 3839 3437 2031 3233 3134  344.268947 12314
 00144d90: 2e30 3133 3234 3720 0a43 2033 3433 2e33  .013247 .C 343.3
 00144da0: 3336 3231 3320 3132 3331 352e 3134 3530  36213 12315.1450
 00144db0: 3935 2033 3432 2e36 3039 3435 3220 3132  95 342.609452 12
 00144dc0: 3331 362e 3433 3230 3031 2033 3432 2e31  316.432001 342.1
 00144dd0: 3231 3833 3720 3132 3331 372e 3831 3532  21837 12317.8152
 00144de0: 3233 200a 2220 636c 6970 2d70 6174 683d  23 ." clip-path=
-00144df0: 2275 726c 2823 7061 6237 3934 3561 3463  "url(#pab7945a4c
-00144e00: 3829 2220 7374 796c 653d 2266 696c 6c3a  8)" style="fill:
+00144df0: 2275 726c 2823 7033 3261 3235 6266 3632  "url(#p32a25bf62
+00144e00: 3929 2220 7374 796c 653d 2266 696c 6c3a  9)" style="fill:
 00144e10: 2023 6666 6666 3939 3b20 6f70 6163 6974   #ffff99; opacit
 00144e20: 793a 2030 2e34 222f 3e0a 2020 203c 2f67  y: 0.4"/>.   </g
 00144e30: 3e0a 2020 203c 6720 6964 3d22 7061 7463  >.   <g id="patc
 00144e40: 685f 3739 3022 3e0a 2020 2020 3c70 6174  h_790">.    <pat
 00144e50: 6820 643d 224d 2033 3432 2e31 3231 3833  h d="M 342.12183
 00144e60: 3720 3132 3332 362e 3134 3531 3137 200a  7 12326.145117 .
 00144e70: 4320 3334 322e 3239 3833 3933 2031 3233  C 342.298393 123
@@ -83188,16 +83188,16 @@
 00144f30: 3533 3820 3334 312e 3430 3932 3134 2031  538 341.409214 1
 00144f40: 3233 3231 2e39 3830 3137 200a 4320 3334  2321.98017 .C 34
 00144f50: 312e 3430 3932 3134 2031 3233 3233 2e33  1.409214 12323.3
 00144f60: 3938 3830 3320 3334 312e 3635 3031 3838  98803 341.650188
 00144f70: 2031 3233 3234 2e38 3037 3138 3420 3334   12324.807184 34
 00144f80: 322e 3132 3138 3337 2031 3233 3236 2e31  2.121837 12326.1
 00144f90: 3435 3131 3720 0a22 2063 6c69 702d 7061  45117 ." clip-pa
-00144fa0: 7468 3d22 7572 6c28 2370 6162 3739 3435  th="url(#pab7945
-00144fb0: 6134 6338 2922 2073 7479 6c65 3d22 6669  a4c8)" style="fi
+00144fa0: 7468 3d22 7572 6c28 2370 3332 6132 3562  th="url(#p32a25b
+00144fb0: 6636 3239 2922 2073 7479 6c65 3d22 6669  f629)" style="fi
 00144fc0: 6c6c 3a20 2366 6464 6464 373b 206f 7061  ll: #fdddd7; opa
 00144fd0: 6369 7479 3a20 302e 3422 2f3e 0a20 2020  city: 0.4"/>.   
 00144fe0: 3c2f 673e 0a20 2020 3c67 2069 643d 2274  </g>.   <g id="t
 00144ff0: 6578 745f 3133 3333 223e 0a20 2020 203c  ext_1333">.    <
 00145000: 212d 2d20 3331 3033 202d 2d3e 0a20 2020  !-- 3103 -->.   
 00145010: 203c 6720 7374 796c 653d 2266 696c 6c3a   <g style="fill:
 00145020: 2023 3236 3236 3236 2220 7472 616e 7366   #262626" transf
@@ -83386,16 +83386,16 @@
 00145b90: 2035 3239 2e39 3638 3334 3320 3132 3333   529.968343 1233
 00145ba0: 332e 3234 3736 3136 200a 4320 3533 312e  3.247616 .C 531.
 00145bb0: 3337 3333 3731 2031 3233 3330 2e38 3532  373371 12330.852
 00145bc0: 3235 3520 3533 322e 3331 3830 3338 2031  255 532.318038 1
 00145bd0: 3233 3238 2e32 3135 3038 3420 3533 322e  2328.215084 532.
 00145be0: 3735 3335 3134 2031 3233 3235 2e34 3732  753514 12325.472
 00145bf0: 3431 3820 0a22 2063 6c69 702d 7061 7468  418 ." clip-path
-00145c00: 3d22 7572 6c28 2370 3439 3966 3737 3736  ="url(#p499f7776
-00145c10: 6664 2922 2073 7479 6c65 3d22 6669 6c6c  fd)" style="fill
+00145c00: 3d22 7572 6c28 2370 3336 3962 6238 3466  ="url(#p369bb84f
+00145c10: 3839 2922 2073 7479 6c65 3d22 6669 6c6c  89)" style="fill
 00145c20: 3a20 2336 6133 6439 613b 206f 7061 6369  : #6a3d9a; opaci
 00145c30: 7479 3a20 302e 3422 2f3e 0a20 2020 3c2f  ty: 0.4"/>.   </
 00145c40: 673e 0a20 2020 3c67 2069 643d 2270 6174  g>.   <g id="pat
 00145c50: 6368 5f37 3932 223e 0a20 2020 203c 7061  ch_792">.    <pa
 00145c60: 7468 2064 3d22 4d20 3533 322e 3735 3335  th d="M 532.7535
 00145c70: 3134 2031 3233 3138 2e34 3837 3932 3320  14 12318.487923 
 00145c80: 0a43 2035 3332 2e39 3336 3931 2031 3233  .C 532.93691 123
@@ -83478,16 +83478,16 @@
 00146150: 372e 3734 3735 2035 3335 2e36 3237 3836  7.7475 535.62786
 00146160: 3820 3132 3331 302e 3237 3937 3731 200a  8 12310.279771 .
 00146170: 4320 3533 342e 3136 3531 3039 2031 3233  C 534.165109 123
 00146180: 3132 2e38 3132 3034 3120 3533 332e 3139  12.812041 533.19
 00146190: 3031 3038 2031 3233 3135 2e35 3936 3330  0108 12315.59630
 001461a0: 3720 3533 322e 3735 3335 3134 2031 3233  7 532.753514 123
 001461b0: 3138 2e34 3837 3932 3320 0a22 2063 6c69  18.487923 ." cli
-001461c0: 702d 7061 7468 3d22 7572 6c28 2370 3439  p-path="url(#p49
-001461d0: 3966 3737 3736 6664 2922 2073 7479 6c65  9f7776fd)" style
+001461c0: 702d 7061 7468 3d22 7572 6c28 2370 3336  p-path="url(#p36
+001461d0: 3962 6238 3466 3839 2922 2073 7479 6c65  9bb84f89)" style
 001461e0: 3d22 6669 6c6c 3a20 2362 3135 3932 383b  ="fill: #b15928;
 001461f0: 206f 7061 6369 7479 3a20 302e 3422 2f3e   opacity: 0.4"/>
 00146200: 0a20 2020 3c2f 673e 0a20 2020 3c67 2069  .   </g>.   <g i
 00146210: 643d 2270 6174 6368 5f37 3933 223e 0a20  d="patch_793">. 
 00146220: 2020 203c 7061 7468 2064 3d22 4d20 3533     <path d="M 53
 00146230: 322e 3735 3335 3134 2031 3233 3235 2e34  2.753514 12325.4
 00146240: 3732 3431 3820 0a43 2035 3332 2e39 3336  72418 .C 532.936
@@ -83505,16 +83505,16 @@
 00146300: 302e 3831 3131 3733 2035 3332 2e34 3931  0.811173 532.491
 00146310: 3336 2031 3233 3231 2e39 3830 3137 200a  36 12321.98017 .
 00146320: 4320 3533 322e 3439 3133 3620 3132 3332  C 532.49136 1232
 00146330: 332e 3134 3931 3637 2035 3332 2e35 3738  3.149167 532.578
 00146340: 3939 2031 3233 3234 2e33 3136 3532 3220  99 12324.316522 
 00146350: 3533 322e 3735 3335 3134 2031 3233 3235  532.753514 12325
 00146360: 2e34 3732 3431 3820 0a22 2063 6c69 702d  .472418 ." clip-
-00146370: 7061 7468 3d22 7572 6c28 2370 3439 3966  path="url(#p499f
-00146380: 3737 3736 6664 2922 2073 7479 6c65 3d22  7776fd)" style="
+00146370: 7061 7468 3d22 7572 6c28 2370 3336 3962  path="url(#p369b
+00146380: 6238 3466 3839 2922 2073 7479 6c65 3d22  b84f89)" style="
 00146390: 6669 6c6c 3a20 2363 3636 3938 383b 206f  fill: #c66988; o
 001463a0: 7061 6369 7479 3a20 302e 3422 2f3e 0a20  pacity: 0.4"/>. 
 001463b0: 2020 3c2f 673e 0a20 2020 3c67 2069 643d    </g>.   <g id=
 001463c0: 2274 6578 745f 3133 3338 223e 0a20 2020  "text_1338">.   
 001463d0: 203c 212d 2d20 3331 3033 202d 2d3e 0a20   <!-- 3103 -->. 
 001463e0: 2020 203c 6720 7374 796c 653d 2266 696c     <g style="fil
 001463f0: 6c3a 2023 3236 3236 3236 2220 7472 616e  l: #262626" tran
@@ -83717,16 +83717,16 @@
 00147040: 3820 3732 312e 3938 3336 3336 2031 3233  8 721.983636 123
 00147050: 3330 2e37 3635 3737 3520 0a43 2037 3232  30.765775 .C 722
 00147060: 2e39 3632 3839 3720 3132 3332 392e 3832  .962897 12329.82
 00147070: 3636 3033 2037 3233 2e37 3738 3238 2031  6603 723.77828 1
 00147080: 3233 3238 2e37 3330 3237 3920 3732 342e  2328.730279 724.
 00147090: 3339 3630 3038 2031 3233 3237 2e35 3232  396008 12327.522
 001470a0: 3231 3920 0a22 2063 6c69 702d 7061 7468  219 ." clip-path
-001470b0: 3d22 7572 6c28 2370 3632 3431 3933 6163  ="url(#p624193ac
-001470c0: 3931 2922 2073 7479 6c65 3d22 6669 6c6c  91)" style="fill
+001470b0: 3d22 7572 6c28 2370 3462 6639 3561 3938  ="url(#p4bf95a98
+001470c0: 3465 2922 2073 7479 6c65 3d22 6669 6c6c  4e)" style="fill
 001470d0: 3a20 2366 6666 6639 393b 206f 7061 6369  : #ffff99; opaci
 001470e0: 7479 3a20 302e 3422 2f3e 0a20 2020 3c2f  ty: 0.4"/>.   </
 001470f0: 673e 0a20 2020 3c67 2069 643d 2270 6174  g>.   <g id="pat
 00147100: 6368 5f37 3935 223e 0a20 2020 203c 7061  ch_795">.    <pa
 00147110: 7468 2064 3d22 4d20 3732 342e 3339 3630  th d="M 724.3960
 00147120: 3038 2031 3233 3136 2e34 3338 3132 3120  08 12316.438121 
 00147130: 0a43 2037 3235 2e32 3733 3235 3220 3132  .C 725.273252 12
@@ -83809,16 +83809,16 @@
 00147600: 3936 3431 2037 3238 2e36 3731 3136 3320  9641 728.671163 
 00147610: 3132 3330 342e 3739 3935 3639 200a 4320  12304.799569 .C 
 00147620: 3732 362e 3533 3439 3739 2031 3233 3038  726.534979 12308
 00147630: 2e33 3739 3439 3620 3732 352e 3038 3530  .379496 725.0850
 00147640: 3839 2031 3233 3132 2e33 3236 3633 3420  89 12312.326634 
 00147650: 3732 342e 3339 3630 3038 2031 3233 3136  724.396008 12316
 00147660: 2e34 3338 3132 3120 0a22 2063 6c69 702d  .438121 ." clip-
-00147670: 7061 7468 3d22 7572 6c28 2370 3632 3431  path="url(#p6241
-00147680: 3933 6163 3931 2922 2073 7479 6c65 3d22  93ac91)" style="
+00147670: 7061 7468 3d22 7572 6c28 2370 3462 6639  path="url(#p4bf9
+00147680: 3561 3938 3465 2922 2073 7479 6c65 3d22  5a984e)" style="
 00147690: 6669 6c6c 3a20 2362 3135 3932 383b 206f  fill: #b15928; o
 001476a0: 7061 6369 7479 3a20 302e 3422 2f3e 0a20  pacity: 0.4"/>. 
 001476b0: 2020 3c2f 673e 0a20 2020 3c67 2069 643d    </g>.   <g id=
 001476c0: 2270 6174 6368 5f37 3936 223e 0a20 2020  "patch_796">.   
 001476d0: 203c 7061 7468 2064 3d22 4d20 3732 342e   <path d="M 724.
 001476e0: 3339 3630 3038 2031 3233 3237 2e35 3232  396008 12327.522
 001476f0: 3231 3920 0a43 2037 3235 2e32 3733 3235  219 .C 725.27325
@@ -83837,15 +83837,15 @@
 001477c0: 3933 3438 3033 2031 3233 3231 2e39 3830  934803 12321.980
 001477d0: 3137 200a 4320 3732 332e 3933 3438 3033  17 .C 723.934803
 001477e0: 2031 3233 3233 2e38 3337 3130 3320 3732   12323.837103 72
 001477f0: 342e 3038 3930 3639 2031 3233 3235 2e36  4.089069 12325.6
 00147800: 3930 3833 2037 3234 2e33 3936 3030 3820  9083 724.396008 
 00147810: 3132 3332 372e 3532 3232 3139 200a 2220  12327.522219 ." 
 00147820: 636c 6970 2d70 6174 683d 2275 726c 2823  clip-path="url(#
-00147830: 7036 3234 3139 3361 6339 3129 2220 7374  p624193ac91)" st
+00147830: 7034 6266 3935 6139 3834 6529 2220 7374  p4bf95a984e)" st
 00147840: 796c 653d 2266 696c 6c3a 2023 6666 6631  yle="fill: #fff1
 00147850: 3837 3b20 6f70 6163 6974 793a 2030 2e34  87; opacity: 0.4
 00147860: 222f 3e0a 2020 203c 2f67 3e0a 2020 203c  "/>.   </g>.   <
 00147870: 6720 6964 3d22 7465 7874 5f31 3334 3322  g id="text_1343"
 00147880: 3e0a 2020 2020 3c21 2d2d 2034 3339 202d  >.    <!-- 439 -
 00147890: 2d3e 0a20 2020 203c 6720 7374 796c 653d  ->.    <g style=
 001478a0: 2266 696c 6c3a 2023 3236 3236 3236 2220  "fill: #262626" 
@@ -83950,15 +83950,15 @@
 00147ed0: 3339 3036 3222 2f3e 0a20 2020 203c 2f67  39062"/>.    </g
 00147ee0: 3e0a 2020 203c 2f67 3e0a 2020 3c2f 673e  >.   </g>.  </g>
 00147ef0: 0a20 203c 6720 6964 3d22 7465 7874 5f31  .  <g id="text_1
 00147f00: 3334 3822 3e0a 2020 203c 212d 2d20 6874  348">.   <!-- ht
 00147f10: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
 00147f20: 2f62 696f 7072 6167 6d61 7469 6373 2f62  /biopragmatics/b
 00147f30: 696f 7265 6769 7374 7279 2028 3230 3233  ioregistry (2023
-00147f40: 2d30 352d 3036 2920 2d2d 3e0a 2020 203c  -05-06) -->.   <
+00147f40: 2d30 352d 3037 2920 2d2d 3e0a 2020 203c  -05-07) -->.   <
 00147f50: 6720 7374 796c 653d 2266 696c 6c3a 2023  g style="fill: #
 00147f60: 3830 3830 3830 3b20 6f70 6163 6974 793a  808080; opacity:
 00147f70: 2030 2e35 2220 7472 616e 7366 6f72 6d3d   0.5" transform=
 00147f80: 2274 7261 6e73 6c61 7465 2832 3236 2e36  "translate(226.6
 00147f90: 3833 3433 3720 3132 3431 372e 3038 3834  83437 12417.0884
 00147fa0: 3338 2920 7363 616c 6528 302e 3134 202d  38) scale(0.14 -
 00147fb0: 302e 3134 2922 3e0a 2020 2020 3c64 6566  0.14)">.    <def
@@ -84236,15 +84236,15 @@
 001490b0: 5361 6e73 2d32 6422 2078 3d22 3237 3330  Sans-2d" x="2730
 001490c0: 2e37 3537 3831 3222 2f3e 0a20 2020 203c  .757812"/>.    <
 001490d0: 7573 6520 786c 696e 6b3a 6872 6566 3d22  use xlink:href="
 001490e0: 2344 656a 6156 7553 616e 732d 3330 2220  #DejaVuSans-30" 
 001490f0: 783d 2232 3736 362e 3834 3137 3937 222f  x="2766.841797"/
 00149100: 3e0a 2020 2020 3c75 7365 2078 6c69 6e6b  >.    <use xlink
 00149110: 3a68 7265 663d 2223 4465 6a61 5675 5361  :href="#DejaVuSa
-00149120: 6e73 2d33 3622 2078 3d22 3238 3330 2e34  ns-36" x="2830.4
+00149120: 6e73 2d33 3722 2078 3d22 3238 3330 2e34  ns-37" x="2830.4
 00149130: 3634 3834 3422 2f3e 0a20 2020 203c 7573  64844"/>.    <us
 00149140: 6520 786c 696e 6b3a 6872 6566 3d22 2344  e xlink:href="#D
 00149150: 656a 6156 7553 616e 732d 3239 2220 783d  ejaVuSans-29" x=
 00149160: 2232 3839 342e 3038 3738 3931 222f 3e0a  "2894.087891"/>.
 00149170: 2020 203c 2f67 3e0a 2020 3c2f 673e 0a20     </g>.  </g>. 
 00149180: 3c2f 673e 0a20 3c64 6566 733e 0a20 203c  </g>. <defs>.  <
 00149190: 636c 6970 5061 7468 2069 643d 2270 6461  clipPath id="pda
@@ -85436,15 +85436,15 @@
 0014dbb0: 6130 3236 6622 3e0a 2020 203c 7265 6374  a026f">.   <rect
 0014dbc0: 2078 3d22 3438 322e 3736 3636 3622 2079   x="482.76666" y
 0014dbd0: 3d22 3638 3932 2e38 3738 3730 3822 2077  ="6892.878708" w
 0014dbe0: 6964 7468 3d22 3130 322e 3233 3036 3535  idth="102.230655
 0014dbf0: 2220 6865 6967 6874 3d22 3636 2e30 3238  " height="66.028
 0014dc00: 3635 3222 2f3e 0a20 203c 2f63 6c69 7050  652"/>.  </clipP
 0014dc10: 6174 683e 0a20 203c 636c 6970 5061 7468  ath>.  <clipPath
-0014dc20: 2069 643d 2270 6531 3662 3537 6666 3864   id="pe16b57ff8d
+0014dc20: 2069 643d 2270 3238 3330 3938 3033 3233   id="p2830980323
 0014dc30: 223e 0a20 2020 3c72 6563 7420 783d 2236  ">.   <rect x="6
 0014dc40: 3935 2e30 3732 3930 3122 2079 3d22 3638  95.072901" y="68
 0014dc50: 3839 2e31 3834 3437 3422 2077 6964 7468  89.184474" width
 0014dc60: 3d22 3130 322e 3233 3036 3535 2220 6865  ="102.230655" he
 0014dc70: 6967 6874 3d22 3733 2e34 3137 3132 222f  ight="73.41712"/
 0014dc80: 3e0a 2020 3c2f 636c 6970 5061 7468 3e0a  >.  </clipPath>.
 0014dc90: 2020 3c63 6c69 7050 6174 6820 6964 3d22    <clipPath id="
@@ -85775,15 +85775,15 @@
 0014f0e0: 3762 223e 0a20 2020 3c72 6563 7420 783d  7b">.   <rect x=
 0014f0f0: 2234 3832 2e37 3636 3636 2220 793d 2238  "482.76666" y="8
 0014f100: 3837 322e 3333 3032 3131 2220 7769 6474  872.330211" widt
 0014f110: 683d 2231 3032 2e32 3330 3635 3522 2068  h="102.230655" h
 0014f120: 6569 6768 743d 2236 342e 3235 3632 3134  eight="64.256214
 0014f130: 222f 3e0a 2020 3c2f 636c 6970 5061 7468  "/>.  </clipPath
 0014f140: 3e0a 2020 3c63 6c69 7050 6174 6820 6964  >.  <clipPath id
-0014f150: 3d22 7032 3461 3262 3762 3633 3522 3e0a  ="p24a2b7b635">.
+0014f150: 3d22 7062 6238 3963 6261 3533 3922 3e0a  ="pbb89cba539">.
 0014f160: 2020 203c 7265 6374 2078 3d22 3639 352e     <rect x="695.
 0014f170: 3037 3239 3031 2220 793d 2238 3837 332e  072901" y="8873.
 0014f180: 3335 3336 3234 2220 7769 6474 683d 2231  353624" width="1
 0014f190: 3032 2e32 3330 3635 3522 2068 6569 6768  02.230655" heigh
 0014f1a0: 743d 2236 322e 3230 3933 3837 222f 3e0a  t="62.209387"/>.
 0014f1b0: 2020 3c2f 636c 6970 5061 7468 3e0a 2020    </clipPath>.  
 0014f1c0: 3c63 6c69 7050 6174 6820 6964 3d22 7034  <clipPath id="p4
@@ -85882,16 +85882,16 @@
 0014f790: 643d 2270 6436 6263 3766 3638 3464 223e  d="pd6bc7f684d">
 0014f7a0: 0a20 2020 3c72 6563 7420 783d 2235 382e  .   <rect x="58.
 0014f7b0: 3135 3431 3738 2220 793d 2239 3538 332e  154178" y="9583.
 0014f7c0: 3332 3230 3332 2220 7769 6474 683d 2231  322032" width="1
 0014f7d0: 3032 2e32 3330 3635 3522 2068 6569 6768  02.230655" heigh
 0014f7e0: 743d 2238 312e 3232 3931 3431 222f 3e0a  t="81.229141"/>.
 0014f7f0: 2020 3c2f 636c 6970 5061 7468 3e0a 2020    </clipPath>.  
-0014f800: 3c63 6c69 7050 6174 6820 6964 3d22 7064  <clipPath id="pd
-0014f810: 6538 3965 6265 3232 3122 3e0a 2020 203c  e89ebe221">.   <
+0014f800: 3c63 6c69 7050 6174 6820 6964 3d22 7063  <clipPath id="pc
+0014f810: 3537 3465 3931 6237 3822 3e0a 2020 203c  574e91b78">.   <
 0014f820: 7265 6374 2078 3d22 3237 302e 3436 3034  rect x="270.4604
 0014f830: 3139 2220 793d 2239 3539 332e 3531 3731  19" y="9593.5171
 0014f840: 3437 2220 7769 6474 683d 2231 3032 2e32  47" width="102.2
 0014f850: 3330 3635 3522 2068 6569 6768 743d 2236  30655" height="6
 0014f860: 302e 3833 3839 3122 2f3e 0a20 203c 2f63  0.83891"/>.  </c
 0014f870: 6c69 7050 6174 683e 0a20 203c 636c 6970  lipPath>.  <clip
 0014f880: 5061 7468 2069 643d 2270 6564 3864 6261  Path id="ped8dba
@@ -85936,24 +85936,24 @@
 0014faf0: 2270 3834 3034 3564 3331 3162 223e 0a20  "p84045d311b">. 
 0014fb00: 2020 3c72 6563 7420 783d 2236 3935 2e30    <rect x="695.0
 0014fb10: 3732 3930 3122 2079 3d22 3937 3636 2e38  72901" y="9766.8
 0014fb20: 3739 3935 3522 2077 6964 7468 3d22 3130  79955" width="10
 0014fb30: 322e 3233 3036 3535 2220 6865 6967 6874  2.230655" height
 0014fb40: 3d22 3733 2e38 3532 3433 3722 2f3e 0a20  ="73.852437"/>. 
 0014fb50: 203c 2f63 6c69 7050 6174 683e 0a20 203c   </clipPath>.  <
-0014fb60: 636c 6970 5061 7468 2069 643d 2270 6338  clipPath id="pc8
-0014fb70: 3463 6464 6366 6431 223e 0a20 2020 3c72  4cddcfd1">.   <r
+0014fb60: 636c 6970 5061 7468 2069 643d 2270 3936  clipPath id="p96
+0014fb70: 6436 3238 6236 3233 223e 0a20 2020 3c72  d628b623">.   <r
 0014fb80: 6563 7420 783d 2235 382e 3135 3431 3738  ect x="58.154178
 0014fb90: 2220 793d 2239 3933 392e 3130 3434 3236  " y="9939.104426
 0014fba0: 2220 7769 6474 683d 2231 3032 2e32 3330  " width="102.230
 0014fbb0: 3635 3522 2068 6569 6768 743d 2238 392e  655" height="89.
 0014fbc0: 3134 3236 3337 222f 3e0a 2020 3c2f 636c  142637"/>.  </cl
 0014fbd0: 6970 5061 7468 3e0a 2020 3c63 6c69 7050  ipPath>.  <clipP
-0014fbe0: 6174 6820 6964 3d22 7033 6635 3666 6132  ath id="p3f56fa2
-0014fbf0: 6465 3022 3e0a 2020 203c 7265 6374 2078  de0">.   <rect x
+0014fbe0: 6174 6820 6964 3d22 7037 6437 3934 3039  ath id="p7d79409
+0014fbf0: 3136 6322 3e0a 2020 203c 7265 6374 2078  16c">.   <rect x
 0014fc00: 3d22 3237 302e 3436 3034 3139 2220 793d  ="270.460419" y=
 0014fc10: 2239 3934 312e 3539 3936 3335 2220 7769  "9941.599635" wi
 0014fc20: 6474 683d 2231 3032 2e32 3330 3635 3522  dth="102.230655"
 0014fc30: 2068 6569 6768 743d 2238 342e 3135 3232   height="84.1522
 0014fc40: 3138 222f 3e0a 2020 3c2f 636c 6970 5061  18"/>.  </clipPa
 0014fc50: 7468 3e0a 2020 3c63 6c69 7050 6174 6820  th>.  <clipPath 
 0014fc60: 6964 3d22 7033 3330 3836 3038 3433 3622  id="p3308608436"
@@ -86185,15 +86185,15 @@
 00150a80: 3322 3e0a 2020 203c 7265 6374 2078 3d22  3">.   <rect x="
 00150a90: 3639 352e 3037 3239 3031 2220 793d 2231  695.072901" y="1
 00150aa0: 3132 3039 2e38 3130 3135 3222 2077 6964  1209.810152" wid
 00150ab0: 7468 3d22 3130 322e 3233 3036 3535 2220  th="102.230655" 
 00150ac0: 6865 6967 6874 3d22 3635 2e39 3035 3138  height="65.90518
 00150ad0: 3222 2f3e 0a20 203c 2f63 6c69 7050 6174  2"/>.  </clipPat
 00150ae0: 683e 0a20 203c 636c 6970 5061 7468 2069  h>.  <clipPath i
-00150af0: 643d 2270 3066 3434 3364 6532 3830 223e  d="p0f443de280">
+00150af0: 643d 2270 3162 3234 6539 3633 6632 223e  d="p1b24e963f2">
 00150b00: 0a20 2020 3c72 6563 7420 783d 2235 382e  .   <rect x="58.
 00150b10: 3135 3431 3738 2220 793d 2231 3133 3739  154178" y="11379
 00150b20: 2e32 3432 3736 3322 2077 6964 7468 3d22  .242763" width="
 00150b30: 3130 322e 3233 3036 3535 2220 6865 6967  102.230655" heig
 00150b40: 6874 3d22 3836 2e37 3739 3130 3222 2f3e  ht="86.779102"/>
 00150b50: 0a20 203c 2f63 6c69 7050 6174 683e 0a20  .  </clipPath>. 
 00150b60: 203c 636c 6970 5061 7468 2069 643d 2270   <clipPath id="p
@@ -86208,16 +86208,16 @@
 00150bf0: 3362 3838 3863 6622 3e0a 2020 203c 7265  3b888cf">.   <re
 00150c00: 6374 2078 3d22 3438 322e 3736 3636 3622  ct x="482.76666"
 00150c10: 2079 3d22 3131 3337 382e 3736 3232 3434   y="11378.762244
 00150c20: 2220 7769 6474 683d 2231 3032 2e32 3330  " width="102.230
 00150c30: 3635 3522 2068 6569 6768 743d 2238 372e  655" height="87.
 00150c40: 3734 3031 3431 222f 3e0a 2020 3c2f 636c  740141"/>.  </cl
 00150c50: 6970 5061 7468 3e0a 2020 3c63 6c69 7050  ipPath>.  <clipP
-00150c60: 6174 6820 6964 3d22 7061 6637 3433 3330  ath id="paf74330
-00150c70: 3330 3422 3e0a 2020 203c 7265 6374 2078  304">.   <rect x
+00150c60: 6174 6820 6964 3d22 7038 3037 3139 6365  ath id="p80719ce
+00150c70: 6662 3522 3e0a 2020 203c 7265 6374 2078  fb5">.   <rect x
 00150c80: 3d22 3639 352e 3037 3239 3031 2220 793d  ="695.072901" y=
 00150c90: 2231 3133 3735 2e32 3533 3634 2220 7769  "11375.25364" wi
 00150ca0: 6474 683d 2231 3032 2e32 3330 3635 3522  dth="102.230655"
 00150cb0: 2068 6569 6768 743d 2239 342e 3735 3733   height="94.7573
 00150cc0: 3439 222f 3e0a 2020 3c2f 636c 6970 5061  49"/>.  </clipPa
 00150cd0: 7468 3e0a 2020 3c63 6c69 7050 6174 6820  th>.  <clipPath 
 00150ce0: 6964 3d22 7030 3239 6661 6634 3631 6122  id="p029faf461a"
@@ -86247,15 +86247,15 @@
 00150e60: 3630 6522 3e0a 2020 203c 7265 6374 2078  60e">.   <rect x
 00150e70: 3d22 3639 352e 3037 3239 3031 2220 793d  ="695.072901" y=
 00150e80: 2231 3135 3638 2e31 3131 3036 3722 2077  "11568.111067" w
 00150e90: 6964 7468 3d22 3130 322e 3233 3036 3535  idth="102.230655
 00150ea0: 2220 6865 6967 6874 3d22 3638 2e37 3831  " height="68.781
 00150eb0: 3633 3722 2f3e 0a20 203c 2f63 6c69 7050  637"/>.  </clipP
 00150ec0: 6174 683e 0a20 203c 636c 6970 5061 7468  ath>.  <clipPath
-00150ed0: 2069 643d 2270 3763 6361 6563 3664 6139   id="p7ccaec6da9
+00150ed0: 2069 643d 2270 3138 3766 3938 6565 3663   id="p187f98ee6c
 00150ee0: 223e 0a20 2020 3c72 6563 7420 783d 2235  ">.   <rect x="5
 00150ef0: 382e 3135 3431 3738 2220 793d 2231 3137  8.154178" y="117
 00150f00: 3334 2e34 3333 3239 3222 2077 6964 7468  34.433292" width
 00150f10: 3d22 3130 322e 3233 3036 3535 2220 6865  ="102.230655" he
 00150f20: 6967 6874 3d22 3935 2e38 3736 3332 3922  ight="95.876329"
 00150f30: 2f3e 0a20 203c 2f63 6c69 7050 6174 683e  />.  </clipPath>
 00150f40: 0a20 203c 636c 6970 5061 7468 2069 643d  .  <clipPath id=
@@ -86332,47 +86332,47 @@
 001513b0: 3d22 7062 6162 6139 6333 3266 3122 3e0a  ="pbaba9c32f1">.
 001513c0: 2020 203c 7265 6374 2078 3d22 3438 322e     <rect x="482.
 001513d0: 3736 3636 3622 2079 3d22 3132 3039 392e  76666" y="12099.
 001513e0: 3430 3233 3635 2220 7769 6474 683d 2231  402365" width="1
 001513f0: 3032 2e32 3330 3635 3522 2068 6569 6768  02.230655" heigh
 00151400: 743d 2238 352e 3431 3634 3638 222f 3e0a  t="85.416468"/>.
 00151410: 2020 3c2f 636c 6970 5061 7468 3e0a 2020    </clipPath>.  
-00151420: 3c63 6c69 7050 6174 6820 6964 3d22 7033  <clipPath id="p3
-00151430: 3265 3039 3063 3830 3122 3e0a 2020 203c  2e090c801">.   <
+00151420: 3c63 6c69 7050 6174 6820 6964 3d22 7039  <clipPath id="p9
+00151430: 6266 3330 3832 3636 3822 3e0a 2020 203c  bf3082668">.   <
 00151440: 7265 6374 2078 3d22 3639 352e 3037 3239  rect x="695.0729
 00151450: 3031 2220 793d 2231 3231 3039 2e38 3736  01" y="12109.876
 00151460: 3834 3622 2077 6964 7468 3d22 3130 322e  846" width="102.
 00151470: 3233 3036 3535 2220 6865 6967 6874 3d22  230655" height="
 00151480: 3634 2e34 3637 3530 3622 2f3e 0a20 203c  64.467506"/>.  <
 00151490: 2f63 6c69 7050 6174 683e 0a20 203c 636c  /clipPath>.  <cl
 001514a0: 6970 5061 7468 2069 643d 2270 3263 3665  ipPath id="p2c6e
 001514b0: 6265 6339 3637 223e 0a20 2020 3c72 6563  bec967">.   <rec
 001514c0: 7420 783d 2235 382e 3135 3431 3738 2220  t x="58.154178" 
 001514d0: 793d 2231 3232 3738 2e33 3330 3937 3222  y="12278.330972"
 001514e0: 2077 6964 7468 3d22 3130 322e 3233 3036   width="102.2306
 001514f0: 3535 2220 6865 6967 6874 3d22 3837 2e32  55" height="87.2
 00151500: 3938 3339 3722 2f3e 0a20 203c 2f63 6c69  98397"/>.  </cli
 00151510: 7050 6174 683e 0a20 203c 636c 6970 5061  pPath>.  <clipPa
-00151520: 7468 2069 643d 2270 6162 3739 3435 6134  th id="pab7945a4
-00151530: 6338 223e 0a20 2020 3c72 6563 7420 783d  c8">.   <rect x=
+00151520: 7468 2069 643d 2270 3332 6132 3562 6636  th id="p32a25bf6
+00151530: 3239 223e 0a20 2020 3c72 6563 7420 783d  29">.   <rect x=
 00151540: 2232 3730 2e34 3630 3431 3922 2079 3d22  "270.460419" y="
 00151550: 3132 3238 322e 3930 3333 3622 2077 6964  12282.90336" wid
 00151560: 7468 3d22 3130 322e 3233 3036 3535 2220  th="102.230655" 
 00151570: 6865 6967 6874 3d22 3738 2e31 3533 3632  height="78.15362
 00151580: 222f 3e0a 2020 3c2f 636c 6970 5061 7468  "/>.  </clipPath
 00151590: 3e0a 2020 3c63 6c69 7050 6174 6820 6964  >.  <clipPath id
-001515a0: 3d22 7034 3939 6637 3737 3666 6422 3e0a  ="p499f7776fd">.
+001515a0: 3d22 7033 3639 6262 3834 6638 3922 3e0a  ="p369bb84f89">.
 001515b0: 2020 203c 7265 6374 2078 3d22 3438 322e     <rect x="482.
 001515c0: 3736 3636 3622 2079 3d22 3132 3239 322e  76666" y="12292.
 001515d0: 3836 3539 3937 2220 7769 6474 683d 2231  865997" width="1
 001515e0: 3032 2e32 3330 3635 3522 2068 6569 6768  02.230655" heigh
 001515f0: 743d 2235 382e 3232 3833 3436 222f 3e0a  t="58.228346"/>.
 00151600: 2020 3c2f 636c 6970 5061 7468 3e0a 2020    </clipPath>.  
-00151610: 3c63 6c69 7050 6174 6820 6964 3d22 7036  <clipPath id="p6
-00151620: 3234 3139 3361 6339 3122 3e0a 2020 203c  24193ac91">.   <
+00151610: 3c63 6c69 7050 6174 6820 6964 3d22 7034  <clipPath id="p4
+00151620: 6266 3935 6139 3834 6522 3e0a 2020 203c  bf95a984e">.   <
 00151630: 7265 6374 2078 3d22 3639 352e 3037 3239  rect x="695.0729
 00151640: 3031 2220 793d 2231 3232 3832 2e31 3339  01" y="12282.139
 00151650: 3932 3722 2077 6964 7468 3d22 3130 322e  927" width="102.
 00151660: 3233 3036 3535 2220 6865 6967 6874 3d22  230655" height="
 00151670: 3739 2e36 3830 3438 3622 2f3e 0a20 203c  79.680486"/>.  <
 00151680: 2f63 6c69 7050 6174 683e 0a20 3c2f 6465  /clipPath>. </de
 00151690: 6673 3e0a 3c2f 7376 673e 0a              fs>.</svg>.
```

### Comparing `bioregistry-0.9.6/docs/img/has_attribute.svg` & `bioregistry-0.9.7/docs/img/has_attribute.svg`

 * *Files 0% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 000001c0: 3032 2f32 322d 7264 662d 7379 6e74 6178  02/22-rdf-syntax
 000001d0: 2d6e 7323 223e 0a20 2020 3c63 633a 576f  -ns#">.   <cc:Wo
 000001e0: 726b 3e0a 2020 2020 3c64 633a 7479 7065  rk>.    <dc:type
 000001f0: 2072 6466 3a72 6573 6f75 7263 653d 2268   rdf:resource="h
 00000200: 7474 703a 2f2f 7075 726c 2e6f 7267 2f64  ttp://purl.org/d
 00000210: 632f 6463 6d69 7479 7065 2f53 7469 6c6c  c/dcmitype/Still
 00000220: 496d 6167 6522 2f3e 0a20 2020 203c 6463  Image"/>.    <dc
-00000230: 3a64 6174 653e 3230 3233 2d30 352d 3036  :date>2023-05-06
-00000240: 5430 313a 3038 3a33 382e 3534 3437 3936  T01:08:38.544796
+00000230: 3a64 6174 653e 3230 3233 2d30 352d 3037  :date>2023-05-07
+00000240: 5430 313a 3134 3a33 352e 3231 3138 3337  T01:14:35.211837
 00000250: 3c2f 6463 3a64 6174 653e 0a20 2020 203c  </dc:date>.    <
 00000260: 6463 3a66 6f72 6d61 743e 696d 6167 652f  dc:format>image/
 00000270: 7376 672b 786d 6c3c 2f64 633a 666f 726d  svg+xml</dc:form
 00000280: 6174 3e0a 2020 2020 3c64 633a 6372 6561  at>.    <dc:crea
 00000290: 746f 723e 0a20 2020 2020 3c63 633a 4167  tor>.     <cc:Ag
 000002a0: 656e 743e 0a20 2020 2020 203c 6463 3a74  ent>.      <dc:t
 000002b0: 6974 6c65 3e4d 6174 706c 6f74 6c69 6220  itle>Matplotlib 
@@ -4243,15 +4243,15 @@
 00010920: 3c2f 673e 0a20 203c 6720 6964 3d22 6178  </g>.  <g id="ax
 00010930: 6573 5f31 3522 2f3e 0a20 203c 6720 6964  es_15"/>.  <g id
 00010940: 3d22 6178 6573 5f31 3622 2f3e 0a20 203c  ="axes_16"/>.  <
 00010950: 6720 6964 3d22 7465 7874 5f37 3522 3e0a  g id="text_75">.
 00010960: 2020 203c 212d 2d20 6874 7470 733a 2f2f     <!-- https://
 00010970: 6769 7468 7562 2e63 6f6d 2f62 696f 7072  github.com/biopr
 00010980: 6167 6d61 7469 6373 2f62 696f 7265 6769  agmatics/bioregi
-00010990: 7374 7279 2028 3230 3233 2d30 352d 3036  stry (2023-05-06
+00010990: 7374 7279 2028 3230 3233 2d30 352d 3037  stry (2023-05-07
 000109a0: 2920 2d2d 3e0a 2020 203c 6720 7374 796c  ) -->.   <g styl
 000109b0: 653d 2266 696c 6c3a 2023 3830 3830 3830  e="fill: #808080
 000109c0: 3b20 6f70 6163 6974 793a 2030 2e35 2220  ; opacity: 0.5" 
 000109d0: 7472 616e 7366 6f72 6d3d 2274 7261 6e73  transform="trans
 000109e0: 6c61 7465 2832 3738 2e36 3736 3235 2035  late(278.67625 5
 000109f0: 3734 2e33 3336 3235 2920 7363 616c 6528  74.33625) scale(
 00010a00: 302e 3038 202d 302e 3038 2922 3e0a 2020  0.08 -0.08)">.  
@@ -4518,15 +4518,15 @@
 00011a50: 4465 6a61 5675 5361 6e73 2d32 6422 2078  DejaVuSans-2d" x
 00011a60: 3d22 3237 3330 2e37 3537 3831 3222 2f3e  ="2730.757812"/>
 00011a70: 0a20 2020 203c 7573 6520 786c 696e 6b3a  .    <use xlink:
 00011a80: 6872 6566 3d22 2344 656a 6156 7553 616e  href="#DejaVuSan
 00011a90: 732d 3330 2220 783d 2232 3736 362e 3834  s-30" x="2766.84
 00011aa0: 3137 3937 222f 3e0a 2020 2020 3c75 7365  1797"/>.    <use
 00011ab0: 2078 6c69 6e6b 3a68 7265 663d 2223 4465   xlink:href="#De
-00011ac0: 6a61 5675 5361 6e73 2d33 3622 2078 3d22  jaVuSans-36" x="
+00011ac0: 6a61 5675 5361 6e73 2d33 3722 2078 3d22  jaVuSans-37" x="
 00011ad0: 3238 3330 2e34 3634 3834 3422 2f3e 0a20  2830.464844"/>. 
 00011ae0: 2020 203c 7573 6520 786c 696e 6b3a 6872     <use xlink:hr
 00011af0: 6566 3d22 2344 656a 6156 7553 616e 732d  ef="#DejaVuSans-
 00011b00: 3239 2220 783d 2232 3839 342e 3038 3738  29" x="2894.0878
 00011b10: 3931 222f 3e0a 2020 203c 2f67 3e0a 2020  91"/>.   </g>.  
 00011b20: 3c2f 673e 0a20 3c2f 673e 0a3c 2f73 7667  </g>. </g>.</svg
 00011b30: 3e0a                                     >.
```

### Comparing `bioregistry-0.9.6/docs/img/providers.svg` & `bioregistry-0.9.7/docs/img/providers.svg`

 * *Files 0% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 000001c0: 3032 2f32 322d 7264 662d 7379 6e74 6178  02/22-rdf-syntax
 000001d0: 2d6e 7323 223e 0a20 2020 3c63 633a 576f  -ns#">.   <cc:Wo
 000001e0: 726b 3e0a 2020 2020 3c64 633a 7479 7065  rk>.    <dc:type
 000001f0: 2072 6466 3a72 6573 6f75 7263 653d 2268   rdf:resource="h
 00000200: 7474 703a 2f2f 7075 726c 2e6f 7267 2f64  ttp://purl.org/d
 00000210: 632f 6463 6d69 7479 7065 2f53 7469 6c6c  c/dcmitype/Still
 00000220: 496d 6167 6522 2f3e 0a20 2020 203c 6463  Image"/>.    <dc
-00000230: 3a64 6174 653e 3230 3233 2d30 352d 3036  :date>2023-05-06
-00000240: 5430 313a 3132 3a33 332e 3038 3337 3130  T01:12:33.083710
+00000230: 3a64 6174 653e 3230 3233 2d30 352d 3037  :date>2023-05-07
+00000240: 5430 313a 3138 3a30 362e 3137 3333 3633  T01:18:06.173363
 00000250: 3c2f 6463 3a64 6174 653e 0a20 2020 203c  </dc:date>.    <
 00000260: 6463 3a66 6f72 6d61 743e 696d 6167 652f  dc:format>image/
 00000270: 7376 672b 786d 6c3c 2f64 633a 666f 726d  svg+xml</dc:form
 00000280: 6174 3e0a 2020 2020 3c64 633a 6372 6561  at>.    <dc:crea
 00000290: 746f 723e 0a20 2020 2020 3c63 633a 4167  tor>.     <cc:Ag
 000002a0: 656e 743e 0a20 2020 2020 203c 6463 3a74  ent>.      <dc:t
 000002b0: 6974 6c65 3e4d 6174 706c 6f74 6c69 6220  itle>Matplotlib 
@@ -1304,15 +1304,15 @@
 00005170: 3b20 7374 726f 6b65 2d6c 696e 6563 6170  ; stroke-linecap
 00005180: 3a20 7371 7561 7265 222f 3e0a 2020 203c  : square"/>.   <
 00005190: 2f67 3e0a 2020 3c2f 673e 0a20 203c 6720  /g>.  </g>.  <g 
 000051a0: 6964 3d22 7465 7874 5f31 3522 3e0a 2020  id="text_15">.  
 000051b0: 203c 212d 2d20 6874 7470 733a 2f2f 6769   <!-- https://gi
 000051c0: 7468 7562 2e63 6f6d 2f62 696f 7072 6167  thub.com/bioprag
 000051d0: 6d61 7469 6373 2f62 696f 7265 6769 7374  matics/bioregist
-000051e0: 7279 2028 3230 3233 2d30 352d 3036 2920  ry (2023-05-06) 
+000051e0: 7279 2028 3230 3233 2d30 352d 3037 2920  ry (2023-05-07) 
 000051f0: 2d2d 3e0a 2020 203c 6720 7374 796c 653d  -->.   <g style=
 00005200: 2266 696c 6c3a 2023 3830 3830 3830 3b20  "fill: #808080; 
 00005210: 6f70 6163 6974 793a 2030 2e35 2220 7472  opacity: 0.5" tr
 00005220: 616e 7366 6f72 6d3d 2274 7261 6e73 6c61  ansform="transla
 00005230: 7465 2835 3932 2e33 3336 3235 2032 3433  te(592.33625 243
 00005240: 2e33 3233 3735 2920 726f 7461 7465 282d  .32375) rotate(-
 00005250: 3930 2920 7363 616c 6528 302e 3038 202d  90) scale(0.08 -
@@ -1755,15 +1755,15 @@
 00006da0: 656a 6156 7553 616e 732d 3264 2220 783d  ejaVuSans-2d" x=
 00006db0: 2232 3733 302e 3735 3738 3132 222f 3e0a  "2730.757812"/>.
 00006dc0: 2020 2020 3c75 7365 2078 6c69 6e6b 3a68      <use xlink:h
 00006dd0: 7265 663d 2223 4465 6a61 5675 5361 6e73  ref="#DejaVuSans
 00006de0: 2d33 3022 2078 3d22 3237 3636 2e38 3431  -30" x="2766.841
 00006df0: 3739 3722 2f3e 0a20 2020 203c 7573 6520  797"/>.    <use 
 00006e00: 786c 696e 6b3a 6872 6566 3d22 2344 656a  xlink:href="#Dej
-00006e10: 6156 7553 616e 732d 3336 2220 783d 2232  aVuSans-36" x="2
+00006e10: 6156 7553 616e 732d 3337 2220 783d 2232  aVuSans-37" x="2
 00006e20: 3833 302e 3436 3438 3434 222f 3e0a 2020  830.464844"/>.  
 00006e30: 2020 3c75 7365 2078 6c69 6e6b 3a68 7265    <use xlink:hre
 00006e40: 663d 2223 4465 6a61 5675 5361 6e73 2d32  f="#DejaVuSans-2
 00006e50: 3922 2078 3d22 3238 3934 2e30 3837 3839  9" x="2894.08789
 00006e60: 3122 2f3e 0a20 2020 3c2f 673e 0a20 203c  1"/>.   </g>.  <
 00006e70: 2f67 3e0a 203c 2f67 3e0a 203c 6465 6673  /g>. </g>. <defs
 00006e80: 3e0a 2020 3c63 6c69 7050 6174 6820 6964  >.  <clipPath id
```

### Comparing `bioregistry-0.9.6/docs/img/regex_report.svg` & `bioregistry-0.9.7/docs/img/regex_report.svg`

 * *Files 0% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 000001c0: 3032 2f32 322d 7264 662d 7379 6e74 6178  02/22-rdf-syntax
 000001d0: 2d6e 7323 223e 0a20 2020 3c63 633a 576f  -ns#">.   <cc:Wo
 000001e0: 726b 3e0a 2020 2020 3c64 633a 7479 7065  rk>.    <dc:type
 000001f0: 2072 6466 3a72 6573 6f75 7263 653d 2268   rdf:resource="h
 00000200: 7474 703a 2f2f 7075 726c 2e6f 7267 2f64  ttp://purl.org/d
 00000210: 632f 6463 6d69 7479 7065 2f53 7469 6c6c  c/dcmitype/Still
 00000220: 496d 6167 6522 2f3e 0a20 2020 203c 6463  Image"/>.    <dc
-00000230: 3a64 6174 653e 3230 3233 2d30 352d 3036  :date>2023-05-06
-00000240: 5430 313a 3132 3a33 342e 3138 3233 3136  T01:12:34.182316
+00000230: 3a64 6174 653e 3230 3233 2d30 352d 3037  :date>2023-05-07
+00000240: 5430 313a 3138 3a30 372e 3131 3036 3636  T01:18:07.110666
 00000250: 3c2f 6463 3a64 6174 653e 0a20 2020 203c  </dc:date>.    <
 00000260: 6463 3a66 6f72 6d61 743e 696d 6167 652f  dc:format>image/
 00000270: 7376 672b 786d 6c3c 2f64 633a 666f 726d  svg+xml</dc:form
 00000280: 6174 3e0a 2020 2020 3c64 633a 6372 6561  at>.    <dc:crea
 00000290: 746f 723e 0a20 2020 2020 3c63 633a 4167  tor>.     <cc:Ag
 000002a0: 656e 743e 0a20 2020 2020 203c 6463 3a74  ent>.      <dc:t
 000002b0: 6974 6c65 3e4d 6174 706c 6f74 6c69 6220  itle>Matplotlib
```

### Comparing `bioregistry-0.9.6/docs/img/xrefs.svg` & `bioregistry-0.9.7/docs/img/xrefs.svg`

 * *Files 0% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 000001c0: 3032 2f32 322d 7264 662d 7379 6e74 6178  02/22-rdf-syntax
 000001d0: 2d6e 7323 223e 0a20 2020 3c63 633a 576f  -ns#">.   <cc:Wo
 000001e0: 726b 3e0a 2020 2020 3c64 633a 7479 7065  rk>.    <dc:type
 000001f0: 2072 6466 3a72 6573 6f75 7263 653d 2268   rdf:resource="h
 00000200: 7474 703a 2f2f 7075 726c 2e6f 7267 2f64  ttp://purl.org/d
 00000210: 632f 6463 6d69 7479 7065 2f53 7469 6c6c  c/dcmitype/Still
 00000220: 496d 6167 6522 2f3e 0a20 2020 203c 6463  Image"/>.    <dc
-00000230: 3a64 6174 653e 3230 3233 2d30 352d 3036  :date>2023-05-06
-00000240: 5430 313a 3038 3a30 372e 3536 3134 3032  T01:08:07.561402
+00000230: 3a64 6174 653e 3230 3233 2d30 352d 3037  :date>2023-05-07
+00000240: 5430 313a 3134 3a30 362e 3635 3932 3031  T01:14:06.659201
 00000250: 3c2f 6463 3a64 6174 653e 0a20 2020 203c  </dc:date>.    <
 00000260: 6463 3a66 6f72 6d61 743e 696d 6167 652f  dc:format>image/
 00000270: 7376 672b 786d 6c3c 2f64 633a 666f 726d  svg+xml</dc:form
 00000280: 6174 3e0a 2020 2020 3c64 633a 6372 6561  at>.    <dc:crea
 00000290: 746f 723e 0a20 2020 2020 3c63 633a 4167  tor>.     <cc:Ag
 000002a0: 656e 743e 0a20 2020 2020 203c 6463 3a74  ent>.      <dc:t
 000002b0: 6974 6c65 3e4d 6174 706c 6f74 6c69 6220  itle>Matplotlib 
@@ -2920,15 +2920,15 @@
 0000b670: 352e 3638 3535 3437 222f 3e0a 2020 2020  5.685547"/>.    
 0000b680: 3c2f 673e 0a20 2020 3c2f 673e 0a20 203c  </g>.   </g>.  <
 0000b690: 2f67 3e0a 2020 3c67 2069 643d 2274 6578  /g>.  <g id="tex
 0000b6a0: 745f 3438 223e 0a20 2020 3c21 2d2d 2068  t_48">.   <!-- h
 0000b6b0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
 0000b6c0: 6d2f 6269 6f70 7261 676d 6174 6963 732f  m/biopragmatics/
 0000b6d0: 6269 6f72 6567 6973 7472 7920 2832 3032  bioregistry (202
-0000b6e0: 332d 3035 2d30 3629 202d 2d3e 0a20 2020  3-05-06) -->.   
+0000b6e0: 332d 3035 2d30 3729 202d 2d3e 0a20 2020  3-05-07) -->.   
 0000b6f0: 3c67 2073 7479 6c65 3d22 6669 6c6c 3a20  <g style="fill: 
 0000b700: 2338 3038 3038 303b 206f 7061 6369 7479  #808080; opacity
 0000b710: 3a20 302e 3522 2074 7261 6e73 666f 726d  : 0.5" transform
 0000b720: 3d22 7472 616e 736c 6174 6528 3539 322e  ="translate(592.
 0000b730: 3333 3632 3520 3234 332e 3332 3337 3529  33625 243.32375)
 0000b740: 2072 6f74 6174 6528 2d39 3029 2073 6361   rotate(-90) sca
 0000b750: 6c65 2830 2e30 3820 2d30 2e30 3829 223e  le(0.08 -0.08)">
@@ -3199,15 +3199,15 @@
 0000c7e0: 7553 616e 732d 3264 2220 783d 2232 3733  uSans-2d" x="273
 0000c7f0: 302e 3735 3738 3132 222f 3e0a 2020 2020  0.757812"/>.    
 0000c800: 3c75 7365 2078 6c69 6e6b 3a68 7265 663d  <use xlink:href=
 0000c810: 2223 4465 6a61 5675 5361 6e73 2d33 3022  "#DejaVuSans-30"
 0000c820: 2078 3d22 3237 3636 2e38 3431 3739 3722   x="2766.841797"
 0000c830: 2f3e 0a20 2020 203c 7573 6520 786c 696e  />.    <use xlin
 0000c840: 6b3a 6872 6566 3d22 2344 656a 6156 7553  k:href="#DejaVuS
-0000c850: 616e 732d 3336 2220 783d 2232 3833 302e  ans-36" x="2830.
+0000c850: 616e 732d 3337 2220 783d 2232 3833 302e  ans-37" x="2830.
 0000c860: 3436 3438 3434 222f 3e0a 2020 2020 3c75  464844"/>.    <u
 0000c870: 7365 2078 6c69 6e6b 3a68 7265 663d 2223  se xlink:href="#
 0000c880: 4465 6a61 5675 5361 6e73 2d32 3922 2078  DejaVuSans-29" x
 0000c890: 3d22 3238 3934 2e30 3837 3839 3122 2f3e  ="2894.087891"/>
 0000c8a0: 0a20 2020 3c2f 673e 0a20 203c 2f67 3e0a  .   </g>.  </g>.
 0000c8b0: 203c 2f67 3e0a 203c 6465 6673 3e0a 2020   </g>. <defs>.  
 0000c8c0: 3c63 6c69 7050 6174 6820 6964 3d22 7031  <clipPath id="p1
```

### Comparing `bioregistry-0.9.6/docs/source/conf.py` & `bioregistry-0.9.7/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "bioregistry"
 copyright = f"{date.today().year}, Charles Tapley Hoyt"
 author = "Charles Tapley Hoyt"
 
 # The full version, including alpha/beta/rc tags.
-release = "0.9.6"
+release = "0.9.7"
 
 # The short X.Y version.
 parsed_version = re.match(
     "(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?:-(?P<release>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?(?:\+(?P<build>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?",
     release,
 )
 version = parsed_version.expand("\g<major>.\g<minor>.\g<patch>")
```

### Comparing `bioregistry-0.9.6/docs/source/deployment.rst` & `bioregistry-0.9.7/docs/source/deployment.rst`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/docs/source/index.rst` & `bioregistry-0.9.7/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/docs/source/logo.png` & `bioregistry-0.9.7/docs/source/logo.png`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/setup.cfg` & `bioregistry-0.9.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = bioregistry
-version = 0.9.6
+version = 0.9.7
 description = Integrated registry of biological databases and nomenclatures
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/biopragmatics/bioregistry
 download_url = https://github.com/biopragmatics/bioregistry/releases
 project_urls = 
 	Bug Tracker = https://github.com/biopragmatics/bioregistry/issues
```

### Comparing `bioregistry-0.9.6/src/bioregistry/__init__.py` & `bioregistry-0.9.7/src/bioregistry/__init__.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/align/__init__.py` & `bioregistry-0.9.7/src/bioregistry/align/__init__.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/align/biocontext.py` & `bioregistry-0.9.7/src/bioregistry/align/biocontext.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/align/biolink.py` & `bioregistry-0.9.7/src/bioregistry/align/biolink.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/align/bioportal.py` & `bioregistry-0.9.7/src/bioregistry/align/bioportal.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/align/cellosaurus.py` & `bioregistry-0.9.7/src/bioregistry/align/cellosaurus.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/align/cheminf.py` & `bioregistry-0.9.7/src/bioregistry/align/cheminf.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/align/edam.py` & `bioregistry-0.9.7/src/bioregistry/align/edam.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/align/fairsharing.py` & `bioregistry-0.9.7/src/bioregistry/align/fairsharing.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/align/go.py` & `bioregistry-0.9.7/src/bioregistry/align/go.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/align/hl7.py` & `bioregistry-0.9.7/src/bioregistry/align/hl7.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/align/n2t.py` & `bioregistry-0.9.7/src/bioregistry/align/n2t.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/align/ncbi.py` & `bioregistry-0.9.7/src/bioregistry/align/ncbi.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/align/obofoundry.py` & `bioregistry-0.9.7/src/bioregistry/align/obofoundry.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/align/ols.py` & `bioregistry-0.9.7/src/bioregistry/align/ols.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/align/ontobee.py` & `bioregistry-0.9.7/src/bioregistry/align/ontobee.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/align/prefixcommons.py` & `bioregistry-0.9.7/src/bioregistry/align/prefixcommons.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/align/re3data.py` & `bioregistry-0.9.7/src/bioregistry/align/re3data.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/align/uniprot.py` & `bioregistry-0.9.7/src/bioregistry/align/uniprot.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/align/utils.py` & `bioregistry-0.9.7/src/bioregistry/align/utils.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/align/wikidata.py` & `bioregistry-0.9.7/src/bioregistry/align/wikidata.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/analysis/title_tfidf.py` & `bioregistry-0.9.7/src/bioregistry/analysis/title_tfidf.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/app/api.py` & `bioregistry-0.9.7/src/bioregistry/app/api.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/app/cli.py` & `bioregistry-0.9.7/src/bioregistry/app/cli.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/app/constants.py` & `bioregistry-0.9.7/src/bioregistry/app/constants.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/app/impl.py` & `bioregistry-0.9.7/src/bioregistry/app/impl.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/app/static/logo.svg` & `bioregistry-0.9.7/src/bioregistry/app/static/logo.svg`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/app/templates/base.html` & `bioregistry-0.9.7/src/bioregistry/app/templates/base.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/app/templates/collection.html` & `bioregistry-0.9.7/src/bioregistry/app/templates/collection.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/app/templates/collections.html` & `bioregistry-0.9.7/src/bioregistry/app/templates/collections.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/app/templates/context.html` & `bioregistry-0.9.7/src/bioregistry/app/templates/context.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/app/templates/contexts.html` & `bioregistry-0.9.7/src/bioregistry/app/templates/contexts.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/app/templates/contributor.html` & `bioregistry-0.9.7/src/bioregistry/app/templates/contributor.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/app/templates/contributors.html` & `bioregistry-0.9.7/src/bioregistry/app/templates/contributors.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/app/templates/highlights/keywords.html` & `bioregistry-0.9.7/src/bioregistry/app/templates/highlights/keywords.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/app/templates/highlights/owners.html` & `bioregistry-0.9.7/src/bioregistry/app/templates/highlights/owners.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/app/templates/highlights/relations.html` & `bioregistry-0.9.7/src/bioregistry/app/templates/highlights/relations.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/app/templates/highlights/twitter.html` & `bioregistry-0.9.7/src/bioregistry/app/templates/highlights/twitter.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/app/templates/home.html` & `bioregistry-0.9.7/src/bioregistry/app/templates/home.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/app/templates/macros.html` & `bioregistry-0.9.7/src/bioregistry/app/templates/macros.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/app/templates/meta/access.html` & `bioregistry-0.9.7/src/bioregistry/app/templates/meta/access.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/app/templates/meta/acknowledgements.html` & `bioregistry-0.9.7/src/bioregistry/app/templates/meta/acknowledgements.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/app/templates/meta/download.html` & `bioregistry-0.9.7/src/bioregistry/app/templates/meta/download.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/app/templates/meta/related.html` & `bioregistry-0.9.7/src/bioregistry/app/templates/meta/related.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/app/templates/meta/schema.html` & `bioregistry-0.9.7/src/bioregistry/app/templates/meta/schema.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/app/templates/meta/summary.html` & `bioregistry-0.9.7/src/bioregistry/app/templates/meta/summary.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/app/templates/meta/sustainability.html` & `bioregistry-0.9.7/src/bioregistry/app/templates/meta/sustainability.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/app/templates/metaresource.html` & `bioregistry-0.9.7/src/bioregistry/app/templates/metaresource.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/app/templates/metaresources.html` & `bioregistry-0.9.7/src/bioregistry/app/templates/metaresources.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/app/templates/prose.html` & `bioregistry-0.9.7/src/bioregistry/app/templates/prose.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/app/templates/reference.html` & `bioregistry-0.9.7/src/bioregistry/app/templates/reference.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/app/templates/resolve_errors/disallowed_identifier.html` & `bioregistry-0.9.7/src/bioregistry/app/templates/resolve_errors/disallowed_identifier.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/app/templates/resolve_errors/invalid_identifier.html` & `bioregistry-0.9.7/src/bioregistry/app/templates/resolve_errors/invalid_identifier.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/app/templates/resolve_errors/missing_prefix.html` & `bioregistry-0.9.7/src/bioregistry/app/templates/resolve_errors/missing_prefix.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/app/templates/resolve_errors/missing_providers.html` & `bioregistry-0.9.7/src/bioregistry/app/templates/resolve_errors/missing_providers.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/app/templates/resource.html` & `bioregistry-0.9.7/src/bioregistry/app/templates/resource.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/app/templates/resources.html` & `bioregistry-0.9.7/src/bioregistry/app/templates/resources.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/app/test.py` & `bioregistry-0.9.7/src/bioregistry/app/test.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/app/ui.py` & `bioregistry-0.9.7/src/bioregistry/app/ui.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/app/utils.py` & `bioregistry-0.9.7/src/bioregistry/app/utils.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/benchmarks/cli.py` & `bioregistry-0.9.7/src/bioregistry/benchmarks/cli.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/benchmarks/curie_parsing.py` & `bioregistry-0.9.7/src/bioregistry/benchmarks/curie_parsing.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/benchmarks/curie_validation.py` & `bioregistry-0.9.7/src/bioregistry/benchmarks/curie_validation.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/benchmarks/uri_parsing.py` & `bioregistry-0.9.7/src/bioregistry/benchmarks/uri_parsing.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/bibliometrics.py` & `bioregistry-0.9.7/src/bioregistry/bibliometrics.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/cli.py` & `bioregistry-0.9.7/src/bioregistry/cli.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/collection_api.py` & `bioregistry-0.9.7/src/bioregistry/collection_api.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/compare.py` & `bioregistry-0.9.7/src/bioregistry/compare.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/constants.py` & `bioregistry-0.9.7/src/bioregistry/constants.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/curation/add_co_providers.py` & `bioregistry-0.9.7/src/bioregistry/curation/add_co_providers.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/curation/add_descriptions_from_gs.py` & `bioregistry-0.9.7/src/bioregistry/curation/add_descriptions_from_gs.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/curation/add_examples.py` & `bioregistry-0.9.7/src/bioregistry/curation/add_examples.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/curation/add_examples_from_javert.py` & `bioregistry-0.9.7/src/bioregistry/curation/add_examples_from_javert.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/curation/add_examples_from_ols.py` & `bioregistry-0.9.7/src/bioregistry/curation/add_examples_from_ols.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/curation/add_ontology_regexes.py` & `bioregistry-0.9.7/src/bioregistry/curation/add_ontology_regexes.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/curation/bulk_import.py` & `bioregistry-0.9.7/src/bioregistry/curation/bulk_import.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/curation/clean_licenses.py` & `bioregistry-0.9.7/src/bioregistry/curation/clean_licenses.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/curation/clean_name_suffixes.py` & `bioregistry-0.9.7/src/bioregistry/curation/clean_name_suffixes.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/curation/clean_publications.py` & `bioregistry-0.9.7/src/bioregistry/curation/clean_publications.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/curation/cleanup_authors.py` & `bioregistry-0.9.7/src/bioregistry/curation/cleanup_authors.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/curation/deprecation_diff.py` & `bioregistry-0.9.7/src/bioregistry/curation/deprecation_diff.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/curation/enrich_publications.py` & `bioregistry-0.9.7/src/bioregistry/curation/enrich_publications.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/curation/import_pc_semiautomatic.py` & `bioregistry-0.9.7/src/bioregistry/curation/import_pc_semiautomatic.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/curation/make_description_curation_sheet.py` & `bioregistry-0.9.7/src/bioregistry/curation/make_description_curation_sheet.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/curation/map_bartoc_via_wikidata.py` & `bioregistry-0.9.7/src/bioregistry/curation/map_bartoc_via_wikidata.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/curation/map_re3data_via_fairsharing.py` & `bioregistry-0.9.7/src/bioregistry/curation/map_re3data_via_fairsharing.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/curation/rename_metaprefix.py` & `bioregistry-0.9.7/src/bioregistry/curation/rename_metaprefix.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/curation/review_pc.py` & `bioregistry-0.9.7/src/bioregistry/curation/review_pc.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/curation/suggest_author_curation.py` & `bioregistry-0.9.7/src/bioregistry/curation/suggest_author_curation.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/curation/suggest_uniprot_providers.py` & `bioregistry-0.9.7/src/bioregistry/curation/suggest_uniprot_providers.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/README.md` & `bioregistry-0.9.7/src/bioregistry/data/README.md`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/bioregistry.json` & `bioregistry-0.9.7/src/bioregistry/data/bioregistry.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999724517906337%*

 * *Differences: {"'wikipathways.vocab'": "{'description': 'An ontology supporting data modeling in WikiPathways', "*

 * *                         "'name': 'WikiPathways Ontology'}"}*

```diff
@@ -103260,23 +103260,23 @@
         },
         "contact": {
             "email": "egon.willighagen@gmail.com",
             "github": "egonw",
             "name": "Egon Willighagen",
             "orcid": "0000-0001-7542-0286"
         },
-        "description": "An ontology supporting data modeling in Wikipathways",
+        "description": "An ontology supporting data modeling in WikiPathways",
         "example": "DataNode",
         "homepage": "http://www.wikipathways.org",
         "mappings": {
             "aberowl": "WIKIPATHWAYS",
             "bioportal": "WIKIPATHWAYS"
         },
         "mastodon": "wikipathways@fosstodon.org",
-        "name": "Wikipathways Ontology",
+        "name": "WikiPathways Ontology",
         "references": [
             "https://github.com/biopragmatics/bioregistry/issues/818"
         ],
         "uri_format": "https://bioportal.bioontology.org/ontologies/WIKIPATHWAYS/?p=classes&conceptid=http%3A%2F%2Fvocabularies.wikipathways.org%2Fwp%23$1"
     },
     "wikipedia.en": {
         "biocontext": {
```

### Comparing `bioregistry-0.9.6/src/bioregistry/data/collections.json` & `bioregistry-0.9.7/src/bioregistry/data/collections.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/contexts.json` & `bioregistry-0.9.7/src/bioregistry/data/contexts.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/aberowl/curation.tsv` & `bioregistry-0.9.7/src/bioregistry/data/external/aberowl/curation.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/aberowl/processed.json` & `bioregistry-0.9.7/src/bioregistry/data/external/aberowl/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/aberowl/raw.json` & `bioregistry-0.9.7/src/bioregistry/data/external/aberowl/raw.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/agroportal/curation.tsv` & `bioregistry-0.9.7/src/bioregistry/data/external/agroportal/curation.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/agroportal/processed.json` & `bioregistry-0.9.7/src/bioregistry/data/external/agroportal/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/agroportal/raw.json` & `bioregistry-0.9.7/src/bioregistry/data/external/agroportal/raw.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/bartoc/curation.tsv` & `bioregistry-0.9.7/src/bioregistry/data/external/bartoc/curation.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/bartoc/processed.json` & `bioregistry-0.9.7/src/bioregistry/data/external/bartoc/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/biocontext/curation.tsv` & `bioregistry-0.9.7/src/bioregistry/data/external/biocontext/curation.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/biocontext/processed.json` & `bioregistry-0.9.7/src/bioregistry/data/external/biocontext/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/biocontext/raw.json` & `bioregistry-0.9.7/src/bioregistry/data/external/biocontext/raw.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/biolink/curation.tsv` & `bioregistry-0.9.7/src/bioregistry/data/external/biolink/curation.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/biolink/processed.json` & `bioregistry-0.9.7/src/bioregistry/data/external/biolink/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/biolink/raw.yaml` & `bioregistry-0.9.7/src/bioregistry/data/external/biolink/raw.yaml`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/bioportal/curation.tsv` & `bioregistry-0.9.7/src/bioregistry/data/external/bioportal/curation.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/bioportal/processed.json` & `bioregistry-0.9.7/src/bioregistry/data/external/bioportal/processed.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999177406087196%*

 * *Differences: {"'BAO'": "{'version': '2.8.1'}", "'MS'": "{'version': '4.1.120'}"}*

```diff
@@ -565,15 +565,15 @@
             "name": "Stephan Schurer"
         },
         "description": "The BioAssay Ontology (BAO) describes chemical biology screening assays and their results including high-throughput screening (HTS) data for the purpose of categorizing assays and data analysis. BAO is an extensible, knowledge-based, highly expressive (currently SHOIQ(D)) description of biological assays making use of descriptive logic based features of the Web Ontology Language (OWL). BAO currently has over 1000 classes and also makes use of several other ontologies. It describes several concepts related to biological screening, including Perturbagen, Format, Meta Target, Design, Detection Technology, and Endpoint. Perturbagens are perturbing agents that are screened in an assay; they are mostly small molecules. Assay Meta Target describes what is known about the biological system and / or its components interrogated in the assay (and influenced by the Perturbagen). Meta target can be directly described as a molecular entity (e.g. a purified protein or a protein complex), or indirectly by a biological process or event (e.g. phosphorylation). Format describes the biological or chemical features common to each test condition in the assay and includes biochemical, cell-based, organism-based, and variations thereof. The assay Design describes the assay methodology and implementation of how the perturbation of the biological system is translated into a detectable signal. Detection Technology relates to the physical method and technical details to detect and record a signal. Endpoints are the final HTS results as they are usually published (such as IC50, percent inhibition, etc.). BAO has been designed to accommodate multiplexed assays. All main BAO components include multiple levels of sub-categories and specification classes, which are linked via object property relationships forming an expressive knowledge-based representation.",
         "homepage": "http://www.bioassayontology.org/",
         "name": "BioAssay Ontology",
         "prefix": "BAO",
         "publication": "http://www.bioassayontology.org/",
-        "version": "2.8"
+        "version": "2.8.1"
     },
     "BAO-GPCR": {
         "contact": {
             "email": "sschurer@med.miami.edu",
             "name": "Stephan Schurer"
         },
         "description": "The G protein-coupled receptors (GPCRs) ontology (http://www.bioassayontology.org/bao_gpcr) describes pharmacology, biochemistry and physiology of these important and therapeutically promising class of academic and pharmaceutical research targets. Incorporation and comparison of various small molecule screening data sets, such as those deposited in PubChem, ChEMBL, KEGG, PDSP, and/or IUPHAR databases, requires a formalized electronic organization system. In order to bridge the gap between the overflow of HTS data and the bottleneck of integrated analysis tools, herein, we provide the first comprehensive GPCR ontology. The development and utility of GPCR ontology was based on previously developed BioAssay Ontology (BAO). The GPCR ontology contains information about biochemical, pharmacological, and functional properties of individual GPCRs as well as GPCR-selective ligands inclusive of their HTS screening results and other records. This provides the first all-inclusive GPCR ontology with all available data to model the relationship between the GPCR binding sites and their physiologic and pharmacologic role in physiology via small molecule chemical structures. We developed this system using emerging semantic technologies, by leveraging existing and descriptive domain level ontologies.",
@@ -6428,15 +6428,15 @@
         "prefix": "MRO"
     },
     "MS": {
         "homepage": "http://www.psidev.info/groups/controlled-vocabularies",
         "name": "Mass Spectrometry Ontology",
         "prefix": "MS",
         "publication": "http://database.oxfordjournals.org/content/2013/bat009.long",
-        "version": "4.1.119"
+        "version": "4.1.120"
     },
     "MSO": {
         "contact": {
             "email": "ashutosh.malhotra@scai.fraunhofer.de",
             "name": "Ashutosh Malhotra"
         },
         "description": "Multiple sclerosis ontology integrated with Basic formal ontology.",
```

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/bioportal/raw.json` & `bioregistry-0.9.7/src/bioregistry/data/external/bioportal/raw.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999120281509917%*

 * *Differences: {'657': "{'version': '4.1.120'}", '916': "{'version': '2.8.1'}"}*

```diff
@@ -36009,15 +36009,15 @@
             "submissions": "https://data.bioontology.org/ontologies/MS/submissions",
             "ui": "http://bioportal.bioontology.org/ontologies/MS",
             "views": "https://data.bioontology.org/ontologies/MS/views"
         },
         "name": "Mass Spectrometry Ontology",
         "ontologyType": "https://data.bioontology.org/ontology_types/ONTOLOGY",
         "publication": "http://database.oxfordjournals.org/content/2013/bat009.long",
-        "version": "4.1.119"
+        "version": "4.1.120"
     },
     {
         "@id": "https://data.bioontology.org/ontologies/OPTION-ONTOLOGY",
         "@type": "http://data.bioontology.org/metadata/Ontology",
         "acronym": "OPTION-ONTOLOGY",
         "administeredBy": [
             "https://data.bioontology.org/users/anakk"
@@ -50190,15 +50190,15 @@
             "submissions": "https://data.bioontology.org/ontologies/BAO/submissions",
             "ui": "http://bioportal.bioontology.org/ontologies/BAO",
             "views": "https://data.bioontology.org/ontologies/BAO/views"
         },
         "name": "BioAssay Ontology",
         "ontologyType": "https://data.bioontology.org/ontology_types/ONTOLOGY",
         "publication": "http://www.bioassayontology.org/",
-        "version": "2.8"
+        "version": "2.8.1"
     },
     {
         "@id": "https://data.bioontology.org/ontologies/MA",
         "@type": "http://data.bioontology.org/metadata/Ontology",
         "acronym": "MA",
         "administeredBy": [
             "https://data.bioontology.org/users/anatomy%40informatics.jax.org"
```

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/cellosaurus/curation.tsv` & `bioregistry-0.9.7/src/bioregistry/data/external/cellosaurus/curation.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/cellosaurus/processed.json` & `bioregistry-0.9.7/src/bioregistry/data/external/cellosaurus/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/cellosaurus/raw.txt` & `bioregistry-0.9.7/src/bioregistry/data/external/cellosaurus/raw.txt`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/cheminf/processed.json` & `bioregistry-0.9.7/src/bioregistry/data/external/cheminf/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/cropoct/processed.json` & `bioregistry-0.9.7/src/bioregistry/data/external/cropoct/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/cropoct/raw.yaml` & `bioregistry-0.9.7/src/bioregistry/data/external/cropoct/raw.yaml`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/ecoportal/curation.tsv` & `bioregistry-0.9.7/src/bioregistry/data/external/ecoportal/curation.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/ecoportal/processed.json` & `bioregistry-0.9.7/src/bioregistry/data/external/ecoportal/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/ecoportal/raw.json` & `bioregistry-0.9.7/src/bioregistry/data/external/ecoportal/raw.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/edam/curation.tsv` & `bioregistry-0.9.7/src/bioregistry/data/external/edam/curation.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/edam/processed.json` & `bioregistry-0.9.7/src/bioregistry/data/external/edam/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/fairsharing/curation.tsv` & `bioregistry-0.9.7/src/bioregistry/data/external/fairsharing/curation.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/fairsharing/processed.json` & `bioregistry-0.9.7/src/bioregistry/data/external/fairsharing/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/go/curation.tsv` & `bioregistry-0.9.7/src/bioregistry/data/external/go/curation.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/go/processed.json` & `bioregistry-0.9.7/src/bioregistry/data/external/go/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/go/raw.yml` & `bioregistry-0.9.7/src/bioregistry/data/external/go/raw.yml`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/hl7/curation.tsv` & `bioregistry-0.9.7/src/bioregistry/data/external/hl7/curation.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/miriam/processed.json` & `bioregistry-0.9.7/src/bioregistry/data/external/miriam/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/miriam/raw.json` & `bioregistry-0.9.7/src/bioregistry/data/external/miriam/raw.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/n2t/processed.json` & `bioregistry-0.9.7/src/bioregistry/data/external/n2t/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/n2t/raw.yml` & `bioregistry-0.9.7/src/bioregistry/data/external/n2t/raw.yml`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/ncbi/curation.tsv` & `bioregistry-0.9.7/src/bioregistry/data/external/ncbi/curation.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/ncbi/processed.json` & `bioregistry-0.9.7/src/bioregistry/data/external/ncbi/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/ncbi/raw.html` & `bioregistry-0.9.7/src/bioregistry/data/external/ncbi/raw.html`

 * *Files 0% similar despite different names*

#### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/ncbi/raw.html` & `bioregistry-0.9.7/src/bioregistry/data/external/ncbi/raw.html`

```diff
@@ -30,15 +30,15 @@
     <meta name="modified" content="2021-10-25T17:46:25Z"/>
     <meta xmlns:ncbi-portal="http://ncbi.gov/portal/XSLT/namespace" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" name="cms-edit-aux-url" content="http://cms.ncbi.nlm.nih.gov/node//edit"/>
     <!-- Page headcontent end -->
     <!-- PageFixtures resources begin -->
     <link xmlns="http://www.w3.org/1999/xhtml" type="text/css" rel="stylesheet" href="//static.pubmed.gov/portal/portal3rc.fcgi/4208398/css/4207974/4206132.css" xml:base="http://127.0.0.1/sites/static/header_footer"/>
     <!-- PageFixtures resources end -->
     <link rel="shortcut icon" href="//www.ncbi.nlm.nih.gov/favicon.ico"/>
-    <meta name="ncbi_phid" content="CE8C0E9345579FD100000000055403AF.m_6"/>
+    <meta name="ncbi_phid" content="CE884B84456D0B610000000004F8035B.m_6"/>
     <meta name="referrer" content="origin-when-cross-origin"/>
     <link type="text/css" rel="stylesheet" href="//static.pubmed.gov/portal/portal3rc.fcgi/4181609/css/4121862/3974050/3917732/251717/4108189/14534/45193/3534283/4128070/3407145/4005757/4062871.css"/>
     <link type="text/css" rel="stylesheet" href="//static.pubmed.gov/portal/portal3rc.fcgi/4181609/css/3529741/3529739.css" media="print"/>
   </head>
   <body class=" col2  custom-page">
     <div class="grid">
       <div class="col twelve_col nomargin shadow">
@@ -3248,17 +3248,17 @@
             <div id="NCBIFooter_dynamic">
               <div class="breadcrumbs">
                 You are here:
                 <span id="breadcrumb_text">
                   <a href="/guide/">NCBI</a>
                 </span>
               </div>
-              <a id="help-desk-link" class="help_desk" href="https://support.ncbi.nlm.nih.gov/ics/support/default.asp?Time=2023-05-05T20:58:43-04:00&amp;Snapshot=%2Fprojects%2Fstaticsites%2Fgenbank%2Fgenbank@2.20&amp;Host=portal105&amp;ncbi_phid=CE8C0E9345579FD100000000055403AF&amp;ncbi_session=CE8C0E93455A6421_1364SID&amp;from=https%3A%2F%2Fwww.ncbi.nlm.nih.gov%2Fgenbank%2Fcollab%2Fdb_xref%2F&amp;Ncbi_App=genbank&amp;Page=custom-page&amp;style=classic&amp;deptID=28049" target="_blank">Support Center</a>
+              <a id="help-desk-link" class="help_desk" href="https://support.ncbi.nlm.nih.gov/ics/support/default.asp?Time=2023-05-06T21:04:42-04:00&amp;Snapshot=%2Fprojects%2Fstaticsites%2Fgenbank%2Fgenbank@2.20&amp;Host=portal101&amp;ncbi_phid=CE884B84456D0B610000000004F8035B&amp;ncbi_session=CE884B84456F92A1_1272SID&amp;from=https%3A%2F%2Fwww.ncbi.nlm.nih.gov%2Fgenbank%2Fcollab%2Fdb_xref%2F&amp;Ncbi_App=genbank&amp;Page=custom-page&amp;style=classic&amp;deptID=28049" target="_blank">Support Center</a>
               <noscript>
-                <img alt="" src="/stat?jsdisabled=true&amp;ncbi_app=genbank&amp;ncbi_db=&amp;ncbi_pdid=custom-page&amp;ncbi_phid=CE8C0E9345579FD100000000055403AF"/>
+                <img alt="" src="/stat?jsdisabled=true&amp;ncbi_app=genbank&amp;ncbi_db=&amp;ncbi_pdid=custom-page&amp;ncbi_phid=CE884B84456D0B610000000004F8035B"/>
               </noscript>
             </div>
             <div xmlns:xi="http://www.w3.org/2001/XInclude">
               <div xmlns="http://www.w3.org/1999/xhtml" class="footer" id="footer" xml:base="http://127.0.0.1/sites/static/header_footer">
                 <section class="icon-section">
                   <div id="icon-section-header" class="icon-section_header">Follow NCBI</div>
                   <div class="grid-container container">
@@ -3465,12 +3465,12 @@
         <span class="PAFAppResources"/>
       </div>
       <!-- /.twelve_col -->
     </div>
     <!-- /.grid -->
     <!-- usually for JS scripts at page bottom -->
     <span class="pagefixtures"/>
-    <!-- CE8C0E93455A6421_1364SID /projects/staticsites/genbank/genbank@2.20 portal105 v4.1.r643667 Fri, Jan 14 2022 01:18:35 -->
-    <span id="portal-csrf-token" style="display:none" data-token="CE8C0E93455A6421_1364SID"/>
+    <!-- CE884B84456F92A1_1272SID /projects/staticsites/genbank/genbank@2.20 portal101 v4.1.r643667 Fri, Jan 14 2022 01:18:35 -->
+    <span id="portal-csrf-token" style="display:none" data-token="CE884B84456F92A1_1272SID"/>
     <script type="text/javascript" src="//static.pubmed.gov/portal/portal3rc.fcgi/4181609/js/3879255/4121861/1490097/4087685.js" snapshot="genbank"/>
   </body>
 </html>
```

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/obofoundry/processed.json` & `bioregistry-0.9.7/src/bioregistry/data/external/obofoundry/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/obofoundry/raw.yaml` & `bioregistry-0.9.7/src/bioregistry/data/external/obofoundry/raw.yaml`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/ols/processed.json` & `bioregistry-0.9.7/src/bioregistry/data/external/ols/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/ols/raw.json` & `bioregistry-0.9.7/src/bioregistry/data/external/ols/raw.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/ontobee/curation.tsv` & `bioregistry-0.9.7/src/bioregistry/data/external/ontobee/curation.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/ontobee/processed.json` & `bioregistry-0.9.7/src/bioregistry/data/external/ontobee/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/ontobee/raw.html` & `bioregistry-0.9.7/src/bioregistry/data/external/ontobee/raw.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/prefixcommons/curation.tsv` & `bioregistry-0.9.7/src/bioregistry/data/external/prefixcommons/curation.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/prefixcommons/processed.json` & `bioregistry-0.9.7/src/bioregistry/data/external/prefixcommons/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/prefixcommons/raw.tsv` & `bioregistry-0.9.7/src/bioregistry/data/external/prefixcommons/raw.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/re3data/curation.tsv` & `bioregistry-0.9.7/src/bioregistry/data/external/re3data/curation.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/re3data/processed.json` & `bioregistry-0.9.7/src/bioregistry/data/external/re3data/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/uniprot/curation.tsv` & `bioregistry-0.9.7/src/bioregistry/data/external/uniprot/curation.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/uniprot/processed.json` & `bioregistry-0.9.7/src/bioregistry/data/external/uniprot/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/uniprot/raw.json` & `bioregistry-0.9.7/src/bioregistry/data/external/uniprot/raw.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/wikidata/curation.tsv` & `bioregistry-0.9.7/src/bioregistry/data/external/wikidata/curation.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/external/wikidata/processed.json` & `bioregistry-0.9.7/src/bioregistry/data/external/wikidata/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/metaregistry.json` & `bioregistry-0.9.7/src/bioregistry/data/metaregistry.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/mismatch.json` & `bioregistry-0.9.7/src/bioregistry/data/mismatch.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/data/processing_ols.json` & `bioregistry-0.9.7/src/bioregistry/data/processing_ols.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/export/cli.py` & `bioregistry-0.9.7/src/bioregistry/export/cli.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/export/prefix_maps.py` & `bioregistry-0.9.7/src/bioregistry/export/prefix_maps.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/export/rdf_export.py` & `bioregistry-0.9.7/src/bioregistry/export/rdf_export.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/export/sssom_export.py` & `bioregistry-0.9.7/src/bioregistry/export/sssom_export.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/export/tables_export.py` & `bioregistry-0.9.7/src/bioregistry/export/tables_export.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/export/tsv_export.py` & `bioregistry-0.9.7/src/bioregistry/export/tsv_export.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/export/warnings_export.py` & `bioregistry-0.9.7/src/bioregistry/export/warnings_export.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/export/yaml_export.py` & `bioregistry-0.9.7/src/bioregistry/export/yaml_export.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/external/__init__.py` & `bioregistry-0.9.7/src/bioregistry/external/__init__.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/external/aberowl.py` & `bioregistry-0.9.7/src/bioregistry/external/aberowl.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/external/bartoc.py` & `bioregistry-0.9.7/src/bioregistry/external/bartoc.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/external/biocontext.py` & `bioregistry-0.9.7/src/bioregistry/external/biocontext.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/external/biolink.py` & `bioregistry-0.9.7/src/bioregistry/external/biolink.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/external/bioportal.py` & `bioregistry-0.9.7/src/bioregistry/external/bioportal.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/external/cellosaurus.py` & `bioregistry-0.9.7/src/bioregistry/external/cellosaurus.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/external/cheminf.py` & `bioregistry-0.9.7/src/bioregistry/external/cheminf.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/external/cropoct.py` & `bioregistry-0.9.7/src/bioregistry/external/cropoct.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/external/edam.py` & `bioregistry-0.9.7/src/bioregistry/external/edam.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/external/fairsharing.py` & `bioregistry-0.9.7/src/bioregistry/external/fairsharing.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/external/go.py` & `bioregistry-0.9.7/src/bioregistry/external/go.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/external/hl7/OID_Report.csv` & `bioregistry-0.9.7/src/bioregistry/external/hl7/OID_Report.csv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/external/hl7/__init__.py` & `bioregistry-0.9.7/src/bioregistry/external/hl7/__init__.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/external/miriam.py` & `bioregistry-0.9.7/src/bioregistry/external/miriam.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/external/n2t.py` & `bioregistry-0.9.7/src/bioregistry/external/n2t.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/external/ncbi.py` & `bioregistry-0.9.7/src/bioregistry/external/ncbi.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/external/obofoundry.py` & `bioregistry-0.9.7/src/bioregistry/external/obofoundry.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/external/ols.py` & `bioregistry-0.9.7/src/bioregistry/external/ols.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/external/ontobee.py` & `bioregistry-0.9.7/src/bioregistry/external/ontobee.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/external/prefixcommons.py` & `bioregistry-0.9.7/src/bioregistry/external/prefixcommons.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/external/re3data.py` & `bioregistry-0.9.7/src/bioregistry/external/re3data.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/external/uniprot.py` & `bioregistry-0.9.7/src/bioregistry/external/uniprot.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/external/wikidata.py` & `bioregistry-0.9.7/src/bioregistry/external/wikidata.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/gh/github_client.py` & `bioregistry-0.9.7/src/bioregistry/gh/github_client.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/gh/new_prefix.py` & `bioregistry-0.9.7/src/bioregistry/gh/new_prefix.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/health/check_homepages.py` & `bioregistry-0.9.7/src/bioregistry/health/check_homepages.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/health/check_providers.py` & `bioregistry-0.9.7/src/bioregistry/health/check_providers.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/health/cli.py` & `bioregistry-0.9.7/src/bioregistry/health/cli.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/license_standardizer.py` & `bioregistry-0.9.7/src/bioregistry/license_standardizer.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/lint.py` & `bioregistry-0.9.7/src/bioregistry/lint.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/metaresource_api.py` & `bioregistry-0.9.7/src/bioregistry/metaresource_api.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/pandas.py` & `bioregistry-0.9.7/src/bioregistry/pandas.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/parse_iri.py` & `bioregistry-0.9.7/src/bioregistry/parse_iri.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/record_accumulator.py` & `bioregistry-0.9.7/src/bioregistry/record_accumulator.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/resolve.py` & `bioregistry-0.9.7/src/bioregistry/resolve.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/resolve_identifier.py` & `bioregistry-0.9.7/src/bioregistry/resolve_identifier.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/resource_manager.py` & `bioregistry-0.9.7/src/bioregistry/resource_manager.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/schema/constants.py` & `bioregistry-0.9.7/src/bioregistry/schema/constants.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/schema/schema.json` & `bioregistry-0.9.7/src/bioregistry/schema/schema.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/schema/struct.py` & `bioregistry-0.9.7/src/bioregistry/schema/struct.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/schema/utils.py` & `bioregistry-0.9.7/src/bioregistry/schema/utils.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/schema_utils.py` & `bioregistry-0.9.7/src/bioregistry/schema_utils.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/summary.py` & `bioregistry-0.9.7/src/bioregistry/summary.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/upload_ndex.py` & `bioregistry-0.9.7/src/bioregistry/upload_ndex.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/uri_format.py` & `bioregistry-0.9.7/src/bioregistry/uri_format.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/utils.py` & `bioregistry-0.9.7/src/bioregistry/utils.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry/version.py` & `bioregistry-0.9.7/src/bioregistry/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 __all__ = [
     "VERSION",
     "get_version",
     "get_git_hash",
 ]
 
-VERSION = "0.9.6"
+VERSION = "0.9.7"
 
 
 def get_git_hash() -> Optional[str]:
     """Get the bioregistry git hash."""
     with open(os.devnull, "w") as devnull:
         try:
             ret = check_output(  # noqa: S603,S607
```

### Comparing `bioregistry-0.9.6/src/bioregistry.egg-info/PKG-INFO` & `bioregistry-0.9.7/src/bioregistry.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioregistry
-Version: 0.9.6
+Version: 0.9.7
 Summary: Integrated registry of biological databases and nomenclatures
 Home-page: https://github.com/biopragmatics/bioregistry
 Download-URL: https://github.com/biopragmatics/bioregistry/releases
 Author: Charles Tapley Hoyt
 Author-email: cthoyt@gmail.com
 Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bioregistry Version: 0.9.6 Summary: Integrated
+Metadata-Version: 2.1 Name: bioregistry Version: 0.9.7 Summary: Integrated
 registry of biological databases and nomenclatures Home-page: https://
 github.com/biopragmatics/bioregistry Download-URL: https://github.com/
 biopragmatics/bioregistry/releases Author: Charles Tapley Hoyt Author-email:
 cthoyt@gmail.com Maintainer: Charles Tapley Hoyt Maintainer-email:
 cthoyt@gmail.com License: MIT Project-URL: Bug Tracker, https://github.com/
 biopragmatics/bioregistry/issues Keywords: databases,biological
 databases,biomedical databases Classifier: Development Status :: 4 - Beta
```

### Comparing `bioregistry-0.9.6/src/bioregistry.egg-info/SOURCES.txt` & `bioregistry-0.9.7/src/bioregistry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/src/bioregistry.egg-info/requires.txt` & `bioregistry-0.9.7/src/bioregistry.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/tests/test_api.py` & `bioregistry-0.9.7/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/tests/test_collections.py` & `bioregistry-0.9.7/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/tests/test_contexts.py` & `bioregistry-0.9.7/tests/test_contexts.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/tests/test_data.py` & `bioregistry-0.9.7/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/tests/test_duplicates.py` & `bioregistry-0.9.7/tests/test_duplicates.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/tests/test_identifiers_org.py` & `bioregistry-0.9.7/tests/test_identifiers_org.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/tests/test_indra.py` & `bioregistry-0.9.7/tests/test_indra.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/tests/test_manager.py` & `bioregistry-0.9.7/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/tests/test_metaregistry.py` & `bioregistry-0.9.7/tests/test_metaregistry.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/tests/test_ols.py` & `bioregistry-0.9.7/tests/test_ols.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/tests/test_pandas.py` & `bioregistry-0.9.7/tests/test_pandas.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/tests/test_resolve.py` & `bioregistry-0.9.7/tests/test_resolve.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/tests/test_sparql.py` & `bioregistry-0.9.7/tests/test_sparql.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/tests/test_usages.py` & `bioregistry-0.9.7/tests/test_usages.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/tests/test_utils.py` & `bioregistry-0.9.7/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/tests/test_web/test_api.py` & `bioregistry-0.9.7/tests/test_web/test_api.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.6/tests/test_web/test_ui.py` & `bioregistry-0.9.7/tests/test_web/test_ui.py`

 * *Files identical despite different names*

