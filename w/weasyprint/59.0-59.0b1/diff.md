# Comparing `tmp/weasyprint-59.0.tar.gz` & `tmp/weasyprint-59.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weasyprint-59.0.tar", last modified: Thu May 11 09:28:40 2023, max compression
+gzip compressed data, was "weasyprint-59.0b1.tar", last modified: Fri Apr 14 14:53:15 2023, max compression
```

## Comparing `weasyprint-59.0.tar` & `weasyprint-59.0b1.tar`

### file list

```diff
@@ -1,170 +1,170 @@
--rw-r--r--   0        0        0     1534 2022-11-12 08:45:13.781084 weasyprint-59.0/LICENSE
--rw-r--r--   0        0        0     1636 2023-03-29 18:33:03.496477 weasyprint-59.0/README.rst
--rw-r--r--   0        0        0    30741 2023-04-14 12:31:21.691807 weasyprint-59.0/docs/api_reference.rst
--rw-r--r--   0        0        0    93772 2023-05-11 09:25:06.858252 weasyprint-59.0/docs/changelog.rst
--rw-r--r--   0        0        0     4756 2023-03-06 15:20:25.288055 weasyprint-59.0/docs/common_use_cases.rst
--rw-r--r--   0        0        0     2705 2023-03-06 15:32:25.177425 weasyprint-59.0/docs/conf.py
--rw-r--r--   0        0        0     1956 2023-03-06 15:32:25.178425 weasyprint-59.0/docs/contribute.rst
--rw-r--r--   0        0        0    24221 2023-05-10 07:35:16.326974 weasyprint-59.0/docs/first_steps.rst
--rw-r--r--   0        0        0    11753 2023-03-06 15:32:25.178425 weasyprint-59.0/docs/going_further.rst
--rw-r--r--   0        0        0      308 2022-11-14 22:25:38.213016 weasyprint-59.0/docs/index.rst
--rw-r--r--   0        0        0      180 2023-03-06 15:32:25.178425 weasyprint-59.0/docs/manpage.rst
--rw-r--r--   0        0        0      882 2022-11-14 22:25:38.213016 weasyprint-59.0/docs/support.rst
--rw-r--r--   0        0        0     2306 2023-04-12 15:06:57.524514 weasyprint-59.0/pyproject.toml
--rw-r--r--   0        0        0       33 2022-11-14 22:25:38.214017 weasyprint-59.0/tests/__init__.py
--rw-r--r--   0        0        0     3516 2023-04-14 12:31:21.691807 weasyprint-59.0/tests/conftest.py
--rw-r--r--   0        0        0     5063 2023-03-06 15:32:25.178425 weasyprint-59.0/tests/draw/__init__.py
--rw-r--r--   0        0        0        0 2022-11-14 22:25:38.223017 weasyprint-59.0/tests/draw/svg/__init__.py
--rw-r--r--   0        0        0     8388 2023-03-29 18:33:03.506477 weasyprint-59.0/tests/draw/svg/test_bounding_box.py
--rw-r--r--   0        0        0     2384 2023-03-29 18:33:03.506477 weasyprint-59.0/tests/draw/svg/test_clip.py
--rw-r--r--   0        0        0     1014 2023-04-29 14:59:50.493574 weasyprint-59.0/tests/draw/svg/test_defs.py
--rw-r--r--   0        0        0    28515 2023-03-29 18:33:03.506477 weasyprint-59.0/tests/draw/svg/test_gradients.py
--rw-r--r--   0        0        0     6647 2023-03-29 18:33:03.506477 weasyprint-59.0/tests/draw/svg/test_images.py
--rw-r--r--   0        0        0     5052 2023-03-29 18:33:03.507477 weasyprint-59.0/tests/draw/svg/test_opacity.py
--rw-r--r--   0        0        0    15490 2023-03-29 18:33:03.507477 weasyprint-59.0/tests/draw/svg/test_paths.py
--rw-r--r--   0        0        0     7333 2023-03-29 18:33:03.507477 weasyprint-59.0/tests/draw/svg/test_patterns.py
--rw-r--r--   0        0        0    10177 2023-03-29 18:33:03.507477 weasyprint-59.0/tests/draw/svg/test_shapes.py
--rw-r--r--   0        0        0     8940 2023-03-29 18:33:03.507477 weasyprint-59.0/tests/draw/svg/test_text.py
--rw-r--r--   0        0        0     9861 2023-03-29 18:33:03.508477 weasyprint-59.0/tests/draw/svg/test_transform.py
--rw-r--r--   0        0        0     2317 2023-03-29 18:33:03.508477 weasyprint-59.0/tests/draw/svg/test_units.py
--rw-r--r--   0        0        0     4525 2023-03-29 18:33:03.508477 weasyprint-59.0/tests/draw/svg/test_visibility.py
--rw-r--r--   0        0        0    18191 2023-03-29 18:33:03.508477 weasyprint-59.0/tests/draw/test_absolute.py
--rw-r--r--   0        0        0    26656 2023-03-29 18:33:03.509477 weasyprint-59.0/tests/draw/test_background.py
--rw-r--r--   0        0        0     2078 2023-03-06 15:20:25.290055 weasyprint-59.0/tests/draw/test_before_after.py
--rw-r--r--   0        0        0     6270 2023-03-06 15:32:25.179425 weasyprint-59.0/tests/draw/test_box.py
--rw-r--r--   0        0        0     2085 2023-03-06 15:32:25.179425 weasyprint-59.0/tests/draw/test_column.py
--rw-r--r--   0        0        0     2152 2023-03-06 15:32:25.179425 weasyprint-59.0/tests/draw/test_current_color.py
--rw-r--r--   0        0        0    21996 2023-03-29 18:33:03.509477 weasyprint-59.0/tests/draw/test_float.py
--rw-r--r--   0        0        0     8144 2023-03-06 15:32:25.179425 weasyprint-59.0/tests/draw/test_footnote.py
--rw-r--r--   0        0        0     9233 2023-03-06 15:32:25.179425 weasyprint-59.0/tests/draw/test_footnote_column.py
--rw-r--r--   0        0        0     6259 2023-03-06 15:32:25.179425 weasyprint-59.0/tests/draw/test_gradient.py
--rw-r--r--   0        0        0    14997 2023-03-06 15:32:25.179425 weasyprint-59.0/tests/draw/test_image.py
--rw-r--r--   0        0        0    10467 2023-03-06 15:20:25.290055 weasyprint-59.0/tests/draw/test_leader.py
--rw-r--r--   0        0        0     1970 2023-03-06 15:20:25.291055 weasyprint-59.0/tests/draw/test_list.py
--rw-r--r--   0        0        0     1082 2023-03-06 15:20:25.291055 weasyprint-59.0/tests/draw/test_opacity.py
--rw-r--r--   0        0        0     4229 2023-03-06 15:20:25.291055 weasyprint-59.0/tests/draw/test_overflow.py
--rw-r--r--   0        0        0      739 2023-03-06 15:20:25.291055 weasyprint-59.0/tests/draw/test_page.py
--rw-r--r--   0        0        0    43002 2023-03-29 18:33:03.509477 weasyprint-59.0/tests/draw/test_table.py
--rw-r--r--   0        0        0    19952 2023-05-11 08:53:40.164397 weasyprint-59.0/tests/draw/test_text.py
--rw-r--r--   0        0        0     7009 2023-03-06 15:20:25.291055 weasyprint-59.0/tests/draw/test_transform.py
--rw-r--r--   0        0        0     1492 2023-03-06 15:20:25.291055 weasyprint-59.0/tests/draw/test_visibility.py
--rw-r--r--   0        0        0     6055 2023-03-06 15:32:25.180425 weasyprint-59.0/tests/draw/test_whitespace.py
--rw-r--r--   0        0        0      101 2022-11-14 22:25:38.227017 weasyprint-59.0/tests/layout/__init__.py
--rw-r--r--   0        0        0    29787 2023-03-06 15:32:25.180425 weasyprint-59.0/tests/layout/test_block.py
--rw-r--r--   0        0        0    35252 2022-11-14 22:25:38.230017 weasyprint-59.0/tests/layout/test_column.py
--rw-r--r--   0        0        0    17077 2022-11-14 22:25:38.230017 weasyprint-59.0/tests/layout/test_flex.py
--rw-r--r--   0        0        0    24661 2023-03-06 15:32:25.180425 weasyprint-59.0/tests/layout/test_footnotes.py
--rw-r--r--   0        0        0    19528 2023-03-06 15:20:25.292055 weasyprint-59.0/tests/layout/test_image.py
--rw-r--r--   0        0        0    35015 2023-03-06 15:32:25.180425 weasyprint-59.0/tests/layout/test_inline.py
--rw-r--r--   0        0        0     3747 2022-11-14 22:25:38.230017 weasyprint-59.0/tests/layout/test_inline_block.py
--rw-r--r--   0        0        0     3739 2023-03-06 15:32:25.180425 weasyprint-59.0/tests/layout/test_list.py
--rw-r--r--   0        0        0    43675 2023-03-06 15:32:25.180425 weasyprint-59.0/tests/layout/test_page.py
--rw-r--r--   0        0        0    15572 2023-03-29 18:33:03.510477 weasyprint-59.0/tests/layout/test_position.py
--rw-r--r--   0        0        0     1697 2022-11-14 22:25:38.231017 weasyprint-59.0/tests/layout/test_shrink_to_fit.py
--rw-r--r--   0        0        0    85568 2023-03-06 15:32:25.181425 weasyprint-59.0/tests/layout/test_table.py
--rw-r--r--   0        0        0     2556 2022-11-14 22:25:38.231017 weasyprint-59.0/tests/resources/acid2-reference.html
--rw-r--r--   0        0        0    14267 2022-11-14 22:25:38.231017 weasyprint-59.0/tests/resources/acid2-test.html
--rw-r--r--   0        0        0      289 2022-11-14 22:25:38.231017 weasyprint-59.0/tests/resources/blue.jpg
--rw-r--r--   0        0        0     2109 2022-11-14 22:25:38.231017 weasyprint-59.0/tests/resources/doc1.html
--rw-r--r--   0        0        0      804 2022-11-14 22:25:38.232017 weasyprint-59.0/tests/resources/doc1_UTF-16BE.html
--rw-r--r--   0        0        0      814 2022-11-14 22:25:38.232017 weasyprint-59.0/tests/resources/icon.png
--rw-r--r--   0        0        0       85 2022-11-14 22:25:38.232017 weasyprint-59.0/tests/resources/latin1-test.css
--rw-r--r--   0        0        0     6523 2022-11-14 22:25:38.232017 weasyprint-59.0/tests/resources/logo_small.png
--rw-r--r--   0        0        0      153 2022-11-14 22:25:38.232017 weasyprint-59.0/tests/resources/mini_ua.css
--rw-r--r--   0        0        0      805 2023-03-06 15:32:25.181425 weasyprint-59.0/tests/resources/not-optimized-exif.jpg
--rw-r--r--   0        0        0      704 2022-11-14 22:25:38.232017 weasyprint-59.0/tests/resources/not-optimized.jpg
--rw-r--r--   0        0        0       45 2022-11-14 22:25:38.232017 weasyprint-59.0/tests/resources/pattern.gif
--rw-r--r--   0        0        0      140 2022-11-14 22:25:38.232017 weasyprint-59.0/tests/resources/pattern.palette.png
--rw-r--r--   0        0        0       76 2022-11-14 22:25:38.232017 weasyprint-59.0/tests/resources/pattern.png
--rw-r--r--   0        0        0      203 2022-11-14 22:25:38.232017 weasyprint-59.0/tests/resources/pattern.svg
--rw-r--r--   0        0        0       76 2022-11-14 22:25:38.232017 weasyprint-59.0/tests/resources/really-a-png.svg
--rw-r--r--   0        0        0      203 2022-11-14 22:25:38.232017 weasyprint-59.0/tests/resources/really-a-svg.png
--rw-r--r--   0        0        0      120 2022-11-14 22:25:38.232017 weasyprint-59.0/tests/resources/sheet2.css
--rw-r--r--   0        0        0      249 2022-11-14 22:25:38.232017 weasyprint-59.0/tests/resources/sub_directory/sheet1.css
--rw-r--r--   0        0        0       84 2022-11-14 22:25:38.232017 weasyprint-59.0/tests/resources/user.css
--rw-r--r--   0        0        0       88 2022-11-14 22:25:38.232017 weasyprint-59.0/tests/resources/utf8-test.css
--rw-r--r--   0        0        0     1568 2023-03-06 15:20:25.293055 weasyprint-59.0/tests/resources/weasyprint.otb
--rw-r--r--   0        0        0    12744 2022-11-14 22:25:38.232017 weasyprint-59.0/tests/resources/weasyprint.otf
--rw-r--r--   0        0        0     3512 2022-11-14 22:25:38.232017 weasyprint-59.0/tests/resources/weasyprint.woff
--rw-r--r--   0        0        0     1131 2023-03-06 15:32:25.181425 weasyprint-59.0/tests/test_acid2.py
--rw-r--r--   0        0        0    41493 2023-04-14 12:31:37.912026 weasyprint-59.0/tests/test_api.py
--rw-r--r--   0        0        0    39942 2023-03-06 15:32:25.181425 weasyprint-59.0/tests/test_boxes.py
--rw-r--r--   0        0        0    20051 2023-03-06 15:32:25.181425 weasyprint-59.0/tests/test_counters.py
--rw-r--r--   0        0        0    17622 2023-03-29 18:33:03.511477 weasyprint-59.0/tests/test_css.py
--rw-r--r--   0        0        0     7851 2023-03-06 15:32:25.181425 weasyprint-59.0/tests/test_css_descriptors.py
--rw-r--r--   0        0        0    44261 2023-03-06 15:32:25.182425 weasyprint-59.0/tests/test_css_validation.py
--rw-r--r--   0        0        0    20732 2023-04-22 21:27:49.220186 weasyprint-59.0/tests/test_float.py
--rw-r--r--   0        0        0     4966 2022-11-14 22:25:38.234017 weasyprint-59.0/tests/test_fonts.py
--rw-r--r--   0        0        0    22050 2023-04-14 12:31:21.692807 weasyprint-59.0/tests/test_pdf.py
--rw-r--r--   0        0        0     9480 2022-11-14 22:25:38.234017 weasyprint-59.0/tests/test_presentational_hints.py
--rw-r--r--   0        0        0     2227 2023-03-06 15:20:25.294055 weasyprint-59.0/tests/test_stacking.py
--rw-r--r--   0        0        0     6189 2023-03-06 15:32:25.182425 weasyprint-59.0/tests/test_target.py
--rw-r--r--   0        0        0    42914 2023-04-12 15:06:54.898471 weasyprint-59.0/tests/test_text.py
--rw-r--r--   0        0        0     1648 2023-03-06 15:20:25.294055 weasyprint-59.0/tests/test_unicode.py
--rw-r--r--   0        0        0     3181 2023-03-06 15:20:25.294055 weasyprint-59.0/tests/test_variables.py
--rw-r--r--   0        0        0     9311 2023-04-14 14:06:57.625262 weasyprint-59.0/tests/testing_utils.py
--rw-r--r--   0        0        0    15640 2023-05-11 09:25:32.468751 weasyprint-59.0/weasyprint/__init__.py
--rw-r--r--   0        0        0     7555 2023-04-14 13:04:00.612377 weasyprint-59.0/weasyprint/__main__.py
--rw-r--r--   0        0        0     5988 2023-03-29 18:33:03.513477 weasyprint-59.0/weasyprint/anchors.py
--rw-r--r--   0        0        0    49314 2023-03-29 18:33:03.513477 weasyprint-59.0/weasyprint/css/__init__.py
--rw-r--r--   0        0        0    27436 2023-03-29 18:33:03.514477 weasyprint-59.0/weasyprint/css/computed_values.py
--rw-r--r--   0        0        0    11373 2022-11-14 22:25:38.256017 weasyprint-59.0/weasyprint/css/counters.py
--rw-r--r--   0        0        0     7407 2022-11-14 22:25:38.256017 weasyprint-59.0/weasyprint/css/html5_ph.css
--rw-r--r--   0        0        0    40755 2023-03-29 18:33:03.514477 weasyprint-59.0/weasyprint/css/html5_ua.css
--rw-r--r--   0        0        0       96 2023-03-29 18:33:03.514477 weasyprint-59.0/weasyprint/css/html5_ua_form.css
--rw-r--r--   0        0        0     1072 2022-11-14 22:25:38.257017 weasyprint-59.0/weasyprint/css/media_queries.py
--rw-r--r--   0        0        0    10186 2023-03-29 18:33:03.515477 weasyprint-59.0/weasyprint/css/properties.py
--rw-r--r--   0        0        0     8853 2023-03-06 15:32:25.183425 weasyprint-59.0/weasyprint/css/targets.py
--rw-r--r--   0        0        0     1630 2022-11-14 22:25:38.257017 weasyprint-59.0/weasyprint/css/tests_ua.css
--rw-r--r--   0        0        0    23770 2023-03-06 15:32:25.183425 weasyprint-59.0/weasyprint/css/utils.py
--rw-r--r--   0        0        0     4042 2022-11-14 22:25:38.257017 weasyprint-59.0/weasyprint/css/validation/__init__.py
--rw-r--r--   0        0        0    10905 2023-03-06 15:32:25.183425 weasyprint-59.0/weasyprint/css/validation/descriptors.py
--rw-r--r--   0        0        0    24748 2023-03-06 15:32:25.183425 weasyprint-59.0/weasyprint/css/validation/expanders.py
--rw-r--r--   0        0        0    47315 2023-03-29 18:33:03.515477 weasyprint-59.0/weasyprint/css/validation/properties.py
--rw-r--r--   0        0        0    17135 2023-04-14 14:01:46.252102 weasyprint-59.0/weasyprint/document.py
--rw-r--r--   0        0        0    51370 2023-05-11 08:46:30.124406 weasyprint-59.0/weasyprint/draw.py
--rw-r--r--   0        0        0    24104 2023-04-22 20:36:44.828750 weasyprint-59.0/weasyprint/formatting_structure/boxes.py
--rw-r--r--   0        0        0    61787 2023-03-29 18:33:03.518477 weasyprint-59.0/weasyprint/formatting_structure/build.py
--rw-r--r--   0        0        0    11492 2023-04-14 12:31:21.694807 weasyprint-59.0/weasyprint/html.py
--rw-r--r--   0        0        0    34099 2023-05-08 19:32:38.600652 weasyprint-59.0/weasyprint/images.py
--rw-r--r--   0        0        0    15614 2023-04-14 12:31:21.695807 weasyprint-59.0/weasyprint/layout/__init__.py
--rw-r--r--   0        0        0    13681 2023-03-29 18:33:03.520477 weasyprint-59.0/weasyprint/layout/absolute.py
--rw-r--r--   0        0        0     9003 2023-03-06 15:32:25.185425 weasyprint-59.0/weasyprint/layout/background.py
--rw-r--r--   0        0        0    43976 2023-03-29 18:33:03.520477 weasyprint-59.0/weasyprint/layout/block.py
--rw-r--r--   0        0        0    17028 2023-04-22 20:05:02.618072 weasyprint-59.0/weasyprint/layout/column.py
--rw-r--r--   0        0        0    38558 2023-03-06 15:32:25.186425 weasyprint-59.0/weasyprint/layout/flex.py
--rw-r--r--   0        0        0     8756 2023-04-29 11:57:54.459868 weasyprint-59.0/weasyprint/layout/float.py
--rw-r--r--   0        0        0    47911 2023-04-29 11:57:54.459868 weasyprint-59.0/weasyprint/layout/inline.py
--rw-r--r--   0        0        0     2816 2022-11-14 22:25:38.288018 weasyprint-59.0/weasyprint/layout/leader.py
--rw-r--r--   0        0        0     1527 2022-11-14 22:25:38.288018 weasyprint-59.0/weasyprint/layout/min_max.py
--rw-r--r--   0        0        0    35142 2023-04-14 12:31:21.696807 weasyprint-59.0/weasyprint/layout/page.py
--rw-r--r--   0        0        0     5940 2023-03-06 15:32:25.186425 weasyprint-59.0/weasyprint/layout/percent.py
--rw-r--r--   0        0        0    29564 2023-04-12 15:06:54.900471 weasyprint-59.0/weasyprint/layout/preferred.py
--rw-r--r--   0        0        0    11178 2023-03-06 15:32:25.187425 weasyprint-59.0/weasyprint/layout/replaced.py
--rw-r--r--   0        0        0    40754 2023-03-06 15:32:25.187425 weasyprint-59.0/weasyprint/layout/table.py
--rw-r--r--   0        0        0      803 2022-11-14 22:25:38.289018 weasyprint-59.0/weasyprint/logger.py
--rw-r--r--   0        0        0     1909 2022-11-20 12:51:28.692242 weasyprint-59.0/weasyprint/matrix.py
--rw-r--r--   0        0        0    10604 2023-05-08 19:25:04.028979 weasyprint-59.0/weasyprint/pdf/__init__.py
--rw-r--r--   0        0        0    13252 2023-05-08 19:25:04.029980 weasyprint-59.0/weasyprint/pdf/anchors.py
--rw-r--r--   0        0        0    12739 2023-04-14 12:31:21.697807 weasyprint-59.0/weasyprint/pdf/fonts.py
--rw-r--r--   0        0        0     3907 2023-04-12 15:06:57.526514 weasyprint-59.0/weasyprint/pdf/metadata.py
--rw-r--r--   0        0        0     1684 2023-04-12 15:06:57.526514 weasyprint-59.0/weasyprint/pdf/pdfa.py
--rw-r--r--   0        0        0     5456 2023-04-12 15:06:57.526514 weasyprint-59.0/weasyprint/pdf/pdfua.py
--rw-r--r--   0        0        0     3024 2023-03-06 15:20:25.299055 weasyprint-59.0/weasyprint/pdf/sRGB2014.icc
--rw-r--r--   0        0        0    18357 2023-05-08 19:31:17.792815 weasyprint-59.0/weasyprint/pdf/stream.py
--rw-r--r--   0        0        0     5506 2023-03-06 15:32:25.188425 weasyprint-59.0/weasyprint/stacking.py
--rw-r--r--   0        0        0    27650 2023-05-08 19:25:04.029980 weasyprint-59.0/weasyprint/svg/__init__.py
--rw-r--r--   0        0        0    12690 2023-03-06 15:32:25.188425 weasyprint-59.0/weasyprint/svg/bounding_box.py
--rw-r--r--   0        0        0     3833 2023-03-06 15:32:25.188425 weasyprint-59.0/weasyprint/svg/css.py
--rw-r--r--   0        0        0    21088 2023-05-08 19:25:04.030979 weasyprint-59.0/weasyprint/svg/defs.py
--rw-r--r--   0        0        0     2503 2023-05-08 19:25:04.030979 weasyprint-59.0/weasyprint/svg/images.py
--rw-r--r--   0        0        0    10064 2023-04-29 12:31:07.478191 weasyprint-59.0/weasyprint/svg/path.py
--rw-r--r--   0        0        0     3845 2023-04-29 12:31:07.478191 weasyprint-59.0/weasyprint/svg/shapes.py
--rw-r--r--   0        0        0     6095 2023-04-29 12:31:07.478191 weasyprint-59.0/weasyprint/svg/text.py
--rw-r--r--   0        0        0     6644 2023-03-29 18:33:03.524477 weasyprint-59.0/weasyprint/svg/utils.py
--rw-r--r--   0        0        0     7498 2023-03-06 15:20:25.300055 weasyprint-59.0/weasyprint/text/constants.py
--rw-r--r--   0        0        0    15189 2023-03-29 18:33:03.525477 weasyprint-59.0/weasyprint/text/ffi.py
--rw-r--r--   0        0        0    14918 2023-03-29 18:33:03.525477 weasyprint-59.0/weasyprint/text/fonts.py
--rw-r--r--   0        0        0    23959 2023-04-14 12:31:21.697807 weasyprint-59.0/weasyprint/text/line_break.py
--rw-r--r--   0        0        0     9636 2023-04-14 12:31:21.697807 weasyprint-59.0/weasyprint/urls.py
--rw-r--r--   0        0        0     3745 1970-01-01 00:00:00.000000 weasyprint-59.0/PKG-INFO
+-rw-r--r--   0        0        0     1534 2022-11-12 08:45:13.781084 weasyprint-59.0b1/LICENSE
+-rw-r--r--   0        0        0     1636 2023-03-29 18:33:03.496477 weasyprint-59.0b1/README.rst
+-rw-r--r--   0        0        0    30741 2023-04-14 12:31:21.691807 weasyprint-59.0b1/docs/api_reference.rst
+-rw-r--r--   0        0        0    92665 2023-04-14 14:53:05.753391 weasyprint-59.0b1/docs/changelog.rst
+-rw-r--r--   0        0        0     4756 2023-03-06 15:20:25.288055 weasyprint-59.0b1/docs/common_use_cases.rst
+-rw-r--r--   0        0        0     2705 2023-03-06 15:32:25.177425 weasyprint-59.0b1/docs/conf.py
+-rw-r--r--   0        0        0     1956 2023-03-06 15:32:25.178425 weasyprint-59.0b1/docs/contribute.rst
+-rw-r--r--   0        0        0    23809 2023-04-12 15:06:57.523514 weasyprint-59.0b1/docs/first_steps.rst
+-rw-r--r--   0        0        0    11753 2023-03-06 15:32:25.178425 weasyprint-59.0b1/docs/going_further.rst
+-rw-r--r--   0        0        0      308 2022-11-14 22:25:38.213016 weasyprint-59.0b1/docs/index.rst
+-rw-r--r--   0        0        0      180 2023-03-06 15:32:25.178425 weasyprint-59.0b1/docs/manpage.rst
+-rw-r--r--   0        0        0      882 2022-11-14 22:25:38.213016 weasyprint-59.0b1/docs/support.rst
+-rw-r--r--   0        0        0     2306 2023-04-12 15:06:57.524514 weasyprint-59.0b1/pyproject.toml
+-rw-r--r--   0        0        0       33 2022-11-14 22:25:38.214017 weasyprint-59.0b1/tests/__init__.py
+-rw-r--r--   0        0        0     3516 2023-04-14 12:31:21.691807 weasyprint-59.0b1/tests/conftest.py
+-rw-r--r--   0        0        0     5063 2023-03-06 15:32:25.178425 weasyprint-59.0b1/tests/draw/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-14 22:25:38.223017 weasyprint-59.0b1/tests/draw/svg/__init__.py
+-rw-r--r--   0        0        0     8388 2023-03-29 18:33:03.506477 weasyprint-59.0b1/tests/draw/svg/test_bounding_box.py
+-rw-r--r--   0        0        0     2384 2023-03-29 18:33:03.506477 weasyprint-59.0b1/tests/draw/svg/test_clip.py
+-rw-r--r--   0        0        0     1014 2023-03-29 18:33:03.506477 weasyprint-59.0b1/tests/draw/svg/test_defs.py
+-rw-r--r--   0        0        0    28515 2023-03-29 18:33:03.506477 weasyprint-59.0b1/tests/draw/svg/test_gradients.py
+-rw-r--r--   0        0        0     6647 2023-03-29 18:33:03.506477 weasyprint-59.0b1/tests/draw/svg/test_images.py
+-rw-r--r--   0        0        0     5052 2023-03-29 18:33:03.507477 weasyprint-59.0b1/tests/draw/svg/test_opacity.py
+-rw-r--r--   0        0        0    15490 2023-03-29 18:33:03.507477 weasyprint-59.0b1/tests/draw/svg/test_paths.py
+-rw-r--r--   0        0        0     7333 2023-03-29 18:33:03.507477 weasyprint-59.0b1/tests/draw/svg/test_patterns.py
+-rw-r--r--   0        0        0    10177 2023-03-29 18:33:03.507477 weasyprint-59.0b1/tests/draw/svg/test_shapes.py
+-rw-r--r--   0        0        0     8940 2023-03-29 18:33:03.507477 weasyprint-59.0b1/tests/draw/svg/test_text.py
+-rw-r--r--   0        0        0     9861 2023-03-29 18:33:03.508477 weasyprint-59.0b1/tests/draw/svg/test_transform.py
+-rw-r--r--   0        0        0     2317 2023-03-29 18:33:03.508477 weasyprint-59.0b1/tests/draw/svg/test_units.py
+-rw-r--r--   0        0        0     4525 2023-03-29 18:33:03.508477 weasyprint-59.0b1/tests/draw/svg/test_visibility.py
+-rw-r--r--   0        0        0    18191 2023-03-29 18:33:03.508477 weasyprint-59.0b1/tests/draw/test_absolute.py
+-rw-r--r--   0        0        0    26656 2023-03-29 18:33:03.509477 weasyprint-59.0b1/tests/draw/test_background.py
+-rw-r--r--   0        0        0     2078 2023-03-06 15:20:25.290055 weasyprint-59.0b1/tests/draw/test_before_after.py
+-rw-r--r--   0        0        0     6270 2023-03-06 15:32:25.179425 weasyprint-59.0b1/tests/draw/test_box.py
+-rw-r--r--   0        0        0     2085 2023-03-06 15:32:25.179425 weasyprint-59.0b1/tests/draw/test_column.py
+-rw-r--r--   0        0        0     2152 2023-03-06 15:32:25.179425 weasyprint-59.0b1/tests/draw/test_current_color.py
+-rw-r--r--   0        0        0    21996 2023-03-29 18:33:03.509477 weasyprint-59.0b1/tests/draw/test_float.py
+-rw-r--r--   0        0        0     8144 2023-03-06 15:32:25.179425 weasyprint-59.0b1/tests/draw/test_footnote.py
+-rw-r--r--   0        0        0     9233 2023-03-06 15:32:25.179425 weasyprint-59.0b1/tests/draw/test_footnote_column.py
+-rw-r--r--   0        0        0     6259 2023-03-06 15:32:25.179425 weasyprint-59.0b1/tests/draw/test_gradient.py
+-rw-r--r--   0        0        0    14997 2023-03-06 15:32:25.179425 weasyprint-59.0b1/tests/draw/test_image.py
+-rw-r--r--   0        0        0    10467 2023-03-06 15:20:25.290055 weasyprint-59.0b1/tests/draw/test_leader.py
+-rw-r--r--   0        0        0     1970 2023-03-06 15:20:25.291055 weasyprint-59.0b1/tests/draw/test_list.py
+-rw-r--r--   0        0        0     1082 2023-03-06 15:20:25.291055 weasyprint-59.0b1/tests/draw/test_opacity.py
+-rw-r--r--   0        0        0     4229 2023-03-06 15:20:25.291055 weasyprint-59.0b1/tests/draw/test_overflow.py
+-rw-r--r--   0        0        0      739 2023-03-06 15:20:25.291055 weasyprint-59.0b1/tests/draw/test_page.py
+-rw-r--r--   0        0        0    43002 2023-03-29 18:33:03.509477 weasyprint-59.0b1/tests/draw/test_table.py
+-rw-r--r--   0        0        0    19867 2023-03-06 15:32:25.179425 weasyprint-59.0b1/tests/draw/test_text.py
+-rw-r--r--   0        0        0     7009 2023-03-06 15:20:25.291055 weasyprint-59.0b1/tests/draw/test_transform.py
+-rw-r--r--   0        0        0     1492 2023-03-06 15:20:25.291055 weasyprint-59.0b1/tests/draw/test_visibility.py
+-rw-r--r--   0        0        0     6055 2023-03-06 15:32:25.180425 weasyprint-59.0b1/tests/draw/test_whitespace.py
+-rw-r--r--   0        0        0      101 2022-11-14 22:25:38.227017 weasyprint-59.0b1/tests/layout/__init__.py
+-rw-r--r--   0        0        0    29787 2023-03-06 15:32:25.180425 weasyprint-59.0b1/tests/layout/test_block.py
+-rw-r--r--   0        0        0    35252 2022-11-14 22:25:38.230017 weasyprint-59.0b1/tests/layout/test_column.py
+-rw-r--r--   0        0        0    17077 2022-11-14 22:25:38.230017 weasyprint-59.0b1/tests/layout/test_flex.py
+-rw-r--r--   0        0        0    24661 2023-03-06 15:32:25.180425 weasyprint-59.0b1/tests/layout/test_footnotes.py
+-rw-r--r--   0        0        0    19528 2023-03-06 15:20:25.292055 weasyprint-59.0b1/tests/layout/test_image.py
+-rw-r--r--   0        0        0    35015 2023-03-06 15:32:25.180425 weasyprint-59.0b1/tests/layout/test_inline.py
+-rw-r--r--   0        0        0     3747 2022-11-14 22:25:38.230017 weasyprint-59.0b1/tests/layout/test_inline_block.py
+-rw-r--r--   0        0        0     3739 2023-03-06 15:32:25.180425 weasyprint-59.0b1/tests/layout/test_list.py
+-rw-r--r--   0        0        0    43675 2023-03-06 15:32:25.180425 weasyprint-59.0b1/tests/layout/test_page.py
+-rw-r--r--   0        0        0    15572 2023-03-29 18:33:03.510477 weasyprint-59.0b1/tests/layout/test_position.py
+-rw-r--r--   0        0        0     1697 2022-11-14 22:25:38.231017 weasyprint-59.0b1/tests/layout/test_shrink_to_fit.py
+-rw-r--r--   0        0        0    85568 2023-03-06 15:32:25.181425 weasyprint-59.0b1/tests/layout/test_table.py
+-rw-r--r--   0        0        0     2556 2022-11-14 22:25:38.231017 weasyprint-59.0b1/tests/resources/acid2-reference.html
+-rw-r--r--   0        0        0    14267 2022-11-14 22:25:38.231017 weasyprint-59.0b1/tests/resources/acid2-test.html
+-rw-r--r--   0        0        0      289 2022-11-14 22:25:38.231017 weasyprint-59.0b1/tests/resources/blue.jpg
+-rw-r--r--   0        0        0     2109 2022-11-14 22:25:38.231017 weasyprint-59.0b1/tests/resources/doc1.html
+-rw-r--r--   0        0        0      804 2022-11-14 22:25:38.232017 weasyprint-59.0b1/tests/resources/doc1_UTF-16BE.html
+-rw-r--r--   0        0        0      814 2022-11-14 22:25:38.232017 weasyprint-59.0b1/tests/resources/icon.png
+-rw-r--r--   0        0        0       85 2022-11-14 22:25:38.232017 weasyprint-59.0b1/tests/resources/latin1-test.css
+-rw-r--r--   0        0        0     6523 2022-11-14 22:25:38.232017 weasyprint-59.0b1/tests/resources/logo_small.png
+-rw-r--r--   0        0        0      153 2022-11-14 22:25:38.232017 weasyprint-59.0b1/tests/resources/mini_ua.css
+-rw-r--r--   0        0        0      805 2023-03-06 15:32:25.181425 weasyprint-59.0b1/tests/resources/not-optimized-exif.jpg
+-rw-r--r--   0        0        0      704 2022-11-14 22:25:38.232017 weasyprint-59.0b1/tests/resources/not-optimized.jpg
+-rw-r--r--   0        0        0       45 2022-11-14 22:25:38.232017 weasyprint-59.0b1/tests/resources/pattern.gif
+-rw-r--r--   0        0        0      140 2022-11-14 22:25:38.232017 weasyprint-59.0b1/tests/resources/pattern.palette.png
+-rw-r--r--   0        0        0       76 2022-11-14 22:25:38.232017 weasyprint-59.0b1/tests/resources/pattern.png
+-rw-r--r--   0        0        0      203 2022-11-14 22:25:38.232017 weasyprint-59.0b1/tests/resources/pattern.svg
+-rw-r--r--   0        0        0       76 2022-11-14 22:25:38.232017 weasyprint-59.0b1/tests/resources/really-a-png.svg
+-rw-r--r--   0        0        0      203 2022-11-14 22:25:38.232017 weasyprint-59.0b1/tests/resources/really-a-svg.png
+-rw-r--r--   0        0        0      120 2022-11-14 22:25:38.232017 weasyprint-59.0b1/tests/resources/sheet2.css
+-rw-r--r--   0        0        0      249 2022-11-14 22:25:38.232017 weasyprint-59.0b1/tests/resources/sub_directory/sheet1.css
+-rw-r--r--   0        0        0       84 2022-11-14 22:25:38.232017 weasyprint-59.0b1/tests/resources/user.css
+-rw-r--r--   0        0        0       88 2022-11-14 22:25:38.232017 weasyprint-59.0b1/tests/resources/utf8-test.css
+-rw-r--r--   0        0        0     1568 2023-03-06 15:20:25.293055 weasyprint-59.0b1/tests/resources/weasyprint.otb
+-rw-r--r--   0        0        0    12744 2022-11-14 22:25:38.232017 weasyprint-59.0b1/tests/resources/weasyprint.otf
+-rw-r--r--   0        0        0     3512 2022-11-14 22:25:38.232017 weasyprint-59.0b1/tests/resources/weasyprint.woff
+-rw-r--r--   0        0        0     1131 2023-03-06 15:32:25.181425 weasyprint-59.0b1/tests/test_acid2.py
+-rw-r--r--   0        0        0    41493 2023-04-14 12:31:37.912026 weasyprint-59.0b1/tests/test_api.py
+-rw-r--r--   0        0        0    39942 2023-03-06 15:32:25.181425 weasyprint-59.0b1/tests/test_boxes.py
+-rw-r--r--   0        0        0    20051 2023-03-06 15:32:25.181425 weasyprint-59.0b1/tests/test_counters.py
+-rw-r--r--   0        0        0    17622 2023-03-29 18:33:03.511477 weasyprint-59.0b1/tests/test_css.py
+-rw-r--r--   0        0        0     7851 2023-03-06 15:32:25.181425 weasyprint-59.0b1/tests/test_css_descriptors.py
+-rw-r--r--   0        0        0    44261 2023-03-06 15:32:25.182425 weasyprint-59.0b1/tests/test_css_validation.py
+-rw-r--r--   0        0        0    20732 2023-03-06 15:20:25.294055 weasyprint-59.0b1/tests/test_float.py
+-rw-r--r--   0        0        0     4966 2022-11-14 22:25:38.234017 weasyprint-59.0b1/tests/test_fonts.py
+-rw-r--r--   0        0        0    22050 2023-04-14 12:31:21.692807 weasyprint-59.0b1/tests/test_pdf.py
+-rw-r--r--   0        0        0     9480 2022-11-14 22:25:38.234017 weasyprint-59.0b1/tests/test_presentational_hints.py
+-rw-r--r--   0        0        0     2227 2023-03-06 15:20:25.294055 weasyprint-59.0b1/tests/test_stacking.py
+-rw-r--r--   0        0        0     6189 2023-03-06 15:32:25.182425 weasyprint-59.0b1/tests/test_target.py
+-rw-r--r--   0        0        0    42914 2023-04-12 15:06:54.898471 weasyprint-59.0b1/tests/test_text.py
+-rw-r--r--   0        0        0     1648 2023-03-06 15:20:25.294055 weasyprint-59.0b1/tests/test_unicode.py
+-rw-r--r--   0        0        0     3181 2023-03-06 15:20:25.294055 weasyprint-59.0b1/tests/test_variables.py
+-rw-r--r--   0        0        0     9311 2023-04-14 14:06:57.625262 weasyprint-59.0b1/tests/testing_utils.py
+-rw-r--r--   0        0        0    15642 2023-04-14 13:55:17.740479 weasyprint-59.0b1/weasyprint/__init__.py
+-rw-r--r--   0        0        0     7555 2023-04-14 13:04:00.612377 weasyprint-59.0b1/weasyprint/__main__.py
+-rw-r--r--   0        0        0     5988 2023-03-29 18:33:03.513477 weasyprint-59.0b1/weasyprint/anchors.py
+-rw-r--r--   0        0        0    49314 2023-03-29 18:33:03.513477 weasyprint-59.0b1/weasyprint/css/__init__.py
+-rw-r--r--   0        0        0    27436 2023-03-29 18:33:03.514477 weasyprint-59.0b1/weasyprint/css/computed_values.py
+-rw-r--r--   0        0        0    11373 2022-11-14 22:25:38.256017 weasyprint-59.0b1/weasyprint/css/counters.py
+-rw-r--r--   0        0        0     7407 2022-11-14 22:25:38.256017 weasyprint-59.0b1/weasyprint/css/html5_ph.css
+-rw-r--r--   0        0        0    40755 2023-03-29 18:33:03.514477 weasyprint-59.0b1/weasyprint/css/html5_ua.css
+-rw-r--r--   0        0        0       96 2023-03-29 18:33:03.514477 weasyprint-59.0b1/weasyprint/css/html5_ua_form.css
+-rw-r--r--   0        0        0     1072 2022-11-14 22:25:38.257017 weasyprint-59.0b1/weasyprint/css/media_queries.py
+-rw-r--r--   0        0        0    10186 2023-03-29 18:33:03.515477 weasyprint-59.0b1/weasyprint/css/properties.py
+-rw-r--r--   0        0        0     8853 2023-03-06 15:32:25.183425 weasyprint-59.0b1/weasyprint/css/targets.py
+-rw-r--r--   0        0        0     1630 2022-11-14 22:25:38.257017 weasyprint-59.0b1/weasyprint/css/tests_ua.css
+-rw-r--r--   0        0        0    23770 2023-03-06 15:32:25.183425 weasyprint-59.0b1/weasyprint/css/utils.py
+-rw-r--r--   0        0        0     4042 2022-11-14 22:25:38.257017 weasyprint-59.0b1/weasyprint/css/validation/__init__.py
+-rw-r--r--   0        0        0    10905 2023-03-06 15:32:25.183425 weasyprint-59.0b1/weasyprint/css/validation/descriptors.py
+-rw-r--r--   0        0        0    24748 2023-03-06 15:32:25.183425 weasyprint-59.0b1/weasyprint/css/validation/expanders.py
+-rw-r--r--   0        0        0    47315 2023-03-29 18:33:03.515477 weasyprint-59.0b1/weasyprint/css/validation/properties.py
+-rw-r--r--   0        0        0    17135 2023-04-14 14:01:46.252102 weasyprint-59.0b1/weasyprint/document.py
+-rw-r--r--   0        0        0    51200 2023-04-12 15:06:57.525514 weasyprint-59.0b1/weasyprint/draw.py
+-rw-r--r--   0        0        0    24104 2023-03-29 18:33:03.517477 weasyprint-59.0b1/weasyprint/formatting_structure/boxes.py
+-rw-r--r--   0        0        0    61787 2023-03-29 18:33:03.518477 weasyprint-59.0b1/weasyprint/formatting_structure/build.py
+-rw-r--r--   0        0        0    11492 2023-04-14 12:31:21.694807 weasyprint-59.0b1/weasyprint/html.py
+-rw-r--r--   0        0        0    34642 2023-04-14 12:31:21.695807 weasyprint-59.0b1/weasyprint/images.py
+-rw-r--r--   0        0        0    15614 2023-04-14 12:31:21.695807 weasyprint-59.0b1/weasyprint/layout/__init__.py
+-rw-r--r--   0        0        0    13681 2023-03-29 18:33:03.520477 weasyprint-59.0b1/weasyprint/layout/absolute.py
+-rw-r--r--   0        0        0     9003 2023-03-06 15:32:25.185425 weasyprint-59.0b1/weasyprint/layout/background.py
+-rw-r--r--   0        0        0    43976 2023-03-29 18:33:03.520477 weasyprint-59.0b1/weasyprint/layout/block.py
+-rw-r--r--   0        0        0    17028 2023-04-12 08:20:18.725979 weasyprint-59.0b1/weasyprint/layout/column.py
+-rw-r--r--   0        0        0    38558 2023-03-06 15:32:25.186425 weasyprint-59.0b1/weasyprint/layout/flex.py
+-rw-r--r--   0        0        0     8756 2023-03-06 15:32:25.186425 weasyprint-59.0b1/weasyprint/layout/float.py
+-rw-r--r--   0        0        0    47911 2023-04-07 06:25:18.902255 weasyprint-59.0b1/weasyprint/layout/inline.py
+-rw-r--r--   0        0        0     2816 2022-11-14 22:25:38.288018 weasyprint-59.0b1/weasyprint/layout/leader.py
+-rw-r--r--   0        0        0     1527 2022-11-14 22:25:38.288018 weasyprint-59.0b1/weasyprint/layout/min_max.py
+-rw-r--r--   0        0        0    35142 2023-04-14 12:31:21.696807 weasyprint-59.0b1/weasyprint/layout/page.py
+-rw-r--r--   0        0        0     5940 2023-03-06 15:32:25.186425 weasyprint-59.0b1/weasyprint/layout/percent.py
+-rw-r--r--   0        0        0    29564 2023-04-12 15:06:54.900471 weasyprint-59.0b1/weasyprint/layout/preferred.py
+-rw-r--r--   0        0        0    11178 2023-03-06 15:32:25.187425 weasyprint-59.0b1/weasyprint/layout/replaced.py
+-rw-r--r--   0        0        0    40754 2023-03-06 15:32:25.187425 weasyprint-59.0b1/weasyprint/layout/table.py
+-rw-r--r--   0        0        0      803 2022-11-14 22:25:38.289018 weasyprint-59.0b1/weasyprint/logger.py
+-rw-r--r--   0        0        0     1909 2022-11-20 12:51:28.692242 weasyprint-59.0b1/weasyprint/matrix.py
+-rw-r--r--   0        0        0    10594 2023-04-14 12:31:21.696807 weasyprint-59.0b1/weasyprint/pdf/__init__.py
+-rw-r--r--   0        0        0    13466 2023-04-12 15:06:57.526514 weasyprint-59.0b1/weasyprint/pdf/anchors.py
+-rw-r--r--   0        0        0    12739 2023-04-14 12:31:21.697807 weasyprint-59.0b1/weasyprint/pdf/fonts.py
+-rw-r--r--   0        0        0     3907 2023-04-12 15:06:57.526514 weasyprint-59.0b1/weasyprint/pdf/metadata.py
+-rw-r--r--   0        0        0     1684 2023-04-12 15:06:57.526514 weasyprint-59.0b1/weasyprint/pdf/pdfa.py
+-rw-r--r--   0        0        0     5456 2023-04-12 15:06:57.526514 weasyprint-59.0b1/weasyprint/pdf/pdfua.py
+-rw-r--r--   0        0        0     3024 2023-03-06 15:20:25.299055 weasyprint-59.0b1/weasyprint/pdf/sRGB2014.icc
+-rw-r--r--   0        0        0    17875 2023-04-12 15:06:57.526514 weasyprint-59.0b1/weasyprint/pdf/stream.py
+-rw-r--r--   0        0        0     5506 2023-03-06 15:32:25.188425 weasyprint-59.0b1/weasyprint/stacking.py
+-rw-r--r--   0        0        0    27607 2023-03-29 18:33:03.523477 weasyprint-59.0b1/weasyprint/svg/__init__.py
+-rw-r--r--   0        0        0    12690 2023-03-06 15:32:25.188425 weasyprint-59.0b1/weasyprint/svg/bounding_box.py
+-rw-r--r--   0        0        0     3833 2023-03-06 15:32:25.188425 weasyprint-59.0b1/weasyprint/svg/css.py
+-rw-r--r--   0        0        0    21140 2023-03-29 18:33:03.524477 weasyprint-59.0b1/weasyprint/svg/defs.py
+-rw-r--r--   0        0        0     2456 2023-03-29 08:57:00.550761 weasyprint-59.0b1/weasyprint/svg/images.py
+-rw-r--r--   0        0        0    10064 2023-03-06 15:20:25.299055 weasyprint-59.0b1/weasyprint/svg/path.py
+-rw-r--r--   0        0        0     3845 2023-03-06 15:32:25.188425 weasyprint-59.0b1/weasyprint/svg/shapes.py
+-rw-r--r--   0        0        0     6095 2023-04-12 15:06:57.526514 weasyprint-59.0b1/weasyprint/svg/text.py
+-rw-r--r--   0        0        0     6644 2023-03-29 18:33:03.524477 weasyprint-59.0b1/weasyprint/svg/utils.py
+-rw-r--r--   0        0        0     7498 2023-03-06 15:20:25.300055 weasyprint-59.0b1/weasyprint/text/constants.py
+-rw-r--r--   0        0        0    15189 2023-03-29 18:33:03.525477 weasyprint-59.0b1/weasyprint/text/ffi.py
+-rw-r--r--   0        0        0    14918 2023-03-29 18:33:03.525477 weasyprint-59.0b1/weasyprint/text/fonts.py
+-rw-r--r--   0        0        0    23959 2023-04-14 12:31:21.697807 weasyprint-59.0b1/weasyprint/text/line_break.py
+-rw-r--r--   0        0        0     9636 2023-04-14 12:31:21.697807 weasyprint-59.0b1/weasyprint/urls.py
+-rw-r--r--   0        0        0     3747 1970-01-01 00:00:00.000000 weasyprint-59.0b1/PKG-INFO
```

### Comparing `weasyprint-59.0/LICENSE` & `weasyprint-59.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/README.rst` & `weasyprint-59.0b1/README.rst`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/docs/api_reference.rst` & `weasyprint-59.0b1/docs/api_reference.rst`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/docs/changelog.rst` & `weasyprint-59.0b1/docs/changelog.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,60 +1,11 @@
 Changelog
 =========
 
 
