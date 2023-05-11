# Comparing `tmp/vocalpy-0.2.0.post1.tar.gz` & `tmp/vocalpy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vocalpy-0.2.0.post1.tar", last modified: Sun May  7 22:11:50 2023, max compression
+gzip compressed data, was "vocalpy-0.3.0.tar", last modified: Thu May 11 16:08:23 2023, max compression
```

## Comparing `vocalpy-0.2.0.post1.tar` & `vocalpy-0.3.0.tar`

### file list

```diff
@@ -1,82 +1,93 @@
--rw-r--r--   0        0        0     1307 2023-05-07 21:41:12.898528 vocalpy-0.2.0.post1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      248 2023-05-07 21:39:43.229568 vocalpy-0.2.0.post1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      615 2023-05-07 21:39:43.228362 vocalpy-0.2.0.post1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      750 2023-05-07 20:16:29.801006 vocalpy-0.2.0.post1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      286 2023-04-25 13:42:56.058591 vocalpy-0.2.0.post1/.gitignore
--rw-r--r--   0        0        0      769 2023-04-25 13:42:56.059258 vocalpy-0.2.0.post1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      367 2023-05-07 21:38:34.576998 vocalpy-0.2.0.post1/.readthedocs.yaml
--rw-r--r--   0        0        0     5556 2023-05-07 20:52:52.998672 vocalpy-0.2.0.post1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1867 2023-05-07 20:53:11.404957 vocalpy-0.2.0.post1/CONTRIBUTING.md
--rw-r--r--   0        0        0     1540 2023-04-08 15:55:30.246016 vocalpy-0.2.0.post1/LICENSE
--rw-r--r--   0        0        0     2064 2023-04-08 15:55:30.246197 vocalpy-0.2.0.post1/Makefile
--rw-r--r--   0        0        0     3353 2023-05-07 22:07:24.777217 vocalpy-0.2.0.post1/README.md
--rw-r--r--   0        0        0      251 2023-05-07 20:48:44.343584 vocalpy-0.2.0.post1/docs/CHANGELOG.md
--rw-r--r--   0        0        0    29965 2023-05-07 20:41:50.515176 vocalpy-0.2.0.post1/docs/_static/vocalpy-logomark.png
--rw-r--r--   0        0        0   285798 2023-05-07 20:41:50.763203 vocalpy-0.2.0.post1/docs/_static/vocalpy-primary.png
--rw-r--r--   0        0        0   194159 2023-05-07 20:41:50.588788 vocalpy-0.2.0.post1/docs/_static/vocalpy-secondary.png
--rw-r--r--   0        0        0     6436 2023-05-07 21:36:59.006708 vocalpy-0.2.0.post1/noxfile.py
--rw-r--r--   0        0        0     1453 2023-05-07 22:11:05.316861 vocalpy-0.2.0.post1/pyproject.toml
--rw-r--r--   0        0        0    19133 2023-04-25 13:43:12.342347 vocalpy-0.2.0.post1/src/scripts/attrs-sqlalchemy.ipynb
--rw-r--r--   0        0        0     5151 2023-04-25 13:43:12.360555 vocalpy-0.2.0.post1/src/scripts/carpentries-sql-practice.ipynb
--rw-r--r--   0        0        0    46531 2023-04-25 13:43:12.330739 vocalpy-0.2.0.post1/src/scripts/dataclass-orm.ipynb
--rw-r--r--   0        0        0    21715 2023-04-25 13:43:12.389389 vocalpy-0.2.0.post1/src/scripts/dataset.ipynb
--rw-r--r--   0        0        0     3130 2023-05-04 01:22:37.617838 vocalpy-0.2.0.post1/src/scripts/sqlite-python-tutorial.ipynb
--rw-r--r--   0        0        0    22868 2023-05-07 21:52:44.503972 vocalpy-0.2.0.post1/src/scripts/vocalpy-sqlalchemy-orm.ipynb
--rw-r--r--   0        0        0      810 2023-05-07 22:11:05.312790 vocalpy-0.2.0.post1/src/vocalpy/__about__.py
--rw-r--r--   0        0        0     1304 2023-05-07 21:44:06.314669 vocalpy-0.2.0.post1/src/vocalpy/__init__.py
--rw-r--r--   0        0        0       33 2023-04-25 13:42:56.065849 vocalpy-0.2.0.post1/src/vocalpy/annotation/__init__.py
--rw-r--r--   0        0        0     1895 2023-05-04 01:22:20.075891 vocalpy-0.2.0.post1/src/vocalpy/annotation_file.py
--rw-r--r--   0        0        0        0 2023-05-04 01:22:20.076056 vocalpy-0.2.0.post1/src/vocalpy/annotator.py
--rw-r--r--   0        0        0     7738 2023-05-07 21:44:41.309650 vocalpy-0.2.0.post1/src/vocalpy/audio.py
--rw-r--r--   0        0        0      635 2023-05-04 01:22:20.078518 vocalpy-0.2.0.post1/src/vocalpy/audio_file.py
--rw-r--r--   0        0        0       30 2023-04-25 13:42:56.066572 vocalpy-0.2.0.post1/src/vocalpy/constants.py
--rw-r--r--   0        0        0        0 2023-04-08 15:55:30.247903 vocalpy-0.2.0.post1/src/vocalpy/converters.py
--rw-r--r--   0        0        0     4879 2023-05-04 01:22:20.079083 vocalpy-0.2.0.post1/src/vocalpy/dataset.py
--rw-r--r--   0        0        0     2552 2023-05-07 21:02:40.315808 vocalpy-0.2.0.post1/src/vocalpy/dataset_file.py
--rw-r--r--   0        0        0        0 2023-05-04 01:22:20.079995 vocalpy-0.2.0.post1/src/vocalpy/feature_extractor.py
--rw-r--r--   0        0        0     1918 2023-05-04 01:22:20.080691 vocalpy-0.2.0.post1/src/vocalpy/feature_file.py
--rw-r--r--   0        0        0     1118 2023-04-25 13:42:56.072844 vocalpy-0.2.0.post1/src/vocalpy/paths.py
--rw-r--r--   0        0        0      146 2023-05-07 20:16:29.802759 vocalpy-0.2.0.post1/src/vocalpy/repository/__init__.py
--rw-r--r--   0        0        0      441 2023-05-07 20:16:29.803288 vocalpy-0.2.0.post1/src/vocalpy/repository/base.py
--rw-r--r--   0        0        0     3136 2023-05-04 01:22:20.081989 vocalpy-0.2.0.post1/src/vocalpy/repository/orm.py
--rw-r--r--   0        0        0      677 2023-05-07 20:16:29.803723 vocalpy-0.2.0.post1/src/vocalpy/repository/sqlalchemy.py
--rw-r--r--   0        0        0     3155 2023-05-07 21:44:06.438381 vocalpy-0.2.0.post1/src/vocalpy/segmenter.py
--rw-r--r--   0        0        0     2502 2023-05-07 21:44:06.401117 vocalpy-0.2.0.post1/src/vocalpy/sequence.py
--rw-r--r--   0        0        0      114 2023-05-04 01:22:20.084546 vocalpy-0.2.0.post1/src/vocalpy/signal/__init__.py
--rw-r--r--   0        0        0     2301 2023-05-07 21:45:30.491360 vocalpy-0.2.0.post1/src/vocalpy/signal/audio.py
--rw-r--r--   0        0        0     2244 2023-05-04 01:22:20.085058 vocalpy-0.2.0.post1/src/vocalpy/signal/preprocess.py
--rw-r--r--   0        0        0     3012 2023-05-07 21:45:41.887997 vocalpy-0.2.0.post1/src/vocalpy/signal/segment.py
--rw-r--r--   0        0        0     3062 2023-05-07 21:07:37.895584 vocalpy-0.2.0.post1/src/vocalpy/signal/spectrogram.py
--rw-r--r--   0        0        0     7437 2023-05-04 01:22:20.086913 vocalpy-0.2.0.post1/src/vocalpy/spectrogram.py
--rw-r--r--   0        0        0     1491 2023-05-04 01:22:20.087395 vocalpy-0.2.0.post1/src/vocalpy/spectrogram_file.py
--rw-r--r--   0        0        0     8358 2023-05-07 21:44:06.512977 vocalpy-0.2.0.post1/src/vocalpy/spectrogram_maker.py
--rw-r--r--   0        0        0      508 2023-05-04 01:22:20.088654 vocalpy-0.2.0.post1/src/vocalpy/spectrogram_parameters.py
--rw-r--r--   0        0        0     1565 2023-05-07 21:44:06.416113 vocalpy-0.2.0.post1/src/vocalpy/unit.py
--rw-r--r--   0        0        0      738 2023-04-25 13:42:56.074584 vocalpy-0.2.0.post1/src/vocalpy/validators.py
--rw-r--r--   0        0        0        0 2023-04-08 15:55:30.249971 vocalpy-0.2.0.post1/tests/__init__.py
--rw-r--r--   0        0        0       24 2023-04-08 15:55:30.250132 vocalpy-0.2.0.post1/tests/conftest.py
--rw-r--r--   0        0        0      112 2023-04-25 13:42:56.075165 vocalpy-0.2.0.post1/tests/fixtures/__init__.py
--rw-r--r--   0        0        0     2744 2023-04-25 13:42:56.075834 vocalpy-0.2.0.post1/tests/fixtures/annot.py
--rw-r--r--   0        0        0     4620 2023-04-25 13:42:56.076380 vocalpy-0.2.0.post1/tests/fixtures/audio.py
--rw-r--r--   0        0        0      834 2023-04-25 13:42:56.076724 vocalpy-0.2.0.post1/tests/fixtures/datasets.py
--rw-r--r--   0        0        0     6669 2023-05-04 01:22:20.090376 vocalpy-0.2.0.post1/tests/fixtures/spect.py
--rw-r--r--   0        0        0     1032 2023-04-25 13:42:56.077753 vocalpy-0.2.0.post1/tests/fixtures/test_data.py
--rw-r--r--   0        0        0     2248 2023-04-25 13:42:56.078328 vocalpy-0.2.0.post1/tests/scripts/generate_data_for_tests.py
--rw-r--r--   0        0        0     2695 2023-05-04 01:22:20.090889 vocalpy-0.2.0.post1/tests/test_annotation_file.py
--rw-r--r--   0        0        0     8793 2023-05-07 21:46:44.905812 vocalpy-0.2.0.post1/tests/test_audio.py
--rw-r--r--   0        0        0      992 2023-05-04 01:22:20.091867 vocalpy-0.2.0.post1/tests/test_audio_file.py
--rw-r--r--   0        0        0     1605 2023-05-04 01:22:20.092370 vocalpy-0.2.0.post1/tests/test_dataset.py
--rw-r--r--   0        0        0     2819 2023-05-07 21:46:44.715868 vocalpy-0.2.0.post1/tests/test_paths.py
--rw-r--r--   0        0        0        0 2023-05-04 01:22:20.093556 vocalpy-0.2.0.post1/tests/test_repository/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 01:22:20.093841 vocalpy-0.2.0.post1/tests/test_repository/test_repository.py
--rw-r--r--   0        0        0     2258 2023-05-07 21:46:44.720020 vocalpy-0.2.0.post1/tests/test_segmenter.py
--rw-r--r--   0        0        0      547 2023-05-07 21:46:44.670223 vocalpy-0.2.0.post1/tests/test_sequence.py
--rw-r--r--   0        0        0        0 2023-04-08 15:55:30.252298 vocalpy-0.2.0.post1/tests/test_signal/__init__.py
--rw-r--r--   0        0        0      314 2023-05-07 20:16:29.809278 vocalpy-0.2.0.post1/tests/test_signal/test_audio.py
--rw-r--r--   0        0        0      629 2023-05-07 20:16:29.809675 vocalpy-0.2.0.post1/tests/test_signal/test_segment.py
--rw-r--r--   0        0        0        0 2023-04-08 15:55:30.252385 vocalpy-0.2.0.post1/tests/test_signal/test_spectrogram.py
--rw-r--r--   0        0        0     4186 2023-05-04 01:22:20.095358 vocalpy-0.2.0.post1/tests/test_spectrogram.py
--rw-r--r--   0        0        0     1500 2023-05-04 01:22:20.095856 vocalpy-0.2.0.post1/tests/test_spectrogram_file.py
--rw-r--r--   0        0        0     4476 2023-05-07 21:09:06.876025 vocalpy-0.2.0.post1/tests/test_spectrogram_maker.py
--rw-r--r--   0        0        0      848 2023-05-07 21:46:44.691384 vocalpy-0.2.0.post1/tests/test_unit.py
--rw-r--r--   0        0        0     5055 1970-01-01 00:00:00.000000 vocalpy-0.2.0.post1/PKG-INFO
+-rw-r--r--   0        0        0     1307 2023-05-07 21:41:12.898528 vocalpy-0.3.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      248 2023-05-07 21:39:43.229568 vocalpy-0.3.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      615 2023-05-07 21:39:43.228362 vocalpy-0.3.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      832 2023-05-11 16:02:58.480074 vocalpy-0.3.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      286 2023-04-25 13:42:56.058591 vocalpy-0.3.0/.gitignore
+-rw-r--r--   0        0        0      769 2023-04-25 13:42:56.059258 vocalpy-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      368 2023-05-11 16:02:58.480875 vocalpy-0.3.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     5556 2023-05-07 20:52:52.998672 vocalpy-0.3.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1867 2023-05-07 20:53:11.404957 vocalpy-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1540 2023-04-08 15:55:30.246016 vocalpy-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2064 2023-04-08 15:55:30.246197 vocalpy-0.3.0/Makefile
+-rw-r--r--   0        0        0    12899 2023-05-11 16:02:58.481702 vocalpy-0.3.0/README.md
+-rw-r--r--   0        0        0      251 2023-05-07 20:48:44.343584 vocalpy-0.3.0/docs/CHANGELOG.md
+-rw-r--r--   0        0        0      634 2023-05-11 16:02:58.482218 vocalpy-0.3.0/docs/Makefile
+-rw-r--r--   0        0        0    29965 2023-05-07 20:41:50.515176 vocalpy-0.3.0/docs/_static/vocalpy-logomark.png
+-rw-r--r--   0        0        0   285798 2023-05-07 20:41:50.763203 vocalpy-0.3.0/docs/_static/vocalpy-primary.png
+-rw-r--r--   0        0        0   194159 2023-05-07 20:41:50.588788 vocalpy-0.3.0/docs/_static/vocalpy-secondary.png
+-rw-r--r--   0        0        0     2804 2023-05-11 16:02:58.482702 vocalpy-0.3.0/docs/conf.py
+-rw-r--r--   0        0        0    11760 2023-05-11 16:02:58.483277 vocalpy-0.3.0/docs/index.md
+-rw-r--r--   0        0        0      800 2023-05-11 16:02:58.483745 vocalpy-0.3.0/docs/make.bat
+-rw-r--r--   0        0        0      881 2023-05-11 16:02:58.484382 vocalpy-0.3.0/docs/nitpick-ignore.txt
+-rw-r--r--   0        0        0      631 2023-05-11 16:02:58.485051 vocalpy-0.3.0/docs/reference/about.md
+-rw-r--r--   0        0        0       92 2023-05-11 16:02:58.485475 vocalpy-0.3.0/docs/reference/index.md
+-rw-r--r--   0        0        0     7342 2023-05-11 16:02:58.486449 vocalpy-0.3.0/noxfile.py
+-rw-r--r--   0        0        0     1768 2023-05-11 16:02:58.487203 vocalpy-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    19133 2023-04-25 13:43:12.342347 vocalpy-0.3.0/src/scripts/attrs-sqlalchemy.ipynb
+-rw-r--r--   0        0        0     5151 2023-04-25 13:43:12.360555 vocalpy-0.3.0/src/scripts/carpentries-sql-practice.ipynb
+-rw-r--r--   0        0        0    46531 2023-04-25 13:43:12.330739 vocalpy-0.3.0/src/scripts/dataclass-orm.ipynb
+-rw-r--r--   0        0        0    21715 2023-04-25 13:43:12.389389 vocalpy-0.3.0/src/scripts/dataset.ipynb
+-rw-r--r--   0        0        0     3130 2023-05-04 01:22:37.617838 vocalpy-0.3.0/src/scripts/sqlite-python-tutorial.ipynb
+-rw-r--r--   0        0        0    22868 2023-05-11 16:03:09.046030 vocalpy-0.3.0/src/scripts/vocalpy-sqlalchemy-orm.ipynb
+-rw-r--r--   0        0        0      804 2023-05-11 16:02:58.488926 vocalpy-0.3.0/src/vocalpy/__about__.py
+-rw-r--r--   0        0        0     1331 2023-05-11 16:02:58.489904 vocalpy-0.3.0/src/vocalpy/__init__.py
+-rw-r--r--   0        0        0     1092 2023-05-11 16:02:58.490571 vocalpy-0.3.0/src/vocalpy/annotation.py
+-rw-r--r--   0        0        0     1895 2023-05-04 01:22:20.075891 vocalpy-0.3.0/src/vocalpy/annotation_file.py
+-rw-r--r--   0        0        0        0 2023-05-04 01:22:20.076056 vocalpy-0.3.0/src/vocalpy/annotator.py
+-rw-r--r--   0        0        0     7747 2023-05-11 16:02:58.491514 vocalpy-0.3.0/src/vocalpy/audio.py
+-rw-r--r--   0        0        0      635 2023-05-04 01:22:20.078518 vocalpy-0.3.0/src/vocalpy/audio_file.py
+-rw-r--r--   0        0        0       30 2023-04-25 13:42:56.066572 vocalpy-0.3.0/src/vocalpy/constants.py
+-rw-r--r--   0        0        0        0 2023-04-08 15:55:30.247903 vocalpy-0.3.0/src/vocalpy/converters.py
+-rw-r--r--   0        0        0      137 2023-05-11 16:02:58.492731 vocalpy-0.3.0/src/vocalpy/dataset/__init__.py
+-rw-r--r--   0        0        0       54 2023-05-11 16:02:58.493366 vocalpy-0.3.0/src/vocalpy/dataset/schema/__init__.py
+-rw-r--r--   0        0        0     3136 2023-05-11 16:02:58.493703 vocalpy-0.3.0/src/vocalpy/dataset/schema/orm.py
+-rw-r--r--   0        0        0     2085 2023-05-11 16:02:58.495449 vocalpy-0.3.0/src/vocalpy/dataset/schema/sequence.py
+-rw-r--r--   0        0        0     8833 2023-05-11 16:02:58.496679 vocalpy-0.3.0/src/vocalpy/dataset/sequence.py
+-rw-r--r--   0        0        0     2581 2023-05-11 16:02:58.497633 vocalpy-0.3.0/src/vocalpy/dataset_file.py
+-rw-r--r--   0        0        0        0 2023-05-04 01:22:20.079995 vocalpy-0.3.0/src/vocalpy/feature_extractor.py
+-rw-r--r--   0        0        0     1918 2023-05-04 01:22:20.080691 vocalpy-0.3.0/src/vocalpy/feature_file.py
+-rw-r--r--   0        0        0     1118 2023-04-25 13:42:56.072844 vocalpy-0.3.0/src/vocalpy/paths.py
+-rw-r--r--   0        0        0      165 2023-05-11 16:02:58.498226 vocalpy-0.3.0/src/vocalpy/plot/__init__.py
+-rw-r--r--   0        0        0     7243 2023-05-11 16:02:58.499083 vocalpy-0.3.0/src/vocalpy/plot/annot.py
+-rw-r--r--   0        0        0     4698 2023-05-11 16:02:58.499578 vocalpy-0.3.0/src/vocalpy/plot/spect.py
+-rw-r--r--   0        0        0     3263 2023-05-11 16:02:58.500435 vocalpy-0.3.0/src/vocalpy/segmenter.py
+-rw-r--r--   0        0        0     2461 2023-05-11 16:02:58.501062 vocalpy-0.3.0/src/vocalpy/sequence.py
+-rw-r--r--   0        0        0      114 2023-05-04 01:22:20.084546 vocalpy-0.3.0/src/vocalpy/signal/__init__.py
+-rw-r--r--   0        0        0     2301 2023-05-07 21:45:30.491360 vocalpy-0.3.0/src/vocalpy/signal/audio.py
+-rw-r--r--   0        0        0     2201 2023-05-11 16:02:58.501656 vocalpy-0.3.0/src/vocalpy/signal/preprocess.py
+-rw-r--r--   0        0        0     3012 2023-05-07 21:45:41.887997 vocalpy-0.3.0/src/vocalpy/signal/segment.py
+-rw-r--r--   0        0        0     3055 2023-05-11 16:02:58.502442 vocalpy-0.3.0/src/vocalpy/signal/spectrogram.py
+-rw-r--r--   0        0        0     7459 2023-05-11 16:02:58.503198 vocalpy-0.3.0/src/vocalpy/spectrogram.py
+-rw-r--r--   0        0        0     1491 2023-05-04 01:22:20.087395 vocalpy-0.3.0/src/vocalpy/spectrogram_file.py
+-rw-r--r--   0        0        0     8351 2023-05-11 16:02:58.504211 vocalpy-0.3.0/src/vocalpy/spectrogram_maker.py
+-rw-r--r--   0        0        0      508 2023-05-04 01:22:20.088654 vocalpy-0.3.0/src/vocalpy/spectrogram_parameters.py
+-rw-r--r--   0        0        0     1565 2023-05-07 21:44:06.416113 vocalpy-0.3.0/src/vocalpy/unit.py
+-rw-r--r--   0        0        0      738 2023-04-25 13:42:56.074584 vocalpy-0.3.0/src/vocalpy/validators.py
+-rw-r--r--   0        0        0        0 2023-04-08 15:55:30.249971 vocalpy-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0       24 2023-04-08 15:55:30.250132 vocalpy-0.3.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-05-11 16:02:58.504631 vocalpy-0.3.0/tests/data-for-tests/generated/.gitkeep
+-rw-r--r--   0        0        0        0 2023-05-11 16:02:58.505087 vocalpy-0.3.0/tests/data-for-tests/source/.gitkeep
+-rw-r--r--   0        0        0      112 2023-04-25 13:42:56.075165 vocalpy-0.3.0/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0     2744 2023-04-25 13:42:56.075834 vocalpy-0.3.0/tests/fixtures/annot.py
+-rw-r--r--   0        0        0     4620 2023-04-25 13:42:56.076380 vocalpy-0.3.0/tests/fixtures/audio.py
+-rw-r--r--   0        0        0      834 2023-04-25 13:42:56.076724 vocalpy-0.3.0/tests/fixtures/datasets.py
+-rw-r--r--   0        0        0     6669 2023-05-04 01:22:20.090376 vocalpy-0.3.0/tests/fixtures/spect.py
+-rw-r--r--   0        0        0     1032 2023-04-25 13:42:56.077753 vocalpy-0.3.0/tests/fixtures/test_data.py
+-rw-r--r--   0        0        0     2248 2023-04-25 13:42:56.078328 vocalpy-0.3.0/tests/scripts/generate_data_for_tests.py
+-rw-r--r--   0        0        0     2695 2023-05-04 01:22:20.090889 vocalpy-0.3.0/tests/test_annotation_file.py
+-rw-r--r--   0        0        0     8793 2023-05-07 21:46:44.905812 vocalpy-0.3.0/tests/test_audio.py
+-rw-r--r--   0        0        0      992 2023-05-04 01:22:20.091867 vocalpy-0.3.0/tests/test_audio_file.py
+-rw-r--r--   0        0        0        0 2023-05-11 16:02:58.505296 vocalpy-0.3.0/tests/test_dataset/__init__.py
+-rw-r--r--   0        0        0     1003 2023-05-11 16:02:58.505928 vocalpy-0.3.0/tests/test_dataset/test_sequence.py
+-rw-r--r--   0        0        0     2819 2023-05-07 21:46:44.715868 vocalpy-0.3.0/tests/test_paths.py
+-rw-r--r--   0        0        0     2258 2023-05-07 21:46:44.720020 vocalpy-0.3.0/tests/test_segmenter.py
+-rw-r--r--   0        0        0      547 2023-05-07 21:46:44.670223 vocalpy-0.3.0/tests/test_sequence.py
+-rw-r--r--   0        0        0        0 2023-04-08 15:55:30.252298 vocalpy-0.3.0/tests/test_signal/__init__.py
+-rw-r--r--   0        0        0      314 2023-05-07 20:16:29.809278 vocalpy-0.3.0/tests/test_signal/test_audio.py
+-rw-r--r--   0        0        0      629 2023-05-07 20:16:29.809675 vocalpy-0.3.0/tests/test_signal/test_segment.py
+-rw-r--r--   0        0        0        0 2023-04-08 15:55:30.252385 vocalpy-0.3.0/tests/test_signal/test_spectrogram.py
+-rw-r--r--   0        0        0     4186 2023-05-04 01:22:20.095358 vocalpy-0.3.0/tests/test_spectrogram.py
+-rw-r--r--   0        0        0     1500 2023-05-04 01:22:20.095856 vocalpy-0.3.0/tests/test_spectrogram_file.py
+-rw-r--r--   0        0        0     4476 2023-05-07 21:09:06.876025 vocalpy-0.3.0/tests/test_spectrogram_maker.py
+-rw-r--r--   0        0        0      848 2023-05-07 21:46:44.691384 vocalpy-0.3.0/tests/test_unit.py
+-rw-r--r--   0        0        0    15084 1970-01-01 00:00:00.000000 vocalpy-0.3.0/PKG-INFO
```

### Comparing `vocalpy-0.2.0.post1/.github/ISSUE_TEMPLATE/bug_report.md` & `vocalpy-0.3.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0.post1/.github/ISSUE_TEMPLATE/feature_request.md` & `vocalpy-0.3.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0.post1/.github/workflows/ci.yml` & `vocalpy-0.3.0/.github/workflows/ci.yml`

 * *Files 16% similar despite different names*

```diff
@@ -21,10 +21,12 @@
       - name: install libsndfile1 on ubuntu
         if: matrix.os == 'ubuntu-latest'
         run: sudo apt install libsndfile1
       - name: run tests
         run: |
           pip install nox
           pip install '.[test]'
