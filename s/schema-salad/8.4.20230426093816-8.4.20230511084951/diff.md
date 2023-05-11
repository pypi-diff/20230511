# Comparing `tmp/schema-salad-8.4.20230426093816.tar.gz` & `tmp/schema-salad-8.4.20230511084951.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schema-salad-8.4.20230426093816.tar", last modified: Wed Apr 26 10:11:35 2023, max compression
+gzip compressed data, was "schema-salad-8.4.20230511084951.tar", last modified: Thu May 11 15:28:58 2023, max compression
```

## Comparing `schema-salad-8.4.20230426093816.tar` & `schema-salad-8.4.20230511084951.tar`

### file list

```diff
@@ -1,450 +1,450 @@
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.387567 schema-salad-8.4.20230426093816/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.323566 schema-salad-8.4.20230426093816/.circleci/
--rw-r--r--   0 michael   (1000) michael   (1000)     3370 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/.circleci/config.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      324 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/.coveragerc
--rw-r--r--   0 michael   (1000) michael   (1000)      304 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/.dockerignore
--rw-r--r--   0 michael   (1000) michael   (1000)      282 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/.flake8
--rw-r--r--   0 michael   (1000) michael   (1000)      229 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/.git-blame-ignore-revs
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.323566 schema-salad-8.4.20230426093816/.github/
--rw-r--r--   0 michael   (1000) michael   (1000)      603 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/.github/dependabot.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.323566 schema-salad-8.4.20230426093816/.github/workflows/
--rw-r--r--   0 michael   (1000) michael   (1000)     3859 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/.github/workflows/ci-tests.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      835 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     1090 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/.github/workflows/quay-publish.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      169 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/.github/workflows/wheel-prep.sh
--rw-r--r--   0 michael   (1000) michael   (1000)     5664 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/.github/workflows/wheels.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      219 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/.gitignore
--rw-r--r--   0 michael   (1000) michael   (1000)      113 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/.isort.cfg
--rw-r--r--   0 michael   (1000) michael   (1000)      585 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/.mergify.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    21223 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/.pylintrc
--rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/.readthedocs.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     1643 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/CONTRIBUTING.md
--rw-r--r--   0 michael   (1000) michael   (1000)    11358 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/LICENSE.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      680 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/MANIFEST.in
--rw-r--r--   0 michael   (1000) michael   (1000)     8324 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/Makefile
--rw-r--r--   0 michael   (1000) michael   (1000)    15861 2023-04-26 10:11:35.387567 schema-salad-8.4.20230426093816/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)    14703 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/README.rst
--rwxr-xr-x   0 michael   (1000) michael   (1000)      438 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/build-schema_salad-docker.sh
--rw-r--r--   0 michael   (1000) michael   (1000)      209 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/dev-requirements.txt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.323566 schema-salad-8.4.20230426093816/docs/
--rw-r--r--   0 michael   (1000) michael   (1000)      634 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/docs/Makefile
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.323566 schema-salad-8.4.20230426093816/docs/_static/
--rw-r--r--   0 michael   (1000) michael   (1000)    15086 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/docs/_static/favicon.ico
--rw-r--r--   0 michael   (1000) michael   (1000)      200 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/docs/cli.rst
--rw-r--r--   0 michael   (1000) michael   (1000)     3461 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/docs/conf.py
--rw-r--r--   0 michael   (1000) michael   (1000)      220 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/docs/index.rst
--rw-r--r--   0 michael   (1000) michael   (1000)      795 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/docs/make.bat
--rw-r--r--   0 michael   (1000) michael   (1000)      656 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/docs/typeshed.rst
--rw-r--r--   0 michael   (1000) michael   (1000)      325 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/lgtm.yml
--rwxr-xr-x   0 michael   (1000) michael   (1000)      819 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/manual_wheel_publish.sh
--rw-r--r--   0 michael   (1000) michael   (1000)       99 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-requirements.txt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.315565 schema-salad-8.4.20230426093816/mypy-stubs/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.323566 schema-salad-8.4.20230426093816/mypy-stubs/cachecontrol/
--rw-r--r--   0 michael   (1000) michael   (1000)      219 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/cachecontrol/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      226 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/cachecontrol/cache.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.327566 schema-salad-8.4.20230426093816/mypy-stubs/cachecontrol/caches/
--rw-r--r--   0 michael   (1000) michael   (1000)      273 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/cachecontrol/caches/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      873 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/cachecontrol/caches/file_cache.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      169 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/cachecontrol/compat.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      470 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/cachecontrol/controller.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      532 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/cachecontrol/wrapper.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.327566 schema-salad-8.4.20230426093816/mypy-stubs/mistune/
--rw-r--r--   0 michael   (1000) michael   (1000)      922 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/mistune/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      168 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/mistune/_types.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     5480 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/mistune/block_parser.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     2848 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/mistune/inline_parser.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1535 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/mistune/markdown.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.327566 schema-salad-8.4.20230426093816/mypy-stubs/mistune/plugins/
--rw-r--r--   0 michael   (1000) michael   (1000)      458 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/mistune/plugins/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      566 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/mistune/plugins/table.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     4159 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/mistune/renderers.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1870 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/mistune/scanner.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      191 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/mistune/util.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.327566 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/
--rw-r--r--   0 michael   (1000) michael   (1000)     1292 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      674 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/collection.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      231 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/compare.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      182 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/exceptions.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     8337 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/graph.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.331566 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/
--rw-r--r--   0 michael   (1000) michael   (1000)     2010 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_CSVW.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_DC.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1034 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_DCAT.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     2361 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_DCTERMS.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1109 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_DOAP.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1847 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_FOAF.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     4691 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_ODRL2.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1259 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_ORG.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     2260 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_OWL.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      441 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_PROF.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     4520 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_PROV.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1105 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_QB.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      620 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_RDF.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      519 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_RDFS.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)    41401 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_SDO.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     4965 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_SH.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      943 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_SKOS.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1075 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_SOSA.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      680 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_SSN.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     2462 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_TIME.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      927 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_VOID.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1742 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_XSD.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     2282 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      131 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/parser.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      724 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/paths.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      893 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/plugin.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.331566 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/plugins/
--rw-r--r--   0 michael   (1000) michael   (1000)      118 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/plugins/__init__.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.331566 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/plugins/parsers/
--rw-r--r--   0 michael   (1000) michael   (1000)      126 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/plugins/parsers/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)       34 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/plugins/parsers/notation3.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1354 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/query.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1370 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/resource.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1337 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/term.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      115 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/util.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.335566 schema-salad-8.4.20230426093816/mypy-stubs/ruamel/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/ruamel/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)      137 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy.ini
--rw-r--r--   0 michael   (1000) michael   (1000)     1061 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/pyproject.toml
--rwxr-xr-x   0 michael   (1000) michael   (1000)     3512 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/release-test.sh
--rw-r--r--   0 michael   (1000) michael   (1000)      292 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/requirements.txt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.339566 schema-salad-8.4.20230426093816/schema_salad/
--rw-r--r--   0 michael   (1000) michael   (1000)      395 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)      110 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/__main__.py
--rw-r--r--   0 michael   (1000) michael   (1000)      186 2023-04-26 10:11:35.000000 schema-salad-8.4.20230426093816/schema_salad/_version.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.339566 schema-salad-8.4.20230426093816/schema_salad/avro/
--rw-r--r--   0 michael   (1000) michael   (1000)    11359 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/avro/LICENSE
--rw-r--r--   0 michael   (1000) michael   (1000)      166 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/avro/NOTICE
--rw-r--r--   0 michael   (1000) michael   (1000)      802 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/avro/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    23815 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/avro/schema.py
--rw-r--r--   0 michael   (1000) michael   (1000)     7237 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/codegen.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4412 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/codegen_base.py
--rw-r--r--   0 michael   (1000) michael   (1000)    19604 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/cpp_codegen.py
--rw-r--r--   0 michael   (1000) michael   (1000)    10930 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dlang_codegen.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.339566 schema-salad-8.4.20230426093816/schema_salad/dotnet/
--rw-r--r--   0 michael   (1000) michael   (1000)       82 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/AssemblyInfo.cs
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.343566 schema-salad-8.4.20230426093816/schema_salad/dotnet/DocFx/
--rw-r--r--   0 michael   (1000) michael   (1000)      445 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/DocFx/filterConfig.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       22 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/DocFx/index.md
--rw-r--r--   0 michael   (1000) michael   (1000)       71 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/DocFx/toc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    11356 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/LICENSE
--rw-r--r--   0 michael   (1000) michael   (1000)     1442 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/Project.csproj.template
--rw-r--r--   0 michael   (1000) michael   (1000)       40 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1788 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/Solution.sln
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.343566 schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.343566 schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/data/
--rw-r--r--   0 michael   (1000) michael   (1000)        4 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/data/test.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      333 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/runsettings.xml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.343566 schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/
--rw-r--r--   0 michael   (1000) michael   (1000)      207 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/ExampleTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     2173 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/FetcherTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1151 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/UtilitiesTests.cs
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.343566 schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/loaders/
--rw-r--r--   0 michael   (1000) michael   (1000)     1027 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/loaders/AnyLoaderTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1321 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/loaders/ArrayLoaderTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     2429 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/loaders/EnumLoaderTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      749 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/loaders/ExpressionLoaderTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1742 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/loaders/IdMapLoaderTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      766 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/loaders/NullLoaderTests.cs
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.343566 schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/
--rw-r--r--   0 michael   (1000) michael   (1000)     1435 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderDoubleTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1431 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderFloatTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1393 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderIntTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1246 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderStringTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1087 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/loaders/UnionLoaderTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1188 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/Test.csproj.template
--rw-r--r--   0 michael   (1000) michael   (1000)     1459 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/docfx.json
--rw-r--r--   0 michael   (1000) michael   (1000)    11383 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/editorconfig
--rw-r--r--   0 michael   (1000) michael   (1000)     6894 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/gitignore
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.347566 schema-salad-8.4.20230426093816/schema_salad/dotnet/util/
--rw-r--r--   0 michael   (1000) michael   (1000)     2262 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Fetcher.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      167 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/util/LoaderInstances.cs
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.347566 schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/
--rw-r--r--   0 michael   (1000) michael   (1000)      338 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/AnyLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1754 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/ArrayLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      905 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/EnumLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      646 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/ExpressionLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     2168 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/IdMapLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     4481 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/Loader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      362 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/NullLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      745 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/PrimitiveLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      734 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/RecordLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1674 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/RootLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     3984 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/SecondaryDSLLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     3056 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/TypeDSLLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      793 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/UnionLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1656 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/UriLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     5215 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/util/LoadingOptions.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     4595 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Saveable.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1490 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/util/ScalarNodeTypeResolver.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      501 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/util/UriExtensions.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1624 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Utilities.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1913 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/util/ValidationException.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      264 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Vocabs.cs
--rw-r--r--   0 michael   (1000) michael   (1000)    33304 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet_codegen.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4175 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/exceptions.py
--rw-r--r--   0 michael   (1000) michael   (1000)     8025 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/fetcher.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.347566 schema-salad-8.4.20230426093816/schema_salad/java/
--rw-r--r--   0 michael   (1000) michael   (1000)       61 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/MANIFEST.MF
--rw-r--r--   0 michael   (1000) michael   (1000)      993 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)        8 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/gitignore
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.355566 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/
--rw-r--r--   0 michael   (1000) michael   (1000)      335 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/AnyLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)     1248 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/ArrayLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)      296 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/ConstantMaps.java
--rw-r--r--   0 michael   (1000) michael   (1000)     1521 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/DefaultFetcher.java
--rw-r--r--   0 michael   (1000) michael   (1000)      984 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/EnumLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)      416 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/ExpressionLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)      186 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/Fetcher.java
--rw-r--r--   0 michael   (1000) michael   (1000)     1697 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/IdMapLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)     4613 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/Loader.java
--rw-r--r--   0 michael   (1000) michael   (1000)      125 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/LoaderInstances.java
--rw-r--r--   0 michael   (1000) michael   (1000)     3815 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/LoadingOptions.java
--rw-r--r--   0 michael   (1000) michael   (1000)     1944 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/LoadingOptionsBuilder.java
--rw-r--r--   0 michael   (1000) michael   (1000)      332 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/NullLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)     1113 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/OneOrListOf.java
--rw-r--r--   0 michael   (1000) michael   (1000)     1050 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/OneOrListOfLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)      543 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/OptionalLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)      384 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/PrimitiveLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)     1175 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/RecordLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)     3734 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/RootLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)      180 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/Saveable.java
--rw-r--r--   0 michael   (1000) michael   (1000)      177 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/SaveableImpl.java
--rw-r--r--   0 michael   (1000) michael   (1000)     3035 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/SecondaryFilesDslLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)     2555 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/TypeDslLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)      866 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/UnionLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)     1511 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/UriLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)     3293 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/Uris.java
--rw-r--r--   0 michael   (1000) michael   (1000)     2254 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/ValidationException.java
--rw-r--r--   0 michael   (1000) michael   (1000)      789 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/Validator.java
--rw-r--r--   0 michael   (1000) michael   (1000)     1025 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/YamlUtils.java
--rw-r--r--   0 michael   (1000) michael   (1000)      131 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/package.html
--rw-r--r--   0 michael   (1000) michael   (1000)      237 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/overview.html
--rw-r--r--   0 michael   (1000) michael   (1000)      187 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/package.html
--rw-r--r--   0 michael   (1000) michael   (1000)     5467 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/pom.xml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.355566 schema-salad-8.4.20230426093816/schema_salad/java/test_utils/
--rw-r--r--   0 michael   (1000) michael   (1000)     1347 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/test_utils/DefaultFetcherTest.java
--rw-r--r--   0 michael   (1000) michael   (1000)       74 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/test_utils/ExamplesTest.java
--rw-r--r--   0 michael   (1000) michael   (1000)     1134 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/test_utils/ShortnameTest.java
--rw-r--r--   0 michael   (1000) michael   (1000)      402 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/test_utils/YamlUtilsTest.java
--rw-r--r--   0 michael   (1000) michael   (1000)    32358 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java_codegen.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     8476 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/jsonld_context.py
--rw-r--r--   0 michael   (1000) michael   (1000)    14154 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/main.py
--rw-r--r--   0 michael   (1000) michael   (1000)    33109 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/makedoc.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.359567 schema-salad-8.4.20230426093816/schema_salad/metaschema/
--rw-r--r--   0 michael   (1000) michael   (1000)     1327 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/field_name.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/field_name_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      283 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/field_name_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/field_name_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2442 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/ident_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/ident_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      473 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/ident_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      437 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/ident_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     3322 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/import_include.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1804 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/link_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      411 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/link_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      264 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/link_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      313 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/link_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      932 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/map_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      183 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/map_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/map_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       90 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/map_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    12751 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/metaschema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     3940 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/metaschema_base.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    13475 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/salad.md
--rw-r--r--   0 michael   (1000) michael   (1000)      882 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/sfdsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      367 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/sfdsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      289 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/sfdsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      190 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/sfdsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      830 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/typedsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      394 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/typedsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      299 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/typedsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      111 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/typedsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      846 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/vocab_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      243 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/vocab_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      345 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/vocab_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      267 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/vocab_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)   130989 2023-04-26 10:03:15.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema.py
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/py.typed
--rw-r--r--   0 michael   (1000) michael   (1000)    23034 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/python_codegen.py
--rw-r--r--   0 michael   (1000) michael   (1000)    28705 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/python_codegen_support.py
--rw-r--r--   0 michael   (1000) michael   (1000)    46610 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/ref_resolver.py
--rw-r--r--   0 michael   (1000) michael   (1000)    29944 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/schema.py
--rw-r--r--   0 michael   (1000) michael   (1000)     9031 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/sourceline.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.371567 schema-salad-8.4.20230426093816/schema_salad/tests/
--rw-r--r--   0 michael   (1000) michael   (1000)  2615816 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/EDAM.owl
--rw-r--r--   0 michael   (1000) michael   (1000)      827 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/Process.yml
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)      125 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/bad_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       65 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/bad_schema2.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      140 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/basket.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     1267 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/basket_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      590 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/class_field_test.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      452 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/conftest.py
--rw-r--r--   0 michael   (1000) michael   (1000)   126068 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/cwl-pre.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.371567 schema-salad-8.4.20230426093816/schema_salad/tests/docimp/
--rw-r--r--   0 michael   (1000) michael   (1000)      155 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/docimp/d1.yml
--rw-r--r--   0 michael   (1000) michael   (1000)        7 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/docimp/d2.md
--rw-r--r--   0 michael   (1000) michael   (1000)       42 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/docimp/d3.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       42 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/docimp/d4.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       18 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/docimp/d5.md
--rw-r--r--   0 michael   (1000) michael   (1000)      320 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/docimp/dpre.json
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.375567 schema-salad-8.4.20230426093816/schema_salad/tests/foreign/
--rwxr-xr-x   0 michael   (1000) michael   (1000)      347 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/foreign/foreign_prop1.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      302 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/foreign/foreign_prop2.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      436 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/foreign/foreign_prop3.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      390 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/foreign/foreign_prop4.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      428 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/foreign/foreign_prop5.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      294 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/foreign/foreign_prop6.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      292 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/foreign/foreign_prop7.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/formattest2.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       41 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/frag.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       13 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/hello.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       71 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/hellofield.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      946 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/inherited-attributes.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       17 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/inject-id1.yml
--rw-r--r--   0 michael   (1000) michael   (1000)        9 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/inject-id2.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       32 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/inject-id3.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       25 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/list.json
--rw-r--r--   0 michael   (1000) michael   (1000)     1241 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/matcher.py
--rw-r--r--   0 michael   (1000) michael   (1000)      289 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/memory-leak-check.py
--rw-r--r--   0 michael   (1000) michael   (1000)    61408 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/metaschema-pre.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      208 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/missing_step_name.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       18 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/mixin.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      154 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/multidoc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      900 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/pt.yml
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1466 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/revtool_bad_schema.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_avro_names.py
--rw-r--r--   0 michael   (1000) michael   (1000)     7342 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_cg.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1146 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_cli_args.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1144 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_cpp_codegen.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2406 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_cwl11.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1071 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_dlang_codegen.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3366 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_dotnet_codegen.py
--rw-r--r--   0 michael   (1000) michael   (1000)    15557 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_errors.py
--rw-r--r--   0 michael   (1000) michael   (1000)    19849 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_examples.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2660 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_fetch.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1603 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_fp.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1868 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_java_codegen.py
--rw-r--r--   0 michael   (1000) michael   (1000)     9277 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_makedoc.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1334 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_misc.py
--rw-r--r--   0 michael   (1000) michael   (1000)      818 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_pickling.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6218 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_print_oneline.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4547 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_python_codegen.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.375567 schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.375567 schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/
--rw-r--r--   0 michael   (1000) michael   (1000)      227 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/PreprocessedFilesType.yaml
--rw-r--r--   0 michael   (1000) michael   (1000)      912 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/preprocess_util.js
--rwxr-xr-x   0 michael   (1000) michael   (1000)    11901 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/preprocess_vcf.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      148 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/vcf_merge_util.js
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.375567 schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl/bio-cwl-tools/
--rwxr-xr-x   0 michael   (1000) michael   (1000)     4732 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl/bio-cwl-tools/bamtools_stats.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)     4701 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl/bio-cwl-tools/bamtools_stats_invalid_schema_ref.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     5757 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl/bio-cwl-tools/picard_CreateSequenceDictionary.cwl
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.375567 schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl/h3agatk/
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1905 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl/h3agatk/GATK-Sub-Workflow-h3abionet-snp.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)    10910 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl/h3agatk/GATK-complete-WES-Workflow-h3abionet.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1122 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl/tabs_rna_seq_workflow.cwl
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.375567 schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl/topmed/
--rwxr-xr-x   0 michael   (1000) michael   (1000)     5976 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl/topmed/topmed_variant_calling_pipeline.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     2231 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl.py
--rw-r--r--   0 michael   (1000) michael   (1000)     9625 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_ref_resolver.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.379567 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/
--rw-r--r--   0 michael   (1000) michael   (1000)    30591 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/CommandLineTool.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      209 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/CommonWorkflowLanguage.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    25402 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/Process.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    20107 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/Workflow.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      453 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/avro_naming.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      529 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/avro_naming_base.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      529 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/avro_subtype.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      524 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/avro_subtype_bad.yml
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/concepts.md
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/contrib.md
--rw-r--r--   0 michael   (1000) michael   (1000)      514 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/cwltest-schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/intro.md
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/invocation.md
--rw-r--r--   0 michael   (1000) michael   (1000)     3933 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/metaschema_base.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      514 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/misc_schema_v1.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      575 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/misc_schema_v2.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       54 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/no_field_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       70 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/one_line_primary_doc.yml
--rwxr-xr-x   0 michael   (1000) michael   (1000)       42 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/test1.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      157 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/test10.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      147 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/test11.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      299 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/test12.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      302 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/test13.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      208 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/test14.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      247 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/test15.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      274 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/test16.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      238 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/test17.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      241 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/test18.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      269 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/test19.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)       43 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/test2.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)       98 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/test3.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)       93 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/test4.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)       99 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/test5.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)       83 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/test6.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      154 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/test7.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      152 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/test8.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      151 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/test9.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1233 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1536 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schemas_directive.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3545 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_subtypes.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3412 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_typescript_codegen.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1613 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/util.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.383567 schema-salad-8.4.20230426093816/schema_salad/typescript/
--rw-r--r--   0 michael   (1000) michael   (1000)     1617 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/.gitignore
--rw-r--r--   0 michael   (1000) michael   (1000)    11357 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/LICENSE
--rw-r--r--   0 michael   (1000) michael   (1000)      138 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/index.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     1082 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/package.json
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.383567 schema-salad-8.4.20230426093816/schema_salad/typescript/test/
--rw-r--r--   0 michael   (1000) michael   (1000)      879 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/test/AnyLoader.spec.ts
--rw-r--r--   0 michael   (1000) michael   (1000)      147 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/test/ExampleTest.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     3118 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/test/Fetcher.spec.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     1390 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/test/IdMap.spec.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     3265 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/test/Typeguards.spec.ts
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.383567 schema-salad-8.4.20230426093816/schema_salad/typescript/test/data/
--rw-r--r--   0 michael   (1000) michael   (1000)       70 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/test/data/hellofield.yml
--rw-r--r--   0 michael   (1000) michael   (1000)        5 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/test/data/test.txt
--rw-r--r--   0 michael   (1000) michael   (1000)     1418 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/test/utilities.spec.ts
--rw-r--r--   0 michael   (1000) michael   (1000)      541 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/tsconfig.json
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.383567 schema-salad-8.4.20230426093816/schema_salad/typescript/util/
--rw-r--r--   0 michael   (1000) michael   (1000)       60 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/util/Dict.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     2336 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/util/Fetcher.ts
--rw-r--r--   0 michael   (1000) michael   (1000)      860 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/util/Internal.ts
--rw-r--r--   0 michael   (1000) michael   (1000)      282 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/util/LoaderInstances.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     1554 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/util/LoadingOptions.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     3536 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/util/Saveable.ts
--rw-r--r--   0 michael   (1000) michael   (1000)      593 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/util/Typeguards.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     1406 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/util/ValidationException.ts
--rw-r--r--   0 michael   (1000) michael   (1000)       74 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/util/Vocabs.ts
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.387567 schema-salad-8.4.20230426093816/schema_salad/typescript/util/loaders/
--rw-r--r--   0 michael   (1000) michael   (1000)      345 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/util/loaders/AnyLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     1005 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/util/loaders/ArrayLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)      481 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/util/loaders/EnumLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)      350 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/util/loaders/ExpressionLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     1180 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/util/loaders/IdMapLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     3228 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/util/loaders/Loader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)      497 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/util/loaders/PrimitiveLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)      721 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/util/loaders/RecordLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     2508 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/util/loaders/RootLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     2421 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/util/loaders/SecondaryDSLLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     1776 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/util/loaders/TypeDSLLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)      789 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/util/loaders/UnionLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     1043 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/util/loaders/UriLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)    29355 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript_codegen.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3640 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/utils.py
--rw-r--r--   0 michael   (1000) michael   (1000)    15546 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/validate.py
--rw-r--r--   0 michael   (1000) michael   (1000)      836 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad.Dockerfile
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.339566 schema-salad-8.4.20230426093816/schema_salad.egg-info/
--rw-r--r--   0 michael   (1000) michael   (1000)    15861 2023-04-26 10:11:35.000000 schema-salad-8.4.20230426093816/schema_salad.egg-info/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)    15666 2023-04-26 10:11:35.000000 schema-salad-8.4.20230426093816/schema_salad.egg-info/SOURCES.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-04-26 10:11:35.000000 schema-salad-8.4.20230426093816/schema_salad.egg-info/dependency_links.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      106 2023-04-26 10:11:35.000000 schema-salad-8.4.20230426093816/schema_salad.egg-info/entry_points.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      425 2023-04-26 10:11:35.000000 schema-salad-8.4.20230426093816/schema_salad.egg-info/requires.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       13 2023-04-26 10:11:35.000000 schema-salad-8.4.20230426093816/schema_salad.egg-info/top_level.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-04-26 10:02:44.000000 schema-salad-8.4.20230426093816/schema_salad.egg-info/zip-safe
--rw-r--r--   0 michael   (1000) michael   (1000)      189 2023-04-26 10:11:35.387567 schema-salad-8.4.20230426093816/setup.cfg
--rw-r--r--   0 michael   (1000) michael   (1000)     5699 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/setup.py
--rw-r--r--   0 michael   (1000) michael   (1000)       45 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/test-requirements.txt
--rw-r--r--   0 michael   (1000) michael   (1000)     2721 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/tox.ini
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 15:28:58.398093 schema-salad-8.4.20230511084951/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 15:28:58.354092 schema-salad-8.4.20230511084951/.circleci/
+-rw-r--r--   0 michael   (1000) michael   (1000)     3370 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/.circleci/config.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      324 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/.coveragerc
+-rw-r--r--   0 michael   (1000) michael   (1000)      304 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/.dockerignore
+-rw-r--r--   0 michael   (1000) michael   (1000)      282 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/.flake8
+-rw-r--r--   0 michael   (1000) michael   (1000)      229 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/.git-blame-ignore-revs
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 15:28:58.354092 schema-salad-8.4.20230511084951/.github/
+-rw-r--r--   0 michael   (1000) michael   (1000)      603 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/.github/dependabot.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 15:28:58.354092 schema-salad-8.4.20230511084951/.github/workflows/
+-rw-r--r--   0 michael   (1000) michael   (1000)     3859 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/.github/workflows/ci-tests.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      835 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1090 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/.github/workflows/quay-publish.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      169 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/.github/workflows/wheel-prep.sh
+-rw-r--r--   0 michael   (1000) michael   (1000)     5664 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/.github/workflows/wheels.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      219 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/.gitignore
+-rw-r--r--   0 michael   (1000) michael   (1000)      113 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/.isort.cfg
+-rw-r--r--   0 michael   (1000) michael   (1000)      585 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/.mergify.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    21223 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/.pylintrc
+-rw-r--r--   0 michael   (1000) michael   (1000)      558 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/.readthedocs.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1643 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/CONTRIBUTING.md
+-rw-r--r--   0 michael   (1000) michael   (1000)    11358 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/LICENSE.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      680 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/MANIFEST.in
+-rw-r--r--   0 michael   (1000) michael   (1000)     8324 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/Makefile
+-rw-r--r--   0 michael   (1000) michael   (1000)    15861 2023-05-11 15:28:58.398093 schema-salad-8.4.20230511084951/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)    14703 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/README.rst
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      438 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/build-schema_salad-docker.sh
+-rw-r--r--   0 michael   (1000) michael   (1000)      209 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/dev-requirements.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 15:28:58.358092 schema-salad-8.4.20230511084951/docs/
+-rw-r--r--   0 michael   (1000) michael   (1000)      634 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/docs/Makefile
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 15:28:58.358092 schema-salad-8.4.20230511084951/docs/_static/
+-rw-r--r--   0 michael   (1000) michael   (1000)    15086 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/docs/_static/favicon.ico
+-rw-r--r--   0 michael   (1000) michael   (1000)      200 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/docs/cli.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)     3461 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/docs/conf.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      220 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/docs/index.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)      795 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/docs/make.bat
+-rw-r--r--   0 michael   (1000) michael   (1000)      656 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/docs/typeshed.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)      325 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/lgtm.yml
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      819 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/manual_wheel_publish.sh
+-rw-r--r--   0 michael   (1000) michael   (1000)      132 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-requirements.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 15:28:58.350093 schema-salad-8.4.20230511084951/mypy-stubs/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 15:28:58.358092 schema-salad-8.4.20230511084951/mypy-stubs/cachecontrol/
+-rw-r--r--   0 michael   (1000) michael   (1000)      219 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/cachecontrol/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      226 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/cachecontrol/cache.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 15:28:58.358092 schema-salad-8.4.20230511084951/mypy-stubs/cachecontrol/caches/
+-rw-r--r--   0 michael   (1000) michael   (1000)      273 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/cachecontrol/caches/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      873 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/cachecontrol/caches/file_cache.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      169 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/cachecontrol/compat.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      470 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/cachecontrol/controller.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      532 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/cachecontrol/wrapper.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 15:28:58.358092 schema-salad-8.4.20230511084951/mypy-stubs/mistune/
+-rw-r--r--   0 michael   (1000) michael   (1000)      922 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/mistune/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      168 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/mistune/_types.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     5480 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/mistune/block_parser.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2848 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/mistune/inline_parser.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1535 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/mistune/markdown.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 15:28:58.358092 schema-salad-8.4.20230511084951/mypy-stubs/mistune/plugins/
+-rw-r--r--   0 michael   (1000) michael   (1000)      458 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/mistune/plugins/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      566 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/mistune/plugins/table.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     4159 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/mistune/renderers.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1870 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/mistune/scanner.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      191 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/mistune/util.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 15:28:58.358092 schema-salad-8.4.20230511084951/mypy-stubs/rdflib/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1292 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/rdflib/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      674 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/rdflib/collection.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      231 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/rdflib/compare.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      182 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/rdflib/exceptions.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     8337 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/rdflib/graph.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 15:28:58.362093 schema-salad-8.4.20230511084951/mypy-stubs/rdflib/namespace/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2010 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/rdflib/namespace/_CSVW.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/rdflib/namespace/_DC.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1034 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/rdflib/namespace/_DCAT.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2361 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/rdflib/namespace/_DCTERMS.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1109 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/rdflib/namespace/_DOAP.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1847 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/rdflib/namespace/_FOAF.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     4691 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/rdflib/namespace/_ODRL2.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1259 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/rdflib/namespace/_ORG.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2260 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/rdflib/namespace/_OWL.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      441 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/rdflib/namespace/_PROF.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     4520 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/rdflib/namespace/_PROV.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1105 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/rdflib/namespace/_QB.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      620 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/rdflib/namespace/_RDF.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      519 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/rdflib/namespace/_RDFS.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)    41401 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/rdflib/namespace/_SDO.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     4965 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/rdflib/namespace/_SH.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      943 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/rdflib/namespace/_SKOS.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1075 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/rdflib/namespace/_SOSA.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      680 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/rdflib/namespace/_SSN.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2462 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/rdflib/namespace/_TIME.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      927 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/rdflib/namespace/_VOID.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1742 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/rdflib/namespace/_XSD.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2282 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/rdflib/namespace/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      131 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/rdflib/parser.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      724 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/rdflib/paths.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      893 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/rdflib/plugin.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 15:28:58.362093 schema-salad-8.4.20230511084951/mypy-stubs/rdflib/plugins/
+-rw-r--r--   0 michael   (1000) michael   (1000)      118 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/rdflib/plugins/__init__.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 15:28:58.362093 schema-salad-8.4.20230511084951/mypy-stubs/rdflib/plugins/parsers/
+-rw-r--r--   0 michael   (1000) michael   (1000)      126 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/rdflib/plugins/parsers/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)       34 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/rdflib/plugins/parsers/notation3.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1354 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/rdflib/query.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1370 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/rdflib/resource.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1337 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/rdflib/term.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      115 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/rdflib/util.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 15:28:58.362093 schema-salad-8.4.20230511084951/mypy-stubs/ruamel/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy-stubs/ruamel/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      137 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/mypy.ini
+-rw-r--r--   0 michael   (1000) michael   (1000)     1097 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/pyproject.toml
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     3512 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/release-test.sh
+-rw-r--r--   0 michael   (1000) michael   (1000)      364 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/requirements.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 15:28:58.366093 schema-salad-8.4.20230511084951/schema_salad/
+-rw-r--r--   0 michael   (1000) michael   (1000)      395 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      110 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/__main__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      186 2023-05-11 15:28:58.000000 schema-salad-8.4.20230511084951/schema_salad/_version.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 15:28:58.366093 schema-salad-8.4.20230511084951/schema_salad/avro/
+-rw-r--r--   0 michael   (1000) michael   (1000)    11359 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/avro/LICENSE
+-rw-r--r--   0 michael   (1000) michael   (1000)      166 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/avro/NOTICE
+-rw-r--r--   0 michael   (1000) michael   (1000)      802 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/avro/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    23815 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/avro/schema.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     7237 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/codegen.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4412 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/codegen_base.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    19604 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/cpp_codegen.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    10930 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/dlang_codegen.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 15:28:58.366093 schema-salad-8.4.20230511084951/schema_salad/dotnet/
+-rw-r--r--   0 michael   (1000) michael   (1000)       82 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/dotnet/AssemblyInfo.cs
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 15:28:58.366093 schema-salad-8.4.20230511084951/schema_salad/dotnet/DocFx/
+-rw-r--r--   0 michael   (1000) michael   (1000)      445 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/dotnet/DocFx/filterConfig.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       22 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/dotnet/DocFx/index.md
+-rw-r--r--   0 michael   (1000) michael   (1000)       71 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/dotnet/DocFx/toc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    11356 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/dotnet/LICENSE
+-rw-r--r--   0 michael   (1000) michael   (1000)     1442 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/dotnet/Project.csproj.template
+-rw-r--r--   0 michael   (1000) michael   (1000)       40 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/dotnet/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1788 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/dotnet/Solution.sln
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 15:28:58.370093 schema-salad-8.4.20230511084951/schema_salad/dotnet/Test/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 15:28:58.370093 schema-salad-8.4.20230511084951/schema_salad/dotnet/Test/data/
+-rw-r--r--   0 michael   (1000) michael   (1000)        4 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/dotnet/Test/data/test.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      333 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/dotnet/Test/runsettings.xml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 15:28:58.370093 schema-salad-8.4.20230511084951/schema_salad/dotnet/Test/src/
+-rw-r--r--   0 michael   (1000) michael   (1000)      207 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/dotnet/Test/src/ExampleTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     2173 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/dotnet/Test/src/FetcherTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1151 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/dotnet/Test/src/UtilitiesTests.cs
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 15:28:58.370093 schema-salad-8.4.20230511084951/schema_salad/dotnet/Test/src/loaders/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1027 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/dotnet/Test/src/loaders/AnyLoaderTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1321 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/dotnet/Test/src/loaders/ArrayLoaderTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     2429 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/dotnet/Test/src/loaders/EnumLoaderTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      749 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/dotnet/Test/src/loaders/ExpressionLoaderTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1742 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/dotnet/Test/src/loaders/IdMapLoaderTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      766 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/dotnet/Test/src/loaders/NullLoaderTests.cs
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 15:28:58.370093 schema-salad-8.4.20230511084951/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1435 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderDoubleTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1431 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderFloatTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1393 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderIntTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1246 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderStringTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1087 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/dotnet/Test/src/loaders/UnionLoaderTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1188 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/dotnet/Test.csproj.template
+-rw-r--r--   0 michael   (1000) michael   (1000)     1459 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/dotnet/docfx.json
+-rw-r--r--   0 michael   (1000) michael   (1000)    11383 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/dotnet/editorconfig
+-rw-r--r--   0 michael   (1000) michael   (1000)     6894 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/dotnet/gitignore
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 15:28:58.370093 schema-salad-8.4.20230511084951/schema_salad/dotnet/util/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2262 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/dotnet/util/Fetcher.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      167 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/dotnet/util/LoaderInstances.cs
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 15:28:58.370093 schema-salad-8.4.20230511084951/schema_salad/dotnet/util/Loaders/
+-rw-r--r--   0 michael   (1000) michael   (1000)      338 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/dotnet/util/Loaders/AnyLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1754 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/dotnet/util/Loaders/ArrayLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      905 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/dotnet/util/Loaders/EnumLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      646 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/dotnet/util/Loaders/ExpressionLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     2168 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/dotnet/util/Loaders/IdMapLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     4481 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/dotnet/util/Loaders/Loader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      362 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/dotnet/util/Loaders/NullLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      745 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/dotnet/util/Loaders/PrimitiveLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      734 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/dotnet/util/Loaders/RecordLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1674 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/dotnet/util/Loaders/RootLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     3984 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/dotnet/util/Loaders/SecondaryDSLLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     3056 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/dotnet/util/Loaders/TypeDSLLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      793 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/dotnet/util/Loaders/UnionLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1656 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/dotnet/util/Loaders/UriLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     5215 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/dotnet/util/LoadingOptions.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     4595 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/dotnet/util/Saveable.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1490 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/dotnet/util/ScalarNodeTypeResolver.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      501 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/dotnet/util/UriExtensions.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1624 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/dotnet/util/Utilities.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1913 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/dotnet/util/ValidationException.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      264 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/dotnet/util/Vocabs.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)    33304 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/dotnet_codegen.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4175 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/exceptions.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     8025 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/fetcher.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 15:28:58.374093 schema-salad-8.4.20230511084951/schema_salad/java/
+-rw-r--r--   0 michael   (1000) michael   (1000)       61 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/java/MANIFEST.MF
+-rw-r--r--   0 michael   (1000) michael   (1000)      993 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/java/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)        8 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/java/gitignore
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 15:28:58.374093 schema-salad-8.4.20230511084951/schema_salad/java/main_utils/
+-rw-r--r--   0 michael   (1000) michael   (1000)      335 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/java/main_utils/AnyLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     1248 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/java/main_utils/ArrayLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      296 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/java/main_utils/ConstantMaps.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     1521 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/java/main_utils/DefaultFetcher.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      984 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/java/main_utils/EnumLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      416 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/java/main_utils/ExpressionLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      186 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/java/main_utils/Fetcher.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     1697 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/java/main_utils/IdMapLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     4613 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/java/main_utils/Loader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      125 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/java/main_utils/LoaderInstances.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     3815 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/java/main_utils/LoadingOptions.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     1944 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/java/main_utils/LoadingOptionsBuilder.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      332 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/java/main_utils/NullLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     1113 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/java/main_utils/OneOrListOf.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     1050 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/java/main_utils/OneOrListOfLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      543 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/java/main_utils/OptionalLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      384 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/java/main_utils/PrimitiveLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     1175 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/java/main_utils/RecordLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     3734 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/java/main_utils/RootLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      180 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/java/main_utils/Saveable.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      177 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/java/main_utils/SaveableImpl.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     3035 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/java/main_utils/SecondaryFilesDslLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     2555 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/java/main_utils/TypeDslLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      866 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/java/main_utils/UnionLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     1511 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/java/main_utils/UriLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     3293 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/java/main_utils/Uris.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     2254 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/java/main_utils/ValidationException.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      789 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/java/main_utils/Validator.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     1025 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/java/main_utils/YamlUtils.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      131 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/java/main_utils/package.html
+-rw-r--r--   0 michael   (1000) michael   (1000)      237 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/java/overview.html
+-rw-r--r--   0 michael   (1000) michael   (1000)      187 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/java/package.html
+-rw-r--r--   0 michael   (1000) michael   (1000)     5467 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/java/pom.xml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 15:28:58.374093 schema-salad-8.4.20230511084951/schema_salad/java/test_utils/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1347 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/java/test_utils/DefaultFetcherTest.java
+-rw-r--r--   0 michael   (1000) michael   (1000)       74 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/java/test_utils/ExamplesTest.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     1134 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/java/test_utils/ShortnameTest.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      402 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/java/test_utils/YamlUtilsTest.java
+-rw-r--r--   0 michael   (1000) michael   (1000)    32358 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/java_codegen.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     8476 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/jsonld_context.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    14154 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/main.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    33109 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/makedoc.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 15:28:58.378093 schema-salad-8.4.20230511084951/schema_salad/metaschema/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1327 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/metaschema/field_name.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/metaschema/field_name_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      283 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/metaschema/field_name_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/metaschema/field_name_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2442 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/metaschema/ident_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/metaschema/ident_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      473 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/metaschema/ident_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      437 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/metaschema/ident_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     3322 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/metaschema/import_include.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1804 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/metaschema/link_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      411 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/metaschema/link_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      264 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/metaschema/link_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      313 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/metaschema/link_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      932 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/metaschema/map_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      183 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/metaschema/map_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/metaschema/map_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       90 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/metaschema/map_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    12751 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/metaschema/metaschema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     3940 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/metaschema/metaschema_base.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    13461 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/metaschema/salad.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      882 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/metaschema/sfdsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      367 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/metaschema/sfdsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      289 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/metaschema/sfdsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      190 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/metaschema/sfdsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      830 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/metaschema/typedsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      394 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/metaschema/typedsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      299 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/metaschema/typedsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      111 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/metaschema/typedsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      846 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/metaschema/vocab_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      243 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/metaschema/vocab_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      345 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/metaschema/vocab_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/metaschema/vocab_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)   130989 2023-05-11 15:22:29.000000 schema-salad-8.4.20230511084951/schema_salad/metaschema.py
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/py.typed
+-rw-r--r--   0 michael   (1000) michael   (1000)    23034 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/python_codegen.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    28705 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/python_codegen_support.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    46746 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/ref_resolver.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    29944 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/schema.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     9031 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/sourceline.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 15:28:58.386093 schema-salad-8.4.20230511084951/schema_salad/tests/
+-rw-r--r--   0 michael   (1000) michael   (1000)  2615816 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/EDAM.owl
+-rw-r--r--   0 michael   (1000) michael   (1000)      827 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/Process.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      125 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/bad_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       65 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/bad_schema2.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      140 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/basket.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1267 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/basket_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      590 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/class_field_test.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      452 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/conftest.py
+-rw-r--r--   0 michael   (1000) michael   (1000)   126068 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/cwl-pre.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 15:28:58.386093 schema-salad-8.4.20230511084951/schema_salad/tests/docimp/
+-rw-r--r--   0 michael   (1000) michael   (1000)      155 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/docimp/d1.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)        7 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/docimp/d2.md
+-rw-r--r--   0 michael   (1000) michael   (1000)       42 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/docimp/d3.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       42 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/docimp/d4.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       18 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/docimp/d5.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      320 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/docimp/dpre.json
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 15:28:58.390093 schema-salad-8.4.20230511084951/schema_salad/tests/foreign/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      347 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/foreign/foreign_prop1.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      302 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/foreign/foreign_prop2.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      436 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/foreign/foreign_prop3.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      390 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/foreign/foreign_prop4.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      428 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/foreign/foreign_prop5.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      294 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/foreign/foreign_prop6.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      292 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/foreign/foreign_prop7.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/formattest2.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       41 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/frag.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       13 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/hello.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       71 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/hellofield.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      946 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/inherited-attributes.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       17 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/inject-id1.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)        9 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/inject-id2.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       32 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/inject-id3.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       25 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/list.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     1241 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/matcher.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      289 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/memory-leak-check.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    61394 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/metaschema-pre.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      208 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/missing_step_name.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       18 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/mixin.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      154 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/multidoc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      900 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/pt.yml
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1466 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/revtool_bad_schema.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_avro_names.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     7342 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_cg.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1146 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_cli_args.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1144 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_cpp_codegen.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2406 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_cwl11.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1071 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_dlang_codegen.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3366 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_dotnet_codegen.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    15557 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_errors.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    19849 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_examples.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2660 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_fetch.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1603 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_fp.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1868 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_java_codegen.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     9277 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_makedoc.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1334 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_misc.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      818 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_pickling.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6218 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_print_oneline.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4547 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_python_codegen.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 15:28:58.390093 schema-salad-8.4.20230511084951/schema_salad/tests/test_real_cwl/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 15:28:58.390093 schema-salad-8.4.20230511084951/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/
+-rw-r--r--   0 michael   (1000) michael   (1000)      227 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/PreprocessedFilesType.yaml
+-rw-r--r--   0 michael   (1000) michael   (1000)      912 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/preprocess_util.js
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    11901 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/preprocess_vcf.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      148 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/vcf_merge_util.js
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 15:28:58.390093 schema-salad-8.4.20230511084951/schema_salad/tests/test_real_cwl/bio-cwl-tools/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     4732 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_real_cwl/bio-cwl-tools/bamtools_stats.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     4701 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_real_cwl/bio-cwl-tools/bamtools_stats_invalid_schema_ref.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     5757 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_real_cwl/bio-cwl-tools/picard_CreateSequenceDictionary.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 15:28:58.390093 schema-salad-8.4.20230511084951/schema_salad/tests/test_real_cwl/h3agatk/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1905 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_real_cwl/h3agatk/GATK-Sub-Workflow-h3abionet-snp.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    10910 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_real_cwl/h3agatk/GATK-complete-WES-Workflow-h3abionet.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1122 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_real_cwl/tabs_rna_seq_workflow.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 15:28:58.390093 schema-salad-8.4.20230511084951/schema_salad/tests/test_real_cwl/topmed/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     5976 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_real_cwl/topmed/topmed_variant_calling_pipeline.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     2231 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_real_cwl.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     9625 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_ref_resolver.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 15:28:58.394093 schema-salad-8.4.20230511084951/schema_salad/tests/test_schema/
+-rw-r--r--   0 michael   (1000) michael   (1000)    30591 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_schema/CommandLineTool.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      209 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_schema/CommonWorkflowLanguage.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    25402 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_schema/Process.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    20107 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_schema/Workflow.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      453 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_schema/avro_naming.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      529 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_schema/avro_naming_base.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      529 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_schema/avro_subtype.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      524 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_schema/avro_subtype_bad.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_schema/concepts.md
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_schema/contrib.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      514 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_schema/cwltest-schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_schema/intro.md
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_schema/invocation.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     3933 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_schema/metaschema_base.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      514 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_schema/misc_schema_v1.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      575 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_schema/misc_schema_v2.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       54 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_schema/no_field_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       70 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_schema/one_line_primary_doc.yml
+-rwxr-xr-x   0 michael   (1000) michael   (1000)       42 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_schema/test1.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      157 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_schema/test10.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      147 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_schema/test11.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      299 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_schema/test12.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      302 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_schema/test13.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      208 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_schema/test14.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      247 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_schema/test15.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      274 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_schema/test16.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      238 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_schema/test17.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      241 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_schema/test18.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      269 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_schema/test19.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)       43 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_schema/test2.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)       98 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_schema/test3.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)       93 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_schema/test4.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)       99 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_schema/test5.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)       83 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_schema/test6.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      154 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_schema/test7.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      152 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_schema/test8.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      151 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_schema/test9.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1233 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_schema.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1536 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_schemas_directive.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3545 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_subtypes.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3412 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/test_typescript_codegen.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1613 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/tests/util.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 15:28:58.394093 schema-salad-8.4.20230511084951/schema_salad/typescript/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1617 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/typescript/.gitignore
+-rw-r--r--   0 michael   (1000) michael   (1000)    11357 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/typescript/LICENSE
+-rw-r--r--   0 michael   (1000) michael   (1000)      138 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/typescript/index.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     1082 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/typescript/package.json
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 15:28:58.394093 schema-salad-8.4.20230511084951/schema_salad/typescript/test/
+-rw-r--r--   0 michael   (1000) michael   (1000)      879 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/typescript/test/AnyLoader.spec.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)      147 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/typescript/test/ExampleTest.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     3118 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/typescript/test/Fetcher.spec.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     1390 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/typescript/test/IdMap.spec.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     3265 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/typescript/test/Typeguards.spec.ts
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 15:28:58.394093 schema-salad-8.4.20230511084951/schema_salad/typescript/test/data/
+-rw-r--r--   0 michael   (1000) michael   (1000)       70 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/typescript/test/data/hellofield.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)        5 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/typescript/test/data/test.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)     1418 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/typescript/test/utilities.spec.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)      541 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/typescript/tsconfig.json
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 15:28:58.398093 schema-salad-8.4.20230511084951/schema_salad/typescript/util/
+-rw-r--r--   0 michael   (1000) michael   (1000)       60 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/typescript/util/Dict.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     2336 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/typescript/util/Fetcher.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)      860 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/typescript/util/Internal.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)      282 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/typescript/util/LoaderInstances.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     1554 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/typescript/util/LoadingOptions.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     3536 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/typescript/util/Saveable.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)      593 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/typescript/util/Typeguards.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     1406 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/typescript/util/ValidationException.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)       74 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/typescript/util/Vocabs.ts
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 15:28:58.398093 schema-salad-8.4.20230511084951/schema_salad/typescript/util/loaders/
+-rw-r--r--   0 michael   (1000) michael   (1000)      345 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/typescript/util/loaders/AnyLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     1005 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/typescript/util/loaders/ArrayLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)      481 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/typescript/util/loaders/EnumLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)      350 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/typescript/util/loaders/ExpressionLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     1180 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/typescript/util/loaders/IdMapLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     3228 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/typescript/util/loaders/Loader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)      497 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/typescript/util/loaders/PrimitiveLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)      721 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/typescript/util/loaders/RecordLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     2508 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/typescript/util/loaders/RootLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     2421 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/typescript/util/loaders/SecondaryDSLLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     1776 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/typescript/util/loaders/TypeDSLLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)      789 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/typescript/util/loaders/UnionLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     1043 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/typescript/util/loaders/UriLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)    29355 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/typescript_codegen.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3672 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/utils.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    15546 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad/validate.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      836 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/schema_salad.Dockerfile
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 15:28:58.366093 schema-salad-8.4.20230511084951/schema_salad.egg-info/
+-rw-r--r--   0 michael   (1000) michael   (1000)    15861 2023-05-11 15:28:58.000000 schema-salad-8.4.20230511084951/schema_salad.egg-info/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)    15666 2023-05-11 15:28:58.000000 schema-salad-8.4.20230511084951/schema_salad.egg-info/SOURCES.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-05-11 15:28:58.000000 schema-salad-8.4.20230511084951/schema_salad.egg-info/dependency_links.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      106 2023-05-11 15:28:58.000000 schema-salad-8.4.20230511084951/schema_salad.egg-info/entry_points.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      435 2023-05-11 15:28:58.000000 schema-salad-8.4.20230511084951/schema_salad.egg-info/requires.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       13 2023-05-11 15:28:58.000000 schema-salad-8.4.20230511084951/schema_salad.egg-info/top_level.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-05-11 15:22:05.000000 schema-salad-8.4.20230511084951/schema_salad.egg-info/zip-safe
+-rw-r--r--   0 michael   (1000) michael   (1000)      189 2023-05-11 15:28:58.398093 schema-salad-8.4.20230511084951/setup.cfg
+-rw-r--r--   0 michael   (1000) michael   (1000)     5766 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/setup.py
+-rw-r--r--   0 michael   (1000) michael   (1000)       45 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/test-requirements.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)     2721 2023-05-11 15:21:55.000000 schema-salad-8.4.20230511084951/tox.ini
```

### Comparing `schema-salad-8.4.20230426093816/.circleci/config.yml` & `schema-salad-8.4.20230511084951/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/.github/dependabot.yml` & `schema-salad-8.4.20230511084951/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/.github/workflows/ci-tests.yml` & `schema-salad-8.4.20230511084951/.github/workflows/ci-tests.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/.github/workflows/codeql-analysis.yml` & `schema-salad-8.4.20230511084951/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/.github/workflows/quay-publish.yml` & `schema-salad-8.4.20230511084951/.github/workflows/quay-publish.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/.github/workflows/wheels.yml` & `schema-salad-8.4.20230511084951/.github/workflows/wheels.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/.mergify.yml` & `schema-salad-8.4.20230511084951/.mergify.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/.pylintrc` & `schema-salad-8.4.20230511084951/.pylintrc`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/.readthedocs.yml` & `schema-salad-8.4.20230511084951/.readthedocs.yml`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 # Build documentation in the docs/ directory with Sphinx
 sphinx:
   configuration: docs/conf.py
 
 # Optionally build your docs in additional formats such as PDF and ePub
 formats: all
 
