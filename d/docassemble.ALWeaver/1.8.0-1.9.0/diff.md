# Comparing `tmp/docassemble.ALWeaver-1.8.0.tar.gz` & `tmp/docassemble.ALWeaver-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docassemble.ALWeaver-1.8.0.tar", last modified: Thu Dec  1 21:13:42 2022, max compression
+gzip compressed data, was "docassemble.ALWeaver-1.9.0.tar", last modified: Wed Mar 15 15:33:26 2023, max compression
```

## Comparing `docassemble.ALWeaver-1.8.0.tar` & `docassemble.ALWeaver-1.9.0.tar`

### file list

```diff
@@ -1,89 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 21:13:42.766493 docassemble.ALWeaver-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1092 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (122)       18 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     3449 2022-12-01 21:13:42.766493 docassemble.ALWeaver-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3286 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 21:13:42.750493 docassemble.ALWeaver-1.8.0/docassemble/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 21:13:42.754493 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/
--rw-r--r--   0 runner    (1001) docker     (122)       22 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      303 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/advertise_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (122)    11811 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/custom_values.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 21:13:42.750493 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 21:13:42.758493 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/questions/
--rw-r--r--   0 runner    (1001) docker     (122)    59564 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/questions/assembly_line.yml
--rw-r--r--   0 runner    (1001) docker     (122)     3516 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/questions/config.yml
--rw-r--r--   0 runner    (1001) docker     (122)    14253 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/questions/feedback.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1511 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/questions/generator-test.yml
--rw-r--r--   0 runner    (1001) docker     (122)    28159 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/questions/template_validation.yml
--rw-r--r--   0 runner    (1001) docker     (122)     7439 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/questions/visual.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1103 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/questions/weaver_configuration.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 21:13:42.758493 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/sources/
--rw-r--r--   0 runner    (1001) docker     (122)      134 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/sources/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     1637 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/sources/configuration_capabilities.yml
--rw-r--r--   0 runner    (1001) docker     (122)    16960 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/sources/test_1.feature
--rw-r--r--   0 runner    (1001) docker     (122)    58510 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/sources/test_civil_docketing_statement.pdf
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 21:13:42.762493 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/static/
--rw-r--r--   0 runner    (1001) docker     (122)      105 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/static/README.md
--rw-r--r--   0 runner    (1001) docker     (122)    23095 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/static/branding_extra.png
--rw-r--r--   0 runner    (1001) docker     (122)      215 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/static/drag.png
--rw-r--r--   0 runner    (1001) docker     (122)      822 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/static/draggable_table.css
--rw-r--r--   0 runner    (1001) docker     (122)     3106 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/static/draggable_table.js
--rw-r--r--   0 runner    (1001) docker     (122)     3725 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/static/green_light.png
--rw-r--r--   0 runner    (1001) docker     (122)     5401 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/static/logo.png
--rw-r--r--   0 runner    (1001) docker     (122)    38704 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/static/logo.svg
--rw-r--r--   0 runner    (1001) docker     (122)    20509 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/static/next_steps_appeal.docx
--rw-r--r--   0 runner    (1001) docker     (122)    18507 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/static/next_steps_existing_case.docx
--rw-r--r--   0 runner    (1001) docker     (122)    18305 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/static/next_steps_letter.docx
--rw-r--r--   0 runner    (1001) docker     (122)    18000 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/static/next_steps_other.docx
--rw-r--r--   0 runner    (1001) docker     (122)    18470 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/static/next_steps_starts_case.docx
--rw-r--r--   0 runner    (1001) docker     (122)    15666 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/static/placeholder_signature.png
--rw-r--r--   0 runner    (1001) docker     (122)    10080 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/static/quality_check_overlay.pdf
--rw-r--r--   0 runner    (1001) docker     (122)      791 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/static/stop_sign.png
--rw-r--r--   0 runner    (1001) docker     (122)     3019 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/static/styles.css
--rw-r--r--   0 runner    (1001) docker     (122)    25987 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/static/undraw_collecting_re_lp6p.svg
--rw-r--r--   0 runner    (1001) docker     (122)     9154 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/static/undraw_filing_system_re_56h6.svg
--rw-r--r--   0 runner    (1001) docker     (122)    13301 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/static/undraw_start_building_re_xani.svg
--rw-r--r--   0 runner    (1001) docker     (122)    15685 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/static/undraw_upload_re_pasx.svg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 21:13:42.766493 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      102 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/templates/README.md
--rw-r--r--   0 runner    (1001) docker     (122)    23781 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/templates/next_steps_appeal.docx
--rw-r--r--   0 runner    (1001) docker     (122)    23466 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/templates/next_steps_existing_case.docx
--rw-r--r--   0 runner    (1001) docker     (122)    23143 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/templates/next_steps_letter.docx
--rw-r--r--   0 runner    (1001) docker     (122)    22933 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/templates/next_steps_other.docx
--rw-r--r--   0 runner    (1001) docker     (122)    23144 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/templates/next_steps_other_form.docx
--rw-r--r--   0 runner    (1001) docker     (122)    28185 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/templates/next_steps_starts_case.docx
--rw-r--r--   0 runner    (1001) docker     (122)    14078 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/templates/output.mako
--rw-r--r--   0 runner    (1001) docker     (122)     6327 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/templates/output_defs.mako
--rw-r--r--   0 runner    (1001) docker     (122)    68239 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/templates/quality_check_overlay.docx
--rw-r--r--   0 runner    (1001) docker     (122)    31392 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/templates/test.pdf
--rw-r--r--   0 runner    (1001) docker     (122)    60439 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/templates/test_docx.docx
--rw-r--r--   0 runner    (1001) docker     (122)   231758 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/templates/test_pdf.pdf
--rw-r--r--   0 runner    (1001) docker     (122)     4957 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/draggable_table.py
--rw-r--r--   0 runner    (1001) docker     (122)     9203 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/generator_constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    87415 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/interview_generator.py
--rw-r--r--   0 runner    (1001) docker     (122)       86 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 21:13:42.766493 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/test/
--rw-r--r--   0 runner    (1001) docker     (122)    12568 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/test/docx_file_with_reserved_keywords.docx
--rw-r--r--   0 runner    (1001) docker     (122)     9430 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/test/pdf_variables_in_docx.docx
--rw-r--r--   0 runner    (1001) docker     (122)    11473 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/test/reserved_docx_variables.docx
--rw-r--r--   0 runner    (1001) docker     (122)     4271 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/test/test_docx_no_pdf_field_names.docx
--rw-r--r--   0 runner    (1001) docker     (122)   231758 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/test/test_petition_to_enforce_sanitary_code.pdf
--rw-r--r--   0 runner    (1001) docker     (122)     6654 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/test/test_push_button.pdf
--rw-r--r--   0 runner    (1001) docker     (122)     7968 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/test/unmap_suffixes.docx
--rw-r--r--   0 runner    (1001) docker     (122)     4424 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/test_docx_files.py
--rw-r--r--   0 runner    (1001) docker     (122)     1643 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/test_feeling_lucky.py
--rw-r--r--   0 runner    (1001) docker     (122)     3208 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/test_fill_in_field_attributes.py
--rw-r--r--   0 runner    (1001) docker     (122)     9172 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/test_map_names.py
--rw-r--r--   0 runner    (1001) docker     (122)     1733 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/test_pdf_files.py
--rw-r--r--   0 runner    (1001) docker     (122)     4951 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/validate_template_files.py
--rw-r--r--   0 runner    (1001) docker     (122)      155 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/docassemble/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 21:13:42.754493 docassemble.ALWeaver-1.8.0/docassemble.ALWeaver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3449 2022-12-01 21:13:42.000000 docassemble.ALWeaver-1.8.0/docassemble.ALWeaver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3785 2022-12-01 21:13:42.000000 docassemble.ALWeaver-1.8.0/docassemble.ALWeaver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-01 21:13:42.000000 docassemble.ALWeaver-1.8.0/docassemble.ALWeaver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2022-12-01 21:13:42.000000 docassemble.ALWeaver-1.8.0/docassemble.ALWeaver.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-01 21:13:42.000000 docassemble.ALWeaver-1.8.0/docassemble.ALWeaver.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      212 2022-12-01 21:13:42.000000 docassemble.ALWeaver-1.8.0/docassemble.ALWeaver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2022-12-01 21:13:42.000000 docassemble.ALWeaver-1.8.0/docassemble.ALWeaver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       79 2022-12-01 21:13:42.770493 docassemble.ALWeaver-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     5994 2022-12-01 21:13:31.000000 docassemble.ALWeaver-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 15:33:26.766163 docassemble.ALWeaver-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3443 2023-03-15 15:33:26.766163 docassemble.ALWeaver-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2288 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 15:33:26.758163 docassemble.ALWeaver-1.9.0/docassemble/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 15:33:26.758163 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      303 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/advertise_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11812 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/custom_values.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 15:33:26.758163 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 15:33:26.762163 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/questions/
+-rw-r--r--   0 runner    (1001) docker     (122)    59591 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/questions/assembly_line.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3516 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/questions/config.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    14253 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/questions/feedback.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1511 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/questions/generator-test.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    27691 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/questions/template_validation.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     7439 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/questions/visual.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1103 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/questions/weaver_configuration.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 15:33:26.762163 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/sources/
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/sources/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1637 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/sources/configuration_capabilities.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    16960 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/sources/test_1.feature
+-rw-r--r--   0 runner    (1001) docker     (122)    58510 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/sources/test_civil_docketing_statement.pdf
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 15:33:26.762163 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/static/
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/static/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)    23095 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/static/branding_extra.png
+-rw-r--r--   0 runner    (1001) docker     (122)      215 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/static/drag.png
+-rw-r--r--   0 runner    (1001) docker     (122)      822 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/static/draggable_table.css
+-rw-r--r--   0 runner    (1001) docker     (122)     3106 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/static/draggable_table.js
+-rw-r--r--   0 runner    (1001) docker     (122)     3725 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/static/green_light.png
+-rw-r--r--   0 runner    (1001) docker     (122)     5401 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (122)    38704 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/static/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (122)    20509 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/static/next_steps_appeal.docx
+-rw-r--r--   0 runner    (1001) docker     (122)    18507 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/static/next_steps_existing_case.docx
+-rw-r--r--   0 runner    (1001) docker     (122)    18305 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/static/next_steps_letter.docx
+-rw-r--r--   0 runner    (1001) docker     (122)    18000 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/static/next_steps_other.docx
+-rw-r--r--   0 runner    (1001) docker     (122)    18470 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/static/next_steps_starts_case.docx
+-rw-r--r--   0 runner    (1001) docker     (122)    15666 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/static/placeholder_signature.png
+-rw-r--r--   0 runner    (1001) docker     (122)    10080 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/static/quality_check_overlay.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)      791 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/static/stop_sign.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3019 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/static/styles.css
+-rw-r--r--   0 runner    (1001) docker     (122)    25987 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/static/undraw_collecting_re_lp6p.svg
+-rw-r--r--   0 runner    (1001) docker     (122)     9154 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/static/undraw_filing_system_re_56h6.svg
+-rw-r--r--   0 runner    (1001) docker     (122)    13301 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/static/undraw_start_building_re_xani.svg
+-rw-r--r--   0 runner    (1001) docker     (122)    15685 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/static/undraw_upload_re_pasx.svg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 15:33:26.766163 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      102 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/templates/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)    23781 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/templates/next_steps_appeal.docx
+-rw-r--r--   0 runner    (1001) docker     (122)    23466 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/templates/next_steps_existing_case.docx
+-rw-r--r--   0 runner    (1001) docker     (122)    23143 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/templates/next_steps_letter.docx
+-rw-r--r--   0 runner    (1001) docker     (122)    22933 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/templates/next_steps_other.docx
+-rw-r--r--   0 runner    (1001) docker     (122)    23144 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/templates/next_steps_other_form.docx
+-rw-r--r--   0 runner    (1001) docker     (122)    28185 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/templates/next_steps_starts_case.docx
+-rw-r--r--   0 runner    (1001) docker     (122)    14078 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/templates/output.mako
+-rw-r--r--   0 runner    (1001) docker     (122)     6327 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/templates/output_defs.mako
+-rw-r--r--   0 runner    (1001) docker     (122)    68239 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/templates/quality_check_overlay.docx
+-rw-r--r--   0 runner    (1001) docker     (122)    31392 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/templates/test.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)    60439 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/templates/test_docx.docx
+-rw-r--r--   0 runner    (1001) docker     (122)   231758 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/templates/test_pdf.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)     4956 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/draggable_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9204 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/generator_constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    89193 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/interview_generator.py
+-rw-r--r--   0 runner    (1001) docker     (122)       86 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 15:33:26.766163 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/test/
+-rw-r--r--   0 runner    (1001) docker     (122)    12568 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/test/docx_file_with_reserved_keywords.docx
+-rw-r--r--   0 runner    (1001) docker     (122)     9430 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/test/pdf_variables_in_docx.docx
+-rw-r--r--   0 runner    (1001) docker     (122)    11473 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/test/reserved_docx_variables.docx
+-rw-r--r--   0 runner    (1001) docker     (122)     4271 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/test/test_docx_no_pdf_field_names.docx
+-rw-r--r--   0 runner    (1001) docker     (122)   231758 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/test/test_petition_to_enforce_sanitary_code.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)     6654 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/test/test_push_button.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)     7968 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/test/unmap_suffixes.docx
+-rw-r--r--   0 runner    (1001) docker     (122)     4424 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/test_docx_files.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1643 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/test_feeling_lucky.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3882 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/test_fill_in_field_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9172 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/test_map_names.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1733 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/test_pdf_files.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4951 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/validate_template_files.py
+-rw-r--r--   0 runner    (1001) docker     (122)      155 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/docassemble/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 15:33:26.758163 docassemble.ALWeaver-1.9.0/docassemble.ALWeaver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3443 2023-03-15 15:33:26.000000 docassemble.ALWeaver-1.9.0/docassemble.ALWeaver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3800 2023-03-15 15:33:26.000000 docassemble.ALWeaver-1.9.0/docassemble.ALWeaver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-15 15:33:26.000000 docassemble.ALWeaver-1.9.0/docassemble.ALWeaver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-03-15 15:33:26.000000 docassemble.ALWeaver-1.9.0/docassemble.ALWeaver.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-15 15:33:26.000000 docassemble.ALWeaver-1.9.0/docassemble.ALWeaver.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      217 2023-03-15 15:33:26.000000 docassemble.ALWeaver-1.9.0/docassemble.ALWeaver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-03-15 15:33:26.000000 docassemble.ALWeaver-1.9.0/docassemble.ALWeaver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1078 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-03-15 15:33:26.766163 docassemble.ALWeaver-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5993 2023-03-15 15:33:16.000000 docassemble.ALWeaver-1.9.0/setup.py
```

### Comparing `docassemble.ALWeaver-1.8.0/LICENSE.md` & `docassemble.ALWeaver-1.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `docassemble.ALWeaver-1.8.0/PKG-INFO` & `docassemble.ALWeaver-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docassemble.ALWeaver
-Version: 1.8.0
+Version: 1.9.0
 Home-page: https://docassemble.org
 Author: Quinten Steenhuis
 Author-email: qsteenhuis@suffolk.edu
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
@@ -30,15 +30,15 @@
 
 
 # Related repositories
 
 * https://github.com/SuffolkLitLab/docassemble-AssemblyLine
 * https://github.com/SuffolkLitLab/docassemble-ALMassachusetts
 * https://github.com/SuffolkLitLab/docassemble-MassAccess
-* https://github.com/SuffolkLitLab/docassemble-ALGenericJurisdiction
+* https://github.com/SuffolkLitLab/docassemble-ALThemeTemplate
 * https://github.com/SuffolkLitLab/EfileProxyServer
 
 # Documentation
 
 https://suffolklitlab.org/docassemble-AssemblyLine-documentation/
 
 ## History
```