-          nox --session coverage
+          nox -s test-data-download-source
+          nox -s test-data-download-generated
+          nox -s coverage
       - name: upload coverage to Codecov
         uses: codecov/codecov-action@v3
```

### Comparing `vocalpy-0.2.0.post1/.pre-commit-config.yaml` & `vocalpy-0.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0.post1/CODE_OF_CONDUCT.md` & `vocalpy-0.3.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0.post1/CONTRIBUTING.md` & `vocalpy-0.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0.post1/LICENSE` & `vocalpy-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0.post1/Makefile` & `vocalpy-0.3.0/Makefile`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0.post1/docs/_static/vocalpy-logomark.png` & `vocalpy-0.3.0/docs/_static/vocalpy-logomark.png`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0.post1/docs/_static/vocalpy-primary.png` & `vocalpy-0.3.0/docs/_static/vocalpy-primary.png`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0.post1/docs/_static/vocalpy-secondary.png` & `vocalpy-0.3.0/docs/_static/vocalpy-secondary.png`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0.post1/noxfile.py` & `vocalpy-0.3.0/noxfile.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 import os
 import pathlib
 import shutil
 import sys
 import tarfile
-import urllib
+import urllib.request
 
 import nox
 
-# ---- keep this at top of noxfile
-nox.options.sessions = ["lint", "tests"]
-
 
 # ---- this constant is used by more than one session: dev, download-test-data
 DIR = pathlib.Path(__file__).parent.resolve()
 
 VENV_DIR = pathlib.Path('./.venv').resolve()
 
 
