# Comparing `tmp/orjson-3.8.8.tar.gz` & `tmp/orjson-3.8.9.tar.gz`

## Comparing `orjson-3.8.8.tar` & `orjson-3.8.9.tar`

### file list

```diff
@@ -1,491 +1,491 @@
--rw-r--r--   0        0        0     2560 1970-01-01 00:00:00.000000 orjson-3.8.8/Cargo.toml
--rw-r--r--   0     1001      123    16475 2023-03-20 23:21:57.000000 orjson-3.8.8/CHANGELOG.md
--rw-r--r--   0     1001      123    10847 2023-03-20 23:21:57.000000 orjson-3.8.8/LICENSE-APACHE
--rw-r--r--   0     1001      123     1023 2023-03-20 23:21:57.000000 orjson-3.8.8/LICENSE-MIT
--rw-r--r--   0     1001      123    46350 2023-03-20 23:21:57.000000 orjson-3.8.8/README.md
--rw-r--r--   0     1001      123     8780 2023-03-20 23:21:57.000000 orjson-3.8.8/data/blns.txt.xz
--rw-r--r--   0     1001      123   376512 2023-03-20 23:21:57.000000 orjson-3.8.8/data/canada.json.xz
--rw-r--r--   0     1001      123    12336 2023-03-20 23:21:57.000000 orjson-3.8.8/data/citm_catalog.json.xz
--rw-r--r--   0     1001      123     8264 2023-03-20 23:21:57.000000 orjson-3.8.8/data/github.json.xz
--rw-r--r--   0     1001      123      592 2023-03-20 23:21:57.000000 orjson-3.8.8/data/issue331_1.json.xz
--rw-r--r--   0     1001      123      592 2023-03-20 23:21:57.000000 orjson-3.8.8/data/issue331_2.json.xz
--rw-r--r--   0     1001      123       60 2023-03-20 23:21:57.000000 orjson-3.8.8/data/jsonchecker/fail01.json
--rw-r--r--   0     1001      123       17 2023-03-20 23:21:57.000000 orjson-3.8.8/data/jsonchecker/fail02.json
--rw-r--r--   0     1001      123       37 2023-03-20 23:21:57.000000 orjson-3.8.8/data/jsonchecker/fail03.json
--rw-r--r--   0     1001      123       16 2023-03-20 23:21:57.000000 orjson-3.8.8/data/jsonchecker/fail04.json
--rw-r--r--   0     1001      123       24 2023-03-20 23:21:57.000000 orjson-3.8.8/data/jsonchecker/fail05.json
--rw-r--r--   0     1001      123       26 2023-03-20 23:21:57.000000 orjson-3.8.8/data/jsonchecker/fail06.json
--rw-r--r--   0     1001      123       26 2023-03-20 23:21:57.000000 orjson-3.8.8/data/jsonchecker/fail07.json
--rw-r--r--   0     1001      123       16 2023-03-20 23:21:57.000000 orjson-3.8.8/data/jsonchecker/fail08.json
--rw-r--r--   0     1001      123       22 2023-03-20 23:21:57.000000 orjson-3.8.8/data/jsonchecker/fail09.json
--rw-r--r--   0     1001      123       58 2023-03-20 23:21:57.000000 orjson-3.8.8/data/jsonchecker/fail10.json
--rw-r--r--   0     1001      123       29 2023-03-20 23:21:57.000000 orjson-3.8.8/data/jsonchecker/fail11.json
--rw-r--r--   0     1001      123       31 2023-03-20 23:21:57.000000 orjson-3.8.8/data/jsonchecker/fail12.json
--rw-r--r--   0     1001      123       43 2023-03-20 23:21:57.000000 orjson-3.8.8/data/jsonchecker/fail13.json
--rw-r--r--   0     1001      123       31 2023-03-20 23:21:57.000000 orjson-3.8.8/data/jsonchecker/fail14.json
--rw-r--r--   0     1001      123       34 2023-03-20 23:21:57.000000 orjson-3.8.8/data/jsonchecker/fail15.json
--rw-r--r--   0     1001      123        8 2023-03-20 23:21:57.000000 orjson-3.8.8/data/jsonchecker/fail16.json
--rw-r--r--   0     1001      123       34 2023-03-20 23:21:57.000000 orjson-3.8.8/data/jsonchecker/fail17.json
--rw-r--r--   0     1001      123       50 2023-03-20 23:21:57.000000 orjson-3.8.8/data/jsonchecker/fail18.json
--rw-r--r--   0     1001      123       22 2023-03-20 23:21:57.000000 orjson-3.8.8/data/jsonchecker/fail19.json
--rw-r--r--   0     1001      123       23 2023-03-20 23:21:57.000000 orjson-3.8.8/data/jsonchecker/fail20.json
--rw-r--r--   0     1001      123       32 2023-03-20 23:21:57.000000 orjson-3.8.8/data/jsonchecker/fail21.json
--rw-r--r--   0     1001      123       33 2023-03-20 23:21:57.000000 orjson-3.8.8/data/jsonchecker/fail22.json
--rw-r--r--   0     1001      123       20 2023-03-20 23:21:57.000000 orjson-3.8.8/data/jsonchecker/fail23.json
--rw-r--r--   0     1001      123       16 2023-03-20 23:21:57.000000 orjson-3.8.8/data/jsonchecker/fail24.json
--rw-r--r--   0     1001      123       29 2023-03-20 23:21:57.000000 orjson-3.8.8/data/jsonchecker/fail25.json
--rw-r--r--   0     1001      123       38 2023-03-20 23:21:57.000000 orjson-3.8.8/data/jsonchecker/fail26.json
--rw-r--r--   0     1001      123       14 2023-03-20 23:21:57.000000 orjson-3.8.8/data/jsonchecker/fail27.json
--rw-r--r--   0     1001      123       15 2023-03-20 23:21:57.000000 orjson-3.8.8/data/jsonchecker/fail28.json
--rw-r--r--   0     1001      123        4 2023-03-20 23:21:57.000000 orjson-3.8.8/data/jsonchecker/fail29.json
--rw-r--r--   0     1001      123        5 2023-03-20 23:21:57.000000 orjson-3.8.8/data/jsonchecker/fail30.json
--rw-r--r--   0     1001      123        7 2023-03-20 23:21:57.000000 orjson-3.8.8/data/jsonchecker/fail31.json
--rw-r--r--   0     1001      123       40 2023-03-20 23:21:57.000000 orjson-3.8.8/data/jsonchecker/fail32.json
--rw-r--r--   0     1001      123       12 2023-03-20 23:21:57.000000 orjson-3.8.8/data/jsonchecker/fail33.json
--rw-r--r--   0     1001      123     1441 2023-03-20 23:21:57.000000 orjson-3.8.8/data/jsonchecker/pass01.json
--rw-r--r--   0     1001      123       52 2023-03-20 23:21:57.000000 orjson-3.8.8/data/jsonchecker/pass02.json
--rw-r--r--   0     1001      123      148 2023-03-20 23:21:57.000000 orjson-3.8.8/data/jsonchecker/pass03.json
--rw-r--r--   0     1001      123       14 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/i_number_double_huge_neg_exp.json
--rw-r--r--   0     1001      123      137 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/i_number_huge_exp.json
--rw-r--r--   0     1001      123       10 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/i_number_neg_int_huge_exp.json
--rw-r--r--   0     1001      123       11 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/i_number_pos_double_huge_exp.json
--rw-r--r--   0     1001      123       16 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/i_number_real_neg_overflow.json
--rw-r--r--   0     1001      123       15 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/i_number_real_pos_overflow.json
--rw-r--r--   0     1001      123       15 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/i_number_real_underflow.json
--rw-r--r--   0     1001      123       33 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/i_number_too_big_neg_int.json
--rw-r--r--   0     1001      123       23 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/i_number_too_big_pos_int.json
--rw-r--r--   0     1001      123       51 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/i_number_very_big_negative_int.json
--rw-r--r--   0     1001      123       12 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/i_object_key_lone_2nd_surrogate.json
--rw-r--r--   0     1001      123       10 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/i_string_1st_surrogate_but_2nd_missing.json
--rw-r--r--   0     1001      123       16 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/i_string_1st_valid_surrogate_2nd_invalid.json
--rw-r--r--   0     1001      123       12 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/i_string_UTF-16LE_with_BOM.json
--rw-r--r--   0     1001      123       10 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/i_string_UTF-8_invalid_sequence.json
--rw-r--r--   0     1001      123        7 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/i_string_UTF8_surrogate_U+D800.json
--rw-r--r--   0     1001      123       12 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/i_string_incomplete_surrogate_and_escape_valid.json
--rw-r--r--   0     1001      123       11 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/i_string_incomplete_surrogate_pair.json
--rw-r--r--   0     1001      123       18 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/i_string_incomplete_surrogates_escape_valid.json
--rw-r--r--   0     1001      123       10 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/i_string_invalid_lonely_surrogate.json
--rw-r--r--   0     1001      123       13 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/i_string_invalid_surrogate.json
--rw-r--r--   0     1001      123        5 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/i_string_invalid_utf-8.json
--rw-r--r--   0     1001      123       16 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/i_string_inverted_surrogates_U+1D11E.json
--rw-r--r--   0     1001      123        5 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/i_string_iso_latin_1.json
--rw-r--r--   0     1001      123       10 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/i_string_lone_second_surrogate.json
--rw-r--r--   0     1001      123        5 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/i_string_lone_utf8_continuation_byte.json
--rw-r--r--   0     1001      123        8 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/i_string_not_in_unicode_range.json
--rw-r--r--   0     1001      123        6 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/i_string_overlong_sequence_2_bytes.json
--rw-r--r--   0     1001      123       10 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/i_string_overlong_sequence_6_bytes.json
--rw-r--r--   0     1001      123       10 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/i_string_overlong_sequence_6_bytes_null.json
--rw-r--r--   0     1001      123        6 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/i_string_truncated-utf-8.json
--rw-r--r--   0     1001      123       10 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/i_string_utf16BE_no_BOM.json
--rw-r--r--   0     1001      123       10 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/i_string_utf16LE_no_BOM.json
--rw-r--r--   0     1001      123       80 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/i_structure_500_nested_arrays.json.xz
--rw-r--r--   0     1001      123        5 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/i_structure_UTF-8_BOM_empty_object.json
--rw-r--r--   0     1001      123        8 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_array_1_true_without_comma.json
--rw-r--r--   0     1001      123        4 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_array_a_invalid_utf8.json
--rw-r--r--   0     1001      123        7 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_array_colon_instead_of_comma.json
--rw-r--r--   0     1001      123        5 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_array_comma_after_close.json
--rw-r--r--   0     1001      123        4 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_array_comma_and_number.json
--rw-r--r--   0     1001      123        6 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_array_double_comma.json
--rw-r--r--   0     1001      123        7 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_array_double_extra_comma.json
--rw-r--r--   0     1001      123        6 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_array_extra_close.json
--rw-r--r--   0     1001      123        5 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_array_extra_comma.json
--rw-r--r--   0     1001      123        4 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_array_incomplete.json
--rw-r--r--   0     1001      123        2 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_array_incomplete_invalid_value.json
--rw-r--r--   0     1001      123        6 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_array_inner_array_no_comma.json
--rw-r--r--   0     1001      123        3 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_array_invalid_utf8.json
--rw-r--r--   0     1001      123        5 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_array_items_separated_by_semicolon.json
--rw-r--r--   0     1001      123        3 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_array_just_comma.json
--rw-r--r--   0     1001      123        3 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_array_just_minus.json
--rw-r--r--   0     1001      123        9 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_array_missing_value.json
--rw-r--r--   0     1001      123       11 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_array_newlines_unclosed.json
--rw-r--r--   0     1001      123        4 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_array_number_and_comma.json
--rw-r--r--   0     1001      123        5 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_array_number_and_several_commas.json
--rw-r--r--   0     1001      123        8 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_array_spaces_vertical_tab_formfeed.json
--rw-r--r--   0     1001      123        3 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_array_star_inside.json
--rw-r--r--   0     1001      123        3 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_array_unclosed.json
--rw-r--r--   0     1001      123        3 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_array_unclosed_trailing_comma.json
--rw-r--r--   0     1001      123        8 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_array_unclosed_with_new_lines.json
--rw-r--r--   0     1001      123        3 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_array_unclosed_with_object_inside.json
--rw-r--r--   0     1001      123        6 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_incomplete_false.json
--rw-r--r--   0     1001      123        5 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_incomplete_null.json
--rw-r--r--   0     1001      123        5 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_incomplete_true.json
--rw-r--r--   0     1001      123        4 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_multidigit_number_then_00.json
--rw-r--r--   0     1001      123        8 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_number_++.json
--rw-r--r--   0     1001      123        4 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_number_+1.json
--rw-r--r--   0     1001      123        6 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_number_+Inf.json
--rw-r--r--   0     1001      123        5 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_number_-01.json
--rw-r--r--   0     1001      123        7 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_number_-1.0..json
--rw-r--r--   0     1001      123        5 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_number_-2..json
--rw-r--r--   0     1001      123        6 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_number_-NaN.json
--rw-r--r--   0     1001      123        5 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_number_.-1.json
--rw-r--r--   0     1001      123        7 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_number_.2e-3.json
--rw-r--r--   0     1001      123        7 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_number_0.1.2.json
--rw-r--r--   0     1001      123        7 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_number_0.3e+.json
--rw-r--r--   0     1001      123        6 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_number_0.3e.json
--rw-r--r--   0     1001      123        6 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_number_0.e1.json
--rw-r--r--   0     1001      123        5 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_number_0_capital_E+.json
--rw-r--r--   0     1001      123        4 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_number_0_capital_E.json
--rw-r--r--   0     1001      123        5 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_number_0e+.json
--rw-r--r--   0     1001      123        4 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_number_0e.json
--rw-r--r--   0     1001      123        7 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_number_1.0e+.json
--rw-r--r--   0     1001      123        7 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_number_1.0e-.json
--rw-r--r--   0     1001      123        6 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_number_1.0e.json
--rw-r--r--   0     1001      123        9 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_number_1_000.json
--rw-r--r--   0     1001      123        6 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_number_1eE2.json
--rw-r--r--   0     1001      123        7 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_number_2.e+3.json
--rw-r--r--   0     1001      123        7 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_number_2.e-3.json
--rw-r--r--   0     1001      123        6 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_number_2.e3.json
--rw-r--r--   0     1001      123        6 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_number_9.e+.json
--rw-r--r--   0     1001      123        5 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_number_Inf.json
--rw-r--r--   0     1001      123        5 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_number_NaN.json
--rw-r--r--   0     1001      123        5 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_number_U+FF11_fullwidth_digit_one.json
--rw-r--r--   0     1001      123        5 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_number_expression.json
--rw-r--r--   0     1001      123        5 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_number_hex_1_digit.json
--rw-r--r--   0     1001      123        6 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_number_hex_2_digits.json
--rw-r--r--   0     1001      123       10 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_number_infinity.json
--rw-r--r--   0     1001      123        7 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_number_invalid+-.json
--rw-r--r--   0     1001      123       13 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_number_invalid-negative-real.json
--rw-r--r--   0     1001      123        6 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_number_invalid-utf-8-in-bigger-int.json
--rw-r--r--   0     1001      123        6 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_number_invalid-utf-8-in-exponent.json
--rw-r--r--   0     1001      123        5 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_number_invalid-utf-8-in-int.json
--rw-r--r--   0     1001      123       11 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_number_minus_infinity.json
--rw-r--r--   0     1001      123        6 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_number_minus_sign_with_trailing_garbage.json
--rw-r--r--   0     1001      123        5 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_number_minus_space_1.json
--rw-r--r--   0     1001      123        6 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_number_neg_int_starting_with_zero.json
--rw-r--r--   0     1001      123        7 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_number_neg_real_without_int_part.json
--rw-r--r--   0     1001      123        5 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_number_neg_with_garbage_at_end.json
--rw-r--r--   0     1001      123        5 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_number_real_garbage_after_e.json
--rw-r--r--   0     1001      123        5 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_number_real_with_invalid_utf8_after_e.json
--rw-r--r--   0     1001      123        4 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_number_real_without_fractional_part.json
--rw-r--r--   0     1001      123        6 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_number_starting_with_dot.json
--rw-r--r--   0     1001      123        8 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_number_with_alpha.json
--rw-r--r--   0     1001      123       25 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_number_with_alpha_char.json
--rw-r--r--   0     1001      123        5 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_number_with_leading_zero.json
--rw-r--r--   0     1001      123       12 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_object_bad_value.json
--rw-r--r--   0     1001      123        9 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_object_bracket_key.json
--rw-r--r--   0     1001      123       11 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_object_comma_instead_of_colon.json
--rw-r--r--   0     1001      123       10 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_object_double_colon.json
--rw-r--r--   0     1001      123       10 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_object_emoji.json
--rw-r--r--   0     1001      123       13 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_object_garbage_at_end.json
--rw-r--r--   0     1001      123       14 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_object_key_with_single_quotes.json
--rw-r--r--   0     1001      123       10 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_object_lone_continuation_byte_in_key_and_trailing_comma.json
--rw-r--r--   0     1001      123        7 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_object_missing_colon.json
--rw-r--r--   0     1001      123        6 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_object_missing_key.json
--rw-r--r--   0     1001      123        9 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_object_missing_semicolon.json
--rw-r--r--   0     1001      123        5 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_object_missing_value.json
--rw-r--r--   0     1001      123        4 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_object_no-colon.json
--rw-r--r--   0     1001      123        5 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_object_non_string_key.json
--rw-r--r--   0     1001      123       13 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_object_non_string_key_but_huge_number_instead.json
--rw-r--r--   0     1001      123       21 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_object_repeated_null_null.json
--rw-r--r--   0     1001      123       13 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_object_several_trailing_commas.json
--rw-r--r--   0     1001      123        7 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_object_single_quote.json
--rw-r--r--   0     1001      123        9 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_object_trailing_comma.json
--rw-r--r--   0     1001      123       13 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_object_trailing_comment.json
--rw-r--r--   0     1001      123       14 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_object_trailing_comment_open.json
--rw-r--r--   0     1001      123       11 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_object_trailing_comment_slash_open.json
--rw-r--r--   0     1001      123       10 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_object_trailing_comment_slash_open_incomplete.json
--rw-r--r--   0     1001      123       18 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_object_two_commas_in_a_row.json
--rw-r--r--   0     1001      123        8 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_object_unquoted_key.json
--rw-r--r--   0     1001      123        7 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_object_unterminated-value.json
--rw-r--r--   0     1001      123       22 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_object_with_single_string.json
--rw-r--r--   0     1001      123       10 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_object_with_trailing_garbage.json
--rw-r--r--   0     1001      123        1 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_single_space.json
--rw-r--r--   0     1001      123       11 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_string_1_surrogate_then_escape.json
--rw-r--r--   0     1001      123       12 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_string_1_surrogate_then_escape_u.json
--rw-r--r--   0     1001      123       13 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_string_1_surrogate_then_escape_u1.json
--rw-r--r--   0     1001      123       14 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_string_1_surrogate_then_escape_u1x.json
--rw-r--r--   0     1001      123        4 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_string_accentuated_char_no_quotes.json
--rw-r--r--   0     1001      123        6 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_string_backslash_00.json
--rw-r--r--   0     1001      123        8 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_string_escape_x.json
--rw-r--r--   0     1001      123        7 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_string_escaped_backslash_bad.json
--rw-r--r--   0     1001      123        6 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_string_escaped_ctrl_char_tab.json
--rw-r--r--   0     1001      123        9 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_string_escaped_emoji.json
--rw-r--r--   0     1001      123        5 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_string_incomplete_escape.json
--rw-r--r--   0     1001      123        9 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_string_incomplete_escaped_character.json
--rw-r--r--   0     1001      123       14 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_string_incomplete_surrogate.json
--rw-r--r--   0     1001      123       18 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_string_incomplete_surrogate_escape_invalid.json
--rw-r--r--   0     1001      123        7 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_string_invalid-utf-8-in-escape.json
--rw-r--r--   0     1001      123        6 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_string_invalid_backslash_esc.json
--rw-r--r--   0     1001      123       10 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_string_invalid_unicode_escape.json
--rw-r--r--   0     1001      123        6 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_string_invalid_utf8_after_escape.json
--rw-r--r--   0     1001      123       13 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_string_leading_uescaped_thinspace.json
--rw-r--r--   0     1001      123        4 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_string_no_quotes_with_bad_escape.json
--rw-r--r--   0     1001      123        1 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_string_single_doublequote.json
--rw-r--r--   0     1001      123       16 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_string_single_quote.json
--rw-r--r--   0     1001      123        3 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_string_single_string_no_double_quotes.json
--rw-r--r--   0     1001      123        3 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_string_start_escape_unclosed.json
--rw-r--r--   0     1001      123        7 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_string_unescaped_crtl_char.json
--rw-r--r--   0     1001      123       12 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_string_unescaped_newline.json
--rw-r--r--   0     1001      123        5 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_string_unescaped_tab.json
--rw-r--r--   0     1001      123        8 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_string_unicode_CapitalU.json
--rw-r--r--   0     1001      123        3 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_string_with_trailing_garbage.json
--rw-r--r--   0     1001      123      148 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_structure_100000_opening_arrays.json.xz
--rw-r--r--   0     1001      123        5 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_structure_U+2060_word_joined.json
--rw-r--r--   0     1001      123        3 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_structure_UTF8_BOM_no_data.json
--rw-r--r--   0     1001      123        3 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_structure_angle_bracket_..json
--rw-r--r--   0     1001      123        8 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_structure_angle_bracket_null.json
--rw-r--r--   0     1001      123        4 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_structure_array_trailing_garbage.json
--rw-r--r--   0     1001      123        4 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_structure_array_with_extra_array_close.json
--rw-r--r--   0     1001      123        6 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_structure_array_with_unclosed_string.json
--rw-r--r--   0     1001      123        3 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_structure_ascii-unicode-identifier.json
--rw-r--r--   0     1001      123        6 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_structure_capitalized_True.json
--rw-r--r--   0     1001      123        2 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_structure_close_unopened_array.json
--rw-r--r--   0     1001      123       11 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_structure_comma_instead_of_closing_brace.json
--rw-r--r--   0     1001      123        4 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_structure_double_array.json
--rw-r--r--   0     1001      123        1 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_structure_end_array.json
--rw-r--r--   0     1001      123        4 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_structure_incomplete_UTF8_BOM.json
--rw-r--r--   0     1001      123        1 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_structure_lone-invalid-utf-8.json
--rw-r--r--   0     1001      123        1 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_structure_lone-open-bracket.json
--rw-r--r--   0     1001      123        0 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_structure_no_data.json
--rw-r--r--   0     1001      123        3 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_structure_null-byte-outside-string.json
--rw-r--r--   0     1001      123        2 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_structure_number_with_trailing_garbage.json
--rw-r--r--   0     1001      123        3 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_structure_object_followed_by_closing_object.json
--rw-r--r--   0     1001      123        4 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_structure_object_unclosed_no_value.json
--rw-r--r--   0     1001      123       20 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_structure_object_with_comment.json
--rw-r--r--   0     1001      123       15 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_structure_object_with_trailing_garbage.json
--rw-r--r--   0     1001      123        2 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_structure_open_array_apostrophe.json
--rw-r--r--   0     1001      123        2 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_structure_open_array_comma.json
--rw-r--r--   0     1001      123      176 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_structure_open_array_object.json.xz
--rw-r--r--   0     1001      123        2 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_structure_open_array_open_object.json
--rw-r--r--   0     1001      123        3 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_structure_open_array_open_string.json
--rw-r--r--   0     1001      123        4 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_structure_open_array_string.json
--rw-r--r--   0     1001      123        1 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_structure_open_object.json
--rw-r--r--   0     1001      123        2 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_structure_open_object_close_array.json
--rw-r--r--   0     1001      123        2 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_structure_open_object_comma.json
--rw-r--r--   0     1001      123        2 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_structure_open_object_open_array.json
--rw-r--r--   0     1001      123        3 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_structure_open_object_open_string.json
--rw-r--r--   0     1001      123        4 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_structure_open_object_string_with_apostrophes.json
--rw-r--r--   0     1001      123       16 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_structure_open_open.json
--rw-r--r--   0     1001      123        1 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_structure_single_eacute.json
--rw-r--r--   0     1001      123        1 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_structure_single_star.json
--rw-r--r--   0     1001      123       12 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_structure_trailing_#.json
--rw-r--r--   0     1001      123       10 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_structure_uescaped_LF_before_string.json
--rw-r--r--   0     1001      123        2 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_structure_unclosed_array.json
--rw-r--r--   0     1001      123       12 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_structure_unclosed_array_partial_null.json
--rw-r--r--   0     1001      123       12 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_structure_unclosed_array_unfinished_false.json
--rw-r--r--   0     1001      123       12 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_structure_unclosed_array_unfinished_true.json
--rw-r--r--   0     1001      123       12 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_structure_unclosed_object.json
--rw-r--r--   0     1001      123        2 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_structure_unicode-identifier.json
--rw-r--r--   0     1001      123        5 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_structure_whitespace_U+2060_word_joiner.json
--rw-r--r--   0     1001      123        3 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/n_structure_whitespace_formfeed.json
--rw-r--r--   0     1001      123        7 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_array_arraysWithSpaces.json
--rw-r--r--   0     1001      123        4 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_array_empty-string.json
--rw-r--r--   0     1001      123        2 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_array_empty.json
--rw-r--r--   0     1001      123        5 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_array_ending_with_newline.json
--rw-r--r--   0     1001      123        7 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_array_false.json
--rw-r--r--   0     1001      123       18 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_array_heterogeneous.json
--rw-r--r--   0     1001      123        6 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_array_null.json
--rw-r--r--   0     1001      123        4 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_array_with_1_and_newline.json
--rw-r--r--   0     1001      123        4 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_array_with_leading_space.json
--rw-r--r--   0     1001      123       20 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_array_with_several_null.json
--rw-r--r--   0     1001      123        4 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_array_with_trailing_space.json
--rw-r--r--   0     1001      123        8 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_number.json
--rw-r--r--   0     1001      123        6 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_number_0e+1.json
--rw-r--r--   0     1001      123        5 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_number_0e1.json
--rw-r--r--   0     1001      123        4 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_number_after_space.json
--rw-r--r--   0     1001      123       84 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_number_double_close_to_zero.json
--rw-r--r--   0     1001      123        6 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_number_int_with_exp.json
--rw-r--r--   0     1001      123        4 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_number_minus_zero.json
--rw-r--r--   0     1001      123        6 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_number_negative_int.json
--rw-r--r--   0     1001      123        4 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_number_negative_one.json
--rw-r--r--   0     1001      123        4 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_number_negative_zero.json
--rw-r--r--   0     1001      123        6 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_number_real_capital_e.json
--rw-r--r--   0     1001      123        6 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_number_real_capital_e_neg_exp.json
--rw-r--r--   0     1001      123        6 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_number_real_capital_e_pos_exp.json
--rw-r--r--   0     1001      123        8 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_number_real_exponent.json
--rw-r--r--   0     1001      123       12 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_number_real_fraction_exponent.json
--rw-r--r--   0     1001      123        6 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_number_real_neg_exp.json
--rw-r--r--   0     1001      123        6 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_number_real_pos_exponent.json
--rw-r--r--   0     1001      123        5 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_number_simple_int.json
--rw-r--r--   0     1001      123       12 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_number_simple_real.json
--rw-r--r--   0     1001      123       26 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_object.json
--rw-r--r--   0     1001      123       13 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_object_basic.json
--rw-r--r--   0     1001      123       17 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_object_duplicated_key.json
--rw-r--r--   0     1001      123       17 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_object_duplicated_key_and_value.json
--rw-r--r--   0     1001      123        2 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_object_empty.json
--rw-r--r--   0     1001      123        6 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_object_empty_key.json
--rw-r--r--   0     1001      123       20 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_object_escaped_null_in_key.json
--rw-r--r--   0     1001      123       35 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_object_extreme_numbers.json
--rw-r--r--   0     1001      123      108 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_object_long_strings.json
--rw-r--r--   0     1001      123        8 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_object_simple.json
--rw-r--r--   0     1001      123      110 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_object_string_unicode.json
--rw-r--r--   0     1001      123       12 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_object_with_newlines.json
--rw-r--r--   0     1001      123       22 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_string_1_2_3_bytes_UTF-8_sequences.json
--rw-r--r--   0     1001      123       16 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_string_accepted_surrogate_pair.json
--rw-r--r--   0     1001      123       28 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_string_accepted_surrogate_pairs.json
--rw-r--r--   0     1001      123       20 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_string_allowed_escapes.json
--rw-r--r--   0     1001      123       11 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_string_backslash_and_u_escaped_zero.json
--rw-r--r--   0     1001      123        6 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_string_backslash_doublequotes.json
--rw-r--r--   0     1001      123       17 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_string_comments.json
--rw-r--r--   0     1001      123        7 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_string_double_escape_a.json
--rw-r--r--   0     1001      123        7 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_string_double_escape_n.json
--rw-r--r--   0     1001      123       10 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_string_escaped_control_character.json
--rw-r--r--   0     1001      123       10 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_string_escaped_noncharacter.json
--rw-r--r--   0     1001      123        7 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_string_in_array.json
--rw-r--r--   0     1001      123        8 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_string_in_array_with_leading_space.json
--rw-r--r--   0     1001      123       16 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_string_last_surrogates_1_and_2.json
--rw-r--r--   0     1001      123       17 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_string_nbsp_uescaped.json
--rw-r--r--   0     1001      123        8 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_string_nonCharacterInUTF-8_U+10FFFF.json
--rw-r--r--   0     1001      123        7 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_string_nonCharacterInUTF-8_U+FFFF.json
--rw-r--r--   0     1001      123       10 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_string_null_escape.json
--rw-r--r--   0     1001      123       10 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_string_one-byte-utf-8.json
--rw-r--r--   0     1001      123        6 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_string_pi.json
--rw-r--r--   0     1001      123        8 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_string_reservedCharacterInUTF-8_U+1BFFF.json
--rw-r--r--   0     1001      123        8 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_string_simple_ascii.json
--rw-r--r--   0     1001      123        3 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_string_space.json
--rw-r--r--   0     1001      123       16 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_string_surrogates_U+1D11E_MUSICAL_SYMBOL_G_CLEF.json
--rw-r--r--   0     1001      123       10 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_string_three-byte-utf-8.json
--rw-r--r--   0     1001      123       10 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_string_two-byte-utf-8.json
--rw-r--r--   0     1001      123        7 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_string_u+2028_line_sep.json
--rw-r--r--   0     1001      123        7 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_string_u+2029_par_sep.json
--rw-r--r--   0     1001      123       28 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_string_uEscape.json
--rw-r--r--   0     1001      123       17 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_string_uescaped_newline.json
--rw-r--r--   0     1001      123        5 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_string_unescaped_char_delete.json
--rw-r--r--   0     1001      123       10 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_string_unicode.json
--rw-r--r--   0     1001      123       10 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_string_unicodeEscapedBackslash.json
--rw-r--r--   0     1001      123       13 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_string_unicode_2.json
--rw-r--r--   0     1001      123       16 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_string_unicode_U+10FFFE_nonchar.json
--rw-r--r--   0     1001      123       16 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_string_unicode_U+1FFFE_nonchar.json
--rw-r--r--   0     1001      123       10 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_string_unicode_U+200B_ZERO_WIDTH_SPACE.json
--rw-r--r--   0     1001      123       10 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_string_unicode_U+2064_invisible_plus.json
--rw-r--r--   0     1001      123       10 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_string_unicode_U+FDD0_nonchar.json
--rw-r--r--   0     1001      123       10 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_string_unicode_U+FFFE_nonchar.json
--rw-r--r--   0     1001      123       10 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_string_unicode_escaped_double_quote.json
--rw-r--r--   0     1001      123       11 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_string_utf8.json
--rw-r--r--   0     1001      123        7 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_string_with_del_character.json
--rw-r--r--   0     1001      123        5 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_structure_lonely_false.json
--rw-r--r--   0     1001      123        2 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_structure_lonely_int.json
--rw-r--r--   0     1001      123        4 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_structure_lonely_negative_real.json
--rw-r--r--   0     1001      123        4 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_structure_lonely_null.json
--rw-r--r--   0     1001      123        5 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_structure_lonely_string.json
--rw-r--r--   0     1001      123        4 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_structure_lonely_true.json
--rw-r--r--   0     1001      123        2 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_structure_string_empty.json
--rw-r--r--   0     1001      123        6 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_structure_trailing_newline.json
--rw-r--r--   0     1001      123        6 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_structure_true_in_array.json
--rw-r--r--   0     1001      123        4 2023-03-20 23:21:57.000000 orjson-3.8.8/data/parsing/y_structure_whitespace_array.json
--rw-r--r--   0     1001      123        6 2023-03-20 23:21:57.000000 orjson-3.8.8/data/roundtrip/roundtrip01.json
--rw-r--r--   0     1001      123        6 2023-03-20 23:21:57.000000 orjson-3.8.8/data/roundtrip/roundtrip02.json
--rw-r--r--   0     1001      123        7 2023-03-20 23:21:57.000000 orjson-3.8.8/data/roundtrip/roundtrip03.json
--rw-r--r--   0     1001      123        3 2023-03-20 23:21:57.000000 orjson-3.8.8/data/roundtrip/roundtrip04.json
--rw-r--r--   0     1001      123        7 2023-03-20 23:21:57.000000 orjson-3.8.8/data/roundtrip/roundtrip05.json
--rw-r--r--   0     1001      123        2 2023-03-20 23:21:57.000000 orjson-3.8.8/data/roundtrip/roundtrip06.json
--rw-r--r--   0     1001      123        2 2023-03-20 23:21:57.000000 orjson-3.8.8/data/roundtrip/roundtrip07.json
--rw-r--r--   0     1001      123        5 2023-03-20 23:21:57.000000 orjson-3.8.8/data/roundtrip/roundtrip08.json
--rw-r--r--   0     1001      123       13 2023-03-20 23:21:57.000000 orjson-3.8.8/data/roundtrip/roundtrip09.json
--rw-r--r--   0     1001      123       22 2023-03-20 23:21:57.000000 orjson-3.8.8/data/roundtrip/roundtrip10.json
--rw-r--r--   0     1001      123        4 2023-03-20 23:21:57.000000 orjson-3.8.8/data/roundtrip/roundtrip11.json
--rw-r--r--   0     1001      123       13 2023-03-20 23:21:57.000000 orjson-3.8.8/data/roundtrip/roundtrip12.json
--rw-r--r--   0     1001      123       22 2023-03-20 23:21:57.000000 orjson-3.8.8/data/roundtrip/roundtrip13.json
--rw-r--r--   0     1001      123       22 2023-03-20 23:21:57.000000 orjson-3.8.8/data/roundtrip/roundtrip14.json
--rw-r--r--   0     1001      123        3 2023-03-20 23:21:57.000000 orjson-3.8.8/data/roundtrip/roundtrip15.json
--rw-r--r--   0     1001      123       12 2023-03-20 23:21:57.000000 orjson-3.8.8/data/roundtrip/roundtrip16.json
--rw-r--r--   0     1001      123       12 2023-03-20 23:21:57.000000 orjson-3.8.8/data/roundtrip/roundtrip17.json
--rw-r--r--   0     1001      123       21 2023-03-20 23:21:57.000000 orjson-3.8.8/data/roundtrip/roundtrip18.json
--rw-r--r--   0     1001      123       21 2023-03-20 23:21:57.000000 orjson-3.8.8/data/roundtrip/roundtrip19.json
--rw-r--r--   0     1001      123        5 2023-03-20 23:21:57.000000 orjson-3.8.8/data/roundtrip/roundtrip20.json
--rw-r--r--   0     1001      123        6 2023-03-20 23:21:57.000000 orjson-3.8.8/data/roundtrip/roundtrip21.json
--rw-r--r--   0     1001      123        8 2023-03-20 23:21:57.000000 orjson-3.8.8/data/roundtrip/roundtrip22.json
--rw-r--r--   0     1001      123        9 2023-03-20 23:21:57.000000 orjson-3.8.8/data/roundtrip/roundtrip23.json
--rw-r--r--   0     1001      123        8 2023-03-20 23:21:57.000000 orjson-3.8.8/data/roundtrip/roundtrip24.json
--rw-r--r--   0     1001      123       24 2023-03-20 23:21:57.000000 orjson-3.8.8/data/roundtrip/roundtrip25.json
--rw-r--r--   0     1001      123       25 2023-03-20 23:21:57.000000 orjson-3.8.8/data/roundtrip/roundtrip26.json
--rw-r--r--   0     1001      123       24 2023-03-20 23:21:57.000000 orjson-3.8.8/data/roundtrip/roundtrip27.json
--rw-r--r--   0     1001      123        5 2023-03-20 23:21:57.000000 orjson-3.8.8/data/transform/number_1.0.json
--rw-r--r--   0     1001      123       22 2023-03-20 23:21:57.000000 orjson-3.8.8/data/transform/number_1.000000000000000005.json
--rw-r--r--   0     1001      123       19 2023-03-20 23:21:57.000000 orjson-3.8.8/data/transform/number_1000000000000000.json
--rw-r--r--   0     1001      123       22 2023-03-20 23:21:57.000000 orjson-3.8.8/data/transform/number_10000000000000000999.json
--rw-r--r--   0     1001      123        8 2023-03-20 23:21:57.000000 orjson-3.8.8/data/transform/number_1e-999.json
--rw-r--r--   0     1001      123        5 2023-03-20 23:21:57.000000 orjson-3.8.8/data/transform/number_1e6.json
--rw-r--r--   0     1001      123       24 2023-03-20 23:21:57.000000 orjson-3.8.8/data/transform/object_key_nfc_nfd.json
--rw-r--r--   0     1001      123       24 2023-03-20 23:21:57.000000 orjson-3.8.8/data/transform/object_key_nfd_nfc.json
--rw-r--r--   0     1001      123       13 2023-03-20 23:21:57.000000 orjson-3.8.8/data/transform/object_same_key_different_values.json
--rw-r--r--   0     1001      123       13 2023-03-20 23:21:57.000000 orjson-3.8.8/data/transform/object_same_key_same_value.json
--rw-r--r--   0     1001      123       16 2023-03-20 23:21:57.000000 orjson-3.8.8/data/transform/object_same_key_unclear_values.json
--rw-r--r--   0     1001      123       10 2023-03-20 23:21:57.000000 orjson-3.8.8/data/transform/string_1_escaped_invalid_codepoint.json
--rw-r--r--   0     1001      123        7 2023-03-20 23:21:57.000000 orjson-3.8.8/data/transform/string_1_invalid_codepoint.json
--rw-r--r--   0     1001      123       16 2023-03-20 23:21:57.000000 orjson-3.8.8/data/transform/string_2_escaped_invalid_codepoints.json
--rw-r--r--   0     1001      123       10 2023-03-20 23:21:57.000000 orjson-3.8.8/data/transform/string_2_invalid_codepoints.json
--rw-r--r--   0     1001      123       22 2023-03-20 23:21:57.000000 orjson-3.8.8/data/transform/string_3_escaped_invalid_codepoints.json
--rw-r--r--   0     1001      123       13 2023-03-20 23:21:57.000000 orjson-3.8.8/data/transform/string_3_invalid_codepoints.json
--rw-r--r--   0     1001      123       12 2023-03-20 23:21:57.000000 orjson-3.8.8/data/transform/string_with_escaped_NULL.json
--rw-r--r--   0     1001      123    34780 2023-03-20 23:21:57.000000 orjson-3.8.8/data/twitter.json.xz
--rw-r--r--   0     1001      123   311326 2023-03-20 23:21:57.000000 orjson-3.8.8/include/yyjson/yyjson.c
--rw-r--r--   0     1001      123   230528 2023-03-20 23:21:57.000000 orjson-3.8.8/include/yyjson/yyjson.h
--rw-r--r--   0     1001      123     1161 2023-03-20 23:21:57.000000 orjson-3.8.8/pyproject.toml
--rw-r--r--   0     1001      123     1161 2023-03-20 23:21:57.000000 orjson-3.8.8/src/deserialize/cache.rs
--rw-r--r--   0     1001      123     1017 2023-03-20 23:21:57.000000 orjson-3.8.8/src/deserialize/deserializer.rs
--rw-r--r--   0     1001      123     3101 2023-03-20 23:21:57.000000 orjson-3.8.8/src/deserialize/error.rs
--rw-r--r--   0     1001      123     3985 2023-03-20 23:21:57.000000 orjson-3.8.8/src/deserialize/json.rs
--rw-r--r--   0     1001      123      312 2023-03-20 23:21:57.000000 orjson-3.8.8/src/deserialize/mod.rs
--rw-r--r--   0     1001      123     1961 2023-03-20 23:21:57.000000 orjson-3.8.8/src/deserialize/pyobject.rs
--rw-r--r--   0     1001      123     3013 2023-03-20 23:21:57.000000 orjson-3.8.8/src/deserialize/utf8.rs
--rw-r--r--   0     1001      123     5669 2023-03-20 23:21:57.000000 orjson-3.8.8/src/deserialize/yyjson.rs
--rw-r--r--   0     1001      123      129 2023-03-20 23:21:57.000000 orjson-3.8.8/src/error.rs
--rw-r--r--   0     1001      123      727 2023-03-20 23:21:57.000000 orjson-3.8.8/src/ffi/buffer.rs
--rw-r--r--   0     1001      123      550 2023-03-20 23:21:57.000000 orjson-3.8.8/src/ffi/bytes.rs
--rw-r--r--   0     1001      123     1237 2023-03-20 23:21:57.000000 orjson-3.8.8/src/ffi/dict.rs
--rw-r--r--   0     1001      123     1016 2023-03-20 23:21:57.000000 orjson-3.8.8/src/ffi/list.rs
--rw-r--r--   0     1001      123      204 2023-03-20 23:21:57.000000 orjson-3.8.8/src/ffi/mod.rs
--rw-r--r--   0     1001      123      284 2023-03-20 23:21:57.000000 orjson-3.8.8/src/ffi/pytype.rs
--rw-r--r--   0     1001      123    12670 2023-03-20 23:21:57.000000 orjson-3.8.8/src/lib.rs
--rw-r--r--   0     1001      123     1133 2023-03-20 23:21:57.000000 orjson-3.8.8/src/opt.rs
--rw-r--r--   0     1001      123     4288 2023-03-20 23:21:57.000000 orjson-3.8.8/src/serialize/dataclass.rs
--rw-r--r--   0     1001      123     7830 2023-03-20 23:21:57.000000 orjson-3.8.8/src/serialize/datetime.rs
--rw-r--r--   0     1001      123     6045 2023-03-20 23:21:57.000000 orjson-3.8.8/src/serialize/datetimelike.rs
--rw-r--r--   0     1001      123     2082 2023-03-20 23:21:57.000000 orjson-3.8.8/src/serialize/default.rs
--rw-r--r--   0     1001      123     9941 2023-03-20 23:21:57.000000 orjson-3.8.8/src/serialize/dict.rs
--rw-r--r--   0     1001      123     2473 2023-03-20 23:21:57.000000 orjson-3.8.8/src/serialize/error.rs
--rw-r--r--   0     1001      123      544 2023-03-20 23:21:57.000000 orjson-3.8.8/src/serialize/float.rs
--rw-r--r--   0     1001      123     2640 2023-03-20 23:21:57.000000 orjson-3.8.8/src/serialize/int.rs
--rw-r--r--   0     1001      123    36189 2023-03-20 23:21:57.000000 orjson-3.8.8/src/serialize/json.rs
--rw-r--r--   0     1001      123     1543 2023-03-20 23:21:57.000000 orjson-3.8.8/src/serialize/list.rs
--rw-r--r--   0     1001      123      326 2023-03-20 23:21:57.000000 orjson-3.8.8/src/serialize/mod.rs
--rw-r--r--   0     1001      123    34798 2023-03-20 23:21:57.000000 orjson-3.8.8/src/serialize/numpy.rs
--rw-r--r--   0     1001      123     1248 2023-03-20 23:21:57.000000 orjson-3.8.8/src/serialize/pyenum.rs
--rw-r--r--   0     1001      123    10717 2023-03-20 23:21:57.000000 orjson-3.8.8/src/serialize/serializer.rs
--rw-r--r--   0     1001      123     1285 2023-03-20 23:21:57.000000 orjson-3.8.8/src/serialize/str.rs
--rw-r--r--   0     1001      123     1606 2023-03-20 23:21:57.000000 orjson-3.8.8/src/serialize/tuple.rs
--rw-r--r--   0     1001      123     1958 2023-03-20 23:21:57.000000 orjson-3.8.8/src/serialize/uuid.rs
--rw-r--r--   0     1001      123     5349 2023-03-20 23:21:57.000000 orjson-3.8.8/src/serialize/writer.rs
--rw-r--r--   0     1001      123     1053 2023-03-20 23:21:57.000000 orjson-3.8.8/src/str/check.rs
--rw-r--r--   0     1001      123     2610 2023-03-20 23:21:57.000000 orjson-3.8.8/src/str/create.rs
--rw-r--r--   0     1001      123     2723 2023-03-20 23:21:57.000000 orjson-3.8.8/src/str/ffi.rs
--rw-r--r--   0     1001      123      135 2023-03-20 23:21:57.000000 orjson-3.8.8/src/str/mod.rs
--rw-r--r--   0     1001      123    11958 2023-03-20 23:21:57.000000 orjson-3.8.8/src/typeref.rs
--rw-r--r--   0     1001      123     2574 2023-03-20 23:21:57.000000 orjson-3.8.8/src/util.rs
--rw-r--r--   0     1001      123     1884 2023-03-20 23:21:57.000000 orjson-3.8.8/src/yyjson.rs
--rw-r--r--   0     1001      123        0 2023-03-20 23:21:57.000000 orjson-3.8.8/test/__init__.py
--rw-r--r--   0     1001      123      430 2023-03-20 23:21:57.000000 orjson-3.8.8/test/requirements.txt
--rw-r--r--   0     1001      123     6205 2023-03-20 23:21:57.000000 orjson-3.8.8/test/test_api.py
--rw-r--r--   0     1001      123     1319 2023-03-20 23:21:57.000000 orjson-3.8.8/test/test_append_newline.py
--rw-r--r--   0     1001      123      680 2023-03-20 23:21:57.000000 orjson-3.8.8/test/test_canonical.py
--rw-r--r--   0     1001      123      857 2023-03-20 23:21:57.000000 orjson-3.8.8/test/test_circular.py
--rw-r--r--   0     1001      123     7288 2023-03-20 23:21:57.000000 orjson-3.8.8/test/test_dataclass.py
--rw-r--r--   0     1001      123    22769 2023-03-20 23:21:57.000000 orjson-3.8.8/test/test_datetime.py
--rw-r--r--   0     1001      123     6758 2023-03-20 23:21:57.000000 orjson-3.8.8/test/test_default.py
--rw-r--r--   0     1001      123     1926 2023-03-20 23:21:57.000000 orjson-3.8.8/test/test_dict.py
--rw-r--r--   0     1001      123     2630 2023-03-20 23:21:57.000000 orjson-3.8.8/test/test_enum.py
--rw-r--r--   0     1001      123     2254 2023-03-20 23:21:57.000000 orjson-3.8.8/test/test_error.py
--rw-r--r--   0     1001      123     1492 2023-03-20 23:21:57.000000 orjson-3.8.8/test/test_fixture.py
--rw-r--r--   0     1001      123     2496 2023-03-20 23:21:57.000000 orjson-3.8.8/test/test_indent.py
--rw-r--r--   0     1001      123      274 2023-03-20 23:21:57.000000 orjson-3.8.8/test/test_issue221.py
--rw-r--r--   0     1001      123    11816 2023-03-20 23:21:57.000000 orjson-3.8.8/test/test_issue331.py
--rw-r--r--   0     1001      123     6187 2023-03-20 23:21:57.000000 orjson-3.8.8/test/test_jsonchecker.py
--rw-r--r--   0     1001      123     7135 2023-03-20 23:21:57.000000 orjson-3.8.8/test/test_memory.py
--rw-r--r--   0     1001      123     9175 2023-03-20 23:21:57.000000 orjson-3.8.8/test/test_non_str_keys.py
--rw-r--r--   0     1001      123    26610 2023-03-20 23:21:57.000000 orjson-3.8.8/test/test_numpy.py
--rw-r--r--   0     1001      123    57008 2023-03-20 23:21:57.000000 orjson-3.8.8/test/test_parsing.py
--rw-r--r--   0     1001      123     3994 2023-03-20 23:21:57.000000 orjson-3.8.8/test/test_roundtrip.py
--rw-r--r--   0     1001      123     1656 2023-03-20 23:21:57.000000 orjson-3.8.8/test/test_sort_keys.py
--rw-r--r--   0     1001      123     3126 2023-03-20 23:21:57.000000 orjson-3.8.8/test/test_subclass.py
--rw-r--r--   0     1001      123     3725 2023-03-20 23:21:57.000000 orjson-3.8.8/test/test_transform.py
--rw-r--r--   0     1001      123    16264 2023-03-20 23:21:57.000000 orjson-3.8.8/test/test_type.py
--rw-r--r--   0     1001      123      437 2023-03-20 23:21:57.000000 orjson-3.8.8/test/test_typeddict.py
--rw-r--r--   0     1001      123    10773 2023-03-20 23:21:57.000000 orjson-3.8.8/test/test_ujson.py
--rw-r--r--   0     1001      123     3445 2023-03-20 23:21:57.000000 orjson-3.8.8/test/test_uuid.py
--rw-r--r--   0     1001      123      948 2023-03-20 23:21:57.000000 orjson-3.8.8/test/util.py
--rw-r--r--   0     1001      123     7067 2023-03-20 23:21:57.000000 orjson-3.8.8/Cargo.lock
--rw-r--r--   0     1001      123      705 2023-03-20 23:21:57.000000 orjson-3.8.8/pysrc/orjson/__init__.pyi
--rw-r--r--   0     1001      123      573 2023-03-20 23:21:57.000000 orjson-3.8.8/pysrc/orjson/__init__.py
--rw-r--r--   0     1001      123        0 2023-03-20 23:21:57.000000 orjson-3.8.8/pysrc/orjson/py.typed
--rw-r--r--   0        0        0    47778 1970-01-01 00:00:00.000000 orjson-3.8.8/PKG-INFO
+-rw-r--r--   0        0        0     2560 1970-01-01 00:00:00.000000 orjson-3.8.9/Cargo.toml
+-rw-r--r--   0     1001      123    16551 2023-03-28 15:16:49.000000 orjson-3.8.9/CHANGELOG.md
+-rw-r--r--   0     1001      123    10847 2023-03-28 15:16:49.000000 orjson-3.8.9/LICENSE-APACHE
+-rw-r--r--   0     1001      123     1023 2023-03-28 15:16:49.000000 orjson-3.8.9/LICENSE-MIT
+-rw-r--r--   0     1001      123    46350 2023-03-28 15:16:49.000000 orjson-3.8.9/README.md
+-rw-r--r--   0     1001      123     8780 2023-03-28 15:16:49.000000 orjson-3.8.9/data/blns.txt.xz
+-rw-r--r--   0     1001      123   376512 2023-03-28 15:16:49.000000 orjson-3.8.9/data/canada.json.xz
+-rw-r--r--   0     1001      123    12336 2023-03-28 15:16:49.000000 orjson-3.8.9/data/citm_catalog.json.xz
+-rw-r--r--   0     1001      123     8264 2023-03-28 15:16:49.000000 orjson-3.8.9/data/github.json.xz
+-rw-r--r--   0     1001      123      592 2023-03-28 15:16:49.000000 orjson-3.8.9/data/issue331_1.json.xz
+-rw-r--r--   0     1001      123      592 2023-03-28 15:16:49.000000 orjson-3.8.9/data/issue331_2.json.xz
+-rw-r--r--   0     1001      123       60 2023-03-28 15:16:49.000000 orjson-3.8.9/data/jsonchecker/fail01.json
+-rw-r--r--   0     1001      123       17 2023-03-28 15:16:49.000000 orjson-3.8.9/data/jsonchecker/fail02.json
+-rw-r--r--   0     1001      123       37 2023-03-28 15:16:49.000000 orjson-3.8.9/data/jsonchecker/fail03.json
+-rw-r--r--   0     1001      123       16 2023-03-28 15:16:49.000000 orjson-3.8.9/data/jsonchecker/fail04.json
+-rw-r--r--   0     1001      123       24 2023-03-28 15:16:49.000000 orjson-3.8.9/data/jsonchecker/fail05.json
+-rw-r--r--   0     1001      123       26 2023-03-28 15:16:49.000000 orjson-3.8.9/data/jsonchecker/fail06.json
+-rw-r--r--   0     1001      123       26 2023-03-28 15:16:49.000000 orjson-3.8.9/data/jsonchecker/fail07.json
+-rw-r--r--   0     1001      123       16 2023-03-28 15:16:49.000000 orjson-3.8.9/data/jsonchecker/fail08.json
+-rw-r--r--   0     1001      123       22 2023-03-28 15:16:49.000000 orjson-3.8.9/data/jsonchecker/fail09.json
+-rw-r--r--   0     1001      123       58 2023-03-28 15:16:49.000000 orjson-3.8.9/data/jsonchecker/fail10.json
+-rw-r--r--   0     1001      123       29 2023-03-28 15:16:49.000000 orjson-3.8.9/data/jsonchecker/fail11.json
+-rw-r--r--   0     1001      123       31 2023-03-28 15:16:49.000000 orjson-3.8.9/data/jsonchecker/fail12.json
+-rw-r--r--   0     1001      123       43 2023-03-28 15:16:49.000000 orjson-3.8.9/data/jsonchecker/fail13.json
+-rw-r--r--   0     1001      123       31 2023-03-28 15:16:49.000000 orjson-3.8.9/data/jsonchecker/fail14.json
+-rw-r--r--   0     1001      123       34 2023-03-28 15:16:49.000000 orjson-3.8.9/data/jsonchecker/fail15.json
+-rw-r--r--   0     1001      123        8 2023-03-28 15:16:49.000000 orjson-3.8.9/data/jsonchecker/fail16.json
+-rw-r--r--   0     1001      123       34 2023-03-28 15:16:49.000000 orjson-3.8.9/data/jsonchecker/fail17.json
+-rw-r--r--   0     1001      123       50 2023-03-28 15:16:49.000000 orjson-3.8.9/data/jsonchecker/fail18.json
+-rw-r--r--   0     1001      123       22 2023-03-28 15:16:49.000000 orjson-3.8.9/data/jsonchecker/fail19.json
+-rw-r--r--   0     1001      123       23 2023-03-28 15:16:49.000000 orjson-3.8.9/data/jsonchecker/fail20.json
+-rw-r--r--   0     1001      123       32 2023-03-28 15:16:49.000000 orjson-3.8.9/data/jsonchecker/fail21.json
+-rw-r--r--   0     1001      123       33 2023-03-28 15:16:49.000000 orjson-3.8.9/data/jsonchecker/fail22.json
+-rw-r--r--   0     1001      123       20 2023-03-28 15:16:49.000000 orjson-3.8.9/data/jsonchecker/fail23.json
+-rw-r--r--   0     1001      123       16 2023-03-28 15:16:49.000000 orjson-3.8.9/data/jsonchecker/fail24.json
+-rw-r--r--   0     1001      123       29 2023-03-28 15:16:49.000000 orjson-3.8.9/data/jsonchecker/fail25.json
+-rw-r--r--   0     1001      123       38 2023-03-28 15:16:49.000000 orjson-3.8.9/data/jsonchecker/fail26.json
+-rw-r--r--   0     1001      123       14 2023-03-28 15:16:49.000000 orjson-3.8.9/data/jsonchecker/fail27.json
+-rw-r--r--   0     1001      123       15 2023-03-28 15:16:49.000000 orjson-3.8.9/data/jsonchecker/fail28.json
+-rw-r--r--   0     1001      123        4 2023-03-28 15:16:49.000000 orjson-3.8.9/data/jsonchecker/fail29.json
+-rw-r--r--   0     1001      123        5 2023-03-28 15:16:49.000000 orjson-3.8.9/data/jsonchecker/fail30.json
+-rw-r--r--   0     1001      123        7 2023-03-28 15:16:49.000000 orjson-3.8.9/data/jsonchecker/fail31.json
+-rw-r--r--   0     1001      123       40 2023-03-28 15:16:49.000000 orjson-3.8.9/data/jsonchecker/fail32.json
+-rw-r--r--   0     1001      123       12 2023-03-28 15:16:49.000000 orjson-3.8.9/data/jsonchecker/fail33.json
+-rw-r--r--   0     1001      123     1441 2023-03-28 15:16:49.000000 orjson-3.8.9/data/jsonchecker/pass01.json
+-rw-r--r--   0     1001      123       52 2023-03-28 15:16:49.000000 orjson-3.8.9/data/jsonchecker/pass02.json
+-rw-r--r--   0     1001      123      148 2023-03-28 15:16:49.000000 orjson-3.8.9/data/jsonchecker/pass03.json
+-rw-r--r--   0     1001      123       14 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/i_number_double_huge_neg_exp.json
+-rw-r--r--   0     1001      123      137 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/i_number_huge_exp.json
+-rw-r--r--   0     1001      123       10 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/i_number_neg_int_huge_exp.json
+-rw-r--r--   0     1001      123       11 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/i_number_pos_double_huge_exp.json
+-rw-r--r--   0     1001      123       16 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/i_number_real_neg_overflow.json
+-rw-r--r--   0     1001      123       15 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/i_number_real_pos_overflow.json
+-rw-r--r--   0     1001      123       15 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/i_number_real_underflow.json
+-rw-r--r--   0     1001      123       33 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/i_number_too_big_neg_int.json
+-rw-r--r--   0     1001      123       23 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/i_number_too_big_pos_int.json
+-rw-r--r--   0     1001      123       51 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/i_number_very_big_negative_int.json
+-rw-r--r--   0     1001      123       12 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/i_object_key_lone_2nd_surrogate.json
+-rw-r--r--   0     1001      123       10 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/i_string_1st_surrogate_but_2nd_missing.json
+-rw-r--r--   0     1001      123       16 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/i_string_1st_valid_surrogate_2nd_invalid.json
+-rw-r--r--   0     1001      123       12 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/i_string_UTF-16LE_with_BOM.json
+-rw-r--r--   0     1001      123       10 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/i_string_UTF-8_invalid_sequence.json
+-rw-r--r--   0     1001      123        7 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/i_string_UTF8_surrogate_U+D800.json
+-rw-r--r--   0     1001      123       12 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/i_string_incomplete_surrogate_and_escape_valid.json
+-rw-r--r--   0     1001      123       11 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/i_string_incomplete_surrogate_pair.json
+-rw-r--r--   0     1001      123       18 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/i_string_incomplete_surrogates_escape_valid.json
+-rw-r--r--   0     1001      123       10 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/i_string_invalid_lonely_surrogate.json
+-rw-r--r--   0     1001      123       13 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/i_string_invalid_surrogate.json
+-rw-r--r--   0     1001      123        5 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/i_string_invalid_utf-8.json
+-rw-r--r--   0     1001      123       16 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/i_string_inverted_surrogates_U+1D11E.json
+-rw-r--r--   0     1001      123        5 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/i_string_iso_latin_1.json
+-rw-r--r--   0     1001      123       10 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/i_string_lone_second_surrogate.json
+-rw-r--r--   0     1001      123        5 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/i_string_lone_utf8_continuation_byte.json
+-rw-r--r--   0     1001      123        8 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/i_string_not_in_unicode_range.json
+-rw-r--r--   0     1001      123        6 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/i_string_overlong_sequence_2_bytes.json
+-rw-r--r--   0     1001      123       10 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/i_string_overlong_sequence_6_bytes.json
+-rw-r--r--   0     1001      123       10 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/i_string_overlong_sequence_6_bytes_null.json
+-rw-r--r--   0     1001      123        6 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/i_string_truncated-utf-8.json
+-rw-r--r--   0     1001      123       10 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/i_string_utf16BE_no_BOM.json
+-rw-r--r--   0     1001      123       10 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/i_string_utf16LE_no_BOM.json
+-rw-r--r--   0     1001      123       80 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/i_structure_500_nested_arrays.json.xz
+-rw-r--r--   0     1001      123        5 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/i_structure_UTF-8_BOM_empty_object.json
+-rw-r--r--   0     1001      123        8 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_array_1_true_without_comma.json
+-rw-r--r--   0     1001      123        4 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_array_a_invalid_utf8.json
+-rw-r--r--   0     1001      123        7 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_array_colon_instead_of_comma.json
+-rw-r--r--   0     1001      123        5 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_array_comma_after_close.json
+-rw-r--r--   0     1001      123        4 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_array_comma_and_number.json
+-rw-r--r--   0     1001      123        6 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_array_double_comma.json
+-rw-r--r--   0     1001      123        7 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_array_double_extra_comma.json
+-rw-r--r--   0     1001      123        6 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_array_extra_close.json
+-rw-r--r--   0     1001      123        5 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_array_extra_comma.json
+-rw-r--r--   0     1001      123        4 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_array_incomplete.json
+-rw-r--r--   0     1001      123        2 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_array_incomplete_invalid_value.json
+-rw-r--r--   0     1001      123        6 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_array_inner_array_no_comma.json
+-rw-r--r--   0     1001      123        3 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_array_invalid_utf8.json
+-rw-r--r--   0     1001      123        5 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_array_items_separated_by_semicolon.json
+-rw-r--r--   0     1001      123        3 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_array_just_comma.json
+-rw-r--r--   0     1001      123        3 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_array_just_minus.json
+-rw-r--r--   0     1001      123        9 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_array_missing_value.json
+-rw-r--r--   0     1001      123       11 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_array_newlines_unclosed.json
+-rw-r--r--   0     1001      123        4 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_array_number_and_comma.json
+-rw-r--r--   0     1001      123        5 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_array_number_and_several_commas.json
+-rw-r--r--   0     1001      123        8 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_array_spaces_vertical_tab_formfeed.json
+-rw-r--r--   0     1001      123        3 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_array_star_inside.json
+-rw-r--r--   0     1001      123        3 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_array_unclosed.json
+-rw-r--r--   0     1001      123        3 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_array_unclosed_trailing_comma.json
+-rw-r--r--   0     1001      123        8 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_array_unclosed_with_new_lines.json
+-rw-r--r--   0     1001      123        3 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_array_unclosed_with_object_inside.json
+-rw-r--r--   0     1001      123        6 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_incomplete_false.json
+-rw-r--r--   0     1001      123        5 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_incomplete_null.json
+-rw-r--r--   0     1001      123        5 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_incomplete_true.json
+-rw-r--r--   0     1001      123        4 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_multidigit_number_then_00.json
+-rw-r--r--   0     1001      123        8 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_number_++.json
+-rw-r--r--   0     1001      123        4 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_number_+1.json
+-rw-r--r--   0     1001      123        6 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_number_+Inf.json
+-rw-r--r--   0     1001      123        5 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_number_-01.json
+-rw-r--r--   0     1001      123        7 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_number_-1.0..json
+-rw-r--r--   0     1001      123        5 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_number_-2..json
+-rw-r--r--   0     1001      123        6 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_number_-NaN.json
+-rw-r--r--   0     1001      123        5 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_number_.-1.json
+-rw-r--r--   0     1001      123        7 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_number_.2e-3.json
+-rw-r--r--   0     1001      123        7 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_number_0.1.2.json
+-rw-r--r--   0     1001      123        7 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_number_0.3e+.json
+-rw-r--r--   0     1001      123        6 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_number_0.3e.json
+-rw-r--r--   0     1001      123        6 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_number_0.e1.json
+-rw-r--r--   0     1001      123        5 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_number_0_capital_E+.json
+-rw-r--r--   0     1001      123        4 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_number_0_capital_E.json
+-rw-r--r--   0     1001      123        5 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_number_0e+.json
+-rw-r--r--   0     1001      123        4 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_number_0e.json
+-rw-r--r--   0     1001      123        7 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_number_1.0e+.json
+-rw-r--r--   0     1001      123        7 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_number_1.0e-.json
+-rw-r--r--   0     1001      123        6 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_number_1.0e.json
+-rw-r--r--   0     1001      123        9 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_number_1_000.json
+-rw-r--r--   0     1001      123        6 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_number_1eE2.json
+-rw-r--r--   0     1001      123        7 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_number_2.e+3.json
+-rw-r--r--   0     1001      123        7 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_number_2.e-3.json
+-rw-r--r--   0     1001      123        6 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_number_2.e3.json
+-rw-r--r--   0     1001      123        6 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_number_9.e+.json
+-rw-r--r--   0     1001      123        5 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_number_Inf.json
+-rw-r--r--   0     1001      123        5 2023-03-28 15:16:49.000000 orjson-3.8.9/data/parsing/n_number_NaN.json
+-rw-r--r--   0     1001      123        5 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_number_U+FF11_fullwidth_digit_one.json
+-rw-r--r--   0     1001      123        5 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_number_expression.json
+-rw-r--r--   0     1001      123        5 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_number_hex_1_digit.json
+-rw-r--r--   0     1001      123        6 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_number_hex_2_digits.json
+-rw-r--r--   0     1001      123       10 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_number_infinity.json
+-rw-r--r--   0     1001      123        7 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_number_invalid+-.json
+-rw-r--r--   0     1001      123       13 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_number_invalid-negative-real.json
+-rw-r--r--   0     1001      123        6 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_number_invalid-utf-8-in-bigger-int.json
+-rw-r--r--   0     1001      123        6 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_number_invalid-utf-8-in-exponent.json
+-rw-r--r--   0     1001      123        5 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_number_invalid-utf-8-in-int.json
+-rw-r--r--   0     1001      123       11 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_number_minus_infinity.json
+-rw-r--r--   0     1001      123        6 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_number_minus_sign_with_trailing_garbage.json
+-rw-r--r--   0     1001      123        5 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_number_minus_space_1.json
+-rw-r--r--   0     1001      123        6 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_number_neg_int_starting_with_zero.json
+-rw-r--r--   0     1001      123        7 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_number_neg_real_without_int_part.json
+-rw-r--r--   0     1001      123        5 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_number_neg_with_garbage_at_end.json
+-rw-r--r--   0     1001      123        5 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_number_real_garbage_after_e.json
+-rw-r--r--   0     1001      123        5 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_number_real_with_invalid_utf8_after_e.json
+-rw-r--r--   0     1001      123        4 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_number_real_without_fractional_part.json
+-rw-r--r--   0     1001      123        6 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_number_starting_with_dot.json
+-rw-r--r--   0     1001      123        8 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_number_with_alpha.json
+-rw-r--r--   0     1001      123       25 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_number_with_alpha_char.json
+-rw-r--r--   0     1001      123        5 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_number_with_leading_zero.json
+-rw-r--r--   0     1001      123       12 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_object_bad_value.json
+-rw-r--r--   0     1001      123        9 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_object_bracket_key.json
+-rw-r--r--   0     1001      123       11 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_object_comma_instead_of_colon.json
+-rw-r--r--   0     1001      123       10 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_object_double_colon.json
+-rw-r--r--   0     1001      123       10 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_object_emoji.json
+-rw-r--r--   0     1001      123       13 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_object_garbage_at_end.json
+-rw-r--r--   0     1001      123       14 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_object_key_with_single_quotes.json
+-rw-r--r--   0     1001      123       10 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_object_lone_continuation_byte_in_key_and_trailing_comma.json
+-rw-r--r--   0     1001      123        7 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_object_missing_colon.json
+-rw-r--r--   0     1001      123        6 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_object_missing_key.json
+-rw-r--r--   0     1001      123        9 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_object_missing_semicolon.json
+-rw-r--r--   0     1001      123        5 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_object_missing_value.json
+-rw-r--r--   0     1001      123        4 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_object_no-colon.json
+-rw-r--r--   0     1001      123        5 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_object_non_string_key.json
+-rw-r--r--   0     1001      123       13 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_object_non_string_key_but_huge_number_instead.json
+-rw-r--r--   0     1001      123       21 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_object_repeated_null_null.json
+-rw-r--r--   0     1001      123       13 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_object_several_trailing_commas.json
+-rw-r--r--   0     1001      123        7 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_object_single_quote.json
+-rw-r--r--   0     1001      123        9 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_object_trailing_comma.json
+-rw-r--r--   0     1001      123       13 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_object_trailing_comment.json
+-rw-r--r--   0     1001      123       14 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_object_trailing_comment_open.json
+-rw-r--r--   0     1001      123       11 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_object_trailing_comment_slash_open.json
+-rw-r--r--   0     1001      123       10 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_object_trailing_comment_slash_open_incomplete.json
+-rw-r--r--   0     1001      123       18 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_object_two_commas_in_a_row.json
+-rw-r--r--   0     1001      123        8 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_object_unquoted_key.json
+-rw-r--r--   0     1001      123        7 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_object_unterminated-value.json
+-rw-r--r--   0     1001      123       22 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_object_with_single_string.json
+-rw-r--r--   0     1001      123       10 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_object_with_trailing_garbage.json
+-rw-r--r--   0     1001      123        1 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_single_space.json
+-rw-r--r--   0     1001      123       11 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_string_1_surrogate_then_escape.json
+-rw-r--r--   0     1001      123       12 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_string_1_surrogate_then_escape_u.json
+-rw-r--r--   0     1001      123       13 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_string_1_surrogate_then_escape_u1.json
+-rw-r--r--   0     1001      123       14 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_string_1_surrogate_then_escape_u1x.json
+-rw-r--r--   0     1001      123        4 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_string_accentuated_char_no_quotes.json
+-rw-r--r--   0     1001      123        6 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_string_backslash_00.json
+-rw-r--r--   0     1001      123        8 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_string_escape_x.json
+-rw-r--r--   0     1001      123        7 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_string_escaped_backslash_bad.json
+-rw-r--r--   0     1001      123        6 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_string_escaped_ctrl_char_tab.json
+-rw-r--r--   0     1001      123        9 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_string_escaped_emoji.json
+-rw-r--r--   0     1001      123        5 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_string_incomplete_escape.json
+-rw-r--r--   0     1001      123        9 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_string_incomplete_escaped_character.json
+-rw-r--r--   0     1001      123       14 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_string_incomplete_surrogate.json
+-rw-r--r--   0     1001      123       18 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_string_incomplete_surrogate_escape_invalid.json
+-rw-r--r--   0     1001      123        7 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_string_invalid-utf-8-in-escape.json
+-rw-r--r--   0     1001      123        6 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_string_invalid_backslash_esc.json
+-rw-r--r--   0     1001      123       10 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_string_invalid_unicode_escape.json
+-rw-r--r--   0     1001      123        6 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_string_invalid_utf8_after_escape.json
+-rw-r--r--   0     1001      123       13 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_string_leading_uescaped_thinspace.json
+-rw-r--r--   0     1001      123        4 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_string_no_quotes_with_bad_escape.json
+-rw-r--r--   0     1001      123        1 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_string_single_doublequote.json
+-rw-r--r--   0     1001      123       16 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_string_single_quote.json
+-rw-r--r--   0     1001      123        3 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_string_single_string_no_double_quotes.json
+-rw-r--r--   0     1001      123        3 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_string_start_escape_unclosed.json
+-rw-r--r--   0     1001      123        7 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_string_unescaped_crtl_char.json
+-rw-r--r--   0     1001      123       12 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_string_unescaped_newline.json
+-rw-r--r--   0     1001      123        5 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_string_unescaped_tab.json
+-rw-r--r--   0     1001      123        8 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_string_unicode_CapitalU.json
+-rw-r--r--   0     1001      123        3 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_string_with_trailing_garbage.json
+-rw-r--r--   0     1001      123      148 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_structure_100000_opening_arrays.json.xz
+-rw-r--r--   0     1001      123        5 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_structure_U+2060_word_joined.json
+-rw-r--r--   0     1001      123        3 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_structure_UTF8_BOM_no_data.json
+-rw-r--r--   0     1001      123        3 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_structure_angle_bracket_..json
+-rw-r--r--   0     1001      123        8 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_structure_angle_bracket_null.json
+-rw-r--r--   0     1001      123        4 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_structure_array_trailing_garbage.json
+-rw-r--r--   0     1001      123        4 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_structure_array_with_extra_array_close.json
+-rw-r--r--   0     1001      123        6 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_structure_array_with_unclosed_string.json
+-rw-r--r--   0     1001      123        3 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_structure_ascii-unicode-identifier.json
+-rw-r--r--   0     1001      123        6 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_structure_capitalized_True.json
+-rw-r--r--   0     1001      123        2 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_structure_close_unopened_array.json
+-rw-r--r--   0     1001      123       11 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_structure_comma_instead_of_closing_brace.json
+-rw-r--r--   0     1001      123        4 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_structure_double_array.json
+-rw-r--r--   0     1001      123        1 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_structure_end_array.json
+-rw-r--r--   0     1001      123        4 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_structure_incomplete_UTF8_BOM.json
+-rw-r--r--   0     1001      123        1 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_structure_lone-invalid-utf-8.json
+-rw-r--r--   0     1001      123        1 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_structure_lone-open-bracket.json
+-rw-r--r--   0     1001      123        0 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_structure_no_data.json
+-rw-r--r--   0     1001      123        3 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_structure_null-byte-outside-string.json
+-rw-r--r--   0     1001      123        2 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_structure_number_with_trailing_garbage.json
+-rw-r--r--   0     1001      123        3 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_structure_object_followed_by_closing_object.json
+-rw-r--r--   0     1001      123        4 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_structure_object_unclosed_no_value.json
+-rw-r--r--   0     1001      123       20 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_structure_object_with_comment.json
+-rw-r--r--   0     1001      123       15 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_structure_object_with_trailing_garbage.json
+-rw-r--r--   0     1001      123        2 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_structure_open_array_apostrophe.json
+-rw-r--r--   0     1001      123        2 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_structure_open_array_comma.json
+-rw-r--r--   0     1001      123      176 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_structure_open_array_object.json.xz
+-rw-r--r--   0     1001      123        2 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_structure_open_array_open_object.json
+-rw-r--r--   0     1001      123        3 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_structure_open_array_open_string.json
+-rw-r--r--   0     1001      123        4 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_structure_open_array_string.json
+-rw-r--r--   0     1001      123        1 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_structure_open_object.json
+-rw-r--r--   0     1001      123        2 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_structure_open_object_close_array.json
+-rw-r--r--   0     1001      123        2 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_structure_open_object_comma.json
+-rw-r--r--   0     1001      123        2 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_structure_open_object_open_array.json
+-rw-r--r--   0     1001      123        3 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_structure_open_object_open_string.json
+-rw-r--r--   0     1001      123        4 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_structure_open_object_string_with_apostrophes.json
+-rw-r--r--   0     1001      123       16 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_structure_open_open.json
+-rw-r--r--   0     1001      123        1 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_structure_single_eacute.json
+-rw-r--r--   0     1001      123        1 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_structure_single_star.json
+-rw-r--r--   0     1001      123       12 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_structure_trailing_#.json
+-rw-r--r--   0     1001      123       10 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_structure_uescaped_LF_before_string.json
+-rw-r--r--   0     1001      123        2 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_structure_unclosed_array.json
+-rw-r--r--   0     1001      123       12 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_structure_unclosed_array_partial_null.json
+-rw-r--r--   0     1001      123       12 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_structure_unclosed_array_unfinished_false.json
+-rw-r--r--   0     1001      123       12 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_structure_unclosed_array_unfinished_true.json
+-rw-r--r--   0     1001      123       12 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_structure_unclosed_object.json
+-rw-r--r--   0     1001      123        2 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_structure_unicode-identifier.json
+-rw-r--r--   0     1001      123        5 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_structure_whitespace_U+2060_word_joiner.json
+-rw-r--r--   0     1001      123        3 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/n_structure_whitespace_formfeed.json
+-rw-r--r--   0     1001      123        7 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_array_arraysWithSpaces.json
+-rw-r--r--   0     1001      123        4 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_array_empty-string.json
+-rw-r--r--   0     1001      123        2 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_array_empty.json
+-rw-r--r--   0     1001      123        5 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_array_ending_with_newline.json
+-rw-r--r--   0     1001      123        7 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_array_false.json
+-rw-r--r--   0     1001      123       18 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_array_heterogeneous.json
+-rw-r--r--   0     1001      123        6 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_array_null.json
+-rw-r--r--   0     1001      123        4 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_array_with_1_and_newline.json
+-rw-r--r--   0     1001      123        4 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_array_with_leading_space.json
+-rw-r--r--   0     1001      123       20 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_array_with_several_null.json
+-rw-r--r--   0     1001      123        4 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_array_with_trailing_space.json
+-rw-r--r--   0     1001      123        8 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_number.json
+-rw-r--r--   0     1001      123        6 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_number_0e+1.json
+-rw-r--r--   0     1001      123        5 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_number_0e1.json
+-rw-r--r--   0     1001      123        4 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_number_after_space.json
+-rw-r--r--   0     1001      123       84 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_number_double_close_to_zero.json
+-rw-r--r--   0     1001      123        6 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_number_int_with_exp.json
+-rw-r--r--   0     1001      123        4 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_number_minus_zero.json
+-rw-r--r--   0     1001      123        6 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_number_negative_int.json
+-rw-r--r--   0     1001      123        4 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_number_negative_one.json
+-rw-r--r--   0     1001      123        4 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_number_negative_zero.json
+-rw-r--r--   0     1001      123        6 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_number_real_capital_e.json
+-rw-r--r--   0     1001      123        6 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_number_real_capital_e_neg_exp.json
+-rw-r--r--   0     1001      123        6 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_number_real_capital_e_pos_exp.json
+-rw-r--r--   0     1001      123        8 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_number_real_exponent.json
+-rw-r--r--   0     1001      123       12 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_number_real_fraction_exponent.json
+-rw-r--r--   0     1001      123        6 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_number_real_neg_exp.json
+-rw-r--r--   0     1001      123        6 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_number_real_pos_exponent.json
+-rw-r--r--   0     1001      123        5 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_number_simple_int.json
+-rw-r--r--   0     1001      123       12 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_number_simple_real.json
+-rw-r--r--   0     1001      123       26 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_object.json
+-rw-r--r--   0     1001      123       13 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_object_basic.json
+-rw-r--r--   0     1001      123       17 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_object_duplicated_key.json
+-rw-r--r--   0     1001      123       17 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_object_duplicated_key_and_value.json
+-rw-r--r--   0     1001      123        2 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_object_empty.json
+-rw-r--r--   0     1001      123        6 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_object_empty_key.json
+-rw-r--r--   0     1001      123       20 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_object_escaped_null_in_key.json
+-rw-r--r--   0     1001      123       35 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_object_extreme_numbers.json
+-rw-r--r--   0     1001      123      108 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_object_long_strings.json
+-rw-r--r--   0     1001      123        8 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_object_simple.json
+-rw-r--r--   0     1001      123      110 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_object_string_unicode.json
+-rw-r--r--   0     1001      123       12 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_object_with_newlines.json
+-rw-r--r--   0     1001      123       22 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_string_1_2_3_bytes_UTF-8_sequences.json
+-rw-r--r--   0     1001      123       16 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_string_accepted_surrogate_pair.json
+-rw-r--r--   0     1001      123       28 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_string_accepted_surrogate_pairs.json
+-rw-r--r--   0     1001      123       20 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_string_allowed_escapes.json
+-rw-r--r--   0     1001      123       11 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_string_backslash_and_u_escaped_zero.json
+-rw-r--r--   0     1001      123        6 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_string_backslash_doublequotes.json
+-rw-r--r--   0     1001      123       17 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_string_comments.json
+-rw-r--r--   0     1001      123        7 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_string_double_escape_a.json
+-rw-r--r--   0     1001      123        7 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_string_double_escape_n.json
+-rw-r--r--   0     1001      123       10 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_string_escaped_control_character.json
+-rw-r--r--   0     1001      123       10 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_string_escaped_noncharacter.json
+-rw-r--r--   0     1001      123        7 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_string_in_array.json
+-rw-r--r--   0     1001      123        8 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_string_in_array_with_leading_space.json
+-rw-r--r--   0     1001      123       16 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_string_last_surrogates_1_and_2.json
+-rw-r--r--   0     1001      123       17 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_string_nbsp_uescaped.json
+-rw-r--r--   0     1001      123        8 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_string_nonCharacterInUTF-8_U+10FFFF.json
+-rw-r--r--   0     1001      123        7 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_string_nonCharacterInUTF-8_U+FFFF.json
+-rw-r--r--   0     1001      123       10 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_string_null_escape.json
+-rw-r--r--   0     1001      123       10 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_string_one-byte-utf-8.json
+-rw-r--r--   0     1001      123        6 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_string_pi.json
+-rw-r--r--   0     1001      123        8 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_string_reservedCharacterInUTF-8_U+1BFFF.json
+-rw-r--r--   0     1001      123        8 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_string_simple_ascii.json
+-rw-r--r--   0     1001      123        3 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_string_space.json
+-rw-r--r--   0     1001      123       16 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_string_surrogates_U+1D11E_MUSICAL_SYMBOL_G_CLEF.json
+-rw-r--r--   0     1001      123       10 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_string_three-byte-utf-8.json
+-rw-r--r--   0     1001      123       10 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_string_two-byte-utf-8.json
+-rw-r--r--   0     1001      123        7 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_string_u+2028_line_sep.json
+-rw-r--r--   0     1001      123        7 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_string_u+2029_par_sep.json
+-rw-r--r--   0     1001      123       28 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_string_uEscape.json
+-rw-r--r--   0     1001      123       17 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_string_uescaped_newline.json
+-rw-r--r--   0     1001      123        5 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_string_unescaped_char_delete.json
+-rw-r--r--   0     1001      123       10 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_string_unicode.json
+-rw-r--r--   0     1001      123       10 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_string_unicodeEscapedBackslash.json
+-rw-r--r--   0     1001      123       13 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_string_unicode_2.json
+-rw-r--r--   0     1001      123       16 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_string_unicode_U+10FFFE_nonchar.json
+-rw-r--r--   0     1001      123       16 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_string_unicode_U+1FFFE_nonchar.json
+-rw-r--r--   0     1001      123       10 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_string_unicode_U+200B_ZERO_WIDTH_SPACE.json
+-rw-r--r--   0     1001      123       10 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_string_unicode_U+2064_invisible_plus.json
+-rw-r--r--   0     1001      123       10 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_string_unicode_U+FDD0_nonchar.json
+-rw-r--r--   0     1001      123       10 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_string_unicode_U+FFFE_nonchar.json
+-rw-r--r--   0     1001      123       10 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_string_unicode_escaped_double_quote.json
+-rw-r--r--   0     1001      123       11 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_string_utf8.json
+-rw-r--r--   0     1001      123        7 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_string_with_del_character.json
+-rw-r--r--   0     1001      123        5 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_structure_lonely_false.json
+-rw-r--r--   0     1001      123        2 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_structure_lonely_int.json
+-rw-r--r--   0     1001      123        4 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_structure_lonely_negative_real.json
+-rw-r--r--   0     1001      123        4 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_structure_lonely_null.json
+-rw-r--r--   0     1001      123        5 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_structure_lonely_string.json
+-rw-r--r--   0     1001      123        4 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_structure_lonely_true.json
+-rw-r--r--   0     1001      123        2 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_structure_string_empty.json
+-rw-r--r--   0     1001      123        6 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_structure_trailing_newline.json
+-rw-r--r--   0     1001      123        6 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_structure_true_in_array.json
+-rw-r--r--   0     1001      123        4 2023-03-28 15:16:50.000000 orjson-3.8.9/data/parsing/y_structure_whitespace_array.json
+-rw-r--r--   0     1001      123        6 2023-03-28 15:16:50.000000 orjson-3.8.9/data/roundtrip/roundtrip01.json
+-rw-r--r--   0     1001      123        6 2023-03-28 15:16:50.000000 orjson-3.8.9/data/roundtrip/roundtrip02.json
+-rw-r--r--   0     1001      123        7 2023-03-28 15:16:50.000000 orjson-3.8.9/data/roundtrip/roundtrip03.json
+-rw-r--r--   0     1001      123        3 2023-03-28 15:16:50.000000 orjson-3.8.9/data/roundtrip/roundtrip04.json
+-rw-r--r--   0     1001      123        7 2023-03-28 15:16:50.000000 orjson-3.8.9/data/roundtrip/roundtrip05.json
+-rw-r--r--   0     1001      123        2 2023-03-28 15:16:50.000000 orjson-3.8.9/data/roundtrip/roundtrip06.json
+-rw-r--r--   0     1001      123        2 2023-03-28 15:16:50.000000 orjson-3.8.9/data/roundtrip/roundtrip07.json
+-rw-r--r--   0     1001      123        5 2023-03-28 15:16:50.000000 orjson-3.8.9/data/roundtrip/roundtrip08.json
+-rw-r--r--   0     1001      123       13 2023-03-28 15:16:50.000000 orjson-3.8.9/data/roundtrip/roundtrip09.json
+-rw-r--r--   0     1001      123       22 2023-03-28 15:16:50.000000 orjson-3.8.9/data/roundtrip/roundtrip10.json
+-rw-r--r--   0     1001      123        4 2023-03-28 15:16:50.000000 orjson-3.8.9/data/roundtrip/roundtrip11.json
+-rw-r--r--   0     1001      123       13 2023-03-28 15:16:50.000000 orjson-3.8.9/data/roundtrip/roundtrip12.json
+-rw-r--r--   0     1001      123       22 2023-03-28 15:16:50.000000 orjson-3.8.9/data/roundtrip/roundtrip13.json
+-rw-r--r--   0     1001      123       22 2023-03-28 15:16:50.000000 orjson-3.8.9/data/roundtrip/roundtrip14.json
+-rw-r--r--   0     1001      123        3 2023-03-28 15:16:50.000000 orjson-3.8.9/data/roundtrip/roundtrip15.json
+-rw-r--r--   0     1001      123       12 2023-03-28 15:16:50.000000 orjson-3.8.9/data/roundtrip/roundtrip16.json
+-rw-r--r--   0     1001      123       12 2023-03-28 15:16:50.000000 orjson-3.8.9/data/roundtrip/roundtrip17.json
+-rw-r--r--   0     1001      123       21 2023-03-28 15:16:50.000000 orjson-3.8.9/data/roundtrip/roundtrip18.json
+-rw-r--r--   0     1001      123       21 2023-03-28 15:16:50.000000 orjson-3.8.9/data/roundtrip/roundtrip19.json
+-rw-r--r--   0     1001      123        5 2023-03-28 15:16:50.000000 orjson-3.8.9/data/roundtrip/roundtrip20.json
+-rw-r--r--   0     1001      123        6 2023-03-28 15:16:50.000000 orjson-3.8.9/data/roundtrip/roundtrip21.json
+-rw-r--r--   0     1001      123        8 2023-03-28 15:16:50.000000 orjson-3.8.9/data/roundtrip/roundtrip22.json
+-rw-r--r--   0     1001      123        9 2023-03-28 15:16:50.000000 orjson-3.8.9/data/roundtrip/roundtrip23.json
+-rw-r--r--   0     1001      123        8 2023-03-28 15:16:50.000000 orjson-3.8.9/data/roundtrip/roundtrip24.json
+-rw-r--r--   0     1001      123       24 2023-03-28 15:16:50.000000 orjson-3.8.9/data/roundtrip/roundtrip25.json
+-rw-r--r--   0     1001      123       25 2023-03-28 15:16:50.000000 orjson-3.8.9/data/roundtrip/roundtrip26.json
+-rw-r--r--   0     1001      123       24 2023-03-28 15:16:50.000000 orjson-3.8.9/data/roundtrip/roundtrip27.json
+-rw-r--r--   0     1001      123        5 2023-03-28 15:16:50.000000 orjson-3.8.9/data/transform/number_1.0.json
+-rw-r--r--   0     1001      123       22 2023-03-28 15:16:50.000000 orjson-3.8.9/data/transform/number_1.000000000000000005.json
+-rw-r--r--   0     1001      123       19 2023-03-28 15:16:50.000000 orjson-3.8.9/data/transform/number_1000000000000000.json
+-rw-r--r--   0     1001      123       22 2023-03-28 15:16:50.000000 orjson-3.8.9/data/transform/number_10000000000000000999.json
+-rw-r--r--   0     1001      123        8 2023-03-28 15:16:50.000000 orjson-3.8.9/data/transform/number_1e-999.json
+-rw-r--r--   0     1001      123        5 2023-03-28 15:16:50.000000 orjson-3.8.9/data/transform/number_1e6.json
+-rw-r--r--   0     1001      123       24 2023-03-28 15:16:50.000000 orjson-3.8.9/data/transform/object_key_nfc_nfd.json
+-rw-r--r--   0     1001      123       24 2023-03-28 15:16:50.000000 orjson-3.8.9/data/transform/object_key_nfd_nfc.json
+-rw-r--r--   0     1001      123       13 2023-03-28 15:16:50.000000 orjson-3.8.9/data/transform/object_same_key_different_values.json
+-rw-r--r--   0     1001      123       13 2023-03-28 15:16:50.000000 orjson-3.8.9/data/transform/object_same_key_same_value.json
+-rw-r--r--   0     1001      123       16 2023-03-28 15:16:50.000000 orjson-3.8.9/data/transform/object_same_key_unclear_values.json
+-rw-r--r--   0     1001      123       10 2023-03-28 15:16:50.000000 orjson-3.8.9/data/transform/string_1_escaped_invalid_codepoint.json
+-rw-r--r--   0     1001      123        7 2023-03-28 15:16:50.000000 orjson-3.8.9/data/transform/string_1_invalid_codepoint.json
+-rw-r--r--   0     1001      123       16 2023-03-28 15:16:50.000000 orjson-3.8.9/data/transform/string_2_escaped_invalid_codepoints.json
+-rw-r--r--   0     1001      123       10 2023-03-28 15:16:50.000000 orjson-3.8.9/data/transform/string_2_invalid_codepoints.json
+-rw-r--r--   0     1001      123       22 2023-03-28 15:16:50.000000 orjson-3.8.9/data/transform/string_3_escaped_invalid_codepoints.json
+-rw-r--r--   0     1001      123       13 2023-03-28 15:16:50.000000 orjson-3.8.9/data/transform/string_3_invalid_codepoints.json
+-rw-r--r--   0     1001      123       12 2023-03-28 15:16:50.000000 orjson-3.8.9/data/transform/string_with_escaped_NULL.json
+-rw-r--r--   0     1001      123    34780 2023-03-28 15:16:50.000000 orjson-3.8.9/data/twitter.json.xz
+-rw-r--r--   0     1001      123   311326 2023-03-28 15:16:50.000000 orjson-3.8.9/include/yyjson/yyjson.c
+-rw-r--r--   0     1001      123   230528 2023-03-28 15:16:50.000000 orjson-3.8.9/include/yyjson/yyjson.h
+-rw-r--r--   0     1001      123     1161 2023-03-28 15:16:50.000000 orjson-3.8.9/pyproject.toml
+-rw-r--r--   0     1001      123     1182 2023-03-28 15:16:50.000000 orjson-3.8.9/src/deserialize/cache.rs
+-rw-r--r--   0     1001      123     1017 2023-03-28 15:16:50.000000 orjson-3.8.9/src/deserialize/deserializer.rs
+-rw-r--r--   0     1001      123     3101 2023-03-28 15:16:50.000000 orjson-3.8.9/src/deserialize/error.rs
+-rw-r--r--   0     1001      123     3985 2023-03-28 15:16:50.000000 orjson-3.8.9/src/deserialize/json.rs
+-rw-r--r--   0     1001      123      312 2023-03-28 15:16:50.000000 orjson-3.8.9/src/deserialize/mod.rs
+-rw-r--r--   0     1001      123     1961 2023-03-28 15:16:50.000000 orjson-3.8.9/src/deserialize/pyobject.rs
+-rw-r--r--   0     1001      123     3013 2023-03-28 15:16:50.000000 orjson-3.8.9/src/deserialize/utf8.rs
+-rw-r--r--   0     1001      123     5690 2023-03-28 15:16:50.000000 orjson-3.8.9/src/deserialize/yyjson.rs
+-rw-r--r--   0     1001      123      129 2023-03-28 15:16:50.000000 orjson-3.8.9/src/error.rs
+-rw-r--r--   0     1001      123      727 2023-03-28 15:16:50.000000 orjson-3.8.9/src/ffi/buffer.rs
+-rw-r--r--   0     1001      123      550 2023-03-28 15:16:50.000000 orjson-3.8.9/src/ffi/bytes.rs
+-rw-r--r--   0     1001      123     1237 2023-03-28 15:16:50.000000 orjson-3.8.9/src/ffi/dict.rs
+-rw-r--r--   0     1001      123     1016 2023-03-28 15:16:50.000000 orjson-3.8.9/src/ffi/list.rs
+-rw-r--r--   0     1001      123      204 2023-03-28 15:16:50.000000 orjson-3.8.9/src/ffi/mod.rs
+-rw-r--r--   0     1001      123      284 2023-03-28 15:16:50.000000 orjson-3.8.9/src/ffi/pytype.rs
+-rw-r--r--   0     1001      123    12670 2023-03-28 15:16:50.000000 orjson-3.8.9/src/lib.rs
+-rw-r--r--   0     1001      123     1133 2023-03-28 15:16:50.000000 orjson-3.8.9/src/opt.rs
+-rw-r--r--   0     1001      123     4310 2023-03-28 15:16:50.000000 orjson-3.8.9/src/serialize/dataclass.rs
+-rw-r--r--   0     1001      123     7830 2023-03-28 15:16:50.000000 orjson-3.8.9/src/serialize/datetime.rs
+-rw-r--r--   0     1001      123     6045 2023-03-28 15:16:50.000000 orjson-3.8.9/src/serialize/datetimelike.rs
+-rw-r--r--   0     1001      123     2082 2023-03-28 15:16:50.000000 orjson-3.8.9/src/serialize/default.rs
+-rw-r--r--   0     1001      123     9941 2023-03-28 15:16:50.000000 orjson-3.8.9/src/serialize/dict.rs
+-rw-r--r--   0     1001      123     2473 2023-03-28 15:16:50.000000 orjson-3.8.9/src/serialize/error.rs
+-rw-r--r--   0     1001      123      544 2023-03-28 15:16:50.000000 orjson-3.8.9/src/serialize/float.rs
+-rw-r--r--   0     1001      123     2640 2023-03-28 15:16:50.000000 orjson-3.8.9/src/serialize/int.rs
+-rw-r--r--   0     1001      123    36189 2023-03-28 15:16:50.000000 orjson-3.8.9/src/serialize/json.rs
+-rw-r--r--   0     1001      123     1543 2023-03-28 15:16:50.000000 orjson-3.8.9/src/serialize/list.rs
+-rw-r--r--   0     1001      123      326 2023-03-28 15:16:50.000000 orjson-3.8.9/src/serialize/mod.rs
+-rw-r--r--   0     1001      123    35019 2023-03-28 15:16:50.000000 orjson-3.8.9/src/serialize/numpy.rs
+-rw-r--r--   0     1001      123     1248 2023-03-28 15:16:50.000000 orjson-3.8.9/src/serialize/pyenum.rs
+-rw-r--r--   0     1001      123    10717 2023-03-28 15:16:50.000000 orjson-3.8.9/src/serialize/serializer.rs
+-rw-r--r--   0     1001      123     1285 2023-03-28 15:16:50.000000 orjson-3.8.9/src/serialize/str.rs
+-rw-r--r--   0     1001      123     1606 2023-03-28 15:16:50.000000 orjson-3.8.9/src/serialize/tuple.rs
+-rw-r--r--   0     1001      123     1958 2023-03-28 15:16:50.000000 orjson-3.8.9/src/serialize/uuid.rs
+-rw-r--r--   0     1001      123     5349 2023-03-28 15:16:50.000000 orjson-3.8.9/src/serialize/writer.rs
+-rw-r--r--   0     1001      123     1053 2023-03-28 15:16:50.000000 orjson-3.8.9/src/str/check.rs
+-rw-r--r--   0     1001      123     2610 2023-03-28 15:16:50.000000 orjson-3.8.9/src/str/create.rs
+-rw-r--r--   0     1001      123     2723 2023-03-28 15:16:50.000000 orjson-3.8.9/src/str/ffi.rs
+-rw-r--r--   0     1001      123      135 2023-03-28 15:16:50.000000 orjson-3.8.9/src/str/mod.rs
+-rw-r--r--   0     1001      123    12361 2023-03-28 15:16:50.000000 orjson-3.8.9/src/typeref.rs
+-rw-r--r--   0     1001      123     2574 2023-03-28 15:16:50.000000 orjson-3.8.9/src/util.rs
+-rw-r--r--   0     1001      123     1884 2023-03-28 15:16:50.000000 orjson-3.8.9/src/yyjson.rs
+-rw-r--r--   0     1001      123        0 2023-03-28 15:16:50.000000 orjson-3.8.9/test/__init__.py
+-rw-r--r--   0     1001      123      430 2023-03-28 15:16:50.000000 orjson-3.8.9/test/requirements.txt
+-rw-r--r--   0     1001      123     6205 2023-03-28 15:16:50.000000 orjson-3.8.9/test/test_api.py
+-rw-r--r--   0     1001      123     1319 2023-03-28 15:16:50.000000 orjson-3.8.9/test/test_append_newline.py
+-rw-r--r--   0     1001      123      680 2023-03-28 15:16:50.000000 orjson-3.8.9/test/test_canonical.py
+-rw-r--r--   0     1001      123      857 2023-03-28 15:16:50.000000 orjson-3.8.9/test/test_circular.py
+-rw-r--r--   0     1001      123     7288 2023-03-28 15:16:50.000000 orjson-3.8.9/test/test_dataclass.py
+-rw-r--r--   0     1001      123    22769 2023-03-28 15:16:50.000000 orjson-3.8.9/test/test_datetime.py
+-rw-r--r--   0     1001      123     6758 2023-03-28 15:16:50.000000 orjson-3.8.9/test/test_default.py
+-rw-r--r--   0     1001      123     1926 2023-03-28 15:16:50.000000 orjson-3.8.9/test/test_dict.py
+-rw-r--r--   0     1001      123     2630 2023-03-28 15:16:50.000000 orjson-3.8.9/test/test_enum.py
+-rw-r--r--   0     1001      123     2254 2023-03-28 15:16:50.000000 orjson-3.8.9/test/test_error.py
+-rw-r--r--   0     1001      123     1492 2023-03-28 15:16:50.000000 orjson-3.8.9/test/test_fixture.py
+-rw-r--r--   0     1001      123     2496 2023-03-28 15:16:50.000000 orjson-3.8.9/test/test_indent.py
+-rw-r--r--   0     1001      123      274 2023-03-28 15:16:50.000000 orjson-3.8.9/test/test_issue221.py
+-rw-r--r--   0     1001      123    11816 2023-03-28 15:16:50.000000 orjson-3.8.9/test/test_issue331.py
+-rw-r--r--   0     1001      123     6187 2023-03-28 15:16:50.000000 orjson-3.8.9/test/test_jsonchecker.py
+-rw-r--r--   0     1001      123     7135 2023-03-28 15:16:50.000000 orjson-3.8.9/test/test_memory.py
+-rw-r--r--   0     1001      123     9175 2023-03-28 15:16:50.000000 orjson-3.8.9/test/test_non_str_keys.py
+-rw-r--r--   0     1001      123    26610 2023-03-28 15:16:50.000000 orjson-3.8.9/test/test_numpy.py
+-rw-r--r--   0     1001      123    57008 2023-03-28 15:16:50.000000 orjson-3.8.9/test/test_parsing.py
+-rw-r--r--   0     1001      123     3994 2023-03-28 15:16:50.000000 orjson-3.8.9/test/test_roundtrip.py
+-rw-r--r--   0     1001      123     1656 2023-03-28 15:16:50.000000 orjson-3.8.9/test/test_sort_keys.py
+-rw-r--r--   0     1001      123     3126 2023-03-28 15:16:50.000000 orjson-3.8.9/test/test_subclass.py
+-rw-r--r--   0     1001      123     3725 2023-03-28 15:16:50.000000 orjson-3.8.9/test/test_transform.py
+-rw-r--r--   0     1001      123    16264 2023-03-28 15:16:50.000000 orjson-3.8.9/test/test_type.py
+-rw-r--r--   0     1001      123      437 2023-03-28 15:16:50.000000 orjson-3.8.9/test/test_typeddict.py
+-rw-r--r--   0     1001      123    10773 2023-03-28 15:16:50.000000 orjson-3.8.9/test/test_ujson.py
+-rw-r--r--   0     1001      123     3445 2023-03-28 15:16:50.000000 orjson-3.8.9/test/test_uuid.py
+-rw-r--r--   0     1001      123      948 2023-03-28 15:16:50.000000 orjson-3.8.9/test/util.py
+-rw-r--r--   0     1001      123     7067 2023-03-28 15:16:49.000000 orjson-3.8.9/Cargo.lock
+-rw-r--r--   0     1001      123      705 2023-03-28 15:16:50.000000 orjson-3.8.9/pysrc/orjson/__init__.pyi
+-rw-r--r--   0     1001      123      573 2023-03-28 15:16:50.000000 orjson-3.8.9/pysrc/orjson/__init__.py
+-rw-r--r--   0     1001      123        0 2023-03-28 15:16:50.000000 orjson-3.8.9/pysrc/orjson/py.typed
+-rw-r--r--   0        0        0    47778 1970-01-01 00:00:00.000000 orjson-3.8.9/PKG-INFO
```