-Version 59.0
-------------
-
-Released on 2023-05-11.
-
-This version also includes the changes from unstable b1 version listed
-below.
-
-Bug fixes:
-
-* `#1864 <https://github.com/Kozea/WeasyPrint/issues/1864>`_:
-  Handle overflow for svg and symbol tags in SVG images
-* `#1867 <https://github.com/Kozea/WeasyPrint/pull/1867>`_:
-  Remove duplicate compression of attachments
-* `d0ad5c1 <https://github.com/Kozea/WeasyPrint/commit/d0ad5c1>`_:
-  Override use tag children instead of drawing their references
-* `93df1a5 <https://github.com/Kozea/WeasyPrint/commit/93df1a5>`_:
-  Don’t resize the same image twice when the --dpi option is set
-* `#1874 <https://github.com/Kozea/WeasyPrint/pull/1874>`_:
-  Drawn underline and overline behind text
-
-Contributors:
-
-* Guillaume Ayoub
-* Timo Ramsauer
-* Alexander Mankuta
-
-Backers and sponsors:
-
-* Castedo Ellerman
-* Kobalt
-* Spacinov
-* Grip Angebotssoftware
-* Crisp BV
-* Manuel Barkhau
-* SimonSoft
-* Menutech
-* KontextWork
-* NCC Group
-* René Fritz
-* Moritz Mahringer
-* Yanal-Yvez Fargialla
-* Piotr Horzycki
-* Healthchecks.io
-* TrainingSparkle
-* Hammerbacher
-* Synapsium
-
-
 Version 59.0b1
 --------------
 
 Released on 2023-04-14.
 
 **This version is experimental, don't use it in production. If you find bugs,
 please report them!**