+build:
+  os: ubuntu-22.04
+  tools:
+    python: "3.11"
+
 # Optionally set the version of Python and requirements required to build your docs
 python:
-  version: 3.7
   install:
    - method: pip
      path: .
      extra_requirements: [ docs ]
```

### Comparing `schema-salad-8.4.20230426093816/CONTRIBUTING.md` & `schema-salad-8.4.20230511084951/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/LICENSE.txt` & `schema-salad-8.4.20230511084951/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/MANIFEST.in` & `schema-salad-8.4.20230511084951/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/Makefile` & `schema-salad-8.4.20230511084951/Makefile`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/PKG-INFO` & `schema-salad-8.4.20230511084951/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schema-salad
-Version: 8.4.20230426093816
+Version: 8.4.20230511084951
 Summary: Schema Annotations for Linked Avro Data (SALAD)
 Home-page: https://github.com/common-workflow-language/schema_salad
 Download-URL: https://github.com/common-workflow-language/schema_salad/releases
 Author: Common workflow language working group
 Author-email: common-workflow-language@googlegroups.com
 License: Apache 2.0
 Classifier: Environment :: Console
```

### Comparing `schema-salad-8.4.20230426093816/README.rst` & `schema-salad-8.4.20230511084951/README.rst`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/docs/Makefile` & `schema-salad-8.4.20230511084951/docs/Makefile`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/docs/_static/favicon.ico` & `schema-salad-8.4.20230511084951/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/docs/conf.py` & `schema-salad-8.4.20230511084951/docs/conf.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/docs/make.bat` & `schema-salad-8.4.20230511084951/docs/make.bat`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/docs/typeshed.rst` & `schema-salad-8.4.20230511084951/docs/typeshed.rst`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/manual_wheel_publish.sh` & `schema-salad-8.4.20230511084951/manual_wheel_publish.sh`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/mypy-stubs/cachecontrol/caches/file_cache.pyi` & `schema-salad-8.4.20230511084951/mypy-stubs/cachecontrol/caches/file_cache.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/mypy-stubs/cachecontrol/wrapper.pyi` & `schema-salad-8.4.20230511084951/mypy-stubs/cachecontrol/wrapper.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/mypy-stubs/mistune/__init__.pyi` & `schema-salad-8.4.20230511084951/mypy-stubs/mistune/__init__.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/mypy-stubs/mistune/block_parser.pyi` & `schema-salad-8.4.20230511084951/mypy-stubs/mistune/block_parser.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/mypy-stubs/mistune/inline_parser.pyi` & `schema-salad-8.4.20230511084951/mypy-stubs/mistune/inline_parser.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/mypy-stubs/mistune/markdown.pyi` & `schema-salad-8.4.20230511084951/mypy-stubs/mistune/markdown.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/mypy-stubs/mistune/plugins/table.pyi` & `schema-salad-8.4.20230511084951/mypy-stubs/mistune/plugins/table.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/mypy-stubs/mistune/renderers.pyi` & `schema-salad-8.4.20230511084951/mypy-stubs/mistune/renderers.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/mypy-stubs/mistune/scanner.pyi` & `schema-salad-8.4.20230511084951/mypy-stubs/mistune/scanner.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/__init__.pyi` & `schema-salad-8.4.20230511084951/mypy-stubs/rdflib/__init__.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/collection.pyi` & `schema-salad-8.4.20230511084951/mypy-stubs/rdflib/collection.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/graph.pyi` & `schema-salad-8.4.20230511084951/mypy-stubs/rdflib/graph.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_CSVW.pyi` & `schema-salad-8.4.20230511084951/mypy-stubs/rdflib/namespace/_CSVW.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_DCAT.pyi` & `schema-salad-8.4.20230511084951/mypy-stubs/rdflib/namespace/_DCAT.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_DCTERMS.pyi` & `schema-salad-8.4.20230511084951/mypy-stubs/rdflib/namespace/_DCTERMS.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_DOAP.pyi` & `schema-salad-8.4.20230511084951/mypy-stubs/rdflib/namespace/_DOAP.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_FOAF.pyi` & `schema-salad-8.4.20230511084951/mypy-stubs/rdflib/namespace/_FOAF.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_ODRL2.pyi` & `schema-salad-8.4.20230511084951/mypy-stubs/rdflib/namespace/_ODRL2.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_ORG.pyi` & `schema-salad-8.4.20230511084951/mypy-stubs/rdflib/namespace/_ORG.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_OWL.pyi` & `schema-salad-8.4.20230511084951/mypy-stubs/rdflib/namespace/_OWL.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_PROV.pyi` & `schema-salad-8.4.20230511084951/mypy-stubs/rdflib/namespace/_PROV.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_QB.pyi` & `schema-salad-8.4.20230511084951/mypy-stubs/rdflib/namespace/_QB.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_RDF.pyi` & `schema-salad-8.4.20230511084951/mypy-stubs/rdflib/namespace/_RDF.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_RDFS.pyi` & `schema-salad-8.4.20230511084951/mypy-stubs/rdflib/namespace/_RDFS.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_SDO.pyi` & `schema-salad-8.4.20230511084951/mypy-stubs/rdflib/namespace/_SDO.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_SH.pyi` & `schema-salad-8.4.20230511084951/mypy-stubs/rdflib/namespace/_SH.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_SKOS.pyi` & `schema-salad-8.4.20230511084951/mypy-stubs/rdflib/namespace/_SKOS.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_SOSA.pyi` & `schema-salad-8.4.20230511084951/mypy-stubs/rdflib/namespace/_SOSA.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_SSN.pyi` & `schema-salad-8.4.20230511084951/mypy-stubs/rdflib/namespace/_SSN.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_TIME.pyi` & `schema-salad-8.4.20230511084951/mypy-stubs/rdflib/namespace/_TIME.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_VOID.pyi` & `schema-salad-8.4.20230511084951/mypy-stubs/rdflib/namespace/_VOID.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_XSD.pyi` & `schema-salad-8.4.20230511084951/mypy-stubs/rdflib/namespace/_XSD.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/__init__.pyi` & `schema-salad-8.4.20230511084951/mypy-stubs/rdflib/namespace/__init__.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/paths.pyi` & `schema-salad-8.4.20230511084951/mypy-stubs/rdflib/paths.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/plugin.pyi` & `schema-salad-8.4.20230511084951/mypy-stubs/rdflib/plugin.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/query.pyi` & `schema-salad-8.4.20230511084951/mypy-stubs/rdflib/query.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/resource.pyi` & `schema-salad-8.4.20230511084951/mypy-stubs/rdflib/resource.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/term.pyi` & `schema-salad-8.4.20230511084951/mypy-stubs/rdflib/term.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/pyproject.toml` & `schema-salad-8.4.20230511084951/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = [
     "setuptools>=45",
     "setuptools_scm[toml]>=6.2",
     'mypy==0.971; python_version == "3.6"',  # last version for Python 3.6
