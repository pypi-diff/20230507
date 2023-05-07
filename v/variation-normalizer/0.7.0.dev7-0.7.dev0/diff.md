# Comparing `tmp/variation-normalizer-0.7.0.dev7.tar.gz` & `tmp/variation-normalizer-0.7.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "variation-normalizer-0.7.0.dev7.tar", last modified: Tue May  2 11:48:55 2023, max compression
+gzip compressed data, was "variation-normalizer-0.7.dev0.tar", last modified: Mon Oct  3 15:18:18 2022, max compression
```

## Comparing `variation-normalizer-0.7.0.dev7.tar` & `variation-normalizer-0.7.dev0.tar`

### file list

```diff
@@ -1,259 +1,270 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:48:55.978095 variation-normalizer-0.7.0.dev7/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7720 2023-05-02 11:48:55.978095 variation-normalizer-0.7.0.dev7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-02 11:48:55.978095 variation-normalizer-0.7.0.dev7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:48:55.958094 variation-normalizer-0.7.0.dev7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:48:55.958094 variation-normalizer-0.7.0.dev7/tests/classifiers/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/classifiers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/classifiers/classifier_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/classifiers/test_amplification.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/classifiers/test_coding_dna_deletion.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/classifiers/test_coding_dna_delins.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/classifiers/test_coding_dna_insertion.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/classifiers/test_coding_dna_silent_mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/classifiers/test_coding_dna_substitution.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/classifiers/test_genomic_deletion.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/classifiers/test_genomic_deletion_range.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/classifiers/test_genomic_delins.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/classifiers/test_genomic_duplication.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/classifiers/test_genomic_insertion.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/classifiers/test_genomic_silent_mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/classifiers/test_genomic_substitution.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/classifiers/test_genomic_uncertain_deletion.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/classifiers/test_polypeptide_truncation.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/classifiers/test_protein_deletion.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/classifiers/test_protein_delins.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/classifiers/test_protein_insertion.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/classifiers/test_protein_substitution.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/classifiers/test_silent_mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)    38420 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/test_codon_table.py
--rw-r--r--   0 runner    (1001) docker     (123)    30125 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/test_gnomad_vcf_to_protein.py
--rw-r--r--   0 runner    (1001) docker     (123)   131096 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/test_hgvs_dup_del_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    54645 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/test_normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)    19317 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/test_to_canonical_variation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:48:55.962094 variation-normalizer-0.7.0.dev7/tests/tokenizers/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/tokenizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/tokenizers/test_amplification.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/tokenizers/test_coding_dna_deletion.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/tokenizers/test_coding_dna_delins.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/tokenizers/test_coding_dna_insertion.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/tokenizers/test_coding_dna_silent_mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/tokenizers/test_coding_dna_substitution.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/tokenizers/test_gene_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/tokenizers/test_genomic_deletion.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/tokenizers/test_genomic_deletion_range.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/tokenizers/test_genomic_delins.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/tokenizers/test_genomic_duplication.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/tokenizers/test_genomic_duplication_range.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/tokenizers/test_genomic_insertion.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/tokenizers/test_genomic_silent_mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/tokenizers/test_genomic_substitution.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/tokenizers/test_genomic_uncertain_deletion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/tokenizers/test_gnomad_vcf.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/tokenizers/test_hgvs.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/tokenizers/test_locus_reference_genomic.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/tokenizers/test_polypeptide_truncation.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/tokenizers/test_protein_deletion.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/tokenizers/test_protein_delins.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/tokenizers/test_protein_insertion.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/tokenizers/test_protein_substitution.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/tokenizers/test_silent_mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/tokenizers/tokenizer_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:48:55.962094 variation-normalizer-0.7.0.dev7/tests/translators/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/translators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/translators/test_coding_dna_deletion.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/translators/test_coding_dna_delins.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/translators/test_coding_dna_insertion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/translators/test_coding_dna_silent_mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/translators/test_coding_dna_substitution.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/translators/test_genomic_deletion.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/translators/test_genomic_delins.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/translators/test_genomic_duplication.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/translators/test_genomic_insertion.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/translators/test_genomic_silent_mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/translators/test_genomic_substitution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/translators/test_genomic_uncertain_deletion.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/translators/test_polypeptide_truncation.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/translators/test_protein_deletion.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/translators/test_protein_delins.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/translators/test_protein_insertion.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/translators/test_protein_substitution.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/translators/test_silent_mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/translators/translator_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:48:55.966094 variation-normalizer-0.7.0.dev7/tests/validators/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/validators/test_coding_dna_deletion.py
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/validators/test_coding_dna_delins.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/validators/test_coding_dna_insertion.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/validators/test_coding_dna_silent_mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/validators/test_coding_dna_subsitution.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/validators/test_genomic_deletion.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/validators/test_genomic_delins.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/validators/test_genomic_duplication.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/validators/test_genomic_insertion.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/validators/test_genomic_silent_mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/validators/test_genomic_substitution.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/validators/test_genomic_uncertain_deletion.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/validators/test_polypeptide_truncation.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/validators/test_protein_deletion.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/validators/test_protein_delins.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/validators/test_protein_insertion.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/validators/test_protein_substitution.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/validators/test_silent_mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/tests/validators/validator_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:48:55.966094 variation-normalizer-0.7.0.dev7/variation/
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:48:55.970095 variation-normalizer-0.7.0.dev7/variation/classifiers/
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/classifiers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/classifiers/amplification_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/classifiers/classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/classifiers/classify.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/classifiers/coding_dna_deletion_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/classifiers/coding_dna_delins_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/classifiers/coding_dna_insertion_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/classifiers/coding_dna_silent_mutation_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/classifiers/coding_dna_substitution_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/classifiers/genomic_deletion_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/classifiers/genomic_deletion_range_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/classifiers/genomic_delins_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/classifiers/genomic_duplication_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/classifiers/genomic_insertion_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/classifiers/genomic_silent_mutation_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/classifiers/genomic_substitution_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/classifiers/genomic_uncertain_deletion_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/classifiers/polypeptide_truncation_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/classifiers/protein_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/classifiers/protein_deletion_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/classifiers/protein_delins_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/classifiers/protein_insertion_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/classifiers/protein_termination_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/classifiers/set_based_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/classifiers/silent_mutation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:48:55.970095 variation-normalizer-0.7.0.dev7/variation/data_sources/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/data_sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/data_sources/codon_table.py
--rw-r--r--   0 runner    (1001) docker     (123)    18272 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/gnomad_vcf_to_protein_variation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10423 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/hgvs_dup_del_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    30257 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:48:55.970095 variation-normalizer-0.7.0.dev7/variation/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/schemas/app_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/schemas/classification_response_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/schemas/hgvs_to_copy_number_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    11444 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/schemas/normalize_response_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/schemas/service_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/schemas/to_vrs_response_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    17745 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/schemas/token_response_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/schemas/validation_response_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/schemas/vrs_python_translator_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    13123 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/to_canonical_variation.py
--rw-r--r--   0 runner    (1001) docker     (123)    18893 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/to_copy_number_variation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10294 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/to_vrs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/to_vrsatile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:48:55.974094 variation-normalizer-0.7.0.dev7/variation/tokenizers/
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/tokenizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/tokenizers/coding_dna_deletion.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/tokenizers/coding_dna_delins.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/tokenizers/coding_dna_insertion.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/tokenizers/coding_dna_silent_mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/tokenizers/coding_dna_substitution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/tokenizers/deletion_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/tokenizers/deletion_range_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/tokenizers/delins_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/tokenizers/duplication_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/tokenizers/free_text_categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/tokenizers/gene_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/tokenizers/genomic_deletion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/tokenizers/genomic_deletion_range.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/tokenizers/genomic_delins.py
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/tokenizers/genomic_duplication.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/tokenizers/genomic_insertion.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/tokenizers/genomic_silent_mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/tokenizers/genomic_substitution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/tokenizers/genomic_uncertain_deletion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/tokenizers/gnomad_vcf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/tokenizers/hgvs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/tokenizers/insertion_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/tokenizers/locus_reference_genomic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/tokenizers/polypeptide_sequence_variation_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/tokenizers/polypeptide_truncation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/tokenizers/protein_deletion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/tokenizers/protein_delins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/tokenizers/protein_insertion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/tokenizers/protein_substitution.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/tokenizers/reference_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/tokenizers/silent_mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/tokenizers/single_nucleotide_variation_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/tokenizers/tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/tokenizers/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:48:55.974094 variation-normalizer-0.7.0.dev7/variation/translators/
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/translators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/translators/amplification.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/translators/coding_dna_deletion.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/translators/coding_dna_delins.py
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/translators/coding_dna_insertion.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/translators/coding_dna_silent_mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/translators/coding_dna_substitution.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/translators/genomic_deletion.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/translators/genomic_deletion_range.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/translators/genomic_delins.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/translators/genomic_duplication.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/translators/genomic_insertion.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/translators/genomic_silent_mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/translators/genomic_substitution.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/translators/genomic_uncertain_deletion.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/translators/polypeptide_truncation.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/translators/protein_deletion.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/translators/protein_delins.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/translators/protein_insertion.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/translators/protein_substitution.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/translators/silent_mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/translators/translate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/translators/translator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6628 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:48:55.978095 variation-normalizer-0.7.0.dev7/variation/validators/
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/validators/amplification.py
--rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/validators/coding_dna_deletion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/validators/coding_dna_delins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/validators/coding_dna_insertion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/validators/coding_dna_silent_mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/validators/coding_dna_substitution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/validators/delins_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    14567 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/validators/duplication_deletion_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/validators/genomic_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/validators/genomic_deletion.py
--rw-r--r--   0 runner    (1001) docker     (123)    11546 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/validators/genomic_deletion_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/validators/genomic_delins.py
--rw-r--r--   0 runner    (1001) docker     (123)    15221 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/validators/genomic_duplication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/validators/genomic_insertion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/validators/genomic_silent_mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/validators/genomic_substitution.py
--rw-r--r--   0 runner    (1001) docker     (123)    11539 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/validators/genomic_uncertain_deletion.py
--rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/validators/insertion_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/validators/polypeptide_sequence_variation_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/validators/polypeptide_truncation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/validators/protein_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7762 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/validators/protein_deletion.py
--rw-r--r--   0 runner    (1001) docker     (123)     7148 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/validators/protein_delins.py
--rw-r--r--   0 runner    (1001) docker     (123)     7209 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/validators/protein_insertion.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/validators/protein_substitution.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/validators/silent_mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9749 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/validators/single_nucleotide_variation_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6634 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/validators/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)    30105 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/validators/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10814 2023-05-02 11:48:45.000000 variation-normalizer-0.7.0.dev7/variation/vrs_representation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:48:55.978095 variation-normalizer-0.7.0.dev7/variation_normalizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7720 2023-05-02 11:48:55.000000 variation-normalizer-0.7.0.dev7/variation_normalizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10359 2023-05-02 11:48:55.000000 variation-normalizer-0.7.0.dev7/variation_normalizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 11:48:55.000000 variation-normalizer-0.7.0.dev7/variation_normalizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 11:48:55.000000 variation-normalizer-0.7.0.dev7/variation_normalizer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-02 11:48:55.000000 variation-normalizer-0.7.0.dev7/variation_normalizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-02 11:48:55.000000 variation-normalizer-0.7.0.dev7/variation_normalizer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 15:18:18.250050 variation-normalizer-0.7.dev0/
+-rw-r--r--   0 runner    (1001) docker     (121)     1062 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     7389 2022-10-03 15:18:18.250050 variation-normalizer-0.7.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     6682 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1303 2022-10-03 15:18:18.250050 variation-normalizer-0.7.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      156 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 15:18:18.150050 variation-normalizer-0.7.dev0/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)       97 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 15:18:18.154050 variation-normalizer-0.7.dev0/tests/classifiers/
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/classifiers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1894 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/classifiers/classifier_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)      545 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/classifiers/test_amplification.py
+-rw-r--r--   0 runner    (1001) docker     (121)      587 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/classifiers/test_coding_dna_deletion.py
+-rw-r--r--   0 runner    (1001) docker     (121)      571 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/classifiers/test_coding_dna_delins.py
+-rw-r--r--   0 runner    (1001) docker     (121)      595 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/classifiers/test_coding_dna_insertion.py
+-rw-r--r--   0 runner    (1001) docker     (121)      638 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/classifiers/test_coding_dna_silent_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (121)      619 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/classifiers/test_coding_dna_substitution.py
+-rw-r--r--   0 runner    (1001) docker     (121)      568 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/classifiers/test_genomic_deletion.py
+-rw-r--r--   0 runner    (1001) docker     (121)      647 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/classifiers/test_genomic_deletion_range.py
+-rw-r--r--   0 runner    (1001) docker     (121)      552 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/classifiers/test_genomic_delins.py
+-rw-r--r--   0 runner    (1001) docker     (121)      592 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/classifiers/test_genomic_duplication.py
+-rw-r--r--   0 runner    (1001) docker     (121)      576 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/classifiers/test_genomic_insertion.py
+-rw-r--r--   0 runner    (1001) docker     (121)      619 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/classifiers/test_genomic_silent_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (121)      603 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/classifiers/test_genomic_substitution.py
+-rw-r--r--   0 runner    (1001) docker     (121)      683 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/classifiers/test_genomic_uncertain_deletion.py
+-rw-r--r--   0 runner    (1001) docker     (121)      616 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/classifiers/test_polypeptide_truncation.py
+-rw-r--r--   0 runner    (1001) docker     (121)      568 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/classifiers/test_protein_deletion.py
+-rw-r--r--   0 runner    (1001) docker     (121)      552 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/classifiers/test_protein_delins.py
+-rw-r--r--   0 runner    (1001) docker     (121)      576 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/classifiers/test_protein_insertion.py
+-rw-r--r--   0 runner    (1001) docker     (121)      600 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/classifiers/test_protein_substitution.py
+-rw-r--r--   0 runner    (1001) docker     (121)      560 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/classifiers/test_silent_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (121)    38453 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1358 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/test_codon_table.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30116 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/test_gnomad_vcf_to_protein.py
+-rw-r--r--   0 runner    (1001) docker     (121)   131374 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/test_hgvs_dup_del_mode.py
+-rw-r--r--   0 runner    (1001) docker     (121)    51679 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/test_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19337 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/test_to_canonical_variation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 15:18:18.158050 variation-normalizer-0.7.dev0/tests/tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (121)       30 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/tokenizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      721 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/tokenizers/test_amplification.py
+-rw-r--r--   0 runner    (1001) docker     (121)      781 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/tokenizers/test_coding_dna_deletion.py
+-rw-r--r--   0 runner    (1001) docker     (121)      761 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/tokenizers/test_coding_dna_delins.py
+-rw-r--r--   0 runner    (1001) docker     (121)      791 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/tokenizers/test_coding_dna_insertion.py
+-rw-r--r--   0 runner    (1001) docker     (121)      740 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/tokenizers/test_coding_dna_silent_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (121)      714 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/tokenizers/test_coding_dna_substitution.py
+-rw-r--r--   0 runner    (1001) docker     (121)      660 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/tokenizers/test_gene.py
+-rw-r--r--   0 runner    (1001) docker     (121)      566 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/tokenizers/test_gene_pair.py
+-rw-r--r--   0 runner    (1001) docker     (121)      758 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/tokenizers/test_genomic_deletion.py
+-rw-r--r--   0 runner    (1001) docker     (121)      705 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/tokenizers/test_genomic_deletion_range.py
+-rw-r--r--   0 runner    (1001) docker     (121)      735 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/tokenizers/test_genomic_delins.py
+-rw-r--r--   0 runner    (1001) docker     (121)      678 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/tokenizers/test_genomic_duplication.py
+-rw-r--r--   0 runner    (1001) docker     (121)      700 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/tokenizers/test_genomic_duplication_range.py
+-rw-r--r--   0 runner    (1001) docker     (121)      765 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/tokenizers/test_genomic_insertion.py
+-rw-r--r--   0 runner    (1001) docker     (121)      718 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/tokenizers/test_genomic_silent_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (121)      688 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/tokenizers/test_genomic_substitution.py
+-rw-r--r--   0 runner    (1001) docker     (121)      744 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/tokenizers/test_genomic_uncertain_deletion.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3999 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/tokenizers/test_gnomad_vcf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      528 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/tokenizers/test_hgvs.py
+-rw-r--r--   0 runner    (1001) docker     (121)      610 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/tokenizers/test_locus_reference_genomic.py
+-rw-r--r--   0 runner    (1001) docker     (121)      780 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/tokenizers/test_polypeptide_truncation.py
+-rw-r--r--   0 runner    (1001) docker     (121)      755 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/tokenizers/test_protein_deletion.py
+-rw-r--r--   0 runner    (1001) docker     (121)      735 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/tokenizers/test_protein_delins.py
+-rw-r--r--   0 runner    (1001) docker     (121)      765 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/tokenizers/test_protein_insertion.py
+-rw-r--r--   0 runner    (1001) docker     (121)      759 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/tokenizers/test_protein_substitution.py
+-rw-r--r--   0 runner    (1001) docker     (121)      709 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/tokenizers/test_silent_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1537 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/tokenizers/tokenizer_base.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 15:18:18.162050 variation-normalizer-0.7.dev0/tests/translators/
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/translators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      936 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/translators/test_coding_dna_deletion.py
+-rw-r--r--   0 runner    (1001) docker     (121)      922 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/translators/test_coding_dna_delins.py
+-rw-r--r--   0 runner    (1001) docker     (121)      948 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/translators/test_coding_dna_insertion.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1025 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/translators/test_coding_dna_silent_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (121)      994 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/translators/test_coding_dna_substitution.py
+-rw-r--r--   0 runner    (1001) docker     (121)      902 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/translators/test_genomic_deletion.py
+-rw-r--r--   0 runner    (1001) docker     (121)      895 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/translators/test_genomic_delins.py
+-rw-r--r--   0 runner    (1001) docker     (121)      938 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/translators/test_genomic_duplication.py
+-rw-r--r--   0 runner    (1001) docker     (121)      915 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/translators/test_genomic_insertion.py
+-rw-r--r--   0 runner    (1001) docker     (121)      998 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/translators/test_genomic_silent_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (121)      955 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/translators/test_genomic_substitution.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/translators/test_genomic_uncertain_deletion.py
+-rw-r--r--   0 runner    (1001) docker     (121)      980 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/translators/test_polypeptide_truncation.py
+-rw-r--r--   0 runner    (1001) docker     (121)      904 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/translators/test_protein_deletion.py
+-rw-r--r--   0 runner    (1001) docker     (121)      878 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/translators/test_protein_delins.py
+-rw-r--r--   0 runner    (1001) docker     (121)      917 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/translators/test_protein_insertion.py
+-rw-r--r--   0 runner    (1001) docker     (121)      960 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/translators/test_protein_substitution.py
+-rw-r--r--   0 runner    (1001) docker     (121)      889 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/translators/test_silent_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4123 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/translators/translator_base.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 15:18:18.166050 variation-normalizer-0.7.dev0/tests/validators/
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      770 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/validators/test_coding_dna_deletion.py
+-rw-r--r--   0 runner    (1001) docker     (121)      750 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/validators/test_coding_dna_delins.py
+-rw-r--r--   0 runner    (1001) docker     (121)      781 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/validators/test_coding_dna_insertion.py
+-rw-r--r--   0 runner    (1001) docker     (121)      844 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/validators/test_coding_dna_silent_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (121)      816 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/validators/test_coding_dna_subsitution.py
+-rw-r--r--   0 runner    (1001) docker     (121)      743 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/validators/test_genomic_deletion.py
+-rw-r--r--   0 runner    (1001) docker     (121)      721 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/validators/test_genomic_delins.py
+-rw-r--r--   0 runner    (1001) docker     (121)      777 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/validators/test_genomic_duplication.py
+-rw-r--r--   0 runner    (1001) docker     (121)      754 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/validators/test_genomic_insertion.py
+-rw-r--r--   0 runner    (1001) docker     (121)      816 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/validators/test_genomic_silent_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (121)      788 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/validators/test_genomic_substitution.py
+-rw-r--r--   0 runner    (1001) docker     (121)      849 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/validators/test_genomic_uncertain_deletion.py
+-rw-r--r--   0 runner    (1001) docker     (121)      813 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/validators/test_polypeptide_truncation.py
+-rw-r--r--   0 runner    (1001) docker     (121)      747 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/validators/test_protein_deletion.py
+-rw-r--r--   0 runner    (1001) docker     (121)      725 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/validators/test_protein_delins.py
+-rw-r--r--   0 runner    (1001) docker     (121)      758 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/validators/test_protein_insertion.py
+-rw-r--r--   0 runner    (1001) docker     (121)      798 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/validators/test_protein_substitution.py
+-rw-r--r--   0 runner    (1001) docker     (121)      736 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/validators/test_silent_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3847 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/tests/validators/validator_base.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 15:18:18.166050 variation-normalizer-0.7.dev0/variation/
+-rw-r--r--   0 runner    (1001) docker     (121)     2484 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 15:18:18.170050 variation-normalizer-0.7.dev0/variation/classifiers/
+-rw-r--r--   0 runner    (1001) docker     (121)     1657 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/classifiers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      658 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/classifiers/amplification_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (121)      681 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/classifiers/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3042 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/classifiers/classify.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1008 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/classifiers/coding_dna_deletion_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (121)      984 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/classifiers/coding_dna_delins_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1020 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/classifiers/coding_dna_insertion_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1084 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/classifiers/coding_dna_silent_mutation_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1056 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/classifiers/coding_dna_substitution_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (121)      994 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/classifiers/genomic_deletion_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (121)      983 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/classifiers/genomic_deletion_range_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (121)      914 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/classifiers/genomic_delins_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1244 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/classifiers/genomic_duplication_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1006 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/classifiers/genomic_insertion_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1006 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/classifiers/genomic_silent_mutation_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (121)      980 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/classifiers/genomic_substitution_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1027 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/classifiers/genomic_uncertain_deletion_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (121)      859 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/classifiers/polypeptide_truncation_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (121)      840 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/classifiers/protein_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (121)      980 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/classifiers/protein_deletion_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (121)      956 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/classifiers/protein_delins_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (121)      992 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/classifiers/protein_insertion_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (121)      741 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/classifiers/protein_termination_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3574 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/classifiers/set_based_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (121)      796 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/classifiers/silent_mutation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 15:18:18.170050 variation-normalizer-0.7.dev0/variation/data/
+-rw-r--r--   0 runner    (1001) docker     (121)      315 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/data/amino_acids.csv
+-rw-r--r--   0 runner    (1001) docker     (121) 24138769 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/data/transcript_mapping.tsv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 15:18:18.210050 variation-normalizer-0.7.dev0/variation/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (121)       76 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/data_sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2673 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/data_sources/codon_table.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17902 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/gnomad_vcf_to_protein_variation.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10733 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/hgvs_dup_del_mode.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30406 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/main.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5101 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5289 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/query.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 15:18:18.214050 variation-normalizer-0.7.dev0/variation/schemas/
+-rw-r--r--   0 runner    (1001) docker     (121)      427 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      485 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/schemas/app_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2098 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/schemas/classification_response_schema.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4193 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/schemas/hgvs_to_copy_number_schema.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11422 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/schemas/normalize_response_schema.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5359 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/schemas/service_schema.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4868 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/schemas/to_vrs_response_schema.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19165 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/schemas/token_response_schema.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1197 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/schemas/validation_response_schema.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4401 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/schemas/vrs_python_translator_schema.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13308 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/to_canonical_variation.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19085 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/to_copy_number_variation.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10501 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/to_vrs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3488 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/to_vrsatile.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 15:18:18.226050 variation-normalizer-0.7.dev0/variation/tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (121)     1606 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/tokenizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 15:18:18.226050 variation-normalizer-0.7.dev0/variation/tokenizers/caches/
+-rw-r--r--   0 runner    (1001) docker     (121)      164 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/tokenizers/caches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1651 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/tokenizers/caches/amino_acid_cache.py
+-rw-r--r--   0 runner    (1001) docker     (121)      847 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/tokenizers/caches/nucleotide_cache.py
+-rw-r--r--   0 runner    (1001) docker     (121)      570 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/tokenizers/coding_dna_deletion.py
+-rw-r--r--   0 runner    (1001) docker     (121)      550 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/tokenizers/coding_dna_delins.py
+-rw-r--r--   0 runner    (1001) docker     (121)      580 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/tokenizers/coding_dna_insertion.py
+-rw-r--r--   0 runner    (1001) docker     (121)      768 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/tokenizers/coding_dna_silent_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (121)      759 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/tokenizers/coding_dna_substitution.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3246 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/tokenizers/deletion_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2149 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/tokenizers/deletion_range_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3770 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/tokenizers/delins_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1595 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/tokenizers/duplication_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)      957 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/tokenizers/free_text_categorical.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1286 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/tokenizers/gene_pair.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2166 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/tokenizers/gene_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (121)      553 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/tokenizers/genomic_deletion.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2312 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/tokenizers/genomic_deletion_range.py
+-rw-r--r--   0 runner    (1001) docker     (121)      549 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/tokenizers/genomic_delins.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5111 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/tokenizers/genomic_duplication.py
+-rw-r--r--   0 runner    (1001) docker     (121)      563 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/tokenizers/genomic_insertion.py
+-rw-r--r--   0 runner    (1001) docker     (121)      758 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/tokenizers/genomic_silent_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (121)      749 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/tokenizers/genomic_substitution.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3913 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/tokenizers/genomic_uncertain_deletion.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4674 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/tokenizers/gnomad_vcf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1837 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/tokenizers/hgvs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3285 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/tokenizers/insertion_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2545 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/tokenizers/locus_reference_genomic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1885 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/tokenizers/polypeptide_sequence_variation_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3664 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/tokenizers/polypeptide_truncation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1193 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/tokenizers/protein_alternate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2614 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/tokenizers/protein_deletion.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2743 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/tokenizers/protein_delins.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2791 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/tokenizers/protein_insertion.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2735 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/tokenizers/protein_substitution.py
+-rw-r--r--   0 runner    (1001) docker     (121)      915 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/tokenizers/reference_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2779 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/tokenizers/silent_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4538 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/tokenizers/single_nucleotide_variation_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5496 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/tokenizers/tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7630 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/tokenizers/tokenize_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)      380 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/tokenizers/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 15:18:18.234050 variation-normalizer-0.7.dev0/variation/translators/
+-rw-r--r--   0 runner    (1001) docker     (121)     1131 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/translators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      700 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/translators/amplification.py
+-rw-r--r--   0 runner    (1001) docker     (121)      742 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/translators/coding_dna_deletion.py
+-rw-r--r--   0 runner    (1001) docker     (121)      726 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/translators/coding_dna_delins.py
+-rw-r--r--   0 runner    (1001) docker     (121)      750 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/translators/coding_dna_insertion.py
+-rw-r--r--   0 runner    (1001) docker     (121)      812 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/translators/coding_dna_silent_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (121)      774 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/translators/coding_dna_substitution.py
+-rw-r--r--   0 runner    (1001) docker     (121)      721 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/translators/genomic_deletion.py
+-rw-r--r--   0 runner    (1001) docker     (121)      762 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/translators/genomic_deletion_range.py
+-rw-r--r--   0 runner    (1001) docker     (121)      705 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/translators/genomic_delins.py
+-rw-r--r--   0 runner    (1001) docker     (121)      843 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/translators/genomic_duplication.py
+-rw-r--r--   0 runner    (1001) docker     (121)      729 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/translators/genomic_insertion.py
+-rw-r--r--   0 runner    (1001) docker     (121)      791 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/translators/genomic_silent_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (121)      753 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/translators/genomic_substitution.py
+-rw-r--r--   0 runner    (1001) docker     (121)      820 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/translators/genomic_uncertain_deletion.py
+-rw-r--r--   0 runner    (1001) docker     (121)      769 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/translators/polypeptide_truncation.py
+-rw-r--r--   0 runner    (1001) docker     (121)      721 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/translators/protein_deletion.py
+-rw-r--r--   0 runner    (1001) docker     (121)      705 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/translators/protein_delins.py
+-rw-r--r--   0 runner    (1001) docker     (121)      729 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/translators/protein_insertion.py
+-rw-r--r--   0 runner    (1001) docker     (121)      753 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/translators/protein_substitution.py
+-rw-r--r--   0 runner    (1001) docker     (121)      713 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/translators/silent_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2407 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/translators/translate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1929 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/translators/translator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6624 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 15:18:18.246050 variation-normalizer-0.7.dev0/variation/validators/
+-rw-r--r--   0 runner    (1001) docker     (121)     1287 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5278 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/validators/amplification.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5848 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/validators/coding_dna_deletion.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5713 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/validators/coding_dna_delins.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2035 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/validators/coding_dna_insertion.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4281 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/validators/coding_dna_silent_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6017 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/validators/coding_dna_substitution.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4794 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/validators/delins_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14647 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/validators/duplication_deletion_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2486 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/validators/genomic_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8386 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/validators/genomic_deletion.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11704 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/validators/genomic_deletion_range.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5449 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/validators/genomic_delins.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15408 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/validators/genomic_duplication.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1991 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/validators/genomic_insertion.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4198 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/validators/genomic_silent_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5903 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/validators/genomic_substitution.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11701 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/validators/genomic_uncertain_deletion.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7626 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/validators/insertion_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6575 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/validators/polypeptide_sequence_variation_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)      971 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/validators/polypeptide_truncation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1411 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/validators/protein_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7445 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/validators/protein_deletion.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7435 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/validators/protein_delins.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7465 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/validators/protein_insertion.py
+-rw-r--r--   0 runner    (1001) docker     (121)      961 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/validators/protein_substitution.py
+-rw-r--r--   0 runner    (1001) docker     (121)      921 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/validators/silent_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9771 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/validators/single_nucleotide_variation_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7052 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/validators/validate.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30179 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/validators/validator.py
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/version.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11048 2022-10-03 15:18:09.000000 variation-normalizer-0.7.dev0/variation/vrs_representation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 15:18:18.250050 variation-normalizer-0.7.dev0/variation_normalizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     7389 2022-10-03 15:18:18.000000 variation-normalizer-0.7.dev0/variation_normalizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    10706 2022-10-03 15:18:18.000000 variation-normalizer-0.7.dev0/variation_normalizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-03 15:18:18.000000 variation-normalizer-0.7.dev0/variation_normalizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-03 15:18:18.000000 variation-normalizer-0.7.dev0/variation_normalizer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      212 2022-10-03 15:18:18.000000 variation-normalizer-0.7.dev0/variation_normalizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-10-03 15:18:18.000000 variation-normalizer-0.7.dev0/variation_normalizer.egg-info/top_level.txt
```

### Comparing `variation-normalizer-0.7.0.dev7/LICENSE` & `variation-normalizer-0.7.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/PKG-INFO` & `variation-normalizer-0.7.dev0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: variation-normalizer
-Version: 0.7.0.dev7
+Version: 0.7.dev0
 Summary: VICC normalization routine for variations
 Home-page: https://github.com/cancervariants/variation-normalization
 Author: VICC
 Author-email: help@cancervariants.org
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -48,15 +47,15 @@
 
 We are working towards adding more types of variations, coordinates, and representations.
 
 ### Endpoints
 
 The `/to_vrs` endpoint returns a list of validated VRS [Variations](https://vrs.ga4gh.org/en/1.2.0/terms_and_model.html#variation).
 
-The `/normalize` endpoint returns a [Variation Descriptor](https://vrsatile.readthedocs.io/en/latest/value_object_descriptor/vod_index.html#variation-descriptor) containing the MANE Transcript, if one is found. If a genomic query is not given a gene, `normalize` will return its GRCh38 representation. Variation Normalizer relies on [**C**ommon **O**perations **O**n **L**ots-of **Seq**uences Tool (cool-seq-tool)](https://github.com/GenomicMedLab/cool-seq-tool) for retrieving MANE Transcript data. More information on the transcript selection algorithm can be found [here](https://github.com/GenomicMedLab/cool-seq-tool/blob/main/docs/TranscriptSelectionPriority.md).
+The `/normalize` endpoint returns a [Variation Descriptor](https://vrsatile.readthedocs.io/en/latest/value_object_descriptor/vod_index.html#variation-descriptor) containing the MANE Transcript, if one is found. If a genomic query is not given a gene, `normalize` will return its GRCh38 representation. Variation Normalizer relies on [UTA Tools](https://github.com/GenomicMedLab/uta-tools) for retrieving MANE Transcript data. More information on the transcript selection algorithm can be found [here](https://github.com/GenomicMedLab/uta-tools/blob/main/docs/TranscriptSelectionPriority.md).
 
 ## Developer Instructions
 
 Clone the repo:
 ```
 git clone https://github.com/cancervariants/variation-normalization.git
 cd variation-normalization
@@ -107,18 +106,16 @@
 You will want to do the following:\
 (*Might not be ._fkuefgd, so replace with your error message path*)
 ```console
 sudo mv /usr/local/share/seqrepo/2021-01-29._fkuefgd /usr/local/share/seqrepo/2021-01-29
 exit
 ```
 
-Use the `SEQREPO_ROOT_DIR` environment variable to set the path of an already existing SeqRepo directory. The default is `/usr/local/share/seqrepo/latest`.
-
 #### UTA
-Variation Normalizer also uses [**C**ommon **O**perations **O**n **L**ots-of **Seq**uences Tool (cool-seq-tool)](https://github.com/GenomicMedLab/cool-seq-tool) which uses [UTA](https://github.com/biocommons/uta) as the underlying PostgreSQL database.
+Variation Normalizer also uses [UTA Tools](https://github.com/GenomicMedLab/uta-tools) which uses [UTA](https://github.com/biocommons/uta) as the underlying PostgreSQL database.
 
 _The following commands will likely need modification appropriate for the installation environment._
 1. Install [PostgreSQL](https://www.postgresql.org/)
 2. Create user and database.
 
     ```
     $ createuser -U postgres uta_admin
@@ -172,9 +169,7 @@
 ```
 
 ### Testing
 From the _root_ directory of the repository:
 ```
 pytest tests/
 ```
-
-
```

### Comparing `variation-normalizer-0.7.0.dev7/README.md` & `variation-normalizer-0.7.dev0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 We are working towards adding more types of variations, coordinates, and representations.
 
 ### Endpoints
 
 The `/to_vrs` endpoint returns a list of validated VRS [Variations](https://vrs.ga4gh.org/en/1.2.0/terms_and_model.html#variation).
 
-The `/normalize` endpoint returns a [Variation Descriptor](https://vrsatile.readthedocs.io/en/latest/value_object_descriptor/vod_index.html#variation-descriptor) containing the MANE Transcript, if one is found. If a genomic query is not given a gene, `normalize` will return its GRCh38 representation. Variation Normalizer relies on [**C**ommon **O**perations **O**n **L**ots-of **Seq**uences Tool (cool-seq-tool)](https://github.com/GenomicMedLab/cool-seq-tool) for retrieving MANE Transcript data. More information on the transcript selection algorithm can be found [here](https://github.com/GenomicMedLab/cool-seq-tool/blob/main/docs/TranscriptSelectionPriority.md).
+The `/normalize` endpoint returns a [Variation Descriptor](https://vrsatile.readthedocs.io/en/latest/value_object_descriptor/vod_index.html#variation-descriptor) containing the MANE Transcript, if one is found. If a genomic query is not given a gene, `normalize` will return its GRCh38 representation. Variation Normalizer relies on [UTA Tools](https://github.com/GenomicMedLab/uta-tools) for retrieving MANE Transcript data. More information on the transcript selection algorithm can be found [here](https://github.com/GenomicMedLab/uta-tools/blob/main/docs/TranscriptSelectionPriority.md).
 
 ## Developer Instructions
 
 Clone the repo:
 ```
 git clone https://github.com/cancervariants/variation-normalization.git
 cd variation-normalization
@@ -86,18 +86,16 @@
 You will want to do the following:\
 (*Might not be ._fkuefgd, so replace with your error message path*)
 ```console
 sudo mv /usr/local/share/seqrepo/2021-01-29._fkuefgd /usr/local/share/seqrepo/2021-01-29
 exit
 ```
 
-Use the `SEQREPO_ROOT_DIR` environment variable to set the path of an already existing SeqRepo directory. The default is `/usr/local/share/seqrepo/latest`.
-
 #### UTA
-Variation Normalizer also uses [**C**ommon **O**perations **O**n **L**ots-of **Seq**uences Tool (cool-seq-tool)](https://github.com/GenomicMedLab/cool-seq-tool) which uses [UTA](https://github.com/biocommons/uta) as the underlying PostgreSQL database.
+Variation Normalizer also uses [UTA Tools](https://github.com/GenomicMedLab/uta-tools) which uses [UTA](https://github.com/biocommons/uta) as the underlying PostgreSQL database.
 
 _The following commands will likely need modification appropriate for the installation environment._
 1. Install [PostgreSQL](https://www.postgresql.org/)
 2. Create user and database.
 
     ```
     $ createuser -U postgres uta_admin
```

### Comparing `variation-normalizer-0.7.0.dev7/setup.cfg` & `variation-normalizer-0.7.dev0/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 name = variation-normalizer
 author = VICC
 author_email = help@cancervariants.org
 description = VICC normalization routine for variations
 long_description = file:README.md
 long_description_content_type = text/markdown
 home-page = https://github.com/cancervariants/variation-normalization
-license_files = LICENSE
+license-file = LICENSE
 license = MIT
 classifiers = 
 	Development Status :: 3 - Alpha
 	Intended Audience :: Science/Research
 	Intended Audience :: Developers
 	Topic :: Scientific/Engineering :: Bio-Informatics
 	License :: OSI Approved :: MIT License
@@ -23,41 +23,37 @@
 zip_safe = False
 include_package_data = True
 install_requires = 
 	biocommons.seqrepo
 	fastapi
 	uvicorn
 	pydantic
-	ga4gh.vrs[extras] >= 0.9.0a0
-	gene-normalizer >= 0.2.9
+	ga4gh.vrs[extras] >= 0.8.7dev0
+	gene-normalizer >= 0.2.3
 	pyliftover
 	boto3
-	ga4gh.vrsatile.pydantic >= 0.1.0.dev8, < 0.2.0
-	cool-seq-tool >= 0.1.13
-	bioutils
+	ga4gh.vrsatile.pydantic >= 0.1.dev3
+	uta-tools >= 0.1.2
 tests_require = 
 	pytest
 	pytest-cov
 	pyyaml
 	pytest-asyncio
 
+[options.package_data]
+variation = 
+	data/amino_acids.csv
+	data/transcript_mapping.tsv
+
 [options.extras_require]
 dev = 
 	pytest
 	pytest-cov
+	pyyaml
 	psycopg2-binary
-	pytest-asyncio
-	flake8
-	flake8-docstrings
-	flake8-quotes
-	flake8-annotations
-	flake8-import-order
-	pre-commit
-	jupyter
-	ipykernel
 
 [tool:pytest]
 addopts = --ignore setup.py --ignore=codebuild/ --doctest-modules --cov-report term-missing --cov .
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `variation-normalizer-0.7.0.dev7/tests/classifiers/classifier_base.py` & `variation-normalizer-0.7.dev0/tests/classifiers/classifier_base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 """A module for testing classifier classes."""
 import yaml
-from gene.database.dynamodb import DynamoDbDatabase
 from gene.query import QueryHandler as GeneQueryHandler
 
-from variation.schemas.classification_response_schema import ConfidenceRating
 from variation.tokenizers import Tokenize
-from variation.tokenizers import GeneSymbol
 from tests import PROJECT_ROOT
+from variation.tokenizers.caches import AminoAcidCache
+from variation.tokenizers import GeneSymbol
 
 
 class ClassifierBase:
     """The classifier base class."""
 
     def setUp(self):
         """Set up the test cases."""
         with open(f"{PROJECT_ROOT}/tests/fixtures/classifiers.yml") as stream:
             self.all_fixtures = yaml.safe_load(stream)
         self.fixtures = self.all_fixtures.get(
             self.fixture_name(),
             {"should_match": [], "should_not_match": []}
         )
         self.classifier = self.classifier_instance()
-        self.tokenizer = Tokenize(GeneSymbol(GeneQueryHandler(DynamoDbDatabase())))
+        self.tokenizer = Tokenize(AminoAcidCache(),
+                                  GeneSymbol(GeneQueryHandler()))
 
     def classifier_instance(self):
         """Check that the classifier_instance method is implemented."""
         raise NotImplementedError()
 
     def fixture_name(self):
         """Check that the fixture_name method is implemented."""
@@ -33,16 +33,16 @@
 
     def test_matches(self):
         """Test that classifier matches correctly."""
         for x in self.fixtures["should_match"]:
             tokens = self.tokenizer.perform(x["query"], [])
             classification = self.classifier.match(tokens)
             self.assertIsNotNone(classification, msg=x)
-            self.assertEqual(getattr(ConfidenceRating, x["confidence"]),
-                             classification.confidence,
+            self.assertEqual(x["confidence"],
+                             str(classification.confidence),
                              msg=x)
 
     def test_not_matches(self):
         """Test that classifier matches correctly."""
         for x in self.fixtures["should_not_match"]:
             tokens = self.tokenizer.perform(x["query"], [])
             classification = self.classifier.match(tokens)
```

### Comparing `variation-normalizer-0.7.0.dev7/tests/classifiers/test_amplification.py` & `variation-normalizer-0.7.dev0/tests/classifiers/test_amplification.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/classifiers/test_coding_dna_deletion.py` & `variation-normalizer-0.7.dev0/tests/classifiers/test_coding_dna_deletion.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/classifiers/test_coding_dna_delins.py` & `variation-normalizer-0.7.dev0/tests/classifiers/test_coding_dna_delins.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/classifiers/test_coding_dna_insertion.py` & `variation-normalizer-0.7.dev0/tests/classifiers/test_coding_dna_insertion.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/classifiers/test_coding_dna_silent_mutation.py` & `variation-normalizer-0.7.dev0/tests/classifiers/test_coding_dna_silent_mutation.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/classifiers/test_coding_dna_substitution.py` & `variation-normalizer-0.7.dev0/tests/classifiers/test_coding_dna_substitution.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/classifiers/test_genomic_deletion.py` & `variation-normalizer-0.7.dev0/tests/classifiers/test_genomic_deletion.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/classifiers/test_genomic_deletion_range.py` & `variation-normalizer-0.7.dev0/tests/classifiers/test_genomic_deletion_range.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/classifiers/test_genomic_delins.py` & `variation-normalizer-0.7.dev0/tests/classifiers/test_genomic_delins.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/classifiers/test_genomic_duplication.py` & `variation-normalizer-0.7.dev0/tests/classifiers/test_genomic_duplication.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/classifiers/test_genomic_insertion.py` & `variation-normalizer-0.7.dev0/tests/classifiers/test_genomic_insertion.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/classifiers/test_genomic_silent_mutation.py` & `variation-normalizer-0.7.dev0/tests/classifiers/test_genomic_silent_mutation.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/classifiers/test_genomic_substitution.py` & `variation-normalizer-0.7.dev0/tests/classifiers/test_genomic_substitution.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/classifiers/test_genomic_uncertain_deletion.py` & `variation-normalizer-0.7.dev0/tests/classifiers/test_genomic_uncertain_deletion.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/classifiers/test_polypeptide_truncation.py` & `variation-normalizer-0.7.dev0/tests/classifiers/test_polypeptide_truncation.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/classifiers/test_protein_deletion.py` & `variation-normalizer-0.7.dev0/tests/classifiers/test_protein_deletion.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/classifiers/test_protein_delins.py` & `variation-normalizer-0.7.dev0/tests/classifiers/test_protein_delins.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/classifiers/test_protein_insertion.py` & `variation-normalizer-0.7.dev0/tests/classifiers/test_protein_insertion.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/classifiers/test_protein_substitution.py` & `variation-normalizer-0.7.dev0/tests/classifiers/test_protein_substitution.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/classifiers/test_silent_mutation.py` & `variation-normalizer-0.7.dev0/tests/classifiers/test_silent_mutation.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/conftest.py` & `variation-normalizer-0.7.dev0/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,15 +64,14 @@
                     "pubmed:9671762",
                     "refseq:NM_000551",
                     "cosmic:VHL",
                     "omim:608537",
                     "vega:OTTHUMG00000128668",
                     "ccds:CCDS2598",
                     "ena.embl:L15409",
-                    "iuphar:3204",
                     "orphanet:120467",
                     "ccds:CCDS2597",
                     "uniprot:P40337"
                 ]
             },
             {
                 "type": "Extension",
@@ -820,20 +819,20 @@
         "start": {"value": 49531260, "type": "Number"},
         "end": {"value": 49531262, "type": "Number"},
         "type": "SequenceLocation"
     }
 
 
 @pytest.fixture(scope="session")
-def genomic_dup1_38_cn(genomic_dup1_seq_loc):
-    """Create test fixture for copy number count dup1 on GRCh38"""
+def genomic_dup1_38_vac(genomic_dup1_seq_loc):
+    """Create test fixture for absolute copy number dup1 on GRCh38"""
     return {
-        "type": "CopyNumberCount",
-        "id": "ga4gh:CN._qniTzHEtNOc6CNjb5bhlV5bf527692Q",
-        "subject": genomic_dup1_seq_loc,
+        "type": "AbsoluteCopyNumber",
+        "id": "ga4gh:ACN._C6yp4SRGVfuRmMiJShIKYCK3dSX0vNF",
+        "location": genomic_dup1_seq_loc,
         "copies": {"type": "Number", "value": 3}
     }
 
 
 @pytest.fixture(scope="session")
 def genomic_dup2_seq_loc():
     """Create genomic dup2 sequence location"""
@@ -843,20 +842,20 @@
         "start": {"value": 2087937, "type": "Number"},
         "end": {"value": 2087948, "type": "Number"},
         "type": "SequenceLocation"
     }
 
 
 @pytest.fixture(scope="session")
-def genomic_dup2_38_cn(genomic_dup2_seq_loc):
-    """Create test fixture for copy number count dup2 on GRCh38"""
+def genomic_dup2_38_vac(genomic_dup2_seq_loc):
+    """Create test fixture for absolute copy number dup2 on GRCh38"""
     return {
-        "type": "CopyNumberCount",
-        "id": "ga4gh:CN.ipqs1zEPgioTqdi3U-m5ex5TCu4QOT7Q",
-        "subject": genomic_dup2_seq_loc,
+        "type": "AbsoluteCopyNumber",
+        "id": "ga4gh:ACN.pUVPSxSZ5n9__GwA2FOQZvNtF_XtIzh1",
+        "location": genomic_dup2_seq_loc,
         "copies": {"type": "Number", "value": 3}
     }
 
 
 @pytest.fixture(scope="session")
 def genomic_del3_dup3_loc():
     """Create genomic del3 dup3 sequence location"""
@@ -866,40 +865,40 @@
         "start": {"min": 31060226, "max": 31100350, "type": "DefiniteRange"},
         "end": {"min": 33274279, "max": 33417152, "type": "DefiniteRange"},
         "type": "SequenceLocation"
     }
 
 
 @pytest.fixture(scope="session")
-def genomic_dup4_loc():
-    """Create genomic dup4 sequence location"""
+def genoimc_dup4_loc():
+    """Create genoimc dup4 sequence location"""
     return {
         "id": "ga4gh:SL.uD8efGXIXdiMNyHX4MogVF0jA28jIWb4",
         "sequence_id": "ga4gh:SQ.-A1QmD_MatoqxvgVxBLZTONHz9-c7nQo",
         "start": {"value": 30417575, "comparator": "<=", "type": "IndefiniteRange"},
         "end": {"value": 31394018, "comparator": ">=", "type": "IndefiniteRange"},
         "type": "SequenceLocation"
     }
 
 
 @pytest.fixture(scope="session")
 def genomic_dup5_loc():
-    """Create genomic dup5 sequence location"""
+    """Create genoimc dup5 sequence location"""
     return {
         "id": "ga4gh:SL.GzmuP1MBA9qILR8fVFhp4BdUEcaLwKaR",
         "sequence_id": "ga4gh:SQ.w0WZEvgJF0zf_P4yyTzjjv9oW1z61HHP",
         "start": {"value": 154021811, "comparator": "<=", "type": "IndefiniteRange"},
         "end": {"value": 154092209, "type": "Number"},
         "type": "SequenceLocation"
     }
 
 
 @pytest.fixture(scope="session")
-def genomic_dup6_loc():
-    """Create genomic dup6 sequence location"""
+def genoimc_dup6_loc():
+    """Create genoimc dup6 sequence location"""
     return {
         "id": "ga4gh:SL.8j0dwTvx7zKHVk2JCDt1eqoEt-o993hg",
         "sequence_id": "ga4gh:SQ.w0WZEvgJF0zf_P4yyTzjjv9oW1z61HHP",
         "start": {"value": 154021811, "type": "Number"},
         "end": {"value": 154092209, "comparator": ">=", "type": "IndefiniteRange"},
         "type": "SequenceLocation"
     }
@@ -914,20 +913,20 @@
         "start": {"value": 10149810, "type": "Number"},
         "end": {"value": 10149811, "type": "Number"},
         "type": "SequenceLocation"
     }
 
 
 @pytest.fixture(scope="session")
-def genomic_del1_38_cn(genomic_del1_seq_loc):
-    """Create test fixture for copy number count del1 on GRCh38"""
+def genomic_del1_38_vac(genomic_del1_seq_loc):
+    """Create test fixture for absolute copy number del1 on GRCh38"""
     return {
-        "type": "CopyNumberCount",
-        "id": "ga4gh:CN.4SoY4bWbd7hDMJmIPr2vVjCMWetgtunL",
-        "subject": genomic_del1_seq_loc,
+        "type": "AbsoluteCopyNumber",
+        "id": "ga4gh:ACN.-B_iqSMiz6RCkwNC4PeL0DGUPHz0ZuAO",
+        "location": genomic_del1_seq_loc,
         "copies": {"type": "Number", "value": 1}
     }
 
 
 @pytest.fixture(scope="session")
 def genomic_del2_seq_loc():
     """Create genomic del2 sequence location"""
@@ -937,20 +936,20 @@
         "start": {"value": 10146594, "type": "Number"},
         "end": {"value": 10146613, "type": "Number"},
         "type": "SequenceLocation"
     }
 
 
 @pytest.fixture(scope="session")
-def genomic_del2_38_cn(genomic_del2_seq_loc):
-    """Create test fixture for copy number count del1 on GRCh38"""
+def genomic_del2_38_vac(genomic_del2_seq_loc):
+    """Create test fixture for absolute copy number del1 on GRCh38"""
     return {
-        "type": "CopyNumberCount",
-        "id": "ga4gh:CN.-4obfHvLoblo593QiHeJkCORSBT3SbNV",
-        "subject": genomic_del2_seq_loc,
+        "type": "AbsoluteCopyNumber",
+        "id": "ga4gh:ACN.GXkCtgRsF6xmzYowbGt6RFTYck07nCWW",
+        "location": genomic_del2_seq_loc,
         "copies": {"type": "Number", "value": 1}
     }
 
 
 @pytest.fixture(scope="session")
 def genomic_del4_seq_loc():
     """Create genomic del4 sequence location"""
@@ -1016,18 +1015,18 @@
 @pytest.fixture(scope="session")
 def braf_amplification(braf_ncbi_seq_loc, braf_gene_context):
     """Create test fixture for BRAF Amplification"""
     params = {
         "id": "normalize.variation:BRAF%20Amplification",
         "type": "VariationDescriptor",
         "variation": {
-            "id": "ga4gh:CX.1RJp1zW60x2t4Exc4965_a3CvYFtsL4q",
-            "subject": braf_ncbi_seq_loc,
-            "copy_change": "efo:0030072",
-            "type": "CopyNumberChange"
+            "id": "ga4gh:RCN.avsI73-9i6ykDIRB3eB89jeU1lhyBbYt",
+            "location": braf_ncbi_seq_loc,
+            "relative_copy_class": "high-level gain",
+            "type": "RelativeCopyNumber"
         },
         "molecule_context": "genomic",
         "structural_type": "SO:0001880",
         "gene_context": braf_gene_context
     }
     return VariationDescriptor(**params)
 
@@ -1035,18 +1034,18 @@
 @pytest.fixture(scope="session")
 def prpf8_amplification(prpf8_ncbi_seq_loc, prpf8_gene_context):
     """Create test fixture for PRPF8 Amplification"""
     params = {
         "id": "normalize.variation:PRPF8%20AMPLIFICATION",
         "type": "VariationDescriptor",
         "variation": {
-            "id": "ga4gh:CX.juBTsOcCmUPHUAMu-s-Bu0oZhj1VktTL",
-            "subject": prpf8_ncbi_seq_loc,
-            "copy_change": "efo:0030072",
-            "type": "CopyNumberChange"
+            "id": "ga4gh:RCN.w44H1MxQusrCBDxUoLr30E1iJBMGXF14",
+            "location": prpf8_ncbi_seq_loc,
+            "relative_copy_class": "high-level gain",
+            "type": "RelativeCopyNumber"
         },
         "molecule_context": "genomic",
         "structural_type": "SO:0001880",
         "gene_context": prpf8_gene_context
     }
     return VariationDescriptor(**params)
```

### Comparing `variation-normalizer-0.7.0.dev7/tests/test_codon_table.py` & `variation-normalizer-0.7.dev0/tests/test_codon_table.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Module for testing Codon Table class."""
 import pytest
 
 from variation.data_sources.codon_table import CodonTable
+from variation.tokenizers.caches import AminoAcidCache
 
 
 @pytest.fixture(scope="module")
 def test_codon_table():
     """Build codon table test fixture."""
-    return CodonTable()
+    return CodonTable(AminoAcidCache())
 
 
 def test_get_codons(test_codon_table):
     """Test that _get_codons method works correctly."""
     ala_codons = ["GCA", "GCC", "GCG", "GCU"]
     assert test_codon_table.get_codons("A") == ala_codons
     assert test_codon_table.get_codons("a") == ala_codons
```

### Comparing `variation-normalizer-0.7.0.dev7/tests/test_gnomad_vcf_to_protein.py` & `variation-normalizer-0.7.dev0/tests/test_gnomad_vcf_to_protein.py`

 * *Files 0% similar despite different names*

```diff
@@ -794,17 +794,16 @@
     variation = resp.variation_descriptor.dict()["variation"]
     assert variation == kras_g12d
 
 
 @pytest.mark.asyncio
 async def test_silent_mutation(test_handler, vhl_silent):
     """Test that silent queries return correct response"""
-    # https://www.ncbi.nlm.nih.gov/clinvar/variation/379039/?new_evidence=true
-    resp = await test_handler.gnomad_vcf_to_protein("3-10142030-C-C")
-    assertion_checks(resp.variation_descriptor, vhl_silent, "3-10142030-C-C",
+    resp = await test_handler.gnomad_vcf_to_protein("3-10183714-C-C")
+    assertion_checks(resp.variation_descriptor, vhl_silent, "3-10183714-C-C",
                      ignore_id=True)
     assert resp.warnings == []
 
 
 @pytest.mark.asyncio
 async def test_insertion(test_handler, protein_insertion,
                          protein_insertion2):
@@ -847,14 +846,15 @@
     assert resp.warnings == ["BRAF V600E is not a supported gnomad vcf query"]
 
     resp = await test_handler.gnomad_vcf_to_protein("7-140753336-T-G",
                                                     untranslatable_returns_text=True)
     assert resp.variation_descriptor.variation.type == "Text"
     assert resp.variation_descriptor.label == "7-140753336-T-G"
     assert set(resp.warnings) == {
+        "Unable to get transcripts given NC_000007.13 and 140753336",
         "Expected T but found A on NC_000007.14 at position 140753336",
     }
 
     resp = await test_handler.gnomad_vcf_to_protein("20-2-TC-TG",
                                                     untranslatable_returns_text=True)
     assert resp.variation_descriptor.variation.type == "Text"
     assert resp.variation_descriptor.label == "20-2-TC-TG"
```

### Comparing `variation-normalizer-0.7.0.dev7/tests/test_hgvs_dup_del_mode.py` & `variation-normalizer-0.7.dev0/tests/test_hgvs_dup_del_mode.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 """Module for testing HGVS Dup Del mode."""
-from copy import deepcopy
-
 import pytest
 from ga4gh.vrsatile.pydantic.vrsatile_models import VariationDescriptor
 
 from tests.conftest import assertion_checks
 
 
 @pytest.fixture(scope="module")
@@ -305,28 +303,28 @@
             "sequence": "GGG"
         }
     }
     return VariationDescriptor(**genomic_dup1)
 
 
 @pytest.fixture(scope="module")
-def genomic_dup1_cn(genomic_dup1, genomic_dup1_38_cn):
-    """Create a test fixture for genomic dup copy number count."""
-    genomic_dup1["variation"] = genomic_dup1_38_cn
+def genomic_dup1_vac(genomic_dup1, genomic_dup1_38_vac):
+    """Create a test fixture for genomic dup absolute CNV."""
+    genomic_dup1["variation"] = genomic_dup1_38_vac
     return VariationDescriptor(**genomic_dup1)
 
 
 @pytest.fixture(scope="module")
-def genomic_dup1_cx(genomic_dup1, genomic_dup1_seq_loc):
-    """Create a test fixture for genomic dup copy number change."""
+def genomic_dup1_vrc(genomic_dup1, genomic_dup1_seq_loc):
+    """Create a test fixture for genomic dup relative CNV."""
     genomic_dup1["variation"] = {
-        "type": "CopyNumberChange",
-        "id": "ga4gh:CX.z-wPsq2XjN_knrIpLUTAeFzO6xt13QrR",
-        "subject": genomic_dup1_seq_loc,
-        "copy_change": "efo:0030072"
+        "type": "RelativeCopyNumber",
+        "id": "ga4gh:RCN.qSnPCsf9ylOaecpSBjTkxWFqxmmyYWtL",
+        "location": genomic_dup1_seq_loc,
+        "relative_copy_class": "high-level gain"
     }
     return VariationDescriptor(**genomic_dup1)
 
 
 @pytest.fixture(scope="module")
 def genomic_dup1_rse(genomic_dup1, genomic_dup1_seq_loc):
     """Create a test fixture for genomic dup RSE."""
@@ -503,20 +501,22 @@
             "sequence": "GGG"
         }
     }
     return VariationDescriptor(**genomic_dup1_free_text)
 
 
 @pytest.fixture(scope="module")
-def genomic_dup1_free_text_cn(genomic_dup1_free_text, genomic_dup1_free_text_seq_loc):
-    """Create a test fixture for genomic dup copy number count."""
+def genomic_dup1_free_text_vac(genomic_dup1_free_text,
+                               genomic_dup1_free_text_seq_loc):
+    """Create a test fixture for genomic dup absolute CNV."""
+    _id = "ga4gh:ACN.TpprCQKgSaGlbBdbAAv4RoOS5yvE4jf2"
     genomic_dup1_free_text["variation"] = {
-        "type": "CopyNumberCount",
-        "id": "ga4gh:CN.sdovzZNQZz5lIHy3ME4i4jw4kXCzJmI2",
-        "subject": genomic_dup1_free_text_seq_loc,
+        "type": "AbsoluteCopyNumber",
+        "id": _id,
+        "location": genomic_dup1_free_text_seq_loc,
         "copies": {"type": "Number", "value": 3}
     }
     return VariationDescriptor(**genomic_dup1_free_text)
 
 
 @pytest.fixture(scope="module")
 def genomic_dup1_free_text_rse(genomic_dup1_free_text,
@@ -570,28 +570,28 @@
             "sequence": "AAAGGTAGGGCAAAGGTAGGGC"
         }
     }
     return VariationDescriptor(**genomic_dup2)
 
 
 @pytest.fixture(scope="module")
-def genomic_dup2_cn(genomic_dup2, genomic_dup2_38_cn):
-    """Create a test fixture for genomic dup copy number count."""
-    genomic_dup2["variation"] = genomic_dup2_38_cn
+def genomic_dup2_vac(genomic_dup2, genomic_dup2_38_vac):
+    """Create a test fixture for genomic dup absolute CNV."""
+    genomic_dup2["variation"] = genomic_dup2_38_vac
     return VariationDescriptor(**genomic_dup2)
 
 
 @pytest.fixture(scope="module")
-def genomic_dup2_cx(genomic_dup2, genomic_dup2_seq_loc):
-    """Create a test fixture for genomic dup copy number change."""
+def genomic_dup2_vrc(genomic_dup2, genomic_dup2_seq_loc):
+    """Create a test fixture for genomic dup relative CNV."""
     genomic_dup2["variation"] = {
-        "type": "CopyNumberChange",
-        "id": "ga4gh:CX.mLcltO7D-Wq6td1IBIcn4Wo0h5trqM-S",
-        "subject": genomic_dup2_seq_loc,
-        "copy_change": "efo:0030070"
+        "type": "RelativeCopyNumber",
+        "id": "ga4gh:RCN.zizBAY460E_wbra9Y6oCxojd8YCbIfnx",
+        "location": genomic_dup2_seq_loc,
+        "relative_copy_class": "low-level gain"
     }
     return VariationDescriptor(**genomic_dup2)
 
 
 @pytest.fixture(scope="module")
 def genomic_dup2_rse(genomic_dup2, genomic_dup2_seq_loc):
     """Create a test fixture for genomic dup RSE."""
@@ -657,20 +657,22 @@
             "sequence": "TAGATAGA"
         }
     }
     return VariationDescriptor(**genomic_dup2_free_text)
 
 
 @pytest.fixture(scope="module")
-def genomic_dup2_free_text_cn(genomic_dup2_free_text, genomic_dup2_free_text_seq_loc):
-    """Create a test fixture for genomic dup copy number count."""
+def genomic_dup2_free_text_vac(genomic_dup2_free_text,
+                               genomic_dup2_free_text_seq_loc):
+    """Create a test fixture for genomic dup absolute CNV."""
+    _id = "ga4gh:ACN.McPtQ3LSldeGzC6-qMEGJXIjPLGNEyky"
     genomic_dup2_free_text["variation"] = {
-        "type": "CopyNumberCount",
-        "id": "ga4gh:CN.gNWVM7yYOrhA5rzRs3zrj3stQT3Phvyn",
-        "subject": genomic_dup2_free_text_seq_loc,
+        "type": "AbsoluteCopyNumber",
+        "id": _id,
+        "location": genomic_dup2_free_text_seq_loc,
         "copies": {"type": "Number", "value": 3}
     }
     return VariationDescriptor(**genomic_dup2_free_text)
 
 
 @pytest.fixture(scope="module")
 def genomic_dup2_free_text_rse(genomic_dup2_free_text,
@@ -708,33 +710,35 @@
         "structural_type": "SO:0001742",
         "vrs_ref_allele_seq": None
     }
     return params
 
 
 @pytest.fixture(scope="module")
-def genomic_dup3_cn(genomic_dup3, genomic_del3_dup3_loc):
-    """Create a test fixture for genomic dup copy number count."""
+def genomic_dup3_vac(genomic_dup3, genomic_del3_dup3_loc):
+    """Create a test fixture for genomic dup absolute cnv."""
+    _id = "ga4gh:ACN.2ZUQcccwvtoGZ5LZZRUoDZp6218Y6sQK"
     genomic_dup3["variation"] = {
-        "type": "CopyNumberCount",
-        "id": "ga4gh:CN.a2-YlA01Q-y2zAOgn4r-cP9hiIEGaaqq",
-        "subject": genomic_del3_dup3_loc,
+        "type": "AbsoluteCopyNumber",
+        "id": _id,
+        "location": genomic_del3_dup3_loc,
         "copies": {"type": "Number", "value": 2}
     }
     return VariationDescriptor(**genomic_dup3)
 
 
 @pytest.fixture(scope="module")
-def genomic_dup3_cx(genomic_dup3, genomic_del3_dup3_loc):
-    """Create a test fixture for genomic dup copy number change."""
+def genomic_dup3_vrc(genomic_dup3, genomic_del3_dup3_loc):
+    """Create a test fixture for genomic dup relative cnv."""
+    _id = "ga4gh:RCN.4m1TD2538i7v4NQ_OeJ-pIEhlRpYZ3_y"
     genomic_dup3["variation"] = {
-        "type": "CopyNumberChange",
-        "id": "ga4gh:CX.cmQ2h4FXbNHHTZHJ8N0sOXIE01RfyBxb",
-        "subject": genomic_del3_dup3_loc,
-        "copy_change": "efo:0030070"
+        "type": "RelativeCopyNumber",
+        "id": _id,
+        "location": genomic_del3_dup3_loc,
+        "relative_copy_class": "low-level gain"
     }
     return VariationDescriptor(**genomic_dup3)
 
 
 @pytest.fixture(scope="module")
 def genomic_dup3_rse_lse(genomic_dup3):
     """Create test fixture for genomic dup rse and lse."""
@@ -774,32 +778,34 @@
         "start": {"min": 31147273, "max": 31147277, "type": "DefiniteRange"},
         "end": {"min": 31182738, "max": 31182740, "type": "DefiniteRange"},
         "type": "SequenceLocation"
     }
 
 
 @pytest.fixture(scope="module")
-def genomic_dup3_free_text_cx(genomic_dup3_free_text, genomic_dup3_free_text_subject):
-    """Create a test fixture for genomic dup copy number change."""
+def genomic_dup3_free_text_vrc(genomic_dup3_free_text, genomic_dup3_free_text_subject):
+    """Create a test fixture for genomic dup relative cnv."""
+    _id = "ga4gh:RCN.ReWfNwAnchjIPJQEXM038T9M3OsOO7yK"
     genomic_dup3_free_text["variation"] = {
-        "type": "CopyNumberChange",
-        "id": "ga4gh:CX.C0njAM6WcOua46XljTLLCVQkNVIChQU0",
-        "subject": genomic_dup3_free_text_subject,
-        "copy_change": "efo:0030070"
+        "type": "RelativeCopyNumber",
+        "id": _id,
+        "location": genomic_dup3_free_text_subject,
+        "relative_copy_class": "low-level gain"
     }
     return VariationDescriptor(**genomic_dup3_free_text)
 
 
 @pytest.fixture(scope="module")
-def genomic_dup3_free_text_cn(genomic_dup3_free_text, genomic_dup3_free_text_subject):
-    """Create a test fixture for genomic dup copy number count."""
+def genomic_dup3_free_text_vac(genomic_dup3_free_text, genomic_dup3_free_text_subject):
+    """Create a test fixture for genomic dup absolute cnv."""
+    _id = "ga4gh:ACN.5B1zY9uirjKRQ5gT_6C0Z0FhdJHwG_yS"
     genomic_dup3_free_text["variation"] = {
-        "type": "CopyNumberCount",
-        "id": "ga4gh:CN.yfsv4o1sfFpFUxKTS1de9ODUN8fSWMQh",
-        "subject": genomic_dup3_free_text_subject,
+        "type": "AbsoluteCopyNumber",
+        "id": _id,
+        "location": genomic_dup3_free_text_subject,
         "copies": {"type": "Number", "value": 4}
     }
     return VariationDescriptor(**genomic_dup3_free_text)
 
 
 @pytest.fixture(scope="module")
 def genomic_dup3_free_text_rse_lse(genomic_dup3_free_text):
@@ -827,32 +833,34 @@
         "structural_type": "SO:0001742",
         "vrs_ref_allele_seq": None
     }
     return params
 
 
 @pytest.fixture(scope="module")
-def genomic_dup4_cx(genomic_dup4, genomic_dup4_loc):
-    """Create a test fixture for genomic dup copy number change."""
+def genomic_dup4_vrc(genomic_dup4, genoimc_dup4_loc):
+    """Create a test fixture for genomic dup relative cnv."""
+    _id = "ga4gh:RCN.uSGvLYzpzivqDzhuKR44DHc5imZJSmoV"
     genomic_dup4["variation"] = {
-        "type": "CopyNumberChange",
-        "id": "ga4gh:CX.b7MlHXZcBEe4M81yZviR-Fujo4OKrcw3",
-        "subject": genomic_dup4_loc,
-        "copy_change": "efo:0030070"
+        "type": "RelativeCopyNumber",
+        "id": _id,
+        "location": genoimc_dup4_loc,
+        "relative_copy_class": "low-level gain"
     }
     return VariationDescriptor(**genomic_dup4)
 
 
 @pytest.fixture(scope="module")
-def genomic_dup4_cn(genomic_dup4, genomic_dup4_loc):
-    """Create a test fixture for genomic dup copy number count."""
+def genomic_dup4_vac(genomic_dup4, genoimc_dup4_loc):
+    """Create a test fixture for genomic dup absolute cnv."""
+    _id = "ga4gh:ACN.OBSQ6SY9waWJ7YOyYA_qK0te_mTfOT4A"
     genomic_dup4["variation"] = {
-        "type": "CopyNumberCount",
-        "id": "ga4gh:CN.Fvt2VSCSLNROTjZd20vKZUzdMYxz-cfZ",
-        "subject": genomic_dup4_loc,
+        "type": "AbsoluteCopyNumber",
+        "id": _id,
+        "location": genoimc_dup4_loc,
         "copies": {"type": "Number", "value": 3}
     }
     return VariationDescriptor(**genomic_dup4)
 
 
 @pytest.fixture(scope="module")
 def genomic_dup4_rse_lse(genomic_dup4):
@@ -893,32 +901,34 @@
         "start": {"value": 1674441, "comparator": "<=", "type": "IndefiniteRange"},
         "end": {"value": 1684571, "comparator": ">=", "type": "IndefiniteRange"},
         "type": "SequenceLocation"
     }
 
 
 @pytest.fixture(scope="module")
-def genomic_dup4_free_text_cx(genomic_dup4_free_text, genomic_dup4_free_text_subject):
-    """Create a test fixture for genomic dup copy number change."""
+def genomic_dup4_free_text_vrc(genomic_dup4_free_text, genomic_dup4_free_text_subject):
+    """Create a test fixture for genomic dup relative cnv."""
+    _id = "ga4gh:RCN.Cf9r8JDpUC18VkkEv44jf8b8WMqUIRFu"
     genomic_dup4_free_text["variation"] = {
-        "type": "CopyNumberChange",
-        "id": "ga4gh:CX.vhV4v1BK5hFQXHX9qysZFpIYhrgI5-Nf",
-        "subject": genomic_dup4_free_text_subject,
-        "copy_change": "efo:0030070"
+        "type": "RelativeCopyNumber",
+        "id": _id,
+        "location": genomic_dup4_free_text_subject,
+        "relative_copy_class": "low-level gain"
     }
     return VariationDescriptor(**genomic_dup4_free_text)
 
 
 @pytest.fixture(scope="module")
-def genomic_dup4_free_text_cn(genomic_dup4_free_text, genomic_dup4_free_text_subject):
-    """Create a test fixture for genomic dup copy number count."""
+def genomic_dup4_free_text_vac(genomic_dup4_free_text, genomic_dup4_free_text_subject):
+    """Create a test fixture for genomic dup absolute cnv."""
+    _id = "ga4gh:ACN.g4-wQni3sHHQNArM4DaIYjh2YuZFKkiv"
     genomic_dup4_free_text["variation"] = {
-        "type": "CopyNumberCount",
-        "id": "ga4gh:CN.oFSw_z1nfk0Yr1mCIi3uKIF-KGC-x8lQ",
-        "subject": genomic_dup4_free_text_subject,
+        "type": "AbsoluteCopyNumber",
+        "id": _id,
+        "location": genomic_dup4_free_text_subject,
         "copies": {"type": "Number", "value": 3}
     }
     return VariationDescriptor(**genomic_dup4_free_text)
 
 
 @pytest.fixture(scope="module")
 def genomic_dup4_free_text_rse_lse(genomic_dup4_free_text):
@@ -945,45 +955,47 @@
         "molecule_context": "genomic",
         "structural_type": "SO:0001742",
         "vrs_ref_allele_seq": None
     }
     return params
 
 
-def genomic_dup5_cn_var(params, genomic_dup5_loc):
-    """Create genomic dup5 copy number count"""
+def genomic_dup5_abs_cnv(params, genomic_dup5_loc):
+    """Create genomic dup5 aboluste cnv"""
+    _id = "ga4gh:ACN.BoEis2HKjiA0yZKs2yvvX-xOSkLxKHlC"
     params["variation"] = {
-        "type": "CopyNumberCount",
-        "id": "ga4gh:CN.uhQfl3d-UonMZDnK6FAASUtY8FTaHplR",
-        "subject": genomic_dup5_loc,
+        "type": "AbsoluteCopyNumber",
+        "id": _id,
+        "location": genomic_dup5_loc,
         "copies": {"type": "Number", "value": 3}
     }
 
 
-def genomic_dup5_cx_var(params, genomic_dup5_loc):
-    """Create genomic dup4 copy number change"""
+def genomic_dup5_rel_cnv(params, genomic_dup5_loc):
+    """Create genomic dup4 relative cnv"""
+    _id = "ga4gh:RCN.tr_brFSOfykm3I3ufLQTS9pV8KKjqLhK"
     params["variation"] = {
-        "type": "CopyNumberChange",
-        "id": "ga4gh:CX.rBUl0BJiar7-NX0pU23NEln2KAifk03p",
-        "subject": genomic_dup5_loc,
-        "copy_change": "efo:0030070"
+        "type": "RelativeCopyNumber",
+        "id": _id,
+        "location": genomic_dup5_loc,
+        "relative_copy_class": "low-level gain"
     }
 
 
 @pytest.fixture(scope="module")
-def genomic_dup5_cx(genomic_dup5, genomic_dup5_loc):
-    """Create a test fixture for genomic dup5 copy number change."""
-    genomic_dup5_cx_var(genomic_dup5, genomic_dup5_loc)
+def genomic_dup5_vrc(genomic_dup5, genomic_dup5_loc):
+    """Create a test fixture for genomic dup5 relative cnv."""
+    genomic_dup5_rel_cnv(genomic_dup5, genomic_dup5_loc)
     return VariationDescriptor(**genomic_dup5)
 
 
 @pytest.fixture(scope="module")
-def genomic_dup5_cn(genomic_dup5, genomic_dup5_loc):
-    """Create a test fixture for genomic dup5 copy number count."""
-    genomic_dup5_cn_var(genomic_dup5, genomic_dup5_loc)
+def genomic_dup5_vac(genomic_dup5, genomic_dup5_loc):
+    """Create a test fixture for genomic dup5 absolute cnv."""
+    genomic_dup5_abs_cnv(genomic_dup5, genomic_dup5_loc)
     return VariationDescriptor(**genomic_dup5)
 
 
 @pytest.fixture(scope="module")
 def genomic_dup5_rse_lse(genomic_dup5):
     """Create test fixture for genomic dup rse and lse."""
     params = {
@@ -1010,24 +1022,24 @@
         "vrs_ref_allele_seq": None,
         "gene_context": mecp2_gene_context
     }
     return params
 
 
 @pytest.fixture(scope="module")
-def genomic_dup5_free_text_cx(genomic_dup5_free_text, genomic_dup5_loc):
-    """Create a test fixture for genomic dup copy number change."""
-    genomic_dup5_cx_var(genomic_dup5_free_text, genomic_dup5_loc)
+def genomic_dup5_free_text_vrc(genomic_dup5_free_text, genomic_dup5_loc):
+    """Create a test fixture for genomic dup relative cnv."""
+    genomic_dup5_rel_cnv(genomic_dup5_free_text, genomic_dup5_loc)
     return VariationDescriptor(**genomic_dup5_free_text)
 
 
 @pytest.fixture(scope="module")
-def genomic_dup5_free_text_cn(genomic_dup5_free_text, genomic_dup5_loc):
-    """Create a test fixture for genomic dup copy number count."""
-    genomic_dup5_cn_var(genomic_dup5_free_text, genomic_dup5_loc)
+def genomic_dup5_free_text_vac(genomic_dup5_free_text, genomic_dup5_loc):
+    """Create a test fixture for genomic dup absolute cnv."""
+    genomic_dup5_abs_cnv(genomic_dup5_free_text, genomic_dup5_loc)
     return VariationDescriptor(**genomic_dup5_free_text)
 
 
 @pytest.fixture(scope="module")
 def genomic_dup5_free_text_rse_lse(genomic_dup5_free_text):
     """Create test fixture for genomic dup rse and lse."""
     params = {
@@ -1052,45 +1064,47 @@
         "molecule_context": "genomic",
         "structural_type": "SO:0001742",
         "vrs_ref_allele_seq": None
     }
     return params
 
 
-def genomic_dup6_cx_var(params, genomic_dup6_loc):
-    """Create genomic dup6 copy number change"""
+def genomic_dup6_rel_cnv(params, genoimc_dup6_loc):
+    """Create genomic dup6 relative cnv"""
+    _id = "ga4gh:RCN.c5Uq3TFDNpQSyDlbXb0BRonw9AYHHk0H"
     params["variation"] = {
-        "type": "CopyNumberChange",
-        "id": "ga4gh:CX.IbkRumjnx-rxHbWONhJKgl-9zixCnArU",
-        "subject": genomic_dup6_loc,
-        "copy_change": "efo:0030070"
+        "type": "RelativeCopyNumber",
+        "id": _id,
+        "location": genoimc_dup6_loc,
+        "relative_copy_class": "low-level gain"
     }
 
 
-def genomic_dup6_cn_var(params, genomic_dup6_loc):
-    """Create genomic dup6 copy number count"""
+def genomic_dup6_abs_cnv(params, genoimc_dup6_loc):
+    """Create genomic dup6 absolute cnv"""
+    _id = "ga4gh:ACN.6q8D5d_ie9MO0HdNEJmRJmGMg8C5LdAM"
     params["variation"] = {
-        "type": "CopyNumberCount",
-        "id": "ga4gh:CN.Tuvj2C1xYVUF0UL3CSB1GZjCRC6K_eSt",
-        "subject": genomic_dup6_loc,
+        "type": "AbsoluteCopyNumber",
+        "id": _id,
+        "location": genoimc_dup6_loc,
         "copies": {"type": "Number", "value": 2}
     }
 
 
 @pytest.fixture(scope="module")
-def genomic_dup6_cx(genomic_dup6, genomic_dup6_loc):
-    """Create a test fixture for genomic dup copy number change."""
-    genomic_dup6_cx_var(genomic_dup6, genomic_dup6_loc)
+def genomic_dup6_vrc(genomic_dup6, genoimc_dup6_loc):
+    """Create a test fixture for genomic dup relative cnv."""
+    genomic_dup6_rel_cnv(genomic_dup6, genoimc_dup6_loc)
     return VariationDescriptor(**genomic_dup6)
 
 
 @pytest.fixture(scope="module")
-def genomic_dup6_cn(genomic_dup6, genomic_dup6_loc):
-    """Create a test fixture for genomic dup copy number count."""
-    genomic_dup6_cn_var(genomic_dup6, genomic_dup6_loc)
+def genomic_dup6_vac(genomic_dup6, genoimc_dup6_loc):
+    """Create a test fixture for genomic dup absolute cnv."""
+    genomic_dup6_abs_cnv(genomic_dup6, genoimc_dup6_loc)
     return VariationDescriptor(**genomic_dup6)
 
 
 @pytest.fixture(scope="module")
 def genomic_dup6_rse_lse(genomic_dup6):
     """Create test fixture for genomic dup rse and lse."""
     params = {
@@ -1117,24 +1131,24 @@
         "vrs_ref_allele_seq": None,
         "gene_context": mecp2_gene_context
     }
     return params
 
 
 @pytest.fixture(scope="module")
-def genomic_dup6_free_text_cx(genomic_dup6_free_text, genomic_dup6_loc):
-    """Create a test fixture for genomic dup copy number change."""
-    genomic_dup6_cx_var(genomic_dup6_free_text, genomic_dup6_loc)
+def genomic_dup6_free_text_vrc(genomic_dup6_free_text, genoimc_dup6_loc):
+    """Create a test fixture for genomic dup relative cnv."""
+    genomic_dup6_rel_cnv(genomic_dup6_free_text, genoimc_dup6_loc)
     return VariationDescriptor(**genomic_dup6_free_text)
 
 
 @pytest.fixture(scope="module")
-def genomic_dup6_free_text_cn(genomic_dup6_free_text, genomic_dup6_loc):
-    """Create a test fixture for genomic dup copy number count."""
-    genomic_dup6_cn_var(genomic_dup6_free_text, genomic_dup6_loc)
+def genomic_dup6_free_text_vac(genomic_dup6_free_text, genoimc_dup6_loc):
+    """Create a test fixture for genomic dup absolute cnv."""
+    genomic_dup6_abs_cnv(genomic_dup6_free_text, genoimc_dup6_loc)
     return VariationDescriptor(**genomic_dup6_free_text)
 
 
 @pytest.fixture(scope="module")
 def genomic_dup6_free_text_rse_lse(genomic_dup6_free_text):
     """Create test fixture for genomic dup rse and lse."""
     params = {
@@ -1176,28 +1190,28 @@
             "sequence": ""
         }
     }
     return VariationDescriptor(**genomic_del1)
 
 
 @pytest.fixture(scope="module")
-def genomic_del1_cn(genomic_del1, genomic_del1_38_cn):
-    """Create a test fixture for genomic del copy number count."""
-    genomic_del1["variation"] = genomic_del1_38_cn
+def genomic_del1_vac(genomic_del1, genomic_del1_38_vac):
+    """Create a test fixture for genomic del absolute CNV."""
+    genomic_del1["variation"] = genomic_del1_38_vac
     return VariationDescriptor(**genomic_del1)
 
 
 @pytest.fixture(scope="module")
-def genomic_del1_cx(genomic_del1, genomic_del1_seq_loc):
-    """Create a test fixture for genomic del copy number change."""
+def genomic_del1_vrc(genomic_del1, genomic_del1_seq_loc):
+    """Create a test fixture for genomic del relative CNV."""
     genomic_del1["variation"] = {
-        "type": "CopyNumberChange",
-        "id": "ga4gh:CX.LIMo4t9dxh_lxtppith_0xULcbIoGYi0",
-        "subject": genomic_del1_seq_loc,
-        "copy_change": "efo:0030067"
+        "type": "RelativeCopyNumber",
+        "id": "ga4gh:RCN.z7MU8QUSR_aeWG7MP161H4jwPGoyo1No",
+        "location": genomic_del1_seq_loc,
+        "relative_copy_class": "copy neutral"
     }
     return VariationDescriptor(**genomic_del1)
 
 
 @pytest.fixture(scope="module")
 def genomic_del1_rse(genomic_del1, genomic_del1_seq_loc):
     """Create a test fixture for genomic del RSE."""
@@ -1263,20 +1277,22 @@
             "sequence": ""
         }
     }
     return VariationDescriptor(**genomic_del1_free_text)
 
 
 @pytest.fixture(scope="module")
-def genomic_del1_free_text_cn(genomic_del1_free_text, genomic_del1_free_text_seq_loc):
-    """Create a test fixture for genomic del copy number count."""
+def genomic_del1_free_text_vac(genomic_del1_free_text,
+                               genomic_del1_free_text_seq_loc):
+    """Create a test fixture for genomic del absolute CNV."""
+    _id = "ga4gh:ACN.3dlkcT_WnurdradNYgs8gHW_pyP-FLYA"
     genomic_del1_free_text["variation"] = {
-        "type": "CopyNumberCount",
-        "id": "ga4gh:CN.ftCNLk6wg-0szErbIRcEZLhF6aUXd-3D",
-        "subject": genomic_del1_free_text_seq_loc,
+        "type": "AbsoluteCopyNumber",
+        "id": _id,
+        "location": genomic_del1_free_text_seq_loc,
         "copies": {"type": "Number", "value": 1}
     }
     return VariationDescriptor(**genomic_del1_free_text)
 
 
 @pytest.fixture(scope="module")
 def genomic_del1_free_text_rse(genomic_del1_free_text,
@@ -1330,28 +1346,28 @@
             "sequence": ""
         }
     }
     return VariationDescriptor(**genomic_del2)
 
 
 @pytest.fixture(scope="module")
-def genomic_del2_cn(genomic_del2, genomic_del2_38_cn):
-    """Create a test fixture for genomic del copy number count."""
-    genomic_del2["variation"] = genomic_del2_38_cn
+def genomic_del2_vac(genomic_del2, genomic_del2_38_vac):
+    """Create a test fixture for genomic del absolute CNV."""
+    genomic_del2["variation"] = genomic_del2_38_vac
     return VariationDescriptor(**genomic_del2)
 
 
 @pytest.fixture(scope="module")
-def genomic_del2_cx(genomic_del2, genomic_del2_seq_loc):
-    """Create a test fixture for genomic del copy number change."""
+def genomic_del2_vrc(genomic_del2, genomic_del2_seq_loc):
+    """Create a test fixture for genomic del relative CNV."""
     genomic_del2["variation"] = {
-        "type": "CopyNumberChange",
-        "id": "ga4gh:CX.sfbYfDVrJCocGMvSivZAppmAnZ21Sp3-",
-        "subject": genomic_del2_seq_loc,
-        "copy_change": "efo:0030069"
+        "type": "RelativeCopyNumber",
+        "id": "ga4gh:RCN._19twDngCtP3U-8ED2Kly2HM53I_7CV7",
+        "location": genomic_del2_seq_loc,
+        "relative_copy_class": "complete loss"
     }
     return VariationDescriptor(**genomic_del2)
 
 
 @pytest.fixture(scope="module")
 def genomic_del2_rse(genomic_del2, genomic_del2_seq_loc):
     """Create a test fixture for genomic del RSE."""
@@ -1420,18 +1436,19 @@
     return VariationDescriptor(**genomic_del2_free_text)
 
 
 @pytest.fixture(scope="module")
 def genomic_del2_free_text_cnv(genomic_del2_free_text,
                                genomic_del2_free_text_seq_loc):
     """Create a test fixture for genomic del CNV."""
+    _id = "ga4gh:ACN.frpOM82FmXnicV0mpJ7R1oGLzJsGjj8F"
     genomic_del2_free_text["variation"] = {
-        "type": "CopyNumberCount",
-        "id": "ga4gh:CN.4gVfUDeIuWIwLhBU34UrjZWoKbWdG3B7",
-        "subject": genomic_del2_free_text_seq_loc,
+        "type": "AbsoluteCopyNumber",
+        "id": _id,
+        "location": genomic_del2_free_text_seq_loc,
         "copies": {"type": "Number", "value": 1}
     }
     return VariationDescriptor(**genomic_del2_free_text)
 
 
 @pytest.fixture(scope="module")
 def genomic_del2_free_text_rse(genomic_del2_free_text,
@@ -1469,32 +1486,34 @@
         "structural_type": "SO:0001743",
         "vrs_ref_allele_seq": None
     }
     return params
 
 
 @pytest.fixture(scope="module")
-def genomic_del3_cx(genomic_del3, genomic_del3_dup3_loc):
-    """Create a test fixture for genomic del copy number change."""
+def genomic_del3_vrc(genomic_del3, genomic_del3_dup3_loc):
+    """Create a test fixture for genomic del relative cnv."""
+    _id = "ga4gh:RCN.dYerC8FSiqcexo8X1n3XUKpAckoAsfOK"
     genomic_del3["variation"] = {
-        "type": "CopyNumberChange",
-        "id": "ga4gh:CX.XOE1DDGAyMEUeknUAXNHFkt7FKsQBUfh",
-        "subject": genomic_del3_dup3_loc,
-        "copy_change": "efo:0030067"
+        "type": "RelativeCopyNumber",
+        "id": _id,
+        "location": genomic_del3_dup3_loc,
+        "relative_copy_class": "partial loss"
     }
     return VariationDescriptor(**genomic_del3)
 
 
 @pytest.fixture(scope="module")
-def genomic_del3_cn(genomic_del3, genomic_del3_dup3_loc):
-    """Create a test fixture for genomic del copy number count."""
+def genomic_del3_vac(genomic_del3, genomic_del3_dup3_loc):
+    """Create a test fixture for genomic del absolute cnv."""
+    _id = "ga4gh:ACN.2ZUQcccwvtoGZ5LZZRUoDZp6218Y6sQK"
     genomic_del3["variation"] = {
-        "type": "CopyNumberCount",
-        "id": "ga4gh:CN.a2-YlA01Q-y2zAOgn4r-cP9hiIEGaaqq",
-        "subject": genomic_del3_dup3_loc,
+        "type": "AbsoluteCopyNumber",
+        "id": _id,
+        "location": genomic_del3_dup3_loc,
         "copies": {"type": "Number", "value": 2}
     }
     return VariationDescriptor(**genomic_del3)
 
 
 @pytest.fixture(scope="module")
 def genomic_del3_rse_lse(genomic_del3):
@@ -1653,32 +1672,34 @@
         "start": {"min": 68839264, "max": 68839267, "type": "DefiniteRange"},
         "end": {"min": 68841121, "max": 68841126, "type": "DefiniteRange"},
         "type": "SequenceLocation"
     }
 
 
 @pytest.fixture(scope="module")
-def genomic_del3_free_text_cx(genomic_del3_free_text, genomic_del3_free_text_subject):
-    """Create a test fixture for genomic del copy number change."""
+def genomic_del3_free_text_vrc(genomic_del3_free_text, genomic_del3_free_text_subject):
+    """Create a test fixture for genomic del relative cnv."""
+    _id = "ga4gh:RCN.6c0tRlHyFYGSeDEmSyn0nrZJLQDkwVsG"
     genomic_del3_free_text["variation"] = {
-        "type": "CopyNumberChange",
-        "id": "ga4gh:CX.k7s-BiYoxXGlBaGXpqcUdimdsUygemat",
-        "subject": genomic_del3_free_text_subject,
-        "copy_change": "efo:0030067"
+        "type": "RelativeCopyNumber",
+        "id": _id,
+        "location": genomic_del3_free_text_subject,
+        "relative_copy_class": "partial loss"
     }
     return VariationDescriptor(**genomic_del3_free_text)
 
 
 @pytest.fixture(scope="module")
-def genomic_del3_free_text_cn(genomic_del3_free_text, genomic_del3_free_text_subject):
-    """Create a test fixture for genomic del copy number count."""
+def genomic_del3_free_text_vac(genomic_del3_free_text, genomic_del3_free_text_subject):
+    """Create a test fixture for genomic del absolute cnv."""
+    _id = "ga4gh:ACN.ZIaBXgnKLD-AkQhs3W3SMuhMmk80DSlQ"
     genomic_del3_free_text["variation"] = {
-        "type": "CopyNumberCount",
-        "id": "ga4gh:CN.qWnA8lNUMVz8vNKikQ6dWFjdV5E8FJ3U",
-        "subject": genomic_del3_free_text_subject,
+        "type": "AbsoluteCopyNumber",
+        "id": _id,
+        "location": genomic_del3_free_text_subject,
         "copies": {"type": "Number", "value": 2}
     }
     return VariationDescriptor(**genomic_del3_free_text)
 
 
 @pytest.fixture(scope="module")
 def genomic_del3_free_text_rse_lse(genomic_del3_free_text):
@@ -1706,32 +1727,34 @@
         "structural_type": "SO:0001743",
         "vrs_ref_allele_seq": None
     }
     return params
 
 
 @pytest.fixture(scope="module")
-def genomic_del4_cx(genomic_del4, genomic_del4_seq_loc):
-    """Create a test fixture for genomic del copy number change."""
+def genomic_del4_vrc(genomic_del4, genomic_del4_seq_loc):
+    """Create a test fixture for genomic del relative cnv."""
+    _id = "ga4gh:RCN.BwZOFAfo5u8TcwbR3DMi8qbIImv96VQU"
     genomic_del4["variation"] = {
-        "type": "CopyNumberChange",
-        "id": "ga4gh:CX.fYi0dG6Q8kACkyY-ICBzzvslv-ONWrPF",
-        "subject": genomic_del4_seq_loc,
-        "copy_change": "efo:0030067"
+        "type": "RelativeCopyNumber",
+        "id": _id,
+        "location": genomic_del4_seq_loc,
+        "relative_copy_class": "partial loss"
     }
     return VariationDescriptor(**genomic_del4)
 
 
 @pytest.fixture(scope="module")
-def genomic_del4_cn(genomic_del4, genomic_del4_seq_loc):
-    """Create a test fixture for genomic del copy number count."""
+def genomic_del4_vac(genomic_del4, genomic_del4_seq_loc):
+    """Create a test fixture for genomic del absolute cnv."""
+    _id = "ga4gh:ACN.C9lafWMOwiuIc8SbJ3Ie32zYFiJwS9j7"
     genomic_del4["variation"] = {
-        "type": "CopyNumberCount",
-        "id": "ga4gh:CN.vU4Q8TzrKFU3aQvSn2RiRS3ikh58gw_3",
-        "subject": genomic_del4_seq_loc,
+        "type": "AbsoluteCopyNumber",
+        "id": _id,
+        "location": genomic_del4_seq_loc,
         "copies": {"type": "Number", "value": 1}
     }
     return VariationDescriptor(**genomic_del4)
 
 
 @pytest.fixture(scope="module")
 def genomic_del4_rse_lse(genomic_del4):
@@ -1875,32 +1898,34 @@
         "start": {"value": 227022027, "comparator": "<=", "type": "IndefiniteRange"},
         "end": {"value": 227025830, "comparator": ">=", "type": "IndefiniteRange"},
         "type": "SequenceLocation"
     }
 
 
 @pytest.fixture(scope="module")
-def genomic_del4_free_text_cx(genomic_del4_free_text, genomic_del4_free_text_subject):
-    """Create a test fixture for genomic del copy number change."""
+def genomic_del4_free_text_vrc(genomic_del4_free_text, genomic_del4_free_text_subject):
+    """Create a test fixture for genomic del relative cnv."""
+    _id = "ga4gh:RCN.XqfrZ9k9mwDO0cM9duK7ooOih0iR1H2Q"
     genomic_del4_free_text["variation"] = {
-        "type": "CopyNumberChange",
-        "id": "ga4gh:CX.q5LCBF00ZpNiutyADSXuiM0-u1--cHSA",
-        "subject": genomic_del4_free_text_subject,
-        "copy_change": "efo:0030067"
+        "type": "RelativeCopyNumber",
+        "id": _id,
+        "location": genomic_del4_free_text_subject,
+        "relative_copy_class": "partial loss"
     }
     return VariationDescriptor(**genomic_del4_free_text)
 
 
 @pytest.fixture(scope="module")
-def genomic_del4_free_text_cn(genomic_del4_free_text, genomic_del4_free_text_subject):
-    """Create a test fixture for genomic del copy number count."""
+def genomic_del4_free_text_vac(genomic_del4_free_text, genomic_del4_free_text_subject):
+    """Create a test fixture for genomic del absolute cnv."""
+    _id = "ga4gh:ACN.xE7GFDRDsq5DHaRhcJ8xgdC6FYawHoxP"
     genomic_del4_free_text["variation"] = {
-        "type": "CopyNumberCount",
-        "id": "ga4gh:CN.FF3yHxoyJB0JUt9FEeYuKx5vVOUe-w39",
-        "subject": genomic_del4_free_text_subject,
+        "type": "AbsoluteCopyNumber",
+        "id": _id,
+        "location": genomic_del4_free_text_subject,
         "copies": {"type": "Number", "value": 1}
     }
     return VariationDescriptor(**genomic_del4_free_text)
 
 
 @pytest.fixture(scope="module")
 def genomic_del4_free_text_rse_lse(genomic_del4_free_text):
@@ -1920,64 +1945,64 @@
 @pytest.fixture(scope="module")
 def genomic_uncertain_del_2():
     """Create a genomic uncertain deletion on chr 2 test fixture."""
     params = {
         "id": "normalize.variation:NC_000002.12%3Ag.%28%3F_110104900%29_%28110207160_%3F%29del",  # noqa: E501
         "type": "VariationDescriptor",
         "variation": {
-            "id": "ga4gh:CX.0pYLRyzBmiHSiFa_IQqrz8H6iNEYqobh",
-            "subject": {
+            "id": "ga4gh:RCN.7EM-Wsg_7mmAE1LW8cmRI3QwKhJCA24a",
+            "location": {
                 "id": "ga4gh:SL.gUeB872FGVaphqoSAfI0gz4KXJvpZKL_",
                 "sequence_id": "ga4gh:SQ.pnAqCRBrTsUoBghSD1yp_jXWSmlbdh4g",
                 "start": {
                     "value": 110104899,
                     "comparator": "<=",
                     "type": "IndefiniteRange"
                 },
                 "end": {
                     "value": 110207160,
                     "comparator": ">=",
                     "type": "IndefiniteRange"
                 },
                 "type": "SequenceLocation"
             },
-            "copy_change": "efo:0030067",
-            "type": "CopyNumberChange"
+            "relative_copy_class": "partial loss",
+            "type": "RelativeCopyNumber"
         },
         "molecule_context": "genomic",
         "structural_type": "SO:0001743"
     }
     return VariationDescriptor(**params)
 
 
 @pytest.fixture(scope="module")
 def genomic_uncertain_del_y():
     """Create a genomic uncertain deletion on chr Y test fixture."""
     params = {
         "id": "normalize.variation:NC_000024.10%3Ag.%28%3F_14076802%29_%2857165209_%3F%29del",  # noqa: E501
         "type": "VariationDescriptor",
         "variation": {
-            "id": "ga4gh:CX.vcj0GssihvRHGln6RNrWpFnbid70T2Bf",
-            "subject": {
+            "id": "ga4gh:RCN.2q7DKevv8nUh87Sl00Z7l50h047Ti2at",
+            "location": {
                 "id": "ga4gh:SL.ykRzA8IFueiCG7oznnN4teL2nXXBshHV",
                 "sequence_id": "ga4gh:SQ.8_liLu1aycC0tPQPFmUaGXJLDs5SbPZ5",
                 "start": {
                     "value": 14076801,
                     "comparator": "<=",
                     "type": "IndefiniteRange"
                 },
                 "end": {
                     "value": 57165209,
                     "comparator": ">=",
                     "type": "IndefiniteRange"
                 },
                 "type": "SequenceLocation"
             },
-            "copy_change": "efo:0030067",
-            "type": "CopyNumberChange"
+            "relative_copy_class": "partial loss",
+            "type": "RelativeCopyNumber"
         },
         "molecule_context": "genomic",
         "structural_type": "SO:0001743"
     }
     return VariationDescriptor(**params)
 
 
@@ -1991,45 +2016,47 @@
         "molecule_context": "genomic",
         "structural_type": "SO:0001743",
         "vrs_ref_allele_seq": None
     }
     return params
 
 
-def genomic_del5_cn_var(params, genomic_del5_seq_loc):
-    """Create genomic del5 copy number count"""
+def genomic_del5_abs_cnv(params, genomic_del5_seq_loc):
+    """Create genomic del5 absolute cnv"""
+    _id = "ga4gh:ACN.UFPa9YtomnJ00-rlfsQPzc2G05EXgFM3"
     params["variation"] = {
-        "type": "CopyNumberCount",
-        "id": "ga4gh:CN.ZKXhoSguNUA8MBU9SpXmS52FmnZMhgy3",
-        "subject": genomic_del5_seq_loc,
+        "type": "AbsoluteCopyNumber",
+        "id": _id,
+        "location": genomic_del5_seq_loc,
         "copies": {"type": "Number", "value": 3}
     }
 
 
-def genomic_del5_cx_var(params, genomic_del5_seq_loc):
-    """Create genomic del5 copy number change"""
+def genomic_del5_rel_cnv(params, genomic_del5_seq_loc):
+    """Create genomic del5 relative cnv"""
+    _id = "ga4gh:RCN.9rG3a5u3JODwQGVrv1IgAjG6SZgdvraH"
     params["variation"] = {
-        "type": "CopyNumberChange",
-        "id": "ga4gh:CX.0TqknNhM5e5i-5tAKxGXv4yDJlaQgDRR",
-        "subject": genomic_del5_seq_loc,
-        "copy_change": "efo:0030067"
+        "type": "RelativeCopyNumber",
+        "id": _id,
+        "location": genomic_del5_seq_loc,
+        "relative_copy_class": "partial loss"
     }
 
 
 @pytest.fixture(scope="module")
-def genomic_del5_cx(genomic_del5, genomic_del5_seq_loc):
-    """Create a test fixture for genomic del copy number change."""
-    genomic_del5_cx_var(genomic_del5, genomic_del5_seq_loc)
+def genomic_del5_vrc(genomic_del5, genomic_del5_seq_loc):
+    """Create a test fixture for genomic del relative cnv."""
+    genomic_del5_rel_cnv(genomic_del5, genomic_del5_seq_loc)
     return VariationDescriptor(**genomic_del5)
 
 
 @pytest.fixture(scope="module")
-def genomic_del5_cn(genomic_del5, genomic_del5_seq_loc):
-    """Create a test fixture for genomic del copy number count."""
-    genomic_del5_cn_var(genomic_del5, genomic_del5_seq_loc)
+def genomic_del5_vac(genomic_del5, genomic_del5_seq_loc):
+    """Create a test fixture for genomic del absolute cnv."""
+    genomic_del5_abs_cnv(genomic_del5, genomic_del5_seq_loc)
     return VariationDescriptor(**genomic_del5)
 
 
 @pytest.fixture(scope="module")
 def genomic_del5_rse_lse(genomic_del5):
     """Create test fixture for genomic del rse and lse."""
     params = {
@@ -2172,24 +2199,24 @@
             "gene": "hgnc:11411"
         }
     }
     return params
 
 
 @pytest.fixture(scope="module")
-def genomic_del5_free_text_cx(genomic_del5_free_text, genomic_del5_seq_loc):
-    """Create a test fixture for genomic del copy number change."""
-    genomic_del5_cx_var(genomic_del5_free_text, genomic_del5_seq_loc)
+def genomic_del5_free_text_vrc(genomic_del5_free_text, genomic_del5_seq_loc):
+    """Create a test fixture for genomic del relative cnv."""
+    genomic_del5_rel_cnv(genomic_del5_free_text, genomic_del5_seq_loc)
     return VariationDescriptor(**genomic_del5_free_text)
 
 
 @pytest.fixture(scope="module")
-def genomic_del5_free_text_cn(genomic_del5_free_text, genomic_del5_seq_loc):
-    """Create a test fixture for genomic del copy number count."""
-    genomic_del5_cn_var(genomic_del5_free_text, genomic_del5_seq_loc)
+def genomic_del5_free_text_vac(genomic_del5_free_text, genomic_del5_seq_loc):
+    """Create a test fixture for genomic del absolute cnv."""
+    genomic_del5_abs_cnv(genomic_del5_free_text, genomic_del5_seq_loc)
     return VariationDescriptor(**genomic_del5_free_text)
 
 
 @pytest.fixture(scope="module")
 def genomic_del5_free_text_rse_lse(genomic_del5_free_text):
     """Create test fixture for genomic del rse and lse."""
     params = {
@@ -2214,45 +2241,47 @@
         "molecule_context": "genomic",
         "structural_type": "SO:0001743",
         "vrs_ref_allele_seq": None
     }
     return params
 
 
-def genomic_del6_cx_var(params, genomic_del6_seq_loc):
-    """Create genomic del6 copy number change"""
+def genomic_del6_rel_cnv(params, genomic_del6_seq_loc):
+    """Create genomic del6 relative cnv"""
+    _id = "ga4gh:RCN.zsagK87b_RdK4_QZGMnbNl39LCuJUjAr"
     params["variation"] = {
-        "type": "CopyNumberChange",
-        "id": "ga4gh:CX.kzLS3Xs3qhMarky22So-4JW_mZAIhVW2",
-        "subject": genomic_del6_seq_loc,
-        "copy_change": "efo:0030067"
+        "type": "RelativeCopyNumber",
+        "id": _id,
+        "location": genomic_del6_seq_loc,
+        "relative_copy_class": "partial loss"
     }
 
 
-def genomic_del6_cn_var(params, genomic_del6_seq_loc):
-    """Create genomic del6 copy number count"""
+def genomic_del6_abs_cnv(params, genomic_del6_seq_loc):
+    """Create genomic del6 absolute cnv"""
+    _id = "ga4gh:ACN.ZnnJNutwCrHNzFQamAWXMbLC7PfILmqA"
     params["variation"] = {
-        "type": "CopyNumberCount",
-        "id": "ga4gh:CN.lfI0nj_cOjRwul_R_4tohZK_vqiZ-LSz",
-        "subject": genomic_del6_seq_loc,
+        "type": "AbsoluteCopyNumber",
+        "id": _id,
+        "location": genomic_del6_seq_loc,
         "copies": {"type": "Number", "value": 1}
     }
 
 
 @pytest.fixture(scope="module")
-def genomic_del6_cx(genomic_del6, genomic_del6_seq_loc):
-    """Create a test fixture for genomic del copy number change."""
-    genomic_del6_cx_var(genomic_del6, genomic_del6_seq_loc)
+def genomic_del6_vrc(genomic_del6, genomic_del6_seq_loc):
+    """Create a test fixture for genomic del relative cnv."""
+    genomic_del6_rel_cnv(genomic_del6, genomic_del6_seq_loc)
     return VariationDescriptor(**genomic_del6)
 
 
 @pytest.fixture(scope="module")
-def genomic_del6_cn(genomic_del6, genomic_del6_seq_loc):
-    """Create a test fixture for genomic del copy number count."""
-    genomic_del6_cn_var(genomic_del6, genomic_del6_seq_loc)
+def genomic_del6_vac(genomic_del6, genomic_del6_seq_loc):
+    """Create a test fixture for genomic del absolute cnv."""
+    genomic_del6_abs_cnv(genomic_del6, genomic_del6_seq_loc)
     return VariationDescriptor(**genomic_del6)
 
 
 @pytest.fixture(scope="module")
 def genomic_del6_rse_lse(genomic_del6):
     """Create test fixture for genomic del rse and lse."""
     params = {
@@ -2395,24 +2424,24 @@
             "gene": "hgnc:3522"
         }
     }
     return params
 
 
 @pytest.fixture(scope="module")
-def genomic_del6_free_text_cx(genomic_del6_free_text, genomic_del6_seq_loc):
-    """Create a test fixture for genomic del copy number change."""
-    genomic_del6_cx_var(genomic_del6_free_text, genomic_del6_seq_loc)
+def genomic_del6_free_text_vrc(genomic_del6_free_text, genomic_del6_seq_loc):
+    """Create a test fixture for genomic del relative cnv."""
+    genomic_del6_rel_cnv(genomic_del6_free_text, genomic_del6_seq_loc)
     return VariationDescriptor(**genomic_del6_free_text)
 
 
 @pytest.fixture(scope="module")
-def genomic_del6_free_text_cn(genomic_del6_free_text, genomic_del6_seq_loc):
-    """Create a test fixture for genomic del copy number count."""
-    genomic_del6_cn_var(genomic_del6_free_text, genomic_del6_seq_loc)
+def genomic_del6_free_text_vac(genomic_del6_free_text, genomic_del6_seq_loc):
+    """Create a test fixture for genomic del absolute cnv."""
+    genomic_del6_abs_cnv(genomic_del6_free_text, genomic_del6_seq_loc)
     return VariationDescriptor(**genomic_del6_free_text)
 
 
 @pytest.fixture(scope="module")
 def genomic_del6_free_text_rse_lse(genomic_del6_free_text):
     """Create test fixture for genomic del rse and lse."""
     params = {
@@ -2435,51 +2464,51 @@
                                             untranslatable_returns_text=True)
         assert resp.variation_descriptor.label == q.strip()
         assert (resp.variation_descriptor.variation.type == "Text"), q
 
 
 @pytest.mark.asyncio
 async def test_genomic_dup1(test_handler, genomic_dup1_lse,
-                            genomic_dup1_cn, genomic_dup1_cx, genomic_dup1_rse,
+                            genomic_dup1_vac, genomic_dup1_vrc, genomic_dup1_rse,
                             genomic_dup1_free_text_lse,
-                            genomic_dup1_free_text_cn, genomic_dup1_free_text_rse):
+                            genomic_dup1_free_text_vac, genomic_dup1_free_text_rse):
     """Test that genomic duplication works correctly."""
     q = "NC_000003.12:g.49531262dup"  # 38
     resp = await test_handler.normalize(q, "default")
     assertion_checks(resp.variation_descriptor, genomic_dup1_lse, q)
 
     resp = await test_handler.normalize(q, "default")
     assertion_checks(resp.variation_descriptor, genomic_dup1_lse, q)
 
-    resp = await test_handler.normalize(q, "copy_number_count", baseline_copies=2)
-    assertion_checks(resp.variation_descriptor, genomic_dup1_cn, q)
+    resp = await test_handler.normalize(q, "absolute_cnv", baseline_copies=2)
+    assertion_checks(resp.variation_descriptor, genomic_dup1_vac, q)
 
-    resp = await test_handler.normalize(q, "copy_number_change",
-                                        copy_change="efo:0030072")
-    assertion_checks(resp.variation_descriptor, genomic_dup1_cx, q)
+    resp = await test_handler.normalize(q, "relative_cnv",
+                                        relative_copy_class="high-level gain")
+    assertion_checks(resp.variation_descriptor, genomic_dup1_vrc, q)
 
     resp = await test_handler.normalize(q, "repeated_seq_expr")
     assertion_checks(resp.variation_descriptor, genomic_dup1_rse, q)
 
     resp = await test_handler.normalize(q, "literal_seq_expr")
     assertion_checks(resp.variation_descriptor, genomic_dup1_lse, q)
 
     q = "NC_000003.11:g.49568695dup"  # 37
     resp = await test_handler.normalize(q, "default")
     assertion_checks(resp.variation_descriptor, genomic_dup1_lse, q, ignore_id=True)
 
     resp = await test_handler.normalize(q, "default")
     assertion_checks(resp.variation_descriptor, genomic_dup1_lse, q, ignore_id=True)
 
-    resp = await test_handler.normalize(q, "copy_number_count", baseline_copies=2)
-    assertion_checks(resp.variation_descriptor, genomic_dup1_cn, q, ignore_id=True)
+    resp = await test_handler.normalize(q, "absolute_cnv", baseline_copies=2)
+    assertion_checks(resp.variation_descriptor, genomic_dup1_vac, q, ignore_id=True)
 
-    resp = await test_handler.normalize(q, "copy_number_change",
-                                        copy_change="efo:0030072")
-    assertion_checks(resp.variation_descriptor, genomic_dup1_cx, q, ignore_id=True)
+    resp = await test_handler.normalize(q, "relative_cnv",
+                                        relative_copy_class="high-level gain")
+    assertion_checks(resp.variation_descriptor, genomic_dup1_vrc, q, ignore_id=True)
 
     resp = await test_handler.normalize(q, "repeated_seq_expr")
     assertion_checks(resp.variation_descriptor, genomic_dup1_rse, q, ignore_id=True)
 
     resp = await test_handler.normalize(q, "literal_seq_expr")
     assertion_checks(resp.variation_descriptor, genomic_dup1_lse, q, ignore_id=True)
 
@@ -2492,16 +2521,16 @@
         assertion_checks(resp.variation_descriptor, genomic_dup1_free_text_lse, q,
                          ignore_id=True)
 
         resp = await test_handler.normalize(q, "default")
         assertion_checks(resp.variation_descriptor, genomic_dup1_free_text_lse, q,
                          ignore_id=True)
 
-        resp = await test_handler.normalize(q, "copy_number_count", baseline_copies=2)
-        assertion_checks(resp.variation_descriptor, genomic_dup1_free_text_cn, q,
+        resp = await test_handler.normalize(q, "absolute_cnv", baseline_copies=2)
+        assertion_checks(resp.variation_descriptor, genomic_dup1_free_text_vac, q,
                          ignore_id=True)
 
         resp = await test_handler.normalize(q, "repeated_seq_expr")
         assertion_checks(resp.variation_descriptor, genomic_dup1_free_text_rse, q,
                          ignore_id=True)
 
         resp = await test_handler.normalize(q, "literal_seq_expr")
@@ -2514,44 +2543,44 @@
         "NC_000007.14:g.159345976dup",
         "BRAF g.140219337dup", "BRAF g.141024929dup"
     ]
     await assert_text_variation(invalid_queries, test_handler)
 
 
 @pytest.mark.asyncio
-async def test_genomic_dup2(test_handler, genomic_dup2_lse, genomic_dup2_cn,
-                            genomic_dup2_cx, genomic_dup2_rse,
-                            genomic_dup2_free_text_default, genomic_dup2_free_text_cn,
+async def test_genomic_dup2(test_handler, genomic_dup2_lse, genomic_dup2_vac,
+                            genomic_dup2_vrc, genomic_dup2_rse,
+                            genomic_dup2_free_text_default, genomic_dup2_free_text_vac,
                             genomic_dup2_free_text_rse):
     """Test that genomic duplication works correctly."""
     q = "NC_000016.10:g.2087938_2087948dup"  # 38
     resp = await test_handler.normalize(q, "default")
     assertion_checks(resp.variation_descriptor, genomic_dup2_lse, q)
 
-    resp = await test_handler.normalize(q, "copy_number_count", baseline_copies=2)
-    assertion_checks(resp.variation_descriptor, genomic_dup2_cn, q)
+    resp = await test_handler.normalize(q, "absolute_cnv", baseline_copies=2)
+    assertion_checks(resp.variation_descriptor, genomic_dup2_vac, q)
 
-    resp = await test_handler.normalize(q, "copy_number_change")
-    assertion_checks(resp.variation_descriptor, genomic_dup2_cx, q)
+    resp = await test_handler.normalize(q, "relative_cnv")
+    assertion_checks(resp.variation_descriptor, genomic_dup2_vrc, q)
 
     resp = await test_handler.normalize(q, "repeated_seq_expr")
     assertion_checks(resp.variation_descriptor, genomic_dup2_rse, q)
 
     resp = await test_handler.normalize(q, "literal_seq_expr")
     assertion_checks(resp.variation_descriptor, genomic_dup2_lse, q)
 
     q = "NC_000016.9:g.2137939_2137949dup"  # 37
     resp = await test_handler.normalize(q, "default")
     assertion_checks(resp.variation_descriptor, genomic_dup2_lse, q, ignore_id=True)
 
-    resp = await test_handler.normalize(q, "copy_number_count", baseline_copies=2)
-    assertion_checks(resp.variation_descriptor, genomic_dup2_cn, q, ignore_id=True)
+    resp = await test_handler.normalize(q, "absolute_cnv", baseline_copies=2)
+    assertion_checks(resp.variation_descriptor, genomic_dup2_vac, q, ignore_id=True)
 
-    resp = await test_handler.normalize(q, "copy_number_change")
-    assertion_checks(resp.variation_descriptor, genomic_dup2_cx, q, ignore_id=True)
+    resp = await test_handler.normalize(q, "relative_cnv")
+    assertion_checks(resp.variation_descriptor, genomic_dup2_vrc, q, ignore_id=True)
 
     resp = await test_handler.normalize(q, "repeated_seq_expr")
     assertion_checks(resp.variation_descriptor, genomic_dup2_rse, q, ignore_id=True)
 
     resp = await test_handler.normalize(q, "literal_seq_expr")
     assertion_checks(resp.variation_descriptor, genomic_dup2_lse, q, ignore_id=True)
 
@@ -2560,16 +2589,16 @@
         "DMD g.33229407_33229410dup",  # 37
         "DMD g.33211290_33211293dup"  # 38
     ]:
         resp = await test_handler.normalize(q, "default")
         assertion_checks(resp.variation_descriptor, genomic_dup2_free_text_default, q,
                          ignore_id=True)
 
-        resp = await test_handler.normalize(q, "copy_number_count", baseline_copies=2)
-        assertion_checks(resp.variation_descriptor, genomic_dup2_free_text_cn, q,
+        resp = await test_handler.normalize(q, "absolute_cnv", baseline_copies=2)
+        assertion_checks(resp.variation_descriptor, genomic_dup2_free_text_vac, q,
                          ignore_id=True)
 
         resp = await test_handler.normalize(q, "repeated_seq_expr")
         assertion_checks(resp.variation_descriptor, genomic_dup2_free_text_rse, q,
                          ignore_id=True)
 
         resp = await test_handler.normalize(q, "literal_seq_expr")
@@ -2582,50 +2611,47 @@
         "NC_000007.14:g.140413127_159345976dup",
         "BRAF g.140219337_140924929dup", "BRAF g.140719326_141024929dup"
     ]
     await assert_text_variation(invalid_queries, test_handler)
 
 
 @pytest.mark.asyncio
-async def test_genomic_dup3(test_handler, genomic_dup3_cx, genomic_dup3_cn,
-                            genomic_dup3_rse_lse, genomic_dup3_free_text_cn,
-                            genomic_dup3_free_text_cx,
+async def test_genomic_dup3(test_handler, genomic_dup3_vrc, genomic_dup3_vac,
+                            genomic_dup3_rse_lse, genomic_dup3_free_text_vac,
+                            genomic_dup3_free_text_vrc,
                             genomic_dup3_free_text_rse_lse):
     """Test that genomic duplication works correctly."""
     q = "NC_000023.11:g.(31060227_31100351)_(33274278_33417151)dup"  # 38
     resp = await test_handler.normalize(q, "default")
-    assertion_checks(resp.variation_descriptor, genomic_dup3_cx, q)
+    assertion_checks(resp.variation_descriptor, genomic_dup3_vrc, q)
 
-    resp = await test_handler.normalize(q, "copy_number_count", baseline_copies=1)
-    assertion_checks(resp.variation_descriptor, genomic_dup3_cn, q)
+    resp = await test_handler.normalize(q, "absolute_cnv", baseline_copies=1)
+    assertion_checks(resp.variation_descriptor, genomic_dup3_vac, q)
 
-    resp = await test_handler.normalize(q, "copy_number_change",
-                                        copy_change="efo:0030071")
-    test_var = deepcopy(genomic_dup3_cx)
-    test_var.variation.copy_change = "efo:0030071"
-    test_var.variation.id = "ga4gh:CX.ir2HTTvlRlyuUNV6hUfIAbQmQOIbG5xo"
-    assertion_checks(resp.variation_descriptor, test_var, q)
+    resp = await test_handler.normalize(q, "relative_cnv",
+                                        relative_copy_class="low-level gain")
+    assertion_checks(resp.variation_descriptor, genomic_dup3_vrc, q)
 
     resp = await test_handler.normalize(q, "repeated_seq_expr",
                                         untranslatable_returns_text=True)
     assertion_checks(resp.variation_descriptor, genomic_dup3_rse_lse, q)
 
     resp = await test_handler.normalize(q, "literal_seq_expr",
                                         untranslatable_returns_text=True)
     assertion_checks(resp.variation_descriptor, genomic_dup3_rse_lse, q)
 
     q = "NC_000023.10:g.(31078344_31118468)_(33292395_33435268)dup"  # 37
     resp = await test_handler.normalize(q, "default")
-    assertion_checks(resp.variation_descriptor, genomic_dup3_cx, q, ignore_id=True)
+    assertion_checks(resp.variation_descriptor, genomic_dup3_vrc, q, ignore_id=True)
 
-    resp = await test_handler.normalize(q, "copy_number_count", baseline_copies=1)
-    assertion_checks(resp.variation_descriptor, genomic_dup3_cn, q, ignore_id=True)
+    resp = await test_handler.normalize(q, "absolute_cnv", baseline_copies=1)
+    assertion_checks(resp.variation_descriptor, genomic_dup3_vac, q, ignore_id=True)
 
-    resp = await test_handler.normalize(q, "copy_number_change")
-    assertion_checks(resp.variation_descriptor, genomic_dup3_cx, q, ignore_id=True)
+    resp = await test_handler.normalize(q, "relative_cnv")
+    assertion_checks(resp.variation_descriptor, genomic_dup3_vrc, q, ignore_id=True)
 
     genomic_dup3_rse_lse.variation.definition = q
     resp = await test_handler.normalize(q, "repeated_seq_expr",
                                         untranslatable_returns_text=True)
     assertion_checks(resp.variation_descriptor, genomic_dup3_rse_lse, q, ignore_id=True)
 
     resp = await test_handler.normalize(q, "literal_seq_expr",
@@ -2635,19 +2661,19 @@
     # Free Text
     for q in [
         # TODO:  issue-176
         # "DMD g.(31165391_31165395)_(31200854_31200856)dup",
         "DMD g.(31147274_31147278)_(31182737_31182739)dup"  # 38
     ]:
         resp = await test_handler.normalize(q, "default")
-        assertion_checks(resp.variation_descriptor, genomic_dup3_free_text_cx, q,
+        assertion_checks(resp.variation_descriptor, genomic_dup3_free_text_vrc, q,
                          ignore_id=True)
 
-        resp = await test_handler.normalize(q, "copy_number_count", baseline_copies=3)
-        assertion_checks(resp.variation_descriptor, genomic_dup3_free_text_cn, q,
+        resp = await test_handler.normalize(q, "absolute_cnv", baseline_copies=3)
+        assertion_checks(resp.variation_descriptor, genomic_dup3_free_text_vac, q,
                          ignore_id=True)
 
         genomic_dup3_rse_lse.variation.definition = q
         resp = await test_handler.normalize(q, "repeated_seq_expr",
                                             untranslatable_returns_text=True)
         assertion_checks(resp.variation_descriptor, genomic_dup3_free_text_rse_lse, q,
                          ignore_id=True)
@@ -2663,46 +2689,46 @@
         "NC_000023.11:g.(31119221_31119227)_(31119300_156040899)dup",
         "DMD g.(31060227_31100351)_(33274278_33417151)dup"
     ]
     await assert_text_variation(invalid_queries, test_handler)
 
 
 @pytest.mark.asyncio
-async def test_genomic_dup4(test_handler, genomic_dup4_cn, genomic_dup4_cx,
-                            genomic_dup4_rse_lse, genomic_dup4_free_text_cn,
-                            genomic_dup4_free_text_cx,
+async def test_genomic_dup4(test_handler, genomic_dup4_vac, genomic_dup4_vrc,
+                            genomic_dup4_rse_lse, genomic_dup4_free_text_vac,
+                            genomic_dup4_free_text_vrc,
                             genomic_dup4_free_text_rse_lse):
     """Test that genomic duplication works correctly."""
     q = "NC_000020.11:g.(?_30417576)_(31394018_?)dup"  # 38
     resp = await test_handler.normalize(q, "default")
-    assertion_checks(resp.variation_descriptor, genomic_dup4_cx, q)
+    assertion_checks(resp.variation_descriptor, genomic_dup4_vrc, q)
 
-    resp = await test_handler.normalize(q, "copy_number_count", baseline_copies=2)
-    assertion_checks(resp.variation_descriptor, genomic_dup4_cn, q)
+    resp = await test_handler.normalize(q, "absolute_cnv", baseline_copies=2)
+    assertion_checks(resp.variation_descriptor, genomic_dup4_vac, q)
 
-    resp = await test_handler.normalize(q, "copy_number_change")
-    assertion_checks(resp.variation_descriptor, genomic_dup4_cx, q)
+    resp = await test_handler.normalize(q, "relative_cnv")
+    assertion_checks(resp.variation_descriptor, genomic_dup4_vrc, q)
 
     resp = await test_handler.normalize(q, "repeated_seq_expr",
                                         untranslatable_returns_text=True)
     assertion_checks(resp.variation_descriptor, genomic_dup4_rse_lse, q)
 
     resp = await test_handler.normalize(q, "literal_seq_expr",
                                         untranslatable_returns_text=True)
     assertion_checks(resp.variation_descriptor, genomic_dup4_rse_lse, q)
 
     q = "NC_000020.10:g.(?_29652252)_(29981821_?)dup"  # 37
     resp = await test_handler.normalize(q, "default")
-    assertion_checks(resp.variation_descriptor, genomic_dup4_cx, q, ignore_id=True)
+    assertion_checks(resp.variation_descriptor, genomic_dup4_vrc, q, ignore_id=True)
 
-    resp = await test_handler.normalize(q, "copy_number_count", baseline_copies=2)
-    assertion_checks(resp.variation_descriptor, genomic_dup4_cn, q, ignore_id=True)
+    resp = await test_handler.normalize(q, "absolute_cnv", baseline_copies=2)
+    assertion_checks(resp.variation_descriptor, genomic_dup4_vac, q, ignore_id=True)
 
-    resp = await test_handler.normalize(q, "copy_number_change")
-    assertion_checks(resp.variation_descriptor, genomic_dup4_cx, q, ignore_id=True)
+    resp = await test_handler.normalize(q, "relative_cnv")
+    assertion_checks(resp.variation_descriptor, genomic_dup4_vrc, q, ignore_id=True)
 
     genomic_dup4_rse_lse.variation.definition = q
     resp = await test_handler.normalize(q, "repeated_seq_expr",
                                         untranslatable_returns_text=True)
     assertion_checks(resp.variation_descriptor, genomic_dup4_rse_lse, q, ignore_id=True)
 
     resp = await test_handler.normalize(q, "literal_seq_expr",
@@ -2711,19 +2737,19 @@
 
     # Free Text
     for q in [
         "PRPF8 g.(?_1577736)_(1587865_?)dup",  # 37
         "PRPF8 g.(?_1674442)_(1684571_?)dup"  # 38
     ]:
         resp = await test_handler.normalize(q, "default")
-        assertion_checks(resp.variation_descriptor, genomic_dup4_free_text_cx, q,
+        assertion_checks(resp.variation_descriptor, genomic_dup4_free_text_vrc, q,
                          ignore_id=True)
 
-        resp = await test_handler.normalize(q, "copy_number_count", baseline_copies=2)
-        assertion_checks(resp.variation_descriptor, genomic_dup4_free_text_cn, q,
+        resp = await test_handler.normalize(q, "absolute_cnv", baseline_copies=2)
+        assertion_checks(resp.variation_descriptor, genomic_dup4_free_text_vac, q,
                          ignore_id=True)
 
         genomic_dup4_rse_lse.variation.definition = q
         resp = await test_handler.normalize(q, "repeated_seq_expr",
                                             untranslatable_returns_text=True)
         genomic_dup4_free_text_rse_lse.variation.definition = q
         assertion_checks(resp.variation_descriptor, genomic_dup4_free_text_rse_lse, q,
@@ -2740,46 +2766,46 @@
         "NC_000020.11:g.(?_29652252)_(64444169_?)dup",
         "PRPF8 g.(?_1650628)_(1684571_?)dup"
     ]
     await assert_text_variation(invalid_queries, test_handler)
 
 
 @pytest.mark.asyncio
-async def test_genomic_dup5(test_handler, genomic_dup5_cn, genomic_dup5_cx,
-                            genomic_dup5_rse_lse, genomic_dup5_free_text_cn,
-                            genomic_dup5_free_text_cx,
+async def test_genomic_dup5(test_handler, genomic_dup5_vac, genomic_dup5_vrc,
+                            genomic_dup5_rse_lse, genomic_dup5_free_text_vac,
+                            genomic_dup5_free_text_vrc,
                             genomic_dup5_free_text_rse_lse):
     """Test that genomic duplication works correctly."""
     q = "NC_000023.11:g.(?_154021812)_154092209dup"  # 38
     resp = await test_handler.normalize(q, "default")
-    assertion_checks(resp.variation_descriptor, genomic_dup5_cx, q)
+    assertion_checks(resp.variation_descriptor, genomic_dup5_vrc, q)
 
-    resp = await test_handler.normalize(q, "copy_number_count", baseline_copies=2)
-    assertion_checks(resp.variation_descriptor, genomic_dup5_cn, q)
+    resp = await test_handler.normalize(q, "absolute_cnv", baseline_copies=2)
+    assertion_checks(resp.variation_descriptor, genomic_dup5_vac, q)
 
-    resp = await test_handler.normalize(q, "copy_number_change")
-    assertion_checks(resp.variation_descriptor, genomic_dup5_cx, q)
+    resp = await test_handler.normalize(q, "relative_cnv")
+    assertion_checks(resp.variation_descriptor, genomic_dup5_vrc, q)
 
     resp = await test_handler.normalize(q, "repeated_seq_expr",
                                         untranslatable_returns_text=True)
     assertion_checks(resp.variation_descriptor, genomic_dup5_rse_lse, q)
 
     resp = await test_handler.normalize(q, "literal_seq_expr",
                                         untranslatable_returns_text=True)
     assertion_checks(resp.variation_descriptor, genomic_dup5_rse_lse, q)
 
     q = "NC_000023.10:g.(?_153287263)_153357667dup"  # 37
     resp = await test_handler.normalize(q, "default")
-    assertion_checks(resp.variation_descriptor, genomic_dup5_cx, q, ignore_id=True)
+    assertion_checks(resp.variation_descriptor, genomic_dup5_vrc, q, ignore_id=True)
 
-    resp = await test_handler.normalize(q, "copy_number_count", baseline_copies=2)
-    assertion_checks(resp.variation_descriptor, genomic_dup5_cn, q, ignore_id=True)
+    resp = await test_handler.normalize(q, "absolute_cnv", baseline_copies=2)
+    assertion_checks(resp.variation_descriptor, genomic_dup5_vac, q, ignore_id=True)
 
-    resp = await test_handler.normalize(q, "copy_number_change")
-    assertion_checks(resp.variation_descriptor, genomic_dup5_cx, q, ignore_id=True)
+    resp = await test_handler.normalize(q, "relative_cnv")
+    assertion_checks(resp.variation_descriptor, genomic_dup5_vrc, q, ignore_id=True)
 
     genomic_dup5_rse_lse.variation.definition = q
     resp = await test_handler.normalize(q, "repeated_seq_expr",
                                         untranslatable_returns_text=True)
     assertion_checks(resp.variation_descriptor, genomic_dup5_rse_lse, q, ignore_id=True)
 
     resp = await test_handler.normalize(q, "literal_seq_expr",
@@ -2788,19 +2814,19 @@
 
     # Free Text
     for q in [
         "MECP2 g.(?_153287263)_153357667dup",  # 37
         "MECP2 g.(?_154021812)_154092209dup"  # 38
     ]:
         resp = await test_handler.normalize(q, "default")
-        assertion_checks(resp.variation_descriptor, genomic_dup5_free_text_cx, q,
+        assertion_checks(resp.variation_descriptor, genomic_dup5_free_text_vrc, q,
                          ignore_id=True)
 
-        resp = await test_handler.normalize(q, "copy_number_count", baseline_copies=2)
-        assertion_checks(resp.variation_descriptor, genomic_dup5_free_text_cn, q,
+        resp = await test_handler.normalize(q, "absolute_cnv", baseline_copies=2)
+        assertion_checks(resp.variation_descriptor, genomic_dup5_free_text_vac, q,
                          ignore_id=True)
 
         genomic_dup5_free_text_rse_lse.variation.definition = q
         resp = await test_handler.normalize(q, "repeated_seq_expr",
                                             untranslatable_returns_text=True)
         assertion_checks(resp.variation_descriptor, genomic_dup5_free_text_rse_lse, q,
                          ignore_id=True)
@@ -2819,46 +2845,46 @@
     ]:
         resp = await test_handler.normalize(q, "default",
                                             untranslatable_returns_text=True)
         assert resp.variation_descriptor.variation.type == "Text"
 
 
 @pytest.mark.asyncio
-async def test_genomic_dup6(test_handler, genomic_dup6_cn, genomic_dup6_cx,
-                            genomic_dup6_rse_lse, genomic_dup6_free_text_cn,
-                            genomic_dup6_free_text_cx,
+async def test_genomic_dup6(test_handler, genomic_dup6_vac, genomic_dup6_vrc,
+                            genomic_dup6_rse_lse, genomic_dup6_free_text_vac,
+                            genomic_dup6_free_text_vrc,
                             genomic_dup6_free_text_rse_lse):
     """Test that genomic duplication works correctly."""
     q = "NC_000023.11:g.154021812_(154092209_?)dup"  # 38
     resp = await test_handler.normalize(q, "default")
-    assertion_checks(resp.variation_descriptor, genomic_dup6_cx, q)
+    assertion_checks(resp.variation_descriptor, genomic_dup6_vrc, q)
 
-    resp = await test_handler.normalize(q, "copy_number_count", baseline_copies=1)
-    assertion_checks(resp.variation_descriptor, genomic_dup6_cn, q)
+    resp = await test_handler.normalize(q, "absolute_cnv", baseline_copies=1)
+    assertion_checks(resp.variation_descriptor, genomic_dup6_vac, q)
 
-    resp = await test_handler.normalize(q, "copy_number_change")
-    assertion_checks(resp.variation_descriptor, genomic_dup6_cx, q)
+    resp = await test_handler.normalize(q, "relative_cnv")
+    assertion_checks(resp.variation_descriptor, genomic_dup6_vrc, q)
 
     resp = await test_handler.normalize(q, "repeated_seq_expr",
                                         untranslatable_returns_text=True)
     assertion_checks(resp.variation_descriptor, genomic_dup6_rse_lse, q)
 
     resp = await test_handler.normalize(q, "literal_seq_expr",
                                         untranslatable_returns_text=True)
     assertion_checks(resp.variation_descriptor, genomic_dup6_rse_lse, q)
 
     q = "NC_000023.10:g.153287263_(153357667_?)dup"  # 37
     resp = await test_handler.normalize(q, "default")
-    assertion_checks(resp.variation_descriptor, genomic_dup6_cx, q, ignore_id=True)
+    assertion_checks(resp.variation_descriptor, genomic_dup6_vrc, q, ignore_id=True)
 
-    resp = await test_handler.normalize(q, "copy_number_count", baseline_copies=1)
-    assertion_checks(resp.variation_descriptor, genomic_dup6_cn, q, ignore_id=True)
+    resp = await test_handler.normalize(q, "absolute_cnv", baseline_copies=1)
+    assertion_checks(resp.variation_descriptor, genomic_dup6_vac, q, ignore_id=True)
 
-    resp = await test_handler.normalize(q, "copy_number_change")
-    assertion_checks(resp.variation_descriptor, genomic_dup6_cx, q, ignore_id=True)
+    resp = await test_handler.normalize(q, "relative_cnv")
+    assertion_checks(resp.variation_descriptor, genomic_dup6_vrc, q, ignore_id=True)
 
     genomic_dup6_rse_lse.variation.definition = q
     resp = await test_handler.normalize(q, "repeated_seq_expr",
                                         untranslatable_returns_text=True)
     assertion_checks(resp.variation_descriptor, genomic_dup6_rse_lse, q, ignore_id=True)
 
     resp = await test_handler.normalize(q, "literal_seq_expr",
@@ -2867,19 +2893,19 @@
 
     # Free Text
     for q in [
         "MECP2 g.153287263_(153357667_?)dup",  # 37
         "MECP2 g.154021812_(154092209_?)dup"  # 38
     ]:
         resp = await test_handler.normalize(q, "default")
-        assertion_checks(resp.variation_descriptor, genomic_dup6_free_text_cx, q,
+        assertion_checks(resp.variation_descriptor, genomic_dup6_free_text_vrc, q,
                          ignore_id=True)
 
-        resp = await test_handler.normalize(q, "copy_number_count", baseline_copies=1)
-        assertion_checks(resp.variation_descriptor, genomic_dup6_free_text_cn, q,
+        resp = await test_handler.normalize(q, "absolute_cnv", baseline_copies=1)
+        assertion_checks(resp.variation_descriptor, genomic_dup6_free_text_vac, q,
                          ignore_id=True)
 
         genomic_dup6_free_text_rse_lse.variation.definition = q
         resp = await test_handler.normalize(q, "repeated_seq_expr",
                                             untranslatable_returns_text=True)
         assertion_checks(resp.variation_descriptor, genomic_dup6_free_text_rse_lse, q,
                          ignore_id=True)
@@ -2898,46 +2924,46 @@
     ]:
         resp = await test_handler.normalize(q, "default",
                                             untranslatable_returns_text=True)
         assert resp.variation_descriptor.variation.type == "Text"
 
 
 @pytest.mark.asyncio
-async def test_genomic_del1(test_handler, genomic_del1_lse, genomic_del1_cn,
-                            genomic_del1_cx, genomic_del1_rse,
-                            genomic_del1_free_text_lse, genomic_del1_free_text_cn,
+async def test_genomic_del1(test_handler, genomic_del1_lse, genomic_del1_vac,
+                            genomic_del1_vrc, genomic_del1_rse,
+                            genomic_del1_free_text_lse, genomic_del1_free_text_vac,
                             genomic_del1_free_text_rse):
     """Test that genomic deletion works correctly."""
     q = "NC_000003.12:g.10149811del"  # 38
     resp = await test_handler.normalize(q, "default")
     assertion_checks(resp.variation_descriptor, genomic_del1_lse, q)
 
-    resp = await test_handler.normalize(q, "copy_number_count", baseline_copies=2)
-    assertion_checks(resp.variation_descriptor, genomic_del1_cn, q)
+    resp = await test_handler.normalize(q, "absolute_cnv", baseline_copies=2)
+    assertion_checks(resp.variation_descriptor, genomic_del1_vac, q)
 
-    resp = await test_handler.normalize(q, "copy_number_change",
-                                        copy_change="efo:0030067")
-    assertion_checks(resp.variation_descriptor, genomic_del1_cx, q)
+    resp = await test_handler.normalize(q, "relative_cnv",
+                                        relative_copy_class="copy neutral")
+    assertion_checks(resp.variation_descriptor, genomic_del1_vrc, q)
 
     resp = await test_handler.normalize(q, "repeated_seq_expr")
     assertion_checks(resp.variation_descriptor, genomic_del1_rse, q)
 
     resp = await test_handler.normalize(q, "literal_seq_expr")
     assertion_checks(resp.variation_descriptor, genomic_del1_lse, q)
 
     q = "NC_000003.11:g.10191495del"  # 37
     resp = await test_handler.normalize(q, "default")
     assertion_checks(resp.variation_descriptor, genomic_del1_lse, q, ignore_id=True)
 
-    resp = await test_handler.normalize(q, "copy_number_count", baseline_copies=2)
-    assertion_checks(resp.variation_descriptor, genomic_del1_cn, q, ignore_id=True)
+    resp = await test_handler.normalize(q, "absolute_cnv", baseline_copies=2)
+    assertion_checks(resp.variation_descriptor, genomic_del1_vac, q, ignore_id=True)
 
-    resp = await test_handler.normalize(q, "copy_number_change",
-                                        copy_change="efo:0030067")
-    assertion_checks(resp.variation_descriptor, genomic_del1_cx, q, ignore_id=True)
+    resp = await test_handler.normalize(q, "relative_cnv",
+                                        relative_copy_class="copy neutral")
+    assertion_checks(resp.variation_descriptor, genomic_del1_vrc, q, ignore_id=True)
 
     resp = await test_handler.normalize(q, "repeated_seq_expr")
     assertion_checks(resp.variation_descriptor, genomic_del1_rse, q, ignore_id=True)
 
     resp = await test_handler.normalize(q, "literal_seq_expr")
     assertion_checks(resp.variation_descriptor, genomic_del1_lse, q, ignore_id=True)
 
@@ -2946,16 +2972,16 @@
         "VHL g.10191495del",  # 37
         "VHL g.10149811del"  # 38
     ]:
         resp = await test_handler.normalize(q, "default")
         assertion_checks(resp.variation_descriptor, genomic_del1_free_text_lse, q,
                          ignore_id=True)
 
-        resp = await test_handler.normalize(q, "copy_number_count", baseline_copies=2)
-        assertion_checks(resp.variation_descriptor, genomic_del1_free_text_cn, q,
+        resp = await test_handler.normalize(q, "absolute_cnv", baseline_copies=2)
+        assertion_checks(resp.variation_descriptor, genomic_del1_free_text_vac, q,
                          ignore_id=True)
 
         resp = await test_handler.normalize(q, "repeated_seq_expr")
         assertion_checks(resp.variation_descriptor, genomic_del1_free_text_rse, q,
                          ignore_id=True)
 
         resp = await test_handler.normalize(q, "literal_seq_expr")
@@ -2963,15 +2989,15 @@
                          ignore_id=True)
 
     # gnomad vcf
     q = "3-10149810-CT-C"  # 38
     resp = await test_handler.normalize(q)
     assertion_checks(resp.variation_descriptor, genomic_del1_lse, q, ignore_id=True)
 
-    resp = await test_handler.normalize(q, "copy_number_count")
+    resp = await test_handler.normalize(q, "absolute_cnv")
     assertion_checks(resp.variation_descriptor, genomic_del1_lse, q, ignore_id=True)
 
     q = "3-10191494-CT-C"  # 37
     resp = await test_handler.normalize(q)
     assertion_checks(resp.variation_descriptor, genomic_del1_lse, q, ignore_id=True)
 
     resp = await test_handler.normalize(q, "repeated_seq_expr")
@@ -2983,46 +3009,46 @@
         "NC_000003.12:g.198295567del",
         "BRAF g.140413127del", "BRAF g.141024929del"
     ]
     await assert_text_variation(invalid_queries, test_handler)
 
 
 @pytest.mark.asyncio
-async def test_genomic_del2(test_handler, genomic_del2_lse, genomic_del2_cn,
-                            genomic_del2_cx, genomic_del2_rse,
+async def test_genomic_del2(test_handler, genomic_del2_lse, genomic_del2_vac,
+                            genomic_del2_vrc, genomic_del2_rse,
                             genomic_del2_free_text_default, genomic_del2_free_text_cnv,
                             genomic_del2_free_text_rse):
     """Test that genomic deletion works correctly."""
     q = "NC_000003.12:g.10146595_10146613del"  # 38
     resp = await test_handler.normalize(q, "default")
     assertion_checks(resp.variation_descriptor, genomic_del2_lse, q)
 
-    resp = await test_handler.normalize(q, "copy_number_count", baseline_copies=2)
-    assertion_checks(resp.variation_descriptor, genomic_del2_cn, q)
+    resp = await test_handler.normalize(q, "absolute_cnv", baseline_copies=2)
+    assertion_checks(resp.variation_descriptor, genomic_del2_vac, q)
 
-    resp = await test_handler.normalize(q, "copy_number_change",
-                                        copy_change="efo:0030069")
-    assertion_checks(resp.variation_descriptor, genomic_del2_cx, q)
+    resp = await test_handler.normalize(q, "relative_cnv",
+                                        relative_copy_class="complete loss")
+    assertion_checks(resp.variation_descriptor, genomic_del2_vrc, q)
 
     resp = await test_handler.normalize(q, "repeated_seq_expr")
     assertion_checks(resp.variation_descriptor, genomic_del2_rse, q)
 
     resp = await test_handler.normalize(q, "literal_seq_expr")
     assertion_checks(resp.variation_descriptor, genomic_del2_lse, q)
 
     q = "NC_000003.11:g.10188279_10188297del"  # 37
     resp = await test_handler.normalize(q, "default")
     assertion_checks(resp.variation_descriptor, genomic_del2_lse, q, ignore_id=True)
 
-    resp = await test_handler.normalize(q, "copy_number_count", baseline_copies=2)
-    assertion_checks(resp.variation_descriptor, genomic_del2_cn, q, ignore_id=True)
+    resp = await test_handler.normalize(q, "absolute_cnv", baseline_copies=2)
+    assertion_checks(resp.variation_descriptor, genomic_del2_vac, q, ignore_id=True)
 
-    resp = await test_handler.normalize(q, "copy_number_change",
-                                        copy_change="efo:0030069")
-    assertion_checks(resp.variation_descriptor, genomic_del2_cx, q, ignore_id=True)
+    resp = await test_handler.normalize(q, "relative_cnv",
+                                        relative_copy_class="complete loss")
+    assertion_checks(resp.variation_descriptor, genomic_del2_vrc, q, ignore_id=True)
 
     resp = await test_handler.normalize(q, "repeated_seq_expr")
     assertion_checks(resp.variation_descriptor, genomic_del2_rse, q, ignore_id=True)
 
     resp = await test_handler.normalize(q, "literal_seq_expr")
     assertion_checks(resp.variation_descriptor, genomic_del2_lse, q, ignore_id=True)
 
@@ -3031,15 +3057,15 @@
         "VHL g.10188279_10188297del",  # 37
         "VHL g.10146595_10146613del"  # 38
     ]:
         resp = await test_handler.normalize(q, "default")
         assertion_checks(resp.variation_descriptor, genomic_del2_free_text_default, q,
                          ignore_id=True)
 
-        resp = await test_handler.normalize(q, "copy_number_count", baseline_copies=2)
+        resp = await test_handler.normalize(q, "absolute_cnv", baseline_copies=2)
         assertion_checks(resp.variation_descriptor, genomic_del2_free_text_cnv, q,
                          ignore_id=True)
 
         resp = await test_handler.normalize(q, "repeated_seq_expr")
         assertion_checks(resp.variation_descriptor, genomic_del2_free_text_rse, q,
                          ignore_id=True)
 
@@ -3062,46 +3088,46 @@
         "NC_000003.11:g.198022435_198022437del",
         "BRAF g.140413127_140419136del", "BRAF g.140719326_141024929del"
     ]
     await assert_text_variation(invalid_queries, test_handler)
 
 
 @pytest.mark.asyncio
-async def test_genomic_del3(test_handler, genomic_del3_cn, genomic_del3_cx,
-                            genomic_del3_rse_lse, genomic_del3_free_text_cn,
-                            genomic_del3_free_text_cx,
+async def test_genomic_del3(test_handler, genomic_del3_vac, genomic_del3_vrc,
+                            genomic_del3_rse_lse, genomic_del3_free_text_vac,
+                            genomic_del3_free_text_vrc,
                             genomic_del3_free_text_rse_lse):
     """Test that genomic deletion works correctly."""
     q = "NC_000023.11:g.(31060227_31100351)_(33274278_33417151)del"  # 38
     resp = await test_handler.normalize(q, "default")
-    assertion_checks(resp.variation_descriptor, genomic_del3_cx, q)
+    assertion_checks(resp.variation_descriptor, genomic_del3_vrc, q)
 
-    resp = await test_handler.normalize(q, "copy_number_count", baseline_copies=3)
-    assertion_checks(resp.variation_descriptor, genomic_del3_cn, q)
+    resp = await test_handler.normalize(q, "absolute_cnv", baseline_copies=3)
+    assertion_checks(resp.variation_descriptor, genomic_del3_vac, q)
 
-    resp = await test_handler.normalize(q, "copy_number_change")
-    assertion_checks(resp.variation_descriptor, genomic_del3_cx, q)
+    resp = await test_handler.normalize(q, "relative_cnv")
+    assertion_checks(resp.variation_descriptor, genomic_del3_vrc, q)
 
     resp = await test_handler.normalize(q, "repeated_seq_expr",
                                         untranslatable_returns_text=True)
     assertion_checks(resp.variation_descriptor, genomic_del3_rse_lse, q)
 
     resp = await test_handler.normalize(q, "literal_seq_expr",
                                         untranslatable_returns_text=True)
     assertion_checks(resp.variation_descriptor, genomic_del3_rse_lse, q)
 
     q = "NC_000023.10:g.(31078344_31118468)_(33292395_33435268)del"  # 37
     resp = await test_handler.normalize(q, "default")
-    assertion_checks(resp.variation_descriptor, genomic_del3_cx, q, ignore_id=True)
+    assertion_checks(resp.variation_descriptor, genomic_del3_vrc, q, ignore_id=True)
 
-    resp = await test_handler.normalize(q, "copy_number_count", baseline_copies=3)
-    assertion_checks(resp.variation_descriptor, genomic_del3_cn, q, ignore_id=True)
+    resp = await test_handler.normalize(q, "absolute_cnv", baseline_copies=3)
+    assertion_checks(resp.variation_descriptor, genomic_del3_vac, q, ignore_id=True)
 
-    resp = await test_handler.normalize(q, "copy_number_change")
-    assertion_checks(resp.variation_descriptor, genomic_del3_cx, q, ignore_id=True)
+    resp = await test_handler.normalize(q, "relative_cnv")
+    assertion_checks(resp.variation_descriptor, genomic_del3_vrc, q, ignore_id=True)
 
     genomic_del3_rse_lse.variation.definition = q
     resp = await test_handler.normalize(q, "repeated_seq_expr",
                                         untranslatable_returns_text=True)
     assertion_checks(resp.variation_descriptor, genomic_del3_rse_lse, q, ignore_id=True)
 
     resp = await test_handler.normalize(q, "literal_seq_expr",
@@ -3110,19 +3136,19 @@
 
     # Free Text
     for q in [
         "EFNB1 g.(68059108_68059111)_(68060963_68060968)del",  # 37
         "EFNB1 g.(68839265_68839268)_(68841120_68841125)del"  # 38
     ]:
         resp = await test_handler.normalize(q, "default")
-        assertion_checks(resp.variation_descriptor, genomic_del3_free_text_cx, q,
+        assertion_checks(resp.variation_descriptor, genomic_del3_free_text_vrc, q,
                          ignore_id=True)
 
-        resp = await test_handler.normalize(q, "copy_number_count", baseline_copies=3)
-        assertion_checks(resp.variation_descriptor, genomic_del3_free_text_cn, q,
+        resp = await test_handler.normalize(q, "absolute_cnv", baseline_copies=3)
+        assertion_checks(resp.variation_descriptor, genomic_del3_free_text_vac, q,
                          ignore_id=True)
 
         genomic_del3_free_text_rse_lse.variation.definition = q
         resp = await test_handler.normalize(q, "repeated_seq_expr",
                                             untranslatable_returns_text=True)
         assertion_checks(resp.variation_descriptor, genomic_del3_free_text_rse_lse, q,
                          ignore_id=True)
@@ -3139,46 +3165,46 @@
         "EFNB1 g.(68048863_68048870)_(68842150_68842152)del",  # 37
         "EFNB1 g.(68829022_68829030)_(68842150_68842161)del"  # 38
     ]
     await assert_text_variation(invalid_queries, test_handler)
 
 
 @pytest.mark.asyncio
-async def test_genomic_del4(test_handler, genomic_del4_cn, genomic_del4_cx,
+async def test_genomic_del4(test_handler, genomic_del4_vac, genomic_del4_vrc,
                             genomic_del4_rse_lse, genomic_uncertain_del_2,
-                            genomic_uncertain_del_y, genomic_del4_free_text_cn,
-                            genomic_del4_free_text_rse_lse, genomic_del4_free_text_cx):
+                            genomic_uncertain_del_y, genomic_del4_free_text_vac,
+                            genomic_del4_free_text_rse_lse, genomic_del4_free_text_vrc):
     """Test that genomic deletion works correctly."""
     q = "NC_000023.11:g.(?_31120496)_(33339477_?)del"  # 38
     resp = await test_handler.normalize(q, "default")
-    assertion_checks(resp.variation_descriptor, genomic_del4_cx, q)
+    assertion_checks(resp.variation_descriptor, genomic_del4_vrc, q)
 
-    resp = await test_handler.normalize(q, "copy_number_count", baseline_copies=2)
-    assertion_checks(resp.variation_descriptor, genomic_del4_cn, q)
+    resp = await test_handler.normalize(q, "absolute_cnv", baseline_copies=2)
+    assertion_checks(resp.variation_descriptor, genomic_del4_vac, q)
 
-    resp = await test_handler.normalize(q, "copy_number_change")
-    assertion_checks(resp.variation_descriptor, genomic_del4_cx, q)
+    resp = await test_handler.normalize(q, "relative_cnv")
+    assertion_checks(resp.variation_descriptor, genomic_del4_vrc, q)
 
     resp = await test_handler.normalize(q, "repeated_seq_expr",
                                         untranslatable_returns_text=True)
     assertion_checks(resp.variation_descriptor, genomic_del4_rse_lse, q)
 
     resp = await test_handler.normalize(q, "literal_seq_expr",
                                         untranslatable_returns_text=True)
     assertion_checks(resp.variation_descriptor, genomic_del4_rse_lse, q)
 
     q = "NC_000023.10:g.(?_31138613)_(33357594_?)del"  # 37
     resp = await test_handler.normalize(q, "default")
-    assertion_checks(resp.variation_descriptor, genomic_del4_cx, q, ignore_id=True)
+    assertion_checks(resp.variation_descriptor, genomic_del4_vrc, q, ignore_id=True)
 
-    resp = await test_handler.normalize(q, "copy_number_count", baseline_copies=2)
-    assertion_checks(resp.variation_descriptor, genomic_del4_cn, q, ignore_id=True)
+    resp = await test_handler.normalize(q, "absolute_cnv", baseline_copies=2)
+    assertion_checks(resp.variation_descriptor, genomic_del4_vac, q, ignore_id=True)
 
-    resp = await test_handler.normalize(q, "copy_number_change")
-    assertion_checks(resp.variation_descriptor, genomic_del4_cx, q, ignore_id=True)
+    resp = await test_handler.normalize(q, "relative_cnv")
+    assertion_checks(resp.variation_descriptor, genomic_del4_vrc, q, ignore_id=True)
 
     genomic_del4_rse_lse.variation.definition = q
     resp = await test_handler.normalize(q, "repeated_seq_expr",
                                         untranslatable_returns_text=True)
     assertion_checks(resp.variation_descriptor, genomic_del4_rse_lse, q, ignore_id=True)
 
     resp = await test_handler.normalize(q, "literal_seq_expr",
@@ -3196,19 +3222,19 @@
     # Free Text
     for q in [
         # TODO:  issue-176
         # "COL4A4 g.(?_227886744)_(227890546_?)del",  # 37
         "COL4A4 g.(?_227022028)_(227025830_?)del"  # 38
     ]:
         resp = await test_handler.normalize(q, "default")
-        assertion_checks(resp.variation_descriptor, genomic_del4_free_text_cx, q,
+        assertion_checks(resp.variation_descriptor, genomic_del4_free_text_vrc, q,
                          ignore_id=True)
 
-        resp = await test_handler.normalize(q, "copy_number_count", baseline_copies=2)
-        assertion_checks(resp.variation_descriptor, genomic_del4_free_text_cn, q,
+        resp = await test_handler.normalize(q, "absolute_cnv", baseline_copies=2)
+        assertion_checks(resp.variation_descriptor, genomic_del4_free_text_vac, q,
                          ignore_id=True)
 
         resp = await test_handler.normalize(q, "repeated_seq_expr",
                                             untranslatable_returns_text=True)
         assertion_checks(resp.variation_descriptor, genomic_del4_free_text_rse_lse, q,
                          ignore_id=True)
 
@@ -3224,46 +3250,46 @@
         "COL4A4 g.(?_227002710)_(227003710_?)del",
         "COL4A4 g.(?_227867430)_(228029276_?)del",
     ]
     await assert_text_variation(invalid_queries, test_handler)
 
 
 @pytest.mark.asyncio
-async def test_genomic_del5(test_handler, genomic_del5_cn, genomic_del5_cx,
-                            genomic_del5_rse_lse, genomic_del5_free_text_cn,
-                            genomic_del5_free_text_cx,
+async def test_genomic_del5(test_handler, genomic_del5_vac, genomic_del5_vrc,
+                            genomic_del5_rse_lse, genomic_del5_free_text_vac,
+                            genomic_del5_free_text_vrc,
                             genomic_del5_free_text_rse_lse):
     """Test that genomic deletion works correctly."""
     q = "NC_000023.11:g.(?_18575354)_18653629del"  # 38
     resp = await test_handler.normalize(q, "default")
-    assertion_checks(resp.variation_descriptor, genomic_del5_cx, q)
+    assertion_checks(resp.variation_descriptor, genomic_del5_vrc, q)
 
-    resp = await test_handler.normalize(q, "copy_number_count", baseline_copies=4)
-    assertion_checks(resp.variation_descriptor, genomic_del5_cn, q)
+    resp = await test_handler.normalize(q, "absolute_cnv", baseline_copies=4)
+    assertion_checks(resp.variation_descriptor, genomic_del5_vac, q)
 
-    resp = await test_handler.normalize(q, "copy_number_change")
-    assertion_checks(resp.variation_descriptor, genomic_del5_cx, q)
+    resp = await test_handler.normalize(q, "relative_cnv")
+    assertion_checks(resp.variation_descriptor, genomic_del5_vrc, q)
 
     resp = await test_handler.normalize(q, "repeated_seq_expr",
                                         untranslatable_returns_text=True)
     assertion_checks(resp.variation_descriptor, genomic_del5_rse_lse, q)
 
     resp = await test_handler.normalize(q, "literal_seq_expr",
                                         untranslatable_returns_text=True)
     assertion_checks(resp.variation_descriptor, genomic_del5_rse_lse, q)
 
     q = "NC_000023.10:g.(?_18593474)_18671749del"  # 37
     resp = await test_handler.normalize(q, "default")
-    assertion_checks(resp.variation_descriptor, genomic_del5_cx, q, ignore_id=True)
+    assertion_checks(resp.variation_descriptor, genomic_del5_vrc, q, ignore_id=True)
 
-    resp = await test_handler.normalize(q, "copy_number_count", baseline_copies=4)
-    assertion_checks(resp.variation_descriptor, genomic_del5_cn, q, ignore_id=True)
+    resp = await test_handler.normalize(q, "absolute_cnv", baseline_copies=4)
+    assertion_checks(resp.variation_descriptor, genomic_del5_vac, q, ignore_id=True)
 
-    resp = await test_handler.normalize(q, "copy_number_change")
-    assertion_checks(resp.variation_descriptor, genomic_del5_cx, q, ignore_id=True)
+    resp = await test_handler.normalize(q, "relative_cnv")
+    assertion_checks(resp.variation_descriptor, genomic_del5_vrc, q, ignore_id=True)
 
     genomic_del5_rse_lse.variation.definition = q
     resp = await test_handler.normalize(q, "repeated_seq_expr",
                                         untranslatable_returns_text=True)
     assertion_checks(resp.variation_descriptor, genomic_del5_rse_lse, q, ignore_id=True)
 
     resp = await test_handler.normalize(q, "literal_seq_expr",
@@ -3273,19 +3299,19 @@
     # Free text
     for q in [
         # TODO:  issue-176
         # "CDKL5 g.(?_18593474)_18671749del",
         "CDKL5 g.(?_18575354)_18653629del"
     ]:
         resp = await test_handler.normalize(q, "default")
-        assertion_checks(resp.variation_descriptor, genomic_del5_free_text_cx, q,
+        assertion_checks(resp.variation_descriptor, genomic_del5_free_text_vrc, q,
                          ignore_id=True)
 
-        resp = await test_handler.normalize(q, "copy_number_count", baseline_copies=4)
-        assertion_checks(resp.variation_descriptor, genomic_del5_free_text_cn, q,
+        resp = await test_handler.normalize(q, "absolute_cnv", baseline_copies=4)
+        assertion_checks(resp.variation_descriptor, genomic_del5_free_text_vac, q,
                          ignore_id=True)
 
         genomic_del5_free_text_rse_lse.variation.definition = q
         resp = await test_handler.normalize(q, "repeated_seq_expr",
                                             untranslatable_returns_text=True)
         assertion_checks(resp.variation_descriptor, genomic_del5_free_text_rse_lse, q,
                          ignore_id=True)
@@ -3303,46 +3329,46 @@
         "CDKL5  g.(?_18425585)_18653631del",  # 38
         "CDKL5  g.(?_18425582)_18653500del"  # 38
     ]
     await assert_text_variation(invalid_queries, test_handler)
 
 
 @pytest.mark.asyncio
-async def test_genomic_del6(test_handler, genomic_del6_cn, genomic_del6_cx,
-                            genomic_del6_rse_lse, genomic_del6_free_text_cn,
-                            genomic_del6_free_text_cx,
+async def test_genomic_del6(test_handler, genomic_del6_vac, genomic_del6_vrc,
+                            genomic_del6_rse_lse, genomic_del6_free_text_vac,
+                            genomic_del6_free_text_vrc,
                             genomic_del6_free_text_rse_lse):
     """Test that genomic deletion works correctly."""
     q = "NC_000006.12:g.133462764_(133464858_?)del"  # 38
     resp = await test_handler.normalize(q, "default")
-    assertion_checks(resp.variation_descriptor, genomic_del6_cx, q)
+    assertion_checks(resp.variation_descriptor, genomic_del6_vrc, q)
 
-    resp = await test_handler.normalize(q, "copy_number_count", baseline_copies=2)
-    assertion_checks(resp.variation_descriptor, genomic_del6_cn, q)
+    resp = await test_handler.normalize(q, "absolute_cnv", baseline_copies=2)
+    assertion_checks(resp.variation_descriptor, genomic_del6_vac, q)
 
-    resp = await test_handler.normalize(q, "copy_number_change")
-    assertion_checks(resp.variation_descriptor, genomic_del6_cx, q)
+    resp = await test_handler.normalize(q, "relative_cnv")
+    assertion_checks(resp.variation_descriptor, genomic_del6_vrc, q)
 
     resp = await test_handler.normalize(q, "repeated_seq_expr",
                                         untranslatable_returns_text=True)
     assertion_checks(resp.variation_descriptor, genomic_del6_rse_lse, q)
 
     resp = await test_handler.normalize(q, "literal_seq_expr",
                                         untranslatable_returns_text=True)
     assertion_checks(resp.variation_descriptor, genomic_del6_rse_lse, q)
 
     q = "NC_000006.11:g.133783902_(133785996_?)del"  # 37
     resp = await test_handler.normalize(q, "default")
-    assertion_checks(resp.variation_descriptor, genomic_del6_cx, q, ignore_id=True)
+    assertion_checks(resp.variation_descriptor, genomic_del6_vrc, q, ignore_id=True)
 
-    resp = await test_handler.normalize(q, "copy_number_count", baseline_copies=2)
-    assertion_checks(resp.variation_descriptor, genomic_del6_cn, q, ignore_id=True)
+    resp = await test_handler.normalize(q, "absolute_cnv", baseline_copies=2)
+    assertion_checks(resp.variation_descriptor, genomic_del6_vac, q, ignore_id=True)
 
-    resp = await test_handler.normalize(q, "copy_number_change")
-    assertion_checks(resp.variation_descriptor, genomic_del6_cx, q, ignore_id=True)
+    resp = await test_handler.normalize(q, "relative_cnv")
+    assertion_checks(resp.variation_descriptor, genomic_del6_vrc, q, ignore_id=True)
 
     genomic_del6_rse_lse.variation.definition = q
     resp = await test_handler.normalize(q, "repeated_seq_expr",
                                         untranslatable_returns_text=True)
     assertion_checks(resp.variation_descriptor, genomic_del6_rse_lse, q, ignore_id=True)
 
     resp = await test_handler.normalize(q, "literal_seq_expr",
@@ -3352,19 +3378,19 @@
     # Free text
     for q in [
         # TODO:  issue-176
         # "EYA4 g.133783902_(133785996_?)del",  # 37
         "EYA4 g.133462764_(133464858_?)del"  # 38
     ]:
         resp = await test_handler.normalize(q, "default")
-        assertion_checks(resp.variation_descriptor, genomic_del6_free_text_cx, q,
+        assertion_checks(resp.variation_descriptor, genomic_del6_free_text_vrc, q,
                          ignore_id=True)
 
-        resp = await test_handler.normalize(q, "copy_number_count", baseline_copies=2)
-        assertion_checks(resp.variation_descriptor, genomic_del6_free_text_cn, q,
+        resp = await test_handler.normalize(q, "absolute_cnv", baseline_copies=2)
+        assertion_checks(resp.variation_descriptor, genomic_del6_free_text_vac, q,
                          ignore_id=True)
 
         genomic_del6_rse_lse.variation.definition = q
         resp = await test_handler.normalize(q, "repeated_seq_expr",
                                             untranslatable_returns_text=True)
         assertion_checks(resp.variation_descriptor, genomic_del6_free_text_rse_lse, q,
                          ignore_id=True)
@@ -3398,18 +3424,18 @@
     assert resp.variation_descriptor
     assert resp.warnings == []
 
     resp = await test_handler.normalize(q, None)
     assert resp.variation_descriptor
     assert resp.warnings == []
 
-    resp = await test_handler.normalize(q, " copy_Number_Count ", baseline_copies=2)
+    resp = await test_handler.normalize(q, " absolute_CnV ", baseline_copies=2)
     assert resp.variation_descriptor
     assert resp.warnings == []
 
-    resp = await test_handler.normalize(q, " copy_Number_Count ")
+    resp = await test_handler.normalize(q, " absolute_CnV ")
     assert resp.variation_descriptor is None
-    assert resp.warnings == ["copy_number_count mode requires `baseline_copies`"]
+    assert resp.warnings == ["absolute_cnv mode requires `baseline_copies`"]
 
-    resp = await test_handler.normalize(q, " copy_Number_Change ")
+    resp = await test_handler.normalize(q, " relative_CnV ")
     assert resp.variation_descriptor
     assert resp.warnings == []
```

### Comparing `variation-normalizer-0.7.0.dev7/tests/test_normalize.py` & `variation-normalizer-0.7.dev0/tests/test_normalize.py`

 * *Files 2% similar despite different names*

```diff
@@ -514,44 +514,14 @@
         "vrs_ref_allele_seq": "TTGAGGGAAAACACAT",
         "gene_context": erbb2_context
     }
     return VariationDescriptor(**params)
 
 
 @pytest.fixture(scope="module")
-def genomic_deletion():
-    """Create test fixture for genomic deletion range with deleted sequence.
-    (CA915940709)
-    """
-    params = {
-        "id": "normalize.variation:NC_000003.12%3Ag.10146527_10146528del",
-        "type": "VariationDescriptor",
-        "variation": {
-            "id": "ga4gh:VA.AoFRR6KWkw6_YfrGAxGkT9SJsXieSk93",
-            "location": {
-                "id": "ga4gh:SL.6D7Wbq7XOvga3y-057BKIra4g9RgAFy9",
-                "end": {"value": 10146528, "type": "Number"},
-                "start": {"value": 10146524, "type": "Number"},
-                "sequence_id": "ga4gh:SQ.Zu7h9AggXxhTaGVsy7h_EZSChSZGcmgX",
-                "type": "SequenceLocation"
-            },
-            "state": {
-                "sequence": "CT",
-                "type": "LiteralSequenceExpression"
-            },
-            "type": "Allele"
-        },
-        "molecule_context": "genomic",
-        "structural_type": "SO:0000159",
-        "vrs_ref_allele_seq": "CTCT"
-    }
-    return VariationDescriptor(**params)
-
-
-@pytest.fixture(scope="module")
 def coding_dna_insertion(limk2_gene_context):
     """Create test fixture for coding DNA insertion."""
     params = {
         "id": "normalize.variation:ENST00000331728.9%3Ac.2049_2050insA",
         "type": "VariationDescriptor",
         "variation": {
             "id": "ga4gh:VA.NuvjUrfrwALQWlI0qkWEiv4IngxNZO8f",
@@ -693,16 +663,16 @@
 @pytest.fixture(scope="module")
 def genomic_uncertain_del_x():
     """Create a genomic uncertain deletion on chr X test fixture."""
     params = {
         "id": "normalize.variation:NC_000023.11%3Ag.%28%3F_31120496%29_%2833339477_%3F%29del",  # noqa: E501
         "type": "VariationDescriptor",
         "variation": {
-            "id": "ga4gh:CN.GrUeefilHb49CXKX7Noidga41FQnR_qT",
-            "subject": {
+            "id": "ga4gh:ACN.gT8vZlUghIFxFv-ztGpOQirOGgwjyvjW",
+            "location": {
                 "id": "ga4gh:SL.dRc1d9ymsXhbb439OQE830RBELZ4aMXi",
                 "sequence_id": "ga4gh:SQ.w0WZEvgJF0zf_P4yyTzjjv9oW1z61HHP",
                 "start": {
                     "value": 31120495,
                     "comparator": "<=",
                     "type": "IndefiniteRange"
                 },
@@ -714,15 +684,15 @@
                 "type": "SequenceLocation"
             },
             "copies": {
                 "min": 0,
                 "max": 1,
                 "type": "DefiniteRange"
             },
-            "type": "CopyNumberCount"
+            "type": "AbsoluteCopyNumber"
         },
         "molecule_context": "genomic",
         "structural_type": "SO:0001743"
     }
     return VariationDescriptor(**params)
 
 
@@ -1113,66 +1083,33 @@
     assert resp.variation_descriptor.id == \
         "normalize.variation:ERBB2%20Leu755_Thr759del"
     resp.variation_descriptor.id = \
         "normalize.variation:NP_004439.2%3Ap.Leu755_Thr759del"
     assertion_checks(resp.variation_descriptor, protein_deletion_np_range,
                      "ERBB2 Leu755_Thr759del")
 
-    resp1 = await test_handler.normalize("EGFR L747_T751del")
-    resp2 = await test_handler.normalize("EGFR L747_T751delLREAT")
-    assert resp1.variation_descriptor.variation.id == \
-        resp2.variation_descriptor.variation.id
-
-    # incorrect deleted sequence
-    resp = await test_handler.normalize("EGFR L747_T751delLREA")
-    assert not resp.variation_descriptor
-
 
 @pytest.mark.asyncio
 async def test_coding_dna_deletion(test_handler, coding_dna_deletion):
     """Test that coding dna deletion normalizes correctly."""
     # https://reg.clinicalgenome.org/redmine/projects/registry/genboree_registry/by_caid?caid=CA645372623  # noqa: E501
     q = "NM_004448.3:c.2264_2278delTGAGGGAAAACACAT"
-    resp1 = await test_handler.normalize(q)
-    assertion_checks(resp1.variation_descriptor, coding_dna_deletion, q)
-
-    # incorrected deleted sequence
-    resp = await test_handler.normalize("NM_004448.3:c.2264_2278delTGAGGGAAAACACTA")
-    assert not resp.variation_descriptor
-
-    resp2 = await test_handler.normalize("NM_004448.3:c.2264_2278del")
-    assert resp1.variation_descriptor.variation.id == resp2.variation_descriptor.variation.id  # noqa: E501
+    resp = await test_handler.normalize(q)
+    assertion_checks(resp.variation_descriptor, coding_dna_deletion, q)
 
     q = "ERBB2 c.2264_2278delTGAGGGAAAACACAT"
     resp = await test_handler.normalize(q)
     assert resp.variation_descriptor.id == \
            "normalize.variation:ERBB2%20c.2264_2278delTGAGGGAAAACACAT"
     resp.variation_descriptor.id = \
         "normalize.variation:NM_004448.3%3Ac.2264_2278delTGAGGGAAAACACAT"
     assertion_checks(resp.variation_descriptor, coding_dna_deletion, q)
 
 
 @pytest.mark.asyncio
-async def test_genomic_deletion(test_handler, genomic_deletion):
-    """Test that genomic deletion normalizes correctly"""
-    # CA915940709
-    q = "NC_000003.12:g.10146527_10146528del"
-    resp1 = await test_handler.normalize(q)
-    assertion_checks(resp1.variation_descriptor, genomic_deletion, q)
-
-    resp2 = await test_handler.normalize("NC_000003.12:g.10146527_10146528delCT")
-    assert resp1.variation_descriptor.variation.id == \
-        resp2.variation_descriptor.variation.id
-
-    # incorrect deleted sequence
-    resp = await test_handler.normalize("NC_000003.12:g.10146527_10146528delCC")
-    assert not resp.variation_descriptor
-
-
-@pytest.mark.asyncio
 async def test_protein_insertion(test_handler, protein_insertion):
     """Test that protein insertion normalizes correctly."""
     resp = await test_handler.normalize("NP_005219.2:p.Asp770_Asn771insGlyLeu")
     assertion_checks(resp.variation_descriptor, protein_insertion,
                      "NP_005219.2:p.Asp770_Asn771insGlyLeu")
 
     def change_resp(response):
@@ -1273,29 +1210,14 @@
 
     resp = await test_handler.normalize("NC_000002.12:g.73448098_73448100delCTC")
     assert resp
     assert resp.variation_descriptor.variation.state.sequence == "CTC"
     assert resp.variation_descriptor.variation.id == \
         "ga4gh:VA.M0oqztcpIsGcwxeOfxR32Q9_2Xvpu4BE"
 
-    resp = await test_handler.normalize("NG_008212.3:g.5426_5445del")
-    assert resp.variation_descriptor
-
-    # Test ambiguous IUPAC code N
-    for q in [
-        "NC_000017.10:g.7572948_7572949insTTTTTTTTTNNNNN",
-        "NC_000007.13:g.140453136A>N",
-        "NC_000007.13:g.140453135_140453136delinsATN",
-        "NM_007294.3:c.2902_2903insTCN",
-        "NM_004333.4:c.1799T>N",
-        "NM_001289937.1:c.2326_2327delinsCTN"
-    ]:
-        resp = await test_handler.normalize(q)
-        assert resp.variation_descriptor, q
-
 
 @pytest.mark.asyncio
 async def test_no_matches(test_handler):
     """Test no matches work correctly."""
     queries = [
         "braf", "braf v600000932092039e", "NP_000213.1:cp.Leu862=",
         "NP_000213.1:cp.Leu862", "BRAF V600E 33", "NP_004324.2:p.Glu600Val",
```

### Comparing `variation-normalizer-0.7.0.dev7/tests/test_to_canonical_variation.py` & `variation-normalizer-0.7.dev0/tests/test_to_canonical_variation.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     }
 
 
 @pytest.fixture(scope="module")
 def variation1_lse(variation1_seq_loc):
     """Create test fixture for NC_000013.11:20189346:GGG:GG"""
     params = {
-        "id": "ga4gh:CAN.tg0nG9q1DMP_J-vcWiaASPW44GMEh47k",
+        "id": "ga4gh:CLV.tg0nG9q1DMP_J-vcWiaASPW44GMEh47k",
         "type": "CanonicalVariation",
         "canonical_context": {
             "id": "ga4gh:VA.jkAILAe4dK4tQ3y2hz-GHtZRAnbVC__T",
             "type": "Allele",
             "location": variation1_seq_loc,
             "state": {
                 "type": "LiteralSequenceExpression",
@@ -43,15 +43,15 @@
     return CanonicalVariation(**params)
 
 
 @pytest.fixture(scope="module")
 def variation_del_lse():
     """Create test fixture for NC_000013.11:20003096:C:"""
     params = {
-        "id": "ga4gh:CAN.6_wBT_bhV-hwjaqDxq3kEs3nyILkF4du",
+        "id": "ga4gh:CLV.6_wBT_bhV-hwjaqDxq3kEs3nyILkF4du",
         "type": "CanonicalVariation",
         "canonical_context": {
             "id": "ga4gh:VA.l55oQYOlWUoYwAxb4trpbqmMNaknTa1U",
             "type": "Allele",
             "location": {
                 "id": "ga4gh:SL.aEhVhpZMgXXidD4yA4wQbqxKPAf2gnjq",
                 "end": {"value": 20003097, "type": "Number"},
@@ -65,50 +65,50 @@
             }
         }
     }
     return CanonicalVariation(**params)
 
 
 @pytest.fixture(scope="module")
-def variation1_cn_var(variation1_seq_loc):
-    """Create test fixture for variation1 represented as copy number count"""
+def variation1_abs_cnv(variation1_seq_loc):
+    """Create test fixture for variation1 represented as absolute cnv"""
     params = {
-        "id": "ga4gh:CAN.COZ3w7stbXexmpHiSIcVkGDXjRs_uJWn",
+        "id": "ga4gh:CLV.hQ2OOqFOxd_bdXJbZx4-AwJgvQcPZeLq",
         "type": "CanonicalVariation",
         "canonical_context": {
-            "id": "ga4gh:CN.BEQZ7WHuRThM0k0pKzZEPe3hLBNjMDWN",
-            "type": "CopyNumberCount",
-            "subject": variation1_seq_loc,
+            "id": "ga4gh:ACN.p_KPDMw49gN0frUAlt_FRBN7Ls4vToZu",
+            "type": "AbsoluteCopyNumber",
+            "location": variation1_seq_loc,
             "copies": {"type": "Number", "value": 2}
         }
     }
     return CanonicalVariation(**params)
 
 
 @pytest.fixture(scope="module")
-def variation1_cx_var(variation1_seq_loc):
-    """Create test fixture for variation1 represented as copy number change"""
+def variation1_rel_cnv(variation1_seq_loc):
+    """Create test fixture for variation1 represented as relative cnv"""
     params = {
-        "id": "ga4gh:CAN.o0zxV2pHejFzHNNNNefrE4EbxlGPN5sU",
+        "id": "ga4gh:CLV.Ue8qumkG57LEqjS2_xXeW9PVDuKDKdd0",
         "type": "CanonicalVariation",
         "canonical_context": {
-            "id": "ga4gh:CX.mKsge5NlTOn_azljwHIQ7cvdjmyHNI8E",
-            "type": "CopyNumberChange",
-            "subject": variation1_seq_loc,
-            "copy_change": "efo:0030069"
+            "id": "ga4gh:RCN.FEoHs6XOuAI0Lx5mJfKN4LF4iLpmeJZu",
+            "type": "RelativeCopyNumber",
+            "location": variation1_seq_loc,
+            "relative_copy_class": "complete loss"
         }
     }
     return CanonicalVariation(**params)
 
 
 @pytest.fixture(scope="module")
 def variation1_rse(variation1_seq_loc):
     """Create test fixture for variation1 represented as RSE"""
     params = {
-        "id": "ga4gh:CAN.oizMWSwBdIddFvs_vA8YqxR7YWupBMrF",
+        "id": "ga4gh:CLV.oizMWSwBdIddFvs_vA8YqxR7YWupBMrF",
         "type": "CanonicalVariation",
         "canonical_context": {
             "id": "ga4gh:VA.91WFk_XWzbzUEI-SfYZip8r1g7I5wqBo",
             "type": "Allele",
             "location": variation1_seq_loc,
             "state": {
                 "type": "RepeatedSequenceExpression",
@@ -127,69 +127,69 @@
     return CanonicalVariation(**params)
 
 
 @pytest.fixture(scope="module")
 def variation2(braf_v600e_genomic_sub):
     """Create test fixture for NC_000007.14:140753335:A:T"""
     params = {
-        "id": "ga4gh:CAN.dP6z4p7SoGJFmlFQcjOQo2d1mXuo1QiY",
+        "id": "ga4gh:CLV.dP6z4p7SoGJFmlFQcjOQo2d1mXuo1QiY",
         "type": "CanonicalVariation",
         "canonical_context": braf_v600e_genomic_sub
     }
     return CanonicalVariation(**params)
 
 
 @pytest.fixture(scope="module")
 def variation3_lse(grch38_genomic_insertion_variation):
     """Create test fixture for NC_000017.10:g.37880993_37880994insGCTTACGTGATG"""
     params = {
-        "id": "ga4gh:CAN.8Pi46FGQsmKIb-6Q0NYKQh0baDBOMvFF",
+        "id": "ga4gh:CLV.8Pi46FGQsmKIb-6Q0NYKQh0baDBOMvFF",
         "type": "CanonicalVariation",
         "canonical_context": grch38_genomic_insertion_variation
     }
     return CanonicalVariation(**params)
 
 
 @pytest.fixture(scope="module")
-def variation3_cn_var(grch38_genomic_insertion_seq_loc):
-    """Create test fixture for variation3 represented as copy number count"""
+def variation3_abs_cnv(grch38_genomic_insertion_seq_loc):
+    """Create test fixture for variation3 represented as absolute cnv"""
     params = {
-        "id": "ga4gh:CAN.e0xl0wFhoZamh4rMZ9h5F8-bIvrMk2Jp",
+        "id": "ga4gh:CLV.DzOrKfPgfowNyivzu3WP48H8iPFiLdd1",
         "type": "CanonicalVariation",
         "canonical_context": {
-            "id": "ga4gh:CN.AGpJnGGrAb0EyFNYbQm8Xl3ycImaoR0s",
-            "type": "CopyNumberCount",
-            "subject": grch38_genomic_insertion_seq_loc,
+            "id": "ga4gh:ACN.e_Nd4RGisOcOmrWVklM-3gGZIo6jSnml",
+            "type": "AbsoluteCopyNumber",
+            "location": grch38_genomic_insertion_seq_loc,
             "copies": {"type": "Number", "value": 2}
         }
     }
     return CanonicalVariation(**params)
 
 
 @pytest.fixture(scope="module")
-def variation3_cx_var(grch38_genomic_insertion_seq_loc):
-    """Create test fixture for variation3 represented as copy number change"""
+def variation3_rel_cnv(grch38_genomic_insertion_seq_loc):
+    """Create test fixture for variation3 represented as relative cnv"""
     params = {
-        "id": "ga4gh:CAN.cMEZCpwf-Y1830nNv2VWxee-VdOKl-cg",
+        "id": "ga4gh:CLV.3VhMDipw7_25RSuPvtz-DCYhzjQCoED7",
         "type": "CanonicalVariation",
         "canonical_context": {
-            "id": "ga4gh:CX.upJUYyGZaVMvnwsDGJeAC4Ngdf6XIeiJ",
-            "type": "CopyNumberChange",
-            "subject": grch38_genomic_insertion_seq_loc,
-            "copy_change": "efo:0030072"
+            "id": "ga4gh:RCN.XOeH_PqiR6pkFMmHewn9SjxZEOOZoXVp",
+            "type": "RelativeCopyNumber",
+            "location": grch38_genomic_insertion_seq_loc,
+            "relative_copy_class": "high-level gain"
         }
     }
     return CanonicalVariation(**params)
 
 
 @pytest.fixture(scope="module")
 def variation3_rse(grch38_genomic_insertion_seq_loc):
     """Create test fixture for variation3 represented as RSE"""
     params = {
-        "id": "ga4gh:CAN.Ohalqu5SLmNmwjaE00v26KskGfggXwjq",
+        "id": "ga4gh:CLV.Ohalqu5SLmNmwjaE00v26KskGfggXwjq",
         "type": "CanonicalVariation",
         "canonical_context": {
             "id": "ga4gh:VA.j6BnT9kvqTO_BQCjTsOzhcnjiwNlhMHv",
             "type": "Allele",
             "location": grch38_genomic_insertion_seq_loc,
             "state": {
                 "type": "RepeatedSequenceExpression",
@@ -208,15 +208,15 @@
     return CanonicalVariation(**params)
 
 
 @pytest.fixture(scope="module")
 def variation4():
     """Create test fixture for NC_000001.11:g.2229202_2229203insCTC"""
     params = {
-        "id": "ga4gh:CAN.azUwFImJO4pTH6rSRx6UItCoxJcTvxln",
+        "id": "ga4gh:CLV.azUwFImJO4pTH6rSRx6UItCoxJcTvxln",
         "type": "CanonicalVariation",
         "canonical_context": {
             "id": "ga4gh:VA.M9Ekcss52lqr1IoX3wZeLTxVsrPW1MSq",
             "type": "Allele",
             "location": {
                 "id": "ga4gh:SL.UdTlDoFUhChBvTu2PXFg_QHA8QsxAy0m",
                 "type": "SequenceLocation",
@@ -228,15 +228,15 @@
         }
     }
     return CanonicalVariation(**params)
 
 
 @pytest.mark.asyncio
 async def test_to_canonical_variation_deletion(
-    test_handler, variation1_lse, variation1_cn_var, variation1_cx_var,
+    test_handler, variation1_lse, variation1_abs_cnv, variation1_rel_cnv,
     variation1_rse, variation_del_lse
 ):
     """Test that to_canonical_variation works correctly for deletions"""
     # https://www.ncbi.nlm.nih.gov/clinvar/variation/17014/?new_evidence=true
     q = " NC_000013.11:20189346:GGG:GG "  # 38
     resp = await test_handler.to_canonical_variation(q, fmt="spdi")
     assert resp.canonical_variation == variation1_lse
@@ -277,23 +277,23 @@
     # Testing hgvs dup del mode params
     resp = await test_handler.to_canonical_variation(
         q, fmt="hgvs", do_liftover=True, hgvs_dup_del_mode="default")
     assert resp.canonical_variation == variation1_lse
     assert resp.warnings == []
 
     resp = await test_handler.to_canonical_variation(
-        q, fmt="hgvs", do_liftover=True, hgvs_dup_del_mode="copy_number_count",
+        q, fmt="hgvs", do_liftover=True, hgvs_dup_del_mode="absolute_cnv",
         baseline_copies=3)
-    assert resp.canonical_variation == variation1_cn_var
+    assert resp.canonical_variation == variation1_abs_cnv
     assert resp.warnings == []
 
     resp = await test_handler.to_canonical_variation(
-        q, fmt="hgvs", do_liftover=True, hgvs_dup_del_mode="copy_number_change",
-        copy_change="efo:0030069")
-    assert resp.canonical_variation == variation1_cx_var
+        q, fmt="hgvs", do_liftover=True, hgvs_dup_del_mode="relative_cnv",
+        relative_copy_class="complete loss")
+    assert resp.canonical_variation == variation1_rel_cnv
     assert resp.warnings == []
 
     resp = await test_handler.to_canonical_variation(
         q, fmt="hgvs", do_liftover=True, hgvs_dup_del_mode="repeated_seq_expr")
     assert resp.canonical_variation == variation1_rse
     assert resp.warnings == []
 
@@ -333,15 +333,15 @@
             q, fmt="hgvs", hgvs_dup_del_mode=mode, baseline_copies=2)
         assert resp.canonical_variation == variation2
         assert resp.warnings == []
 
 
 @pytest.mark.asyncio
 async def test_to_canonical_variation_duplication(
-    test_handler, variation3_lse, variation3_cn_var, variation3_cx_var,
+    test_handler, variation3_lse, variation3_abs_cnv, variation3_rel_cnv,
     variation3_rse
 ):
     """Test that to_canonical_variation works correctly for duplications"""
     # https://www.ncbi.nlm.nih.gov/clinvar/variation/44985/
     q = "NC_000017.10:g.37880993_37880994insGCTTACGTGATG"  # 37
     resp = await test_handler.to_canonical_variation(
         q, fmt="hgvs", do_liftover=True)
@@ -373,23 +373,23 @@
     # Testing hgvs dup del mode params
     resp = await test_handler.to_canonical_variation(
         q, fmt="hgvs", do_liftover=True, hgvs_dup_del_mode="default")
     assert resp.canonical_variation == variation3_lse
     assert resp.warnings == []
 
     resp = await test_handler.to_canonical_variation(
-        q, fmt="hgvs", do_liftover=True, hgvs_dup_del_mode="copy_number_count",
+        q, fmt="hgvs", do_liftover=True, hgvs_dup_del_mode="absolute_cnv",
         baseline_copies=1)
-    assert resp.canonical_variation == variation3_cn_var
+    assert resp.canonical_variation == variation3_abs_cnv
     assert resp.warnings == []
 
     resp = await test_handler.to_canonical_variation(
-        q, fmt="hgvs", do_liftover=True, hgvs_dup_del_mode="copy_number_change",
-        copy_change="efo:0030072")
-    assert resp.canonical_variation == variation3_cx_var
+        q, fmt="hgvs", do_liftover=True, hgvs_dup_del_mode="relative_cnv",
+        relative_copy_class="high-level gain")
+    assert resp.canonical_variation == variation3_rel_cnv
     assert resp.warnings == []
 
     resp = await test_handler.to_canonical_variation(
         q, fmt="hgvs", do_liftover=True, hgvs_dup_del_mode="repeated_seq_expr")
     assert resp.canonical_variation == variation3_rse
     assert resp.warnings == []
 
@@ -481,10 +481,10 @@
         q, fmt="spdi", do_liftover=True)
     assert resp.canonical_variation is None
     assert resp.warnings == \
         ["Expected to find reference sequence A but found C on NC_000001.11"]
 
     q = " NC_000013.11:g.20189349del "  # 38
     resp = await test_handler.to_canonical_variation(
-        q, fmt="hgvs", hgvs_dup_del_mode="copy_number_count")
+        q, fmt="hgvs", hgvs_dup_del_mode="absolute_cnv")
     assert resp.canonical_variation is None
-    assert resp.warnings == ["copy_number_count requires `baseline_copies`"]
+    assert resp.warnings == ["absolute_cnv requires `baseline_copies`"]
```

### Comparing `variation-normalizer-0.7.0.dev7/tests/tokenizers/test_amplification.py` & `variation-normalizer-0.7.dev0/tests/tokenizers/test_amplification.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/tokenizers/test_coding_dna_deletion.py` & `variation-normalizer-0.7.dev0/tests/tokenizers/test_coding_dna_insertion.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-"""A module for testing Coding DNA Deletion Tokenization."""
+"""A module for testing Coding DNA Insertion Tokenization."""
 import unittest
 
-from variation.tokenizers import CodingDNADeletion
+from variation.tokenizers.caches import AminoAcidCache, NucleotideCache
+from variation.tokenizers import CodingDNAInsertion
 from .tokenizer_base import TokenizerBase
 
 
-class TestCodingDNADeletionTokenizer(TokenizerBase, unittest.TestCase):
-    """A class for testing Coding DNA Deletion Tokenization."""
+class TestCodingDNAInsertionTokenizer(TokenizerBase, unittest.TestCase):
+    """A class for testing Coding DNA Insertion Tokenization."""
 
     def tokenizer_instance(self):
-        """Return Coding DNA Deletion instance."""
-        return CodingDNADeletion()
+        """Return Coding DNA Insertion instance."""
+        return CodingDNAInsertion(AminoAcidCache(), NucleotideCache())
 
     def token_type(self):
-        """Return Coding DNA deletion token type."""
-        return "CodingDNADeletion"
+        """Return Coding DNA insertion token type."""
+        return "CodingDNAInsertion"
 
     def fixture_name(self):
-        """Return the fixture name for Coding DNA Deletion."""
-        return "coding_dna_deletion"
+        """Return the fixture name for Coding DNA Insertion."""
+        return "coding_dna_insertion"
```

### Comparing `variation-normalizer-0.7.0.dev7/tests/tokenizers/test_coding_dna_delins.py` & `variation-normalizer-0.7.dev0/tests/tokenizers/test_coding_dna_delins.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """A module for testing Coding DNA DelIns tokenization."""
 import unittest
 
+from variation.tokenizers.caches import AminoAcidCache, NucleotideCache
 from variation.tokenizers import CodingDNADelIns
 from .tokenizer_base import TokenizerBase
 
 
 class TestCodingDNADelInsTokenizer(TokenizerBase, unittest.TestCase):
     """A class for testing Coding DNA DelIns Tokenization."""
 
     def tokenizer_instance(self):
         """Return Coding DNA DelIns instance."""
-        return CodingDNADelIns()
+        return CodingDNADelIns(AminoAcidCache(), NucleotideCache())
 
     def token_type(self):
         """Return DNA coding delins token type."""
         return "CodingDNADelIns"
 
     def fixture_name(self):
         """Return the fixture name for DNA coding delins."""
```

### Comparing `variation-normalizer-0.7.0.dev7/tests/tokenizers/test_coding_dna_insertion.py` & `variation-normalizer-0.7.dev0/tests/tokenizers/test_protein_insertion.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-"""A module for testing Coding DNA Insertion Tokenization."""
+"""A module for testing Protein Insertion Tokenization."""
 import unittest
 
-from variation.tokenizers import CodingDNAInsertion
+from variation.tokenizers import ProteinInsertion
+from variation.tokenizers.caches import AminoAcidCache, NucleotideCache
 from .tokenizer_base import TokenizerBase
 
 
-class TestCodingDNAInsertionTokenizer(TokenizerBase, unittest.TestCase):
-    """A class for testing Coding DNA Insertion Tokenization."""
+class TestProteinInsertionTokenizer(TokenizerBase, unittest.TestCase):
+    """A class for testing Protein Insertion Tokenization."""
 
     def tokenizer_instance(self):
-        """Return Coding DNA Insertion instance."""
-        return CodingDNAInsertion()
+        """Return Protein Insertion instance."""
+        return ProteinInsertion(AminoAcidCache(), NucleotideCache())
 
     def token_type(self):
-        """Return Coding DNA insertion token type."""
-        return "CodingDNAInsertion"
+        """Return protein insertion token type."""
+        return "ProteinInsertion"
 
     def fixture_name(self):
-        """Return the fixture name for Coding DNA Insertion."""
-        return "coding_dna_insertion"
+        """Return the fixture name for protein insertion."""
+        return "protein_insertion"
```

### Comparing `variation-normalizer-0.7.0.dev7/tests/tokenizers/test_coding_dna_silent_mutation.py` & `variation-normalizer-0.7.dev0/tests/tokenizers/test_coding_dna_silent_mutation.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/tokenizers/test_coding_dna_substitution.py` & `variation-normalizer-0.7.dev0/tests/tokenizers/test_coding_dna_substitution.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/tokenizers/test_gene_symbol.py` & `variation-normalizer-0.7.dev0/tests/tokenizers/test_hgvs.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,21 @@
-"""A module for testing the Gene Pair Tokenizer."""
+"""A module for testing HGVS tokenization."""
 import unittest
 
-from gene.database.dynamodb import DynamoDbDatabase
-from gene.query import QueryHandler as GeneQueryHandler
-
-from variation.tokenizers import GeneSymbol
+from variation.tokenizers import HGVS
 from .tokenizer_base import TokenizerBase
 
 
-class TestGeneSymbolTokenizer(TokenizerBase, unittest.TestCase):
-    """The Gene Pair Tokenizer class."""
+class TestHGVSTokenizer(TokenizerBase, unittest.TestCase):
+    """A class for testing HGVS Tokenization."""
 
     def tokenizer_instance(self):
-        """Return the Gene Pair tokenizer instance."""
-        return GeneSymbol(GeneQueryHandler(DynamoDbDatabase()))
+        """Return HGVS instance."""
+        return HGVS()
 
     def token_type(self):
-        """Return the Gene Pair token type."""
-        return "GeneSymbol"
+        """Return HGVS token type."""
+        return "HGVS"
 
     def fixture_name(self):
-        """Return the fixture name for Gene Pair."""
-        return "gene"
+        """Return fixture name for HGVS."""
+        return "hgvs"
```

### Comparing `variation-normalizer-0.7.0.dev7/tests/tokenizers/test_genomic_deletion.py` & `variation-normalizer-0.7.dev0/tests/tokenizers/test_genomic_deletion.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """A module for testing Genomic Deletion Tokenization."""
 import unittest
 
+from variation.tokenizers.caches import AminoAcidCache, NucleotideCache
 from variation.tokenizers import GenomicDeletion
 from .tokenizer_base import TokenizerBase
 
 
 class TestGenomicDeletionTokenizer(TokenizerBase, unittest.TestCase):
     """A class for testing Coding DNA Deletion Tokenization."""
 
     def tokenizer_instance(self):
         """Return Genomic Deletion instance."""
-        return GenomicDeletion()
+        return GenomicDeletion(AminoAcidCache(), NucleotideCache())
 
     def token_type(self):
         """Return genomic deletion token type."""
         return "GenomicDeletion"
 
     def fixture_name(self):
         """Return the fixture name for Genomic Deletion."""
```

### Comparing `variation-normalizer-0.7.0.dev7/tests/tokenizers/test_genomic_deletion_range.py` & `variation-normalizer-0.7.dev0/tests/tokenizers/test_genomic_deletion_range.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/tokenizers/test_genomic_delins.py` & `variation-normalizer-0.7.dev0/tests/tokenizers/test_genomic_delins.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """A module for testing Genomic DelIns tokenization."""
 import unittest
 
+from variation.tokenizers.caches import AminoAcidCache, NucleotideCache
 from variation.tokenizers import GenomicDelIns
 from .tokenizer_base import TokenizerBase
 
 
 class TestGenomicDelInsTokenizer(TokenizerBase, unittest.TestCase):
     """A class for testing Genomic DelIns Tokenization."""
 
     def tokenizer_instance(self):
         """Return Genomic DelIns instance."""
-        return GenomicDelIns()
+        return GenomicDelIns(AminoAcidCache(), NucleotideCache())
 
     def token_type(self):
         """Return genomic delins token type."""
         return "GenomicDelIns"
 
     def fixture_name(self):
         """Return the fixture name for genomic delins."""
```

### Comparing `variation-normalizer-0.7.0.dev7/tests/tokenizers/test_genomic_duplication.py` & `variation-normalizer-0.7.dev0/tests/tokenizers/test_genomic_duplication.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/tokenizers/test_genomic_duplication_range.py` & `variation-normalizer-0.7.dev0/tests/tokenizers/test_genomic_duplication_range.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/tokenizers/test_genomic_insertion.py` & `variation-normalizer-0.7.dev0/tests/tokenizers/test_genomic_insertion.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """A module for testing Genomic Insertion Tokenization."""
 import unittest
 
+from variation.tokenizers.caches import AminoAcidCache, NucleotideCache
 from variation.tokenizers import GenomicInsertion
 from .tokenizer_base import TokenizerBase
 
 
 class TestGenomicInsertionTokenizer(TokenizerBase, unittest.TestCase):
     """A class for testing Genomic Insertion Tokenization."""
 
     def tokenizer_instance(self):
         """Return Genomic Insertion instance."""
-        return GenomicInsertion()
+        return GenomicInsertion(AminoAcidCache(), NucleotideCache())
 
     def token_type(self):
         """Return genomic insertion token type."""
         return "GenomicInsertion"
 
     def fixture_name(self):
         """Return the fixture name for Genomic Insertion."""
```

### Comparing `variation-normalizer-0.7.0.dev7/tests/tokenizers/test_genomic_silent_mutation.py` & `variation-normalizer-0.7.dev0/tests/tokenizers/test_genomic_silent_mutation.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/tokenizers/test_genomic_substitution.py` & `variation-normalizer-0.7.dev0/tests/tokenizers/test_genomic_substitution.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/tokenizers/test_genomic_uncertain_deletion.py` & `variation-normalizer-0.7.dev0/tests/tokenizers/test_genomic_uncertain_deletion.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/tokenizers/test_gnomad_vcf.py` & `variation-normalizer-0.7.dev0/tests/tokenizers/test_gnomad_vcf.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/tokenizers/test_hgvs.py` & `variation-normalizer-0.7.dev0/tests/tokenizers/test_silent_mutation.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-"""A module for testing HGVS tokenization."""
+"""A module for testing Silent Mutation tokenization."""
 import unittest
 
-from variation.tokenizers import HGVS
+from variation.tokenizers.caches import AminoAcidCache
+from variation.tokenizers import SilentMutation
 from .tokenizer_base import TokenizerBase
 
 
-class TestHGVSTokenizer(TokenizerBase, unittest.TestCase):
-    """A class for testing HGVS Tokenization."""
+class TestSilentMutationTokenizer(TokenizerBase, unittest.TestCase):
+    """A class for testing Silent Mutation Tokenization."""
 
     def tokenizer_instance(self):
-        """Return HGVS instance."""
-        return HGVS()
+        """Return Silent Mutation instance."""
+        return SilentMutation(AminoAcidCache())
 
     def token_type(self):
-        """Return HGVS token type."""
-        return "HGVS"
+        """Return Silent Mutation token type."""
+        return "SilentMutation"
 
     def fixture_name(self):
-        """Return fixture name for HGVS."""
-        return "hgvs"
+        """Return the fixture name for Silent Mutation."""
+        return "silent_mutation"
```

### Comparing `variation-normalizer-0.7.0.dev7/tests/tokenizers/test_locus_reference_genomic.py` & `variation-normalizer-0.7.dev0/tests/tokenizers/test_locus_reference_genomic.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/tokenizers/test_polypeptide_truncation.py` & `variation-normalizer-0.7.dev0/tests/tokenizers/test_polypeptide_truncation.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """A module for testing Polypeptide Truncation tokenization."""
 import unittest
 
+from variation.tokenizers.caches import AminoAcidCache
 from variation.tokenizers import PolypeptideTruncation
 from .tokenizer_base import TokenizerBase
 
 
 class TestPolypeptideTruncationTokenizer(TokenizerBase, unittest.TestCase):
     """A class for testing Polypeptide Truncation  Tokenization."""
 
     def tokenizer_instance(self):
         """Return Polypeptide Truncation instance."""
-        return PolypeptideTruncation()
+        return PolypeptideTruncation(AminoAcidCache())
 
     def token_type(self):
         """Return Polypeptide Truncation token type."""
         return "PolypeptideTruncation"
 
     def fixture_name(self):
         """Return the fixture name for Polypeptide Truncation."""
```

### Comparing `variation-normalizer-0.7.0.dev7/tests/tokenizers/test_protein_deletion.py` & `variation-normalizer-0.7.dev0/tests/tokenizers/test_protein_deletion.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """A module for testing Protein Deletion Tokenization."""
 import unittest
 
+from variation.tokenizers.caches import AminoAcidCache, NucleotideCache
 from variation.tokenizers import ProteinDeletion
 from .tokenizer_base import TokenizerBase
 
 
 class TestProteinDeletionTokenizer(TokenizerBase, unittest.TestCase):
     """A class for testing Protein Deletion Tokenization."""
 
     def tokenizer_instance(self):
         """Return Protein Deletion instance."""
-        return ProteinDeletion()
+        return ProteinDeletion(AminoAcidCache(), NucleotideCache())
 
     def token_type(self):
         """Return protein deletion token type."""
         return "ProteinDeletion"
 
     def fixture_name(self):
         """Return the fixture name for protein deletion."""
```

### Comparing `variation-normalizer-0.7.0.dev7/tests/tokenizers/test_protein_delins.py` & `variation-normalizer-0.7.dev0/tests/tokenizers/test_protein_delins.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """A module for testing Protein DelIns tokenization."""
 import unittest
 
+from variation.tokenizers.caches import AminoAcidCache, NucleotideCache
 from variation.tokenizers import ProteinDelIns
 from .tokenizer_base import TokenizerBase
 
 
 class TestProteinDelInsTokenizer(TokenizerBase, unittest.TestCase):
     """A class for testing Protein DelIns Tokenization."""
 
     def tokenizer_instance(self):
         """Return Protein DelIns instance."""
-        return ProteinDelIns()
+        return ProteinDelIns(AminoAcidCache(), NucleotideCache())
 
     def token_type(self):
         """Return protein delins token type."""
         return "ProteinDelIns"
 
     def fixture_name(self):
         """Return the fixture name for protein delins."""
```

### Comparing `variation-normalizer-0.7.0.dev7/tests/tokenizers/test_protein_insertion.py` & `variation-normalizer-0.7.dev0/tests/tokenizers/test_protein_substitution.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-"""A module for testing Protein Insertion Tokenization."""
+"""A module for testing Protein Substitution tokenization."""
 import unittest
 
-from variation.tokenizers import ProteinInsertion
+from variation.tokenizers.caches import AminoAcidCache
+from variation.tokenizers import ProteinSubstitution
 from .tokenizer_base import TokenizerBase
 
 
-class TestProteinInsertionTokenizer(TokenizerBase, unittest.TestCase):
-    """A class for testing Protein Insertion Tokenization."""
+class TestProteinSubstitutionTokenizer(TokenizerBase, unittest.TestCase):
+    """A class for testing Protein Substitution Tokenization."""
 
     def tokenizer_instance(self):
-        """Return Protein Insertion instance."""
-        return ProteinInsertion()
+        """Return protein substitution instance."""
+        return ProteinSubstitution(AminoAcidCache())
 
     def token_type(self):
-        """Return protein insertion token type."""
-        return "ProteinInsertion"
+        """Return protein substitution token type."""
+        return "ProteinSubstitution"
 
     def fixture_name(self):
-        """Return the fixture name for protein insertion."""
-        return "protein_insertion"
+        """Return the fixture name for protein substitution."""
+        return "protein_substitution"
```

### Comparing `variation-normalizer-0.7.0.dev7/tests/tokenizers/test_silent_mutation.py` & `variation-normalizer-0.7.dev0/tests/validators/test_silent_mutation.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-"""A module for testing Silent Mutation tokenization."""
+"""Module for testing Silent Mutation Validator."""
 import unittest
 
-from variation.tokenizers import SilentMutation
-from .tokenizer_base import TokenizerBase
+from variation.validators import SilentMutation
+from variation.classifiers import SilentMutationClassifier
+from .validator_base import ValidatorBase
 
 
-class TestSilentMutationTokenizer(TokenizerBase, unittest.TestCase):
-    """A class for testing Silent Mutation Tokenization."""
+class TestSilentMutationValidator(ValidatorBase, unittest.TestCase):
+    """A class to test the Silent Mutation Validator."""
 
-    def tokenizer_instance(self):
+    def validator_instance(self):
         """Return Silent Mutation instance."""
-        return SilentMutation()
+        return SilentMutation(*self.aa_params)
 
-    def token_type(self):
-        """Return Silent Mutation token type."""
-        return "SilentMutation"
+    def classifier_instance(self):
+        """Return the Silent Mutation classifier instance."""
+        return SilentMutationClassifier()
 
     def fixture_name(self):
         """Return the fixture name for Silent Mutation."""
         return "silent_mutation"
```

### Comparing `variation-normalizer-0.7.0.dev7/tests/tokenizers/tokenizer_base.py` & `variation-normalizer-0.7.dev0/tests/tokenizers/tokenizer_base.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/translators/test_coding_dna_deletion.py` & `variation-normalizer-0.7.dev0/tests/translators/test_coding_dna_deletion.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/translators/test_coding_dna_delins.py` & `variation-normalizer-0.7.dev0/tests/translators/test_coding_dna_delins.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/translators/test_coding_dna_insertion.py` & `variation-normalizer-0.7.dev0/tests/translators/test_coding_dna_insertion.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/translators/test_coding_dna_silent_mutation.py` & `variation-normalizer-0.7.dev0/tests/translators/test_coding_dna_silent_mutation.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/translators/test_coding_dna_substitution.py` & `variation-normalizer-0.7.dev0/tests/translators/test_coding_dna_substitution.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/translators/test_genomic_deletion.py` & `variation-normalizer-0.7.dev0/tests/translators/test_genomic_deletion.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/translators/test_genomic_delins.py` & `variation-normalizer-0.7.dev0/tests/translators/test_genomic_delins.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/translators/test_genomic_duplication.py` & `variation-normalizer-0.7.dev0/tests/translators/test_genomic_duplication.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/translators/test_genomic_insertion.py` & `variation-normalizer-0.7.dev0/tests/translators/test_genomic_insertion.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/translators/test_genomic_silent_mutation.py` & `variation-normalizer-0.7.dev0/tests/translators/test_genomic_silent_mutation.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/translators/test_genomic_substitution.py` & `variation-normalizer-0.7.dev0/tests/translators/test_genomic_substitution.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/translators/test_genomic_uncertain_deletion.py` & `variation-normalizer-0.7.dev0/tests/translators/test_genomic_uncertain_deletion.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/translators/test_polypeptide_truncation.py` & `variation-normalizer-0.7.dev0/tests/translators/test_polypeptide_truncation.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/translators/test_protein_deletion.py` & `variation-normalizer-0.7.dev0/tests/translators/test_protein_deletion.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/translators/test_protein_delins.py` & `variation-normalizer-0.7.dev0/tests/translators/test_protein_delins.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/translators/test_protein_insertion.py` & `variation-normalizer-0.7.dev0/tests/translators/test_protein_insertion.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/translators/test_protein_substitution.py` & `variation-normalizer-0.7.dev0/tests/translators/test_protein_substitution.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/translators/test_silent_mutation.py` & `variation-normalizer-0.7.dev0/tests/translators/test_silent_mutation.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/translators/translator_base.py` & `variation-normalizer-0.7.dev0/tests/translators/translator_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 """A module for testing translator classes."""
 import yaml
-from biocommons.seqrepo import SeqRepo
+from ga4gh.vrs.dataproxy import SeqRepoDataProxy
 from ga4gh.vrs.extras.translator import Translator
-from gene.database.dynamodb import DynamoDbDatabase
 from gene.query import QueryHandler as GeneQueryHandler
-from cool_seq_tool import SEQREPO_ROOT_DIR
-from cool_seq_tool.data_sources import TranscriptMappings, SeqRepoAccess, \
+from uta_tools.data_sources import TranscriptMappings, SeqRepoAccess, \
     MANETranscriptMappings, UTADatabase, MANETranscript
 
 from tests import PROJECT_ROOT
 from variation.schemas.app_schemas import Endpoint
 from variation.vrs_representation import VRSRepresentation
 from variation.tokenizers import Tokenize, GeneSymbol
+from variation.tokenizers.caches import AminoAcidCache
 
 
 class TranslatorBase:
     """The translator base class."""
 
     @classmethod
     def setUpClass(cls):
         """Set up the test cases."""
         with open(f"{PROJECT_ROOT}/tests/fixtures/translators.yml") as stream:
             cls.all_fixtures = yaml.safe_load(stream)
-        gene_normalizer = GeneQueryHandler(DynamoDbDatabase())
+        amino_acid_cache = AminoAcidCache()
+        gene_normalizer = GeneQueryHandler()
         gene_symbol = GeneSymbol(gene_normalizer)
-        cls.tokenizer = Tokenize(gene_symbol)
+        cls.tokenizer = Tokenize(amino_acid_cache, gene_symbol)
 
-        sr = SeqRepo(root_dir=SEQREPO_ROOT_DIR)
-        seqrepo_access = SeqRepoAccess(sr)
+        seqrepo_access = SeqRepoAccess()
         transcript_mappings = TranscriptMappings()
         uta = UTADatabase()
-        tlr = Translator(data_proxy=seqrepo_access)
+        dp = SeqRepoDataProxy(seqrepo_access.seqrepo_client)
+        tlr = Translator(data_proxy=dp)
         mane_transcript = MANETranscript(
             seqrepo_access, transcript_mappings, MANETranscriptMappings(), uta,
             gene_normalizer)
-        vrs = VRSRepresentation(seqrepo_access)
+        vrs = VRSRepresentation(dp, seqrepo_access)
 
         cls.aa_params = [
             seqrepo_access, transcript_mappings, gene_symbol,
-            mane_transcript, uta, tlr, gene_normalizer, vrs
+            mane_transcript, uta, tlr, gene_normalizer,
+            vrs, amino_acid_cache
         ]
         cls.params = cls.aa_params[:-1]
 
     def classifier_instance(self):
         """Check that the classifier_instance method is implemented."""
         raise NotImplementedError()
 
@@ -82,15 +83,15 @@
             for vr in validation_results:
                 if vr.is_valid:
                     variation = self.translator.translate(vr)
                     if variation["type"] == "Allele":
                         variation["location"] = variation["location"]
                         if "id" in variation["location"].keys():
                             del variation["location"]["id"]
-                    elif variation["type"] == "CopyNumberCount":
+                    elif variation["type"] == "AbsoluteCopyNumber":
                         variation["location"] = variation["location"]
                         if "id" in variation["location"]["location"].keys():
                             del variation["location"]["location"]["id"]
 
                     if variation not in found:
                         found.append(variation)
                         num_valid += 1
```

### Comparing `variation-normalizer-0.7.0.dev7/tests/validators/test_coding_dna_deletion.py` & `variation-normalizer-0.7.dev0/tests/validators/test_coding_dna_deletion.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/validators/test_coding_dna_delins.py` & `variation-normalizer-0.7.dev0/tests/validators/test_coding_dna_delins.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/validators/test_coding_dna_insertion.py` & `variation-normalizer-0.7.dev0/tests/validators/test_coding_dna_insertion.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/validators/test_coding_dna_silent_mutation.py` & `variation-normalizer-0.7.dev0/tests/validators/test_coding_dna_silent_mutation.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/validators/test_coding_dna_subsitution.py` & `variation-normalizer-0.7.dev0/tests/validators/test_coding_dna_subsitution.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/validators/test_genomic_deletion.py` & `variation-normalizer-0.7.dev0/tests/validators/test_genomic_deletion.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/validators/test_genomic_delins.py` & `variation-normalizer-0.7.dev0/tests/validators/test_genomic_delins.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/validators/test_genomic_duplication.py` & `variation-normalizer-0.7.dev0/tests/validators/test_genomic_duplication.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/validators/test_genomic_insertion.py` & `variation-normalizer-0.7.dev0/tests/validators/test_genomic_insertion.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/validators/test_genomic_silent_mutation.py` & `variation-normalizer-0.7.dev0/tests/validators/test_genomic_silent_mutation.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/validators/test_genomic_substitution.py` & `variation-normalizer-0.7.dev0/tests/validators/test_genomic_substitution.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/validators/test_genomic_uncertain_deletion.py` & `variation-normalizer-0.7.dev0/tests/validators/test_genomic_uncertain_deletion.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/validators/test_polypeptide_truncation.py` & `variation-normalizer-0.7.dev0/tests/validators/test_polypeptide_truncation.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/validators/test_protein_deletion.py` & `variation-normalizer-0.7.dev0/tests/validators/test_protein_deletion.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/validators/test_protein_delins.py` & `variation-normalizer-0.7.dev0/tests/validators/test_protein_delins.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/validators/test_protein_insertion.py` & `variation-normalizer-0.7.dev0/tests/validators/test_protein_insertion.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/validators/test_protein_substitution.py` & `variation-normalizer-0.7.dev0/tests/validators/test_protein_substitution.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/tests/validators/validator_base.py` & `variation-normalizer-0.7.dev0/tests/validators/validator_base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 """A module for testing validator classes."""
 import yaml
-from biocommons.seqrepo import SeqRepo
+from ga4gh.vrs.dataproxy import SeqRepoDataProxy
 from ga4gh.vrs.extras.translator import Translator
-from gene.database.dynamodb import DynamoDbDatabase
 from gene.query import QueryHandler as GeneQueryHandler
-from cool_seq_tool import SEQREPO_ROOT_DIR
-from cool_seq_tool.data_sources import TranscriptMappings, SeqRepoAccess, \
+from uta_tools.data_sources import TranscriptMappings, SeqRepoAccess, \
     MANETranscriptMappings, UTADatabase, MANETranscript
 
 from tests import PROJECT_ROOT
 from variation.schemas.app_schemas import Endpoint
 from variation.vrs_representation import VRSRepresentation
 from variation.tokenizers import Tokenize, GeneSymbol
+from variation.tokenizers.caches import AminoAcidCache
 
 
 class ValidatorBase:
     """The validator base class."""
 
     @classmethod
     def setUpClass(cls):
         """Set up the test cases."""
         with open(f"{PROJECT_ROOT}/tests/fixtures/validators.yml") as stream:
             cls.all_fixtures = yaml.safe_load(stream)
-        gene_normalizer = GeneQueryHandler(DynamoDbDatabase())
+        amino_acid_cache = AminoAcidCache()
+        gene_normalizer = GeneQueryHandler()
         gene_symbol = GeneSymbol(gene_normalizer)
-        cls.tokenizer = Tokenize(gene_symbol)
+        cls.tokenizer = Tokenize(amino_acid_cache, gene_symbol)
 
-        sr = SeqRepo(root_dir=SEQREPO_ROOT_DIR)
-        seqrepo_access = SeqRepoAccess(sr)
+        seqrepo_access = SeqRepoAccess()
         transcript_mappings = TranscriptMappings()
         uta = UTADatabase()
-        tlr = Translator(data_proxy=seqrepo_access)
+        dp = SeqRepoDataProxy(seqrepo_access.seqrepo_client)
+        tlr = Translator(data_proxy=dp)
         mane_transcript = MANETranscript(
             seqrepo_access, transcript_mappings, MANETranscriptMappings(), uta,
             gene_normalizer)
-        vrs = VRSRepresentation(seqrepo_access)
+        vrs = VRSRepresentation(dp, seqrepo_access)
 
         cls.aa_params = [
             seqrepo_access, transcript_mappings, gene_symbol,
-            mane_transcript, uta, tlr, gene_normalizer, vrs
+            mane_transcript, uta, tlr, gene_normalizer,
+            vrs, amino_acid_cache
         ]
         cls.params = cls.aa_params[:-1]
 
     def classifier_instance(self):
         """Check that the classifier_instance method is implemented."""
         raise NotImplementedError()
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/classifiers/__init__.py` & `variation-normalizer-0.7.dev0/variation/classifiers/__init__.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/classifiers/amplification_classifier.py` & `variation-normalizer-0.7.dev0/variation/classifiers/amplification_classifier.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/classifiers/classifier.py` & `variation-normalizer-0.7.dev0/variation/classifiers/classifier.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/classifiers/classify.py` & `variation-normalizer-0.7.dev0/variation/classifiers/classify.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/classifiers/coding_dna_deletion_classifier.py` & `variation-normalizer-0.7.dev0/variation/classifiers/coding_dna_deletion_classifier.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/classifiers/coding_dna_delins_classifier.py` & `variation-normalizer-0.7.dev0/variation/classifiers/coding_dna_delins_classifier.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/classifiers/coding_dna_insertion_classifier.py` & `variation-normalizer-0.7.dev0/variation/classifiers/coding_dna_insertion_classifier.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/classifiers/coding_dna_silent_mutation_classifier.py` & `variation-normalizer-0.7.dev0/variation/classifiers/coding_dna_silent_mutation_classifier.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/classifiers/coding_dna_substitution_classifier.py` & `variation-normalizer-0.7.dev0/variation/classifiers/coding_dna_substitution_classifier.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/classifiers/genomic_deletion_classifier.py` & `variation-normalizer-0.7.dev0/variation/classifiers/genomic_deletion_classifier.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/classifiers/genomic_deletion_range_classifier.py` & `variation-normalizer-0.7.dev0/variation/classifiers/genomic_deletion_range_classifier.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/classifiers/genomic_delins_classifier.py` & `variation-normalizer-0.7.dev0/variation/classifiers/genomic_delins_classifier.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/classifiers/genomic_duplication_classifier.py` & `variation-normalizer-0.7.dev0/variation/classifiers/genomic_duplication_classifier.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/classifiers/genomic_insertion_classifier.py` & `variation-normalizer-0.7.dev0/variation/classifiers/genomic_insertion_classifier.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/classifiers/genomic_silent_mutation_classifier.py` & `variation-normalizer-0.7.dev0/variation/classifiers/genomic_silent_mutation_classifier.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/classifiers/genomic_substitution_classifier.py` & `variation-normalizer-0.7.dev0/variation/classifiers/genomic_substitution_classifier.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/classifiers/genomic_uncertain_deletion_classifier.py` & `variation-normalizer-0.7.dev0/variation/classifiers/genomic_uncertain_deletion_classifier.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/classifiers/polypeptide_truncation_classifier.py` & `variation-normalizer-0.7.dev0/variation/classifiers/polypeptide_truncation_classifier.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/classifiers/protein_classifier.py` & `variation-normalizer-0.7.dev0/variation/classifiers/protein_classifier.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/classifiers/protein_deletion_classifier.py` & `variation-normalizer-0.7.dev0/variation/classifiers/protein_deletion_classifier.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/classifiers/protein_delins_classifier.py` & `variation-normalizer-0.7.dev0/variation/classifiers/protein_delins_classifier.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/classifiers/protein_insertion_classifier.py` & `variation-normalizer-0.7.dev0/variation/classifiers/protein_insertion_classifier.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/classifiers/protein_termination_classifier.py` & `variation-normalizer-0.7.dev0/variation/classifiers/protein_termination_classifier.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/classifiers/set_based_classifier.py` & `variation-normalizer-0.7.dev0/variation/classifiers/set_based_classifier.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/classifiers/silent_mutation.py` & `variation-normalizer-0.7.dev0/variation/classifiers/silent_mutation.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/data_sources/codon_table.py` & `variation-normalizer-0.7.dev0/variation/data_sources/codon_table.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 """Module for Codon Table."""
 from typing import Dict, List
 
-from bioutils.sequences import aa3_to_aa1
+from variation.tokenizers.caches import AminoAcidCache
 
 
 MULTIPLE_CODONS = {"Leu", "Ser", "Arg"}
 
 
 class CodonTable:
     """Class for codon table data."""
 
-    def __init__(self) -> None:
-        """Initialize codon table class."""
+    def __init__(self, amino_acid_cache: AminoAcidCache) -> None:
+        """Initialize codon table class.
+
+        :param AminoAcidCache amino_acid_cache: Amino acid code data
+        """
         self.table = self._set_codon_table()
+        self.amino_acid_cache = amino_acid_cache
         self._dna_to_rna = {
             "T": "A", "A": "U",
             "G": "C", "C": "G"
         }
 
     @staticmethod
     def _set_codon_table() -> Dict[str, str]:
@@ -45,18 +49,17 @@
 
     def get_codons(self, amino_acid: str) -> List[str]:
         """Return a list of codons for an amino acid.
 
         :param str amino_acid: Amino acid to get codons for
         :return: List of codons
         """
+        amino_acid = amino_acid.upper()
         if len(amino_acid) == 3:
-            amino_acid = aa3_to_aa1(amino_acid.capitalize())
-        else:
-            amino_acid = amino_acid.upper()
+            amino_acid = self.amino_acid_cache.convert_three_to_one(amino_acid)
 
         codons = list()
         for k, v in self.table.items():
             if v == amino_acid:
                 codons.append(k)
         codons.sort()
         return codons
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/gnomad_vcf_to_protein_variation.py` & `variation-normalizer-0.7.dev0/variation/gnomad_vcf_to_protein_variation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Module for going from gnomAD VCF to VRS variation on the protein coordinate"""
 from typing import Optional, Tuple, List, Dict
 from urllib.parse import quote
 from datetime import datetime
 
-from cool_seq_tool.data_sources import SeqRepoAccess, UTADatabase, MANETranscript,\
+from uta_tools.data_sources import SeqRepoAccess, UTADatabase, MANETranscript,\
     MANETranscriptMappings
-from cool_seq_tool.schemas import ResidueMode
+from uta_tools.schemas import ResidueMode
 from gene.query import QueryHandler as GeneQueryHandler
+from ga4gh.vrs.dataproxy import SeqRepoDataProxy
 
 from variation.classifiers.classify import Classify
 from variation.data_sources.codon_table import CodonTable
 from variation.hgvs_dup_del_mode import HGVSDupDelMode
 from variation.to_vrsatile import ToVRSATILE
 from variation.tokenizers.tokenize import Tokenize
 from variation.translators.translate import Translate
@@ -24,39 +25,40 @@
     import HGVSDupDelMode as HGVSDupDelModeEnum, NormalizeService, ServiceMeta
 from variation.version import __version__
 
 
 class GnomadVcfToProteinVariation(ToVRSATILE):
     """Class for translating gnomAD VCF representation to protein representation"""
 
-    def __init__(self, seqrepo_access: SeqRepoAccess,
+    def __init__(self, seqrepo_access: SeqRepoAccess, dp: SeqRepoDataProxy,
                  tokenizer: Tokenize, classifier: Classify, validator: Validate,
                  translator: Translate, hgvs_dup_del_mode: HGVSDupDelMode,
                  gene_normalizer: GeneQueryHandler,
                  uta: UTADatabase, mane_transcript: MANETranscript,
                  mane_transcript_mappings: MANETranscriptMappings,
                  codon_table: CodonTable) -> None:
         """Initialize the GnomadVcfToProteinVariation class
 
-        :param SeqRepoAccess seqrepo_access: Access to SeqRepo
+        :param SeqRepoAccess seqrepo_access: Access to SeqRepo via UTA Tools
+        :param SeqRepoDataProxy dp: Access to SeqRepo via VRS Python
         :param Tokenize tokenizer: Tokenizer class for tokenizing
         :param Classify classifier: Classifier class for classifying tokens
         :param Validate validator: Validator class for validating valid inputs
         :param Translate translator: Translating valid inputs
         :param HGVSDupDelMode hgvs_dup_del_mode: Class for handling
             HGVS dup/del expressions
         :parm GeneQueryHandler gene_normalizer: Client for normalizing gene concepts
         :param UTADatabase uta: Access to db containing alignment data
         :param MANETranscript mane_transcript: Access MANE Transcript
             information
         :param MANETranscriptMappings mane_transcript_mappings: Mappings for
             MANE Transcript data
         :param CodonTable codon_table: Codon table data
         """
-        super().__init__(seqrepo_access, tokenizer, classifier, validator,
+        super().__init__(seqrepo_access, dp, tokenizer, classifier, validator,
                          translator, hgvs_dup_del_mode, gene_normalizer)
         self.uta = uta
         self.mane_transcript = mane_transcript
         self.mane_transcript_mappings = mane_transcript_mappings
         self.codon_table = codon_table
 
     async def _get_gnomad_vcf_validations(
@@ -87,15 +89,15 @@
         """Get genomic ac from variation sequence_id
 
         :param Dict variation: VRS variation object
         :return: RefSeq genomic accession
         """
         # genomic ac should always be in 38
         alt_ac = variation["location"]["sequence_id"]
-        aliases = self.seqrepo_access.sr.translate_identifier(
+        aliases = self.seqrepo_access.seqrepo_client.translate_identifier(
             alt_ac, target_namespaces="refseq")
         return aliases[0].split("refseq:")[-1]
 
     def _update_gnomad_vcf_mane_c_pos(
             self, reading_frame: int, mane_c_ac: str,
             mane_c_pos_change: Tuple[int, int], coding_start_site: int,
             warnings: List) -> Optional[Tuple[int, int]]:
@@ -219,16 +221,15 @@
             for i in range(int(len(alt) / 3)):
                 aa_alt += self.codon_table.table[alt[3 * i:(3 * i) + 3]]
             return aa_alt
 
     async def gnomad_vcf_to_protein(
         self, q: str, untranslatable_returns_text: bool = False
     ) -> NormalizeService:
-        """Get MANE protein consequence for gnomad vcf (chr-pos-ref-alt).
-        Assumes using GRCh38 coordinates
+        """Get protein consequence for gnomad vcf
 
         :param str q: gnomad vcf (chr-pos-ref-alt)
         :param bool untranslatable_returns_text: `True` return VRS Text Object when
             unable to translate or normalize query. `False` return `None` when
             unable to translate or normalize query.
         :return: Normalize Service containing variation descriptor and warnings
         """
@@ -237,34 +238,20 @@
         warnings = list()
         if q:
             _id = f"normalize.variation:{quote(' '.join(q.split()))}"
             warnings = list()
             valid_list = list()
             validations = await self._get_gnomad_vcf_validations(q, warnings)
             if validations:
-                validations.valid_results = sorted(validations.valid_results,
-                                                   key=lambda x: x.is_mane_transcript,
-                                                   reverse=True)
-
-                all_warnings = set()
-                checked_valid_results = list()
+                all_warnings = list()
                 for valid_result in validations.valid_results:
                     warnings = list()
                     # all gnomad vcf will be alleles with a literal seq expression
                     variation = valid_result.variation
                     classification_token = valid_result.classification_token
-
-                    # We do not need to check the same variation that has the same
-                    # classification
-                    checked_tuple = (variation["id"], valid_result.identifier,
-                                     valid_result.classification.classification_type.value)  # noqa: E501
-                    if checked_tuple in checked_valid_results:
-                        continue
-
-                    checked_valid_results.append(checked_tuple)
                     alt_ac = self._get_refseq_alt_ac_from_variation(variation)
 
                     # 0-based
                     g_start_pos = None
                     g_end_pos = None
                     if classification_token.alt_type == "deletion":
                         g_start_pos = classification_token.start_pos_del
@@ -275,45 +262,50 @@
                     elif classification_token.alt_type in ["silent_mutation",
                                                            "substitution"]:
                         g_start_pos = classification_token.position
                         g_end_pos = classification_token.position
                         ref_seq, w = self.seqrepo_access.get_reference_sequence(
                             alt_ac, g_start_pos)
                         if not ref_seq:
-                            all_warnings.add(w)
+                            all_warnings.append(w)
                         else:
                             if ref_seq != classification_token.ref_nucleotide:
-                                all_warnings.add(
+                                all_warnings.append(
                                     f"Expected {classification_token.ref_nucleotide}"
                                     f" but found {ref_seq} on {alt_ac} at position"
                                     f" {g_start_pos}"
                                 )
                                 continue
                     else:
-                        all_warnings.add(
+                        all_warnings.append(
                             f"{classification_token.alt_type} alt_type not supported"
                         )
                         continue
 
-                    mane_data = self.mane_transcript_mappings.get_mane_data_from_chr_pos(  # noqa: E501
-                        alt_ac, g_start_pos, g_end_pos)
-                    mane_data_len = len(mane_data)
                     g_start_pos -= 1
                     g_end_pos -= 1
 
+                    transcripts = await self.uta.get_transcripts_from_genomic_pos(
+                        alt_ac, g_start_pos)
+
+                    if not transcripts:
+                        all_warnings.append(f"Unable to get transcripts given {alt_ac}"
+                                            f" and {g_start_pos + 1}")
+                        continue
+                    mane_data = self.mane_transcript_mappings.get_mane_from_transcripts(transcripts)  # noqa: E501
+                    mane_data_len = len(mane_data)
                     for i in range(mane_data_len):
-                        current_mane_data = mane_data[i]
+                        index = mane_data_len - i - 1
+                        current_mane_data = mane_data[index]
                         mane_c_ac = current_mane_data["RefSeq_nuc"]
                         mane_tx_genomic_data = await self.uta.get_mane_c_genomic_data(
                             mane_c_ac, alt_ac, g_start_pos, g_end_pos)
                         if not mane_tx_genomic_data:
-                            all_warnings.add(
-                                f"Unable to get MANE data for {mane_c_ac} using "
-                                f"{alt_ac} at positions {g_start_pos} to {g_end_pos}")
-                            continue
+                            all_warnings.append("Unable to get mane transcript and "
+                                                "genomic data")
 
                         coding_start_site = mane_tx_genomic_data["coding_start_site"]
                         mane_c_pos_change = \
                             self.mane_transcript.get_mane_c_pos_change(
                                 mane_tx_genomic_data, coding_start_site)
 
                         # We use 1-based
@@ -322,15 +314,15 @@
                         if classification_token.alt_type in ["substitution",
                                                              "silent_mutation"]:
                             mane_c_pos_change = self._update_gnomad_vcf_mane_c_pos(
                                 reading_frame, mane_c_ac, mane_c_pos_change,
                                 coding_start_site, warnings)
                             if mane_c_pos_change is None:
                                 if len(warnings) > 0:
-                                    all_warnings.add(warnings[0])
+                                    all_warnings.append(warnings[0])
                                 continue
 
                         mane_p = self.mane_transcript._get_mane_p(
                             current_mane_data,
                             (mane_c_pos_change[0] + 1, mane_c_pos_change[1] + 1)
                         )
                         if mane_p["pos"][0] > mane_p["pos"][1]:
@@ -352,15 +344,15 @@
                                         q, variation, valid_result, _id, warnings,
                                         gene=current_mane_data["HGNC_ID"]))
 
                 if valid_list:
                     vd, warnings = valid_list[0]
                 else:
                     if all_warnings:
-                        vd, warnings = no_variation_resp(q, _id, list(all_warnings),
+                        vd, warnings = no_variation_resp(q, _id, all_warnings,
                                                          untranslatable_returns_text)
                     else:
                         vd, warnings = no_variation_resp(
                             q, _id, [f"Unable to get protein variation for {q}"],
                             untranslatable_returns_text)
             else:
                 vd, warnings = no_variation_resp(q, _id, warnings,
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/hgvs_dup_del_mode.py` & `variation-normalizer-0.7.dev0/variation/hgvs_dup_del_mode.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Module for hgvs_dup_del_mode in normalize endpoint."""
 import logging
 from typing import Optional, Dict, Tuple, List
 
 from ga4gh.vrs import models
 from ga4gh.core import ga4gh_identify
-from cool_seq_tool.data_sources import SeqRepoAccess
-from ga4gh.vrsatile.pydantic.vrs_models import CopyChange
+from uta_tools.data_sources import SeqRepoAccess
 
+from variation.schemas.hgvs_to_copy_number_schema import RelativeCopyClass
 from variation.schemas.normalize_response_schema\
     import HGVSDupDelMode as HGVSDupDelModeEnum
 
 logger = logging.getLogger("variation")
 logger.setLevel(logging.DEBUG)
 
 
@@ -23,15 +23,15 @@
         :param SeqRepoAccess seqrepo_access: Access to seqrepo
         """
         self.seqrepo_access = seqrepo_access
         self.valid_dup_del_modes = {mode.value for mode in
                                     HGVSDupDelModeEnum.__members__.values()}
         self.valid_copy_number_modes = {mode.value for mode in
                                         HGVSDupDelModeEnum.__members__.values() if
-                                        mode.value.startswith("copy_number_")}
+                                        mode.value.endswith("_cnv")}
 
     def is_valid_dup_del_mode(self, mode: str) -> bool:
         """Determine if mode is a valid input for HGVS Dup Del Mode.
 
         :param str mode: Entered mode
         :return: `True` if valid mode. `False` otherwise.
         """
@@ -46,93 +46,94 @@
         """
         copy_number_type_mode = mode.strip().lower()
         return copy_number_type_mode in self.valid_copy_number_modes
 
     def default_mode(
         self, alt_type: str, pos: Tuple[int, int], del_or_dup: str,
         location: Dict, allele: Dict = None, baseline_copies: Optional[int] = None,
-        copy_change: Optional[CopyChange] = None
+        relative_copy_class: Optional[RelativeCopyClass] = None
     ) -> Optional[Dict]:
         """Use default characteristics to return a variation.
-        If baseline_copies not provided and endpoints are ambiguous: copy_number_change
-            if copy_change not provided:
-                copy_change = `efo:0030067` (loss) if del, `efo:0030070` (gain) if dup
-        elif baseline_copies provided: copy_number_count
+        If baseline_copies not provided and endpoints are ambiguous: relative_cnv
+            if relative_copy_class not provided:
+                relative_copy_class = `partial loss` if del, `low-level gain` if dup
+        elif baseline_copies provided: absolute_cnv
             copies are baseline + 1 for dup, baseline - 1 for del
         elif len del or dup > 100bp (use outermost coordinates):
             repeated_seq_expr with a derived_seq_expr subject (Allele)
         else:
             literal_seq_expr (normalized LiteralSequenceExpression Allele)
 
         :param str alt_type: Alteration type
         :param tuple pos: start_pos, end_pos
         :param str del_or_dup: Must be either `del` or `dup`
         :param Dict location: Sequence Location object
         :param Dict allele: VRS Allele object represented as a dict
-        :param Optional[int] baseline_copies: Baseline copies for Copy Number Count
-            variation
-        :param Optional[CopyChange] copy_change: copy change for Copy Number Change
-            Variation
+        :param Optional[int] baseline_copies: Baseline copies for Absolute Relative
+            Copy Number Variation
+        :param Optional[RelativeCopyClass] relative_copy_class: Relative copy class
+            for Relative Copy Number Variation
         :return: VRS Variation object represented as a dict
         """
         variation = None
         if not baseline_copies and ("uncertain" in alt_type or "range" in alt_type):
-            variation = self.copy_number_change_mode(del_or_dup, location, copy_change)
+            variation = self.relative_copy_number_mode(del_or_dup, location,
+                                                       relative_copy_class)
         elif baseline_copies:
-            variation = self.copy_number_count_mode(del_or_dup, location,
-                                                    baseline_copies)
+            variation = self.absolute_copy_number_mode(del_or_dup, location,
+                                                       baseline_copies)
         elif pos and (pos[1] - pos[0] > 100):
             variation = self.repeated_seq_expr_mode(alt_type, location)
         else:
             variation = self.literal_seq_expr_mode(allele, alt_type)
         return variation
 
-    def copy_number_count_mode(self, del_or_dup: str, location: Dict,
-                               baseline_copies: int) -> Optional[Dict]:
-        """Return a VRS Copy Number Count Variation.
+    def absolute_copy_number_mode(self, del_or_dup: str, location: Dict,
+                                  baseline_copies: int) -> Optional[Dict]:
+        """Return a VRS Copy Number Variation.
 
         :param str del_or_dup: Must be either `del` or `dup`
         :param Dict location: VRS SequenceLocation
         :param int baseline_copies: Baseline copies number
-        :return: VRS Copy Number Count object represented as a dict
+        :return: VRS Copy Number object represented as a dict
         """
         copies = models.Number(
             value=baseline_copies - 1 if del_or_dup == "del" else baseline_copies + 1,
             type="Number"
         )
         variation = {
-            "type": "CopyNumberCount",
-            "subject": location,
+            "type": "AbsoluteCopyNumber",
+            "location": location,
             "copies": copies.as_dict()
         }
-        variation["id"] = ga4gh_identify(models.CopyNumberCount(**variation))
+        variation["id"] = ga4gh_identify(models.AbsoluteCopyNumber(**variation))
         return variation
 
-    def copy_number_change_mode(
+    def relative_copy_number_mode(
         self, del_or_dup: str, location: Dict,
-        copy_change: Optional[CopyChange] = None
+        relative_copy_class: Optional[RelativeCopyClass] = None
     ) -> Optional[Dict]:
-        """Return copy number change variation
+        """Return relative copy number variation
 
         :param str del_or_dup: Must be either `del` or `dup`
         :param Dict location: VRS SequenceLocation
-        :param Optional[CopyChange] copy_change: The copy change
-        :return: Copy Number Change variation as a dict
+        :param Optional[RelativeCopyClass] relative_copy_class: The relative copy class
+        :return: Relative copy number variation as a dict
         """
-        if not copy_change:
+        if not relative_copy_class:
             if del_or_dup == "del":
-                copy_change = CopyChange.LOSS.value
+                relative_copy_class = RelativeCopyClass.PARTIAL_LOSS.value
             else:
-                copy_change = CopyChange.GAIN.value
+                relative_copy_class = RelativeCopyClass.LOW_LEVEL_GAIN.value
         variation = {
-            "type": "CopyNumberChange",
-            "subject": location,
-            "copy_change": copy_change
+            "type": "RelativeCopyNumber",
+            "location": location,
+            "relative_copy_class": relative_copy_class
         }
-        variation["id"] = ga4gh_identify(models.CopyNumberChange(**variation))
+        variation["id"] = ga4gh_identify(models.RelativeCopyNumber(**variation))
         return variation
 
     def repeated_seq_expr_mode(self, alt_type: str, location: Dict) -> Optional[Dict]:
         """Return a VRS Allele with a RepeatedSequenceExpression.
         The RepeatedSequenceExpression subject will be a
             DerivedSequenceExpression.
 
@@ -195,54 +196,54 @@
             variation.id = ga4gh_identify(variation)
             return variation.as_dict()
 
     def interpret_variation(
         self, alt_type: str, allele: Dict, errors: List,
         hgvs_dup_del_mode: HGVSDupDelModeEnum, pos: Optional[Tuple[int, int]] = None,
         baseline_copies: Optional[int] = None,
-        copy_change: Optional[CopyChange] = None
+        relative_copy_class: Optional[RelativeCopyClass] = None
     ) -> Dict:
         """Interpret variation using HGVSDupDelMode
 
         :param str alt_type: Alteration type
         :param Dict allele: VRS Allele object
         :param List errors: List of errors
         :param HGVSDupDelModeEnum hgvs_dup_del_mode: Mode to use for
             interpreting HGVS duplications and deletions
         :param Optional[Tuple[int, int]] pos: Position changes
         :param Optional[int] baseline_copies: Baseline copies number
-        :param Optional[CopyChange] copy_change: The copy change
+        :param Optional[RelativeCopyClass] relative_copy_class: The relative copy class
         :return: VRS Variation object
         """
         if "deletion" in alt_type:
             del_or_dup = "del"
         else:
             del_or_dup = "dup"
         variation = None
         if allele is None:
             errors.append("Unable to get Allele")
         else:
             if hgvs_dup_del_mode == HGVSDupDelModeEnum.DEFAULT:
                 variation = self.default_mode(
                     alt_type, pos, del_or_dup, allele["location"],
                     allele=allele, baseline_copies=baseline_copies,
-                    copy_change=copy_change)
+                    relative_copy_class=relative_copy_class)
             elif hgvs_dup_del_mode == HGVSDupDelModeEnum.REPEATED_SEQ_EXPR:
                 variation = self.repeated_seq_expr_mode(
                     alt_type, allele["location"]
                 )
             elif hgvs_dup_del_mode == HGVSDupDelModeEnum.LITERAL_SEQ_EXPR:
                 variation = self.literal_seq_expr_mode(allele, alt_type)
-            elif hgvs_dup_del_mode == HGVSDupDelModeEnum.COPY_NUMBER_COUNT:
+            elif hgvs_dup_del_mode == HGVSDupDelModeEnum.ABSOLUTE_CNV:
                 if baseline_copies:
-                    variation = self.copy_number_count_mode(
+                    variation = self.absolute_copy_number_mode(
                         del_or_dup, allele["location"], baseline_copies)
                 else:
-                    errors.append("`baseline_copies` must be provided for Copy Number "
-                                  "Count Variation")
-            elif hgvs_dup_del_mode == HGVSDupDelModeEnum.COPY_NUMBER_CHANGE:
-                variation = self.copy_number_change_mode(
+                    errors.append("`baseline_copies` must be provided for Absolute"
+                                  " Copy Number Variation")
+            elif hgvs_dup_del_mode == HGVSDupDelModeEnum.RELATIVE_CNV:
+                variation = self.relative_copy_number_mode(
                     del_or_dup, allele["location"],
-                    copy_change=copy_change)
+                    relative_copy_class=relative_copy_class)
             if not variation:
                 errors.append("Unable to get VRS Variation")
         return variation
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/main.py` & `variation-normalizer-0.7.dev0/variation/main.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 from urllib.parse import unquote
 
 import pkg_resources
 from fastapi import FastAPI, Query
 from fastapi.openapi.utils import get_openapi
 from pydantic import ValidationError
 import python_jsonschema_objects
-from ga4gh.vrsatile.pydantic.vrs_models import CopyChange
+from ga4gh.vrsatile.pydantic.vrs_models import RelativeCopyClass
 from hgvs.exceptions import HGVSError
 from bioutils.exceptions import BioutilsError
 from ga4gh.vrs import models
 
 from variation.schemas import ToVRSService, NormalizeService, ServiceMeta
 from variation.schemas.hgvs_to_copy_number_schema import \
-    HgvsToCopyNumberCountService, HgvsToCopyNumberChangeService
+    HgvsToAbsoluteCopyNumberService, HgvsToRelativeCopyNumberService
 from variation.query import QueryHandler
 from variation.schemas.normalize_response_schema \
     import HGVSDupDelMode as HGVSDupDelModeEnum, ToCanonicalVariationFmt, \
     ToCanonicalVariationService, TranslateIdentifierService
-from variation.schemas.service_schema import AmplificationToCxVarService, \
-    ClinVarAssembly, ParsedToCnVarService
+from variation.schemas.service_schema import AmplificationToRelCnvService, \
+    ClinVarAssembly, ParsedToAbsCnvService
 from .version import __version__
 from .schemas.vrs_python_translator_schema import TranslateFromFormat, \
     TranslateFromService, TranslateFromQuery, TranslateToHGVSQuery, TranslateToQuery,\
     TranslateToService, VrsPythonMeta
 
 
 class Tags(Enum):
@@ -117,59 +117,59 @@
 normalize_response_description = "A response to a validly-formed query."
 normalize_description = ("Normalizes and translates a human readable variation "
                          "description to a single VRSATILE Variation Descriptor. "
                          "Performs fully-justified allele normalization. Will liftover"
                          " to GRCh38 and aligns to a priority transcript. Will make "
                          "inferences about the query.")
 q_description = "Human readable variation description on GRCh37 or GRCh38 assembly"
-hgvs_dup_del_mode_decsr = ("Must be one of: `default`, `copy_number_count`, "
-                           "`copy_number_change`, `repeated_seq_expr`, "
-                           "`literal_seq_expr`. This parameter determines how to "
-                           "interpret HGVS dup/del expressions in VRS.")
+hgvs_dup_del_mode_decsr = ("Must be one of: `default`, `absolute_cnv`, `relative_cnv`, "
+                           "`repeated_seq_expr`, `literal_seq_expr`. This"
+                           " parameter determines how to interpret HGVS "
+                           "dup/del expressions in VRS.")
 
 
 @app.get("/variation/normalize",
          summary=normalize_summary,
          response_description=normalize_response_description,
          response_model=NormalizeService,
          description=normalize_description
          )
 async def normalize(
     q: str = Query(..., description=q_description),
     hgvs_dup_del_mode: Optional[HGVSDupDelModeEnum] = Query(
         HGVSDupDelModeEnum.DEFAULT, description=hgvs_dup_del_mode_decsr),
     baseline_copies: Optional[int] = Query(
-        None, description="Baseline copies for HGVS duplications and deletions represented as Copy Number Count Variation"),  # noqa: E501
-    copy_change: Optional[CopyChange] = Query(
-        None, description="The copy change for HGVS duplications and deletions represented as Copy Number Change Variation."),  # noqa: E501
+        None, description="Baseline copies for HGVS duplications and deletions represented as Absolute Copy Number Variation"),  # noqa: E501
+    relative_copy_class: Optional[RelativeCopyClass] = Query(
+        None, description="The relative copy class for HGVS duplications and deletions represented as Relative Copy Number Variation."),  # noqa: E501
     untranslatable_returns_text: bool = Query(False, description=untranslatable_descr)
 ) -> NormalizeService:
     """Normalize and translate a human readable variation description to a single
         VRSATILE Variation Descriptor. Performs fully-justified allele normalization.
         Will liftover to GRCh38 and aligns to a priority transcript. Will make
         inferences about the query.
 
     :param str q: Human readable variation description on GRCh37 or GRCh38 assembly
     :param Optional[HGVSDupDelModeEnum] hgvs_dup_del_mode:
-        Must be: `default`, `copy_number_count`, `copy_number_change`,
-        `repeated_seq_expr`, `literal_seq_expr`. This parameter determines how to
-        interpret HGVS dup/del expressions in VRS.
+        Must be: `default`, `absolute_cnv`, `relative_cnv`, `repeated_seq_expr`,
+        `literal_seq_expr`. This parameter determines how to interpret HGVS dup/del
+        expressions in VRS.
     :param Optional[int] baseline_copies: Baseline copies for HGVS duplications and
-        deletions. Required when `hgvs_dup_del_mode` is set to `copy_number_count`.
-    :param Optional[CopyChange] copy_change: The copy change
-        for HGVS duplications and deletions represented as Copy Number Change
-        Variation. If not set, will use default `copy_change` for query.
+        deletions. Required when `hgvs_dup_del_mode` is set to `absolute_cnv`.
+    :param Optional[RelativeCopyClass] relative_copy_class: The relative copy class
+        for HGVS duplications and deletions represented as Relative Copy Number
+        Variation. If not set, will use default `relative_copy_class` for query.
     :param bool untranslatable_returns_text: `True` return VRS Text Object when
         unable to translate or normalize query. `False` return `None` when
         unable to translate or normalize query.
     :return: NormalizeService for variation
     """
     normalize_resp = await query_handler.normalize_handler.normalize(
         unquote(q), hgvs_dup_del_mode=hgvs_dup_del_mode,
-        baseline_copies=baseline_copies, copy_change=copy_change,
+        baseline_copies=baseline_copies, relative_copy_class=relative_copy_class,
         untranslatable_returns_text=untranslatable_returns_text)
     return normalize_resp
 
 
 @app.get("/variation/translate_identifier",
          summary="Given an identifier, use SeqRepo to return a list of aliases.",
          response_description="A response to a validly-formed query.",
@@ -188,15 +188,15 @@
         separated by commas
     :return: TranslateIdentifierService data
     """
     aliases = []
     warnings = None
     identifier = identifier.strip()
     try:
-        aliases = query_handler._seqrepo_access.sr.translate_identifier(
+        aliases = query_handler._seqrepo_access.seqrepo_client.translate_identifier(
             identifier, target_namespaces=target_namespaces)
     except KeyError:
         warnings = [f"Identifier, {identifier}, does not exist in SeqRepo"]
     except Exception as e:
         warnings = [f"SeqRepo could not translate identifier, {identifier}:"
                     f" {e}"]
 
@@ -260,19 +260,19 @@
         ),
         vrs_python_meta_=VrsPythonMeta(
             version=pkg_resources.get_distribution("ga4gh.vrs").version
         )
     )
 
 
-g_to_p_summary = "Given GRCh38 gnomAD VCF, return VRSATILE object on MANE protein coordinate."  # noqa: E501
+g_to_p_summary = "Given gnomad VCF, return VRSATILE object on protein coordinate."
 g_to_p_response_description = "A response to a validly-formed query."
 g_to_p_description = \
     "Return VRSATILE object on protein coordinate for variation provided."
-q_description = "GRCh38 gnomAD VCF (chr-pos-ref-alt) to normalize to MANE protein variation."  # noqa: E501
+q_description = "gnomad VCF to normalize to protein variation."
 
 
 @app.get("/variation/gnomad_vcf_to_protein",
          summary=g_to_p_summary,
          response_description=g_to_p_response_description,
          description=g_to_p_description,
          response_model=NormalizeService,
@@ -297,20 +297,20 @@
 
 
 complement_descr = "This field indicates that a categorical variation is defined to " \
                    "include (false) or exclude (true) variation concepts matching " \
                    "the categorical variation."
 hgvs_dup_del_mode_decsr = "This parameter determines how to interpret HGVS dup/del "\
                           "expressions in VRS. Must be one of: `default`, " \
-                          "`copy_number_count`, `copy_number_change`, " \
-                          "`repeated_seq_expr`, `literal_seq_expr`."
-copy_change_descr = ("The copy change. Only used when `fmt`=`hgvs` and Copy Number "
-                     "Change Variation.")
+                          "`absolute_cnv`, `relative_cnv`, `repeated_seq_expr`, " \
+                          "`literal_seq_expr`."
+relative_copy_class_descr = "The relative copy class. Only used when `fmt`=`hgvs` "\
+                            "and Relative CNV."
 baseline_copies_descr = "Baseline copies for duplication or deletion. Only used when "\
-                        "`fmt`=`hgvs` and Copy Number Count Variation.`"
+                        "`fmt`=`hgvs` and Absolute CNV.`"
 
 
 @app.get("/variation/to_canonical_variation",
          summary="Given SPDI or HGVS, return VRSATILE Canonical Variation",
          response_description="A response to a validly-formed query.",
          description="Return VRSATILE Canonical Variation",
          response_model=ToCanonicalVariationService,
@@ -319,43 +319,43 @@
         q: str = Query(..., description="HGVS or SPDI query"),
         fmt: ToCanonicalVariationFmt = Query(...,
                                              description="Format of the input variation. Must be `spdi` or `hgvs`"),  # noqa: E501
         do_liftover: bool = Query(False, description="Whether or not to liftover to "
                                   "GRCh38 assembly."),
         hgvs_dup_del_mode: Optional[HGVSDupDelModeEnum] = Query(
             HGVSDupDelModeEnum.DEFAULT, description=hgvs_dup_del_mode_decsr),
-        copy_change: Optional[CopyChange] = Query(
-            None, description=copy_change_descr),
+        relative_copy_class: Optional[RelativeCopyClass] = Query(
+            None, description=relative_copy_class_descr),
         baseline_copies: Optional[int] = Query(
             None, description=baseline_copies_descr),
         untranslatable_returns_text: bool = Query(
             False, description=untranslatable_descr)
 ) -> ToCanonicalVariationService:
     """Return categorical variation for canonical SPDI
 
     :param str q: HGVS or SPDI query
     :param ToCanonicalVariationFmt fmt: Format of the input variation. Must be
         `spdi` or `hgvs`.
     :param Optional[HGVSDupDelModeEnum] hgvs_dup_del_mode: Determines how to interpret
-        HGVS dup/del expressions in VRS. Must be one of: `default`, `copy_number_count`,
-        `copy_number_change`, `repeated_seq_expr`, `literal_seq_expr`
-    :param Optional[CopyChange] copy_change: copy change.
-        Only used when `fmt`=`hgvs` and Copy Number Change Variation.
+        HGVS dup/del expressions in VRS. Must be one of: `default`, `absolute_cnv`,
+        `relative_cnv`, `repeated_seq_expr`, `literal_seq_expr`
+    :param Optional[RelativeCopyClass] relative_copy_class: Relative copy class.
+        Only used when `fmt`=`hgvs` and Relative CNV.
     :param Optional[int] baseline_copies: Baseline copies number
-        Only used when `fmt`=`hgvs` and Copy Number Count Variation
+        Only used when `fmt`=`hgvs` and Absolute CNV
     :param bool untranslatable_returns_text: `True` return VRS Text Object when
         unable to translate or normalize query. `False` return `None` when
         unable to translate or normalize query.
     :return: ToCanonicalVariationService for variation query
     """
     q = unquote(q)
     resp = await query_handler.to_canonical_handler.to_canonical_variation(
         q, fmt, do_liftover=do_liftover,
         hgvs_dup_del_mode=hgvs_dup_del_mode, baseline_copies=baseline_copies,
-        copy_change=copy_change,
+        relative_copy_class=relative_copy_class,
         untranslatable_returns_text=untranslatable_returns_text)
     return resp
 
 
 def _get_allele(request_body: Union[TranslateToQuery, TranslateToHGVSQuery],
                 warnings: List) -> Optional[models.Allele]:
     """Return VRS allele object from request body. `warnings` will get updated if
@@ -472,161 +472,161 @@
         ),
         vrs_python_meta_=VrsPythonMeta(
             version=pkg_resources.get_distribution("ga4gh.vrs").version
         )
     )
 
 
-@app.get("/variation/hgvs_to_copy_number_count",
-         summary="Given HGVS expression, return VRS Copy Number Count Variation",
+@app.get("/variation/hgvs_to_absolute_copy_number",
+         summary="Given HGVS expression, return VRS Absolute Copy Number Variation",
          response_description="A response to a validly-formed query.",
-         description="Return VRS Copy Number Count Variation",
-         response_model=HgvsToCopyNumberCountService,
+         description="Return VRS Absoluter Copy Number Variation",
+         response_model=HgvsToAbsoluteCopyNumberService,
          tags=[Tags.TO_COPY_NUMBER_VARIATION])
-async def hgvs_to_copy_number_count(
+async def hgvs_to_absolute_copy_number(
     hgvs_expr: str = Query(..., description="Variation query"),
     baseline_copies: Optional[int] = Query(
         None, description="Baseline copies for duplication"),
     do_liftover: bool = Query(False, description="Whether or not to liftover "
                               "to GRCh38 assembly."),
     untranslatable_returns_text: bool = Query(False, description=untranslatable_descr)
-) -> HgvsToCopyNumberCountService:
-    """Given hgvs expression, return copy number count variation
+) -> HgvsToAbsoluteCopyNumberService:
+    """Given hgvs expression, return absolute copy number variation
 
     :param str hgvs_expr: HGVS expression
     :param Optional[int] baseline_copies: Baseline copies number
     :param bool do_liftover: Whether or not to liftover to GRCh38 assembly
     :param bool untranslatable_returns_text: `True` return VRS Text Object when
         unable to translate or normalize query. `False` return `None` when
         unable to translate or normalize query.
-    :return: HgvsToCopyNumberCountService
+    :return: HgvsToAbsoluteCopyNumberService
     """
-    resp = await query_handler.to_copy_number_handler.hgvs_to_copy_number_count(
+    resp = await query_handler.to_copy_number_handler.hgvs_to_absolute_copy_number(
         unquote(hgvs_expr.strip()), baseline_copies, do_liftover,
         untranslatable_returns_text=untranslatable_returns_text)
     return resp
 
 
-@app.get("/variation/hgvs_to_copy_number_change",
-         summary="Given HGVS expression, return VRS Copy Number Change Variation",
+@app.get("/variation/hgvs_to_relative_copy_number",
+         summary="Given HGVS expression, return VRS Relative Copy Number Variation",
          response_description="A response to a validly-formed query.",
-         description="Return VRS Copy Number Change Variation",
-         response_model=HgvsToCopyNumberChangeService,
+         description="Return VRS Relative Copy Number Variation",
+         response_model=HgvsToRelativeCopyNumberService,
          tags=[Tags.TO_COPY_NUMBER_VARIATION])
-async def hgvs_to_copy_number_change(
+async def hgvs_to_relative_copy_number(
     hgvs_expr: str = Query(..., description="Variation query"),
-    copy_change: CopyChange = Query(
-        ..., description="The copy change"),
+    relative_copy_class: RelativeCopyClass = Query(
+        ..., description="The relative copy class"),
     do_liftover: bool = Query(False, description="Whether or not to liftover "
                               "to GRCh38 assembly."),
     untranslatable_returns_text: bool = Query(False, description=untranslatable_descr)
-) -> HgvsToCopyNumberChangeService:
-    """Given hgvs expression, return copy number change variation
+) -> HgvsToRelativeCopyNumberService:
+    """Given hgvs expression, return relative copy number variation
 
     :param str hgvs_expr: HGVS expression
-    :param CopyChange copy_change: copy change
+    :param RelativeCopyClass relative_copy_class: Relative copy class
     :param bool do_liftover: Whether or not to liftover to GRCh38 assembly
     :param bool untranslatable_returns_text: `True` return VRS Text Object when
         unable to translate or normalize query. `False` return `None` when
         unable to translate or normalize query.
-    :return: HgvsToCopyNumberChangeService
+    :return: HgvsToRelativeCopyNumberService
     """
-    resp = await query_handler.to_copy_number_handler.hgvs_to_copy_number_change(
-        unquote(hgvs_expr.strip()), copy_change, do_liftover,
+    resp = await query_handler.to_copy_number_handler.hgvs_to_relative_copy_number(
+        unquote(hgvs_expr.strip()), relative_copy_class, do_liftover,
         untranslatable_returns_text=untranslatable_returns_text)
     return resp
 
 
 assembly_descr = "Assembly. If `accession` is set, will ignore `assembly` and `chr`. "\
                  "If `accession` not set, must provide both `assembly` and `chr`."
 chr_descr = "Chromosome. Must set when `assembly` is set."
 accession_descr = "Accession. If `accession` is set, will ignore `assembly` and "\
                   "`chr`. If `accession` not set, must provide both `assembly` and `chr`."  # noqa: E501
 start_descr = "Start position as residue coordinate"
 end_descr = "End position as residue coordinate"
-total_copies_descr = "Total copies for Copy Number Count variation object"
+total_copies_descr = "Total copies for Absolute Copy Number variation object"
 
 
-@app.get("/variation/parsed_to_cn_var",
+@app.get("/variation/parsed_to_abs_cnv",
          summary="Given parsed ClinVar Copy Number Gain/Loss components, return "
-         "VRS Copy Number Count Variation",
+         "VRS Absolute Copy Number Variation",
          response_description="A response to a validly-formed query.",
-         description="Return VRS Copy Number Count Variation",
-         response_model=ParsedToCnVarService,
+         description="Return VRS Absolute Copy Number Variation",
+         response_model=ParsedToAbsCnvService,
          tags=[Tags.TO_COPY_NUMBER_VARIATION]
          )
-def parsed_to_cn_var(
+def parsed_to_abs_cnv(
     assembly: Optional[ClinVarAssembly] = Query(None, description=assembly_descr),
     chr: Optional[str] = Query(None, description=chr_descr),
     accession: Optional[str] = Query(None, description=accession_descr),
     start: int = Query(..., description=start_descr),
     end: int = Query(..., description=end_descr),
     total_copies: int = Query(..., description=total_copies_descr),
     untranslatable_returns_text: bool = Query(False, description=untranslatable_descr)
-) -> ParsedToCnVarService:
-    """Given parsed ClinVar Copy Number Gain/Loss components, return Copy Number Count
-    Variation
+) -> ParsedToAbsCnvService:
+    """Given parsed ClinVar Copy Number Gain/Loss components, return Absolute
+    Copy Number Variation
 
     :param int start: Start position as residue coordinate
     :param int end: End position as residue coordinate
-    :param int total_copies: Total copies for Copy Number Count variation object
+    :param int total_copies: Total copies for Absolute Copy Number variation object
     :param Optional[ClinVarAssembly] assembly: Assembly. If `accession` is set,
         will ignore `assembly` and `chr`. If `accession` not set, must provide
         both `assembly` and `chr`.
     :param Optional[str] chr: Chromosome. Must set when `assembly` is set.
     :param Optional[str] accession: Accession. If `accession` is set,
         will ignore `assembly` and `chr`. If `accession` not set, must provide
         both `assembly` and `chr`.
     :param bool untranslatable_returns_text: `True` return VRS Text Object when
         unable to translate or normalize query. `False` return `None` when
         unable to translate or normalize query.
-    :return: Tuple containing Copy Number Count variation and list of warnings
+    :return: Tuple containing Absolute Copy Number variation and list of warnings
     """
-    resp = query_handler.to_copy_number_handler.parsed_to_cn_var(
+    resp = query_handler.to_copy_number_handler.parsed_to_abs_cnv(
         start, end, total_copies, assembly, chr, accession,
         untranslatable_returns_text=untranslatable_returns_text)
     return resp
 
 
-amplification_to_cx_var_descr = ("Translate amplification to VRS Copy Number Change "
-                                 "Variation. If `sequence_id`, `start`, and `end` are "
-                                 "all provided, will return a SequenceLocation with "
-                                 "those properties. Else, gene-normalizer will be "
-                                 "used to retrieve the SequenceLocation.")
+amplification_to_rel_cnv_descr = ("Translate amplification to VRS Relative Copy Number "
+                                  "Variation. If `sequence_id`, `start`, and `end` are "
+                                  "all provided, will return a SequenceLocation with "
+                                  "those properties. Else, gene-normalizer will be "
+                                  "used to retrieve the SequenceLocation.")
 
 
-@app.get("/variation/amplification_to_cx_var",
-         summary="Given amplification query, return VRS Copy Number Change Variation",
+@app.get("/variation/amplification_to_rel_cnv",
+         summary="Given amplification query, return VRS Relative Copy Number Variation",
          response_description="A response to a validly-formed query.",
-         description=amplification_to_cx_var_descr,
-         response_model=AmplificationToCxVarService,
+         description=amplification_to_rel_cnv_descr,
+         response_model=AmplificationToRelCnvService,
          tags=[Tags.TO_COPY_NUMBER_VARIATION])
-def amplification_to_cx_var(
+def amplification_to_rel_cnv(
     gene: str = Query(..., description="Gene query"),
     sequence_id: Optional[str] = Query(None, description="Sequence identifier"),
     start: Optional[int] = Query(None,
                                  description="Start position as residue coordinate"),
     end: Optional[int] = Query(None, description="End position as residue coordinate"),
     untranslatable_returns_text: bool = Query(False, description=untranslatable_descr)
-) -> AmplificationToCxVarService:
-    """Given amplification query, return Copy Number Change Variation
+) -> AmplificationToRelCnvService:
+    """Given amplification query, return Relative Copy Number Variation
     Parameter priority:
         1. sequence_id, start, end (must provide ALL)
         2. use the gene-normalizer to get the SequenceLocation
 
     :param str gene: Gene query
     :param Optional[str] sequence_id: Sequence ID for the location. If set,
         must also provide `start` and `end`
     :param Optional[int] start: Start position as residue coordinate for the sequence
         location. If set, must also provide `sequence_id` and `end`
     :param Optional[int] end: End position as residue coordinate for the sequence
         location. If set, must also provide `sequence_id` and `start`
     :param bool untranslatable_returns_text: `True` return VRS Text Object when
         unable to translate or normalize query. `False` return `None` when
         unable to translate or normalize query.
-    :return: AmplificationToCxVarService containing Copy Number Change and
+    :return: AmplificationToRelCnvService containing Relative Copy Number and
         list of warnings
     """
-    resp = query_handler.to_copy_number_handler.amplification_to_cx_var(
+    resp = query_handler.to_copy_number_handler.amplification_to_rel_cnv(
         gene=gene, sequence_id=sequence_id, start=start, end=end,
         untranslatable_returns_text=untranslatable_returns_text)
     return resp
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/normalize.py` & `variation-normalizer-0.7.dev0/variation/normalize.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,72 +1,74 @@
 """Module for Variation Normalization."""
 from typing import Optional
 from urllib.parse import quote
 from datetime import datetime
 
 from gene.query import QueryHandler as GeneQueryHandler
-from cool_seq_tool.data_sources import SeqRepoAccess, UTADatabase
+from uta_tools.data_sources import SeqRepoAccess, UTADatabase
+from ga4gh.vrs.dataproxy import SeqRepoDataProxy
 
 from variation.classifiers.classify import Classify
 from variation.to_vrsatile import ToVRSATILE
 from variation.hgvs_dup_del_mode import HGVSDupDelMode
 from variation.tokenizers.tokenize import Tokenize
 from variation.translators.translate import Translate
 from variation.utils import get_mane_valid_result, no_variation_entered, \
     no_variation_resp
 from variation.validators.validate import Validate
 from variation.schemas.app_schemas import Endpoint
 from variation.schemas.normalize_response_schema\
     import HGVSDupDelMode as HGVSDupDelModeEnum, NormalizeService, ServiceMeta
-from variation.schemas.hgvs_to_copy_number_schema import CopyChange
+from variation.schemas.hgvs_to_copy_number_schema import RelativeCopyClass
 from variation.version import __version__
 
 
 class Normalize(ToVRSATILE):
     """The Normalize class used to normalize a given variation."""
 
-    def __init__(self, seqrepo_access: SeqRepoAccess,
+    def __init__(self, seqrepo_access: SeqRepoAccess, dp: SeqRepoDataProxy,
                  tokenizer: Tokenize, classifier: Classify, validator: Validate,
                  translator: Translate, hgvs_dup_del_mode: HGVSDupDelMode,
                  gene_normalizer: GeneQueryHandler, uta: UTADatabase) -> None:
         """Initialize Normalize class.
 
-        :param SeqRepoAccess seqrepo_access: Access to SeqRepo
+        :param SeqRepoAccess seqrepo_access: Access to SeqRepo via UTA Tools
+        :param SeqRepoDataProxy dp: Access to SeqRepo via VRS Python
         :param Tokenize tokenizer: Tokenizer class for tokenizing
         :param Classify classifier: Classifier class for classifying tokens
         :param Validate validator: Validator class for validating valid inputs
         :param Translate translator: Translating valid inputs
         :param HGVSDupDelMode hgvs_dup_del_mode: Class for handling
             HGVS dup/del expressions
         :parm GeneQueryHandler gene_normalizer: Client for normalizing gene concepts
         :param UTADatabase uta: Access to db containing alignment data
         """
-        super().__init__(seqrepo_access, tokenizer, classifier, validator,
+        super().__init__(seqrepo_access, dp, tokenizer, classifier, validator,
                          translator, hgvs_dup_del_mode, gene_normalizer)
         self.uta = uta
 
     async def normalize(
         self, q: str,
         hgvs_dup_del_mode: Optional[HGVSDupDelModeEnum] = HGVSDupDelModeEnum.DEFAULT,
         baseline_copies: Optional[int] = None,
-        copy_change: Optional[CopyChange] = None,
+        relative_copy_class: Optional[RelativeCopyClass] = None,
         untranslatable_returns_text: bool = False
     ) -> NormalizeService:
         """Normalize a given variation.
 
         :param str q: The variation to normalize
         :param Optional[HGVSDupDelModeEnum] hgvs_dup_del_mode:
             Must be set when querying HGVS dup/del expressions.
-            Must be: `default`, `copy_number_count`, `copy_number_change`,
-            `repeated_seq_expr`, `literal_seq_expr`. This parameter determines how to
-            interpret HGVS dup/del expressions in VRS.
+            Must be: `default`, `absolute_cnv`, `relative_cnv`, `repeated_seq_expr`,
+            `literal_seq_expr`. This parameter determines how to interpret HGVS dup/del
+            expressions in VRS.
         :param Optional[int] baseline_copies: Baseline copies for HGVS duplications and
             deletions
-        :param Optional[CopyChange] copy_change: The copy change
-            for HGVS duplications and deletions represented as Copy Number Change
+        :param Optional[RelativeCopyClass] relative_copy_class: The relative copy class
+            for HGVS duplications and deletions represented as Relative Copy Number
             Variation.
         :param bool untranslatable_returns_text: `True` return VRS Text Object when
             unable to translate or normalize query. `False` return `None` when
             unable to translate or normalize query.
         :return: NormalizeService with variation descriptor and warnings
         """
         vd = None
@@ -74,15 +76,15 @@
         if not q:
             vd, warnings = no_variation_entered()
         else:
             validations, warnings = await self.get_validations(
                 q, endpoint_name=Endpoint.NORMALIZE,
                 hgvs_dup_del_mode=hgvs_dup_del_mode,
                 baseline_copies=baseline_copies,
-                copy_change=copy_change)
+                relative_copy_class=relative_copy_class)
 
             if validations:
                 label = q.strip()
                 _id = f"normalize.variation:{quote(' '.join(label.split()))}"
                 if len(validations.valid_results) > 0:
                     valid_result = get_mane_valid_result(q, validations, warnings)
                     vd, warnings = self.get_variation_descriptor(
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/query.py` & `variation-normalizer-0.7.dev0/variation/query.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """This module provides methods for handling queries."""
 from typing import Optional
 from os import environ
 
 from gene.query import QueryHandler as GeneQueryHandler
+from ga4gh.vrs.dataproxy import SeqRepoDataProxy
 from ga4gh.vrs.extras.translator import Translator
-from cool_seq_tool import TRANSCRIPT_MAPPINGS_PATH, LRG_REFSEQGENE_PATH, \
-    MANE_SUMMARY_PATH, CoolSeqTool
+from uta_tools import SEQREPO_DATA_PATH, TRANSCRIPT_MAPPINGS_PATH, \
+    LRG_REFSEQGENE_PATH, MANE_SUMMARY_PATH, UTATools
 
-from variation import UTA_DB_URL
+from variation import AMINO_ACID_PATH, UTA_DB_URL
 from variation.tokenizers import GeneSymbol
+from variation.tokenizers.caches import AminoAcidCache
 from variation.hgvs_dup_del_mode import HGVSDupDelMode
 from variation.to_vrs import VRSRepresentation, ToVRS
 from variation.classifiers import Classify
 from variation.tokenizers import Tokenize
 from variation.validators import Validate
 from variation.translators import Translate
 from variation.data_sources import CodonTable
@@ -22,80 +24,79 @@
 from variation.to_canonical_variation import ToCanonicalVariation
 from variation.to_copy_number_variation import ToCopyNumberVariation
 
 
 class QueryHandler:
     """Class for initializing handlers that make app queries."""
 
-    def __init__(
-        self, dynamodb_url: str = "", dynamodb_region: str = "us-east-2",
-        gene_query_handler: Optional[GeneQueryHandler] = None,
-        transcript_file_path: str = None, refseq_file_path: str = None,
-        mane_data_path: str = None, uta_db_url: str = UTA_DB_URL,
-        uta_db_pwd: Optional[str] = None
-    ) -> None:
+    def __init__(self,
+                 dynamodb_url: str = "",
+                 dynamodb_region: str = "us-east-2",
+                 seqrepo_data_path: str = None,
+                 amino_acids_file_path: str = AMINO_ACID_PATH,
+                 transcript_file_path: str = None,
+                 refseq_file_path: str = None,
+                 mane_data_path: str = None,
+                 uta_db_url: str = UTA_DB_URL,
+                 uta_db_pwd: Optional[str] = None) -> None:
         """Initialize QueryHandler instance.
-        :param str dynamodb_url: URL to gene normalizer dynamodb. Only used when
-            `gene_query_handler` is `None`.
-        :param str dynamodb_region: AWS region for gene normalizer db. Only used when
-            `gene_query_handler` is `None`.
-        :param Optional[GeneQueryHandler] gene_query_handler: Gene normalizer query
-            handler instance. If this is provided, will use a current instance. If this
-            is not provided, will create a new instance.
+        :param str dynamodb_url: URL to gene-normalizer database source.
+        :param str dynamodb_region: AWS default region for gene-normalizer.
+        :param str seqrepo_data_path: Path to seqrepo data directory
+        :param str amino_acids_file_path: Path to amino acids file
         :param str transcript_file_path: Path to transcript mappings file
         :param str refseq_file_path: Path to refseq gene symbol file
         :param str mane_data_path: Path to refseq mane data file
         :param str uta_db_url: URL for UTA database
         :param Optional[str] uta_db_pwd: Password for UTA database user
         """
+        if not seqrepo_data_path:
+            seqrepo_data_path = environ.get("SEQREPO_DATA_PATH", SEQREPO_DATA_PATH)
         if not transcript_file_path:
             transcript_file_path = environ.get("TRANSCRIPT_MAPPINGS_PATH",
                                                TRANSCRIPT_MAPPINGS_PATH)
         if not refseq_file_path:
             refseq_file_path = environ.get("LRG_REFSEQGENE_PATH", LRG_REFSEQGENE_PATH)
-
         if not mane_data_path:
             mane_data_path = environ.get("MANE_SUMMARY_PATH", MANE_SUMMARY_PATH)
-
-        cool_seq_tool = CoolSeqTool(
-            transcript_file_path=transcript_file_path,
-            lrg_refseqgene_path=refseq_file_path,
-            mane_data_path=mane_data_path,
-            db_url=uta_db_url,
-            db_pwd=uta_db_pwd,
-            gene_query_handler=gene_query_handler,
-            gene_db_url=dynamodb_url,
-            gene_db_region=dynamodb_region
-        )
-        self._seqrepo_access = cool_seq_tool.seqrepo_access
-        gene_query_handler = cool_seq_tool.gene_query_handler
-
-        vrs_representation = VRSRepresentation(self._seqrepo_access)
-        gene_symbol = GeneSymbol(gene_query_handler)
-        tokenizer = Tokenize(gene_symbol)
+        uta_tools = UTATools(seqrepo_data_path=seqrepo_data_path,
+                             transcript_file_path=transcript_file_path,
+                             lrg_refseqgene_path=refseq_file_path,
+                             mane_data_path=mane_data_path,
+                             db_url=uta_db_url, db_pwd=uta_db_pwd)
+        self._seqrepo_access = uta_tools.seqrepo_access
+
+        dp = SeqRepoDataProxy(self._seqrepo_access.seqrepo_client)
+
+        vrs_representation = VRSRepresentation(dp, self._seqrepo_access)
+
+        amino_acid_cache = AminoAcidCache(amino_acids_file_path=amino_acids_file_path)
+        gene_normalizer = GeneQueryHandler(db_url=dynamodb_url,
+                                           db_region=dynamodb_region)
+        gene_symbol = GeneSymbol(gene_normalizer)
+        tokenizer = Tokenize(amino_acid_cache, gene_symbol)
         classifier = Classify()
-        uta_db = cool_seq_tool.uta_db
-        mane_transcript = cool_seq_tool.mane_transcript
-        transcript_mappings = cool_seq_tool.transcript_mappings
-        self._tlr = Translator(data_proxy=self._seqrepo_access)
+        uta_db = uta_tools.uta_db
+        mane_transcript = uta_tools.mane_transcript
+        transcript_mappings = uta_tools.transcript_mappings
+        self._tlr = Translator(data_proxy=dp)
         validator = Validate(
             self._seqrepo_access, transcript_mappings, gene_symbol, mane_transcript,
-            uta_db, self._tlr, gene_query_handler, vrs_representation
+            uta_db, self._tlr, amino_acid_cache, gene_normalizer, vrs_representation
         )
         translator = Translate()
         hgvs_dup_del_mode = HGVSDupDelMode(self._seqrepo_access)
-        to_vrs_params = [self._seqrepo_access, tokenizer,
-                         classifier, validator, translator, hgvs_dup_del_mode,
-                         gene_query_handler]
+        to_vrs_params = [self._seqrepo_access, dp, tokenizer, classifier, validator,
+                         translator, hgvs_dup_del_mode, gene_normalizer]
         self.to_vrs_handler = ToVRS(*to_vrs_params)
         self.to_vrsatile_handler = ToVRSATILE(*to_vrs_params)
         self.normalize_handler = Normalize(*to_vrs_params + [uta_db])
 
-        codon_table = CodonTable()
-        mane_transcript_mappings = cool_seq_tool.mane_transcript_mappings
+        codon_table = CodonTable(amino_acid_cache)
+        mane_transcript_mappings = uta_tools.mane_transcript_mappings
         to_protein_params = to_vrs_params + [uta_db,
                                              mane_transcript, mane_transcript_mappings,
                                              codon_table]
         self.gnomad_vcf_to_protein_handler = GnomadVcfToProteinVariation(
             *to_protein_params)
         self.to_canonical_handler = ToCanonicalVariation(
             *to_vrs_params + [self._tlr, uta_db])
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/schemas/classification_response_schema.py` & `variation-normalizer-0.7.dev0/variation/schemas/classification_response_schema.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/schemas/hgvs_to_copy_number_schema.py` & `variation-normalizer-0.7.dev0/variation/schemas/hgvs_to_copy_number_schema.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,51 +1,52 @@
 """Module containing schemas used in HGVS To Copy Number endpoints"""
 from typing import Optional, Type, Any, Dict, Union
 
-from ga4gh.vrsatile.pydantic.vrs_models import CopyChange, CopyNumberCount, \
-    CopyNumberChange, Text
+from ga4gh.vrsatile.pydantic.vrs_models import RelativeCopyClass, AbsoluteCopyNumber, \
+    RelativeCopyNumber, Text
 from pydantic import StrictStr
 
 from variation.schemas.classification_response_schema import ClassificationType
 from variation.schemas.normalize_response_schema import ServiceResponse
 
 
 VALID_CLASSIFICATION_TYPES = [
     ClassificationType.GENOMIC_DUPLICATION,
     ClassificationType.GENOMIC_DELETION,
     ClassificationType.GENOMIC_DELETION_RANGE,
     ClassificationType.GENOMIC_UNCERTAIN_DELETION
 ]
 
-VALID_COPY_CHANGE = [rcc.value for rcc in CopyChange.__members__.values()]
+VALID_RELATIVE_COPY_CLASS = [rcc.value for
+                             rcc in RelativeCopyClass.__members__.values()]
 
 
-class HgvsToCopyNumberCountService(ServiceResponse):
-    """A response for translating HGVS to copy number count."""
+class HgvsToAbsoluteCopyNumberService(ServiceResponse):
+    """A response for translating HGVS to absolute copy number."""
 
     hgvs_expr: StrictStr
-    copy_number_count: Optional[Union[CopyNumberCount, Text]]
+    absolute_copy_number: Optional[Union[AbsoluteCopyNumber, Text]]
 
     class Config:
         """Configure model."""
 
         @staticmethod
         def schema_extra(schema: Dict[str, Any],
-                         model: Type["HgvsToCopyNumberCountService"]) -> None:
+                         model: Type["HgvsToAbsoluteCopyNumberService"]) -> None:
             """Configure OpenAPI schema."""
             if "title" in schema.keys():
                 schema.pop("title", None)
             for prop in schema.get("properties", {}).values():
                 prop.pop("title", None)
             schema["example"] = {
                 "hgvs_expr": "NC_000003.12:g.49531262dup",
-                "copy_number_count": {
-                    "id": "ga4gh:CN._qniTzHEtNOc6CNjb5bhlV5bf527692Q",
-                    "type": "CopyNumberCount",
-                    "subject": {
+                "absolute_copy_number": {
+                    "id": "ga4gh:ACN._C6yp4SRGVfuRmMiJShIKYCK3dSX0vNF",
+                    "type": "AbsoluteCopyNumber",
+                    "location": {
                         "id": "ga4gh:SL.KefUQwlqEBGtzoNO-MzOozx7_H1uP-fD",
                         "type": "SequenceLocation",
                         "sequence_id": "ga4gh:SQ.Zu7h9AggXxhTaGVsy7h_EZSChSZGcmgX",
                         "start": {"type": "Number", "value": 49531260},
                         "end": {"type": "Number", "value": 49531262}
                     },
                     "copies": {"type": "Number", "value": 3}
@@ -55,44 +56,44 @@
                     "version": "0.2.17",
                     "response_datetime": "2022-01-26T22:23:41.821673",
                     "url": "https://github.com/cancervariants/variation-normalization"
                 }
             }
 
 
-class HgvsToCopyNumberChangeService(ServiceResponse):
-    """A response for translating HGVS to copy number change."""
+class HgvsToRelativeCopyNumberService(ServiceResponse):
+    """A response for translating HGVS to relative copy number."""
 
     hgvs_expr: StrictStr
-    copy_number_change: Optional[Union[CopyNumberChange, Text]]
+    relative_copy_number: Optional[Union[RelativeCopyNumber, Text]]
 
     class Config:
         """Configure model."""
 
         @staticmethod
         def schema_extra(schema: Dict[str, Any],
-                         model: Type["HgvsToCopyNumberChangeService"]) -> None:
+                         model: Type["HgvsToRelativeCopyNumberService"]) -> None:
             """Configure OpenAPI schema."""
             if "title" in schema.keys():
                 schema.pop("title", None)
             for prop in schema.get("properties", {}).values():
                 prop.pop("title", None)
             schema["example"] = {
                 "hgvs_expr": "NC_000003.12:g.49531262dup",
-                "copy_number_change": {
-                    "id": "ga4gh:CX.ENQD2_J-4FE964fFrO9cjBDBee09ORWH",
-                    "type": "CopyNumberChange",
-                    "subject": {
+                "relative_copy_number": {
+                    "id": "ga4gh:RCN._1Nz0yj2g9Q6cRO8j6oRi5peUJYjTAga",
+                    "type": "RelativeCopyNumber",
+                    "location": {
                         "id": "ga4gh:SL.KefUQwlqEBGtzoNO-MzOozx7_H1uP-fD",
                         "type": "SequenceLocation",
                         "sequence_id": "ga4gh:SQ.Zu7h9AggXxhTaGVsy7h_EZSChSZGcmgX",
                         "start": {"type": "Number", "value": 49531260},
                         "end": {"type": "Number", "value": 49531262}
                     },
-                    "copy_change": "efo:0030069"
+                    "relative_copy_class": "complete loss"
                 },
                 "service_meta_": {
                     "name": "variation-normalizer",
                     "version": "0.2.17",
                     "response_datetime": "2022-01-26T22:23:41.821673",
                     "url": "https://github.com/cancervariants/variation-normalization"
                 }
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/schemas/normalize_response_schema.py` & `variation-normalizer-0.7.dev0/variation/schemas/normalize_response_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 
 class HGVSDupDelMode(str, Enum):
     """Define options for HGVSDupDelMode.
     This mode determines how to interpret HGVS dup/del.
     """
 
     DEFAULT = "default"
-    COPY_NUMBER_COUNT = "copy_number_count"
-    COPY_NUMBER_CHANGE = "copy_number_change"
+    ABSOLUTE_CNV = "absolute_cnv"
+    RELATIVE_CNV = "relative_cnv"
     REPEATED_SEQ_EXPR = "repeated_seq_expr"  # VRS Allele
     LITERAL_SEQ_EXPR = "literal_seq_expr"  # VRS Allele
 
 
 class ServiceMeta(BaseModel):
     """Metadata regarding the variation-normalization service."""
 
@@ -250,15 +250,15 @@
                 schema.pop("title", None)
             for prop in schema.get("properties", {}).values():
                 prop.pop("title", None)
             schema["example"] = {
                 "query": "NC_000007.14:140753335:A:T",
                 "warnings": [],
                 "canonical_variation": {
-                    "id": "ga4gh:CAN.dP6z4p7SoGJFmlFQcjOQo2d1mXuo1QiY",
+                    "id": "ga4gh:CLV.dP6z4p7SoGJFmlFQcjOQo2d1mXuo1QiY",
                     "type": "CanonicalVariation",
                     "canonical_context": {
                         "id": "ga4gh:VA.3xFHF399HGbG1JUf5uwcj3oWVKZJ70oX",
                         "type": "Allele",
                         "location": {
                             "id": "ga4gh:SL.WBLxdkoypnRME6b8tJtlOWqZKU1ruqY1",
                             "type": "SequenceLocation",
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/schemas/service_schema.py` & `variation-normalizer-0.7.dev0/variation/schemas/service_schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Module containing schemas for services"""
 from enum import Enum
 from typing import Optional, Union, Dict, Any, Type
 
 from pydantic import BaseModel, StrictStr
-from ga4gh.vrsatile.pydantic.vrs_models import CopyNumberCount, Text, \
-    SequenceLocation, CopyNumberChange
+from ga4gh.vrsatile.pydantic.vrs_models import AbsoluteCopyNumber, Text, \
+    SequenceLocation, RelativeCopyNumber
 
 from variation.schemas.normalize_response_schema import ServiceResponse
 
 
 class ClinVarAssembly(str, Enum):
     """Define assemblies in ClinVar"""
 
@@ -16,55 +16,55 @@
     GRCH37 = "GRCh37"
     NCBI36 = "NCBI36"
     HG38 = "hg38"
     HG19 = "hg19"
     HG18 = "hg18"
 
 
-class ParsedToCnVarQuery(BaseModel):
-    """Define query for parsed to copy number count variation endpoint"""
+class ParsedToAbsCnvQuery(BaseModel):
+    """Define query for parsed to abs cnv endpoint"""
 
     assembly: Optional[ClinVarAssembly] = None
     chr: Optional[StrictStr] = None
     accession: Optional[StrictStr] = None
     start: int
     end: int
     total_copies: int
 
 
-class ParsedToCnVarService(ServiceResponse):
-    """A response for translating parsed components to Copy Number Count"""
+class ParsedToAbsCnvService(ServiceResponse):
+    """A response for translating parsed components to Absolute Copy Number"""
 
-    query: Optional[ParsedToCnVarQuery] = None
-    copy_number_count: Optional[Union[Text, CopyNumberCount]]
+    query: Optional[ParsedToAbsCnvQuery] = None
+    absolute_copy_number: Optional[Union[Text, AbsoluteCopyNumber]]
 
     class Config:
         """Configure model."""
 
         @staticmethod
         def schema_extra(schema: Dict[str, Any],
-                         model: Type["ParsedToCnVarService"]) -> None:
+                         model: Type["ParsedToAbsCnvService"]) -> None:
             """Configure OpenAPI schema."""
             if "title" in schema.keys():
                 schema.pop("title", None)
             for prop in schema.get("properties", {}).values():
                 prop.pop("title", None)
             schema["example"] = {
                 "query": {
                     "assembly": "GRCh37",
                     "chr": "1",
                     "accession": None,
                     "start": 143134063,
                     "end": 143284670,
                     "total_copies": 3
                 },
-                "copy_number_count": {
-                    "id": "ga4gh:CN._IYaKE4CoDa01tkcgOuqPhnYbZ5RuPcj",
-                    "type": "CopyNumberCount",
-                    "subject": {
+                "absolute_copy_number": {
+                    "id": "ga4gh:ACN.cbjEAj7SGM_RPXxs7foqsO0ZsNwz_kNM",
+                    "type": "AbsoluteCopyNumber",
+                    "location": {
                         "id": "ga4gh:SL.RIgksXkT_kWCJv3poK4WQ9PK5_YSRBuh",
                         "type": "SequenceLocation",
                         "sequence_id": "ga4gh:SQ.S_KjnFVz-FE7M0W6yoaUDgYxLPc1jyWU",
                         "start": {
                             "type": "IndefiniteRange",
                             "value": 143134062,
                             "comparator": "<="
@@ -82,62 +82,62 @@
                     "version": "0.2.17",
                     "response_datetime": "2022-01-26T22:23:41.821673",
                     "url": "https://github.com/cancervariants/variation-normalization"
                 }
             }
 
 
-class AmplificationToCxVarQuery(BaseModel):
-    """Define query for amplification to copy number change variation endpoint"""
+class AmplificationToRelCnvQuery(BaseModel):
+    """Define query for amplification to relative copy number variation endpoint"""
 
     gene: str
     sequence_id: Optional[str]
     start: Optional[int]
     end: Optional[int]
     sequence_location: Optional[SequenceLocation]
 
 
-class AmplificationToCxVarService(ServiceResponse):
-    """A response for translating Amplification queries to Copy Number Change"""
+class AmplificationToRelCnvService(ServiceResponse):
+    """A response for translating Amplification queries to Relative Copy Number"""
 
-    query: Optional[AmplificationToCxVarQuery] = None
+    query: Optional[AmplificationToRelCnvQuery] = None
     amplification_label: Optional[str]
-    copy_number_change: Optional[Union[Text, CopyNumberChange]]
+    relative_copy_number: Optional[Union[Text, RelativeCopyNumber]]
 
     class Config:
         """Configure model."""
 
         @staticmethod
         def schema_extra(schema: Dict[str, Any],
-                         model: Type["AmplificationToCxVarService"]) -> None:
+                         model: Type["AmplificationToRelCnvService"]) -> None:
             """Configure OpenAPI schema."""
             if "title" in schema.keys():
                 schema.pop("title", None)
             for prop in schema.get("properties", {}).values():
                 prop.pop("title", None)
             schema["example"] = {
                 "query": {
                     "gene": "braf",
                     "sequence_id": None,
                     "start": None,
                     "end": None,
                     "sequence_location": None
                 },
                 "amplification_label": "BRAF Amplification",
-                "copy_number_change": {
-                    "id": "ga4gh:CX.1RJp1zW60x2t4Exc4965_a3CvYFtsL4q",
-                    "type": "CopyNumberChange",
-                    "subject": {
+                "relative_copy_number": {
+                    "id": "ga4gh:RCN.avsI73-9i6ykDIRB3eB89jeU1lhyBbYt",
+                    "type": "RelativeCopyNumber",
+                    "location": {
                         "id": "ga4gh:SL.po-AExwyqkstDx3JWYn6plIlxn5eojv4",
                         "type": "SequenceLocation",
                         "sequence_id": "ga4gh:SQ.F-LrLMe1SRpfUZHkQmvkVKFEGaoDeHul",
                         "start": {"type": "Number", "value": 140713327},
                         "end": {"type": "Number", "value": 140924929}
                     },
-                    "copy_change": "efo:0030072"
+                    "relative_copy_class": "high-level gain"
                 },
                 "service_meta_": {
                     "version": "0.7.dev0",
                     "response_datetime": "2022-09-29T15:08:18.696882",
                     "name": "variation-normalizer",
                     "url": "https://github.com/cancervariants/variation-normalization"
                 }
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/schemas/to_vrs_response_schema.py` & `variation-normalizer-0.7.dev0/variation/schemas/to_vrs_response_schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """Module for to_vrs endpoint response schema."""
 from typing import List, Dict, Type, Any, Optional, Union
 
 from pydantic import BaseModel
 from pydantic.types import StrictStr
 from ga4gh.vrsatile.pydantic.vrs_models import Allele, Text, Haplotype, \
-    CopyNumberCount, VariationSet, CopyNumberChange
+    AbsoluteCopyNumber, VariationSet, RelativeCopyNumber
 
 from variation.schemas.normalize_response_schema import ServiceMeta
 
 
 class ToVRSService(BaseModel):
     """Define model for translation response."""
 
     search_term: StrictStr
     warnings: Optional[List[StrictStr]]
     variations: Optional[Union[List[Allele], List[Text], List[Haplotype],
-                               List[CopyNumberCount], List[CopyNumberChange],
+                               List[AbsoluteCopyNumber], List[RelativeCopyNumber],
                                List[VariationSet]]]
     service_meta_: ServiceMeta
 
     class Config:
         """Configure model."""
 
         @staticmethod
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/schemas/token_response_schema.py` & `variation-normalizer-0.7.dev0/variation/schemas/token_response_schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,14 +107,57 @@
                 "match_type": 2,
                 "input_string": "BRAF",
                 "object_type": "Token",
                 "matched_value": "BRAF"
             }
 
 
+class GenePairMatchToken(Token):
+    """Define model for gene pair token."""
+
+    left_gene_token: GeneMatchToken
+    right_gene_token: GeneMatchToken
+    token_type = "GenePair"
+
+    class Config:
+        """Configure model."""
+
+        @staticmethod
+        def schema_extra(schema: Dict[str, Any],
+                         model: Type["GenePairMatchToken"]) -> None:
+            """Configure OpenAPI schema."""
+            if "title" in schema.keys():
+                schema.pop("title", None)
+            for prop in schema.get("properties", {}).values():
+                prop.pop("title", None)
+            schema["example"] = {
+                "token": "BRAF-ABL1",
+                "token_type": "GenePair",
+                "match_type": 5,
+                "input_string": "braf-abl1",
+                "object_type": "Token",
+                "left_gene_token": {
+                    "token": "BRAF",
+                    "token_type": "GeneSymbol",
+                    "match_type": 2,
+                    "input_string": "BRAF",
+                    "object_type": "Token",
+                    "matched_value": "BRAF"
+                },
+                "right_gene_token": {
+                    "token": "ABL1",
+                    "token_type": "GeneSymbol",
+                    "match_type": 2,
+                    "input_string": "ABL1",
+                    "object_type": "Token",
+                    "matched_value": "ABL1"
+                }
+            }
+
+
 class CoordinateType(str, Enum):
     """Define constraints for coordinate types."""
 
     CODING_DNA = "c"
     LINEAR_GENOMIC = "g"
     PROTEIN = "p"
 
@@ -228,23 +271,17 @@
             }
 
 
 class TokenResponseSchema(BaseModel):
     """Define model for token response."""
 
     search_term: str
-    tokens: List[
-        Union[
-            GeneMatchToken,
-            ProteinSubstitutionToken,
-            PolypeptideTruncationToken,
-            SilentMutationToken,
-            Token
-        ]
-    ]
+    tokens: List[Union[GeneMatchToken, GenePairMatchToken,
+                       ProteinSubstitutionToken, PolypeptideTruncationToken,
+                       SilentMutationToken, Token]]
 
     class Config:
         """Configure model."""
 
         @staticmethod
         def schema_extra(schema: Dict[str, Any],
                          model: Type["TokenResponseSchema"]) -> None:
@@ -468,15 +505,14 @@
     """A sequence change between the translation initiation (start) and
     termination (stop) codon where, compared to a reference sequence, one or
     more amino acids are not present (deleted) - varnomen.hgvs.org
     """
 
     start_aa_del: str
     end_aa_del: Optional[str]
-    deleted_aa: Optional[str]
     coordinate_type = CoordinateType.PROTEIN
     token_type = "ProteinDeletion"
     so_id = SequenceOntology.PROTEIN_DELETION
     molecule_context = "protein"
 
 
 class CodingDNADeletionToken(Deletion):
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/schemas/validation_response_schema.py` & `variation-normalizer-0.7.dev0/variation/schemas/validation_response_schema.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/schemas/vrs_python_translator_schema.py` & `variation-normalizer-0.7.dev0/variation/schemas/vrs_python_translator_schema.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/to_canonical_variation.py` & `variation-normalizer-0.7.dev0/variation/to_canonical_variation.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,80 +3,81 @@
 from datetime import datetime
 
 import python_jsonschema_objects
 from ga4gh.vrsatile.pydantic.vrs_models import Text, VRSTypes
 from ga4gh.vrsatile.pydantic.vrsatile_models import CanonicalVariation
 from ga4gh.vrs import models
 from ga4gh.core import ga4gh_identify
+from ga4gh.vrs.dataproxy import SeqRepoDataProxy
 from ga4gh.vrs.extras.translator import Translator
-from cool_seq_tool.schemas import Assembly
-from cool_seq_tool.data_sources import UTADatabase, SeqRepoAccess
+from uta_tools.schemas import Assembly
+from uta_tools.data_sources import UTADatabase, SeqRepoAccess
 from gene.query import QueryHandler as GeneQueryHandler
 
 from variation.classifiers.classify import Classify
 from variation.hgvs_dup_del_mode import HGVSDupDelMode
 from variation.schemas.app_schemas import Endpoint
 from variation.schemas.normalize_response_schema import ServiceMeta, \
     ToCanonicalVariationFmt, ToCanonicalVariationService
 from variation.schemas.normalize_response_schema\
     import HGVSDupDelMode as HGVSDupDelModeEnum
-from variation.schemas.hgvs_to_copy_number_schema import VALID_COPY_CHANGE,\
-    CopyChange
+from variation.schemas.hgvs_to_copy_number_schema import VALID_RELATIVE_COPY_CLASS,\
+    RelativeCopyClass
 from variation.to_vrs import ToVRS
 from variation.tokenizers.tokenize import Tokenize
 from variation.translators.translate import Translate
 from variation.utils import get_mane_valid_result, no_variation_entered
 from variation.validators.validate import Validate
 from variation.version import __version__
 
 
 class ToCanonicalVariation(ToVRS):
     """Class for translating to canonical variation"""
 
-    def __init__(self, seqrepo_access: SeqRepoAccess,
+    def __init__(self, seqrepo_access: SeqRepoAccess, dp: SeqRepoDataProxy,
                  tokenizer: Tokenize, classifier: Classify, validator: Validate,
                  translator: Translate, hgvs_dup_del_mode: HGVSDupDelMode,
                  gene_normalizer: GeneQueryHandler,
                  tlr: Translator, uta: UTADatabase) -> None:
         """Initialize the to canonical variation class
 
-        :param SeqRepoAccess seqrepo_access: Access to SeqRepo via cool-seq-tool
+        :param SeqRepoAccess seqrepo_access: Access to SeqRepo via UTA Tools
+        :param SeqRepoDataProxy dp: Access to SeqRepo via VRS Python
         :param Tokenize tokenizer: Tokenizer class for tokenizing
         :param Classify classifier: Classifier class for classifying tokens
         :param Validate validator: Validator class for validating valid inputs
         :param Translate translator: Translating valid inputs
         :param HGVSDupDelMode hgvs_dup_del_mode: Class for handling
             HGVS dup/del expressions
         :param Translator tlr: Class for translating nomenclatures to and from VRS
         :param UTADatabase uta: Access to UTA queries
         """
-        super().__init__(seqrepo_access, tokenizer, classifier, validator,
+        super().__init__(seqrepo_access, dp, tokenizer, classifier, validator,
                          translator, hgvs_dup_del_mode, gene_normalizer)
         self.tlr = tlr
         self.uta = uta
 
     async def to_canonical_variation(
         self, q: str,
         fmt: ToCanonicalVariationFmt,
         do_liftover: bool = False,
         hgvs_dup_del_mode: Optional[HGVSDupDelModeEnum] = None,
-        copy_change: Optional[CopyChange] = None,
+        relative_copy_class: Optional[RelativeCopyClass] = None,
         baseline_copies: Optional[int] = None,
         untranslatable_returns_text: bool = False
     ) -> ToCanonicalVariationService:
         """Given query as ToCanonicalVariationFmt, return canonical variation
 
         :param str q: Query to translate to canonical variation
         :param ToCanonicalVariationFmt fmt: The representation for `q`
         :param bool do_liftover: Whether or not to liftover to GRCh38 assembly.
         :param Optional[HGVSDupDelModeEnum] hgvs_dup_del_mode: Determines how to
             interpret HGVS dup/del expressions in VRS. Must be one of: `default`,
-            `copy_number_count`, `copy_number_change`, `repeated_seq_expr`,
-            `literal_seq_expr`
-        :param CopyChange copy_change: The copy change
+            `absolute_cnv`, `relative_cnv`, `repeated_seq_expr`, `literal_seq_expr`
+        :param RelativeCopyClass relative_copy_class: The relative copy class
         :param Optional[int] baseline_copies: Baseline copies number
         :param bool untranslatable_returns_text: `True` return VRS Text Object when
             unable to translate or normalize query. `False` return `None` when
             unable to translate or normalize query.
         :return: ToCanonicalVariationService containing Canonical Variation and
             list of warnings
         """
@@ -87,29 +88,27 @@
             if fmt == ToCanonicalVariationFmt.SPDI:
                 variation, warnings = await self.spdi_to_canonical_variation(
                     q, warnings, do_liftover=do_liftover)
             elif fmt == ToCanonicalVariationFmt.HGVS:
                 variation, warnings = await self.hgvs_to_canonical_variation(
                     q, warnings, do_liftover=do_liftover,
                     hgvs_dup_del_mode=hgvs_dup_del_mode,
-                    copy_change=copy_change,
+                    relative_copy_class=relative_copy_class,
                     baseline_copies=baseline_copies)
             else:
                 warnings = [f"fmt, {fmt}, is not supported. "
                             f"Must be either `spdi` or `hgvs`"]
 
             if variation and not warnings:
                 variation_type = variation["type"]
                 if variation_type in {VRSTypes.ALLELE.value,
-                                      VRSTypes.COPY_NUMBER_COUNT.value,
-                                      VRSTypes.COPY_NUMBER_CHANGE.value}:
-                    key = "location" if variation_type == VRSTypes.ALLELE else "subject"
-                    variation[key]["id"] = ga4gh_identify(
-                        models.Location(**variation[key])
-                    )
+                                      VRSTypes.ABSOLUTE_COPY_NUMBER.value,
+                                      VRSTypes.RELATIVE_COPY_NUMBER.value}:
+                    variation["location"]["id"] = ga4gh_identify(
+                        models.Location(**variation["location"]))
                 else:
                     warnings = [f"Variation type, {variation_type}, not supported"]
 
             if not variation and untranslatable_returns_text:
                 text = models.Text(definition=q, type="Text")
                 text.id = ga4gh_identify(text)
                 variation = Text(**text.as_dict()).dict(by_alias=True)
@@ -169,15 +168,15 @@
             end_pos = start_pos + int(deleted_seq)
 
         if do_liftover:
             newest_assembly_acs = await self.uta.get_newest_assembly_ac(ac)
             if not newest_assembly_acs:
                 warnings.append(f"Unable to get newest assemblies for {ac}")
                 return variation, None
-            new_ac = newest_assembly_acs[0]
+            new_ac = newest_assembly_acs[0][0]
             if new_ac != ac:
                 ac = new_ac
                 chromosome, warning = self.seqrepo_access.ac_to_chromosome(ac)
                 if not chromosome:
                     warnings.append(warning)
                     return variation, warnings
                 chromosome = f"chr{chromosome}"
@@ -199,15 +198,16 @@
             warnings.append(f"vrs-python translator raised error: {e}")
         except KeyError as e:
             warnings.append(f"vrs-python translator raised error: "
                             f"seqrepo could not translate identifier {e}")
         else:
             # Validate SPDI
             try:
-                sequence = self.seqrepo_access.sr.fetch(ac, start_pos, end=end_pos)
+                sequence = self.seqrepo_access.seqrepo_client.fetch(
+                    ac, start_pos, end=end_pos)
             except ValueError as e:
                 warnings.append(str(e))
             else:
                 if not sequence:
                     warnings.append(f"Position, {start_pos}, does not exist on {ac}")
                 else:
                     if not deleted_seq_is_int and deleted_seq != sequence:
@@ -219,27 +219,26 @@
             else:
                 variation = variation.as_dict()
         return variation, warnings
 
     async def hgvs_to_canonical_variation(
         self, q: str, warnings: List, do_liftover: bool = False,
         hgvs_dup_del_mode: Optional[HGVSDupDelModeEnum] = None,
-        copy_change: Optional[CopyChange] = None,
+        relative_copy_class: Optional[RelativeCopyClass] = None,
         baseline_copies: Optional[int] = None
     ) -> Tuple[Optional[Dict], List]:
         """Given HGVS representation, return canonical variation
 
         :param str q: HGVS query
         :param List warnings: List of warnings
         :param bool do_liftover: Whether or not to liftover to GRCh38 assembly
         :param Optional[HGVSDupDelModeEnum] hgvs_dup_del_mode: Determines how to
             interpret HGVS dup/del expressions in VRS. Must be one of: `default`,
-            `copy_number_count`, `copy_number_change`, `repeated_seq_expr`,
-            `literal_seq_expr`
-        :param CopyChange copy_change: The copy change
+            `absolute_cnv`, `relative_cnv`, `repeated_seq_expr`, `literal_seq_expr`
+        :param RelativeCopyClass relative_copy_class: The relative copy class
         :param Optional[int] baseline_copies: Baseline copies number
         :return: Canonical Variation and warnings
         """
         variation = None
         match = self.tlr.hgvs_re.match(q)
         if not match:
             warnings.append(f"{q} is not a valid HGVS expression")
@@ -251,29 +250,29 @@
         for c in classifications:
             if "HGVS" in c.matching_tokens or "ReferenceSequence" in c.matching_tokens:
                 hgvs_classifications.append(c)
         if not hgvs_classifications:
             warnings = [f"{q} is not a supported HGVS expression"]
             return variation, warnings
 
-        if hgvs_dup_del_mode == HGVSDupDelModeEnum.COPY_NUMBER_CHANGE:
-            if copy_change:
-                if copy_change.lower() not in VALID_COPY_CHANGE:
-                    return None, [f"{copy_change} is not a valid copy change value: "
-                                  f"{VALID_COPY_CHANGE}"]
-        elif hgvs_dup_del_mode == HGVSDupDelModeEnum.COPY_NUMBER_COUNT:
+        if hgvs_dup_del_mode == HGVSDupDelModeEnum.RELATIVE_CNV:
+            if relative_copy_class:
+                if relative_copy_class.lower() not in VALID_RELATIVE_COPY_CLASS:
+                    return None, [f"{relative_copy_class} is not a valid relative "
+                                  f"copy class: {VALID_RELATIVE_COPY_CLASS}"]
+        elif hgvs_dup_del_mode == HGVSDupDelModeEnum.ABSOLUTE_CNV:
             if not baseline_copies:
                 return None, [f"{hgvs_dup_del_mode} requires `baseline_copies`"]
         elif not hgvs_dup_del_mode:
             hgvs_dup_del_mode = HGVSDupDelModeEnum.DEFAULT
 
         validations = await self.validator.perform(
             classifications, endpoint_name=Endpoint.TO_CANONICAL, warnings=warnings,
             hgvs_dup_del_mode=hgvs_dup_del_mode, do_liftover=do_liftover,
-            copy_change=copy_change, baseline_copies=baseline_copies)
+            relative_copy_class=relative_copy_class, baseline_copies=baseline_copies)
         if not warnings:
             warnings = validations.warnings
 
         if do_liftover:
             if len(validations.valid_results) > 0:
                 valid_result = get_mane_valid_result(q, validations, warnings)
                 if valid_result:
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/to_copy_number_variation.py` & `variation-normalizer-0.7.dev0/variation/to_copy_number_variation.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 """Module for to copy number variation translation"""
 from typing import Tuple, Optional, List, Union
 from datetime import datetime
 
-from ga4gh.vrsatile.pydantic.vrs_models import CopyNumberCount, CopyNumberChange, \
-    Text, CopyChange
+from ga4gh.vrsatile.pydantic.vrs_models import AbsoluteCopyNumber, RelativeCopyNumber, \
+    Text, RelativeCopyClass
 from ga4gh.vrs import models
 from ga4gh.core import ga4gh_identify
 from pydantic import ValidationError
 from gene.schemas import MatchType as GeneMatchType
 
 from variation.to_vrs import ToVRS
 from variation.schemas.app_schemas import Endpoint
 from variation.schemas.hgvs_to_copy_number_schema import \
-    HgvsToCopyNumberCountService, HgvsToCopyNumberChangeService, \
-    VALID_COPY_CHANGE
-from variation.schemas.service_schema import AmplificationToCxVarQuery, \
-    AmplificationToCxVarService, ClinVarAssembly, ParsedToCnVarQuery, \
-    ParsedToCnVarService
+    HgvsToAbsoluteCopyNumberService, HgvsToRelativeCopyNumberService, \
+    VALID_RELATIVE_COPY_CLASS
+from variation.schemas.service_schema import AmplificationToRelCnvQuery, \
+    AmplificationToRelCnvService, ClinVarAssembly, ParsedToAbsCnvQuery, \
+    ParsedToAbsCnvService
 from variation.schemas.validation_response_schema import ValidationSummary
 from variation.schemas.normalize_response_schema\
     import HGVSDupDelMode as HGVSDupDelModeEnum, ServiceMeta
 from variation.utils import get_mane_valid_result, get_priority_sequence_location
 from variation.version import __version__
 
 
 class ToCopyNumberVariation(ToVRS):
     """Class for representing copy number variation"""
 
     @staticmethod
     def _parsed_to_text(start: int, end: int, total_copies: int, warnings: List[str],
                         assembly: Optional[str] = None, chr: Optional[str] = None,
                         accession: Optional[str] = None) -> Tuple[Text, List[str]]:
-        """Return response for invalid query for parsed_to_cn_var
+        """Return response for invalid query for parsed_to_abs_cnv
 
         :param int start: Start position as residue coordinate
         :param int end: End position as residue coordinate
-        :param int total_copies: Total copies for Copy Number Count variation object
+        :param int total_copies: Total copies for Absolute Copy Number variation object
         :param List[str] warnings: List of warnings
         :param Optional[ClinVarAssembly] assembly: Assembly. If `accession` is set,
             will ignore `assembly` and `chr`. If `accession` not set, must provide
             both `assembly` and `chr`.
         :param Optional[str] chr: Chromosome. Must set when `assembly` is set.
         :param Optional[str] accession: Accession. If `accession` is set,
             will ignore `assembly` and `chr`. If `accession` not set, must provide
@@ -59,19 +59,19 @@
         variation = Text(definition=definition, id=_id)
         return variation, warnings
 
     def _hgvs_to_cnv_resp(
         self, copy_number_type: HGVSDupDelModeEnum, hgvs_expr: str, do_liftover: bool,
         validations: Tuple[Optional[ValidationSummary], Optional[List[str]]],
         warnings: List[str], untranslatable_returns_text: bool = False
-    ) -> Tuple[Optional[Union[CopyNumberCount, CopyNumberChange, Text]], List[str]]:  # noqa: E501
+    ) -> Tuple[Optional[Union[AbsoluteCopyNumber, RelativeCopyNumber, Text]], List[str]]:  # noqa: E501
         """Return copy number variation and warnings response
 
         :param HGVSDupDelModeEnum copy_number_type: The type of copy number variation.
-            Must be either `copy_number_count` or `copy_number_change`
+            Must be either `absolute_cnv` or `relative_cnv`
         :param str hgvs_expr: HGVS expression
         :param bool do_liftover: Whether or not to liftover to GRCh38 assembly
         :param Tuple[Optional[ValidationSummary], Optional[List[str]]]: Validation
             summary and warnings for hgvs_expr
         :param List[str] warnings: List of warnings
         :param bool untranslatable_returns_text: `True` return VRS Text Object when
             unable to translate or normalize query. `False` return `None` when
@@ -93,121 +93,121 @@
 
         if not variation:
             if hgvs_expr and hgvs_expr.strip() and untranslatable_returns_text:
                 text = models.Text(definition=hgvs_expr, type="Text")
                 text.id = ga4gh_identify(text)
                 variation = Text(**text.as_dict())
         else:
-            if copy_number_type == HGVSDupDelModeEnum.COPY_NUMBER_COUNT:
-                variation = CopyNumberCount(**variation)
+            if copy_number_type == HGVSDupDelModeEnum.ABSOLUTE_CNV:
+                variation = AbsoluteCopyNumber(**variation)
             else:
-                variation = CopyNumberChange(**variation)
+                variation = RelativeCopyNumber(**variation)
         return variation, warnings
 
-    async def hgvs_to_copy_number_count(
+    async def hgvs_to_absolute_copy_number(
         self, hgvs_expr: str, baseline_copies: int,
         do_liftover: bool = False, untranslatable_returns_text: bool = False
-    ) -> HgvsToCopyNumberCountService:
+    ) -> HgvsToAbsoluteCopyNumberService:
         """Given hgvs, return abolute copy number variation
 
         :param str hgvs_expr: HGVS expression
         :param int baseline_copies: Baseline copies number
         :param bool do_liftover: Whether or not to liftover to GRCh38 assembly
         :param bool untranslatable_returns_text: `True` return VRS Text Object when
             unable to translate or normalize query. `False` return `None` when
             unable to translate or normalize query.
-        :return: HgvsToCopyNumberCountService containing Copy Number Count
+        :return: HgvsToAbsoluteCopyNumberService containing Absolute Copy Number
             Variation and warnings
         """
         validations, warnings = await self.get_validations(
-            hgvs_expr, endpoint_name=Endpoint.HGVS_TO_COPY_NUMBER_COUNT,
-            hgvs_dup_del_mode=HGVSDupDelModeEnum.COPY_NUMBER_COUNT,
+            hgvs_expr, endpoint_name=Endpoint.HGVS_TO_ABSOLUTE_CN,
+            hgvs_dup_del_mode=HGVSDupDelModeEnum.ABSOLUTE_CNV,
             baseline_copies=baseline_copies, do_liftover=do_liftover
         )
-        cn_var, warnings = self._hgvs_to_cnv_resp(
-            HGVSDupDelModeEnum.COPY_NUMBER_COUNT, hgvs_expr, do_liftover, validations,
+        abs_cnv, warnings = self._hgvs_to_cnv_resp(
+            HGVSDupDelModeEnum.ABSOLUTE_CNV, hgvs_expr, do_liftover, validations,
             warnings, untranslatable_returns_text)
 
-        return HgvsToCopyNumberCountService(
+        return HgvsToAbsoluteCopyNumberService(
             hgvs_expr=hgvs_expr,
             warnings=warnings,
             service_meta_=ServiceMeta(
                 version=__version__,
                 response_datetime=datetime.now()
             ),
-            copy_number_count=cn_var
+            absolute_copy_number=abs_cnv
         )
 
-    async def hgvs_to_copy_number_change(
-        self, hgvs_expr: str, copy_change: Optional[CopyChange],
+    async def hgvs_to_relative_copy_number(
+        self, hgvs_expr: str, relative_copy_class: Optional[RelativeCopyClass],
         do_liftover: bool = False, untranslatable_returns_text: bool = False
-    ) -> HgvsToCopyNumberChangeService:
-        """Given hgvs, return copy number change variation
+    ) -> HgvsToRelativeCopyNumberService:
+        """Given hgvs, return relative copy number variation
 
         :param str hgvs_expr: HGVS expression
-        :param Optional[CopyChange] copy_change: The copy change
+        :param Optional[RelativeCopyClass] relative_copy_class: The relative copy class
         :param bool do_liftover: Whether or not to liftover to GRCh38 assembly
         :param bool untranslatable_returns_text: `True` return VRS Text Object when
             unable to translate or normalize query. `False` return `None` when
             unable to translate or normalize query.
-        :return: HgvsToCopyNumberChangeService containing Copy Number Change
+        :return: HgvsToRelativeCopyNumberService containing Relative Copy Number
             Variation and warnings
         """
-        if copy_change and copy_change.lower() not in VALID_COPY_CHANGE:  # noqa: E501
-            return None, [f"{copy_change} is not a valid copy change: "
-                          f"{VALID_COPY_CHANGE}"]
+        if relative_copy_class and relative_copy_class.lower() not in VALID_RELATIVE_COPY_CLASS:  # noqa: E501
+            return None, [f"{relative_copy_class} is not a valid relative copy class: "
+                          f"{VALID_RELATIVE_COPY_CLASS}"]
 
         validations, warnings = await self.get_validations(
-            hgvs_expr, endpoint_name=Endpoint.HGVS_TO_COPY_NUMBER_CHANGE,
-            hgvs_dup_del_mode=HGVSDupDelModeEnum.COPY_NUMBER_CHANGE,
-            copy_change=copy_change, do_liftover=do_liftover
+            hgvs_expr, endpoint_name=Endpoint.HGVS_TO_RELATIVE_CN,
+            hgvs_dup_del_mode=HGVSDupDelModeEnum.RELATIVE_CNV,
+            relative_copy_class=relative_copy_class, do_liftover=do_liftover
         )
 
-        cx_var, warnings = self._hgvs_to_cnv_resp(
-            HGVSDupDelModeEnum.COPY_NUMBER_CHANGE, hgvs_expr, do_liftover, validations,
+        rel_cnv, warnings = self._hgvs_to_cnv_resp(
+            HGVSDupDelModeEnum.RELATIVE_CNV, hgvs_expr, do_liftover, validations,
             warnings, untranslatable_returns_text)
 
-        return HgvsToCopyNumberChangeService(
+        return HgvsToRelativeCopyNumberService(
             hgvs_expr=hgvs_expr,
             warnings=warnings,
             service_meta_=ServiceMeta(
                 version=__version__,
                 response_datetime=datetime.now()
             ),
-            copy_number_change=cx_var
+            relative_copy_number=rel_cnv
         )
 
-    def parsed_to_cn_var(
+    def parsed_to_abs_cnv(
         self, start: int, end: int, total_copies: int,
         assembly: Optional[ClinVarAssembly] = None, chr: Optional[str] = None,
         accession: Optional[str] = None, untranslatable_returns_text: bool = False
-    ) -> ParsedToCnVarService:
-        """Given parsed ClinVar Copy Number Gain/Loss components, return Copy Number
-        Count Variation
+    ) -> ParsedToAbsCnvService:
+        """Given parsed ClinVar Copy Number Gain/Loss components, return Absolute
+        Copy Number Variation
 
         :param int start: Start position as residue coordinate
         :param int end: End position as residue coordinate
-        :param int total_copies: Total copies for Copy Number Count variation object
+        :param int total_copies: Total copies for Absolute Copy Number variation object
         :param Optional[ClinVarAssembly] assembly: Assembly. If `accession` is set,
             will ignore `assembly` and `chr`. If `accession` not set, must provide
             both `assembly` and `chr`.
         :param Optional[str] chr: Chromosome. Must set when `assembly` is set.
         :param Optional[str] accession: Accession. If `accession` is set,
             will ignore `assembly` and `chr`. If `accession` not set, must provide
             both `assembly` and `chr`.
         :param bool untranslatable_returns_text: `True` return VRS Text Object when
             unable to translate or normalize query. `False` return `None` when
             unable to translate or normalize query.
-        :return: ParsedToCnVarService containing Copy Number Count variation
+        :return: ParsedToAbsCnvService containing Absolute Copy Number variation
             and list of warnings
         """
         variation = None
         warnings = list()
         try:
-            og_query = ParsedToCnVarQuery(
+            og_query = ParsedToAbsCnvQuery(
                 assembly=assembly, chr=chr, accession=accession, start=start, end=end,
                 total_copies=total_copies)
         except ValidationError as e:
             warnings.append(str(e))
             og_query = None
         else:
             if accession:
@@ -218,24 +218,24 @@
                 elif assembly == ClinVarAssembly.HG19:
                     assembly = ClinVarAssembly.GRCH37
                 elif assembly == ClinVarAssembly.HG18:
                     assembly = ClinVarAssembly.NCBI36
 
                 if assembly != ClinVarAssembly.NCBI36:
                     # Variation Normalizer does not support NCBI36 yet
-                    query = f"{assembly.value}:{chr}"
+                    query = f"{assembly}:{chr}"
                     aliases, w = self.seqrepo_access.translate_identifier(query)
                     if w:
                         warnings.append(w)
                     else:
                         accession = ([a for a in aliases if a.startswith("refseq:")] or [None])[0]  # noqa: E501
                         if not accession:
                             warnings.append(f"Unable to find RefSeq accession for {query}")  # noqa: E501
                 else:
-                    warnings.append(f"{assembly.value} assembly is not currently supported")  # noqa: E501
+                    warnings.append(f"{assembly} assembly is not current supported")
             else:
                 warnings.append("Must provide either `accession` or both `assembly` "
                                 "and `chr`.")
 
         if warnings:
             if untranslatable_returns_text:
                 variation, warnings = self._parsed_to_text(
@@ -255,82 +255,82 @@
 
             if warnings:
                 if untranslatable_returns_text:
                     variation, warnings = self._parsed_to_text(
                         start, end, total_copies, warnings, assembly, chr, accession)
             else:
                 try:
-                    self.seqrepo_access.sr[accession][start - 1]
-                    self.seqrepo_access.sr[accession][end]
+                    self.seqrepo_access.seqrepo_client[accession][start - 1]
+                    self.seqrepo_access.seqrepo_client[accession][end]
                 except ValueError as e:
                     warnings.append(str(e).replace("start", "Position"))
                     if untranslatable_returns_text:
                         variation, warnings = self._parsed_to_text(
                             start, end, total_copies, warnings, assembly, chr,
                             accession)
                 else:
-                    subject = models.SequenceLocation(
+                    location = models.SequenceLocation(
                         type="SequenceLocation",
                         sequence_id=sequence_id,
                         start=models.IndefiniteRange(
                             comparator="<=",
                             value=start - 1,
                             type="IndefiniteRange"),
                         end=models.IndefiniteRange(
                             comparator=">=",
                             value=end,
                             type="IndefiniteRange")
                     )
-                    subject.id = ga4gh_identify(subject)
+                    location.id = ga4gh_identify(location)
                     variation = {
-                        "type": "CopyNumberCount",
-                        "subject": subject.as_dict(),
+                        "type": "AbsoluteCopyNumber",
+                        "location": location.as_dict(),
                         "copies": {"value": total_copies, "type": "Number"}
                     }
                     variation["id"] = ga4gh_identify(
-                        models.CopyNumberCount(**variation))
-                    variation = CopyNumberCount(**variation)
+                        models.AbsoluteCopyNumber(**variation))
+                    variation = AbsoluteCopyNumber(**variation)
 
-        return ParsedToCnVarService(
+        return ParsedToAbsCnvService(
             query=og_query,
-            copy_number_count=variation,
+            absolute_copy_number=variation,
             warnings=warnings,
             service_meta_=ServiceMeta(
                 version=__version__,
                 response_datetime=datetime.now()
             )
         )
 
-    def amplification_to_cx_var(
+    def amplification_to_rel_cnv(
         self, gene: str, sequence_id: Optional[str] = None, start: Optional[int] = None,
         end: Optional[int] = None, untranslatable_returns_text: bool = False
-    ) -> AmplificationToCxVarService:
-        """Return Copy Number Change Variation for Amplification query
+    ) -> AmplificationToRelCnvService:
+        """Return Relative Copy Number Variation for Amplification query
         Parameter priority:
             1. sequence_id, start, end (must provide ALL)
             2. use the gene-normalizer to get the SequenceLocation
 
         :param str gene: Gene query
         :param Optional[str] sequence_id: Sequence ID for the location. If set,
             must also provide `start` and `end`
         :param Optional[int] start: Start position as residue coordinate for the
             sequence location. If set, must also provide `sequence_id` and `end`
         :param Optional[int] end: End position as residue coordinate for the sequence
             location. If set, must also provide `sequence_id` and `start`
         :param bool untranslatable_returns_text: `True` return VRS Text Object when
             unable to translate or normalize query. `False` return `None` when
             unable to translate or normalize query.
-        :return: AmplificationToCxVarService containing Copy Number Change and
+        :return: AmplificationToRelCnvService containing Relative Copy Number and
             list of warnings
         """
         warnings = list()
         amplification_label = None
         variation = None
         try:
-            og_query = AmplificationToCxVarQuery(
+            og_query = AmplificationToRelCnvQuery(
                 gene=gene, sequence_id=sequence_id, start=start, end=end)
         except ValidationError as e:
             warnings.append(str(e))
             og_query = None
         else:
             # Need to validate the input gene
             gene_norm_resp = self.gene_normalizer.normalize(gene)
@@ -365,28 +365,28 @@
                     else:
                         warnings.append(
                             f"gene-normalizer could not find a priority sequence "
                             f"location for gene: {gene_norm_label}")
 
                 if vrs_location:
                     vrs_location.id = ga4gh_identify(vrs_location)
-                    vrs_cx = models.CopyNumberChange(
-                        subject=vrs_location,
-                        copy_change=CopyChange.HIGH_LEVEL_GAIN.value)
-                    vrs_cx.id = ga4gh_identify(vrs_cx)
-                    variation = CopyNumberChange(**vrs_cx.as_dict())
+                    vrs_rcn = models.RelativeCopyNumber(
+                        location=vrs_location,
+                        relative_copy_class=RelativeCopyClass.HIGH_LEVEL_GAIN.value)
+                    vrs_rcn.id = ga4gh_identify(vrs_rcn)
+                    variation = RelativeCopyNumber(**vrs_rcn.as_dict())
             else:
                 warnings.append(f"gene-normalizer returned no match for gene: {gene}")
 
         if not variation and untranslatable_returns_text:
             text_variation = models.Text(definition=amplification_label)
             text_variation.id = ga4gh_identify(text_variation)
             variation = Text(**text_variation.as_dict())
 
-        return AmplificationToCxVarService(
+        return AmplificationToRelCnvService(
             query=og_query,
             amplification_label=amplification_label,
-            copy_number_change=variation,
+            relative_copy_number=variation,
             warnings=warnings,
             service_meta_=ServiceMeta(
                 version=__version__,
                 response_datetime=datetime.now()))
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/to_vrs.py` & `variation-normalizer-0.7.dev0/variation/to_vrs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,125 +1,127 @@
 """Module for to_vrs endpoint."""
 from typing import Tuple, Optional, List, Union, Dict
 from urllib.parse import unquote
 from datetime import datetime
 
-from ga4gh.vrsatile.pydantic.vrs_models import Allele, Haplotype, CopyNumberCount,\
+from ga4gh.vrsatile.pydantic.vrs_models import Allele, Haplotype, AbsoluteCopyNumber,\
     VariationSet, Text
 from ga4gh.vrs import models
 from ga4gh.core import ga4gh_identify
-from cool_seq_tool.schemas import ResidueMode
-from cool_seq_tool.data_sources import SeqRepoAccess
+from uta_tools.schemas import ResidueMode
+from uta_tools.data_sources import SeqRepoAccess
+from ga4gh.vrs.dataproxy import SeqRepoDataProxy
 from gene.query import QueryHandler as GeneQueryHandler
 
 from variation.schemas.normalize_response_schema\
     import HGVSDupDelMode as HGVSDupDelModeEnum, ServiceMeta
 from variation.hgvs_dup_del_mode import HGVSDupDelMode
 from variation.schemas.app_schemas import Endpoint
 from variation.schemas.hgvs_to_copy_number_schema import VALID_CLASSIFICATION_TYPES,\
-    CopyChange
+    RelativeCopyClass
 from variation.schemas.to_vrs_response_schema import ToVRSService
 from variation.schemas.token_response_schema import Nomenclature
 from variation.schemas.validation_response_schema import ValidationSummary
 from variation.classifiers import Classify
 from variation.tokenizers import Tokenize
 from variation.validators import Validate
 from variation.translators import Translate
 from variation.vrs_representation import VRSRepresentation
 from variation.version import __version__
 
 
 class ToVRS(VRSRepresentation):
     """The class for translating variation strings to VRS representations."""
 
-    def __init__(self, seqrepo_access: SeqRepoAccess,
+    def __init__(self, seqrepo_access: SeqRepoAccess, dp: SeqRepoDataProxy,
                  tokenizer: Tokenize, classifier: Classify, validator: Validate,
                  translator: Translate, hgvs_dup_del_mode: HGVSDupDelMode,
                  gene_normalizer: GeneQueryHandler) -> None:
         """Initialize the ToVrsAndVrsatile class.
 
-        :param SeqRepoAccess seqrepo_access: Access to SeqRepo
+        :param SeqRepoAccess seqrepo_access: Access to SeqRepo via UTA Tools
+        :param SeqRepoDataProxy dp: Access to SeqRepo via VRS Python
         :param Tokenize tokenizer: Tokenizer class for tokenizing
         :param Classify classifier: Classifier class for classifying tokens
         :param Validate validator: Validator class for validating valid inputs
         :param Translate translator: Translating valid inputs
         :param HGVSDupDelMode hgvs_dup_del_mode: Class for handling
             HGVS dup/del expressions
         :param GeneQueryHandler gene_normalizer: Client for normalizing gene concepts
         """
-        super().__init__(seqrepo_access)
+        super().__init__(dp, seqrepo_access)
         self.tokenizer = tokenizer
         self.classifier = classifier
         self.validator = validator
         self.translator = translator
         self.hgvs_dup_del_mode = hgvs_dup_del_mode
         self.gene_normalizer = gene_normalizer
 
     async def get_validations(
             self, q: str, endpoint_name: Optional[Endpoint] = None,
             hgvs_dup_del_mode: Optional[HGVSDupDelModeEnum] = None,  # noqa: E501
             baseline_copies: Optional[int] = None,
-            copy_change: Optional[CopyChange] = None,
+            relative_copy_class: Optional[RelativeCopyClass] = None,
             do_liftover: bool = False
     ) -> Tuple[Optional[ValidationSummary], Optional[List[str]]]:
         """Return validation results for a given variation.
 
         :param str q: variation to get validation results for
         :param Optional[Endpoint] endpoint_name: Then name of the endpoint being used
         :param Optional HGVSDupDelModeEnum hgvs_dup_del_mode: This parameter determines
             how to interpret HGVS dup/del expressions in VRS.
         :param Optional[int] baseline_copies: Baseline copies number
-        :param Optional[CopyChange] copy_change: The copy change
+        :param Optional[RelativeCopyClass] relative_copy_class: The relative copy class
         :param bool do_liftover: Whether or not to liftover to GRCh38 assembly
         :return: ValidationSummary for the variation and list of warnings
         """
         warnings = list()
         if q is None:
             return None, ["No variation entered"]
         tokens = self.tokenizer.perform(unquote(q.strip()), warnings)
 
         # gnomad vcf should always be a literal seq expression (allele)
         nomenclature = {t.nomenclature for t in tokens}
         if Nomenclature.GNOMAD_VCF in nomenclature:
             hgvs_dup_del_mode = HGVSDupDelModeEnum.LITERAL_SEQ_EXPR
         else:
-            if endpoint_name in [Endpoint.NORMALIZE, Endpoint.HGVS_TO_COPY_NUMBER_COUNT,
-                                 Endpoint.HGVS_TO_COPY_NUMBER_CHANGE]:
+            if endpoint_name in [Endpoint.NORMALIZE, Endpoint.HGVS_TO_ABSOLUTE_CN,
+                                 Endpoint.HGVS_TO_RELATIVE_CN]:
                 if hgvs_dup_del_mode:
                     hgvs_dup_del_mode = hgvs_dup_del_mode.strip().lower()
                     if endpoint_name == Endpoint.NORMALIZE:
                         if not self.hgvs_dup_del_mode.is_valid_dup_del_mode(hgvs_dup_del_mode):  # noqa: E501
                             warnings.append(
                                 f"hgvs_dup_del_mode must be one of: "
                                 f"{self.hgvs_dup_del_mode.valid_dup_del_modes}")
                             return None, warnings
                     else:
                         if not self.hgvs_dup_del_mode.is_valid_copy_number_mode(hgvs_dup_del_mode):  # noqa: E501
                             warnings.append(f"hgvs_dup_del_mode must be one of "
                                             f"{self.hgvs_dup_del_mode.valid_copy_number_modes}")  # noqa: E501
                             return None, warnings
-                    if hgvs_dup_del_mode == HGVSDupDelModeEnum.COPY_NUMBER_COUNT:
+                    if hgvs_dup_del_mode == HGVSDupDelModeEnum.ABSOLUTE_CNV:
                         if not baseline_copies:
                             warnings.append(f"{hgvs_dup_del_mode} mode "
                                             f"requires `baseline_copies`")
                             return None, warnings
                 elif not hgvs_dup_del_mode and endpoint_name == Endpoint.NORMALIZE:
                     hgvs_dup_del_mode = HGVSDupDelModeEnum.DEFAULT
                 else:
                     warnings.append(f"hgvs_dup_del_mode must be either "
-                                    f"{HGVSDupDelModeEnum.COPY_NUMBER_COUNT.value} or "
-                                    f"{HGVSDupDelModeEnum.COPY_NUMBER_CHANGE.value}")
+                                    f"{HGVSDupDelModeEnum.ABSOLUTE_CNV.value} or "
+                                    f"{HGVSDupDelModeEnum.RELATIVE_CNV.value}")
                     return None, warnings
             else:
                 hgvs_dup_del_mode = HGVSDupDelModeEnum.DEFAULT
 
         classifications = self.classifier.perform(tokens)
 
-        if endpoint_name in [Endpoint.HGVS_TO_COPY_NUMBER_COUNT,
-                             Endpoint.HGVS_TO_COPY_NUMBER_CHANGE]:
+        if endpoint_name in [Endpoint.HGVS_TO_ABSOLUTE_CN,
+                             Endpoint.HGVS_TO_RELATIVE_CN]:
             tmp_classifications = []
             for c in classifications:
                 conditions = (
                     c.classification_type in VALID_CLASSIFICATION_TYPES,
                     ("HGVS" in c.matching_tokens or "ReferenceSequence" in c.matching_tokens)  # noqa: E501
                 )
                 if all(conditions):
@@ -129,23 +131,23 @@
                 warnings = [f"{q} is not a supported HGVS genomic "
                             f"duplication or deletion"]
                 return None, warnings
 
         validations = await self.validator.perform(
             classifications, endpoint_name=endpoint_name, warnings=warnings,
             hgvs_dup_del_mode=hgvs_dup_del_mode, baseline_copies=baseline_copies,
-            copy_change=copy_change, do_liftover=do_liftover
+            relative_copy_class=relative_copy_class, do_liftover=do_liftover
         )
         if not warnings:
             warnings = validations.warnings
         return validations, warnings
 
     def get_translations(self, validations: ValidationSummary,
                          warnings: List)\
-            -> Tuple[Optional[Union[List[Allele], List[CopyNumberCount],
+            -> Tuple[Optional[Union[List[Allele], List[AbsoluteCopyNumber],
                                     List[Text], List[Haplotype],
                                     List[VariationSet]]],
                      Optional[List[str]]]:
         """Return a list translations from a ValidationSummary.
 
         :param ValidationSummary validations: Valid and Invalid results
         :param List warnings: List of warnings
@@ -157,24 +159,25 @@
                 result = self.translator.perform(valid_variation)
                 if result not in translations:
                     translations.append(result)
             if not translations and not warnings:
                 warnings.append("Unable to validate variation")
         return translations, warnings
 
-    def get_ref_allele_seq(self, location: Dict,
+    def get_ref_allele_seq(self, allele: Dict,
                            identifier: str) -> Optional[str]:
         """Return ref allele seq for transcript.
 
-        :param Dict location: VRS Location object
+        :param Dict allele: VRS Allele object
         :param str identifier: Identifier for allele
         :return: Ref seq allele
         """
         start = None
         end = None
+        location = allele["location"]
         if location["start"]["type"] == "Number":
             start = location["start"]["value"]
             end = location["end"]["value"]
 
             if start == end:
                 return None
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/to_vrsatile.py` & `variation-normalizer-0.7.dev0/variation/to_vrsatile.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,20 +30,20 @@
         token_type = valid_result.classification_token.token_type
         token_type_l = token_type.lower()
 
         vrs_ref_allele_seq = None
         if "uncertain" in token_type_l:
             warnings = ["Ambiguous regions cannot be normalized"]
         elif "range" not in token_type_l and token_type != TokenType.AMPLIFICATION:
-            variation_type = variation["type"]
-            if variation_type in {VRSTypes.ALLELE.value,
-                                  VRSTypes.COPY_NUMBER_COUNT.value,
-                                  VRSTypes.COPY_NUMBER_CHANGE.value}:
-                key = "location" if variation_type == VRSTypes.ALLELE else "subject"
-                vrs_ref_allele_seq = self.get_ref_allele_seq(variation[key], identifier)
+            if variation["type"] in {VRSTypes.ALLELE.value,
+                                     VRSTypes.ABSOLUTE_COPY_NUMBER.value,
+                                     VRSTypes.RELATIVE_COPY_NUMBER.value}:
+                vrs_ref_allele_seq = self.get_ref_allele_seq(
+                    variation, identifier
+                )
 
         if valid_result.gene_tokens:
             gene_token = valid_result.gene_tokens[0]
             gene_context = self.get_gene_descriptor(gene_token=gene_token)
         else:
             if gene:
                 gene_context = self.get_gene_descriptor(gene=gene)
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/tokenizers/__init__.py` & `variation-normalizer-0.7.dev0/variation/tokenizers/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Module to load and init namespace at package level."""
 from .tokenizer import Tokenizer
 from .tokenize import Tokenize
+from .gene_pair import GenePair
 from .gene_symbol import GeneSymbol
+from .protein_alternate import ProteinAlternate
 from .protein_delins import ProteinDelIns
 from .hgvs import HGVS
 from .reference_sequence import ReferenceSequence
 from .protein_substitution import ProteinSubstitution
 from .polypeptide_truncation import PolypeptideTruncation
 from .silent_mutation import SilentMutation
 from .polypeptide_sequence_variation_base import PolypeptideSequenceVariationBase
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/tokenizers/coding_dna_deletion.py` & `variation-normalizer-0.7.dev0/variation/tokenizers/coding_dna_deletion.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,14 +5,10 @@
 from variation.tokenizers.deletion_base import DeletionBase
 
 
 class CodingDNADeletion(DeletionBase):
     """Class for tokenizing Deletion at the coding dna reference sequence."""
 
     def return_token(self, params: Dict) -> Optional[CodingDNADeletionToken]:
-        """Return coding DNA Deletion token if match
-
-        :param Dict params: Matched parameters for deletion
-        :return: `CodingDNADeletionToken` if on c coordinate, else `None`
-        """
-        if params["coordinate_type"] == "c":
+        """Return coding DNA Deletion token."""
+        if self.parts["coordinate_type"] == "c":
             return CodingDNADeletionToken(**params)
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/tokenizers/coding_dna_delins.py` & `variation-normalizer-0.7.dev0/variation/tokenizers/coding_dna_delins.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/tokenizers/coding_dna_insertion.py` & `variation-normalizer-0.7.dev0/variation/tokenizers/coding_dna_insertion.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/tokenizers/coding_dna_silent_mutation.py` & `variation-normalizer-0.7.dev0/variation/tokenizers/coding_dna_silent_mutation.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/tokenizers/coding_dna_substitution.py` & `variation-normalizer-0.7.dev0/variation/tokenizers/coding_dna_substitution.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/tokenizers/deletion_base.py` & `variation-normalizer-0.7.dev0/variation/tokenizers/deletion_range_base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-"""A module for Deletion Tokenization Base Class."""
+"""A module for tokenizing genomic deletion ranges."""
+from typing import Dict, Optional, List
 from abc import abstractmethod
-from typing import Optional, Dict
-import re
 
-from variation.schemas.token_response_schema import Deletion, TokenMatchType
+from variation.schemas.token_response_schema import TokenMatchType, \
+    DeletionRange
 from .tokenizer import Tokenizer
 
 
-class DeletionBase(Tokenizer):
-    """Class for tokenizing Deletions."""
+class DeletionRangeBase(Tokenizer):
+    """The tokenizer class for genomic deletion range."""
 
-    pattern = r"^(?P<start_pos>\d+)" \
-              r"(_(?P<end_pos>\d+))?del(?P<deleted_seq>[actgn]+)?$"
-    splitter = re.compile(pattern)
+    def __init__(self) -> None:
+        """Initialize the Genomic Deletion Range Class."""
+        self.parts = None
 
-    def match(self, input_string: str) -> Optional[Deletion]:
+    def match(self, input_string: str) -> Optional[DeletionRange]:
         """Return tokens that match the input string.
 
         :param str input_string: Input string
-        :return: Deletion token if a match is found, else `None`
+        :return: DeletionRange token if a match is found
         """
-        parts = {
+        if input_string is None:
+            return None
+
+        self.parts = {
             "token": input_string,
             "input_string": input_string,
             "match_type": TokenMatchType.UNSPECIFIED.value,
-            "start_pos_del": None,
-            "end_pos_del": None,
-            "deleted_sequence": None,
+            "start_pos1_del": None,
+            "start_pos2_del": None,
+            "end_pos1_del": None,
+            "end_pos2_del": None,
             "coordinate_type": None
         }
 
-        input_str_l = str(input_string).lower()
-
-        if input_str_l.startswith("p."):
+        input_string = str(input_string).lower()
+        if not input_string.endswith("del"):
             return None
 
-        if input_str_l.startswith(("c.", "g.")):
-            parts["coordinate_type"] = input_str_l[:1]
-            input_str_l = input_str_l[2:]
-
-        if input_str_l.startswith("(") and input_str_l.endswith(")"):
-            input_str_l = input_str_l[1:-1]
-
-        match = self.splitter.match(input_str_l)
-        if not match:
+        if input_string.startswith("g."):
+            self.parts["coordinate_type"] = "g"
+        elif input_string.startswith("c."):
+            self.parts["coordinate_type"] = "c"
+        elif input_string.startswith("p."):
+            self.parts["coordinate_type"] = "p"
+        else:
             return None
 
-        params = match.groupdict()
+        parts = input_string.split("_")
+        self._get_parts(parts)
+        return self.return_token(self.parts)
 
-        parts["start_pos_del"] = params["start_pos"]
-        parts["end_pos_del"] = params["end_pos"]
-        if parts["start_pos_del"] and parts["end_pos_del"]:
-            if parts["start_pos_del"] > parts["end_pos_del"]:
-                return None
-
-        parts["deleted_sequence"] = \
-            params["deleted_seq"].upper() if params["deleted_seq"] else None
+    @abstractmethod
+    def _get_parts(self, parts: List) -> None:
+        """Set `self.parts` for genomic deletion range
 
-        return self.return_token(parts)
+        :param List parts: Parts of input string
+        """
+        raise NotImplementedError
 
     @abstractmethod
-    def return_token(self, params: Dict[str, str]) -> Optional[Deletion]:
+    def return_token(self, params: Dict[str, str]) -> Optional[DeletionRange]:
         """Return token instance.
 
-        :param Dict params: Params for Deletion token
-        :return: Deletion token
+        :param Dict params: Params for DeletionRange token
+        :return: DeletionRange token
         """
         raise NotImplementedError
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/tokenizers/deletion_range_base.py` & `variation-normalizer-0.7.dev0/variation/tokenizers/protein_insertion.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,69 +1,81 @@
-"""A module for tokenizing genomic deletion ranges."""
-from typing import Dict, Optional, List
-from abc import abstractmethod
+"""A module for Protein Insertion Tokenization Class."""
+from typing import List, Optional
 
-from variation.schemas.token_response_schema import TokenMatchType, \
-    DeletionRange
-from .tokenizer import Tokenizer
+from pydantic.error_wrappers import ValidationError
 
+from variation.schemas.token_response_schema import ProteinInsertionToken, \
+    TokenMatchType
+from .caches import AminoAcidCache, NucleotideCache
+from .tokenizer import Tokenizer
+from .tokenize_base import TokenizeBase
 
-class DeletionRangeBase(Tokenizer):
-    """The tokenizer class for genomic deletion range."""
 
-    def __init__(self) -> None:
-        """Initialize the Genomic Deletion Range Class."""
-        self.parts = None
+class ProteinInsertion(Tokenizer):
+    """Class for tokenizing Insertions on the protein reference sequence."""
 
-    def match(self, input_string: str) -> Optional[DeletionRange]:
-        """Return tokens that match the input string.
+    def __init__(self, amino_acid_cache: AminoAcidCache,
+                 nucleotide_cache: NucleotideCache) -> None:
+        """Initialize the Protein Insertion Class.
 
-        :param str input_string: Input string
-        :return: DeletionRange token if a match is found
+        :param AminoAcidCache amino_acid_cache: Valid amino acid codes
+        :param NucleotideCache nucleotide_cache: Valid nucleotides
         """
+        self.parts = None
+        self.tokenize_base = TokenizeBase(amino_acid_cache, nucleotide_cache)
+
+    def match(self, input_string: str) -> Optional[ProteinInsertionToken]:
+        """Return token that match the input string."""
         if input_string is None:
             return None
 
         self.parts = {
+            "used_one_letter": False,
             "token": input_string,
             "input_string": input_string,
             "match_type": TokenMatchType.UNSPECIFIED.value,
-            "start_pos1_del": None,
-            "start_pos2_del": None,
-            "end_pos1_del": None,
-            "end_pos2_del": None,
-            "coordinate_type": None
+            "start_aa_flank": None,
+            "start_pos_flank": None,
+            "end_aa_flank": None,
+            "end_pos_flank": None
         }
 
         input_string = str(input_string).lower()
-        if not input_string.endswith("del"):
+
+        if "c." in input_string or "g." in input_string:
             return None
 
-        if input_string.startswith("g."):
-            self.parts["coordinate_type"] = "g"
-        elif input_string.startswith("c."):
-            self.parts["coordinate_type"] = "c"
-        elif input_string.startswith("p."):
-            self.parts["coordinate_type"] = "p"
-        else:
+        if input_string.startswith("p."):
+            input_string = input_string[2:]
+
+        if input_string.startswith("(") and input_string.endswith(")"):
+            input_string = input_string[1:-1]
+
+        if "ins" not in input_string:
             return None
 
-        parts = input_string.split("_")
+        parts = input_string.split("ins")
         self._get_parts(parts)
-        return self.return_token(self.parts)
 
-    @abstractmethod
+        try:
+            return ProteinInsertionToken(**self.parts)
+        except ValidationError:
+            return None
+
     def _get_parts(self, parts: List) -> None:
-        """Set `self.parts` for genomic deletion range
+        """Get parts for Protein Insertion.
 
         :param List parts: Parts of input string
         """
-        raise NotImplementedError
-
-    @abstractmethod
-    def return_token(self, params: Dict[str, str]) -> Optional[DeletionRange]:
-        """Return token instance.
+        if len(parts) != 2:
+            return
 
-        :param Dict params: Params for DeletionRange token
-        :return: DeletionRange token
-        """
-        raise NotImplementedError
+        range_aa_pos = self.tokenize_base.get_aa_pos_range(parts)
+        if range_aa_pos:
+            self.parts["start_aa_flank"] = range_aa_pos[0]
+            self.parts["end_aa_flank"] = range_aa_pos[1]
+            self.parts["start_pos_flank"] = range_aa_pos[2]
+            self.parts["end_pos_flank"] = range_aa_pos[3]
+            self.parts["used_one_letter"] = range_aa_pos[4]
+        self.parts["inserted_sequence"] = \
+            self.tokenize_base.get_protein_inserted_sequence(
+                parts, self.parts["used_one_letter"])
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/tokenizers/delins_base.py` & `variation-normalizer-0.7.dev0/variation/tokenizers/delins_base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 """A module for DelIns Tokenization Base Class."""
 from abc import abstractmethod
 from typing import Optional, Dict, List
 
 from variation.schemas.token_response_schema import DelIns, TokenMatchType, Token
 from .tokenizer import Tokenizer
+from .caches import AminoAcidCache, NucleotideCache
+from .tokenize_base import TokenizeBase
 
 
 class DelInsBase(Tokenizer):
     """Class for tokenizing DelIns."""
 
-    def __init__(self) -> None:
-        """Initialize the DelIns Class."""
+    def __init__(self, amino_acid_cache: AminoAcidCache,
+                 nucleotide_cache: NucleotideCache) -> None:
+        """Initialize the DelIns Class.
+
+        :param AminoAcidCache amino_acid_cache: Valid amino acid codes
+        :param NucleotideCache nucleotide_cache: Valid nucleotides
+        """
         self.parts = None
+        self.tokenize_base = TokenizeBase(amino_acid_cache, nucleotide_cache)
 
     def match(self, input_string: str) -> Optional[DelIns]:
         """Return tokens that match the input string."""
         if input_string is None:
             return None
 
         input_string = str(input_string).lower()
@@ -67,21 +75,22 @@
         if not parts[0].startswith("c.") and not parts[0].startswith("g."):
             return
 
         # Get reference sequence
         coordinate_type = parts[0][:1]
         parts[0] = parts[0][2:]
 
-        positions_deleted = self.get_positions_deleted(parts)
+        positions_deleted = self.tokenize_base.get_positions_deleted(parts)
         if not positions_deleted:
             return
         start_pos_del = positions_deleted[0]
         end_pos_del = positions_deleted[1]
 
-        inserted_sequences = self.get_transcript_genomic_inserted_sequence(parts)
+        inserted_sequences = \
+            self.tokenize_base.get_transcript_genomic_inserted_sequence(parts)
         if not inserted_sequences:
             return
         inserted_sequence1 = inserted_sequences[0]
         inserted_sequence2 = inserted_sequences[1]
 
         if not inserted_sequence1 and not inserted_sequence2:
             return
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/tokenizers/duplication_base.py` & `variation-normalizer-0.7.dev0/variation/tokenizers/duplication_base.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/tokenizers/free_text_categorical.py` & `variation-normalizer-0.7.dev0/variation/tokenizers/free_text_categorical.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/tokenizers/gene_symbol.py` & `variation-normalizer-0.7.dev0/variation/tokenizers/gene_symbol.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/tokenizers/genomic_deletion.py` & `variation-normalizer-0.7.dev0/variation/tokenizers/genomic_deletion.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,10 @@
 from variation.tokenizers.deletion_base import DeletionBase
 
 
 class GenomicDeletion(DeletionBase):
     """Class for tokenizing Deletion at the genomic reference sequence."""
 
     def return_token(self, params: Dict) -> Optional[GenomicDeletionToken]:
-        """Return Genomic Deletion token if match
-
-        :param Dict params: Matched parameters for deletion
-        :return: `GenomicDeletionToken` if on c coordinate, else `None`
-        """
-        if params["coordinate_type"] == "g":
+        """Return Genomic Deletion token."""
+        if self.parts["coordinate_type"] == "g":
             return GenomicDeletionToken(**params)
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/tokenizers/genomic_deletion_range.py` & `variation-normalizer-0.7.dev0/variation/tokenizers/genomic_deletion_range.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/tokenizers/genomic_delins.py` & `variation-normalizer-0.7.dev0/variation/tokenizers/genomic_delins.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/tokenizers/genomic_duplication.py` & `variation-normalizer-0.7.dev0/variation/tokenizers/genomic_duplication.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/tokenizers/genomic_insertion.py` & `variation-normalizer-0.7.dev0/variation/tokenizers/genomic_insertion.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/tokenizers/genomic_silent_mutation.py` & `variation-normalizer-0.7.dev0/variation/tokenizers/genomic_silent_mutation.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/tokenizers/genomic_substitution.py` & `variation-normalizer-0.7.dev0/variation/tokenizers/genomic_substitution.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/tokenizers/genomic_uncertain_deletion.py` & `variation-normalizer-0.7.dev0/variation/tokenizers/genomic_uncertain_deletion.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/tokenizers/gnomad_vcf.py` & `variation-normalizer-0.7.dev0/variation/tokenizers/gnomad_vcf.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,19 @@
     Nomenclature
 from .tokenizer import Tokenizer
 
 
 class GnomadVCF(Tokenizer):
     """The gnomad VCF tokenizer class"""
 
-    splitter = re.compile(
-        r"^(?P<chromosome>(chr|chromosome)?([1-9]|[1][0-9]|[2][0-2]|X|Y))-"
-        r"(?P<pos>[1-9]\d*)-(?P<ref>[actg]+)-(?P<alt>[actg]+)$", re.IGNORECASE)
+    def __init__(self) -> None:
+        """Initialize the gnomad VCF tokenizer class"""
+        self.splitter = re.compile(
+            r"^(?P<chromosome>(chr|chromosome)?([1-9]|[1][0-9]|[2][0-2]|X|Y))-"
+            r"(?P<pos>[1-9]\d*)-(?P<ref>(?i)[actg]+)-(?P<alt>(?i)[actg]+)$")
 
     def match(self, input_string: str) -> Optional[List[Token]]:
         """Return a GnomadVCFToken if a match exists.
 
         :param str input_string: The input string to match
         :return: List of tokens
         """
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/tokenizers/hgvs.py` & `variation-normalizer-0.7.dev0/variation/tokenizers/hgvs.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,16 +11,18 @@
 from .tokenizer import Tokenizer
 from .locus_reference_genomic import LocusReferenceGenomic
 
 
 class HGVS(Tokenizer):
     """The HGVS tokenizer class."""
 
-    parser = Parser()
-    validator = IntrinsicValidator()
+    def __init__(self) -> None:
+        """Initialize the HGVS tokenizer class."""
+        self.parser = Parser()
+        self.validator = IntrinsicValidator()
 
     def match(self, input_string: str) -> Optional[Token]:
         """Return token matches from input string."""
         valid_prefix = False
         for prefix in REFSEQ_PREFIXES:
             if input_string.upper().startswith(prefix):
                 valid_prefix = True
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/tokenizers/insertion_base.py` & `variation-normalizer-0.7.dev0/variation/tokenizers/insertion_base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 """A module for Insertion Tokenization Base Class."""
 from abc import abstractmethod
 from typing import Optional, Dict, List
 
 from variation.schemas.token_response_schema import Insertion, TokenMatchType, Token
 from .tokenizer import Tokenizer
+from .caches import AminoAcidCache, NucleotideCache
+from .tokenize_base import TokenizeBase
 
 
 class InsertionBase(Tokenizer):
     """Class for tokenizing Insertion."""
 
-    def __init__(self) -> None:
-        """Initialize the Insertion Class."""
+    def __init__(self, amino_acid_cache: AminoAcidCache,
+                 nucleotide_cache: NucleotideCache) -> None:
+        """Initialize the Insertion Class.
+
+        :param AminoAcidCache amino_acid_cache: Valid amino acid codes
+        :param NucleotideCache nucleotide_cache: Valid nucleotides
+        """
         self.parts = None
+        self.tokenize_base = TokenizeBase(amino_acid_cache, nucleotide_cache)
 
     def match(self, input_string: str) -> Optional[Insertion]:
         """Return tokens that match the input string."""
         if input_string is None:
             return None
 
         self.parts = {
@@ -57,21 +65,22 @@
         if not parts[0].startswith("c.") and not parts[0].startswith("g."):
             return None
 
         # Get reference sequence
         coordinate_type = parts[0][:1]
         parts[0] = parts[0][2:]
 
-        positions = self.get_positions_deleted(parts)
+        positions = self.tokenize_base.get_positions_deleted(parts)
         if not positions:
             return None
         start_pos = positions[0]
         end_pos = positions[1]
 
-        inserted_sequences = self.get_transcript_genomic_inserted_sequence(parts)
+        inserted_sequences = \
+            self.tokenize_base.get_transcript_genomic_inserted_sequence(parts)
         if not inserted_sequences or not inserted_sequences[0]:
             return None
 
         if "_" in parts[0] and parts[0].count("_") ==\
                 2 and not inserted_sequences[1]:
             return None
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/tokenizers/locus_reference_genomic.py` & `variation-normalizer-0.7.dev0/variation/tokenizers/locus_reference_genomic.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,18 @@
     LocusReferenceGenomicToken
 from .tokenizer import Tokenizer
 
 
 class LocusReferenceGenomic(Tokenizer):
     """The LRG class for tokenization."""
 
-    regex = r"lrg_\d+((t|p)\d+)?"
-
     def __init__(self) -> None:
         """Initialize the LRG class."""
+        self.splitter = re.compile(r"(\d+)")
+        self.regex = r"lrg_\d+((t|p)\d+)?"
         self.parts = None
 
     def match(self, input_string: str) -> Optional[LocusReferenceGenomicToken]:
         """Return a LocusReferenceGenomicToken if a match exists.
 
         :param str input_string: The input string to match
         :return: A LocusReferenceGenomicToken if a match exists.
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/tokenizers/polypeptide_sequence_variation_base.py` & `variation-normalizer-0.7.dev0/variation/tokenizers/polypeptide_sequence_variation_base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 """A module for Polypeptide Sequence Variation Tokenization Base Class."""
+import re
 from abc import abstractmethod
 from typing import List, Optional
 
-from bioutils.sequences import aa3_to_aa1, aa3_to_aa1_lut
-
+from .caches import AminoAcidCache
 from .tokenizer import Tokenizer
 from ..schemas.token_response_schema import Token
 
 
 class PolypeptideSequenceVariationBase(Tokenizer):
     """Class for tokenizing Polypeptide Sequence Variations."""
 
-    def __init__(self) -> None:
-        """Initialize the Polypeptide Sequence Variation Base Class."""
+    def __init__(self, amino_acid_cache: AminoAcidCache) -> None:
+        """Initialize the Polypeptide Sequence Variation Base Class.
+
+        :param AminoAcidCache amino_acid_cache: Valid amino acid codes.
+        """
+        self.amino_acid_cache = amino_acid_cache
+        self.splitter = re.compile(r"(\d+)")
         self.psub = None
 
     def _set_psub(self, amino_acid: str, position: int, new_amino_acid: str) -> None:
         """Initialize protein substitution.
 
         :param str amino_acid: Reference amino acid
         :param int position: The position of the amino acid substituted
         :param str new_amino_acid: The new amino_acid
         """
-        for (key, aa_val) in [("amino_acid", amino_acid),
-                              ("new_amino_acid", new_amino_acid)]:
-            if len(aa_val) == 1:
-                self.psub[key] = aa_val.upper()
-            else:
-                try:
-                    self.psub[key] = aa3_to_aa1(aa_val.capitalize())
-                except KeyError:
-                    self.psub[key] = None
+        self.psub["amino_acid"] = amino_acid.upper() if len(amino_acid) == 1 \
+            else self.amino_acid_cache.convert_three_to_one(amino_acid)
         self.psub["position"] = int(position)
+        self.psub["new_amino_acid"] = new_amino_acid.upper() if \
+            len(new_amino_acid) == 1 else \
+            self.amino_acid_cache.convert_three_to_one(new_amino_acid)
 
     def _is_valid_amino_acid(self, amino_acids: List) -> bool:
         """Return whether or not amino acids are valid."""
-        valid = aa3_to_aa1_lut.values()
         for amino_acid_code in amino_acids:
-            if amino_acid_code not in valid:
+            if not self.amino_acid_cache.__contains__(amino_acid_code):
                 return False
         return True
 
     @abstractmethod
     def match(self, input_string: str) -> Optional[Token]:
         """Return tokens that match the input string."""
         raise NotImplementedError
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/tokenizers/polypeptide_truncation.py` & `variation-normalizer-0.7.dev0/variation/tokenizers/polypeptide_truncation.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,19 +36,19 @@
             split_whitespace = input_string.split()
             if not input_string.startswith("p."):
                 if not len(split_whitespace) == 2:
                     return None
             else:
                 p_count = input_string.count("p.")
                 if p_count == 1:
-                    psub_parts = self.splitter_paren_digits.split(input_string)
+                    psub_parts = self.splitter.split(input_string)
             if len(split_whitespace) == 2:
                 psub_parts = split_whitespace
         else:
-            psub_parts = self.splitter_paren_digits.split(input_string)
+            psub_parts = self.splitter.split(input_string)
 
         self._get_psub(psub_parts)
 
         if None not in self.psub.values():
             if self.psub["new_amino_acid"] == "*" or \
                     self.psub["new_amino_acid"] == "Ter":
                 amino_acids = {self.psub["amino_acid"]}
@@ -88,9 +88,9 @@
         elif psub_parts_len == 2:
             if "ter" in psub_parts[0]:
                 if "p." not in psub_parts[0] and "p." in psub_parts[1]:
                     psub_parts[0] = f"p.{psub_parts[0]}"
                 check_nonsense = f"({psub_parts[0].replace('ter', '*')})"
                 if check_nonsense == psub_parts[1]:
                     psub_parts = \
-                        self.splitter_paren_digits.split(psub_parts[0].split("p.")[-1])
+                        self.splitter.split(psub_parts[0].split("p.")[-1])
                     self._get_psub(psub_parts)
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/tokenizers/protein_delins.py` & `variation-normalizer-0.7.dev0/variation/tokenizers/protein_deletion.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,71 +1,78 @@
-"""A module for Protein DelIns Tokenization Class."""
-from typing import List, Optional
+"""A module for Protein Deletion Tokenization Class."""
+from typing import Optional, List
 
 from pydantic.error_wrappers import ValidationError
 
-from variation.schemas.token_response_schema import ProteinDelInsToken, \
+from variation.schemas.token_response_schema import ProteinDeletionToken, \
     TokenMatchType
+from .caches import AminoAcidCache, NucleotideCache
 from .tokenizer import Tokenizer
+from .tokenize_base import TokenizeBase
 
 
-class ProteinDelIns(Tokenizer):
-    """Class for tokenizing DelIns on the protein reference sequence."""
+class ProteinDeletion(Tokenizer):
+    """Class for tokenizing Deletions on the protein reference sequence."""
 
-    def __init__(self) -> None:
-        """Initialize the Protein DelIns Class."""
+    def __init__(self, amino_acid_cache: AminoAcidCache,
+                 nucleotide_cache: NucleotideCache) -> None:
+        """Initialize the Protein Deletion Class.
+
+        :param AminoAcidCache amino_acid_cache: Valid amino acid codes
+        :param NucleotideCache nucleotide_cache: Valid nucleotides
+        """
         self.parts = None
+        self.tokenize_base = TokenizeBase(amino_acid_cache, nucleotide_cache)
 
-    def match(self, input_string: str) -> Optional[ProteinDelInsToken]:
+    def match(self, input_string: str) -> Optional[ProteinDeletionToken]:
         """Return token that match the input string."""
         if input_string is None:
             return None
 
+        self.parts = {
+            "used_one_letter": False,
+            "token": input_string,
+            "input_string": input_string,
+            "match_type": TokenMatchType.UNSPECIFIED.value,
+            "start_aa_del": None,
+            "start_pos_del": None,
+            "end_aa_del": None,
+            "end_pos_del": None
+        }
+
         input_string = str(input_string).lower()
 
-        if "delins" not in input_string:
+        if "c." in input_string or "g." in input_string:
             return None
 
         if input_string.startswith("p."):
             input_string = input_string[2:]
 
         if input_string.startswith("(") and input_string.endswith(")"):
             input_string = input_string[1:-1]
 
-        self.parts = {
-            "used_one_letter": False,
-            "token": input_string,
-            "input_string": input_string,
-            "match_type": TokenMatchType.UNSPECIFIED.value,
-            "start_aa_del": None,
-            "start_pos_del": None,
-            "end_aa_del": None,
-            "end_pos_del": None,
-            "inserted_sequence": None
-        }
+        if not input_string.endswith("del"):
+            return None
 
-        parts = input_string.split("delins")
+        parts = input_string.split("del")
         self._get_parts(parts)
 
         try:
-            return ProteinDelInsToken(**self.parts)
+            return ProteinDeletionToken(**self.parts)
         except ValidationError:
             return None
 
     def _get_parts(self, parts: List) -> None:
-        """Get parts for DelIns.
+        """Get parts for Protein Deletion.
 
         :param List parts: Parts of input string
         """
         if len(parts) != 2:
-            return None
+            return
 
-        # Get reference sequence
-        range_aa_pos = self.get_aa_pos_range(parts)
+        range_aa_pos = self.tokenize_base.get_aa_pos_range(parts)
         if range_aa_pos:
             self.parts["start_aa_del"] = range_aa_pos[0]
             self.parts["end_aa_del"] = range_aa_pos[1]
             self.parts["start_pos_del"] = range_aa_pos[2]
             self.parts["end_pos_del"] = range_aa_pos[3]
             self.parts["used_one_letter"] = range_aa_pos[4]
-        self.parts["inserted_sequence"] = self.get_protein_inserted_sequence(
-            parts, self.parts["used_one_letter"])
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/tokenizers/protein_substitution.py` & `variation-normalizer-0.7.dev0/variation/tokenizers/protein_substitution.py`

 * *Files 21% similar despite different names*

```diff
@@ -17,35 +17,31 @@
             Otherwise, None.
         """
         if input_string is None:
             return None
 
         input_string = str(input_string).lower()
 
-        if input_string.endswith(("*", "ter")):
-            # Handled in polypeptide truncation
-            return None
-
         psub_parts = None
         self.psub = {
             "amino_acid": None,
             "position": None,
             "new_amino_acid": None
         }
 
         if "." in input_string:
             if not input_string.startswith("p."):
                 return None
             p_count = input_string.count("p.")
             if p_count == 1:
-                psub_parts = self.splitter_paren_digits.split(input_string)
+                psub_parts = self.splitter.split(input_string)
             elif p_count == 2:
                 psub_parts = input_string.split()
         else:
-            psub_parts = self.splitter_paren_digits.split(input_string)
+            psub_parts = self.splitter.split(input_string)
 
         self._get_psub(psub_parts)
 
         if None not in self.psub.values():
             amino_acids = {self.psub["amino_acid"],
                            self.psub["new_amino_acid"]}
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/tokenizers/reference_sequence.py` & `variation-normalizer-0.7.dev0/variation/tokenizers/reference_sequence.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/tokenizers/silent_mutation.py` & `variation-normalizer-0.7.dev0/variation/tokenizers/silent_mutation.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,17 +29,17 @@
         }
 
         if "." in input_string:
             if not input_string.startswith("p."):
                 return None
             p_count = input_string.count("p.")
             if p_count == 1:
-                psub_parts = self.splitter_paren_digits.split(input_string)
+                psub_parts = self.splitter.split(input_string)
         else:
-            psub_parts = self.splitter_paren_digits.split(input_string)
+            psub_parts = self.splitter.split(input_string)
 
         self._get_psub(psub_parts)
 
         if None not in self.psub.values():
             if self.psub["new_amino_acid"] == "=":
                 if not self._is_valid_amino_acid({self.psub["amino_acid"]}):
                     return None
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/tokenizers/single_nucleotide_variation_base.py` & `variation-normalizer-0.7.dev0/variation/tokenizers/single_nucleotide_variation_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 """A module for Single Nucleotide Variation Tokenization Base Class."""
+import re
 from abc import abstractmethod
 from typing import List, Optional, Dict
 
-from variation.schemas.token_response_schema import SingleNucleotideVariation, \
-    TokenMatchType
+from variation.schemas.token_response_schema import \
+    SingleNucleotideVariation, TokenMatchType
+from variation.tokenizers.caches import NucleotideCache
 from .tokenizer import Tokenizer
 
 
 class SingleNucleotideVariationBase(Tokenizer):
     """Class for tokenizing Single Nucleotide Variations."""
 
     def __init__(self) -> None:
         """Initialize the Single Nucleotide Variation Base Class."""
+        self.splitter = re.compile(r"(\d+)")
         self.sub = None
+        self.nucleotide_cache = NucleotideCache()
 
     def match(self, input_string: str) -> Optional[SingleNucleotideVariation]:
         """Return a SingleNucleotideVariationToken match if one exists.
 
         :param str input_string: The input string to match
         :return: A SingleNucleotideVariationToken if a match one exists.
         """
@@ -31,15 +35,15 @@
             "coordinate_type": None
         }
 
         # TODO: Need to add m., and n.
         if "c." not in input_string and "g." not in input_string:
             return None
 
-        sub_parts = self.splitter_paren_digits.split(input_string)
+        sub_parts = self.splitter.split(input_string)
         self._get_sub(sub_parts)
         if None not in self.sub.values():
             params = {
                 "token": input_string,
                 "input_string": input_string,
                 "match_type": TokenMatchType.UNSPECIFIED.value,
                 "position": self.sub["position"],
@@ -72,16 +76,17 @@
                 sub_parts[0] = sub_parts[0].split("(")[-1]
                 sub_parts[2] = sub_parts[2].split(")")[0]
 
             if sub_parts[1].isdigit():
                 if ">" in sub_parts[2]:
                     # Substitution
                     ref_nuc, new_nuc = sub_parts[2].split(">")
-                    if ref_nuc.upper() in self.base_nucleotides \
-                            and new_nuc.upper() in self.base_nucleotides:
+                    nucleotides = self.nucleotide_cache.nucleotides.keys()
+                    if ref_nuc.upper() in nucleotides \
+                            and new_nuc.upper() in nucleotides:  # noqa: E501
                         self._set_sub(ref_nuc, sub_parts[1], new_nuc,
                                       sub_parts[0].split(".")[0])
                 elif sub_parts[2] == "=":
                     # Silent Mutation
                     self._set_sub(None, sub_parts[1], sub_parts[2],
                                   sub_parts[0].split(".")[0])
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/tokenizers/tokenizer.py` & `variation-normalizer-0.7.dev0/variation/tokenizers/tokenize_base.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,27 @@
-"""Module for Tokenization."""
+"""Module for commonly used tokenization methods."""
+from typing import Tuple, Optional, Union, List
 import re
-from abc import ABC, abstractmethod
-from typing import Optional, Tuple, Union, List
 
-from bioutils.sequences import aa3_to_aa1_lut, aa3_to_aa1, aa1_to_aa3
+from variation.tokenizers.caches import NucleotideCache, AminoAcidCache
 
-from variation.schemas.token_response_schema import Token
 
+class TokenizeBase:
+    """Class for Tokenize methods."""
 
-class Tokenizer(ABC):
-    """The tokenizer class."""
+    def __init__(self, amino_acid_cache: AminoAcidCache,
+                 nucleotide_cache: NucleotideCache) -> None:
+        """Initialize Token Base class.
 
-    base_nucleotides = {"A", "C", "T", "G", "N"}
-    splitter_char_digit = re.compile("([a-zA-Z]+)([0-9]+)")
-    splitter_paren_digits = re.compile(r"(\d+)")
-
-    @abstractmethod
-    def match(self, input_string: str) -> Optional[Token]:
-        """Return tokens that match the input string."""
-        raise NotImplementedError
+        :param AminoAcidCache amino_acid_cache: Valid amino acid codes
+        :param NucleotideCache nucleotide_cache: Valid nucleotides
+        """
+        self.nucleotide_cache = nucleotide_cache
+        self.amino_acid_cache = amino_acid_cache
+        self.splitter_char_digit = re.compile("([a-zA-Z]+)([0-9]+)")
 
     def get_amino_acid_and_pos(
         self, part: List, used_one_letter: bool
     ) -> Optional[Tuple[str, int, bool]]:
         """Return amino acid and position.
 
         :param List part: Tokenized input string
@@ -40,27 +39,22 @@
                 (len(char_and_digits[0]) + len(char_and_digits[1])):
             return None
 
         aa = char_and_digits[0]
         if len(aa) == 1:
             if not used_one_letter:
                 used_one_letter = True
-
-            try:
-                tmp_aa = aa1_to_aa3(aa.upper())
-            except KeyError:
-                tmp_aa = None
+            tmp_aa = \
+                self.amino_acid_cache.amino_acid_code_conversion[aa.upper()]
         else:
-            if aa.capitalize() in aa3_to_aa1_lut:
-                tmp_aa = aa
-            else:
-                tmp_aa = None
+            tmp_aa = aa
         pos = char_and_digits[1]
 
-        if not tmp_aa or not pos.isdigit():
+        if not self.amino_acid_cache.__contains__(tmp_aa) \
+                or not pos.isdigit():
             return None
         return aa.upper(), pos, used_one_letter
 
     def get_protein_inserted_sequence(self, parts: List,
                                       used_one_letter: bool) -> Optional[str]:
         """Return inserted sequence for protein reference sequence.
 
@@ -73,32 +67,31 @@
         inserted_sequence = ""
         if used_one_letter:
             for i in range(len(parts[1])):
                 aa = parts[1][i:i + 1]
                 if len(aa) != 1:
                     return None
                 try:
-                    aa3_to_aa1_lut[aa1_to_aa3(aa.upper())]
+                    self.amino_acid_cache.amino_acid_code_conversion[aa.upper()]  # noqa: E501
                 except KeyError:
                     return None
                 else:
                     inserted_sequence += aa.upper()
         else:
             for i in range(0, len(parts[1]), 3):
                 aa = parts[1][i:i + 3]
-                if len(aa) != 3 or aa.capitalize() not in aa3_to_aa1_lut:
+                if len(aa) != 3 or not self.amino_acid_cache.__contains__(aa):
                     if aa != "ter":
                         return None
+                inserted_sequence += \
+                    self.amino_acid_cache.convert_three_to_one(aa)
 
-                try:
-                    inserted_sequence += aa3_to_aa1(aa.capitalize())
-                except KeyError:
-                    return None
-
-        return inserted_sequence if inserted_sequence else None
+        if inserted_sequence == "":
+            return None
+        return inserted_sequence
 
     def get_aa_pos_range(self,
                          parts: List) -> Optional[Tuple[str, str, str, int, bool]]:
         """Get amino acid(s) and positions(s) for protein reference sequence.
 
         :param List parts: Tokenized input string
         :return: Beginning AA, End AA,  Beginning position, End position,
@@ -194,15 +187,15 @@
     def get_sequence(self, part: str) -> Optional[str]:
         """Return validated sequence for transcript and genomic references.
 
         :param str part: Sequence to validate
         :return: Sequence of nucleotides
         """
         for char in part:
-            if char.upper() not in self.base_nucleotides:
+            if char.upper() not in self.nucleotide_cache.base_nucleotides:
                 return None
         return part.upper()
 
     def get_valid_digits(self, part: str) -> Optional[Tuple[str, str]]:
         """Return valid digits after splitting on `_`.
 
         :param str part: Range of digits
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/translators/__init__.py` & `variation-normalizer-0.7.dev0/variation/translators/__init__.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/translators/amplification.py` & `variation-normalizer-0.7.dev0/variation/translators/amplification.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/translators/coding_dna_deletion.py` & `variation-normalizer-0.7.dev0/variation/translators/coding_dna_deletion.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/translators/coding_dna_delins.py` & `variation-normalizer-0.7.dev0/variation/translators/coding_dna_delins.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/translators/coding_dna_insertion.py` & `variation-normalizer-0.7.dev0/variation/translators/coding_dna_insertion.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/translators/coding_dna_silent_mutation.py` & `variation-normalizer-0.7.dev0/variation/translators/coding_dna_silent_mutation.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/translators/coding_dna_substitution.py` & `variation-normalizer-0.7.dev0/variation/translators/coding_dna_substitution.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/translators/genomic_deletion.py` & `variation-normalizer-0.7.dev0/variation/translators/genomic_deletion.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/translators/genomic_deletion_range.py` & `variation-normalizer-0.7.dev0/variation/translators/genomic_deletion_range.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/translators/genomic_delins.py` & `variation-normalizer-0.7.dev0/variation/translators/genomic_delins.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/translators/genomic_duplication.py` & `variation-normalizer-0.7.dev0/variation/translators/genomic_duplication.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/translators/genomic_insertion.py` & `variation-normalizer-0.7.dev0/variation/translators/genomic_insertion.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/translators/genomic_silent_mutation.py` & `variation-normalizer-0.7.dev0/variation/translators/genomic_silent_mutation.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/translators/genomic_substitution.py` & `variation-normalizer-0.7.dev0/variation/translators/genomic_substitution.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/translators/genomic_uncertain_deletion.py` & `variation-normalizer-0.7.dev0/variation/translators/genomic_uncertain_deletion.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/translators/polypeptide_truncation.py` & `variation-normalizer-0.7.dev0/variation/translators/polypeptide_truncation.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/translators/protein_deletion.py` & `variation-normalizer-0.7.dev0/variation/translators/protein_deletion.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/translators/protein_delins.py` & `variation-normalizer-0.7.dev0/variation/translators/protein_delins.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/translators/protein_insertion.py` & `variation-normalizer-0.7.dev0/variation/translators/protein_insertion.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/translators/protein_substitution.py` & `variation-normalizer-0.7.dev0/variation/translators/protein_substitution.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/translators/silent_mutation.py` & `variation-normalizer-0.7.dev0/variation/translators/silent_mutation.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/translators/translate.py` & `variation-normalizer-0.7.dev0/variation/translators/translate.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/translators/translator.py` & `variation-normalizer-0.7.dev0/variation/translators/translator.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/utils.py` & `variation-normalizer-0.7.dev0/variation/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import List, Tuple, Optional, Dict
 import re
 
 from ga4gh.vrsatile.pydantic.vrs_models import Text
 from ga4gh.vrsatile.pydantic.vrsatile_models import VariationDescriptor, GeneDescriptor
 from ga4gh.core import ga4gh_identify
 from ga4gh.vrs import models
-from cool_seq_tool.data_sources import SeqRepoAccess
+from uta_tools.data_sources import SeqRepoAccess
 
 from variation.schemas.classification_response_schema import ClassificationType
 from variation.schemas.validation_response_schema import ValidationSummary, \
     ValidationResult
 from variation.schemas.token_response_schema import Token
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/validators/__init__.py` & `variation-normalizer-0.7.dev0/variation/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/validators/amplification.py` & `variation-normalizer-0.7.dev0/variation/validators/delins_base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,115 +1,114 @@
-"""Module for Amplification validation"""
+"""The module for DelIns Validation."""
 from typing import List, Dict, Optional
+import logging
 
-from ga4gh.vrsatile.pydantic.vrs_models import CopyChange
-from ga4gh.vrs import models
+from ga4gh.vrsatile.pydantic.vrs_models import RelativeCopyClass
 
-from variation.schemas.token_response_schema import GeneMatchToken, TokenType
-from variation.schemas.classification_response_schema import Classification,\
+from variation.schemas.classification_response_schema import Classification, \
     ClassificationType
 from variation.schemas.app_schemas import Endpoint
-from variation.schemas.token_response_schema import Token
+from variation.schemas.token_response_schema import Token, GeneMatchToken
 from variation.validators.validator import Validator
 from variation.schemas.normalize_response_schema\
     import HGVSDupDelMode as HGVSDupDelModeEnum
-from variation.utils import get_priority_sequence_location
 
+logger = logging.getLogger("variation")
+logger.setLevel(logging.DEBUG)
 
-class Amplification(Validator):
-    """The Insertion Validator Base class."""
+
+class DelInsBase(Validator):
+    """The DelIns Validator Base class."""
+
+    def is_token_instance(self, t: Token) -> bool:
+        """Check to see if token is instance of a token type.
+
+        :param Token t: Classification token to find type of
+        :return: `True` if token is instance of class token. `False` otherwise.
+        """
+        raise NotImplementedError
+
+    def variation_name(self) -> str:
+        """Return the variation name.
+
+        :return: variation class name
+        """
+        raise NotImplementedError
+
+    def get_gene_tokens(
+            self, classification: Classification) -> List[GeneMatchToken]:
+        """Return a list of gene tokens for a classification.
+
+        :param Classification classification: Classification for a list of
+            tokens
+        :return: A list of gene tokens for the classification
+        """
+        raise NotImplementedError
+
+    async def get_transcripts(self, gene_tokens: List, classification: Classification,
+                              errors: List) -> Optional[List[str]]:
+        """Get transcript accessions for a given classification.
+
+        :param List gene_tokens: A list of gene tokens
+        :param Classification classification: A classification for a list of
+            tokens
+        :param List errors: List of errors
+        :return: List of transcript accessions
+        """
+        raise NotImplementedError
+
+    def validates_classification_type(
+            self, classification_type: ClassificationType) -> bool:
+        """Check that classification type can be validated by validator.
+
+        :param ClassificationType classification_type: The type of variation
+        :return: `True` if classification_type matches validator's
+            classification type. `False` otherwise.
+        """
+        raise NotImplementedError
 
     async def get_valid_invalid_results(
         self, classification_tokens: List, transcripts: List,
         classification: Classification, results: List, gene_tokens: List,
         mane_data_found: Dict, is_identifier: bool,
         hgvs_dup_del_mode: HGVSDupDelModeEnum,
         endpoint_name: Optional[Endpoint] = None,
         baseline_copies: Optional[int] = None,
-        copy_change: Optional[CopyChange] = None,
+        relative_copy_class: Optional[RelativeCopyClass] = None,
         do_liftover: bool = False
     ) -> None:
         """Add validation result objects to a list of results.
 
         :param List classification_tokens: A list of classification Tokens
         :param List transcripts: A list of transcript accessions
         :param Classification classification: A classification for a list of
             tokens
         :param List results: Stores validation result objects
         :param List gene_tokens: List of GeneMatchTokens for a classification
         :param Dict mane_data_found: MANE Transcript information found
         :param bool is_identifier: `True` if identifier is given for exact
             location. `False` otherwise.
-        :param HGVSDupDelModeEnum hgvs_dup_del_mode: Must be: `default`,
-            `copy_number_count`, `copy_number_change`, `repeated_seq_expr`,
-            `literal_seq_expr`. This parameter determines how to represent HGVS dup/del
-            expressions as VRS objects.
+        :param HGVSDupDelModeEnum hgvs_dup_del_mode: Must be: `default`, `absolute_cnv`,
+            `relative_cnv`, `repeated_seq_expr`, `literal_seq_expr`. This parameter
+            determines how to represent HGVS dup/del expressions as VRS objects.
         :param Optional[Endpoint] endpoint_name: Then name of the endpoint being used
         :param Optional[int] baseline_copies: Baseline copies number
-        :param Optional[CopyChange] copy_change: The copy change
+        :param Optional[RelativeCopyClass] relative_copy_class: The relative copy class
         :param bool do_liftover: Whether or not to liftover to GRCh38 assembly
         """
-        valid_variations = list()
-        gene_match_tokens = [token for token in classification.all_tokens
-                             if token.token_type == "GeneSymbol"]
-        for s in classification_tokens:
-            errors = list()
-            cx = None
-
-            if gene_match_tokens:
-                gene_match_token = gene_match_tokens[0]
-                gene = gene_match_token.token
-                gene_descriptor = gene_match_token.gene_descriptor
-                seq_loc = get_priority_sequence_location(
-                    gene_descriptor, self.seqrepo_access)
-                if seq_loc:
-                    cx = self.vrs.to_cx_var(
-                        models.SequenceLocation(**seq_loc),
-                        CopyChange.HIGH_LEVEL_GAIN)
-                else:
-                    errors.append(f"No SequenceLocation found for gene: {gene}")
-            else:
-                errors.append("No gene_tokens found")
-
-            self.add_validation_result(cx, valid_variations, results, classification,
-                                       s, None, gene_tokens, errors)
-
-    def get_gene_tokens(self, classification: Classification) -> List[GeneMatchToken]:
-        """Return gene tokens for a classification.
+        raise NotImplementedError
 
-        :param Classification classification: The classification for tokens
-        :return: A list of Gene Match Tokens in the classification
-        """
-        return self.get_protein_gene_symbol_tokens(classification)
+    def check_pos_index(self, t: str, s: Token, errors: List) -> None:
+        """Check that position exists on transcript.
 
-    async def get_transcripts(self, gene_tokens: List, classification: Classification,
-                              errors: List) -> Optional[List[str]]:
-        """Get transcript accessions for a given classification.
-
-        :param List gene_tokens: A list of gene tokens
-        :param Classification classification: A classification for a list of tokens
+        :param str t: Transcript accession
+        :param Token s: Classification token
         :param List errors: List of errors
-        :return: List of transcript accessions
-        """
-        return []
-
-    def variation_name(self) -> str:
-        """Return the variation name."""
-        return "amplification"
-
-    def is_token_instance(self, t: Token) -> bool:
-        """Check that token is Amplification.
-
-        :param Token t: Classification token
-        :return: `True` if amplification. `False` otherwise
-        """
-        return t.token_type == TokenType.AMPLIFICATION
-
-    def validates_classification_type(self,
-                                      classification_type: ClassificationType) -> bool:
-        """Check that classification type can be validated by validator.
-
-        :param ClassificationType classification_type: The type of variation
-        :return: `True` if classification_type matches validator's
-            classification type. `False` otherwise.
         """
-        return classification_type == ClassificationType.AMPLIFICATION
+        if s.end_pos_del:
+            sequence, w = self.seqrepo_access.get_reference_sequence(
+                t, int(s.start_pos_del), int(s.end_pos_del))
+        else:
+            sequence, w = self.seqrepo_access.get_reference_sequence(
+                t, int(s.start_pos_del))
+        if sequence is None:
+            errors.append(w)
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/validators/coding_dna_deletion.py` & `variation-normalizer-0.7.dev0/variation/validators/coding_dna_deletion.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """The module for Coding DNA Deletion Validation."""
 import logging
 from typing import List, Optional, Dict
 
-from ga4gh.vrsatile.pydantic.vrs_models import CopyChange
+from ga4gh.vrsatile.pydantic.vrs_models import RelativeCopyClass
 
 from variation.schemas.app_schemas import Endpoint
 from variation.validators.duplication_deletion_base import\
     DuplicationDeletionBase
 from variation.schemas.classification_response_schema import \
     ClassificationType, Classification
 from variation.schemas.token_response_schema import GeneMatchToken, Token
@@ -36,35 +36,34 @@
     async def get_valid_invalid_results(
         self, classification_tokens: List, transcripts: List,
         classification: Classification, results: List, gene_tokens: List,
         mane_data_found: Dict, is_identifier: bool,
         hgvs_dup_del_mode: HGVSDupDelModeEnum,
         endpoint_name: Optional[Endpoint] = None,
         baseline_copies: Optional[int] = None,
-        copy_change: Optional[CopyChange] = None,
+        relative_copy_class: Optional[RelativeCopyClass] = None,
         do_liftover: bool = False
     ) -> None:
         """Add validation result objects to a list of results.
 
         :param List classification_tokens: A list of classification Tokens
         :param List transcripts: A list of transcript accessions
         :param Classification classification: A classification for a list of
             tokens
         :param List results: Stores validation result objects
         :param List gene_tokens: List of GeneMatchTokens for a classification
         :param Dict mane_data_found: MANE Transcript information found
         :param bool is_identifier: `True` if identifier is given for exact
             location. `False` otherwise.
-        :param HGVSDupDelModeEnum hgvs_dup_del_mode: Must be: `default`,
-            `copy_number_count`, `copy_number_change`, `repeated_seq_expr`,
-            `literal_seq_expr`. This parameter determines how to represent HGVS dup/del
-            expressions as VRS objects.
+        :param HGVSDupDelModeEnum hgvs_dup_del_mode: Must be: `default`, `absolute_cnv`,
+            `relative_cnv`, `repeated_seq_expr`, `literal_seq_expr`. This parameter
+            determines how to represent HGVS dup/del expressions as VRS objects.
         :param Optional[Endpoint] endpoint_name: Then name of the endpoint being used
         :param Optional[int] baseline_copies: Baseline copies number
-        :param Optional[CopyChange] copy_change: The copy change
+        :param Optional[RelativeCopyClass] relative_copy_class: The relative copy class
         :param bool do_liftover: Whether or not to liftover to GRCh38 assembly
         """
         valid_alleles = list()
         for s in classification_tokens:
             for t in transcripts:
                 errors = list()
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/validators/coding_dna_delins.py` & `variation-normalizer-0.7.dev0/variation/validators/coding_dna_delins.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """The module for Coding DNA DelIns Validation."""
 from typing import List, Optional, Dict
 import logging
 
-from ga4gh.vrsatile.pydantic.vrs_models import CopyChange
+from ga4gh.vrsatile.pydantic.vrs_models import RelativeCopyClass
 
 from variation.schemas.app_schemas import Endpoint
 from variation.validators.delins_base import DelInsBase
 from variation.schemas.classification_response_schema import \
     ClassificationType, Classification
 from variation.schemas.token_response_schema import Token
 from variation.schemas.token_response_schema import GeneMatchToken
@@ -36,35 +36,34 @@
     async def get_valid_invalid_results(
         self, classification_tokens: List, transcripts: List,
         classification: Classification, results: List, gene_tokens: List,
         mane_data_found: Dict, is_identifier: bool,
         hgvs_dup_del_mode: HGVSDupDelModeEnum,
         endpoint_name: Optional[Endpoint] = None,
         baseline_copies: Optional[int] = None,
-        copy_change: Optional[CopyChange] = None,
+        relative_copy_class: Optional[RelativeCopyClass] = None,
         do_liftover: bool = False
     ) -> None:
         """Add validation result objects to a list of results.
 
         :param List classification_tokens: A list of classification Tokens
         :param List transcripts: A list of transcript accessions
         :param Classification classification: A classification for a list of
             tokens
         :param List results: Stores validation result objects
         :param List gene_tokens: List of GeneMatchTokens for a classification
         :param Dict mane_data_found: MANE Transcript information found
         :param bool is_identifier: `True` if identifier is given for exact
             location. `False` otherwise.
-        :param HGVSDupDelModeEnum hgvs_dup_del_mode: Must be: `default`,
-            `copy_number_count`, `copy_number_change`, `repeated_seq_expr`,
-            `literal_seq_expr`. This parameter determines how to represent HGVS dup/del
-            expressions as VRS objects.
+        :param HGVSDupDelModeEnum hgvs_dup_del_mode: Must be: `default`, `absolute_cnv`,
+            `relative_cnv`, `repeated_seq_expr`, `literal_seq_expr`. This parameter
+            determines how to represent HGVS dup/del expressions as VRS objects.
         :param Optional[Endpoint] endpoint_name: Then name of the endpoint being used
         :param Optional[int] baseline_copies: Baseline copies number
-        :param Optional[CopyChange] copy_change: The copy change
+        :param Optional[RelativeCopyClass] relative_copy_class: The relative copy class
         :param bool do_liftover: Whether or not to liftover to GRCh38 assembly
         """
         valid_alleles = list()
         for s in classification_tokens:
             for t in transcripts:
                 errors = list()
                 t = self.get_accession(t, classification)
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/validators/coding_dna_insertion.py` & `variation-normalizer-0.7.dev0/variation/validators/coding_dna_insertion.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/validators/coding_dna_silent_mutation.py` & `variation-normalizer-0.7.dev0/variation/validators/coding_dna_silent_mutation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """The module for Coding DNA Substitution Validation."""
 import logging
 from typing import List, Optional, Dict
 
-from ga4gh.vrsatile.pydantic.vrs_models import CopyChange
+from ga4gh.vrsatile.pydantic.vrs_models import RelativeCopyClass
 
 from variation.schemas.classification_response_schema import ClassificationType, \
     Classification
 from variation.schemas.token_response_schema import Token
 from variation.schemas.token_response_schema import GeneMatchToken
 from variation.schemas.app_schemas import Endpoint
 from variation.schemas.normalize_response_schema\
@@ -36,35 +36,34 @@
     async def get_valid_invalid_results(
         self, classification_tokens: List, transcripts: List,
         classification: Classification, results: List, gene_tokens: List,
         mane_data_found: Dict, is_identifier: bool,
         hgvs_dup_del_mode: HGVSDupDelModeEnum,
         endpoint_name: Optional[Endpoint] = None,
         baseline_copies: Optional[int] = None,
-        copy_change: Optional[CopyChange] = None,
+        relative_copy_class: Optional[RelativeCopyClass] = None,
         do_liftover: bool = False
     ) -> None:
         """Add validation result objects to a list of results.
 
         :param List classification_tokens: A list of classification Tokens
         :param List transcripts: A list of transcript accessions
         :param Classification classification: A classification for a list of
             tokens
         :param List results: Stores validation result objects
         :param List gene_tokens: List of GeneMatchTokens for a classification
         :param Dict mane_data_found: MANE Transcript information found
         :param bool is_identifier: `True` if identifier is given for exact
             location. `False` otherwise.
-        :param HGVSDupDelModeEnum hgvs_dup_del_mode: Must be: `default`,
-            `copy_number_count`, `copy_number_change`, `repeated_seq_expr`,
-            `literal_seq_expr`. This parameter determines how to represent HGVS dup/del
-            expressions as VRS objects.
+        :param HGVSDupDelModeEnum hgvs_dup_del_mode: Must be: `default`, `absolute_cnv`,
+            `relative_cnv`, `repeated_seq_expr`, `literal_seq_expr`. This parameter
+            determines how to represent HGVS dup/del expressions as VRS objects.
         :param Optional[Endpoint] endpoint_name: Then name of the endpoint being used
         :param Optional[int] baseline_copies: Baseline copies number
-        :param Optional[CopyChange] copy_change: The copy change
+        :param Optional[RelativeCopyClass] relative_copy_class: The relative copy class
         :param bool do_liftover: Whether or not to liftover to GRCh38 assembly
         """
         await self.silent_mutation_valid_invalid_results(
             classification_tokens, transcripts, classification, results,
             gene_tokens, endpoint_name, mane_data_found, is_identifier,
             do_liftover=do_liftover
         )
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/validators/coding_dna_substitution.py` & `variation-normalizer-0.7.dev0/variation/validators/coding_dna_substitution.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """The module for Coding DNA Substitution Validation."""
 import logging
 from typing import List, Optional, Dict
 
-from ga4gh.vrsatile.pydantic.vrs_models import CopyChange
+from ga4gh.vrsatile.pydantic.vrs_models import RelativeCopyClass
 
 from variation.schemas.classification_response_schema import \
     ClassificationType, Classification
 from variation.schemas.token_response_schema import Token
 from variation.schemas.token_response_schema import GeneMatchToken
 from variation.schemas.app_schemas import Endpoint
 from variation.schemas.normalize_response_schema\
@@ -39,35 +39,34 @@
     async def get_valid_invalid_results(
         self, classification_tokens: List, transcripts: List,
         classification: Classification, results: List, gene_tokens: List,
         mane_data_found: Dict, is_identifier: bool,
         hgvs_dup_del_mode: HGVSDupDelModeEnum,
         endpoint_name: Optional[Endpoint] = None,
         baseline_copies: Optional[int] = None,
-        copy_change: Optional[CopyChange] = None,
+        relative_copy_class: Optional[RelativeCopyClass] = None,
         do_liftover: bool = False
     ) -> None:
         """Add validation result objects to a list of results.
 
         :param List classification_tokens: A list of classification Tokens
         :param List transcripts: A list of transcript accessions
         :param Classification classification: A classification for a list of
             tokens
         :param List results: Stores validation result objects
         :param List gene_tokens: List of GeneMatchTokens for a classification
         :param Dict mane_data_found: MANE Transcript information found
         :param bool is_identifier: `True` if identifier is given for exact
             location. `False` otherwise.
-        :param HGVSDupDelModeEnum hgvs_dup_del_mode: Must be: `default`,
-            `copy_number_count`, `copy_number_change`, `repeated_seq_expr`,
-            `literal_seq_expr`. This parameter determines how to represent HGVS dup/del
-            expressions as VRS objects.
+        :param HGVSDupDelModeEnum hgvs_dup_del_mode: Must be: `default`, `absolute_cnv`,
+            `relative_cnv`, `repeated_seq_expr`, `literal_seq_expr`. This parameter
+            determines how to represent HGVS dup/del expressions as VRS objects.
         :param Optional[Endpoint] endpoint_name: Then name of the endpoint being used
         :param Optional[int] baseline_copies: Baseline copies number
-        :param Optional[CopyChange] copy_change: The copy change
+        :param Optional[RelativeCopyClass] relative_copy_class: The relative copy class
         :param bool do_liftover: Whether or not to liftover to GRCh38 assembly
         """
         valid_alleles = list()
         for s in classification_tokens:
             for t in transcripts:
                 errors = list()
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/validators/delins_base.py` & `variation-normalizer-0.7.dev0/variation/validators/genomic_silent_mutation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,115 +1,89 @@
-"""The module for DelIns Validation."""
-from typing import List, Dict, Optional
+"""The module for Genomic Silent Mutation Validation."""
 import logging
+from typing import Optional, List, Dict
 
-from ga4gh.vrsatile.pydantic.vrs_models import CopyChange
+from ga4gh.vrsatile.pydantic.vrs_models import RelativeCopyClass
 
-from variation.schemas.classification_response_schema import Classification, \
-    ClassificationType
 from variation.schemas.app_schemas import Endpoint
-from variation.schemas.token_response_schema import Token, GeneMatchToken
-from variation.validators.validator import Validator
-from variation.schemas.normalize_response_schema\
-    import HGVSDupDelMode as HGVSDupDelModeEnum
+from variation.schemas.classification_response_schema import ClassificationType, \
+    Classification
+from variation.schemas.token_response_schema import Token
+from variation.schemas.normalize_response_schema import HGVSDupDelMode as HGVSDupDelModeEnum   # noqa: E501
+from .single_nucleotide_variation_base import SingleNucleotideVariationBase
+
 
 logger = logging.getLogger("variation")
 logger.setLevel(logging.DEBUG)
 
 
-class DelInsBase(Validator):
-    """The DelIns Validator Base class."""
-
-    def is_token_instance(self, t: Token) -> bool:
-        """Check to see if token is instance of a token type.
-
-        :param Token t: Classification token to find type of
-        :return: `True` if token is instance of class token. `False` otherwise.
-        """
-        raise NotImplementedError
-
-    def variation_name(self) -> str:
-        """Return the variation name.
-
-        :return: variation class name
-        """
-        raise NotImplementedError
-
-    def get_gene_tokens(
-            self, classification: Classification) -> List[GeneMatchToken]:
-        """Return a list of gene tokens for a classification.
-
-        :param Classification classification: Classification for a list of
-            tokens
-        :return: A list of gene tokens for the classification
-        """
-        raise NotImplementedError
+class GenomicSilentMutation(SingleNucleotideVariationBase):
+    """The Genomic Silent Mutation Validator class."""
 
     async def get_transcripts(self, gene_tokens: List, classification: Classification,
                               errors: List) -> Optional[List[str]]:
         """Get transcript accessions for a given classification.
 
         :param List gene_tokens: A list of gene tokens
         :param Classification classification: A classification for a list of
             tokens
         :param List errors: List of errors
         :return: List of transcript accessions
         """
-        raise NotImplementedError
-
-    def validates_classification_type(
-            self, classification_type: ClassificationType) -> bool:
-        """Check that classification type can be validated by validator.
-
-        :param ClassificationType classification_type: The type of variation
-        :return: `True` if classification_type matches validator's
-            classification type. `False` otherwise.
-        """
-        raise NotImplementedError
+        transcripts = await self.get_genomic_transcripts(classification, errors)
+        return transcripts
 
     async def get_valid_invalid_results(
         self, classification_tokens: List, transcripts: List,
         classification: Classification, results: List, gene_tokens: List,
         mane_data_found: Dict, is_identifier: bool,
         hgvs_dup_del_mode: HGVSDupDelModeEnum,
         endpoint_name: Optional[Endpoint] = None,
         baseline_copies: Optional[int] = None,
-        copy_change: Optional[CopyChange] = None,
+        relative_copy_class: Optional[RelativeCopyClass] = None,
         do_liftover: bool = False
     ) -> None:
         """Add validation result objects to a list of results.
 
         :param List classification_tokens: A list of classification Tokens
         :param List transcripts: A list of transcript accessions
         :param Classification classification: A classification for a list of
             tokens
         :param List results: Stores validation result objects
         :param List gene_tokens: List of GeneMatchTokens for a classification
         :param Dict mane_data_found: MANE Transcript information found
         :param bool is_identifier: `True` if identifier is given for exact
             location. `False` otherwise.
-        :param HGVSDupDelModeEnum hgvs_dup_del_mode: Must be: `default`,
-            `copy_number_count`, `copy_number_change`, `repeated_seq_expr`,
-            `literal_seq_expr`. This parameter determines how to represent HGVS dup/del
-            expressions as VRS objects.
+        :param HGVSDupDelModeEnum hgvs_dup_del_mode: Must be: `default`, `absolute_cnv`,
+            `relative_cnv`, `repeated_seq_expr`, `literal_seq_expr`. This parameter
+            determines how to represent HGVS dup/del expressions as VRS objects.
         :param Optional[Endpoint] endpoint_name: Then name of the endpoint being used
         :param Optional[int] baseline_copies: Baseline copies number
-        :param Optional[CopyChange] copy_change: The copy change
+        :param Optional[RelativeCopyClass] relative_copy_class: The relative copy class
         :param bool do_liftover: Whether or not to liftover to GRCh38 assembly
         """
-        raise NotImplementedError
+        await self.silent_mutation_valid_invalid_results(
+            classification_tokens, transcripts, classification, results,
+            gene_tokens, endpoint_name, mane_data_found, is_identifier,
+            do_liftover=do_liftover
+        )
 
-    def check_pos_index(self, t: str, s: Token, errors: List) -> None:
-        """Check that position exists on transcript.
+    def get_gene_tokens(self, classification: Classification) -> List:
+        """Return gene tokens for a classification.
 
-        :param str t: Transcript accession
-        :param Token s: Classification token
-        :param List errors: List of errors
+        :param Classification classification: The classification for tokens
+        :return: A list of Gene Match Tokens in the classification
         """
-        if s.end_pos_del:
-            sequence, w = self.seqrepo_access.get_reference_sequence(
-                t, int(s.start_pos_del), int(s.end_pos_del))
-        else:
-            sequence, w = self.seqrepo_access.get_reference_sequence(
-                t, int(s.start_pos_del))
-        if sequence is None:
-            errors.append(w)
+        return self.get_gene_symbol_tokens(classification)
+
+    def variation_name(self) -> str:
+        """Return the variation name."""
+        return "genomic silent mutation"
+
+    def is_token_instance(self, t: Token) -> bool:
+        """Check that token is Genomic Silent Mutation."""
+        return t.token_type == "GenomicSilentMutation"
+
+    def validates_classification_type(
+            self, classification_type: ClassificationType) -> bool:
+        """Return whether or not the classification type is genomic substitution."""
+        return classification_type == ClassificationType.GENOMIC_SILENT_MUTATION
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/validators/duplication_deletion_base.py` & `variation-normalizer-0.7.dev0/variation/validators/duplication_deletion_base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """The base class for Duplication and Deletion Validation."""
 import logging
 from typing import Optional, List, Dict, Tuple, Union
 
-from ga4gh.vrsatile.pydantic.vrs_models import CopyChange
+from ga4gh.vrsatile.pydantic.vrs_models import RelativeCopyClass
 from ga4gh.vrs import models
 from ga4gh.vrs.extras.translator import Translator
 from gene.query import QueryHandler as GeneQueryHandler
-from cool_seq_tool.data_sources import SeqRepoAccess, TranscriptMappings, UTADatabase, \
+from uta_tools.data_sources import SeqRepoAccess, TranscriptMappings, UTADatabase, \
     MANETranscript
 
 from variation.schemas.classification_response_schema import Classification, \
     ClassificationType
 from variation.schemas.app_schemas import Endpoint
 from variation.schemas.token_response_schema import Token, GeneMatchToken
 from variation.validators.validator import Validator
@@ -101,35 +101,34 @@
     async def get_valid_invalid_results(
         self, classification_tokens: List, transcripts: List,
         classification: Classification, results: List, gene_tokens: List,
         mane_data_found: Dict, is_identifier: bool,
         hgvs_dup_del_mode: HGVSDupDelModeEnum,
         endpoint_name: Optional[Endpoint] = None,
         baseline_copies: Optional[int] = None,
-        copy_change: Optional[CopyChange] = None,
+        relative_copy_class: Optional[RelativeCopyClass] = None,
         do_liftover: bool = False
     ) -> None:
         """Add validation result objects to a list of results.
 
         :param List classification_tokens: A list of classification Tokens
         :param List transcripts: A list of transcript accessions
         :param Classification classification: A classification for a list of
             tokens
         :param List results: Stores validation result objects
         :param List gene_tokens: List of GeneMatchTokens for a classification
         :param Dict mane_data_found: MANE Transcript information found
         :param bool is_identifier: `True` if identifier is given for exact
             location. `False` otherwise.
-        :param HGVSDupDelModeEnum hgvs_dup_del_mode: Must be: `default`,
-            `copy_number_count`, `copy_number_change`, `repeated_seq_expr`,
-            `literal_seq_expr`. This parameter determines how to represent HGVS dup/del
-            expressions as VRS objects.
+        :param HGVSDupDelModeEnum hgvs_dup_del_mode: Must be: `default`, `absolute_cnv`,
+            `relative_cnv`, `repeated_seq_expr`, `literal_seq_expr`. This parameter
+            determines how to represent HGVS dup/del expressions as VRS objects.
         :param Optional[Endpoint] endpoint_name: Then name of the endpoint being used
         :param Optional[int] baseline_copies: Baseline copies number
-        :param Optional[CopyChange] copy_change: The copy change
+        :param Optional[RelativeCopyClass] relative_copy_class: The relative copy class
         :param bool do_liftover: Whether or not to liftover to GRCh38 assembly
         """
         raise NotImplementedError
 
     def get_reference_sequence(
             self, ac: str, start: int, end: int, errors: List,
             cds_start: int = None) -> Optional[str]:
@@ -183,31 +182,30 @@
                     return False
         return True
 
     async def add_normalized_genomic_dup_del(
             self, s: Token, t: str, start: int, end: int, gene: str,
             so_id: str, errors: List, hgvs_dup_del_mode: HGVSDupDelModeEnum,
             mane_data_found: Dict, baseline_copies: Optional[int] = None,
-            copy_change: Optional[CopyChange] = None) -> None:
+            relative_copy_class: Optional[RelativeCopyClass] = None) -> None:
         """Add normalized genomic dup or del to mane data
 
         :param Token s: Classification token
         :param str t: Accession
         :param int start: Start position
         :param int end: ENd position
         :param str gene: Gene
         :param str so_id: Sequence ontology id
         :param List errors: List of errors
-        :param HGVSDupDelModeEnum hgvs_dup_del_mode: Must be: `default`,
-            `copy_number_count`, `copy_number_change`, `repeated_seq_expr`,
-            `literal_seq_expr`. This parameter determines how to represent HGVS dup/del
-            expressions as VRS objects.
+        :param HGVSDupDelModeEnum hgvs_dup_del_mode: Must be: `default`, `absolute_cnv`,
+            `relative_cnv`, `repeated_seq_expr`, `literal_seq_expr`. This parameter
+            determines how to represent HGVS dup/del expressions as VRS objects.
         :param Dict mane_data_found: MANE Transcript information found
         :param Optional[int] baseline_copies: Baseline copies number
-        :param Optional[CopyChange] copy_change: The copy change
+        :param Optional[RelativeCopyClass] relative_copy_class: The relative copy class
         """
         mane = await self.mane_transcript.get_mane_transcript(
             t, start, s.coordinate_type, end_pos=end, gene=gene,
             try_longest_compatible=True)
 
         if mane:
             s.coordinate_type = "c"
@@ -218,15 +216,15 @@
                 mane["refseq"], mane["pos"][0] + 1, mane["pos"][1] + 1,
                 s.coordinate_type, s.alt_type, errors,
                 cds_start=mane["coding_start_site"])
 
             mane_variation = self.hgvs_dup_del_mode.interpret_variation(
                 s.alt_type, allele, errors, hgvs_dup_del_mode,
                 baseline_copies=baseline_copies,
-                copy_change=copy_change)
+                relative_copy_class=relative_copy_class)
 
             if mane_variation:
                 self._add_dict_to_mane_data(mane["refseq"], s, mane_variation,
                                             mane_data_found, mane["status"])
 
     async def validate_gene_or_accession_pos(
         self, t: str, pos_list: List, errors: List, gene: Optional[str] = None
@@ -282,38 +280,37 @@
         self, t: str, s: Token, errors: List,
         grch38: Dict, mane_data_found: Dict,
         hgvs_dup_del_mode: HGVSDupDelModeEnum,
         start: Optional[Union[models.Number, models.DefiniteRange, models.IndefiniteRange]] = None,  # noqa: E501
         end: Optional[Union[models.Number, models.DefiniteRange, models.IndefiniteRange]] = None,  # noqa: E501
         use_vrs_allele_range: bool = True,
         baseline_copies: Optional[int] = None,
-        copy_change: Optional[CopyChange] = None
+        relative_copy_class: Optional[RelativeCopyClass] = None
     ) -> None:
         """Add grch38 variation to mane data
 
         :param str t: Accession
         :param Token s: Classification token
         :param List errors: List of errors
         :param Dict grch38: GRCh38 data
         :param Dict mane_data_found: MANE data found for initial query
-        :param HGVSDupDelModeEnum hgvs_dup_del_mode: Must be: `default`,
-            `copy_number_count`, `copy_number_change`, `repeated_seq_expr`,
-            `literal_seq_expr`. This parameter determines how to represent HGVS dup/del
-            expressions as VRS objects.
+        :param HGVSDupDelModeEnum hgvs_dup_del_mode: Must be: `default`, `absolute_cnv`,
+            `relative_cnv`, `repeated_seq_expr`, `literal_seq_expr`. This parameter
+            determines how to represent HGVS dup/del expressions as VRS objects.
         :param start: start pos
         :type start:
             models.Number or models.DefiniteRange or models.IndefiniteRange or None
         :param end: end pos
         :type end:
             models.Number or models.DefiniteRange or models.IndefiniteRange or None
         :param bool use_vrs_allele_range: `True` if allele should be computed
             using `to_vrs_allele_ranges` method. `False` if allele should be
             computed using `to_vrs_allele` method.
         :param Optional[int] baseline_copies: Baseline copies number
-        :param Optional[CopyChange] copy_change: The copy change
+        :param Optional[RelativeCopyClass] relative_copy_class: The relative copy class
         """
         if errors:
             return
 
         if grch38:
             t = grch38["ac"]
 
@@ -323,12 +320,12 @@
         else:
             allele = self.vrs.to_vrs_allele(
                 t, grch38["pos"][0], grch38["pos"][1], s.coordinate_type,
                 s.alt_type, errors)
 
         grch38_variation = self.hgvs_dup_del_mode.interpret_variation(
             s.alt_type, allele, errors, hgvs_dup_del_mode,
-            baseline_copies=baseline_copies, copy_change=copy_change)
+            baseline_copies=baseline_copies, relative_copy_class=relative_copy_class)
 
         if grch38_variation:
             self._add_dict_to_mane_data(
                 grch38["ac"], s, grch38_variation, mane_data_found, "GRCh38")
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/validators/genomic_base.py` & `variation-normalizer-0.7.dev0/variation/validators/genomic_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """Module for Genomic Validation methods."""
 import logging
 from typing import List, Optional
 
-from cool_seq_tool.data_sources import UTADatabase, SeqRepoAccess
+from uta_tools.data_sources import UTADatabase, SeqRepoAccess
 
 from variation.schemas.classification_response_schema import Classification
 
 
 logger = logging.getLogger("variation")
 logger.setLevel(logging.DEBUG)
 
 
 class GenomicBase:
     """Genomic Base class for validation methods."""
 
     def __init__(self, seqrepo_access: SeqRepoAccess, uta: UTADatabase) -> None:
         """Initialize the Genomic base class.
 
-        :param SeqRepoAccess seqrepo_access: Access to seqrepo
+        :param SeqRepoDataProxy dp: Access to seqrepo data
         :param UTADatabase uta: Access to UTA queries
         """
         self.seqrepo_access = seqrepo_access
         self.uta = uta
 
     """The Genomic Base class."""
     async def get_nc_accessions(self, classification: Classification) -> List[str]:
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/validators/genomic_deletion.py` & `variation-normalizer-0.7.dev0/variation/validators/genomic_deletion.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """The module for Genomic Deletion Validation."""
 import logging
 from typing import List, Optional, Dict
 
-from ga4gh.vrsatile.pydantic.vrs_models import CopyChange
+from ga4gh.vrsatile.pydantic.vrs_models import RelativeCopyClass
 
 from variation.schemas.app_schemas import Endpoint
 from variation.validators.duplication_deletion_base import\
     DuplicationDeletionBase
 from variation.schemas.classification_response_schema import \
     ClassificationType, Classification
 from variation.schemas.token_response_schema import Token, SequenceOntology
@@ -38,35 +38,34 @@
     async def get_valid_invalid_results(
         self, classification_tokens: List, transcripts: List,
         classification: Classification, results: List, gene_tokens: List,
         mane_data_found: Dict, is_identifier: bool,
         hgvs_dup_del_mode: HGVSDupDelModeEnum,
         endpoint_name: Optional[Endpoint] = None,
         baseline_copies: Optional[int] = None,
-        copy_change: Optional[CopyChange] = None,
+        relative_copy_class: Optional[RelativeCopyClass] = None,
         do_liftover: bool = False
     ) -> None:
         """Add validation result objects to a list of results.
 
         :param List classification_tokens: A list of classification Tokens
         :param List transcripts: A list of transcript accessions
         :param Classification classification: A classification for a list of
             tokens
         :param List results: Stores validation result objects
         :param List gene_tokens: List of GeneMatchTokens for a classification
         :param Dict mane_data_found: MANE Transcript information found
         :param bool is_identifier: `True` if identifier is given for exact
             location. `False` otherwise.
-        :param HGVSDupDelModeEnum hgvs_dup_del_mode: Must be: `default`,
-            `copy_number_count`, `copy_number_change`, `repeated_seq_expr`,
-            `literal_seq_expr`. This parameter determines how to represent HGVS dup/del
-            expressions as VRS objects.
+        :param HGVSDupDelModeEnum hgvs_dup_del_mode: Must be: `default`, `absolute_cnv`,
+            `relative_cnv`, `repeated_seq_expr`, `literal_seq_expr`. This parameter
+            determines how to represent HGVS dup/del expressions as VRS objects.
         :param Optional[Endpoint] endpoint_name: Then name of the endpoint being used
         :param Optional[int] baseline_copies: Baseline copies number
-        :param Optional[CopyChange] copy_change: The copy change
+        :param Optional[RelativeCopyClass] relative_copy_class: The relative copy class
         :param bool do_liftover: Whether or not to liftover to GRCh38 assembly
         """
         valid_alleles = list()
         for s in classification_tokens:
             for t in transcripts:
                 errors = list()
                 t = self.get_accession(t, classification)
@@ -86,25 +85,25 @@
                 if not errors:
                     allele = self.vrs.to_vrs_allele(
                         t, s.start_pos_del, s.end_pos_del,
                         s.coordinate_type, s.alt_type, errors)
 
                     variation = self.hgvs_dup_del_mode.interpret_variation(
                         s.alt_type, allele, errors, hgvs_dup_del_mode,
-                        pos=(start, end), copy_change=copy_change,
+                        pos=(start, end), relative_copy_class=relative_copy_class,
                         baseline_copies=baseline_copies
                     )
                 else:
                     variation = None
 
                 if not errors and (endpoint_name == Endpoint.NORMALIZE or do_liftover):
                     await self._get_normalize_variation(
                         gene_tokens, s, t, errors, hgvs_dup_del_mode,
                         mane_data_found, start, end,
-                        copy_change=copy_change,
+                        relative_copy_class=relative_copy_class,
                         baseline_copies=baseline_copies)
 
                 self.add_validation_result(
                     variation, valid_alleles, results,
                     classification, s, t, gene_tokens, errors
                 )
 
@@ -117,48 +116,48 @@
                 classification, gene_tokens
             )
 
     async def _get_normalize_variation(
             self, gene_tokens: List, s: Token, t: str, errors: List,
             hgvs_dup_del_mode: HGVSDupDelModeEnum, mane_data_found: Dict,
             start: int, end: int,
-            copy_change: Optional[CopyChange] = None,
+            relative_copy_class: Optional[RelativeCopyClass] = None,
             baseline_copies: Optional[int] = None) -> None:
         """Get variation that will be returned in normalize endpoint.
 
         :param List gene_tokens: List of gene tokens
         :param Token s: Classification token
         :param str t: Accession
         :param HGVSDupDelModeEnum hgvs_dup_del_mode: Mode to use for
             interpreting HGVS duplications and deletions
         :param Dict mane_data_found: MANE Transcript data found for given query
         :param int start: Start pos change
         :param int end: End pos change
-        :param Optional[CopyChange] copy_change: The copy change
+        :param Optional[RelativeCopyClass] relative_copy_class: The relative copy class
         :param Optional[int] baseline_copies: Baseline copies number
         """
         if gene_tokens:
             await self.add_normalized_genomic_dup_del(
                 s, t, s.start_pos_del, s.end_pos_del, gene_tokens[0].token,
                 SequenceOntology.DELETION, errors, hgvs_dup_del_mode,
-                mane_data_found, copy_change=copy_change,
+                mane_data_found, relative_copy_class=relative_copy_class,
                 baseline_copies=baseline_copies)
         else:
             # No gene provided, then use GRCh38 assembly
             if not self._is_grch38_assembly(t):
                 grch38 = await self.mane_transcript.g_to_grch38(t, start, end)
             else:
                 grch38 = dict(ac=t, pos=(start, end))
 
             if grch38:
                 await self.validate_gene_or_accession_pos(
                     grch38["ac"], [grch38["pos"][0], grch38["pos"][1]], errors)
                 self.add_grch38_to_mane_data(
                     t, s, errors, grch38, mane_data_found, hgvs_dup_del_mode,
-                    use_vrs_allele_range=False, copy_change=copy_change,
+                    use_vrs_allele_range=False, relative_copy_class=relative_copy_class,
                     baseline_copies=baseline_copies)
 
     def get_gene_tokens(
             self, classification: Classification) -> List[GeneMatchToken]:
         """Return gene tokens for a classification.
 
         :param Classification classification: The classification for tokens
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/validators/genomic_deletion_range.py` & `variation-normalizer-0.7.dev0/variation/validators/genomic_deletion_range.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """The module for Genomic Deletion Range Validation."""
 import logging
 from typing import List, Optional, Dict, Tuple, Union
 
-from ga4gh.vrsatile.pydantic.vrs_models import CopyChange
+from ga4gh.vrsatile.pydantic.vrs_models import RelativeCopyClass
 from ga4gh.vrs.extras.translator import Translator
 from ga4gh.vrs import models
 from gene.query import QueryHandler as GeneQueryHandler
-from cool_seq_tool.data_sources import SeqRepoAccess, TranscriptMappings, UTADatabase, \
+from uta_tools.data_sources import SeqRepoAccess, TranscriptMappings, UTADatabase, \
     MANETranscript
 
 from variation.schemas.classification_response_schema import \
     ClassificationType, Classification
 from variation.schemas.app_schemas import Endpoint
 from variation.schemas.token_response_schema import Token
 from variation.schemas.token_response_schema import GeneMatchToken
@@ -70,52 +70,51 @@
     async def get_valid_invalid_results(
         self, classification_tokens: List, transcripts: List,
         classification: Classification, results: List, gene_tokens: List,
         mane_data_found: Dict, is_identifier: bool,
         hgvs_dup_del_mode: HGVSDupDelModeEnum,
         endpoint_name: Optional[Endpoint] = None,
         baseline_copies: Optional[int] = None,
-        copy_change: Optional[CopyChange] = None,
+        relative_copy_class: Optional[RelativeCopyClass] = None,
         do_liftover: bool = False
     ) -> None:
         """Add validation result objects to a list of results.
 
         :param List classification_tokens: A list of classification Tokens
         :param List transcripts: A list of transcript accessions
         :param Classification classification: A classification for a list of
             tokens
         :param List results: Stores validation result objects
         :param List gene_tokens: List of GeneMatchTokens for a classification
         :param Dict mane_data_found: MANE Transcript information found
         :param bool is_identifier: `True` if identifier is given for exact
             location. `False` otherwise.
-        :param HGVSDupDelModeEnum hgvs_dup_del_mode: Must be: `default`,
-            `copy_number_count`, `copy_number_change`, `repeated_seq_expr`,
-            `literal_seq_expr`. This parameter determines how to represent HGVS dup/del
-            expressions as VRS objects.
+        :param HGVSDupDelModeEnum hgvs_dup_del_mode: Must be: `default`, `absolute_cnv`,
+            `relative_cnv`, `repeated_seq_expr`, `literal_seq_expr`. This parameter
+            determines how to represent HGVS dup/del expressions as VRS objects.
         :param Optional[Endpoint] endpoint_name: Then name of the endpoint being used
         :param Optional[int] baseline_copies: Baseline copies number
-        :param Optional[CopyChange] copy_change: The copy change
+        :param Optional[RelativeCopyClass] relative_copy_class: The relative copy class
         :param bool do_liftover: Whether or not to liftover to GRCh38 assembly
         """
         valid_alleles = list()
         for s in classification_tokens:
             for t in transcripts:
                 errors = list()
                 t = self.get_accession(t, classification)
 
                 variation = await self._get_variation(
                     s, t, errors, gene_tokens, hgvs_dup_del_mode,
-                    copy_change=copy_change,
+                    relative_copy_class=relative_copy_class,
                     baseline_copies=baseline_copies)
 
                 if not errors and (endpoint_name == Endpoint.NORMALIZE or do_liftover):
                     await self._get_normalize_variation(
                         gene_tokens, s, t, errors, hgvs_dup_del_mode,
-                        mane_data_found, copy_change=copy_change,
+                        mane_data_found, relative_copy_class=relative_copy_class,
                         baseline_copies=baseline_copies)
 
                 self.add_validation_result(
                     variation, valid_alleles, results,
                     classification, s, t, gene_tokens, errors
                 )
 
@@ -127,25 +126,25 @@
                 mane_data_found, valid_alleles, results,
                 classification, gene_tokens
             )
 
     async def _get_variation(
             self, s: Token, t: str, errors: List, gene_tokens: List,
             hgvs_dup_del_mode: HGVSDupDelModeEnum,
-            copy_change: Optional[CopyChange] = None,
+            relative_copy_class: Optional[RelativeCopyClass] = None,
             baseline_copies: Optional[int] = None) -> Optional[Dict]:
         """Get variation data.
 
         :param Token s: Classification token
         :param str t: Accession
         :param List errors: List of errors
         :param List gene_tokens: List of GeneMatchTokens for a classification
         :param HGVSDupDelMode hgvs_dup_del_mode: Mode to use for interpreting
             HGVS duplications and deletions
-        :param Optional[CopyChange] copy_change: The copy change
+        :param Optional[RelativeCopyClass] relative_copy_class: The relative copy class
         :param Optional[int] baseline_copies: Baseline copies number
         :return: Dictionary containing start/end position changes and variation
         """
         variation, start, end = None, None, None
         ival, grch38 = await self._get_ival(t, s, errors, gene_tokens)
 
         if not errors:
@@ -158,39 +157,39 @@
             if start is not None and end is not None:
                 pos = (start, end)
             else:
                 pos = None
 
             variation = self.hgvs_dup_del_mode.interpret_variation(
                 s.alt_type, allele, errors,
-                hgvs_dup_del_mode, pos=pos, copy_change=copy_change,
+                hgvs_dup_del_mode, pos=pos, relative_copy_class=relative_copy_class,
                 baseline_copies=baseline_copies)
         return variation
 
     async def _get_normalize_variation(
             self, gene_tokens: List, s: Token, t: str, errors: List,
             hgvs_dup_del_mode: HGVSDupDelModeEnum,
             mane_data_found: Dict,
-            copy_change: Optional[CopyChange] = None,
+            relative_copy_class: Optional[RelativeCopyClass] = None,
             baseline_copies: Optional[int] = None) -> None:
         """Get variation that will be returned in normalize endpoint.
 
         :param List gene_tokens: List of gene tokens
         :param Token s: Classification token
         :param str t: Accession
         :param HGVSDupDelModeEnum hgvs_dup_del_mode: Mode to use for
             interpreting HGVS duplications and deletions
         :param Dict mane_data_found: MANE Transcript data found for given query
-        :param Optional[CopyChange] copy_change: The copy change
+        :param Optional[RelativeCopyClass] relative_copy_class: The relative copy class
         :param Optional[int] baseline_copies: Baseline copies number
         """
         ival, grch38 = await self._get_ival(t, s, errors, gene_tokens, is_norm=True)
         self.add_grch38_to_mane_data(
             t, s, errors, grch38, mane_data_found, hgvs_dup_del_mode,
-            start=ival[0], end=ival[1], copy_change=copy_change,
+            start=ival[0], end=ival[1], relative_copy_class=relative_copy_class,
             baseline_copies=baseline_copies)
 
     async def _get_ival(
         self, t: str, s: Token, errors: List, gene_tokens: List, is_norm: bool = False
     ) -> Optional[Tuple[Tuple[Union[models.Number, models.DefiniteRange, models.IndefiniteRange],  # noqa: E501
                               Union[models.Number, models.DefiniteRange, models.IndefiniteRange]],  # noqa: E501
                         Dict]]:
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/validators/genomic_delins.py` & `variation-normalizer-0.7.dev0/variation/validators/genomic_substitution.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,27 @@
-"""The module for Genomic DelIns Validation."""
+"""The module for Genomic Substitution Validation."""
+from typing import Optional, List, Dict
 import logging
-from typing import List, Optional, Dict
 
-from ga4gh.vrsatile.pydantic.vrs_models import CopyChange
+from ga4gh.vrsatile.pydantic.vrs_models import RelativeCopyClass
 
 from variation.schemas.app_schemas import Endpoint
-from variation.validators.delins_base import DelInsBase
 from variation.schemas.classification_response_schema import \
     ClassificationType, Classification
 from variation.schemas.token_response_schema import Token
-from variation.schemas.token_response_schema import GeneMatchToken
 from variation.schemas.normalize_response_schema\
     import HGVSDupDelMode as HGVSDupDelModeEnum
-
+from .single_nucleotide_variation_base import SingleNucleotideVariationBase
 
 logger = logging.getLogger("variation")
 logger.setLevel(logging.DEBUG)
 
 
-class GenomicDelIns(DelInsBase):
-    """The Genomic DelIns Validator class."""
+class GenomicSubstitution(SingleNucleotideVariationBase):
+    """The Genomic Substitution Validator class."""
 
     async def get_transcripts(self, gene_tokens: List, classification: Classification,
                               errors: List) -> Optional[List[str]]:
         """Get transcript accessions for a given classification.
 
         :param List gene_tokens: A list of gene tokens
         :param Classification classification: A classification for a list of
@@ -37,86 +35,90 @@
     async def get_valid_invalid_results(
         self, classification_tokens: List, transcripts: List,
         classification: Classification, results: List, gene_tokens: List,
         mane_data_found: Dict, is_identifier: bool,
         hgvs_dup_del_mode: HGVSDupDelModeEnum,
         endpoint_name: Optional[Endpoint] = None,
         baseline_copies: Optional[int] = None,
-        copy_change: Optional[CopyChange] = None,
+        relative_copy_class: Optional[RelativeCopyClass] = None,
         do_liftover: bool = False
     ) -> None:
         """Add validation result objects to a list of results.
 
         :param List classification_tokens: A list of classification Tokens
         :param List transcripts: A list of transcript accessions
         :param Classification classification: A classification for a list of
             tokens
         :param List results: Stores validation result objects
         :param List gene_tokens: List of GeneMatchTokens for a classification
         :param Dict mane_data_found: MANE Transcript information found
         :param bool is_identifier: `True` if identifier is given for exact
             location. `False` otherwise.
-        :param HGVSDupDelModeEnum hgvs_dup_del_mode: Must be: `default`,
-            `copy_number_count`, `copy_number_change`, `repeated_seq_expr`,
-            `literal_seq_expr`. This parameter determines how to represent HGVS dup/del
-            expressions as VRS objects.
+        :param HGVSDupDelModeEnum hgvs_dup_del_mode: Must be: `default`, `absolute_cnv`,
+            `relative_cnv`, `repeated_seq_expr`, `literal_seq_expr`. This parameter
+            determines how to represent HGVS dup/del expressions as VRS objects.
         :param Optional[Endpoint] endpoint_name: Then name of the endpoint being used
         :param Optional[int] baseline_copies: Baseline copies number
-        :param Optional[CopyChange] copy_change: The copy change
+        :param Optional[RelativeCopyClass] relative_copy_class: The relative copy class
         :param bool do_liftover: Whether or not to liftover to GRCh38 assembly
         """
         valid_alleles = list()
         for s in classification_tokens:
             for t in transcripts:
                 errors = list()
                 t = self.get_accession(t, classification)
                 allele = self.vrs.to_vrs_allele(
-                    t, s.start_pos_del, s.end_pos_del, s.coordinate_type,
-                    s.alt_type, errors, alt=s.inserted_sequence1)
+                    t, s.position, s.position, s.coordinate_type,
+                    s.alt_type, errors, alt=s.new_nucleotide)
 
                 if not errors:
-                    self.check_pos_index(t, s, errors)
-
-                if not errors and endpoint_name == Endpoint.NORMALIZE:
-                    mane = await self.mane_transcript.get_mane_transcript(
-                        t, int(s.start_pos_del), s.coordinate_type,
-                        end_pos=int(s.end_pos_del) if s.end_pos_del else None,
-                        gene=gene_tokens[0].token if gene_tokens else None,
-                        try_longest_compatible=True
-                    )
+                    ref_nuc, _ = self.seqrepo_access.get_reference_sequence(
+                        t, s.position)
+                    self.check_ref_nucleotide(ref_nuc, s.ref_nucleotide,
+                                              s.position, t, errors)
 
-                    self.add_mane_data(mane, mane_data_found, s.coordinate_type,
-                                       s.alt_type, s, alt=s.inserted_sequence1)
+                if not errors:
+                    if endpoint_name == Endpoint.NORMALIZE:
+                        mane = await self.mane_transcript.get_mane_transcript(
+                            t, s.position, s.coordinate_type, end_pos=s.position,
+                            gene=gene_tokens[0].token if gene_tokens else None,
+                            try_longest_compatible=True, residue_mode="residue"
+                        )
+                        self.add_mane_data(mane, mane_data_found, s.coordinate_type,
+                                           s.alt_type, s, alt=s.new_nucleotide)
+                    elif endpoint_name == Endpoint.TO_CANONICAL and do_liftover:
+                        await self._liftover_genomic_data(
+                            gene_tokens, t, s, errors, valid_alleles, results,
+                            classification)
 
                 self.add_validation_result(allele, valid_alleles, results,
                                            classification, s, t, gene_tokens, errors)
 
                 if is_identifier:
                     break
 
         if endpoint_name == Endpoint.NORMALIZE:
             self.add_mane_to_validation_results(mane_data_found, valid_alleles, results,
                                                 classification, gene_tokens)
 
-    def get_gene_tokens(self, classification: Classification) -> List[GeneMatchToken]:
+    def get_gene_tokens(self, classification: Classification) -> List:
         """Return gene tokens for a classification.
 
         :param Classification classification: The classification for tokens
         :return: A list of Gene Match Tokens in the classification
         """
         return self.get_gene_symbol_tokens(classification)
 
     def variation_name(self) -> str:
         """Return the variation name."""
-        return "genomic delins"
+        return "genomic substitution"
 
     def is_token_instance(self, t: Token) -> bool:
-        """Check that token is Genomic DelIns."""
-        return t.token_type == "GenomicDelIns"
+        """Check that token is genomic substitution."""
+        return t.token_type == "GenomicSubstitution"
 
     def validates_classification_type(
-        self, classification_type: ClassificationType
-    ) -> bool:
-        """Return whether or not the classification type is
-        Genomic DelIns.
+            self, classification_type: ClassificationType) -> bool:
+        """Return whether or not the classification type is genomic
+        substitution.
         """
-        return classification_type == ClassificationType.GENOMIC_DELINS
+        return classification_type == ClassificationType.GENOMIC_SUBSTITUTION
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/validators/genomic_duplication.py` & `variation-normalizer-0.7.dev0/variation/validators/genomic_duplication.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """The module for Genomic Duplication Validation."""
 import logging
 from typing import List, Optional, Dict, Tuple, Union
 
 from ga4gh.vrs import models
-from ga4gh.vrsatile.pydantic.vrs_models import CopyChange
+from ga4gh.vrsatile.pydantic.vrs_models import RelativeCopyClass
 
 from variation.schemas.app_schemas import Endpoint
 from variation.validators.duplication_deletion_base import\
     DuplicationDeletionBase
 from variation.schemas.classification_response_schema import \
     ClassificationType, Classification
 from variation.schemas.token_response_schema import \
@@ -39,57 +39,56 @@
     async def get_valid_invalid_results(
         self, classification_tokens: List, transcripts: List,
         classification: Classification, results: List, gene_tokens: List,
         mane_data_found: Dict, is_identifier: bool,
         hgvs_dup_del_mode: HGVSDupDelModeEnum,
         endpoint_name: Optional[Endpoint] = None,
         baseline_copies: Optional[int] = None,
-        copy_change: Optional[CopyChange] = None,
+        relative_copy_class: Optional[RelativeCopyClass] = None,
         do_liftover: bool = False
     ) -> None:
         """Add validation result objects to a list of results.
 
         :param List classification_tokens: A list of classification Tokens
         :param List transcripts: A list of transcript accessions
         :param Classification classification: A classification for a list of
             tokens
         :param List results: Stores validation result objects
         :param List gene_tokens: List of GeneMatchTokens for a classification
         :param Dict mane_data_found: MANE Transcript information found
         :param bool is_identifier: `True` if identifier is given for exact
             location. `False` otherwise.
-        :param HGVSDupDelModeEnum hgvs_dup_del_mode: Must be: `default`,
-            `copy_number_count`, `copy_number_change`, `repeated_seq_expr`,
-            `literal_seq_expr`. This parameter determines how to represent HGVS dup/del
-            expressions as VRS objects.
+        :param HGVSDupDelModeEnum hgvs_dup_del_mode: Must be: `default`, `absolute_cnv`,
+            `relative_cnv`, `repeated_seq_expr`, `literal_seq_expr`. This parameter
+            determines how to represent HGVS dup/del expressions as VRS objects.
         :param Optional[Endpoint] endpoint_name: Then name of the endpoint being used
         :param Optional[int] baseline_copies: Baseline copies number
-        :param Optional[CopyChange] copy_change: The copy change
+        :param Optional[RelativeCopyClass] relative_copy_class: The relative copy class
         :param bool do_liftover: Whether or not to liftover to GRCh38 assembly
         """
         valid_alleles = list()
         for s in classification_tokens:
             for t in transcripts:
                 errors = list()
                 t = self.get_accession(t, classification)
 
                 result = await self._get_variation(
                     s, t, errors, gene_tokens, hgvs_dup_del_mode,
                     gene=gene_tokens[0].token if gene_tokens else None,
                     baseline_copies=baseline_copies,
-                    copy_change=copy_change)
+                    relative_copy_class=relative_copy_class)
                 variation = result["variation"]
                 start = result["start"]
                 end = result["end"]
 
                 if not errors and (endpoint_name == Endpoint.NORMALIZE or do_liftover):
                     await self._get_normalize_variation(
                         gene_tokens, s, t, errors, hgvs_dup_del_mode,
                         mane_data_found, start, end,
-                        copy_change=copy_change,
+                        relative_copy_class=relative_copy_class,
                         baseline_copies=baseline_copies)
 
                 self.add_validation_result(
                     variation, valid_alleles, results,
                     classification, s, t, gene_tokens, errors
                 )
 
@@ -102,15 +101,15 @@
                 classification, gene_tokens
             )
 
     async def _get_variation(
         self, s: Token, t: str, errors: List, gene_tokens: List,
         hgvs_dup_del_mode: HGVSDupDelModeEnum, gene: str = None,
         baseline_copies: Optional[int] = None,
-        copy_change: Optional[CopyChange] = None
+        relative_copy_class: Optional[RelativeCopyClass] = None
     ) -> Optional[Dict]:
         """Get variation data.
 
         :param Token s: Classification token
         :param str t: Accession
         :param List errors: List of errors
         :param HGVSDupDelMode hgvs_dup_del_mode: Mode to use for interpreting
@@ -134,15 +133,15 @@
             if not errors:
                 allele = self.vrs.to_vrs_allele(
                     t, start, end, s.coordinate_type,
                     s.alt_type, errors)
                 variation = self.hgvs_dup_del_mode.interpret_variation(
                     s.alt_type, allele, errors, hgvs_dup_del_mode,
                     pos=(start, end), baseline_copies=baseline_copies,
-                    copy_change=copy_change)
+                    relative_copy_class=relative_copy_class)
         elif s.token_type == TokenType.GENOMIC_DUPLICATION_RANGE:
             ival, grch38 = await self._get_ival(t, s, errors, gene_tokens)
 
             if not errors:
                 if grch38:
                     t = grch38["ac"]
 
@@ -151,78 +150,78 @@
                 if start is not None and end is not None:
                     pos = (start, end)
                 else:
                     pos = None
                 variation = self.hgvs_dup_del_mode.interpret_variation(
                     s.alt_type, allele, errors,
                     hgvs_dup_del_mode, pos=pos, baseline_copies=baseline_copies,
-                    copy_change=copy_change)
+                    relative_copy_class=relative_copy_class)
         else:
             errors.append(f"Token type not supported: {s.token_type}")
 
         return {
             "start": start,
             "end": end,
             "variation": variation
         }
 
     async def _get_normalize_variation(
         self, gene_tokens: List, s: Token, t: str, errors: List,
         hgvs_dup_del_mode: HGVSDupDelModeEnum, mane_data_found: Dict, start: int,
         end: int, baseline_copies: Optional[int] = None,
-        copy_change: Optional[CopyChange] = None
+        relative_copy_class: Optional[RelativeCopyClass] = None
     ) -> None:
         """Get variation that will be returned in normalize endpoint.
 
         :param List gene_tokens: List of gene tokens
         :param Token s: Classification token
         :param str t: Accession
         :param HGVSDupDelModeEnum hgvs_dup_del_mode: Mode to use for
             interpreting HGVS duplications and deletions
         :param Dict mane_data_found: MANE Transcript data found for given query
         :param int start: Start pos change
         :param int end: End pos change
-        :param Optional[CopyChange] copy_change: The copy change
+        :param Optional[RelativeCopyClass] relative_copy_class: The relative copy class
         :param Optional[int] baseline_copies: Baseline copies number
         """
         if s.token_type == TokenType.GENOMIC_DUPLICATION_RANGE:
             # (#_#)_(#_#)
             ival, grch38 = await self._get_ival(t, s, errors, gene_tokens, is_norm=True)
             self.add_grch38_to_mane_data(
                 t, s, errors, grch38, mane_data_found, hgvs_dup_del_mode, start=ival[0],
                 end=ival[1], baseline_copies=baseline_copies,
-                copy_change=copy_change)
+                relative_copy_class=relative_copy_class)
         else:
             # #dup or #_#dup
             if gene_tokens:
                 gene = gene_tokens[0].token
 
                 # Validate position
                 await self._validate_gene_pos(gene, t, start, end, errors)
                 if errors:
                     return
 
                 await self.add_normalized_genomic_dup_del(
                     s, t, start, end, gene_tokens[0].token,
                     SequenceOntology.DUPLICATION, errors, hgvs_dup_del_mode,
                     mane_data_found, baseline_copies=baseline_copies,
-                    copy_change=copy_change)
+                    relative_copy_class=relative_copy_class)
             else:
                 grch38 = await self.mane_transcript.g_to_grch38(
                     t, start, end)
 
                 if grch38:
                     await self.validate_gene_or_accession_pos(
                         grch38["ac"], [grch38["pos"][0], grch38["pos"][1]],
                         errors)
                     self.add_grch38_to_mane_data(
                         t, s, errors, grch38, mane_data_found,
                         hgvs_dup_del_mode, use_vrs_allele_range=False,
                         baseline_copies=baseline_copies,
-                        copy_change=copy_change
+                        relative_copy_class=relative_copy_class
                     )
 
     async def _get_ival(
         self, t: str, s: Token, errors: List, gene_tokens: List, is_norm: bool = False
     ) -> Optional[Tuple[Tuple[Union[models.Number, models.DefiniteRange, models.IndefiniteRange],  # noqa: E501
                               Union[models.Number, models.DefiniteRange, models.IndefiniteRange]],  # noqa: E501
                         Dict]]:
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/validators/genomic_insertion.py` & `variation-normalizer-0.7.dev0/variation/validators/genomic_insertion.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/validators/genomic_silent_mutation.py` & `variation-normalizer-0.7.dev0/variation/validators/genomic_delins.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,29 @@
-"""The module for Genomic Silent Mutation Validation."""
+"""The module for Genomic DelIns Validation."""
 import logging
-from typing import Optional, List, Dict
+from typing import List, Optional, Dict
 
-from ga4gh.vrsatile.pydantic.vrs_models import CopyChange
+from ga4gh.vrsatile.pydantic.vrs_models import RelativeCopyClass
 
 from variation.schemas.app_schemas import Endpoint
-from variation.schemas.classification_response_schema import ClassificationType, \
-    Classification
+from variation.validators.delins_base import DelInsBase
+from variation.schemas.classification_response_schema import \
+    ClassificationType, Classification
 from variation.schemas.token_response_schema import Token
-from variation.schemas.normalize_response_schema import HGVSDupDelMode as HGVSDupDelModeEnum   # noqa: E501
-from .single_nucleotide_variation_base import SingleNucleotideVariationBase
+from variation.schemas.token_response_schema import GeneMatchToken
+from variation.schemas.normalize_response_schema\
+    import HGVSDupDelMode as HGVSDupDelModeEnum
 
 
 logger = logging.getLogger("variation")
 logger.setLevel(logging.DEBUG)
 
 
-class GenomicSilentMutation(SingleNucleotideVariationBase):
-    """The Genomic Silent Mutation Validator class."""
+class GenomicDelIns(DelInsBase):
+    """The Genomic DelIns Validator class."""
 
     async def get_transcripts(self, gene_tokens: List, classification: Classification,
                               errors: List) -> Optional[List[str]]:
         """Get transcript accessions for a given classification.
 
         :param List gene_tokens: A list of gene tokens
         :param Classification classification: A classification for a list of
@@ -35,56 +37,85 @@
     async def get_valid_invalid_results(
         self, classification_tokens: List, transcripts: List,
         classification: Classification, results: List, gene_tokens: List,
         mane_data_found: Dict, is_identifier: bool,
         hgvs_dup_del_mode: HGVSDupDelModeEnum,
         endpoint_name: Optional[Endpoint] = None,
         baseline_copies: Optional[int] = None,
-        copy_change: Optional[CopyChange] = None,
+        relative_copy_class: Optional[RelativeCopyClass] = None,
         do_liftover: bool = False
     ) -> None:
         """Add validation result objects to a list of results.
 
         :param List classification_tokens: A list of classification Tokens
         :param List transcripts: A list of transcript accessions
         :param Classification classification: A classification for a list of
             tokens
         :param List results: Stores validation result objects
         :param List gene_tokens: List of GeneMatchTokens for a classification
         :param Dict mane_data_found: MANE Transcript information found
         :param bool is_identifier: `True` if identifier is given for exact
             location. `False` otherwise.
-        :param HGVSDupDelModeEnum hgvs_dup_del_mode: Must be: `default`,
-            `copy_number_count`, `copy_number_change`, `repeated_seq_expr`,
-            `literal_seq_expr`. This parameter determines how to represent HGVS dup/del
-            expressions as VRS objects.
+        :param HGVSDupDelModeEnum hgvs_dup_del_mode: Must be: `default`, `absolute_cnv`,
+            `relative_cnv`, `repeated_seq_expr`, `literal_seq_expr`. This parameter
+            determines how to represent HGVS dup/del expressions as VRS objects.
         :param Optional[Endpoint] endpoint_name: Then name of the endpoint being used
         :param Optional[int] baseline_copies: Baseline copies number
-        :param Optional[CopyChange] copy_change: The copy change
+        :param Optional[RelativeCopyClass] relative_copy_class: The relative copy class
         :param bool do_liftover: Whether or not to liftover to GRCh38 assembly
         """
-        await self.silent_mutation_valid_invalid_results(
-            classification_tokens, transcripts, classification, results,
-            gene_tokens, endpoint_name, mane_data_found, is_identifier,
-            do_liftover=do_liftover
-        )
+        valid_alleles = list()
+        for s in classification_tokens:
+            for t in transcripts:
+                errors = list()
+                t = self.get_accession(t, classification)
+                allele = self.vrs.to_vrs_allele(
+                    t, s.start_pos_del, s.end_pos_del, s.coordinate_type,
+                    s.alt_type, errors, alt=s.inserted_sequence1)
+
+                if not errors:
+                    self.check_pos_index(t, s, errors)
+
+                if not errors and endpoint_name == Endpoint.NORMALIZE:
+                    mane = await self.mane_transcript.get_mane_transcript(
+                        t, int(s.start_pos_del), s.coordinate_type,
+                        end_pos=int(s.end_pos_del) if s.end_pos_del else None,
+                        gene=gene_tokens[0].token if gene_tokens else None,
+                        try_longest_compatible=True
+                    )
+
+                    self.add_mane_data(mane, mane_data_found, s.coordinate_type,
+                                       s.alt_type, s, alt=s.inserted_sequence1)
+
+                self.add_validation_result(allele, valid_alleles, results,
+                                           classification, s, t, gene_tokens, errors)
+
+                if is_identifier:
+                    break
+
+        if endpoint_name == Endpoint.NORMALIZE:
+            self.add_mane_to_validation_results(mane_data_found, valid_alleles, results,
+                                                classification, gene_tokens)
 
-    def get_gene_tokens(self, classification: Classification) -> List:
+    def get_gene_tokens(self, classification: Classification) -> List[GeneMatchToken]:
         """Return gene tokens for a classification.
 
         :param Classification classification: The classification for tokens
         :return: A list of Gene Match Tokens in the classification
         """
         return self.get_gene_symbol_tokens(classification)
 
     def variation_name(self) -> str:
         """Return the variation name."""
-        return "genomic silent mutation"
+        return "genomic delins"
 
     def is_token_instance(self, t: Token) -> bool:
-        """Check that token is Genomic Silent Mutation."""
-        return t.token_type == "GenomicSilentMutation"
+        """Check that token is Genomic DelIns."""
+        return t.token_type == "GenomicDelIns"
 
     def validates_classification_type(
-            self, classification_type: ClassificationType) -> bool:
-        """Return whether or not the classification type is genomic substitution."""
-        return classification_type == ClassificationType.GENOMIC_SILENT_MUTATION
+        self, classification_type: ClassificationType
+    ) -> bool:
+        """Return whether or not the classification type is
+        Genomic DelIns.
+        """
+        return classification_type == ClassificationType.GENOMIC_DELINS
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/validators/genomic_substitution.py` & `variation-normalizer-0.7.dev0/variation/validators/polypeptide_sequence_variation_base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,125 +1,136 @@
-"""The module for Genomic Substitution Validation."""
-from typing import Optional, List, Dict
+"""The module for Polypeptide Sequence Variation Validation."""
 import logging
+from typing import List, Optional, Dict
 
-from ga4gh.vrsatile.pydantic.vrs_models import CopyChange
+from gene.query import QueryHandler as GeneQueryHandler
+from ga4gh.vrs.extras.translator import Translator
+from ga4gh.vrsatile.pydantic.vrs_models import RelativeCopyClass
+from uta_tools.data_sources import SeqRepoAccess, TranscriptMappings, UTADatabase, \
+    MANETranscript
 
 from variation.schemas.app_schemas import Endpoint
-from variation.schemas.classification_response_schema import \
-    ClassificationType, Classification
-from variation.schemas.token_response_schema import Token
+from variation.schemas.token_response_schema import GeneMatchToken
+from variation.tokenizers import GeneSymbol
+from variation.tokenizers.caches import AminoAcidCache
+from variation.schemas.classification_response_schema import Classification
 from variation.schemas.normalize_response_schema\
     import HGVSDupDelMode as HGVSDupDelModeEnum
-from .single_nucleotide_variation_base import SingleNucleotideVariationBase
+from variation.vrs_representation import VRSRepresentation
+from .validator import Validator
+from .protein_base import ProteinBase
 
 logger = logging.getLogger("variation")
 logger.setLevel(logging.DEBUG)
 
 
-class GenomicSubstitution(SingleNucleotideVariationBase):
-    """The Genomic Substitution Validator class."""
+class PolypeptideSequenceVariationBase(Validator):
+    """The Polypeptide Sequence Variation Validator Base class."""
+
+    def __init__(self, seq_repo_access: SeqRepoAccess,
+                 transcript_mappings: TranscriptMappings,
+                 gene_symbol: GeneSymbol,
+                 mane_transcript: MANETranscript,
+                 uta: UTADatabase, tlr: Translator,
+                 gene_normalizer: GeneQueryHandler, vrs: VRSRepresentation,
+                 amino_acid_cache: AminoAcidCache) -> None:
+        """Initialize the validator.
+
+        :param SeqRepoAccess seq_repo_access: Access to SeqRepo data
+        :param TranscriptMappings transcript_mappings: Access to transcript
+            mappings
+        :param GeneSymbol gene_symbol: Gene symbol tokenizer
+        :param MANETranscript mane_transcript: Access MANE Transcript
+            information
+        :param UTADatabase uta: Access to UTA queries
+        :param Translator tlr: Class for translating nomenclatures to and from VRS
+        :param GeneQueryHandler gene_normalizer: Access to gene-normalizer
+        :param VRSRepresentation vrs: Class for creating VRS objects
+        :param AminoAcidCache amino_acid_cache: Amino Acid codes and conversions
+        """
+        super().__init__(
+            seq_repo_access, transcript_mappings, gene_symbol, mane_transcript,
+            uta, tlr, gene_normalizer, vrs
+        )
+        self._amino_acid_cache = amino_acid_cache
+        self.protein_base = ProteinBase(seq_repo_access, amino_acid_cache)
+        self.mane_transcript = mane_transcript
 
     async def get_transcripts(self, gene_tokens: List, classification: Classification,
                               errors: List) -> Optional[List[str]]:
         """Get transcript accessions for a given classification.
 
         :param List gene_tokens: A list of gene tokens
         :param Classification classification: A classification for a list of
             tokens
         :param List errors: List of errors
         :return: List of transcript accessions
         """
-        transcripts = await self.get_genomic_transcripts(classification, errors)
-        return transcripts
+        return self.get_protein_transcripts(gene_tokens, errors)
 
     async def get_valid_invalid_results(
         self, classification_tokens: List, transcripts: List,
         classification: Classification, results: List, gene_tokens: List,
         mane_data_found: Dict, is_identifier: bool,
         hgvs_dup_del_mode: HGVSDupDelModeEnum,
         endpoint_name: Optional[Endpoint] = None,
         baseline_copies: Optional[int] = None,
-        copy_change: Optional[CopyChange] = None,
+        relative_copy_class: Optional[RelativeCopyClass] = None,
         do_liftover: bool = False
     ) -> None:
         """Add validation result objects to a list of results.
 
         :param List classification_tokens: A list of classification Tokens
         :param List transcripts: A list of transcript accessions
         :param Classification classification: A classification for a list of
             tokens
         :param List results: Stores validation result objects
         :param List gene_tokens: List of GeneMatchTokens for a classification
         :param Dict mane_data_found: MANE Transcript information found
         :param bool is_identifier: `True` if identifier is given for exact
             location. `False` otherwise.
-        :param HGVSDupDelModeEnum hgvs_dup_del_mode: Must be: `default`,
-            `copy_number_count`, `copy_number_change`, `repeated_seq_expr`,
-            `literal_seq_expr`. This parameter determines how to represent HGVS dup/del
-            expressions as VRS objects.
+        :param HGVSDupDelModeEnum hgvs_dup_del_mode: Must be: `default`, `absolute_cnv`,
+            `relative_cnv`, `repeated_seq_expr`, `literal_seq_expr`. This parameter
+            determines how to represent HGVS dup/del expressions as VRS objects.
         :param Optional[Endpoint] endpoint_name: Then name of the endpoint being used
         :param Optional[int] baseline_copies: Baseline copies number
-        :param Optional[CopyChange] copy_change: The copy change
+        :param Optional[RelativeCopyClass] relative_copy_class: The relative copy class
         :param bool do_liftover: Whether or not to liftover to GRCh38 assembly
         """
         valid_alleles = list()
         for s in classification_tokens:
             for t in transcripts:
                 errors = list()
+
                 t = self.get_accession(t, classification)
                 allele = self.vrs.to_vrs_allele(
                     t, s.position, s.position, s.coordinate_type,
-                    s.alt_type, errors, alt=s.new_nucleotide)
+                    s.alt_type, errors, alt=s.alt_protein)
 
                 if not errors:
-                    ref_nuc, _ = self.seqrepo_access.get_reference_sequence(
-                        t, s.position)
-                    self.check_ref_nucleotide(ref_nuc, s.ref_nucleotide,
-                                              s.position, t, errors)
+                    self.protein_base.check_ref_aa(t, s.ref_protein, s.position, errors)
 
-                if not errors:
-                    if endpoint_name == Endpoint.NORMALIZE:
-                        mane = await self.mane_transcript.get_mane_transcript(
-                            t, s.position, s.coordinate_type, end_pos=s.position,
-                            gene=gene_tokens[0].token if gene_tokens else None,
-                            try_longest_compatible=True, residue_mode="residue"
-                        )
-                        self.add_mane_data(mane, mane_data_found, s.coordinate_type,
-                                           s.alt_type, s, alt=s.new_nucleotide)
-                    elif endpoint_name == Endpoint.TO_CANONICAL and do_liftover:
-                        await self._liftover_genomic_data(
-                            gene_tokens, t, s, errors, valid_alleles, results,
-                            classification)
+                if not errors and endpoint_name == Endpoint.NORMALIZE:
+                    mane = await self.mane_transcript.get_mane_transcript(
+                        t, s.position, s.coordinate_type, end_pos=s.position,
+                        ref=s.ref_protein, try_longest_compatible=True
+                    )
+
+                    self.add_mane_data(mane, mane_data_found, s.coordinate_type,
+                                       s.alt_type, s, alt=s.alt_protein)
 
                 self.add_validation_result(allele, valid_alleles, results,
                                            classification, s, t, gene_tokens, errors)
-
                 if is_identifier:
                     break
 
         if endpoint_name == Endpoint.NORMALIZE:
             self.add_mane_to_validation_results(mane_data_found, valid_alleles, results,
                                                 classification, gene_tokens)
 
-    def get_gene_tokens(self, classification: Classification) -> List:
+    def get_gene_tokens(self, classification: Classification) -> List[GeneMatchToken]:
         """Return gene tokens for a classification.
 
         :param Classification classification: The classification for tokens
         :return: A list of Gene Match Tokens in the classification
         """
-        return self.get_gene_symbol_tokens(classification)
-
-    def variation_name(self) -> str:
-        """Return the variation name."""
-        return "genomic substitution"
-
-    def is_token_instance(self, t: Token) -> bool:
-        """Check that token is genomic substitution."""
-        return t.token_type == "GenomicSubstitution"
-
-    def validates_classification_type(
-            self, classification_type: ClassificationType) -> bool:
-        """Return whether or not the classification type is genomic
-        substitution.
-        """
-        return classification_type == ClassificationType.GENOMIC_SUBSTITUTION
+        return self.get_protein_gene_symbol_tokens(classification)
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/validators/genomic_uncertain_deletion.py` & `variation-normalizer-0.7.dev0/variation/validators/genomic_uncertain_deletion.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """The module for Genomic Uncertain Deletion Validation."""
 from typing import List, Optional, Dict, Tuple, Union
 import logging
 
 from ga4gh.vrs import models
-from ga4gh.vrsatile.pydantic.vrs_models import CopyChange
+from ga4gh.vrsatile.pydantic.vrs_models import RelativeCopyClass
 
 from variation.schemas.app_schemas import Endpoint
 from variation.validators.duplication_deletion_base import\
     DuplicationDeletionBase
 from variation.schemas.classification_response_schema import \
     ClassificationType, Classification
 from variation.schemas.token_response_schema import Token
@@ -39,53 +39,52 @@
     async def get_valid_invalid_results(
         self, classification_tokens: List, transcripts: List,
         classification: Classification, results: List, gene_tokens: List,
         mane_data_found: Dict, is_identifier: bool,
         hgvs_dup_del_mode: HGVSDupDelModeEnum,
         endpoint_name: Optional[Endpoint] = None,
         baseline_copies: Optional[int] = None,
-        copy_change: Optional[CopyChange] = None,
+        relative_copy_class: Optional[RelativeCopyClass] = None,
         do_liftover: bool = False
     ) -> None:
         """Add validation result objects to a list of results.
 
         :param List classification_tokens: A list of classification Tokens
         :param List transcripts: A list of transcript accessions
         :param Classification classification: A classification for a list of
             tokens
         :param List results: Stores validation result objects
         :param List gene_tokens: List of GeneMatchTokens for a classification
         :param Dict mane_data_found: MANE Transcript information found
         :param bool is_identifier: `True` if identifier is given for exact
             location. `False` otherwise.
-        :param HGVSDupDelModeEnum hgvs_dup_del_mode: Must be: `default`,
-            `copy_number_count`, `copy_number_change`, `repeated_seq_expr`,
-            `literal_seq_expr`. This parameter determines how to represent HGVS dup/del
-            expressions as VRS objects.
+        :param HGVSDupDelModeEnum hgvs_dup_del_mode: Must be: `default`, `absolute_cnv`,
+            `relative_cnv`, `repeated_seq_expr`, `literal_seq_expr`. This parameter
+            determines how to represent HGVS dup/del expressions as VRS objects.
         :param Optional[Endpoint] endpoint_name: Then name of the endpoint being used
         :param Optional[int] baseline_copies: Baseline copies number
-        :param Optional[CopyChange] copy_change: The copy change
+        :param Optional[RelativeCopyClass] relative_copy_class: The relative copy class
         :param bool do_liftover: Whether or not to liftover to GRCh38 assembly
         """
         valid_alleles = list()
         for s in classification_tokens:
             for t in transcripts:
                 errors = list()
                 t = self.get_accession(t, classification)
 
                 result = await self._get_variation(
                     s, t, errors, gene_tokens, hgvs_dup_del_mode,
-                    copy_change=copy_change,
+                    relative_copy_class=relative_copy_class,
                     baseline_copies=baseline_copies)
                 variation = result["variation"]
 
                 if not errors and (endpoint_name == Endpoint.NORMALIZE or do_liftover):
                     await self._get_normalize_variation(
                         gene_tokens, s, t, errors, hgvs_dup_del_mode,
-                        mane_data_found, copy_change=copy_change,
+                        mane_data_found, relative_copy_class=relative_copy_class,
                         baseline_copies=baseline_copies)
 
                 self.add_validation_result(
                     variation, valid_alleles, results,
                     classification, s, t, gene_tokens, errors
                 )
 
@@ -97,25 +96,25 @@
                 mane_data_found, valid_alleles, results,
                 classification, gene_tokens
             )
 
     async def _get_variation(
         self, s: Token, t: str, errors: List, gene_tokens: List,
         hgvs_dup_del_mode: HGVSDupDelModeEnum,
-        copy_change: Optional[CopyChange] = None,
+        relative_copy_class: Optional[RelativeCopyClass] = None,
         baseline_copies: Optional[int] = None
     ) -> Optional[Dict]:
         """Get variation data.
 
         :param Token s: Classification token
         :param str t: Accession
         :param List errors: List of errors
         :param HGVSDupDelModeEnum hgvs_dup_del_mode: Mode to use for
             interpreting HGVS duplications and deletions
-        :param Optional[CopyChange] copy_change: The copy change
+        :param Optional[RelativeCopyClass] relative_copy_class: The relative copy class
         :param Optional[int] baseline_copies: Baseline copies number
         :return: Dictionary containing start/end position changes and variation
         """
         variation, start, end = None, None, None
         ival, grch38 = await self._get_ival(t, s, errors, gene_tokens)
 
         if not errors:
@@ -126,46 +125,46 @@
                 t, s.coordinate_type, s.alt_type, errors, ival[0], ival[1])
             if start is not None and end is not None:
                 pos = (start, end)
             else:
                 pos = None
             variation = self.hgvs_dup_del_mode.interpret_variation(
                 s.alt_type, allele, errors,
-                hgvs_dup_del_mode, pos=pos, copy_change=copy_change,
+                hgvs_dup_del_mode, pos=pos, relative_copy_class=relative_copy_class,
                 baseline_copies=baseline_copies)
 
         return {
             "start": start,
             "end": end,
             "variation": variation
         }
 
     async def _get_normalize_variation(
             self, gene_tokens: List, s: Token, t: str, errors: List,
             hgvs_dup_del_mode: HGVSDupDelModeEnum,
             mane_data_found: Dict,
-            copy_change: Optional[CopyChange] = None,
+            relative_copy_class: Optional[RelativeCopyClass] = None,
             baseline_copies: Optional[int] = None) -> None:
         """Get variation that will be returned in normalize endpoint.
 
         :param List gene_tokens: List of gene tokens
         :param Token s: Classification token
         :param str t: Accession
         :param HGVSDupDelModeEnum hgvs_dup_del_mode: Mode to use for
             interpreting HGVS duplications and deletions
         :param Dict mane_data_found: MANE Transcript data found for given query
-        :param Optional[CopyChange] copy_change: The copy change
+        :param Optional[RelativeCopyClass] relative_copy_class: The relative copy class
         :param Optional[int] baseline_copies: Baseline copies number
         """
         if not gene_tokens:
             ival, grch38 = await self._get_ival(
                 t, s, errors, gene_tokens, is_norm=True)
             self.add_grch38_to_mane_data(
                 t, s, errors, grch38, mane_data_found, hgvs_dup_del_mode,
-                start=ival[0], end=ival[1], copy_change=copy_change,
+                start=ival[0], end=ival[1], relative_copy_class=relative_copy_class,
                 baseline_copies=baseline_copies)
 
     async def _get_ival(
         self, t: str, s: Token, errors: List, gene_tokens: List, is_norm: bool = False
     ) -> Optional[Tuple[Tuple[Union[models.Number, models.DefiniteRange, models.IndefiniteRange],  # noqa: E501
                               Union[models.Number, models.DefiniteRange, models.IndefiniteRange]],  # noqa: E501
                         Dict]]:
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/validators/insertion_base.py` & `variation-normalizer-0.7.dev0/variation/validators/insertion_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """The module for Insertion Validation."""
 from typing import List, Dict, Optional
 import logging
 
-from ga4gh.vrsatile.pydantic.vrs_models import CopyChange
+from ga4gh.vrsatile.pydantic.vrs_models import RelativeCopyClass
 
 from variation.schemas.classification_response_schema import Classification
 from variation.schemas.app_schemas import Endpoint
 from variation.schemas.token_response_schema import Token
 from variation.validators.validator import Validator
 from variation.schemas.normalize_response_schema\
     import HGVSDupDelMode as HGVSDupDelModeEnum
@@ -21,35 +21,34 @@
     async def get_valid_invalid_results(
         self, classification_tokens: List, transcripts: List,
         classification: Classification, results: List, gene_tokens: List,
         mane_data_found: Dict, is_identifier: bool,
         hgvs_dup_del_mode: HGVSDupDelModeEnum,
         endpoint_name: Optional[Endpoint] = None,
         baseline_copies: Optional[int] = None,
-        copy_change: Optional[CopyChange] = None,
+        relative_copy_class: Optional[RelativeCopyClass] = None,
         do_liftover: bool = False
     ) -> None:
         """Add validation result objects to a list of results.
 
         :param List classification_tokens: A list of classification Tokens
         :param List transcripts: A list of transcript accessions
         :param Classification classification: A classification for a list of
             tokens
         :param List results: Stores validation result objects
         :param List gene_tokens: List of GeneMatchTokens for a classification
         :param Dict mane_data_found: MANE Transcript information found
         :param bool is_identifier: `True` if identifier is given for exact
             location. `False` otherwise.
-        :param HGVSDupDelModeEnum hgvs_dup_del_mode: Must be: `default`,
-            `copy_number_count`, `copy_number_change`, `repeated_seq_expr`,
-            `literal_seq_expr`. This parameter determines how to represent HGVS dup/del
-            expressions as VRS objects.
+        :param HGVSDupDelModeEnum hgvs_dup_del_mode: Must be: `default`, `absolute_cnv`,
+            `relative_cnv`, `repeated_seq_expr`, `literal_seq_expr`. This parameter
+            determines how to represent HGVS dup/del expressions as VRS objects.
         :param Optional[Endpoint] endpoint_name: Then name of the endpoint being used
         :param Optional[int] baseline_copies: Baseline copies number
-        :param Optional[CopyChange] copy_change: The copy change
+        :param Optional[RelativeCopyClass] relative_copy_class: The relative copy class
         :param bool do_liftover: Whether or not to liftover to GRCh38 assembly
         """
         valid_alleles = list()
         for s in classification_tokens:
             for t in transcripts:
                 errors = list()
                 t = self.get_accession(t, classification)
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/validators/polypeptide_sequence_variation_base.py` & `variation-normalizer-0.7.dev0/variation/validators/protein_deletion.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,58 +1,65 @@
-"""The module for Polypeptide Sequence Variation Validation."""
+"""The module for Protein Deletion Validation."""
 import logging
-from typing import List, Optional, Dict
+from typing import Dict, List, Optional
 
+from ga4gh.vrsatile.pydantic.vrs_models import RelativeCopyClass
 from gene.query import QueryHandler as GeneQueryHandler
 from ga4gh.vrs.extras.translator import Translator
-from ga4gh.vrsatile.pydantic.vrs_models import CopyChange
-from cool_seq_tool.data_sources import SeqRepoAccess, TranscriptMappings, UTADatabase, \
+from uta_tools.data_sources import SeqRepoAccess, TranscriptMappings, UTADatabase, \
     MANETranscript
 
+from variation.schemas.classification_response_schema import \
+    Classification, ClassificationType
+from variation.schemas.normalize_response_schema\
+    import HGVSDupDelMode as HGVSDupDelModeEnum
 from variation.schemas.app_schemas import Endpoint
+from variation.schemas.token_response_schema import Token
+from variation.validators.validator import Validator
 from variation.schemas.token_response_schema import GeneMatchToken
 from variation.tokenizers import GeneSymbol
-from variation.schemas.classification_response_schema import Classification
-from variation.schemas.normalize_response_schema\
-    import HGVSDupDelMode as HGVSDupDelModeEnum
+from variation.tokenizers.caches import AminoAcidCache
 from variation.vrs_representation import VRSRepresentation
-from .validator import Validator
 from .protein_base import ProteinBase
 
 logger = logging.getLogger("variation")
 logger.setLevel(logging.DEBUG)
 
 
-class PolypeptideSequenceVariationBase(Validator):
-    """The Polypeptide Sequence Variation Validator Base class."""
+class ProteinDeletion(Validator):
+    """The Protein Deletion Validator class."""
 
     def __init__(self, seq_repo_access: SeqRepoAccess,
                  transcript_mappings: TranscriptMappings,
                  gene_symbol: GeneSymbol,
                  mane_transcript: MANETranscript,
                  uta: UTADatabase, tlr: Translator,
-                 gene_normalizer: GeneQueryHandler, vrs: VRSRepresentation) -> None:
+                 gene_normalizer: GeneQueryHandler, vrs: VRSRepresentation,
+                 amino_acid_cache: AminoAcidCache) \
+            -> None:
         """Initialize the validator.
 
         :param SeqRepoAccess seq_repo_access: Access to SeqRepo data
         :param TranscriptMappings transcript_mappings: Access to transcript
             mappings
         :param GeneSymbol gene_symbol: Gene symbol tokenizer
         :param MANETranscript mane_transcript: Access MANE Transcript
             information
         :param UTADatabase uta: Access to UTA queries
         :param Translator tlr: Class for translating nomenclatures to and from VRS
         :param GeneQueryHandler gene_normalizer: Access to gene-normalizer
         :param VRSRepresentation vrs: Class for creating VRS objects
+        :param AminoAcidCache amino_acid_cache: Amino Acid codes and conversions
         """
         super().__init__(
             seq_repo_access, transcript_mappings, gene_symbol, mane_transcript,
             uta, tlr, gene_normalizer, vrs
         )
-        self.protein_base = ProteinBase(seq_repo_access)
+        self._amino_acid_cache = amino_acid_cache
+        self.protein_base = ProteinBase(seq_repo_access, amino_acid_cache)
         self.mane_transcript = mane_transcript
 
     async def get_transcripts(self, gene_tokens: List, classification: Classification,
                               errors: List) -> Optional[List[str]]:
         """Get transcript accessions for a given classification.
 
         :param List gene_tokens: A list of gene tokens
@@ -66,68 +73,88 @@
     async def get_valid_invalid_results(
         self, classification_tokens: List, transcripts: List,
         classification: Classification, results: List, gene_tokens: List,
         mane_data_found: Dict, is_identifier: bool,
         hgvs_dup_del_mode: HGVSDupDelModeEnum,
         endpoint_name: Optional[Endpoint] = None,
         baseline_copies: Optional[int] = None,
-        copy_change: Optional[CopyChange] = None,
+        relative_copy_class: Optional[RelativeCopyClass] = None,
         do_liftover: bool = False
     ) -> None:
         """Add validation result objects to a list of results.
 
         :param List classification_tokens: A list of classification Tokens
         :param List transcripts: A list of transcript accessions
         :param Classification classification: A classification for a list of
             tokens
         :param List results: Stores validation result objects
         :param List gene_tokens: List of GeneMatchTokens for a classification
         :param Dict mane_data_found: MANE Transcript information found
         :param bool is_identifier: `True` if identifier is given for exact
             location. `False` otherwise.
-        :param HGVSDupDelModeEnum hgvs_dup_del_mode: Must be: `default`,
-            `copy_number_count`, `copy_number_change`, `repeated_seq_expr`,
-            `literal_seq_expr`. This parameter determines how to represent HGVS dup/del
-            expressions as VRS objects.
+        :param HGVSDupDelModeEnum hgvs_dup_del_mode: Must be: `default`, `absolute_cnv`,
+            `relative_cnv`, `repeated_seq_expr`, `literal_seq_expr`. This parameter
+            determines how to represent HGVS dup/del expressions as VRS objects.
         :param Optional[Endpoint] endpoint_name: Then name of the endpoint being used
         :param Optional[int] baseline_copies: Baseline copies number
-        :param Optional[CopyChange] copy_change: The copy change
+        :param Optional[RelativeCopyClass] relative_copy_class: The relative copy class
         :param bool do_liftover: Whether or not to liftover to GRCh38 assembly
         """
         valid_alleles = list()
         for s in classification_tokens:
             for t in transcripts:
                 errors = list()
-
                 t = self.get_accession(t, classification)
                 allele = self.vrs.to_vrs_allele(
-                    t, s.position, s.position, s.coordinate_type,
-                    s.alt_type, errors, alt=s.alt_protein)
+                    t, s.start_pos_del, s.end_pos_del, s.coordinate_type,
+                    s.alt_type, errors)
 
                 if not errors:
-                    self.protein_base.check_ref_aa(t, s.ref_protein, s.position, errors)
+                    # Check ref start/end protein matches expected
+                    self.protein_base.check_ref_aa(
+                        t, s.start_aa_del, s.start_pos_del, errors
+                    )
+
+                    if not errors and s.end_aa_del:
+                        self.protein_base.check_ref_aa(
+                            t, s.end_aa_del, s.end_pos_del, errors
+                        )
 
                 if not errors and endpoint_name == Endpoint.NORMALIZE:
                     mane = await self.mane_transcript.get_mane_transcript(
-                        t, s.position, s.coordinate_type, end_pos=s.position,
-                        ref=s.ref_protein, try_longest_compatible=True
-                    )
-
+                        t, s.start_pos_del, s.coordinate_type, end_pos=s.end_pos_del,
+                        try_longest_compatible=True)
                     self.add_mane_data(mane, mane_data_found, s.coordinate_type,
-                                       s.alt_type, s, alt=s.alt_protein)
+                                       s.alt_type, s)
 
                 self.add_validation_result(allele, valid_alleles, results,
                                            classification, s, t, gene_tokens, errors)
+
                 if is_identifier:
                     break
 
         if endpoint_name == Endpoint.NORMALIZE:
             self.add_mane_to_validation_results(mane_data_found, valid_alleles, results,
                                                 classification, gene_tokens)
 
     def get_gene_tokens(self, classification: Classification) -> List[GeneMatchToken]:
         """Return gene tokens for a classification.
 
         :param Classification classification: The classification for tokens
         :return: A list of Gene Match Tokens in the classification
         """
         return self.get_protein_gene_symbol_tokens(classification)
+
+    def variation_name(self) -> str:
+        """Return the variation name."""
+        return "protein deletion"
+
+    def is_token_instance(self, t: Token) -> bool:
+        """Check that token is Protein DelIns."""
+        return t.token_type == "ProteinDeletion"
+
+    def validates_classification_type(
+            self, classification_type: ClassificationType) -> bool:
+        """Return whether or not the classification type is
+        Protein Deletion.
+        """
+        return classification_type == ClassificationType.PROTEIN_DELETION
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/validators/polypeptide_truncation.py` & `variation-normalizer-0.7.dev0/variation/validators/polypeptide_truncation.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/validators/protein_deletion.py` & `variation-normalizer-0.7.dev0/variation/validators/protein_insertion.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,60 +1,64 @@
-"""The module for Protein Deletion Validation."""
+"""The module for Protein Insertion Validation."""
 import logging
-from typing import Dict, List, Optional
+from typing import List, Optional, Dict
 
-from ga4gh.vrsatile.pydantic.vrs_models import CopyChange
-from gene.query import QueryHandler as GeneQueryHandler
+from ga4gh.vrsatile.pydantic.vrs_models import RelativeCopyClass
 from ga4gh.vrs.extras.translator import Translator
-from cool_seq_tool.data_sources import SeqRepoAccess, TranscriptMappings, UTADatabase, \
+from gene.query import QueryHandler as GeneQueryHandler
+from uta_tools.data_sources import SeqRepoAccess, TranscriptMappings, UTADatabase, \
     MANETranscript
 
 from variation.schemas.classification_response_schema import \
-    Classification, ClassificationType
-from variation.schemas.normalize_response_schema\
-    import HGVSDupDelMode as HGVSDupDelModeEnum
-from variation.schemas.app_schemas import Endpoint
+    ClassificationType, Classification
 from variation.schemas.token_response_schema import Token
+from variation.schemas.app_schemas import Endpoint
 from variation.validators.validator import Validator
 from variation.schemas.token_response_schema import GeneMatchToken
 from variation.tokenizers import GeneSymbol
+from variation.tokenizers.caches import AminoAcidCache
+from variation.schemas.normalize_response_schema\
+    import HGVSDupDelMode as HGVSDupDelModeEnum
 from variation.vrs_representation import VRSRepresentation
 from .protein_base import ProteinBase
 
+
 logger = logging.getLogger("variation")
 logger.setLevel(logging.DEBUG)
 
 
-class ProteinDeletion(Validator):
-    """The Protein Deletion Validator class."""
+class ProteinInsertion(Validator):
+    """The Protein Insertion Validator class."""
 
-    def __init__(self, seq_repo_access: SeqRepoAccess,
-                 transcript_mappings: TranscriptMappings,
-                 gene_symbol: GeneSymbol,
-                 mane_transcript: MANETranscript,
-                 uta: UTADatabase, tlr: Translator,
-                 gene_normalizer: GeneQueryHandler, vrs: VRSRepresentation) -> None:
+    def __init__(
+        self, seq_repo_access: SeqRepoAccess, transcript_mappings: TranscriptMappings,
+        gene_symbol: GeneSymbol, mane_transcript: MANETranscript, uta: UTADatabase,
+        tlr: Translator, gene_normalizer: GeneQueryHandler,
+        vrs: VRSRepresentation, amino_acid_cache: AminoAcidCache
+    ) -> None:
         """Initialize the validator.
 
         :param SeqRepoAccess seq_repo_access: Access to SeqRepo data
         :param TranscriptMappings transcript_mappings: Access to transcript
             mappings
         :param GeneSymbol gene_symbol: Gene symbol tokenizer
         :param MANETranscript mane_transcript: Access MANE Transcript
             information
         :param UTADatabase uta: Access to UTA queries
         :param Translator tlr: Class for translating nomenclatures to and from VRS
         :param GeneQueryHandler gene_normalizer: Access to gene-normalizer
         :param VRSRepresentation vrs: Class for creating VRS objects
+        :param AminoAcidCache amino_acid_cache: Amino Acid codes and conversions
         """
         super().__init__(
             seq_repo_access, transcript_mappings, gene_symbol, mane_transcript,
             uta, tlr, gene_normalizer, vrs
         )
-        self.protein_base = ProteinBase(seq_repo_access)
+        self._amino_acid_cache = amino_acid_cache
+        self.protein_base = ProteinBase(seq_repo_access, amino_acid_cache)
         self.mane_transcript = mane_transcript
 
     async def get_transcripts(self, gene_tokens: List, classification: Classification,
                               errors: List) -> Optional[List[str]]:
         """Get transcript accessions for a given classification.
 
         :param List gene_tokens: A list of gene tokens
@@ -68,76 +72,64 @@
     async def get_valid_invalid_results(
         self, classification_tokens: List, transcripts: List,
         classification: Classification, results: List, gene_tokens: List,
         mane_data_found: Dict, is_identifier: bool,
         hgvs_dup_del_mode: HGVSDupDelModeEnum,
         endpoint_name: Optional[Endpoint] = None,
         baseline_copies: Optional[int] = None,
-        copy_change: Optional[CopyChange] = None,
+        relative_copy_class: Optional[RelativeCopyClass] = None,
         do_liftover: bool = False
     ) -> None:
         """Add validation result objects to a list of results.
 
         :param List classification_tokens: A list of classification Tokens
         :param List transcripts: A list of transcript accessions
         :param Classification classification: A classification for a list of
             tokens
         :param List results: Stores validation result objects
         :param List gene_tokens: List of GeneMatchTokens for a classification
         :param Dict mane_data_found: MANE Transcript information found
         :param bool is_identifier: `True` if identifier is given for exact
             location. `False` otherwise.
-        :param HGVSDupDelModeEnum hgvs_dup_del_mode: Must be: `default`,
-            `copy_number_count`, `copy_number_change`, `repeated_seq_expr`,
-            `literal_seq_expr`. This parameter determines how to represent HGVS dup/del
-            expressions as VRS objects.
+        :param HGVSDupDelModeEnum hgvs_dup_del_mode: Must be: `default`, `absolute_cnv`,
+            `relative_cnv`, `repeated_seq_expr`, `literal_seq_expr`. This parameter
+            determines how to represent HGVS dup/del expressions as VRS objects.
         :param Optional[Endpoint] endpoint_name: Then name of the endpoint being used
         :param Optional[int] baseline_copies: Baseline copies number
-        :param Optional[CopyChange] copy_change: The copy change
+        :param Optional[RelativeCopyClass] relative_copy_class: The relative copy class
         :param bool do_liftover: Whether or not to liftover to GRCh38 assembly
         """
         valid_alleles = list()
         for s in classification_tokens:
             for t in transcripts:
                 errors = list()
                 t = self.get_accession(t, classification)
                 allele = self.vrs.to_vrs_allele(
-                    t, s.start_pos_del, s.end_pos_del, s.coordinate_type,
-                    s.alt_type, errors)
+                    t, s.start_pos_flank, s.end_pos_flank,
+                    s.coordinate_type, s.alt_type, errors,
+                    alt=s.inserted_sequence
+                )
 
                 if not errors:
                     # Check ref start/end protein matches expected
                     self.protein_base.check_ref_aa(
-                        t, s.start_aa_del, s.start_pos_del, errors
+                        t, s.start_aa_flank, s.start_pos_flank, errors
                     )
 
-                    if not errors and s.end_aa_del:
+                    if not errors:
                         self.protein_base.check_ref_aa(
-                            t, s.end_aa_del, s.end_pos_del, errors
+                            t, s.end_aa_flank, s.end_pos_flank, errors
                         )
 
-                    if not errors and s.deleted_aa:
-                        try:
-                            ref = self.seqrepo_access.sr.fetch(
-                                t, s.start_pos_del - 1, s.end_pos_del
-                            )
-                        except (KeyError, ValueError) as e:
-                            errors.append(str(e))
-                        else:
-                            if ref != s.deleted_aa:
-                                errors.append(
-                                    f"Needed to find {s.deleted_aa} but found {ref}"
-                                )
-
                 if not errors and endpoint_name == Endpoint.NORMALIZE:
                     mane = await self.mane_transcript.get_mane_transcript(
-                        t, s.start_pos_del, s.coordinate_type, end_pos=s.end_pos_del,
-                        try_longest_compatible=True)
+                        t, s.start_pos_flank, s.coordinate_type,
+                        end_pos=s.end_pos_flank, try_longest_compatible=True)
                     self.add_mane_data(mane, mane_data_found, s.coordinate_type,
-                                       s.alt_type, s)
+                                       s.alt_type, s, alt=s.inserted_sequence)
 
                 self.add_validation_result(allele, valid_alleles, results,
                                            classification, s, t, gene_tokens, errors)
 
                 if is_identifier:
                     break
 
@@ -151,19 +143,20 @@
         :param Classification classification: The classification for tokens
         :return: A list of Gene Match Tokens in the classification
         """
         return self.get_protein_gene_symbol_tokens(classification)
 
     def variation_name(self) -> str:
         """Return the variation name."""
-        return "protein deletion"
+        return "protein insertion"
 
     def is_token_instance(self, t: Token) -> bool:
-        """Check that token is Protein DelIns."""
-        return t.token_type == "ProteinDeletion"
+        """Check that token is Protein Insertion."""
+        return t.token_type == "ProteinInsertion"
 
     def validates_classification_type(
-            self, classification_type: ClassificationType) -> bool:
+        self, classification_type: ClassificationType
+    ) -> bool:
         """Return whether or not the classification type is
-        Protein Deletion.
+        Protein Insertion.
         """
-        return classification_type == ClassificationType.PROTEIN_DELETION
+        return classification_type == ClassificationType.PROTEIN_INSERTION
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/validators/protein_delins.py` & `variation-normalizer-0.7.dev0/variation/validators/protein_delins.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """The module for Protein DelIns Validation."""
 from typing import List, Optional, Dict
 import logging
 
-from ga4gh.vrsatile.pydantic.vrs_models import CopyChange
+from ga4gh.vrsatile.pydantic.vrs_models import RelativeCopyClass
 from ga4gh.vrs.extras.translator import Translator
 from gene.query import QueryHandler as GeneQueryHandler
-from cool_seq_tool.data_sources import SeqRepoAccess, TranscriptMappings, UTADatabase, \
+from uta_tools.data_sources import SeqRepoAccess, TranscriptMappings, UTADatabase, \
     MANETranscript
 
 from variation.schemas.classification_response_schema import \
     ClassificationType, Classification
 from variation.schemas.app_schemas import Endpoint
 from variation.schemas.token_response_schema import Token
 from variation.validators.validator import Validator
 from variation.schemas.token_response_schema import GeneMatchToken
 from variation.tokenizers import GeneSymbol
+from variation.tokenizers.caches import AminoAcidCache
 from variation.schemas.normalize_response_schema\
     import HGVSDupDelMode as HGVSDupDelModeEnum
 from variation.vrs_representation import VRSRepresentation
 from .protein_base import ProteinBase
 
 logger = logging.getLogger("variation")
 logger.setLevel(logging.DEBUG)
@@ -28,33 +29,37 @@
     """The Protein DelIns Validator class."""
 
     def __init__(self, seq_repo_access: SeqRepoAccess,
                  transcript_mappings: TranscriptMappings,
                  gene_symbol: GeneSymbol,
                  mane_transcript: MANETranscript,
                  uta: UTADatabase, tlr: Translator,
-                 gene_normalizer: GeneQueryHandler, vrs: VRSRepresentation) -> None:
+                 gene_normalizer: GeneQueryHandler, vrs: VRSRepresentation,
+                 amino_acid_cache: AminoAcidCache) \
+            -> None:
         """Initialize the validator.
 
         :param SeqRepoAccess seq_repo_access: Access to SeqRepo data
         :param TranscriptMappings transcript_mappings: Access to transcript
             mappings
         :param GeneSymbol gene_symbol: Gene symbol tokenizer
         :param MANETranscript mane_transcript: Access MANE Transcript
             information
         :param UTADatabase uta: Access to UTA queries
         :param Translator tlr: Class for translating nomenclatures to and from VRS
         :param GeneQueryHandler gene_normalizer: Access to gene-normalizer
         :param VRSRepresentation vrs: Class for creating VRS objects
+        :param AminoAcidCache amino_acid_cache: Amino Acid codes and conversions
         """
         super().__init__(
             seq_repo_access, transcript_mappings, gene_symbol, mane_transcript,
             uta, tlr, gene_normalizer, vrs
         )
-        self.protein_base = ProteinBase(seq_repo_access)
+        self._amino_acid_cache = amino_acid_cache
+        self.protein_base = ProteinBase(seq_repo_access, amino_acid_cache)
         self.mane_transcript = mane_transcript
 
     async def get_transcripts(self, gene_tokens: List, classification: Classification,
                               errors: List) -> Optional[List[str]]:
         """Get transcript accessions for a given classification.
 
         :param List gene_tokens: A list of gene tokens
@@ -68,35 +73,34 @@
     async def get_valid_invalid_results(
         self, classification_tokens: List, transcripts: List,
         classification: Classification, results: List, gene_tokens: List,
         mane_data_found: Dict, is_identifier: bool,
         hgvs_dup_del_mode: HGVSDupDelModeEnum,
         endpoint_name: Optional[Endpoint] = None,
         baseline_copies: Optional[int] = None,
-        copy_change: Optional[CopyChange] = None,
+        relative_copy_class: Optional[RelativeCopyClass] = None,
         do_liftover: bool = False
     ) -> None:
         """Add validation result objects to a list of results.
 
         :param List classification_tokens: A list of classification Tokens
         :param List transcripts: A list of transcript accessions
         :param Classification classification: A classification for a list of
             tokens
         :param List results: Stores validation result objects
         :param List gene_tokens: List of GeneMatchTokens for a classification
         :param Dict mane_data_found: MANE Transcript information found
         :param bool is_identifier: `True` if identifier is given for exact
             location. `False` otherwise.
-        :param HGVSDupDelModeEnum hgvs_dup_del_mode: Must be: `default`,
-            `copy_number_count`, `copy_number_change`, `repeated_seq_expr`,
-            `literal_seq_expr`. This parameter determines how to represent HGVS dup/del
-            expressions as VRS objects.
+        :param HGVSDupDelModeEnum hgvs_dup_del_mode: Must be: `default`, `absolute_cnv`,
+            `relative_cnv`, `repeated_seq_expr`, `literal_seq_expr`. This parameter
+            determines how to represent HGVS dup/del expressions as VRS objects.
         :param Optional[Endpoint] endpoint_name: Then name of the endpoint being used
         :param Optional[int] baseline_copies: Baseline copies number
-        :param Optional[CopyChange] copy_change: The copy change
+        :param Optional[RelativeCopyClass] relative_copy_class: The relative copy class
         :param bool do_liftover: Whether or not to liftover to GRCh38 assembly
         """
         valid_alleles = list()
         for s in classification_tokens:
             for t in transcripts:
                 errors = list()
                 t = self.get_accession(t, classification)
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/validators/protein_substitution.py` & `variation-normalizer-0.7.dev0/variation/validators/protein_substitution.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/validators/silent_mutation.py` & `variation-normalizer-0.7.dev0/variation/validators/silent_mutation.py`

 * *Files identical despite different names*

### Comparing `variation-normalizer-0.7.0.dev7/variation/validators/single_nucleotide_variation_base.py` & `variation-normalizer-0.7.dev0/variation/validators/single_nucleotide_variation_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """The module for Single Nucleotide Variation Validation."""
 from typing import List, Dict, Optional
 import logging
 
-from ga4gh.vrsatile.pydantic.vrs_models import CopyChange
+from ga4gh.vrsatile.pydantic.vrs_models import RelativeCopyClass
 
 from variation.schemas.app_schemas import Endpoint
 from variation.schemas.classification_response_schema import Classification, \
     ClassificationType
 from variation.schemas.token_response_schema import Token, GeneMatchToken
 from variation.schemas.normalize_response_schema\
     import HGVSDupDelMode as HGVSDupDelModeEnum
@@ -69,35 +69,34 @@
     async def get_valid_invalid_results(
         self, classification_tokens: List, transcripts: List,
         classification: Classification, results: List, gene_tokens: List,
         mane_data_found: Dict, is_identifier: bool,
         hgvs_dup_del_mode: HGVSDupDelModeEnum,
         endpoint_name: Optional[Endpoint] = None,
         baseline_copies: Optional[int] = None,
-        copy_change: Optional[CopyChange] = None,
+        relative_copy_class: Optional[RelativeCopyClass] = None,
         do_liftover: bool = False
     ) -> None:
         """Add validation result objects to a list of results.
 
         :param List classification_tokens: A list of classification Tokens
         :param List transcripts: A list of transcript accessions
         :param Classification classification: A classification for a list of
             tokens
         :param List results: Stores validation result objects
         :param List gene_tokens: List of GeneMatchTokens for a classification
         :param Dict mane_data_found: MANE Transcript information found
         :param bool is_identifier: `True` if identifier is given for exact
             location. `False` otherwise.
-        :param HGVSDupDelModeEnum hgvs_dup_del_mode: Must be: `default`,
-            `copy_number_count`, `copy_number_change`, `repeated_seq_expr`,
-            `literal_seq_expr`. This parameter determines how to represent HGVS dup/del
-            expressions as VRS objects.
+        :param HGVSDupDelModeEnum hgvs_dup_del_mode: Must be: `default`, `absolute_cnv`,
+            `relative_cnv`, `repeated_seq_expr`, `literal_seq_expr`. This parameter
+            determines how to represent HGVS dup/del expressions as VRS objects.
         :param Optional[Endpoint] endpoint_name: Then name of the endpoint being used
         :param Optional[int] baseline_copies: Baseline copies number
-        :param Optional[CopyChange] copy_change: The copy change
+        :param Optional[RelativeCopyClass] relative_copy_class: The relative copy class
         :param bool do_liftover: Whether or not to liftover to GRCh38 assembly
         """
         raise NotImplementedError
 
     async def silent_mutation_valid_invalid_results(
             self, classification_tokens: List, transcripts: List,
             classification: Classification, results: List, gene_tokens: List,
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/validators/validate.py` & `variation-normalizer-0.7.dev0/variation/validators/validate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """Module for Validation."""
 from typing import List, Optional
 
-from ga4gh.vrsatile.pydantic.vrs_models import CopyChange
+from ga4gh.vrsatile.pydantic.vrs_models import RelativeCopyClass
 from ga4gh.vrs.extras.translator import Translator
 from gene.query import QueryHandler as GeneQueryHandler
-from cool_seq_tool.data_sources import TranscriptMappings, SeqRepoAccess, UTADatabase, \
+from uta_tools.data_sources import TranscriptMappings, SeqRepoAccess, UTADatabase, \
     MANETranscript
 
 from variation.schemas.normalize_response_schema\
     import HGVSDupDelMode as HGVSDupDelModeEnum
 from variation.vrs_representation import VRSRepresentation
 from variation.schemas.app_schemas import Endpoint
 from variation.schemas.validation_response_schema import ValidationSummary
 from variation.schemas.classification_response_schema import Classification
 from variation.tokenizers import GeneSymbol
+from variation.tokenizers.caches import AminoAcidCache
 from .protein_substitution import ProteinSubstitution
 from .polypeptide_truncation import PolypeptideTruncation
 from .silent_mutation import SilentMutation
 from .coding_dna_substitution import CodingDNASubstitution
 from .coding_dna_silent_mutation import CodingDNASilentMutation
 from .genomic_silent_mutation import GenomicSilentMutation
 from .genomic_substitution import GenomicSubstitution
@@ -40,74 +41,78 @@
     """The validation class."""
 
     def __init__(self, seqrepo_access: SeqRepoAccess,
                  transcript_mappings: TranscriptMappings,
                  gene_symbol: GeneSymbol,
                  mane_transcript: MANETranscript,
                  uta: UTADatabase, tlr: Translator,
+                 amino_acid_cache: AminoAcidCache,
                  gene_normalizer: GeneQueryHandler, vrs: VRSRepresentation) -> None:
         """Initialize the validate class.
 
         :param SeqRepoAccess seqrepo_access: Access to SeqRepo data
         :param TranscriptMappings transcript_mappings: Access to transcript
             mappings
         :param GeneSymbol gene_symbol: Gene symbol tokenizer
         :param MANETranscript mane_transcript: Access MANE Transcript
             information
         :param UTADatabase uta: Access to UTA queries
         :param Translator tlr: Class for translating nomenclatures to and from VRS
+        :param AminoAcidCache amino_acid_cache: Amino Acid codes and conversions
         :param GeneQueryHandler gene_normalizer: Access to gene-normalizer
         :param VRSRepresentation vrs: Class for representing VRS objects
+        :param amino_acid_cache: Amino Acid codes and conversions
         """
         params = [
             seqrepo_access, transcript_mappings, gene_symbol,
             mane_transcript, uta, tlr, gene_normalizer, vrs
         ]
+        protein_params = params[:]
+        protein_params.append(amino_acid_cache)
         self.validators = [
-            ProteinSubstitution(*params),
-            PolypeptideTruncation(*params),
-            SilentMutation(*params),
+            ProteinSubstitution(*protein_params),
+            PolypeptideTruncation(*protein_params),
+            SilentMutation(*protein_params),
             CodingDNASubstitution(*params),
             GenomicSubstitution(*params),
             CodingDNASilentMutation(*params),
             GenomicSilentMutation(*params),
-            ProteinDelIns(*params),
+            ProteinDelIns(*protein_params),
             CodingDNADelIns(*params),
             GenomicDelIns(*params),
-            ProteinDeletion(*params),
+            ProteinDeletion(*protein_params),
             CodingDNADeletion(*params),
             GenomicDeletion(*params),
-            ProteinInsertion(*params),
+            ProteinInsertion(*protein_params),
             CodingDNAInsertion(*params),
             GenomicInsertion(*params),
             GenomicDeletionRange(*params),
             GenomicUncertainDeletion(*params),
             GenomicDuplication(*params),
             Amplification(*params)
         ]
 
     async def perform(
             self, classifications: List[Classification],
             endpoint_name: Optional[Endpoint] = None, warnings: List = None,
             hgvs_dup_del_mode: HGVSDupDelModeEnum = HGVSDupDelModeEnum.DEFAULT,
             baseline_copies: Optional[int] = None,
-            copy_change: Optional[CopyChange] = None,
+            relative_copy_class: Optional[RelativeCopyClass] = None,
             do_liftover: bool = False
     ) -> ValidationSummary:
         """Validate a list of classifications.
 
         :param List classifications: List of classifications
         :param Optional[Endpoint] endpoint_name: Then name of the endpoint being used
         :param List warnings: List of warnings
-        :param HGVSDupDelModeEnum hgvs_dup_del_mode: Must be: `default`,
-            `copy_number_count`, `copy_number_change`, `repeated_seq_expr`,
-            `literal_seq_expr`. This parameter determines how to represent HGVS dup/del
-            expressions as VRS objects.
+        :param HGVSDupDelModeEnum hgvs_dup_del_mode: Must be: `default`, `absolute_cnv`,
+            `relative_cnv`, `repeated_seq_expr`, `literal_seq_expr`. This parameter
+            determines how to represent HGVS dup/del expressions as VRS objects.
         :param Optional[int] baseline_copies: Baseline copies number
-        :param Optional[CopyChange] copy_change: The copy change
+        :param Optional[RelativeCopyClass] relative_copy_class: The relative copy class
         :param bool do_liftover: Whether or not to liftover to GRCh38 assembly
         :return: ValidationSummary containing valid and invalid results
         """
         valid_possibilities = list()
         invalid_possibilities = list()
         if not warnings:
             warnings = list()
@@ -117,15 +122,15 @@
         for classification in classifications:
             for validator in self.validators:
                 if validator.validates_classification_type(
                         classification.classification_type):
                     results = await validator.validate(
                         classification, hgvs_dup_del_mode=hgvs_dup_del_mode,
                         endpoint_name=endpoint_name, baseline_copies=baseline_copies,
-                        copy_change=copy_change,
+                        relative_copy_class=relative_copy_class,
                         do_liftover=do_liftover)
                     for res in results:
                         if res.is_valid:
                             found_valid_result = True
                             valid_possibilities.append(res)
                         else:
                             invalid_possibilities.append(res)
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/validators/validator.py` & `variation-normalizer-0.7.dev0/variation/validators/validator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Module for Validation."""
 import copy
 from typing import List, Optional, Dict, Tuple
 from abc import ABC, abstractmethod
 import logging
 
-from ga4gh.vrsatile.pydantic.vrs_models import CopyChange
+from ga4gh.vrsatile.pydantic.vrs_models import RelativeCopyClass
 from gene.query import QueryHandler as GeneQueryHandler
 from ga4gh.vrs.extras.translator import Translator
-from cool_seq_tool.data_sources import SeqRepoAccess, TranscriptMappings, \
-    MANETranscript, UTADatabase
+from uta_tools.data_sources import SeqRepoAccess, TranscriptMappings, MANETranscript, \
+    UTADatabase
 
 from variation.schemas.classification_response_schema import Classification, \
     ClassificationType
 from variation.schemas.app_schemas import Endpoint
 from variation.schemas.token_response_schema import GeneMatchToken, Token, \
     GenomicSubstitutionToken
 from variation.schemas.validation_response_schema import ValidationResult
@@ -115,58 +115,56 @@
     async def get_valid_invalid_results(
         self, classification_tokens: List, transcripts: List,
         classification: Classification, results: List, gene_tokens: List,
         mane_data_found: Dict, is_identifier: bool,
         hgvs_dup_del_mode: HGVSDupDelModeEnum,
         endpoint_name: Optional[Endpoint] = None,
         baseline_copies: Optional[int] = None,
-        copy_change: Optional[CopyChange] = None,
+        relative_copy_class: Optional[RelativeCopyClass] = None,
         do_liftover: bool = False
     ) -> None:
         """Add validation result objects to a list of results.
 
         :param List classification_tokens: A list of classification Tokens
         :param List transcripts: A list of transcript accessions
         :param Classification classification: A classification for a list of
             tokens
         :param List results: Stores validation result objects
         :param List gene_tokens: List of GeneMatchTokens for a classification
         :param Dict mane_data_found: MANE Transcript information found
         :param bool is_identifier: `True` if identifier is given for exact
             location. `False` otherwise.
-        :param HGVSDupDelModeEnum hgvs_dup_del_mode: Must be: `default`,
-            `copy_number_count`, `copy_number_change`, `repeated_seq_expr`,
-            `literal_seq_expr`. This parameter determines how to represent HGVS dup/del
-            expressions as VRS objects.
+        :param HGVSDupDelModeEnum hgvs_dup_del_mode: Must be: `default`, `absolute_cnv`,
+            `relative_cnv`, `repeated_seq_expr`, `literal_seq_expr`. This parameter
+            determines how to represent HGVS dup/del expressions as VRS objects.
         :param Optional[Endpoint] endpoint_name: Then name of the endpoint being used
         :param Optional[int] baseline_copies: Baseline copies number
-        :param Optional[CopyChange] copy_change: The copy change
+        :param Optional[RelativeCopyClass] relative_copy_class: The relative copy class
         :param bool do_liftover: Whether or not to liftover to GRCh38 assembly
         """
         raise NotImplementedError
 
     async def validate(
             self, classification: Classification,
             hgvs_dup_del_mode: HGVSDupDelModeEnum = HGVSDupDelModeEnum.DEFAULT,
             endpoint_name: Optional[Endpoint] = None,
             baseline_copies: Optional[int] = None,
-            copy_change: Optional[CopyChange] = None,
+            relative_copy_class: Optional[RelativeCopyClass] = None,
             do_liftover: bool = False
     ) -> List[ValidationResult]:
         """Return validation result for a given classification.
 
         :param Classification classification: A classification for a list of
             tokens
-        :param HGVSDupDelModeEnum hgvs_dup_del_mode: Must be: `default`,
-            `copy_number_count`, `copy_number_change`, `repeated_seq_expr`,
-            `literal_seq_expr`. This parameter determines how to represent HGVS dup/del
-            expressions as VRS objects.
+        :param HGVSDupDelModeEnum hgvs_dup_del_mode: Must be: `default`, `absolute_cnv`,
+            `relative_cnv`, `repeated_seq_expr`, `literal_seq_expr`. This parameter
+            determines how to represent HGVS dup/del expressions as VRS objects.
         :param Optional[Endpoint] endpoint_name: Then name of the endpoint being used
         :param Optional[int] baseline_copies: Baseline copies number
-        :param Optional[CopyChange] copy_change: The copy change
+        :param Optional[RelativeCopyClass] relative_copy_class: The relative copy class
         :param bool do_liftover: Whether or not to liftover to GRCh38 assembly
         :return: List of ValidationResult's containing valid and invalid
             results
         """
         results = list()
         errors = list()
 
@@ -207,15 +205,15 @@
         else:
             is_identifier = False
 
         await self.get_valid_invalid_results(
             classification_tokens, transcripts, classification,
             results, gene_tokens, mane_data_found,
             is_identifier, hgvs_dup_del_mode, endpoint_name, baseline_copies,
-            copy_change, do_liftover
+            relative_copy_class, do_liftover
         )
         return results
 
     @staticmethod
     def get_validation_result(
             classification: Classification, classification_token: Token,
             is_valid: bool, confidence_score: int, variation: Dict,
@@ -664,17 +662,17 @@
 
     def _is_grch38_assembly(self, t: str) -> bool:
         """Return whether or not accession is GRCh38 assembly.
 
         :param str t: Accession
         :return: `True` if accession is GRCh38 assembly. `False` otherwise
         """
-        translated_identifiers, _ = self.seqrepo_access.translate_identifier(t)
+        translated_identifiers, w = self.seqrepo_access.translate_identifier(t)
         if translated_identifiers:
-            return bool([a for a in translated_identifiers if a.startswith("GRCh38")])
+            return "GRCh38" in ([a for a in translated_identifiers if a.startswith("GRCh")] or [None])[0]  # noqa: E501
         return False
 
     async def add_genomic_liftover_to_results(
         self, grch38: Dict, errors: List, alt: str, valid_alleles: List, results: List,
         classification: Classification, s: Token, t: str, gene_tokens: List
     ) -> None:
         """Add genomic liftover data to results if genomic GRCh38 variation found
```

### Comparing `variation-normalizer-0.7.0.dev7/variation/vrs_representation.py` & `variation-normalizer-0.7.dev0/variation/vrs_representation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 """Module for generating VRS objects"""
 from typing import List, Optional, Tuple, Union, Dict
 
-from ga4gh.vrsatile.pydantic.vrs_models import CURIE, CopyChange
+from ga4gh.vrsatile.pydantic.vrs_models import CURIE, RelativeCopyClass
+from ga4gh.vrs.dataproxy import SeqRepoDataProxy
 from ga4gh.vrs import models, normalize
 from ga4gh.core import ga4gh_identify
-from cool_seq_tool.data_sources import SeqRepoAccess
+from uta_tools.data_sources import SeqRepoAccess
 from bioutils.accessions import coerce_namespace
 
 
 class VRSRepresentation:
     """Class for representing VRS objects"""
 
-    def __init__(self, seqrepo_access: SeqRepoAccess) -> None:
+    def __init__(self, dp: SeqRepoDataProxy, seqrepo_access: SeqRepoAccess) -> None:
         """Initialize the VRSRepresentation class
 
-        :param SeqRepoAccess seqrepo_access: Access to SeqRepo
+        :param SeqRepoAccess seqrepo_access: Access to SeqRepo via UTA Tools
+        :param SeqRepoDataProxy dp: Access to SeqRepo via VRS Python
         """
         self.seqrepo_access = seqrepo_access
+        self.dp = dp
 
     @staticmethod
     def get_start_end(
             coordinate: str, start: int, end: int, cds_start: int,
             errors: List) -> Optional[Tuple[int, int]]:
         """Get start and end coordinates.
 
@@ -140,15 +143,15 @@
             errors.append(f"Unable to get sequence location: {e}")
             return None
         allele = models.Allele(location=location, state=sstate, type="Allele")
         # Ambiguous regions do not get normalized
         if alt_type not in ["uncertain_deletion", "uncertain_duplication",
                             "duplication_range", "deletion_range"]:
             try:
-                allele = normalize(allele, self.seqrepo_access)
+                allele = normalize(allele, self.dp)
             except (KeyError, AttributeError) as e:
                 errors.append(f"vrs-python unable to normalize allele: {e}")
                 return None
 
         if not allele:
             errors.append("Unable to get allele")
             return None
@@ -253,26 +256,26 @@
             )
         else:
             errors.append("No state")
             return None
 
         return self.vrs_allele(ac, start, end, sstate, alt_type, errors)
 
-    def to_cx_var(
+    def to_rel_cnv(
         self,
         location: Union[models.SequenceLocation, models.ChromosomeLocation, CURIE],
-        copy_change: CopyChange
+        relative_copy_class: RelativeCopyClass
     ) -> Dict:
-        """Return VRS Copy Number Change Variation
+        """Return VRS Relative Copy Number Variation
 
-        :param location: Location for copy number change
+        :param location: Location for relative copy number
         :type location: models.SequenceLocation or models.ChromosomeLocation or CURIE
-        :param CopyChange copy_change: copy change value
-        :return: VRS Copy Number Change Variation represented as a dictionary
+        :param RelativeCopyClass relative_copy_class: Relative copy class value
+        :return: VRS Relative Copy Number Variation represented as a dictionary
         """
         location.id = ga4gh_identify(location)
-        cx = models.CopyNumberChange(
-            subject=location,
-            copy_change=copy_change.value
+        rcn = models.RelativeCopyNumber(
+            location=location,
+            relative_copy_class=relative_copy_class.value
         )
-        cx.id = ga4gh_identify(cx)
-        return cx.as_dict()
+        rcn.id = ga4gh_identify(rcn)
+        return rcn.as_dict()
```

### Comparing `variation-normalizer-0.7.0.dev7/variation_normalizer.egg-info/PKG-INFO` & `variation-normalizer-0.7.dev0/variation_normalizer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: variation-normalizer
-Version: 0.7.0.dev7
+Version: 0.7.dev0
 Summary: VICC normalization routine for variations
 Home-page: https://github.com/cancervariants/variation-normalization
 Author: VICC
 Author-email: help@cancervariants.org
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -48,15 +47,15 @@
 
 We are working towards adding more types of variations, coordinates, and representations.
 
 ### Endpoints
 
 The `/to_vrs` endpoint returns a list of validated VRS [Variations](https://vrs.ga4gh.org/en/1.2.0/terms_and_model.html#variation).
 
-The `/normalize` endpoint returns a [Variation Descriptor](https://vrsatile.readthedocs.io/en/latest/value_object_descriptor/vod_index.html#variation-descriptor) containing the MANE Transcript, if one is found. If a genomic query is not given a gene, `normalize` will return its GRCh38 representation. Variation Normalizer relies on [**C**ommon **O**perations **O**n **L**ots-of **Seq**uences Tool (cool-seq-tool)](https://github.com/GenomicMedLab/cool-seq-tool) for retrieving MANE Transcript data. More information on the transcript selection algorithm can be found [here](https://github.com/GenomicMedLab/cool-seq-tool/blob/main/docs/TranscriptSelectionPriority.md).
+The `/normalize` endpoint returns a [Variation Descriptor](https://vrsatile.readthedocs.io/en/latest/value_object_descriptor/vod_index.html#variation-descriptor) containing the MANE Transcript, if one is found. If a genomic query is not given a gene, `normalize` will return its GRCh38 representation. Variation Normalizer relies on [UTA Tools](https://github.com/GenomicMedLab/uta-tools) for retrieving MANE Transcript data. More information on the transcript selection algorithm can be found [here](https://github.com/GenomicMedLab/uta-tools/blob/main/docs/TranscriptSelectionPriority.md).
 
 ## Developer Instructions
 
 Clone the repo:
 ```
 git clone https://github.com/cancervariants/variation-normalization.git
 cd variation-normalization
@@ -107,18 +106,16 @@
 You will want to do the following:\
 (*Might not be ._fkuefgd, so replace with your error message path*)
 ```console
 sudo mv /usr/local/share/seqrepo/2021-01-29._fkuefgd /usr/local/share/seqrepo/2021-01-29
 exit
 ```
 
-Use the `SEQREPO_ROOT_DIR` environment variable to set the path of an already existing SeqRepo directory. The default is `/usr/local/share/seqrepo/latest`.
-
 #### UTA
-Variation Normalizer also uses [**C**ommon **O**perations **O**n **L**ots-of **Seq**uences Tool (cool-seq-tool)](https://github.com/GenomicMedLab/cool-seq-tool) which uses [UTA](https://github.com/biocommons/uta) as the underlying PostgreSQL database.
+Variation Normalizer also uses [UTA Tools](https://github.com/GenomicMedLab/uta-tools) which uses [UTA](https://github.com/biocommons/uta) as the underlying PostgreSQL database.
 
 _The following commands will likely need modification appropriate for the installation environment._
 1. Install [PostgreSQL](https://www.postgresql.org/)
 2. Create user and database.
 
     ```
     $ createuser -U postgres uta_admin
@@ -172,9 +169,7 @@
 ```
 
 ### Testing
 From the _root_ directory of the repository:
 ```
 pytest tests/
 ```
-
-
```

### Comparing `variation-normalizer-0.7.0.dev7/variation_normalizer.egg-info/SOURCES.txt` & `variation-normalizer-0.7.dev0/variation_normalizer.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,16 @@
 tests/tokenizers/__init__.py
 tests/tokenizers/test_amplification.py
 tests/tokenizers/test_coding_dna_deletion.py
 tests/tokenizers/test_coding_dna_delins.py
 tests/tokenizers/test_coding_dna_insertion.py
 tests/tokenizers/test_coding_dna_silent_mutation.py
 tests/tokenizers/test_coding_dna_substitution.py
-tests/tokenizers/test_gene_symbol.py
+tests/tokenizers/test_gene.py
+tests/tokenizers/test_gene_pair.py
 tests/tokenizers/test_genomic_deletion.py
 tests/tokenizers/test_genomic_deletion_range.py
 tests/tokenizers/test_genomic_delins.py
 tests/tokenizers/test_genomic_duplication.py
 tests/tokenizers/test_genomic_duplication_range.py
 tests/tokenizers/test_genomic_insertion.py
 tests/tokenizers/test_genomic_silent_mutation.py
@@ -132,14 +133,16 @@
 variation/classifiers/protein_classifier.py
 variation/classifiers/protein_deletion_classifier.py
 variation/classifiers/protein_delins_classifier.py
 variation/classifiers/protein_insertion_classifier.py
 variation/classifiers/protein_termination_classifier.py
 variation/classifiers/set_based_classifier.py
 variation/classifiers/silent_mutation.py
+variation/data/amino_acids.csv
+variation/data/transcript_mapping.tsv
 variation/data_sources/__init__.py
 variation/data_sources/codon_table.py
 variation/schemas/__init__.py
 variation/schemas/app_schemas.py
 variation/schemas/classification_response_schema.py
 variation/schemas/hgvs_to_copy_number_schema.py
 variation/schemas/normalize_response_schema.py
@@ -155,14 +158,15 @@
 variation/tokenizers/coding_dna_silent_mutation.py
 variation/tokenizers/coding_dna_substitution.py
 variation/tokenizers/deletion_base.py
 variation/tokenizers/deletion_range_base.py
 variation/tokenizers/delins_base.py
 variation/tokenizers/duplication_base.py
 variation/tokenizers/free_text_categorical.py
+variation/tokenizers/gene_pair.py
 variation/tokenizers/gene_symbol.py
 variation/tokenizers/genomic_deletion.py
 variation/tokenizers/genomic_deletion_range.py
 variation/tokenizers/genomic_delins.py
 variation/tokenizers/genomic_duplication.py
 variation/tokenizers/genomic_insertion.py
 variation/tokenizers/genomic_silent_mutation.py
@@ -170,23 +174,28 @@
 variation/tokenizers/genomic_uncertain_deletion.py
 variation/tokenizers/gnomad_vcf.py
 variation/tokenizers/hgvs.py
 variation/tokenizers/insertion_base.py
 variation/tokenizers/locus_reference_genomic.py
 variation/tokenizers/polypeptide_sequence_variation_base.py
 variation/tokenizers/polypeptide_truncation.py
+variation/tokenizers/protein_alternate.py
 variation/tokenizers/protein_deletion.py
 variation/tokenizers/protein_delins.py
 variation/tokenizers/protein_insertion.py
 variation/tokenizers/protein_substitution.py
 variation/tokenizers/reference_sequence.py
 variation/tokenizers/silent_mutation.py
 variation/tokenizers/single_nucleotide_variation_base.py
 variation/tokenizers/tokenize.py
+variation/tokenizers/tokenize_base.py
 variation/tokenizers/tokenizer.py
+variation/tokenizers/caches/__init__.py
+variation/tokenizers/caches/amino_acid_cache.py
+variation/tokenizers/caches/nucleotide_cache.py
 variation/translators/__init__.py
 variation/translators/amplification.py
 variation/translators/coding_dna_deletion.py
 variation/translators/coding_dna_delins.py
 variation/translators/coding_dna_insertion.py
 variation/translators/coding_dna_silent_mutation.py
 variation/translators/coding_dna_substitution.py
```