@@ -85,15 +36,15 @@
   1. Use named parameters for these functions, not positioned parameters.
   2. Rename some the parameters:
 
      * ``image_cache`` becomes ``cache`` (see below),
      * ``identifier`` becomes ``pdf_identifier``,
      * ``variant`` becomes ``pdf_variant``,
      * ``version`` becomes ``pdf_version``,
-     * ``forms`` becomes ``pdf_forms``.
+     * ``forms`` becomes ``pdf_forms``,
 
 * The ``optimize_size`` parameter of ``HTML.render()``, ``HTML.write_pdf()``
   and ``Document()`` has been removed and will be ignored. You can now use the
   ``uncompressed_pdf``, ``full_fonts``, ``hinting``, ``dpi`` and
   ``jpeg_quality`` parameters that are included in ``**options``.
 
 * The ``cache`` parameter can be included in ``**options`` to replace
```

### Comparing `weasyprint-59.0/docs/common_use_cases.rst` & `weasyprint-59.0b1/docs/common_use_cases.rst`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/docs/conf.py` & `weasyprint-59.0b1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/docs/contribute.rst` & `weasyprint-59.0b1/docs/contribute.rst`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/docs/first_steps.rst` & `weasyprint-59.0b1/docs/first_steps.rst`

 * *Files 3% similar despite different names*

```diff
@@ -504,51 +504,44 @@
 .. _Flask: https://flask.pocoo.org/
 .. _Django-WeasyPrint: https://github.com/fdemmer/django-weasyprint
 .. _Django: https://www.djangoproject.com/
 
 Image Cache and Optimization
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-WeasyPrint provides many options to deal with images: ``optimize_images``,
-``jpeg_quality``, ``dpi`` and ``image_cache``.
+WeasyPrint provides two options to deal with images: ``optimize_size`` and
+``image_cache``.
 
