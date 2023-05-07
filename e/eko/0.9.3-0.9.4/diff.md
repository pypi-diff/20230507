# Comparing `tmp/eko-0.9.3.tar.gz` & `tmp/eko-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eko-0.9.3.tar", max compression
+gzip compressed data, was "eko-0.9.4.tar", max compression
```

## Comparing `eko-0.9.3.tar` & `eko-0.9.4.tar`

### file list

```diff
@@ -1,104 +1,104 @@
--rw-r--r--   0        0        0    35149 2022-05-25 15:57:29.274746 eko-0.9.3/LICENSE
--rw-r--r--   0        0        0     3081 2022-05-25 15:57:29.274746 eko-0.9.3/README.md
--rw-r--r--   0        0        0    26695 2022-05-25 15:57:29.438748 eko-0.9.3/doc/source/img/Logo.png
--rw-r--r--   0        0        0     4770 2022-05-25 15:59:00.411952 eko-0.9.3/pyproject.toml
--rw-r--r--   0        0        0      801 2022-05-25 15:57:29.446748 eko-0.9.3/src/eko/__init__.py
--rw-r--r--   0        0        0     5519 2022-05-25 15:57:29.446748 eko-0.9.3/src/eko/anomalous_dimensions/__init__.py
--rw-r--r--   0        0        0     2168 2022-05-25 15:57:29.446748 eko-0.9.3/src/eko/anomalous_dimensions/aem1.py
--rw-r--r--   0        0        0     8511 2022-05-25 15:57:29.446748 eko-0.9.3/src/eko/anomalous_dimensions/aem2.py
--rw-r--r--   0        0        0     3466 2022-05-25 15:57:29.446748 eko-0.9.3/src/eko/anomalous_dimensions/as1.py
--rw-r--r--   0        0        0     8666 2022-05-25 15:57:29.446748 eko-0.9.3/src/eko/anomalous_dimensions/as1aem1.py
--rw-r--r--   0        0        0    11173 2022-05-25 15:57:29.446748 eko-0.9.3/src/eko/anomalous_dimensions/as2.py
--rw-r--r--   0        0        0    15369 2022-05-25 15:57:29.446748 eko-0.9.3/src/eko/anomalous_dimensions/as3.py
--rw-r--r--   0        0        0     5549 2022-05-25 15:57:29.446748 eko-0.9.3/src/eko/basis_rotation.py
--rw-r--r--   0        0        0     3576 2022-05-25 15:57:29.446748 eko-0.9.3/src/eko/beta.py
--rw-r--r--   0        0        0     1338 2022-05-25 15:57:29.446748 eko-0.9.3/src/eko/constants.py
--rw-r--r--   0        0        0    15151 2022-05-25 15:57:29.446748 eko-0.9.3/src/eko/evolution_operator/__init__.py
--rw-r--r--   0        0        0     6806 2022-05-25 15:57:29.446748 eko-0.9.3/src/eko/evolution_operator/flavors.py
--rw-r--r--   0        0        0    10595 2022-05-25 15:57:29.446748 eko-0.9.3/src/eko/evolution_operator/grid.py
--rw-r--r--   0        0        0     4251 2022-05-25 15:57:29.446748 eko-0.9.3/src/eko/evolution_operator/physical.py
--rw-r--r--   0        0        0     2890 2022-05-25 15:57:29.446748 eko-0.9.3/src/eko/gamma.py
--rw-r--r--   0        0        0     5126 2022-05-25 15:57:29.446748 eko-0.9.3/src/eko/harmonics/__init__.py
--rw-r--r--   0        0        0      373 2022-05-25 15:57:29.446748 eko-0.9.3/src/eko/harmonics/constants.py
--rw-r--r--   0        0        0      735 2022-05-25 15:57:29.446748 eko-0.9.3/src/eko/harmonics/f_functions/__init__.py
--rw-r--r--   0        0        0     3492 2022-05-25 15:57:29.446748 eko-0.9.3/src/eko/harmonics/f_functions/f11.py
--rw-r--r--   0        0        0     3982 2022-05-25 15:57:29.446748 eko-0.9.3/src/eko/harmonics/f_functions/f13.py
--rw-r--r--   0        0        0    55653 2022-05-25 15:57:29.446748 eko-0.9.3/src/eko/harmonics/f_functions/f14_f12.py
--rw-r--r--   0        0        0   133423 2022-05-25 15:57:29.446748 eko-0.9.3/src/eko/harmonics/f_functions/f16.py
--rw-r--r--   0        0        0     8657 2022-05-25 15:57:29.446748 eko-0.9.3/src/eko/harmonics/f_functions/f17.py
--rw-r--r--   0        0        0    83813 2022-05-25 15:57:29.446748 eko-0.9.3/src/eko/harmonics/f_functions/f18.py
--rw-r--r--   0        0        0     2413 2022-05-25 15:57:29.446748 eko-0.9.3/src/eko/harmonics/f_functions/f19.py
--rw-r--r--   0        0        0     3298 2022-05-25 15:57:29.446748 eko-0.9.3/src/eko/harmonics/f_functions/f20.py
--rw-r--r--   0        0        0     3307 2022-05-25 15:57:29.446748 eko-0.9.3/src/eko/harmonics/f_functions/f21.py
--rw-r--r--   0        0        0     1763 2022-05-25 15:57:29.446748 eko-0.9.3/src/eko/harmonics/f_functions/f9.py
--rw-r--r--   0        0        0    10045 2022-05-25 15:57:29.446748 eko-0.9.3/src/eko/harmonics/g_functions.py
--rw-r--r--   0        0        0     4675 2022-05-25 15:57:29.446748 eko-0.9.3/src/eko/harmonics/polygamma.py
--rw-r--r--   0        0        0     1692 2022-05-25 15:57:29.446748 eko-0.9.3/src/eko/harmonics/w1.py
--rw-r--r--   0        0        0     1738 2022-05-25 15:57:29.446748 eko-0.9.3/src/eko/harmonics/w2.py
--rw-r--r--   0        0        0     5086 2022-05-25 15:57:29.446748 eko-0.9.3/src/eko/harmonics/w3.py
--rw-r--r--   0        0        0     6520 2022-05-25 15:57:29.446748 eko-0.9.3/src/eko/harmonics/w4.py
--rw-r--r--   0        0        0    10499 2022-05-25 15:57:29.446748 eko-0.9.3/src/eko/harmonics/w5.py
--rw-r--r--   0        0        0    20116 2022-05-25 15:57:29.446748 eko-0.9.3/src/eko/interpolation.py
--rw-r--r--   0        0        0      111 2022-05-25 15:57:29.446748 eko-0.9.3/src/eko/kernels/__init__.py
--rw-r--r--   0        0        0     8532 2022-05-25 15:57:29.446748 eko-0.9.3/src/eko/kernels/evolution_integrals.py
--rw-r--r--   0        0        0     9414 2022-05-25 15:57:29.446748 eko-0.9.3/src/eko/kernels/non_singlet.py
--rw-r--r--   0        0        0    14820 2022-05-25 15:57:29.446748 eko-0.9.3/src/eko/kernels/singlet.py
--rw-r--r--   0        0        0      550 2022-05-25 15:57:29.446748 eko-0.9.3/src/eko/kernels/utils.py
--rw-r--r--   0        0        0     3247 2022-05-25 15:57:29.450748 eko-0.9.3/src/eko/matching_conditions/__init__.py
--rw-r--r--   0        0        0     4664 2022-05-25 15:57:29.450748 eko-0.9.3/src/eko/matching_conditions/as1.py
--rw-r--r--   0        0        0    13204 2022-05-25 15:57:29.450748 eko-0.9.3/src/eko/matching_conditions/as2.py
--rw-r--r--   0        0        0     6703 2022-05-25 15:57:29.450748 eko-0.9.3/src/eko/matching_conditions/as3/__init__.py
--rw-r--r--   0        0        0   125937 2022-05-25 15:57:29.450748 eko-0.9.3/src/eko/matching_conditions/as3/aHg.py
--rw-r--r--   0        0        0    35866 2022-05-25 15:57:29.450748 eko-0.9.3/src/eko/matching_conditions/as3/aHgstfac.py
--rw-r--r--   0        0        0    72823 2022-05-25 15:57:29.450748 eko-0.9.3/src/eko/matching_conditions/as3/aHq.py
--rw-r--r--   0        0        0    54700 2022-05-25 15:57:29.450748 eko-0.9.3/src/eko/matching_conditions/as3/agg.py
--rw-r--r--   0        0        0    10300 2022-05-25 15:57:29.450748 eko-0.9.3/src/eko/matching_conditions/as3/aggTF2.py
--rw-r--r--   0        0        0    33489 2022-05-25 15:57:29.450748 eko-0.9.3/src/eko/matching_conditions/as3/agq.py
--rw-r--r--   0        0        0    21524 2022-05-25 15:57:29.450748 eko-0.9.3/src/eko/matching_conditions/as3/aqg.py
--rw-r--r--   0        0        0    28518 2022-05-25 15:57:29.450748 eko-0.9.3/src/eko/matching_conditions/as3/aqqNS.py
--rw-r--r--   0        0        0     6347 2022-05-25 15:57:29.450748 eko-0.9.3/src/eko/matching_conditions/as3/aqqPS.py
--rw-r--r--   0        0        0    13039 2022-05-25 15:57:29.450748 eko-0.9.3/src/eko/matching_conditions/operator_matrix_element.py
--rw-r--r--   0        0        0     5763 2022-05-25 15:57:29.450748 eko-0.9.3/src/eko/mellin.py
--rw-r--r--   0        0        0     7850 2022-05-25 15:57:29.450748 eko-0.9.3/src/eko/member.py
--rw-r--r--   0        0        0    13771 2022-05-25 15:57:29.450748 eko-0.9.3/src/eko/msbar_masses.py
--rw-r--r--   0        0        0    14823 2022-05-25 15:57:29.450748 eko-0.9.3/src/eko/output.py
--rw-r--r--   0        0        0     3808 2022-05-25 15:57:29.450748 eko-0.9.3/src/eko/runner.py
--rw-r--r--   0        0        0      292 2022-05-25 15:57:29.450748 eko-0.9.3/src/eko/scale_variations/__init__.py
--rw-r--r--   0        0        0     4297 2022-05-25 15:57:29.450748 eko-0.9.3/src/eko/scale_variations/expanded.py
--rw-r--r--   0        0        0     1399 2022-05-25 15:57:29.450748 eko-0.9.3/src/eko/scale_variations/exponentiated.py
--rw-r--r--   0        0        0    17169 2022-05-25 15:57:29.450748 eko-0.9.3/src/eko/strong_coupling.py
--rw-r--r--   0        0        0     8715 2022-05-25 15:57:29.450748 eko-0.9.3/src/eko/thresholds.py
--rw-r--r--   0        0        0       46 2022-05-25 15:59:00.411952 eko-0.9.3/src/eko/version.py
--rw-r--r--   0        0        0      104 2022-05-25 15:57:29.450748 eko-0.9.3/src/ekobox/__init__.py
--rw-r--r--   0        0        0     3601 2022-05-25 15:57:29.450748 eko-0.9.3/src/ekobox/evol_pdf.py
--rw-r--r--   0        0        0     1820 2022-05-25 15:57:29.450748 eko-0.9.3/src/ekobox/gen_info.py
--rw-r--r--   0        0        0     1889 2022-05-25 15:57:29.450748 eko-0.9.3/src/ekobox/gen_op.py
--rw-r--r--   0        0        0     2044 2022-05-25 15:57:29.450748 eko-0.9.3/src/ekobox/gen_theory.py
--rw-r--r--   0        0        0     2209 2022-05-25 15:57:29.450748 eko-0.9.3/src/ekobox/genpdf/Toy.info
--rw-r--r--   0        0        0     7471 2022-05-25 15:57:29.450748 eko-0.9.3/src/ekobox/genpdf/__init__.py
--rw-r--r--   0        0        0      964 2022-05-25 15:57:29.450748 eko-0.9.3/src/ekobox/genpdf/cli.py
--rw-r--r--   0        0        0     3463 2022-05-25 15:57:29.450748 eko-0.9.3/src/ekobox/genpdf/export.py
--rw-r--r--   0        0        0     3177 2022-05-25 15:57:29.450748 eko-0.9.3/src/ekobox/genpdf/flavors.py
--rw-r--r--   0        0        0     2436 2022-05-25 15:57:29.450748 eko-0.9.3/src/ekobox/genpdf/load.py
--rw-r--r--   0        0        0     1428 2022-05-25 15:57:29.450748 eko-0.9.3/src/ekobox/genpdf/templatePDF.info
--rw-r--r--   0        0        0      772 2022-05-25 15:57:29.450748 eko-0.9.3/src/ekobox/mock.py
--rw-r--r--   0        0        0     1928 2022-05-25 15:57:29.450748 eko-0.9.3/src/ekobox/utils.py
--rw-r--r--   0        0        0      298 2022-05-25 15:57:29.450748 eko-0.9.3/src/ekomark/__init__.py
--rw-r--r--   0        0        0     3655 2022-05-25 15:57:29.450748 eko-0.9.3/src/ekomark/apply.py
--rw-r--r--   0        0        0        0 2022-05-25 15:57:29.450748 eko-0.9.3/src/ekomark/benchmark/__init__.py
--rw-r--r--   0        0        0    15861 2022-05-25 15:57:29.454748 eko-0.9.3/src/ekomark/benchmark/external/LHA.yaml
--rw-r--r--   0        0        0     6428 2022-05-25 15:57:29.454748 eko-0.9.3/src/ekomark/benchmark/external/LHA_utils.py
--rw-r--r--   0        0        0        0 2022-05-25 15:57:29.454748 eko-0.9.3/src/ekomark/benchmark/external/__init__.py
--rw-r--r--   0        0        0     3028 2022-05-25 15:57:29.454748 eko-0.9.3/src/ekomark/benchmark/external/apfel_utils.py
--rw-r--r--   0        0        0     1551 2022-05-25 15:57:29.454748 eko-0.9.3/src/ekomark/benchmark/external/lhapdf_utils.py
--rw-r--r--   0        0        0     3171 2022-05-25 15:57:29.454748 eko-0.9.3/src/ekomark/benchmark/external/pegasus_utils.py
--rw-r--r--   0        0        0     6654 2022-05-25 15:57:29.454748 eko-0.9.3/src/ekomark/benchmark/runner.py
--rw-r--r--   0        0        0        0 2022-05-25 15:57:29.454748 eko-0.9.3/src/ekomark/data/__init__.py
--rw-r--r--   0        0        0      636 2022-05-25 15:57:29.454748 eko-0.9.3/src/ekomark/data/db.py
--rw-r--r--   0        0        0     1933 2022-05-25 15:57:29.454748 eko-0.9.3/src/ekomark/data/operators.py
--rw-r--r--   0        0        0     1829 2022-05-25 15:57:29.454748 eko-0.9.3/src/ekomark/navigator/__init__.py
--rw-r--r--   0        0        0       52 2022-05-25 15:57:29.454748 eko-0.9.3/src/ekomark/navigator/glob.py
--rw-r--r--   0        0        0     8874 2022-05-25 15:57:29.454748 eko-0.9.3/src/ekomark/navigator/navigator.py
--rw-r--r--   0        0        0     9371 2022-05-25 15:57:29.454748 eko-0.9.3/src/ekomark/plots.py
--rw-r--r--   0        0        0     4964 2022-05-25 15:59:00.799896 eko-0.9.3/setup.py
--rw-r--r--   0        0        0     4619 2022-05-25 15:59:00.800392 eko-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-06-01 15:00:04.334630 eko-0.9.4/LICENSE
+-rw-r--r--   0        0        0     3081 2022-06-01 15:00:04.334630 eko-0.9.4/README.md
+-rw-r--r--   0        0        0    26695 2022-06-01 15:00:04.518636 eko-0.9.4/doc/source/img/Logo.png
+-rw-r--r--   0        0        0     4770 2022-06-01 15:01:10.453810 eko-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0      801 2022-06-01 15:00:04.526636 eko-0.9.4/src/eko/__init__.py
+-rw-r--r--   0        0        0     5519 2022-06-01 15:00:04.526636 eko-0.9.4/src/eko/anomalous_dimensions/__init__.py
+-rw-r--r--   0        0        0     2168 2022-06-01 15:00:04.526636 eko-0.9.4/src/eko/anomalous_dimensions/aem1.py
+-rw-r--r--   0        0        0     8511 2022-06-01 15:00:04.526636 eko-0.9.4/src/eko/anomalous_dimensions/aem2.py
+-rw-r--r--   0        0        0     3466 2022-06-01 15:00:04.526636 eko-0.9.4/src/eko/anomalous_dimensions/as1.py
+-rw-r--r--   0        0        0     8666 2022-06-01 15:00:04.526636 eko-0.9.4/src/eko/anomalous_dimensions/as1aem1.py
+-rw-r--r--   0        0        0    11173 2022-06-01 15:00:04.526636 eko-0.9.4/src/eko/anomalous_dimensions/as2.py
+-rw-r--r--   0        0        0    15369 2022-06-01 15:00:04.526636 eko-0.9.4/src/eko/anomalous_dimensions/as3.py
+-rw-r--r--   0        0        0     5549 2022-06-01 15:00:04.526636 eko-0.9.4/src/eko/basis_rotation.py
+-rw-r--r--   0        0        0     3576 2022-06-01 15:00:04.526636 eko-0.9.4/src/eko/beta.py
+-rw-r--r--   0        0        0     1338 2022-06-01 15:00:04.526636 eko-0.9.4/src/eko/constants.py
+-rw-r--r--   0        0        0    15151 2022-06-01 15:00:04.526636 eko-0.9.4/src/eko/evolution_operator/__init__.py
+-rw-r--r--   0        0        0     6806 2022-06-01 15:00:04.526636 eko-0.9.4/src/eko/evolution_operator/flavors.py
+-rw-r--r--   0        0        0    10595 2022-06-01 15:00:04.526636 eko-0.9.4/src/eko/evolution_operator/grid.py
+-rw-r--r--   0        0        0     4251 2022-06-01 15:00:04.526636 eko-0.9.4/src/eko/evolution_operator/physical.py
+-rw-r--r--   0        0        0     2890 2022-06-01 15:00:04.526636 eko-0.9.4/src/eko/gamma.py
+-rw-r--r--   0        0        0     5126 2022-06-01 15:00:04.526636 eko-0.9.4/src/eko/harmonics/__init__.py
+-rw-r--r--   0        0        0      373 2022-06-01 15:00:04.526636 eko-0.9.4/src/eko/harmonics/constants.py
+-rw-r--r--   0        0        0      735 2022-06-01 15:00:04.526636 eko-0.9.4/src/eko/harmonics/f_functions/__init__.py
+-rw-r--r--   0        0        0     3492 2022-06-01 15:00:04.526636 eko-0.9.4/src/eko/harmonics/f_functions/f11.py
+-rw-r--r--   0        0        0     3982 2022-06-01 15:00:04.526636 eko-0.9.4/src/eko/harmonics/f_functions/f13.py
+-rw-r--r--   0        0        0    55653 2022-06-01 15:00:04.526636 eko-0.9.4/src/eko/harmonics/f_functions/f14_f12.py
+-rw-r--r--   0        0        0   133423 2022-06-01 15:00:04.526636 eko-0.9.4/src/eko/harmonics/f_functions/f16.py
+-rw-r--r--   0        0        0     8657 2022-06-01 15:00:04.526636 eko-0.9.4/src/eko/harmonics/f_functions/f17.py
+-rw-r--r--   0        0        0    83813 2022-06-01 15:00:04.526636 eko-0.9.4/src/eko/harmonics/f_functions/f18.py
+-rw-r--r--   0        0        0     2413 2022-06-01 15:00:04.526636 eko-0.9.4/src/eko/harmonics/f_functions/f19.py
+-rw-r--r--   0        0        0     3298 2022-06-01 15:00:04.526636 eko-0.9.4/src/eko/harmonics/f_functions/f20.py
+-rw-r--r--   0        0        0     3307 2022-06-01 15:00:04.526636 eko-0.9.4/src/eko/harmonics/f_functions/f21.py
+-rw-r--r--   0        0        0     1763 2022-06-01 15:00:04.526636 eko-0.9.4/src/eko/harmonics/f_functions/f9.py
+-rw-r--r--   0        0        0    10045 2022-06-01 15:00:04.526636 eko-0.9.4/src/eko/harmonics/g_functions.py
+-rw-r--r--   0        0        0     4675 2022-06-01 15:00:04.526636 eko-0.9.4/src/eko/harmonics/polygamma.py
+-rw-r--r--   0        0        0     1692 2022-06-01 15:00:04.526636 eko-0.9.4/src/eko/harmonics/w1.py
+-rw-r--r--   0        0        0     1738 2022-06-01 15:00:04.526636 eko-0.9.4/src/eko/harmonics/w2.py
+-rw-r--r--   0        0        0     5086 2022-06-01 15:00:04.526636 eko-0.9.4/src/eko/harmonics/w3.py
+-rw-r--r--   0        0        0     6520 2022-06-01 15:00:04.526636 eko-0.9.4/src/eko/harmonics/w4.py
+-rw-r--r--   0        0        0    10499 2022-06-01 15:00:04.526636 eko-0.9.4/src/eko/harmonics/w5.py
+-rw-r--r--   0        0        0    20241 2022-06-01 15:00:04.526636 eko-0.9.4/src/eko/interpolation.py
+-rw-r--r--   0        0        0      111 2022-06-01 15:00:04.526636 eko-0.9.4/src/eko/kernels/__init__.py
+-rw-r--r--   0        0        0     8532 2022-06-01 15:00:04.526636 eko-0.9.4/src/eko/kernels/evolution_integrals.py
+-rw-r--r--   0        0        0     9414 2022-06-01 15:00:04.526636 eko-0.9.4/src/eko/kernels/non_singlet.py
+-rw-r--r--   0        0        0    14820 2022-06-01 15:00:04.526636 eko-0.9.4/src/eko/kernels/singlet.py
+-rw-r--r--   0        0        0      550 2022-06-01 15:00:04.526636 eko-0.9.4/src/eko/kernels/utils.py
+-rw-r--r--   0        0        0     3247 2022-06-01 15:00:04.526636 eko-0.9.4/src/eko/matching_conditions/__init__.py
+-rw-r--r--   0        0        0     4664 2022-06-01 15:00:04.526636 eko-0.9.4/src/eko/matching_conditions/as1.py
+-rw-r--r--   0        0        0    13204 2022-06-01 15:00:04.530636 eko-0.9.4/src/eko/matching_conditions/as2.py
+-rw-r--r--   0        0        0     6703 2022-06-01 15:00:04.530636 eko-0.9.4/src/eko/matching_conditions/as3/__init__.py
+-rw-r--r--   0        0        0   125937 2022-06-01 15:00:04.530636 eko-0.9.4/src/eko/matching_conditions/as3/aHg.py
+-rw-r--r--   0        0        0    35866 2022-06-01 15:00:04.530636 eko-0.9.4/src/eko/matching_conditions/as3/aHgstfac.py
+-rw-r--r--   0        0        0    72823 2022-06-01 15:00:04.530636 eko-0.9.4/src/eko/matching_conditions/as3/aHq.py
+-rw-r--r--   0        0        0    54700 2022-06-01 15:00:04.530636 eko-0.9.4/src/eko/matching_conditions/as3/agg.py
+-rw-r--r--   0        0        0    10300 2022-06-01 15:00:04.530636 eko-0.9.4/src/eko/matching_conditions/as3/aggTF2.py
+-rw-r--r--   0        0        0    33489 2022-06-01 15:00:04.530636 eko-0.9.4/src/eko/matching_conditions/as3/agq.py
+-rw-r--r--   0        0        0    21524 2022-06-01 15:00:04.530636 eko-0.9.4/src/eko/matching_conditions/as3/aqg.py
+-rw-r--r--   0        0        0    28518 2022-06-01 15:00:04.530636 eko-0.9.4/src/eko/matching_conditions/as3/aqqNS.py
+-rw-r--r--   0        0        0     6347 2022-06-01 15:00:04.530636 eko-0.9.4/src/eko/matching_conditions/as3/aqqPS.py
+-rw-r--r--   0        0        0    13277 2022-06-01 15:00:04.530636 eko-0.9.4/src/eko/matching_conditions/operator_matrix_element.py
+-rw-r--r--   0        0        0     5763 2022-06-01 15:00:04.530636 eko-0.9.4/src/eko/mellin.py
+-rw-r--r--   0        0        0     7850 2022-06-01 15:00:04.530636 eko-0.9.4/src/eko/member.py
+-rw-r--r--   0        0        0    13771 2022-06-01 15:00:04.530636 eko-0.9.4/src/eko/msbar_masses.py
+-rw-r--r--   0        0        0    14823 2022-06-01 15:00:04.530636 eko-0.9.4/src/eko/output.py
+-rw-r--r--   0        0        0     3808 2022-06-01 15:00:04.530636 eko-0.9.4/src/eko/runner.py
+-rw-r--r--   0        0        0      292 2022-06-01 15:00:04.530636 eko-0.9.4/src/eko/scale_variations/__init__.py
+-rw-r--r--   0        0        0     4297 2022-06-01 15:00:04.530636 eko-0.9.4/src/eko/scale_variations/expanded.py
+-rw-r--r--   0        0        0     1399 2022-06-01 15:00:04.530636 eko-0.9.4/src/eko/scale_variations/exponentiated.py
+-rw-r--r--   0        0        0    17169 2022-06-01 15:00:04.530636 eko-0.9.4/src/eko/strong_coupling.py
+-rw-r--r--   0        0        0     8715 2022-06-01 15:00:04.530636 eko-0.9.4/src/eko/thresholds.py
+-rw-r--r--   0        0        0       46 2022-06-01 15:01:10.453810 eko-0.9.4/src/eko/version.py
+-rw-r--r--   0        0        0      104 2022-06-01 15:00:04.530636 eko-0.9.4/src/ekobox/__init__.py
+-rw-r--r--   0        0        0     3601 2022-06-01 15:00:04.530636 eko-0.9.4/src/ekobox/evol_pdf.py
+-rw-r--r--   0        0        0     1820 2022-06-01 15:00:04.530636 eko-0.9.4/src/ekobox/gen_info.py
+-rw-r--r--   0        0        0     1889 2022-06-01 15:00:04.530636 eko-0.9.4/src/ekobox/gen_op.py
+-rw-r--r--   0        0        0     2044 2022-06-01 15:00:04.530636 eko-0.9.4/src/ekobox/gen_theory.py
+-rw-r--r--   0        0        0     2209 2022-06-01 15:00:04.530636 eko-0.9.4/src/ekobox/genpdf/Toy.info
+-rw-r--r--   0        0        0     7471 2022-06-01 15:00:04.530636 eko-0.9.4/src/ekobox/genpdf/__init__.py
+-rw-r--r--   0        0        0      964 2022-06-01 15:00:04.530636 eko-0.9.4/src/ekobox/genpdf/cli.py
+-rw-r--r--   0        0        0     3463 2022-06-01 15:00:04.530636 eko-0.9.4/src/ekobox/genpdf/export.py
+-rw-r--r--   0        0        0     3177 2022-06-01 15:00:04.530636 eko-0.9.4/src/ekobox/genpdf/flavors.py
+-rw-r--r--   0        0        0     2436 2022-06-01 15:00:04.530636 eko-0.9.4/src/ekobox/genpdf/load.py
+-rw-r--r--   0        0        0     1428 2022-06-01 15:00:04.530636 eko-0.9.4/src/ekobox/genpdf/templatePDF.info
+-rw-r--r--   0        0        0      772 2022-06-01 15:00:04.534637 eko-0.9.4/src/ekobox/mock.py
+-rw-r--r--   0        0        0     1928 2022-06-01 15:00:04.534637 eko-0.9.4/src/ekobox/utils.py
+-rw-r--r--   0        0        0      298 2022-06-01 15:00:04.534637 eko-0.9.4/src/ekomark/__init__.py
+-rw-r--r--   0        0        0     3655 2022-06-01 15:00:04.534637 eko-0.9.4/src/ekomark/apply.py
+-rw-r--r--   0        0        0        0 2022-06-01 15:00:04.534637 eko-0.9.4/src/ekomark/benchmark/__init__.py
+-rw-r--r--   0        0        0    15861 2022-06-01 15:00:04.534637 eko-0.9.4/src/ekomark/benchmark/external/LHA.yaml
+-rw-r--r--   0        0        0     6428 2022-06-01 15:00:04.534637 eko-0.9.4/src/ekomark/benchmark/external/LHA_utils.py
+-rw-r--r--   0        0        0        0 2022-06-01 15:00:04.534637 eko-0.9.4/src/ekomark/benchmark/external/__init__.py
+-rw-r--r--   0        0        0     3028 2022-06-01 15:00:04.534637 eko-0.9.4/src/ekomark/benchmark/external/apfel_utils.py
+-rw-r--r--   0        0        0     1551 2022-06-01 15:00:04.534637 eko-0.9.4/src/ekomark/benchmark/external/lhapdf_utils.py
+-rw-r--r--   0        0        0     3171 2022-06-01 15:00:04.534637 eko-0.9.4/src/ekomark/benchmark/external/pegasus_utils.py
+-rw-r--r--   0        0        0     6654 2022-06-01 15:00:04.534637 eko-0.9.4/src/ekomark/benchmark/runner.py
+-rw-r--r--   0        0        0        0 2022-06-01 15:00:04.534637 eko-0.9.4/src/ekomark/data/__init__.py
+-rw-r--r--   0        0        0      636 2022-06-01 15:00:04.534637 eko-0.9.4/src/ekomark/data/db.py
+-rw-r--r--   0        0        0     1933 2022-06-01 15:00:04.534637 eko-0.9.4/src/ekomark/data/operators.py
+-rw-r--r--   0        0        0     1829 2022-06-01 15:00:04.534637 eko-0.9.4/src/ekomark/navigator/__init__.py
+-rw-r--r--   0        0        0       52 2022-06-01 15:00:04.534637 eko-0.9.4/src/ekomark/navigator/glob.py
+-rw-r--r--   0        0        0     8874 2022-06-01 15:00:04.534637 eko-0.9.4/src/ekomark/navigator/navigator.py
+-rw-r--r--   0        0        0     9371 2022-06-01 15:00:04.534637 eko-0.9.4/src/ekomark/plots.py
+-rw-r--r--   0        0        0     4964 2022-06-01 15:01:10.867905 eko-0.9.4/setup.py
+-rw-r--r--   0        0        0     4619 2022-06-01 15:01:10.868449 eko-0.9.4/PKG-INFO
```

### Comparing `eko-0.9.3/LICENSE` & `eko-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/README.md` & `eko-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/doc/source/img/Logo.png` & `eko-0.9.4/doc/source/img/Logo.png`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/pyproject.toml` & `eko-0.9.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "eko"
-version = "0.9.3"
+version = "0.9.4"
 description = "Evolution Kernel Operator"
 readme = "README.md"
 authors = [
   "A. Candido <alessandro.candido@mi.infn.it>",
   "F. Hekhorn <felix.hekhorn@mi.infn.it>",
   "G. Magni <gmagni@nikhef.nl>",
 ]
```