-    'mypy==1.0.0; python_version >= "3.7"',
+    'mypy==1.3.0; python_version >= "3.7"',  # update mypy-requirements as well
     "black>=19.10b0",
     "types-pkg_resources",
     "types-requests",
     "types-dataclasses",
     "ruamel.yaml>= 0.12.4, != 0.16.6, < 0.18",
     "types-setuptools"
 ]
```

### Comparing `schema-salad-8.4.20230426093816/release-test.sh` & `schema-salad-8.4.20230511084951/release-test.sh`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/avro/LICENSE` & `schema-salad-8.4.20230511084951/schema_salad/avro/LICENSE`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/avro/__init__.py` & `schema-salad-8.4.20230511084951/schema_salad/avro/__init__.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/avro/schema.py` & `schema-salad-8.4.20230511084951/schema_salad/avro/schema.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/codegen.py` & `schema-salad-8.4.20230511084951/schema_salad/codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/codegen_base.py` & `schema-salad-8.4.20230511084951/schema_salad/codegen_base.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/cpp_codegen.py` & `schema-salad-8.4.20230511084951/schema_salad/cpp_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/dlang_codegen.py` & `schema-salad-8.4.20230511084951/schema_salad/dlang_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/dotnet/LICENSE` & `schema-salad-8.4.20230511084951/schema_salad/dotnet/LICENSE`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/dotnet/Project.csproj.template` & `schema-salad-8.4.20230511084951/schema_salad/dotnet/Project.csproj.template`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/dotnet/Solution.sln` & `schema-salad-8.4.20230511084951/schema_salad/dotnet/Solution.sln`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/FetcherTests.cs` & `schema-salad-8.4.20230511084951/schema_salad/dotnet/Test/src/FetcherTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/UtilitiesTests.cs` & `schema-salad-8.4.20230511084951/schema_salad/dotnet/Test/src/UtilitiesTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/loaders/AnyLoaderTests.cs` & `schema-salad-8.4.20230511084951/schema_salad/dotnet/Test/src/loaders/AnyLoaderTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/loaders/ArrayLoaderTests.cs` & `schema-salad-8.4.20230511084951/schema_salad/dotnet/Test/src/loaders/ArrayLoaderTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/loaders/EnumLoaderTests.cs` & `schema-salad-8.4.20230511084951/schema_salad/dotnet/Test/src/loaders/EnumLoaderTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/loaders/ExpressionLoaderTests.cs` & `schema-salad-8.4.20230511084951/schema_salad/dotnet/Test/src/loaders/ExpressionLoaderTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/loaders/IdMapLoaderTests.cs` & `schema-salad-8.4.20230511084951/schema_salad/dotnet/Test/src/loaders/IdMapLoaderTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/loaders/NullLoaderTests.cs` & `schema-salad-8.4.20230511084951/schema_salad/dotnet/Test/src/loaders/NullLoaderTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderDoubleTests.cs` & `schema-salad-8.4.20230511084951/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderDoubleTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderFloatTests.cs` & `schema-salad-8.4.20230511084951/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderFloatTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderIntTests.cs` & `schema-salad-8.4.20230511084951/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderIntTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderStringTests.cs` & `schema-salad-8.4.20230511084951/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderStringTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/loaders/UnionLoaderTests.cs` & `schema-salad-8.4.20230511084951/schema_salad/dotnet/Test/src/loaders/UnionLoaderTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/dotnet/Test.csproj.template` & `schema-salad-8.4.20230511084951/schema_salad/dotnet/Test.csproj.template`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/dotnet/docfx.json` & `schema-salad-8.4.20230511084951/schema_salad/dotnet/docfx.json`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/dotnet/editorconfig` & `schema-salad-8.4.20230511084951/schema_salad/dotnet/editorconfig`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/dotnet/gitignore` & `schema-salad-8.4.20230511084951/schema_salad/dotnet/gitignore`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Fetcher.cs` & `schema-salad-8.4.20230511084951/schema_salad/dotnet/util/Fetcher.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/ArrayLoader.cs` & `schema-salad-8.4.20230511084951/schema_salad/dotnet/util/Loaders/ArrayLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/EnumLoader.cs` & `schema-salad-8.4.20230511084951/schema_salad/dotnet/util/Loaders/EnumLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/ExpressionLoader.cs` & `schema-salad-8.4.20230511084951/schema_salad/dotnet/util/Loaders/ExpressionLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/IdMapLoader.cs` & `schema-salad-8.4.20230511084951/schema_salad/dotnet/util/Loaders/IdMapLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/Loader.cs` & `schema-salad-8.4.20230511084951/schema_salad/dotnet/util/Loaders/Loader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/PrimitiveLoader.cs` & `schema-salad-8.4.20230511084951/schema_salad/dotnet/util/Loaders/PrimitiveLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/RecordLoader.cs` & `schema-salad-8.4.20230511084951/schema_salad/dotnet/util/Loaders/RecordLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/RootLoader.cs` & `schema-salad-8.4.20230511084951/schema_salad/dotnet/util/Loaders/RootLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/SecondaryDSLLoader.cs` & `schema-salad-8.4.20230511084951/schema_salad/dotnet/util/Loaders/SecondaryDSLLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/TypeDSLLoader.cs` & `schema-salad-8.4.20230511084951/schema_salad/dotnet/util/Loaders/TypeDSLLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/UnionLoader.cs` & `schema-salad-8.4.20230511084951/schema_salad/dotnet/util/Loaders/UnionLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/UriLoader.cs` & `schema-salad-8.4.20230511084951/schema_salad/dotnet/util/Loaders/UriLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/dotnet/util/LoadingOptions.cs` & `schema-salad-8.4.20230511084951/schema_salad/dotnet/util/LoadingOptions.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Saveable.cs` & `schema-salad-8.4.20230511084951/schema_salad/dotnet/util/Saveable.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/dotnet/util/ScalarNodeTypeResolver.cs` & `schema-salad-8.4.20230511084951/schema_salad/dotnet/util/ScalarNodeTypeResolver.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Utilities.cs` & `schema-salad-8.4.20230511084951/schema_salad/dotnet/util/Utilities.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/dotnet/util/ValidationException.cs` & `schema-salad-8.4.20230511084951/schema_salad/dotnet/util/ValidationException.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/dotnet_codegen.py` & `schema-salad-8.4.20230511084951/schema_salad/dotnet_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/exceptions.py` & `schema-salad-8.4.20230511084951/schema_salad/exceptions.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/fetcher.py` & `schema-salad-8.4.20230511084951/schema_salad/fetcher.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/java/README.md` & `schema-salad-8.4.20230511084951/schema_salad/java/README.md`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/java/main_utils/ArrayLoader.java` & `schema-salad-8.4.20230511084951/schema_salad/java/main_utils/ArrayLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/java/main_utils/DefaultFetcher.java` & `schema-salad-8.4.20230511084951/schema_salad/java/main_utils/DefaultFetcher.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/java/main_utils/EnumLoader.java` & `schema-salad-8.4.20230511084951/schema_salad/java/main_utils/EnumLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/java/main_utils/IdMapLoader.java` & `schema-salad-8.4.20230511084951/schema_salad/java/main_utils/IdMapLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/java/main_utils/Loader.java` & `schema-salad-8.4.20230511084951/schema_salad/java/main_utils/Loader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/java/main_utils/LoadingOptions.java` & `schema-salad-8.4.20230511084951/schema_salad/java/main_utils/LoadingOptions.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/java/main_utils/LoadingOptionsBuilder.java` & `schema-salad-8.4.20230511084951/schema_salad/java/main_utils/LoadingOptionsBuilder.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/java/main_utils/OneOrListOf.java` & `schema-salad-8.4.20230511084951/schema_salad/java/main_utils/OneOrListOf.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/java/main_utils/OneOrListOfLoader.java` & `schema-salad-8.4.20230511084951/schema_salad/java/main_utils/OneOrListOfLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/java/main_utils/OptionalLoader.java` & `schema-salad-8.4.20230511084951/schema_salad/java/main_utils/OptionalLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/java/main_utils/RecordLoader.java` & `schema-salad-8.4.20230511084951/schema_salad/java/main_utils/RecordLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/java/main_utils/RootLoader.java` & `schema-salad-8.4.20230511084951/schema_salad/java/main_utils/RootLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/java/main_utils/SecondaryFilesDslLoader.java` & `schema-salad-8.4.20230511084951/schema_salad/java/main_utils/SecondaryFilesDslLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/java/main_utils/TypeDslLoader.java` & `schema-salad-8.4.20230511084951/schema_salad/java/main_utils/TypeDslLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/java/main_utils/UnionLoader.java` & `schema-salad-8.4.20230511084951/schema_salad/java/main_utils/UnionLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/java/main_utils/UriLoader.java` & `schema-salad-8.4.20230511084951/schema_salad/java/main_utils/UriLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/java/main_utils/Uris.java` & `schema-salad-8.4.20230511084951/schema_salad/java/main_utils/Uris.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/java/main_utils/ValidationException.java` & `schema-salad-8.4.20230511084951/schema_salad/java/main_utils/ValidationException.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/java/main_utils/Validator.java` & `schema-salad-8.4.20230511084951/schema_salad/java/main_utils/Validator.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/java/main_utils/YamlUtils.java` & `schema-salad-8.4.20230511084951/schema_salad/java/main_utils/YamlUtils.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/java/pom.xml` & `schema-salad-8.4.20230511084951/schema_salad/java/pom.xml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/java/test_utils/DefaultFetcherTest.java` & `schema-salad-8.4.20230511084951/schema_salad/java/test_utils/DefaultFetcherTest.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/java/test_utils/ShortnameTest.java` & `schema-salad-8.4.20230511084951/schema_salad/java/test_utils/ShortnameTest.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/java_codegen.py` & `schema-salad-8.4.20230511084951/schema_salad/java_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/jsonld_context.py` & `schema-salad-8.4.20230511084951/schema_salad/jsonld_context.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/main.py` & `schema-salad-8.4.20230511084951/schema_salad/main.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/makedoc.py` & `schema-salad-8.4.20230511084951/schema_salad/makedoc.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/metaschema/field_name.yml` & `schema-salad-8.4.20230511084951/schema_salad/metaschema/field_name.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/metaschema/ident_res.yml` & `schema-salad-8.4.20230511084951/schema_salad/metaschema/ident_res.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/metaschema/import_include.md` & `schema-salad-8.4.20230511084951/schema_salad/metaschema/import_include.md`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/metaschema/link_res.yml` & `schema-salad-8.4.20230511084951/schema_salad/metaschema/link_res.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/metaschema/map_res.yml` & `schema-salad-8.4.20230511084951/schema_salad/metaschema/map_res.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/metaschema/map_res_schema.yml` & `schema-salad-8.4.20230511084951/schema_salad/metaschema/map_res_schema.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/metaschema/metaschema.yml` & `schema-salad-8.4.20230511084951/schema_salad/metaschema/metaschema.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/metaschema/metaschema_base.yml` & `schema-salad-8.4.20230511084951/schema_salad/metaschema/metaschema_base.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/metaschema/salad.md` & `schema-salad-8.4.20230511084951/schema_salad/metaschema/salad.md`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 data interpretation of the content, enables generation of JSON-LD context
 and RDF schema, and production of RDF triples by applying the JSON-LD
 context.  The schema language also provides for robust support of inline
 documentation.
 
 ## Introduction to v1.1
 