@@ -89,17 +86,15 @@
         session.run("sphinx-build", "-nW", "--keep-going", "-b", "html", "doc/", "doc/_build/html")
 
 
 @nox.session
 def coverage(session: nox.Session) -> None:
     """Run tests and measure coverage"""
     session.run(
-        "pytest",
-        "--cov=./",
-        "--cov-report=xml",
+        "pytest", "-n", "auto", "--cov=./", "--cov-report=xml", *session.posargs
     )
 
 
 @nox.session
 def build(session: nox.Session) -> None:
     """
     Build an SDist and wheel with ``flit``.
@@ -152,16 +147,21 @@
 
 
 def copy_url(url: str, path: str) -> None:
     """Copy data from a url to a local file."""
     urllib.request.urlretrieve(url, path)
 
 
-# TODO: fix this url! don't use vak data!!!
-SOURCE_TEST_DATA_URL = "https://osf.io/hbg4k/download"
+def make_tarfile(name: str, to_add: list):
+    with tarfile.open(name, "w:gz") as tf:
+        for add_name in to_add:
+            tf.add(name=add_name)
+
+
+SOURCE_TEST_DATA_URL = "https://osf.io/xq6hf/download"
 SOURCE_TEST_DATA_TAR = SOURCE_TEST_DATA_DIR / "source-test-data.tar.gz"
 
 
 @nox.session(name='test-data-tar-source')
 def test_data_tar_source(session) -> None:
     """
     Make a .tar.gz file of just the 'generated' test data used to run tests on CI.
