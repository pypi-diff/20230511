# Comparing `tmp/pretext-1.5.3.dev20230509.tar.gz` & `tmp/pretext-1.5.3.dev20230510.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretext-1.5.3.dev20230509.tar", max compression
+gzip compressed data, was "pretext-1.5.3.dev20230510.tar", max compression
```

## Comparing `pretext-1.5.3.dev20230509.tar` & `pretext-1.5.3.dev20230510.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    35148 2023-05-09 06:18:39.212331 pretext-1.5.3.dev20230509/LICENSE
--rw-r--r--   0        0        0     9664 2023-05-09 06:18:39.212331 pretext-1.5.3.dev20230509/README.md
--rw-r--r--   0        0        0     1440 2023-05-09 06:19:11.560216 pretext-1.5.3.dev20230509/pretext/__init__.py
--rw-r--r--   0        0        0       61 2023-05-09 06:18:39.212331 pretext-1.5.3.dev20230509/pretext/__main__.py
--rw-r--r--   0        0        0     7344 2023-05-09 06:18:39.212331 pretext-1.5.3.dev20230509/pretext/build.py
--rw-r--r--   0        0        0    22954 2023-05-09 06:18:39.212331 pretext-1.5.3.dev20230509/pretext/cli.py
--rw-r--r--   0        0        0     5694 2023-05-09 06:18:39.212331 pretext-1.5.3.dev20230509/pretext/codechat.py
--rw-r--r--   0        0        0     5692 2023-05-09 06:18:39.212331 pretext-1.5.3.dev20230509/pretext/config/xml_overlay.py
--rw-r--r--   0        0        0      350 2023-05-09 06:18:39.212331 pretext-1.5.3.dev20230509/pretext/core/__init__.py
--rw-r--r--   0        0        0   173946 2023-05-09 06:19:16.492198 pretext-1.5.3.dev20230509/pretext/core/pretext.py
--rw-r--r--   0        0        0     1465 2023-05-09 06:18:39.212331 pretext-1.5.3.dev20230509/pretext/core/resources.py
--rw-r--r--   0        0        0  1052638 2023-05-09 06:19:16.492198 pretext-1.5.3.dev20230509/pretext/core/resources.zip
--rw-r--r--   0        0        0    15723 2023-05-09 06:18:39.212331 pretext-1.5.3.dev20230509/pretext/generate.py
--rw-r--r--   0        0        0    24172 2023-05-09 06:18:39.212331 pretext-1.5.3.dev20230509/pretext/project.py
--rw-r--r--   0        0        0      516 2023-05-09 06:18:39.212331 pretext-1.5.3.dev20230509/pretext/templates/__init__.py
--rw-r--r--   0        0        0     1676 2023-05-09 06:19:16.564198 pretext-1.5.3.dev20230509/pretext/templates/resources/.gitignore
--rw-r--r--   0        0        0        0 2023-05-09 06:19:16.564198 pretext-1.5.3.dev20230509/pretext/templates/resources/__init__.py
--rw-r--r--   0        0        0   160171 2023-05-09 06:19:16.540198 pretext-1.5.3.dev20230509/pretext/templates/resources/article.zip
--rw-r--r--   0        0        0     7677 2023-05-09 06:19:16.556198 pretext-1.5.3.dev20230509/pretext/templates/resources/book.zip
--rw-r--r--   0        0        0   173370 2023-05-09 06:19:16.552198 pretext-1.5.3.dev20230509/pretext/templates/resources/demo.zip
--rw-r--r--   0        0        0     1236 2023-05-09 06:19:16.564198 pretext-1.5.3.dev20230509/pretext/templates/resources/devcontainer.json
--rw-r--r--   0        0        0     4718 2023-05-09 06:19:16.560198 pretext-1.5.3.dev20230509/pretext/templates/resources/hello.zip
--rw-r--r--   0        0        0      630 2023-05-09 06:19:16.564198 pretext-1.5.3.dev20230509/pretext/templates/resources/postCreateCommand.sh
--rw-r--r--   0        0        0     1710 2023-05-09 06:19:16.560198 pretext-1.5.3.dev20230509/pretext/templates/resources/project.ptx
--rw-r--r--   0        0        0      242 2023-05-09 06:19:16.560198 pretext-1.5.3.dev20230509/pretext/templates/resources/publication.ptx
--rw-r--r--   0        0        0     8453 2023-05-09 06:19:16.560198 pretext-1.5.3.dev20230509/pretext/templates/resources/slideshow.zip
--rw-r--r--   0        0        0    18300 2023-05-09 06:18:39.212331 pretext-1.5.3.dev20230509/pretext/utils.py
--rw-r--r--   0        0        0     1119 2023-05-09 06:19:11.560216 pretext-1.5.3.dev20230509/pyproject.toml
--rw-r--r--   0        0        0    10761 1970-01-01 00:00:00.000000 pretext-1.5.3.dev20230509/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-05-10 06:18:01.553898 pretext-1.5.3.dev20230510/LICENSE
+-rw-r--r--   0        0        0     9664 2023-05-10 06:18:01.553898 pretext-1.5.3.dev20230510/README.md
+-rw-r--r--   0        0        0     1440 2023-05-10 06:18:49.694404 pretext-1.5.3.dev20230510/pretext/__init__.py
+-rw-r--r--   0        0        0       61 2023-05-10 06:18:01.557898 pretext-1.5.3.dev20230510/pretext/__main__.py
+-rw-r--r--   0        0        0     7344 2023-05-10 06:18:01.557898 pretext-1.5.3.dev20230510/pretext/build.py
+-rw-r--r--   0        0        0    22954 2023-05-10 06:18:01.557898 pretext-1.5.3.dev20230510/pretext/cli.py
+-rw-r--r--   0        0        0     5694 2023-05-10 06:18:01.557898 pretext-1.5.3.dev20230510/pretext/codechat.py
+-rw-r--r--   0        0        0     5692 2023-05-10 06:18:01.557898 pretext-1.5.3.dev20230510/pretext/config/xml_overlay.py
+-rw-r--r--   0        0        0      350 2023-05-10 06:18:01.557898 pretext-1.5.3.dev20230510/pretext/core/__init__.py
+-rw-r--r--   0        0        0   173946 2023-05-10 06:18:55.010459 pretext-1.5.3.dev20230510/pretext/core/pretext.py
+-rw-r--r--   0        0        0     1465 2023-05-10 06:18:01.557898 pretext-1.5.3.dev20230510/pretext/core/resources.py
+-rw-r--r--   0        0        0  1054092 2023-05-10 06:18:55.010459 pretext-1.5.3.dev20230510/pretext/core/resources.zip
+-rw-r--r--   0        0        0    15723 2023-05-10 06:18:01.557898 pretext-1.5.3.dev20230510/pretext/generate.py
+-rw-r--r--   0        0        0    24172 2023-05-10 06:18:01.557898 pretext-1.5.3.dev20230510/pretext/project.py
+-rw-r--r--   0        0        0      516 2023-05-10 06:18:01.557898 pretext-1.5.3.dev20230510/pretext/templates/__init__.py
+-rw-r--r--   0        0        0     1676 2023-05-10 06:18:55.098460 pretext-1.5.3.dev20230510/pretext/templates/resources/.gitignore
+-rw-r--r--   0        0        0        0 2023-05-10 06:18:55.098460 pretext-1.5.3.dev20230510/pretext/templates/resources/__init__.py
+-rw-r--r--   0        0        0   160171 2023-05-10 06:18:55.074460 pretext-1.5.3.dev20230510/pretext/templates/resources/article.zip
+-rw-r--r--   0        0        0     7677 2023-05-10 06:18:55.062460 pretext-1.5.3.dev20230510/pretext/templates/resources/book.zip
+-rw-r--r--   0        0        0   173370 2023-05-10 06:18:55.098460 pretext-1.5.3.dev20230510/pretext/templates/resources/demo.zip
+-rw-r--r--   0        0        0     1236 2023-05-10 06:18:55.098460 pretext-1.5.3.dev20230510/pretext/templates/resources/devcontainer.json
+-rw-r--r--   0        0        0     4718 2023-05-10 06:18:55.078460 pretext-1.5.3.dev20230510/pretext/templates/resources/hello.zip
+-rw-r--r--   0        0        0      630 2023-05-10 06:18:55.098460 pretext-1.5.3.dev20230510/pretext/templates/resources/postCreateCommand.sh
+-rw-r--r--   0        0        0     1710 2023-05-10 06:18:55.098460 pretext-1.5.3.dev20230510/pretext/templates/resources/project.ptx
+-rw-r--r--   0        0        0      242 2023-05-10 06:18:55.098460 pretext-1.5.3.dev20230510/pretext/templates/resources/publication.ptx
+-rw-r--r--   0        0        0     8453 2023-05-10 06:18:55.082460 pretext-1.5.3.dev20230510/pretext/templates/resources/slideshow.zip
+-rw-r--r--   0        0        0    18300 2023-05-10 06:18:01.557898 pretext-1.5.3.dev20230510/pretext/utils.py
+-rw-r--r--   0        0        0     1119 2023-05-10 06:18:49.698404 pretext-1.5.3.dev20230510/pyproject.toml
+-rw-r--r--   0        0        0    10761 1970-01-01 00:00:00.000000 pretext-1.5.3.dev20230510/PKG-INFO
```

### Comparing `pretext-1.5.3.dev20230509/LICENSE` & `pretext-1.5.3.dev20230510/LICENSE`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230509/README.md` & `pretext-1.5.3.dev20230510/README.md`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230509/pretext/__init__.py` & `pretext-1.5.3.dev20230510/pretext/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from pathlib import Path
 from single_version import get_version
 
 VERSION = get_version("pretext", Path(__file__).parent.parent)
 
 