### Comparing `docassemble.ALWeaver-1.8.0/README.md` & `docassemble.ALWeaver-1.9.0/docassemble.ALWeaver.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,78 +1,88 @@
-# Assembly Line Weaver: Suffolk LIT Lab Document Assembly Line
-
-<img src="https://user-images.githubusercontent.com/7645641/142245862-c2eb02ab-3090-4e97-9653-bb700bf4c54d.png" alt="drawing" width="300" alt="work together" style="align: center;"/>
-
-The Assembly Line Project is a collection of volunteers, students, and institutions who joined together
-during the COVID-19 pandemic to help increase access to the court system. Our vision is mobile-friendly,
-easy to use **guided** online forms that help empower litigants to access the court remotely.
-
-Our signature project is [CourtFormsOnline.org](https://courtformsonline.org).
-
-We designed a step-by-step, assembly line style process for automating court forms on top of Docassemble
-and built several tools along the way that **you** can use in your home jurisdiction.
-
-This package contains an **automation and rapid prototyping tool** to support authoring robust, 
-consistent, and attractive Docassemble interviews that help complete court forms. Upload a labeled
-PDF or DOCX file, and the Assembly Line Weaver will produce a runnable, clean code, draft of a
-Docassemble interview that you can continue to edit and refine.
-
-Read more on our [documentation page](https://suffolklitlab.org/docassemble-AssemblyLine-documentation/).
-
-
-# Related repositories
-
-* https://github.com/SuffolkLitLab/docassemble-AssemblyLine
-* https://github.com/SuffolkLitLab/docassemble-ALMassachusetts
-* https://github.com/SuffolkLitLab/docassemble-MassAccess
-* https://github.com/SuffolkLitLab/docassemble-ALGenericJurisdiction
-* https://github.com/SuffolkLitLab/EfileProxyServer
-
-# Documentation
-
-https://suffolklitlab.org/docassemble-AssemblyLine-documentation/
-
-## History
-* 2021-11-03
-    * Add support for *plural* names for people in PDF files
-
-* 2021-10-15
-    * Handle overflow in addendum
-    * Multiple choice radio/checkbox fields
-    * DOCX validation
-* 2021-09-09
-    * Improved internationalization
-    * Simplified PDF checker
-* 2021-04-14 Multiple fixes:
-    * Migrated to more flexible Mako template structure for generated 
-      interview blocks
-    * Package can be installed (for test purposes) after being
-      generated
-    * Various refactors and code cleanup
-    * Simplified and improved generated code and order of blocks
-    * Added version number/date stamp to generated code
-
-* 2021-03-09 Extensive improvements:
-    * Improvements to review screens
-    * Question/field editing and reordering
-    * Improvements to YAML structure
-    * Generate interstitial screens
-    * Refactoring and bug fixes
-* 2021-02-09 Combine yes/no variables; more flexible handling of people variables and assistance with gathering varying numbers w/ less code
-* 2021-01-29 Bug fixes; migration to AssemblyLine complete
-* 2021-01-25 Bug fixes, start migration to [AssemblyLine](https://github.com/SuffolkLITLab/docassemble-AssemblyLine) dependency and away from MAVirtualCourt
-
-## Authors
-
-Quinten Steenhuis, qsteenhuis@suffolk.edu  
-Michelle  
-Bryce Willey  
-Lily  
-David Colarusso  
-Nharika Singh  
-
-## Installation requirements
-
-* Create a Docassemble API key and add it your configuration like this:
-```
-install packages api key: 123458abcdefghijlklmno99A
-```
+Metadata-Version: 2.1
+Name: docassemble.ALWeaver
+Version: 1.9.0
+Home-page: https://docassemble.org
+Author: Quinten Steenhuis
+Author-email: qsteenhuis@suffolk.edu
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+# Assembly Line Weaver: Suffolk LIT Lab Document Assembly Line
+
+<img src="https://user-images.githubusercontent.com/7645641/142245862-c2eb02ab-3090-4e97-9653-bb700bf4c54d.png" alt="drawing" width="300" alt="work together" style="align: center;"/>
+
+The Assembly Line Project is a collection of volunteers, students, and institutions who joined together
+during the COVID-19 pandemic to help increase access to the court system. Our vision is mobile-friendly,
+easy to use **guided** online forms that help empower litigants to access the court remotely.
+
+Our signature project is [CourtFormsOnline.org](https://courtformsonline.org).
+
+We designed a step-by-step, assembly line style process for automating court forms on top of Docassemble
+and built several tools along the way that **you** can use in your home jurisdiction.
+
+This package contains an **automation and rapid prototyping tool** to support authoring robust, 
+consistent, and attractive Docassemble interviews that help complete court forms. Upload a labeled
+PDF or DOCX file, and the Assembly Line Weaver will produce a runnable, clean code, draft of a
+Docassemble interview that you can continue to edit and refine.
+
+Read more on our [documentation page](https://suffolklitlab.org/docassemble-AssemblyLine-documentation/).
+
+
+# Related repositories
+
+* https://github.com/SuffolkLitLab/docassemble-AssemblyLine
+* https://github.com/SuffolkLitLab/docassemble-ALMassachusetts
+* https://github.com/SuffolkLitLab/docassemble-MassAccess
+* https://github.com/SuffolkLitLab/docassemble-ALThemeTemplate
+* https://github.com/SuffolkLitLab/EfileProxyServer
+
+# Documentation
+
+https://suffolklitlab.org/docassemble-AssemblyLine-documentation/
+
+## History
+* 2021-11-03
+    * Add support for *plural* names for people in PDF files
+
+* 2021-10-15
+    * Handle overflow in addendum
+    * Multiple choice radio/checkbox fields
+    * DOCX validation
+* 2021-09-09
+    * Improved internationalization
+    * Simplified PDF checker
+* 2021-04-14 Multiple fixes:
+    * Migrated to more flexible Mako template structure for generated 
+      interview blocks
+    * Package can be installed (for test purposes) after being
+      generated
+    * Various refactors and code cleanup
+    * Simplified and improved generated code and order of blocks
+    * Added version number/date stamp to generated code
+
+* 2021-03-09 Extensive improvements:
+    * Improvements to review screens
+    * Question/field editing and reordering
+    * Improvements to YAML structure
+    * Generate interstitial screens
+    * Refactoring and bug fixes
+* 2021-02-09 Combine yes/no variables; more flexible handling of people variables and assistance with gathering varying numbers w/ less code
+* 2021-01-29 Bug fixes; migration to AssemblyLine complete
+* 2021-01-25 Bug fixes, start migration to [AssemblyLine](https://github.com/SuffolkLITLab/docassemble-AssemblyLine) dependency and away from MAVirtualCourt
+
+## Authors
+
+Quinten Steenhuis, qsteenhuis@suffolk.edu  
+Michelle  
+Bryce Willey  
+Lily  
+David Colarusso  
+Nharika Singh  
+
+## Installation requirements
+
+* Create a Docassemble API key and add it your configuration like this:
+```
+install packages api key: 123458abcdefghijlklmno99A
+```
```

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/custom_values.py` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/custom_values.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Any, Dict, List, Union, Optional
 from pathlib import Path
 import ruamel.yaml as yaml
 from docassemble.base.util import log, DADict, DAList, DAStore, path_and_mimetype
 from packaging.version import Version
 from more_itertools import unique_everseen
 
+
 ################# To refactor - I don't think these are used but they are mentioned in interview_generator.py
 class CustomValues(object):
     people_plurals_map: Dict[str, str]
     org_specific_config: Any
 
 
 custom_values = CustomValues()
```

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/questions/assembly_line.yml` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/questions/assembly_line.yml`

 * *Files 0% similar despite different names*

```diff
@@ -48,14 +48,15 @@
       elif all(map(lambda y: True if y.filename.endswith(".docx") else False, interview.uploaded_templates)):
         initial_get_fields
         validate_field_names
         if no_recognized_docx_fields:
           warn_no_recognized_al_labels
         validate_docx
       else: # mixed PDF and DOCX templates
+        initial_get_fields
         validate_mixed_documents
  
   if have_template_to_load:  
     interview.all_fields.gathered
   # Display Weaver question screens
   interview.jurisdiction_choices
   interview.form_type
```

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/questions/config.yml` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/questions/config.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/questions/feedback.yml` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/questions/feedback.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/questions/generator-test.yml` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/questions/generator-test.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/questions/template_validation.yml` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/questions/template_validation.yml`

 * *Files 2% similar despite different names*

```diff
@@ -402,21 +402,21 @@
   
 fields:
   - note: |
       Confirm your approval of the filled-in PDF. All the boxes must be checked, or you'll get an error message along with instructions to correct the issues.
   - Confirm the fields are filled in correctly: all_look_good
     datatype: checkboxes
     choices:
-      - All the checkboxes are checked: all_checkboxes_checked
+      - All the checkboxes are checked and at least one radio button in each group is selected: all_checkboxes_checked
       - The fonts and styles in the preview look okay OR I am comfortable fixing them later: no_unusual_size_text
         help: |
           While you may prefer to fix font size now, it will not change your experience
           with the Weaver. You can upload the fixed template to the Playground later.
       - All signature fields are filled in with the signature image: signature_filled_in
-    none of the above: False    
+    none of the above: False
 validation code: |
   checkboxes_msg = ''
   text_mst = ''
   signature_msg = ''
   if not all_look_good['all_checkboxes_checked']:
     checkboxes_msg = "<ul><li>You didn't confirm 'All the checkboxes are checked'. Check the field's 'export' value. It should be set to 'Yes'.</li></ul>"
   if not all_look_good['no_unusual_size_text']:
@@ -472,42 +472,24 @@
     code: |
       interview.uploaded_templates
   code: |
     reflect_fields(interview.uploaded_templates[0].get_pdf_fields(), placeholder_signature)
 ---
 code: |
   from pdfminer.pdfparser import PDFSyntaxError
-  from PyPDF2.utils import PdfReadError
   
   try:
     pdf_concatenate(interview.uploaded_templates)
   except PDFSyntaxError:
     # Handle PDF read error
     force_ask('exit_invalid_pdf')
-  except PdfReadError:
-    force_ask('exit_xref_table')
   except:
     pass # Continue on to safer checks with get_pdf_fields
   validate_pdf = True
 ---
-event: exit_xref_table
-question: |
-  This PDF is not valid
-subquestion: |
-  There was a problem reading this PDF.
-  
-  Sometimes you can fix this problem by using 
-  [documate.org/pdf](https://www.documate.org/pdf) or by using 
-  [qpdf](http://qpdf.sourceforge.net/).
-  
-  [Read 
-  more](https://suffolklitlab.org/docassemble-AssemblyLine-documentation/docs/pdfs#corrupted-or-locked-pdfs).
-buttons:
-  - Restart: restart
----
 ###################### DOCX validation stuff #############################
 ---
 code: |
   verify_docx_fields 
   validate_docx = True
 ---
 code: |
```

#### html2text {}

```diff
@@ -191,23 +191,23 @@
 | Here is the filled-in PDF subquestion: | The fields are filled in with the
 names listed in the table on the previous screen. All signature fields should
 be filled in with this image: ${placeholder_signature} % for document in
 interview.uploaded_templates: ${ collapse_template(document.preview_template) }
 % endfor fields: - note: | Confirm your approval of the filled-in PDF. All the
 boxes must be checked, or you'll get an error message along with instructions
 to correct the issues. - Confirm the fields are filled in correctly:
-all_look_good datatype: checkboxes choices: - All the checkboxes are checked:
-all_checkboxes_checked - The fonts and styles in the preview look okay OR I am
-comfortable fixing them later: no_unusual_size_text help: | While you may
-prefer to fix font size now, it will not change your experience with the
-Weaver. You can upload the fixed template to the Playground later. - All
-signature fields are filled in with the signature image: signature_filled_in
-none of the above: False validation code: | checkboxes_msg = '' text_mst = ''
-signature_msg = '' if not all_look_good['all_checkboxes_checked']:
-checkboxes_msg = "
+all_look_good datatype: checkboxes choices: - All the checkboxes are checked
+and at least one radio button in each group is selected: all_checkboxes_checked
+- The fonts and styles in the preview look okay OR I am comfortable fixing them
+later: no_unusual_size_text help: | While you may prefer to fix font size now,
+it will not change your experience with the Weaver. You can upload the fixed
+template to the Playground later. - All signature fields are filled in with the
+signature image: signature_filled_in none of the above: False validation code:
+| checkboxes_msg = '' text_mst = '' signature_msg = '' if not all_look_good
+['all_checkboxes_checked']: checkboxes_msg = "
     * You didn't confirm 'All the checkboxes are checked'. Check the field's
       'export' value. It should be set to 'Yes'.
 " if not all_look_good['no_unusual_size_text']: text_mst = "
     * You didn't confirm 'No unusually sized text'. Check the font sizes of
       those fields, and if the field is set to allow multiple lines.
 " if not all_look_good['signature_filled_in']: signature_msg = "
     * You didn't confirm 'All signature fields are filled in with the signature
@@ -230,32 +230,26 @@
 ()] right: | #### Preview of PDF label placement  _note_: This preview will not
 update with live changes. continue button field: display_rename_field_choices -
 -- code: | rename_pdf_fields(interview.uploaded_templates[0].path(),
 rename_fields) renamed_fields = True --- attachment: variable name:
 field_preview_pdf editable: False pdf template file: code: |
 interview.uploaded_templates code: | reflect_fields
 (interview.uploaded_templates[0].get_pdf_fields(), placeholder_signature) --
-- code: | from pdfminer.pdfparser import PDFSyntaxError from PyPDF2.utils
-import PdfReadError try: pdf_concatenate(interview.uploaded_templates) except
-PDFSyntaxError: # Handle PDF read error force_ask('exit_invalid_pdf') except
-PdfReadError: force_ask('exit_xref_table') except: pass # Continue on to safer
-checks with get_pdf_fields validate_pdf = True --- event: exit_xref_table
-question: | This PDF is not valid subquestion: | There was a problem reading
-this PDF. Sometimes you can fix this problem by using [documate.org/pdf](https:
-//www.documate.org/pdf) or by using [qpdf](http://qpdf.sourceforge.net/). [Read
-more](https://suffolklitlab.org/docassemble-AssemblyLine-documentation/docs/
-pdfs#corrupted-or-locked-pdfs). buttons: - Restart: restart --
-- ###################### DOCX validation stuff ############################# --
-- code: | verify_docx_fields validate_docx = True --- code: |
-no_recognized_docx_fields = not (any(field for field in validation_fields if
-field.reserved) or len(validation_people_list)) --- id: Did you intend to use
-Mako syntax question: | Did you intend to use Mako syntax? subquestion: | Your
-DOCX template looks like it is using the Mako syntax ${ }. Usually this is an
-error. DOCX files use Jinja2 syntax, not Mako. You may want to stop here and
-fix your template by replacing any instances of <%text>`${ }` with `{{ }}`.
+- code: | from pdfminer.pdfparser import PDFSyntaxError try: pdf_concatenate
+(interview.uploaded_templates) except PDFSyntaxError: # Handle PDF read error
+force_ask('exit_invalid_pdf') except: pass # Continue on to safer checks with
+get_pdf_fields validate_pdf = True --- ###################### DOCX validation
+stuff ############################# --- code: | verify_docx_fields
+validate_docx = True --- code: | no_recognized_docx_fields = not (any(field for
+field in validation_fields if field.reserved) or len(validation_people_list)) -
+-- id: Did you intend to use Mako syntax question: | Did you intend to use Mako
+syntax? subquestion: | Your DOCX template looks like it is using the Mako
+syntax ${ }. Usually this is an error. DOCX files use Jinja2 syntax, not Mako.
+You may want to stop here and fix your template by replacing any instances of
+<%text>`${ }` with `{{ }}`.
 text> These are the lines that look like they contain Mako syntax: % for match
 in mako_matches: * ${ match } % endfor If the matches above are "false
 positives" or you intentionally used Mako syntax in your DOCX file, keep on
 going, but your template might not do what you intended. Check out the
 documentation for [python-docx-template](https://docxtpl.readthedocs.io/en/
 latest/#jinja2-like-syntax) and for [Jinja2](https://jinja.palletsprojects.com/
 en/3.0.x/) to learn more. sets: mako_syntax_in_docx buttons: - I understand,
```

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/questions/visual.yml` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/questions/visual.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/questions/weaver_configuration.yml` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/questions/weaver_configuration.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/sources/configuration_capabilities.yml` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/sources/configuration_capabilities.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/sources/test_1.feature` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/sources/test_1.feature`

 * *Files identical despite different names*

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/sources/test_civil_docketing_statement.pdf` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/sources/test_civil_docketing_statement.pdf`

 * *Files identical despite different names*

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/static/branding_extra.png` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/static/branding_extra.png`

 * *Files identical despite different names*

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/static/draggable_table.css` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/static/draggable_table.css`

 * *Files identical despite different names*

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/static/draggable_table.js` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/static/draggable_table.js`

 * *Files identical despite different names*

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/static/green_light.png` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/static/green_light.png`

 * *Files identical despite different names*

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/static/logo.png` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/static/logo.png`

 * *Files identical despite different names*

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/static/logo.svg` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/static/logo.svg`

 * *Files identical despite different names*

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/static/next_steps_appeal.docx` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/static/next_steps_appeal.docx`

 * *Files identical despite different names*

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/static/next_steps_existing_case.docx` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/static/next_steps_existing_case.docx`

 * *Files identical despite different names*

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/static/next_steps_letter.docx` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/static/next_steps_letter.docx`

 * *Files identical despite different names*

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/static/next_steps_other.docx` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/static/next_steps_other.docx`

 * *Files identical despite different names*

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/static/next_steps_starts_case.docx` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/static/next_steps_starts_case.docx`

 * *Files identical despite different names*

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/static/placeholder_signature.png` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/static/placeholder_signature.png`

 * *Files identical despite different names*

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/static/quality_check_overlay.pdf` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/static/quality_check_overlay.pdf`

 * *Files identical despite different names*

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/static/stop_sign.png` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/static/stop_sign.png`

 * *Files identical despite different names*

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/static/styles.css` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/static/styles.css`

 * *Files identical despite different names*

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/static/undraw_collecting_re_lp6p.svg` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/static/undraw_collecting_re_lp6p.svg`

 * *Files identical despite different names*

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/static/undraw_filing_system_re_56h6.svg` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/static/undraw_filing_system_re_56h6.svg`

 * *Files identical despite different names*

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/static/undraw_start_building_re_xani.svg` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/static/undraw_start_building_re_xani.svg`

 * *Files identical despite different names*

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/static/undraw_upload_re_pasx.svg` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/static/undraw_upload_re_pasx.svg`

 * *Files identical despite different names*

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/templates/next_steps_appeal.docx` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/templates/next_steps_appeal.docx`

 * *Files identical despite different names*

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/templates/next_steps_existing_case.docx` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/templates/next_steps_existing_case.docx`

 * *Files identical despite different names*

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/templates/next_steps_letter.docx` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/templates/next_steps_letter.docx`

 * *Files identical despite different names*

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/templates/next_steps_other.docx` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/templates/next_steps_other.docx`

 * *Files identical despite different names*

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/templates/next_steps_other_form.docx` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/templates/next_steps_other_form.docx`

 * *Files identical despite different names*

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/templates/next_steps_starts_case.docx` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/templates/next_steps_starts_case.docx`

 * *Files identical despite different names*

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/templates/output.mako` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/templates/output.mako`

 * *Files identical despite different names*

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/templates/output_defs.mako` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/templates/output_defs.mako`

 * *Files identical despite different names*

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/templates/quality_check_overlay.docx` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/templates/quality_check_overlay.docx`

 * *Files identical despite different names*

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/templates/test.pdf` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/templates/test.pdf`

 * *Files identical despite different names*

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/templates/test_docx.docx` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/templates/test_docx.docx`

 * *Files identical despite different names*

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/data/templates/test_pdf.pdf` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/data/templates/test_pdf.pdf`

 * *Files identical despite different names*

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/draggable_table.py` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/draggable_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,14 @@
     # 2. Prepare for json string
     collections = list()
     headings = list()
     headings = old_soup.find_all("th")
 
     # 3. Loop thru the adjusted order and copy data from old_soup to collections
     for j, row_name in enumerate(adjusted_order):
-
         # Handle one row at a time.
         old_tbl_rows = old_soup.find_all("tr")[1:]  # skip heading row
         for old_row in old_tbl_rows:
             old_cells = old_row.find_all("td")
 
             if row_name in old_cells[1].get_text():  # found a matching row (field name)
                 # Create a dict record using heading as its keys.
```

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/generator_constants.py` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/generator_constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Constants for interview_generator.py
 """
 from typing import Dict, List
 
+
 # This is to workaround fact you can't do local import in Docassemble playground
 class GeneratorConstantObject(object):
     RESERVED_WHOLE_WORDS: List[str]
     UNDEFINED_PERSON_PREFIXES: List[str]
     ALLOW_SINGULAR_SUFFIXES: List[str]
     RESERVED_PERSON_PLURALIZERS_MAP: Dict[str, str]
     RESERVED_PREFIXES: List[str]
```

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/interview_generator.py` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/interview_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 )
 from docx2python import docx2python
 from enum import Enum
 from itertools import zip_longest, chain
 from pdfminer.pdfparser import PDFSyntaxError
 from pdfminer.psparser import PSEOF
 from pikepdf import Pdf
-from PyPDF2.utils import PdfReadError
 from typing import Any, Dict, List, Optional, Set, Tuple, Union, Iterable
 from urllib.parse import urlparse
 from zipfile import BadZipFile
 import ast
 import ast
 import datetime
 import docassemble.base.functions
@@ -153,15 +152,19 @@
 
     0: horizontal start
     1: vertical start
     2: horizontal end
     3: vertical end
     """
     # Make sure it's the right kind of tuple
-    if len(pdf_field_tuple) < 3 or (pdf_field_tuple[3] and len(pdf_field_tuple[3]) < 4):
+    if (
+        len(pdf_field_tuple) < 4
+        or not pdf_field_tuple[3]
+        or len(pdf_field_tuple[3]) < 4
+    ):
         return None  # we can't really guess
 
     # Did a little testing for typical field width/number of chars with both w and e.
     # 176 = 25-34 chars. from w to e
     # 121 = 17-22
     # Average about 6 pixels width per character
     # about 12 pixels high is one row
@@ -264,27 +267,40 @@
         self.final_display_var = map_raw_to_final_display(self.variable)
 
         variable_name_guess = self.variable.replace("_", " ").capitalize()
         self.has_label = True
         self.maxlength = get_character_limit(pdf_field_tuple)
         self.variable_name_guess = variable_name_guess
 
+        self.export_value = pdf_field_tuple[5] if len(pdf_field_tuple) >= 6 else ""
         if self.variable.endswith("_date"):
             self.field_type_guess = "date"
             self.variable_name_guess = "Date of " + self.variable[:-5].replace("_", " ")
         elif self.variable.endswith("_yes") or self.variable.endswith("_no"):
             self.field_type_guess = "yesno"
             name_no_suffix = (
                 self.variable[:-3]
                 if self.variable.endswith("_no")
                 else self.variable[:-4]
             )
             self.variable_name_guess = name_no_suffix.replace("_", " ").capitalize()
         elif pdf_field_tuple[4] == "/Btn":
-            self.field_type_guess = "yesno"
+            if str(self.export_value.lower()) in [
+                "yes",
+                "true",
+                "on",
+                "no",
+                "false",
+                "off",
+                "",
+            ]:
+                self.field_type_guess = "yesno"
+            else:
+                self.field_type_guess = "multiple choice radio"
+                self.choice_options = [self.export_value]
         elif pdf_field_tuple[4] == "/Sig":
             self.field_type_guess = "signature"
         elif self.maxlength and self.maxlength > 100:
             self.field_type_guess = "area"
         elif self.variable.endswith("_amount"):
             self.field_type_guess = "currency"
         elif self.variable.endswith("_value"):
@@ -411,14 +427,17 @@
         )
         field_questions.append(
             {
                 "label": "Options (one per line)",
                 "field": self.attr_name("choices"),
                 "datatype": "area",
                 "js show if": f"['multiple choice dropdown','multiple choice combobox','multiselect', 'multiple choice radio', 'multiple choice checkboxes'].includes(val('{ self.attr_name('field_type') }'))",
+                "default": "\n".join(self.choice_options)
+                if hasattr(self, "choice_options")
+                else None,
                 "hint": "Like 'Descriptive name: key_name', or just 'Descriptive name'",
             }
         )
         if hasattr(self, "maxlength"):
             field_questions.append(
                 {
                     "label": "Send overflow text to addendum",
@@ -657,14 +676,34 @@
 
             if len(yesno_map[field.variable_name_guess]) > 1:
                 mark_to_remove.append(idx)
 
         self.delitem(*mark_to_remove)
         self.there_are_any = len(self.elements) > 0
 
+    def consolidate_radios(self) -> None:
+        """Combines separate radio buttons into a single variable"""
+        radio_map: Dict[str, Any] = defaultdict(list)
+        mark_to_remove: List[int] = []
+        for idx, field in enumerate(self.elements):
+            if field.field_type_guess != "multiple choice radio":
+                continue
+
+            if len(radio_map[field.variable_name_guess]) > 0:
+                radio_map[field.variable_name_guess][0].choice_options.append(
+                    field.export_value
+                )
+            radio_map[field.variable_name_guess].append(field)
+
+            if len(radio_map[field.variable_name_guess]) > 1:
+                mark_to_remove.append(idx)
+
+        self.delitem(*mark_to_remove)
+        self.there_are_any = len(self.elements) > 0
+
     def consolidate_duplicate_fields(self, document_type: str = "pdf") -> None:
         """Removes all duplicate fields from a PDF (docx's are handled elsewhere) that really just
         represent a single variable, leaving one remaining field that writes all of the original vars
         """
         if document_type.lower() == "docx":
             return
 
@@ -719,14 +758,15 @@
             pike_fields: Dict = {}
             pike_obj = Pdf.open(document.path())
             if pike_obj.Root.AcroForm.Fields and isinstance(
                 pike_obj.Root.AcroForm.Fields, Iterable
             ):
                 for pike_info in pike_obj.Root.AcroForm.Fields:
                     pike_fields[str(pike_info.T)] = pike_info
+            pike_obj.close()
             for pdf_field_tuple, pike_info in zip_longest(all_fields, pike_fields):
                 pdf_field_name = pdf_field_tuple[0]
                 if pdf_field_name in pike_fields:
                     pike_info = pike_fields[pdf_field_name]
                     # PDF fields have bit flags that set specific options. The 17th bit (or hex
                     # 10000) on Buttons says it's a "push button", that "does not retain a
                     # permanent value" (e.g. a "Print this PDF" button.) They generally aren't
@@ -768,14 +808,15 @@
                     new_field.group = DAFieldGroup.SIGNATURE
                 else:
                     new_field.group = DAFieldGroup.CUSTOM
                 new_field.fill_in_docx_attributes(field)
                 if new_field.group in [DAFieldGroup.BUILT_IN, DAFieldGroup.RESERVED]:
                     new_field.label = new_field.variable_name_guess
 
+        self.consolidate_radios()
         self.consolidate_duplicate_fields(document_type)
         self.consolidate_yesnos()
 
     def ask_about_fields(self) -> List[dict]:
         """
         Return a list of Docassemble fields that ask the user to verify type and
         label each "custom" field in the field list
@@ -1180,15 +1221,14 @@
 
     def create_package(
         self,
         interview_mako_output: DAFileCollection,
         generate_download_screen: bool = True,
         output_file: Optional[DAFile] = None,
     ) -> DAFile:
-
         # 2. Build data for folders_and_files and package_info
         folders_and_files = {
             "questions": [interview_mako_output],
             "modules": [],
             "static": [],
             "sources": [],
         }
@@ -1854,15 +1894,15 @@
 
 def get_pdf_validation_errors(document: DAFile) -> Optional[ValidationError]:
     try:
         fields = DAFieldList()
         fields.add_fields_from_file(document)
     except ParsingException as ex:
         return ("parsing_exception", ex)
-    except (PDFSyntaxError, PdfReadError):
+    except PDFSyntaxError:
         return ("invalid_pdf", "Invalid PDF")
     except PSEOF:
         return (
             "pseof",
             "File appears incomplete (PSEOF error). Is this a valid PDF file?",
         )
     except:
@@ -1934,15 +1974,22 @@
 ) -> List[Dict[str, str]]:
     """Return a mapping between the field names and either the same name, or "yes"
     if the field is a checkbox value, in order to visually capture the location of
     labeled fields on the PDF."""
     mapping = []
     for field in pdf_field_tuples:
         if field[4] == "/Btn":
-            mapping.append({field[0]: "Yes"})
+            export_val = field[5] if len(field) >= 6 else ""
+            if str(export_val).lower() in ["yes", "on", "true", ""]:
+                mapping.append({field[0]: "Yes"})
+            else:
+                if field[0] not in [
+                    next(iter(field_val.keys())) for field_val in mapping
+                ]:
+                    mapping.append({field[0]: export_val})
         elif field[4] == "/Sig" and image_placeholder:
             mapping.append({field[0]: image_placeholder})
         else:
             mapping.append({field[0]: field[0]})
     return mapping
```

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/test/docx_file_with_reserved_keywords.docx` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/test/docx_file_with_reserved_keywords.docx`

 * *Files identical despite different names*

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/test/pdf_variables_in_docx.docx` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/test/pdf_variables_in_docx.docx`

 * *Files identical despite different names*

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/test/reserved_docx_variables.docx` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/test/reserved_docx_variables.docx`

 * *Files identical despite different names*

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/test/test_docx_no_pdf_field_names.docx` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/test/test_docx_no_pdf_field_names.docx`

 * *Files identical despite different names*

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/test/test_petition_to_enforce_sanitary_code.pdf` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/test/test_petition_to_enforce_sanitary_code.pdf`

 * *Files identical despite different names*

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/test/test_push_button.pdf` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/test/test_push_button.pdf`

 * *Files identical despite different names*

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/test/unmap_suffixes.docx` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/test/unmap_suffixes.docx`

 * *Files identical despite different names*

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/test_docx_files.py` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/test_docx_files.py`

 * *Files identical despite different names*

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/test_feeling_lucky.py` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/test_feeling_lucky.py`

 * *Files identical despite different names*

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/test_fill_in_field_attributes.py` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/test_fill_in_field_attributes.py`

 * *Files 12% similar despite different names*

```diff
@@ -59,10 +59,28 @@
         new_field.fill_in_pdf_attributes(pdf_field_tuple)
         self.assertEqual(new_field.variable, "signature")
         self.assertEqual(new_field.final_display_var, "signature")
         self.assertEqual(new_field.has_label, True)
         self.assertEqual(new_field.field_type_guess, "signature")
         self.assertEqual(new_field.variable_name_guess, "Signature")
 
+    def test_multiple_choice(self):
+        # From an Adobe-Acrobat made radio button field
+        pdf_field_tuple = (
+            "Group1",
+            "No",
+            1,
+            [162.9, 631.3, 180.9, 649.3],
+            "/Btn",
+            "Choice3",
+        )
+        new_field = DAField()
+        new_field.fill_in_pdf_attributes(pdf_field_tuple)
+        self.assertEqual(new_field.variable, "Group1")
+        self.assertEqual(new_field.final_display_var, "Group1")
+        self.assertEqual(new_field.has_label, True)
+        self.assertEqual(new_field.field_type_guess, "multiple choice radio")
+        self.assertEqual(new_field.variable_name_guess, "Group1")
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/test_map_names.py` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/test_map_names.py`

 * *Files identical despite different names*

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/test_pdf_files.py` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/test_pdf_files.py`

 * *Files identical despite different names*

### Comparing `docassemble.ALWeaver-1.8.0/docassemble/ALWeaver/validate_template_files.py` & `docassemble.ALWeaver-1.9.0/docassemble/ALWeaver/validate_template_files.py`

 * *Files identical despite different names*

### Comparing `docassemble.ALWeaver-1.8.0/docassemble.ALWeaver.egg-info/SOURCES.txt` & `docassemble.ALWeaver-1.9.0/docassemble.ALWeaver.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE.md
 MANIFEST.in
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 docassemble/__init__.py
 docassemble.ALWeaver.egg-info/PKG-INFO
 docassemble.ALWeaver.egg-info/SOURCES.txt
 docassemble.ALWeaver.egg-info/dependency_links.txt
 docassemble.ALWeaver.egg-info/namespace_packages.txt
```

### Comparing `docassemble.ALWeaver-1.8.0/setup.py` & `docassemble.ALWeaver-1.9.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,22 +39,22 @@
                         break
                 if bad_name:
                     continue
                 out.setdefault(package, []).append(prefix+name)
     return out
 
 setup(name='docassemble.ALWeaver',
-      version='1.8.0',
+      version='1.9.0',
       description=(''),
-      long_description='# Assembly Line Weaver: Suffolk LIT Lab Document Assembly Line\r\n\r\n<img src="https://user-images.githubusercontent.com/7645641/142245862-c2eb02ab-3090-4e97-9653-bb700bf4c54d.png" alt="drawing" width="300" alt="work together" style="align: center;"/>\r\n\r\nThe Assembly Line Project is a collection of volunteers, students, and institutions who joined together\r\nduring the COVID-19 pandemic to help increase access to the court system. Our vision is mobile-friendly,\r\neasy to use **guided** online forms that help empower litigants to access the court remotely.\r\n\r\nOur signature project is [CourtFormsOnline.org](https://courtformsonline.org).\r\n\r\nWe designed a step-by-step, assembly line style process for automating court forms on top of Docassemble\r\nand built several tools along the way that **you** can use in your home jurisdiction.\r\n\r\nThis package contains an **automation and rapid prototyping tool** to support authoring robust, \r\nconsistent, and attractive Docassemble interviews that help complete court forms. Upload a labeled\r\nPDF or DOCX file, and the Assembly Line Weaver will produce a runnable, clean code, draft of a\r\nDocassemble interview that you can continue to edit and refine.\r\n\r\nRead more on our [documentation page](https://suffolklitlab.org/docassemble-AssemblyLine-documentation/).\r\n\r\n\r\n# Related repositories\r\n\r\n* https://github.com/SuffolkLitLab/docassemble-AssemblyLine\r\n* https://github.com/SuffolkLitLab/docassemble-ALMassachusetts\r\n* https://github.com/SuffolkLitLab/docassemble-MassAccess\r\n* https://github.com/SuffolkLitLab/docassemble-ALGenericJurisdiction\r\n* https://github.com/SuffolkLitLab/EfileProxyServer\r\n\r\n# Documentation\r\n\r\nhttps://suffolklitlab.org/docassemble-AssemblyLine-documentation/\r\n\r\n## History\r\n* 2021-11-03\r\n    * Add support for *plural* names for people in PDF files\r\n\r\n* 2021-10-15\r\n    * Handle overflow in addendum\r\n    * Multiple choice radio/checkbox fields\r\n    * DOCX validation\r\n* 2021-09-09\r\n    * Improved internationalization\r\n    * Simplified PDF checker\r\n* 2021-04-14 Multiple fixes:\r\n    * Migrated to more flexible Mako template structure for generated \r\n      interview blocks\r\n    * Package can be installed (for test purposes) after being\r\n      generated\r\n    * Various refactors and code cleanup\r\n    * Simplified and improved generated code and order of blocks\r\n    * Added version number/date stamp to generated code\r\n\r\n* 2021-03-09 Extensive improvements:\r\n    * Improvements to review screens\r\n    * Question/field editing and reordering\r\n    * Improvements to YAML structure\r\n    * Generate interstitial screens\r\n    * Refactoring and bug fixes\r\n* 2021-02-09 Combine yes/no variables; more flexible handling of people variables and assistance with gathering varying numbers w/ less code\r\n* 2021-01-29 Bug fixes; migration to AssemblyLine complete\r\n* 2021-01-25 Bug fixes, start migration to [AssemblyLine](https://github.com/SuffolkLITLab/docassemble-AssemblyLine) dependency and away from MAVirtualCourt\r\n\r\n## Authors\r\n\r\nQuinten Steenhuis, qsteenhuis@suffolk.edu  \r\nMichelle  \r\nBryce Willey  \r\nLily  \r\nDavid Colarusso  \r\nNharika Singh  \r\n\r\n## Installation requirements\r\n\r\n* Create a Docassemble API key and add it your configuration like this:\r\n```\r\ninstall packages api key: 123458abcdefghijlklmno99A\r\n```\r\n',
+      long_description='# Assembly Line Weaver: Suffolk LIT Lab Document Assembly Line\r\n\r\n<img src="https://user-images.githubusercontent.com/7645641/142245862-c2eb02ab-3090-4e97-9653-bb700bf4c54d.png" alt="drawing" width="300" alt="work together" style="align: center;"/>\r\n\r\nThe Assembly Line Project is a collection of volunteers, students, and institutions who joined together\r\nduring the COVID-19 pandemic to help increase access to the court system. Our vision is mobile-friendly,\r\neasy to use **guided** online forms that help empower litigants to access the court remotely.\r\n\r\nOur signature project is [CourtFormsOnline.org](https://courtformsonline.org).\r\n\r\nWe designed a step-by-step, assembly line style process for automating court forms on top of Docassemble\r\nand built several tools along the way that **you** can use in your home jurisdiction.\r\n\r\nThis package contains an **automation and rapid prototyping tool** to support authoring robust, \r\nconsistent, and attractive Docassemble interviews that help complete court forms. Upload a labeled\r\nPDF or DOCX file, and the Assembly Line Weaver will produce a runnable, clean code, draft of a\r\nDocassemble interview that you can continue to edit and refine.\r\n\r\nRead more on our [documentation page](https://suffolklitlab.org/docassemble-AssemblyLine-documentation/).\r\n\r\n\r\n# Related repositories\r\n\r\n* https://github.com/SuffolkLitLab/docassemble-AssemblyLine\r\n* https://github.com/SuffolkLitLab/docassemble-ALMassachusetts\r\n* https://github.com/SuffolkLitLab/docassemble-MassAccess\r\n* https://github.com/SuffolkLitLab/docassemble-ALThemeTemplate\r\n* https://github.com/SuffolkLitLab/EfileProxyServer\r\n\r\n# Documentation\r\n\r\nhttps://suffolklitlab.org/docassemble-AssemblyLine-documentation/\r\n\r\n## History\r\n* 2021-11-03\r\n    * Add support for *plural* names for people in PDF files\r\n\r\n* 2021-10-15\r\n    * Handle overflow in addendum\r\n    * Multiple choice radio/checkbox fields\r\n    * DOCX validation\r\n* 2021-09-09\r\n    * Improved internationalization\r\n    * Simplified PDF checker\r\n* 2021-04-14 Multiple fixes:\r\n    * Migrated to more flexible Mako template structure for generated \r\n      interview blocks\r\n    * Package can be installed (for test purposes) after being\r\n      generated\r\n    * Various refactors and code cleanup\r\n    * Simplified and improved generated code and order of blocks\r\n    * Added version number/date stamp to generated code\r\n\r\n* 2021-03-09 Extensive improvements:\r\n    * Improvements to review screens\r\n    * Question/field editing and reordering\r\n    * Improvements to YAML structure\r\n    * Generate interstitial screens\r\n    * Refactoring and bug fixes\r\n* 2021-02-09 Combine yes/no variables; more flexible handling of people variables and assistance with gathering varying numbers w/ less code\r\n* 2021-01-29 Bug fixes; migration to AssemblyLine complete\r\n* 2021-01-25 Bug fixes, start migration to [AssemblyLine](https://github.com/SuffolkLITLab/docassemble-AssemblyLine) dependency and away from MAVirtualCourt\r\n\r\n## Authors\r\n\r\nQuinten Steenhuis, qsteenhuis@suffolk.edu  \r\nMichelle  \r\nBryce Willey  \r\nLily  \r\nDavid Colarusso  \r\nNharika Singh  \r\n\r\n## Installation requirements\r\n\r\n* Create a Docassemble API key and add it your configuration like this:\r\n```\r\ninstall packages api key: 123458abcdefghijlklmno99A\r\n```\r\n',
       long_description_content_type='text/markdown',
       author='Quinten Steenhuis',
       author_email='qsteenhuis@suffolk.edu',
       license='MIT',
       url='https://docassemble.org',
       packages=find_packages(),
       namespace_packages=['docassemble'],
-      install_requires=['PyYAML>=5.1.2', 'beautifulsoup4>=4.11.1', 'docassemble.ALToolbox>=0.4.2', 'docassemble.AssemblyLine>=2.11.3', 'docx2python>=1.27.1', 'formfyxer>=0.0.9', 'more-itertools>=8.6.0', 'numpy>=1.0.4', 'pikepdf>=5.1.1', 'sklearn>=0.0', 'spacy>=3.2.0'],
+      install_requires=['PyYAML>=5.1.2', 'beautifulsoup4>=4.11.1', 'docassemble.ALToolbox>=0.4.2', 'docassemble.AssemblyLine>=2.11.3', 'docx2python>=1.27.1', 'formfyxer>=0.0.9', 'more-itertools>=8.6.0', 'numpy>=1.0.4', 'pikepdf>=5.1.1', 'scikit-learn>=0.0', 'spacy>=3.2.0'],
       zip_safe=False,
       package_data=find_package_data(where='docassemble/ALWeaver/', package='docassemble.ALWeaver'),
      )
```