@@ -183,36 +183,60 @@
     session.log(f'Downloading: {SOURCE_TEST_DATA_URL}')
     copy_url(url=SOURCE_TEST_DATA_URL, path=SOURCE_TEST_DATA_TAR)
     session.log(f'Extracting downloaded tar: {SOURCE_TEST_DATA_TAR}')
     with tarfile.open(SOURCE_TEST_DATA_TAR, "r:gz") as tf:
         tf.extractall(path='.')
 
 
+
 TEST_DATA_GENERATE_SCRIPT = './tests/scripts/generate_data_for_tests.py'
 
 
 @nox.session(name='test-data-generate', python="3.10")
 def test_data_generate(session) -> None:
     """
     Produced 'generated' test data, by running TEST_DATA_GENERATE_SCRIPT on 'source' test data.
     """
     session.install(".[test]")
     session.run("python", TEST_DATA_GENERATE_SCRIPT)
 
 
 # TODO: fix this url!
 GENERATED_TEST_DATA_DIR = DATA_FOR_TESTS_DIR / "generated"
+GENERATED_TEST_DATA_SUBDIRS = [
+    dir_ for dir_
+    in sorted(pathlib.Path(GENERATED_TEST_DATA_DIR).glob('*/'))
+    if dir_.is_dir()
+]
 GENERATED_TEST_DATA_TAR = GENERATED_TEST_DATA_DIR / 'generated_test_data.tar.gz'
 
 
 @nox.session(name='test-data-clean-generated')
 def test_data_clean_generated(session) -> None:
     """
     Clean (remove) 'generated' test data.
     """
     clean_dir(GENERATED_TEST_DATA_DIR)
 
 