-``optimize_images`` can enable size optimization for images. When enabled, the
-generated PDF will include smaller images with no quality penalty, but the
-rendering time may be slightly increased.
-
-The ``jpeg_quality`` option can be set to decrease the quality of JPEG images
-included in the PDF. You can set a value between 95 (best quality) to 0
-(smaller image size), depending on your needs.
-
-The ``dpi`` option offers the possibility to reduce the size (in pixels, and
-thus in bytes) of all included raster images. The resolution, set in dots per
-inch, indicates the maximum number of pixels included in one inch on the
-generated PDF.
+``optimize_size`` can enable size optimization for images, but also for fonts.
+When enabled, the generated PDF will include smaller images and fonts, but the
+rendering time may be slightly increased. The whole structure of the PDF can be
+compressed too.
 
 .. code-block:: python
 
-    # Original high-quality images, faster, but generated PDF is larger
-    HTML('https://weasyprint.org/').write_pdf('weasyprint.pdf')
-
-    # Optimized lower-quality images, a bit slower, but generated PDF is smaller
-    HTML('https://weasyprint.org/').write_pdf(
-        'weasyprint.pdf', optimize_images=True, jpeg_quality=60, dpi=150)
+    # No size optimization, faster, but generated PDF is larger
+    HTML('https://example.org/').write_pdf(
+        'example.pdf', optimize_size=())
+
+    # Full size optimization, slower, but generated PDF is smaller
+    HTML('https://example.org/').write_pdf(
+        'example.pdf', optimize_size=('fonts', 'images', 'hinting', 'pdf'))
 
 ``image_cache`` gives the possibility to use a cache for images, avoiding to
 download, parse and optimize them each time they are used.
 
 By default, the cache is used document by document, but you can share it
 between documents if needed. This feature can save a lot of network and CPU
 time when you render a lot of documents that use the same images.
 
 .. code-block:: python
 
     cache = {}
     for i in range(10):