### Comparing `orjson-3.8.8/Cargo.toml` & `orjson-3.8.9/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "orjson"
-version = "3.8.8"
+version = "3.8.9"
 authors = ["ijl <ijl@mailbox.org>"]
 description = "Fast, correct Python JSON library supporting dataclasses, datetimes, and numpy"
 edition = "2021"
 resolver = "2"
 rust-version = "1.60"
 license = "Apache-2.0 OR MIT"
 repository = "https://github.com/ijl/orjson"
```

### Comparing `orjson-3.8.8/CHANGELOG.md` & `orjson-3.8.9/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Changelog
 
+## 3.8.9 - 2023-03-28
+
+### Fixed
+
+- Fix parallel initialization of orjson.
+
 ## 3.8.8 - 2023-03-20
 
 ### Changed
 
 - Publish ppc64le wheels.
 
 ## 3.8.7 - 2023-02-28
```

### Comparing `orjson-3.8.8/LICENSE-APACHE` & `orjson-3.8.9/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/LICENSE-MIT` & `orjson-3.8.9/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/README.md` & `orjson-3.8.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1161,15 +1161,15 @@
 maturin build --release --strip
 ```
 
 It benefits from also having a C build environment to compile a faster
 deserialization backend. See this project's `manylinux_2_28` builds for an
 example using clang and LTO.
 
-The project's own CI tests against `nightly-2023-03-20` and stable 1.60. It
+The project's own CI tests against `nightly-2023-03-28` and stable 1.60. It
 is prudent to pin the nightly version because that channel can introduce
 breaking changes.
 
 orjson is tested for amd64, aarch64, arm7, and ppc64le on Linux. It is tested for
 amd64 on macOS and cross-compiles for aarch64. For Windows it is tested on
 amd64.
```