-def make_tarfile(name: str, to_add: list):
-    with tarfile.open(name, "w:gz") as tf:
-        for add_name in to_add:
-            tf.add(name=add_name)
+@nox.session(name='test-data-tar-generated')
+def test_data_tar_generated(session) -> None:
+    """
+    Make a .tar.gz file of all 'generated' test data.
+    """
+    session.log(f"Making tarfile with all generated data: {GENERATED_TEST_DATA_TAR}")
+    make_tarfile(GENERATED_TEST_DATA_TAR, GENERATED_TEST_DATA_SUBDIRS)
+
+
+GENERATED_TEST_DATA_URL = 'https://osf.io/3fzye/download'
+
+
+@nox.session(name='test-data-download-generated')
+def test_data_download_generated(session) -> None:
+    """
+    Download and extract a .tar.gz file of all 'generated' test data
+    """
+    session.log(f'Downloading: {GENERATED_TEST_DATA_URL}')
+    copy_url(url=GENERATED_TEST_DATA_URL, path=GENERATED_TEST_DATA_TAR)
+    session.log(f'Extracting downloaded tar: {GENERATED_TEST_DATA_TAR}')
+    with tarfile.open(GENERATED_TEST_DATA_TAR, "r:gz") as tf:
+        tf.extractall(path='.')
```

### Comparing `vocalpy-0.2.0.post1/pyproject.toml` & `vocalpy-0.3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -3,57 +3,66 @@
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "vocalpy"
 authors = [
     {name = "David Nicholson", email = "nickledave@users.noreply.github.com"}
 ]
-description = "Core package for acoustic communication in Python"
-version = "0.2.0.post1"
+description = "A core package for acoustic communication research in Python"
+version = "0.3.0"
 classifiers = [
         'License :: OSI Approved :: BSD License',
         'Development Status :: 5 - Production/Stable',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython'
 ]
 requires-python = ">=3.9"
 readme = "README.md"
 license = {file = "LICENSE"}
 dependencies = [
     "attrs >=23.1.0",
     "crowsetta >=5.0.0",
     "dask >=2.10.1",
     "evfuncs >= 0.3.3",
     "librosa >= 0.10.0.post2",
+    "matplotlib >=3.7.1",
     "numpy >=1.21.0",
     "pandas >= 1.3.5",
     "scipy >=1.7.0",
     "SoundFile >=0.12.1",
     "SQLAlchemy >=2.0.12",
 ]
 
 [project.urls]