### Comparing `eko-0.9.3/src/eko/__init__.py` & `eko-0.9.4/src/eko/__init__.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/anomalous_dimensions/__init__.py` & `eko-0.9.4/src/eko/anomalous_dimensions/__init__.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/anomalous_dimensions/aem1.py` & `eko-0.9.4/src/eko/anomalous_dimensions/aem1.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/anomalous_dimensions/aem2.py` & `eko-0.9.4/src/eko/anomalous_dimensions/aem2.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/anomalous_dimensions/as1.py` & `eko-0.9.4/src/eko/anomalous_dimensions/as1.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/anomalous_dimensions/as1aem1.py` & `eko-0.9.4/src/eko/anomalous_dimensions/as1aem1.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/anomalous_dimensions/as2.py` & `eko-0.9.4/src/eko/anomalous_dimensions/as2.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/anomalous_dimensions/as3.py` & `eko-0.9.4/src/eko/anomalous_dimensions/as3.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/basis_rotation.py` & `eko-0.9.4/src/eko/basis_rotation.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/beta.py` & `eko-0.9.4/src/eko/beta.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/constants.py` & `eko-0.9.4/src/eko/constants.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/evolution_operator/__init__.py` & `eko-0.9.4/src/eko/evolution_operator/__init__.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/evolution_operator/flavors.py` & `eko-0.9.4/src/eko/evolution_operator/flavors.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/evolution_operator/grid.py` & `eko-0.9.4/src/eko/evolution_operator/grid.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/evolution_operator/physical.py` & `eko-0.9.4/src/eko/evolution_operator/physical.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/gamma.py` & `eko-0.9.4/src/eko/gamma.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/harmonics/__init__.py` & `eko-0.9.4/src/eko/harmonics/__init__.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/harmonics/f_functions/__init__.py` & `eko-0.9.4/src/eko/harmonics/f_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/harmonics/f_functions/f11.py` & `eko-0.9.4/src/eko/harmonics/f_functions/f11.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/harmonics/f_functions/f13.py` & `eko-0.9.4/src/eko/harmonics/f_functions/f13.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/harmonics/f_functions/f14_f12.py` & `eko-0.9.4/src/eko/harmonics/f_functions/f14_f12.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/harmonics/f_functions/f16.py` & `eko-0.9.4/src/eko/harmonics/f_functions/f16.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/harmonics/f_functions/f17.py` & `eko-0.9.4/src/eko/harmonics/f_functions/f17.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/harmonics/f_functions/f18.py` & `eko-0.9.4/src/eko/harmonics/f_functions/f18.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/harmonics/f_functions/f19.py` & `eko-0.9.4/src/eko/harmonics/f_functions/f19.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/harmonics/f_functions/f20.py` & `eko-0.9.4/src/eko/harmonics/f_functions/f20.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/harmonics/f_functions/f21.py` & `eko-0.9.4/src/eko/harmonics/f_functions/f21.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/harmonics/f_functions/f9.py` & `eko-0.9.4/src/eko/harmonics/f_functions/f9.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/harmonics/g_functions.py` & `eko-0.9.4/src/eko/harmonics/g_functions.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/harmonics/polygamma.py` & `eko-0.9.4/src/eko/harmonics/polygamma.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/harmonics/w1.py` & `eko-0.9.4/src/eko/harmonics/w1.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/harmonics/w2.py` & `eko-0.9.4/src/eko/harmonics/w2.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/harmonics/w3.py` & `eko-0.9.4/src/eko/harmonics/w3.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/harmonics/w4.py` & `eko-0.9.4/src/eko/harmonics/w4.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/harmonics/w5.py` & `eko-0.9.4/src/eko/harmonics/w5.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/interpolation.py` & `eko-0.9.4/src/eko/interpolation.py`

 * *Files 1% similar despite different names*