-This is the third version of of the Schema Salad specification.  It is
+This is the third version of the Schema Salad specification.  It is
 developed concurrently with v1.1 of the Common Workflow Language for use in
 specifying the Common Workflow Language, however Schema Salad is intended to be
 useful to a broader audience.  Compared to the v1.0 schema salad
 specification, the following changes have been made:
 
 * Support for `default` values on record fields to specify default values
 * Add subscoped fields (fields which introduce a new inner scope for identifiers)
@@ -117,15 +117,15 @@
 a specific implementation of Salad, however it may serve as a reference for
 the behavior of conforming implementations.
 
 ## Terminology
 
 The terminology used to describe Salad documents is defined in the Concepts
 section of the specification. The terms defined in the following list are
-used in building those definitions and in describing the actions of an
+used in building those definitions and in describing the actions of a
 Salad implementation:
 
 **may**: Conforming Salad documents and Salad implementations are permitted but
 not required to be interpreted as described.
 
 **must**: Conforming Salad documents and Salad implementations are required
 to be interpreted as described; otherwise they are in error.
@@ -264,22 +264,22 @@
 
   * If the value of `jsonldPredicate` is an object which contains the
   field `_type` with the value `@vocab`, the field value is subject to
   [vocabulary resolution](#Vocabulary_resolution).
 
 ## Document traversal
 
-To perform document document preprocessing, link validation and schema
+To perform document preprocessing, link validation and schema
 validation, the document must be traversed starting from the fields or
 array items of the root object or array and recursively visiting each child
 item which contains an object or arrays.
 
 ## Short names
 
-The "short name" of an fully qualified identifier is the portion of
+The "short name" of a fully qualified identifier is the portion of
 the identifier following the final slash `/` of either the fragment
 identifier following `#` or the path portion, if there is no fragment.
 Some examples:
 
 * the short name of `http://example.com/foo` is `foo`
 * the short name of `http://example.com/#bar` is `bar`
 * the short name of `http://example.com/foo/bar` is `bar`
```

### Comparing `schema-salad-8.4.20230426093816/schema_salad/metaschema/sfdsl_res.yml` & `schema-salad-8.4.20230511084951/schema_salad/metaschema/sfdsl_res.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/metaschema/typedsl_res.yml` & `schema-salad-8.4.20230511084951/schema_salad/metaschema/typedsl_res.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/metaschema/vocab_res.yml` & `schema-salad-8.4.20230511084951/schema_salad/metaschema/vocab_res.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/metaschema.py` & `schema-salad-8.4.20230511084951/schema_salad/metaschema.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/python_codegen.py` & `schema-salad-8.4.20230511084951/schema_salad/python_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/python_codegen_support.py` & `schema-salad-8.4.20230511084951/schema_salad/python_codegen_support.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/ref_resolver.py` & `schema-salad-8.4.20230511084951/schema_salad/ref_resolver.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import copy
 import logging
 import os
 import pathlib
 import re
 import tempfile
+import traceback
 import urllib
 import xml.sax  # nosec
 from io import StringIO
 from typing import (
     Any,
     Callable,
     Dict,
@@ -286,15 +287,17 @@
         for sch in aslist(ns):
             fetchurl = self.fetcher.urljoin(base_url, sch)
             if fetchurl not in self.cache or self.cache[fetchurl] is True:
                 _logger.debug("Getting external schema %s", fetchurl)
                 try:
                     content = self.fetch_text(fetchurl)
                 except Exception as e:
+                    tb = traceback.format_exception(type(e), e, e.__traceback__)
                     _logger.warning("Could not load extension schema %s: %s", fetchurl, str(e))
+                    _logger.debug(tb)
                     continue
                 newGraph = Graph()
                 err_msg = "unknown error"
                 for fmt in [
                     guess_format(sch),
                     "xml",
                     "turtle",
```

### Comparing `schema-salad-8.4.20230426093816/schema_salad/schema.py` & `schema-salad-8.4.20230511084951/schema_salad/schema.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/sourceline.py` & `schema-salad-8.4.20230511084951/schema_salad/sourceline.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/tests/EDAM.owl` & `schema-salad-8.4.20230511084951/schema_salad/tests/EDAM.owl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/tests/Process.yml` & `schema-salad-8.4.20230511084951/schema_salad/tests/Process.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/tests/basket_schema.yml` & `schema-salad-8.4.20230511084951/schema_salad/tests/basket_schema.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/tests/class_field_test.yml` & `schema-salad-8.4.20230511084951/schema_salad/tests/class_field_test.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/tests/cwl-pre.yml` & `schema-salad-8.4.20230511084951/schema_salad/tests/cwl-pre.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/tests/inherited-attributes.yml` & `schema-salad-8.4.20230511084951/schema_salad/tests/inherited-attributes.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/tests/matcher.py` & `schema-salad-8.4.20230511084951/schema_salad/tests/matcher.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/tests/metaschema-pre.yml` & `schema-salad-8.4.20230511084951/schema_salad/tests/metaschema-pre.yml`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996794871794872%*

 * *Differences: {'0': "{'doc': {insert: [(0, '# Semantic Annotations for Linked Avro Data "*

 * *      '(SALAD)\\n\\nAuthor:\\n\\n* Peter Amstutz <peter.amstutz@curii.com>, Curii '*

 * *      'Corporation\\n\\nContributors:\\n\\n* The developers of Apache Avro\\n* The developers of '*

 * *      'JSON-LD\\n* Nebojša Tijanić <nebojsa.tijanic@sbgenomics.com>, Seven Bridges Genomics\\n* '*

 * *      'Michael R. Crusoe, ELIXIR-DE\\n\\n# Abstract\\n\\nSalad is a schema language for describing '*

 * *      'structured linked data documents\\nin JSON or Y […]*

```diff
@@ -1,11 +1,11 @@
 [
     {
         "doc": [
-            "# Semantic Annotations for Linked Avro Data (SALAD)\n\nAuthor:\n\n* Peter Amstutz <peter.amstutz@curii.com>, Curii Corporation\n\nContributors:\n\n* The developers of Apache Avro\n* The developers of JSON-LD\n* Neboj\u0161a Tijani\u0107 <nebojsa.tijanic@sbgenomics.com>, Seven Bridges Genomics\n* Michael R. Crusoe, ELIXIR-DE\n\n# Abstract\n\nSalad is a schema language for describing structured linked data documents\nin JSON or YAML documents.  A Salad schema provides rules for\npreprocessing, structural validation, and link checking for documents\ndescribed by a Salad schema.  Salad builds on JSON-LD and the Apache Avro\ndata serialization system, and extends Avro with features for rich data\nmodeling such as inheritance, template specialization, object identifiers,\nand object references.  Salad was developed to provide a bridge between the\nrecord oriented data modeling supported by Apache Avro and the Semantic\nWeb.\n\n# Status of This Document\n\nThis document is the product of the [Common Workflow Language working\ngroup](https://groups.google.com/forum/#!forum/common-workflow-language).  The\nlatest version of this document is available in the \"schema_salad\" repository at\n\nhttps://github.com/common-workflow-language/schema_salad\n\nThe products of the CWL working group (including this document) are made available\nunder the terms of the Apache License, version 2.0.\n\n<!--ToC-->\n\n# Introduction\n\nThe JSON data model is an extremely popular way to represent structured\ndata.  It is attractive because of its relative simplicity and is a\nnatural fit with the standard types of many programming languages.\nHowever, this simplicity means that basic JSON lacks expressive features\nuseful for working with complex data structures and document formats, such\nas schemas, object references, and namespaces.\n\nJSON-LD is a W3C standard providing a way to describe how to interpret a\nJSON document as Linked Data by means of a \"context\".  JSON-LD provides a\npowerful solution for representing object references and namespaces in JSON\nbased on standard web URIs, but is not itself a schema language.  Without a\nschema providing a well defined structure, it is difficult to process an\narbitrary JSON-LD document as idiomatic JSON because there are many ways to\nexpress the same data that are logically equivalent but structurally\ndistinct.\n\nSeveral schema languages exist for describing and validating JSON data,\nsuch as the Apache Avro data serialization system, however none understand\nlinked data.  As a result, to fully take advantage of JSON-LD to build the\nnext generation of linked data applications, one must maintain separate\nJSON schema, JSON-LD context, RDF schema, and human documentation, despite\nsignificant overlap of content and obvious need for these documents to stay\nsynchronized.\n\nSchema Salad is designed to address this gap.  It provides a schema\nlanguage and processing rules for describing structured JSON content\npermitting URI resolution and strict document validation.  The schema\nlanguage supports linked data through annotations that describe the linked\ndata interpretation of the content, enables generation of JSON-LD context\nand RDF schema, and production of RDF triples by applying the JSON-LD\ncontext.  The schema language also provides for robust support of inline\ndocumentation.\n\n## Introduction to v1.1\n\nThis is the third version of of the Schema Salad specification.  It is\ndeveloped concurrently with v1.1 of the Common Workflow Language for use in\nspecifying the Common Workflow Language, however Schema Salad is intended to be\nuseful to a broader audience.  Compared to the v1.0 schema salad\nspecification, the following changes have been made:\n\n* Support for `default` values on record fields to specify default values\n* Add subscoped fields (fields which introduce a new inner scope for identifiers)\n* Add the *inVocab* flag (default true) to indicate if a type is added to the vocabulary of well known terms or must be prefixed\n* Add *secondaryFilesDSL* micro DSL (domain specific language) to convert text strings to a secondaryFiles record type used in CWL\n* The `$mixin` feature has been removed from the specification, as it\n  is poorly documented, not included in conformance testing,\n  and not widely supported.\n\n## Introduction to v1.2\n\nThis is the fourth version of the Schema Salad specification. It was created to\nease the development of extensions to CWL v1.2. The only change is that\ninherited records can narrow the types of fields if those fields are re-specified\nwith a matching jsonldPredicate.\n\n## References to Other Specifications\n\n**Javascript Object Notation (JSON)**: http://json.org\n\n**JSON Linked Data (JSON-LD)**: http://json-ld.org\n\n**YAML**: https://yaml.org/spec/1.2/spec.html\n\n**Avro**: https://avro.apache.org/docs/current/spec.html\n\n**Uniform Resource Identifier (URI) Generic Syntax**: https://tools.ietf.org/html/rfc3986)\n\n**Resource Description Framework (RDF)**: http://www.w3.org/RDF/\n\n**UTF-8**: https://www.ietf.org/rfc/rfc2279.txt)\n\n## Scope\n\nThis document describes the syntax, data model, algorithms, and schema\nlanguage for working with Salad documents.  It is not intended to document\na specific implementation of Salad, however it may serve as a reference for\nthe behavior of conforming implementations.\n\n## Terminology\n\nThe terminology used to describe Salad documents is defined in the Concepts\nsection of the specification. The terms defined in the following list are\nused in building those definitions and in describing the actions of an\nSalad implementation:\n\n**may**: Conforming Salad documents and Salad implementations are permitted but\nnot required to be interpreted as described.\n\n**must**: Conforming Salad documents and Salad implementations are required\nto be interpreted as described; otherwise they are in error.\n\n**error**: A violation of the rules of this specification; results are\nundefined. Conforming implementations may detect and report an error and may\nrecover from it.\n\n**fatal error**: A violation of the rules of this specification; results\nare undefined. Conforming implementations must not continue to process the\ndocument and may report an error.\n\n**at user option**: Conforming software may or must (depending on the modal verb in\nthe sentence) behave as described; if it does, it must provide users a means to\nenable or disable the behavior described.\n\n# Document model\n\n## Data concepts\n\nAn **object** is a data structure equivalent to the \"object\" type in JSON,\nconsisting of a unordered set of name/value pairs (referred to here as\n**fields**) and where the name is a string and the value is a string, number,\nboolean, array, or object.\n\nA **document** is a file containing a serialized object, or an array of\nobjects.\n\nA **document type** is a class of files that share a common structure and\nsemantics.\n\nA **document schema** is a formal description of the grammar of a document type.\n\nA **base URI** is a context-dependent URI used to resolve relative references.\n\nAn **identifier** is a URI that designates a single document or single\nobject within a document.\n\nA **vocabulary** is the set of symbolic field names and enumerated symbols defined\nby a document schema, where each term maps to absolute URI.\n\n## Syntax\n\nConforming Salad v1.1 documents are serialized and loaded using a\nsubset of YAML 1.2 syntax and UTF-8 text encoding.  Salad documents\nare written using the [JSON-compatible subset of YAML described in\nsection 10.2](https://yaml.org/spec/1.2/spec.html#id2803231).  The\nfollowing features of YAML must not be used in conforming Salad\ndocuments:\n\n* Use of explicit node tags with leading `!` or `!!`\n* Use of anchors with leading `&` and aliases with leading `*`\n* %YAML directives\n* %TAG directives\n\nIt is a fatal error if the document is not valid YAML.\n\nA Salad document must consist only of either a single root object or an\narray of objects.\n\n## Document context\n\n### Implied context\n\nThe implicit context consists of the vocabulary defined by the schema and\nthe base URI.  By default, the base URI must be the URI that was used to\nload the document.  It may be overridden by an explicit context.\n\n### Explicit context\n\nIf a document consists of a root object, this object may contain the\nfields `$base`, `$namespaces`, `$schemas`, and `$graph`:\n\n  * `$base`: Must be a string.  Set the base URI for the document used to\n    resolve relative references.\n\n  * `$namespaces`: Must be an object with strings as values.  The keys of\n    the object are namespace prefixes used in the document; the values of\n    the object are the prefix expansions.\n\n  * `$schemas`: Must be an array of strings.  This field may list URI\n    references to documents in RDF-XML format which will be queried for RDF\n    schema data.  The subjects and predicates described by the RDF schema\n    may provide additional semantic context for the document, and may be\n    used for validation of prefixed extension fields found in the document.\n\nOther directives beginning with `$` must be ignored.\n\n## Document graph\n\nIf a document consists of a single root object, this object may contain the\nfield `$graph`.  This field must be an array of objects.  If present, this\nfield holds the primary content of the document.  A document that consists\nof array of objects at the root is an implicit graph.\n\n## Document metadata\n\nIf a document consists of a single root object, metadata about the\ndocument, such as authorship, may be declared in the root object.\n\n## Document schema\n\nDocument preprocessing, link validation and schema validation require a\ndocument schema.  A schema may consist of:\n\n  * At least one record definition object which defines valid fields that\n  make up a record type.  Record field definitions include the valid types\n  that may be assigned to each field and annotations to indicate fields\n  that represent identifiers and links, described below in \"Semantic\n  Annotations\".\n\n  * Any number of enumerated type objects which define a set of finite set of symbols that are\n  valid value of the type.\n\n  * Any number of documentation objects which allow in-line documentation of the schema.\n\nThe schema for defining a salad schema (the metaschema) is described in\ndetail in the [Schema](#Schema) section.\n\n## Record field annotations\n\nIn a document schema, record field definitions may include the field\n`jsonldPredicate`, which may be either a string or object.  Implementations\nmust use the following document preprocessing of fields by the following\nrules:\n\n  * If the value of `jsonldPredicate` is `@id`, the field is an identifier\n  field.\n\n  * If the value of `jsonldPredicate` is an object, and that\n  object contains the field `_type` with the value `@id`, the\n  field is a link field.  If the field `jsonldPredicate` also\n  has the field `identity` with the value `true`, the field is\n  resolved with [identifier resolution](#Identifier_resolution).\n  Otherwise it is resolved with [link resolution](#Link_resolution).\n\n  * If the value of `jsonldPredicate` is an object which contains the\n  field `_type` with the value `@vocab`, the field value is subject to\n  [vocabulary resolution](#Vocabulary_resolution).\n\n## Document traversal\n\nTo perform document document preprocessing, link validation and schema\nvalidation, the document must be traversed starting from the fields or\narray items of the root object or array and recursively visiting each child\nitem which contains an object or arrays.\n\n## Short names\n\nThe \"short name\" of an fully qualified identifier is the portion of\nthe identifier following the final slash `/` of either the fragment\nidentifier following `#` or the path portion, if there is no fragment.\nSome examples:\n\n* the short name of `http://example.com/foo` is `foo`\n* the short name of `http://example.com/#bar` is `bar`\n* the short name of `http://example.com/foo/bar` is `bar`\n* the short name of `http://example.com/foo#bar` is `bar`\n* the short name of `http://example.com/#foo/bar` is `bar`\n* the short name of `http://example.com/foo#bar/baz` is `baz`\n\n## Inheritance and specialization\n\nA record definition may inherit from one or more record definitions\nwith the `extends` field.  This copies the fields defined in the\nparent record(s) as the base for the new record.  A record definition\nmay `specialize` type declarations of the fields inherited from the\nbase record.  For each field inherited from the base record, any\ninstance of the type in `specializeFrom` is replaced with the type in\n`specializeTo`.  The type in `specializeTo` should extend from the\ntype in `specializeFrom`.\n\nA record definition may be `abstract`.  This means the record\ndefinition is not used for validation on its own, but may be extended\nby other definitions.  If an abstract type appears in a field\ndefinition, it is logically replaced with a union of all concrete\nsubtypes of the abstract type.  In other words, the field value does\nnot validate as the abstract type, but must validate as some concrete\ntype that inherits from the abstract type.\n\n# Document preprocessing\n\nAfter processing the explicit context (if any), document preprocessing\nbegins.  Starting from the document root, object fields values or array\nitems which contain objects or arrays are recursively traversed\ndepth-first.  For each visited object, field names, identifier fields, link\nfields, vocabulary fields, and `$import` and `$include` directives must be\nprocessed as described in this section.  The order of traversal of child\nnodes within a parent node is undefined.\n",
+            "# Semantic Annotations for Linked Avro Data (SALAD)\n\nAuthor:\n\n* Peter Amstutz <peter.amstutz@curii.com>, Curii Corporation\n\nContributors:\n\n* The developers of Apache Avro\n* The developers of JSON-LD\n* Neboj\u0161a Tijani\u0107 <nebojsa.tijanic@sbgenomics.com>, Seven Bridges Genomics\n* Michael R. Crusoe, ELIXIR-DE\n\n# Abstract\n\nSalad is a schema language for describing structured linked data documents\nin JSON or YAML documents.  A Salad schema provides rules for\npreprocessing, structural validation, and link checking for documents\ndescribed by a Salad schema.  Salad builds on JSON-LD and the Apache Avro\ndata serialization system, and extends Avro with features for rich data\nmodeling such as inheritance, template specialization, object identifiers,\nand object references.  Salad was developed to provide a bridge between the\nrecord oriented data modeling supported by Apache Avro and the Semantic\nWeb.\n\n# Status of This Document\n\nThis document is the product of the [Common Workflow Language working\ngroup](https://groups.google.com/forum/#!forum/common-workflow-language).  The\nlatest version of this document is available in the \"schema_salad\" repository at\n\nhttps://github.com/common-workflow-language/schema_salad\n\nThe products of the CWL working group (including this document) are made available\nunder the terms of the Apache License, version 2.0.\n\n<!--ToC-->\n\n# Introduction\n\nThe JSON data model is an extremely popular way to represent structured\ndata.  It is attractive because of its relative simplicity and is a\nnatural fit with the standard types of many programming languages.\nHowever, this simplicity means that basic JSON lacks expressive features\nuseful for working with complex data structures and document formats, such\nas schemas, object references, and namespaces.\n\nJSON-LD is a W3C standard providing a way to describe how to interpret a\nJSON document as Linked Data by means of a \"context\".  JSON-LD provides a\npowerful solution for representing object references and namespaces in JSON\nbased on standard web URIs, but is not itself a schema language.  Without a\nschema providing a well defined structure, it is difficult to process an\narbitrary JSON-LD document as idiomatic JSON because there are many ways to\nexpress the same data that are logically equivalent but structurally\ndistinct.\n\nSeveral schema languages exist for describing and validating JSON data,\nsuch as the Apache Avro data serialization system, however none understand\nlinked data.  As a result, to fully take advantage of JSON-LD to build the\nnext generation of linked data applications, one must maintain separate\nJSON schema, JSON-LD context, RDF schema, and human documentation, despite\nsignificant overlap of content and obvious need for these documents to stay\nsynchronized.\n\nSchema Salad is designed to address this gap.  It provides a schema\nlanguage and processing rules for describing structured JSON content\npermitting URI resolution and strict document validation.  The schema\nlanguage supports linked data through annotations that describe the linked\ndata interpretation of the content, enables generation of JSON-LD context\nand RDF schema, and production of RDF triples by applying the JSON-LD\ncontext.  The schema language also provides for robust support of inline\ndocumentation.\n\n## Introduction to v1.1\n\nThis is the third version of the Schema Salad specification.  It is\ndeveloped concurrently with v1.1 of the Common Workflow Language for use in\nspecifying the Common Workflow Language, however Schema Salad is intended to be\nuseful to a broader audience.  Compared to the v1.0 schema salad\nspecification, the following changes have been made:\n\n* Support for `default` values on record fields to specify default values\n* Add subscoped fields (fields which introduce a new inner scope for identifiers)\n* Add the *inVocab* flag (default true) to indicate if a type is added to the vocabulary of well known terms or must be prefixed\n* Add *secondaryFilesDSL* micro DSL (domain specific language) to convert text strings to a secondaryFiles record type used in CWL\n* The `$mixin` feature has been removed from the specification, as it\n  is poorly documented, not included in conformance testing,\n  and not widely supported.\n\n## Introduction to v1.2\n\nThis is the fourth version of the Schema Salad specification. It was created to\nease the development of extensions to CWL v1.2. The only change is that\ninherited records can narrow the types of fields if those fields are re-specified\nwith a matching jsonldPredicate.\n\n## References to Other Specifications\n\n**Javascript Object Notation (JSON)**: http://json.org\n\n**JSON Linked Data (JSON-LD)**: http://json-ld.org\n\n**YAML**: https://yaml.org/spec/1.2/spec.html\n\n**Avro**: https://avro.apache.org/docs/current/spec.html\n\n**Uniform Resource Identifier (URI) Generic Syntax**: https://tools.ietf.org/html/rfc3986)\n\n**Resource Description Framework (RDF)**: http://www.w3.org/RDF/\n\n**UTF-8**: https://www.ietf.org/rfc/rfc2279.txt)\n\n## Scope\n\nThis document describes the syntax, data model, algorithms, and schema\nlanguage for working with Salad documents.  It is not intended to document\na specific implementation of Salad, however it may serve as a reference for\nthe behavior of conforming implementations.\n\n## Terminology\n\nThe terminology used to describe Salad documents is defined in the Concepts\nsection of the specification. The terms defined in the following list are\nused in building those definitions and in describing the actions of a\nSalad implementation:\n\n**may**: Conforming Salad documents and Salad implementations are permitted but\nnot required to be interpreted as described.\n\n**must**: Conforming Salad documents and Salad implementations are required\nto be interpreted as described; otherwise they are in error.\n\n**error**: A violation of the rules of this specification; results are\nundefined. Conforming implementations may detect and report an error and may\nrecover from it.\n\n**fatal error**: A violation of the rules of this specification; results\nare undefined. Conforming implementations must not continue to process the\ndocument and may report an error.\n\n**at user option**: Conforming software may or must (depending on the modal verb in\nthe sentence) behave as described; if it does, it must provide users a means to\nenable or disable the behavior described.\n\n# Document model\n\n## Data concepts\n\nAn **object** is a data structure equivalent to the \"object\" type in JSON,\nconsisting of a unordered set of name/value pairs (referred to here as\n**fields**) and where the name is a string and the value is a string, number,\nboolean, array, or object.\n\nA **document** is a file containing a serialized object, or an array of\nobjects.\n\nA **document type** is a class of files that share a common structure and\nsemantics.\n\nA **document schema** is a formal description of the grammar of a document type.\n\nA **base URI** is a context-dependent URI used to resolve relative references.\n\nAn **identifier** is a URI that designates a single document or single\nobject within a document.\n\nA **vocabulary** is the set of symbolic field names and enumerated symbols defined\nby a document schema, where each term maps to absolute URI.\n\n## Syntax\n\nConforming Salad v1.1 documents are serialized and loaded using a\nsubset of YAML 1.2 syntax and UTF-8 text encoding.  Salad documents\nare written using the [JSON-compatible subset of YAML described in\nsection 10.2](https://yaml.org/spec/1.2/spec.html#id2803231).  The\nfollowing features of YAML must not be used in conforming Salad\ndocuments:\n\n* Use of explicit node tags with leading `!` or `!!`\n* Use of anchors with leading `&` and aliases with leading `*`\n* %YAML directives\n* %TAG directives\n\nIt is a fatal error if the document is not valid YAML.\n\nA Salad document must consist only of either a single root object or an\narray of objects.\n\n## Document context\n\n### Implied context\n\nThe implicit context consists of the vocabulary defined by the schema and\nthe base URI.  By default, the base URI must be the URI that was used to\nload the document.  It may be overridden by an explicit context.\n\n### Explicit context\n\nIf a document consists of a root object, this object may contain the\nfields `$base`, `$namespaces`, `$schemas`, and `$graph`:\n\n  * `$base`: Must be a string.  Set the base URI for the document used to\n    resolve relative references.\n\n  * `$namespaces`: Must be an object with strings as values.  The keys of\n    the object are namespace prefixes used in the document; the values of\n    the object are the prefix expansions.\n\n  * `$schemas`: Must be an array of strings.  This field may list URI\n    references to documents in RDF-XML format which will be queried for RDF\n    schema data.  The subjects and predicates described by the RDF schema\n    may provide additional semantic context for the document, and may be\n    used for validation of prefixed extension fields found in the document.\n\nOther directives beginning with `$` must be ignored.\n\n## Document graph\n\nIf a document consists of a single root object, this object may contain the\nfield `$graph`.  This field must be an array of objects.  If present, this\nfield holds the primary content of the document.  A document that consists\nof array of objects at the root is an implicit graph.\n\n## Document metadata\n\nIf a document consists of a single root object, metadata about the\ndocument, such as authorship, may be declared in the root object.\n\n## Document schema\n\nDocument preprocessing, link validation and schema validation require a\ndocument schema.  A schema may consist of:\n\n  * At least one record definition object which defines valid fields that\n  make up a record type.  Record field definitions include the valid types\n  that may be assigned to each field and annotations to indicate fields\n  that represent identifiers and links, described below in \"Semantic\n  Annotations\".\n\n  * Any number of enumerated type objects which define a set of finite set of symbols that are\n  valid value of the type.\n\n  * Any number of documentation objects which allow in-line documentation of the schema.\n\nThe schema for defining a salad schema (the metaschema) is described in\ndetail in the [Schema](#Schema) section.\n\n## Record field annotations\n\nIn a document schema, record field definitions may include the field\n`jsonldPredicate`, which may be either a string or object.  Implementations\nmust use the following document preprocessing of fields by the following\nrules:\n\n  * If the value of `jsonldPredicate` is `@id`, the field is an identifier\n  field.\n\n  * If the value of `jsonldPredicate` is an object, and that\n  object contains the field `_type` with the value `@id`, the\n  field is a link field.  If the field `jsonldPredicate` also\n  has the field `identity` with the value `true`, the field is\n  resolved with [identifier resolution](#Identifier_resolution).\n  Otherwise it is resolved with [link resolution](#Link_resolution).\n\n  * If the value of `jsonldPredicate` is an object which contains the\n  field `_type` with the value `@vocab`, the field value is subject to\n  [vocabulary resolution](#Vocabulary_resolution).\n\n## Document traversal\n\nTo perform document preprocessing, link validation and schema\nvalidation, the document must be traversed starting from the fields or\narray items of the root object or array and recursively visiting each child\nitem which contains an object or arrays.\n\n## Short names\n\nThe \"short name\" of a fully qualified identifier is the portion of\nthe identifier following the final slash `/` of either the fragment\nidentifier following `#` or the path portion, if there is no fragment.\nSome examples:\n\n* the short name of `http://example.com/foo` is `foo`\n* the short name of `http://example.com/#bar` is `bar`\n* the short name of `http://example.com/foo/bar` is `bar`\n* the short name of `http://example.com/foo#bar` is `bar`\n* the short name of `http://example.com/#foo/bar` is `bar`\n* the short name of `http://example.com/foo#bar/baz` is `baz`\n\n## Inheritance and specialization\n\nA record definition may inherit from one or more record definitions\nwith the `extends` field.  This copies the fields defined in the\nparent record(s) as the base for the new record.  A record definition\nmay `specialize` type declarations of the fields inherited from the\nbase record.  For each field inherited from the base record, any\ninstance of the type in `specializeFrom` is replaced with the type in\n`specializeTo`.  The type in `specializeTo` should extend from the\ntype in `specializeFrom`.\n\nA record definition may be `abstract`.  This means the record\ndefinition is not used for validation on its own, but may be extended\nby other definitions.  If an abstract type appears in a field\ndefinition, it is logically replaced with a union of all concrete\nsubtypes of the abstract type.  In other words, the field value does\nnot validate as the abstract type, but must validate as some concrete\ntype that inherits from the abstract type.\n\n# Document preprocessing\n\nAfter processing the explicit context (if any), document preprocessing\nbegins.  Starting from the document root, object fields values or array\nitems which contain objects or arrays are recursively traversed\ndepth-first.  For each visited object, field names, identifier fields, link\nfields, vocabulary fields, and `$import` and `$include` directives must be\nprocessed as described in this section.  The order of traversal of child\nnodes within a parent node is undefined.\n",
             "## Field name resolution\n\nThe document schema declares the vocabulary of known field names.  During\npreprocessing traversal, field name in the document which are not part of\nthe schema vocabulary must be resolved to absolute URIs.  Under \"strict\"\nvalidation, it is an error for a document to include fields which are not\npart of the vocabulary and not resolvable to absolute URIs.  Fields names\nwhich are not part of the vocabulary are resolved using the following\nrules:\n\n* If a field name URI begins with a namespace prefix declared in the\ndocument context (`@context`) followed by a colon `:`, the prefix and\ncolon must be replaced by the namespace declared in `@context`.\n\n* If there is a vocabulary term which maps to the URI of a resolved\nfield, the field name must be replace with the vocabulary term.\n\n* If a field name URI is an absolute URI consisting of a scheme and path\nand is not part of the vocabulary, no processing occurs.\n\nField name resolution is not relative.  It must not be affected by the\nbase URI.\n\n### Field name resolution example\n\nGiven the following schema:\n\n```\n",
             "{\n  \"$namespaces\": {\n    \"acid\": \"http://example.com/acid#\"\n  },\n  \"$graph\": [{\n    \"name\": \"ExampleType\",\n    \"type\": \"record\",\n    \"documentRoot\": true,\n    \"fields\": [{\n      \"name\": \"base\",\n      \"type\": \"string\",\n      \"jsonldPredicate\": \"http://example.com/base\"\n    }]\n  }]\n}\n",
             "```\n\nProcess the following example:\n\n```\n",
             "    {\n      \"base\": \"one\",\n      \"form\": {\n        \"http://example.com/base\": \"two\",\n        \"http://example.com/three\": \"three\",\n      },\n      \"acid:four\": \"four\"\n    }\n",
             "```\n\nThis becomes:\n\n```\n",
             "    {\n      \"base\": \"one\",\n      \"form\": {\n        \"base\": \"two\",\n        \"http://example.com/three\": \"three\",\n      },\n      \"http://example.com/acid#four\": \"four\"\n    }\n",
             "```\n",
```

### Comparing `schema-salad-8.4.20230426093816/schema_salad/tests/pt.yml` & `schema-salad-8.4.20230511084951/schema_salad/tests/pt.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/tests/revtool_bad_schema.cwl` & `schema-salad-8.4.20230511084951/schema_salad/tests/revtool_bad_schema.cwl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/tests/test_avro_names.py` & `schema-salad-8.4.20230511084951/schema_salad/tests/test_avro_names.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/tests/test_cg.py` & `schema-salad-8.4.20230511084951/schema_salad/tests/test_cg.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/tests/test_cli_args.py` & `schema-salad-8.4.20230511084951/schema_salad/tests/test_cli_args.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/tests/test_cpp_codegen.py` & `schema-salad-8.4.20230511084951/schema_salad/tests/test_cpp_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/tests/test_cwl11.py` & `schema-salad-8.4.20230511084951/schema_salad/tests/test_cwl11.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/tests/test_dlang_codegen.py` & `schema-salad-8.4.20230511084951/schema_salad/tests/test_dlang_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/tests/test_dotnet_codegen.py` & `schema-salad-8.4.20230511084951/schema_salad/tests/test_dotnet_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/tests/test_errors.py` & `schema-salad-8.4.20230511084951/schema_salad/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/tests/test_examples.py` & `schema-salad-8.4.20230511084951/schema_salad/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/tests/test_fetch.py` & `schema-salad-8.4.20230511084951/schema_salad/tests/test_fetch.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/tests/test_fp.py` & `schema-salad-8.4.20230511084951/schema_salad/tests/test_fp.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/tests/test_java_codegen.py` & `schema-salad-8.4.20230511084951/schema_salad/tests/test_java_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/tests/test_makedoc.py` & `schema-salad-8.4.20230511084951/schema_salad/tests/test_makedoc.py`

 * *Files 4% similar despite different names*

```diff
@@ -235,9 +235,9 @@
     # 6. If the changes are agreeable, then update the hash below
     hasher = hashlib.sha256()
     hasher.update(metaschema_doc.encode("utf-8"))
     result = tmp_path / "result.html"
     with open(result, "w") as h:
         h.write(metaschema_doc)
     assert (
-        hasher.hexdigest() == "5fd520208b242c0fbf50235c83c88bc462f2b8d67b3dfbb9ffb399d7851fdab2"
+        hasher.hexdigest() == "4e67cb0a28829f9e14ecce93183fcf89fedb2446ae6cd717ccb2966609fe76a2"
     ), result
```

### Comparing `schema-salad-8.4.20230426093816/schema_salad/tests/test_misc.py` & `schema-salad-8.4.20230511084951/schema_salad/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/tests/test_pickling.py` & `schema-salad-8.4.20230511084951/schema_salad/tests/test_pickling.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/tests/test_print_oneline.py` & `schema-salad-8.4.20230511084951/schema_salad/tests/test_print_oneline.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/tests/test_python_codegen.py` & `schema-salad-8.4.20230511084951/schema_salad/tests/test_python_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/preprocess_util.js` & `schema-salad-8.4.20230511084951/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/preprocess_util.js`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/preprocess_vcf.cwl` & `schema-salad-8.4.20230511084951/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/preprocess_vcf.cwl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl/bio-cwl-tools/bamtools_stats.cwl` & `schema-salad-8.4.20230511084951/schema_salad/tests/test_real_cwl/bio-cwl-tools/bamtools_stats.cwl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl/bio-cwl-tools/bamtools_stats_invalid_schema_ref.cwl` & `schema-salad-8.4.20230511084951/schema_salad/tests/test_real_cwl/bio-cwl-tools/bamtools_stats_invalid_schema_ref.cwl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl/bio-cwl-tools/picard_CreateSequenceDictionary.cwl` & `schema-salad-8.4.20230511084951/schema_salad/tests/test_real_cwl/bio-cwl-tools/picard_CreateSequenceDictionary.cwl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl/h3agatk/GATK-Sub-Workflow-h3abionet-snp.cwl` & `schema-salad-8.4.20230511084951/schema_salad/tests/test_real_cwl/h3agatk/GATK-Sub-Workflow-h3abionet-snp.cwl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl/h3agatk/GATK-complete-WES-Workflow-h3abionet.cwl` & `schema-salad-8.4.20230511084951/schema_salad/tests/test_real_cwl/h3agatk/GATK-complete-WES-Workflow-h3abionet.cwl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl/tabs_rna_seq_workflow.cwl` & `schema-salad-8.4.20230511084951/schema_salad/tests/test_real_cwl/tabs_rna_seq_workflow.cwl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl/topmed/topmed_variant_calling_pipeline.cwl` & `schema-salad-8.4.20230511084951/schema_salad/tests/test_real_cwl/topmed/topmed_variant_calling_pipeline.cwl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl.py` & `schema-salad-8.4.20230511084951/schema_salad/tests/test_real_cwl.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/tests/test_ref_resolver.py` & `schema-salad-8.4.20230511084951/schema_salad/tests/test_ref_resolver.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/CommandLineTool.yml` & `schema-salad-8.4.20230511084951/schema_salad/tests/test_schema/CommandLineTool.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/Process.yml` & `schema-salad-8.4.20230511084951/schema_salad/tests/test_schema/Process.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/Workflow.yml` & `schema-salad-8.4.20230511084951/schema_salad/tests/test_schema/Workflow.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/avro_naming_base.yml` & `schema-salad-8.4.20230511084951/schema_salad/tests/test_schema/avro_naming_base.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/avro_subtype.yml` & `schema-salad-8.4.20230511084951/schema_salad/tests/test_schema/avro_subtype.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/avro_subtype_bad.yml` & `schema-salad-8.4.20230511084951/schema_salad/tests/test_schema/avro_subtype_bad.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/cwltest-schema.yml` & `schema-salad-8.4.20230511084951/schema_salad/tests/test_schema/cwltest-schema.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/metaschema_base.yml` & `schema-salad-8.4.20230511084951/schema_salad/tests/test_schema/metaschema_base.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/misc_schema_v1.yml` & `schema-salad-8.4.20230511084951/schema_salad/tests/test_schema/misc_schema_v1.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/misc_schema_v2.yml` & `schema-salad-8.4.20230511084951/schema_salad/tests/test_schema/misc_schema_v2.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/tests/test_schema.py` & `schema-salad-8.4.20230511084951/schema_salad/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/tests/test_schemas_directive.py` & `schema-salad-8.4.20230511084951/schema_salad/tests/test_schemas_directive.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/tests/test_subtypes.py` & `schema-salad-8.4.20230511084951/schema_salad/tests/test_subtypes.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/tests/test_typescript_codegen.py` & `schema-salad-8.4.20230511084951/schema_salad/tests/test_typescript_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/tests/util.py` & `schema-salad-8.4.20230511084951/schema_salad/tests/util.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/typescript/.gitignore` & `schema-salad-8.4.20230511084951/schema_salad/typescript/.gitignore`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/typescript/LICENSE` & `schema-salad-8.4.20230511084951/schema_salad/typescript/LICENSE`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/typescript/package.json` & `schema-salad-8.4.20230511084951/schema_salad/typescript/package.json`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/typescript/test/AnyLoader.spec.ts` & `schema-salad-8.4.20230511084951/schema_salad/typescript/test/AnyLoader.spec.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/typescript/test/Fetcher.spec.ts` & `schema-salad-8.4.20230511084951/schema_salad/typescript/test/Fetcher.spec.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/typescript/test/IdMap.spec.ts` & `schema-salad-8.4.20230511084951/schema_salad/typescript/test/IdMap.spec.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/typescript/test/Typeguards.spec.ts` & `schema-salad-8.4.20230511084951/schema_salad/typescript/test/Typeguards.spec.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/typescript/test/utilities.spec.ts` & `schema-salad-8.4.20230511084951/schema_salad/typescript/test/utilities.spec.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/typescript/tsconfig.json` & `schema-salad-8.4.20230511084951/schema_salad/typescript/tsconfig.json`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/typescript/util/Fetcher.ts` & `schema-salad-8.4.20230511084951/schema_salad/typescript/util/Fetcher.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/typescript/util/Internal.ts` & `schema-salad-8.4.20230511084951/schema_salad/typescript/util/Internal.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/typescript/util/LoadingOptions.ts` & `schema-salad-8.4.20230511084951/schema_salad/typescript/util/LoadingOptions.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/typescript/util/Saveable.ts` & `schema-salad-8.4.20230511084951/schema_salad/typescript/util/Saveable.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/typescript/util/Typeguards.ts` & `schema-salad-8.4.20230511084951/schema_salad/typescript/util/Typeguards.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/typescript/util/ValidationException.ts` & `schema-salad-8.4.20230511084951/schema_salad/typescript/util/ValidationException.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/typescript/util/loaders/ArrayLoader.ts` & `schema-salad-8.4.20230511084951/schema_salad/typescript/util/loaders/ArrayLoader.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/typescript/util/loaders/IdMapLoader.ts` & `schema-salad-8.4.20230511084951/schema_salad/typescript/util/loaders/IdMapLoader.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/typescript/util/loaders/Loader.ts` & `schema-salad-8.4.20230511084951/schema_salad/typescript/util/loaders/Loader.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/typescript/util/loaders/RecordLoader.ts` & `schema-salad-8.4.20230511084951/schema_salad/typescript/util/loaders/RecordLoader.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/typescript/util/loaders/RootLoader.ts` & `schema-salad-8.4.20230511084951/schema_salad/typescript/util/loaders/RootLoader.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/typescript/util/loaders/SecondaryDSLLoader.ts` & `schema-salad-8.4.20230511084951/schema_salad/typescript/util/loaders/SecondaryDSLLoader.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/typescript/util/loaders/TypeDSLLoader.ts` & `schema-salad-8.4.20230511084951/schema_salad/typescript/util/loaders/TypeDSLLoader.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/typescript/util/loaders/UnionLoader.ts` & `schema-salad-8.4.20230511084951/schema_salad/typescript/util/loaders/UnionLoader.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/typescript/util/loaders/UriLoader.ts` & `schema-salad-8.4.20230511084951/schema_salad/typescript/util/loaders/UriLoader.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/typescript_codegen.py` & `schema-salad-8.4.20230511084951/schema_salad/typescript_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad/utils.py` & `schema-salad-8.4.20230511084951/schema_salad/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,14 +117,16 @@
 
 
 _RoundTripNoTimeStampConstructor.add_constructor(
     "tag:yaml.org,2002:timestamp",
     _RoundTripNoTimeStampConstructor.construct_yaml_timestamp,
 )
 
+# mypy: no-warn-unused-ignores
+
 
 def yaml_no_ts() -> YAML:
     """
     Get a YAML loader that won't parse timestamps into datetime objects.
 
     Such datetime objects can't be easily dumped into JSON.
     """
```

### Comparing `schema-salad-8.4.20230426093816/schema_salad/validate.py` & `schema-salad-8.4.20230511084951/schema_salad/validate.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad.Dockerfile` & `schema-salad-8.4.20230511084951/schema_salad.Dockerfile`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/schema_salad.egg-info/PKG-INFO` & `schema-salad-8.4.20230511084951/schema_salad.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schema-salad
-Version: 8.4.20230426093816
+Version: 8.4.20230511084951
 Summary: Schema Annotations for Linked Avro Data (SALAD)
 Home-page: https://github.com/common-workflow-language/schema_salad
 Download-URL: https://github.com/common-workflow-language/schema_salad/releases
 Author: Common workflow language working group
 Author-email: common-workflow-language@googlegroups.com
 License: Apache 2.0
 Classifier: Environment :: Console
```

### Comparing `schema-salad-8.4.20230426093816/schema_salad.egg-info/SOURCES.txt` & `schema-salad-8.4.20230511084951/schema_salad.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230426093816/setup.py` & `schema-salad-8.4.20230511084951/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -77,20 +77,21 @@
     opt_level = os.getenv("MYPYC_OPT_LEVEL", "3")
     ext_modules = mypycify(mypyc_targets, opt_level=opt_level, debug_level="0", verbose=True)
 else:
     ext_modules = []
 
 install_requires = [
     "requests >= 1.0",
-    "ruamel.yaml >= 0.17.6, < 0.17.22;python_version>='3.7'",
-    "ruamel.yaml >= 0.16.12, < 0.17.22",
+    "ruamel.yaml >= 0.17.6, < 0.17.27;python_version>='3.7'",
+    "ruamel.yaml >= 0.16.12, < 0.17.27",
     "rdflib >= 4.2.2, < 7.0.0",
     "rdflib-jsonld>=0.4.0, <= 0.6.1;python_version<='3.6'",
     "mistune>=2.0.3,<2.1",
     "CacheControl[filecache] >= 0.11.7, < 0.13",
+    "urllib3<2",  # until CacheControl fixes their incompatability
     "mypy_extensions",
 ]
 
 extras_require = {
     "docs": [
         "sphinx >= 2.2",
         "sphinx-rtd-theme",
```

### Comparing `schema-salad-8.4.20230426093816/tox.ini` & `schema-salad-8.4.20230511084951/tox.ini`

 * *Files identical despite different names*