### Comparing `orjson-3.8.8/data/blns.txt.xz` & `orjson-3.8.9/data/blns.txt.xz`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/data/canada.json.xz` & `orjson-3.8.9/data/canada.json.xz`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/data/citm_catalog.json.xz` & `orjson-3.8.9/data/citm_catalog.json.xz`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/data/github.json.xz` & `orjson-3.8.9/data/github.json.xz`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/data/issue331_1.json.xz` & `orjson-3.8.9/data/issue331_1.json.xz`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/data/issue331_2.json.xz` & `orjson-3.8.9/data/issue331_2.json.xz`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/data/jsonchecker/pass01.json` & `orjson-3.8.9/data/jsonchecker/pass01.json`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/data/twitter.json.xz` & `orjson-3.8.9/data/twitter.json.xz`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/include/yyjson/yyjson.c` & `orjson-3.8.9/include/yyjson/yyjson.c`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/include/yyjson/yyjson.h` & `orjson-3.8.9/include/yyjson/yyjson.h`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/pyproject.toml` & `orjson-3.8.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/src/deserialize/cache.rs` & `orjson-3.8.9/src/deserialize/cache.rs`

 * *Files 8% similar despite different names*

```diff
@@ -38,11 +38,11 @@
 
 pub type KeyMap =
     AssociativeCache<u64, CachedKey, Capacity1024, HashDirectMapped, RoundRobinReplacement>;
 
 pub static mut KEY_MAP: OnceCell<KeyMap> = OnceCell::new();
 
 pub fn cache_hash(key: &[u8]) -> u64 {
-    let mut hasher = unsafe { (*HASH_BUILDER).build_hasher() };
+    let mut hasher = unsafe { HASH_BUILDER.get_or_init(ahash_init).build_hasher() };
     hasher.write(key);
     hasher.finish()
 }
```