-Home = "https://github.com/NickleDave/vocalpy"
+Home = "https://github.com/vocalpy/vocalpy"
+Docs = "https://vocalpy.readthedocs.io"
 
 [project.optional-dependencies]
-dev = [
-    "twine >=3.7.1",
-    "black >=21.12b0",
-    "ipython >=8.0.0",
-    "nox >= 2022.1.7",
-    "vocalpy[doc, test]"
-]
 test = [
     "pytest >=6.2.5",
     "pytest-cov >=2.11.1",
     "pytest-xdist >=3.2.0",
 ]
 doc = [
     "ipython != 8.7.0",
     "jupyterlab >=3.0.3",
     "jupytext >=1.13.8",
     "myst-nb >=0.15.0",
-    "sphinx >=4.4.0"
+    "Sphinx >=3.4.3",
+    "sphinx-autobuild >= 2021.3.14",
+    "sphinx-book-theme >=0.3.2",
+    "sphinx-copybutton >=0.4.0",
+    "sphinx-design >=0.2.0",
+    "sphinxext-opengraph  >=0.5.1",
+    "sphinx-tabs >= 3.3.1",
+]
+dev = [
+    "twine >=3.7.1",
+    "black >=21.12b0",
+    "ipython >=8.0.0",
+    "nox >= 2022.1.7",
+    "vocalpy[doc, test]"
 ]
```

### Comparing `vocalpy-0.2.0.post1/src/scripts/attrs-sqlalchemy.ipynb` & `vocalpy-0.3.0/src/scripts/attrs-sqlalchemy.ipynb`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0.post1/src/scripts/carpentries-sql-practice.ipynb` & `vocalpy-0.3.0/src/scripts/carpentries-sql-practice.ipynb`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0.post1/src/scripts/dataclass-orm.ipynb` & `vocalpy-0.3.0/src/scripts/dataclass-orm.ipynb`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0.post1/src/scripts/dataset.ipynb` & `vocalpy-0.3.0/src/scripts/dataset.ipynb`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0.post1/src/scripts/sqlite-python-tutorial.ipynb` & `vocalpy-0.3.0/src/scripts/sqlite-python-tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0.post1/src/scripts/vocalpy-sqlalchemy-orm.ipynb` & `vocalpy-0.3.0/src/scripts/vocalpy-sqlalchemy-orm.ipynb`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0.post1/src/vocalpy/__about__.py` & `vocalpy-0.3.0/src/vocalpy/__about__.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     base_dir = None
 
 
 __title__ = "vocalpy"
 __summary__ = "A core package for acoustic communication research in Python"
 __uri__ = "https://github.com/vocalpy/vocalpy"
 
-__version__ = "0.2.0.post1"
+__version__ = "0.3.0"
 
 if base_dir is not None and os.path.exists(os.path.join(base_dir, ".commit")):
     with open(os.path.join(base_dir, ".commit")) as fp:
         __commit__ = fp.read().strip()
 else:
     __commit__ = None
```

### Comparing `vocalpy-0.2.0.post1/src/vocalpy/__init__.py` & `vocalpy-0.3.0/src/vocalpy/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from . import constants, dataset, paths, signal, validators
+from . import constants, dataset, paths, plot, signal, validators
 from .__about__ import (
     __author__,
     __commit__,
     __copyright__,
     __email__,
     __license__,
     __summary__,
     __title__,
     __uri__,
     __version__,
 )
+from .annotation import Annotation
 from .annotation_file import AnnotationFile
 from .audio import Audio
 from .audio_file import AudioFile
-from .dataset import Dataset
 from .dataset_file import DatasetFile, DatasetFileType, DatasetFileTypeEnum
 from .feature_file import FeatureFile
 from .segmenter import Segmenter
 from .sequence import Sequence
 from .spectrogram import Spectrogram
 from .spectrogram_file import SpectrogramFile
 from .spectrogram_maker import SpectrogramMaker
@@ -30,25 +30,26 @@
     "__copyright__",
     "__email__",
     "__license__",
     "__summary__",
     "__title__",
     "__uri__",
     "__version__",
+    "Annotation",
     "AnnotationFile",
     "Audio",
     "AudioFile",
     "constants",
     "dataset",
-    "Dataset",
     "DatasetFile",
     "DatasetFileType",
     "DatasetFileTypeEnum",
     "FeatureFile",
     "paths",
+    "plot",
     "Segmenter",
     "Sequence",
     "signal",
     "Spectrogram",
     "SpectrogramFile",
     "SpectrogramMaker",
     "SpectrogramParameters",
```

### Comparing `vocalpy-0.2.0.post1/src/vocalpy/annotation_file.py` & `vocalpy-0.3.0/src/vocalpy/annotation_file.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0.post1/src/vocalpy/audio.py` & `vocalpy-0.3.0/src/vocalpy/audio.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,19 +145,19 @@
     def channels(self):
         if self._channels is None:
             self._read()
         return self._channels
 
     def __repr__(self):
         return (
-            f"{self.__class__.__name__}("
+            f"vocalpy.{self.__class__.__name__}("
             f"data={reprlib.repr(self._data)}, "
             f"samplerate={reprlib.repr(self._samplerate)}, "
             f"channels={self._channels}), "
-            f"path={self.path}"
+            f"path={self.path})"
         )
 
     def asdict(self):
         """Convert this :class:`vocalpy.Audio`
         to a :class:`dict`.
 
         Returns
```

### Comparing `vocalpy-0.2.0.post1/src/vocalpy/audio_file.py` & `vocalpy-0.3.0/src/vocalpy/audio_file.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0.post1/src/vocalpy/dataset_file.py` & `vocalpy-0.3.0/src/vocalpy/dataset_file.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 The list created by :class:`vocalpy.dataset.Dataset`
 becomes the central table in a relational database
 representing the dataset.
 """
 from __future__ import annotations
 
 import enum
+from typing import Union
 
 import attrs
 
 from .annotation_file import AnnotationFile
 from .audio_file import AudioFile
 from .feature_file import FeatureFile
 from .spectrogram_file import SpectrogramFile
@@ -32,15 +33,15 @@
 class DatasetFileTypeEnum(enum.Enum):
     ANNOTATION = AnnotationFile
     AUDIO = AudioFile
     FEATURE = FeatureFile
     SPECTROGRAM = SpectrogramFile
 
 