-CORE_COMMIT = '7db4ce5c1b6b52969c4cbc53f52445b5322eb2f8'
+CORE_COMMIT = '0987ca59f3984be8bc1851d5ba5ffa4d11f56e1a'
 
 
 def activate():
     """
     This function was provided by the original `pretext` package
     deployed to PyPI by Alex Willmer. Thanks to their generosity,
     we were allowed to adopt this namespace as of 1.0, so we raise an error here
```

### Comparing `pretext-1.5.3.dev20230509/pretext/build.py` & `pretext-1.5.3.dev20230510/pretext/build.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230509/pretext/cli.py` & `pretext-1.5.3.dev20230510/pretext/cli.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230509/pretext/codechat.py` & `pretext-1.5.3.dev20230510/pretext/codechat.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230509/pretext/config/xml_overlay.py` & `pretext-1.5.3.dev20230510/pretext/config/xml_overlay.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230509/pretext/core/pretext.py` & `pretext-1.5.3.dev20230510/pretext/core/pretext.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230509/pretext/core/resources.py` & `pretext-1.5.3.dev20230510/pretext/core/resources.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230509/pretext/core/resources.zip` & `pretext-1.5.3.dev20230510/pretext/core/resources.zip`

 * *Files 8% similar despite different names*

#### zipinfo {}

```diff
@@ -1,150 +1,150 @@
-Zip file size: 1052638 bytes, number of entries: 148
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-09 06:19 css/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-09 06:19 pretext/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-09 06:19 schema/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-09 06:19 script/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-09 06:19 xsl/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-09 06:19 xsl/latex/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-09 06:19 xsl/localizations/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-09 06:19 xsl/support/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-09 06:19 xsl/utilities/
--rw-r--r--  2.0 unx    11766 b- defN 23-May-09 06:19 xsl/pretext-sage-doctest.xsl
--rw-r--r--  2.0 unx   261852 b- defN 23-May-09 06:19 xsl/publisher-variables.xsl
--rw-r--r--  2.0 unx     6066 b- defN 23-May-09 06:19 xsl/pretext-json-manifest.xsl
--rw-r--r--  2.0 unx    21086 b- defN 23-May-09 06:19 xsl/pretext-smc.xsl
--rw-r--r--  2.0 unx    17293 b- defN 23-May-09 06:19 xsl/pretext-ww-problem-sets.xsl
--rw-r--r--  2.0 unx    13186 b- defN 23-May-09 06:19 xsl/pretext-solution-manual-latex.xsl
--rw-r--r--  2.0 unx    13037 b- defN 23-May-09 06:19 xsl/pretext-text.xsl
--rw-r--r--  2.0 unx     3239 b- defN 23-May-09 06:19 xsl/extract-interactive.xsl
--rw-r--r--  2.0 unx    67275 b- defN 23-May-09 06:19 xsl/pretext-epub.xsl
--rw-r--r--  2.0 unx     2597 b- defN 23-May-09 06:19 xsl/extract-trace.xsl
--rw-r--r--  2.0 unx    43020 b- defN 23-May-09 06:19 xsl/pretext-text-utilities.xsl
--rw-r--r--  2.0 unx    69315 b- defN 23-May-09 06:19 xsl/pretext-braille.xsl
--rw-r--r--  2.0 unx     8130 b- defN 23-May-09 06:19 xsl/extract-identity.xsl
--rw-r--r--  2.0 unx   544213 b- defN 23-May-09 06:19 xsl/pretext-common.xsl
--rw-r--r--  2.0 unx    65459 b- defN 23-May-09 06:19 xsl/pretext-braille-preprint.xsl
--rw-r--r--  2.0 unx     8535 b- defN 23-May-09 06:19 xsl/pretext-view-source.xsl
--rw-r--r--  2.0 unx     2709 b- defN 23-May-09 06:19 xsl/extract-qrcode.xsl
--rw-r--r--  2.0 unx     3560 b- defN 23-May-09 06:19 xsl/pretext-basic-html.xsl
--rw-r--r--  2.0 unx     2725 b- defN 23-May-09 06:19 xsl/extract-asymptote.xsl
--rw-r--r--  2.0 unx    19072 b- defN 23-May-09 06:19 xsl/extract-latex-image.xsl
--rw-r--r--  2.0 unx     2601 b- defN 23-May-09 06:19 xsl/pretext-merge.xsl
--rw-r--r--  2.0 unx   139486 b- defN 23-May-09 06:19 xsl/extract-pg.xsl
--rw-r--r--  2.0 unx     1768 b- defN 23-May-09 06:19 xsl/README.md
--rw-r--r--  2.0 unx     2740 b- defN 23-May-09 06:19 xsl/extract-youtube.xsl
--rw-r--r--  2.0 unx   604691 b- defN 23-May-09 06:19 xsl/pretext-html.xsl
--rw-r--r--  2.0 unx     9787 b- defN 23-May-09 06:19 xsl/entities.ent
--rw-r--r--  2.0 unx     2846 b- defN 23-May-09 06:19 xsl/extract-datafile.xsl
--rw-r--r--  2.0 unx    22121 b- defN 23-May-09 06:19 xsl/pretext-revealjs.xsl
--rw-r--r--  2.0 unx    41730 b- defN 23-May-09 06:19 xsl/pretext-beamer.xsl
--rw-r--r--  2.0 unx     6281 b- defN 23-May-09 06:19 xsl/pretext-numbers.xsl
--rw-r--r--  2.0 unx   541182 b- defN 23-May-09 06:19 xsl/pretext-latex.xsl
--rw-r--r--  2.0 unx    40230 b- defN 23-May-09 06:19 xsl/pretext-jupyter.xsl
--rw-r--r--  2.0 unx     2248 b- defN 23-May-09 06:19 xsl/extract-mom.xsl
--rw-r--r--  2.0 unx    39922 b- defN 23-May-09 06:19 xsl/pretext-runestone-static.xsl
--rw-r--r--  2.0 unx     8125 b- defN 23-May-09 06:19 xsl/extract-sageplot.xsl
--rw-r--r--  2.0 unx   103788 b- defN 23-May-09 06:19 xsl/pretext-runestone.xsl
--rw-r--r--  2.0 unx    10708 b- defN 23-May-09 06:19 xsl/pretext-units.xsl
--rw-r--r--  2.0 unx   111553 b- defN 23-May-09 06:19 xsl/pretext-assembly.xsl
--rw-r--r--  2.0 unx     4571 b- defN 23-May-09 06:19 xsl/pretext-litprog.xsl
--rw-r--r--  2.0 unx      787 b- defN 23-May-09 06:19 xsl/utilities/deprecate-index.sed
--rw-r--r--  2.0 unx     1810 b- defN 23-May-09 06:19 xsl/utilities/README.md
--rw-r--r--  2.0 unx      513 b- defN 23-May-09 06:19 xsl/utilities/deprecate-autoname.sed
--rw-r--r--  2.0 unx     4299 b- defN 23-May-09 06:19 xsl/utilities/author-report.xsl
--rw-r--r--  2.0 unx    30257 b- defN 23-May-09 06:19 xsl/utilities/fix-deprecations.xsl
--rw-r--r--  2.0 unx     4926 b- defN 23-May-09 06:19 xsl/utilities/pretext-enhanced-source.xsl
--rw-r--r--  2.0 unx    17285 b- defN 23-May-09 06:19 xsl/localizations/fi-FI.xml
--rw-r--r--  2.0 unx    16333 b- defN 23-May-09 06:19 xsl/localizations/fr-FR.xml
--rw-r--r--  2.0 unx    16518 b- defN 23-May-09 06:19 xsl/localizations/es-ES.xml
--rw-r--r--  2.0 unx    19049 b- defN 23-May-09 06:19 xsl/localizations/en-US.xml
--rw-r--r--  2.0 unx    15736 b- defN 23-May-09 06:19 xsl/localizations/cs-CZ.xml
--rw-r--r--  2.0 unx    17040 b- defN 23-May-09 06:19 xsl/localizations/bg-BG.xml
--rw-r--r--  2.0 unx    16236 b- defN 23-May-09 06:19 xsl/localizations/ca-ES.xml
--rw-r--r--  2.0 unx    19169 b- defN 23-May-09 06:19 xsl/localizations/nl-NL.xml
--rw-r--r--  2.0 unx    16296 b- defN 23-May-09 06:19 xsl/localizations/pt-BR.xml
--rw-r--r--  2.0 unx     4708 b- defN 23-May-09 06:19 xsl/localizations/README.md
--rw-r--r--  2.0 unx     2227 b- defN 23-May-09 06:19 xsl/localizations/localizations.xml
--rw-r--r--  2.0 unx    17215 b- defN 23-May-09 06:19 xsl/localizations/de-DE.xml
--rw-r--r--  2.0 unx    16821 b- defN 23-May-09 06:19 xsl/localizations/af-ZA.xml
--rw-r--r--  2.0 unx    16069 b- defN 23-May-09 06:19 xsl/localizations/hu-HU.xml
--rw-r--r--  2.0 unx    15938 b- defN 23-May-09 06:19 xsl/localizations/it-IT.xml
--rw-r--r--  2.0 unx    16484 b- defN 23-May-09 06:19 xsl/localizations/fr-CA.xml
--rw-r--r--  2.0 unx    17065 b- defN 23-May-09 06:19 xsl/localizations/pt-PT.xml
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-09 06:19 xsl/support/play-button/
--rw-r--r--  2.0 unx     5800 b- defN 23-May-09 06:19 xsl/support/tactile-svg.xsl
--rw-r--r--  2.0 unx     5879 b- defN 23-May-09 06:19 xsl/support/package-math.xsl
--rw-r--r--  2.0 unx     5065 b- defN 23-May-09 06:19 xsl/support/extract-latex-image-labels.xsl
--rw-r--r--  2.0 unx    10306 b- defN 23-May-09 06:19 xsl/support/extract-math.xsl
--rw-r--r--  2.0 unx      504 b- defN 23-May-09 06:19 xsl/support/README.md
--rw-r--r--  2.0 unx      486 b- defN 23-May-09 06:19 xsl/support/runestone-services.xml
--rw-r--r--  2.0 unx     5241 b- defN 23-May-09 06:19 xsl/support/pretext-pg-macros.xsl
--rw-r--r--  2.0 unx      722 b- defN 23-May-09 06:19 xsl/support/play-button/play-button.svg
--rw-r--r--  2.0 unx     2657 b- defN 23-May-09 06:19 xsl/support/play-button/README.md
--rw-r--r--  2.0 unx     6621 b- defN 23-May-09 06:19 xsl/support/play-button/play-button.png
--rw-r--r--  2.0 unx     3024 b- defN 23-May-09 06:19 xsl/latex/pretext-latex-dyslexic-font.xsl
--rw-r--r--  2.0 unx     5135 b- defN 23-May-09 06:19 xsl/latex/pretext-latex-guide.xsl
--rw-r--r--  2.0 unx    14482 b- defN 23-May-09 06:19 xsl/latex/pretext-latex-chaos.xsl
--rw-r--r--  2.0 unx     2261 b- defN 23-May-09 06:19 xsl/latex/pretext-latex-AIM.xsl
--rw-r--r--  2.0 unx     7526 b- defN 23-May-09 06:19 xsl/latex/pretext-latex-CLP.xsl
--rw-r--r--  2.0 unx   133930 b- defN 23-May-09 06:19 schema/pretext.xml
--rw-r--r--  2.0 unx   124610 b- defN 23-May-09 06:19 schema/pretext.xsd
--rw-r--r--  2.0 unx    18421 b- defN 23-May-09 06:19 schema/pretext-schematron.xsl
--rw-r--r--  2.0 unx      326 b- defN 23-May-09 06:19 schema/xml.xsd
--rw-r--r--  2.0 unx    57973 b- defN 23-May-09 06:19 schema/pretext.rnc
--rw-r--r--  2.0 unx     1180 b- defN 23-May-09 06:19 schema/README.md
--rw-r--r--  2.0 unx     3135 b- defN 23-May-09 06:19 schema/build.sh
--rw-r--r--  2.0 unx    34210 b- defN 23-May-09 06:19 schema/pretext-dev.rng
--rw-r--r--  2.0 unx    25290 b- defN 23-May-09 06:19 schema/pretext-validation-plus.xsl
--rw-r--r--  2.0 unx    17587 b- defN 23-May-09 06:19 schema/pretext-dev.rnc
--rw-r--r--  2.0 unx   101444 b- defN 23-May-09 06:19 schema/pretext.rng
--rw-r--r--  2.0 unx     2446 b- defN 23-May-09 06:19 css/colors_darkmartiansands.css
--rw-r--r--  2.0 unx      691 b- defN 23-May-09 06:19 css/colors_pastel_blue_orange.css
--rw-r--r--  2.0 unx    71198 b- defN 23-May-09 06:19 css/pretext_add_on.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-09 06:19 css/colors_green_blue.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-09 06:19 css/colors_green_plum.css
--rw-r--r--  2.0 unx     2446 b- defN 23-May-09 06:19 css/colors_martiansands.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-09 06:19 css/colors_orange_navy.css
--rw-r--r--  2.0 unx     1280 b- defN 23-May-09 06:19 css/colors_brown_gold.css
--rw-r--r--  2.0 unx     2438 b- defN 23-May-09 06:19 css/colors_blue_grey.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-09 06:19 css/colors_ruby_turquoise.css
--rw-r--r--  2.0 unx    12567 b- defN 23-May-09 06:19 css/style_oscarlevin.css
--rw-r--r--  2.0 unx    14069 b- defN 23-May-09 06:19 css/setcolors.css
--rw-r--r--  2.0 unx     1865 b- defN 23-May-09 06:19 css/README.md
--rw-r--r--  2.0 unx     4021 b- defN 23-May-09 06:19 css/update_css
--rw-r--r--  2.0 unx     4308 b- defN 23-May-09 06:19 css/colors_blue_green.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-09 06:19 css/colors_ruby_emerald.css
--rw-r--r--  2.0 unx   146685 b- defN 23-May-09 06:19 css/mathbook-content.css
--rw-r--r--  2.0 unx    22438 b- defN 23-May-09 06:19 css/pretext.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-09 06:19 css/colors_blue_red.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-09 06:19 css/colors_ruby_amethyst.css
--rw-r--r--  2.0 unx     7761 b- defN 23-May-09 06:19 css/style_default.css
--rw-r--r--  2.0 unx     1362 b- defN 23-May-09 06:19 css/epub.css
--rw-r--r--  2.0 unx     2608 b- defN 23-May-09 06:19 css/colors_default.css
--rw-r--r--  2.0 unx     3473 b- defN 23-May-09 06:19 css/style_soundwriting.css
--rw-r--r--  2.0 unx   435680 b- defN 23-May-09 06:19 css/mathbook-3.css
--rw-r--r--  2.0 unx     1338 b- defN 23-May-09 06:19 css/colors_red_blue.css
--rw-r--r--  2.0 unx     2441 b- defN 23-May-09 06:19 css/kindle.css
--rw-r--r--  2.0 unx    63664 b- defN 23-May-09 06:19 css/mathbook-add-on.css
--rw-r--r--  2.0 unx     1276 b- defN 23-May-09 06:19 css/colors_maroon_grey.css
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-09 06:19 script/braille/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-09 06:19 script/mjsre/
--rw-r--r--  2.0 unx      258 b- defN 23-May-09 06:19 script/README.md
--rw-r--r--  2.0 unx     2666 b- defN 23-May-09 06:19 script/mbx
--rw-r--r--  2.0 unx     2573 b- defN 23-May-09 06:19 script/braille/pretext-symbol.dis
--rw-r--r--  2.0 unx     8913 b- defN 23-May-09 06:19 script/braille/pretext.sem
--rw-r--r--  2.0 unx      735 b- defN 23-May-09 06:19 script/braille/README.md
--rw-r--r--  2.0 unx     6616 b- defN 23-May-09 06:19 script/braille/pretext-liblouis.cfg
--rw-r--r--  2.0 unx     1011 b- defN 23-May-09 06:19 script/braille/pretext-liblouis-emboss.cfg
--rw-r--r--  2.0 unx      490 b- defN 23-May-09 06:19 script/braille/pretext-liblouis-electronic.cfg
--rw-r--r--  2.0 unx      481 b- defN 23-May-09 06:19 script/mjsre/README.md
--rw-r--r--  2.0 unx       92 b- defN 23-May-09 06:19 script/mjsre/update-sre
--rw-r--r--  2.0 unx     9251 b- defN 23-May-09 06:19 script/mjsre/mj-sre-page.js
--rw-r--r--  2.0 unx      116 b- defN 23-May-09 06:19 script/mjsre/package.json
--rw-r--r--  2.0 unx     2566 b- defN 23-May-09 06:19 pretext/pretext.cfg
--rw-r--r--  2.0 unx     1367 b- defN 23-May-09 06:19 pretext/README.md
--rw-r--r--  2.0 unx   173946 b- defN 23-May-09 06:19 pretext/pretext.py
--rw-r--r--  2.0 unx    35057 b- defN 23-May-09 06:19 pretext/braille_format.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-09 06:19 pretext/__init__.py
--rw-r--r--  2.0 unx     1955 b- defN 23-May-09 06:19 pretext/module-test.py
--rw-r--r--  2.0 unx    31361 b- defN 23-May-09 06:19 pretext/pretext
-148 files, 4879397 bytes uncompressed, 1034214 bytes compressed:  78.8%
+Zip file size: 1054092 bytes, number of entries: 148
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-10 06:18 css/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-10 06:18 pretext/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-10 06:18 schema/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-10 06:18 script/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-10 06:18 xsl/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-10 06:18 script/braille/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-10 06:18 script/mjsre/
+-rw-r--r--  2.0 unx      258 b- defN 23-May-10 06:18 script/README.md
+-rw-r--r--  2.0 unx     2666 b- defN 23-May-10 06:18 script/mbx
+-rw-r--r--  2.0 unx       92 b- defN 23-May-10 06:18 script/mjsre/update-sre
+-rw-r--r--  2.0 unx      481 b- defN 23-May-10 06:18 script/mjsre/README.md
+-rw-r--r--  2.0 unx      116 b- defN 23-May-10 06:18 script/mjsre/package.json
+-rw-r--r--  2.0 unx     9251 b- defN 23-May-10 06:18 script/mjsre/mj-sre-page.js
+-rw-r--r--  2.0 unx     8913 b- defN 23-May-10 06:18 script/braille/pretext.sem
+-rw-r--r--  2.0 unx      735 b- defN 23-May-10 06:18 script/braille/README.md
+-rw-r--r--  2.0 unx     2573 b- defN 23-May-10 06:18 script/braille/pretext-symbol.dis
+-rw-r--r--  2.0 unx     6616 b- defN 23-May-10 06:18 script/braille/pretext-liblouis.cfg
+-rw-r--r--  2.0 unx     1011 b- defN 23-May-10 06:18 script/braille/pretext-liblouis-emboss.cfg
+-rw-r--r--  2.0 unx      490 b- defN 23-May-10 06:18 script/braille/pretext-liblouis-electronic.cfg
+-rw-r--r--  2.0 unx    18421 b- defN 23-May-10 06:18 schema/pretext-schematron.xsl
+-rw-r--r--  2.0 unx    57973 b- defN 23-May-10 06:18 schema/pretext.rnc
+-rw-r--r--  2.0 unx    25290 b- defN 23-May-10 06:18 schema/pretext-validation-plus.xsl
+-rw-r--r--  2.0 unx   133930 b- defN 23-May-10 06:18 schema/pretext.xml
+-rw-r--r--  2.0 unx     1180 b- defN 23-May-10 06:18 schema/README.md
+-rw-r--r--  2.0 unx   124610 b- defN 23-May-10 06:18 schema/pretext.xsd
+-rw-r--r--  2.0 unx      326 b- defN 23-May-10 06:18 schema/xml.xsd
+-rw-r--r--  2.0 unx    34210 b- defN 23-May-10 06:18 schema/pretext-dev.rng
+-rw-r--r--  2.0 unx   101444 b- defN 23-May-10 06:18 schema/pretext.rng
+-rw-r--r--  2.0 unx    17587 b- defN 23-May-10 06:18 schema/pretext-dev.rnc
+-rw-r--r--  2.0 unx     3135 b- defN 23-May-10 06:18 schema/build.sh
+-rw-r--r--  2.0 unx     1367 b- defN 23-May-10 06:18 pretext/README.md
+-rw-r--r--  2.0 unx   173946 b- defN 23-May-10 06:18 pretext/pretext.py
+-rw-r--r--  2.0 unx     1955 b- defN 23-May-10 06:18 pretext/module-test.py
+-rw-r--r--  2.0 unx    31361 b- defN 23-May-10 06:18 pretext/pretext
+-rw-r--r--  2.0 unx        0 b- defN 23-May-10 06:18 pretext/__init__.py
+-rw-r--r--  2.0 unx    35057 b- defN 23-May-10 06:18 pretext/braille_format.py
+-rw-r--r--  2.0 unx     2566 b- defN 23-May-10 06:18 pretext/pretext.cfg
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-10 06:18 xsl/latex/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-10 06:18 xsl/localizations/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-10 06:18 xsl/support/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-10 06:18 xsl/utilities/
+-rw-r--r--  2.0 unx     9787 b- defN 23-May-10 06:18 xsl/entities.ent
+-rw-r--r--  2.0 unx     3239 b- defN 23-May-10 06:18 xsl/extract-interactive.xsl
+-rw-r--r--  2.0 unx    13037 b- defN 23-May-10 06:18 xsl/pretext-text.xsl
+-rw-r--r--  2.0 unx     1768 b- defN 23-May-10 06:18 xsl/README.md
+-rw-r--r--  2.0 unx   139486 b- defN 23-May-10 06:18 xsl/extract-pg.xsl
+-rw-r--r--  2.0 unx     6066 b- defN 23-May-10 06:18 xsl/pretext-json-manifest.xsl
+-rw-r--r--  2.0 unx    22121 b- defN 23-May-10 06:18 xsl/pretext-revealjs.xsl
+-rw-r--r--  2.0 unx     2846 b- defN 23-May-10 06:18 xsl/extract-datafile.xsl
+-rw-r--r--  2.0 unx     8130 b- defN 23-May-10 06:18 xsl/extract-identity.xsl
+-rw-r--r--  2.0 unx     8125 b- defN 23-May-10 06:18 xsl/extract-sageplot.xsl
+-rw-r--r--  2.0 unx    69315 b- defN 23-May-10 06:18 xsl/pretext-braille.xsl
+-rw-r--r--  2.0 unx   261852 b- defN 23-May-10 06:18 xsl/publisher-variables.xsl
+-rw-r--r--  2.0 unx   103788 b- defN 23-May-10 06:18 xsl/pretext-runestone.xsl
+-rw-r--r--  2.0 unx    11766 b- defN 23-May-10 06:18 xsl/pretext-sage-doctest.xsl
+-rw-r--r--  2.0 unx    39922 b- defN 23-May-10 06:18 xsl/pretext-runestone-static.xsl
+-rw-r--r--  2.0 unx    17293 b- defN 23-May-10 06:18 xsl/pretext-ww-problem-sets.xsl
+-rw-r--r--  2.0 unx   541182 b- defN 23-May-10 06:18 xsl/pretext-latex.xsl
+-rw-r--r--  2.0 unx     2601 b- defN 23-May-10 06:18 xsl/pretext-merge.xsl
+-rw-r--r--  2.0 unx     4571 b- defN 23-May-10 06:18 xsl/pretext-litprog.xsl
+-rw-r--r--  2.0 unx    19072 b- defN 23-May-10 06:18 xsl/extract-latex-image.xsl
+-rw-r--r--  2.0 unx    67275 b- defN 23-May-10 06:18 xsl/pretext-epub.xsl
+-rw-r--r--  2.0 unx     8535 b- defN 23-May-10 06:18 xsl/pretext-view-source.xsl
+-rw-r--r--  2.0 unx     6281 b- defN 23-May-10 06:18 xsl/pretext-numbers.xsl
+-rw-r--r--  2.0 unx   111553 b- defN 23-May-10 06:18 xsl/pretext-assembly.xsl
+-rw-r--r--  2.0 unx     2248 b- defN 23-May-10 06:18 xsl/extract-mom.xsl
+-rw-r--r--  2.0 unx    21086 b- defN 23-May-10 06:18 xsl/pretext-smc.xsl
+-rw-r--r--  2.0 unx   544213 b- defN 23-May-10 06:18 xsl/pretext-common.xsl
+-rw-r--r--  2.0 unx     2740 b- defN 23-May-10 06:18 xsl/extract-youtube.xsl
+-rw-r--r--  2.0 unx    41730 b- defN 23-May-10 06:18 xsl/pretext-beamer.xsl
+-rw-r--r--  2.0 unx    13186 b- defN 23-May-10 06:18 xsl/pretext-solution-manual-latex.xsl
+-rw-r--r--  2.0 unx    72788 b- defN 23-May-10 06:18 xsl/pretext-braille-preprint.xsl
+-rw-r--r--  2.0 unx    10708 b- defN 23-May-10 06:18 xsl/pretext-units.xsl
+-rw-r--r--  2.0 unx     3560 b- defN 23-May-10 06:18 xsl/pretext-basic-html.xsl
+-rw-r--r--  2.0 unx     2725 b- defN 23-May-10 06:18 xsl/extract-asymptote.xsl
+-rw-r--r--  2.0 unx   604691 b- defN 23-May-10 06:18 xsl/pretext-html.xsl
+-rw-r--r--  2.0 unx     2597 b- defN 23-May-10 06:18 xsl/extract-trace.xsl
+-rw-r--r--  2.0 unx    43020 b- defN 23-May-10 06:18 xsl/pretext-text-utilities.xsl
+-rw-r--r--  2.0 unx    40230 b- defN 23-May-10 06:18 xsl/pretext-jupyter.xsl
+-rw-r--r--  2.0 unx     2709 b- defN 23-May-10 06:18 xsl/extract-qrcode.xsl
+-rw-r--r--  2.0 unx     7526 b- defN 23-May-10 06:18 xsl/latex/pretext-latex-CLP.xsl
+-rw-r--r--  2.0 unx     3024 b- defN 23-May-10 06:18 xsl/latex/pretext-latex-dyslexic-font.xsl
+-rw-r--r--  2.0 unx     2261 b- defN 23-May-10 06:18 xsl/latex/pretext-latex-AIM.xsl
+-rw-r--r--  2.0 unx    14482 b- defN 23-May-10 06:18 xsl/latex/pretext-latex-chaos.xsl
+-rw-r--r--  2.0 unx     5135 b- defN 23-May-10 06:18 xsl/latex/pretext-latex-guide.xsl
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-10 06:18 xsl/support/play-button/
+-rw-r--r--  2.0 unx      504 b- defN 23-May-10 06:18 xsl/support/README.md
+-rw-r--r--  2.0 unx    10306 b- defN 23-May-10 06:18 xsl/support/extract-math.xsl
+-rw-r--r--  2.0 unx     5241 b- defN 23-May-10 06:18 xsl/support/pretext-pg-macros.xsl
+-rw-r--r--  2.0 unx     5879 b- defN 23-May-10 06:18 xsl/support/package-math.xsl
+-rw-r--r--  2.0 unx      486 b- defN 23-May-10 06:18 xsl/support/runestone-services.xml
+-rw-r--r--  2.0 unx     5800 b- defN 23-May-10 06:18 xsl/support/tactile-svg.xsl
+-rw-r--r--  2.0 unx     5065 b- defN 23-May-10 06:18 xsl/support/extract-latex-image-labels.xsl
+-rw-r--r--  2.0 unx     2657 b- defN 23-May-10 06:18 xsl/support/play-button/README.md
+-rw-r--r--  2.0 unx      722 b- defN 23-May-10 06:18 xsl/support/play-button/play-button.svg
+-rw-r--r--  2.0 unx     6621 b- defN 23-May-10 06:18 xsl/support/play-button/play-button.png
+-rw-r--r--  2.0 unx    16518 b- defN 23-May-10 06:18 xsl/localizations/es-ES.xml
+-rw-r--r--  2.0 unx    16069 b- defN 23-May-10 06:18 xsl/localizations/hu-HU.xml
+-rw-r--r--  2.0 unx    17215 b- defN 23-May-10 06:18 xsl/localizations/de-DE.xml
+-rw-r--r--  2.0 unx    16333 b- defN 23-May-10 06:18 xsl/localizations/fr-FR.xml
+-rw-r--r--  2.0 unx    17285 b- defN 23-May-10 06:18 xsl/localizations/fi-FI.xml
+-rw-r--r--  2.0 unx     4708 b- defN 23-May-10 06:18 xsl/localizations/README.md
+-rw-r--r--  2.0 unx    15938 b- defN 23-May-10 06:18 xsl/localizations/it-IT.xml
+-rw-r--r--  2.0 unx    16821 b- defN 23-May-10 06:18 xsl/localizations/af-ZA.xml
+-rw-r--r--  2.0 unx    16236 b- defN 23-May-10 06:18 xsl/localizations/ca-ES.xml
+-rw-r--r--  2.0 unx    19049 b- defN 23-May-10 06:18 xsl/localizations/en-US.xml
+-rw-r--r--  2.0 unx    19169 b- defN 23-May-10 06:18 xsl/localizations/nl-NL.xml
+-rw-r--r--  2.0 unx     2227 b- defN 23-May-10 06:18 xsl/localizations/localizations.xml
+-rw-r--r--  2.0 unx    15736 b- defN 23-May-10 06:18 xsl/localizations/cs-CZ.xml
+-rw-r--r--  2.0 unx    17040 b- defN 23-May-10 06:18 xsl/localizations/bg-BG.xml
+-rw-r--r--  2.0 unx    17065 b- defN 23-May-10 06:18 xsl/localizations/pt-PT.xml
+-rw-r--r--  2.0 unx    16484 b- defN 23-May-10 06:18 xsl/localizations/fr-CA.xml
+-rw-r--r--  2.0 unx    16296 b- defN 23-May-10 06:18 xsl/localizations/pt-BR.xml
+-rw-r--r--  2.0 unx     1810 b- defN 23-May-10 06:18 xsl/utilities/README.md
+-rw-r--r--  2.0 unx    30257 b- defN 23-May-10 06:18 xsl/utilities/fix-deprecations.xsl
+-rw-r--r--  2.0 unx     4926 b- defN 23-May-10 06:18 xsl/utilities/pretext-enhanced-source.xsl
+-rw-r--r--  2.0 unx      513 b- defN 23-May-10 06:18 xsl/utilities/deprecate-autoname.sed
+-rw-r--r--  2.0 unx     4299 b- defN 23-May-10 06:18 xsl/utilities/author-report.xsl
+-rw-r--r--  2.0 unx      787 b- defN 23-May-10 06:18 xsl/utilities/deprecate-index.sed
+-rw-r--r--  2.0 unx     1276 b- defN 23-May-10 06:18 css/colors_maroon_grey.css
+-rw-r--r--  2.0 unx     7761 b- defN 23-May-10 06:18 css/style_default.css
+-rw-r--r--  2.0 unx     3473 b- defN 23-May-10 06:18 css/style_soundwriting.css
+-rw-r--r--  2.0 unx    63664 b- defN 23-May-10 06:18 css/mathbook-add-on.css
+-rw-r--r--  2.0 unx     1865 b- defN 23-May-10 06:18 css/README.md
+-rw-r--r--  2.0 unx     1280 b- defN 23-May-10 06:18 css/colors_brown_gold.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-10 06:18 css/colors_blue_red.css
+-rw-r--r--  2.0 unx   435680 b- defN 23-May-10 06:18 css/mathbook-3.css
+-rw-r--r--  2.0 unx   146685 b- defN 23-May-10 06:18 css/mathbook-content.css
+-rw-r--r--  2.0 unx    22438 b- defN 23-May-10 06:18 css/pretext.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-10 06:18 css/colors_green_plum.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-10 06:18 css/colors_ruby_turquoise.css
+-rw-r--r--  2.0 unx     4308 b- defN 23-May-10 06:18 css/colors_blue_green.css
+-rw-r--r--  2.0 unx    71198 b- defN 23-May-10 06:18 css/pretext_add_on.css
+-rw-r--r--  2.0 unx     2608 b- defN 23-May-10 06:18 css/colors_default.css
+-rw-r--r--  2.0 unx     2438 b- defN 23-May-10 06:18 css/colors_blue_grey.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-10 06:18 css/colors_green_blue.css
+-rw-r--r--  2.0 unx     2446 b- defN 23-May-10 06:18 css/colors_darkmartiansands.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-10 06:18 css/colors_orange_navy.css
+-rw-r--r--  2.0 unx    12567 b- defN 23-May-10 06:18 css/style_oscarlevin.css
+-rw-r--r--  2.0 unx      691 b- defN 23-May-10 06:18 css/colors_pastel_blue_orange.css
+-rw-r--r--  2.0 unx     1338 b- defN 23-May-10 06:18 css/colors_red_blue.css
+-rw-r--r--  2.0 unx    14069 b- defN 23-May-10 06:18 css/setcolors.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-10 06:18 css/colors_ruby_amethyst.css
+-rw-r--r--  2.0 unx     2446 b- defN 23-May-10 06:18 css/colors_martiansands.css
+-rw-r--r--  2.0 unx     1362 b- defN 23-May-10 06:18 css/epub.css
+-rw-r--r--  2.0 unx     2441 b- defN 23-May-10 06:18 css/kindle.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-10 06:18 css/colors_ruby_emerald.css
+-rw-r--r--  2.0 unx     4021 b- defN 23-May-10 06:18 css/update_css
+148 files, 4886726 bytes uncompressed, 1035668 bytes compressed:  78.8%
```

#### zipnote {}

```diff
@@ -9,437 +9,437 @@
 
 Filename: script/
 Comment: 
 
 Filename: xsl/
 Comment: 
 
-Filename: xsl/latex/
-Comment: 
-
-Filename: xsl/localizations/
+Filename: script/braille/
 Comment: 
 
-Filename: xsl/support/
+Filename: script/mjsre/
 Comment: 
 
-Filename: xsl/utilities/
+Filename: script/README.md
 Comment: 
 
-Filename: xsl/pretext-sage-doctest.xsl
+Filename: script/mbx
 Comment: 
 
-Filename: xsl/publisher-variables.xsl
+Filename: script/mjsre/update-sre
 Comment: 
 
-Filename: xsl/pretext-json-manifest.xsl
+Filename: script/mjsre/README.md
 Comment: 
 
-Filename: xsl/pretext-smc.xsl
+Filename: script/mjsre/package.json
 Comment: 
 
-Filename: xsl/pretext-ww-problem-sets.xsl
+Filename: script/mjsre/mj-sre-page.js
 Comment: 
 
-Filename: xsl/pretext-solution-manual-latex.xsl
+Filename: script/braille/pretext.sem
 Comment: 
 
-Filename: xsl/pretext-text.xsl
+Filename: script/braille/README.md
 Comment: 
 
-Filename: xsl/extract-interactive.xsl
+Filename: script/braille/pretext-symbol.dis
 Comment: 
 
-Filename: xsl/pretext-epub.xsl
+Filename: script/braille/pretext-liblouis.cfg
 Comment: 
 
-Filename: xsl/extract-trace.xsl
+Filename: script/braille/pretext-liblouis-emboss.cfg
 Comment: 
 
-Filename: xsl/pretext-text-utilities.xsl
+Filename: script/braille/pretext-liblouis-electronic.cfg
 Comment: 
 
-Filename: xsl/pretext-braille.xsl
+Filename: schema/pretext-schematron.xsl
 Comment: 
 
-Filename: xsl/extract-identity.xsl
+Filename: schema/pretext.rnc
 Comment: 
 
-Filename: xsl/pretext-common.xsl
+Filename: schema/pretext-validation-plus.xsl
 Comment: 
 
-Filename: xsl/pretext-braille-preprint.xsl
+Filename: schema/pretext.xml
 Comment: 
 
-Filename: xsl/pretext-view-source.xsl
+Filename: schema/README.md
 Comment: 
 
-Filename: xsl/extract-qrcode.xsl
+Filename: schema/pretext.xsd
 Comment: 
 
-Filename: xsl/pretext-basic-html.xsl
+Filename: schema/xml.xsd
 Comment: 
 
-Filename: xsl/extract-asymptote.xsl
+Filename: schema/pretext-dev.rng
 Comment: 
 
-Filename: xsl/extract-latex-image.xsl
+Filename: schema/pretext.rng
 Comment: 
 
-Filename: xsl/pretext-merge.xsl
+Filename: schema/pretext-dev.rnc
 Comment: 
 
-Filename: xsl/extract-pg.xsl
+Filename: schema/build.sh
 Comment: 
 
-Filename: xsl/README.md
+Filename: pretext/README.md
 Comment: 
 
-Filename: xsl/extract-youtube.xsl
+Filename: pretext/pretext.py
 Comment: 
 
-Filename: xsl/pretext-html.xsl
+Filename: pretext/module-test.py
 Comment: 
 
-Filename: xsl/entities.ent
+Filename: pretext/pretext
 Comment: 
 
-Filename: xsl/extract-datafile.xsl
+Filename: pretext/__init__.py
 Comment: 
 
-Filename: xsl/pretext-revealjs.xsl
+Filename: pretext/braille_format.py
 Comment: 
 
-Filename: xsl/pretext-beamer.xsl
+Filename: pretext/pretext.cfg
 Comment: 
 
-Filename: xsl/pretext-numbers.xsl
+Filename: xsl/latex/
 Comment: 
 
-Filename: xsl/pretext-latex.xsl
+Filename: xsl/localizations/
 Comment: 
 
-Filename: xsl/pretext-jupyter.xsl
+Filename: xsl/support/
 Comment: 
 
-Filename: xsl/extract-mom.xsl
+Filename: xsl/utilities/
 Comment: 
 
-Filename: xsl/pretext-runestone-static.xsl
+Filename: xsl/entities.ent
 Comment: 
 
-Filename: xsl/extract-sageplot.xsl
+Filename: xsl/extract-interactive.xsl
 Comment: 
 
-Filename: xsl/pretext-runestone.xsl
+Filename: xsl/pretext-text.xsl
 Comment: 
 
-Filename: xsl/pretext-units.xsl
+Filename: xsl/README.md
 Comment: 
 
-Filename: xsl/pretext-assembly.xsl
+Filename: xsl/extract-pg.xsl
 Comment: 
 
-Filename: xsl/pretext-litprog.xsl
+Filename: xsl/pretext-json-manifest.xsl
 Comment: 
 
-Filename: xsl/utilities/deprecate-index.sed
+Filename: xsl/pretext-revealjs.xsl
 Comment: 
 
-Filename: xsl/utilities/README.md
+Filename: xsl/extract-datafile.xsl
 Comment: 
 
-Filename: xsl/utilities/deprecate-autoname.sed
+Filename: xsl/extract-identity.xsl
 Comment: 
 
-Filename: xsl/utilities/author-report.xsl
+Filename: xsl/extract-sageplot.xsl
 Comment: 
 
-Filename: xsl/utilities/fix-deprecations.xsl
+Filename: xsl/pretext-braille.xsl
 Comment: 
 
-Filename: xsl/utilities/pretext-enhanced-source.xsl
+Filename: xsl/publisher-variables.xsl
 Comment: 
 
-Filename: xsl/localizations/fi-FI.xml
+Filename: xsl/pretext-runestone.xsl
 Comment: 
 
-Filename: xsl/localizations/fr-FR.xml
+Filename: xsl/pretext-sage-doctest.xsl
 Comment: 
 
-Filename: xsl/localizations/es-ES.xml
+Filename: xsl/pretext-runestone-static.xsl
 Comment: 
 
-Filename: xsl/localizations/en-US.xml
+Filename: xsl/pretext-ww-problem-sets.xsl
 Comment: 
 
-Filename: xsl/localizations/cs-CZ.xml
+Filename: xsl/pretext-latex.xsl
 Comment: 
 
-Filename: xsl/localizations/bg-BG.xml
+Filename: xsl/pretext-merge.xsl
 Comment: 
 
-Filename: xsl/localizations/ca-ES.xml
+Filename: xsl/pretext-litprog.xsl
 Comment: 
 
-Filename: xsl/localizations/nl-NL.xml
+Filename: xsl/extract-latex-image.xsl
 Comment: 
 
-Filename: xsl/localizations/pt-BR.xml
+Filename: xsl/pretext-epub.xsl
 Comment: 
 
-Filename: xsl/localizations/README.md
+Filename: xsl/pretext-view-source.xsl
 Comment: 
 
-Filename: xsl/localizations/localizations.xml
+Filename: xsl/pretext-numbers.xsl
 Comment: 
 
-Filename: xsl/localizations/de-DE.xml
+Filename: xsl/pretext-assembly.xsl
 Comment: 
 
-Filename: xsl/localizations/af-ZA.xml
+Filename: xsl/extract-mom.xsl
 Comment: 
 
-Filename: xsl/localizations/hu-HU.xml
+Filename: xsl/pretext-smc.xsl
 Comment: 
 
-Filename: xsl/localizations/it-IT.xml
+Filename: xsl/pretext-common.xsl
 Comment: 
 
-Filename: xsl/localizations/fr-CA.xml
+Filename: xsl/extract-youtube.xsl
 Comment: 
 
-Filename: xsl/localizations/pt-PT.xml
+Filename: xsl/pretext-beamer.xsl
 Comment: 
 
-Filename: xsl/support/play-button/
+Filename: xsl/pretext-solution-manual-latex.xsl
 Comment: 
 
-Filename: xsl/support/tactile-svg.xsl
+Filename: xsl/pretext-braille-preprint.xsl
 Comment: 
 
-Filename: xsl/support/package-math.xsl
+Filename: xsl/pretext-units.xsl
 Comment: 
 
-Filename: xsl/support/extract-latex-image-labels.xsl
+Filename: xsl/pretext-basic-html.xsl
 Comment: 
 
-Filename: xsl/support/extract-math.xsl
+Filename: xsl/extract-asymptote.xsl
 Comment: 
 
-Filename: xsl/support/README.md
+Filename: xsl/pretext-html.xsl
 Comment: 
 
-Filename: xsl/support/runestone-services.xml
+Filename: xsl/extract-trace.xsl
 Comment: 
 
-Filename: xsl/support/pretext-pg-macros.xsl
+Filename: xsl/pretext-text-utilities.xsl
 Comment: 
 
-Filename: xsl/support/play-button/play-button.svg
+Filename: xsl/pretext-jupyter.xsl
 Comment: 
 
-Filename: xsl/support/play-button/README.md
+Filename: xsl/extract-qrcode.xsl
 Comment: 
 
-Filename: xsl/support/play-button/play-button.png
+Filename: xsl/latex/pretext-latex-CLP.xsl
 Comment: 
 
 Filename: xsl/latex/pretext-latex-dyslexic-font.xsl
 Comment: 
 
-Filename: xsl/latex/pretext-latex-guide.xsl
+Filename: xsl/latex/pretext-latex-AIM.xsl
 Comment: 
 
 Filename: xsl/latex/pretext-latex-chaos.xsl
 Comment: 
 
-Filename: xsl/latex/pretext-latex-AIM.xsl
+Filename: xsl/latex/pretext-latex-guide.xsl
 Comment: 
 
-Filename: xsl/latex/pretext-latex-CLP.xsl
+Filename: xsl/support/play-button/
 Comment: 
 
-Filename: schema/pretext.xml
+Filename: xsl/support/README.md
 Comment: 
 
-Filename: schema/pretext.xsd
+Filename: xsl/support/extract-math.xsl
 Comment: 
 
-Filename: schema/pretext-schematron.xsl
+Filename: xsl/support/pretext-pg-macros.xsl
 Comment: 
 
-Filename: schema/xml.xsd
+Filename: xsl/support/package-math.xsl
 Comment: 
 
-Filename: schema/pretext.rnc
+Filename: xsl/support/runestone-services.xml
 Comment: 
 
-Filename: schema/README.md
+Filename: xsl/support/tactile-svg.xsl
 Comment: 
 
-Filename: schema/build.sh
+Filename: xsl/support/extract-latex-image-labels.xsl
 Comment: 
 
-Filename: schema/pretext-dev.rng
+Filename: xsl/support/play-button/README.md
 Comment: 
 
-Filename: schema/pretext-validation-plus.xsl
+Filename: xsl/support/play-button/play-button.svg
 Comment: 
 
-Filename: schema/pretext-dev.rnc
+Filename: xsl/support/play-button/play-button.png
 Comment: 
 
-Filename: schema/pretext.rng
+Filename: xsl/localizations/es-ES.xml
 Comment: 
 
-Filename: css/colors_darkmartiansands.css
+Filename: xsl/localizations/hu-HU.xml
 Comment: 
 
-Filename: css/colors_pastel_blue_orange.css
+Filename: xsl/localizations/de-DE.xml
 Comment: 
 
-Filename: css/pretext_add_on.css
+Filename: xsl/localizations/fr-FR.xml
 Comment: 
 
-Filename: css/colors_green_blue.css
+Filename: xsl/localizations/fi-FI.xml
 Comment: 
 
-Filename: css/colors_green_plum.css
+Filename: xsl/localizations/README.md
 Comment: 
 
-Filename: css/colors_martiansands.css
+Filename: xsl/localizations/it-IT.xml
 Comment: 
 
-Filename: css/colors_orange_navy.css
+Filename: xsl/localizations/af-ZA.xml
 Comment: 
 
-Filename: css/colors_brown_gold.css
+Filename: xsl/localizations/ca-ES.xml
 Comment: 
 
-Filename: css/colors_blue_grey.css
+Filename: xsl/localizations/en-US.xml
 Comment: 
 
-Filename: css/colors_ruby_turquoise.css
+Filename: xsl/localizations/nl-NL.xml
 Comment: 
 
-Filename: css/style_oscarlevin.css
+Filename: xsl/localizations/localizations.xml
 Comment: 
 
-Filename: css/setcolors.css
+Filename: xsl/localizations/cs-CZ.xml
 Comment: 
 
-Filename: css/README.md
+Filename: xsl/localizations/bg-BG.xml
 Comment: 
 
-Filename: css/update_css
+Filename: xsl/localizations/pt-PT.xml
 Comment: 
 
-Filename: css/colors_blue_green.css
+Filename: xsl/localizations/fr-CA.xml
 Comment: 
 
-Filename: css/colors_ruby_emerald.css
+Filename: xsl/localizations/pt-BR.xml
 Comment: 
 
-Filename: css/mathbook-content.css
+Filename: xsl/utilities/README.md
 Comment: 
 
-Filename: css/pretext.css
+Filename: xsl/utilities/fix-deprecations.xsl
 Comment: 
 
-Filename: css/colors_blue_red.css
+Filename: xsl/utilities/pretext-enhanced-source.xsl
 Comment: 
 
-Filename: css/colors_ruby_amethyst.css
+Filename: xsl/utilities/deprecate-autoname.sed
 Comment: 
 
-Filename: css/style_default.css
+Filename: xsl/utilities/author-report.xsl
 Comment: 
 
-Filename: css/epub.css
+Filename: xsl/utilities/deprecate-index.sed
 Comment: 
 
-Filename: css/colors_default.css
+Filename: css/colors_maroon_grey.css
+Comment: 
+
+Filename: css/style_default.css
 Comment: 
 
 Filename: css/style_soundwriting.css
 Comment: 
 
-Filename: css/mathbook-3.css
+Filename: css/mathbook-add-on.css
 Comment: 
 
-Filename: css/colors_red_blue.css
+Filename: css/README.md
 Comment: 
 
-Filename: css/kindle.css
+Filename: css/colors_brown_gold.css
 Comment: 
 
-Filename: css/mathbook-add-on.css
+Filename: css/colors_blue_red.css
 Comment: 
 
-Filename: css/colors_maroon_grey.css
+Filename: css/mathbook-3.css
 Comment: 
 
-Filename: script/braille/
+Filename: css/mathbook-content.css
 Comment: 
 
-Filename: script/mjsre/
+Filename: css/pretext.css
 Comment: 
 
-Filename: script/README.md
+Filename: css/colors_green_plum.css
 Comment: 
 
-Filename: script/mbx
+Filename: css/colors_ruby_turquoise.css
 Comment: 
 
-Filename: script/braille/pretext-symbol.dis
+Filename: css/colors_blue_green.css
 Comment: 
 
-Filename: script/braille/pretext.sem
+Filename: css/pretext_add_on.css
 Comment: 
 
-Filename: script/braille/README.md
+Filename: css/colors_default.css
 Comment: 
 
-Filename: script/braille/pretext-liblouis.cfg
+Filename: css/colors_blue_grey.css
 Comment: 
 
-Filename: script/braille/pretext-liblouis-emboss.cfg
+Filename: css/colors_green_blue.css
 Comment: 
 
-Filename: script/braille/pretext-liblouis-electronic.cfg
+Filename: css/colors_darkmartiansands.css
 Comment: 
 
-Filename: script/mjsre/README.md
+Filename: css/colors_orange_navy.css
 Comment: 
 
-Filename: script/mjsre/update-sre
+Filename: css/style_oscarlevin.css
 Comment: 
 
-Filename: script/mjsre/mj-sre-page.js
+Filename: css/colors_pastel_blue_orange.css
 Comment: 
 
-Filename: script/mjsre/package.json
+Filename: css/colors_red_blue.css
 Comment: 
 
-Filename: pretext/pretext.cfg
+Filename: css/setcolors.css
 Comment: 
 
-Filename: pretext/README.md
+Filename: css/colors_ruby_amethyst.css
 Comment: 
 
-Filename: pretext/pretext.py
+Filename: css/colors_martiansands.css
 Comment: 
 
-Filename: pretext/braille_format.py
+Filename: css/epub.css
 Comment: 
 
-Filename: pretext/__init__.py
+Filename: css/kindle.css
 Comment: 
 
-Filename: pretext/module-test.py
+Filename: css/colors_ruby_emerald.css
 Comment: 
 
-Filename: pretext/pretext
+Filename: css/update_css
 Comment: 
 
 Zip file comment:
```

#### xsl/pretext-braille-preprint.xsl

##### xsl/pretext-braille-preprint.xsl

```diff
@@ -251,14 +251,22 @@
       <xsl:if test="//sbsgroup">
         <xsl:apply-templates select="." mode="transcriber-note">
           <xsl:with-param name="message">
             <xsl:text>A &quot;side-by-side group&quot; is a sequence down the page of &quot;side-by-side&quot; (see previous note).  We announce the start with the number of side-by-side in the group to expect, and let the beginning and ending notes for each side-by-side delineate the sequence.</xsl:text>
           </xsl:with-param>
         </xsl:apply-templates>
       </xsl:if>
+      <!-- mention how "tabular" are implenented and suggest possible improvements-->
+      <xsl:if test="//tabular">
+        <xsl:apply-templates select="." mode="transcriber-note">
+          <xsl:with-param name="message">
+            <xsl:text>Tabular material is always implemented using a &quot;linear table format&quot;.  A human transcriber may be able to improve small tables, or larger tables that could use multiple pages when embossed, by using a different format.</xsl:text>
+          </xsl:with-param>
+        </xsl:apply-templates>
+      </xsl:if>
       <!-- process segments and blocks of "brf" -->
       <xsl:apply-templates select="*"/>
     </brf>
   </xsl:template>
   <!-- ######### -->
   <!-- Divisions -->
   <!-- ######### -->
@@ -646,14 +654,21 @@
       </xsl:apply-templates>
     </block>
   </xsl:template>
   <!-- Other FIGURE-LIKE can be handled together -->
   <xsl:template match="figure|listing|table|list">
     <block breakable="no" box="standard" lines-before="1" lines-after="1">
       <segment indentation="6" runover="4">
+        <!-- [BANA, 2016, 11.17.1a] "Leave a blank line after the title." -->
+        <!-- Guidance for tables, we mimic for PTX "list" block.          -->
+        <xsl:if test="self::table or self::list">
+          <xsl:attribute name="lines-after">
+            <xsl:text>1</xsl:text>
+          </xsl:attribute>
+        </xsl:if>
         <xsl:apply-templates select="." mode="block-title"/>
       </segment>
       <xsl:apply-templates/>
     </block>
   </xsl:template>
   <!-- Caption/title, with label, number, etc.  "caption" and -->
   <!-- "title" elements are metadata, killed in -common,      -->
@@ -845,14 +860,150 @@
       </xsl:when>
       <!-- a bad idea for Braille -->
       <xsl:when test="$format-code = 'none'">
         <xsl:text/>
       </xsl:when>
     </xsl:choose>
   </xsl:template>
+  <!-- ####################### -->
+  <!-- Tabular (table content) -->
+  <!-- ####################### -->
+  <!-- Simple tables can be realized nicely in braille by a human transcriber. -->
+  <!-- We are not even sure how to identify a table as being "simple enough."  -->
+  <!--                                                                         -->
+  <!-- So we implement "Wide Tables: Linear Table Format" [BANA, 2016, 11.17], -->
+  <!-- which is never wrong, and is more or less sympatico with our markup.    -->
+  <!--                                                                         -->
+  <!-- TODO: Suppose a transcriber *does* replace one of our tables with       -->
+  <!-- something better?  We could perhaps capture the BRF version in a new    -->
+  <!-- "braille" element that lived in source and which was used               -->
+  <!-- preferentially once discovered.                                         -->
+  <xsl:template match="tabular">
+    <xsl:variable name="n-column-headings" select="count(row[(@header = 'yes') or (@header = 'vertical')])"/>
+    <xsl:variable name="b-column-headings" select="$n-column-headings &gt; 0"/>
+    <xsl:variable name="b-row-headings" select="@row-headers = 'yes'"/>
+    <block breakable="no">
+      <!-- Transcriber note, if necessary to explain headings -->
+      <xsl:if test="$b-column-headings or $b-row-headings">
+        <xsl:apply-templates select="." mode="transcriber-note">
+          <xsl:with-param name="message">
+            <xsl:if test="$b-column-headings">
+              <xsl:text>The first</xsl:text>
+              <xsl:value-of select="$n-column-headings"/>
+              <xsl:text>rows are columm headings, described next.</xsl:text>
+            </xsl:if>
+            <!-- separate two sentences, if we have both -->
+            <xsl:if test="$b-column-headings and $b-row-headings">
+              <xsl:text/>
+            </xsl:if>
+            <xsl:if test="$b-row-headings">
+              <xsl:text>The first column of this table contains headings for the rows.</xsl:text>
+            </xsl:if>
+          </xsl:with-param>
+        </xsl:apply-templates>
+        <!-- [BANA, 2016] 11.17.1e "Leave a blank line after the note." -->
+        <segment lines-after="1"/>
+      </xsl:if>
+      <!-- enforce header row(s) first -->
+      <!-- BANA says put column headings inside the transcriber note, -->
+      <!-- but switch to 1-3 margins.  We ignore this and write the   -->
+      <!-- column headings out just tlike all the other rows.  One    -->
+      <!-- concession: a blank line separator.                        -->
+      <xsl:apply-templates select="row[(@header = 'yes') or (@header = 'vertical')]"/>
+      <xsl:if test="$b-column-headings">
+        <segment lines-after="1"/>
+      </xsl:if>
+      <!-- now the "regular" lines, possibly with row-headings -->
+      <xsl:apply-templates select="row[not((@header = 'yes') or (@header = 'vertical'))]"/>
+    </block>
+  </xsl:template>
+  <!-- [BANA, 2016] 11.17.1f Each row has 1-3 margins                     -->
+  <!-- [BANA, 2016] 11.17.1g "Do not divide a row between braille pages." -->
+  <xsl:template match="tabular/row">
+    <segment breakable="no" indentation="0" runover="2">
+      <xsl:choose>
+        <xsl:when test="(@header = 'yes') or (@header = 'vertical')">
+          <xsl:apply-templates select="cell[1]" mode="describe-column-headings"/>
+        </xsl:when>
+        <xsl:otherwise>
+          <xsl:apply-templates select="cell"/>
+        </xsl:otherwise>
+      </xsl:choose>
+    </segment>
+  </xsl:template>
+  <!-- "Regular" cells in non-header rows (more typical) -->
+  <xsl:template match="tabular/row/cell">
+    <xsl:apply-templates/>
+    <xsl:choose>
+      <!-- First cell, trailed by a colon -->
+      <xsl:when test="not(preceding-sibling::cell)">
+        <xsl:text>:</xsl:text>
+      </xsl:when>
+      <!-- Last cell, trailed by nothing -->
+      <xsl:when test="not(following-sibling::cell)"/>
+      <!-- Interior cells, trailed by semi-colons -->
+      <xsl:otherwise>
+        <xsl:text>;</xsl:text>
+      </xsl:otherwise>
+    </xsl:choose>
+    <xsl:if test="@colspan">
+      <xsl:call-template name="duplicate-string">
+        <xsl:with-param name="count" select="@colspan - 1"/>
+        <xsl:with-param name="text" select="';'"/>
+      </xsl:call-template>
+    </xsl:if>
+  </xsl:template>
+  <xsl:template match="tabular/row/cell" mode="describe-column-headings">
+    <xsl:param name="prior-column-number" select="0"/>
+    <!-- Analyze  @colspan  implications.  Note this is correct for -->
+    <!-- no attribute at all and a (silly) attribute value of 1.    -->
+    <xsl:variable name="first-column" select="$prior-column-number + 1"/>
+    <xsl:variable name="n-columns">
+      <xsl:choose>
+        <xsl:when test="@colspan">
+          <xsl:value-of select="@colspan"/>
+        </xsl:when>
+        <xsl:otherwise>
+          <xsl:text>1</xsl:text>
+        </xsl:otherwise>
+      </xsl:choose>
+    </xsl:variable>
+    <xsl:variable name="last-column" select="$prior-column-number + $n-columns"/>
+    <xsl:variable name="b-multicolumns" select="$last-column &gt; $first-column"/>
+    <xsl:text>Column</xsl:text>
+    <xsl:if test="$b-multicolumns">
+      <xsl:text>s</xsl:text>
+    </xsl:if>
+    <xsl:text/>
+    <xsl:value-of select="$first-column"/>
+    <xsl:if test="$b-multicolumns">
+      <xsl:text>-</xsl:text>
+      <xsl:value-of select="$last-column"/>
+    </xsl:if>
+    <xsl:text/>
+    <xsl:apply-templates/>
+    <xsl:choose>
+      <!-- First cell, trailed by a colon -->
+      <xsl:when test="not(preceding-sibling::cell)">
+        <xsl:text>:</xsl:text>
+      </xsl:when>
+      <!-- Last cell, trailed by nothing -->
+      <xsl:when test="not(following-sibling::cell)"/>
+      <!-- Interior cells, trailed by semi-colons -->
+      <xsl:otherwise>
+        <xsl:text>;</xsl:text>
+      </xsl:otherwise>
+    </xsl:choose>
+    <!-- recurse if there is more to do -->
+    <xsl:if test="following-sibling::cell">
+      <xsl:apply-templates select="following-sibling::cell" mode="describe-column-headings">
+        <xsl:with-param name="prior-column-number" select="$last-column"/>
+      </xsl:apply-templates>
+    </xsl:if>
+  </xsl:template>
   <!-- ########## -->
   <!-- References -->
   <!-- ########## -->
   <!-- Bibliography [BANA-2016, 22.2.1]                           -->
   <!-- Bibliographic items in a "references" division have a      -->
   <!-- bracketed number leading each new entry, then two spaces   -->
   <!-- of indentation for the remainder .                         -->
@@ -1262,18 +1413,14 @@
     </xsl:for-each>
   </xsl:template>
   <!-- segment with placeholder content at this stage -->
   <xsl:template match="cd">
     <segment>CODE DISPLAY</segment>
   </xsl:template>
   <!-- segment with placeholder content at this stage -->
-  <xsl:template match="tabular">
-    <segment>TABULAR</segment>
-  </xsl:template>
-  <!-- segment with placeholder content at this stage -->
   <xsl:template match="pre">
     <segment>PREFORMATTED TEXT</segment>
   </xsl:template>
   <!-- segment with placeholder content at this stage -->
   <xsl:template match="program">
     <segment>PROGRAM</segment>
   </xsl:template>
```

### Comparing `pretext-1.5.3.dev20230509/pretext/generate.py` & `pretext-1.5.3.dev20230510/pretext/generate.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230509/pretext/project.py` & `pretext-1.5.3.dev20230510/pretext/project.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230509/pretext/templates/__init__.py` & `pretext-1.5.3.dev20230510/pretext/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230509/pretext/templates/resources/.gitignore` & `pretext-1.5.3.dev20230510/pretext/templates/resources/.gitignore`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230509/pretext/templates/resources/article.zip` & `pretext-1.5.3.dev20230510/pretext/templates/resources/article.zip`

 * *Files 4% similar despite different names*

#### zipinfo {}

```diff
@@ -1,17 +1,17 @@
 Zip file size: 160171 bytes, number of entries: 15
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-09 06:19 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-09 06:18 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-09 06:18 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-09 06:18 source/
--rw-r--r--  2.0 unx     2268 b- defN 23-May-09 06:19 codechat_config.yaml
--rw-r--r--  2.0 unx       86 b- defN 23-May-09 06:18 README.md
--rw-r--r--  2.0 unx     1710 b- defN 23-May-09 06:19 project.ptx
--rw-r--r--  2.0 unx     1676 b- defN 23-May-09 06:19 .gitignore
--rw-r--r--  2.0 unx      242 b- defN 23-May-09 06:18 publication/publication.ptx
--rw-r--r--  2.0 unx   154806 b- defN 23-May-09 06:18 assets/frog.jpg
--rw-r--r--  2.0 unx      630 b- defN 23-May-09 06:19 .devcontainer/postCreateCommand.sh
--rw-r--r--  2.0 unx     1236 b- defN 23-May-09 06:19 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx      449 b- defN 23-May-09 06:18 source/section-1.ptx
--rw-r--r--  2.0 unx      982 b- defN 23-May-09 06:18 source/section-2.ptx
--rw-r--r--  2.0 unx      430 b- defN 23-May-09 06:18 source/main.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-10 06:18 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-10 06:18 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-10 06:18 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-10 06:18 source/
+-rw-r--r--  2.0 unx       86 b- defN 23-May-10 06:18 README.md
+-rw-r--r--  2.0 unx     1710 b- defN 23-May-10 06:18 project.ptx
+-rw-r--r--  2.0 unx     2268 b- defN 23-May-10 06:18 codechat_config.yaml
+-rw-r--r--  2.0 unx     1676 b- defN 23-May-10 06:18 .gitignore
+-rw-r--r--  2.0 unx   154806 b- defN 23-May-10 06:18 assets/frog.jpg
+-rw-r--r--  2.0 unx     1236 b- defN 23-May-10 06:18 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx      630 b- defN 23-May-10 06:18 .devcontainer/postCreateCommand.sh
+-rw-r--r--  2.0 unx      242 b- defN 23-May-10 06:18 publication/publication.ptx
+-rw-r--r--  2.0 unx      430 b- defN 23-May-10 06:18 source/main.ptx
+-rw-r--r--  2.0 unx      449 b- defN 23-May-10 06:18 source/section-1.ptx
+-rw-r--r--  2.0 unx      982 b- defN 23-May-10 06:18 source/section-2.ptx
 15 files, 164515 bytes uncompressed, 158505 bytes compressed:  3.7%
```

#### zipnote {}

```diff
@@ -6,41 +6,41 @@
 
 Filename: publication/
 Comment: 
 
 Filename: source/
 Comment: 
 
-Filename: codechat_config.yaml
-Comment: 
-
 Filename: README.md
 Comment: 
 
 Filename: project.ptx
 Comment: 
 
-Filename: .gitignore
+Filename: codechat_config.yaml
 Comment: 
 
-Filename: publication/publication.ptx
+Filename: .gitignore
 Comment: 
 
 Filename: assets/frog.jpg
 Comment: 
 
+Filename: .devcontainer/devcontainer.json
+Comment: 
+
 Filename: .devcontainer/postCreateCommand.sh
 Comment: 
 
-Filename: .devcontainer/devcontainer.json
+Filename: publication/publication.ptx
 Comment: 
 
-Filename: source/section-1.ptx
+Filename: source/main.ptx
 Comment: 
 
-Filename: source/section-2.ptx
+Filename: source/section-1.ptx
 Comment: 
 
-Filename: source/main.ptx
+Filename: source/section-2.ptx
 Comment: 
 
 Zip file comment:
```

### Comparing `pretext-1.5.3.dev20230509/pretext/templates/resources/book.zip` & `pretext-1.5.3.dev20230510/pretext/templates/resources/book.zip`

 * *Files 12% similar despite different names*

#### zipinfo {}

```diff
@@ -1,13 +1,13 @@
 Zip file size: 7677 bytes, number of entries: 11
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-09 06:19 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-09 06:18 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-09 06:18 source/
--rw-r--r--  2.0 unx     2268 b- defN 23-May-09 06:19 codechat_config.yaml
--rw-r--r--  2.0 unx       82 b- defN 23-May-09 06:18 README.md
--rw-r--r--  2.0 unx     1710 b- defN 23-May-09 06:19 project.ptx
--rw-r--r--  2.0 unx     1676 b- defN 23-May-09 06:19 .gitignore
--rw-r--r--  2.0 unx     6114 b- defN 23-May-09 06:18 publication/publication.ptx
--rw-r--r--  2.0 unx      630 b- defN 23-May-09 06:19 .devcontainer/postCreateCommand.sh
--rw-r--r--  2.0 unx     1236 b- defN 23-May-09 06:19 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx     1767 b- defN 23-May-09 06:18 source/main.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-10 06:18 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-10 06:18 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-10 06:18 source/
+-rw-r--r--  2.0 unx       82 b- defN 23-May-10 06:18 README.md
+-rw-r--r--  2.0 unx     1710 b- defN 23-May-10 06:18 project.ptx
+-rw-r--r--  2.0 unx     2268 b- defN 23-May-10 06:18 codechat_config.yaml
+-rw-r--r--  2.0 unx     1676 b- defN 23-May-10 06:18 .gitignore
+-rw-r--r--  2.0 unx     1236 b- defN 23-May-10 06:18 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx      630 b- defN 23-May-10 06:18 .devcontainer/postCreateCommand.sh
+-rw-r--r--  2.0 unx     6114 b- defN 23-May-10 06:18 publication/publication.ptx
+-rw-r--r--  2.0 unx     1767 b- defN 23-May-10 06:18 source/main.ptx
 11 files, 15483 bytes uncompressed, 6439 bytes compressed:  58.4%
```

#### zipnote {}

```diff
@@ -3,32 +3,32 @@
 
 Filename: publication/
 Comment: 
 
 Filename: source/
 Comment: 
 
-Filename: codechat_config.yaml
-Comment: 
-
 Filename: README.md
 Comment: 
 
 Filename: project.ptx
 Comment: 
 
+Filename: codechat_config.yaml
+Comment: 
+
 Filename: .gitignore
 Comment: 
 
-Filename: publication/publication.ptx
+Filename: .devcontainer/devcontainer.json
 Comment: 
 
 Filename: .devcontainer/postCreateCommand.sh
 Comment: 
 
-Filename: .devcontainer/devcontainer.json
+Filename: publication/publication.ptx
 Comment: 
 
 Filename: source/main.ptx
 Comment: 
 
 Zip file comment:
```

### Comparing `pretext-1.5.3.dev20230509/pretext/templates/resources/demo.zip` & `pretext-1.5.3.dev20230510/pretext/templates/resources/demo.zip`

 * *Files 7% similar despite different names*

#### zipinfo {}

```diff
@@ -1,37 +1,37 @@
 Zip file size: 173370 bytes, number of entries: 35
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-09 06:19 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-09 06:18 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-09 06:18 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-09 06:18 source/
--rw-r--r--  2.0 unx     2268 b- defN 23-May-09 06:19 codechat_config.yaml
--rw-r--r--  2.0 unx       82 b- defN 23-May-09 06:18 README.md
--rw-r--r--  2.0 unx     1710 b- defN 23-May-09 06:19 project.ptx
--rw-r--r--  2.0 unx     1676 b- defN 23-May-09 06:19 .gitignore
--rw-r--r--  2.0 unx     6092 b- defN 23-May-09 06:18 publication/publication.ptx
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-09 06:18 assets/jsxgraph/
--rw-r--r--  2.0 unx   154806 b- defN 23-May-09 06:18 assets/frog.jpg
--rw-r--r--  2.0 unx     1737 b- defN 23-May-09 06:18 assets/jsxgraph/infinity.js
--rw-r--r--  2.0 unx      630 b- defN 23-May-09 06:19 .devcontainer/postCreateCommand.sh
--rw-r--r--  2.0 unx     1236 b- defN 23-May-09 06:19 .devcontainer/devcontainer.json
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-09 06:18 source/images/
--rw-r--r--  2.0 unx      339 b- defN 23-May-09 06:18 source/ch-features.ptx
--rw-r--r--  2.0 unx     3036 b- defN 23-May-09 06:18 source/ch-generate.ptx
--rw-r--r--  2.0 unx     2080 b- defN 23-May-09 06:18 source/frontmatter.ptx
--rw-r--r--  2.0 unx      867 b- defN 23-May-09 06:18 source/sec-features.ptx
--rw-r--r--  2.0 unx      847 b- defN 23-May-09 06:18 source/sec-first-intro.ptx
--rw-r--r--  2.0 unx      230 b- defN 23-May-09 06:18 source/ch-empty.ptx
--rw-r--r--  2.0 unx      375 b- defN 23-May-09 06:18 source/fig-sage2d.ptx
--rw-r--r--  2.0 unx      335 b- defN 23-May-09 06:18 source/fig-asymptote.ptx
--rw-r--r--  2.0 unx     1616 b- defN 23-May-09 06:18 source/docinfo.ptx
--rw-r--r--  2.0 unx     1515 b- defN 23-May-09 06:18 source/ex-first.ptx
--rw-r--r--  2.0 unx      885 b- defN 23-May-09 06:18 source/backmatter.ptx
--rw-r--r--  2.0 unx     2517 b- defN 23-May-09 06:18 source/main.ptx
--rw-r--r--  2.0 unx     1697 b- defN 23-May-09 06:18 source/sec-first-examples.ptx
--rw-r--r--  2.0 unx      381 b- defN 23-May-09 06:18 source/fig-tikz.ptx
--rw-r--r--  2.0 unx      411 b- defN 23-May-09 06:18 source/fig-sage3d.ptx
--rw-r--r--  2.0 unx     1115 b- defN 23-May-09 06:18 source/ch-first with spaces.ptx
--rw-r--r--  2.0 unx      835 b- defN 23-May-09 06:18 source/images/cflag.asy
--rw-r--r--  2.0 unx      357 b- defN 23-May-09 06:18 source/images/tikz.tex
--rw-r--r--  2.0 unx       93 b- defN 23-May-09 06:18 source/images/sageplot3d.sage
--rw-r--r--  2.0 unx       10 b- defN 23-May-09 06:18 source/images/sageplot2d.sage
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-10 06:18 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-10 06:18 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-10 06:18 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-10 06:18 source/
+-rw-r--r--  2.0 unx       82 b- defN 23-May-10 06:18 README.md
+-rw-r--r--  2.0 unx     1710 b- defN 23-May-10 06:18 project.ptx
+-rw-r--r--  2.0 unx     2268 b- defN 23-May-10 06:18 codechat_config.yaml
+-rw-r--r--  2.0 unx     1676 b- defN 23-May-10 06:18 .gitignore
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-10 06:18 assets/jsxgraph/
+-rw-r--r--  2.0 unx   154806 b- defN 23-May-10 06:18 assets/frog.jpg
+-rw-r--r--  2.0 unx     1737 b- defN 23-May-10 06:18 assets/jsxgraph/infinity.js
+-rw-r--r--  2.0 unx     1236 b- defN 23-May-10 06:18 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx      630 b- defN 23-May-10 06:18 .devcontainer/postCreateCommand.sh
+-rw-r--r--  2.0 unx     6092 b- defN 23-May-10 06:18 publication/publication.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-10 06:18 source/images/
+-rw-r--r--  2.0 unx      847 b- defN 23-May-10 06:18 source/sec-first-intro.ptx
+-rw-r--r--  2.0 unx     2517 b- defN 23-May-10 06:18 source/main.ptx
+-rw-r--r--  2.0 unx     1697 b- defN 23-May-10 06:18 source/sec-first-examples.ptx
+-rw-r--r--  2.0 unx      375 b- defN 23-May-10 06:18 source/fig-sage2d.ptx
+-rw-r--r--  2.0 unx      381 b- defN 23-May-10 06:18 source/fig-tikz.ptx
+-rw-r--r--  2.0 unx      411 b- defN 23-May-10 06:18 source/fig-sage3d.ptx
+-rw-r--r--  2.0 unx      335 b- defN 23-May-10 06:18 source/fig-asymptote.ptx
+-rw-r--r--  2.0 unx     2080 b- defN 23-May-10 06:18 source/frontmatter.ptx
+-rw-r--r--  2.0 unx      339 b- defN 23-May-10 06:18 source/ch-features.ptx
+-rw-r--r--  2.0 unx     3036 b- defN 23-May-10 06:18 source/ch-generate.ptx
+-rw-r--r--  2.0 unx      867 b- defN 23-May-10 06:18 source/sec-features.ptx
+-rw-r--r--  2.0 unx      885 b- defN 23-May-10 06:18 source/backmatter.ptx
+-rw-r--r--  2.0 unx     1115 b- defN 23-May-10 06:18 source/ch-first with spaces.ptx
+-rw-r--r--  2.0 unx      230 b- defN 23-May-10 06:18 source/ch-empty.ptx
+-rw-r--r--  2.0 unx     1515 b- defN 23-May-10 06:18 source/ex-first.ptx
+-rw-r--r--  2.0 unx     1616 b- defN 23-May-10 06:18 source/docinfo.ptx
+-rw-r--r--  2.0 unx       10 b- defN 23-May-10 06:18 source/images/sageplot2d.sage
+-rw-r--r--  2.0 unx      835 b- defN 23-May-10 06:18 source/images/cflag.asy
+-rw-r--r--  2.0 unx      357 b- defN 23-May-10 06:18 source/images/tikz.tex
+-rw-r--r--  2.0 unx       93 b- defN 23-May-10 06:18 source/images/sageplot3d.sage
 35 files, 189778 bytes uncompressed, 169270 bytes compressed:  10.8%
```

#### zipnote {}

```diff
@@ -6,101 +6,101 @@
 
 Filename: publication/
 Comment: 
 
 Filename: source/
 Comment: 
 
-Filename: codechat_config.yaml
-Comment: 
-
 Filename: README.md
 Comment: 
 
 Filename: project.ptx
 Comment: 
 
-Filename: .gitignore
+Filename: codechat_config.yaml
 Comment: 
 
-Filename: publication/publication.ptx
+Filename: .gitignore
 Comment: 
 
 Filename: assets/jsxgraph/
 Comment: 
 
 Filename: assets/frog.jpg
 Comment: 
 
 Filename: assets/jsxgraph/infinity.js
 Comment: 
 
+Filename: .devcontainer/devcontainer.json
+Comment: 
+
 Filename: .devcontainer/postCreateCommand.sh
 Comment: 
 
-Filename: .devcontainer/devcontainer.json
+Filename: publication/publication.ptx
 Comment: 
 
 Filename: source/images/
 Comment: 
 
-Filename: source/ch-features.ptx
+Filename: source/sec-first-intro.ptx
 Comment: 
 
-Filename: source/ch-generate.ptx
+Filename: source/main.ptx
 Comment: 
 
-Filename: source/frontmatter.ptx
+Filename: source/sec-first-examples.ptx
 Comment: 
 
-Filename: source/sec-features.ptx
+Filename: source/fig-sage2d.ptx
 Comment: 
 
-Filename: source/sec-first-intro.ptx
+Filename: source/fig-tikz.ptx
 Comment: 
 
-Filename: source/ch-empty.ptx
+Filename: source/fig-sage3d.ptx
 Comment: 
 
-Filename: source/fig-sage2d.ptx
+Filename: source/fig-asymptote.ptx
 Comment: 
 
-Filename: source/fig-asymptote.ptx
+Filename: source/frontmatter.ptx
 Comment: 
 
-Filename: source/docinfo.ptx
+Filename: source/ch-features.ptx
 Comment: 
 
-Filename: source/ex-first.ptx
+Filename: source/ch-generate.ptx
+Comment: 
+
+Filename: source/sec-features.ptx
 Comment: 
 
 Filename: source/backmatter.ptx
 Comment: 
 
-Filename: source/main.ptx
+Filename: source/ch-first with spaces.ptx
 Comment: 
 
-Filename: source/sec-first-examples.ptx
+Filename: source/ch-empty.ptx
 Comment: 
 
-Filename: source/fig-tikz.ptx
+Filename: source/ex-first.ptx
 Comment: 
 
-Filename: source/fig-sage3d.ptx
+Filename: source/docinfo.ptx
 Comment: 
 
-Filename: source/ch-first with spaces.ptx
+Filename: source/images/sageplot2d.sage
 Comment: 
 
 Filename: source/images/cflag.asy
 Comment: 
 
 Filename: source/images/tikz.tex
 Comment: 
 
 Filename: source/images/sageplot3d.sage
 Comment: 
 
-Filename: source/images/sageplot2d.sage
-Comment: 
-
 Zip file comment:
```

### Comparing `pretext-1.5.3.dev20230509/pretext/templates/resources/devcontainer.json` & `pretext-1.5.3.dev20230510/pretext/templates/resources/devcontainer.json`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230509/pretext/templates/resources/hello.zip` & `pretext-1.5.3.dev20230510/pretext/templates/resources/hello.zip`

 * *Files 13% similar despite different names*

#### zipinfo {}

```diff
@@ -1,13 +1,13 @@
 Zip file size: 4718 bytes, number of entries: 11
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-09 06:19 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-09 06:18 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-09 06:18 source/
--rw-r--r--  2.0 unx     2268 b- defN 23-May-09 06:19 codechat_config.yaml
--rw-r--r--  2.0 unx       69 b- defN 23-May-09 06:18 README.md
--rw-r--r--  2.0 unx     1217 b- defN 23-May-09 06:18 project.ptx
--rw-r--r--  2.0 unx     1676 b- defN 23-May-09 06:19 .gitignore
--rw-r--r--  2.0 unx      242 b- defN 23-May-09 06:18 publication/publication.ptx
--rw-r--r--  2.0 unx      630 b- defN 23-May-09 06:19 .devcontainer/postCreateCommand.sh
--rw-r--r--  2.0 unx     1236 b- defN 23-May-09 06:19 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx      156 b- defN 23-May-09 06:18 source/main.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-10 06:18 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-10 06:18 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-10 06:18 source/
+-rw-r--r--  2.0 unx       69 b- defN 23-May-10 06:18 README.md
+-rw-r--r--  2.0 unx     1217 b- defN 23-May-10 06:18 project.ptx
+-rw-r--r--  2.0 unx     2268 b- defN 23-May-10 06:18 codechat_config.yaml
+-rw-r--r--  2.0 unx     1676 b- defN 23-May-10 06:18 .gitignore
+-rw-r--r--  2.0 unx     1236 b- defN 23-May-10 06:18 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx      630 b- defN 23-May-10 06:18 .devcontainer/postCreateCommand.sh
+-rw-r--r--  2.0 unx      242 b- defN 23-May-10 06:18 publication/publication.ptx
+-rw-r--r--  2.0 unx      156 b- defN 23-May-10 06:18 source/main.ptx
 11 files, 7494 bytes uncompressed, 3480 bytes compressed:  53.6%
```

#### zipnote {}

```diff
@@ -3,32 +3,32 @@
 
 Filename: publication/
 Comment: 
 
 Filename: source/
 Comment: 
 
-Filename: codechat_config.yaml
-Comment: 
-
 Filename: README.md
 Comment: 
 
 Filename: project.ptx
 Comment: 
 
+Filename: codechat_config.yaml
+Comment: 
+
 Filename: .gitignore
 Comment: 
 
-Filename: publication/publication.ptx
+Filename: .devcontainer/devcontainer.json
 Comment: 
 
 Filename: .devcontainer/postCreateCommand.sh
 Comment: 
 
-Filename: .devcontainer/devcontainer.json
+Filename: publication/publication.ptx
 Comment: 
 
 Filename: source/main.ptx
 Comment: 
 
 Zip file comment:
```

### Comparing `pretext-1.5.3.dev20230509/pretext/templates/resources/postCreateCommand.sh` & `pretext-1.5.3.dev20230510/pretext/templates/resources/postCreateCommand.sh`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230509/pretext/templates/resources/project.ptx` & `pretext-1.5.3.dev20230510/pretext/templates/resources/project.ptx`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230509/pretext/templates/resources/slideshow.zip` & `pretext-1.5.3.dev20230510/pretext/templates/resources/slideshow.zip`

 * *Files 9% similar despite different names*

#### zipinfo {}

```diff
@@ -1,14 +1,14 @@
 Zip file size: 8453 bytes, number of entries: 12
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-09 06:19 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-09 06:18 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-09 06:18 source/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-09 06:18 xsl/
--rw-r--r--  2.0 unx     2268 b- defN 23-May-09 06:19 codechat_config.yaml
--rw-r--r--  2.0 unx      784 b- defN 23-May-09 06:18 project.ptx
--rw-r--r--  2.0 unx     1676 b- defN 23-May-09 06:19 .gitignore
--rw-r--r--  2.0 unx      190 b- defN 23-May-09 06:18 xsl/slides.xsl
--rw-r--r--  2.0 unx     2097 b- defN 23-May-09 06:18 publication/publication.ptx
--rw-r--r--  2.0 unx      630 b- defN 23-May-09 06:19 .devcontainer/postCreateCommand.sh
--rw-r--r--  2.0 unx     1236 b- defN 23-May-09 06:19 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx    11200 b- defN 23-May-09 06:18 source/main.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-10 06:18 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-10 06:18 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-10 06:18 source/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-10 06:18 xsl/
+-rw-r--r--  2.0 unx      784 b- defN 23-May-10 06:18 project.ptx
+-rw-r--r--  2.0 unx     2268 b- defN 23-May-10 06:18 codechat_config.yaml
+-rw-r--r--  2.0 unx     1676 b- defN 23-May-10 06:18 .gitignore
+-rw-r--r--  2.0 unx     1236 b- defN 23-May-10 06:18 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx      630 b- defN 23-May-10 06:18 .devcontainer/postCreateCommand.sh
+-rw-r--r--  2.0 unx      190 b- defN 23-May-10 06:18 xsl/slides.xsl
+-rw-r--r--  2.0 unx     2097 b- defN 23-May-10 06:18 publication/publication.ptx
+-rw-r--r--  2.0 unx    11200 b- defN 23-May-10 06:18 source/main.ptx
 12 files, 20081 bytes uncompressed, 7121 bytes compressed:  64.5%
```

#### zipnote {}

```diff
@@ -6,32 +6,32 @@
 
 Filename: source/
 Comment: 
 
 Filename: xsl/
 Comment: 
 
-Filename: codechat_config.yaml
+Filename: project.ptx
 Comment: 
 
-Filename: project.ptx
+Filename: codechat_config.yaml
 Comment: 
 
 Filename: .gitignore
 Comment: 
 
-Filename: xsl/slides.xsl
+Filename: .devcontainer/devcontainer.json
 Comment: 
 
-Filename: publication/publication.ptx
+Filename: .devcontainer/postCreateCommand.sh
 Comment: 
 
-Filename: .devcontainer/postCreateCommand.sh
+Filename: xsl/slides.xsl
 Comment: 
 
-Filename: .devcontainer/devcontainer.json
+Filename: publication/publication.ptx
 Comment: 
 
 Filename: source/main.ptx
 Comment: 
 
 Zip file comment:
```

### Comparing `pretext-1.5.3.dev20230509/pretext/utils.py` & `pretext-1.5.3.dev20230510/pretext/utils.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230509/pyproject.toml` & `pretext-1.5.3.dev20230510/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pretext"
-version = "1.5.3.dev20230509"
+version = "1.5.3.dev20230510"
 description = "A package to author, build, and deploy PreTeXt projects."
 readme = "README.md"
 homepage = "https://pretextbook.org"
 repository = "https://github.com/PreTeXtBook/pretext-cli"
 authors = ["Oscar Levin <oscar.levin@unco.edu>", "Steven Clontz <steven.clontz@gmail.com>",]
 license = "GPL-3.0-or-later"
 include = [
```

### Comparing `pretext-1.5.3.dev20230509/PKG-INFO` & `pretext-1.5.3.dev20230510/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretext
-Version: 1.5.3.dev20230509
+Version: 1.5.3.dev20230510
 Summary: A package to author, build, and deploy PreTeXt projects.
 Home-page: https://pretextbook.org
 License: GPL-3.0-or-later
 Author: Oscar Levin
 Author-email: oscar.levin@unco.edu
 Requires-Python: >=3.8.5,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

