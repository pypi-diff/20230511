# Comparing `tmp/mocodo-3.1.1.tar.gz` & `tmp/mocodo-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mocodo-3.1.1.tar", max compression
+gzip compressed data, was "mocodo-3.1.2.tar", max compression
```

## Comparing `mocodo-3.1.1.tar` & `mocodo-3.1.2.tar`

### file list

```diff
@@ -1,97 +1,97 @@
--rw-r--r--   0        0        0     1072 2017-09-06 13:23:36.000000 mocodo-3.1.1/LICENSE
--rw-r--r--   0        0        0     5375 2022-12-24 19:43:30.223232 mocodo-3.1.1/README.md
--rw-r--r--   0        0        0       75 2022-09-05 13:09:15.000000 mocodo-3.1.1/mocodo/__init__.py
--rwxr-xr-x   0        0        0     3798 2022-11-02 08:58:46.000000 mocodo-3.1.1/mocodo/__main__.py
--rwxr-xr-x   0        0        0    16611 2022-12-24 19:09:25.460925 mocodo-3.1.1/mocodo/argument_parser.py
--rwxr-xr-x   0        0        0     8988 2022-09-23 10:07:17.000000 mocodo-3.1.1/mocodo/arrange_bb.py
--rwxr-xr-x   0        0        0     5511 2022-09-22 13:40:19.764381 mocodo-3.1.1/mocodo/arrange_ga.py
--rwxr-xr-x   0        0        0    21157 2022-11-18 08:55:22.000000 mocodo-3.1.1/mocodo/association.py
--rwxr-xr-x   0        0        0     3903 2022-09-05 13:09:15.000000 mocodo-3.1.1/mocodo/attribute.py
--rwxr-xr-x   0        0        0     5886 2022-12-24 19:36:16.845859 mocodo-3.1.1/mocodo/common.py
--rwxr-xr-x   0        0        0     1437 2022-09-05 13:09:15.000000 mocodo-3.1.1/mocodo/cross.py
--rw-r--r--   0        0        0     1991 2022-09-05 13:09:15.000000 mocodo-3.1.1/mocodo/damerau_levenshtein.py
--rwxr-xr-x   0        0        0     4484 2022-09-05 13:09:15.000000 mocodo-3.1.1/mocodo/diagram_link.py
--rwxr-xr-x   0        0        0     6558 2022-12-12 09:58:24.700846 mocodo-3.1.1/mocodo/entity.py
--rwxr-xr-x   0        0        0      228 2022-09-05 13:09:15.000000 mocodo-3.1.1/mocodo/file_helpers.py
--rwxr-xr-x   0        0        0     1280 2022-09-05 13:09:15.000000 mocodo-3.1.1/mocodo/fitness.py
--rwxr-xr-x   0        0        0     1110 2022-12-14 18:51:18.000000 mocodo-3.1.1/mocodo/font_metrics.py
--rwxr-xr-x   0        0        0     1957 2022-09-05 13:09:15.000000 mocodo-3.1.1/mocodo/grid.py
--rwxr-xr-x   0        0        0    22715 2022-09-18 13:16:09.000000 mocodo-3.1.1/mocodo/leg.py
--rw-r--r--   0        0        0     5334 2022-12-12 12:51:27.000000 mocodo-3.1.1/mocodo/magic_command.py
--rwxr-xr-x   0        0        0    22987 2022-12-24 19:37:13.695373 mocodo-3.1.1/mocodo/mcd.py
--rw-r--r--   0        0        0    10653 2022-12-24 19:09:25.461733 mocodo-3.1.1/mocodo/mcd_to_svg.py
--rwxr-xr-x   0        0        0      630 2022-09-18 17:39:21.000000 mocodo-3.1.1/mocodo/mocodo_error.py
--rwxr-xr-x   0        0        0     4172 2022-09-22 13:40:20.147827 mocodo-3.1.1/mocodo/obfuscate.py
--rwxr-xr-x   0        0        0      542 2022-09-05 13:09:15.000000 mocodo-3.1.1/mocodo/phantom.py
--rwxr-xr-x   0        0        0     1639 2022-09-12 10:44:29.000000 mocodo-3.1.1/mocodo/pluralize_fr.py
--rwxr-xr-x   0        0        0     4535 2022-12-14 18:51:18.000000 mocodo-3.1.1/mocodo/read_template.py
--rwxr-xr-x   0        0        0    35235 2022-12-14 18:51:18.000000 mocodo-3.1.1/mocodo/relations.py
--rw-r--r--   0        0        0      537 2022-09-05 13:09:15.000000 mocodo-3.1.1/mocodo/resources/colors/blank.json
--rw-r--r--   0        0        0      580 2022-09-05 13:09:15.000000 mocodo-3.1.1/mocodo/resources/colors/brewer+1.json
--rw-r--r--   0        0        0      580 2022-09-05 13:09:15.000000 mocodo-3.1.1/mocodo/resources/colors/brewer+2.json
--rw-r--r--   0        0        0      580 2022-09-05 13:09:15.000000 mocodo-3.1.1/mocodo/resources/colors/brewer+3.json
--rw-r--r--   0        0        0      580 2022-09-05 13:09:15.000000 mocodo-3.1.1/mocodo/resources/colors/brewer+4.json
--rw-r--r--   0        0        0      580 2022-09-05 13:09:15.000000 mocodo-3.1.1/mocodo/resources/colors/brewer+5.json
--rw-r--r--   0        0        0      574 2022-09-05 13:09:15.000000 mocodo-3.1.1/mocodo/resources/colors/brewer+6.json
--rw-r--r--   0        0        0      580 2022-09-05 13:09:15.000000 mocodo-3.1.1/mocodo/resources/colors/brewer+7.json
--rw-r--r--   0        0        0      580 2022-09-05 13:09:15.000000 mocodo-3.1.1/mocodo/resources/colors/brewer+8.json
--rw-r--r--   0        0        0      580 2022-09-05 13:09:15.000000 mocodo-3.1.1/mocodo/resources/colors/brewer+9.json
--rw-r--r--   0        0        0      580 2022-09-05 13:09:15.000000 mocodo-3.1.1/mocodo/resources/colors/brewer-1.json
--rw-r--r--   0        0        0      580 2022-09-05 13:09:15.000000 mocodo-3.1.1/mocodo/resources/colors/brewer-2.json
--rw-r--r--   0        0        0      580 2022-09-05 13:09:15.000000 mocodo-3.1.1/mocodo/resources/colors/brewer-3.json
--rw-r--r--   0        0        0      580 2022-09-05 13:09:15.000000 mocodo-3.1.1/mocodo/resources/colors/brewer-4.json
--rw-r--r--   0        0        0      580 2022-09-05 13:09:15.000000 mocodo-3.1.1/mocodo/resources/colors/brewer-5.json
--rw-r--r--   0        0        0      574 2022-09-05 13:09:15.000000 mocodo-3.1.1/mocodo/resources/colors/brewer-6.json
--rw-r--r--   0        0        0      580 2022-09-05 13:09:15.000000 mocodo-3.1.1/mocodo/resources/colors/brewer-7.json
--rw-r--r--   0        0        0      580 2022-09-05 13:09:15.000000 mocodo-3.1.1/mocodo/resources/colors/brewer-8.json
--rw-r--r--   0        0        0      580 2022-09-05 13:09:15.000000 mocodo-3.1.1/mocodo/resources/colors/brewer-9.json
--rw-r--r--   0        0        0      545 2022-12-08 07:24:06.582353 mocodo-3.1.1/mocodo/resources/colors/bw-alpha.json
--rw-r--r--   0        0        0      547 2022-12-08 07:24:30.916510 mocodo-3.1.1/mocodo/resources/colors/bw.json
--rw-r--r--   0        0        0      587 2022-09-05 13:09:15.000000 mocodo-3.1.1/mocodo/resources/colors/desert.json
--rw-r--r--   0        0        0      545 2022-09-05 13:09:15.000000 mocodo-3.1.1/mocodo/resources/colors/gray.json
--rw-r--r--   0        0        0      577 2022-09-05 13:09:15.000000 mocodo-3.1.1/mocodo/resources/colors/keepsake.json
--rw-r--r--   0        0        0      593 2022-09-05 13:09:15.000000 mocodo-3.1.1/mocodo/resources/colors/mondrian.json
--rw-r--r--   0        0        0      587 2022-09-05 13:09:15.000000 mocodo-3.1.1/mocodo/resources/colors/ocean.json
--rw-r--r--   0        0        0      587 2022-09-05 13:09:15.000000 mocodo-3.1.1/mocodo/resources/colors/pond.json
--rw-r--r--   0        0        0      550 2022-09-05 13:09:15.000000 mocodo-3.1.1/mocodo/resources/colors/wb.json
--rw-r--r--   0        0        0      592 2022-09-05 13:09:15.000000 mocodo-3.1.1/mocodo/resources/colors/xinnian.json
--rw-r--r--   0        0        0    99839 2022-09-05 13:09:15.000000 mocodo-3.1.1/mocodo/resources/font_metrics.json
--rw-r--r--   0        0        0    64345 2022-09-05 13:09:15.000000 mocodo-3.1.1/mocodo/resources/lorem/disparition.txt
--rw-r--r--   0        0        0     3200 2022-09-05 13:09:15.000000 mocodo-3.1.1/mocodo/resources/lorem/four_letter_words.txt
--rw-r--r--   0        0        0     2051 2022-09-05 13:09:15.000000 mocodo-3.1.1/mocodo/resources/lorem/lorem_ipsum.txt
--rw-r--r--   0        0        0      473 2022-09-05 13:09:15.000000 mocodo-3.1.1/mocodo/resources/pristine_sandbox.mcd
--rw-r--r--   0        0        0     3237 2022-12-11 18:28:44.000000 mocodo-3.1.1/mocodo/resources/relation_templates/debug.json
--rw-r--r--   0        0        0     1137 2022-12-15 07:59:15.000000 mocodo-3.1.1/mocodo/resources/relation_templates/dependencies.json
--rw-r--r--   0        0        0      973 2022-12-12 15:29:58.000000 mocodo-3.1.1/mocodo/resources/relation_templates/diagram.json
--rw-r--r--   0        0        0     1362 2022-12-13 17:04:21.000000 mocodo-3.1.1/mocodo/resources/relation_templates/html.json
--rw-r--r--   0        0        0    18311 2022-12-12 15:29:58.000000 mocodo-3.1.1/mocodo/resources/relation_templates/html_verbose.json
--rw-r--r--   0        0        0     7363 2022-12-12 15:29:58.000000 mocodo-3.1.1/mocodo/resources/relation_templates/json.json
--rw-r--r--   0        0        0     1253 2022-12-12 15:29:58.000000 mocodo-3.1.1/mocodo/resources/relation_templates/latex.json
--rw-r--r--   0        0        0      104 2022-12-14 18:51:18.000000 mocodo-3.1.1/mocodo/resources/relation_templates/latex_without_def.json
--rw-r--r--   0        0        0      421 2022-12-12 15:29:58.000000 mocodo-3.1.1/mocodo/resources/relation_templates/markdown.json
--rw-r--r--   0        0        0     1441 2022-12-12 15:29:58.000000 mocodo-3.1.1/mocodo/resources/relation_templates/markdown_data_dict.json
--rw-r--r--   0        0        0    14169 2022-12-12 15:29:58.000000 mocodo-3.1.1/mocodo/resources/relation_templates/markdown_verbose.json
--rw-r--r--   0        0        0     5065 2022-12-12 15:29:58.000000 mocodo-3.1.1/mocodo/resources/relation_templates/mysql.json
--rw-r--r--   0        0        0     5104 2022-12-12 15:29:58.000000 mocodo-3.1.1/mocodo/resources/relation_templates/oracle.json
--rw-r--r--   0        0        0     4918 2022-12-12 15:29:58.000000 mocodo-3.1.1/mocodo/resources/relation_templates/postgresql.json
--rw-r--r--   0        0        0     5311 2022-12-12 15:29:58.000000 mocodo-3.1.1/mocodo/resources/relation_templates/sqlite.json
--rw-r--r--   0        0        0       25 2022-12-14 18:51:18.000000 mocodo-3.1.1/mocodo/resources/relation_templates/text.json
--rw-r--r--   0        0        0      347 2022-12-12 09:58:24.706687 mocodo-3.1.1/mocodo/resources/relation_templates/txt2tags.json
--rw-r--r--   0        0        0     4777 2022-09-05 13:09:15.000000 mocodo-3.1.1/mocodo/resources/res/messages_de.mo
--rw-r--r--   0        0        0     8632 2022-12-14 18:51:18.000000 mocodo-3.1.1/mocodo/resources/res/messages_fr.mo
--rw-r--r--   0        0        0    10357 2022-12-14 18:51:18.000000 mocodo-3.1.1/mocodo/resources/res/messages_fr.po
--rw-r--r--   0        0        0     4048 2022-09-05 13:09:15.000000 mocodo-3.1.1/mocodo/resources/res/messages_zh.mo
--rw-r--r--   0        0        0     1213 2022-09-05 13:09:15.000000 mocodo-3.1.1/mocodo/resources/shapes/arial.json
--rw-r--r--   0        0        0     1215 2022-09-05 13:09:15.000000 mocodo-3.1.1/mocodo/resources/shapes/copperplate.json
--rw-r--r--   0        0        0     1205 2022-09-05 13:09:15.000000 mocodo-3.1.1/mocodo/resources/shapes/georgia.json
--rw-r--r--   0        0        0     1345 2022-09-05 13:09:15.000000 mocodo-3.1.1/mocodo/resources/shapes/mondrian.json
--rw-r--r--   0        0        0     1260 2022-09-05 13:09:15.000000 mocodo-3.1.1/mocodo/resources/shapes/sans.json
--rw-r--r--   0        0        0     1267 2022-09-05 13:09:15.000000 mocodo-3.1.1/mocodo/resources/shapes/serif.json
--rw-r--r--   0        0        0     1245 2022-09-05 13:09:15.000000 mocodo-3.1.1/mocodo/resources/shapes/times.json
--rw-r--r--   0        0        0     1230 2022-09-05 13:09:15.000000 mocodo-3.1.1/mocodo/resources/shapes/trebuchet.json
--rw-r--r--   0        0        0     1333 2022-09-05 13:09:15.000000 mocodo-3.1.1/mocodo/resources/shapes/verdana.json
--rw-r--r--   0        0        0     1245 2022-09-05 13:09:15.000000 mocodo-3.1.1/mocodo/resources/shapes/xinnian.json
--rw-r--r--   0        0        0       18 2022-12-24 19:32:18.692510 mocodo-3.1.1/mocodo/version_number.py
--rw-r--r--   0        0        0     1216 2022-12-24 19:32:18.692333 mocodo-3.1.1/pyproject.toml
--rw-r--r--   0        0        0     6338 1970-01-01 00:00:00.000000 mocodo-3.1.1/setup.py
--rw-r--r--   0        0        0     6585 1970-01-01 00:00:00.000000 mocodo-3.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2017-09-06 13:23:36.000000 mocodo-3.1.2/LICENSE
+-rw-r--r--   0        0        0     5502 2023-05-11 17:23:34.304546 mocodo-3.1.2/README.md
+-rw-r--r--   0        0        0       75 2022-09-05 13:09:15.074760 mocodo-3.1.2/mocodo/__init__.py
+-rwxr-xr-x   0        0        0     3798 2022-11-02 08:58:46.486058 mocodo-3.1.2/mocodo/__main__.py
+-rwxr-xr-x   0        0        0    16632 2023-01-28 11:18:09.584553 mocodo-3.1.2/mocodo/argument_parser.py
+-rwxr-xr-x   0        0        0     8988 2022-09-29 15:13:08.365059 mocodo-3.1.2/mocodo/arrange_bb.py
+-rwxr-xr-x   0        0        0     5511 2022-09-22 13:40:19.000000 mocodo-3.1.2/mocodo/arrange_ga.py
+-rwxr-xr-x   0        0        0    21157 2022-11-18 08:55:22.092728 mocodo-3.1.2/mocodo/association.py
+-rwxr-xr-x   0        0        0     3903 2022-09-05 13:09:15.079105 mocodo-3.1.2/mocodo/attribute.py
+-rwxr-xr-x   0        0        0     5886 2023-01-28 11:16:39.787010 mocodo-3.1.2/mocodo/common.py
+-rwxr-xr-x   0        0        0     1437 2022-09-05 13:09:15.080189 mocodo-3.1.2/mocodo/cross.py
+-rw-r--r--   0        0        0     1991 2022-09-05 13:09:15.080684 mocodo-3.1.2/mocodo/damerau_levenshtein.py
+-rwxr-xr-x   0        0        0     4484 2022-09-05 13:09:15.081151 mocodo-3.1.2/mocodo/diagram_link.py
+-rwxr-xr-x   0        0        0     6558 2022-12-12 09:58:24.000000 mocodo-3.1.2/mocodo/entity.py
+-rwxr-xr-x   0        0        0      228 2022-09-05 13:09:15.082116 mocodo-3.1.2/mocodo/file_helpers.py
+-rwxr-xr-x   0        0        0     1280 2022-09-05 13:09:15.082712 mocodo-3.1.2/mocodo/fitness.py
+-rwxr-xr-x   0        0        0     1110 2023-01-28 11:16:39.787918 mocodo-3.1.2/mocodo/font_metrics.py
+-rwxr-xr-x   0        0        0     1957 2022-09-05 13:09:15.083736 mocodo-3.1.2/mocodo/grid.py
+-rwxr-xr-x   0        0        0    22715 2022-09-18 13:16:09.863651 mocodo-3.1.2/mocodo/leg.py
+-rw-r--r--   0        0        0     5334 2022-12-12 12:51:27.098572 mocodo-3.1.2/mocodo/magic_command.py
+-rwxr-xr-x   0        0        0    22987 2023-01-28 11:18:09.585379 mocodo-3.1.2/mocodo/mcd.py
+-rw-r--r--   0        0        0    10653 2023-01-28 11:18:09.586112 mocodo-3.1.2/mocodo/mcd_to_svg.py
+-rwxr-xr-x   0        0        0      630 2022-09-18 17:39:21.116186 mocodo-3.1.2/mocodo/mocodo_error.py
+-rwxr-xr-x   0        0        0     4172 2022-09-22 13:40:20.000000 mocodo-3.1.2/mocodo/obfuscate.py
+-rwxr-xr-x   0        0        0      542 2022-09-05 13:09:15.088019 mocodo-3.1.2/mocodo/phantom.py
+-rwxr-xr-x   0        0        0     1639 2022-09-12 10:44:29.393788 mocodo-3.1.2/mocodo/pluralize_fr.py
+-rwxr-xr-x   0        0        0     4535 2023-01-28 11:16:39.790562 mocodo-3.1.2/mocodo/read_template.py
+-rwxr-xr-x   0        0        0    35235 2023-01-28 11:16:39.791270 mocodo-3.1.2/mocodo/relations.py
+-rw-r--r--   0        0        0      537 2022-09-05 13:09:15.089872 mocodo-3.1.2/mocodo/resources/colors/blank.json
+-rw-r--r--   0        0        0      580 2022-09-05 13:09:15.090314 mocodo-3.1.2/mocodo/resources/colors/brewer+1.json
+-rw-r--r--   0        0        0      580 2022-09-05 13:09:15.090722 mocodo-3.1.2/mocodo/resources/colors/brewer+2.json
+-rw-r--r--   0        0        0      580 2022-09-05 13:09:15.090974 mocodo-3.1.2/mocodo/resources/colors/brewer+3.json
+-rw-r--r--   0        0        0      580 2022-09-05 13:09:15.091207 mocodo-3.1.2/mocodo/resources/colors/brewer+4.json
+-rw-r--r--   0        0        0      580 2022-09-05 13:09:15.091422 mocodo-3.1.2/mocodo/resources/colors/brewer+5.json
+-rw-r--r--   0        0        0      574 2022-09-05 13:09:15.091816 mocodo-3.1.2/mocodo/resources/colors/brewer+6.json
+-rw-r--r--   0        0        0      580 2022-09-05 13:09:15.092123 mocodo-3.1.2/mocodo/resources/colors/brewer+7.json
+-rw-r--r--   0        0        0      580 2022-09-05 13:09:15.092664 mocodo-3.1.2/mocodo/resources/colors/brewer+8.json
+-rw-r--r--   0        0        0      580 2022-09-05 13:09:15.093089 mocodo-3.1.2/mocodo/resources/colors/brewer+9.json
+-rw-r--r--   0        0        0      580 2022-09-05 13:09:15.093664 mocodo-3.1.2/mocodo/resources/colors/brewer-1.json
+-rw-r--r--   0        0        0      580 2022-09-05 13:09:15.093912 mocodo-3.1.2/mocodo/resources/colors/brewer-2.json
+-rw-r--r--   0        0        0      580 2022-09-05 13:09:15.094140 mocodo-3.1.2/mocodo/resources/colors/brewer-3.json
+-rw-r--r--   0        0        0      580 2022-09-05 13:09:15.094377 mocodo-3.1.2/mocodo/resources/colors/brewer-4.json
+-rw-r--r--   0        0        0      580 2022-09-05 13:09:15.094632 mocodo-3.1.2/mocodo/resources/colors/brewer-5.json
+-rw-r--r--   0        0        0      574 2022-09-05 13:09:15.094880 mocodo-3.1.2/mocodo/resources/colors/brewer-6.json
+-rw-r--r--   0        0        0      580 2022-09-05 13:09:15.095161 mocodo-3.1.2/mocodo/resources/colors/brewer-7.json
+-rw-r--r--   0        0        0      580 2022-09-05 13:09:15.095777 mocodo-3.1.2/mocodo/resources/colors/brewer-8.json
+-rw-r--r--   0        0        0      580 2022-09-05 13:09:15.096030 mocodo-3.1.2/mocodo/resources/colors/brewer-9.json
+-rw-r--r--   0        0        0      545 2022-12-08 07:24:06.000000 mocodo-3.1.2/mocodo/resources/colors/bw-alpha.json
+-rw-r--r--   0        0        0      547 2022-12-08 07:24:30.000000 mocodo-3.1.2/mocodo/resources/colors/bw.json
+-rw-r--r--   0        0        0      587 2022-09-05 13:09:15.097008 mocodo-3.1.2/mocodo/resources/colors/desert.json
+-rw-r--r--   0        0        0      545 2022-09-05 13:09:15.097312 mocodo-3.1.2/mocodo/resources/colors/gray.json
+-rw-r--r--   0        0        0      577 2022-09-05 13:09:15.097927 mocodo-3.1.2/mocodo/resources/colors/keepsake.json
+-rw-r--r--   0        0        0      593 2022-09-05 13:09:15.098329 mocodo-3.1.2/mocodo/resources/colors/mondrian.json
+-rw-r--r--   0        0        0      587 2022-09-05 13:09:15.098577 mocodo-3.1.2/mocodo/resources/colors/ocean.json
+-rw-r--r--   0        0        0      587 2022-09-05 13:09:15.098954 mocodo-3.1.2/mocodo/resources/colors/pond.json
+-rw-r--r--   0        0        0      550 2022-09-05 13:09:15.099350 mocodo-3.1.2/mocodo/resources/colors/wb.json
+-rw-r--r--   0        0        0      592 2022-09-05 13:09:15.099599 mocodo-3.1.2/mocodo/resources/colors/xinnian.json
+-rw-r--r--   0        0        0    99839 2022-09-05 13:09:15.100146 mocodo-3.1.2/mocodo/resources/font_metrics.json
+-rw-r--r--   0        0        0    64345 2022-09-05 13:09:15.100633 mocodo-3.1.2/mocodo/resources/lorem/disparition.txt
+-rw-r--r--   0        0        0     3200 2022-09-05 13:09:15.100777 mocodo-3.1.2/mocodo/resources/lorem/four_letter_words.txt
+-rw-r--r--   0        0        0     2051 2022-09-05 13:09:15.100888 mocodo-3.1.2/mocodo/resources/lorem/lorem_ipsum.txt
+-rw-r--r--   0        0        0      434 2023-05-11 16:54:02.232226 mocodo-3.1.2/mocodo/resources/pristine_sandbox.mcd
+-rw-r--r--   0        0        0     3237 2022-12-11 18:28:56.187987 mocodo-3.1.2/mocodo/resources/relation_templates/debug.json
+-rw-r--r--   0        0        0     1137 2023-01-28 11:16:39.791612 mocodo-3.1.2/mocodo/resources/relation_templates/dependencies.json
+-rw-r--r--   0        0        0      973 2022-12-12 15:29:58.319997 mocodo-3.1.2/mocodo/resources/relation_templates/diagram.json
+-rw-r--r--   0        0        0     1362 2022-12-13 17:17:49.267440 mocodo-3.1.2/mocodo/resources/relation_templates/html.json
+-rw-r--r--   0        0        0    18311 2022-12-12 15:29:58.320955 mocodo-3.1.2/mocodo/resources/relation_templates/html_verbose.json
+-rw-r--r--   0        0        0     7363 2022-12-12 15:29:58.321361 mocodo-3.1.2/mocodo/resources/relation_templates/json.json
+-rw-r--r--   0        0        0     1253 2022-12-12 15:29:58.321750 mocodo-3.1.2/mocodo/resources/relation_templates/latex.json
+-rw-r--r--   0        0        0      104 2023-01-28 11:16:39.792002 mocodo-3.1.2/mocodo/resources/relation_templates/latex_without_def.json
+-rw-r--r--   0        0        0      421 2022-12-12 15:29:58.322622 mocodo-3.1.2/mocodo/resources/relation_templates/markdown.json
+-rw-r--r--   0        0        0     1441 2022-12-12 15:29:58.323069 mocodo-3.1.2/mocodo/resources/relation_templates/markdown_data_dict.json
+-rw-r--r--   0        0        0    14169 2022-12-12 15:29:58.323618 mocodo-3.1.2/mocodo/resources/relation_templates/markdown_verbose.json
+-rw-r--r--   0        0        0     5065 2022-12-12 15:29:58.323968 mocodo-3.1.2/mocodo/resources/relation_templates/mysql.json
+-rw-r--r--   0        0        0     5104 2022-12-12 15:29:58.324305 mocodo-3.1.2/mocodo/resources/relation_templates/oracle.json
+-rw-r--r--   0        0        0     4918 2022-12-12 15:29:58.324644 mocodo-3.1.2/mocodo/resources/relation_templates/postgresql.json
+-rw-r--r--   0        0        0     5311 2022-12-12 15:29:58.325008 mocodo-3.1.2/mocodo/resources/relation_templates/sqlite.json
+-rw-r--r--   0        0        0       25 2023-01-28 11:16:39.792840 mocodo-3.1.2/mocodo/resources/relation_templates/text.json
+-rw-r--r--   0        0        0      347 2022-12-12 09:58:24.000000 mocodo-3.1.2/mocodo/resources/relation_templates/txt2tags.json
+-rw-r--r--   0        0        0     4777 2022-09-05 13:09:15.107446 mocodo-3.1.2/mocodo/resources/res/messages_de.mo
+-rw-r--r--   0        0        0     8632 2023-01-28 11:16:39.793231 mocodo-3.1.2/mocodo/resources/res/messages_fr.mo
+-rw-r--r--   0        0        0    10357 2023-01-28 11:16:39.793653 mocodo-3.1.2/mocodo/resources/res/messages_fr.po
+-rw-r--r--   0        0        0     4048 2022-09-05 13:09:15.109006 mocodo-3.1.2/mocodo/resources/res/messages_zh.mo
+-rw-r--r--   0        0        0     1213 2022-09-05 13:09:15.109826 mocodo-3.1.2/mocodo/resources/shapes/arial.json
+-rw-r--r--   0        0        0     1215 2022-09-05 13:09:15.110327 mocodo-3.1.2/mocodo/resources/shapes/copperplate.json
+-rw-r--r--   0        0        0     1205 2022-09-05 13:09:15.110856 mocodo-3.1.2/mocodo/resources/shapes/georgia.json
+-rw-r--r--   0        0        0     1345 2022-09-05 13:09:15.111318 mocodo-3.1.2/mocodo/resources/shapes/mondrian.json
+-rw-r--r--   0        0        0     1260 2022-09-05 13:09:15.112005 mocodo-3.1.2/mocodo/resources/shapes/sans.json
+-rw-r--r--   0        0        0     1267 2022-09-05 13:09:15.112359 mocodo-3.1.2/mocodo/resources/shapes/serif.json
+-rw-r--r--   0        0        0     1245 2022-09-05 13:09:15.112640 mocodo-3.1.2/mocodo/resources/shapes/times.json
+-rw-r--r--   0        0        0     1230 2022-09-05 13:09:15.112988 mocodo-3.1.2/mocodo/resources/shapes/trebuchet.json
+-rw-r--r--   0        0        0     1333 2022-09-05 13:09:15.113325 mocodo-3.1.2/mocodo/resources/shapes/verdana.json
+-rw-r--r--   0        0        0     1245 2022-09-05 13:09:15.113890 mocodo-3.1.2/mocodo/resources/shapes/xinnian.json
+-rw-r--r--   0        0        0       18 2023-05-11 17:20:56.321498 mocodo-3.1.2/mocodo/version_number.py
+-rw-r--r--   0        0        0     1216 2023-05-11 17:20:56.246865 mocodo-3.1.2/pyproject.toml
+-rw-r--r--   0        0        0     7291 1970-01-01 00:00:00.000000 mocodo-3.1.2/setup.py
+-rw-r--r--   0        0        0     6712 1970-01-01 00:00:00.000000 mocodo-3.1.2/PKG-INFO
```

### Comparing `mocodo-3.1.1/LICENSE` & `mocodo-3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/README.md` & `mocodo-3.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+**11 mai 2023.** Ajout d'un tutoriel / galerie d'exemples dans la [version en ligne](https://www.mocodo.net) de Mocodo 3.1.2.
+
 **24 décembre 2022.** Mocodo 3.1.1 corrige la [gestion des collisions des SVG interactifs](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Éviter-qu'une-interaction-sur-un-SVG-ne-s'applique-à-un-autre).
 
 **14 décembre 2022.** Mocodo 3.1 améliore le passage au relationnel : prise en charge de [gabarits personnels dérivés des gabarits existants](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Dérivation-de-gabarits), traitement des [tables indépendantes réduites à leur clé primaire](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Suppression-des-tables-indépendantes-réduites-à-leur-clé-primaire), génération d'un [graphe des dépendances](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Graphe-des-dépendances) pour le tri topologique des tables, [etc](https://github.com/laowantong/mocodo/releases/tag/3.1.0).
 
 **11 septembre 2022.** Mocodo 3.0 introduit l'[héritage](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Héritage-(ou-spécialisation)), l'[agrégation](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Agrégation-(ou-pseudo-entité)), les [calques](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Héritage-(ou-spécialisation)), les [sorties PDF et PNG](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Héritage-(ou-spécialisation)), [etc](https://github.com/laowantong/mocodo/releases/tag/3.0).
 
 ------
```

### Comparing `mocodo-3.1.1/mocodo/__main__.py` & `mocodo-3.1.2/mocodo/__main__.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/argument_parser.py` & `mocodo-3.1.2/mocodo/argument_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,16 +41,16 @@
   MIT LICENSE.
 
 CONTACT:
   Mail                  <author.full.name>@univ-lorraine.fr
   Author                Aristide Grange
   Address               Université de Lorraine
                         Laboratoire LCOMS - UFR MIM
-                        Ile du Saulcy
-                        57000 Metz
+                        3 rue Augustin Fresnel
+                        57070 METZ Technopôle
                         France
 """  # NB: accents raise an error in Jupyter Notebook
 
 
 class ArgumentDefaultsRawDescriptionHelpFormatter(
     argparse.ArgumentDefaultsHelpFormatter,
     argparse.RawDescriptionHelpFormatter,
```

### Comparing `mocodo-3.1.1/mocodo/arrange_bb.py` & `mocodo-3.1.2/mocodo/arrange_bb.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/arrange_ga.py` & `mocodo-3.1.2/mocodo/arrange_ga.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/association.py` & `mocodo-3.1.2/mocodo/association.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/attribute.py` & `mocodo-3.1.2/mocodo/attribute.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/common.py` & `mocodo-3.1.2/mocodo/common.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/cross.py` & `mocodo-3.1.2/mocodo/cross.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/damerau_levenshtein.py` & `mocodo-3.1.2/mocodo/damerau_levenshtein.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/diagram_link.py` & `mocodo-3.1.2/mocodo/diagram_link.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/entity.py` & `mocodo-3.1.2/mocodo/entity.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/fitness.py` & `mocodo-3.1.2/mocodo/fitness.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/font_metrics.py` & `mocodo-3.1.2/mocodo/font_metrics.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/grid.py` & `mocodo-3.1.2/mocodo/grid.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/leg.py` & `mocodo-3.1.2/mocodo/leg.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/magic_command.py` & `mocodo-3.1.2/mocodo/magic_command.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/mcd.py` & `mocodo-3.1.2/mocodo/mcd.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/mcd_to_svg.py` & `mocodo-3.1.2/mocodo/mcd_to_svg.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/mocodo_error.py` & `mocodo-3.1.2/mocodo/mocodo_error.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/obfuscate.py` & `mocodo-3.1.2/mocodo/obfuscate.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/phantom.py` & `mocodo-3.1.2/mocodo/phantom.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/pluralize_fr.py` & `mocodo-3.1.2/mocodo/pluralize_fr.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/read_template.py` & `mocodo-3.1.2/mocodo/read_template.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/relations.py` & `mocodo-3.1.2/mocodo/relations.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/colors/blank.json` & `mocodo-3.1.2/mocodo/resources/colors/blank.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/colors/brewer+1.json` & `mocodo-3.1.2/mocodo/resources/colors/brewer+1.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/colors/brewer+2.json` & `mocodo-3.1.2/mocodo/resources/colors/brewer+2.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/colors/brewer+3.json` & `mocodo-3.1.2/mocodo/resources/colors/brewer+3.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/colors/brewer+4.json` & `mocodo-3.1.2/mocodo/resources/colors/brewer+4.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/colors/brewer+5.json` & `mocodo-3.1.2/mocodo/resources/colors/brewer+5.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/colors/brewer+6.json` & `mocodo-3.1.2/mocodo/resources/colors/brewer+6.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/colors/brewer+7.json` & `mocodo-3.1.2/mocodo/resources/colors/brewer+7.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/colors/brewer+8.json` & `mocodo-3.1.2/mocodo/resources/colors/brewer+8.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/colors/brewer+9.json` & `mocodo-3.1.2/mocodo/resources/colors/brewer+9.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/colors/brewer-1.json` & `mocodo-3.1.2/mocodo/resources/colors/brewer-1.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/colors/brewer-2.json` & `mocodo-3.1.2/mocodo/resources/colors/brewer-2.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/colors/brewer-3.json` & `mocodo-3.1.2/mocodo/resources/colors/brewer-3.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/colors/brewer-4.json` & `mocodo-3.1.2/mocodo/resources/colors/brewer-4.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/colors/brewer-5.json` & `mocodo-3.1.2/mocodo/resources/colors/brewer-5.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/colors/brewer-6.json` & `mocodo-3.1.2/mocodo/resources/colors/brewer-6.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/colors/brewer-7.json` & `mocodo-3.1.2/mocodo/resources/colors/brewer-7.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/colors/brewer-8.json` & `mocodo-3.1.2/mocodo/resources/colors/brewer-8.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/colors/brewer-9.json` & `mocodo-3.1.2/mocodo/resources/colors/brewer-9.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/colors/bw-alpha.json` & `mocodo-3.1.2/mocodo/resources/colors/bw-alpha.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/colors/bw.json` & `mocodo-3.1.2/mocodo/resources/colors/bw.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/colors/desert.json` & `mocodo-3.1.2/mocodo/resources/colors/desert.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/colors/gray.json` & `mocodo-3.1.2/mocodo/resources/colors/gray.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/colors/keepsake.json` & `mocodo-3.1.2/mocodo/resources/colors/keepsake.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/colors/mondrian.json` & `mocodo-3.1.2/mocodo/resources/colors/mondrian.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/colors/ocean.json` & `mocodo-3.1.2/mocodo/resources/colors/ocean.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/colors/pond.json` & `mocodo-3.1.2/mocodo/resources/colors/pond.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/colors/wb.json` & `mocodo-3.1.2/mocodo/resources/colors/wb.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/colors/xinnian.json` & `mocodo-3.1.2/mocodo/resources/colors/xinnian.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/font_metrics.json` & `mocodo-3.1.2/mocodo/resources/font_metrics.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/lorem/disparition.txt` & `mocodo-3.1.2/mocodo/resources/lorem/disparition.txt`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/lorem/four_letter_words.txt` & `mocodo-3.1.2/mocodo/resources/lorem/four_letter_words.txt`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/lorem/lorem_ipsum.txt` & `mocodo-3.1.2/mocodo/resources/lorem/lorem_ipsum.txt`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/relation_templates/debug.json` & `mocodo-3.1.2/mocodo/resources/relation_templates/debug.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/relation_templates/dependencies.json` & `mocodo-3.1.2/mocodo/resources/relation_templates/dependencies.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/relation_templates/diagram.json` & `mocodo-3.1.2/mocodo/resources/relation_templates/diagram.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/relation_templates/html.json` & `mocodo-3.1.2/mocodo/resources/relation_templates/html.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/relation_templates/html_verbose.json` & `mocodo-3.1.2/mocodo/resources/relation_templates/html_verbose.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/relation_templates/json.json` & `mocodo-3.1.2/mocodo/resources/relation_templates/json.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/relation_templates/latex.json` & `mocodo-3.1.2/mocodo/resources/relation_templates/latex.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/relation_templates/markdown_data_dict.json` & `mocodo-3.1.2/mocodo/resources/relation_templates/markdown_data_dict.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/relation_templates/markdown_verbose.json` & `mocodo-3.1.2/mocodo/resources/relation_templates/markdown_verbose.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/relation_templates/mysql.json` & `mocodo-3.1.2/mocodo/resources/relation_templates/mysql.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/relation_templates/oracle.json` & `mocodo-3.1.2/mocodo/resources/relation_templates/oracle.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/relation_templates/postgresql.json` & `mocodo-3.1.2/mocodo/resources/relation_templates/postgresql.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/relation_templates/sqlite.json` & `mocodo-3.1.2/mocodo/resources/relation_templates/sqlite.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/res/messages_de.mo` & `mocodo-3.1.2/mocodo/resources/res/messages_de.mo`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/res/messages_fr.mo` & `mocodo-3.1.2/mocodo/resources/res/messages_fr.mo`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/res/messages_fr.po` & `mocodo-3.1.2/mocodo/resources/res/messages_fr.po`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/res/messages_zh.mo` & `mocodo-3.1.2/mocodo/resources/res/messages_zh.mo`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/shapes/arial.json` & `mocodo-3.1.2/mocodo/resources/shapes/arial.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/shapes/copperplate.json` & `mocodo-3.1.2/mocodo/resources/shapes/copperplate.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/shapes/georgia.json` & `mocodo-3.1.2/mocodo/resources/shapes/georgia.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/shapes/mondrian.json` & `mocodo-3.1.2/mocodo/resources/shapes/mondrian.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/shapes/sans.json` & `mocodo-3.1.2/mocodo/resources/shapes/sans.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/shapes/serif.json` & `mocodo-3.1.2/mocodo/resources/shapes/serif.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/shapes/times.json` & `mocodo-3.1.2/mocodo/resources/shapes/times.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/shapes/trebuchet.json` & `mocodo-3.1.2/mocodo/resources/shapes/trebuchet.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/shapes/verdana.json` & `mocodo-3.1.2/mocodo/resources/shapes/verdana.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/mocodo/resources/shapes/xinnian.json` & `mocodo-3.1.2/mocodo/resources/shapes/xinnian.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.1.1/pyproject.toml` & `mocodo-3.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mocodo"
-version = "3.1.1"
+version = "3.1.2"
 description = "Modélisation Conceptuelle de Données. Nickel. Ni souris."
 authors = ["Aristide Grange"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://www.mocodo.net"
 repository = "https://github.com/laowantong/mocodo/"
 keywords = ["education",
```

### Comparing `mocodo-3.1.1/setup.py` & `mocodo-3.1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,29 +2,47 @@
 from setuptools import setup
 
 packages = \
 ['mocodo']
 
 package_data = \
 {'': ['*'],
- 'mocodo': ['resources/*',
-            'resources/colors/*',
+ 'mocodo': ['resources/colors/*',
+            'resources/font_metrics.json',
+            'resources/font_metrics.json',
             'resources/lorem/*',
+            'resources/pristine_sandbox.mcd',
+            'resources/pristine_sandbox.mcd',
             'resources/relation_templates/*',
-            'resources/res/*',
+            'resources/res/messages_de.mo',
+            'resources/res/messages_de.mo',
+            'resources/res/messages_de.mo',
+            'resources/res/messages_de.mo',
+            'resources/res/messages_fr.mo',
+            'resources/res/messages_fr.mo',
+            'resources/res/messages_fr.mo',
+            'resources/res/messages_fr.mo',
+            'resources/res/messages_fr.po',
+            'resources/res/messages_fr.po',
+            'resources/res/messages_fr.po',
+            'resources/res/messages_fr.po',
+            'resources/res/messages_zh.mo',
+            'resources/res/messages_zh.mo',
+            'resources/res/messages_zh.mo',
+            'resources/res/messages_zh.mo',
             'resources/shapes/*']}
 
 entry_points = \
 {'console_scripts': ['mocodo = mocodo.__main__:main']}
 
 setup_kwargs = {
     'name': 'mocodo',
-    'version': '3.1.1',
+    'version': '3.1.2',
     'description': 'Modélisation Conceptuelle de Données. Nickel. Ni souris.',
-    'long_description': "**24 décembre 2022.** Mocodo 3.1.1 corrige la [gestion des collisions des SVG interactifs](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Éviter-qu'une-interaction-sur-un-SVG-ne-s'applique-à-un-autre).\n\n**14 décembre 2022.** Mocodo 3.1 améliore le passage au relationnel\xa0: prise en charge de [gabarits personnels dérivés des gabarits existants](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Dérivation-de-gabarits), traitement des [tables indépendantes réduites à leur clé primaire](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Suppression-des-tables-indépendantes-réduites-à-leur-clé-primaire), génération d'un [graphe des dépendances](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Graphe-des-dépendances) pour le tri topologique des tables, [etc](https://github.com/laowantong/mocodo/releases/tag/3.1.0).\n\n**11 septembre 2022.** Mocodo 3.0 introduit l'[héritage](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Héritage-(ou-spécialisation)), l'[agrégation](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Agrégation-(ou-pseudo-entité)), les [calques](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Héritage-(ou-spécialisation)), les [sorties PDF et PNG](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Héritage-(ou-spécialisation)), [etc](https://github.com/laowantong/mocodo/releases/tag/3.0).\n\n------\n\n![](https://cdn.rawgit.com/laowantong/mocodo/master/logos/banner.svg)\n\nMocodo est un logiciel d'aide à l'enseignement et à la conception des [bases de données relationnelles](https://fr.wikipedia.org/wiki/Base_de_données_relationnelle).\n\n- En entrée, il prend une description textuelle des entités et associations du modèle conceptuel de données ([MCD](https://fr.wikipedia.org/wiki/Modèle_entité-association)).\n- En sortie, il produit son diagramme entité-association en [SVG](https://fr.wikipedia.org/wiki/Scalable_Vector_Graphics) et son schéma relationnel ([MLD](\nhttps://fr.wikipedia.org/wiki/Merise_%28informatique%29#MLD_:_mod.C3.A8le_logique_des_donn.C3.A9es)) en [SQL](https://fr.wikipedia.org/wiki/Structured_Query_Language), [LaTeX](https://fr.wikipedia.org/wiki/LaTeX), [Markdown](https://fr.wikipedia.org/wiki/Markdown), etc.\n\nCi-dessous, un exemple sous [Jupyter Notebook](https://jupyter.org). L'appel du programme se fait en première ligne, sur un texte d'entrée donné lignes suivantes.\n\n```\n%%mocodo --mld --colors brewer+1 --shapes copperplate --relations diagram markdown_data_dict\nDF, 11 Élève, 1N Classe\nClasse: Num. classe, Num. salle\nFaire Cours, 1N Classe, 1N Prof: Vol. horaire\nCatégorie: Code catégorie, Nom catégorie\n\nÉlève: Num. élève, Nom élève\nNoter, 1N Élève, 0N Prof, 0N Matière, 1N Date: Note\nProf: Num. prof, Nom prof\nRelever, 0N Catégorie, 11 Prof\n\nDate: Date\nMatière: Libellé matière\nEnseigner, 11 Prof, 1N Matière\n```\n\nEn sortie, le MCD (diagramme conceptuel) et le MLD (schéma relationnel) correspondants:\n\n![](https://cdn.rawgit.com/laowantong/mocodo/master/doc/readme_1.svg)\n\n**Catégorie** (<ins>Code catégorie</ins>, Nom catégorie)<br>\n**Classe** (<ins>Num. classe</ins>, Num. salle)<br>\n**Faire Cours** (<ins>_#Num. classe_</ins>, <ins>_#Num. prof_</ins>, Vol. horaire)<br>\n**Noter** (<ins>_#Num. élève_</ins>, <ins>_#Num. prof_</ins>, <ins>_#Libellé matière_</ins>, <ins>_#Date_</ins>, Note)<br>\n**Prof** (<ins>Num. prof</ins>, Nom prof, _#Code catégorie_, _#Libellé matière_)<br>\n**Élève** (<ins>Num. élève</ins>, Nom élève, _#Num. classe_)\n\nL'appel ci-dessus a également construit le dictionnaire des données:\n\n- Num. classe\n- Num. salle\n- Vol. horaire\n- Code catégorie\n- Nom catégorie\n- Num. élève\n- Nom élève\n- Note\n- Num. prof\n- Nom prof\n- Date\n- Libellé matière\n\nAinsi que le diagramme relationnel, qui peut être visualisé par un nouvel appel:\n\n```\n%mocodo --input mocodo_notebook/sandbox.mld --colors brewer+1\n```\n\n![](https://cdn.rawgit.com/laowantong/mocodo/f06f70a/doc/readme_2.svg)\n\nLa devise de Mocodo, «\xa0nickel, ni souris\xa0», en résume les principaux points forts:\n\n- description textuelle des données. L'utilisateur n'a pas à renseigner, placer et déplacer des éléments comme avec une lessive ordinaire. Il ne fournit rien de plus que les informations définissant son MCD. L'outil s'occupe tout seul du plongement;\n- propreté du rendu. La sortie se fait en vectoriel, prête à être affichée, imprimée, agrandie, exportée dans une multitude de formats sans perte de qualité;\n- rapidité des retouches. L'utilisateur rectifie les alignements en insérant des éléments invisibles, en dupliquant des coordonnées ou en ajustant des facteurs mutiplicatifs: là encore, il travaille sur une description textuelle, et non directement sur le dessin.\n\nMocodo est libre, gratuit et multiplateforme. Si vous l'aimez, répandez la bonne nouvelle en incluant l'un de ses logos dans votre support: cela multipliera ses chances d'attirer des contributeurs qui le feront évoluer.\n\nPour vous familiariser avec Mocodo, le mieux est d'utiliser [sa version en ligne](https://www.mocodo.net).\n\nPour en savoir plus, lisez la documentation [au format HTML](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html) ou téléchargez-la [au format Jupyter Notebook](doc/fr_refman.ipynb).\n",
+    'long_description': "**11 mai 2023.** Ajout d'un tutoriel / galerie d'exemples dans la [version en ligne](https://www.mocodo.net) de Mocodo 3.1.2.\n\n**24 décembre 2022.** Mocodo 3.1.1 corrige la [gestion des collisions des SVG interactifs](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Éviter-qu'une-interaction-sur-un-SVG-ne-s'applique-à-un-autre).\n\n**14 décembre 2022.** Mocodo 3.1 améliore le passage au relationnel\xa0: prise en charge de [gabarits personnels dérivés des gabarits existants](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Dérivation-de-gabarits), traitement des [tables indépendantes réduites à leur clé primaire](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Suppression-des-tables-indépendantes-réduites-à-leur-clé-primaire), génération d'un [graphe des dépendances](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Graphe-des-dépendances) pour le tri topologique des tables, [etc](https://github.com/laowantong/mocodo/releases/tag/3.1.0).\n\n**11 septembre 2022.** Mocodo 3.0 introduit l'[héritage](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Héritage-(ou-spécialisation)), l'[agrégation](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Agrégation-(ou-pseudo-entité)), les [calques](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Héritage-(ou-spécialisation)), les [sorties PDF et PNG](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Héritage-(ou-spécialisation)), [etc](https://github.com/laowantong/mocodo/releases/tag/3.0).\n\n------\n\n![](https://cdn.rawgit.com/laowantong/mocodo/master/logos/banner.svg)\n\nMocodo est un logiciel d'aide à l'enseignement et à la conception des [bases de données relationnelles](https://fr.wikipedia.org/wiki/Base_de_données_relationnelle).\n\n- En entrée, il prend une description textuelle des entités et associations du modèle conceptuel de données ([MCD](https://fr.wikipedia.org/wiki/Modèle_entité-association)).\n- En sortie, il produit son diagramme entité-association en [SVG](https://fr.wikipedia.org/wiki/Scalable_Vector_Graphics) et son schéma relationnel ([MLD](\nhttps://fr.wikipedia.org/wiki/Merise_%28informatique%29#MLD_:_mod.C3.A8le_logique_des_donn.C3.A9es)) en [SQL](https://fr.wikipedia.org/wiki/Structured_Query_Language), [LaTeX](https://fr.wikipedia.org/wiki/LaTeX), [Markdown](https://fr.wikipedia.org/wiki/Markdown), etc.\n\nCi-dessous, un exemple sous [Jupyter Notebook](https://jupyter.org). L'appel du programme se fait en première ligne, sur un texte d'entrée donné lignes suivantes.\n\n```\n%%mocodo --mld --colors brewer+1 --shapes copperplate --relations diagram markdown_data_dict\nDF, 11 Élève, 1N Classe\nClasse: Num. classe, Num. salle\nFaire Cours, 1N Classe, 1N Prof: Vol. horaire\nCatégorie: Code catégorie, Nom catégorie\n\nÉlève: Num. élève, Nom élève\nNoter, 1N Élève, 0N Prof, 0N Matière, 1N Date: Note\nProf: Num. prof, Nom prof\nRelever, 0N Catégorie, 11 Prof\n\nDate: Date\nMatière: Libellé matière\nEnseigner, 11 Prof, 1N Matière\n```\n\nEn sortie, le MCD (diagramme conceptuel) et le MLD (schéma relationnel) correspondants:\n\n![](https://cdn.rawgit.com/laowantong/mocodo/master/doc/readme_1.svg)\n\n**Catégorie** (<ins>Code catégorie</ins>, Nom catégorie)<br>\n**Classe** (<ins>Num. classe</ins>, Num. salle)<br>\n**Faire Cours** (<ins>_#Num. classe_</ins>, <ins>_#Num. prof_</ins>, Vol. horaire)<br>\n**Noter** (<ins>_#Num. élève_</ins>, <ins>_#Num. prof_</ins>, <ins>_#Libellé matière_</ins>, <ins>_#Date_</ins>, Note)<br>\n**Prof** (<ins>Num. prof</ins>, Nom prof, _#Code catégorie_, _#Libellé matière_)<br>\n**Élève** (<ins>Num. élève</ins>, Nom élève, _#Num. classe_)\n\nL'appel ci-dessus a également construit le dictionnaire des données:\n\n- Num. classe\n- Num. salle\n- Vol. horaire\n- Code catégorie\n- Nom catégorie\n- Num. élève\n- Nom élève\n- Note\n- Num. prof\n- Nom prof\n- Date\n- Libellé matière\n\nAinsi que le diagramme relationnel, qui peut être visualisé par un nouvel appel:\n\n```\n%mocodo --input mocodo_notebook/sandbox.mld --colors brewer+1\n```\n\n![](https://cdn.rawgit.com/laowantong/mocodo/f06f70a/doc/readme_2.svg)\n\nLa devise de Mocodo, «\xa0nickel, ni souris\xa0», en résume les principaux points forts:\n\n- description textuelle des données. L'utilisateur n'a pas à renseigner, placer et déplacer des éléments comme avec une lessive ordinaire. Il ne fournit rien de plus que les informations définissant son MCD. L'outil s'occupe tout seul du plongement;\n- propreté du rendu. La sortie se fait en vectoriel, prête à être affichée, imprimée, agrandie, exportée dans une multitude de formats sans perte de qualité;\n- rapidité des retouches. L'utilisateur rectifie les alignements en insérant des éléments invisibles, en dupliquant des coordonnées ou en ajustant des facteurs mutiplicatifs: là encore, il travaille sur une description textuelle, et non directement sur le dessin.\n\nMocodo est libre, gratuit et multiplateforme. Si vous l'aimez, répandez la bonne nouvelle en incluant l'un de ses logos dans votre support: cela multipliera ses chances d'attirer des contributeurs qui le feront évoluer.\n\nPour vous familiariser avec Mocodo, le mieux est d'utiliser [sa version en ligne](https://www.mocodo.net).\n\nPour en savoir plus, lisez la documentation [au format HTML](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html) ou téléchargez-la [au format Jupyter Notebook](doc/fr_refman.ipynb).\n",
     'author': 'Aristide Grange',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://www.mocodo.net',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `mocodo-3.1.1/PKG-INFO` & `mocodo-3.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mocodo
-Version: 3.1.1
+Version: 3.1.2
 Summary: Modélisation Conceptuelle de Données. Nickel. Ni souris.
 Home-page: https://www.mocodo.net
 License: MIT
 Keywords: education,relational,database,drawing,ERD,SVG,Merise
 Author: Aristide Grange
 Requires-Python: >=3.6.1,<4.0.0
 Classifier: Development Status :: 4 - Beta
@@ -24,14 +24,16 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Database
 Classifier: Topic :: Education
 Project-URL: Repository, https://github.com/laowantong/mocodo/
 Project-URL: issues, https://github.com/laowantong/mocodo/issues
 Description-Content-Type: text/markdown
 
+**11 mai 2023.** Ajout d'un tutoriel / galerie d'exemples dans la [version en ligne](https://www.mocodo.net) de Mocodo 3.1.2.
+
 **24 décembre 2022.** Mocodo 3.1.1 corrige la [gestion des collisions des SVG interactifs](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Éviter-qu'une-interaction-sur-un-SVG-ne-s'applique-à-un-autre).
 
 **14 décembre 2022.** Mocodo 3.1 améliore le passage au relationnel : prise en charge de [gabarits personnels dérivés des gabarits existants](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Dérivation-de-gabarits), traitement des [tables indépendantes réduites à leur clé primaire](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Suppression-des-tables-indépendantes-réduites-à-leur-clé-primaire), génération d'un [graphe des dépendances](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Graphe-des-dépendances) pour le tri topologique des tables, [etc](https://github.com/laowantong/mocodo/releases/tag/3.1.0).
 
 **11 septembre 2022.** Mocodo 3.0 introduit l'[héritage](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Héritage-(ou-spécialisation)), l'[agrégation](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Agrégation-(ou-pseudo-entité)), les [calques](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Héritage-(ou-spécialisation)), les [sorties PDF et PNG](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Héritage-(ou-spécialisation)), [etc](https://github.com/laowantong/mocodo/releases/tag/3.0).
 
 ------
```