-        HTML(f'https://weasyprint.org/').write_pdf(
+        HTML(f'https://example.org/?id={i}').write_pdf(
             f'example-{i}.pdf', image_cache=cache)
 
 It’s also possible to cache images on disk instead of keeping them in memory.
 The ``--cache-folder`` CLI option can be used to define the folder used to
 store temporary images. You can also provide this folder path as a string for
 ``image_cache``.
```

### Comparing `weasyprint-59.0/docs/going_further.rst` & `weasyprint-59.0b1/docs/going_further.rst`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/docs/support.rst` & `weasyprint-59.0b1/docs/support.rst`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/pyproject.toml` & `weasyprint-59.0b1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/conftest.py` & `weasyprint-59.0b1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/draw/__init__.py` & `weasyprint-59.0b1/tests/draw/__init__.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/draw/svg/test_bounding_box.py` & `weasyprint-59.0b1/tests/draw/svg/test_bounding_box.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/draw/svg/test_clip.py` & `weasyprint-59.0b1/tests/draw/svg/test_clip.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/draw/svg/test_defs.py` & `weasyprint-59.0b1/tests/draw/svg/test_defs.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/draw/svg/test_gradients.py` & `weasyprint-59.0b1/tests/draw/svg/test_gradients.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/draw/svg/test_images.py` & `weasyprint-59.0b1/tests/draw/svg/test_images.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/draw/svg/test_opacity.py` & `weasyprint-59.0b1/tests/draw/svg/test_opacity.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/draw/svg/test_paths.py` & `weasyprint-59.0b1/tests/draw/svg/test_paths.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/draw/svg/test_patterns.py` & `weasyprint-59.0b1/tests/draw/svg/test_patterns.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/draw/svg/test_shapes.py` & `weasyprint-59.0b1/tests/draw/svg/test_shapes.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/draw/svg/test_text.py` & `weasyprint-59.0b1/tests/draw/svg/test_text.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/draw/svg/test_transform.py` & `weasyprint-59.0b1/tests/draw/svg/test_transform.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/draw/svg/test_units.py` & `weasyprint-59.0b1/tests/draw/svg/test_units.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/draw/svg/test_visibility.py` & `weasyprint-59.0b1/tests/draw/svg/test_visibility.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/draw/test_absolute.py` & `weasyprint-59.0b1/tests/draw/test_absolute.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/draw/test_background.py` & `weasyprint-59.0b1/tests/draw/test_background.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/draw/test_before_after.py` & `weasyprint-59.0b1/tests/draw/test_before_after.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/draw/test_box.py` & `weasyprint-59.0b1/tests/draw/test_box.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/draw/test_column.py` & `weasyprint-59.0b1/tests/draw/test_column.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/draw/test_current_color.py` & `weasyprint-59.0b1/tests/draw/test_current_color.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/draw/test_float.py` & `weasyprint-59.0b1/tests/draw/test_float.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/draw/test_footnote.py` & `weasyprint-59.0b1/tests/draw/test_footnote.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/draw/test_footnote_column.py` & `weasyprint-59.0b1/tests/draw/test_footnote_column.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/draw/test_gradient.py` & `weasyprint-59.0b1/tests/draw/test_gradient.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/draw/test_image.py` & `weasyprint-59.0b1/tests/draw/test_image.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/draw/test_leader.py` & `weasyprint-59.0b1/tests/draw/test_leader.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/draw/test_list.py` & `weasyprint-59.0b1/tests/draw/test_list.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/draw/test_opacity.py` & `weasyprint-59.0b1/tests/draw/test_opacity.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/draw/test_overflow.py` & `weasyprint-59.0b1/tests/draw/test_overflow.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/draw/test_page.py` & `weasyprint-59.0b1/tests/draw/test_page.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/draw/test_table.py` & `weasyprint-59.0b1/tests/draw/test_table.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/draw/test_text.py` & `weasyprint-59.0b1/tests/draw/test_text.py`

 * *Files 11% similar despite different names*

```diff
@@ -516,28 +516,28 @@
       <div>ace</div>''')
 
 
 def test_text_underline(assert_pixels):
     assert_pixels('''
         _____________
         _zzzzzzzzzzz_
-        _zsssssssssz_
-        _zsssssssssz_
-        _zuuuuuuuuuz_
+        _zRRRRRRRRRz_
+        _zRRRRRRRRRz_
+        _zBBBBBBBBBz_
         _zzzzzzzzzzz_
         _____________
     ''', '''
       <style>
         @font-face {src: url(weasyprint.otf); font-family: weasyprint}
         @page {
           size: 13px 7px;
           margin: 2px;
         }
         body {
-          color: rgba(255, 0, 0, 0.5);
+          color: red;
           font-family: weasyprint;
           font-size: 3px;
           text-decoration: underline blue;
         }
       </style>
       <div>abc</div>''')
 
@@ -545,107 +545,107 @@
 def test_text_overline(assert_pixels):
     # Ascent value seems to be a bit random, don’t try to get the exact
     # position of the line
     assert_pixels('''
         _____________
         _zzzzzzzzzzz_
         _zzzzzzzzzzz_
-        _zsssssssssz_
-        _zsssssssssz_
+        _zRRRRRRRRRz_
+        _zRRRRRRRRRz_
         _zzzzzzzzzzz_
         _____________
     ''', '''
       <style>
         @font-face {src: url(weasyprint.otf); font-family: weasyprint}
         @page {
           size: 13px 7px;
           margin: 2px;
         }
         body {
-          color: rgba(255, 0, 0, 0.5);
+          color: red;
           font-family: weasyprint;
           font-size: 3px;
           text-decoration: overline blue;
         }
       </style>
       <div>abc</div>''')
 
 
 def test_text_line_through(assert_pixels):
     assert_pixels('''
         _____________
         _zzzzzzzzzzz_
+        _zRRRRRRRRRz_
         _zBBBBBBBBBz_
-        _zuuuuuuuuuz_
-        _zBBBBBBBBBz_
+        _zRRRRRRRRRz_
         _zzzzzzzzzzz_
         _____________
     ''', '''
       <style>
         @font-face {src: url(weasyprint.otf); font-family: weasyprint}
         @page {
           size: 13px 7px;
           margin: 2px;
         }
         body {
-          color: blue;
+          color: red;
           font-family: weasyprint;
           font-size: 3px;
-          text-decoration: line-through rgba(255, 0, 0, 0.5);
+          text-decoration: line-through blue;
         }
       </style>
       <div>abc</div>''')
 
 
 def test_text_multiple_text_decoration(assert_pixels):
     # Test regression: https://github.com/Kozea/WeasyPrint/issues/1621
     assert_pixels('''
         _____________
         _zzzzzzzzzzz_
-        _zsssssssssz_
+        _zRRRRRRRRRz_
+        _zBBBBBBBBBz_
         _zBBBBBBBBBz_
-        _zuuuuuuuuuz_
         _zzzzzzzzzzz_
         _____________
     ''', '''
       <style>
         @font-face {src: url(weasyprint.otf); font-family: weasyprint}
         @page {
           size: 13px 7px;
           margin: 2px;
         }
         body {
-          color: rgba(255, 0, 0, 0.5);
+          color: red;
           font-family: weasyprint;
           font-size: 3px;
           text-decoration: underline line-through blue;
         }
       </style>
       <div>abc</div>''')
 
 
 def test_text_nested_text_decoration(assert_pixels):
     # Test regression: https://github.com/Kozea/WeasyPrint/issues/1621
     assert_pixels('''
         _____________
         _zzzzzzzzzzz_
-        _zsssssssssz_
-        _zsssBBBsssz_
-        _zuuuuuuuuuz_
+        _zRRRRRRRRRz_
+        _zRRRBBBRRRz_
+        _zBBBBBBBBBz_
         _zzzzzzzzzzz_
         _____________
     ''', '''
       <style>
         @font-face {src: url(weasyprint.otf); font-family: weasyprint}
         @page {
           size: 13px 7px;
           margin: 2px;
         }
         body {
-          color: rgba(255, 0, 0, 0.5);
+          color: red;
           font-family: weasyprint;
           font-size: 3px;
           text-decoration: underline blue;
         }
         span {
           text-decoration: line-through blue;
         }
```

### Comparing `weasyprint-59.0/tests/draw/test_transform.py` & `weasyprint-59.0b1/tests/draw/test_transform.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/draw/test_visibility.py` & `weasyprint-59.0b1/tests/draw/test_visibility.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/draw/test_whitespace.py` & `weasyprint-59.0b1/tests/draw/test_whitespace.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/layout/test_block.py` & `weasyprint-59.0b1/tests/layout/test_block.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/layout/test_column.py` & `weasyprint-59.0b1/tests/layout/test_column.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/layout/test_flex.py` & `weasyprint-59.0b1/tests/layout/test_flex.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/layout/test_footnotes.py` & `weasyprint-59.0b1/tests/layout/test_footnotes.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/layout/test_image.py` & `weasyprint-59.0b1/tests/layout/test_image.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/layout/test_inline.py` & `weasyprint-59.0b1/tests/layout/test_inline.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/layout/test_inline_block.py` & `weasyprint-59.0b1/tests/layout/test_inline_block.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/layout/test_list.py` & `weasyprint-59.0b1/tests/layout/test_list.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/layout/test_page.py` & `weasyprint-59.0b1/tests/layout/test_page.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/layout/test_position.py` & `weasyprint-59.0b1/tests/layout/test_position.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/layout/test_shrink_to_fit.py` & `weasyprint-59.0b1/tests/layout/test_shrink_to_fit.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/layout/test_table.py` & `weasyprint-59.0b1/tests/layout/test_table.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/resources/acid2-reference.html` & `weasyprint-59.0b1/tests/resources/acid2-reference.html`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/resources/acid2-test.html` & `weasyprint-59.0b1/tests/resources/acid2-test.html`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/resources/doc1.html` & `weasyprint-59.0b1/tests/resources/doc1.html`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/resources/doc1_UTF-16BE.html` & `weasyprint-59.0b1/tests/resources/doc1_UTF-16BE.html`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/resources/icon.png` & `weasyprint-59.0b1/tests/resources/icon.png`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/resources/logo_small.png` & `weasyprint-59.0b1/tests/resources/logo_small.png`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/resources/not-optimized-exif.jpg` & `weasyprint-59.0b1/tests/resources/not-optimized-exif.jpg`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/resources/not-optimized.jpg` & `weasyprint-59.0b1/tests/resources/not-optimized.jpg`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/resources/weasyprint.otb` & `weasyprint-59.0b1/tests/resources/weasyprint.otb`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/resources/weasyprint.otf` & `weasyprint-59.0b1/tests/resources/weasyprint.otf`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/resources/weasyprint.woff` & `weasyprint-59.0b1/tests/resources/weasyprint.woff`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/test_acid2.py` & `weasyprint-59.0b1/tests/test_acid2.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/test_api.py` & `weasyprint-59.0b1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/test_boxes.py` & `weasyprint-59.0b1/tests/test_boxes.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/test_counters.py` & `weasyprint-59.0b1/tests/test_counters.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/test_css.py` & `weasyprint-59.0b1/tests/test_css.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/test_css_descriptors.py` & `weasyprint-59.0b1/tests/test_css_descriptors.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/test_css_validation.py` & `weasyprint-59.0b1/tests/test_css_validation.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/test_float.py` & `weasyprint-59.0b1/tests/test_float.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/test_fonts.py` & `weasyprint-59.0b1/tests/test_fonts.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/test_pdf.py` & `weasyprint-59.0b1/tests/test_pdf.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/test_presentational_hints.py` & `weasyprint-59.0b1/tests/test_presentational_hints.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/test_stacking.py` & `weasyprint-59.0b1/tests/test_stacking.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/test_target.py` & `weasyprint-59.0b1/tests/test_target.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/test_text.py` & `weasyprint-59.0b1/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/test_unicode.py` & `weasyprint-59.0b1/tests/test_unicode.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/test_variables.py` & `weasyprint-59.0b1/tests/test_variables.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/tests/testing_utils.py` & `weasyprint-59.0b1/tests/testing_utils.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/__init__.py` & `weasyprint-59.0b1/weasyprint/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from pathlib import Path
 from urllib.parse import urljoin
 
 import cssselect2
 import html5lib
 import tinycss2
 
-VERSION = __version__ = '59.0'
+VERSION = __version__ = '59.0b1'
 
 #: Default values for command-line and Python API options. See
 #: :func:`__main__.main` to learn more about specific options for
 #: command-line.
 #:
 #: :param list stylesheets:
 #:     An optional list of user stylesheets. The list can include
```

### Comparing `weasyprint-59.0/weasyprint/__main__.py` & `weasyprint-59.0b1/weasyprint/__main__.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/anchors.py` & `weasyprint-59.0b1/weasyprint/anchors.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/css/__init__.py` & `weasyprint-59.0b1/weasyprint/css/__init__.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/css/computed_values.py` & `weasyprint-59.0b1/weasyprint/css/computed_values.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/css/counters.py` & `weasyprint-59.0b1/weasyprint/css/counters.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/css/html5_ph.css` & `weasyprint-59.0b1/weasyprint/css/html5_ph.css`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/css/html5_ua.css` & `weasyprint-59.0b1/weasyprint/css/html5_ua.css`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/css/media_queries.py` & `weasyprint-59.0b1/weasyprint/css/media_queries.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/css/properties.py` & `weasyprint-59.0b1/weasyprint/css/properties.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/css/targets.py` & `weasyprint-59.0b1/weasyprint/css/targets.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/css/tests_ua.css` & `weasyprint-59.0b1/weasyprint/css/tests_ua.css`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/css/utils.py` & `weasyprint-59.0b1/weasyprint/css/utils.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/css/validation/__init__.py` & `weasyprint-59.0b1/weasyprint/css/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/css/validation/descriptors.py` & `weasyprint-59.0b1/weasyprint/css/validation/descriptors.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/css/validation/expanders.py` & `weasyprint-59.0b1/weasyprint/css/validation/expanders.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/css/validation/properties.py` & `weasyprint-59.0b1/weasyprint/css/validation/properties.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/document.py` & `weasyprint-59.0b1/weasyprint/document.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/draw.py` & `weasyprint-59.0b1/weasyprint/draw.py`

 * *Files 2% similar despite different names*

```diff
@@ -997,53 +997,50 @@
     """Draw a textbox to a pydyf stream."""
     # Pango crashes with font-size: 0
     assert textbox.style['font_size']
 
     if textbox.style['visibility'] != 'visible':
         return
 
-    text_decoration_values = textbox.style['text_decoration_line']
-    text_decoration_color = textbox.style['text_decoration_color']
-    if text_decoration_color == 'currentColor':
-        text_decoration_color = textbox.style['color']
-    if 'overline' in text_decoration_values:
-        thickness = textbox.pango_layout.underline_thickness
-        offset_y = (
-            textbox.baseline - textbox.pango_layout.ascent + thickness / 2)
-        draw_text_decoration(
-            stream, textbox, offset_x, offset_y, thickness,
-            text_decoration_color)
-    if 'underline' in text_decoration_values:
-        thickness = textbox.pango_layout.underline_thickness
-        offset_y = (
-            textbox.baseline - textbox.pango_layout.underline_position +
-            thickness / 2)
-        draw_text_decoration(
-            stream, textbox, offset_x, offset_y, thickness,
-            text_decoration_color)
-
     x, y = textbox.position_x, textbox.position_y + textbox.baseline
     stream.set_color_rgb(*textbox.style['color'][:3])
     stream.set_alpha(textbox.style['color'][3])
 
     textbox.pango_layout.reactivate(textbox.style)
     stream.begin_text()
     emojis = draw_first_line(
         stream, textbox, text_overflow, block_ellipsis, x, y)
     stream.end_text()
 
     draw_emojis(stream, textbox.style['font_size'], x, y, emojis)
 
-    if 'line-through' in text_decoration_values:
+    # Draw text decoration
+    values = textbox.style['text_decoration_line']
+    color = textbox.style['text_decoration_color']
+    if color == 'currentColor':
+        color = textbox.style['color']
+    if 'overline' in values:
+        thickness = textbox.pango_layout.underline_thickness
+        offset_y = (
+            textbox.baseline - textbox.pango_layout.ascent + thickness / 2)
+        draw_text_decoration(
+            stream, textbox, offset_x, offset_y, thickness, color)
+    if 'underline' in values:
+        thickness = textbox.pango_layout.underline_thickness
+        offset_y = (
+            textbox.baseline - textbox.pango_layout.underline_position +
+            thickness / 2)
+        draw_text_decoration(
+            stream, textbox, offset_x, offset_y, thickness, color)
+    if 'line-through' in values:
         thickness = textbox.pango_layout.strikethrough_thickness
         offset_y = (
             textbox.baseline - textbox.pango_layout.strikethrough_position)
         draw_text_decoration(
-            stream, textbox, offset_x, offset_y, thickness,
-            text_decoration_color)
+            stream, textbox, offset_x, offset_y, thickness, color)
 
     textbox.pango_layout.deactivate()
 
 
 def draw_emojis(stream, font_size, x, y, emojis):
     for image, font, a, d, e, f in emojis:
         stream.push_state()
```

### Comparing `weasyprint-59.0/weasyprint/formatting_structure/boxes.py` & `weasyprint-59.0b1/weasyprint/formatting_structure/boxes.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/formatting_structure/build.py` & `weasyprint-59.0b1/weasyprint/formatting_structure/build.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/html.py` & `weasyprint-59.0b1/weasyprint/html.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/images.py` & `weasyprint-59.0b1/weasyprint/images.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,25 +90,36 @@
         return self.width / resolution, self.height / resolution, self.ratio
 
     def draw(self, stream, concrete_width, concrete_height, image_rendering):
         if self.width <= 0 or self.height <= 0:
             return
 
         width, height = self.width, self.height
-        interpolate = 'true' if image_rendering == 'auto' else 'false'
-        ratio = 1
         if self._dpi:
             pt_to_in = 4 / 3 / 96
             width_inches = abs(concrete_width * stream.ctm[0][0] * pt_to_in)
             height_inches = abs(concrete_height * stream.ctm[1][1] * pt_to_in)
             dpi = max(self.width / width_inches, self.height / height_inches)
             if dpi > self._dpi:
                 ratio = self._dpi / dpi
-        image_name = stream.add_image(self, width, height, interpolate, ratio)
+                image = Image.open(io.BytesIO(self.image_data.data))
+                width = int(round(self.width * ratio))
+                height = int(round(self.height * ratio))
+                image.thumbnail((max(1, width), max(1, height)))
+                image_file = io.BytesIO()
+                image.save(
+                    image_file, format=image.format, optimize=self.optimize)
+                width, height = image.width, image.height
+                self.image_data = self.cache_image_data(image_file.getvalue())
+        else:
+            dpi = None
+
+        interpolate = 'true' if image_rendering == 'auto' else 'false'
 
+        image_name = stream.add_image(self, width, height, interpolate)
         stream.transform(
             concrete_width, 0, 0, -concrete_height, 0, concrete_height)
         stream.draw_x_object(image_name)
 
     def cache_image_data(self, data, filename=None, alpha=False):
         if filename:
             return LazyLocalImage(filename)
```

### Comparing `weasyprint-59.0/weasyprint/layout/__init__.py` & `weasyprint-59.0b1/weasyprint/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/layout/absolute.py` & `weasyprint-59.0b1/weasyprint/layout/absolute.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/layout/background.py` & `weasyprint-59.0b1/weasyprint/layout/background.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/layout/block.py` & `weasyprint-59.0b1/weasyprint/layout/block.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/layout/column.py` & `weasyprint-59.0b1/weasyprint/layout/column.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/layout/flex.py` & `weasyprint-59.0b1/weasyprint/layout/flex.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/layout/float.py` & `weasyprint-59.0b1/weasyprint/layout/float.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/layout/inline.py` & `weasyprint-59.0b1/weasyprint/layout/inline.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/layout/leader.py` & `weasyprint-59.0b1/weasyprint/layout/leader.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/layout/min_max.py` & `weasyprint-59.0b1/weasyprint/layout/min_max.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/layout/page.py` & `weasyprint-59.0b1/weasyprint/layout/page.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/layout/percent.py` & `weasyprint-59.0b1/weasyprint/layout/percent.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/layout/preferred.py` & `weasyprint-59.0b1/weasyprint/layout/preferred.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/layout/replaced.py` & `weasyprint-59.0b1/weasyprint/layout/replaced.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/layout/table.py` & `weasyprint-59.0b1/weasyprint/layout/table.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/logger.py` & `weasyprint-59.0b1/weasyprint/logger.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/matrix.py` & `weasyprint-59.0b1/weasyprint/matrix.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/pdf/__init__.py` & `weasyprint-59.0b1/weasyprint/pdf/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -238,15 +238,15 @@
                 pdf.info[key] = pydyf.String(value)
 
     # Embedded files
     attachments = metadata.attachments + (options['attachments'] or [])
     pdf_attachments = []
     for attachment in attachments:
         pdf_attachment = write_pdf_attachment(
-            pdf, attachment, document.url_fetcher, compress)
+            pdf, attachment, document.url_fetcher)
         if pdf_attachment is not None:
             pdf_attachments.append(pdf_attachment)
     if pdf_attachments:
         content = pydyf.Dictionary({'Names': pydyf.Array()})
         for i, pdf_attachment in enumerate(pdf_attachments):
             content['Names'].append(pydyf.String(f'attachment{i}'))
             content['Names'].append(pdf_attachment.reference)