```diff
@@ -558,29 +558,31 @@
         for basis in self.basis:
             yield basis
 
     def __getitem__(self, item):
         return self.basis[item]
 
     def get_interpolation(self, targetgrid):
-        """
-        Computes interpolation matrix between `targetgrid` and `xgrid`.
+        """Computes interpolation matrix between `targetgrid` and `xgrid`.
 
         .. math::
             f(targetgrid) = R \\cdot f(xgrid)
 
         Parameters
         ----------
-            targetgrid : array
-                grid to interpolate to
+        targetgrid : array
+            grid to interpolate to
 
         Returns
         -------
-            R : array
-                interpolation matrix, do be multiplied from the left(!)
+        R : array
+            interpolation matrix $R_{ij}$, where $i$ is the index over
+            `targetgrid`, and $j$ is the index on the internal basis (the
+            one stored in the :class:`InterpolatorDispatcher` instance)
+
         """
         # trivial?
         if len(targetgrid) == len(self.xgrid_raw) and np.allclose(
             targetgrid, self.xgrid_raw
         ):
             return np.eye(len(self.xgrid_raw))
         # compute map
```

### Comparing `eko-0.9.3/src/eko/kernels/evolution_integrals.py` & `eko-0.9.4/src/eko/kernels/evolution_integrals.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/kernels/non_singlet.py` & `eko-0.9.4/src/eko/kernels/non_singlet.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/kernels/singlet.py` & `eko-0.9.4/src/eko/kernels/singlet.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/kernels/utils.py` & `eko-0.9.4/src/eko/kernels/utils.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/matching_conditions/__init__.py` & `eko-0.9.4/src/eko/matching_conditions/__init__.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/matching_conditions/as1.py` & `eko-0.9.4/src/eko/matching_conditions/as1.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/matching_conditions/as2.py` & `eko-0.9.4/src/eko/matching_conditions/as2.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/matching_conditions/as3/__init__.py` & `eko-0.9.4/src/eko/matching_conditions/as3/__init__.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/matching_conditions/as3/aHg.py` & `eko-0.9.4/src/eko/matching_conditions/as3/aHg.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/matching_conditions/as3/aHgstfac.py` & `eko-0.9.4/src/eko/matching_conditions/as3/aHgstfac.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/matching_conditions/as3/aHq.py` & `eko-0.9.4/src/eko/matching_conditions/as3/aHq.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/matching_conditions/as3/agg.py` & `eko-0.9.4/src/eko/matching_conditions/as3/agg.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/matching_conditions/as3/aggTF2.py` & `eko-0.9.4/src/eko/matching_conditions/as3/aggTF2.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/matching_conditions/as3/agq.py` & `eko-0.9.4/src/eko/matching_conditions/as3/agq.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/matching_conditions/as3/aqg.py` & `eko-0.9.4/src/eko/matching_conditions/as3/aqg.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/matching_conditions/as3/aqqNS.py` & `eko-0.9.4/src/eko/matching_conditions/as3/aqqNS.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/matching_conditions/as3/aqqPS.py` & `eko-0.9.4/src/eko/matching_conditions/as3/aqqPS.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/matching_conditions/operator_matrix_element.py` & `eko-0.9.4/src/eko/matching_conditions/operator_matrix_element.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 
 import numba as nb
 import numpy as np
 
 from .. import basis_rotation as br
 from .. import harmonics
 from ..evolution_operator import Operator, QuadKerBase