### Comparing `orjson-3.8.8/src/deserialize/deserializer.rs` & `orjson-3.8.9/src/deserialize/deserializer.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/src/deserialize/error.rs` & `orjson-3.8.9/src/deserialize/error.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/src/deserialize/json.rs` & `orjson-3.8.9/src/deserialize/json.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/src/deserialize/pyobject.rs` & `orjson-3.8.9/src/deserialize/pyobject.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/src/deserialize/utf8.rs` & `orjson-3.8.9/src/deserialize/utf8.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/src/deserialize/yyjson.rs` & `orjson-3.8.9/src/deserialize/yyjson.rs`

 * *Files 6% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 }
 
 pub fn deserialize_yyjson(
     data: &'static str,
 ) -> Result<NonNull<pyo3_ffi::PyObject>, DeserializeError<'static>> {
     unsafe {
         let allocator = if yyjson_read_max_memory_usage(data.len()) < YYJSON_BUFFER_SIZE {
-            std::ptr::addr_of_mut!(*YYJSON_ALLOC)
+            YYJSON_ALLOC.get_or_init(yyjson_init) as *const yyjson_alc
         } else {
             null_mut()
         };
         let mut err = yyjson_read_err {
             code: YYJSON_READ_SUCCESS,
             msg: null(),
             pos: 0,
```

### Comparing `orjson-3.8.8/src/ffi/buffer.rs` & `orjson-3.8.9/src/ffi/buffer.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/src/ffi/bytes.rs` & `orjson-3.8.9/src/ffi/bytes.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/src/ffi/dict.rs` & `orjson-3.8.9/src/ffi/dict.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/src/ffi/list.rs` & `orjson-3.8.9/src/ffi/list.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/src/lib.rs` & `orjson-3.8.9/src/lib.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/src/opt.rs` & `orjson-3.8.9/src/opt.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/src/serialize/dataclass.rs` & `orjson-3.8.9/src/serialize/dataclass.rs`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         if unlikely!(len == 0) {
             return serializer.serialize_map(Some(0)).unwrap().end();
         }
         let mut map = serializer.serialize_map(None).unwrap();
         for (attr, field) in PyDictIter::from_pyobject(fields) {
             let field_type = ffi!(PyObject_GetAttr(field, FIELD_TYPE_STR));
             ffi!(Py_DECREF(field_type));
-            if unsafe { field_type != FIELD_TYPE.as_ptr() } {
+            if unsafe { field_type as *mut pyo3_ffi::PyTypeObject != FIELD_TYPE } {
                 continue;
             }
             let data = unicode_to_str(attr);
             if unlikely!(data.is_none()) {
                 err!(SerializeError::InvalidStr);
             }
             let key_as_str = data.unwrap();
```

### Comparing `orjson-3.8.8/src/serialize/datetime.rs` & `orjson-3.8.9/src/serialize/datetime.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/src/serialize/datetimelike.rs` & `orjson-3.8.9/src/serialize/datetimelike.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/src/serialize/default.rs` & `orjson-3.8.9/src/serialize/default.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/src/serialize/dict.rs` & `orjson-3.8.9/src/serialize/dict.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/src/serialize/error.rs` & `orjson-3.8.9/src/serialize/error.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/src/serialize/float.rs` & `orjson-3.8.9/src/serialize/float.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/src/serialize/int.rs` & `orjson-3.8.9/src/serialize/int.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/src/serialize/json.rs` & `orjson-3.8.9/src/serialize/json.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/src/serialize/list.rs` & `orjson-3.8.9/src/serialize/list.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/src/serialize/numpy.rs` & `orjson-3.8.9/src/serialize/numpy.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 use crate::opt::*;
 use crate::serialize::datetimelike::{DateTimeBuffer, DateTimeError, DateTimeLike, Offset};
 use crate::serialize::default::*;
 use crate::serialize::error::*;
-use crate::typeref::{ARRAY_STRUCT_STR, DESCR_STR, DTYPE_STR, NUMPY_TYPES};
+use crate::typeref::{load_numpy_types, ARRAY_STRUCT_STR, DESCR_STR, DTYPE_STR, NUMPY_TYPES};
 use chrono::{Datelike, NaiveDate, NaiveDateTime, Timelike};
 use pyo3_ffi::*;
 use serde::ser::{self, Serialize, SerializeSeq, Serializer};
 use std::convert::TryInto;
 use std::fmt;
-use std::ops::DerefMut;
 use std::os::raw::{c_char, c_int, c_void};
 use std::ptr::NonNull;
 
 pub struct NumpySerializer {
     ptr: *mut pyo3_ffi::PyObject,
     opts: Opt,
     default_calls: u8,
@@ -73,18 +72,19 @@
 macro_rules! slice {
     ($ptr:expr, $size:expr) => {
         unsafe { std::slice::from_raw_parts($ptr, $size) }
     };
 }
 
 pub fn is_numpy_scalar(ob_type: *mut PyTypeObject) -> bool {
-    if unsafe { NUMPY_TYPES.is_none() } {
+    let numpy_types = unsafe { NUMPY_TYPES.get_or_init(load_numpy_types) };
+    if numpy_types.is_none() {
         false
     } else {
-        let scalar_types = unsafe { NUMPY_TYPES.as_ref().unwrap() };
+        let scalar_types = unsafe { numpy_types.unwrap().as_ref() };
         ob_type == scalar_types.float64
             || ob_type == scalar_types.float32
             || ob_type == scalar_types.int64
             || ob_type == scalar_types.int16
             || ob_type == scalar_types.int32
             || ob_type == scalar_types.int8
             || ob_type == scalar_types.uint64
@@ -93,18 +93,20 @@
             || ob_type == scalar_types.uint16
             || ob_type == scalar_types.bool_
             || ob_type == scalar_types.datetime64
     }
 }
 
 pub fn is_numpy_array(ob_type: *mut PyTypeObject) -> bool {
-    if unsafe { NUMPY_TYPES.is_none() } {
+    let numpy_types = unsafe { NUMPY_TYPES.get_or_init(load_numpy_types) };
+    if numpy_types.is_none() {
         false
     } else {
-        unsafe { ob_type == NUMPY_TYPES.as_ref().unwrap().array }
+        let scalar_types = unsafe { numpy_types.unwrap().as_ref() };
+        unsafe { ob_type == scalar_types.array }
     }
 }
 
 #[repr(C)]
 pub struct PyCapsule {
     pub ob_refcnt: Py_ssize_t,
     pub ob_type: *mut PyTypeObject,
@@ -802,15 +804,16 @@
     #[inline(never)]
     fn serialize<S>(&self, serializer: S) -> Result<S::Ok, S::Error>
     where
         S: Serializer,
     {
         unsafe {
             let ob_type = ob_type!(self.ptr);
-            let scalar_types = NUMPY_TYPES.deref_mut().as_ref().unwrap();
+            let scalar_types =
+                unsafe { NUMPY_TYPES.get_or_init(load_numpy_types).unwrap().as_ref() };
             if ob_type == scalar_types.float64 {
                 (*(self.ptr as *mut NumpyFloat64)).serialize(serializer)
             } else if ob_type == scalar_types.float32 {
                 (*(self.ptr as *mut NumpyFloat32)).serialize(serializer)
             } else if ob_type == scalar_types.int64 {
                 (*(self.ptr as *mut NumpyInt64)).serialize(serializer)
             } else if ob_type == scalar_types.int32 {
```

### Comparing `orjson-3.8.8/src/serialize/pyenum.rs` & `orjson-3.8.9/src/serialize/pyenum.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/src/serialize/serializer.rs` & `orjson-3.8.9/src/serialize/serializer.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/src/serialize/str.rs` & `orjson-3.8.9/src/serialize/str.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/src/serialize/tuple.rs` & `orjson-3.8.9/src/serialize/tuple.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/src/serialize/uuid.rs` & `orjson-3.8.9/src/serialize/uuid.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/src/serialize/writer.rs` & `orjson-3.8.9/src/serialize/writer.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/src/str/check.rs` & `orjson-3.8.9/src/str/check.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/src/str/create.rs` & `orjson-3.8.9/src/str/create.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/src/str/ffi.rs` & `orjson-3.8.9/src/str/ffi.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/src/typeref.rs` & `orjson-3.8.9/src/typeref.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 // SPDX-License-Identifier: (Apache-2.0 OR MIT)
 
 use ahash::RandomState;
-use once_cell::unsync::Lazy;
+use once_cell::race::OnceBox;
 use pyo3_ffi::*;
 use std::os::raw::c_char;
 use std::ptr::{null_mut, NonNull};
 use std::sync::Once;
 
 pub struct NumpyTypes {
     pub array: *mut PyTypeObject,
@@ -43,17 +43,17 @@
 pub static mut DICT_TYPE: *mut PyTypeObject = null_mut();
 pub static mut DATETIME_TYPE: *mut PyTypeObject = null_mut();
 pub static mut DATE_TYPE: *mut PyTypeObject = null_mut();
 pub static mut TIME_TYPE: *mut PyTypeObject = null_mut();
 pub static mut TUPLE_TYPE: *mut PyTypeObject = null_mut();
 pub static mut UUID_TYPE: *mut PyTypeObject = null_mut();
 pub static mut ENUM_TYPE: *mut PyTypeObject = null_mut();
+pub static mut FIELD_TYPE: *mut PyTypeObject = null_mut();
 
-pub static mut NUMPY_TYPES: Lazy<Option<NumpyTypes>> = Lazy::new(|| unsafe { load_numpy_types() });
-pub static mut FIELD_TYPE: Lazy<NonNull<PyObject>> = Lazy::new(|| unsafe { look_up_field_type() });
+pub static mut NUMPY_TYPES: OnceBox<Option<NonNull<NumpyTypes>>> = OnceBox::new();
 
 #[cfg(Py_3_9)]
 pub static mut ZONEINFO_TYPE: *mut PyTypeObject = null_mut();
 
 pub static mut UTCOFFSET_METHOD_STR: *mut PyObject = null_mut();
 pub static mut NORMALIZE_METHOD_STR: *mut PyObject = null_mut();
 pub static mut CONVERT_METHOD_STR: *mut PyObject = null_mut();
@@ -65,44 +65,54 @@
 pub static mut FIELD_TYPE_STR: *mut PyObject = null_mut();
 pub static mut ARRAY_STRUCT_STR: *mut PyObject = null_mut();
 pub static mut DTYPE_STR: *mut PyObject = null_mut();
 pub static mut DESCR_STR: *mut PyObject = null_mut();
 pub static mut VALUE_STR: *mut PyObject = null_mut();
 pub static mut INT_ATTR_STR: *mut PyObject = null_mut();
 
-pub static mut HASH_BUILDER: Lazy<ahash::RandomState> = Lazy::new(|| unsafe {
-    RandomState::with_seeds(
-        VALUE_STR as u64,
-        DICT_TYPE as u64,
-        STR_TYPE as u64,
-        BYTES_TYPE as u64,
-    )
-});
+pub static mut HASH_BUILDER: OnceBox<ahash::RandomState> = OnceBox::new();
+
+pub fn ahash_init() -> Box<ahash::RandomState> {
+    unsafe {
+        Box::new(RandomState::with_seeds(
+            VALUE_STR as u64,
+            DICT_TYPE as u64,
+            STR_TYPE as u64,
+            BYTES_TYPE as u64,
+        ))
+    }
+}
+
 #[cfg(feature = "yyjson")]
 pub const YYJSON_BUFFER_SIZE: usize = 1024 * 1024 * 8;
 
 #[cfg(feature = "yyjson")]
-pub static mut YYJSON_ALLOC: Lazy<crate::yyjson::yyjson_alc> = Lazy::new(|| unsafe {
-    let buffer = std::alloc::alloc(std::alloc::Layout::from_size_align_unchecked(
-        YYJSON_BUFFER_SIZE,
-        64,
-    ));
-    let mut alloc = crate::yyjson::yyjson_alc {
-        malloc: None,
-        realloc: None,
-        free: None,
-        ctx: null_mut(),
-    };
-    crate::yyjson::yyjson_alc_pool_init(
-        &mut alloc,
-        buffer as *mut std::os::raw::c_void,
-        YYJSON_BUFFER_SIZE,
-    );
-    alloc
-});
+pub static mut YYJSON_ALLOC: OnceBox<crate::yyjson::yyjson_alc> = OnceBox::new();
+
+#[cfg(feature = "yyjson")]
+pub fn yyjson_init() -> Box<crate::yyjson::yyjson_alc> {
+    unsafe {
+        let buffer = std::alloc::alloc(std::alloc::Layout::from_size_align_unchecked(
+            YYJSON_BUFFER_SIZE,
+            64,
+        ));
+        let mut alloc = crate::yyjson::yyjson_alc {
+            malloc: None,
+            realloc: None,
+            free: None,
+            ctx: null_mut(),
+        };
+        crate::yyjson::yyjson_alc_pool_init(
+            &mut alloc,
+            buffer as *mut std::os::raw::c_void,
+            YYJSON_BUFFER_SIZE,
+        );
+        Box::new(alloc)
+    }
+}
 
 #[allow(non_upper_case_globals)]
 pub static mut JsonEncodeError: *mut PyObject = null_mut();
 #[allow(non_upper_case_globals)]
 pub static mut JsonDecodeError: *mut PyObject = null_mut();
 
 static INIT: Once = Once::new();
@@ -140,14 +150,15 @@
         INT_TYPE = (*PyLong_FromLongLong(0)).ob_type;
         FLOAT_TYPE = (*PyFloat_FromDouble(0.0)).ob_type;
         DATETIME_TYPE = look_up_datetime_type();
         DATE_TYPE = look_up_date_type();
         TIME_TYPE = look_up_time_type();
         UUID_TYPE = look_up_uuid_type();
         ENUM_TYPE = look_up_enum_type();
+        FIELD_TYPE = look_up_field_type();
 
         #[cfg(Py_3_9)]
         {
             ZONEINFO_TYPE = look_up_zoneinfo_type();
         }
 
         INT_ATTR_STR = PyUnicode_InternFromString("int\0".as_ptr() as *const c_char);
@@ -200,50 +211,51 @@
     Py_XDECREF(ptr);
     Py_XDECREF(mod_dict);
     ptr as *mut PyTypeObject
 }
 
 #[cold]
 #[cfg_attr(feature = "optimize", optimize(size))]
-unsafe fn load_numpy_types() -> Option<NumpyTypes> {
-    let numpy = PyImport_ImportModule("numpy\0".as_ptr() as *const c_char);
-    if numpy.is_null() {
-        PyErr_Clear();
-        return None;
+pub fn load_numpy_types() -> Box<Option<NonNull<NumpyTypes>>> {
+    unsafe {
+        let numpy = PyImport_ImportModule("numpy\0".as_ptr() as *const c_char);
+        if numpy.is_null() {
+            PyErr_Clear();
+            return Box::new(None);
+        }
+        let types = Box::new(NumpyTypes {
+            array: look_up_numpy_type(numpy, "ndarray\0"),
+            float32: look_up_numpy_type(numpy, "float32\0"),
+            float64: look_up_numpy_type(numpy, "float64\0"),
+            int8: look_up_numpy_type(numpy, "int8\0"),
+            int16: look_up_numpy_type(numpy, "int16\0"),
+            int32: look_up_numpy_type(numpy, "int32\0"),
+            int64: look_up_numpy_type(numpy, "int64\0"),
+            uint16: look_up_numpy_type(numpy, "uint16\0"),
+            uint32: look_up_numpy_type(numpy, "uint32\0"),
+            uint64: look_up_numpy_type(numpy, "uint64\0"),
+            uint8: look_up_numpy_type(numpy, "uint8\0"),
+            bool_: look_up_numpy_type(numpy, "bool_\0"),
+            datetime64: look_up_numpy_type(numpy, "datetime64\0"),
+        });
+        Py_XDECREF(numpy);
+        Box::new(Some(nonnull!(Box::<NumpyTypes>::into_raw(types))))
     }
-
-    let types = Some(NumpyTypes {
-        array: look_up_numpy_type(numpy, "ndarray\0"),
-        float32: look_up_numpy_type(numpy, "float32\0"),
-        float64: look_up_numpy_type(numpy, "float64\0"),
-        int8: look_up_numpy_type(numpy, "int8\0"),
-        int16: look_up_numpy_type(numpy, "int16\0"),
-        int32: look_up_numpy_type(numpy, "int32\0"),
-        int64: look_up_numpy_type(numpy, "int64\0"),
-        uint16: look_up_numpy_type(numpy, "uint16\0"),
-        uint32: look_up_numpy_type(numpy, "uint32\0"),
-        uint64: look_up_numpy_type(numpy, "uint64\0"),
-        uint8: look_up_numpy_type(numpy, "uint8\0"),
-        bool_: look_up_numpy_type(numpy, "bool_\0"),
-        datetime64: look_up_numpy_type(numpy, "datetime64\0"),
-    });
-    Py_XDECREF(numpy);
-    types
 }
 
 #[cold]
 #[cfg_attr(feature = "optimize", optimize(size))]
-unsafe fn look_up_field_type() -> NonNull<PyObject> {
+unsafe fn look_up_field_type() -> *mut PyTypeObject {
     let module = PyImport_ImportModule("dataclasses\0".as_ptr() as *const c_char);
     let module_dict = PyObject_GenericGetDict(module, null_mut());
     let ptr = PyMapping_GetItemString(module_dict, "_FIELD\0".as_ptr() as *const c_char)
         as *mut PyTypeObject;
     Py_DECREF(module_dict);
     Py_DECREF(module);
-    NonNull::new_unchecked(ptr as *mut PyObject)
+    ptr
 }
 
 #[cold]
 #[cfg_attr(feature = "optimize", optimize(size))]
 unsafe fn look_up_enum_type() -> *mut PyTypeObject {
     let module = PyImport_ImportModule("enum\0".as_ptr() as *const c_char);
     let module_dict = PyObject_GenericGetDict(module, null_mut());
```

### Comparing `orjson-3.8.8/src/util.rs` & `orjson-3.8.9/src/util.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/src/yyjson.rs` & `orjson-3.8.9/src/yyjson.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/test/test_api.py` & `orjson-3.8.9/test/test_api.py`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/test/test_append_newline.py` & `orjson-3.8.9/test/test_append_newline.py`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/test/test_canonical.py` & `orjson-3.8.9/test/test_canonical.py`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/test/test_circular.py` & `orjson-3.8.9/test/test_circular.py`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/test/test_dataclass.py` & `orjson-3.8.9/test/test_dataclass.py`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/test/test_datetime.py` & `orjson-3.8.9/test/test_datetime.py`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/test/test_default.py` & `orjson-3.8.9/test/test_default.py`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/test/test_dict.py` & `orjson-3.8.9/test/test_dict.py`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/test/test_enum.py` & `orjson-3.8.9/test/test_enum.py`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/test/test_error.py` & `orjson-3.8.9/test/test_error.py`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/test/test_fixture.py` & `orjson-3.8.9/test/test_fixture.py`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/test/test_indent.py` & `orjson-3.8.9/test/test_indent.py`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/test/test_issue331.py` & `orjson-3.8.9/test/test_issue331.py`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/test/test_jsonchecker.py` & `orjson-3.8.9/test/test_jsonchecker.py`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/test/test_memory.py` & `orjson-3.8.9/test/test_memory.py`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/test/test_non_str_keys.py` & `orjson-3.8.9/test/test_non_str_keys.py`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/test/test_numpy.py` & `orjson-3.8.9/test/test_numpy.py`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/test/test_parsing.py` & `orjson-3.8.9/test/test_parsing.py`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/test/test_roundtrip.py` & `orjson-3.8.9/test/test_roundtrip.py`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/test/test_sort_keys.py` & `orjson-3.8.9/test/test_sort_keys.py`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/test/test_subclass.py` & `orjson-3.8.9/test/test_subclass.py`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/test/test_transform.py` & `orjson-3.8.9/test/test_transform.py`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/test/test_type.py` & `orjson-3.8.9/test/test_type.py`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/test/test_ujson.py` & `orjson-3.8.9/test/test_ujson.py`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/test/test_uuid.py` & `orjson-3.8.9/test/test_uuid.py`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/test/util.py` & `orjson-3.8.9/test/util.py`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/Cargo.lock` & `orjson-3.8.9/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -154,15 +154,15 @@
 name = "once_cell"
 version = "1.17.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
 
 [[package]]
 name = "orjson"
-version = "3.8.8"
+version = "3.8.9"
 dependencies = [
  "ahash",
  "arrayvec",
  "associative-cache",
  "beef",
  "bytecount",
  "cc",
@@ -190,27 +190,27 @@
 dependencies = [
  "cfg-if",
  "libm",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.1"
+version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75439f995d07ddfad42b192dfcf3bc66a7ecfd8b4a1f5f6f046aa5c2c5d7677d"
+checksum = "98a42e7f42e917ce6664c832d5eee481ad514c98250c49e0b03b20593e2c7ed0"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.1"
+version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "839526a5c07a17ff44823679b68add4a58004de00512a95b6c1c98a6dcac0ee5"
+checksum = "a0707f0ab26826fe4ccd59b69106e9df5e12d097457c7b8f9c0fd1d2743eec4d"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "rustversion"
@@ -222,23 +222,23 @@
 name = "ryu"
 version = "1.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
 
 [[package]]
 name = "serde"
-version = "1.0.158"
+version = "1.0.159"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "771d4d9c4163ee138805e12c710dd365e4f44be8be0503cb1bb9eb989425d9c9"
+checksum = "3c04e8343c3daeec41f58990b9d77068df31209f2af111e059e9fe9646693065"
 
 [[package]]
 name = "serde_json"
-version = "1.0.94"
+version = "1.0.95"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1c533a59c9d8a93a09c6ab31f0fd5e5f4dd1b8fc9434804029839884765d04ea"
+checksum = "d721eca97ac802aa7777b701877c8004d950fc142651367300d21c1cc0194744"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
```

### Comparing `orjson-3.8.8/pysrc/orjson/__init__.pyi` & `orjson-3.8.9/pysrc/orjson/__init__.pyi`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/pysrc/orjson/__init__.py` & `orjson-3.8.9/pysrc/orjson/__init__.py`

 * *Files identical despite different names*

### Comparing `orjson-3.8.8/PKG-INFO` & `orjson-3.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orjson
-Version: 3.8.8
+Version: 3.8.9
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
@@ -1194,15 +1194,15 @@
 maturin build --release --strip
 ```
 
 It benefits from also having a C build environment to compile a faster
 deserialization backend. See this project's `manylinux_2_28` builds for an
 example using clang and LTO.
 
-The project's own CI tests against `nightly-2023-03-20` and stable 1.60. It
+The project's own CI tests against `nightly-2023-03-28` and stable 1.60. It
 is prudent to pin the nightly version because that channel can introduce
 breaking changes.
 
 orjson is tested for amd64, aarch64, arm7, and ppc64le on Linux. It is tested for
 amd64 on macOS and cross-compiles for aarch64. For Windows it is tested on
 amd64.
```