```

### Comparing `weasyprint-59.0/weasyprint/pdf/anchors.py` & `weasyprint-59.0b1/weasyprint/pdf/anchors.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Insert anchors, links, bookmarks and inputs in PDFs."""
 
 import hashlib
 import io
+import zlib
 from os.path import basename
 from urllib.parse import unquote, urlsplit
 
 import pydyf
 
 from .. import Attachment
 from ..logger import LOGGER
@@ -209,15 +210,15 @@
             # A single link can be split in multiple regions. We don't want
             # to embed a file multiple times of course, so keep a reference
             # to every embedded URL and reuse the object number.
             # TODO: Use the title attribute as description. The comment
             # above about multiple regions won't always be correct, because
             # two links might have the same href, but different titles.
             annot_files[annot_target] = write_pdf_attachment(
-                pdf, (annot_target, None), document.url_fetcher, compress)
+                pdf, (annot_target, None), document.url_fetcher)
         annot_file = annot_files[annot_target]
         if annot_file is None:
             continue
         rectangle = (
             *matrix.transform_point(*rectangle[:2]),
             *matrix.transform_point(*rectangle[2:]))
         stream = pydyf.Stream([], {
@@ -237,15 +238,15 @@
         })
         pdf.add_object(annot)
         if 'Annots' not in page:
             page['Annots'] = pydyf.Array()
         page['Annots'].append(annot.reference)
 
 
-def write_pdf_attachment(pdf, attachment, url_fetcher, compress):
+def write_pdf_attachment(pdf, attachment, url_fetcher):
     """Write an attachment to the PDF stream."""
     # Attachments from document links like <link> or <a> can only be URLs.
     # They're passed in as tuples
     url = ''
     if isinstance(attachment, tuple):
         url, description = attachment
         attachment = Attachment(
@@ -256,26 +257,31 @@
     try:
         with attachment.source as (source_type, source, url, _):
             if isinstance(source, bytes):
                 source = io.BytesIO(source)
             uncompressed_length = 0
             stream = b''
             md5 = hashlib.md5()
+            compress = zlib.compressobj()
             for data in iter(lambda: source.read(4096), b''):
                 uncompressed_length += len(data)
                 md5.update(data)
-                stream += data
+                compressed = compress.compress(data)
+                stream += compressed
+            compressed = compress.flush(zlib.Z_FINISH)
+            stream += compressed
             file_extra = pydyf.Dictionary({
                 'Type': '/EmbeddedFile',
+                'Filter': '/FlateDecode',
                 'Params': pydyf.Dictionary({
                     'CheckSum': f'<{md5.hexdigest()}>',
                     'Size': uncompressed_length,
                 })
             })
-            file_stream = pydyf.Stream([stream], file_extra, compress=compress)
+            file_stream = pydyf.Stream([stream], file_extra, compress)
             pdf.add_object(file_stream)
 
     except URLFetchingError as exception:
         LOGGER.error('Failed to load attachment: %s', exception)
         return
 
     # TODO: Use the result object from a URL fetch operation to provide more
```

### Comparing `weasyprint-59.0/weasyprint/pdf/fonts.py` & `weasyprint-59.0b1/weasyprint/pdf/fonts.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/pdf/metadata.py` & `weasyprint-59.0b1/weasyprint/pdf/metadata.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/pdf/pdfa.py` & `weasyprint-59.0b1/weasyprint/pdf/pdfa.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/pdf/pdfua.py` & `weasyprint-59.0b1/weasyprint/pdf/pdfua.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/pdf/sRGB2014.icc` & `weasyprint-59.0b1/weasyprint/pdf/sRGB2014.icc`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/pdf/stream.py` & `weasyprint-59.0b1/weasyprint/pdf/stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from functools import lru_cache
 from hashlib import md5
 
 import pydyf
 from fontTools import subset
 from fontTools.ttLib import TTFont, TTLibError, ttFont
 from fontTools.varLib.mutator import instantiateVariableFont
-from PIL import Image
 
 from ..logger import LOGGER
 from ..matrix import Matrix
 from ..text.ffi import ffi, harfbuzz, pango, units_to_double
 
 
 class Font:
@@ -358,32 +357,21 @@
             self._fonts, self.page_rectangle, states, x_objects, patterns,
             shadings, self._images, self._mark, extra=extra,
             compress=self.compress)
         group.id = f'x{len(self._x_objects)}'
         self._x_objects[group.id] = group
         return group
 
-    def add_image(self, image, width, height, interpolate, ratio):
-        image_name = f'i{image.id}{width}{height}{interpolate}{ratio}'
+    def add_image(self, image, width, height, interpolate):
+        image_name = f'i{image.id}{width}{height}{interpolate}'
         self._x_objects[image_name] = None  # Set by write_pdf
         if image_name in self._images:
             # Reuse image already stored in document
             return image_name
 
-        if ratio != 1:
-            thumbnail = Image.open(io.BytesIO(image.image_data.data))
-            width = int(round(image.width * ratio))
-            height = int(round(image.height * ratio))
-            thumbnail.thumbnail((max(1, width), max(1, height)))
-            image_file = io.BytesIO()
-            thumbnail.save(
-                image_file, format=thumbnail.format, optimize=image.optimize)
-            width, height = thumbnail.width, thumbnail.height
-            image.image_data = image.cache_image_data(image_file.getvalue())
-
         xobject = image.get_xobject(width, height, interpolate)
         self._images[image_name] = xobject
         return image_name
 
     def add_pattern(self, x, y, width, height, repeat_width, repeat_height,
                     matrix):
         states = pydyf.Dictionary()
@@ -480,15 +468,19 @@
             return 'BlockQuote'
         elif element_tag == 'p':
             return 'P'
         elif element_tag in ('h1', 'h2', 'h3', 'h4', 'h5', 'h6'):
             return element_tag.upper()
         elif element_tag in ('dl', 'ul', 'ol'):
             return 'L'
-        elif element_tag in ('li', 'dt', 'dd'):
+        elif element_tag == 'li':
+            return 'LI'
+        elif element_tag == 'dt':
+            return 'LI'
+        elif element_tag == 'dd':
             return 'LI'
         elif element_tag == 'table':
             return 'Table'
         elif element_tag in ('tr', 'th', 'td'):
             return element_tag.upper()
         elif element_tag in ('thead', 'tbody', 'tfoot'):
             return element_tag[:2].upper() + element_tag[2:]
```

### Comparing `weasyprint-59.0/weasyprint/stacking.py` & `weasyprint-59.0b1/weasyprint/stacking.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/svg/__init__.py` & `weasyprint-59.0b1/weasyprint/svg/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -280,21 +280,14 @@
 
     def pop_rotation(self, original_rotate, rotate):
         """Merge nested letter rotations."""
         self.attrib['rotate'] = ' '.join(
             str(rotate.pop(0) if rotate else original_rotate[-1])
             for i in range(len(self.text)))
 
-    def override_iter(self, iterator):
-        """Override node’s children iterator."""
-        # As special methods are bound to classes and not instances, we have to
-        # create and assign a new type.
-        self.__class__ = type(
-            'Node', (Node,), {'__iter__': lambda _: iterator})
-
 
 class SVG:
     """An SVG document."""
 
     def __init__(self, tree, url):
         wrapper = ElementWrapper.from_xml_root(tree)
         style = parse_stylesheets(wrapper, url)
@@ -740,15 +733,19 @@
         if not parent:
             return
         self.inherit_element(parent, defs)
         for key, value in parent.attrib.items():
             if key not in element.attrib:
                 element.attrib[key] = value
         if next(iter(element), None) is None:
-            element.override_iter(parent.__iter__())
+            # Override element’s __iter__ with parent’s __iter__. As special
+            # methods are bound to classes and not instances, we have to create
+            # and assign a new type.
+            element.__class__ = type(
+                'Node', (Node,), {'__iter__': lambda self: parent.__iter__()})
 
     def calculate_bounding_box(self, node, font_size, stroke=True):
         """Calculate the bounding box of a node."""
         if stroke or node.bounding_box is None:
             box = bounding_box(self, node, font_size, stroke)
             if is_valid_bounding_box(box) and 0 not in box[2:]:
                 if stroke:
```

### Comparing `weasyprint-59.0/weasyprint/svg/bounding_box.py` & `weasyprint-59.0b1/weasyprint/svg/bounding_box.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/svg/css.py` & `weasyprint-59.0b1/weasyprint/svg/css.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/svg/defs.py` & `weasyprint-59.0b1/weasyprint/svg/defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,16 +56,18 @@
 
     # Cascade
     for key, value in node.attrib.items():
         if key not in NOT_INHERITED_ATTRIBUTES:
             if key not in tree.attrib:
                 tree.attrib[key] = value
 
-    node.override_iter(iter((tree,)))
+    svg.stream.push_state()
     svg.stream.transform(e=x, f=y)
+    svg.draw_node(tree, font_size)
+    svg.stream.pop_state()
 
 
 def draw_gradient_or_pattern(svg, node, name, font_size, opacity, stroke):
     """Draw given gradient or pattern."""
     if name in svg.gradients:
         return draw_gradient(
             svg, node, svg.gradients[name], font_size, opacity, stroke)
```

### Comparing `weasyprint-59.0/weasyprint/svg/images.py` & `weasyprint-59.0b1/weasyprint/svg/images.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     if svg.tree == node:
         width, height = svg.concrete_width, svg.concrete_height
     else:
         width, height = svg.point(
             node.get('width'), node.get('height'), font_size)
     scale_x, scale_y, translate_x, translate_y = preserve_ratio(
         svg, node, font_size, width, height)
-    if svg.tree != node and node.get('overflow', 'hidden') == 'hidden':
+    if svg.tree != node:
         svg.stream.rectangle(0, 0, width, height)
         svg.stream.clip()
         svg.stream.end()
     svg.stream.transform(a=scale_x, d=scale_y, e=translate_x, f=translate_y)
 
 
 def image(svg, node, font_size):
```

### Comparing `weasyprint-59.0/weasyprint/svg/path.py` & `weasyprint-59.0b1/weasyprint/svg/path.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/svg/shapes.py` & `weasyprint-59.0b1/weasyprint/svg/shapes.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/svg/text.py` & `weasyprint-59.0b1/weasyprint/svg/text.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/svg/utils.py` & `weasyprint-59.0b1/weasyprint/svg/utils.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/text/constants.py` & `weasyprint-59.0b1/weasyprint/text/constants.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/text/ffi.py` & `weasyprint-59.0b1/weasyprint/text/ffi.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/text/fonts.py` & `weasyprint-59.0b1/weasyprint/text/fonts.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/text/line_break.py` & `weasyprint-59.0b1/weasyprint/text/line_break.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/weasyprint/urls.py` & `weasyprint-59.0b1/weasyprint/urls.py`

 * *Files identical despite different names*

### Comparing `weasyprint-59.0/PKG-INFO` & `weasyprint-59.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weasyprint
-Version: 59.0
+Version: 59.0b1
 Summary: The Awesome Document Factory
 Keywords: html,css,pdf,converter
 Author-email: Simon Sapin <simon.sapin@exyr.org>
 Maintainer-email: CourtBouillon <contact@courtbouillon.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
```