-from . import as1, as2, as3
+from . import as1, as2
+
+# _N3LO_ from . import as1, as2, as3
 
 logger = logging.getLogger(__name__)
 
 
 @nb.njit(cache=True)
 def compute_harmonics_cache(n, order, is_singlet):
     r"""
@@ -42,27 +44,30 @@
                 [[S_1,S_{-1}],
                 [S_2,S_{-2}],
                 [S_{3}, S_{2,1}, S_{2,-1}, S_{-2,1}, S_{-2,-1}, S_{-3}],
                 [S_{4}, S_{3,1}, S_{2,1,1}, S_{-2,-2}, S_{-3, 1}, S_{-4}],]
 
     """
     # max harmonics sum weight for each qcd order
-    max_weight = {1: 2, 2: 3, 3: 5}
+    max_weight = {1: 2, 2: 3, 3: 3}
+    # _N3LO_ max_weight = {1: 2, 2: 3, 3: 5}
     # max number of harmonics sum of a given weight for each qcd order
-    n_max_sums_weight = {1: 1, 2: 3, 3: 7}
+    n_max_sums_weight = {1: 1, 2: 3, 3: 3}
+    # _N3LO_ n_max_sums_weight = {1: 1, 2: 3, 3: 7}
     sx = harmonics.base_harmonics_cache(
         n, is_singlet, max_weight[order], n_max_sums_weight[order]
     )