-DatasetFileType = AnnotationFile | AudioFile | FeatureFile | SpectrogramFile
+DatasetFileType = Union[AnnotationFile, AudioFile, FeatureFile, SpectrogramFile]
 
 
 @attrs.define
 class DatasetFile:
     """A class that represents any file in a dataset.
     Used when building a :class:`vocalpy.Dataset`.
```

### Comparing `vocalpy-0.2.0.post1/src/vocalpy/feature_file.py` & `vocalpy-0.3.0/src/vocalpy/feature_file.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0.post1/src/vocalpy/paths.py` & `vocalpy-0.3.0/src/vocalpy/paths.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0.post1/src/vocalpy/repository/orm.py` & `vocalpy-0.3.0/src/vocalpy/dataset/schema/orm.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0.post1/src/vocalpy/segmenter.py` & `vocalpy-0.3.0/src/vocalpy/segmenter.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "min_silent_dur": 0.002,
 }
 
 
 class Segmenter:
     def __init__(self, callback: Callable | None = None, method: str | None = None, segment_params: dict | None = None):
         if callback and method:
-            raise ValueError(f"Cannot specify both `callback` and `method`, only one or the other.")
+            raise ValueError("Cannot specify both `callback` and `method`, only one or the other.")
 
         if method:
             import vocalpy.signal.segment
 
             # TODO: fix this
             try:
                 callback = getattr(vocalpy.signal.segment, method)
@@ -50,24 +50,28 @@
         if not isinstance(segment_params, dict):
             raise TypeError(f"`segment_params` should be a `dict` but type was: {type(segment_params)}")
 
         self.segment_params = segment_params
 
     def segment(
         self,
-        audio: Audio | AudioFile | Sequence[Audio | AudioFile],
+        audio: Audio | AudioFile | list[Audio | AudioFile],
         parallelize: bool = True,
-    ) -> Sequence | list[Sequence]:
+    ) -> Sequence | None | list[Sequence | None]:
         validate_audio(audio)
 
         # define nested function so vars are in scope and ``dask`` can call it
         def _to_sequence(audio_: Audio):
             if isinstance(audio_, AudioFile):
                 audio_ = Audio.read(audio_.path)
-            onsets, offsets = self.callback(audio_.data, audio_.samplerate, **self.segment_params)
+            out = self.callback(audio_.data, audio_.samplerate, **self.segment_params)
+            if out is None:
+                return out
+            else:
+                onsets, offsets = out
 
             units = []
             for onset, offset in zip(onsets, offsets):
                 units.append(Unit(onset=onset, offset=offset))
 
             return Sequence(
                 units=units,
```

### Comparing `vocalpy-0.2.0.post1/src/vocalpy/sequence.py` & `vocalpy-0.3.0/src/vocalpy/sequence.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,18 +55,15 @@
     )
 
     def __attrs_post_init__(self):
         units = sorted(self.units, key=lambda unit: unit.onset)
         onsets = [unit.onset for unit in units]
         if len(onsets) > 1:
             if not np.all(onsets[1:] > onsets[:-1]):
-                import pdb
-
-                pdb.set_trace()
-                raise ValueError(f"Onsets of units are not strictly increasing")
+                raise ValueError(f"Onsets of units are not strictly increasing.\nOnsets: {onsets}")
 
     @property
     def onset(self):
         return self.units[0].onset
 
     @property
     def offset(self):
```

### Comparing `vocalpy-0.2.0.post1/src/vocalpy/signal/audio.py` & `vocalpy-0.3.0/src/vocalpy/signal/audio.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0.post1/src/vocalpy/signal/preprocess.py` & `vocalpy-0.3.0/src/vocalpy/signal/preprocess.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,21 +23,20 @@
 
     Returns
     -------
     audio : vocalpy.Audio
         With pre-processing applied to the `data` attribute.
     """
     if freq_cutoffs[0] <= 0:
-        raise ValueError("Low frequency cutoff {} is invalid, " "must be greater than zero.".format(freq_cutoffs[0]))
+        raise ValueError(f"Low frequency cutoff {freq_cutoffs[0]} is invalid, " "must be greater than zero.")
 
     nyquist_rate = audio.samplerate / 2
     if freq_cutoffs[1] >= nyquist_rate:
         raise ValueError(
-            "High frequency cutoff {} is invalid, "
-            "must be less than Nyquist rate, {}.".format(freq_cutoffs[1], nyquist_rate)
+            f"High frequency cutoff {freq_cutoffs[1]} is invalid, " f"must be less than Nyquist rate, {nyquist_rate}."
         )
 
     data = audio.data
     if data.shape[-1] < 387:
         numtaps = 64
     elif data.shape[-1] < 771:
         numtaps = 128
@@ -54,8 +53,8 @@
     # whereas argument to matlab's fir1 is filter *order*
     # for linear FIR, filter length is filter order + 1
     b = scipy.signal.firwin(numtaps + 1, cutoffs, pass_zero=False)
     a = np.zeros((numtaps + 1,))
     a[0] = 1  # make an "all-zero filter"
     padlen = np.max((b.shape[-1] - 1, a.shape[-1] - 1))
     filtdata = scipy.signal.filtfilt(b, a, data, padlen=padlen)
-    return Audio(data=filtdata, samplerate=audio.samplerate, source_path=audio.source_path)
+    return Audio(data=filtdata, samplerate=audio.samplerate, path=audio.path)
```

### Comparing `vocalpy-0.2.0.post1/src/vocalpy/signal/segment.py` & `vocalpy-0.3.0/src/vocalpy/signal/segment.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0.post1/src/vocalpy/signal/spectrogram.py` & `vocalpy-0.3.0/src/vocalpy/signal/spectrogram.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,10 +85,10 @@
             s[s < thresh] = thresh  # set anything less than the threshold as the threshold
 
     if freq_cutoffs:
         f_inds = np.nonzero((f >= freq_cutoffs[0]) & (f < freq_cutoffs[1]))[0]  # returns tuple
         s = s[f_inds, :]
         f = f[f_inds]
 
-    spect = Spectrogram(data=s, frequencies=f, times=t, source_audio_path=audio.path)
+    spect = Spectrogram(data=s, frequencies=f, times=t, audio_path=audio.path)
 
     return spect
```

### Comparing `vocalpy-0.2.0.post1/src/vocalpy/spectrogram.py` & `vocalpy-0.3.0/src/vocalpy/spectrogram.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,18 +27,18 @@
         Must have at least 2 dimensions.
     frequencies : numpy.ndarray
         A vector of size :math:`f` where values are frequencies
         at center of frequency bins in spectrogram.
     times : numpy.ndarray
         Vector of size :math:`t` where values are times
         at center of time bins in spectrogram.
-    source_path : pathlib.Path, optional
+    path : pathlib.Path, optional
         Path to .npz file that spectrogram was loaded from.
         Optional, added automatically by the :meth:`~vocalpy.Spectrogram.read` method.
-    source_audio_path : pathlib.Path, optional
+    audio_path : pathlib.Path, optional
         Path to audio file from which spectrogram was generated.
         Optional, default None. Can be specified as argument
         to :meth:`~vocalpy.Spectrogram.read` method.
 
     Examples
     --------
     An example of creating a spectrogram with toy data,