-    if order == 2:
+    # _N3LO_ if order == 2:
+    if order >= 2:
         # Add Sm21 to cache
         sx[2, 1] = harmonics.Sm21(n, sx[0, 0], sx[0, -1], is_singlet)
-    if order == 3:
-        # Add weight 3 and 4 to cache
-        sx[2, 1:-2] = harmonics.s3x(n, sx[:, 0], sx[:, -1], is_singlet)
-        sx[3, 1:-1] = harmonics.s4x(n, sx[:, 0], sx[:, -1], is_singlet)
+    # _N3LO_ if order == 3:
+    #     # Add weight 3 and 4 to cache
+    #     sx[2, 1:-2] = harmonics.s3x(n, sx[:, 0], sx[:, -1], is_singlet)
+    #     sx[3, 1:-1] = harmonics.s4x(n, sx[:, 0], sx[:, -1], is_singlet)
     # return list of list keeping the non zero values
     return [[el for el in sx_list if el != 0] for sx_list in sx]
 
 
 @nb.njit(cache=True)
 def A_singlet(order, n, sx, nf, L, is_msbar, sx_ns=None):
     r"""
@@ -98,16 +103,16 @@
         eko.matching_conditions.nnlo.A_singlet_2 : :math:`A_{S,(2)}(N)`
     """
     A_s = np.zeros((order, 3, 3), np.complex_)
     if order >= 1:
         A_s[0] = as1.A_singlet(n, sx, L)
     if order >= 2:
         A_s[1] = as2.A_singlet(n, sx, L, is_msbar)