@@ -71,20 +71,20 @@
                 f"Spectrogram array `data` should have at least 2 dimensions, "
                 f"but number of dimensions was {value.ndim}."
             )
 
     frequencies: npt.NDArray = attrs.field(validator=validators.is_1d_ndarray)
     times: npt.NDArray = attrs.field(validator=validators.is_1d_ndarray)
 
-    source_path: pathlib.Path = attrs.field(
+    path: pathlib.Path = attrs.field(
         converter=attrs.converters.optional(pathlib.Path),
         validator=attrs.validators.optional(attrs.validators.instance_of(pathlib.Path)),
         default=None,
     )
-    source_audio_path: pathlib.Path = attrs.field(
+    audio_path: pathlib.Path = attrs.field(
         converter=attrs.converters.optional(pathlib.Path),
         validator=attrs.validators.optional(attrs.validators.instance_of(pathlib.Path)),
         default=None,
     )
 
     def __attrs_post_init__(self):
         if not self.data.shape[0] == self.frequencies.shape[0]:
@@ -99,18 +99,20 @@
                 "Number of columns in spectrogram `data` should match number of elements in "
                 f"`times` vector, but `data` has {self.data.shape[1]} columns and there are "
                 f"{self.times.shape[0]} elements in `times`."
             )
 
     def __repr__(self):
         return (
-            f"{self.__class__.__name__}("
+            f"vocalpy.{self.__class__.__name__}("
             f"data={reprlib.repr(self.data)}, "
             f"frequencies={reprlib.repr(self.frequencies)}, "
-            f"times={reprlib.repr(self.times)})"
+            f"times={reprlib.repr(self.times)}, "
+            f"path={self.path!r}, "
+            f"audio_path={self.audio_path!r})"
         )
 
     def asdict(self):
         """Convert this :class:`vocalpy.Spectrogram`
         to a :class:`dict`.
 
         Returns
@@ -134,15 +136,15 @@
 
     def __ne__(self, other):
         if other.__class__ is not self.__class__:
             return NotImplemented
         return not self.__eq__(other)
 
     @classmethod
-    def read(cls, path: str | pathlib.Path, source_audio_path: str | pathlib.Path | None = None):
+    def read(cls, path: str | pathlib.Path, audio_path: str | pathlib.Path | None = None):
         """Read spectrogram and associated arrays from a Numpy npz file
         at the given ``path``.
 
         Parameters
         ----------
         path : str, pathlib.Path
             The path to the file containing the spectrogram ``s``
@@ -169,15 +171,15 @@
         kwargs = {}
         for key in ("data", "frequencies", "times"):
             try:
                 kwargs[key] = np.array(spect_file_dict[key])
             except KeyError as e:
                 raise KeyError(f"Did not find key '{key}' in path: {path}") from e
 
-        return cls(source_path=path, source_audio_path=source_audio_path, **kwargs)
+        return cls(path=path, audio_path=audio_path, **kwargs)
 
     def write(self, path: [str, pathlib.Path]):
         """Write this :class:`vocalpy.Spectrogram`
         to a Numpy .npz file at the given ``path``.
 
         Parameters
         ----------
@@ -185,12 +187,12 @@
             The path to where the path should be saved
             containing the spectrogram ``data``
             and associated arrays ``frequencies`` and ``times``.
         """
         # TODO: deal with extension here
         path = pathlib.Path(path)
         np.savez(path, data=self.data, frequencies=self.frequencies, times=self.times)
-        if self.source_audio_path:
-            source_audio_file = AudioFile(path=self.source_audio_path)
+        if self.audio_path:
+            source_audio_file = AudioFile(path=self.audio_path)
         else:
             source_audio_file = None
         return SpectrogramFile(path=path, source_audio_file=source_audio_file)
```

### Comparing `vocalpy-0.2.0.post1/src/vocalpy/spectrogram_file.py` & `vocalpy-0.3.0/src/vocalpy/spectrogram_file.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0.post1/src/vocalpy/spectrogram_maker.py` & `vocalpy-0.3.0/src/vocalpy/spectrogram_maker.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
         # define nested function so vars are in scope and ``dask`` can call it
         def _to_spect(audio_):
             """Make a ``Spectrogram`` from an ``Audio`` instance,
             using self.callback"""
             if isinstance(audio_, AudioFile):
                 audio_ = Audio.read(audio_.path)
             spect = self.callback(audio_, **self.spect_params)
-            spect.source_audio_path = audio_.path
+            spect.audio_path = audio_.path
             return spect
 
         if isinstance(audio, (Audio, AudioFile)):
             return _to_spect(audio)
 
         spects = []
         for audio_ in audio:
```

### Comparing `vocalpy-0.2.0.post1/src/vocalpy/unit.py` & `vocalpy-0.3.0/src/vocalpy/unit.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0.post1/src/vocalpy/validators.py` & `vocalpy-0.3.0/src/vocalpy/validators.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0.post1/tests/fixtures/annot.py` & `vocalpy-0.3.0/tests/fixtures/annot.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0.post1/tests/fixtures/audio.py` & `vocalpy-0.3.0/tests/fixtures/audio.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0.post1/tests/fixtures/datasets.py` & `vocalpy-0.3.0/tests/fixtures/datasets.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0.post1/tests/fixtures/spect.py` & `vocalpy-0.3.0/tests/fixtures/spect.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0.post1/tests/fixtures/test_data.py` & `vocalpy-0.3.0/tests/fixtures/test_data.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0.post1/tests/scripts/generate_data_for_tests.py` & `vocalpy-0.3.0/tests/scripts/generate_data_for_tests.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0.post1/tests/test_annotation_file.py` & `vocalpy-0.3.0/tests/test_annotation_file.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0.post1/tests/test_audio.py` & `vocalpy-0.3.0/tests/test_audio.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0.post1/tests/test_audio_file.py` & `vocalpy-0.3.0/tests/test_audio_file.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0.post1/tests/test_paths.py` & `vocalpy-0.3.0/tests/test_paths.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0.post1/tests/test_segmenter.py` & `vocalpy-0.3.0/tests/test_segmenter.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0.post1/tests/test_sequence.py` & `vocalpy-0.3.0/tests/test_sequence.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0.post1/tests/test_signal/test_segment.py` & `vocalpy-0.3.0/tests/test_signal/test_segment.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0.post1/tests/test_spectrogram.py` & `vocalpy-0.3.0/tests/test_spectrogram.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0.post1/tests/test_spectrogram_file.py` & `vocalpy-0.3.0/tests/test_spectrogram_file.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0.post1/tests/test_spectrogram_maker.py` & `vocalpy-0.3.0/tests/test_spectrogram_maker.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0.post1/tests/test_unit.py` & `vocalpy-0.3.0/tests/test_unit.py`

 * *Files identical despite different names*