-    if order >= 3:
-        A_s[2] = as3.A_singlet(n, sx, sx_ns, nf, L)
+    # _N3LO_ if order >= 3:
+    #     A_s[2] = as3.A_singlet(n, sx, sx_ns, nf, L)
     return A_s
 
 
 @nb.njit(cache=True)
 def A_non_singlet(order, n, sx, nf, L):
     r"""
     Computes the tower of the non-singlet |OME|
@@ -136,16 +141,16 @@
         eko.matching_conditions.nnlo.A_ns_2 : :math:`A_{qq,H}^{NS,(2)}`
     """
     A_ns = np.zeros((order, 2, 2), np.complex_)
     if order >= 1:
         A_ns[0] = as1.A_ns(n, sx, L)
     if order >= 2:
         A_ns[1] = as2.A_ns(n, sx, L)
-    if order >= 3:
-        A_ns[2] = as3.A_ns(n, sx, nf, L)
+    # _N3LO_ if order >= 3:
+    #     A_ns[2] = as3.A_ns(n, sx, nf, L)
     return A_ns
 
 
 @nb.njit(cache=True)
 def build_ome(A, order, a_s, backward_method):
     r"""
     Construct the matching expansion in :math:`a_s` with the appropriate method.
@@ -238,32 +243,32 @@
     ker_base = QuadKerBase(u, is_log, logx, mode0)
     integrand = ker_base.integrand(areas)
     if integrand == 0.0:
         return 0.0
 
     sx = compute_harmonics_cache(ker_base.n, order, ker_base.is_singlet)
     sx_ns = None
-    if order == 3 and (
-        (backward_method != "" and ker_base.is_singlet)
-        or (mode0 == 100 and mode0 == 100)
-    ):
-        # At N3LO for A_qq singlet or backward you need to compute
-        # both the singlet and non-singlet like harmonics
-        # avoiding recomputing all of them ...
-        sx_ns = sx.copy()
-        smx_ns = harmonics.smx(ker_base.n, np.array([s[0] for s in sx]), False)
-        for w, sm in enumerate(smx_ns):
-            sx_ns[w][-1] = sm
-        sx_ns[2][2] = harmonics.S2m1(ker_base.n, sx[0][1], smx_ns[0], smx_ns[1], False)
-        sx_ns[2][3] = harmonics.Sm21(ker_base.n, sx[0][0], smx_ns[0], False)
-        sx_ns[3][5] = harmonics.Sm31(ker_base.n, sx[0][0], smx_ns[0], smx_ns[1], False)
-        sx_ns[3][4] = harmonics.Sm211(ker_base.n, sx[0][0], sx[0][1], smx_ns[0], False)
-        sx_ns[3][3] = harmonics.Sm22(
-            ker_base.n, sx[0][0], sx[0][1], smx_ns[1], sx_ns[3][5], False
-        )
+    # _N3LO_ if order == 3 and (
+    #     (backward_method != "" and ker_base.is_singlet)
+    #     or (mode0 == 100 and mode0 == 100)
+    # ):
+    #     # At N3LO for A_qq singlet or backward you need to compute
+    #     # both the singlet and non-singlet like harmonics
+    #     # avoiding recomputing all of them ...
+    #     sx_ns = sx.copy()
+    #     smx_ns = harmonics.smx(ker_base.n, np.array([s[0] for s in sx]), False)
+    #     for w, sm in enumerate(smx_ns):
+    #         sx_ns[w][-1] = sm
+    #     sx_ns[2][2] = harmonics.S2m1(ker_base.n, sx[0][1], smx_ns[0], smx_ns[1], False)
+    #     sx_ns[2][3] = harmonics.Sm21(ker_base.n, sx[0][0], smx_ns[0], False)
+    #     sx_ns[3][5] = harmonics.Sm31(ker_base.n, sx[0][0], smx_ns[0], smx_ns[1], False)
+    #     sx_ns[3][4] = harmonics.Sm211(ker_base.n, sx[0][0], sx[0][1], smx_ns[0], False)
+    #     sx_ns[3][3] = harmonics.Sm22(
+    #         ker_base.n, sx[0][0], sx[0][1], smx_ns[1], sx_ns[3][5], False
+    #     )
 
     # compute the ome
     if ker_base.is_singlet:
         indices = {21: 0, 100: 1, 90: 2}
         A = A_singlet(order, ker_base.n, sx, nf, L, is_msbar, sx_ns)
     else:
         indices = {200: 0, 91: 1}
```

### Comparing `eko-0.9.3/src/eko/mellin.py` & `eko-0.9.4/src/eko/mellin.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/member.py` & `eko-0.9.4/src/eko/member.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/msbar_masses.py` & `eko-0.9.4/src/eko/msbar_masses.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/output.py` & `eko-0.9.4/src/eko/output.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/runner.py` & `eko-0.9.4/src/eko/runner.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/scale_variations/expanded.py` & `eko-0.9.4/src/eko/scale_variations/expanded.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/scale_variations/exponentiated.py` & `eko-0.9.4/src/eko/scale_variations/exponentiated.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/strong_coupling.py` & `eko-0.9.4/src/eko/strong_coupling.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/eko/thresholds.py` & `eko-0.9.4/src/eko/thresholds.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/ekobox/evol_pdf.py` & `eko-0.9.4/src/ekobox/evol_pdf.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/ekobox/gen_info.py` & `eko-0.9.4/src/ekobox/gen_info.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/ekobox/gen_op.py` & `eko-0.9.4/src/ekobox/gen_op.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/ekobox/gen_theory.py` & `eko-0.9.4/src/ekobox/gen_theory.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/ekobox/genpdf/Toy.info` & `eko-0.9.4/src/ekobox/genpdf/Toy.info`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/ekobox/genpdf/__init__.py` & `eko-0.9.4/src/ekobox/genpdf/__init__.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/ekobox/genpdf/cli.py` & `eko-0.9.4/src/ekobox/genpdf/cli.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/ekobox/genpdf/export.py` & `eko-0.9.4/src/ekobox/genpdf/export.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/ekobox/genpdf/flavors.py` & `eko-0.9.4/src/ekobox/genpdf/flavors.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/ekobox/genpdf/load.py` & `eko-0.9.4/src/ekobox/genpdf/load.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/ekobox/genpdf/templatePDF.info` & `eko-0.9.4/src/ekobox/genpdf/templatePDF.info`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/ekobox/mock.py` & `eko-0.9.4/src/ekobox/mock.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/ekobox/utils.py` & `eko-0.9.4/src/ekobox/utils.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/ekomark/apply.py` & `eko-0.9.4/src/ekomark/apply.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/ekomark/benchmark/external/LHA.yaml` & `eko-0.9.4/src/ekomark/benchmark/external/LHA.yaml`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/ekomark/benchmark/external/LHA_utils.py` & `eko-0.9.4/src/ekomark/benchmark/external/LHA_utils.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/ekomark/benchmark/external/apfel_utils.py` & `eko-0.9.4/src/ekomark/benchmark/external/apfel_utils.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/ekomark/benchmark/external/lhapdf_utils.py` & `eko-0.9.4/src/ekomark/benchmark/external/lhapdf_utils.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/ekomark/benchmark/external/pegasus_utils.py` & `eko-0.9.4/src/ekomark/benchmark/external/pegasus_utils.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/ekomark/benchmark/runner.py` & `eko-0.9.4/src/ekomark/benchmark/runner.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/ekomark/data/db.py` & `eko-0.9.4/src/ekomark/data/db.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/ekomark/data/operators.py` & `eko-0.9.4/src/ekomark/data/operators.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/ekomark/navigator/__init__.py` & `eko-0.9.4/src/ekomark/navigator/__init__.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/ekomark/navigator/navigator.py` & `eko-0.9.4/src/ekomark/navigator/navigator.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/src/ekomark/plots.py` & `eko-0.9.4/src/ekomark/plots.py`

 * *Files identical despite different names*

### Comparing `eko-0.9.3/setup.py` & `eko-0.9.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 entry_points = \
 {'console_scripts': ['ekonav = ekomark.navigator:launch_navigator',
                      'genpdf = ekobox.genpdf.cli:cli']}
 
 setup_kwargs = {
     'name': 'eko',
-    'version': '0.9.3',
+    'version': '0.9.4',
     'description': 'Evolution Kernel Operator',
     'long_description': '<p align="center">\n  <a href="https://eko.readthedocs.io/"><img alt="EKO" src="https://raw.githubusercontent.com/N3PDF/eko/master/doc/source/img/Logo.png" width=300></a>\n</p>\n<p align="center">\n  <a href="https://github.com/N3PDF/eko/actions/workflows/unittests.yml"><img alt="Tests" src="https://github.com/N3PDF/eko/actions/workflows/unittests.yml/badge.svg" /></a>\n  <a href="https://eko.readthedocs.io/en/latest/?badge=latest"><img alt="Docs" src="https://readthedocs.org/projects/eko/badge/?version=latest"></a>\n  <a href="https://codecov.io/gh/N3PDF/eko"><img src="https://codecov.io/gh/N3PDF/eko/branch/master/graph/badge.svg" /></a>\n  <a href="https://www.codefactor.io/repository/github/n3pdf/eko"><img src="https://www.codefactor.io/repository/github/n3pdf/eko/badge" alt="CodeFactor" /></a>\n</p>\n\nEKO is a Python module to solve the DGLAP equations in N-space in terms of Evolution Kernel Operators in x-space.\n\n## Installation\nEKO is available via\n- PyPI: <a href="https://pypi.org/project/eko/"><img alt="PyPI" src="https://img.shields.io/pypi/v/eko"/></a>\n```bash\npip install eko\n```\n- conda-forge: [![Conda Version](https://img.shields.io/conda/vn/conda-forge/eko.svg)](https://anaconda.org/conda-forge/eko)\n```bash\nconda install eko\n```\n\n### Development\n\nIf you want to install from source you can run\n```bash\ngit clone git@github.com:N3PDF/eko.git\ncd eko\npoetry install\n```\n\nTo setup `poetry`, and other tools, see [Contribution\nGuidelines](https://github.com/N3PDF/eko/blob/master/.github/CONTRIBUTING.md).\n\n## Documentation\n- The documentation is available here: <a href="https://eko.readthedocs.io/en/latest/?badge=latest"><img alt="Docs" src="https://readthedocs.org/projects/eko/badge/?version=latest"></a>\n- To build the documentation from source install [graphviz](https://www.graphviz.org/) and run in addition to the installation commands\n```bash\npoe docs\n```\n\n## Tests and benchmarks\n- To run unit test you can do\n```bash\npoe tests\n```\n\n- Benchmarks of specific part of the code, such as the strong coupling or msbar masses running, are available doing\n```bash\npoe bench\n```\n\n- The complete list of benchmarks with external codes is available through `ekomark`: [documentation](https://eko.readthedocs.io/en/latest/development/Benchmarks.html)\n\n## Citation policy\nWhen using our code please cite\n- our DOI: <a href="https://doi.org/10.5281/zenodo.3874237"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.3874237.svg" alt="DOI"/></a>\n- our paper: [![arXiv](https://img.shields.io/badge/arXiv-2202.02338-b31b1b?labelColor=222222)](https://arxiv.org/abs/2202.02338)\n\n## Contributing\n- Your feedback is welcome! If you want to report a (possible) bug or want to ask for a new feature, please raise an issue: <a href="https://github.com/N3PDF/eko/issues"><img alt="GitHub issues" src="https://img.shields.io/github/issues/N3PDF/eko"/></a>\n- Please follow our [Code of Conduct](https://github.com/N3PDF/eko/blob/master/.github/CODE_OF_CONDUCT.md) and read the\n  [Contribution Guidelines](https://github.com/N3PDF/eko/blob/master/.github/CONTRIBUTING.md)\n',
     'author': 'A. Candido',
     'author_email': 'alessandro.candido@mi.infn.it',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/N3PDF/eko',
```

#### html2text {}

```diff
@@ -10,15 +10,15 @@
 ['banana-hep>=0.6.5,<0.7.0', 'sqlalchemy>=1.4.21,<2.0.0',
 'pandas>=1.3.0,<2.0.0', 'matplotlib>=3.5.1,<4.0.0'], 'docs':
 ['Sphinx>=4.3.2,<5.0.0', 'sphinx-rtd-theme>=1.0.0,<2.0.0', 'sphinxcontrib-
 bibtex>=2.4.1,<3.0.0', 'nbsphinx>=0.8.8,<0.9.0'], 'mark': ['banana-
 hep>=0.6.5,<0.7.0', 'sqlalchemy>=1.4.21,<2.0.0', 'pandas>=1.3.0,<2.0.0',
 'matplotlib>=3.5.1,<4.0.0']} entry_points = \ {'console_scripts': ['ekonav =
 ekomark.navigator:launch_navigator', 'genpdf = ekobox.genpdf.cli:cli']}
-setup_kwargs = { 'name': 'eko', 'version': '0.9.3', 'description': 'Evolution
+setup_kwargs = { 'name': 'eko', 'version': '0.9.4', 'description': 'Evolution
 Kernel Operator', 'long_description': '
                                   \n [EKO]\n
 \n
   \n [Tests]\n [Docs]\n [https://codecov.io/gh/N3PDF/eko/branch/master/graph/
                           badge.svg]\n [CodeFactor]\n
 \n\nEKO is a Python module to solve the DGLAP equations in N-space in terms of
 Evolution Kernel Operators in x-space.\n\n## Installation\nEKO is available
```

### Comparing `eko-0.9.3/PKG-INFO` & `eko-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eko
-Version: 0.9.3
+Version: 0.9.4
 Summary: Evolution Kernel Operator
 Home-page: https://github.com/N3PDF/eko
 Author: A. Candido
 Author-email: alessandro.candido@mi.infn.it
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: eko Version: 0.9.3 Summary: Evolution Kernel
+Metadata-Version: 2.1 Name: eko Version: 0.9.4 Summary: Evolution Kernel
 Operator Home-page: https://github.com/N3PDF/eko Author: A. Candido Author-
 email: alessandro.candido@mi.infn.it Requires-Python: >=3.8,<3.11 Classifier:
 License :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering Classifier: Topic :: Scientific/
```

